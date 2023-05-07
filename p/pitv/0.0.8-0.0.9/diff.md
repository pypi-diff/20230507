# Comparing `tmp/pitv-0.0.8.tar.gz` & `tmp/pitv-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pitv-0.0.8.tar", max compression
+gzip compressed data, was "pitv-0.0.9.tar", max compression
```

## Comparing `pitv-0.0.8.tar` & `pitv-0.0.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1081 2023-05-06 19:25:58.253937 pitv-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0      906 2023-05-07 20:32:11.521978 pitv-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1039 2023-05-07 20:32:11.521978 pitv-0.0.8/src/pitv/__init__.py
--rw-r--r--   0        0        0      641 2023-05-07 17:40:52.896913 pitv-0.0.8/src/pitv/pitv.py
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 pitv-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-06 19:25:58.253937 pitv-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0      906 2023-05-07 20:35:05.183008 pitv-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1038 2023-05-07 20:35:05.183008 pitv-0.0.9/src/pitv/__init__.py
+-rw-r--r--   0        0        0      641 2023-05-07 17:40:52.896913 pitv-0.0.9/src/pitv/pitv.py
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 pitv-0.0.9/PKG-INFO
```

### Comparing `pitv-0.0.8/LICENSE.txt` & `pitv-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pitv-0.0.8/pyproject.toml` & `pitv-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pitv"
-version = "0.0.8"
+version = "0.0.9"
 description = "Pictures in the vault"
 authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
 license = "MIT"
 homepage = "https://pictures.openknowit.com"
 repository = "https://github.com/JakobHolstDK/picturesinthevault.git"
 
 [tool.poetry.scripts]
```

### Comparing `pitv-0.0.8/src/pitv/__init__.py` & `pitv-0.0.9/src/pitv/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#from  pitv import pitv
+from  pitv import pitv
 import os
 import sys
 import redis
 import time
 import subprocess
 import json
 import argparse
```

### Comparing `pitv-0.0.8/src/pitv/pitv.py` & `pitv-0.0.9/src/pitv/pitv.py`

 * *Files identical despite different names*

### Comparing `pitv-0.0.8/PKG-INFO` & `pitv-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pitv
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pictures in the vault
 Home-page: https://pictures.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

