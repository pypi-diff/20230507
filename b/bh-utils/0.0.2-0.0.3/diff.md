# Comparing `tmp/bh-utils-0.0.2.tar.gz` & `tmp/bh-utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bh-utils-0.0.2.tar", last modified: Wed Jan 25 01:44:31 2023, max compression
+gzip compressed data, was "bh-utils-0.0.3.tar", last modified: Sun May  7 01:33:20 2023, max compression
```

## Comparing `bh-utils-0.0.2.tar` & `bh-utils-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-01-25 01:44:31.307075 bh-utils-0.0.2/
--rw-rw-rw-   0        0        0      855 2023-01-25 01:44:31.306234 bh-utils-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-01-24 05:31:53.000000 bh-utils-0.0.2/README.md
--rw-rw-rw-   0        0        0      924 2023-01-25 01:42:47.000000 bh-utils-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-25 01:44:31.307075 bh-utils-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-25 01:44:31.168659 bh-utils-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-01-25 01:44:31.288664 bh-utils-0.0.2/src/bh_utils/
--rw-rw-rw-   0        0        0       88 2023-01-24 10:02:23.000000 bh-utils-0.0.2/src/bh_utils/__init__.py
--rw-rw-rw-   0        0        0     2352 2023-01-24 04:28:09.000000 bh-utils-0.0.2/src/bh_utils/conversions.py
--rw-rw-rw-   0        0        0     3400 2023-01-24 05:09:57.000000 bh-utils-0.0.2/src/bh_utils/date_funcs.py
--rw-rw-rw-   0        0        0     1587 2023-01-24 04:55:45.000000 bh-utils-0.0.2/src/bh_utils/json_funcs.py
--rw-rw-rw-   0        0        0      814 2023-01-24 04:41:48.000000 bh-utils-0.0.2/src/bh_utils/str_funcs.py
--rw-rw-rw-   0        0        0     3325 2023-01-24 05:18:42.000000 bh-utils-0.0.2/src/bh_utils/template_funcs.py
-drwxrwxrwx   0        0        0        0 2023-01-25 01:44:31.305075 bh-utils-0.0.2/src/bh_utils.egg-info/
--rw-rw-rw-   0        0        0      855 2023-01-25 01:44:31.000000 bh-utils-0.0.2/src/bh_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-01-25 01:44:31.000000 bh-utils-0.0.2/src/bh_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-25 01:44:31.000000 bh-utils-0.0.2/src/bh_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2023-01-25 01:44:31.000000 bh-utils-0.0.2/src/bh_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-01-25 01:44:31.000000 bh-utils-0.0.2/src/bh_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 01:33:20.401244 bh-utils-0.0.3/
+-rw-rw-rw-   0        0        0      855 2023-05-07 01:33:20.401244 bh-utils-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-01-24 05:31:53.000000 bh-utils-0.0.3/README.md
+-rw-rw-rw-   0        0        0      939 2023-05-07 01:31:14.000000 bh-utils-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 01:33:20.401244 bh-utils-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 01:33:20.171690 bh-utils-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 01:33:20.291694 bh-utils-0.0.3/src/bh_utils/
+-rw-rw-rw-   0        0        0       88 2023-01-24 10:02:23.000000 bh-utils-0.0.3/src/bh_utils/__init__.py
+-rw-rw-rw-   0        0        0     2352 2023-01-24 04:28:09.000000 bh-utils-0.0.3/src/bh_utils/conversions.py
+-rw-rw-rw-   0        0        0     3400 2023-01-24 05:09:57.000000 bh-utils-0.0.3/src/bh_utils/date_funcs.py
+-rw-rw-rw-   0        0        0     1587 2023-01-24 04:55:45.000000 bh-utils-0.0.3/src/bh_utils/json_funcs.py
+-rw-rw-rw-   0        0        0     1331 2023-03-28 00:16:41.000000 bh-utils-0.0.3/src/bh_utils/password_funcs.py
+-rw-rw-rw-   0        0        0     1354 2023-03-27 23:57:25.000000 bh-utils-0.0.3/src/bh_utils/str_funcs.py
+-rw-rw-rw-   0        0        0     3325 2023-01-24 05:18:42.000000 bh-utils-0.0.3/src/bh_utils/template_funcs.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:33:20.315695 bh-utils-0.0.3/src/bh_utils.egg-info/
+-rw-rw-rw-   0        0        0      855 2023-05-07 01:33:20.000000 bh-utils-0.0.3/src/bh_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2023-05-07 01:33:20.000000 bh-utils-0.0.3/src/bh_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 01:33:20.000000 bh-utils-0.0.3/src/bh_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2023-05-07 01:33:20.000000 bh-utils-0.0.3/src/bh_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-07 01:33:20.000000 bh-utils-0.0.3/src/bh_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 01:33:20.401244 bh-utils-0.0.3/tests/
+-rw-rw-rw-   0        0        0     3172 2022-12-18 06:58:50.000000 bh-utils-0.0.3/tests/test_conversions.py
+-rw-rw-rw-   0        0        0     1130 2023-01-05 11:53:56.000000 bh-utils-0.0.3/tests/test_date_funcs.py
+-rw-rw-rw-   0        0        0     1236 2023-01-22 23:33:32.000000 bh-utils-0.0.3/tests/test_json_funcs.py
+-rw-rw-rw-   0        0        0      417 2023-03-28 00:19:10.000000 bh-utils-0.0.3/tests/test_password_funcs.py
+-rw-rw-rw-   0        0        0     1535 2023-03-29 03:58:55.000000 bh-utils-0.0.3/tests/test_str_funcs.py
+-rw-rw-rw-   0        0        0     3390 2023-01-26 07:25:30.000000 bh-utils-0.0.3/tests/test_template_funcs.py
```

### Comparing `bh-utils-0.0.2/PKG-INFO` & `bh-utils-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bh-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Utility Functions Library.
 Author-email: Van Be Hai Nguyen <behai_nguyen@hotmail.com>
 Project-URL: repository, https://github.com/behai-nguyen/bh_utils
 Project-URL: documentation, https://bh-utils.readthedocs.io/
 Keywords: utility,functions,library
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `bh-utils-0.0.2/pyproject.toml` & `bh-utils-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bh-utils"
-version = "0.0.2"
+version = "0.0.3"
 description = "Utility Functions Library."
 
 readme = "README.md"
 authors = [{ name = "Van Be Hai Nguyen", email = "behai_nguyen@hotmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["utility", "functions", "library"]
 
 dependencies = [
-    'tomli; python_version < "3.11"',
+    'tomli; python_version >= "3.10"',
     'PyYAML', 
-    'simplejson'
+    'simplejson',
+    'jinja2',
+    'pytest',
+    'coverage'
 ]
 
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 build = [
     "build", 
     "twine"
 ]
 dev = [
-    "pytest",
-    "coverage",
     "sphinx",
     "myst-parser",
     "sphinx-rtd-theme"
 ]
 
 [project.urls]
 repository = "https://github.com/behai-nguyen/bh_utils"
```

