# Comparing `tmp/pitv-0.0.5.tar.gz` & `tmp/pitv-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pitv-0.0.5.tar", max compression
+gzip compressed data, was "pitv-0.0.6.tar", max compression
```

## Comparing `pitv-0.0.5.tar` & `pitv-0.0.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1081 2023-05-06 19:25:58.253937 pitv-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0      907 2023-05-07 17:51:36.940689 pitv-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1038 2023-05-06 19:25:58.253937 pitv-0.0.5/src/pitv/__init__.py
--rw-r--r--   0        0        0      641 2023-05-07 17:40:52.896913 pitv-0.0.5/src/pitv/pitv.py
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 pitv-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-06 19:25:58.253937 pitv-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0      907 2023-05-07 18:07:16.134219 pitv-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1038 2023-05-06 19:25:58.253937 pitv-0.0.6/src/pitv/__init__.py
+-rw-r--r--   0        0        0      641 2023-05-07 17:40:52.896913 pitv-0.0.6/src/pitv/pitv.py
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 pitv-0.0.6/PKG-INFO
```

### Comparing `pitv-0.0.5/LICENSE.txt` & `pitv-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pitv-0.0.5/pyproject.toml` & `pitv-0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pitv"
-version = "0.0.5"
+version = "0.0.6"
 description = "Pictures in the vault"
 authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
 license = "MIT"
 homepage = "https://pictures.openknowit.com"
 repository = "https://github.com/JakobHolstDK/picturesinthevault.git"
 
 [tool.poetry.scripts]
```

### Comparing `pitv-0.0.5/src/pitv/__init__.py` & `pitv-0.0.6/src/pitv/__init__.py`

 * *Files identical despite different names*

### Comparing `pitv-0.0.5/src/pitv/pitv.py` & `pitv-0.0.6/src/pitv/pitv.py`

 * *Files identical despite different names*

### Comparing `pitv-0.0.5/PKG-INFO` & `pitv-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pitv
-Version: 0.0.5
+Version: 0.0.6
 Summary: Pictures in the vault
 Home-page: https://pictures.openknowit.com
 License: MIT
 Author: Jakob Holst
 Author-email: jakob.holst@knowit.dk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

