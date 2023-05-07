# Comparing `tmp/rcmpy-1.3.0.tar.gz` & `tmp/rcmpy-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcmpy-1.3.0.tar", last modified: Sun May  7 03:23:41 2023, max compression
+gzip compressed data, was "rcmpy-1.4.0.tar", last modified: Sun May  7 21:30:24 2023, max compression
```

## Comparing `rcmpy-1.3.0.tar` & `rcmpy-1.4.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-07 03:22:34.000000 rcmpy-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-05-07 03:23:41.245388 rcmpy-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-05-07 03:22:34.000000 rcmpy-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-07 03:22:34.000000 rcmpy-1.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.241388 rcmpy-1.3.0/rcmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/rcmpy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/commands/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/commands/use.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/commands/variant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/commands/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/rcmpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/config/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.241388 rcmpy-1.3.0/rcmpy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/rcmpy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/data/schemas/ManagedFile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/data/schemas/State.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/rcmpy/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/environment/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/environment/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/rcmpy/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/rcmpy/state/
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/rcmpy/xdg/
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/xdg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/rcmpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-05-07 03:23:41.000000 rcmpy-1.3.0/rcmpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-07 03:23:41.000000 rcmpy-1.3.0/rcmpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 03:23:41.000000 rcmpy-1.3.0/rcmpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-07 03:23:41.000000 rcmpy-1.3.0/rcmpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-07 03:23:41.000000 rcmpy-1.3.0/rcmpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 03:23:41.000000 rcmpy-1.3.0/rcmpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 03:23:41.245388 rcmpy-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-07 03:22:34.000000 rcmpy-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-07 03:22:34.000000 rcmpy-1.3.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-07 03:22:34.000000 rcmpy-1.3.0/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-07 03:22:34.000000 rcmpy-1.3.0/tests/test_xdg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.536857 rcmpy-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-07 21:28:52.000000 rcmpy-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-05-07 21:30:24.536857 rcmpy-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-05-07 21:28:52.000000 rcmpy-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-07 21:28:52.000000 rcmpy-1.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.524857 rcmpy-1.4.0/rcmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.528857 rcmpy-1.4.0/rcmpy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/commands/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/commands/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/commands/use.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/commands/variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/commands/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.528857 rcmpy-1.4.0/rcmpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/config/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.524857 rcmpy-1.4.0/rcmpy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.528857 rcmpy-1.4.0/rcmpy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/data/schemas/ManagedFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/data/schemas/State.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.532857 rcmpy-1.4.0/rcmpy/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/environment/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/environment/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.532857 rcmpy-1.4.0/rcmpy/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.532857 rcmpy-1.4.0/rcmpy/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.532857 rcmpy-1.4.0/rcmpy/xdg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-07 21:28:52.000000 rcmpy-1.4.0/rcmpy/xdg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.528857 rcmpy-1.4.0/rcmpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-05-07 21:30:24.000000 rcmpy-1.4.0/rcmpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-07 21:30:24.000000 rcmpy-1.4.0/rcmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 21:30:24.000000 rcmpy-1.4.0/rcmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-07 21:30:24.000000 rcmpy-1.4.0/rcmpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-07 21:30:24.000000 rcmpy-1.4.0/rcmpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 21:30:24.000000 rcmpy-1.4.0/rcmpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 21:30:24.536857 rcmpy-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-07 21:28:52.000000 rcmpy-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:30:24.532857 rcmpy-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-07 21:28:52.000000 rcmpy-1.4.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-07 21:28:52.000000 rcmpy-1.4.0/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-07 21:28:52.000000 rcmpy-1.4.0/tests/test_xdg.py
```

### Comparing `rcmpy-1.3.0/LICENSE` & `rcmpy-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rcmpy-1.3.0/PKG-INFO` & `rcmpy-1.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.3.0
+Version: 1.4.0
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=24348be5017ba83b48349d0ddd2389e4
+    hash=c1786731fe10b81b6b18afa242c53257
     =====================================
 -->
 
