# Comparing `tmp/magpylib-material-response-0.1.0a4.tar.gz` & `tmp/magpylib-material-response-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/magpylib-material-response-0.1.0a4.tar", last modified: Fri May  5 23:50:53 2023, max compression
+gzip compressed data, was "dist/magpylib-material-response-0.1.0a5.tar", last modified: Sun May  7 15:30:22 2023, max compression
```

## Comparing `magpylib-material-response-0.1.0a4.tar` & `magpylib-material-response-0.1.0a5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:50:53.000000 magpylib-material-response-0.1.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 23:50:50.000000 magpylib-material-response-0.1.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-05 23:50:53.000000 magpylib-material-response-0.1.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-05 23:50:50.000000 magpylib-material-response-0.1.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:50:53.000000 magpylib-material-response-0.1.0a4/magpylib_material_response/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-05 23:50:50.000000 magpylib-material-response-0.1.0a4/magpylib_material_response/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:50:53.000000 magpylib-material-response-0.1.0a4/magpylib_material_response/data/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-05 23:50:50.000000 magpylib-material-response-0.1.0a4/magpylib_material_response/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-05-05 23:50:50.000000 magpylib-material-response-0.1.0a4/magpylib_material_response/demag.py
--rw-r--r--   0 runner    (1001) docker     (123)    15995 2023-05-05 23:50:50.000000 magpylib-material-response-0.1.0a4/magpylib_material_response/meshing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-05-05 23:50:50.000000 magpylib-material-response-0.1.0a4/magpylib_material_response/meshing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-05-05 23:50:50.000000 magpylib-material-response-0.1.0a4/magpylib_material_response/polyline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-05 23:50:50.000000 magpylib-material-response-0.1.0a4/magpylib_material_response/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:50:53.000000 magpylib-material-response-0.1.0a4/magpylib_material_response.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-05 23:50:53.000000 magpylib-material-response-0.1.0a4/magpylib_material_response.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-05 23:50:53.000000 magpylib-material-response-0.1.0a4/magpylib_material_response.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 23:50:53.000000 magpylib-material-response-0.1.0a4/magpylib_material_response.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-05 23:50:53.000000 magpylib-material-response-0.1.0a4/magpylib_material_response.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 23:50:53.000000 magpylib-material-response-0.1.0a4/magpylib_material_response.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 23:50:53.000000 magpylib-material-response-0.1.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-05 23:50:50.000000 magpylib-material-response-0.1.0a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:30:22.000000 magpylib-material-response-0.1.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-07 15:30:19.000000 magpylib-material-response-0.1.0a5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-07 15:30:22.000000 magpylib-material-response-0.1.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-07 15:30:19.000000 magpylib-material-response-0.1.0a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:30:22.000000 magpylib-material-response-0.1.0a5/magpylib_material_response/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-07 15:30:19.000000 magpylib-material-response-0.1.0a5/magpylib_material_response/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:30:22.000000 magpylib-material-response-0.1.0a5/magpylib_material_response/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-07 15:30:19.000000 magpylib-material-response-0.1.0a5/magpylib_material_response/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-05-07 15:30:19.000000 magpylib-material-response-0.1.0a5/magpylib_material_response/demag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15995 2023-05-07 15:30:19.000000 magpylib-material-response-0.1.0a5/magpylib_material_response/meshing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-05-07 15:30:19.000000 magpylib-material-response-0.1.0a5/magpylib_material_response/meshing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-07 15:30:19.000000 magpylib-material-response-0.1.0a5/magpylib_material_response/polyline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-07 15:30:19.000000 magpylib-material-response-0.1.0a5/magpylib_material_response/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:30:22.000000 magpylib-material-response-0.1.0a5/magpylib_material_response.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-07 15:30:22.000000 magpylib-material-response-0.1.0a5/magpylib_material_response.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-07 15:30:22.000000 magpylib-material-response-0.1.0a5/magpylib_material_response.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 15:30:22.000000 magpylib-material-response-0.1.0a5/magpylib_material_response.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-07 15:30:22.000000 magpylib-material-response-0.1.0a5/magpylib_material_response.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-07 15:30:22.000000 magpylib-material-response-0.1.0a5/magpylib_material_response.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 15:30:22.000000 magpylib-material-response-0.1.0a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-07 15:30:19.000000 magpylib-material-response-0.1.0a5/setup.py
```

### Comparing `magpylib-material-response-0.1.0a4/PKG-INFO` & `magpylib-material-response-0.1.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magpylib-material-response
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: An extension to the Magpylib library, providing magnetic field analysis for soft materials and demagnetization of hard magnets.
 Home-page: https://github.com/magpylib/magpylib-material-response
 Author: Alexandre Boisselet
 Author-email: magpylib@gmail.com
 License: MIT
 Description: # magpylib-material-response
```

### Comparing `magpylib-material-response-0.1.0a4/README.md` & `magpylib-material-response-0.1.0a5/README.md`

 * *Files identical despite different names*

### Comparing `magpylib-material-response-0.1.0a4/magpylib_material_response/demag.py` & `magpylib-material-response-0.1.0a5/magpylib_material_response/demag.py`

 * *Files identical despite different names*

### Comparing `magpylib-material-response-0.1.0a4/magpylib_material_response/meshing.py` & `magpylib-material-response-0.1.0a5/magpylib_material_response/meshing.py`

 * *Files identical despite different names*

### Comparing `magpylib-material-response-0.1.0a4/magpylib_material_response/meshing_utils.py` & `magpylib-material-response-0.1.0a5/magpylib_material_response/meshing_utils.py`

 * *Files identical despite different names*

### Comparing `magpylib-material-response-0.1.0a4/magpylib_material_response/polyline.py` & `magpylib-material-response-0.1.0a5/magpylib_material_response/polyline.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,16 @@
     Parameters
     ----------
     a, b, c : array-like
         Vertices of a triangle (b is the middle vertex) with shape (2,) or (3,).
     r : float
         Radius of the circle.
     max_ratio : float, optional, default: 0.5
-        Maximum allowed ratio of the distance to the tangent point relative to the length of the triangle sides.
+        Maximum allowed ratio of the distance to the tangent point relative to the length of the
+        triangle sides.
 
     Returns
     -------
     tuple
         Circle center, tangent point a, tangent point b as NumPy arrays.
     """
     # Calculate the unit vectors along AB and BC
```

### Comparing `magpylib-material-response-0.1.0a4/magpylib_material_response/utils.py` & `magpylib-material-response-0.1.0a5/magpylib_material_response/utils.py`

 * *Files identical despite different names*

### Comparing `magpylib-material-response-0.1.0a4/magpylib_material_response.egg-info/PKG-INFO` & `magpylib-material-response-0.1.0a5/magpylib_material_response.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magpylib-material-response
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: An extension to the Magpylib library, providing magnetic field analysis for soft materials and demagnetization of hard magnets.
 Home-page: https://github.com/magpylib/magpylib-material-response
 Author: Alexandre Boisselet
 Author-email: magpylib@gmail.com
 License: MIT
 Description: # magpylib-material-response
```

### Comparing `magpylib-material-response-0.1.0a4/magpylib_material_response.egg-info/SOURCES.txt` & `magpylib-material-response-0.1.0a5/magpylib_material_response.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magpylib-material-response-0.1.0a4/setup.py` & `magpylib-material-response-0.1.0a5/setup.py`

 * *Files identical despite different names*

