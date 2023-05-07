# Comparing `tmp/karcher-home-0.4.1.tar.gz` & `tmp/karcher-home-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karcher-home-0.4.1.tar", last modified: Sun May  7 19:38:22 2023, max compression
+gzip compressed data, was "karcher-home-0.4.2.tar", last modified: Sun May  7 19:56:56 2023, max compression
```

## Comparing `karcher-home-0.4.1.tar` & `karcher-home-0.4.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 19:38:22.339699 karcher-home-0.4.1/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1066 2023-04-23 18:36:52.000000 karcher-home-0.4.1/LICENSE
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1509 2023-05-07 19:38:22.339699 karcher-home-0.4.1/PKG-INFO
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1120 2023-05-07 19:15:47.000000 karcher-home-0.4.1/README.md
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 19:38:22.339699 karcher-home-0.4.1/karcher/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        0 2023-04-26 11:31:28.000000 karcher-home-0.4.1/karcher/__init__.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2147 2023-04-30 14:40:55.000000 karcher-home-0.4.1/karcher/auth.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5229 2023-05-07 19:37:05.000000 karcher-home-0.4.1/karcher/cli.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2287 2023-04-28 20:14:55.000000 karcher-home-0.4.1/karcher/consts.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5705 2023-04-28 20:58:15.000000 karcher-home-0.4.1/karcher/countries.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5060 2023-04-28 20:50:00.000000 karcher-home-0.4.1/karcher/device.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1663 2023-04-28 20:58:33.000000 karcher-home-0.4.1/karcher/exception.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      592 2023-04-26 12:09:03.000000 karcher-home-0.4.1/karcher/identifiers.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)    14293 2023-05-07 19:09:34.000000 karcher-home-0.4.1/karcher/karcher.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      706 2023-04-28 20:53:12.000000 karcher-home-0.4.1/karcher/map.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     7843 2023-04-26 08:16:45.000000 karcher-home-0.4.1/karcher/mapdata_pb2.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3354 2023-04-28 20:53:54.000000 karcher-home-0.4.1/karcher/mqtt.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3305 2023-05-07 19:24:15.000000 karcher-home-0.4.1/karcher/utils.py
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 19:38:22.339699 karcher-home-0.4.1/karcher_home.egg-info/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1509 2023-05-07 19:38:22.000000 karcher-home-0.4.1/karcher_home.egg-info/PKG-INFO
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      514 2023-05-07 19:38:22.000000 karcher-home-0.4.1/karcher_home.egg-info/SOURCES.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        1 2023-05-07 19:38:22.000000 karcher-home-0.4.1/karcher_home.egg-info/dependency_links.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       54 2023-05-07 19:38:22.000000 karcher-home-0.4.1/karcher_home.egg-info/entry_points.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       46 2023-05-07 19:38:22.000000 karcher-home-0.4.1/karcher_home.egg-info/requires.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        8 2023-05-07 19:38:22.000000 karcher-home-0.4.1/karcher_home.egg-info/top_level.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       79 2023-05-07 19:38:22.339699 karcher-home-0.4.1/setup.cfg
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      845 2023-05-07 19:36:23.000000 karcher-home-0.4.1/setup.py
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 19:38:22.339699 karcher-home-0.4.1/tests/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4294 2023-04-23 21:35:44.000000 karcher-home-0.4.1/tests/test_enc.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 19:56:56.311176 karcher-home-0.4.2/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1066 2023-04-23 18:36:52.000000 karcher-home-0.4.2/LICENSE
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1509 2023-05-07 19:56:56.311176 karcher-home-0.4.2/PKG-INFO
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1120 2023-05-07 19:15:47.000000 karcher-home-0.4.2/README.md
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 19:56:56.311176 karcher-home-0.4.2/karcher/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        0 2023-04-26 11:31:28.000000 karcher-home-0.4.2/karcher/__init__.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2147 2023-04-30 14:40:55.000000 karcher-home-0.4.2/karcher/auth.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5326 2023-05-07 19:56:02.000000 karcher-home-0.4.2/karcher/cli.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2287 2023-04-28 20:14:55.000000 karcher-home-0.4.2/karcher/consts.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5705 2023-04-28 20:58:15.000000 karcher-home-0.4.2/karcher/countries.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5060 2023-04-28 20:50:00.000000 karcher-home-0.4.2/karcher/device.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1663 2023-04-28 20:58:33.000000 karcher-home-0.4.2/karcher/exception.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      592 2023-04-26 12:09:03.000000 karcher-home-0.4.2/karcher/identifiers.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)    14764 2023-05-07 19:54:39.000000 karcher-home-0.4.2/karcher/karcher.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      706 2023-04-28 20:53:12.000000 karcher-home-0.4.2/karcher/map.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     7843 2023-04-26 08:16:45.000000 karcher-home-0.4.2/karcher/mapdata_pb2.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3354 2023-04-28 20:53:54.000000 karcher-home-0.4.2/karcher/mqtt.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3305 2023-05-07 19:24:15.000000 karcher-home-0.4.2/karcher/utils.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 19:56:56.311176 karcher-home-0.4.2/karcher_home.egg-info/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1509 2023-05-07 19:56:56.000000 karcher-home-0.4.2/karcher_home.egg-info/PKG-INFO
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      514 2023-05-07 19:56:56.000000 karcher-home-0.4.2/karcher_home.egg-info/SOURCES.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        1 2023-05-07 19:56:56.000000 karcher-home-0.4.2/karcher_home.egg-info/dependency_links.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       54 2023-05-07 19:56:56.000000 karcher-home-0.4.2/karcher_home.egg-info/entry_points.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       46 2023-05-07 19:56:56.000000 karcher-home-0.4.2/karcher_home.egg-info/requires.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        8 2023-05-07 19:56:56.000000 karcher-home-0.4.2/karcher_home.egg-info/top_level.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       79 2023-05-07 19:56:56.311176 karcher-home-0.4.2/setup.cfg
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      845 2023-05-07 19:56:46.000000 karcher-home-0.4.2/setup.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 19:56:56.311176 karcher-home-0.4.2/tests/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4294 2023-04-23 21:35:44.000000 karcher-home-0.4.2/tests/test_enc.py
```

### Comparing `karcher-home-0.4.1/LICENSE` & `karcher-home-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.1/PKG-INFO` & `karcher-home-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: karcher-home
-Version: 0.4.1
+Version: 0.4.2
 Summary: Kärcher Home Robots client
 Home-page: https://github.com/lafriks/python-karcher
-Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.4.1/karcher-home-0.4.1.tar.gz
+Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.4.2/karcher-home-0.4.2.tar.gz
 Author: Lauris BH
 Author-email: lauris@nix.lv
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `karcher-home-0.4.1/README.md` & `karcher-home-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.1/karcher/auth.py` & `karcher-home-0.4.2/karcher/auth.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.1/karcher/cli.py` & `karcher-home-0.4.2/karcher/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,15 +73,16 @@
     """Tool for connectiong and getting information from Kärcher Home Robots."""
     level = logging.INFO
     if debug > 0:
         level = logging.DEBUG
 
     logging.basicConfig(level=level)
 
-    ctx.obj = GlobalContextObject(debug=debug, output=output, country=country.upper())
+    ctx.obj = GlobalContextObject(
+        debug=debug, output=output, country=country.upper())
 
 
 def safe_cli():
     try:
         cli()
     except KarcherHomeException as ex:
         echo(json.dumps({
@@ -95,29 +96,33 @@
 @click.pass_context
 @coro
 async def urls(ctx: click.Context):
     """Get URL information."""
 
     kh = await KarcherHome.create(country=ctx.obj.country)
     d = await kh.get_urls()
+    await kh.close()
 
     ctx.obj.print(d)
 
 
 @cli.command()
 @click.option('--username', '-u', help='Username to login with.')
 @click.option('--password', '-p', help='Password to login with.')
 @click.pass_context
 @coro
 async def login(ctx: click.Context, username: str, password: str):
     """Get user session tokens."""
 
     kh = await KarcherHome.create(country=ctx.obj.country)
+
     ctx.obj.print(kh.login(username, password))
 
+    await kh.close()
+
 
 @cli.command()
 @click.option('--username', '-u', default=None, help='Username to login with.')
 @click.option('--password', '-p', default=None, help='Password to login with.')
 @click.option('--auth-token', '-t', default=None, help='Authorization token.')
 @click.pass_context
 @coro
@@ -135,14 +140,16 @@
 
     devices = await kh.get_devices()
 
     # Logout if we used a username and password
     if auth_token is None:
         await kh.logout()
 
+    await kh.close()
+
     ctx.obj.print(devices)
 
 
 @cli.command()
 @click.option('--username', '-u', default=None, help='Username to login with.')
 @click.option('--password', '-p', default=None, help='Password to login with.')
 @click.option('--auth-token', '-t', default=None, help='Authorization token.')
@@ -179,8 +186,10 @@
 
     props = kh.get_device_properties(dev)
 
     # Logout if we used a username and password
     if auth_token is None:
         await kh.logout()
 
+    await kh.close()
+
     ctx.obj.print(props)
```

