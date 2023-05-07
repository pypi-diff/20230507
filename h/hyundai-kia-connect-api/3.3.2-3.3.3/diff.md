# Comparing `tmp/hyundai_kia_connect_api-3.3.2.tar.gz` & `tmp/hyundai_kia_connect_api-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyundai_kia_connect_api-3.3.2.tar", last modified: Sat May  6 21:35:37 2023, max compression
+gzip compressed data, was "hyundai_kia_connect_api-3.3.3.tar", last modified: Sun May  7 01:49:16 2023, max compression
```

## Comparing `hyundai_kia_connect_api-3.3.2.tar` & `hyundai_kia_connect_api-3.3.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:35:37.266702 hyundai_kia_connect_api-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-06 21:35:37.266702 hyundai_kia_connect_api-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:35:37.258702 hyundai_kia_connect_api-3.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:35:37.266702 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/ApiImpl.py
--rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/KiaUvoAPIUSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    30696 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/KiaUvoApiCA.py
--rw-r--r--   0 runner    (1001) docker     (123)    51311 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/KiaUvoApiCN.py
--rw-r--r--   0 runner    (1001) docker     (123)    53887 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/KiaUvoApiEU.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/Vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/VehicleManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:35:37.266702 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-06 21:35:37.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-06 21:35:37.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 21:35:37.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 21:35:37.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-06 21:35:37.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-06 21:35:37.000000 hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-06 21:35:37.266702 hyundai_kia_connect_api-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-06 21:35:22.000000 hyundai_kia_connect_api-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:35:37.266702 hyundai_kia_connect_api-3.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/tests/ca_login_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/tests/eu_check_response_for_errors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-06 21:34:46.000000 hyundai_kia_connect_api-3.3.2/tests/eu_login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:49:16.471551 hyundai_kia_connect_api-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-07 01:49:16.471551 hyundai_kia_connect_api-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:49:16.471551 hyundai_kia_connect_api-3.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:49:16.471551 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/ApiImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/KiaUvoAPIUSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29918 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/KiaUvoApiCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51311 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/KiaUvoApiCN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53887 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/KiaUvoApiEU.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/Vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/VehicleManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:49:16.471551 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-07 01:49:16.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-07 01:49:16.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 01:49:16.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 01:49:16.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-07 01:49:16.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 01:49:16.000000 hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-07 01:49:16.475551 hyundai_kia_connect_api-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-07 01:49:05.000000 hyundai_kia_connect_api-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:49:16.471551 hyundai_kia_connect_api-3.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/tests/ca_login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/tests/eu_check_response_for_errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-07 01:48:41.000000 hyundai_kia_connect_api-3.3.3/tests/eu_login_test.py
```

### Comparing `hyundai_kia_connect_api-3.3.2/CONTRIBUTING.rst` & `hyundai_kia_connect_api-3.3.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/LICENSE` & `hyundai_kia_connect_api-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/PKG-INFO` & `hyundai_kia_connect_api-3.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyundai_kia_connect_api
-Version: 3.3.2
+Version: 3.3.3
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/fuatakgun/hyundai_kia_connect_api
 Author: Fuat Akgun
 Author-email: fuatakgun@gmail.com
 License: MIT license
 Keywords: hyundai_kia_connect_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hyundai_kia_connect_api-3.3.2/README.rst` & `hyundai_kia_connect_api-3.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/docs/Makefile` & `hyundai_kia_connect_api-3.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/docs/conf.py` & `hyundai_kia_connect_api-3.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/docs/installation.rst` & `hyundai_kia_connect_api-3.3.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/docs/make.bat` & `hyundai_kia_connect_api-3.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/ApiImpl.py` & `hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/ApiImpl.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py` & `hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/KiaUvoAPIUSA.py` & `hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/KiaUvoAPIUSA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/KiaUvoApiCA.py` & `hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/KiaUvoApiCA.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,52 +30,33 @@
 from .exceptions import AuthenticationError, APIError
 from .utils import (
     get_child_value,
     get_hex_temp_into_index,
     get_index_into_hex_temp,
 )
 
