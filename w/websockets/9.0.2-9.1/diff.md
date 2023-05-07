# Comparing `tmp/websockets-9.0.2.tar.gz` & `tmp/websockets-9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "websockets-9.0.2.tar", last modified: Sat May 15 16:02:00 2021, max compression
+gzip compressed data, was "websockets-9.1.tar", last modified: Thu May 27 19:26:04 2021, max compression
```

## Comparing `websockets-9.0.2.tar` & `websockets-9.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 16:02:00.109343 websockets-9.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1536 2021-05-15 16:01:57.000000 websockets-9.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-05-15 16:01:57.000000 websockets-9.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7250 2021-05-15 16:02:00.109343 websockets-9.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6251 2021-05-15 16:01:57.000000 websockets-9.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      430 2021-05-15 16:02:00.109343 websockets-9.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2021-05-15 16:01:57.000000 websockets-9.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 16:02:00.105343 websockets-9.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 16:02:00.109343 websockets-9.0.2/src/websockets/
--rw-r--r--   0 runner    (1001) docker     (121)     3232 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6803 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      111 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)    10270 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    13953 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     4961 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (121)     9007 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 16:02:00.109343 websockets-9.0.2/src/websockets/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2783 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/extensions/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    23221 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/extensions/permessage_deflate.py
--rw-r--r--   0 runner    (1001) docker     (121)     9454 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/frames.py
--rw-r--r--   0 runner    (1001) docker     (121)    14912 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/headers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/http.py
--rw-r--r--   0 runner    (1001) docker     (121)    10688 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/http11.py
--rw-r--r--   0 runner    (1001) docker     (121)     3225 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 16:02:00.109343 websockets-9.0.2/src/websockets/legacy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5531 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/legacy/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)    25679 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/legacy/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4624 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/legacy/framing.py
--rw-r--r--   0 runner    (1001) docker     (121)     6225 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/legacy/handshake.py
--rw-r--r--   0 runner    (1001) docker     (121)     6838 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/legacy/http.py
--rw-r--r--   0 runner    (1001) docker     (121)    51673 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/legacy/protocol.py
--rw-r--r--   0 runner    (1001) docker     (121)    43441 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/legacy/server.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    15936 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/server.py
--rw-r--r--   0 runner    (1001) docker     (121)     5316 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/speedups.c
--rw-r--r--   0 runner    (1001) docker     (121)     3004 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/streams.py
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2828 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/uri.py
--rw-r--r--   0 runner    (1001) docker     (121)      928 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-05-15 16:01:57.000000 websockets-9.0.2/src/websockets/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 16:02:00.109343 websockets-9.0.2/src/websockets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7250 2021-05-15 16:01:59.000000 websockets-9.0.2/src/websockets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2021-05-15 16:02:00.000000 websockets-9.0.2/src/websockets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-15 16:01:59.000000 websockets-9.0.2/src/websockets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-15 16:01:59.000000 websockets-9.0.2/src/websockets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-05-15 16:01:59.000000 websockets-9.0.2/src/websockets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 19:26:04.040748 websockets-9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1536 2021-05-27 19:26:01.000000 websockets-9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2021-05-27 19:26:01.000000 websockets-9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7248 2021-05-27 19:26:04.040748 websockets-9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6251 2021-05-27 19:26:01.000000 websockets-9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      430 2021-05-27 19:26:04.040748 websockets-9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1941 2021-05-27 19:26:01.000000 websockets-9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 19:26:04.032748 websockets-9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 19:26:04.036748 websockets-9.1/src/websockets/
+-rw-r--r--   0 runner    (1001) docker     (121)     3232 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6803 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10270 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13953 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4961 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9007 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 19:26:04.036748 websockets-9.1/src/websockets/extensions/
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2783 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/extensions/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23221 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/extensions/permessage_deflate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9454 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/frames.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14912 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/headers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/http.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10688 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/http11.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3225 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 19:26:04.040748 websockets-9.1/src/websockets/legacy/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5589 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/legacy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25679 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/legacy/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4624 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/legacy/framing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6225 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/legacy/handshake.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6838 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/legacy/http.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51673 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/legacy/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43441 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/legacy/server.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    15936 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/server.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5316 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/speedups.c
+-rw-r--r--   0 runner    (1001) docker     (121)     3004 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/streams.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1508 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/typing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2828 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/uri.py
+-rw-r--r--   0 runner    (1001) docker     (121)      928 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-05-27 19:26:01.000000 websockets-9.1/src/websockets/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-27 19:26:04.036748 websockets-9.1/src/websockets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7248 2021-05-27 19:26:03.000000 websockets-9.1/src/websockets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1134 2021-05-27 19:26:04.000000 websockets-9.1/src/websockets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-27 19:26:03.000000 websockets-9.1/src/websockets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-27 19:26:03.000000 websockets-9.1/src/websockets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2021-05-27 19:26:03.000000 websockets-9.1/src/websockets.egg-info/top_level.txt
```

### Comparing `websockets-9.0.2/LICENSE` & `websockets-9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/PKG-INFO` & `websockets-9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: websockets
-Version: 9.0.2
+Version: 9.1
 Summary: An implementation of the WebSocket Protocol (RFC 6455 & 7692)
 Home-page: https://github.com/aaugustin/websockets
 Author: Aymeric Augustin
 Author-email: aymeric.augustin@m4x.org
 License: BSD
 Description: .. image:: logo/horizontal.svg
            :width: 480px
