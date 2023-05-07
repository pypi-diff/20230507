# Comparing `tmp/karcher-home-0.4.2.tar.gz` & `tmp/karcher-home-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karcher-home-0.4.2.tar", last modified: Sun May  7 19:56:56 2023, max compression
+gzip compressed data, was "karcher-home-0.4.3.tar", last modified: Sun May  7 20:13:18 2023, max compression
```

## Comparing `karcher-home-0.4.2.tar` & `karcher-home-0.4.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 19:56:56.311176 karcher-home-0.4.2/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1066 2023-04-23 18:36:52.000000 karcher-home-0.4.2/LICENSE
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1509 2023-05-07 19:56:56.311176 karcher-home-0.4.2/PKG-INFO
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1120 2023-05-07 19:15:47.000000 karcher-home-0.4.2/README.md
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 19:56:56.311176 karcher-home-0.4.2/karcher/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        0 2023-04-26 11:31:28.000000 karcher-home-0.4.2/karcher/__init__.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2147 2023-04-30 14:40:55.000000 karcher-home-0.4.2/karcher/auth.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5326 2023-05-07 19:56:02.000000 karcher-home-0.4.2/karcher/cli.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2287 2023-04-28 20:14:55.000000 karcher-home-0.4.2/karcher/consts.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5705 2023-04-28 20:58:15.000000 karcher-home-0.4.2/karcher/countries.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5060 2023-04-28 20:50:00.000000 karcher-home-0.4.2/karcher/device.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1663 2023-04-28 20:58:33.000000 karcher-home-0.4.2/karcher/exception.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      592 2023-04-26 12:09:03.000000 karcher-home-0.4.2/karcher/identifiers.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)    14764 2023-05-07 19:54:39.000000 karcher-home-0.4.2/karcher/karcher.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      706 2023-04-28 20:53:12.000000 karcher-home-0.4.2/karcher/map.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     7843 2023-04-26 08:16:45.000000 karcher-home-0.4.2/karcher/mapdata_pb2.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3354 2023-04-28 20:53:54.000000 karcher-home-0.4.2/karcher/mqtt.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3305 2023-05-07 19:24:15.000000 karcher-home-0.4.2/karcher/utils.py
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 19:56:56.311176 karcher-home-0.4.2/karcher_home.egg-info/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1509 2023-05-07 19:56:56.000000 karcher-home-0.4.2/karcher_home.egg-info/PKG-INFO
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      514 2023-05-07 19:56:56.000000 karcher-home-0.4.2/karcher_home.egg-info/SOURCES.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        1 2023-05-07 19:56:56.000000 karcher-home-0.4.2/karcher_home.egg-info/dependency_links.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       54 2023-05-07 19:56:56.000000 karcher-home-0.4.2/karcher_home.egg-info/entry_points.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       46 2023-05-07 19:56:56.000000 karcher-home-0.4.2/karcher_home.egg-info/requires.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        8 2023-05-07 19:56:56.000000 karcher-home-0.4.2/karcher_home.egg-info/top_level.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       79 2023-05-07 19:56:56.311176 karcher-home-0.4.2/setup.cfg
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      845 2023-05-07 19:56:46.000000 karcher-home-0.4.2/setup.py
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 19:56:56.311176 karcher-home-0.4.2/tests/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4294 2023-04-23 21:35:44.000000 karcher-home-0.4.2/tests/test_enc.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 20:13:18.294693 karcher-home-0.4.3/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1066 2023-04-23 18:36:52.000000 karcher-home-0.4.3/LICENSE
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1509 2023-05-07 20:13:18.294693 karcher-home-0.4.3/PKG-INFO
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1120 2023-05-07 19:15:47.000000 karcher-home-0.4.3/README.md
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 20:13:18.290692 karcher-home-0.4.3/karcher/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        0 2023-04-26 11:31:28.000000 karcher-home-0.4.3/karcher/__init__.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2147 2023-04-30 14:40:55.000000 karcher-home-0.4.3/karcher/auth.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5292 2023-05-07 20:09:10.000000 karcher-home-0.4.3/karcher/cli.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2446 2023-05-07 20:08:27.000000 karcher-home-0.4.3/karcher/consts.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5705 2023-04-28 20:58:15.000000 karcher-home-0.4.3/karcher/countries.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5060 2023-04-28 20:50:00.000000 karcher-home-0.4.3/karcher/device.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1663 2023-04-28 20:58:33.000000 karcher-home-0.4.3/karcher/exception.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      592 2023-04-26 12:09:03.000000 karcher-home-0.4.3/karcher/identifiers.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)    14942 2023-05-07 20:09:49.000000 karcher-home-0.4.3/karcher/karcher.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      706 2023-04-28 20:53:12.000000 karcher-home-0.4.3/karcher/map.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     7843 2023-04-26 08:16:45.000000 karcher-home-0.4.3/karcher/mapdata_pb2.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3354 2023-04-28 20:53:54.000000 karcher-home-0.4.3/karcher/mqtt.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3305 2023-05-07 19:24:15.000000 karcher-home-0.4.3/karcher/utils.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 20:13:18.294693 karcher-home-0.4.3/karcher_home.egg-info/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1509 2023-05-07 20:13:18.000000 karcher-home-0.4.3/karcher_home.egg-info/PKG-INFO
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      514 2023-05-07 20:13:18.000000 karcher-home-0.4.3/karcher_home.egg-info/SOURCES.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        1 2023-05-07 20:13:18.000000 karcher-home-0.4.3/karcher_home.egg-info/dependency_links.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       54 2023-05-07 20:13:18.000000 karcher-home-0.4.3/karcher_home.egg-info/entry_points.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       46 2023-05-07 20:13:18.000000 karcher-home-0.4.3/karcher_home.egg-info/requires.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        8 2023-05-07 20:13:18.000000 karcher-home-0.4.3/karcher_home.egg-info/top_level.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       79 2023-05-07 20:13:18.294693 karcher-home-0.4.3/setup.cfg
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      845 2023-05-07 20:12:12.000000 karcher-home-0.4.3/setup.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 20:13:18.294693 karcher-home-0.4.3/tests/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4294 2023-04-23 21:35:44.000000 karcher-home-0.4.3/tests/test_enc.py
```

### Comparing `karcher-home-0.4.2/LICENSE` & `karcher-home-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.2/PKG-INFO` & `karcher-home-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: karcher-home
-Version: 0.4.2
+Version: 0.4.3
 Summary: Kärcher Home Robots client
 Home-page: https://github.com/lafriks/python-karcher
-Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.4.2/karcher-home-0.4.2.tar.gz
+Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.4.3/karcher-home-0.4.3.tar.gz
 Author: Lauris BH
 Author-email: lauris@nix.lv
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `karcher-home-0.4.2/README.md` & `karcher-home-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.2/karcher/auth.py` & `karcher-home-0.4.3/karcher/auth.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.2/karcher/cli.py` & `karcher-home-0.4.3/karcher/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import dataclasses
 import json
 import logging
 from functools import wraps
 
 from karcher.exception import KarcherHomeException
 from karcher.karcher import KarcherHome
-from karcher.consts import Region
 
 try:
     from rich import print as echo
 except ImportError:
     echo = click.echo
```

### Comparing `karcher-home-0.4.2/karcher/consts.py` & `karcher-home-0.4.3/karcher/consts.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,7 +112,8 @@
 ]
 
 TENANT_ID = '1528983614213726208'
 PROJECT_TYPE = 'android_iot.karcher'
 PROTOCOL_VERSION = 'v1'
 APP_VERSION_CODE = 10004
 APP_VERSION_NAME = '1.0.4'
+SSL_CERTIFICATE_THUMBPRINT = bytes.fromhex('68:A3:68:92:5D:B3:DE:51:6A:80:64:FD:70:38:A3:49:45:D8:6E:DF:11:33:08:66:2C:87:85:A4:C9:F5:4A:10'.replace(':', ''))
```

### Comparing `karcher-home-0.4.2/karcher/countries.py` & `karcher-home-0.4.3/karcher/countries.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.2/karcher/device.py` & `karcher-home-0.4.3/karcher/device.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.2/karcher/exception.py` & `karcher-home-0.4.3/karcher/exception.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.2/karcher/identifiers.py` & `karcher-home-0.4.3/karcher/identifiers.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.2/karcher/karcher.py` & `karcher-home-0.4.3/karcher/karcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # -----------------------------------------------------------
 # Copyright (c) 2023 Lauris BH
 # SPDX-License-Identifier: MIT
 # -----------------------------------------------------------
 