-# rcmpy ([1.3.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.4.0](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
@@ -139,29 +139,31 @@
 [top-level configuration file](md/data_repository.md#top-level-configuration).
 
 # Command-line Options
 
 ```
 $ ./venv3.11/bin/rcmpy -h
 
-usage: rcmpy [-h] [--version] [-v] [-C DIR] {apply,use,variant,watch,noop} ...
+usage: rcmpy [-h] [--version] [-v] [-C DIR]
+             {apply,dump,use,variant,watch,noop} ...
 
 A configuration-file management system.
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
   -C DIR, --dir DIR     execute from a specific directory
 
 commands:
-  {apply,use,variant,watch,noop}
+  {apply,dump,use,variant,watch,noop}
                         set of available commands
     apply               apply any pending changes from the active data
                         repository
+    dump                dump template data to stdout as JSON
     use                 set the directory to use as the rcmpy data repository
     variant             set the variant of configuration data to use
     watch               do a task whenever a file in a specified directory
                         changes
     noop                command stub (does nothing)
 
 ```
@@ -178,14 +180,26 @@
 options:
   -h, --help     show this help message and exit
   -f, --force    whether or not to forcibly render all outputs
   -d, --dry-run  whether or not to update output files
 
 ```
 
+### `dump`
+
+```
+$ ./venv3.11/bin/rcmpy dump -h
+
+usage: rcmpy dump [-h]
+
+options:
+  -h, --help  show this help message and exit
+
+```
+
 ### `use`
 
 ```
 $ ./venv3.11/bin/rcmpy use -h
 
 usage: rcmpy use [-h] [-d] [directory]
```

### Comparing `rcmpy-1.3.0/README.md` & `rcmpy-1.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=24348be5017ba83b48349d0ddd2389e4
+    hash=c1786731fe10b81b6b18afa242c53257
     =====================================
 -->
 
-# rcmpy ([1.3.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.4.0](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
@@ -115,29 +115,31 @@
 [top-level configuration file](md/data_repository.md#top-level-configuration).
 
 # Command-line Options
 
 ```
 $ ./venv3.11/bin/rcmpy -h
 
-usage: rcmpy [-h] [--version] [-v] [-C DIR] {apply,use,variant,watch,noop} ...
+usage: rcmpy [-h] [--version] [-v] [-C DIR]
+             {apply,dump,use,variant,watch,noop} ...
 
 A configuration-file management system.
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
   -C DIR, --dir DIR     execute from a specific directory
 
 commands:
-  {apply,use,variant,watch,noop}
+  {apply,dump,use,variant,watch,noop}
                         set of available commands
     apply               apply any pending changes from the active data
                         repository
+    dump                dump template data to stdout as JSON
     use                 set the directory to use as the rcmpy data repository
     variant             set the variant of configuration data to use
     watch               do a task whenever a file in a specified directory
                         changes
     noop                command stub (does nothing)
 
 ```
@@ -154,14 +156,26 @@
 options:
   -h, --help     show this help message and exit
   -f, --force    whether or not to forcibly render all outputs
   -d, --dry-run  whether or not to update output files
 
 ```
 
+### `dump`
+
+```
+$ ./venv3.11/bin/rcmpy dump -h
+
+usage: rcmpy dump [-h]
+
+options:
+  -h, --help  show this help message and exit
+
+```
+
 ### `use`
 
 ```
 $ ./venv3.11/bin/rcmpy use -h
 
 usage: rcmpy use [-h] [-d] [directory]
```

### Comparing `rcmpy-1.3.0/pyproject.toml` & `rcmpy-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "rcmpy"
-version = "1.3.0"
+version = "1.4.0"
 description = "A configuration-file management system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `rcmpy-1.3.0/rcmpy/app.py` & `rcmpy-1.4.0/rcmpy/app.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.3.0/rcmpy/commands/all.py` & `rcmpy-1.4.0/rcmpy/commands/all.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # =====================================
 # generator=datazen
 # version=3.1.2
-# hash=e990bc9fe3294af3d40349e7b0627ad4
+# hash=2b9927a9d538a17ed80c0411b8d02364
 # =====================================
 
 """
 A module aggregating package commands.
 """
 
 # built-in
@@ -13,14 +13,15 @@
 from typing import Tuple as _Tuple
 
 # third-party
 from vcorelib.args import CommandRegister as _CommandRegister
 
 # internal
 from rcmpy.commands.apply import add_apply_cmd
+from rcmpy.commands.dump import add_dump_cmd
 from rcmpy.commands.use import add_use_cmd
 from rcmpy.commands.variant import add_variant_cmd
 from rcmpy.commands.watch import add_watch_cmd
 
 
 def commands() -> _List[_Tuple[str, str, _CommandRegister]]:
     """Get this package's commands."""
@@ -28,14 +29,19 @@
     return [
         (
             "apply",
             "apply any pending changes from the active data repository",
             add_apply_cmd,
         ),
         (
+            "dump",
+            "dump template data to stdout as JSON",
+            add_dump_cmd,
+        ),
+        (
             "use",
             "set the directory to use as the rcmpy data repository",
             add_use_cmd,
         ),
         (
             "variant",
             "set the variant of configuration data to use",
```

### Comparing `rcmpy-1.3.0/rcmpy/commands/apply.py` & `rcmpy-1.4.0/rcmpy/commands/apply.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 An entry-point for the 'apply' command.
 """
 
 # built-in
 from argparse import ArgumentParser as _ArgumentParser
 from argparse import Namespace as _Namespace
-from logging import getLogger
 
 # third-party
 from vcorelib.args import CommandFunction as _CommandFunction
-from vcorelib.logging import log_time
 from vcorelib.paths import rel
 
 # internal
-from rcmpy.environment import Environment, load_environment
+from rcmpy.commands.common import run_env_command
+from rcmpy.environment import Environment
 
 
 def apply_env(args: _Namespace, env: Environment) -> int:
     """Apply pending changes from the environment."""
 
     result = 0
 
@@ -52,23 +51,15 @@
                 file.update(source, env.logger)
 
     return result
 
 
 def apply_cmd(args: _Namespace) -> int:
     """Execute the apply command."""
-
-    result = 1
-
-    with log_time(getLogger(__name__), "Command"):
-        with load_environment() as env:
-            if env.config_loaded:
-                result = apply_env(args, env)
-
-    return result
+    return run_env_command(args, apply_env)
 
 
 def add_apply_cmd(parser: _ArgumentParser) -> _CommandFunction:
     """Add apply-command arguments to its parser."""
 
     parser.add_argument(
         "-f",
```

### Comparing `rcmpy-1.3.0/rcmpy/commands/use.py` & `rcmpy-1.4.0/rcmpy/commands/use.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.3.0/rcmpy/commands/variant.py` & `rcmpy-1.4.0/rcmpy/commands/variant.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.3.0/rcmpy/commands/watch.py` & `rcmpy-1.4.0/rcmpy/commands/watch.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.3.0/rcmpy/config/__init__.py` & `rcmpy-1.4.0/rcmpy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.3.0/rcmpy/config/file.py` & `rcmpy-1.4.0/rcmpy/config/file.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.3.0/rcmpy/data/schemas/ManagedFile.yaml` & `rcmpy-1.4.0/rcmpy/data/schemas/ManagedFile.yaml`

 * *Files identical despite different names*

### Comparing `rcmpy-1.3.0/rcmpy/entry.py` & `rcmpy-1.4.0/rcmpy/entry.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.3.0/rcmpy/environment/__init__.py` & `rcmpy-1.4.0/rcmpy/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.3.0/rcmpy/environment/base.py` & `rcmpy-1.4.0/rcmpy/environment/base.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.3.0/rcmpy/environment/data.py` & `rcmpy-1.4.0/rcmpy/environment/data.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.3.0/rcmpy/environment/template.py` & `rcmpy-1.4.0/rcmpy/environment/template.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.3.0/rcmpy/paths/__init__.py` & `rcmpy-1.4.0/rcmpy/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.3.0/rcmpy/schemas.py` & `rcmpy-1.4.0/rcmpy/schemas.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.3.0/rcmpy/state/__init__.py` & `rcmpy-1.4.0/rcmpy/state/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.3.0/rcmpy/xdg/__init__.py` & `rcmpy-1.4.0/rcmpy/xdg/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.3.0/rcmpy.egg-info/PKG-INFO` & `rcmpy-1.4.0/rcmpy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.3.0
+Version: 1.4.0
 Summary: A configuration-file management system.
 Home-page: https://github.com/vkottler/rcmpy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=24348be5017ba83b48349d0ddd2389e4
+    hash=c1786731fe10b81b6b18afa242c53257
     =====================================
 -->
 
-# rcmpy ([1.3.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.4.0](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
@@ -139,29 +139,31 @@
 [top-level configuration file](md/data_repository.md#top-level-configuration).
 
 # Command-line Options
 
 ```
 $ ./venv3.11/bin/rcmpy -h
 
-usage: rcmpy [-h] [--version] [-v] [-C DIR] {apply,use,variant,watch,noop} ...
+usage: rcmpy [-h] [--version] [-v] [-C DIR]
+             {apply,dump,use,variant,watch,noop} ...
 
 A configuration-file management system.
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
   -C DIR, --dir DIR     execute from a specific directory
 
 commands:
-  {apply,use,variant,watch,noop}
+  {apply,dump,use,variant,watch,noop}
                         set of available commands
     apply               apply any pending changes from the active data
                         repository
+    dump                dump template data to stdout as JSON
     use                 set the directory to use as the rcmpy data repository
     variant             set the variant of configuration data to use
     watch               do a task whenever a file in a specified directory
                         changes
     noop                command stub (does nothing)
 
 ```
@@ -178,14 +180,26 @@
 options:
   -h, --help     show this help message and exit
   -f, --force    whether or not to forcibly render all outputs
   -d, --dry-run  whether or not to update output files
 
 ```
 
+### `dump`
+
+```
+$ ./venv3.11/bin/rcmpy dump -h
+
+usage: rcmpy dump [-h]
+
+options:
+  -h, --help  show this help message and exit
+
+```
+
 ### `use`
 
 ```
 $ ./venv3.11/bin/rcmpy use -h
 
 usage: rcmpy use [-h] [-d] [directory]
```

### Comparing `rcmpy-1.3.0/rcmpy.egg-info/SOURCES.txt` & `rcmpy-1.4.0/rcmpy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 rcmpy.egg-info/entry_points.txt
 rcmpy.egg-info/requires.txt
 rcmpy.egg-info/top_level.txt
 rcmpy/commands/__init__.py
 rcmpy/commands/all.py
 rcmpy/commands/apply.py
 rcmpy/commands/common.py
+rcmpy/commands/dump.py
 rcmpy/commands/use.py
 rcmpy/commands/variant.py
 rcmpy/commands/watch.py
 rcmpy/config/__init__.py
 rcmpy/config/file.py
 rcmpy/data/schemas/Config.yaml
 rcmpy/data/schemas/ManagedFile.yaml
```

### Comparing `rcmpy-1.3.0/setup.py` & `rcmpy-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.3.0/tests/test_entry.py` & `rcmpy-1.4.0/tests/test_entry.py`

 * *Files identical despite different names*

