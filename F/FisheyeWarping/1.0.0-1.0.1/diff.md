# Comparing `tmp/FisheyeWarping-1.0.0.tar.gz` & `tmp/FisheyeWarping-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FisheyeWarping-1.0.0.tar", last modified: Sun May  7 13:55:32 2023, max compression
+gzip compressed data, was "FisheyeWarping-1.0.1.tar", last modified: Sun May  7 13:59:34 2023, max compression
```

## Comparing `FisheyeWarping-1.0.0.tar` & `FisheyeWarping-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:55:32.575317 FisheyeWarping-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-07 13:55:21.000000 FisheyeWarping-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-07 13:55:21.000000 FisheyeWarping-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-05-07 13:55:32.575317 FisheyeWarping-1.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7214 2023-05-07 13:55:21.000000 FisheyeWarping-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:55:32.575317 FisheyeWarping-1.0.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)   379877 2023-05-07 13:55:21.000000 FisheyeWarping-1.0.0/doc/101-fisheye.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    63732 2023-05-07 13:55:21.000000 FisheyeWarping-1.0.0/doc/101-panorama.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1085186 2023-05-07 13:55:21.000000 FisheyeWarping-1.0.0/doc/mesh-fisheye.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   941796 2023-05-07 13:55:21.000000 FisheyeWarping-1.0.0/doc/mesh-panorama.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-07 13:55:21.000000 FisheyeWarping-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-07 13:55:21.000000 FisheyeWarping-1.0.0/reinstall.bat
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-07 13:55:21.000000 FisheyeWarping-1.0.0/reinstall.sh
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-07 13:55:32.579317 FisheyeWarping-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-07 13:55:21.000000 FisheyeWarping-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:55:32.571317 FisheyeWarping-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:55:32.575317 FisheyeWarping-1.0.0/src/FisheyeWarping.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-05-07 13:55:32.000000 FisheyeWarping-1.0.0/src/FisheyeWarping.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-07 13:55:32.000000 FisheyeWarping-1.0.0/src/FisheyeWarping.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 13:55:32.000000 FisheyeWarping-1.0.0/src/FisheyeWarping.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-07 13:55:32.000000 FisheyeWarping-1.0.0/src/FisheyeWarping.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-07 13:55:32.000000 FisheyeWarping-1.0.0/src/FisheyeWarping.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 13:55:32.000000 FisheyeWarping-1.0.0/src/FisheyeWarping.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:55:32.575317 FisheyeWarping-1.0.0/src/fisheyewarping/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-07 13:55:21.000000 FisheyeWarping-1.0.0/src/fisheyewarping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-05-07 13:55:21.000000 FisheyeWarping-1.0.0/src/fisheyewarping/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12085 2023-05-07 13:55:21.000000 FisheyeWarping-1.0.0/src/fisheyewarping/fisheyewarping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:55:32.575317 FisheyeWarping-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-07 13:55:21.000000 FisheyeWarping-1.0.0/tests/test_fisheye_warping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:34.749175 FisheyeWarping-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-07 13:59:23.000000 FisheyeWarping-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-07 13:59:23.000000 FisheyeWarping-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-05-07 13:59:34.749175 FisheyeWarping-1.0.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7472 2023-05-07 13:59:23.000000 FisheyeWarping-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:34.745175 FisheyeWarping-1.0.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)   379877 2023-05-07 13:59:23.000000 FisheyeWarping-1.0.1/doc/101-fisheye.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    63732 2023-05-07 13:59:23.000000 FisheyeWarping-1.0.1/doc/101-panorama.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1085186 2023-05-07 13:59:23.000000 FisheyeWarping-1.0.1/doc/mesh-fisheye.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   941796 2023-05-07 13:59:23.000000 FisheyeWarping-1.0.1/doc/mesh-panorama.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-07 13:59:23.000000 FisheyeWarping-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-07 13:59:23.000000 FisheyeWarping-1.0.1/reinstall.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-07 13:59:23.000000 FisheyeWarping-1.0.1/reinstall.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-07 13:59:34.749175 FisheyeWarping-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-07 13:59:23.000000 FisheyeWarping-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:34.741175 FisheyeWarping-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:34.745175 FisheyeWarping-1.0.1/src/FisheyeWarping.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-05-07 13:59:34.000000 FisheyeWarping-1.0.1/src/FisheyeWarping.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-07 13:59:34.000000 FisheyeWarping-1.0.1/src/FisheyeWarping.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 13:59:34.000000 FisheyeWarping-1.0.1/src/FisheyeWarping.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-07 13:59:34.000000 FisheyeWarping-1.0.1/src/FisheyeWarping.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-07 13:59:34.000000 FisheyeWarping-1.0.1/src/FisheyeWarping.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 13:59:34.000000 FisheyeWarping-1.0.1/src/FisheyeWarping.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:34.749175 FisheyeWarping-1.0.1/src/fisheyewarping/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-07 13:59:23.000000 FisheyeWarping-1.0.1/src/fisheyewarping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-05-07 13:59:23.000000 FisheyeWarping-1.0.1/src/fisheyewarping/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12085 2023-05-07 13:59:23.000000 FisheyeWarping-1.0.1/src/fisheyewarping/fisheyewarping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:59:34.749175 FisheyeWarping-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-07 13:59:23.000000 FisheyeWarping-1.0.1/tests/test_fisheye_warping.py
```

### Comparing `FisheyeWarping-1.0.0/LICENSE` & `FisheyeWarping-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FisheyeWarping-1.0.0/PKG-INFO` & `FisheyeWarping-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FisheyeWarping
-Version: 1.0.0
+Version: 1.0.1
 Summary: Dewarp top-down fisheye image to panorama and rewarp panorama to fisheye image.
 Home-page: https://github.com/NatLee/fisheye-warping
 Author: Nat Lee
 Author-email: natlee.work@gmail.com
 Project-URL: Documentation, https://github.com/NatLee/fisheye-warping
 Project-URL: Bug Reports, https://github.com/NatLee/fisheye-warping/issues
 Project-URL: Source Code, https://github.com/NatLee/fisheye-warping