### Comparing `karcher-home-0.4.1/karcher/consts.py` & `karcher-home-0.4.2/karcher/consts.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.1/karcher/countries.py` & `karcher-home-0.4.2/karcher/countries.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.1/karcher/device.py` & `karcher-home-0.4.2/karcher/device.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.1/karcher/exception.py` & `karcher-home-0.4.2/karcher/exception.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.1/karcher/identifiers.py` & `karcher-home-0.4.2/karcher/identifiers.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.1/karcher/karcher.py` & `karcher-home-0.4.2/karcher/karcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,22 +28,26 @@
 )
 
 
 class KarcherHome:
     """Main class to access Karcher Home Robots API"""
 
     @classmethod
-    async def create(cls, country: str = 'GB', language: Language = Language.EN):
+    async def create(cls, country: str = 'GB', language: Language = Language.EN, session: aiohttp.ClientSession = None):
         """Create Karcher Home Robots API instance"""
 
         self = KarcherHome()
         self._country = country.upper()
         self._base_url = REGION_URLS[get_region_by_country(self._country)]
         self._language = language
 
+        if session is not None:
+            self._http_external = True
+            self._http = session
+
         d = await self.get_urls()
         # Update base URLs
         if d.app_api != '':
             self._base_url = d.app_api
         if d.mqtt != '':
             self._mqtt_url = d.mqtt
 
@@ -58,19 +62,35 @@
         self._mqtt_url = None
         self._language = Language.EN
         self._session = None
         self._mqtt = None
         self._device_props = {}
         self._wait_events = {}
 
+    def __del__(self):
+        """Destructor"""
+
+        self.close()
+
+    async def close(self):
+        """Close underlying connections"""
+
+        if self._mqtt is not None:
+            self._mqtt.disconnect()
+            self._mqtt = None
+
+        if self._http is not None:
+            if self._http_external:
+                self._http.close()
+            self._http = None
+
     async def _request(self, method: str, url: str, **kwargs) -> aiohttp.ClientResponse:
-        session = aiohttp.ClientSession()
-        # TODO: Fix SSL
-        # requests.packages.urllib3.disable_warnings()
-        # session.skip = False
+        if self._http is None:
+            self._http_external = False
+            self._http = aiohttp.ClientSession()
 
         headers = {}
         if kwargs.get('headers') is not None:
             headers = kwargs['headers']
 
         headers['User-Agent'] = 'Android_' + TENANT_ID
         auth = ''
