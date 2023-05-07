# Comparing `tmp/gcsaws-0.0.5.tar.gz` & `tmp/gcsaws-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcsaws-0.0.5.tar", last modified: Sun May  7 15:48:22 2023, max compression
+gzip compressed data, was "gcsaws-0.0.6.tar", last modified: Sun May  7 15:59:54 2023, max compression
```

## Comparing `gcsaws-0.0.5.tar` & `gcsaws-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 15:48:22.759411 gcsaws-0.0.5/
--rw-rw-rw-   0        0        0     1091 2023-05-07 12:57:03.000000 gcsaws-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      412 2023-05-07 15:48:22.759411 gcsaws-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        8 2023-05-07 12:56:41.000000 gcsaws-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 15:48:22.743786 gcsaws-0.0.5/gcsaws/
--rw-rw-rw-   0        0        0      112 2023-05-07 12:59:09.000000 gcsaws-0.0.5/gcsaws/__init__.py
--rw-rw-rw-   0        0        0      684 2023-05-07 12:59:09.000000 gcsaws-0.0.5/gcsaws/helpers.py
--rw-rw-rw-   0        0        0     8669 2023-05-07 13:03:17.000000 gcsaws-0.0.5/gcsaws/nodes.py
--rw-rw-rw-   0        0        0     4037 2023-05-07 13:19:03.000000 gcsaws-0.0.5/gcsaws/visitor_procedure.py
-drwxrwxrwx   0        0        0        0 2023-05-07 15:48:22.759411 gcsaws-0.0.5/gcsaws.egg-info/
--rw-rw-rw-   0        0        0      412 2023-05-07 15:48:22.000000 gcsaws-0.0.5/gcsaws.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-05-07 15:48:22.000000 gcsaws-0.0.5/gcsaws.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 15:48:22.000000 gcsaws-0.0.5/gcsaws.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-07 15:48:22.000000 gcsaws-0.0.5/gcsaws.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-07 15:48:22.000000 gcsaws-0.0.5/gcsaws.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      662 2023-05-07 15:48:00.000000 gcsaws-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 15:48:22.759411 gcsaws-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-07 15:48:22.759411 gcsaws-0.0.5/tests/
--rw-rw-rw-   0        0        0      810 2023-05-07 11:28:19.000000 gcsaws-0.0.5/tests/test_create_target_list.py
--rw-rw-rw-   0        0        0     3258 2023-05-06 18:27:00.000000 gcsaws-0.0.5/tests/test_simple.py
+drwxrwxrwx   0        0        0        0 2023-05-07 15:59:54.978002 gcsaws-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-05-07 12:57:03.000000 gcsaws-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      412 2023-05-07 15:59:54.978002 gcsaws-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        8 2023-05-07 12:56:41.000000 gcsaws-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 15:59:54.962378 gcsaws-0.0.6/gcsaws/
+-rw-rw-rw-   0        0        0      112 2023-05-07 12:59:09.000000 gcsaws-0.0.6/gcsaws/__init__.py
+-rw-rw-rw-   0        0        0      684 2023-05-07 12:59:09.000000 gcsaws-0.0.6/gcsaws/helpers.py
+-rw-rw-rw-   0        0        0     8669 2023-05-07 13:03:17.000000 gcsaws-0.0.6/gcsaws/nodes.py
+-rw-rw-rw-   0        0        0     4037 2023-05-07 13:19:03.000000 gcsaws-0.0.6/gcsaws/visitor_procedure.py
+drwxrwxrwx   0        0        0        0 2023-05-07 15:59:54.978002 gcsaws-0.0.6/gcsaws.egg-info/
+-rw-rw-rw-   0        0        0      412 2023-05-07 15:59:54.000000 gcsaws-0.0.6/gcsaws.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-05-07 15:59:54.000000 gcsaws-0.0.6/gcsaws.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 15:59:54.000000 gcsaws-0.0.6/gcsaws.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-07 15:59:54.000000 gcsaws-0.0.6/gcsaws.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-07 15:59:54.000000 gcsaws-0.0.6/gcsaws.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      662 2023-05-07 15:59:44.000000 gcsaws-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 15:59:54.978002 gcsaws-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 15:59:54.978002 gcsaws-0.0.6/tests/
+-rw-rw-rw-   0        0        0      810 2023-05-07 11:28:19.000000 gcsaws-0.0.6/tests/test_create_target_list.py
+-rw-rw-rw-   0        0        0     3258 2023-05-06 18:27:00.000000 gcsaws-0.0.6/tests/test_simple.py
```

### Comparing `gcsaws-0.0.5/LICENSE` & `gcsaws-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gcsaws-0.0.5/gcsaws/helpers.py` & `gcsaws-0.0.6/gcsaws/helpers.py`

 * *Files identical despite different names*

### Comparing `gcsaws-0.0.5/gcsaws/nodes.py` & `gcsaws-0.0.6/gcsaws/nodes.py`

 * *Files identical despite different names*

### Comparing `gcsaws-0.0.5/gcsaws/visitor_procedure.py` & `gcsaws-0.0.6/gcsaws/visitor_procedure.py`

 * *Files identical despite different names*

### Comparing `gcsaws-0.0.5/pyproject.toml` & `gcsaws-0.0.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gcsaws"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name="Leikt", email="leikt.solreihin@gmail.com" },
 ]
 description = "GCS implementation for the aws-automation package."
 readme = "README.md"
-requires-python = ">=3.6"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "gcscore>=0.0.5"
+    "gcscore>=0.0.6"
 ]
 #[project.urls]
 #"Homepage" = "https://github.com/pypa/sampleproject"
 #"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

### Comparing `gcsaws-0.0.5/tests/test_create_target_list.py` & `gcsaws-0.0.6/tests/test_create_target_list.py`

 * *Files identical despite different names*

### Comparing `gcsaws-0.0.5/tests/test_simple.py` & `gcsaws-0.0.6/tests/test_simple.py`

 * *Files identical despite different names*

