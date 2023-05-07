# Comparing `tmp/bumbo_shogo-0.0.2.tar.gz` & `tmp/bumbo_shogo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bumbo_shogo-0.0.2.tar", last modified: Sun May  7 02:12:45 2023, max compression
+gzip compressed data, was "bumbo_shogo-0.0.3.tar", last modified: Sun May  7 02:48:49 2023, max compression
```

## Comparing `bumbo_shogo-0.0.2.tar` & `bumbo_shogo-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 Shogo      (501) staff       (20)        0 2023-05-07 02:12:45.093917 bumbo_shogo-0.0.2/
--rw-r--r--   0 Shogo      (501) staff       (20)     3828 2023-05-07 02:12:45.093443 bumbo_shogo-0.0.2/PKG-INFO
--rw-r--r--   0 Shogo      (501) staff       (20)     3486 2023-05-07 02:07:23.000000 bumbo_shogo-0.0.2/README.md
-drwxr-xr-x   0 Shogo      (501) staff       (20)        0 2023-05-07 02:12:45.087940 bumbo_shogo-0.0.2/bumbo/
--rw-r--r--   0 Shogo      (501) staff       (20)        0 2023-05-06 14:48:44.000000 bumbo_shogo-0.0.2/bumbo/__init__.py
--rw-r--r--   0 Shogo      (501) staff       (20)     3789 2023-05-06 14:48:23.000000 bumbo_shogo-0.0.2/bumbo/api.py
--rw-r--r--   0 Shogo      (501) staff       (20)      674 2023-05-06 11:54:24.000000 bumbo_shogo-0.0.2/bumbo/middleware.py
--rw-r--r--   0 Shogo      (501) staff       (20)      955 2023-05-06 14:40:43.000000 bumbo_shogo-0.0.2/bumbo/response.py
-drwxr-xr-x   0 Shogo      (501) staff       (20)        0 2023-05-07 02:12:45.092058 bumbo_shogo-0.0.2/bumbo_shogo.egg-info/
--rw-r--r--   0 Shogo      (501) staff       (20)     3828 2023-05-07 02:12:44.000000 bumbo_shogo-0.0.2/bumbo_shogo.egg-info/PKG-INFO
--rw-r--r--   0 Shogo      (501) staff       (20)      261 2023-05-07 02:12:45.000000 bumbo_shogo-0.0.2/bumbo_shogo.egg-info/SOURCES.txt
--rw-r--r--   0 Shogo      (501) staff       (20)        1 2023-05-07 02:12:44.000000 bumbo_shogo-0.0.2/bumbo_shogo.egg-info/dependency_links.txt
--rw-r--r--   0 Shogo      (501) staff       (20)      106 2023-05-07 02:12:44.000000 bumbo_shogo-0.0.2/bumbo_shogo.egg-info/requires.txt
--rw-r--r--   0 Shogo      (501) staff       (20)        6 2023-05-07 02:12:44.000000 bumbo_shogo-0.0.2/bumbo_shogo.egg-info/top_level.txt
--rw-r--r--   0 Shogo      (501) staff       (20)       38 2023-05-07 02:12:45.094063 bumbo_shogo-0.0.2/setup.cfg
--rw-r--r--   0 Shogo      (501) staff       (20)     1792 2023-05-07 02:12:34.000000 bumbo_shogo-0.0.2/setup.py
+drwxr-xr-x   0 Shogo      (501) staff       (20)        0 2023-05-07 02:48:49.401926 bumbo_shogo-0.0.3/
+-rw-r--r--   0 Shogo      (501) staff       (20)     3828 2023-05-07 02:48:49.400036 bumbo_shogo-0.0.3/PKG-INFO
+-rw-r--r--   0 Shogo      (501) staff       (20)     3486 2023-05-07 02:07:23.000000 bumbo_shogo-0.0.3/README.md
+drwxr-xr-x   0 Shogo      (501) staff       (20)        0 2023-05-07 02:48:49.394337 bumbo_shogo-0.0.3/bumbo/
+-rw-r--r--   0 Shogo      (501) staff       (20)        0 2023-05-06 14:48:44.000000 bumbo_shogo-0.0.3/bumbo/__init__.py
+-rw-r--r--   0 Shogo      (501) staff       (20)     3789 2023-05-06 14:48:23.000000 bumbo_shogo-0.0.3/bumbo/api.py
+-rw-r--r--   0 Shogo      (501) staff       (20)      674 2023-05-06 11:54:24.000000 bumbo_shogo-0.0.3/bumbo/middleware.py
+-rw-r--r--   0 Shogo      (501) staff       (20)      955 2023-05-06 14:40:43.000000 bumbo_shogo-0.0.3/bumbo/response.py
+drwxr-xr-x   0 Shogo      (501) staff       (20)        0 2023-05-07 02:48:49.399381 bumbo_shogo-0.0.3/bumbo_shogo.egg-info/
+-rw-r--r--   0 Shogo      (501) staff       (20)     3828 2023-05-07 02:48:49.000000 bumbo_shogo-0.0.3/bumbo_shogo.egg-info/PKG-INFO
+-rw-r--r--   0 Shogo      (501) staff       (20)      261 2023-05-07 02:48:49.000000 bumbo_shogo-0.0.3/bumbo_shogo.egg-info/SOURCES.txt
+-rw-r--r--   0 Shogo      (501) staff       (20)        1 2023-05-07 02:48:49.000000 bumbo_shogo-0.0.3/bumbo_shogo.egg-info/dependency_links.txt
+-rw-r--r--   0 Shogo      (501) staff       (20)      106 2023-05-07 02:48:49.000000 bumbo_shogo-0.0.3/bumbo_shogo.egg-info/requires.txt
+-rw-r--r--   0 Shogo      (501) staff       (20)        6 2023-05-07 02:48:49.000000 bumbo_shogo-0.0.3/bumbo_shogo.egg-info/top_level.txt
+-rw-r--r--   0 Shogo      (501) staff       (20)       38 2023-05-07 02:48:49.402121 bumbo_shogo-0.0.3/setup.cfg
+-rw-r--r--   0 Shogo      (501) staff       (20)     1792 2023-05-07 02:48:40.000000 bumbo_shogo-0.0.3/setup.py
```

### Comparing `bumbo_shogo-0.0.2/PKG-INFO` & `bumbo_shogo-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bumbo_shogo
-Version: 0.0.2
+Version: 0.0.3
 Summary: Bumbo Python Web Framework built for learning purposes.
 Home-page: UNKNOWN
 Author: Shogo Okuda
 Author-email: shougees@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `bumbo_shogo-0.0.2/README.md` & `bumbo_shogo-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bumbo_shogo-0.0.2/bumbo/api.py` & `bumbo_shogo-0.0.3/bumbo/api.py`

 * *Files identical despite different names*

### Comparing `bumbo_shogo-0.0.2/bumbo/middleware.py` & `bumbo_shogo-0.0.3/bumbo/middleware.py`

 * *Files identical despite different names*

### Comparing `bumbo_shogo-0.0.2/bumbo/response.py` & `bumbo_shogo-0.0.3/bumbo/response.py`

 * *Files identical despite different names*

### Comparing `bumbo_shogo-0.0.2/bumbo_shogo.egg-info/PKG-INFO` & `bumbo_shogo-0.0.3/bumbo_shogo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bumbo-shogo
-Version: 0.0.2
+Version: 0.0.3
 Summary: Bumbo Python Web Framework built for learning purposes.
 Home-page: UNKNOWN
 Author: Shogo Okuda
 Author-email: shougees@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `bumbo_shogo-0.0.2/setup.py` & `bumbo_shogo-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Package meta-data.
 NAME = "bumbo_shogo"
 DESCRIPTION = "Bumbo Python Web Framework built for learning purposes."
 EMAIL = "shougees@gmail.com"
 AUTHOR = "Shogo Okuda"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 # Which packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==2.10.3",
     "parse==1.12.1",
     "requests==2.22.0",
     "requests-wsgi-adapter==0.4.1",
```

