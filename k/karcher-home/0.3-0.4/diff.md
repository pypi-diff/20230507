# Comparing `tmp/karcher-home-0.3.tar.gz` & `tmp/karcher-home-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karcher-home-0.3.tar", last modified: Sun Apr 30 14:48:35 2023, max compression
+gzip compressed data, was "karcher-home-0.4.tar", last modified: Sun May  7 19:25:11 2023, max compression
```

## Comparing `karcher-home-0.3.tar` & `karcher-home-0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-30 14:48:35.279430 karcher-home-0.3/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1066 2023-04-23 18:36:52.000000 karcher-home-0.3/LICENSE
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1478 2023-04-30 14:48:35.279430 karcher-home-0.3/PKG-INFO
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1095 2023-04-27 21:15:39.000000 karcher-home-0.3/README.md
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-30 14:48:35.271429 karcher-home-0.3/karcher/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        0 2023-04-26 11:31:28.000000 karcher-home-0.3/karcher/__init__.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2147 2023-04-30 14:40:55.000000 karcher-home-0.3/karcher/auth.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4967 2023-04-27 21:11:26.000000 karcher-home-0.3/karcher/cli.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2287 2023-04-28 20:14:55.000000 karcher-home-0.3/karcher/consts.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5705 2023-04-28 20:58:15.000000 karcher-home-0.3/karcher/countries.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5060 2023-04-28 20:50:00.000000 karcher-home-0.3/karcher/device.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1663 2023-04-28 20:58:33.000000 karcher-home-0.3/karcher/exception.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      592 2023-04-26 12:09:03.000000 karcher-home-0.3/karcher/identifiers.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)    13754 2023-04-30 14:46:08.000000 karcher-home-0.3/karcher/karcher.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      706 2023-04-28 20:53:12.000000 karcher-home-0.3/karcher/map.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     7843 2023-04-26 08:16:45.000000 karcher-home-0.3/karcher/mapdata_pb2.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3354 2023-04-28 20:53:54.000000 karcher-home-0.3/karcher/mqtt.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3192 2023-04-28 20:55:32.000000 karcher-home-0.3/karcher/utils.py
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-30 14:48:35.275430 karcher-home-0.3/karcher_home.egg-info/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1478 2023-04-30 14:48:35.000000 karcher-home-0.3/karcher_home.egg-info/PKG-INFO
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      514 2023-04-30 14:48:35.000000 karcher-home-0.3/karcher_home.egg-info/SOURCES.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        1 2023-04-30 14:48:35.000000 karcher-home-0.3/karcher_home.egg-info/dependency_links.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       54 2023-04-30 14:48:35.000000 karcher-home-0.3/karcher_home.egg-info/entry_points.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       45 2023-04-30 14:48:35.000000 karcher-home-0.3/karcher_home.egg-info/requires.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        8 2023-04-30 14:48:35.000000 karcher-home-0.3/karcher_home.egg-info/top_level.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       79 2023-04-30 14:48:35.279430 karcher-home-0.3/setup.cfg
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      838 2023-04-28 20:56:11.000000 karcher-home-0.3/setup.py
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-04-30 14:48:35.275430 karcher-home-0.3/tests/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4294 2023-04-23 21:35:44.000000 karcher-home-0.3/tests/test_enc.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 19:25:11.395285 karcher-home-0.4/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1066 2023-04-23 18:36:52.000000 karcher-home-0.4/LICENSE
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1503 2023-05-07 19:25:11.395285 karcher-home-0.4/PKG-INFO
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1120 2023-05-07 19:15:47.000000 karcher-home-0.4/README.md
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 19:25:11.395285 karcher-home-0.4/karcher/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        0 2023-04-26 11:31:28.000000 karcher-home-0.4/karcher/__init__.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2147 2023-04-30 14:40:55.000000 karcher-home-0.4/karcher/auth.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5282 2023-05-07 19:20:56.000000 karcher-home-0.4/karcher/cli.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2287 2023-04-28 20:14:55.000000 karcher-home-0.4/karcher/consts.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5705 2023-04-28 20:58:15.000000 karcher-home-0.4/karcher/countries.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5060 2023-04-28 20:50:00.000000 karcher-home-0.4/karcher/device.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1663 2023-04-28 20:58:33.000000 karcher-home-0.4/karcher/exception.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      592 2023-04-26 12:09:03.000000 karcher-home-0.4/karcher/identifiers.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)    14293 2023-05-07 19:09:34.000000 karcher-home-0.4/karcher/karcher.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      706 2023-04-28 20:53:12.000000 karcher-home-0.4/karcher/map.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     7843 2023-04-26 08:16:45.000000 karcher-home-0.4/karcher/mapdata_pb2.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3354 2023-04-28 20:53:54.000000 karcher-home-0.4/karcher/mqtt.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3305 2023-05-07 19:24:15.000000 karcher-home-0.4/karcher/utils.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 19:25:11.395285 karcher-home-0.4/karcher_home.egg-info/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1503 2023-05-07 19:25:11.000000 karcher-home-0.4/karcher_home.egg-info/PKG-INFO
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      514 2023-05-07 19:25:11.000000 karcher-home-0.4/karcher_home.egg-info/SOURCES.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        1 2023-05-07 19:25:11.000000 karcher-home-0.4/karcher_home.egg-info/dependency_links.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       54 2023-05-07 19:25:11.000000 karcher-home-0.4/karcher_home.egg-info/entry_points.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       46 2023-05-07 19:25:11.000000 karcher-home-0.4/karcher_home.egg-info/requires.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        8 2023-05-07 19:25:11.000000 karcher-home-0.4/karcher_home.egg-info/top_level.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       79 2023-05-07 19:25:11.395285 karcher-home-0.4/setup.cfg
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      839 2023-05-07 19:22:45.000000 karcher-home-0.4/setup.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 19:25:11.395285 karcher-home-0.4/tests/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4294 2023-04-23 21:35:44.000000 karcher-home-0.4/tests/test_enc.py
```

### Comparing `karcher-home-0.3/LICENSE` & `karcher-home-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `karcher-home-0.3/PKG-INFO` & `karcher-home-0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: karcher-home
-Version: 0.3
+Version: 0.4
 Summary: Kärcher Home Robots client
 Home-page: https://github.com/lafriks/python-karcher
-Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.3/karcher-home-0.3.tar.gz
+Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.4/karcher-home-0.4.tar.gz
 Author: Lauris BH
 Author-email: lauris@nix.lv
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -45,15 +45,15 @@
 ```
 
 ### From code
 
 ```python
 from karcher.karcher import KarcherHome
 
-kh = KarcherHome()
-kh.login("user@email", "password")
-devices = hk.get_devices()
+kh = await KarcherHome.create()
+await kh.login("user@email", "password")
+devices = await hk.get_devices()
 ```
 
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
```

### Comparing `karcher-home-0.3/README.md` & `karcher-home-0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ```
 
 ### From code
 
 ```python
 from karcher.karcher import KarcherHome
 
