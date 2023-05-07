# Comparing `tmp/nkt_tools-0.0.1.tar.gz` & `tmp/nkt_tools-0.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkt_tools-0.0.1.tar", last modified: Sat May  6 23:10:43 2023, max compression
+gzip compressed data, was "nkt_tools-0.0.1b0.tar", last modified: Sun May  7 03:25:49 2023, max compression
```

## Comparing `nkt_tools-0.0.1.tar` & `nkt_tools-0.0.1b0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 23:10:43.005938 nkt_tools-0.0.1/
--rw-rw-rw-   0        0        0     1094 2023-05-04 02:15:27.000000 nkt_tools-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1333 2023-05-06 23:10:43.004977 nkt_tools-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      770 2023-05-05 20:33:59.000000 nkt_tools-0.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 23:10:43.003982 nkt_tools-0.0.1/nkt_tools.egg-info/
--rw-rw-rw-   0        0        0     1333 2023-05-06 23:10:42.000000 nkt_tools-0.0.1/nkt_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      165 2023-05-06 23:10:42.000000 nkt_tools-0.0.1/nkt_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 23:10:42.000000 nkt_tools-0.0.1/nkt_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-06 23:10:42.000000 nkt_tools-0.0.1/nkt_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      756 2023-05-04 02:24:34.000000 nkt_tools-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 23:10:43.005938 nkt_tools-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 03:25:49.575834 nkt_tools-0.0.1b0/
+-rw-rw-rw-   0        0        0     1094 2023-05-04 02:15:27.000000 nkt_tools-0.0.1b0/LICENSE
+-rw-rw-rw-   0        0        0     1704 2023-05-07 03:25:49.574718 nkt_tools-0.0.1b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1139 2023-05-07 03:19:39.000000 nkt_tools-0.0.1b0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-07 03:25:49.572946 nkt_tools-0.0.1b0/nkt_tools.egg-info/
+-rw-rw-rw-   0        0        0     1704 2023-05-07 03:25:49.000000 nkt_tools-0.0.1b0/nkt_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      165 2023-05-07 03:25:49.000000 nkt_tools-0.0.1b0/nkt_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 03:25:49.000000 nkt_tools-0.0.1b0/nkt_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-07 03:25:49.000000 nkt_tools-0.0.1b0/nkt_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      757 2023-05-07 03:25:23.000000 nkt_tools-0.0.1b0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 03:25:49.575834 nkt_tools-0.0.1b0/setup.cfg
```

### Comparing `nkt_tools-0.0.1/LICENSE` & `nkt_tools-0.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkt_tools-0.0.1/PKG-INFO` & `nkt_tools-0.0.1b0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: nkt_tools
-Version: 0.0.1
+Version: 0.0.1b0
 Summary: Python package for accessing NKT photonics project through NKTPDLL
 Author-email: Briley Bourgeois <bbourge6@stanford.edu>
 Project-URL: Homepage, https://github.com/Dionne-Lab/nkt_tools
 Project-URL: Bug Tracker, https://github.com/Dionne-Lab/nkt_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-# nkt_tools
 This repository contains tools for accessing NKT photonics devices via python through the NKT SDK
 
 nkt_tools turns this:
 
 .. code-block:: python
 
     import NKTP_DLL as nkt
@@ -27,7 +26,21 @@
 .. code-block:: python
 
     from nkt_tools.extreme import Extreme
     laser = Extreme()
     laser.set_emission(True)
 
 nkt_tools is a wrapper around NKT's DLL to provide object oriented interaction with NKT products. NKT Extreme/Fianium lasers and the Varia system are currently supported. Additional systems can be accessed through the DLL by using the registerRead/Write functions within nkt_tools.NKTP_DLL or interested developers can write new modules by following the development notes provided.
+
+**ReadtheDocs Page:**
+https://nkt-tools.readthedocs.io/en/latest/
+
+**PyPI Page:**
+https://pypi.org/project/nkt-tools/
+
+Please also check out my related package, CataLight, which automates data collection and processing for photocatalysis research!
+
+**ReadtheDocs Page:**
+https://catalight.readthedocs.io/en/latest/
+
+**PyPI Page:**
+https://pypi.org/project/catalight/
```

### Comparing `nkt_tools-0.0.1/nkt_tools.egg-info/PKG-INFO` & `nkt_tools-0.0.1b0/nkt_tools.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: nkt-tools
-Version: 0.0.1
+Version: 0.0.1b0
 Summary: Python package for accessing NKT photonics project through NKTPDLL
 Author-email: Briley Bourgeois <bbourge6@stanford.edu>
 Project-URL: Homepage, https://github.com/Dionne-Lab/nkt_tools
 Project-URL: Bug Tracker, https://github.com/Dionne-Lab/nkt_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-# nkt_tools
 This repository contains tools for accessing NKT photonics devices via python through the NKT SDK
 
 nkt_tools turns this:
 
 .. code-block:: python
 
     import NKTP_DLL as nkt
@@ -27,7 +26,21 @@
 .. code-block:: python
 
     from nkt_tools.extreme import Extreme
     laser = Extreme()
     laser.set_emission(True)
 
 nkt_tools is a wrapper around NKT's DLL to provide object oriented interaction with NKT products. NKT Extreme/Fianium lasers and the Varia system are currently supported. Additional systems can be accessed through the DLL by using the registerRead/Write functions within nkt_tools.NKTP_DLL or interested developers can write new modules by following the development notes provided.
+
+**ReadtheDocs Page:**
+https://nkt-tools.readthedocs.io/en/latest/
+
+**PyPI Page:**
+https://pypi.org/project/nkt-tools/
+
+Please also check out my related package, CataLight, which automates data collection and processing for photocatalysis research!
+
+**ReadtheDocs Page:**
+https://catalight.readthedocs.io/en/latest/
+
+**PyPI Page:**
+https://pypi.org/project/catalight/
```

### Comparing `nkt_tools-0.0.1/pyproject.toml` & `nkt_tools-0.0.1b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nkt_tools"
-version = "0.0.1"
+version = "0.0.1b"
 authors = [
   { name="Briley Bourgeois", email="bbourge6@stanford.edu" }
 ]
 description = "Python package for accessing NKT photonics project through NKTPDLL"
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
```

