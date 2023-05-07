# Comparing `tmp/userfs-0.2.0.tar.gz` & `tmp/userfs-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "userfs-0.2.0.tar", last modified: Fri May  5 08:36:45 2023, max compression
+gzip compressed data, was "userfs-0.2.1.tar", last modified: Sun May  7 07:20:28 2023, max compression
```

## Comparing `userfs-0.2.0.tar` & `userfs-0.2.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-05 08:35:34.000000 userfs-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-05 08:36:45.198417 userfs-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-05 08:35:34.000000 userfs-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-05 08:35:34.000000 userfs-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:36:45.198417 userfs-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-05 08:35:34.000000 userfs-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.194416 userfs-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-05 08:35:34.000000 userfs-0.2.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-05 08:35:34.000000 userfs-0.2.0/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/build/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/commands/fetch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/config/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/config/source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/data/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/data/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/data/schemas/Config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/data/schemas/ProjectSpecification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/data/schemas/SourceSpecification.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/fetch/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/fetch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/project/
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/update/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/update/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-05 08:36:45.000000 userfs-0.2.0/userfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-05 08:36:45.000000 userfs-0.2.0/userfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:36:45.000000 userfs-0.2.0/userfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 08:36:45.000000 userfs-0.2.0/userfs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-05 08:36:45.000000 userfs-0.2.0/userfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 08:36:45.000000 userfs-0.2.0/userfs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-07 07:19:20.000000 userfs-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-07 07:20:28.651212 userfs-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-07 07:19:20.000000 userfs-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-07 07:19:20.000000 userfs-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 07:20:28.651212 userfs-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-07 07:19:20.000000 userfs-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.647212 userfs-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-07 07:19:20.000000 userfs-0.2.1/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-07 07:19:20.000000 userfs-0.2.1/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/commands/fetch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/config/source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/data/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/data/schemas/ProjectSpecification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/data/schemas/SourceSpecification.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/fetch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs/update/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-07 07:19:20.000000 userfs-0.2.1/userfs/update/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:20:28.651212 userfs-0.2.1/userfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-07 07:20:28.000000 userfs-0.2.1/userfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-07 07:20:28.000000 userfs-0.2.1/userfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 07:20:28.000000 userfs-0.2.1/userfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-07 07:20:28.000000 userfs-0.2.1/userfs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-07 07:20:28.000000 userfs-0.2.1/userfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 07:20:28.000000 userfs-0.2.1/userfs.egg-info/top_level.txt
```

### Comparing `userfs-0.2.0/LICENSE` & `userfs-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `userfs-0.2.0/PKG-INFO` & `userfs-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: userfs
-Version: 0.2.0
+Version: 0.2.1
 Summary: A system-bootstrapping automation and introspection tool.
 Home-page: https://github.com/vkottler/userfs
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
-    hash=035acc9a20df17a172151cf57e984c39
+    hash=b7e9bcf324a830a391ad3fdcbb3e044e
     =====================================
 -->
 
-# userfs ([0.2.0](https://pypi.org/project/userfs/))
+# userfs ([0.2.1](https://pypi.org/project/userfs/))
 
 [![python](https://img.shields.io/pypi/pyversions/userfs.svg)](https://pypi.org/project/userfs/)
 ![Build Status](https://github.com/vkottler/userfs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/userfs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/userfs)
 ![PyPI - Status](https://img.shields.io/pypi/status/userfs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/userfs)
```

### Comparing `userfs-0.2.0/README.md` & `userfs-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=035acc9a20df17a172151cf57e984c39
+    hash=b7e9bcf324a830a391ad3fdcbb3e044e
     =====================================
 -->
 
