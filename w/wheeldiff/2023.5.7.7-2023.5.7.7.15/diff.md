# Comparing `tmp/wheeldiff-2023.5.7.7.tar.gz` & `tmp/wheeldiff-2023.5.7.7.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheeldiff-2023.5.7.7.tar", last modified: Sun May  7 07:08:43 2023, max compression
+gzip compressed data, was "wheeldiff-2023.5.7.7.15.tar", last modified: Sun May  7 07:15:23 2023, max compression
```

## Comparing `wheeldiff-2023.5.7.7.tar` & `wheeldiff-2023.5.7.7.15.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:08:43.275512 wheeldiff-2023.5.7.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 07:08:31.000000 wheeldiff-2023.5.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-07 07:08:31.000000 wheeldiff-2023.5.7.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    46107 2023-05-07 07:08:43.275512 wheeldiff-2023.5.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-05-07 07:08:31.000000 wheeldiff-2023.5.7.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-07 07:08:31.000000 wheeldiff-2023.5.7.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 07:08:31.000000 wheeldiff-2023.5.7.7/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 07:08:43.275512 wheeldiff-2023.5.7.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:08:43.271512 wheeldiff-2023.5.7.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:08:43.275512 wheeldiff-2023.5.7.7/src/wheeldiff/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-07 07:08:43.000000 wheeldiff-2023.5.7.7/src/wheeldiff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:08:43.275512 wheeldiff-2023.5.7.7/src/wheeldiff/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 07:08:31.000000 wheeldiff-2023.5.7.7/src/wheeldiff/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-05-07 07:08:31.000000 wheeldiff-2023.5.7.7/src/wheeldiff/_impl/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:08:43.275512 wheeldiff-2023.5.7.7/src/wheeldiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46107 2023-05-07 07:08:43.000000 wheeldiff-2023.5.7.7/src/wheeldiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-07 07:08:43.000000 wheeldiff-2023.5.7.7/src/wheeldiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 07:08:43.000000 wheeldiff-2023.5.7.7/src/wheeldiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 07:08:43.000000 wheeldiff-2023.5.7.7/src/wheeldiff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 07:08:43.000000 wheeldiff-2023.5.7.7/src/wheeldiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 07:08:43.000000 wheeldiff-2023.5.7.7/src/wheeldiff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:08:43.275512 wheeldiff-2023.5.7.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-07 07:08:31.000000 wheeldiff-2023.5.7.7/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:15:23.529129 wheeldiff-2023.5.7.7.15/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 07:15:11.000000 wheeldiff-2023.5.7.7.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-07 07:15:11.000000 wheeldiff-2023.5.7.7.15/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    46110 2023-05-07 07:15:23.529129 wheeldiff-2023.5.7.7.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-05-07 07:15:11.000000 wheeldiff-2023.5.7.7.15/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-07 07:15:11.000000 wheeldiff-2023.5.7.7.15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 07:15:11.000000 wheeldiff-2023.5.7.7.15/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 07:15:23.529129 wheeldiff-2023.5.7.7.15/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:15:23.521129 wheeldiff-2023.5.7.7.15/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:15:23.525129 wheeldiff-2023.5.7.7.15/src/wheeldiff/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-07 07:15:23.000000 wheeldiff-2023.5.7.7.15/src/wheeldiff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:15:23.529129 wheeldiff-2023.5.7.7.15/src/wheeldiff/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 07:15:11.000000 wheeldiff-2023.5.7.7.15/src/wheeldiff/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-05-07 07:15:11.000000 wheeldiff-2023.5.7.7.15/src/wheeldiff/_impl/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:15:23.525129 wheeldiff-2023.5.7.7.15/src/wheeldiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46110 2023-05-07 07:15:23.000000 wheeldiff-2023.5.7.7.15/src/wheeldiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-07 07:15:23.000000 wheeldiff-2023.5.7.7.15/src/wheeldiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 07:15:23.000000 wheeldiff-2023.5.7.7.15/src/wheeldiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 07:15:23.000000 wheeldiff-2023.5.7.7.15/src/wheeldiff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 07:15:23.000000 wheeldiff-2023.5.7.7.15/src/wheeldiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 07:15:23.000000 wheeldiff-2023.5.7.7.15/src/wheeldiff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:15:23.529129 wheeldiff-2023.5.7.7.15/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-07 07:15:11.000000 wheeldiff-2023.5.7.7.15/tests/test_import.py
```

### Comparing `wheeldiff-2023.5.7.7/LICENSE` & `wheeldiff-2023.5.7.7.15/LICENSE`

 * *Files identical despite different names*

### Comparing `wheeldiff-2023.5.7.7/PKG-INFO` & `wheeldiff-2023.5.7.7.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wheeldiff
-Version: 2023.5.7.7
+Version: 2023.5.7.7.15
 Summary: Diff two Python wheels
 Author-email: Rohan McGovern <rohan@mcgovern.id.au>
 Maintainer-email: Rohan McGovern <rohan@mcgovern.id.au>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `wheeldiff-2023.5.7.7/README.md` & `wheeldiff-2023.5.7.7.15/README.md`

 * *Files identical despite different names*

### Comparing `wheeldiff-2023.5.7.7/pyproject.toml` & `wheeldiff-2023.5.7.7.15/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wheeldiff-2023.5.7.7/src/wheeldiff/_impl/cmd.py` & `wheeldiff-2023.5.7.7.15/src/wheeldiff/_impl/cmd.py`

 * *Files identical despite different names*

### Comparing `wheeldiff-2023.5.7.7/src/wheeldiff.egg-info/PKG-INFO` & `wheeldiff-2023.5.7.7.15/src/wheeldiff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wheeldiff
-Version: 2023.5.7.7
+Version: 2023.5.7.7.15
 Summary: Diff two Python wheels
 Author-email: Rohan McGovern <rohan@mcgovern.id.au>
 Maintainer-email: Rohan McGovern <rohan@mcgovern.id.au>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

