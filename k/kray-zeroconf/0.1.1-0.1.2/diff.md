# Comparing `tmp/kray_zeroconf-0.1.1.tar.gz` & `tmp/kray_zeroconf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kray_zeroconf-0.1.1.tar", last modified: Sun May  7 15:48:53 2023, max compression
+gzip compressed data, was "kray_zeroconf-0.1.2.tar", last modified: Sun May  7 15:54:36 2023, max compression
```

## Comparing `kray_zeroconf-0.1.1.tar` & `kray_zeroconf-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)        0 2023-05-07 15:48:53.315010 kray_zeroconf-0.1.1/
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)     1047 2023-05-07 04:01:27.000000 kray_zeroconf-0.1.1/LICENSE
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      869 2023-05-07 15:48:53.315010 kray_zeroconf-0.1.1/PKG-INFO
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      176 2023-05-07 04:01:41.000000 kray_zeroconf-0.1.1/README.md
-drwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)        0 2023-05-07 15:48:53.315010 kray_zeroconf-0.1.1/kray_zeroconf.egg-info/
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      869 2023-05-07 15:48:53.000000 kray_zeroconf-0.1.1/kray_zeroconf.egg-info/PKG-INFO
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      379 2023-05-07 15:48:53.000000 kray_zeroconf-0.1.1/kray_zeroconf.egg-info/SOURCES.txt
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)        1 2023-05-07 15:48:53.000000 kray_zeroconf-0.1.1/kray_zeroconf.egg-info/dependency_links.txt
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)        1 2023-05-07 15:18:42.000000 kray_zeroconf-0.1.1/kray_zeroconf.egg-info/not-zip-safe
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)       58 2023-05-07 15:48:53.000000 kray_zeroconf-0.1.1/kray_zeroconf.egg-info/requires.txt
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)        6 2023-05-07 15:48:53.000000 kray_zeroconf-0.1.1/kray_zeroconf.egg-info/top_level.txt
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      723 2023-05-07 15:48:42.000000 kray_zeroconf-0.1.1/pyproject.toml
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)       38 2023-05-07 15:48:53.315010 kray_zeroconf-0.1.1/setup.cfg
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      532 2023-05-07 15:48:37.000000 kray_zeroconf-0.1.1/setup.py
-drwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)        0 2023-05-07 15:48:53.315010 kray_zeroconf-0.1.1/utils/
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)        0 2023-05-07 15:45:44.000000 kray_zeroconf-0.1.1/utils/__init__.py
--rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)     7177 2023-05-07 03:57:36.000000 kray_zeroconf-0.1.1/utils/parse_configs.py
--rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)      873 2023-05-07 03:57:36.000000 kray_zeroconf-0.1.1/utils/pre_process_configs.py
--rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)      709 2023-05-07 03:57:36.000000 kray_zeroconf-0.1.1/utils/stringcalc.py
--rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)     1369 2023-05-07 03:57:36.000000 kray_zeroconf-0.1.1/utils/zc_config.py
--rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)    12100 2023-05-07 15:47:54.000000 kray_zeroconf-0.1.1/zeroconf
+drwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)        0 2023-05-07 15:54:36.354353 kray_zeroconf-0.1.2/
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)     1047 2023-05-07 04:01:27.000000 kray_zeroconf-0.1.2/LICENSE
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      870 2023-05-07 15:54:36.354353 kray_zeroconf-0.1.2/PKG-INFO
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      176 2023-05-07 04:01:41.000000 kray_zeroconf-0.1.2/README.md
+drwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)        0 2023-05-07 15:54:36.354353 kray_zeroconf-0.1.2/kray_zeroconf.egg-info/
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      870 2023-05-07 15:54:36.000000 kray_zeroconf-0.1.2/kray_zeroconf.egg-info/PKG-INFO
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      379 2023-05-07 15:54:36.000000 kray_zeroconf-0.1.2/kray_zeroconf.egg-info/SOURCES.txt
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)        1 2023-05-07 15:54:36.000000 kray_zeroconf-0.1.2/kray_zeroconf.egg-info/dependency_links.txt
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)        1 2023-05-07 15:18:42.000000 kray_zeroconf-0.1.2/kray_zeroconf.egg-info/not-zip-safe
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)       58 2023-05-07 15:54:36.000000 kray_zeroconf-0.1.2/kray_zeroconf.egg-info/requires.txt
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)        6 2023-05-07 15:54:36.000000 kray_zeroconf-0.1.2/kray_zeroconf.egg-info/top_level.txt
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      624 2023-05-07 15:54:28.000000 kray_zeroconf-0.1.2/pyproject.toml
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)       38 2023-05-07 15:54:36.354353 kray_zeroconf-0.1.2/setup.cfg
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      532 2023-05-07 15:52:24.000000 kray_zeroconf-0.1.2/setup.py
+drwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)        0 2023-05-07 15:54:36.354353 kray_zeroconf-0.1.2/utils/
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)        0 2023-05-07 15:45:44.000000 kray_zeroconf-0.1.2/utils/__init__.py
+-rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)     7177 2023-05-07 03:57:36.000000 kray_zeroconf-0.1.2/utils/parse_configs.py
+-rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)      873 2023-05-07 03:57:36.000000 kray_zeroconf-0.1.2/utils/pre_process_configs.py
+-rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)      709 2023-05-07 03:57:36.000000 kray_zeroconf-0.1.2/utils/stringcalc.py
+-rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)     1369 2023-05-07 03:57:36.000000 kray_zeroconf-0.1.2/utils/zc_config.py
+-rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)    12100 2023-05-07 15:47:54.000000 kray_zeroconf-0.1.2/zeroconf
```

### Comparing `kray_zeroconf-0.1.1/LICENSE` & `kray_zeroconf-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kray_zeroconf-0.1.1/PKG-INFO` & `kray_zeroconf-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kray_zeroconf
-Version: 0.1.1
-Summary: Zeroconf auto networking configuration tool for Kray Works DevOps
+Version: 0.1.2
+Summary: TZeroconf auto networking configuration tool for Kray Works DevOps
 Home-page: https://gitlab-ua.kray.technology/lanceoflife/kray-zeroconf
 Author: Dmytro Surdu
 Author-email: Dmytro Surdu <dmytro.surdu@kray.technology>
 Project-URL: Homepage, https://gitlab-ua.kray.technology/lanceoflife/kray-zeroconf
 Project-URL: Bug Tracker, https://gitlab-ua.kray.technology/lanceoflife/kray-zeroconf/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kray_zeroconf-0.1.1/kray_zeroconf.egg-info/PKG-INFO` & `kray_zeroconf-0.1.2/kray_zeroconf.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kray-zeroconf
