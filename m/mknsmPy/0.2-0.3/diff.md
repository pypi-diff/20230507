# Comparing `tmp/mknsmPy-0.2.tar.gz` & `tmp/mknsmPy-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mknsmPy-0.2.tar", last modified: Sun May  7 15:42:19 2023, max compression
+gzip compressed data, was "mknsmPy-0.3.tar", last modified: Sun May  7 15:59:15 2023, max compression
```

## Comparing `mknsmPy-0.2.tar` & `mknsmPy-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 hihimamu  (1000) hihimamu  (1000)        0 2023-05-07 15:42:19.910046 mknsmPy-0.2/
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)     1067 2023-05-07 13:20:58.000000 mknsmPy-0.2/LICENSE
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)       51 2023-05-07 04:48:04.000000 mknsmPy-0.2/MANIFEST.in
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)     1172 2023-05-07 15:42:19.910046 mknsmPy-0.2/PKG-INFO
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      692 2023-05-07 15:39:10.000000 mknsmPy-0.2/README.md
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      851 2023-05-07 15:41:43.000000 mknsmPy-0.2/README.rst
-drwxr-xr-x   0 hihimamu  (1000) hihimamu  (1000)        0 2023-05-07 15:42:19.910046 mknsmPy-0.2/mknsmPy/
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      286 2023-05-07 15:25:15.000000 mknsmPy-0.2/mknsmPy/__init__.py
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)    14451 2023-05-06 15:21:55.000000 mknsmPy-0.2/mknsmPy/mknsmPy.py
-drwxr-xr-x   0 hihimamu  (1000) hihimamu  (1000)        0 2023-05-07 15:42:19.910046 mknsmPy-0.2/mknsmPy.egg-info/
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)     1172 2023-05-07 15:42:19.000000 mknsmPy-0.2/mknsmPy.egg-info/PKG-INFO
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      212 2023-05-07 15:42:19.000000 mknsmPy-0.2/mknsmPy.egg-info/SOURCES.txt
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)        1 2023-05-07 15:42:19.000000 mknsmPy-0.2/mknsmPy.egg-info/dependency_links.txt
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)        8 2023-05-07 15:42:19.000000 mknsmPy-0.2/mknsmPy.egg-info/top_level.txt
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)       38 2023-05-07 15:42:19.910046 mknsmPy-0.2/setup.cfg
--rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      783 2023-05-07 15:23:53.000000 mknsmPy-0.2/setup.py
+drwxr-xr-x   0 hihimamu  (1000) hihimamu  (1000)        0 2023-05-07 15:59:15.769796 mknsmPy-0.3/
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)     1067 2023-05-07 13:20:58.000000 mknsmPy-0.3/LICENSE
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)       51 2023-05-07 04:48:04.000000 mknsmPy-0.3/MANIFEST.in
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)     1135 2023-05-07 15:59:15.769796 mknsmPy-0.3/PKG-INFO
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      692 2023-05-07 15:39:10.000000 mknsmPy-0.3/README.md
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      814 2023-05-07 15:57:17.000000 mknsmPy-0.3/README.rst
+drwxr-xr-x   0 hihimamu  (1000) hihimamu  (1000)        0 2023-05-07 15:59:15.759796 mknsmPy-0.3/mknsmPy/
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      286 2023-05-07 15:58:13.000000 mknsmPy-0.3/mknsmPy/__init__.py
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)    14451 2023-05-06 15:21:55.000000 mknsmPy-0.3/mknsmPy/mknsmPy.py
+drwxr-xr-x   0 hihimamu  (1000) hihimamu  (1000)        0 2023-05-07 15:59:15.769796 mknsmPy-0.3/mknsmPy.egg-info/
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)     1135 2023-05-07 15:59:15.000000 mknsmPy-0.3/mknsmPy.egg-info/PKG-INFO
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      212 2023-05-07 15:59:15.000000 mknsmPy-0.3/mknsmPy.egg-info/SOURCES.txt
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)        1 2023-05-07 15:59:15.000000 mknsmPy-0.3/mknsmPy.egg-info/dependency_links.txt
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)        8 2023-05-07 15:59:15.000000 mknsmPy-0.3/mknsmPy.egg-info/top_level.txt
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)       38 2023-05-07 15:59:15.769796 mknsmPy-0.3/setup.cfg
+-rw-r--r--   0 hihimamu  (1000) hihimamu  (1000)      783 2023-05-07 15:57:57.000000 mknsmPy-0.3/setup.py
```

### Comparing `mknsmPy-0.2/LICENSE` & `mknsmPy-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mknsmPy-0.2/PKG-INFO` & `mknsmPy-0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: mknsmPy
-Version: 0.2
+Version: 0.3
 Summary: mekanism material calculator
 Home-page: https://github.com/hihimamuLab/MekanismCalcLibrary.git
 Author: hihimamu
 Author-email: mamu.pypi@shchiba.uk
 License: MIT
 Keywords: mekanism,mechanism,mknsm,mknsmPy
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 MekanismCalcLiblary
 ===================
 