-kh = KarcherHome()
-kh.login("user@email", "password")
-devices = hk.get_devices()
+kh = await KarcherHome.create()
+await kh.login("user@email", "password")
+devices = await hk.get_devices()
 ```
 
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
```

### Comparing `karcher-home-0.3/karcher/auth.py` & `karcher-home-0.4/karcher/auth.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.3/karcher/cli.py` & `karcher-home-0.4/karcher/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 # -----------------------------------------------------------
 # Copyright (c) 2023 Lauris BH
 # SPDX-License-Identifier: MIT
 # -----------------------------------------------------------
 
+import asyncio
 import click
 import dataclasses
 import json
 import logging
+from functools import wraps
 
 from karcher.exception import KarcherHomeException
 from karcher.karcher import KarcherHome
 from karcher.consts import Region
 
 try:
     from rich import print as echo
 except ImportError:
     echo = click.echo
 
 
+def coro(f):
+    @wraps(f)
+    def wrapper(*args, **kwargs):
+        return asyncio.run(f(*args, **kwargs))
+
+    return wrapper
+
+
 class EnhancedJSONEncoder(json.JSONEncoder):
     def default(self, o):
         if dataclasses.is_dataclass(o):
             return dataclasses.asdict(o)
         return super().default(o)
 
 
@@ -80,94 +90,98 @@
             'message': ex.message
         }))
         return
 
 
 @cli.command()
 @click.pass_context
