# Comparing `tmp/uoy-assessment-uploader-0.1.0.tar.gz` & `tmp/uoy-assessment-uploader-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uoy-assessment-uploader-0.1.0.tar", last modified: Sun May  7 17:26:58 2023, max compression
+gzip compressed data, was "uoy-assessment-uploader-0.1.1.tar", last modified: Sun May  7 17:36:14 2023, max compression
```

## Comparing `uoy-assessment-uploader-0.1.0.tar` & `uoy-assessment-uploader-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,6 @@
--rw-r--r--   0        0        0     3093 2023-05-07 16:35:45.711271 uoy-assessment-uploader-0.1.0/.gitignore
--rw-r--r--   0        0        0    32422 2023-05-07 14:17:04.216222 uoy-assessment-uploader-0.1.0/LICENSE
--rw-r--r--   0        0        0      221 2023-05-07 16:56:25.426336 uoy-assessment-uploader-0.1.0/Pipfile
--rw-r--r--   0        0        0    14318 2023-05-07 16:57:40.683481 uoy-assessment-uploader-0.1.0/Pipfile.lock
--rw-r--r--   0        0        0      872 2023-05-07 17:25:29.018608 uoy-assessment-uploader-0.1.0/README.md
--rw-r--r--   0        0        0      664 2023-05-07 17:16:29.017603 uoy-assessment-uploader-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0     7429 2023-05-07 17:25:14.905104 uoy-assessment-uploader-0.1.0/uoy_assessment_uploader/__init__.py
--rw-r--r--   0        0        0       27 2023-05-07 14:15:07.954388 uoy-assessment-uploader-0.1.0/uoy_assessment_uploader/__main__.py
--rw-r--r--   0        0        0     1434 1970-01-01 00:00:00.000000 uoy-assessment-uploader-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    32422 2023-05-07 14:17:04.216222 uoy-assessment-uploader-0.1.1/LICENSE
+-rw-r--r--   0        0        0      872 2023-05-07 17:25:29.018608 uoy-assessment-uploader-0.1.1/README.md
+-rw-r--r--   0        0        0      741 2023-05-07 17:33:43.930544 uoy-assessment-uploader-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0     7429 2023-05-07 17:35:54.075104 uoy-assessment-uploader-0.1.1/uoy_assessment_uploader/__init__.py
+-rw-r--r--   0        0        0       27 2023-05-07 14:15:07.954388 uoy-assessment-uploader-0.1.1/uoy_assessment_uploader/__main__.py
+-rw-r--r--   0        0        0     1509 1970-01-01 00:00:00.000000 uoy-assessment-uploader-0.1.1/PKG-INFO
```

### Comparing `uoy-assessment-uploader-0.1.0/LICENSE` & `uoy-assessment-uploader-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uoy-assessment-uploader-0.1.0/README.md` & `uoy-assessment-uploader-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `uoy-assessment-uploader-0.1.0/pyproject.toml` & `uoy-assessment-uploader-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 license = {file = "LICENSE"}
 classifiers = [
     "Environment :: Console",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Natural Language :: English",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "selenium ~= 4.9.0",
+    "webdriver-manager ~= 3.8.6"
+]
 dynamic = ["version", "description"]
 
 [project.urls]
 Home = "https://github.com/joelsgp/uoy-assessment-uploader"
 
 [project.scripts]
 uoy-assessment-uploader = "uoy_assessment_uploader:main"
```

### Comparing `uoy-assessment-uploader-0.1.0/uoy_assessment_uploader/__init__.py` & `uoy-assessment-uploader-0.1.1/uoy_assessment_uploader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from selenium.webdriver.support.wait import WebDriverWait
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.core.utils import ChromeType
 
 # todo: re-implement with saml auth and requests, as alternative to selenium
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 # timeout for selenium waits, in seconds
 TIMEOUT = 10
 
 DEFAULT_ARG_FILE = "exam.zip"
 DEFAULT_ARG_COOKIE_FILE = ".cookies.json"
```

### Comparing `uoy-assessment-uploader-0.1.0/PKG-INFO` & `uoy-assessment-uploader-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: uoy-assessment-uploader
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tool for automating submitting assessments to the University of York Computer Science department.
 Author-email: jmcb <joelsgp@protonmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
+Requires-Dist: selenium ~= 4.9.0
+Requires-Dist: webdriver-manager ~= 3.8.6
 Project-URL: Home, https://github.com/joelsgp/uoy-assessment-uploader
 
 # uoy_assessment_uploader
 
 ## Install
 1. When you have python and pip ready, it's as easy as:
     ```shell
```

