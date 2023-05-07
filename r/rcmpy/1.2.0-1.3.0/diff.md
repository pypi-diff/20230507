# Comparing `tmp/rcmpy-1.2.0.tar.gz` & `tmp/rcmpy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcmpy-1.2.0.tar", last modified: Sat Apr 22 17:18:35 2023, max compression
+gzip compressed data, was "rcmpy-1.3.0.tar", last modified: Sun May  7 03:23:41 2023, max compression
```

## Comparing `rcmpy-1.2.0.tar` & `rcmpy-1.3.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-22 17:17:28.000000 rcmpy-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-22 17:18:35.164189 rcmpy-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-04-22 17:17:28.000000 rcmpy-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-22 17:17:28.000000 rcmpy-1.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.160189 rcmpy-1.2.0/rcmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/rcmpy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/commands/apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/commands/use.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/commands/variant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/commands/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/rcmpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/config/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.160189 rcmpy-1.2.0/rcmpy/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/rcmpy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/data/schemas/ManagedFile.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/data/schemas/State.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/rcmpy/environment/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/environment/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/environment/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/rcmpy/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/rcmpy/state/
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/rcmpy/xdg/
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-22 17:17:28.000000 rcmpy-1.2.0/rcmpy/xdg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/rcmpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-04-22 17:18:35.000000 rcmpy-1.2.0/rcmpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-22 17:18:35.000000 rcmpy-1.2.0/rcmpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 17:18:35.000000 rcmpy-1.2.0/rcmpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-22 17:18:35.000000 rcmpy-1.2.0/rcmpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-22 17:18:35.000000 rcmpy-1.2.0/rcmpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-22 17:18:35.000000 rcmpy-1.2.0/rcmpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 17:18:35.164189 rcmpy-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-22 17:17:28.000000 rcmpy-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 17:18:35.164189 rcmpy-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-22 17:17:28.000000 rcmpy-1.2.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-22 17:17:28.000000 rcmpy-1.2.0/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-22 17:17:28.000000 rcmpy-1.2.0/tests/test_xdg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-07 03:22:34.000000 rcmpy-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-05-07 03:23:41.245388 rcmpy-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-05-07 03:22:34.000000 rcmpy-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-07 03:22:34.000000 rcmpy-1.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.241388 rcmpy-1.3.0/rcmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/rcmpy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/commands/apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/commands/use.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/commands/variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/commands/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/rcmpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/config/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.241388 rcmpy-1.3.0/rcmpy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/rcmpy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/data/schemas/ManagedFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/data/schemas/State.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/rcmpy/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/environment/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/environment/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/environment/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/rcmpy/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/rcmpy/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/rcmpy/xdg/
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-07 03:22:34.000000 rcmpy-1.3.0/rcmpy/xdg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/rcmpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-05-07 03:23:41.000000 rcmpy-1.3.0/rcmpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-07 03:23:41.000000 rcmpy-1.3.0/rcmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 03:23:41.000000 rcmpy-1.3.0/rcmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-07 03:23:41.000000 rcmpy-1.3.0/rcmpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-07 03:23:41.000000 rcmpy-1.3.0/rcmpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 03:23:41.000000 rcmpy-1.3.0/rcmpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 03:23:41.245388 rcmpy-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-07 03:22:34.000000 rcmpy-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:23:41.245388 rcmpy-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-07 03:22:34.000000 rcmpy-1.3.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-07 03:22:34.000000 rcmpy-1.3.0/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-07 03:22:34.000000 rcmpy-1.3.0/tests/test_xdg.py
```

### Comparing `rcmpy-1.2.0/LICENSE` & `rcmpy-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rcmpy-1.2.0/PKG-INFO` & `rcmpy-1.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.2.0
+Version: 1.3.0
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
-    hash=a4e47be8738ab981e11e2267b94bc9fc
+    hash=24348be5017ba83b48349d0ddd2389e4
     =====================================
 -->
 
