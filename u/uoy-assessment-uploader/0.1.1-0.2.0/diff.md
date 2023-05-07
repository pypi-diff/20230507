# Comparing `tmp/uoy-assessment-uploader-0.1.1.tar.gz` & `tmp/uoy-assessment-uploader-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uoy-assessment-uploader-0.1.1.tar", last modified: Sun May  7 17:36:14 2023, max compression
+gzip compressed data, was "uoy-assessment-uploader-0.2.0.tar", last modified: Sun May  7 18:15:44 2023, max compression
```

## Comparing `uoy-assessment-uploader-0.1.1.tar` & `uoy-assessment-uploader-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    32422 2023-05-07 14:17:04.216222 uoy-assessment-uploader-0.1.1/LICENSE
--rw-r--r--   0        0        0      872 2023-05-07 17:25:29.018608 uoy-assessment-uploader-0.1.1/README.md
--rw-r--r--   0        0        0      741 2023-05-07 17:33:43.930544 uoy-assessment-uploader-0.1.1/pyproject.toml
--rwxr-xr-x   0        0        0     7429 2023-05-07 17:35:54.075104 uoy-assessment-uploader-0.1.1/uoy_assessment_uploader/__init__.py
--rw-r--r--   0        0        0       27 2023-05-07 14:15:07.954388 uoy-assessment-uploader-0.1.1/uoy_assessment_uploader/__main__.py
--rw-r--r--   0        0        0     1509 1970-01-01 00:00:00.000000 uoy-assessment-uploader-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    32422 2023-05-07 14:17:04.216222 uoy-assessment-uploader-0.2.0/LICENSE
+-rw-r--r--   0        0        0      981 2023-05-07 17:40:29.840917 uoy-assessment-uploader-0.2.0/README.md
+-rw-r--r--   0        0        0      741 2023-05-07 17:33:43.930544 uoy-assessment-uploader-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0     7960 2023-05-07 18:15:27.691661 uoy-assessment-uploader-0.2.0/uoy_assessment_uploader/__init__.py
+-rw-r--r--   0        0        0       27 2023-05-07 14:15:07.954388 uoy-assessment-uploader-0.2.0/uoy_assessment_uploader/__main__.py
+-rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 uoy-assessment-uploader-0.2.0/PKG-INFO
```

### Comparing `uoy-assessment-uploader-0.1.1/LICENSE` & `uoy-assessment-uploader-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uoy-assessment-uploader-0.1.1/README.md` & `uoy-assessment-uploader-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # uoy_assessment_uploader
 
 ## Install
 1. When you have python and pip ready, it's as easy as:
-    ```shell
-    python -m pip install "git+https://github.com/joelsgp/uoy-assessment-uploader"
-    ```
+   ```shell
+   python -m pip install "uoy-assessment-uploader"
+   ```
+   - or, directly from the repo:
+      ```shell
+      python -m pip install "git+https://github.com/joelsgp/uoy-assessment-uploader"
+      ```
 2. You need the Chrome browser installed. Sorry!
     - I need a cookie management feature Firefox doesn't have.
     - If you have Chromium instead, pass the `--chromium` flag.
 
 ## Use
 Like this:
 - ```shell
```

### Comparing `uoy-assessment-uploader-0.1.1/pyproject.toml` & `uoy-assessment-uploader-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uoy-assessment-uploader-0.1.1/uoy_assessment_uploader/__init__.py` & `uoy-assessment-uploader-0.2.0/uoy_assessment_uploader/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """Tool for automating submitting assessments to the University of York Computer Science department."""
 
 import getpass
 import json
 import sys
 from argparse import ArgumentParser
 from pathlib import Path
+from typing import Optional
 
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service as ChromeService
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.support import expected_conditions as ec
 from selenium.webdriver.support.wait import WebDriverWait
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.core.utils import ChromeType
 
+
 # todo: re-implement with saml auth and requests, as alternative to selenium
 
 
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 
 # timeout for selenium waits, in seconds
 TIMEOUT = 10
 
 DEFAULT_ARG_FILE = "exam.zip"
 DEFAULT_ARG_COOKIE_FILE = ".cookies.json"
 
@@ -31,28 +33,28 @@
 URL_EXAM_NUMBER = "https://teaching.cs.york.ac.uk/student/confirm-exam-number"
 
 
 def get_parser() -> ArgumentParser:
     parser = ArgumentParser(description=__doc__)
 
     # core functionality arguments