@@ -109,35 +129,40 @@
                 kwargs['json'] = v
 
         headers['sign'] = md5(auth + ts + nonce + data)
         headers['ts'] = ts
         headers['nonce'] = nonce
 
         kwargs['headers'] = headers
+        # TODO: Fix SSL
         kwargs['verify_ssl'] = False
-        return await session.request(method, self._base_url + url, **kwargs)
+        return await self._http.request(method, self._base_url + url, **kwargs)
 
     async def _download(self, url) -> bytes:
-        session = aiohttp.ClientSession()
         headers = {
             'User-Agent': 'Android_' + TENANT_ID,
         }
 
-        resp = await session.get(url, headers=headers)
+        resp = await self._http.get(url, headers=headers)
         if resp.status != 200:
             raise KarcherHomeException(-1,
                                        'HTTP error: ' + str(resp.status_code))
 
-        return await resp.content.read(-1)
+        data = await resp.content.read(-1)
+        resp.close()
+
+        return data
 
     async def _process_response(self, resp: aiohttp.ClientResponse, prop=None) -> Any:
         if resp.status != 200:
             raise KarcherHomeException(-1,
                                        'HTTP error: ' + str(resp.status))
         data = await resp.json()
+        resp.close()
+
         # Check for error response
         if data['code'] != 0:
             handle_error_code(data['code'], data['msg'])
         # Check for empty response
         if 'result' not in data:
             return None
         # Handle special response types
@@ -248,17 +273,15 @@
             self._session = None
             return
 
         await self._process_response(await self._request(
             'POST', '/user-center/auth/logout'))
         self._session = None
 
-        if self._mqtt is not None:
-            self._mqtt.disconnect()
-            self._mqtt = None
+        await self.close()
 
     async def get_devices(self) -> List[Device]:
         """Get all user devices."""
 
         if self._session is None \
                 or self._session.auth_token == '' or self._session.user_id == '':
             raise KarcherHomeAccessDenied('Not authorized')
```

### Comparing `karcher-home-0.4.1/karcher/map.py` & `karcher-home-0.4.2/karcher/map.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.1/karcher/mapdata_pb2.py` & `karcher-home-0.4.2/karcher/mapdata_pb2.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.1/karcher/mqtt.py` & `karcher-home-0.4.2/karcher/mqtt.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.1/karcher/utils.py` & `karcher-home-0.4.2/karcher/utils.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.1/karcher_home.egg-info/PKG-INFO` & `karcher-home-0.4.2/karcher_home.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: karcher-home
-Version: 0.4.1
+Version: 0.4.2
 Summary: Kärcher Home Robots client
 Home-page: https://github.com/lafriks/python-karcher
-Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.4.1/karcher-home-0.4.1.tar.gz
+Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.4.2/karcher-home-0.4.2.tar.gz
 Author: Lauris BH
 Author-email: lauris@nix.lv
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `karcher-home-0.4.1/karcher_home.egg-info/SOURCES.txt` & `karcher-home-0.4.2/karcher_home.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.1/setup.py` & `karcher-home-0.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 except ImportError:
     from distutils.core import setup
 
 setup(
     name='karcher-home',
     packages=['karcher'],
     include_package_data=True,
-    version='0.4.1',
+    version='0.4.2',
     license='MIT',
     description='Kärcher Home Robots client',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Lauris BH',
     author_email='lauris@nix.lv',
     url='https://github.com/lafriks/python-karcher',
-    download_url='https://github.com/lafriks/python-karcher/releases/download/v0.4.1/karcher-home-0.4.1.tar.gz',
+    download_url='https://github.com/lafriks/python-karcher/releases/download/v0.4.2/karcher-home-0.4.2.tar.gz',
     platforms='any',
     install_requires=[
         'click',
         'aiohttp',
         'paho-mqtt',
         'cryptography',
         'protobuf'
```

### Comparing `karcher-home-0.4.1/tests/test_enc.py` & `karcher-home-0.4.2/tests/test_enc.py`

 * *Files identical despite different names*

