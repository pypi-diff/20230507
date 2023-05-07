# Comparing `tmp/pfelogic-2023.5.5.0.tar.gz` & `tmp/pfelogic-2023.5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfelogic-2023.5.5.0.tar", last modified: Sat May  6 05:22:20 2023, max compression
+gzip compressed data, was "pfelogic-2023.5.6.0.tar", last modified: Sun May  7 00:14:10 2023, max compression
```

## Comparing `pfelogic-2023.5.5.0.tar` & `pfelogic-2023.5.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:22:20.546723 pfelogic-2023.5.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-06 05:22:04.000000 pfelogic-2023.5.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-06 05:22:20.546723 pfelogic-2023.5.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-06 05:22:04.000000 pfelogic-2023.5.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:22:20.546723 pfelogic-2023.5.5.0/pfe/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-06 05:22:04.000000 pfelogic-2023.5.5.0/pfe/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11683 2023-05-06 05:22:04.000000 pfelogic-2023.5.5.0/pfe/comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 05:22:20.546723 pfelogic-2023.5.5.0/pfelogic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-06 05:22:20.000000 pfelogic-2023.5.5.0/pfelogic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-06 05:22:20.000000 pfelogic-2023.5.5.0/pfelogic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 05:22:20.000000 pfelogic-2023.5.5.0/pfelogic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 05:22:20.000000 pfelogic-2023.5.5.0/pfelogic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-06 05:22:20.000000 pfelogic-2023.5.5.0/pfelogic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-06 05:22:04.000000 pfelogic-2023.5.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 05:22:20.546723 pfelogic-2023.5.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:14:10.332196 pfelogic-2023.5.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-07 00:13:54.000000 pfelogic-2023.5.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-07 00:14:10.332196 pfelogic-2023.5.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-07 00:13:54.000000 pfelogic-2023.5.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:14:10.332196 pfelogic-2023.5.6.0/pfe/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-07 00:13:54.000000 pfelogic-2023.5.6.0/pfe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11683 2023-05-07 00:13:54.000000 pfelogic-2023.5.6.0/pfe/comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:14:10.332196 pfelogic-2023.5.6.0/pfelogic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-07 00:14:10.000000 pfelogic-2023.5.6.0/pfelogic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-07 00:14:10.000000 pfelogic-2023.5.6.0/pfelogic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 00:14:10.000000 pfelogic-2023.5.6.0/pfelogic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 00:14:10.000000 pfelogic-2023.5.6.0/pfelogic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-07 00:14:10.000000 pfelogic-2023.5.6.0/pfelogic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-07 00:13:54.000000 pfelogic-2023.5.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 00:14:10.332196 pfelogic-2023.5.6.0/setup.cfg
```

### Comparing `pfelogic-2023.5.5.0/LICENSE` & `pfelogic-2023.5.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pfelogic-2023.5.5.0/PKG-INFO` & `pfelogic-2023.5.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pfelogic
-Version: 2023.5.5.0
+Version: 2023.5.6.0
 Summary: An opinionated pass fail exempt library that I wanted to stop making in every project.
 Author-email: Chris Halbersma <chalbersma@halbersma.us>
 License: BSD-2-Clause
 Keywords: manowar
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pfelogic
 
 pfelogic is a pass, fail, exempt comparison library for objects and lists of objects that I keep repeately making.
 Orignally for github.com/chalbermsa/manowar but should be generic(ish)
```

### Comparing `pfelogic-2023.5.5.0/pfe/comparison.py` & `pfelogic-2023.5.6.0/pfe/comparison.py`

 * *Files identical despite different names*

### Comparing `pfelogic-2023.5.5.0/pfelogic.egg-info/PKG-INFO` & `pfelogic-2023.5.6.0/pfelogic.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pfelogic
-Version: 2023.5.5.0
+Version: 2023.5.6.0
 Summary: An opinionated pass fail exempt library that I wanted to stop making in every project.
 Author-email: Chris Halbersma <chalbersma@halbersma.us>
 License: BSD-2-Clause
 Keywords: manowar
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pfelogic
 
 pfelogic is a pass, fail, exempt comparison library for objects and lists of objects that I keep repeately making.
 Orignally for github.com/chalbermsa/manowar but should be generic(ish)
```

### Comparing `pfelogic-2023.5.5.0/pyproject.toml` & `pfelogic-2023.5.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,21 @@
   "twine",
   "setuptools"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pfelogic"
-version = "2023.05.05.0"
+version = "2023.05.06.0"
 authors = [
     {name = "Chris Halbersma", email = "chalbersma@halbersma.us"},
 ]
 description = "An opinionated pass fail exempt library that I wanted to stop making in every project."
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 keywords = ["manowar"]
 license = {text = "BSD-2-Clause"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "packaging",
```

