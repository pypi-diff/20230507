# Comparing `tmp/wheeldiff-2023.5.7.7.39.tar.gz` & `tmp/wheeldiff-2023.5.7.7.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheeldiff-2023.5.7.7.39.tar", last modified: Sun May  7 07:39:48 2023, max compression
+gzip compressed data, was "wheeldiff-2023.5.7.7.44.tar", last modified: Sun May  7 07:44:06 2023, max compression
```

## Comparing `wheeldiff-2023.5.7.7.39.tar` & `wheeldiff-2023.5.7.7.44.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:39:48.251313 wheeldiff-2023.5.7.7.39/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 07:39:34.000000 wheeldiff-2023.5.7.7.39/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-07 07:39:34.000000 wheeldiff-2023.5.7.7.39/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    46110 2023-05-07 07:39:48.251313 wheeldiff-2023.5.7.7.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-05-07 07:39:34.000000 wheeldiff-2023.5.7.7.39/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-07 07:39:34.000000 wheeldiff-2023.5.7.7.39/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 07:39:34.000000 wheeldiff-2023.5.7.7.39/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 07:39:48.251313 wheeldiff-2023.5.7.7.39/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:39:48.243313 wheeldiff-2023.5.7.7.39/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:39:48.247313 wheeldiff-2023.5.7.7.39/src/wheeldiff/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-07 07:39:47.000000 wheeldiff-2023.5.7.7.39/src/wheeldiff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:39:48.251313 wheeldiff-2023.5.7.7.39/src/wheeldiff/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 07:39:34.000000 wheeldiff-2023.5.7.7.39/src/wheeldiff/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-07 07:39:34.000000 wheeldiff-2023.5.7.7.39/src/wheeldiff/_impl/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:39:48.251313 wheeldiff-2023.5.7.7.39/src/wheeldiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46110 2023-05-07 07:39:48.000000 wheeldiff-2023.5.7.7.39/src/wheeldiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-07 07:39:48.000000 wheeldiff-2023.5.7.7.39/src/wheeldiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 07:39:48.000000 wheeldiff-2023.5.7.7.39/src/wheeldiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 07:39:48.000000 wheeldiff-2023.5.7.7.39/src/wheeldiff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 07:39:48.000000 wheeldiff-2023.5.7.7.39/src/wheeldiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 07:39:48.000000 wheeldiff-2023.5.7.7.39/src/wheeldiff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:39:48.251313 wheeldiff-2023.5.7.7.39/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-07 07:39:34.000000 wheeldiff-2023.5.7.7.39/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:44:06.540750 wheeldiff-2023.5.7.7.44/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 07:43:52.000000 wheeldiff-2023.5.7.7.44/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-07 07:43:52.000000 wheeldiff-2023.5.7.7.44/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    46110 2023-05-07 07:44:06.540750 wheeldiff-2023.5.7.7.44/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-05-07 07:43:52.000000 wheeldiff-2023.5.7.7.44/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-07 07:43:52.000000 wheeldiff-2023.5.7.7.44/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 07:43:52.000000 wheeldiff-2023.5.7.7.44/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 07:44:06.540750 wheeldiff-2023.5.7.7.44/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:44:06.536750 wheeldiff-2023.5.7.7.44/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:44:06.540750 wheeldiff-2023.5.7.7.44/src/wheeldiff/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-07 07:44:06.000000 wheeldiff-2023.5.7.7.44/src/wheeldiff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:44:06.540750 wheeldiff-2023.5.7.7.44/src/wheeldiff/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 07:43:52.000000 wheeldiff-2023.5.7.7.44/src/wheeldiff/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-07 07:43:52.000000 wheeldiff-2023.5.7.7.44/src/wheeldiff/_impl/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:44:06.540750 wheeldiff-2023.5.7.7.44/src/wheeldiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46110 2023-05-07 07:44:06.000000 wheeldiff-2023.5.7.7.44/src/wheeldiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-07 07:44:06.000000 wheeldiff-2023.5.7.7.44/src/wheeldiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 07:44:06.000000 wheeldiff-2023.5.7.7.44/src/wheeldiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 07:44:06.000000 wheeldiff-2023.5.7.7.44/src/wheeldiff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 07:44:06.000000 wheeldiff-2023.5.7.7.44/src/wheeldiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 07:44:06.000000 wheeldiff-2023.5.7.7.44/src/wheeldiff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:44:06.540750 wheeldiff-2023.5.7.7.44/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-07 07:43:52.000000 wheeldiff-2023.5.7.7.44/tests/test_import.py
```

### Comparing `wheeldiff-2023.5.7.7.39/LICENSE` & `wheeldiff-2023.5.7.7.44/LICENSE`

 * *Files identical despite different names*

### Comparing `wheeldiff-2023.5.7.7.39/PKG-INFO` & `wheeldiff-2023.5.7.7.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wheeldiff
-Version: 2023.5.7.7.39
+Version: 2023.5.7.7.44
 Summary: Diff two Python wheels
 Author-email: Rohan McGovern <rohan@mcgovern.id.au>
 Maintainer-email: Rohan McGovern <rohan@mcgovern.id.au>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `wheeldiff-2023.5.7.7.39/README.md` & `wheeldiff-2023.5.7.7.44/README.md`

 * *Files identical despite different names*

### Comparing `wheeldiff-2023.5.7.7.39/pyproject.toml` & `wheeldiff-2023.5.7.7.44/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wheeldiff-2023.5.7.7.39/src/wheeldiff/_impl/cmd.py` & `wheeldiff-2023.5.7.7.44/src/wheeldiff/_impl/cmd.py`

 * *Files identical despite different names*

### Comparing `wheeldiff-2023.5.7.7.39/src/wheeldiff.egg-info/PKG-INFO` & `wheeldiff-2023.5.7.7.44/src/wheeldiff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wheeldiff
-Version: 2023.5.7.7.39
+Version: 2023.5.7.7.44
 Summary: Diff two Python wheels
 Author-email: Rohan McGovern <rohan@mcgovern.id.au>
 Maintainer-email: Rohan McGovern <rohan@mcgovern.id.au>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