-Version: 0.1.1
-Summary: Zeroconf auto networking configuration tool for Kray Works DevOps
+Version: 0.1.2
+Summary: TZeroconf auto networking configuration tool for Kray Works DevOps
 Home-page: https://gitlab-ua.kray.technology/lanceoflife/kray-zeroconf
 Author: Dmytro Surdu
 Author-email: Dmytro Surdu <dmytro.surdu@kray.technology>
 Project-URL: Homepage, https://gitlab-ua.kray.technology/lanceoflife/kray-zeroconf
 Project-URL: Bug Tracker, https://gitlab-ua.kray.technology/lanceoflife/kray-zeroconf/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kray_zeroconf-0.1.1/pyproject.toml` & `kray_zeroconf-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [build-system]
-requires = ["setuptools>=61.0","zeroconf == 0.24.4","pyyaml","netifaces","psutil"]
+requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "kray_zeroconf"
-version = "0.1.1"
+dynamic = ["version", "description","dependencies"]
 authors = [
   { name="Dmytro Surdu", email="dmytro.surdu@kray.technology" },
 ]
-description = "Zeroconf auto networking configuration tool for Kray Works DevOps"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
 ]
```

### Comparing `kray_zeroconf-0.1.1/setup.py` & `kray_zeroconf-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup,find_packages
 
 setup(name='kray-zeroconf',
-      version='0.1.1',
+      version='0.1.2',
       description='TZeroconf auto networking configuration tool for Kray Works DevOps',
       url='https://gitlab-ua.kray.technology/lanceoflife/kray-zeroconf',
       author='Dmytro Surdu',
       author_email='dmytro.surdu@kray.technology',
       scripts=['zeroconf'],
       install_requires=[
           "setuptools>=61.0","zeroconf == 0.24.4","pyyaml","netifaces","psutil",
```

### Comparing `kray_zeroconf-0.1.1/utils/parse_configs.py` & `kray_zeroconf-0.1.2/utils/parse_configs.py`

 * *Files identical despite different names*

### Comparing `kray_zeroconf-0.1.1/utils/pre_process_configs.py` & `kray_zeroconf-0.1.2/utils/pre_process_configs.py`

 * *Files identical despite different names*

### Comparing `kray_zeroconf-0.1.1/utils/stringcalc.py` & `kray_zeroconf-0.1.2/utils/stringcalc.py`

 * *Files identical despite different names*

### Comparing `kray_zeroconf-0.1.1/utils/zc_config.py` & `kray_zeroconf-0.1.2/utils/zc_config.py`

 * *Files identical despite different names*

### Comparing `kray_zeroconf-0.1.1/zeroconf` & `kray_zeroconf-0.1.2/zeroconf`

 * *Files identical despite different names*

