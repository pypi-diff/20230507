# Comparing `tmp/cos_uploader-2.0.0a1.tar.gz` & `tmp/cos_uploader-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cos_uploader-2.0.0a1.tar", max compression
+gzip compressed data, was "cos_uploader-2.0.0a2.tar", max compression
```

## Comparing `cos_uploader-2.0.0a1.tar` & `cos_uploader-2.0.0a2.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0       15 2023-05-07 14:40:37.069441 cos_uploader-2.0.0a1/README.md
--rw-r--r--   0        0        0      631 2023-05-07 14:43:29.630252 cos_uploader-2.0.0a1/config.toml
--rw-r--r--   0        0        0     6768 2023-05-07 14:59:26.557401 cos_uploader-2.0.0a1/cos_uploader/__init__.py
--rw-r--r--   0        0        0      554 2023-05-07 15:01:36.652694 cos_uploader-2.0.0a1/pyproject.toml
--rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 cos_uploader-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0       15 2023-05-07 14:40:37.069441 cos_uploader-2.0.0a2/README.md
+-rw-r--r--   0        0        0     4259 2023-05-07 15:47:35.650972 cos_uploader-2.0.0a2/cos_uploader/__init__.py
+-rw-r--r--   0        0        0      716 2023-05-07 15:23:47.518741 cos_uploader-2.0.0a2/cos_uploader/common.py
+-rw-r--r--   0        0        0      631 2023-05-07 14:43:29.630252 cos_uploader-2.0.0a2/cos_uploader/config.toml
+-rw-r--r--   0        0        0     2052 2023-05-07 15:25:57.984080 cos_uploader-2.0.0a2/cos_uploader/history.py
+-rw-r--r--   0        0        0     1192 2023-05-07 15:48:09.394167 cos_uploader-2.0.0a2/cos_uploader/install.py
+-rw-r--r--   0        0        0      618 2023-05-07 15:48:13.584301 cos_uploader-2.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 cos_uploader-2.0.0a2/PKG-INFO
```

### Comparing `cos_uploader-2.0.0a1/config.toml` & `cos_uploader-2.0.0a2/cos_uploader/config.toml`

 * *Files identical despite different names*

### Comparing `cos_uploader-2.0.0a1/pyproject.toml` & `cos_uploader-2.0.0a2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "cos-uploader"
-version = "2.0.0-alpha.1"
+version = "2.0.0-alpha.2"
 description = "Upload files to Tencent COS"
 authors = ["Joseph Chris <joseph@josephcz.xyz>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "cos_uploader"}]
-include = ["LICENSE", "config.toml"]
+include = ["LICENSE", "cos_uploader/config.toml"]
 
 [tool.poetry.scripts]
 cos-uploader = "cos_uploader:main"
-cos-uploader-history = "cos_uploader:show_history"
+cos-uploader-history = "cos_uploader.history:main"
+cos-uploader-install = "cos_uploader.install:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 cos-python-sdk-v5 = "^1.9.24"
 toml = "^0.10.2"
 
 [build-system]
```

### Comparing `cos_uploader-2.0.0a1/PKG-INFO` & `cos_uploader-2.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cos-uploader
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: Upload files to Tencent COS
 License: MIT
 Author: Joseph Chris
 Author-email: joseph@josephcz.xyz
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