-def urls(ctx: click.Context):
+@coro
+async def urls(ctx: click.Context):
     """Get region information."""
 
-    kh = KarcherHome(region=ctx.obj.region)
-    d = kh.get_urls()
+    kh = await KarcherHome.create(region=ctx.obj.region)
+    d = await kh.get_urls()
 
     ctx.obj.print(d)
 
 
 @cli.command()
 @click.option('--username', '-u', help='Username to login with.')
 @click.option('--password', '-p', help='Password to login with.')
 @click.pass_context
-def login(ctx: click.Context, username: str, password: str):
+@coro
+async def login(ctx: click.Context, username: str, password: str):
     """Get user session tokens."""
 
-    kh = KarcherHome(region=ctx.obj.region)
+    kh = await KarcherHome.create(region=ctx.obj.region)
     ctx.obj.print(kh.login(username, password))
 
 
 @cli.command()
 @click.option('--username', '-u', default=None, help='Username to login with.')
 @click.option('--password', '-p', default=None, help='Password to login with.')
 @click.option('--auth-token', '-t', default=None, help='Authorization token.')
 @click.pass_context
-def devices(ctx: click.Context, username: str, password: str, auth_token: str):
+@coro
+async def devices(ctx: click.Context, username: str, password: str, auth_token: str):
     """List all devices."""
 
-    kh = KarcherHome(region=ctx.obj.region)
+    kh = await KarcherHome.create(region=ctx.obj.region)
     if auth_token is not None:
         kh.login_token(auth_token, '')
     elif username is not None and password is not None:
-        kh.login(username, password)
+        await kh.login(username, password)
     else:
         raise click.BadParameter(
             'Must provide either token or username and password.')
 
-    devices = kh.get_devices()
+    devices = await kh.get_devices()
 
     # Logout if we used a username and password
     if auth_token is None:
-        kh.logout()
+        await kh.logout()
 
     ctx.obj.print(devices)
 
 
 @cli.command()
 @click.option('--username', '-u', default=None, help='Username to login with.')
 @click.option('--password', '-p', default=None, help='Password to login with.')
 @click.option('--auth-token', '-t', default=None, help='Authorization token.')
 @click.option('--mqtt-token', '-m', default=None, help='MQTT authorization token.')
 @click.option('--device-id', '-d', required=True, help='Device ID.')
 @click.pass_context
