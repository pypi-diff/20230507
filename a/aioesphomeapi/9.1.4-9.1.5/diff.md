# Comparing `tmp/aioesphomeapi-9.1.4.tar.gz` & `tmp/aioesphomeapi-9.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioesphomeapi-9.1.4.tar", last modified: Mon Oct  4 10:34:20 2021, max compression
+gzip compressed data, was "aioesphomeapi-9.1.5.tar", last modified: Tue Oct  5 08:57:45 2021, max compression
```

## Comparing `aioesphomeapi-9.1.4.tar` & `aioesphomeapi-9.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 10:34:20.568634 aioesphomeapi-9.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-10-04 10:34:03.000000 aioesphomeapi-9.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       72 2021-10-04 10:34:03.000000 aioesphomeapi-9.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3696 2021-10-04 10:34:20.568634 aioesphomeapi-9.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3343 2021-10-04 10:34:03.000000 aioesphomeapi-9.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 10:34:20.568634 aioesphomeapi-9.1.4/aioesphomeapi/
--rw-r--r--   0 runner    (1001) docker     (121)      416 2021-10-04 10:34:03.000000 aioesphomeapi-9.1.4/aioesphomeapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6831 2021-10-04 10:34:03.000000 aioesphomeapi-9.1.4/aioesphomeapi/api_options_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)   216246 2021-10-04 10:34:03.000000 aioesphomeapi-9.1.4/aioesphomeapi/api_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    22062 2021-10-04 10:34:03.000000 aioesphomeapi-9.1.4/aioesphomeapi/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    26752 2021-10-04 10:34:03.000000 aioesphomeapi-9.1.4/aioesphomeapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     4080 2021-10-04 10:34:03.000000 aioesphomeapi-9.1.4/aioesphomeapi/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     8086 2021-10-04 10:34:03.000000 aioesphomeapi-9.1.4/aioesphomeapi/host_resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)     2342 2021-10-04 10:34:03.000000 aioesphomeapi-9.1.4/aioesphomeapi/log_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)    17604 2021-10-04 10:34:03.000000 aioesphomeapi-9.1.4/aioesphomeapi/model.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-04 10:34:03.000000 aioesphomeapi-9.1.4/aioesphomeapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    10563 2021-10-04 10:34:03.000000 aioesphomeapi-9.1.4/aioesphomeapi/reconnect_logic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2021-10-04 10:34:03.000000 aioesphomeapi-9.1.4/aioesphomeapi/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-04 10:34:20.568634 aioesphomeapi-9.1.4/aioesphomeapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3696 2021-10-04 10:34:20.000000 aioesphomeapi-9.1.4/aioesphomeapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      619 2021-10-04 10:34:20.000000 aioesphomeapi-9.1.4/aioesphomeapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-04 10:34:20.000000 aioesphomeapi-9.1.4/aioesphomeapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-04 10:34:10.000000 aioesphomeapi-9.1.4/aioesphomeapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-10-04 10:34:20.000000 aioesphomeapi-9.1.4/aioesphomeapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-10-04 10:34:20.000000 aioesphomeapi-9.1.4/aioesphomeapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      617 2021-10-04 10:34:03.000000 aioesphomeapi-9.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-10-04 10:34:03.000000 aioesphomeapi-9.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      178 2021-10-04 10:34:20.568634 aioesphomeapi-9.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1534 2021-10-04 10:34:03.000000 aioesphomeapi-9.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 08:57:45.514539 aioesphomeapi-9.1.5/
+-rw-r--r--   0 runner    (1001) docker     (121)     1067 2021-10-05 08:57:25.000000 aioesphomeapi-9.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2021-10-05 08:57:25.000000 aioesphomeapi-9.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3696 2021-10-05 08:57:45.514539 aioesphomeapi-9.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3343 2021-10-05 08:57:25.000000 aioesphomeapi-9.1.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 08:57:45.514539 aioesphomeapi-9.1.5/aioesphomeapi/
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2021-10-05 08:57:25.000000 aioesphomeapi-9.1.5/aioesphomeapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6831 2021-10-05 08:57:25.000000 aioesphomeapi-9.1.5/aioesphomeapi/api_options_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)   216246 2021-10-05 08:57:25.000000 aioesphomeapi-9.1.5/aioesphomeapi/api_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22062 2021-10-05 08:57:25.000000 aioesphomeapi-9.1.5/aioesphomeapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26784 2021-10-05 08:57:25.000000 aioesphomeapi-9.1.5/aioesphomeapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4080 2021-10-05 08:57:25.000000 aioesphomeapi-9.1.5/aioesphomeapi/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8086 2021-10-05 08:57:25.000000 aioesphomeapi-9.1.5/aioesphomeapi/host_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2342 2021-10-05 08:57:25.000000 aioesphomeapi-9.1.5/aioesphomeapi/log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17604 2021-10-05 08:57:25.000000 aioesphomeapi-9.1.5/aioesphomeapi/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-05 08:57:25.000000 aioesphomeapi-9.1.5/aioesphomeapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    10563 2021-10-05 08:57:25.000000 aioesphomeapi-9.1.5/aioesphomeapi/reconnect_logic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1494 2021-10-05 08:57:25.000000 aioesphomeapi-9.1.5/aioesphomeapi/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 08:57:45.514539 aioesphomeapi-9.1.5/aioesphomeapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3696 2021-10-05 08:57:45.000000 aioesphomeapi-9.1.5/aioesphomeapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2021-10-05 08:57:45.000000 aioesphomeapi-9.1.5/aioesphomeapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-05 08:57:45.000000 aioesphomeapi-9.1.5/aioesphomeapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-05 08:57:35.000000 aioesphomeapi-9.1.5/aioesphomeapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2021-10-05 08:57:45.000000 aioesphomeapi-9.1.5/aioesphomeapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2021-10-05 08:57:45.000000 aioesphomeapi-9.1.5/aioesphomeapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2021-10-05 08:57:25.000000 aioesphomeapi-9.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-10-05 08:57:25.000000 aioesphomeapi-9.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2021-10-05 08:57:45.514539 aioesphomeapi-9.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1534 2021-10-05 08:57:25.000000 aioesphomeapi-9.1.5/setup.py
```

### Comparing `aioesphomeapi-9.1.4/LICENSE` & `aioesphomeapi-9.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aioesphomeapi-9.1.4/PKG-INFO` & `aioesphomeapi-9.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: aioesphomeapi
-Version: 9.1.4
+Version: 9.1.5
 Summary: Python API for interacting with ESPHome devices.
 Home-page: https://esphome.io/
 Author: Otto Winter
 Author-email: esphome@nabucasa.com
 License: MIT
