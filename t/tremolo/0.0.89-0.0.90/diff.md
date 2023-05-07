# Comparing `tmp/tremolo-0.0.89.tar.gz` & `tmp/tremolo-0.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tremolo-0.0.89.tar", last modified: Sun May  7 03:11:30 2023, max compression
+gzip compressed data, was "dist/tremolo-0.0.90.tar", last modified: Sun May  7 06:39:38 2023, max compression
```

## Comparing `tremolo-0.0.89.tar` & `tremolo-0.0.90.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 03:11:30.000000 tremolo-0.0.89/
--rw-r--r--   0 tux       (1000) users      (100)     4740 2023-05-07 03:11:30.000000 tremolo-0.0.89/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)     3143 2023-05-07 03:11:14.000000 tremolo-0.0.89/README.md
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-07 03:11:30.000000 tremolo-0.0.89/setup.cfg
--rwxr-xr-x   0 tux       (1000) users      (100)      973 2023-05-07 03:11:14.000000 tremolo-0.0.89/setup.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 03:11:30.000000 tremolo-0.0.89/tremolo/
--rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-05-07 03:11:14.000000 tremolo-0.0.89/tremolo/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)     4465 2023-05-07 03:11:14.000000 tremolo-0.0.89/tremolo/__main__.py
--rw-r--r--   0 tux       (1000) users      (100)     2278 2023-05-07 03:11:14.000000 tremolo-0.0.89/tremolo/asgi_lifespan.py
--rw-r--r--   0 tux       (1000) users      (100)     5356 2023-05-07 03:11:14.000000 tremolo-0.0.89/tremolo/asgi_server.py
--rw-r--r--   0 tux       (1000) users      (100)      542 2023-05-07 03:11:14.000000 tremolo-0.0.89/tremolo/contexts.py
--rw-r--r--   0 tux       (1000) users      (100)      586 2023-05-07 03:11:14.000000 tremolo-0.0.89/tremolo/exceptions.py
--rw-r--r--   0 tux       (1000) users      (100)    11243 2023-05-07 03:11:14.000000 tremolo-0.0.89/tremolo/http_server.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 03:11:30.000000 tremolo-0.0.89/tremolo/lib/
--rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 03:11:14.000000 tremolo-0.0.89/tremolo/lib/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)      846 2023-05-07 03:11:14.000000 tremolo-0.0.89/tremolo/lib/connection_pool.py
--rw-r--r--   0 tux       (1000) users      (100)     1798 2023-05-07 03:11:14.000000 tremolo-0.0.89/tremolo/lib/http_exception.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13737 2023-05-07 03:11:14.000000 tremolo-0.0.89/tremolo/lib/http_protocol.py
--rwxr-xr-x   0 tux       (1000) users      (100)     9155 2023-05-07 03:11:14.000000 tremolo-0.0.89/tremolo/lib/http_request.py
--rwxr-xr-x   0 tux       (1000) users      (100)    10924 2023-05-07 03:11:14.000000 tremolo-0.0.89/tremolo/lib/http_response.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 03:11:30.000000 tremolo-0.0.89/tremolo/lib/parsed/
--rw-r--r--   0 tux       (1000) users      (100)       31 2023-05-07 03:11:14.000000 tremolo-0.0.89/tremolo/lib/parsed/__init__.py
--rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-05-07 03:11:14.000000 tremolo-0.0.89/tremolo/lib/parsed/parse.py
--rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-05-07 03:11:14.000000 tremolo-0.0.89/tremolo/lib/request.py
--rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-05-07 03:11:14.000000 tremolo-0.0.89/tremolo/lib/response.py
--rwxr-xr-x   0 tux       (1000) users      (100)    15012 2023-05-07 03:11:14.000000 tremolo-0.0.89/tremolo/tremolo.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 03:11:30.000000 tremolo-0.0.89/tremolo.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)     4740 2023-05-07 03:11:30.000000 tremolo-0.0.89/tremolo.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      591 2023-05-07 03:11:30.000000 tremolo-0.0.89/tremolo.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2023-05-07 03:11:30.000000 tremolo-0.0.89/tremolo.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)        8 2023-05-07 03:11:30.000000 tremolo-0.0.89/tremolo.egg-info/top_level.txt
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 06:39:38.000000 tremolo-0.0.90/
+-rw-r--r--   0 tux       (1000) users      (100)     1063 2023-05-07 06:39:21.000000 tremolo-0.0.90/LICENSE.txt
+-rw-r--r--   0 tux       (1000) users      (100)     3743 2023-05-07 06:39:38.000000 tremolo-0.0.90/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)     3143 2023-05-07 06:39:21.000000 tremolo-0.0.90/README.md
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-07 06:39:38.000000 tremolo-0.0.90/setup.cfg
+-rwxr-xr-x   0 tux       (1000) users      (100)      973 2023-05-07 06:39:21.000000 tremolo-0.0.90/setup.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 06:39:38.000000 tremolo-0.0.90/tremolo/
+-rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)     4465 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/__main__.py
+-rw-r--r--   0 tux       (1000) users      (100)     2278 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/asgi_lifespan.py
+-rw-r--r--   0 tux       (1000) users      (100)     5356 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/asgi_server.py
+-rw-r--r--   0 tux       (1000) users      (100)      542 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/contexts.py
+-rw-r--r--   0 tux       (1000) users      (100)      586 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/exceptions.py
+-rw-r--r--   0 tux       (1000) users      (100)    11243 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/http_server.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 06:39:38.000000 tremolo-0.0.90/tremolo/lib/
+-rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)      846 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/connection_pool.py
+-rw-r--r--   0 tux       (1000) users      (100)     1798 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/http_exception.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    13737 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/http_protocol.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     9307 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/http_request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    10924 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/http_response.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 06:39:38.000000 tremolo-0.0.90/tremolo/lib/parsed/
+-rw-r--r--   0 tux       (1000) users      (100)       31 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/parsed/__init__.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/parsed/parse.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/lib/response.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    15012 2023-05-07 06:39:21.000000 tremolo-0.0.90/tremolo/tremolo.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-07 06:39:38.000000 tremolo-0.0.90/tremolo.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)     3743 2023-05-07 06:39:38.000000 tremolo-0.0.90/tremolo.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      603 2023-05-07 06:39:38.000000 tremolo-0.0.90/tremolo.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2023-05-07 06:39:38.000000 tremolo-0.0.90/tremolo.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)        8 2023-05-07 06:39:38.000000 tremolo-0.0.90/tremolo.egg-info/top_level.txt
```

### Comparing `tremolo-0.0.89/README.md` & `tremolo-0.0.90/README.md`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.89/setup.py` & `tremolo-0.0.90/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tremolo',
     packages=['tremolo'],
     package_data={'': ['lib/*', 'lib/parsed/*']},
-    version='0.0.89',
+    version='0.0.90',
     license='MIT',
     author='nggit',
     author_email='contact@anggit.com',
     description='Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nggit/tremolo',
```

