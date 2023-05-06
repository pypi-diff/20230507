# Comparing `tmp/geolibs-0.0.3.tar.gz` & `tmp/geolibs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geolibs-0.0.3.tar", max compression
+gzip compressed data, was "geolibs-0.0.4.tar", max compression
```

## Comparing `geolibs-0.0.3.tar` & `geolibs-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rwxr-xr-x   0        0        0      528 2023-05-04 20:41:51.294192 geolibs-0.0.3/README.rst
--rwxr-xr-x   0        0        0      465 2023-05-06 20:54:28.831474 geolibs-0.0.3/geolibs/__init__.py
--rwxr-xr-x   0        0        0     5514 2023-05-06 20:36:53.288107 geolibs-0.0.3/geolibs/engine_cocoext.py
--rwxr-xr-x   0        0        0     2469 2023-05-03 11:53:56.288065 geolibs-0.0.3/geolibs/engine_cocometric.py
--rwxr-xr-x   0        0        0     5015 2023-05-03 11:53:56.299297 geolibs-0.0.3/geolibs/enginelogger_hook.py
--rwxr-xr-x   0        0        0    12304 2023-05-06 20:53:44.332058 geolibs-0.0.3/geolibs/loading.py
--rwxr-xr-x   0        0        0     1122 2023-05-03 11:53:56.323004 geolibs-0.0.3/geolibs/misc.py
--rwxr-xr-x   0        0        0     1066 2023-05-06 20:54:28.826392 geolibs-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1671 1970-01-01 00:00:00.000000 geolibs-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0      566 2023-05-06 21:58:44.569227 geolibs-0.0.4/README.rst
+-rwxr-xr-x   0        0        0      512 2023-05-06 22:05:37.281858 geolibs-0.0.4/geolibs/__init__.py
+-rwxr-xr-x   0        0        0     5514 2023-05-06 20:36:53.288107 geolibs-0.0.4/geolibs/engine_cocoext.py
+-rwxr-xr-x   0        0        0     2469 2023-05-03 11:53:56.288065 geolibs-0.0.4/geolibs/engine_cocometric.py
+-rwxr-xr-x   0        0        0     4167 2023-05-06 21:58:44.616807 geolibs-0.0.4/geolibs/engine_csv.py
+-rwxr-xr-x   0        0        0     5015 2023-05-03 11:53:56.299297 geolibs-0.0.4/geolibs/enginelogger_hook.py
+-rwxr-xr-x   0        0        0    12304 2023-05-06 20:53:44.332058 geolibs-0.0.4/geolibs/loading.py
+-rwxr-xr-x   0        0        0     1122 2023-05-03 11:53:56.323004 geolibs-0.0.4/geolibs/misc.py
+-rwxr-xr-x   0        0        0     1066 2023-05-06 22:05:37.276852 geolibs-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1709 1970-01-01 00:00:00.000000 geolibs-0.0.4/PKG-INFO
```

### Comparing `geolibs-0.0.3/README.rst` & `geolibs-0.0.4/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
    pip install torch torchvision
    pip install -U openmim
    mim install "mmengine>=0.6.0"
    mim install "mmcv>=2.0.0rc4,<2.1.0"
    mim install "mmdet>=3.0.0rc6,<3.1.0"
    mim install "mmyolo"
    mim install "mmsegmentation>=1.0.0"
+   mim install "mmpretrain>=1.0.0rc7"
    pip install geolibs
 
 License
 -------
 
 GPLv3
```

### Comparing `geolibs-0.0.3/geolibs/engine_cocoext.py` & `geolibs-0.0.4/geolibs/engine_cocoext.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.3/geolibs/engine_cocometric.py` & `geolibs-0.0.4/geolibs/engine_cocometric.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.3/geolibs/enginelogger_hook.py` & `geolibs-0.0.4/geolibs/enginelogger_hook.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.3/geolibs/loading.py` & `geolibs-0.0.4/geolibs/loading.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.3/geolibs/misc.py` & `geolibs-0.0.4/geolibs/misc.py`

 * *Files identical despite different names*

### Comparing `geolibs-0.0.3/pyproject.toml` & `geolibs-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geolibs"
-version = "v0.0.3"
+version = "v0.0.4"
 description = "A wrapper library that integrates GeoEngine and MMLab libraries for GeoSpatial ML development."
 authors = ["Sagar Verma <sagar@granular.ai>"]
 license = "MIT"
 readme = "README.rst"
 packages = [{include = "geolibs"}]
 classifiers = [
     'Intended Audience :: Developers',
```

### Comparing `geolibs-0.0.3/PKG-INFO` & `geolibs-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geolibs
-Version: 0.0.3
+Version: 0.0.4
 Summary: A wrapper library that integrates GeoEngine and MMLab libraries for GeoSpatial ML development.
 Home-page: https://github.com/granularai/geolibs
 License: MIT
 Author: Sagar Verma
 Author-email: sagar@granular.ai
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Intended Audience :: Developers
@@ -40,14 +40,15 @@
    pip install torch torchvision
    pip install -U openmim
    mim install "mmengine>=0.6.0"
    mim install "mmcv>=2.0.0rc4,<2.1.0"
    mim install "mmdet>=3.0.0rc6,<3.1.0"
    mim install "mmyolo"
    mim install "mmsegmentation>=1.0.0"
+   mim install "mmpretrain>=1.0.0rc7"
    pip install geolibs
 
 License
 -------
 
 GPLv3
```

