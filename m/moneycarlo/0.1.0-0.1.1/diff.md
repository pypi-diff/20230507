# Comparing `tmp/moneycarlo-0.1.0.tar.gz` & `tmp/moneycarlo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneycarlo-0.1.0.tar", last modified: Sun May  7 17:27:21 2023, max compression
+gzip compressed data, was "moneycarlo-0.1.1.tar", last modified: Sun May  7 17:31:31 2023, max compression
```

## Comparing `moneycarlo-0.1.0.tar` & `moneycarlo-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-07 17:27:21.073077 moneycarlo-0.1.0/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    35149 2023-05-07 15:16:09.000000 moneycarlo-0.1.0/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)    40903 2023-05-07 17:27:21.073077 moneycarlo-0.1.0/PKG-INFO
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       68 2023-05-07 15:18:11.000000 moneycarlo-0.1.0/README.md
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      699 2023-05-07 17:27:02.000000 moneycarlo-0.1.0/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-07 17:27:21.073077 moneycarlo-0.1.0/setup.cfg
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-07 17:27:21.073077 moneycarlo-0.1.0/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-07 17:27:21.073077 moneycarlo-0.1.0/src/moneycarlo/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-05-07 15:20:57.000000 moneycarlo-0.1.0/src/moneycarlo/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      164 2023-05-07 16:50:18.000000 moneycarlo-0.1.0/src/moneycarlo/__main__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1879 2023-05-07 17:25:51.000000 moneycarlo-0.1.0/src/moneycarlo/contracts.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-07 17:27:21.073077 moneycarlo-0.1.0/src/moneycarlo.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    40903 2023-05-07 17:27:21.000000 moneycarlo-0.1.0/src/moneycarlo.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      327 2023-05-07 17:27:21.000000 moneycarlo-0.1.0/src/moneycarlo.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-07 17:27:21.000000 moneycarlo-0.1.0/src/moneycarlo.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       42 2023-05-07 17:27:21.000000 moneycarlo-0.1.0/src/moneycarlo.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       11 2023-05-07 17:27:21.000000 moneycarlo-0.1.0/src/moneycarlo.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-07 17:27:21.073077 moneycarlo-0.1.0/tests/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1870 2023-05-07 16:16:06.000000 moneycarlo-0.1.0/tests/test_contracts.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-07 17:31:31.421559 moneycarlo-0.1.1/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    35149 2023-05-07 15:16:09.000000 moneycarlo-0.1.1/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    40903 2023-05-07 17:31:31.421559 moneycarlo-0.1.1/PKG-INFO
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       68 2023-05-07 15:18:11.000000 moneycarlo-0.1.1/README.md
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      699 2023-05-07 17:30:52.000000 moneycarlo-0.1.1/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-07 17:31:31.421559 moneycarlo-0.1.1/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-07 17:31:31.417559 moneycarlo-0.1.1/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-07 17:31:31.421559 moneycarlo-0.1.1/src/moneycarlo/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-05-07 15:20:57.000000 moneycarlo-0.1.1/src/moneycarlo/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      240 2023-05-07 17:30:39.000000 moneycarlo-0.1.1/src/moneycarlo/__main__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1879 2023-05-07 17:25:51.000000 moneycarlo-0.1.1/src/moneycarlo/contracts.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-07 17:31:31.421559 moneycarlo-0.1.1/src/moneycarlo.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    40903 2023-05-07 17:31:31.000000 moneycarlo-0.1.1/src/moneycarlo.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      327 2023-05-07 17:31:31.000000 moneycarlo-0.1.1/src/moneycarlo.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-07 17:31:31.000000 moneycarlo-0.1.1/src/moneycarlo.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       42 2023-05-07 17:31:31.000000 moneycarlo-0.1.1/src/moneycarlo.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       11 2023-05-07 17:31:31.000000 moneycarlo-0.1.1/src/moneycarlo.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-07 17:31:31.421559 moneycarlo-0.1.1/tests/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1870 2023-05-07 16:16:06.000000 moneycarlo-0.1.1/tests/test_contracts.py
```

### Comparing `moneycarlo-0.1.0/LICENSE` & `moneycarlo-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moneycarlo-0.1.0/PKG-INFO` & `moneycarlo-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneycarlo
-Version: 0.1.0
+Version: 0.1.1
 Summary: Project to model revenue based on contract conditions.
 Author-email: Brandon Sexton <brandon.sexton.1@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `moneycarlo-0.1.0/pyproject.toml` & `moneycarlo-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "moneycarlo"
-version = "0.1.0"
+version = "0.1.1"
 description = "Project to model revenue based on contract conditions."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
   {name = "Brandon Sexton", email = "brandon.sexton.1@outlook.com" }
 ]
```

### Comparing `moneycarlo-0.1.0/src/moneycarlo/contracts.py` & `moneycarlo-0.1.1/src/moneycarlo/contracts.py`

 * *Files identical despite different names*

### Comparing `moneycarlo-0.1.0/src/moneycarlo.egg-info/PKG-INFO` & `moneycarlo-0.1.1/src/moneycarlo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneycarlo
-Version: 0.1.0
+Version: 0.1.1
 Summary: Project to model revenue based on contract conditions.
 Author-email: Brandon Sexton <brandon.sexton.1@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `moneycarlo-0.1.0/tests/test_contracts.py` & `moneycarlo-0.1.1/tests/test_contracts.py`

 * *Files identical despite different names*