### Comparing `tremolo-0.0.89/tremolo/__main__.py` & `tremolo-0.0.90/tremolo/__main__.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.89/tremolo/asgi_lifespan.py` & `tremolo-0.0.90/tremolo/asgi_lifespan.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.89/tremolo/asgi_server.py` & `tremolo-0.0.90/tremolo/asgi_server.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.89/tremolo/contexts.py` & `tremolo-0.0.90/tremolo/contexts.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.89/tremolo/exceptions.py` & `tremolo-0.0.90/tremolo/exceptions.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.89/tremolo/http_server.py` & `tremolo-0.0.90/tremolo/http_server.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.89/tremolo/lib/connection_pool.py` & `tremolo-0.0.90/tremolo/lib/connection_pool.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.89/tremolo/lib/http_exception.py` & `tremolo-0.0.90/tremolo/lib/http_exception.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.89/tremolo/lib/http_protocol.py` & `tremolo-0.0.90/tremolo/lib/http_protocol.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.89/tremolo/lib/http_request.py` & `tremolo-0.0.90/tremolo/lib/http_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 
             while buf != b'0\r\n\r\n':
                 if not paused:
                     try:
                         buf.extend(await agen.__anext__())
                     except StopAsyncIteration:
                         if not buf.endswith(b'0\r\n\r\n'):
+                            del buf[:]
                             raise BadRequest('bad chunked encoding: incomplete read')
 
                 if tobe_read > 0:
                     data = buf[:tobe_read]
 
                     yield data
                     del buf[:tobe_read]
@@ -96,14 +97,15 @@
                     paused = True
                     del buf[:2]
                 else:
                     i = buf.find(b'\r\n')
 
                     if i == -1:
                         if len(buf) > self.protocol.options['buffer_size'] * 4:
+                            del buf[:]
                             raise BadRequest('bad chunked encoding: no chunk size')
 
                         paused = False
                         continue
 
                     try:
                         chunk_size = int(buf[:i].split(b';', 1)[0], 16)
@@ -240,22 +242,24 @@
             data = b''
 
             if not paused:
                 try:
                     data = await agen.__anext__()
                 except StopAsyncIteration:
                     if header_size == -1 or body_size == -1:
+                        del body[:]
                         raise BadRequest('malformed multipart/form-data')
 
             if isinstance(header, bytearray):
                 header.extend(data)
                 header_size = header.find(b'\r\n\r\n')
 
                 if header_size == -1:
                     if len(header) > 8192:
+                        del header[:]
                         raise BadRequest('malformed multipart/form-data')
 
                     paused = False
                 else:
                     body = header[header_size + 4:]
                     info = {}
```

### Comparing `tremolo-0.0.89/tremolo/lib/http_response.py` & `tremolo-0.0.90/tremolo/lib/http_response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.89/tremolo/lib/parsed/parse.py` & `tremolo-0.0.90/tremolo/lib/parsed/parse.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.89/tremolo/lib/request.py` & `tremolo-0.0.90/tremolo/lib/request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.89/tremolo/lib/response.py` & `tremolo-0.0.90/tremolo/lib/response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.89/tremolo/tremolo.py` & `tremolo-0.0.90/tremolo/tremolo.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.89/tremolo.egg-info/SOURCES.txt` & `tremolo-0.0.90/tremolo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 setup.py
 tremolo/__init__.py
 tremolo/__main__.py
 tremolo/asgi_lifespan.py
 tremolo/asgi_server.py
 tremolo/contexts.py
```

