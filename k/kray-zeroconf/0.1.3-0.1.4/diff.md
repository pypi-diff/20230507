# Comparing `tmp/kray_zeroconf-0.1.3.tar.gz` & `tmp/kray_zeroconf-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kray_zeroconf-0.1.3.tar", last modified: Sun May  7 16:27:24 2023, max compression
+gzip compressed data, was "kray_zeroconf-0.1.4.tar", last modified: Sun May  7 16:28:42 2023, max compression
```

## Comparing `kray_zeroconf-0.1.3.tar` & `kray_zeroconf-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)        0 2023-05-07 16:27:24.990540 kray_zeroconf-0.1.3/
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)     1047 2023-05-07 04:01:27.000000 kray_zeroconf-0.1.3/LICENSE
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      869 2023-05-07 16:27:24.990540 kray_zeroconf-0.1.3/PKG-INFO
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      176 2023-05-07 04:01:41.000000 kray_zeroconf-0.1.3/README.md
-drwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)        0 2023-05-07 16:27:24.990540 kray_zeroconf-0.1.3/kray_zeroconf.egg-info/
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      869 2023-05-07 16:27:24.000000 kray_zeroconf-0.1.3/kray_zeroconf.egg-info/PKG-INFO
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      379 2023-05-07 16:27:24.000000 kray_zeroconf-0.1.3/kray_zeroconf.egg-info/SOURCES.txt
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)        1 2023-05-07 16:27:24.000000 kray_zeroconf-0.1.3/kray_zeroconf.egg-info/dependency_links.txt
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)        1 2023-05-07 15:18:42.000000 kray_zeroconf-0.1.3/kray_zeroconf.egg-info/not-zip-safe
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)       58 2023-05-07 16:27:24.000000 kray_zeroconf-0.1.3/kray_zeroconf.egg-info/requires.txt
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)        6 2023-05-07 16:27:24.000000 kray_zeroconf-0.1.3/kray_zeroconf.egg-info/top_level.txt
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      624 2023-05-07 15:54:28.000000 kray_zeroconf-0.1.3/pyproject.toml
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)       38 2023-05-07 16:27:24.990540 kray_zeroconf-0.1.3/setup.cfg
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      531 2023-05-07 16:27:06.000000 kray_zeroconf-0.1.3/setup.py
-drwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)        0 2023-05-07 16:27:24.990540 kray_zeroconf-0.1.3/utils/
--rw-r--r--   0 kray-l7   (1000) dockershare  (1499)        0 2023-05-07 15:45:44.000000 kray_zeroconf-0.1.3/utils/__init__.py
--rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)     7183 2023-05-07 16:26:49.000000 kray_zeroconf-0.1.3/utils/parse_configs.py
--rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)      873 2023-05-07 03:57:36.000000 kray_zeroconf-0.1.3/utils/pre_process_configs.py
--rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)      709 2023-05-07 03:57:36.000000 kray_zeroconf-0.1.3/utils/stringcalc.py
--rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)     1369 2023-05-07 03:57:36.000000 kray_zeroconf-0.1.3/utils/zc_config.py
--rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)    12100 2023-05-07 15:47:54.000000 kray_zeroconf-0.1.3/zeroconf
+drwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)        0 2023-05-07 16:28:42.286389 kray_zeroconf-0.1.4/
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)     1047 2023-05-07 04:01:27.000000 kray_zeroconf-0.1.4/LICENSE
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      869 2023-05-07 16:28:42.286389 kray_zeroconf-0.1.4/PKG-INFO
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      176 2023-05-07 04:01:41.000000 kray_zeroconf-0.1.4/README.md
+drwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)        0 2023-05-07 16:28:42.282389 kray_zeroconf-0.1.4/kray_zeroconf.egg-info/
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      869 2023-05-07 16:28:42.000000 kray_zeroconf-0.1.4/kray_zeroconf.egg-info/PKG-INFO
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      379 2023-05-07 16:28:42.000000 kray_zeroconf-0.1.4/kray_zeroconf.egg-info/SOURCES.txt
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)        1 2023-05-07 16:28:42.000000 kray_zeroconf-0.1.4/kray_zeroconf.egg-info/dependency_links.txt
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)        1 2023-05-07 15:18:42.000000 kray_zeroconf-0.1.4/kray_zeroconf.egg-info/not-zip-safe
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)       63 2023-05-07 16:28:42.000000 kray_zeroconf-0.1.4/kray_zeroconf.egg-info/requires.txt
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)        6 2023-05-07 16:28:42.000000 kray_zeroconf-0.1.4/kray_zeroconf.egg-info/top_level.txt
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      624 2023-05-07 15:54:28.000000 kray_zeroconf-0.1.4/pyproject.toml
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)       38 2023-05-07 16:28:42.286389 kray_zeroconf-0.1.4/setup.cfg
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)      537 2023-05-07 16:28:33.000000 kray_zeroconf-0.1.4/setup.py
+drwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)        0 2023-05-07 16:28:42.286389 kray_zeroconf-0.1.4/utils/
+-rw-r--r--   0 kray-l7   (1000) dockershare  (1499)        0 2023-05-07 15:45:44.000000 kray_zeroconf-0.1.4/utils/__init__.py
+-rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)     7183 2023-05-07 16:26:49.000000 kray_zeroconf-0.1.4/utils/parse_configs.py
+-rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)      873 2023-05-07 03:57:36.000000 kray_zeroconf-0.1.4/utils/pre_process_configs.py
+-rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)      709 2023-05-07 03:57:36.000000 kray_zeroconf-0.1.4/utils/stringcalc.py
+-rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)     1369 2023-05-07 03:57:36.000000 kray_zeroconf-0.1.4/utils/zc_config.py
+-rwxr-xr-x   0 kray-l7   (1000) dockershare  (1499)    12100 2023-05-07 15:47:54.000000 kray_zeroconf-0.1.4/zeroconf
```

### Comparing `kray_zeroconf-0.1.3/LICENSE` & `kray_zeroconf-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kray_zeroconf-0.1.3/PKG-INFO` & `kray_zeroconf-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kray_zeroconf
-Version: 0.1.3
+Version: 0.1.4
 Summary: Zeroconf auto networking configuration tool for Kray Works DevOps
 Home-page: https://gitlab-ua.kray.technology/lanceoflife/kray-zeroconf
 Author: Dmytro Surdu
 Author-email: Dmytro Surdu <dmytro.surdu@kray.technology>
 Project-URL: Homepage, https://gitlab-ua.kray.technology/lanceoflife/kray-zeroconf
 Project-URL: Bug Tracker, https://gitlab-ua.kray.technology/lanceoflife/kray-zeroconf/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kray_zeroconf-0.1.3/kray_zeroconf.egg-info/PKG-INFO` & `kray_zeroconf-0.1.4/kray_zeroconf.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kray-zeroconf
