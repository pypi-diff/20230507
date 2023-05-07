# Comparing `tmp/pythesyncer-23.4.22.13.tar.gz` & `tmp/pythesyncer-23.5.7.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pythesyncer-23.4.22.13.tar", last modified: Sat Apr 22 05:03:12 2023, max compression
+gzip compressed data, was "dist/pythesyncer-23.5.7.12.tar", last modified: Sun May  7 04:35:57 2023, max compression
```

## Comparing `pythesyncer-23.4.22.13.tar` & `pythesyncer-23.5.7.12.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-04-22 05:03:12.103841 pythesyncer-23.4.22.13/
--rw-rw-r--   0 tp03      (1000) tp03      (1000)      434 2023-04-22 05:03:12.099841 pythesyncer-23.4.22.13/PKG-INFO
--rw-r--r--   0 tp03      (1000) tp03      (1000)       76 2023-04-14 11:29:59.000000 pythesyncer-23.4.22.13/README.md
-drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-04-22 05:03:12.099841 pythesyncer-23.4.22.13/pythesyncer/
--rw-r--r--   0 tp03      (1000) tp03      (1000)     3449 2023-04-22 05:02:08.000000 pythesyncer-23.4.22.13/pythesyncer/__init__.py
--rw-r--r--   0 tp03      (1000) tp03      (1000)     1469 2023-04-16 02:52:44.000000 pythesyncer-23.4.22.13/pythesyncer/auth.py
-drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-04-22 05:03:12.099841 pythesyncer-23.4.22.13/pythesyncer.egg-info/
--rw-rw-r--   0 tp03      (1000) tp03      (1000)      434 2023-04-22 05:03:11.000000 pythesyncer-23.4.22.13/pythesyncer.egg-info/PKG-INFO
--rw-rw-r--   0 tp03      (1000) tp03      (1000)      274 2023-04-22 05:03:12.000000 pythesyncer-23.4.22.13/pythesyncer.egg-info/SOURCES.txt
--rw-rw-r--   0 tp03      (1000) tp03      (1000)        1 2023-04-22 05:03:11.000000 pythesyncer-23.4.22.13/pythesyncer.egg-info/dependency_links.txt
--rw-rw-r--   0 tp03      (1000) tp03      (1000)       55 2023-04-22 05:03:11.000000 pythesyncer-23.4.22.13/pythesyncer.egg-info/entry_points.txt
--rw-rw-r--   0 tp03      (1000) tp03      (1000)       20 2023-04-22 05:03:11.000000 pythesyncer-23.4.22.13/pythesyncer.egg-info/requires.txt
--rw-rw-r--   0 tp03      (1000) tp03      (1000)       12 2023-04-22 05:03:11.000000 pythesyncer-23.4.22.13/pythesyncer.egg-info/top_level.txt
--rw-rw-r--   0 tp03      (1000) tp03      (1000)       38 2023-04-22 05:03:12.103841 pythesyncer-23.4.22.13/setup.cfg
--rw-r--r--   0 tp03      (1000) tp03      (1000)      864 2023-04-14 11:58:13.000000 pythesyncer-23.4.22.13/setup.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 04:35:57.698556 pythesyncer-23.5.7.12/
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)      433 2023-05-07 04:35:57.694555 pythesyncer-23.5.7.12/PKG-INFO
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       76 2023-04-14 11:29:59.000000 pythesyncer-23.5.7.12/README.md
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 04:35:57.694555 pythesyncer-23.5.7.12/pythesyncer/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3539 2023-05-07 04:35:08.000000 pythesyncer-23.5.7.12/pythesyncer/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1469 2023-05-07 04:26:41.000000 pythesyncer-23.5.7.12/pythesyncer/auth.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-07 04:35:57.694555 pythesyncer-23.5.7.12/pythesyncer.egg-info/
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)      433 2023-05-07 04:35:57.000000 pythesyncer-23.5.7.12/pythesyncer.egg-info/PKG-INFO
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)      274 2023-05-07 04:35:57.000000 pythesyncer-23.5.7.12/pythesyncer.egg-info/SOURCES.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)        1 2023-05-07 04:35:57.000000 pythesyncer-23.5.7.12/pythesyncer.egg-info/dependency_links.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       55 2023-05-07 04:35:57.000000 pythesyncer-23.5.7.12/pythesyncer.egg-info/entry_points.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       20 2023-05-07 04:35:57.000000 pythesyncer-23.5.7.12/pythesyncer.egg-info/requires.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       12 2023-05-07 04:35:57.000000 pythesyncer-23.5.7.12/pythesyncer.egg-info/top_level.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       38 2023-05-07 04:35:57.698556 pythesyncer-23.5.7.12/setup.cfg
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      864 2023-04-14 11:58:13.000000 pythesyncer-23.5.7.12/setup.py
```

### Comparing `pythesyncer-23.4.22.13/pythesyncer/__init__.py` & `pythesyncer-23.5.7.12/pythesyncer/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 from codefast.asyncio import asyncformer
 from rich import print
 
 from .auth import auth
 
 # —--------------------------------------------
 KEY = 'pythesyncer'
-REDIS_API = auth.redis_api
+POST_API = auth.kv_api + 'set'
+GET_API = auth.kv_api + 'get'
 
 
 class ProgressPercentage(object):
 
     def __init__(self, filename):
         self._filename = filename
         self._size = float(os.path.getsize(filename))
@@ -80,28 +81,29 @@
             format(zipfile, obj))
         await asyncformer(upload_file, zipfile)
         os.remove(zipfile)
         cf.info("Upload done: {}".format(zipfile))
         file_name = zipfile
 
     async with aiohttp.ClientSession() as session:
-        async with session.post(REDIS_API, json={'key': KEY, 'value': file_name}) as resp:
+        async with session.post(POST_API, json={'key': KEY, 'value': file_name}) as resp:
             if resp.status != 200:
                 cf.error('Failed to get redis key: {}'.format(KEY))
 
 
 async def sync_down(obj):
     if not obj:
         async with aiohttp.ClientSession() as session:
-            async with session.post(REDIS_API, json={'key': KEY}) as resp:
+            async with session.post(GET_API, json={'key': KEY}) as resp:
                 if resp.status != 200:
                     cf.error('Failed to get redis key: {}'.format(KEY))
-                js = await resp.json()
-                obj = js['value']
+                text = await resp.text()
+                obj = text.strip()
     remote_file = os.path.join(auth.host_api, obj)
+    cf.info('Downloading file: {}'.format(remote_file))
     await asyncformer(cf.net.download, remote_file, obj)
 
 
 def entry(action: str, obj: str = None):
     if action not in [a.value for a in Action]:
         print('Action must be one of {}'.format([a.value for a in Action]))
         return
```

### Comparing `pythesyncer-23.4.22.13/setup.py` & `pythesyncer-23.5.7.12/setup.py`

 * *Files identical despite different names*