-    parser.add_argument("-u", "--username", required=True)
-    parser.add_argument(
-        "--password",
-        help="Not recommended to pass this as an argument, for security reasons."
-        " Leave it out and you will be securely prompted to enter it at startup.",
-    )
-    parser.add_argument("-e", "--exam-number", required=True)
-    parser.add_argument("-f", "--file", type=Path, default=DEFAULT_ARG_FILE)
     parser.add_argument(
         "-n",
         "--submit-url",
         required=True,
         help="The specific exam to upload to, e.g. /2021-2/submit/COM00012C/901/A",
     )
+    parser.add_argument("-u", "--username")
+    parser.add_argument(
+        "--password",
+        help="Not recommended to pass this as an argument, for security reasons."
+        " Leave it out and you will be securely prompted to enter it at startup.",
+    )
+    parser.add_argument("-e", "--exam-number")
+    parser.add_argument("-f", "--file", type=Path, default=DEFAULT_ARG_FILE)
     # options
     parser.add_argument(
         "--dry-run",
         action="store_true",
         help="Log in but don't actually upload the file.",
     )
     # selenium cookies
@@ -117,38 +119,55 @@
     input_file.send_keys(file_name)
     input_checkbox = driver.find_element(By.ID, "ownwork")
     input_checkbox.click()
     if not dry_run:
         input_checkbox.submit()
 
 
+def ensure_details(current: str, prompt: Optional[str] = None, hide: bool = False) -> str:
+    if current is not None:
+        return current
+
+    if hide:
+        current = getpass.getpass()
+    else:
+        current = input(prompt)
+    return current
+
+
 def do(
     driver: WebDriver,
     submit_url: str,
-    username: str,
-    password: str,
-    exam_number: str,
+    username: Optional[str],
+    password: Optional[str],
+    exam_number: Optional[str],
     file_name: str,
     dry_run: bool,
 ):
     wait = WebDriverWait(driver, TIMEOUT)
 
     # breaks loop on submit
     while True:
         driver.get(submit_url)
+        # username/password login page
         if driver.current_url == URL_LOGIN:
             print("Logging in..")
+            username = ensure_details(username, 'Enter username: ')
+            password = ensure_details(password, hide=True)
             login(driver, username, password)
             wait.until(
                 ec.any_of(ec.url_to_be(URL_EXAM_NUMBER), ec.url_to_be(submit_url))
             )
+        # exam number login page
         elif driver.current_url == URL_EXAM_NUMBER:
             print("Entering exam number..")
+            exam_number = ensure_details(exam_number, 'Enter exam number: ')
             enter_exam_number(driver, exam_number)
             wait.until(ec.url_to_be(submit_url))
+        # logged in, upload page
         elif driver.current_url == submit_url:
             print("Uploading file...")
             upload(driver, file_name, dry_run)
             if dry_run:
                 print("Skipped actual upload.")
             else:
                 wait.until(
@@ -190,16 +209,14 @@
     if not fp.is_file():
         print(f"File doesn't exist '{fp}'.")
         sys.exit(1)
     print(f"Found file '{fp}'.")
     file_name = str(fp.resolve())
 
     # verify arguments
-    if password is None:
-        password = getpass.getpass()
     submit_url = resolve_submit_url(submit_url)
 
     # webdriver setup
     # options
     driver_options = webdriver.ChromeOptions()
     if headless:
         driver_options.add_argument("--headless")
```

### Comparing `uoy-assessment-uploader-0.1.1/PKG-INFO` & `uoy-assessment-uploader-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uoy-assessment-uploader
-Version: 0.1.1
+Version: 0.2.0
 Summary: Tool for automating submitting assessments to the University of York Computer Science department.
 Author-email: jmcb <joelsgp@protonmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
@@ -13,17 +13,21 @@
 Requires-Dist: webdriver-manager ~= 3.8.6
 Project-URL: Home, https://github.com/joelsgp/uoy-assessment-uploader
 
 # uoy_assessment_uploader
 
 ## Install
 1. When you have python and pip ready, it's as easy as:
-    ```shell
-    python -m pip install "git+https://github.com/joelsgp/uoy-assessment-uploader"
-    ```
+   ```shell
+   python -m pip install "uoy-assessment-uploader"
+   ```
+   - or, directly from the repo:
+      ```shell
+      python -m pip install "git+https://github.com/joelsgp/uoy-assessment-uploader"
+      ```
 2. You need the Chrome browser installed. Sorry!
     - I need a cookie management feature Firefox doesn't have.
     - If you have Chromium instead, pass the `--chromium` flag.
 
 ## Use
 Like this:
 - ```shell
```

