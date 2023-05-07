# Comparing `tmp/karcher-home-0.4.5.tar.gz` & `tmp/karcher-home-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karcher-home-0.4.5.tar", last modified: Sun May  7 20:29:39 2023, max compression
+gzip compressed data, was "karcher-home-0.5.tar", last modified: Sun May  7 21:28:42 2023, max compression
```

## Comparing `karcher-home-0.4.5.tar` & `karcher-home-0.5.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 20:29:39.457836 karcher-home-0.4.5/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1066 2023-04-23 18:36:52.000000 karcher-home-0.4.5/LICENSE
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1509 2023-05-07 20:29:39.457836 karcher-home-0.4.5/PKG-INFO
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1120 2023-05-07 19:15:47.000000 karcher-home-0.4.5/README.md
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 20:29:39.453836 karcher-home-0.4.5/karcher/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        0 2023-04-26 11:31:28.000000 karcher-home-0.4.5/karcher/__init__.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2147 2023-04-30 14:40:55.000000 karcher-home-0.4.5/karcher/auth.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5292 2023-05-07 20:09:10.000000 karcher-home-0.4.5/karcher/cli.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2446 2023-05-07 20:08:27.000000 karcher-home-0.4.5/karcher/consts.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5705 2023-04-28 20:58:15.000000 karcher-home-0.4.5/karcher/countries.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5060 2023-04-28 20:50:00.000000 karcher-home-0.4.5/karcher/device.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1663 2023-04-28 20:58:33.000000 karcher-home-0.4.5/karcher/exception.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      592 2023-04-26 12:09:03.000000 karcher-home-0.4.5/karcher/identifiers.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)    14977 2023-05-07 20:25:30.000000 karcher-home-0.4.5/karcher/karcher.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      706 2023-04-28 20:53:12.000000 karcher-home-0.4.5/karcher/map.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     7843 2023-04-26 08:16:45.000000 karcher-home-0.4.5/karcher/mapdata_pb2.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3354 2023-04-28 20:53:54.000000 karcher-home-0.4.5/karcher/mqtt.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3305 2023-05-07 19:24:15.000000 karcher-home-0.4.5/karcher/utils.py
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 20:29:39.457836 karcher-home-0.4.5/karcher_home.egg-info/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1509 2023-05-07 20:29:39.000000 karcher-home-0.4.5/karcher_home.egg-info/PKG-INFO
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      514 2023-05-07 20:29:39.000000 karcher-home-0.4.5/karcher_home.egg-info/SOURCES.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        1 2023-05-07 20:29:39.000000 karcher-home-0.4.5/karcher_home.egg-info/dependency_links.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       54 2023-05-07 20:29:39.000000 karcher-home-0.4.5/karcher_home.egg-info/entry_points.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       46 2023-05-07 20:29:39.000000 karcher-home-0.4.5/karcher_home.egg-info/requires.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        8 2023-05-07 20:29:39.000000 karcher-home-0.4.5/karcher_home.egg-info/top_level.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       79 2023-05-07 20:29:39.457836 karcher-home-0.4.5/setup.cfg
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      845 2023-05-07 20:28:03.000000 karcher-home-0.4.5/setup.py
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 20:29:39.457836 karcher-home-0.4.5/tests/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4294 2023-04-23 21:35:44.000000 karcher-home-0.4.5/tests/test_enc.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 21:28:42.968220 karcher-home-0.5/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1066 2023-04-23 18:36:52.000000 karcher-home-0.5/LICENSE
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1503 2023-05-07 21:28:42.968220 karcher-home-0.5/PKG-INFO
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1120 2023-05-07 19:15:47.000000 karcher-home-0.5/README.md
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 21:28:42.968220 karcher-home-0.5/karcher/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        0 2023-04-26 11:31:28.000000 karcher-home-0.5/karcher/__init__.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2161 2023-05-07 21:09:30.000000 karcher-home-0.5/karcher/auth.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5292 2023-05-07 20:09:10.000000 karcher-home-0.5/karcher/cli.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2446 2023-05-07 20:08:27.000000 karcher-home-0.5/karcher/consts.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5705 2023-04-28 20:58:15.000000 karcher-home-0.5/karcher/countries.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5081 2023-05-07 21:09:48.000000 karcher-home-0.5/karcher/device.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1663 2023-05-07 21:17:16.000000 karcher-home-0.5/karcher/exception.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      592 2023-04-26 12:09:03.000000 karcher-home-0.5/karcher/identifiers.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)    15517 2023-05-07 21:16:41.000000 karcher-home-0.5/karcher/karcher.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      706 2023-04-28 20:53:12.000000 karcher-home-0.5/karcher/map.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     7843 2023-04-26 08:16:45.000000 karcher-home-0.5/karcher/mapdata_pb2.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3354 2023-04-28 20:53:54.000000 karcher-home-0.5/karcher/mqtt.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      898 2023-05-07 21:20:45.000000 karcher-home-0.5/karcher/user.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3305 2023-05-07 19:24:15.000000 karcher-home-0.5/karcher/utils.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 21:28:42.968220 karcher-home-0.5/karcher_home.egg-info/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1503 2023-05-07 21:28:42.000000 karcher-home-0.5/karcher_home.egg-info/PKG-INFO
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      530 2023-05-07 21:28:42.000000 karcher-home-0.5/karcher_home.egg-info/SOURCES.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        1 2023-05-07 21:28:42.000000 karcher-home-0.5/karcher_home.egg-info/dependency_links.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       54 2023-05-07 21:28:42.000000 karcher-home-0.5/karcher_home.egg-info/entry_points.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       46 2023-05-07 21:28:42.000000 karcher-home-0.5/karcher_home.egg-info/requires.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        8 2023-05-07 21:28:42.000000 karcher-home-0.5/karcher_home.egg-info/top_level.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       79 2023-05-07 21:28:42.968220 karcher-home-0.5/setup.cfg
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      839 2023-05-07 21:28:34.000000 karcher-home-0.5/setup.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 21:28:42.968220 karcher-home-0.5/tests/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4294 2023-04-23 21:35:44.000000 karcher-home-0.5/tests/test_enc.py
```

### Comparing `karcher-home-0.4.5/LICENSE` & `karcher-home-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.5/PKG-INFO` & `karcher-home-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: karcher-home
-Version: 0.4.5
+Version: 0.5
 Summary: Kärcher Home Robots client
 Home-page: https://github.com/lafriks/python-karcher
-Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.4.5/karcher-home-0.4.5.tar.gz
+Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.5/karcher-home-0.5.tar.gz
 Author: Lauris BH
 Author-email: lauris@nix.lv
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `karcher-home-0.4.5/README.md` & `karcher-home-0.5/README.md`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.5/karcher/auth.py` & `karcher-home-0.5/karcher/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import json
 
 
 @dataclass(init=False)
 class Domains:
     """Domains URLs class.
 
-    This class represents a Karcher Home access URLs.
+    This class represents a Karcher Home Robots access URLs.
     """
     app_api: str
     mqtt: str
 
     def __init__(self, **kwargs):
         names = set([f.name for f in fields(self)])
         for k, v in kwargs.items():
@@ -27,15 +27,15 @@
                 setattr(self, k, v)
 
 
 @dataclass(init=False)
 class Session:
     """Authorized user session class.
 
-    This class represents a Karcher Home authorized user session.
+    This class represents a Karcher Home Robots authorized user session.
     """
 
     register_id: str
     user_id: str
     auth_token: str
     mqtt_token: str
```

### Comparing `karcher-home-0.4.5/karcher/cli.py` & `karcher-home-0.5/karcher/cli.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.5/karcher/consts.py` & `karcher-home-0.5/karcher/consts.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.5/karcher/countries.py` & `karcher-home-0.5/karcher/countries.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.5/karcher/device.py` & `karcher-home-0.5/karcher/device.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     Online = 1
 
 
 @dataclass(init=False)
 class DeviceVersion:
     """Device version class.
 
-    This class represents a Karcher Home device version.
+    This class represents a Karcher Home Robots device version.
     """
     package_type: str = ''
     version: int = 0
     version_name: str = ''
     ctrl_version: str = ''
 
     def __init__(self, **kwargs):