-def device_properties(
+@coro
+async def device_properties(
         ctx: click.Context,
         username: str,
         password: str,
         auth_token: str,
         mqtt_token: str,
         device_id: str):
     """Get device properties."""
 
-    kh = KarcherHome(region=ctx.obj.region)
+    kh = await KarcherHome.create(region=ctx.obj.region)
     if auth_token is not None:
         kh.login_token(auth_token, mqtt_token)
     elif username is not None and password is not None:
-        kh.login(username, password)
+        await kh.login(username, password)
     else:
         raise click.BadParameter(
             'Must provide either token or username and password.')
 
     dev = None
-    for device in kh.get_devices():
+    for device in await kh.get_devices():
         if device.device_id == device_id:
             dev = device
             break
 
     if dev is None:
         raise click.BadParameter('Device ID not found.')
 
     props = kh.get_device_properties(dev)
 
     # Logout if we used a username and password
     if auth_token is None:
-        kh.logout()
+        await kh.logout()
 
     ctx.obj.print(props)
```

### Comparing `karcher-home-0.3/karcher/consts.py` & `karcher-home-0.4/karcher/consts.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.3/karcher/countries.py` & `karcher-home-0.4/karcher/countries.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.3/karcher/device.py` & `karcher-home-0.4/karcher/device.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.3/karcher/exception.py` & `karcher-home-0.4/karcher/exception.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.3/karcher/identifiers.py` & `karcher-home-0.4/karcher/identifiers.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.3/karcher/karcher.py` & `karcher-home-0.4/karcher/karcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,59 +3,74 @@
 # SPDX-License-Identifier: MIT
 # -----------------------------------------------------------
 
 import collections
 import json
 import threading
 from typing import List, Any
-import requests
+import aiohttp
 import urllib.parse
 
 
 from .auth import Domains, Session
 from .countries import get_country_code, get_region_by_country
-from .consts import APP_VERSION_CODE, APP_VERSION_NAME, PROJECT_TYPE, \
-    PROTOCOL_VERSION, REGION_URLS, ROBOT_PROPERTIES, TENANT_ID, \
-    Language
+from .consts import (
+    APP_VERSION_CODE, APP_VERSION_NAME, PROJECT_TYPE,
+    PROTOCOL_VERSION, REGION_URLS, ROBOT_PROPERTIES, TENANT_ID,
+    Language, Region
+)
 from .device import Device, DeviceProperties
 from .exception import KarcherHomeAccessDenied, KarcherHomeException, handle_error_code
 from .map import Map
 from .mqtt import MqttClient, get_device_topic_property_get_reply, get_device_topics
-from .utils import decrypt, decrypt_map, encrypt, get_nonce, get_random_string, \
+from .utils import (
+    decrypt, decrypt_map, encrypt, get_nonce, get_random_string,
     get_timestamp, get_timestamp_ms, is_email, md5
+)
 
 
 class KarcherHome:
     """Main class to access Karcher Home Robots API"""
 
-    def __init__(self, country: str = 'GB', language: Language = Language.EN):
-        """Initialize Karcher Home Robots API"""
+    @classmethod
+    async def create(cls, country: str = 'GB', language: Language = Language.EN):
+        """Create Karcher Home Robots API instance"""
 
-        super().__init__()
+        self = KarcherHome()
         self._country = country.upper()
         self._base_url = REGION_URLS[get_region_by_country(self._country)]
-        self._mqtt_url = None
         self._language = language
-        self._session = None
-        self._mqtt = None
-        self._device_props = {}
-        self._wait_events = {}
 
-        d = self.get_urls()
+        d = await self.get_urls()
         # Update base URLs
         if d.app_api != '':
             self._base_url = d.app_api
         if d.mqtt != '':
             self._mqtt_url = d.mqtt
 
-    def _request(self, method: str, url: str, **kwargs) -> requests.Response:
-        session = requests.Session()
+        return self
+
+    def __init__(self):
+        """Initialize Karcher Home Robots API"""
+
+        super().__init__()
+        self._country = 'US'
+        self._base_url = REGION_URLS[Region.US]
+        self._mqtt_url = None
+        self._language = Language.EN
+        self._session = None
+        self._mqtt = None
+        self._device_props = {}
+        self._wait_events = {}
+
+    async def _request(self, method: str, url: str, **kwargs) -> aiohttp.ClientResponse:
+        session = aiohttp.ClientSession()
         # TODO: Fix SSL
-        requests.packages.urllib3.disable_warnings()
-        session.verify = False
+        # requests.packages.urllib3.disable_warnings()
+        # session.skip = False
 
         headers = {}
         if kwargs.get('headers') is not None:
             headers = kwargs['headers']
 
         headers['User-Agent'] = 'Android_' + TENANT_ID
         auth = ''
@@ -94,34 +109,35 @@
                 kwargs['json'] = v
 
         headers['sign'] = md5(auth + ts + nonce + data)
         headers['ts'] = ts
         headers['nonce'] = nonce
 
         kwargs['headers'] = headers
-        return session.request(method, self._base_url + url, **kwargs)
+        kwargs['verify_ssl'] = False
+        return await session.request(method, self._base_url + url, **kwargs)
 
-    def _download(self, url) -> bytes:
-        session = requests.Session()
+    async def _download(self, url) -> bytes:
+        session = aiohttp.ClientSession()
         headers = {
             'User-Agent': 'Android_' + TENANT_ID,
         }
 
-        resp = session.get(url, headers=headers)
-        if resp.status_code != 200:
+        resp = await session.get(url, headers=headers)
+        if resp.status != 200:
             raise KarcherHomeException(-1,
                                        'HTTP error: ' + str(resp.status_code))
 
-        return resp.content
+        return await resp.content.read(-1)
 
-    def _process_response(self, resp, prop=None) -> Any:
-        if resp.status_code != 200:
+    async def _process_response(self, resp: aiohttp.ClientResponse, prop=None) -> Any:
+        if resp.status != 200:
             raise KarcherHomeException(-1,
-                                       'HTTP error: ' + str(resp.status_code))
-        data = resp.json()
+                                       'HTTP error: ' + str(resp.status))
+        data = await resp.json()
         # Check for error response
         if data['code'] != 0:
             handle_error_code(data['code'], data['msg'])
         # Check for empty response
         if 'result' not in data:
             return None
         # Handle special response types