-Download-URL: https://github.com/esphome/aioesphomeapi/archive/9.1.4.zip
+Download-URL: https://github.com/esphome/aioesphomeapi/archive/9.1.5.zip
 Platform: UNKNOWN
 Requires-Python: >=3.7
 License-File: LICENSE
 
 aioesphomeapi
 =============
```

### Comparing `aioesphomeapi-9.1.4/README.rst` & `aioesphomeapi-9.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `aioesphomeapi-9.1.4/aioesphomeapi/api_options_pb2.py` & `aioesphomeapi-9.1.5/aioesphomeapi/api_options_pb2.py`

 * *Files identical despite different names*

### Comparing `aioesphomeapi-9.1.4/aioesphomeapi/api_pb2.py` & `aioesphomeapi-9.1.5/aioesphomeapi/api_pb2.py`

 * *Files identical despite different names*

### Comparing `aioesphomeapi-9.1.4/aioesphomeapi/client.py` & `aioesphomeapi-9.1.5/aioesphomeapi/client.py`

 * *Files identical despite different names*

### Comparing `aioesphomeapi-9.1.4/aioesphomeapi/connection.py` & `aioesphomeapi-9.1.5/aioesphomeapi/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -580,17 +580,18 @@
             if do_append(resp):
                 responses.append(resp)
             if do_stop(resp):
                 fut.set_result(responses)
 
         def on_read_exception(exc: Exception) -> None:
             if not fut.done():