@@ -80,15 +80,15 @@
     quiting: int = 0
 
 
 @dataclass(init=False)
 class DeviceProperties:
     """Device properties class.
 
-    This class represents a Karcher Home detailed device properties.
+    This class represents a Karcher Home Robots detailed device properties.
     """
 
     firmware: str = ''
     firmware_code: int = 0
     status: int = 0
     fault: int = 0
     wind: int = 0
@@ -157,15 +157,15 @@
         return updated
 
 
 @dataclass(init=False)
 class Device:
     """Device class.
 
-    This class represents a Karcher Home device.
+    This class represents a Karcher Home Robots device.
     """
 
     device_id: str
     sn: str
     mac: str
     nickname: str
     versions: List[DeviceVersion]
```

### Comparing `karcher-home-0.4.5/karcher/exception.py` & `karcher-home-0.5/karcher/exception.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.5/karcher/identifiers.py` & `karcher-home-0.5/karcher/identifiers.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.5/karcher/karcher.py` & `karcher-home-0.5/karcher/karcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 import collections
 import json
 import threading
 from typing import List, Any
 import aiohttp
 import urllib.parse
 
-
 from .auth import Domains, Session
 from .countries import get_country_code, get_region_by_country
 from .consts import (
     APP_VERSION_CODE, APP_VERSION_NAME, PROJECT_TYPE, PROTOCOL_VERSION,
     REGION_URLS, ROBOT_PROPERTIES, SSL_CERTIFICATE_THUMBPRINT, TENANT_ID,
     Language, Region
 )
 from .device import Device, DeviceProperties
 from .exception import KarcherHomeAccessDenied, KarcherHomeException, handle_error_code
 from .map import Map
 from .mqtt import MqttClient, get_device_topic_property_get_reply, get_device_topics
+from .user import UserProfile
 from .utils import (
     decrypt, decrypt_map, encrypt, get_nonce, get_random_string,
     get_timestamp, get_timestamp_ms, is_email, md5
 )
 
 
 class KarcherHome:
@@ -45,20 +45,20 @@
         self._base_url = REGION_URLS[get_region_by_country(self._country)]
         self._language = language
 
         if session is not None:
             self._http_external = True
             self._http = session
 
-        d = await self.get_urls()
+        data = await self.get_urls()
         # Update base URLs
-        if d.app_api != '':
-            self._base_url = d.app_api
-        if d.mqtt != '':
-            self._mqtt_url = d.mqtt
+        if data.app_api != '':
+            self._base_url = data.app_api
+        if data.mqtt != '':
+            self._mqtt_url = data.mqtt
 
         return self
 
     def __init__(self):
         """Initialize Karcher Home Robots API"""
 
         super().__init__()
@@ -214,16 +214,16 @@
 
         resp = await self._request('GET', '/network-service/domains/list', params={
             'tenantId': TENANT_ID,
             'productModeCode': PROJECT_TYPE,
             'version': PROTOCOL_VERSION,
         })
 
-        d = await self._process_response(resp, 'domain')
-        return Domains(**d)
+        data = await self._process_response(resp, 'domain')
+        return Domains(**data)
 
     async def login(self, username, password, register_id=None) -> Session:
         """Login using provided credentials."""
 
         if register_id is None or register_id == '':
             register_id = get_random_string(19)
 
@@ -245,16 +245,16 @@
             'phoneSys': 1,
             'noticeSetting': {
                 'andIpad': register_id,
                 'android': register_id,
             },
         })
 
