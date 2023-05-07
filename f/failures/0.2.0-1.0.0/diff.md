# Comparing `tmp/failures-0.2.0.tar.gz` & `tmp/failures-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "failures-0.2.0.tar", last modified: Fri Apr 21 08:50:09 2023, max compression
+gzip compressed data, was "failures-1.0.0.tar", last modified: Sun May  7 10:15:49 2023, max compression
```

## Comparing `failures-0.2.0.tar` & `failures-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:50:09.235409 failures-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-21 08:49:49.000000 failures-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-21 08:50:09.235409 failures-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-04-21 08:49:49.000000 failures-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-21 08:49:49.000000 failures-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-21 08:49:49.000000 failures-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:50:09.235409 failures-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:50:09.231409 failures-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:50:09.235409 failures-0.2.0/src/failures/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-21 08:49:49.000000 failures-0.2.0/src/failures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-21 08:49:49.000000 failures-0.2.0/src/failures/_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-21 08:49:49.000000 failures-0.2.0/src/failures/_print.py
--rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-04-21 08:49:49.000000 failures-0.2.0/src/failures/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:50:09.235409 failures-0.2.0/src/failures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-21 08:50:09.000000 failures-0.2.0/src/failures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-21 08:50:09.000000 failures-0.2.0/src/failures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:50:09.000000 failures-0.2.0/src/failures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-21 08:50:09.000000 failures-0.2.0/src/failures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 08:50:09.000000 failures-0.2.0/src/failures.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:50:09.235409 failures-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-04-21 08:49:49.000000 failures-0.2.0/tests/test_handler_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-21 08:49:49.000000 failures-0.2.0/tests/test_print_failures.py
--rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-04-21 08:49:49.000000 failures-0.2.0/tests/test_scope_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-21 08:49:49.000000 failures-0.2.0/tests/test_scoped_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-21 08:49:49.000000 failures-0.2.0/tests/test_version_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:15:49.946576 failures-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-07 10:15:26.000000 failures-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9779 2023-05-07 10:15:49.946576 failures-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-05-07 10:15:26.000000 failures-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-07 10:15:26.000000 failures-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-07 10:15:26.000000 failures-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 10:15:49.946576 failures-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:15:49.942576 failures-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:15:49.946576 failures-1.0.0/src/failures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-07 10:15:26.000000 failures-1.0.0/src/failures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-05-07 10:15:26.000000 failures-1.0.0/src/failures/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-05-07 10:15:26.000000 failures-1.0.0/src/failures/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-05-07 10:15:26.000000 failures-1.0.0/src/failures/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:15:49.946576 failures-1.0.0/src/failures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9779 2023-05-07 10:15:49.000000 failures-1.0.0/src/failures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-07 10:15:49.000000 failures-1.0.0/src/failures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 10:15:49.000000 failures-1.0.0/src/failures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-07 10:15:49.000000 failures-1.0.0/src/failures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-07 10:15:49.000000 failures-1.0.0/src/failures.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:15:49.946576 failures-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-07 10:15:26.000000 failures-1.0.0/tests/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-07 10:15:26.000000 failures-1.0.0/tests/test_print_failures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-05-07 10:15:26.000000 failures-1.0.0/tests/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-05-07 10:15:26.000000 failures-1.0.0/tests/test_scoped_decorator.py
```

### Comparing `failures-0.2.0/LICENSE` & `failures-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `failures-0.2.0/pyproject.toml` & `failures-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "failures"
 dynamic = ["version", "dependencies"]
-description = "Labeling failures for humans"
+description = "Successfully dealing with failures"
 readme = "README.md"
 license = {text = "MIT License"}
 requires-python = ">=3.8"
 authors = [ {name = "MARSO Adnan", email = "mediadnan@gmail.com"} ]
 maintainers = [ {name = "MARSO Adnan", email = "mediadnan@gmail.com"} ]
 keywords = [ "label", "failures", "handle", "handling", "report", "track" ]
 classifiers = [
@@ -35,15 +35,17 @@
 packages = ["failures"]
 
 [tool.setuptools.dynamic]
 version = {attr = "failures.__version__"}
 dependencies = {file = "requirements.txt"}
 
 [project.optional-dependencies]
-colors = ["colorama>=0.4,<1.0"]
+colors = ["colorama>=0.4,<1.0", "types-colorama"]
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 filterwarnings = ['ignore:.*will be removed in failures \d.0.*:DeprecationWarning',]
+addopts = "--cov=failures --cov-report=html --cov-branch"
+testpaths = "tests/"
 
 [tool.mypy]
 implicit_optional = true
```

### Comparing `failures-0.2.0/src/failures/__init__.py` & `failures-1.0.0/src/failures/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-"""Failures package provides tools to label and track errors anywhere in your code easily"""
-from ._print import print_failure
-from .core import handler_ as handler, scope, scoped, FailureHandler, Failure
-from ._legacy import handle, SubScope   # deprecated API
+"""This library provides tools to label and handle errors anywhere in your code easily"""
+from .core import Reporter, Failure, FailureException
+from .functions import scoped
+from .handler import Handler, print_failure, Not
 
-
-# -------------------------------- WARNING --------------------------------- #
+# -------------------------------- WARNING! -------------------------------- #
 #                                                                            #
 #       Anything that starts with an _ or not explicitly imported here       #
 #       or mentioned anywhere in the documentation is considered             #
 #       internal API and implementation details                              #
 #       and could potentially change in minor/patch versions                 #
 #       USING PRIVATE MEMBERS MAY POTENTIALLY BREAK                          #
 #       YOUR APP IN ANY NEXT RELEASE,                                        #
 #       and the package does not commit to keep the                          #
 #       internal API compatibility for the next patch/minor version.         #
 #                                                                            #
 # -------------------------------------------------------------------------- #
 
-
-__version__ = '0.2.0'
+__version__ = '1.0.0'
```

