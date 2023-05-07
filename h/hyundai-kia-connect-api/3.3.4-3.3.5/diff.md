# Comparing `tmp/hyundai_kia_connect_api-3.3.4.tar.gz` & `tmp/hyundai_kia_connect_api-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyundai_kia_connect_api-3.3.4.tar", last modified: Sun May  7 01:58:38 2023, max compression
+gzip compressed data, was "hyundai_kia_connect_api-3.3.5.tar", last modified: Sun May  7 02:20:40 2023, max compression
```

## Comparing `hyundai_kia_connect_api-3.3.4.tar` & `hyundai_kia_connect_api-3.3.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:58:38.863340 hyundai_kia_connect_api-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-07 01:58:38.863340 hyundai_kia_connect_api-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:58:38.863340 hyundai_kia_connect_api-3.3.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:58:38.863340 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/ApiImpl.py
--rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/KiaUvoAPIUSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    29949 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/KiaUvoApiCA.py
--rw-r--r--   0 runner    (1001) docker     (123)    51311 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/KiaUvoApiCN.py
--rw-r--r--   0 runner    (1001) docker     (123)    53887 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/KiaUvoApiEU.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/Vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/VehicleManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:58:38.863340 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-07 01:58:38.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-07 01:58:38.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 01:58:38.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 01:58:38.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-07 01:58:38.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 01:58:38.000000 hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-07 01:58:38.867341 hyundai_kia_connect_api-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-07 01:58:27.000000 hyundai_kia_connect_api-3.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:58:38.863340 hyundai_kia_connect_api-3.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/tests/ca_login_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/tests/eu_check_response_for_errors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-07 01:57:55.000000 hyundai_kia_connect_api-3.3.4/tests/eu_login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:20:40.959416 hyundai_kia_connect_api-3.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-07 02:20:40.959416 hyundai_kia_connect_api-3.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:20:40.959416 hyundai_kia_connect_api-3.3.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:20:40.959416 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/ApiImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/KiaUvoAPIUSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29988 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/KiaUvoApiCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51311 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/KiaUvoApiCN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53887 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/KiaUvoApiEU.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/Vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/VehicleManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:20:40.959416 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-07 02:20:40.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-07 02:20:40.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:20:40.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:20:40.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-07 02:20:40.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 02:20:40.000000 hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-07 02:20:40.959416 hyundai_kia_connect_api-3.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-07 02:20:29.000000 hyundai_kia_connect_api-3.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:20:40.959416 hyundai_kia_connect_api-3.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/tests/ca_login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/tests/eu_check_response_for_errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-07 02:20:06.000000 hyundai_kia_connect_api-3.3.5/tests/eu_login_test.py
```

### Comparing `hyundai_kia_connect_api-3.3.4/CONTRIBUTING.rst` & `hyundai_kia_connect_api-3.3.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/LICENSE` & `hyundai_kia_connect_api-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/PKG-INFO` & `hyundai_kia_connect_api-3.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyundai_kia_connect_api
-Version: 3.3.4
+Version: 3.3.5
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/fuatakgun/hyundai_kia_connect_api
 Author: Fuat Akgun
 Author-email: fuatakgun@gmail.com
 License: MIT license
 Keywords: hyundai_kia_connect_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hyundai_kia_connect_api-3.3.4/README.rst` & `hyundai_kia_connect_api-3.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/docs/Makefile` & `hyundai_kia_connect_api-3.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/docs/conf.py` & `hyundai_kia_connect_api-3.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/docs/installation.rst` & `hyundai_kia_connect_api-3.3.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/docs/make.bat` & `hyundai_kia_connect_api-3.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/ApiImpl.py` & `hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/ApiImpl.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py` & `hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/KiaUvoAPIUSA.py` & `hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/KiaUvoAPIUSA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/KiaUvoApiCA.py` & `hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/KiaUvoApiCA.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,28 +33,28 @@
     get_hex_temp_into_index,
     get_index_into_hex_temp,
 )
 
 import ssl
 import urllib3
 
-CIPHERS = "DEFAULT@SECLEVEL=1"
+CIPHERS = "ALL:@SECLEVEL=0"
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class cipherAdapter(requests.adapters.HTTPAdapter):
     """
     A HTTPAdapter that re-enables poor ciphers required by Hyundai.
     """
 
     def init_poolmanager(self, connections, maxsize, block=False):
         context = ssl.create_default_context()
         context.set_ciphers(CIPHERS)
-        context.options |= 0x4
+        context.options |= getattr(ssl, "OP_LEGACY_SERVER_CONNECT", 0x4)
         self.poolmanager = urllib3.poolmanager.PoolManager(
             ssl_version=ssl.PROTOCOL_TLS,
             ssl_context=context)
 
 
 class KiaUvoApiCA(ApiImpl):
     """KiaUvoApiCA"""
```

### Comparing `hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/KiaUvoApiCN.py` & `hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/KiaUvoApiCN.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/KiaUvoApiEU.py` & `hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/KiaUvoApiEU.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/Vehicle.py` & `hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/Vehicle.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/VehicleManager.py` & `hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/VehicleManager.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/const.py` & `hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/const.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/exceptions.py` & `hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api/utils.py` & `hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api/utils.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api.egg-info/PKG-INFO` & `hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyundai-kia-connect-api
-Version: 3.3.4
+Version: 3.3.5
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/fuatakgun/hyundai_kia_connect_api
 Author: Fuat Akgun
 Author-email: fuatakgun@gmail.com
 License: MIT license
 Keywords: hyundai_kia_connect_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hyundai_kia_connect_api-3.3.4/hyundai_kia_connect_api.egg-info/SOURCES.txt` & `hyundai_kia_connect_api-3.3.5/hyundai_kia_connect_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/setup.py` & `hyundai_kia_connect_api-3.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     name="hyundai_kia_connect_api",
     packages=find_packages(
         include=["hyundai_kia_connect_api", "hyundai_kia_connect_api.*"]
     ),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/fuatakgun/hyundai_kia_connect_api",
-    version="3.3.4",
+    version="3.3.5",
     zip_safe=False,
 )
```

### Comparing `hyundai_kia_connect_api-3.3.4/tests/ca_login_test.py` & `hyundai_kia_connect_api-3.3.5/tests/ca_login_test.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.4/tests/eu_check_response_for_errors_test.py` & `hyundai_kia_connect_api-3.3.5/tests/eu_check_response_for_errors_test.py`

 * *Files identical despite different names*

