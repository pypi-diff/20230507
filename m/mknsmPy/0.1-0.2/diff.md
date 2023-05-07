# Comparing `tmp/mknsmPy-0.1.tar.gz` & `tmp/mknsmPy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mknsmPy-0.1.tar", last modified: Sun May  7 07:12:25 2023, max compression
+gzip compressed data, was "mknsmPy-0.2.tar", last modified: Sun May  7 15:42:19 2023, max compression
```

## Comparing `mknsmPy-0.1.tar` & `mknsmPy-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 hihimamu  (1000) hihimamu  (1000)        0 2023-05-07 07:12:25.546197 mknsmPy-0.1/
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      109 2023-05-07 06:20:23.000000 mknsmPy-0.1/LICENSE
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)       51 2023-05-07 04:48:04.000000 mknsmPy-0.1/MANIFEST.in
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      472 2023-05-07 07:12:25.546197 mknsmPy-0.1/PKG-INFO
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      133 2023-05-07 06:48:44.000000 mknsmPy-0.1/README.md
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      151 2023-05-07 06:52:19.000000 mknsmPy-0.1/README.rst
-drwxr-xr-x   0 hihimamu  (1000) hihimamu  (1000)        0 2023-05-07 07:12:25.546197 mknsmPy-0.1/mknsmPy/
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      286 2023-05-07 06:19:21.000000 mknsmPy-0.1/mknsmPy/__init__.py
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)    14451 2023-05-06 15:21:55.000000 mknsmPy-0.1/mknsmPy/mknsmPy.py
-drwxr-xr-x   0 hihimamu  (1000) hihimamu  (1000)        0 2023-05-07 07:12:25.546197 mknsmPy-0.1/mknsmPy.egg-info/
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      472 2023-05-07 07:12:25.000000 mknsmPy-0.1/mknsmPy.egg-info/PKG-INFO
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      212 2023-05-07 07:12:25.000000 mknsmPy-0.1/mknsmPy.egg-info/SOURCES.txt
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)        1 2023-05-07 07:12:25.000000 mknsmPy-0.1/mknsmPy.egg-info/dependency_links.txt
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)        8 2023-05-07 07:12:25.000000 mknsmPy-0.1/mknsmPy.egg-info/top_level.txt
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)       38 2023-05-07 07:12:25.546197 mknsmPy-0.1/setup.cfg
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      783 2023-05-07 07:01:23.000000 mknsmPy-0.1/setup.py
+drwxr-xr-x   0 hihimamu  (1000) hihimamu  (1000)        0 2023-05-07 15:42:19.910046 mknsmPy-0.2/
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)     1067 2023-05-07 13:20:58.000000 mknsmPy-0.2/LICENSE
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)       51 2023-05-07 04:48:04.000000 mknsmPy-0.2/MANIFEST.in
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)     1172 2023-05-07 15:42:19.910046 mknsmPy-0.2/PKG-INFO
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      692 2023-05-07 15:39:10.000000 mknsmPy-0.2/README.md
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      851 2023-05-07 15:41:43.000000 mknsmPy-0.2/README.rst
+drwxr-xr-x   0 hihimamu  (1000) hihimamu  (1000)        0 2023-05-07 15:42:19.910046 mknsmPy-0.2/mknsmPy/
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      286 2023-05-07 15:25:15.000000 mknsmPy-0.2/mknsmPy/__init__.py
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)    14451 2023-05-06 15:21:55.000000 mknsmPy-0.2/mknsmPy/mknsmPy.py
+drwxr-xr-x   0 hihimamu  (1000) hihimamu  (1000)        0 2023-05-07 15:42:19.910046 mknsmPy-0.2/mknsmPy.egg-info/
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)     1172 2023-05-07 15:42:19.000000 mknsmPy-0.2/mknsmPy.egg-info/PKG-INFO
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      212 2023-05-07 15:42:19.000000 mknsmPy-0.2/mknsmPy.egg-info/SOURCES.txt
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)        1 2023-05-07 15:42:19.000000 mknsmPy-0.2/mknsmPy.egg-info/dependency_links.txt
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)        8 2023-05-07 15:42:19.000000 mknsmPy-0.2/mknsmPy.egg-info/top_level.txt
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)       38 2023-05-07 15:42:19.910046 mknsmPy-0.2/setup.cfg
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      783 2023-05-07 15:23:53.000000 mknsmPy-0.2/setup.py
```

### Comparing `mknsmPy-0.1/mknsmPy/mknsmPy.py` & `mknsmPy-0.2/mknsmPy/mknsmPy.py`

 * *Files identical despite different names*

### Comparing `mknsmPy-0.1/setup.py` & `mknsmPy-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.rst', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name                          = "mknsmPy", 
     license                       = "MIT",
-    version                       = "0.1", 
+    version                       = "0.2", 
     packages                      = find_packages(), 
     author                        = "hihimamu", 
     author_email                  = "mamu.pypi@shchiba.uk", 
     url                           = "https://github.com/hihimamuLab/MekanismCalcLibrary.git", 
     description                   = "mekanism material calculator", 
     long_description              = long_description,
     long_description_content_type = "text/x-rst",
```

