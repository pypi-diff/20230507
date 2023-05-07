# Comparing `tmp/scraperhero-0.1.0.tar.gz` & `tmp/scraperhero-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scraperhero-0.1.0.tar", max compression
+gzip compressed data, was "scraperhero-0.2.0.tar", max compression
```

## Comparing `scraperhero-0.1.0.tar` & `scraperhero-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      637 2023-05-07 08:48:54.680646 scraperhero-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3477 2023-05-07 09:00:36.735173 scraperhero-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-07 04:49:39.666796 scraperhero-0.1.0/scraperhero/__init__.py
--rw-r--r--   0        0        0     1050 2023-05-07 05:16:29.159130 scraperhero-0.1.0/scraperhero/downloader.py
--rw-r--r--   0        0        0      508 2023-05-07 05:32:03.464564 scraperhero-0.1.0/scraperhero/file_utils.py
--rw-r--r--   0        0        0     2408 2023-05-07 05:47:05.253980 scraperhero-0.1.0/scraperhero/pdf_utils.py
--rw-r--r--   0        0        0     6441 2023-05-07 08:48:01.469986 scraperhero-0.1.0/scraperhero/scraperhero.py
--rw-r--r--   0        0        0     4021 1970-01-01 00:00:00.000000 scraperhero-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      658 2023-05-07 09:14:35.635581 scraperhero-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3477 2023-05-07 09:00:36.735173 scraperhero-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 04:49:39.666796 scraperhero-0.2.0/scraperhero/__init__.py
+-rw-r--r--   0        0        0     1050 2023-05-07 05:16:29.159130 scraperhero-0.2.0/scraperhero/downloader.py
+-rw-r--r--   0        0        0      508 2023-05-07 05:32:03.464564 scraperhero-0.2.0/scraperhero/file_utils.py
+-rw-r--r--   0        0        0     2408 2023-05-07 05:47:05.253980 scraperhero-0.2.0/scraperhero/pdf_utils.py
+-rw-r--r--   0        0        0     6441 2023-05-07 08:48:01.469986 scraperhero-0.2.0/scraperhero/scraperhero.py
+-rw-r--r--   0        0        0     4021 1970-01-01 00:00:00.000000 scraperhero-0.2.0/PKG-INFO
```

### Comparing `scraperhero-0.1.0/pyproject.toml` & `scraperhero-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "scraperhero"
-version = "0.1.0"
+version = "0.2.0"
 description = "A Python library for downloading PDF files from a webpage, with support for recursion depth and optional PDF merging."
 authors = ["Mark A. Lifson, Ph.D. <mlifson@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "scraperhero"}]
+exclude = ["tests/*"]
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 requests = "^2.30.0"
 pymupdf = "^1.22.2"
 bs4 = "^0.0.1"
 
@@ -17,8 +18,8 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 responses = "^0.23.1"
 coverage = "^7.2.5"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `scraperhero-0.1.0/README.md` & `scraperhero-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `scraperhero-0.1.0/scraperhero/downloader.py` & `scraperhero-0.2.0/scraperhero/downloader.py`

 * *Files identical despite different names*

### Comparing `scraperhero-0.1.0/scraperhero/pdf_utils.py` & `scraperhero-0.2.0/scraperhero/pdf_utils.py`

 * *Files identical despite different names*

### Comparing `scraperhero-0.1.0/scraperhero/scraperhero.py` & `scraperhero-0.2.0/scraperhero/scraperhero.py`

 * *Files identical despite different names*

### Comparing `scraperhero-0.1.0/PKG-INFO` & `scraperhero-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scraperhero
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python library for downloading PDF files from a webpage, with support for recursion depth and optional PDF merging.
 License: MIT
 Author: Mark A. Lifson, Ph.D.
 Author-email: mlifson@gmail.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scraperhero Version: 0.1.0 Summary: A Python
+Metadata-Version: 2.1 Name: scraperhero Version: 0.2.0 Summary: A Python
 library for downloading PDF files from a webpage, with support for recursion
 depth and optional PDF merging. License: MIT Author: Mark A. Lifson, Ph.D.
 Author-email: mlifson@gmail.com Requires-Python: >=3.10 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-Dist:
 pymupdf (>=1.22.2,<2.0.0) Requires-Dist: requests (>=2.30.0,<3.0.0)
```

