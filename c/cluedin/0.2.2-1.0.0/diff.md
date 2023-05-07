# Comparing `tmp/cluedin-0.2.2.tar.gz` & `tmp/cluedin-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cluedin-0.2.2.tar", max compression
+gzip compressed data, was "cluedin-1.0.0.tar", max compression
```

## Comparing `cluedin-0.2.2.tar` & `cluedin-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1921 2023-05-07 18:04:57.326657 cluedin-0.2.2/README.md
--rw-r--r--   0        0        0      119 2023-05-07 15:56:18.443909 cluedin-0.2.2/cluedin/__init__.py
--rw-r--r--   0        0        0      664 2023-05-06 19:21:43.490227 cluedin-0.2.2/cluedin/auth.py
--rw-r--r--   0        0        0     1120 2023-05-07 16:45:36.605300 cluedin-0.2.2/cluedin/gql.py
--rw-r--r--   0        0        0      681 2023-05-07 15:56:40.250091 cluedin-0.2.2/cluedin/urls.py
--rw-r--r--   0        0        0      264 2023-05-06 19:41:45.000595 cluedin-0.2.2/cluedin/utils.py
--rw-r--r--   0        0        0      562 2023-05-07 19:21:51.712953 cluedin-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 cluedin-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1921 2023-05-07 18:04:57.326657 cluedin-1.0.0/README.md
+-rw-r--r--   0        0        0      119 2023-05-07 15:56:18.443909 cluedin-1.0.0/cluedin/__init__.py
+-rw-r--r--   0        0        0      664 2023-05-06 19:21:43.490227 cluedin-1.0.0/cluedin/auth.py
+-rw-r--r--   0        0        0     1120 2023-05-07 16:45:36.605300 cluedin-1.0.0/cluedin/gql.py
+-rw-r--r--   0        0        0      681 2023-05-07 15:56:40.250091 cluedin-1.0.0/cluedin/urls.py
+-rw-r--r--   0        0        0      264 2023-05-06 19:41:45.000595 cluedin-1.0.0/cluedin/utils.py
+-rw-r--r--   0        0        0      562 2023-05-07 19:23:43.864922 cluedin-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 cluedin-1.0.0/PKG-INFO
```

### Comparing `cluedin-0.2.2/README.md` & `cluedin-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cluedin-0.2.2/cluedin/auth.py` & `cluedin-1.0.0/cluedin/auth.py`

 * *Files identical despite different names*

### Comparing `cluedin-0.2.2/cluedin/gql.py` & `cluedin-1.0.0/cluedin/gql.py`

 * *Files identical despite different names*

### Comparing `cluedin-0.2.2/cluedin/urls.py` & `cluedin-1.0.0/cluedin/urls.py`

 * *Files identical despite different names*

### Comparing `cluedin-0.2.2/pyproject.toml` & `cluedin-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cluedin"
-version = "0.2.2"
+version = "1.0.0"
 description = "A Python client for CluedIn API."
 authors = ["Roman Klimenko <romaklimenko@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["cluedin", "mdm", "master data management"]
 maintainers = ["Roman Klimenko <romaklimenko@gmail.com>"]
 homepage = "https://github.com/romaklimenko/cluedin"
```

### Comparing `cluedin-0.2.2/PKG-INFO` & `cluedin-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluedin
-Version: 0.2.2
+Version: 1.0.0
 Summary: A Python client for CluedIn API.
 Home-page: https://github.com/romaklimenko/cluedin
 License: MIT
 Keywords: cluedin,mdm,master data management
 Author: Roman Klimenko
 Author-email: romaklimenko@gmail.com
 Maintainer: Roman Klimenko
```