### Comparing `bh-utils-0.0.2/src/bh_utils/conversions.py` & `bh-utils-0.0.3/src/bh_utils/conversions.py`

 * *Files identical despite different names*

### Comparing `bh-utils-0.0.2/src/bh_utils/date_funcs.py` & `bh-utils-0.0.3/src/bh_utils/date_funcs.py`

 * *Files identical despite different names*

### Comparing `bh-utils-0.0.2/src/bh_utils/json_funcs.py` & `bh-utils-0.0.3/src/bh_utils/json_funcs.py`

 * *Files identical despite different names*

### Comparing `bh-utils-0.0.2/src/bh_utils/str_funcs.py` & `bh-utils-0.0.3/src/bh_utils/str_funcs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """
 Some string routines.
 
 For usage examples, see ``./tests/test_str_funcs.py``.
 """
+
+from re import sub
+
 def extract_session_cookie(cookie: str) -> str:
     """
     From a string which might have multiple ``name=value`` pair strings, get the value 
     for ``session`` name.
 
     ``name=value`` pair strings are separated by semicolon (``;``). For example:
 
@@ -20,7 +23,26 @@
     """
     
     items = cookie.split(';')
     for itm in items:
         itm_cleaned = itm.strip()
         if ("session=" in itm_cleaned): return itm_cleaned[8:]
     return '--- No Cookie ---'
+
+def camel_case(s: str) -> str:
+    """Convert a string to camelCase.
+
+    Source: https://www.w3resource.com/python-exercises/string/python-data-type-string-exercise-96.php
+	
+    Example::
+	
+    ``project-id`` converted to ``projectId``.	
+    ``name`` to ``name``.
+
+    :param str s: source string to be converted.
+
+    :return: camelCase representation of source string.
+    :rtype: str.
+    """
+
+    s = sub(r"(_|-)+", " ", s).title().replace(" ", "")
+    return ''.join([s[0].lower(), s[1:]])
```

### Comparing `bh-utils-0.0.2/src/bh_utils/template_funcs.py` & `bh-utils-0.0.3/src/bh_utils/template_funcs.py`

 * *Files identical despite different names*

### Comparing `bh-utils-0.0.2/src/bh_utils.egg-info/PKG-INFO` & `bh-utils-0.0.3/src/bh_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bh-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Utility Functions Library.
 Author-email: Van Be Hai Nguyen <behai_nguyen@hotmail.com>
 Project-URL: repository, https://github.com/behai-nguyen/bh_utils
 Project-URL: documentation, https://bh-utils.readthedocs.io/
 Keywords: utility,functions,library
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