-        d = await self._process_response(resp)
-        self._session = Session(**d)
+        data = await self._process_response(resp)
+        self._session = Session(**data)
         self._session.register_id = register_id
 
         return self._session
 
     def login_token(
             self,
             auth_token: str,
@@ -282,14 +282,28 @@
 
         await self._process_response(await self._request(
             'POST', '/user-center/auth/logout'))
         self._session = None
 
         await self.close()
 
+    async def get_user_info(self) -> UserProfile:
+        """Get user profile information."""
+
+        if self._session is None \
+                or self._session.auth_token == '' or self._session.user_id == '':
+            raise KarcherHomeAccessDenied('Not authorized')
+
+        resp = await self._request(
+            'GET',
+            '/user-center/app/user/profile')
+        data = await self._process_response(resp)
+
+        return UserProfile(**data)
+
     async def get_devices(self) -> List[Device]:
         """Get all user devices."""
 
         if self._session is None \
                 or self._session.auth_token == '' or self._session.user_id == '':
             raise KarcherHomeAccessDenied('Not authorized')
 
@@ -311,21 +325,21 @@
                                    json={
                                        'dir': mapDir,
                                        'countryCode': get_country_code(self._country),
                                        'serviceType': 2,
                                        'tenantId': TENANT_ID,
                                    })
 
-        d = await self._process_response(resp)
-        downloadUrl = d['url']
-        if 'cdnDomain' in d and d['cdnDomain'] != '':
-            downloadUrl = 'https://' + d['cdnDomain'] + '/' + d['dir']
+        data = await self._process_response(resp)
+        downloadUrl = data['url']
+        if 'cdnDomain' in data and data['cdnDomain'] != '':
+            downloadUrl = 'https://' + data['cdnDomain'] + '/' + data['dir']
 
-        d = await self._download(downloadUrl)
-        data = decrypt_map(dev.sn, dev.mac, dev.product_id, d)
+        data = await self._download(downloadUrl)
+        data = decrypt_map(dev.sn, dev.mac, dev.product_id, data)
         if map == 1 or map == 2:
             return Map.parse(data)
         else:
             return json.loads(data)
 
     def subscribe_device(self, dev: Device):
         """Subscribe to device real-time events."""
```

### Comparing `karcher-home-0.4.5/karcher/map.py` & `karcher-home-0.5/karcher/map.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.5/karcher/mapdata_pb2.py` & `karcher-home-0.5/karcher/mapdata_pb2.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.5/karcher/mqtt.py` & `karcher-home-0.5/karcher/mqtt.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.5/karcher/utils.py` & `karcher-home-0.5/karcher/utils.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.5/karcher_home.egg-info/PKG-INFO` & `karcher-home-0.5/karcher_home.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: karcher-home
-Version: 0.4.5
+Version: 0.5
 Summary: Kärcher Home Robots client
 Home-page: https://github.com/lafriks/python-karcher
-Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.4.5/karcher-home-0.4.5.tar.gz
+Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.5/karcher-home-0.5.tar.gz
 Author: Lauris BH
 Author-email: lauris@nix.lv
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `karcher-home-0.4.5/karcher_home.egg-info/SOURCES.txt` & `karcher-home-0.5/karcher_home.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 karcher/device.py
 karcher/exception.py
 karcher/identifiers.py
 karcher/karcher.py
 karcher/map.py
 karcher/mapdata_pb2.py
 karcher/mqtt.py
+karcher/user.py
 karcher/utils.py
 karcher_home.egg-info/PKG-INFO
 karcher_home.egg-info/SOURCES.txt
 karcher_home.egg-info/dependency_links.txt
 karcher_home.egg-info/entry_points.txt
 karcher_home.egg-info/requires.txt
 karcher_home.egg-info/top_level.txt
```

### Comparing `karcher-home-0.4.5/setup.py` & `karcher-home-0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 except ImportError:
     from distutils.core import setup
 
 setup(
     name='karcher-home',
     packages=['karcher'],
     include_package_data=True,
-    version='0.4.5',
+    version='0.5',
     license='MIT',
     description='Kärcher Home Robots client',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Lauris BH',
     author_email='lauris@nix.lv',
     url='https://github.com/lafriks/python-karcher',
-    download_url='https://github.com/lafriks/python-karcher/releases/download/v0.4.5/karcher-home-0.4.5.tar.gz',
+    download_url='https://github.com/lafriks/python-karcher/releases/download/v0.5/karcher-home-0.5.tar.gz',
     platforms='any',
     install_requires=[
         'click',
         'aiohttp',
         'paho-mqtt',
         'cryptography',
         'protobuf'
```

### Comparing `karcher-home-0.4.5/tests/test_enc.py` & `karcher-home-0.5/tests/test_enc.py`

 * *Files identical despite different names*