-# userfs ([0.2.0](https://pypi.org/project/userfs/))
+# userfs ([0.2.1](https://pypi.org/project/userfs/))
 
 [![python](https://img.shields.io/pypi/pyversions/userfs.svg)](https://pypi.org/project/userfs/)
 ![Build Status](https://github.com/vkottler/userfs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/userfs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/userfs)
 ![PyPI - Status](https://img.shields.io/pypi/status/userfs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/userfs)
```

### Comparing `userfs-0.2.0/pyproject.toml` & `userfs-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "userfs"
-version = "0.2.0"
+version = "0.2.1"
 description = "A system-bootstrapping automation and introspection tool."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `userfs-0.2.0/setup.py` & `userfs-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `userfs-0.2.0/tests/test_entry.py` & `userfs-0.2.1/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `userfs-0.2.0/userfs/app.py` & `userfs-0.2.1/userfs/app.py`

 * *Files identical despite different names*

### Comparing `userfs-0.2.0/userfs/commands/all.py` & `userfs-0.2.1/userfs/commands/all.py`

 * *Files identical despite different names*

### Comparing `userfs-0.2.0/userfs/commands/build.py` & `userfs-0.2.1/userfs/commands/build.py`

 * *Files identical despite different names*

### Comparing `userfs-0.2.0/userfs/commands/common.py` & `userfs-0.2.1/userfs/commands/common.py`

 * *Files identical despite different names*

### Comparing `userfs-0.2.0/userfs/commands/fetch.py` & `userfs-0.2.1/userfs/commands/fetch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 An entry-point for the 'fetch' command.
 """
 
 # built-in
 from argparse import ArgumentParser as _ArgumentParser
 from argparse import Namespace as _Namespace
+from os import environ
 
 # third-party
 from vcorelib.args import CommandFunction as _CommandFunction
 
 # internal
 from userfs.commands.common import add_common, run_command
 from userfs.config import ProjectInteraction
@@ -17,14 +18,15 @@
 def fetch_cmd(args: _Namespace) -> int:
     """Execute the fetch command."""
 
     interactions = [ProjectInteraction.FETCH]
     if args.update:
         interactions.append(ProjectInteraction.UPDATE)
 
+    environ["GIT_PYTHON_TRACE"] = "full"
     return run_command(interactions, args)
 
 
 def add_fetch_cmd(parser: _ArgumentParser) -> _CommandFunction:
     """Add fetch-command arguments to its parser."""
 
     add_common(parser)
```

### Comparing `userfs-0.2.0/userfs/config/__init__.py` & `userfs-0.2.1/userfs/config/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-0.2.0/userfs/config/project.py` & `userfs-0.2.1/userfs/config/project.py`

 * *Files identical despite different names*

### Comparing `userfs-0.2.0/userfs/config/source.py` & `userfs-0.2.1/userfs/config/source.py`

 * *Files identical despite different names*

### Comparing `userfs-0.2.0/userfs/data/schemas/ProjectSpecification.yaml` & `userfs-0.2.1/userfs/data/schemas/ProjectSpecification.yaml`

 * *Files identical despite different names*

### Comparing `userfs-0.2.0/userfs/entry.py` & `userfs-0.2.1/userfs/entry.py`

 * *Files identical despite different names*

### Comparing `userfs-0.2.0/userfs/fetch/__init__.py` & `userfs-0.2.1/userfs/update/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 """
-A module for fetching projects.
+A module for updating project sources.
 """
 
 # built-in
+from contextlib import suppress
 from pathlib import Path
 from typing import Any, Dict
 
 # third-party
 from git import Repo  # type: ignore
-from vcorelib.paths import rel
+from git.exc import GitCommandError
 
 # internal
-from userfs.config import ProjectSpecification, SourceKind
+from userfs.config import ProjectSpecification
 
 
-def fetch(
+def update(
     root: Path, project: ProjectSpecification, options: Dict[str, Any]
 ) -> None:
-    """Fetch an individual project."""
+    """Update an individual project."""
 
-    location = project.location(root=root)
+    repo = Repo(project.location(root=root))
 
-    if project.source.kind is SourceKind.GIT:
-        # Clone the repository.
-        if not location.is_dir():
-            url = project.url
-            Repo.clone_from(project.url, location, **options)
-            project.logger.info("Cloned from '%s' (%s).", url, options)
-
-    project.logger.info("Location: '%s'.", rel(location))
+    remote_name = options.get("remote", "origin")
+    if remote_name in repo.remotes:
+        remote = repo.remotes[remote_name]
+        with suppress(GitCommandError):
+            remote.pull()
```

### Comparing `userfs-0.2.0/userfs/project/__init__.py` & `userfs-0.2.1/userfs/project/__init__.py`

 * *Files identical despite different names*

### Comparing `userfs-0.2.0/userfs/schemas.py` & `userfs-0.2.1/userfs/schemas.py`

 * *Files identical despite different names*

### Comparing `userfs-0.2.0/userfs.egg-info/PKG-INFO` & `userfs-0.2.1/userfs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: userfs
-Version: 0.2.0
+Version: 0.2.1
 Summary: A system-bootstrapping automation and introspection tool.
 Home-page: https://github.com/vkottler/userfs
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
-    hash=035acc9a20df17a172151cf57e984c39
+    hash=b7e9bcf324a830a391ad3fdcbb3e044e
     =====================================
 -->
 
-# userfs ([0.2.0](https://pypi.org/project/userfs/))
+# userfs ([0.2.1](https://pypi.org/project/userfs/))
 
 [![python](https://img.shields.io/pypi/pyversions/userfs.svg)](https://pypi.org/project/userfs/)
 ![Build Status](https://github.com/vkottler/userfs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/userfs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/userfs)
 ![PyPI - Status](https://img.shields.io/pypi/status/userfs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/userfs)
```

### Comparing `userfs-0.2.0/userfs.egg-info/SOURCES.txt` & `userfs-0.2.1/userfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