-# rcmpy ([1.2.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.3.0](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
@@ -137,21 +137,21 @@
    an existing one at any arbitrary location.
 5. Run `rcmpy apply` to perform tasks specified in the
 [top-level configuration file](md/data_repository.md#top-level-configuration).
 
 # Command-line Options
 
 ```
-$ ./venv3.8/bin/rcmpy -h
+$ ./venv3.11/bin/rcmpy -h
 
 usage: rcmpy [-h] [--version] [-v] [-C DIR] {apply,use,variant,watch,noop} ...
 
 A configuration-file management system.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
   -C DIR, --dir DIR     execute from a specific directory
 
 commands:
   {apply,use,variant,watch,noop}
@@ -167,69 +167,69 @@
 ```
 
 ## Sub-command Options
 
 ### `apply`
 
 ```
-$ ./venv3.8/bin/rcmpy apply -h
+$ ./venv3.11/bin/rcmpy apply -h
 
 usage: rcmpy apply [-h] [-f] [-d]
 
-optional arguments:
+options:
   -h, --help     show this help message and exit
   -f, --force    whether or not to forcibly render all outputs
   -d, --dry-run  whether or not to update output files
 
 ```
 
 ### `use`
 
 ```
-$ ./venv3.8/bin/rcmpy use -h
+$ ./venv3.11/bin/rcmpy use -h
 
 usage: rcmpy use [-h] [-d] [directory]
 
 positional arguments:
   directory      the directory to use
 
-optional arguments:
+options:
   -h, --help     show this help message and exit
   -d, --default  sets the directory back to the package default
 
 ```
 
 ### `variant`
 
 ```
-$ ./venv3.8/bin/rcmpy variant -h
+$ ./venv3.11/bin/rcmpy variant -h
 
 usage: rcmpy variant [-h] [-d] [variant]
 
 positional arguments:
   variant        new variant to use
 
-optional arguments:
+options:
   -h, --help     show this help message and exit
   -d, --default  sets the directory back to the package default
 
 ```
 
 ### `watch`
 
 ```
-$ ./venv3.8/bin/rcmpy watch -h
+$ ./venv3.11/bin/rcmpy watch -h
 
 usage: rcmpy watch [-h] [-p POLL_RATE] [-s] [-i] directory cmd [cmd ...]
 
 positional arguments:
   directory             directory to watch for file changes
   cmd                   command to run
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -p POLL_RATE, --poll-rate POLL_RATE
                         poll period in seconds (default: 0.1s)
   -s, --shell           set to run a shell command
   -i, --single-pass     only run a single iteration
 
 ```
```

### Comparing `rcmpy-1.2.0/README.md` & `rcmpy-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=a4e47be8738ab981e11e2267b94bc9fc
+    hash=24348be5017ba83b48349d0ddd2389e4
     =====================================
 -->
 
-# rcmpy ([1.2.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.3.0](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
@@ -113,21 +113,21 @@
    an existing one at any arbitrary location.
 5. Run `rcmpy apply` to perform tasks specified in the
 [top-level configuration file](md/data_repository.md#top-level-configuration).
 
 # Command-line Options
 
 ```
-$ ./venv3.8/bin/rcmpy -h
+$ ./venv3.11/bin/rcmpy -h
 
 usage: rcmpy [-h] [--version] [-v] [-C DIR] {apply,use,variant,watch,noop} ...
 
 A configuration-file management system.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
   -C DIR, --dir DIR     execute from a specific directory
 
 commands:
   {apply,use,variant,watch,noop}
@@ -143,69 +143,69 @@
 ```
 
 ## Sub-command Options
 
 ### `apply`
 
 ```
-$ ./venv3.8/bin/rcmpy apply -h
+$ ./venv3.11/bin/rcmpy apply -h
 
 usage: rcmpy apply [-h] [-f] [-d]
 
-optional arguments:
+options:
   -h, --help     show this help message and exit
   -f, --force    whether or not to forcibly render all outputs
   -d, --dry-run  whether or not to update output files
 
 ```
 
 ### `use`
 
 ```
-$ ./venv3.8/bin/rcmpy use -h
+$ ./venv3.11/bin/rcmpy use -h
 
 usage: rcmpy use [-h] [-d] [directory]
 
 positional arguments:
   directory      the directory to use
 
-optional arguments:
+options:
   -h, --help     show this help message and exit
   -d, --default  sets the directory back to the package default
 
 ```
 
 ### `variant`
 
 ```
-$ ./venv3.8/bin/rcmpy variant -h
+$ ./venv3.11/bin/rcmpy variant -h
 
 usage: rcmpy variant [-h] [-d] [variant]
 
 positional arguments:
   variant        new variant to use
 
-optional arguments:
+options:
   -h, --help     show this help message and exit
   -d, --default  sets the directory back to the package default
 
 ```
 
 ### `watch`
 
 ```
-$ ./venv3.8/bin/rcmpy watch -h
+$ ./venv3.11/bin/rcmpy watch -h
 
 usage: rcmpy watch [-h] [-p POLL_RATE] [-s] [-i] directory cmd [cmd ...]
 
 positional arguments:
   directory             directory to watch for file changes
   cmd                   command to run
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -p POLL_RATE, --poll-rate POLL_RATE
                         poll period in seconds (default: 0.1s)
   -s, --shell           set to run a shell command
   -i, --single-pass     only run a single iteration
 
 ```
```

### Comparing `rcmpy-1.2.0/pyproject.toml` & `rcmpy-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "rcmpy"
-version = "1.2.0"
+version = "1.3.0"
 description = "A configuration-file management system."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `rcmpy-1.2.0/rcmpy/app.py` & `rcmpy-1.3.0/rcmpy/app.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.2.0/rcmpy/commands/all.py` & `rcmpy-1.3.0/rcmpy/commands/all.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.2.0/rcmpy/commands/apply.py` & `rcmpy-1.3.0/rcmpy/commands/apply.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,38 +17,38 @@
 
 
 def apply_env(args: _Namespace, env: Environment) -> int:
     """Apply pending changes from the environment."""
 
     result = 0
 
+    is_new = env.state.is_new()
+
     for file in env.config.files:
         # Check if a template is found for this file.
         if file.template not in env.templates_by_name:
             result += 1
             env.logger.error("Template '%s' not found!", file.template)
             continue
 
-        if not file.platform:
+        if not file.evaluate(env.env_data):
             continue
 
-        is_new = env.state.is_new()
-
         # Check if this file has any updated templates.
-        if args.force or is_new or env.is_updated(file):
+        if args.force or is_new or not file.present or env.is_updated(file):
             template = env.templates_by_name[file.template]
 
             # If a template doesn't require rendering, use it as-is.
             source = template.path
 
             if template.template is not None:
                 # Render the template to the build directory.
                 source = env.build.joinpath(file.template)
                 with source.open("w") as path_fd:
-                    path_fd.write(template.template.render(env.state.configs))
+                    path_fd.write(template.template.render(env.template_data))
                     env.logger.info("Rendered '%s'.", rel(source))
 
             # Update the output file.
             if not args.dry_run:
                 file.update(source, env.logger)
 
     return result
```

### Comparing `rcmpy-1.2.0/rcmpy/commands/use.py` & `rcmpy-1.3.0/rcmpy/commands/use.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.2.0/rcmpy/commands/variant.py` & `rcmpy-1.3.0/rcmpy/commands/variant.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.2.0/rcmpy/commands/watch.py` & `rcmpy-1.3.0/rcmpy/commands/watch.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.2.0/rcmpy/config/__init__.py` & `rcmpy-1.3.0/rcmpy/config/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,20 +41,18 @@
             new = ManagedFile(
                 file["template"],
                 set(file.get("extra_templates", [])),
                 # Resolve environment variables and any '~' here.
                 Path(expandvars(file["directory"])).expanduser(),
                 file.get("name", file["template"]),
                 file["link"],
+                file["executable"],
+                file["condition"],
                 set(file.get("platforms", [])),
             )
 
             # Keep track of all templates used in any file.
             self.templates.add(new.template)
             for template in new.extra_templates:
                 self.templates.add(template)
 
             self.files.append(new)
-
-    def asdict(self) -> _JsonObject:
-        """Obtain a dictionary representing this instance."""
-        return self.data
```

### Comparing `rcmpy-1.2.0/rcmpy/config/file.py` & `rcmpy-1.3.0/rcmpy/config/file.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,47 +4,67 @@
 
 # built-in
 from contextlib import suppress
 from dataclasses import dataclass
 from pathlib import Path
 from shutil import copyfile
 import sys
-from typing import Set
+from typing import Any, Dict, Set
 
 # third-party
 from vcorelib.logging import LoggerType
 from vcorelib.paths import rel
 
 
+def set_exec_flags(path: Path) -> None:
+    """Set the executable bits, but respect the 'read' bits."""
+    mode = path.stat().st_mode
+    path.chmod(mode | ((mode & 0o444) >> 2))
+
+
 @dataclass
 class ManagedFile:
     """
     A data structure for managed files specified in the configuration data.
     """
 
     template: str
     extra_templates: Set[str]
 
     directory: Path
     name: str
 
     link: bool
+    executable: bool
+
+    condition: str
 
     platforms: Set[str]
 
     @property
     def output(self) -> Path:
         """Get the full output path."""
         return self.directory.joinpath(self.name)
 
     @property
+    def present(self) -> bool:
+        """Determine if this file is currently present in the file system."""
+        return self.output.is_file()
+
+    @property
     def platform(self) -> bool:
         """Determine if the platform is correct for handling this file."""
         return not self.platforms or sys.platform in self.platforms
 
+    def evaluate(self, env: Dict[str, Any]) -> bool:
+        """Determine if this file should be handled."""
+        return self.platform and eval(  # pylint: disable=eval-used
+            self.condition, None, env
+        )
+
     def update_root(self, root: Path) -> None:
         """
         If the output directory is a relative path, update it to be an
         absolute one based on the provided root directory.
         """
 
         if not self.directory.is_absolute():
@@ -64,8 +84,11 @@
         self.directory.mkdir(parents=True, exist_ok=True)
 
         if self.link:
             output.symlink_to(source)
         else:
             copyfile(source, output)
 
+        if self.executable:
+            set_exec_flags(output)
+
         logger.info("'%s' -> '%s'.", rel(source), rel(output))
```

### Comparing `rcmpy-1.2.0/rcmpy/data/schemas/ManagedFile.yaml` & `rcmpy-1.3.0/rcmpy/data/schemas/ManagedFile.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -13,17 +13,28 @@
     default: rcmpy-out
 
   # Whether or not to create a symbolic link instead of a copy.
   link:
     type: boolean
     default: true
 
+  # Whether or not the file should be executable.
+  executable:
+    type: boolean
+    default: false
+
   name:
     type: string
 
+  # A string that will be evaluated for True/False and provided environment
+  # data.
+  condition:
+    type: string
+    default: "True"
+
   platforms:
     type: array
     items:
       type: string
       enum: ["linux", "cygwin", "darwin", "win32"]
 
   # Templates that may be included in the main template.
```

### Comparing `rcmpy-1.2.0/rcmpy/entry.py` & `rcmpy-1.3.0/rcmpy/entry.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.2.0/rcmpy/environment/__init__.py` & `rcmpy-1.3.0/rcmpy/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.2.0/rcmpy/environment/base.py` & `rcmpy-1.3.0/rcmpy/environment/base.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.2.0/rcmpy/environment/template.py` & `rcmpy-1.3.0/rcmpy/environment/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 An environment extension for working with template files.
 """
 
 # built-in
+from copy import copy
 from pathlib import Path
 from typing import Dict, NamedTuple, Optional, Set, Tuple
 
 # third-party
 from datazen.templates import environment
 from jinja2 import Environment, FileSystemLoader, Template
 from vcorelib.paths.info import FileChangeEvent
 from vcorelib.paths.info_cache import FileChanged, file_info_cache
 
 # internal
 from rcmpy.config import ManagedFile
 from rcmpy.environment.base import BaseEnvironment
+from rcmpy.environment.data import system_data
 
 
 class EnvTemplate(NamedTuple):
     """
     A data structure for keeping track of environment templates. If 'template'
     is None, it signals that the template does not require rendering.
     """
@@ -167,8 +169,14 @@
         # attribute set here to detect this).
         assert not hasattr(self, "jinja")
 
         # Templates that are newly updated on this iteration.
         self.updated_templates: Set[Path] = set()
         self.updated_template_names: Set[str] = set()
 
+        # Add additional information to template data.
+        self.env_data = system_data()
+        self.template_data = copy(self.state.configs)
+        assert "env" not in self.template_data
+        self.template_data["env"] = self.env_data
+
         return result and self._init_templates(self.config.templates)
```

### Comparing `rcmpy-1.2.0/rcmpy/paths/__init__.py` & `rcmpy-1.3.0/rcmpy/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.2.0/rcmpy/schemas.py` & `rcmpy-1.3.0/rcmpy/schemas.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.2.0/rcmpy/state/__init__.py` & `rcmpy-1.3.0/rcmpy/state/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
         self.variant: str = cast(str, data["variant"])
         if self.variant:
             self.logger.info("Using variant '%s'.", self.variant)
 
         data.setdefault("previous", {})
         self.previous: Dict[str, Any] = data["previous"]  # type: ignore
+        self.previous.setdefault("variant", "default")
 
         # Variables.
         self.variables: Dict[str, Any] = {}
         self.variables_new = False
         self.previous.setdefault("variables", {})
         self._load_variables()
```

### Comparing `rcmpy-1.2.0/rcmpy/xdg/__init__.py` & `rcmpy-1.3.0/rcmpy/xdg/__init__.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.2.0/rcmpy.egg-info/PKG-INFO` & `rcmpy-1.3.0/rcmpy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcmpy
-Version: 1.2.0
+Version: 1.3.0
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
-    hash=a4e47be8738ab981e11e2267b94bc9fc
+    hash=24348be5017ba83b48349d0ddd2389e4
     =====================================
 -->
 
-# rcmpy ([1.2.0](https://pypi.org/project/rcmpy/))
+# rcmpy ([1.3.0](https://pypi.org/project/rcmpy/))
 
 [![python](https://img.shields.io/pypi/pyversions/rcmpy.svg)](https://pypi.org/project/rcmpy/)
 ![Build Status](https://github.com/vkottler/rcmpy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/rcmpy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/rcmpy)
 ![PyPI - Status](https://img.shields.io/pypi/status/rcmpy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/rcmpy)
 
@@ -137,21 +137,21 @@
    an existing one at any arbitrary location.
 5. Run `rcmpy apply` to perform tasks specified in the
 [top-level configuration file](md/data_repository.md#top-level-configuration).
 
 # Command-line Options
 
 ```
-$ ./venv3.8/bin/rcmpy -h
+$ ./venv3.11/bin/rcmpy -h
 
 usage: rcmpy [-h] [--version] [-v] [-C DIR] {apply,use,variant,watch,noop} ...
 
 A configuration-file management system.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
   -v, --verbose         set to increase logging verbosity
   -C DIR, --dir DIR     execute from a specific directory
 
 commands:
   {apply,use,variant,watch,noop}
@@ -167,69 +167,69 @@
 ```
 
 ## Sub-command Options
 
 ### `apply`
 
 ```
-$ ./venv3.8/bin/rcmpy apply -h
+$ ./venv3.11/bin/rcmpy apply -h
 
 usage: rcmpy apply [-h] [-f] [-d]
 
-optional arguments:
+options:
   -h, --help     show this help message and exit
   -f, --force    whether or not to forcibly render all outputs
   -d, --dry-run  whether or not to update output files
 
 ```
 
 ### `use`
 
 ```
-$ ./venv3.8/bin/rcmpy use -h
+$ ./venv3.11/bin/rcmpy use -h
 
 usage: rcmpy use [-h] [-d] [directory]
 
 positional arguments:
   directory      the directory to use
 
-optional arguments:
+options:
   -h, --help     show this help message and exit
   -d, --default  sets the directory back to the package default
 
 ```
 
 ### `variant`
 
 ```
-$ ./venv3.8/bin/rcmpy variant -h
+$ ./venv3.11/bin/rcmpy variant -h
 
 usage: rcmpy variant [-h] [-d] [variant]
 
 positional arguments:
   variant        new variant to use
 
-optional arguments:
+options:
   -h, --help     show this help message and exit
   -d, --default  sets the directory back to the package default
 
 ```
 
 ### `watch`
 
 ```
-$ ./venv3.8/bin/rcmpy watch -h
+$ ./venv3.11/bin/rcmpy watch -h
 
 usage: rcmpy watch [-h] [-p POLL_RATE] [-s] [-i] directory cmd [cmd ...]
 
 positional arguments:
   directory             directory to watch for file changes
   cmd                   command to run
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -p POLL_RATE, --poll-rate POLL_RATE
                         poll period in seconds (default: 0.1s)
   -s, --shell           set to run a shell command
   -i, --single-pass     only run a single iteration
 
 ```
```

### Comparing `rcmpy-1.2.0/rcmpy.egg-info/SOURCES.txt` & `rcmpy-1.3.0/rcmpy.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 rcmpy/config/__init__.py
 rcmpy/config/file.py
 rcmpy/data/schemas/Config.yaml
 rcmpy/data/schemas/ManagedFile.yaml
 rcmpy/data/schemas/State.yaml
 rcmpy/environment/__init__.py
 rcmpy/environment/base.py
+rcmpy/environment/data.py
 rcmpy/environment/template.py
 rcmpy/paths/__init__.py
 rcmpy/state/__init__.py
 rcmpy/xdg/__init__.py
 tests/test_entry.py
 tests/test_resources.py
 tests/test_xdg.py
```

### Comparing `rcmpy-1.2.0/setup.py` & `rcmpy-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `rcmpy-1.2.0/tests/test_entry.py` & `rcmpy-1.3.0/tests/test_entry.py`

 * *Files identical despite different names*

