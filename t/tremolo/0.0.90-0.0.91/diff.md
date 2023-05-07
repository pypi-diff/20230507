# Comparing `tmp/tremolo-0.0.90.tar.gz` & `tmp/tremolo-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tremolo-0.0.90.tar", last modified: Sun May  7 06:39:38 2023, max compression
+gzip compressed data, was "dist/tremolo-0.0.91.tar", last modified: Sun May  7 12:36:52 2023, max compression
```

## Comparing `tremolo-0.0.90.tar` & `tremolo-0.0.91.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 06:39:38.000000 tremolo-0.0.90/
--rw-r--r--   0 tux       (1000) users      (100)     1063 2023-05-07 06:39:21.000000 tremolo-0.0.90/LICENSE.txt
--rw-r--r--   0 tux       (1000) users      (100)     3743 2023-05-07 06:39:38.000000 tremolo-0.0.90/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)     3143 2023-05-07 06:39:21.000000 tremolo-0.0.90/README.md
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-07 06:39:38.000000 tremolo-0.0.90/setup.cfg
--rwxr-xr-x   0 tux       (1000) users      (100)      973 2023-05-07 06:39:21.000000 tremolo-0.0.90/setup.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 06:39:38.000000 tremolo-0.0.90/tremolo/
--rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)     4465 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/__main__.py
--rw-r--r--   0 tux       (1000) users      (100)     2278 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/asgi_lifespan.py
--rw-r--r--   0 tux       (1000) users      (100)     5356 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/asgi_server.py
--rw-r--r--   0 tux       (1000) users      (100)      542 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/contexts.py
--rw-r--r--   0 tux       (1000) users      (100)      586 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/exceptions.py
--rw-r--r--   0 tux       (1000) users      (100)    11243 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/http_server.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 06:39:38.000000 tremolo-0.0.90/tremolo/lib/
--rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)      846 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/connection_pool.py
--rw-r--r--   0 tux       (1000) users      (100)     1798 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/http_exception.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13737 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/http_protocol.py
--rwxr-xr-x   0 tux       (1000) users      (100)     9307 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/http_request.py
--rwxr-xr-x   0 tux       (1000) users      (100)    10924 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/http_response.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 06:39:38.000000 tremolo-0.0.90/tremolo/lib/parsed/
--rw-r--r--   0 tux       (1000) users      (100)       31 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/parsed/__init__.py
--rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/parsed/parse.py
--rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/request.py
--rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/response.py
--rwxr-xr-x   0 tux       (1000) users      (100)    15012 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/tremolo.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 06:39:38.000000 tremolo-0.0.90/tremolo.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)     3743 2023-05-07 06:39:38.000000 tremolo-0.0.90/tremolo.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      603 2023-05-07 06:39:38.000000 tremolo-0.0.90/tremolo.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2023-05-07 06:39:38.000000 tremolo-0.0.90/tremolo.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)        8 2023-05-07 06:39:38.000000 tremolo-0.0.90/tremolo.egg-info/top_level.txt
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 12:36:52.000000 tremolo-0.0.91/
+-rw-r--r--   0 tux       (1000) users      (100)     1063 2023-05-07 11:58:36.000000 tremolo-0.0.91/LICENSE.txt
+-rw-r--r--   0 tux       (1000) users      (100)     3743 2023-05-07 12:36:52.000000 tremolo-0.0.91/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)     3143 2023-05-07 11:58:36.000000 tremolo-0.0.91/README.md
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-07 12:36:52.000000 tremolo-0.0.91/setup.cfg
+-rwxr-xr-x   0 tux       (1000) users      (100)      975 2023-05-07 12:04:23.000000 tremolo-0.0.91/setup.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 12:36:52.000000 tremolo-0.0.91/tremolo/
+-rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)     4465 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/__main__.py
+-rw-r--r--   0 tux       (1000) users      (100)     2278 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/asgi_lifespan.py
+-rw-r--r--   0 tux       (1000) users      (100)     5356 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/asgi_server.py
+-rw-r--r--   0 tux       (1000) users      (100)      542 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/contexts.py
+-rw-r--r--   0 tux       (1000) users      (100)      586 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/exceptions.py
+-rw-r--r--   0 tux       (1000) users      (100)    11243 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/http_server.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 12:36:52.000000 tremolo-0.0.91/tremolo/lib/
+-rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/lib/__init__.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 12:36:52.000000 tremolo-0.0.91/tremolo/lib/h1parser/
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-07 11:24:03.000000 tremolo-0.0.91/tremolo/lib/h1parser/__init__.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-04-16 22:37:48.000000 tremolo-0.0.91/tremolo/lib/h1parser/parse_header.py
+-rw-r--r--   0 tux       (1000) users      (100)     1798 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/lib/http_exception.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    13737 2023-05-07 12:02:00.000000 tremolo-0.0.91/tremolo/lib/http_protocol.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     9307 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/lib/http_request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    10924 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/lib/http_response.py
+-rw-r--r--   0 tux       (1000) users      (100)      844 2023-05-07 11:23:12.000000 tremolo-0.0.91/tremolo/lib/object_pool.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/lib/request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-05-07 11:58:36.000000 tremolo-0.0.91/tremolo/lib/response.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    15287 2023-05-07 11:18:03.000000 tremolo-0.0.91/tremolo/tremolo.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 12:36:52.000000 tremolo-0.0.91/tremolo.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)     3743 2023-05-07 12:36:51.000000 tremolo-0.0.91/tremolo.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      610 2023-05-07 12:36:51.000000 tremolo-0.0.91/tremolo.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2023-05-07 12:36:51.000000 tremolo-0.0.91/tremolo.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)        8 2023-05-07 12:36:51.000000 tremolo-0.0.91/tremolo.egg-info/top_level.txt
```

### Comparing `tremolo-0.0.90/LICENSE.txt` & `tremolo-0.0.91/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.90/PKG-INFO` & `tremolo-0.0.91/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.90
+Version: 0.0.91
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tremolo-0.0.90/README.md` & `tremolo-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.90/setup.py` & `tremolo-0.0.91/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tremolo',
     packages=['tremolo'],
