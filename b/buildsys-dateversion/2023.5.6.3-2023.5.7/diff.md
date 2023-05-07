# Comparing `tmp/buildsys-dateversion-2023.5.6.3.tar.gz` & `tmp/buildsys-dateversion-2023.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildsys-dateversion-2023.5.6.3.tar", last modified: Sat May  6 03:30:50 2023, max compression
+gzip compressed data, was "buildsys-dateversion-2023.5.7.tar", last modified: Sun May  7 03:07:06 2023, max compression
```

## Comparing `buildsys-dateversion-2023.5.6.3.tar` & `buildsys-dateversion-2023.5.7.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:50.134740 buildsys-dateversion-2023.5.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-06 03:30:38.000000 buildsys-dateversion-2023.5.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-06 03:30:38.000000 buildsys-dateversion-2023.5.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    46507 2023-05-06 03:30:50.134740 buildsys-dateversion-2023.5.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-05-06 03:30:38.000000 buildsys-dateversion-2023.5.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-06 03:30:38.000000 buildsys-dateversion-2023.5.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-06 03:30:38.000000 buildsys-dateversion-2023.5.6.3/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 03:30:50.134740 buildsys-dateversion-2023.5.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:50.134740 buildsys-dateversion-2023.5.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:50.134740 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-06 03:30:49.000000 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:50.134740 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-06 03:30:47.000000 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-05-06 03:30:47.000000 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion/__pycache__/_hooks.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-05-06 03:30:38.000000 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion/_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:50.134740 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46507 2023-05-06 03:30:50.000000 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-06 03:30:50.000000 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 03:30:50.000000 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 03:30:50.000000 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-06 03:30:50.000000 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:50.134740 buildsys-dateversion-2023.5.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-06 03:30:38.000000 buildsys-dateversion-2023.5.6.3/tests/test_sample_projects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:07:06.009730 buildsys-dateversion-2023.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 03:06:50.000000 buildsys-dateversion-2023.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-07 03:06:50.000000 buildsys-dateversion-2023.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    46505 2023-05-07 03:07:06.009730 buildsys-dateversion-2023.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-05-07 03:06:50.000000 buildsys-dateversion-2023.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-07 03:06:50.000000 buildsys-dateversion-2023.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-07 03:06:50.000000 buildsys-dateversion-2023.5.7/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 03:07:06.009730 buildsys-dateversion-2023.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:07:06.005730 buildsys-dateversion-2023.5.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:07:06.005730 buildsys-dateversion-2023.5.7/src/buildsys_dateversion/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-07 03:07:05.000000 buildsys-dateversion-2023.5.7/src/buildsys_dateversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-05-07 03:06:50.000000 buildsys-dateversion-2023.5.7/src/buildsys_dateversion/_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:07:06.005730 buildsys-dateversion-2023.5.7/src/buildsys_dateversion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46505 2023-05-07 03:07:05.000000 buildsys-dateversion-2023.5.7/src/buildsys_dateversion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-07 03:07:06.000000 buildsys-dateversion-2023.5.7/src/buildsys_dateversion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 03:07:05.000000 buildsys-dateversion-2023.5.7/src/buildsys_dateversion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-07 03:07:05.000000 buildsys-dateversion-2023.5.7/src/buildsys_dateversion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 03:07:05.000000 buildsys-dateversion-2023.5.7/src/buildsys_dateversion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:07:06.005730 buildsys-dateversion-2023.5.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:07:06.005730 buildsys-dateversion-2023.5.7/tests/sample_projects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:07:06.005730 buildsys-dateversion-2023.5.7/tests/sample_projects/sample_flit3/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-07 03:06:50.000000 buildsys-dateversion-2023.5.7/tests/sample_projects/sample_flit3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:07:06.005730 buildsys-dateversion-2023.5.7/tests/sample_projects/sample_flit3/sample_flit3/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-07 03:06:50.000000 buildsys-dateversion-2023.5.7/tests/sample_projects/sample_flit3/sample_flit3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:07:06.005730 buildsys-dateversion-2023.5.7/tests/sample_projects/sample_setuptools/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-07 03:06:50.000000 buildsys-dateversion-2023.5.7/tests/sample_projects/sample_setuptools/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:07:06.009730 buildsys-dateversion-2023.5.7/tests/sample_projects/sample_setuptools/sample_setuptools/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-07 03:06:50.000000 buildsys-dateversion-2023.5.7/tests/sample_projects/sample_setuptools/sample_setuptools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-07 03:06:50.000000 buildsys-dateversion-2023.5.7/tests/test_sample_projects.py
```

### Comparing `buildsys-dateversion-2023.5.6.3/LICENSE` & `buildsys-dateversion-2023.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `buildsys-dateversion-2023.5.6.3/PKG-INFO` & `buildsys-dateversion-2023.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildsys-dateversion
-Version: 2023.5.6.3
+Version: 2023.5.7
 Summary: Easy date-based versioning for Python projects
 Author-email: Rohan McGovern <rohan@mcgovern.id.au>
 Maintainer-email: Rohan McGovern <rohan@mcgovern.id.au>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `buildsys-dateversion-2023.5.6.3/README.md` & `buildsys-dateversion-2023.5.7/README.md`

 * *Files identical despite different names*

### Comparing `buildsys-dateversion-2023.5.6.3/pyproject.toml` & `buildsys-dateversion-2023.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion/_hooks.py` & `buildsys-dateversion-2023.5.7/src/buildsys_dateversion/_hooks.py`

 * *Files identical despite different names*

### Comparing `buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion.egg-info/PKG-INFO` & `buildsys-dateversion-2023.5.7/src/buildsys_dateversion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildsys-dateversion
-Version: 2023.5.6.3
+Version: 2023.5.7
 Summary: Easy date-based versioning for Python projects
 Author-email: Rohan McGovern <rohan@mcgovern.id.au>
 Maintainer-email: Rohan McGovern <rohan@mcgovern.id.au>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `buildsys-dateversion-2023.5.6.3/tests/test_sample_projects.py` & `buildsys-dateversion-2023.5.7/tests/test_sample_projects.py`

 * *Files identical despite different names*

