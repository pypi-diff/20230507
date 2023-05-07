# Comparing `tmp/uoy-assessment-uploader-0.2.0.tar.gz` & `tmp/uoy-assessment-uploader-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uoy-assessment-uploader-0.2.0.tar", last modified: Sun May  7 18:15:44 2023, max compression
+gzip compressed data, was "uoy-assessment-uploader-0.2.1.tar", last modified: Sun May  7 18:26:06 2023, max compression
```

## Comparing `uoy-assessment-uploader-0.2.0.tar` & `uoy-assessment-uploader-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    32422 2023-05-07 14:17:04.216222 uoy-assessment-uploader-0.2.0/LICENSE
--rw-r--r--   0        0        0      981 2023-05-07 17:40:29.840917 uoy-assessment-uploader-0.2.0/README.md
--rw-r--r--   0        0        0      741 2023-05-07 17:33:43.930544 uoy-assessment-uploader-0.2.0/pyproject.toml
--rwxr-xr-x   0        0        0     7960 2023-05-07 18:15:27.691661 uoy-assessment-uploader-0.2.0/uoy_assessment_uploader/__init__.py
--rw-r--r--   0        0        0       27 2023-05-07 14:15:07.954388 uoy-assessment-uploader-0.2.0/uoy_assessment_uploader/__main__.py
--rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 uoy-assessment-uploader-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    32422 2023-05-07 14:17:04.216222 uoy-assessment-uploader-0.2.1/LICENSE
+-rw-r--r--   0        0        0      981 2023-05-07 17:40:29.840917 uoy-assessment-uploader-0.2.1/README.md
+-rw-r--r--   0        0        0      741 2023-05-07 17:33:43.930544 uoy-assessment-uploader-0.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0     7895 2023-05-07 18:25:00.108017 uoy-assessment-uploader-0.2.1/uoy_assessment_uploader/__init__.py
+-rw-r--r--   0        0        0       27 2023-05-07 14:15:07.954388 uoy-assessment-uploader-0.2.1/uoy_assessment_uploader/__main__.py
+-rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 uoy-assessment-uploader-0.2.1/PKG-INFO
```

### Comparing `uoy-assessment-uploader-0.2.0/LICENSE` & `uoy-assessment-uploader-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uoy-assessment-uploader-0.2.0/README.md` & `uoy-assessment-uploader-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `uoy-assessment-uploader-0.2.0/pyproject.toml` & `uoy-assessment-uploader-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uoy-assessment-uploader-0.2.0/uoy_assessment_uploader/__init__.py` & `uoy-assessment-uploader-0.2.1/uoy_assessment_uploader/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.core.utils import ChromeType
 
 
 # todo: re-implement with saml auth and requests, as alternative to selenium
 
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 # timeout for selenium waits, in seconds
 TIMEOUT = 10
 
 DEFAULT_ARG_FILE = "exam.zip"
 DEFAULT_ARG_COOKIE_FILE = ".cookies.json"
 
@@ -56,15 +56,15 @@
         "--dry-run",
         action="store_true",
         help="Log in but don't actually upload the file.",
     )
     # selenium cookies
     parser.add_argument("--cookie-file", type=Path, default=DEFAULT_ARG_COOKIE_FILE)
     parser.add_argument(
-        "--no-save-cookies", dest="do_save_cookies", action="store_false"
+        "--no-save-cookies", dest="save_cookies", action="store_false"
     )
     parser.add_argument(
         "--delete-cookies",
         action="store_true",
         help="Before starting, delete previous login cookies (if they exist).",
     )
     # other selenium options
@@ -77,14 +77,28 @@
     parser.add_argument(
         "--chromium", action="store_true", help="Use Chromium instead of Google Chrome."
     )
 
     return parser
 
 
+class Args:
+    username: str
+    password: str
+    exam_number: str
+    submit_url: str
+    file: Path
+    dry_run: bool
+    cookie_file: Path
+    save_cookies: bool
+    delete_cookies: bool
+    headless: bool
+    chromium: bool
+
+
 def save_cookies(driver: WebDriver, fp: Path):
     cookies = driver.get_cookies()
     with open(fp, "w") as f:
         json.dump(cookies, f)
 
 
 def load_cookies(driver: webdriver.Chrome, fp: Path):
@@ -119,15 +133,17 @@
     input_file.send_keys(file_name)
     input_checkbox = driver.find_element(By.ID, "ownwork")
     input_checkbox.click()
     if not dry_run:
         input_checkbox.submit()
 
 
-def ensure_details(current: str, prompt: Optional[str] = None, hide: bool = False) -> str:
+def ensure_details(
+    current: str, prompt: Optional[str] = None, hide: bool = False
+) -> str:
     if current is not None:
         return current
 
     if hide:
         current = getpass.getpass()
     else:
         current = input(prompt)
@@ -147,24 +163,24 @@
 
     # breaks loop on submit
     while True:
         driver.get(submit_url)
         # username/password login page
         if driver.current_url == URL_LOGIN:
             print("Logging in..")
-            username = ensure_details(username, 'Enter username: ')
+            username = ensure_details(username, "Enter username: ")
             password = ensure_details(password, hide=True)
             login(driver, username, password)
             wait.until(
                 ec.any_of(ec.url_to_be(URL_EXAM_NUMBER), ec.url_to_be(submit_url))
             )
         # exam number login page
         elif driver.current_url == URL_EXAM_NUMBER:
             print("Entering exam number..")
-            exam_number = ensure_details(exam_number, 'Enter exam number: ')
+            exam_number = ensure_details(exam_number, "Enter exam number: ")
             enter_exam_number(driver, exam_number)
             wait.until(ec.url_to_be(submit_url))
         # logged in, upload page
         elif driver.current_url == submit_url:
             print("Uploading file...")
             upload(driver, file_name, dry_run)
             if dry_run:
@@ -187,73 +203,62 @@
     submit_url = f"{base}/{submit_url}"
     return submit_url
 
 
 def main():
     # load arguments
     parser = get_parser()
-    args = parser.parse_args()
-
-    username: str = args.username
-    password: str = args.password
-    exam_number: str = args.exam_number
-    submit_url: str = args.submit_url
-    fp: Path = args.file
-    dry_run: bool = args.dry_run
-    cookie_path: Path = args.cookie_file
-    do_save_cookies: bool = args.do_save_cookies
-    delete_cookies: bool = args.delete_cookies
-    headless: bool = args.headless
-    chromium: bool = args.chromium
+    args = Args()
+    parser.parse_args(namespace=args)
 
     # check zip to be uploaded exists
-    if not fp.is_file():
-        print(f"File doesn't exist '{fp}'.")
+    if not args.file.is_file():
+        print(f"File doesn't exist '{args.file}'.")
         sys.exit(1)
-    print(f"Found file '{fp}'.")
-    file_name = str(fp.resolve())
+    print(f"Found file '{args.file}'.")
+    file_name = str(args.file.resolve())
 
     # verify arguments
-    submit_url = resolve_submit_url(submit_url)
+    submit_url = resolve_submit_url(args.submit_url)
 
     # webdriver setup
     # options
     driver_options = webdriver.ChromeOptions()
-    if headless:
+    if args.headless:
         driver_options.add_argument("--headless")
 
     # auto installer
-    if chromium:
+    if args.chromium:
         chrome_type = ChromeType.CHROMIUM
     else:
         chrome_type = ChromeType.GOOGLE
     driver_path = ChromeDriverManager(chrome_type=chrome_type).install()
     driver_service = ChromeService(driver_path)
 
     with webdriver.Chrome(options=driver_options, service=driver_service) as driver:
         driver.implicitly_wait(TIMEOUT)
 
         # load cookies
-        if delete_cookies:
-            cookie_path.unlink(missing_ok=True)
-        elif do_save_cookies:
-            load_cookies(driver, cookie_path)
+        if args.delete_cookies:
+            args.cookie_file.unlink(missing_ok=True)
+        elif args.save_cookies:
+            load_cookies(driver, args.cookie_file)
 
         # run
         do(
             driver=driver,
             submit_url=submit_url,
-            username=username,
-            password=password,
-            exam_number=exam_number,
+            username=args.username,
+            password=args.password,
+            exam_number=args.exam_number,
             file_name=file_name,
-            dry_run=dry_run,
+            dry_run=args.dry_run,
         )
 
         # save cookies
-        if do_save_cookies:
+        if args.save_cookies:
             print("Saving cookies.")
-            save_cookies(driver, cookie_path)
+            save_cookies(driver, args.cookie_file)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `uoy-assessment-uploader-0.2.0/PKG-INFO` & `uoy-assessment-uploader-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uoy-assessment-uploader
-Version: 0.2.0
+Version: 0.2.1
 Summary: Tool for automating submitting assessments to the University of York Computer Science department.
 Author-email: jmcb <joelsgp@protonmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
```

