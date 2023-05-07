# Comparing `tmp/flask-guard-0.0.6.tar.gz` & `tmp/flask-guard-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-guard-0.0.6.tar", last modified: Sun May  7 13:19:53 2023, max compression
+gzip compressed data, was "flask-guard-0.0.7.tar", last modified: Sun May  7 14:01:00 2023, max compression
```

## Comparing `flask-guard-0.0.6.tar` & `flask-guard-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 13:19:53.351012 flask-guard-0.0.6/
--rw-rw-rw-   0        0        0     1107 2023-05-07 07:08:02.000000 flask-guard-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0     2647 2023-05-07 13:19:53.350010 flask-guard-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2166 2023-05-06 09:33:32.000000 flask-guard-0.0.6/README.md
--rw-rw-rw-   0        0        0      102 2023-05-07 07:17:25.000000 flask-guard-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 13:19:53.351012 flask-guard-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      783 2023-05-07 13:19:18.000000 flask-guard-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 13:19:53.311007 flask-guard-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-07 13:19:53.325011 flask-guard-0.0.6/src/FlaskGuard/
--rw-rw-rw-   0        0        0        0 2023-05-07 13:06:37.000000 flask-guard-0.0.6/src/FlaskGuard/__init__.py
--rw-rw-rw-   0        0        0     6937 2023-05-07 13:15:18.000000 flask-guard-0.0.6/src/FlaskGuard/flask_guard.py
--rw-rw-rw-   0        0        0     3160 2023-05-06 08:13:00.000000 flask-guard-0.0.6/src/FlaskGuard/request_parameter.py
-drwxrwxrwx   0        0        0        0 2023-05-07 13:19:53.344037 flask-guard-0.0.6/src/flask_guard.egg-info/
--rw-rw-rw-   0        0        0     2647 2023-05-07 13:19:53.000000 flask-guard-0.0.6/src/flask_guard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-05-07 13:19:53.000000 flask-guard-0.0.6/src/flask_guard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 13:19:53.000000 flask-guard-0.0.6/src/flask_guard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-07 13:19:53.000000 flask-guard-0.0.6/src/flask_guard.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-07 13:19:53.348006 flask-guard-0.0.6/tests/
--rw-rw-rw-   0        0        0    24667 2023-05-07 13:16:37.000000 flask-guard-0.0.6/tests/test_flask_guard.py
--rw-rw-rw-   0        0        0     7282 2023-05-07 13:13:48.000000 flask-guard-0.0.6/tests/test_request_parameter.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:01:00.327684 flask-guard-0.0.7/
+-rw-rw-rw-   0        0        0     1107 2023-05-07 07:08:02.000000 flask-guard-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     2647 2023-05-07 14:01:00.326682 flask-guard-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2166 2023-05-06 09:33:32.000000 flask-guard-0.0.7/README.md
+-rw-rw-rw-   0        0        0      102 2023-05-07 07:17:25.000000 flask-guard-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 14:01:00.327684 flask-guard-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      783 2023-05-07 14:00:36.000000 flask-guard-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:01:00.285683 flask-guard-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 14:01:00.299676 flask-guard-0.0.7/src/FlaskGuard/
+-rw-rw-rw-   0        0        0       86 2023-05-07 14:00:28.000000 flask-guard-0.0.7/src/FlaskGuard/__init__.py
+-rw-rw-rw-   0        0        0     6937 2023-05-07 13:15:18.000000 flask-guard-0.0.7/src/FlaskGuard/flask_guard.py
+-rw-rw-rw-   0        0        0     3160 2023-05-06 08:13:00.000000 flask-guard-0.0.7/src/FlaskGuard/request_parameter.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:01:00.319704 flask-guard-0.0.7/src/flask_guard.egg-info/
+-rw-rw-rw-   0        0        0     2647 2023-05-07 14:01:00.000000 flask-guard-0.0.7/src/flask_guard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-05-07 14:01:00.000000 flask-guard-0.0.7/src/flask_guard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 14:01:00.000000 flask-guard-0.0.7/src/flask_guard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-07 14:01:00.000000 flask-guard-0.0.7/src/flask_guard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 14:01:00.324674 flask-guard-0.0.7/tests/
+-rw-rw-rw-   0        0        0    24667 2023-05-07 13:16:37.000000 flask-guard-0.0.7/tests/test_flask_guard.py
+-rw-rw-rw-   0        0        0     7282 2023-05-07 13:13:48.000000 flask-guard-0.0.7/tests/test_request_parameter.py
```

### Comparing `flask-guard-0.0.6/LICENSE.txt` & `flask-guard-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flask-guard-0.0.6/PKG-INFO` & `flask-guard-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-guard
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library for checking if JSON requests have valid data.
 Home-page: https://github.com/beki1337/FlaskGuard
 Author: Belmin Batic
 Author-email: baticbelmin10@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flask-guard-0.0.6/README.md` & `flask-guard-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `flask-guard-0.0.6/setup.py` & `flask-guard-0.0.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "flask-guard",
-    version = "0.0.6",
+    version = "0.0.7",
     author = "Belmin Batic",
     author_email = "baticbelmin10@gmail.com",
     description = "A library for checking if JSON requests have valid data.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/beki1337/FlaskGuard",
     classifiers = [
```

### Comparing `flask-guard-0.0.6/src/FlaskGuard/flask_guard.py` & `flask-guard-0.0.7/src/FlaskGuard/flask_guard.py`

 * *Files identical despite different names*

### Comparing `flask-guard-0.0.6/src/FlaskGuard/request_parameter.py` & `flask-guard-0.0.7/src/FlaskGuard/request_parameter.py`

 * *Files identical despite different names*

### Comparing `flask-guard-0.0.6/src/flask_guard.egg-info/PKG-INFO` & `flask-guard-0.0.7/src/flask_guard.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-guard
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library for checking if JSON requests have valid data.
 Home-page: https://github.com/beki1337/FlaskGuard
 Author: Belmin Batic
 Author-email: baticbelmin10@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flask-guard-0.0.6/tests/test_flask_guard.py` & `flask-guard-0.0.7/tests/test_flask_guard.py`

 * *Files identical despite different names*

### Comparing `flask-guard-0.0.6/tests/test_request_parameter.py` & `flask-guard-0.0.7/tests/test_request_parameter.py`

 * *Files identical despite different names*