-    package_data={'': ['lib/*', 'lib/parsed/*']},
-    version='0.0.90',
+    package_data={'': ['lib/*', 'lib/h1parser/*']},
+    version='0.0.91',
     license='MIT',
     author='nggit',
     author_email='contact@anggit.com',
     description='Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nggit/tremolo',
```

### Comparing `tremolo-0.0.90/tremolo/__main__.py` & `tremolo-0.0.91/tremolo/__main__.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.90/tremolo/asgi_lifespan.py` & `tremolo-0.0.91/tremolo/asgi_lifespan.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.90/tremolo/asgi_server.py` & `tremolo-0.0.91/tremolo/asgi_server.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.90/tremolo/contexts.py` & `tremolo-0.0.91/tremolo/contexts.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.90/tremolo/exceptions.py` & `tremolo-0.0.91/tremolo/exceptions.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.90/tremolo/http_server.py` & `tremolo-0.0.91/tremolo/http_server.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.90/tremolo/lib/connection_pool.py` & `tremolo-0.0.91/tremolo/lib/object_pool.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) 2023 nggit
 
 import asyncio
 
-from .parsed import ParseHeader
+from .h1parser import ParseHeader
 
-class ConnectionPool:
+class ObjectPool:
     def __init__(self, pool_size, logger):
         self._pool_size = pool_size
         self._pools = []
         self._logger = logger
 
         for _ in range(pool_size):
             self._pools.append(self._create())
```

### Comparing `tremolo-0.0.90/tremolo/lib/http_exception.py` & `tremolo-0.0.91/tremolo/lib/http_exception.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.90/tremolo/lib/http_protocol.py` & `tremolo-0.0.91/tremolo/lib/http_protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,17 +50,17 @@
 
     @property
     def header(self):
         return self._header
 
     def connection_made(self, transport):
         self._transport = transport