@@ -157,36 +173,36 @@
         self._mqtt.connect()
         self._mqtt.on_message = self._process_mqtt_message
 
         if wait_for_connect:
             event.wait()
             self._mqtt.on_connect = None
 
-    def get_urls(self) -> Domains:
+    async def get_urls(self) -> Domains:
         """Get URLs for API and MQTT."""
 
-        resp = self._request('GET', '/network-service/domains/list', params={
+        resp = await self._request('GET', '/network-service/domains/list', params={
             'tenantId': TENANT_ID,
             'productModeCode': PROJECT_TYPE,
             'version': PROTOCOL_VERSION,
         })
 
-        d = self._process_response(resp, 'domain')
+        d = await self._process_response(resp, 'domain')
         return Domains(**d)
 
-    def login(self, username, password, register_id=None) -> Session:
+    async def login(self, username, password, register_id=None) -> Session:
         """Login using provided credentials."""
 
         if register_id is None or register_id == '':
             register_id = get_random_string(19)
 
         if not is_email(username):
             username = '86-' + username
 
-        resp = self._request('POST', '/user-center/auth/login', json={
+        resp = await self._request('POST', '/user-center/auth/login', json={
             'tenantId': TENANT_ID,
             'lang': str(self._language),
             'token': None,
             'userId': None,
             'password': encrypt(password),
             'username': encrypt(username),
             'authcode': None,
@@ -197,15 +213,15 @@
             'phoneSys': 1,
             'noticeSetting': {
                 'andIpad': register_id,
                 'android': register_id,
             },
         })
 
-        d = self._process_response(resp)
+        d = await self._process_response(resp)
         self._session = Session(**d)
         self._session.register_id = register_id
 
         return self._session
 
     def login_token(
             self,
@@ -218,67 +234,67 @@
             register_id = get_random_string(19)
 
         self._session = Session.from_token(auth_token, mqtt_token)
         self._session.register_id = register_id
 
         return self._session
 
-    def logout(self):
+    async def logout(self):
         """End current session.
 
         This will also reset the session object.
         """
         if self._session is None \
                 or self._session.auth_token == '' or self._session.user_id == '':
             self._session = None
             return
 
-        self._process_response(self._request(
+        await self._process_response(await self._request(
             'POST', '/user-center/auth/logout'))
         self._session = None
 
         if self._mqtt is not None:
             self._mqtt.disconnect()
             self._mqtt = None
 
-    def get_devices(self) -> List[Device]:
+    async def get_devices(self) -> List[Device]:
         """Get all user devices."""
 
         if self._session is None \
                 or self._session.auth_token == '' or self._session.user_id == '':
             raise KarcherHomeAccessDenied('Not authorized')
 
-        resp = self._request(
+        resp = await self._request(
             'GET',
             '/smart-home-service/smartHome/user/getDeviceInfoByUserId/'
             + self._session.user_id)
 
-        return [Device(**d) for d in self._process_response(resp)]
+        return [Device(**d) for d in await self._process_response(resp)]
 
-    def get_map_data(self, dev: Device, map: int = 1):
+    async def get_map_data(self, dev: Device, map: int = 1):
         # <tenantId>/<modeType>/<deviceSn>/01-01-2022/map/temp/0046690461_<deviceSn>_1
         mapDir = TENANT_ID + '/' + dev.product_mode_code + '/' +\
             dev.sn + '/01-01-2022/map/temp/0046690461_' + \
             dev.sn + '_' + str(map)
 
-        resp = self._request('POST',
-                             '/storage-management/storage/aws/getAccessUrl',
-                             json={
-                                 'dir': mapDir,
-                                 'countryCode': get_country_code(self._country),
-                                 'serviceType': 2,
-                                 'tenantId': TENANT_ID,
-                             })
+        resp = await self._request('POST',
+                                   '/storage-management/storage/aws/getAccessUrl',
+                                   json={
+                                       'dir': mapDir,
+                                       'countryCode': get_country_code(self._country),
+                                       'serviceType': 2,
+                                       'tenantId': TENANT_ID,
+                                   })
 
-        d = self._process_response(resp)
+        d = await self._process_response(resp)
         downloadUrl = d['url']
         if 'cdnDomain' in d and d['cdnDomain'] != '':
             downloadUrl = 'https://' + d['cdnDomain'] + '/' + d['dir']
 
-        d = self._download(downloadUrl)
+        d = await self._download(downloadUrl)
         data = decrypt_map(dev.sn, dev.mac, dev.product_id, d)
         if map == 1 or map == 2:
             return Map.parse(data)
         else:
             return json.loads(data)
 
     def subscribe_device(self, dev: Device):
```

### Comparing `karcher-home-0.3/karcher/map.py` & `karcher-home-0.4/karcher/map.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.3/karcher/mapdata_pb2.py` & `karcher-home-0.4/karcher/mapdata_pb2.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.3/karcher/mqtt.py` & `karcher-home-0.4/karcher/mqtt.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.3/karcher/utils.py` & `karcher-home-0.4/karcher/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import hashlib
 import random
 import re
 import string
 import time
 from typing import Final
 import zlib
-from Crypto.Cipher import AES
+from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 
 from .consts import TENANT_ID, Product
 
 
 EMAIL_REGEX: Final = "^\\w+([-+.]\\w+)*@\\w+([-.]\\w+)*\\.\\w+([-.]\\w+)*$"
 
 
@@ -44,45 +44,46 @@
     m = hashlib.md5()
     m.update(bytes(TENANT_ID, 'utf-8'))
     h = m.hexdigest()
     return bytes(h[8:24], 'utf-8')
 
 
 def decrypt(data) -> str:
-    cipher = AES.new(get_enc_key(), AES.MODE_ECB)
-    buf = cipher.decrypt(base64.b64decode(data))
+    cipher = Cipher(algorithms.AES128(get_enc_key()), modes.ECB())
+    buf = cipher.decryptor().update(base64.b64decode(data))
     return str(buf[:-ord(buf[-1:])], 'utf-8')
 
 
 def encrypt(data) -> str:
-    cipher = AES.new(get_enc_key(), AES.MODE_ECB)
+    cipher = Cipher(algorithms.AES128(get_enc_key()), modes.ECB())
     buf = bytes(data, 'utf-8')
-    pad_len = cipher.block_size - (len(buf) % cipher.block_size)
+    pad_len = 16 - (len(buf) % 16)
     buf = buf + bytes([pad_len]) * pad_len
-    return base64.b64encode(cipher.encrypt(buf)).decode()
+    return base64.b64encode(cipher.encryptor().update(buf)).decode()
 
 
 def get_map_enc_key(sn: str, mac: str, product_id: Product) -> bytes:
     sub_key = mac.replace(':', '').lower() + str(product_id.value)
-    cipher = AES.new(bytes(sub_key[0:16], 'utf-8'), AES.MODE_ECB)
+    cipher = Cipher(algorithms.AES128(bytes(sub_key[0:16], 'utf-8')), modes.ECB())
     buf = bytes(sn + '+' + str(product_id.value) + '+' + sn, 'utf-8')
-    pad_len = cipher.block_size - (len(buf) % cipher.block_size)
+    pad_len = 16 - (len(buf) % 16)
     buf = buf + bytes([pad_len]) * pad_len
 
-    key = base64.b64encode(cipher.encrypt(buf)).decode()
+    key = base64.b64encode(cipher.encryptor().update(buf)).decode()
 
     m = hashlib.md5()
     m.update(bytes(key, 'utf-8'))
     h = m.hexdigest()
     return bytes(h[8:24], 'utf-8')
 
 
 def decrypt_map(sn: str, mac: str, product_id: Product, data: bytes) -> bytes:
-    cipher = AES.new(get_map_enc_key(sn, mac, product_id), AES.MODE_ECB)
-    buf = cipher.decrypt(base64.b64decode(data))
+    key = get_map_enc_key(sn, mac, product_id)
+    cipher = Cipher(algorithms.AES128(key), modes.ECB())
+    buf = cipher.decryptor().update(base64.b64decode(data))
     try:
         return zlib.decompress(bytes.fromhex(str(buf[:-ord(buf[-1:])], 'utf-8')))
     except Exception:
         return bytes.fromhex(str(buf[:-ord(buf[-1:])], 'utf-8'))
 
 
 def md5(data: str) -> str:
```

### Comparing `karcher-home-0.3/karcher_home.egg-info/PKG-INFO` & `karcher-home-0.4/karcher_home.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: karcher-home
-Version: 0.3
+Version: 0.4
 Summary: Kärcher Home Robots client
 Home-page: https://github.com/lafriks/python-karcher
-Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.3/karcher-home-0.3.tar.gz
+Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.4/karcher-home-0.4.tar.gz
 Author: Lauris BH
 Author-email: lauris@nix.lv
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -45,15 +45,15 @@
 ```
 
 ### From code
 
 ```python
 from karcher.karcher import KarcherHome
 
-kh = KarcherHome()
-kh.login("user@email", "password")
-devices = hk.get_devices()
+kh = await KarcherHome.create()
+await kh.login("user@email", "password")
+devices = await hk.get_devices()
 ```
 
 ## License
 
 Distributed under the MIT License. See `LICENSE` for more information.
```

### Comparing `karcher-home-0.3/karcher_home.egg-info/SOURCES.txt` & `karcher-home-0.4/karcher_home.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `karcher-home-0.3/setup.py` & `karcher-home-0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 except ImportError:
     from distutils.core import setup
 
 setup(
     name='karcher-home',
     packages=['karcher'],
     include_package_data=True,
-    version='0.3',
+    version='0.4',
     license='MIT',
     description='Kärcher Home Robots client',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Lauris BH',
     author_email='lauris@nix.lv',
     url='https://github.com/lafriks/python-karcher',
-    download_url='https://github.com/lafriks/python-karcher/releases/download/v0.3/karcher-home-0.3.tar.gz',
+    download_url='https://github.com/lafriks/python-karcher/releases/download/v0.4/karcher-home-0.4.tar.gz',
     platforms='any',
     install_requires=[
-        'requests',
-        'tzlocal',
         'click',
-        'pycryptodome',
+        'aiohttp',
+        'paho-mqtt',
+        'cryptography',
         'protobuf'
     ],
     entry_points='''
         [console_scripts]
         karcher-home=karcher.cli:safe_cli
     ''',
 )
```

### Comparing `karcher-home-0.3/tests/test_enc.py` & `karcher-home-0.4/tests/test_enc.py`

 * *Files identical despite different names*

