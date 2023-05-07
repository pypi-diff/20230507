# Comparing `tmp/scrainbow-0.0.1.tar.gz` & `tmp/scrainbow-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrainbow-0.0.1.tar", last modified: Sun May  7 06:27:54 2023, max compression
+gzip compressed data, was "scrainbow-0.0.2.tar", last modified: Sun May  7 08:10:54 2023, max compression
```

## Comparing `scrainbow-0.0.1.tar` & `scrainbow-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,17 @@
-drwxrwxr-x   0 sccassuper  (1009) sccassuper  (1010)        0 2023-05-07 06:27:54.108272 scrainbow-0.0.1/
--rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)      840 2023-05-07 06:27:54.108272 scrainbow-0.0.1/PKG-INFO
-drwxrwxr-x   0 sccassuper  (1009) sccassuper  (1010)        0 2023-05-07 06:27:54.108272 scrainbow-0.0.1/scrainbow.egg-info/
--rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)      840 2023-05-07 06:27:54.000000 scrainbow-0.0.1/scrainbow.egg-info/PKG-INFO
--rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)      163 2023-05-07 06:27:54.000000 scrainbow-0.0.1/scrainbow.egg-info/SOURCES.txt
--rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)        1 2023-05-07 06:27:54.000000 scrainbow-0.0.1/scrainbow.egg-info/dependency_links.txt
--rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)      153 2023-05-07 06:27:54.000000 scrainbow-0.0.1/scrainbow.egg-info/requires.txt
--rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)        1 2023-05-07 06:27:54.000000 scrainbow-0.0.1/scrainbow.egg-info/top_level.txt
--rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)       38 2023-05-07 06:27:54.108272 scrainbow-0.0.1/setup.cfg
+drwxrwxr-x   0 sccassuper  (1009) sccassuper  (1010)        0 2023-05-07 08:10:54.864077 scrainbow-0.0.2/
+-rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)     1064 2023-05-07 03:26:18.000000 scrainbow-0.0.2/LICENSE
+-rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)      878 2023-05-07 08:10:54.864077 scrainbow-0.0.2/PKG-INFO
+drwxrwxr-x   0 sccassuper  (1009) sccassuper  (1010)        0 2023-05-07 08:10:54.860077 scrainbow-0.0.2/scrainbow/
+-rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)      139 2023-05-07 02:56:36.000000 scrainbow-0.0.2/scrainbow/__init__.py
+-rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)     2058 2023-05-07 02:55:43.000000 scrainbow-0.0.2/scrainbow/data_processing.py
+-rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)     6157 2023-05-07 07:56:19.000000 scrainbow-0.0.2/scrainbow/model.py
+-rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)     4065 2023-05-07 07:58:52.000000 scrainbow-0.0.2/scrainbow/run.py
+-rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)     3374 2023-05-07 07:57:35.000000 scrainbow-0.0.2/scrainbow/utils.py
+drwxrwxr-x   0 sccassuper  (1009) sccassuper  (1010)        0 2023-05-07 08:10:54.860077 scrainbow-0.0.2/scrainbow.egg-info/
+-rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)      878 2023-05-07 08:10:54.000000 scrainbow-0.0.2/scrainbow.egg-info/PKG-INFO
+-rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)      286 2023-05-07 08:10:54.000000 scrainbow-0.0.2/scrainbow.egg-info/SOURCES.txt
+-rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)        1 2023-05-07 08:10:54.000000 scrainbow-0.0.2/scrainbow.egg-info/dependency_links.txt
+-rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)      153 2023-05-07 08:10:54.000000 scrainbow-0.0.2/scrainbow.egg-info/requires.txt
+-rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)       10 2023-05-07 08:10:54.000000 scrainbow-0.0.2/scrainbow.egg-info/top_level.txt
+-rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)       38 2023-05-07 08:10:54.864077 scrainbow-0.0.2/setup.cfg
+-rw-rw-r--   0 sccassuper  (1009) sccassuper  (1010)     1294 2023-05-07 08:09:49.000000 scrainbow-0.0.2/setup.py
```

### Comparing `scrainbow-0.0.1/PKG-INFO` & `scrainbow-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: scrainbow
-Version: 0.0.1
-Summary: RAINBOW: a scCAS cell type annotation method via contrastive laerning and reference guidance
+Version: 0.0.2
+Summary: RAINBOW: accurate cell type annotation method via contrastive learning and reference guidance for scCAS data
 Home-page: https://github.com/BioX-NKU/RAINBOW
 Author: Siyu Li
 License: MIT License
 Keywords: pip,RAINBOW,single-sell
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >3.6.0
+License-File: LICENSE
 
 RAINBOW provides an accurate and efficient way to automatically annotate celltypes in scCAS datasets. All RAINBOW wheels distributed on PyPI are MIT licensed.
```

### Comparing `scrainbow-0.0.1/scrainbow.egg-info/PKG-INFO` & `scrainbow-0.0.2/scrainbow.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: scrainbow
-Version: 0.0.1
-Summary: RAINBOW: a scCAS cell type annotation method via contrastive laerning and reference guidance
+Version: 0.0.2
+Summary: RAINBOW: accurate cell type annotation method via contrastive learning and reference guidance for scCAS data
 Home-page: https://github.com/BioX-NKU/RAINBOW
 Author: Siyu Li
 License: MIT License
 Keywords: pip,RAINBOW,single-sell
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >3.6.0
+License-File: LICENSE
 
 RAINBOW provides an accurate and efficient way to automatically annotate celltypes in scCAS datasets. All RAINBOW wheels distributed on PyPI are MIT licensed.
```