-from requests.adapters import HTTPAdapter
-from requests.packages.urllib3.util.ssl_ import create_urllib3_context
+import ssl
+import urllib3
 
-CIPHERS = "DEFAULT:!aNULL:!eNULL:!MD5:!3DES:!DES:!RC4:!IDEA:!SEED:!aDSS:!SRP:!PSK"
+CIPHERS = "DEFAULT@SECLEVEL=1"
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class cipherAdapter(HTTPAdapter):
+class cipherAdapter(requests.adapters.HTTPAdapter):
     """
     A HTTPAdapter that re-enables poor ciphers required by Hyundai.
     """
 
-    def init_poolmanager(self, *args, **kwargs):
-        context = create_urllib3_context(ciphers=CIPHERS)
-        kwargs["ssl_context"] = context
-        return super().init_poolmanager(*args, **kwargs)
-
-    def proxy_manager_for(self, *args, **kwargs):
-        context = create_urllib3_context(ciphers=CIPHERS)
-        kwargs["ssl_context"] = context
-        return super().proxy_manager_for(*args, **kwargs)
-
-
-class cipherAdapter(HTTPAdapter):
-    """
-    A HTTPAdapter that re-enables poor ciphers required by Hyundai.
-    """
-
-    def init_poolmanager(self, *args, **kwargs):
-        context = create_urllib3_context(ciphers=CIPHERS)
-        kwargs["ssl_context"] = context
-        return super().init_poolmanager(*args, **kwargs)
-
-    def proxy_manager_for(self, *args, **kwargs):
-        context = create_urllib3_context(ciphers=CIPHERS)
-        kwargs["ssl_context"] = context
-        return super().proxy_manager_for(*args, **kwargs)
+    def init_poolmanager(self, connections, maxsize, block=False):
+        context = ssl.create_default_context()
+        context.set_ciphers(CIPHERS)
+        self.poolmanager = urllib3.poolmanager.PoolManager(
+            ssl_version=ssl.PROTOCOL_TLS,
+            ssl_context=context)
 
 
 class KiaUvoApiCA(ApiImpl):
     """KiaUvoApiCA"""
 
     temperature_range_c_old = [x * 0.5 for x in range(32, 64)]
     temperature_range_c_new = [x * 0.5 for x in range(28, 64)]
```

### Comparing `hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/KiaUvoApiCN.py` & `hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/KiaUvoApiCN.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/KiaUvoApiEU.py` & `hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/KiaUvoApiEU.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/Vehicle.py` & `hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/Vehicle.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/VehicleManager.py` & `hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/VehicleManager.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/const.py` & `hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/const.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/exceptions.py` & `hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api/utils.py` & `hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api/utils.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api.egg-info/PKG-INFO` & `hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyundai-kia-connect-api
-Version: 3.3.2
+Version: 3.3.3
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/fuatakgun/hyundai_kia_connect_api
 Author: Fuat Akgun
 Author-email: fuatakgun@gmail.com
 License: MIT license
 Keywords: hyundai_kia_connect_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hyundai_kia_connect_api-3.3.2/hyundai_kia_connect_api.egg-info/SOURCES.txt` & `hyundai_kia_connect_api-3.3.3/hyundai_kia_connect_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/setup.py` & `hyundai_kia_connect_api-3.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     name="hyundai_kia_connect_api",
     packages=find_packages(
         include=["hyundai_kia_connect_api", "hyundai_kia_connect_api.*"]
     ),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/fuatakgun/hyundai_kia_connect_api",
-    version="3.3.2",
+    version="3.3.3",
     zip_safe=False,
 )
```

### Comparing `hyundai_kia_connect_api-3.3.2/tests/ca_login_test.py` & `hyundai_kia_connect_api-3.3.3/tests/ca_login_test.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.2/tests/eu_check_response_for_errors_test.py` & `hyundai_kia_connect_api-3.3.3/tests/eu_check_response_for_errors_test.py`

 * *Files identical despite different names*