-Version: 0.1.3
+Version: 0.1.4
 Summary: Zeroconf auto networking configuration tool for Kray Works DevOps
 Home-page: https://gitlab-ua.kray.technology/lanceoflife/kray-zeroconf
 Author: Dmytro Surdu
 Author-email: Dmytro Surdu <dmytro.surdu@kray.technology>
 Project-URL: Homepage, https://gitlab-ua.kray.technology/lanceoflife/kray-zeroconf
 Project-URL: Bug Tracker, https://gitlab-ua.kray.technology/lanceoflife/kray-zeroconf/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kray_zeroconf-0.1.3/pyproject.toml` & `kray_zeroconf-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kray_zeroconf-0.1.3/setup.py` & `kray_zeroconf-0.1.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup,find_packages
 
 setup(name='kray-zeroconf',
-      version='0.1.3',
+      version='0.1.4',
       description='Zeroconf auto networking configuration tool for Kray Works DevOps',
       url='https://gitlab-ua.kray.technology/lanceoflife/kray-zeroconf',
       author='Dmytro Surdu',
       author_email='dmytro.surdu@kray.technology',
       scripts=['zeroconf'],
       install_requires=[
-          "setuptools>=61.0","zeroconf == 0.24.4","pyyaml","netifaces","psutil",
+          "setuptools>=61.0","zeroconf == 0.24.4","pyyaml","netifaces","psutil","lxml"
       ],
       packages=find_packages(),
       zip_safe=False)
```

### Comparing `kray_zeroconf-0.1.3/utils/parse_configs.py` & `kray_zeroconf-0.1.4/utils/parse_configs.py`

 * *Files identical despite different names*

### Comparing `kray_zeroconf-0.1.3/utils/pre_process_configs.py` & `kray_zeroconf-0.1.4/utils/pre_process_configs.py`

 * *Files identical despite different names*

### Comparing `kray_zeroconf-0.1.3/utils/stringcalc.py` & `kray_zeroconf-0.1.4/utils/stringcalc.py`

 * *Files identical despite different names*

### Comparing `kray_zeroconf-0.1.3/utils/zc_config.py` & `kray_zeroconf-0.1.4/utils/zc_config.py`

 * *Files identical despite different names*

### Comparing `kray_zeroconf-0.1.3/zeroconf` & `kray_zeroconf-0.1.4/zeroconf`

 * *Files identical despite different names*