@@ -28,17 +28,17 @@
 License-File: LICENSE
 
 <div align="center" style="text-align: center">
 
 # **Fisheye Warping**
 
 <p style="text-align: center">
-  <img align="center" src="./doc/101-panorama.jpg" alt="Panorama" width="70%" height="100%">
+  <img align="center" src="https://github.com/NatLee/fisheye-warping/raw/main/doc/101-panorama.jpg" alt="Panorama" width="70%" height="100%">
   <div></div>
-  <img align="center" src="./doc/101-fisheye.jpg" alt="Fisheye" width="40%" height="40%">
+  <img align="center" src="https://github.com/NatLee/fisheye-warping/raw/main/doc/101-fisheye.jpg" alt="Fisheye" width="40%" height="40%">
 </p>
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/FisheyeWarping.svg)](https://pypi.python.org/pypi/FisheyeWarping/) [![PyPI implementation](https://img.shields.io/pypi/implementation/FisheyeWarping.svg)](https://pypi.python.org/pypi/FisheyeWarping/)
 
 [![Test](https://github.com/NatLee/fisheye-warping/actions/workflows/test.yml/badge.svg)](https://github.com/NatLee/Eagle-Wrappger/actions/workflows/test.yml) [![Release](https://github.com/NatLee/fisheye-warping/actions/workflows/release.yml/badge.svg)](https://github.com/NatLee/fisheye-warping/actions/workflows/release.yml)
 
 [![PyPI status](https://img.shields.io/pypi/status/FisheyeWarping.svg)](https://pypi.python.org/pypi/FisheyeWarping/) [![PyPI license](https://img.shields.io/pypi/l/FisheyeWarping.svg)](https://pypi.python.org/pypi/FisheyeWarping/)
@@ -55,14 +55,16 @@
 
 ## Installation
 
 ```bash
 pip install FisheyeWarping
 ```
 
+Check it in [Pypi](https://pypi.org/project/FisheyeWarping/)
+
 ## Usage
 
 ```bash
 fisheyewarping --help
 ```
 
 ```
@@ -176,21 +178,21 @@
 > The source of mesh image is from (http://paulbourke.net/dome/fish2/).
 
 Here is the mesh image for this tool, it shows the transformation from the original fisheye image to the panorama image.
 
 - Before - **Fisheye**
 
 <div align="center" style="text-align: center">
-<img align="center" src="./doc/mesh-fisheye.jpg" alt="Fisheye" width="40%" height="40%">
+<img align="center" src="https://github.com/NatLee/fisheye-warping/raw/main/doc/mesh-fisheye.jpg" alt="Fisheye" width="40%" height="40%">
 </div>
 
 - After - **Panorama**
 
 <div align="center" style="text-align: center">
-<img align="center" src="./doc/mesh-panorama.jpg" alt="Panorama" width="70%" height="100%">
+<img align="center" src="https://github.com/NatLee/fisheye-warping/raw/main/doc/mesh-panorama.jpg" alt="Panorama" width="70%" height="100%">
 </div>
 
 
 ## Contributor
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
```

### Comparing `FisheyeWarping-1.0.0/README.md` & `FisheyeWarping-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <div align="center" style="text-align: center">
 
 # **Fisheye Warping**
 
 <p style="text-align: center">
-  <img align="center" src="./doc/101-panorama.jpg" alt="Panorama" width="70%" height="100%">
+  <img align="center" src="https://github.com/NatLee/fisheye-warping/raw/main/doc/101-panorama.jpg" alt="Panorama" width="70%" height="100%">
   <div></div>
-  <img align="center" src="./doc/101-fisheye.jpg" alt="Fisheye" width="40%" height="40%">
+  <img align="center" src="https://github.com/NatLee/fisheye-warping/raw/main/doc/101-fisheye.jpg" alt="Fisheye" width="40%" height="40%">
 </p>
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/FisheyeWarping.svg)](https://pypi.python.org/pypi/FisheyeWarping/) [![PyPI implementation](https://img.shields.io/pypi/implementation/FisheyeWarping.svg)](https://pypi.python.org/pypi/FisheyeWarping/)
 
 [![Test](https://github.com/NatLee/fisheye-warping/actions/workflows/test.yml/badge.svg)](https://github.com/NatLee/Eagle-Wrappger/actions/workflows/test.yml) [![Release](https://github.com/NatLee/fisheye-warping/actions/workflows/release.yml/badge.svg)](https://github.com/NatLee/fisheye-warping/actions/workflows/release.yml)
 
 [![PyPI status](https://img.shields.io/pypi/status/FisheyeWarping.svg)](https://pypi.python.org/pypi/FisheyeWarping/) [![PyPI license](https://img.shields.io/pypi/l/FisheyeWarping.svg)](https://pypi.python.org/pypi/FisheyeWarping/)
@@ -26,14 +26,16 @@
 
 ## Installation
 
 ```bash
 pip install FisheyeWarping
 ```
 
+Check it in [Pypi](https://pypi.org/project/FisheyeWarping/)
+
 ## Usage
 
 ```bash
 fisheyewarping --help
 ```
 
 ```
@@ -147,21 +149,21 @@
 > The source of mesh image is from (http://paulbourke.net/dome/fish2/).
 
 Here is the mesh image for this tool, it shows the transformation from the original fisheye image to the panorama image.
 
 - Before - **Fisheye**
 
 <div align="center" style="text-align: center">
-<img align="center" src="./doc/mesh-fisheye.jpg" alt="Fisheye" width="40%" height="40%">
+<img align="center" src="https://github.com/NatLee/fisheye-warping/raw/main/doc/mesh-fisheye.jpg" alt="Fisheye" width="40%" height="40%">
 </div>
 
 - After - **Panorama**
 
 <div align="center" style="text-align: center">
-<img align="center" src="./doc/mesh-panorama.jpg" alt="Panorama" width="70%" height="100%">
+<img align="center" src="https://github.com/NatLee/fisheye-warping/raw/main/doc/mesh-panorama.jpg" alt="Panorama" width="70%" height="100%">
 </div>
 
 
 ## Contributor
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
```

### Comparing `FisheyeWarping-1.0.0/doc/101-fisheye.jpg` & `FisheyeWarping-1.0.1/doc/101-fisheye.jpg`

 * *Files identical despite different names*

### Comparing `FisheyeWarping-1.0.0/doc/101-panorama.jpg` & `FisheyeWarping-1.0.1/doc/101-panorama.jpg`

 * *Files identical despite different names*

### Comparing `FisheyeWarping-1.0.0/doc/mesh-fisheye.jpg` & `FisheyeWarping-1.0.1/doc/mesh-fisheye.jpg`

 * *Files identical despite different names*

### Comparing `FisheyeWarping-1.0.0/doc/mesh-panorama.jpg` & `FisheyeWarping-1.0.1/doc/mesh-panorama.jpg`

 * *Files identical despite different names*

### Comparing `FisheyeWarping-1.0.0/setup.py` & `FisheyeWarping-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `FisheyeWarping-1.0.0/src/FisheyeWarping.egg-info/PKG-INFO` & `FisheyeWarping-1.0.1/src/FisheyeWarping.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FisheyeWarping
-Version: 1.0.0
+Version: 1.0.1
 Summary: Dewarp top-down fisheye image to panorama and rewarp panorama to fisheye image.
 Home-page: https://github.com/NatLee/fisheye-warping
 Author: Nat Lee
 Author-email: natlee.work@gmail.com
 Project-URL: Documentation, https://github.com/NatLee/fisheye-warping
 Project-URL: Bug Reports, https://github.com/NatLee/fisheye-warping/issues
 Project-URL: Source Code, https://github.com/NatLee/fisheye-warping
@@ -28,17 +28,17 @@
 License-File: LICENSE
 
 <div align="center" style="text-align: center">
 
 # **Fisheye Warping**
 
 <p style="text-align: center">
-  <img align="center" src="./doc/101-panorama.jpg" alt="Panorama" width="70%" height="100%">
+  <img align="center" src="https://github.com/NatLee/fisheye-warping/raw/main/doc/101-panorama.jpg" alt="Panorama" width="70%" height="100%">
   <div></div>
-  <img align="center" src="./doc/101-fisheye.jpg" alt="Fisheye" width="40%" height="40%">
+  <img align="center" src="https://github.com/NatLee/fisheye-warping/raw/main/doc/101-fisheye.jpg" alt="Fisheye" width="40%" height="40%">
 </p>
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/FisheyeWarping.svg)](https://pypi.python.org/pypi/FisheyeWarping/) [![PyPI implementation](https://img.shields.io/pypi/implementation/FisheyeWarping.svg)](https://pypi.python.org/pypi/FisheyeWarping/)
 
 [![Test](https://github.com/NatLee/fisheye-warping/actions/workflows/test.yml/badge.svg)](https://github.com/NatLee/Eagle-Wrappger/actions/workflows/test.yml) [![Release](https://github.com/NatLee/fisheye-warping/actions/workflows/release.yml/badge.svg)](https://github.com/NatLee/fisheye-warping/actions/workflows/release.yml)
 
 [![PyPI status](https://img.shields.io/pypi/status/FisheyeWarping.svg)](https://pypi.python.org/pypi/FisheyeWarping/) [![PyPI license](https://img.shields.io/pypi/l/FisheyeWarping.svg)](https://pypi.python.org/pypi/FisheyeWarping/)
@@ -55,14 +55,16 @@
 
 ## Installation
 
 ```bash
 pip install FisheyeWarping
 ```
 
+Check it in [Pypi](https://pypi.org/project/FisheyeWarping/)
+
 ## Usage
 
 ```bash
 fisheyewarping --help
 ```
 
 ```
@@ -176,21 +178,21 @@
 > The source of mesh image is from (http://paulbourke.net/dome/fish2/).
 
 Here is the mesh image for this tool, it shows the transformation from the original fisheye image to the panorama image.
 
 - Before - **Fisheye**
 
 <div align="center" style="text-align: center">
-<img align="center" src="./doc/mesh-fisheye.jpg" alt="Fisheye" width="40%" height="40%">
+<img align="center" src="https://github.com/NatLee/fisheye-warping/raw/main/doc/mesh-fisheye.jpg" alt="Fisheye" width="40%" height="40%">
 </div>
 
 - After - **Panorama**
 
 <div align="center" style="text-align: center">
-<img align="center" src="./doc/mesh-panorama.jpg" alt="Panorama" width="70%" height="100%">
+<img align="center" src="https://github.com/NatLee/fisheye-warping/raw/main/doc/mesh-panorama.jpg" alt="Panorama" width="70%" height="100%">
 </div>
 
 
 ## Contributor
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
```

### Comparing `FisheyeWarping-1.0.0/src/FisheyeWarping.egg-info/SOURCES.txt` & `FisheyeWarping-1.0.1/src/FisheyeWarping.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FisheyeWarping-1.0.0/src/fisheyewarping/cli.py` & `FisheyeWarping-1.0.1/src/fisheyewarping/cli.py`

 * *Files identical despite different names*

### Comparing `FisheyeWarping-1.0.0/src/fisheyewarping/fisheyewarping.py` & `FisheyeWarping-1.0.1/src/fisheyewarping/fisheyewarping.py`

 * *Files identical despite different names*

