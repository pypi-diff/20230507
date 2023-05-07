# Comparing `tmp/s3_simple_compress-0.1.0.tar.gz` & `tmp/s3_simple_compress-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3_simple_compress-0.1.0.tar", max compression
+gzip compressed data, was "s3_simple_compress-0.1.1.tar", max compression
```

## Comparing `s3_simple_compress-0.1.0.tar` & `s3_simple_compress-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1082 2023-05-03 18:18:17.246996 s3_simple_compress-0.1.0/LICENSE
--rw-r--r--   0        0        0     2863 2023-05-06 07:52:41.204216 s3_simple_compress-0.1.0/README.md
--rw-r--r--   0        0        0     2102 2023-05-06 08:05:49.651481 s3_simple_compress-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-03 18:08:48.531909 s3_simple_compress-0.1.0/s3_compress/__init__.py
--rw-r--r--   0        0        0     7107 2023-05-06 05:21:53.244506 s3_simple_compress-0.1.0/s3_compress/zipping_s3.py
--rw-r--r--   0        0        0     4412 1970-01-01 00:00:00.000000 s3_simple_compress-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-03 18:18:17.246996 s3_simple_compress-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2877 2023-05-07 00:07:28.513312 s3_simple_compress-0.1.1/README.md
+-rw-r--r--   0        0        0     2102 2023-05-07 00:09:07.718470 s3_simple_compress-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-03 18:08:48.531909 s3_simple_compress-0.1.1/s3_compress/__init__.py
+-rw-r--r--   0        0        0     7107 2023-05-06 05:21:53.244506 s3_simple_compress-0.1.1/s3_compress/zipping_s3.py
+-rw-r--r--   0        0        0     4426 1970-01-01 00:00:00.000000 s3_simple_compress-0.1.1/PKG-INFO
```

### Comparing `s3_simple_compress-0.1.0/LICENSE` & `s3_simple_compress-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `s3_simple_compress-0.1.0/README.md` & `s3_simple_compress-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,21 @@
 
 Installation
 How to install the project
 
 For installation of the project's CLI, we recommend using poetry to install:
 
 ```console
-poetry add s3-compress
+poetry add s3-simple-compress
 ```
 
 Although this is only a recommendation! You can also install the project with your preferred package manager, such as pip:
 
 ```console
-pip install s3-compress
+pip install s3-simple-compress
 ```
 
 ---
 
 ## How to use the program
 
 To use the AWS S3 file compression (zip) program, follow the steps below:
```

### Comparing `s3_simple_compress-0.1.0/pyproject.toml` & `s3_simple_compress-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "s3-simple-compress"
-version = "0.1.0"
+version = "0.1.1"
 description = "Documentation for AWS S3 In-Memory File Compression (zip) Program "
 license = "MIT"
 authors = ["Bruno Mesquita <bruno.mesquita2707@gmail.com>"]
 readme = "README.md"
 packages = [{include = "s3_compress"}]
 classifiers = [
     "Intended Audience :: Information Technology",
```

### Comparing `s3_simple_compress-0.1.0/s3_compress/zipping_s3.py` & `s3_simple_compress-0.1.1/s3_compress/zipping_s3.py`

 * *Files identical despite different names*

### Comparing `s3_simple_compress-0.1.0/PKG-INFO` & `s3_simple_compress-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3-simple-compress
-Version: 0.1.0
+Version: 0.1.1
 Summary: Documentation for AWS S3 In-Memory File Compression (zip) Program 
 License: MIT
 Author: Bruno Mesquita
 Author-email: bruno.mesquita2707@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -74,21 +74,21 @@
 
 Installation
 How to install the project
 
 For installation of the project's CLI, we recommend using poetry to install:
 
 ```console
-poetry add s3-compress
+poetry add s3-simple-compress
 ```
 
 Although this is only a recommendation! You can also install the project with your preferred package manager, such as pip:
 
 ```console
-pip install s3-compress
+pip install s3-simple-compress
 ```
 
 ---
 
 ## How to use the program
 
 To use the AWS S3 file compression (zip) program, follow the steps below:
```