```

### Comparing `websockets-9.0.2/README.rst` & `websockets-9.1/README.rst`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/setup.py` & `websockets-9.1/setup.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/__init__.py` & `websockets-9.1/src/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/__main__.py` & `websockets-9.1/src/websockets/__main__.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/client.py` & `websockets-9.1/src/websockets/client.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/connection.py` & `websockets-9.1/src/websockets/connection.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/datastructures.py` & `websockets-9.1/src/websockets/datastructures.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/exceptions.py` & `websockets-9.1/src/websockets/exceptions.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/extensions/base.py` & `websockets-9.1/src/websockets/extensions/base.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/extensions/permessage_deflate.py` & `websockets-9.1/src/websockets/extensions/permessage_deflate.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/frames.py` & `websockets-9.1/src/websockets/frames.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/headers.py` & `websockets-9.1/src/websockets/headers.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/http.py` & `websockets-9.1/src/websockets/http.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/http11.py` & `websockets-9.1/src/websockets/http11.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/imports.py` & `websockets-9.1/src/websockets/imports.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/legacy/auth.py` & `websockets-9.1/src/websockets/legacy/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 :mod:`websockets.legacy.auth` provides HTTP Basic Authentication according to
 :rfc:`7235` and :rfc:`7617`.
 
 """
 
 
 import functools
+import hmac
 import http
 from typing import Any, Awaitable, Callable, Iterable, Optional, Tuple, Union, cast
 
 from ..datastructures import Headers
 from ..exceptions import InvalidHeader
 from ..headers import build_www_authenticate_basic, parse_authorization_basic
 from .server import HTTPResponse, WebSocketServerProtocol
@@ -128,35 +129,36 @@
 
     """
     if (credentials is None) == (check_credentials is None):
         raise TypeError("provide either credentials or check_credentials")
 
     if credentials is not None:
         if is_credentials(credentials):
-
-            async def check_credentials(username: str, password: str) -> bool:
-                return (username, password) == credentials
-
+            credentials_list = [cast(Credentials, credentials)]
         elif isinstance(credentials, Iterable):
             credentials_list = list(credentials)
-            if all(is_credentials(item) for item in credentials_list):
-                credentials_dict = dict(credentials_list)
-
-                async def check_credentials(username: str, password: str) -> bool:
-                    return credentials_dict.get(username) == password
-
-            else:
+            if not all(is_credentials(item) for item in credentials_list):
                 raise TypeError(f"invalid credentials argument: {credentials}")
-
         else:
             raise TypeError(f"invalid credentials argument: {credentials}")
 
+        credentials_dict = dict(credentials_list)
+
+        async def check_credentials(username: str, password: str) -> bool:
+            try:
+                expected_password = credentials_dict[username]
+            except KeyError:
+                return False
+            return hmac.compare_digest(expected_password, password)
+
     if create_protocol is None:
         # Not sure why mypy cannot figure this out.
         create_protocol = cast(
             Callable[[Any], BasicAuthWebSocketServerProtocol],
             BasicAuthWebSocketServerProtocol,
         )
 
     return functools.partial(
-        create_protocol, realm=realm, check_credentials=check_credentials
+        create_protocol,
+        realm=realm,
+        check_credentials=check_credentials,
     )
```

### Comparing `websockets-9.0.2/src/websockets/legacy/client.py` & `websockets-9.1/src/websockets/legacy/client.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/legacy/framing.py` & `websockets-9.1/src/websockets/legacy/framing.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/legacy/handshake.py` & `websockets-9.1/src/websockets/legacy/handshake.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/legacy/http.py` & `websockets-9.1/src/websockets/legacy/http.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/legacy/protocol.py` & `websockets-9.1/src/websockets/legacy/protocol.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/legacy/server.py` & `websockets-9.1/src/websockets/legacy/server.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/server.py` & `websockets-9.1/src/websockets/server.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/speedups.c` & `websockets-9.1/src/websockets/speedups.c`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/streams.py` & `websockets-9.1/src/websockets/streams.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/typing.py` & `websockets-9.1/src/websockets/typing.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/uri.py` & `websockets-9.1/src/websockets/uri.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets/utils.py` & `websockets-9.1/src/websockets/utils.py`

 * *Files identical despite different names*

### Comparing `websockets-9.0.2/src/websockets.egg-info/PKG-INFO` & `websockets-9.1/src/websockets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: websockets
-Version: 9.0.2
+Version: 9.1
 Summary: An implementation of the WebSocket Protocol (RFC 6455 & 7692)
 Home-page: https://github.com/aaugustin/websockets
 Author: Aymeric Augustin
 Author-email: aymeric.augustin@m4x.org
 License: BSD
 Description: .. image:: logo/horizontal.svg
            :width: 480px
```

### Comparing `websockets-9.0.2/src/websockets.egg-info/SOURCES.txt` & `websockets-9.1/src/websockets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