-.. figure:: https://user-images.githubusercontent.com/122292089/236683530-15675752-b36e-428e-9e9f-1a1f292853f0.png
-   :alt: mknsmPy rogo
-
-   mknsmPy rogo
+.. figure:: https://user-images.githubusercontent.com/122292089/236683530-15675752-b36e-428e-9e9f-1a1f292853f0.png  
 
 mekanismの材料計算をもっと簡単に
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 |MIT License| |PyPI version|
 
    pip install mknsmPy
```

### Comparing `mknsmPy-0.2/README.md` & `mknsmPy-0.3/README.md`

 * *Files identical despite different names*

### Comparing `mknsmPy-0.2/README.rst` & `mknsmPy-0.3/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 MekanismCalcLiblary
 ===================
 
-.. figure:: https://user-images.githubusercontent.com/122292089/236683530-15675752-b36e-428e-9e9f-1a1f292853f0.png
-   :alt: mknsmPy rogo
-
-   mknsmPy rogo
+.. figure:: https://user-images.githubusercontent.com/122292089/236683530-15675752-b36e-428e-9e9f-1a1f292853f0.png  
 
 mekanismの材料計算をもっと簡単に
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 |MIT License| |PyPI version|
 
    pip install mknsmPy
```

### Comparing `mknsmPy-0.2/mknsmPy/mknsmPy.py` & `mknsmPy-0.3/mknsmPy/mknsmPy.py`

 * *Files identical despite different names*

### Comparing `mknsmPy-0.2/mknsmPy.egg-info/PKG-INFO` & `mknsmPy-0.3/mknsmPy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: mknsmPy
-Version: 0.2
+Version: 0.3
 Summary: mekanism material calculator
 Home-page: https://github.com/hihimamuLab/MekanismCalcLibrary.git
 Author: hihimamu
 Author-email: mamu.pypi@shchiba.uk
 License: MIT
 Keywords: mekanism,mechanism,mknsm,mknsmPy
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 MekanismCalcLiblary
 ===================
 
-.. figure:: https://user-images.githubusercontent.com/122292089/236683530-15675752-b36e-428e-9e9f-1a1f292853f0.png
-   :alt: mknsmPy rogo
-
-   mknsmPy rogo
+.. figure:: https://user-images.githubusercontent.com/122292089/236683530-15675752-b36e-428e-9e9f-1a1f292853f0.png  
 
 mekanismの材料計算をもっと簡単に
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 |MIT License| |PyPI version|
 
    pip install mknsmPy
```

### Comparing `mknsmPy-0.2/setup.py` & `mknsmPy-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.rst', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name                          = "mknsmPy", 
     license                       = "MIT",
-    version                       = "0.2", 
+    version                       = "0.3", 
     packages                      = find_packages(), 
     author                        = "hihimamu", 
     author_email                  = "mamu.pypi@shchiba.uk", 
     url                           = "https://github.com/hihimamuLab/MekanismCalcLibrary.git", 
     description                   = "mekanism material calculator", 
     long_description              = long_description,
     long_description_content_type = "text/x-rst",
```