+import asyncio
 import collections
 import json
 import threading
 from typing import List, Any
 import aiohttp
 import urllib.parse
 
 
 from .auth import Domains, Session
 from .countries import get_country_code, get_region_by_country
 from .consts import (
-    APP_VERSION_CODE, APP_VERSION_NAME, PROJECT_TYPE,
-    PROTOCOL_VERSION, REGION_URLS, ROBOT_PROPERTIES, TENANT_ID,
+    APP_VERSION_CODE, APP_VERSION_NAME, PROJECT_TYPE, PROTOCOL_VERSION,
+    REGION_URLS, ROBOT_PROPERTIES, SSL_CERTIFICATE_THUMBPRINT, TENANT_ID,
     Language, Region
 )
 from .device import Device, DeviceProperties
 from .exception import KarcherHomeAccessDenied, KarcherHomeException, handle_error_code
 from .map import Map
 from .mqtt import MqttClient, get_device_topic_property_get_reply, get_device_topics
 from .utils import (
@@ -28,15 +29,19 @@
 )
 
 
 class KarcherHome:
     """Main class to access Karcher Home Robots API"""
 
     @classmethod
-    async def create(cls, country: str = 'GB', language: Language = Language.EN, session: aiohttp.ClientSession = None):
+    async def create(
+            cls,
+            country: str = 'GB',
+            language: Language = Language.EN,
+            session: aiohttp.ClientSession = None):
         """Create Karcher Home Robots API instance"""
 
         self = KarcherHome()
         self._country = country.upper()
         self._base_url = REGION_URLS[get_region_by_country(self._country)]
         self._language = language
 
@@ -61,19 +66,21 @@
         self._base_url = REGION_URLS[Region.US]
         self._mqtt_url = None
         self._language = Language.EN
         self._session = None
         self._mqtt = None
         self._device_props = {}
         self._wait_events = {}
+        self._http = None
+        self._http_external = False
 
     def __del__(self):
         """Destructor"""
 
-        self.close()
+        asyncio.run(self.close())
 
     async def close(self):
         """Close underlying connections"""
 
         if self._mqtt is not None:
             self._mqtt.disconnect()
             self._mqtt = None
@@ -129,16 +136,15 @@
                 kwargs['json'] = v
 
         headers['sign'] = md5(auth + ts + nonce + data)
         headers['ts'] = ts
         headers['nonce'] = nonce
 
         kwargs['headers'] = headers
-        # TODO: Fix SSL
-        kwargs['verify_ssl'] = False
+        kwargs['ssl'] = aiohttp.Fingerprint(SSL_CERTIFICATE_THUMBPRINT)
         return await self._http.request(method, self._base_url + url, **kwargs)
 
     async def _download(self, url) -> bytes:
         headers = {
             'User-Agent': 'Android_' + TENANT_ID,
         }
```

### Comparing `karcher-home-0.4.2/karcher/map.py` & `karcher-home-0.4.3/karcher/map.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.2/karcher/mapdata_pb2.py` & `karcher-home-0.4.3/karcher/mapdata_pb2.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.2/karcher/mqtt.py` & `karcher-home-0.4.3/karcher/mqtt.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.2/karcher/utils.py` & `karcher-home-0.4.3/karcher/utils.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.2/karcher_home.egg-info/PKG-INFO` & `karcher-home-0.4.3/karcher_home.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: karcher-home
-Version: 0.4.2
+Version: 0.4.3
 Summary: Kärcher Home Robots client
 Home-page: https://github.com/lafriks/python-karcher
-Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.4.2/karcher-home-0.4.2.tar.gz
+Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.4.3/karcher-home-0.4.3.tar.gz
 Author: Lauris BH
 Author-email: lauris@nix.lv
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `karcher-home-0.4.2/karcher_home.egg-info/SOURCES.txt` & `karcher-home-0.4.3/karcher_home.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.2/setup.py` & `karcher-home-0.4.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 except ImportError:
     from distutils.core import setup
 
 setup(
     name='karcher-home',
     packages=['karcher'],
     include_package_data=True,
-    version='0.4.2',
+    version='0.4.3',
     license='MIT',
     description='Kärcher Home Robots client',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Lauris BH',
     author_email='lauris@nix.lv',
     url='https://github.com/lafriks/python-karcher',
-    download_url='https://github.com/lafriks/python-karcher/releases/download/v0.4.2/karcher-home-0.4.2.tar.gz',
+    download_url='https://github.com/lafriks/python-karcher/releases/download/v0.4.3/karcher-home-0.4.3.tar.gz',
     platforms='any',
     install_requires=[
         'click',
         'aiohttp',
         'paho-mqtt',
         'cryptography',
         'protobuf'
```

### Comparing `karcher-home-0.4.2/tests/test_enc.py` & `karcher-home-0.4.3/tests/test_enc.py`

 * *Files identical despite different names*