-                # Wrap error so that caller gets right stacktrace
-                new_exc = ReadFailedAPIError("Read failed")
-                new_exc.__cause__ = exc
+                new_exc = exc
+                if not isinstance(exc, APIConnectionError):
+                    new_exc = ReadFailedAPIError("Read failed")
+                    new_exc.__cause__ = exc
                 fut.set_exception(new_exc)
 
         self._message_handlers.append(on_message)
         self._read_exception_handlers.append(on_read_exception)
         await self.send_message(send_msg)
 
         try:
```

### Comparing `aioesphomeapi-9.1.4/aioesphomeapi/core.py` & `aioesphomeapi-9.1.5/aioesphomeapi/core.py`

 * *Files identical despite different names*

### Comparing `aioesphomeapi-9.1.4/aioesphomeapi/host_resolver.py` & `aioesphomeapi-9.1.5/aioesphomeapi/host_resolver.py`

 * *Files identical despite different names*

### Comparing `aioesphomeapi-9.1.4/aioesphomeapi/log_reader.py` & `aioesphomeapi-9.1.5/aioesphomeapi/log_reader.py`

 * *Files identical despite different names*

### Comparing `aioesphomeapi-9.1.4/aioesphomeapi/model.py` & `aioesphomeapi-9.1.5/aioesphomeapi/model.py`

 * *Files identical despite different names*

### Comparing `aioesphomeapi-9.1.4/aioesphomeapi/reconnect_logic.py` & `aioesphomeapi-9.1.5/aioesphomeapi/reconnect_logic.py`

 * *Files identical despite different names*

### Comparing `aioesphomeapi-9.1.4/aioesphomeapi/util.py` & `aioesphomeapi-9.1.5/aioesphomeapi/util.py`

 * *Files identical despite different names*

### Comparing `aioesphomeapi-9.1.4/aioesphomeapi.egg-info/PKG-INFO` & `aioesphomeapi-9.1.5/aioesphomeapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: aioesphomeapi
-Version: 9.1.4
+Version: 9.1.5
 Summary: Python API for interacting with ESPHome devices.
 Home-page: https://esphome.io/
 Author: Otto Winter
 Author-email: esphome@nabucasa.com
 License: MIT
-Download-URL: https://github.com/esphome/aioesphomeapi/archive/9.1.4.zip
+Download-URL: https://github.com/esphome/aioesphomeapi/archive/9.1.5.zip
 Platform: UNKNOWN
 Requires-Python: >=3.7
 License-File: LICENSE
 
 aioesphomeapi
 =============
```

### Comparing `aioesphomeapi-9.1.4/aioesphomeapi.egg-info/SOURCES.txt` & `aioesphomeapi-9.1.5/aioesphomeapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioesphomeapi-9.1.4/pyproject.toml` & `aioesphomeapi-9.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aioesphomeapi-9.1.4/setup.py` & `aioesphomeapi-9.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "README.rst"), encoding="utf-8") as readme_file:
     long_description = readme_file.read()
 
 
-VERSION = "9.1.4"
+VERSION = "9.1.5"
 PROJECT_NAME = "aioesphomeapi"
 PROJECT_PACKAGE_NAME = "aioesphomeapi"
 PROJECT_LICENSE = "MIT"
 PROJECT_AUTHOR = "Otto Winter"
 PROJECT_COPYRIGHT = " 2019-2020, Otto Winter"
 PROJECT_URL = "https://esphome.io/"
 PROJECT_EMAIL = "esphome@nabucasa.com"
```