-        self._conn = self._options['_pool'].get()
-        self._queue = self._conn['queue']
-        self._header = self._conn['header']
+        self._pool = self._options['_pool'].get()
+        self._queue = self._pool['queue']
+        self._header = self._pool['header']
         self._request = None
         self._response = None
 
         self._data = bytearray()
         self._timeout_waiters = {'request': self._loop.create_future()}
 
         for task in (self._send_data(), self.set_timeout(self._timeout_waiters['request'],
```

### Comparing `tremolo-0.0.90/tremolo/lib/http_request.py` & `tremolo-0.0.91/tremolo/lib/http_request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.90/tremolo/lib/http_response.py` & `tremolo-0.0.91/tremolo/lib/http_response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.90/tremolo/lib/parsed/parse.py` & `tremolo-0.0.91/tremolo/lib/h1parser/parse_header.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.90/tremolo/lib/request.py` & `tremolo-0.0.91/tremolo/lib/request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.90/tremolo/lib/response.py` & `tremolo-0.0.91/tremolo/lib/response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.90/tremolo/tremolo.py` & `tremolo-0.0.91/tremolo/tremolo.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import time
 
 from copy import deepcopy
 from datetime import datetime
 from functools import wraps
 from importlib import import_module
 
-from .lib.connection_pool import ConnectionPool
+from .lib.object_pool import ObjectPool
 from .exceptions import BadRequest
 
 class Tremolo:
     def __init__(self):
         self._ports = []
 
         self._route_handlers = {
@@ -200,15 +200,15 @@
 
         if isinstance(server_name, str):
             server_name = server_name.encode(encoding='latin-1')
 
         if isinstance(host, str):
             host = host.encode(encoding='latin-1')
 
-        pool = ConnectionPool(1024, self._logger)
+        pool = ObjectPool(1024, self._logger)
         lifespan = None
 
         if 'app' in options and isinstance(options['app'], str):
             from .asgi_lifespan import ASGILifespan
             from .asgi_server import ASGIServer as Server
 
             # 'module:app'               -> 'module:app'   (dir: os.getcwd())
@@ -222,14 +222,19 @@
             if dir_name == '':
                 dir_name = os.getcwd()
 
             sys.path.insert(0, dir_name)
 
             options['app'] = getattr(import_module(module_name), attr_name)
 
+            print(datetime.now().strftime('[%Y-%m-%d %H:%M:%S]'), end=' ')
+            sys.stdout.flush()
+            sys.stdout.buffer.write(b'Starting %s as an ASGI server for: ' % server_name)
+            print(getattr(options['app'], '__name__', options['app'].__class__.__name__))
+
             if server_name != b'':
                 server_name = server_name + b' (ASGI)'
 
             lifespan = ASGILifespan(options['app'], loop=self._loop, logger=self._logger)
 
             lifespan.startup()
             exc = await lifespan.exception()
```

### Comparing `tremolo-0.0.90/tremolo.egg-info/PKG-INFO` & `tremolo-0.0.91/tremolo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.90
+Version: 0.0.91
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tremolo-0.0.90/tremolo.egg-info/SOURCES.txt` & `tremolo-0.0.91/tremolo.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 tremolo/http_server.py
 tremolo/tremolo.py
 tremolo.egg-info/PKG-INFO
 tremolo.egg-info/SOURCES.txt
 tremolo.egg-info/dependency_links.txt
 tremolo.egg-info/top_level.txt
 tremolo/lib/__init__.py
-tremolo/lib/connection_pool.py
 tremolo/lib/http_exception.py
 tremolo/lib/http_protocol.py
 tremolo/lib/http_request.py
 tremolo/lib/http_response.py
+tremolo/lib/object_pool.py
 tremolo/lib/request.py
 tremolo/lib/response.py
-tremolo/lib/parsed/__init__.py
-tremolo/lib/parsed/parse.py
+tremolo/lib/h1parser/__init__.py
+tremolo/lib/h1parser/parse_header.py
```

