# Comparing `tmp/karcher-home-0.4.3.tar.gz` & `tmp/karcher-home-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karcher-home-0.4.3.tar", last modified: Sun May  7 20:13:18 2023, max compression
+gzip compressed data, was "karcher-home-0.4.4.tar", last modified: Sun May  7 20:22:01 2023, max compression
```

## Comparing `karcher-home-0.4.3.tar` & `karcher-home-0.4.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 20:13:18.294693 karcher-home-0.4.3/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1066 2023-04-23 18:36:52.000000 karcher-home-0.4.3/LICENSE
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1509 2023-05-07 20:13:18.294693 karcher-home-0.4.3/PKG-INFO
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1120 2023-05-07 19:15:47.000000 karcher-home-0.4.3/README.md
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 20:13:18.290692 karcher-home-0.4.3/karcher/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        0 2023-04-26 11:31:28.000000 karcher-home-0.4.3/karcher/__init__.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2147 2023-04-30 14:40:55.000000 karcher-home-0.4.3/karcher/auth.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5292 2023-05-07 20:09:10.000000 karcher-home-0.4.3/karcher/cli.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2446 2023-05-07 20:08:27.000000 karcher-home-0.4.3/karcher/consts.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5705 2023-04-28 20:58:15.000000 karcher-home-0.4.3/karcher/countries.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5060 2023-04-28 20:50:00.000000 karcher-home-0.4.3/karcher/device.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1663 2023-04-28 20:58:33.000000 karcher-home-0.4.3/karcher/exception.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      592 2023-04-26 12:09:03.000000 karcher-home-0.4.3/karcher/identifiers.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)    14942 2023-05-07 20:09:49.000000 karcher-home-0.4.3/karcher/karcher.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      706 2023-04-28 20:53:12.000000 karcher-home-0.4.3/karcher/map.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     7843 2023-04-26 08:16:45.000000 karcher-home-0.4.3/karcher/mapdata_pb2.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3354 2023-04-28 20:53:54.000000 karcher-home-0.4.3/karcher/mqtt.py
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3305 2023-05-07 19:24:15.000000 karcher-home-0.4.3/karcher/utils.py
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 20:13:18.294693 karcher-home-0.4.3/karcher_home.egg-info/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1509 2023-05-07 20:13:18.000000 karcher-home-0.4.3/karcher_home.egg-info/PKG-INFO
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      514 2023-05-07 20:13:18.000000 karcher-home-0.4.3/karcher_home.egg-info/SOURCES.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        1 2023-05-07 20:13:18.000000 karcher-home-0.4.3/karcher_home.egg-info/dependency_links.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       54 2023-05-07 20:13:18.000000 karcher-home-0.4.3/karcher_home.egg-info/entry_points.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       46 2023-05-07 20:13:18.000000 karcher-home-0.4.3/karcher_home.egg-info/requires.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        8 2023-05-07 20:13:18.000000 karcher-home-0.4.3/karcher_home.egg-info/top_level.txt
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       79 2023-05-07 20:13:18.294693 karcher-home-0.4.3/setup.cfg
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      845 2023-05-07 20:12:12.000000 karcher-home-0.4.3/setup.py
-drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 20:13:18.294693 karcher-home-0.4.3/tests/
--rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4294 2023-04-23 21:35:44.000000 karcher-home-0.4.3/tests/test_enc.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 20:22:01.164382 karcher-home-0.4.4/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1066 2023-04-23 18:36:52.000000 karcher-home-0.4.4/LICENSE
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1509 2023-05-07 20:22:01.164382 karcher-home-0.4.4/PKG-INFO
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1120 2023-05-07 19:15:47.000000 karcher-home-0.4.4/README.md
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 20:22:01.160382 karcher-home-0.4.4/karcher/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        0 2023-04-26 11:31:28.000000 karcher-home-0.4.4/karcher/__init__.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2147 2023-04-30 14:40:55.000000 karcher-home-0.4.4/karcher/auth.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5292 2023-05-07 20:09:10.000000 karcher-home-0.4.4/karcher/cli.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     2446 2023-05-07 20:08:27.000000 karcher-home-0.4.4/karcher/consts.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5705 2023-04-28 20:58:15.000000 karcher-home-0.4.4/karcher/countries.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     5060 2023-04-28 20:50:00.000000 karcher-home-0.4.4/karcher/device.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1663 2023-04-28 20:58:33.000000 karcher-home-0.4.4/karcher/exception.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      592 2023-04-26 12:09:03.000000 karcher-home-0.4.4/karcher/identifiers.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)    14971 2023-05-07 20:19:29.000000 karcher-home-0.4.4/karcher/karcher.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      706 2023-04-28 20:53:12.000000 karcher-home-0.4.4/karcher/map.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     7843 2023-04-26 08:16:45.000000 karcher-home-0.4.4/karcher/mapdata_pb2.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3354 2023-04-28 20:53:54.000000 karcher-home-0.4.4/karcher/mqtt.py
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     3305 2023-05-07 19:24:15.000000 karcher-home-0.4.4/karcher/utils.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 20:22:01.164382 karcher-home-0.4.4/karcher_home.egg-info/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     1509 2023-05-07 20:22:01.000000 karcher-home-0.4.4/karcher_home.egg-info/PKG-INFO
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      514 2023-05-07 20:22:01.000000 karcher-home-0.4.4/karcher_home.egg-info/SOURCES.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        1 2023-05-07 20:22:01.000000 karcher-home-0.4.4/karcher_home.egg-info/dependency_links.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       54 2023-05-07 20:22:01.000000 karcher-home-0.4.4/karcher_home.egg-info/entry_points.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       46 2023-05-07 20:22:01.000000 karcher-home-0.4.4/karcher_home.egg-info/requires.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)        8 2023-05-07 20:22:01.000000 karcher-home-0.4.4/karcher_home.egg-info/top_level.txt
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)       79 2023-05-07 20:22:01.164382 karcher-home-0.4.4/setup.cfg
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)      845 2023-05-07 20:21:39.000000 karcher-home-0.4.4/setup.py
+drwxrwxr-x   0 lafriks   (1000) lafriks   (1000)        0 2023-05-07 20:22:01.164382 karcher-home-0.4.4/tests/
+-rw-rw-r--   0 lafriks   (1000) lafriks   (1000)     4294 2023-04-23 21:35:44.000000 karcher-home-0.4.4/tests/test_enc.py
```

### Comparing `karcher-home-0.4.3/LICENSE` & `karcher-home-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.3/PKG-INFO` & `karcher-home-0.4.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: karcher-home
-Version: 0.4.3
+Version: 0.4.4
 Summary: Kärcher Home Robots client
 Home-page: https://github.com/lafriks/python-karcher
-Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.4.3/karcher-home-0.4.3.tar.gz
+Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.4.4/karcher-home-0.4.4.tar.gz
 Author: Lauris BH
 Author-email: lauris@nix.lv
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `karcher-home-0.4.3/README.md` & `karcher-home-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.3/karcher/auth.py` & `karcher-home-0.4.4/karcher/auth.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.3/karcher/cli.py` & `karcher-home-0.4.4/karcher/cli.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.3/karcher/consts.py` & `karcher-home-0.4.4/karcher/consts.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.3/karcher/countries.py` & `karcher-home-0.4.4/karcher/countries.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.3/karcher/device.py` & `karcher-home-0.4.4/karcher/device.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.3/karcher/exception.py` & `karcher-home-0.4.4/karcher/exception.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.3/karcher/identifiers.py` & `karcher-home-0.4.4/karcher/identifiers.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.3/karcher/karcher.py` & `karcher-home-0.4.4/karcher/karcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         """Close underlying connections"""
 
         if self._mqtt is not None:
             self._mqtt.disconnect()
             self._mqtt = None
 
         if self._http is not None:
-            if self._http_external:
+            if not self._http_external:
                 self._http.close()
             self._http = None
 
     async def _request(self, method: str, url: str, **kwargs) -> aiohttp.ClientResponse:
         if self._http is None:
             self._http_external = False
             self._http = aiohttp.ClientSession()
@@ -156,14 +156,15 @@
         data = await resp.content.read(-1)
         resp.close()
 
         return data
 
     async def _process_response(self, resp: aiohttp.ClientResponse, prop=None) -> Any:
         if resp.status != 200:
+            resp.close()
             raise KarcherHomeException(-1,
                                        'HTTP error: ' + str(resp.status))
         data = await resp.json()
         resp.close()
 
         # Check for error response
         if data['code'] != 0:
```

### Comparing `karcher-home-0.4.3/karcher/map.py` & `karcher-home-0.4.4/karcher/map.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.3/karcher/mapdata_pb2.py` & `karcher-home-0.4.4/karcher/mapdata_pb2.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.3/karcher/mqtt.py` & `karcher-home-0.4.4/karcher/mqtt.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.3/karcher/utils.py` & `karcher-home-0.4.4/karcher/utils.py`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.3/karcher_home.egg-info/PKG-INFO` & `karcher-home-0.4.4/karcher_home.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: karcher-home
-Version: 0.4.3
+Version: 0.4.4
 Summary: Kärcher Home Robots client
 Home-page: https://github.com/lafriks/python-karcher
-Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.4.3/karcher-home-0.4.3.tar.gz
+Download-URL: https://github.com/lafriks/python-karcher/releases/download/v0.4.4/karcher-home-0.4.4.tar.gz
 Author: Lauris BH
 Author-email: lauris@nix.lv
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `karcher-home-0.4.3/karcher_home.egg-info/SOURCES.txt` & `karcher-home-0.4.4/karcher_home.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `karcher-home-0.4.3/setup.py` & `karcher-home-0.4.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 except ImportError:
     from distutils.core import setup
 
 setup(
     name='karcher-home',
     packages=['karcher'],
     include_package_data=True,
-    version='0.4.3',
+    version='0.4.4',
     license='MIT',
     description='Kärcher Home Robots client',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Lauris BH',
     author_email='lauris@nix.lv',
     url='https://github.com/lafriks/python-karcher',
-    download_url='https://github.com/lafriks/python-karcher/releases/download/v0.4.3/karcher-home-0.4.3.tar.gz',
+    download_url='https://github.com/lafriks/python-karcher/releases/download/v0.4.4/karcher-home-0.4.4.tar.gz',
     platforms='any',
     install_requires=[
         'click',
         'aiohttp',
         'paho-mqtt',
         'cryptography',
         'protobuf'
```

### Comparing `karcher-home-0.4.3/tests/test_enc.py` & `karcher-home-0.4.4/tests/test_enc.py`

 * *Files identical despite different names*

