# Comparing `tmp/pitv-0.0.3.tar.gz` & `tmp/pitv-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pitv-0.0.3.tar", max compression
+gzip compressed data, was "pitv-0.0.5.tar", max compression
```

## Comparing `pitv-0.0.3.tar` & `pitv-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1081 2023-05-06 19:25:58.253937 pitv-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0      882 2023-05-06 20:32:21.318107 pitv-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1038 2023-05-06 19:25:58.253937 pitv-0.0.3/src/pitv/__init__.py
--rw-r--r--   0        0        0      553 2023-05-06 19:25:58.253937 pitv-0.0.3/src/pitv/pitv.py
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 pitv-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-06 19:25:58.253937 pitv-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      907 2023-05-07 17:51:36.940689 pitv-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1038 2023-05-06 19:25:58.253937 pitv-0.0.5/src/pitv/__init__.py
+-rw-r--r--   0        0        0      641 2023-05-07 17:40:52.896913 pitv-0.0.5/src/pitv/pitv.py
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 pitv-0.0.5/PKG-INFO
```

### Comparing `pitv-0.0.3/LICENSE.txt` & `pitv-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pitv-0.0.3/pyproject.toml` & `pitv-0.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "pitv"
-version = "0.0.3"
+version = "0.0.5"
 description = "Pictures in the vault"
 authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
 license = "MIT"
 homepage = "https://pictures.openknowit.com"
 repository = "https://github.com/JakobHolstDK/picturesinthevault.git"
 
 [tool.poetry.scripts]
 pitv = "pitv:main"
+pitvapi = "restapi:main"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.30.0"
```

### Comparing `pitv-0.0.3/src/pitv/__init__.py` & `pitv-0.0.5/src/pitv/__init__.py`

 * *Files identical despite different names*

### Comparing `pitv-0.0.3/src/pitv/pitv.py` & `pitv-0.0.5/src/pitv/pitv.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,11 +10,13 @@
 import datetime
 
 def prettyllog(function, action, item, organization, statuscode, text):
   d_date = datetime.datetime.now()
   reg_format_date = d_date.strftime("%Y-%m-%d %I:%M:%S %p")
   print("%-20s: %-12s %20s %-50s %-20s %-4s %-50s " %( reg_format_date, function,action,item,organization,statuscode, text))
 
-def kalm(mytoken, r):
+def pitv(mytoken, r):
   prettyllog("init", "runtime", "config", "init", "001", "Getting secrets from vault")
+  prettyllog("init", "runtime", "config", "init", "001", "Getting secrets from vault")
+
```

### Comparing `pitv-0.0.3/PKG-INFO` & `pitv-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pitv
-Version: 0.0.3
+Version: 0.0.5
 Summary: Pictures in the vault
 Home-page: https://pictures.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

