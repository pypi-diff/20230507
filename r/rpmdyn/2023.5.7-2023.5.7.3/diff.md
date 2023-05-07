# Comparing `tmp/rpmdyn-2023.5.7.tar.gz` & `tmp/rpmdyn-2023.5.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpmdyn-2023.5.7.tar", last modified: Sun May  7 01:28:01 2023, max compression
+gzip compressed data, was "rpmdyn-2023.5.7.3.tar", last modified: Sun May  7 03:03:42 2023, max compression
```

## Comparing `rpmdyn-2023.5.7.tar` & `rpmdyn-2023.5.7.3.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:28:01.533428 rpmdyn-2023.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    43843 2023-05-07 01:28:01.533428 rpmdyn-2023.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:28:01.533428 rpmdyn-2023.5.7/custom_build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:28:01.533428 rpmdyn-2023.5.7/custom_build/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-07 01:28:00.000000 rpmdyn-2023.5.7/custom_build/__pycache__/backend.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/custom_build/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 01:28:01.533428 rpmdyn-2023.5.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:28:01.529428 rpmdyn-2023.5.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:28:01.533428 rpmdyn-2023.5.7/src/rpmdyn/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-07 01:28:01.000000 rpmdyn-2023.5.7/src/rpmdyn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24226 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/src/rpmdyn/_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/src/rpmdyn/_ffi.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/src/rpmdyn/_keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/src/rpmdyn/_pth_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/src/rpmdyn/_rpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/src/rpmdyn/_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/src/rpmdyn/rpmdyn.pth
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:28:01.533428 rpmdyn-2023.5.7/src/rpmdyn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43843 2023-05-07 01:28:01.000000 rpmdyn-2023.5.7/src/rpmdyn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-07 01:28:01.000000 rpmdyn-2023.5.7/src/rpmdyn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 01:28:01.000000 rpmdyn-2023.5.7/src/rpmdyn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-07 01:28:01.000000 rpmdyn-2023.5.7/src/rpmdyn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 01:28:01.000000 rpmdyn-2023.5.7/src/rpmdyn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:28:01.533428 rpmdyn-2023.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/tests/test_labelcompare.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/tests/test_transactionset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:03:42.617071 rpmdyn-2023.5.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    43845 2023-05-07 03:03:42.617071 rpmdyn-2023.5.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:03:42.613070 rpmdyn-2023.5.7.3/custom_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/custom_build/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 03:03:42.621070 rpmdyn-2023.5.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:03:42.613070 rpmdyn-2023.5.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:03:42.617071 rpmdyn-2023.5.7.3/src/rpmdyn/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-07 03:03:42.000000 rpmdyn-2023.5.7.3/src/rpmdyn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24226 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/src/rpmdyn/_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/src/rpmdyn/_ffi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/src/rpmdyn/_keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/src/rpmdyn/_pth_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/src/rpmdyn/_rpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/src/rpmdyn/_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/src/rpmdyn/rpmdyn.pth
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:03:42.617071 rpmdyn-2023.5.7.3/src/rpmdyn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43845 2023-05-07 03:03:42.000000 rpmdyn-2023.5.7.3/src/rpmdyn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-07 03:03:42.000000 rpmdyn-2023.5.7.3/src/rpmdyn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 03:03:42.000000 rpmdyn-2023.5.7.3/src/rpmdyn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-07 03:03:42.000000 rpmdyn-2023.5.7.3/src/rpmdyn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 03:03:42.000000 rpmdyn-2023.5.7.3/src/rpmdyn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:03:42.617071 rpmdyn-2023.5.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:03:42.617071 rpmdyn-2023.5.7.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/tests/data/test-srpm01-1.0-1.src.rpm
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/tests/data/walrus-5.21-1.noarch.rpm
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/tests/test_labelcompare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-07 03:03:26.000000 rpmdyn-2023.5.7.3/tests/test_transactionset.py
```

### Comparing `rpmdyn-2023.5.7/LICENSE` & `rpmdyn-2023.5.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7/PKG-INFO` & `rpmdyn-2023.5.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpmdyn
-Version: 2023.5.7
+Version: 2023.5.7.3
 Summary: Alternative dynamic RPM bindings for Python
 Author-email: Rohan McGovern <rohan@mcgovern.id.au>
 Maintainer-email: Rohan McGovern <rohan@mcgovern.id.au>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `rpmdyn-2023.5.7/README.md` & `rpmdyn-2023.5.7.3/README.md`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7/custom_build/backend.py` & `rpmdyn-2023.5.7.3/custom_build/backend.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7/pyproject.toml` & `rpmdyn-2023.5.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7/src/rpmdyn/_const.py` & `rpmdyn-2023.5.7.3/src/rpmdyn/_const.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7/src/rpmdyn/_ffi.py` & `rpmdyn-2023.5.7.3/src/rpmdyn/_ffi.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7/src/rpmdyn/_pth_hook.py` & `rpmdyn-2023.5.7.3/src/rpmdyn/_pth_hook.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7/src/rpmdyn/_rpm.py` & `rpmdyn-2023.5.7.3/src/rpmdyn/_rpm.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7/src/rpmdyn/_transaction.py` & `rpmdyn-2023.5.7.3/src/rpmdyn/_transaction.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7/src/rpmdyn.egg-info/PKG-INFO` & `rpmdyn-2023.5.7.3/src/rpmdyn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpmdyn
-Version: 2023.5.7
+Version: 2023.5.7.3
 Summary: Alternative dynamic RPM bindings for Python
 Author-email: Rohan McGovern <rohan@mcgovern.id.au>
 Maintainer-email: Rohan McGovern <rohan@mcgovern.id.au>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `rpmdyn-2023.5.7/src/rpmdyn.egg-info/SOURCES.txt` & `rpmdyn-2023.5.7.3/src/rpmdyn.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.in
 custom_build/backend.py
-custom_build/__pycache__/backend.cpython-311.pyc
 src/rpmdyn/__init__.py
 src/rpmdyn/_const.py
 src/rpmdyn/_ffi.py
 src/rpmdyn/_keyring.py
 src/rpmdyn/_pth_hook.py
 src/rpmdyn/_rpm.py
 src/rpmdyn/_transaction.py
 src/rpmdyn/rpmdyn.pth
 src/rpmdyn.egg-info/PKG-INFO
 src/rpmdyn.egg-info/SOURCES.txt
 src/rpmdyn.egg-info/dependency_links.txt
 src/rpmdyn.egg-info/requires.txt
 src/rpmdyn.egg-info/top_level.txt
+tests/__init__.py
+tests/conftest.py
 tests/test_constants.py
 tests/test_headers.py
 tests/test_labelcompare.py
-tests/test_transactionset.py
+tests/test_transactionset.py
+tests/data/test-srpm01-1.0-1.src.rpm
+tests/data/walrus-5.21-1.noarch.rpm
```

### Comparing `rpmdyn-2023.5.7/tests/test_headers.py` & `rpmdyn-2023.5.7.3/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7/tests/test_labelcompare.py` & `rpmdyn-2023.5.7.3/tests/test_labelcompare.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5.7/tests/test_transactionset.py` & `rpmdyn-2023.5.7.3/tests/test_transactionset.py`

 * *Files identical despite different names*

