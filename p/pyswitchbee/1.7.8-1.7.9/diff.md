# Comparing `tmp/pyswitchbee-1.7.8.tar.gz` & `tmp/pyswitchbee-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyswitchbee-1.7.8.tar", last modified: Thu Dec 15 06:51:53 2022, max compression
+gzip compressed data, was "pyswitchbee-1.7.9.tar", last modified: Thu Dec 15 06:57:28 2022, max compression
```

## Comparing `pyswitchbee-1.7.8.tar` & `pyswitchbee-1.7.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:51:53.901073 pyswitchbee-1.7.8/
--rw-r--r--   0 jafaratili   (501) staff       (20)    11357 2022-12-10 07:08:50.000000 pyswitchbee-1.7.8/LICENSE
--rw-r--r--   0 jafaratili   (501) staff       (20)       30 2022-09-27 17:50:42.000000 pyswitchbee-1.7.8/MANIFEST.in
--rw-r--r--   0 jafaratili   (501) staff       (20)     4099 2022-12-15 06:51:53.899908 pyswitchbee-1.7.8/PKG-INFO
--rw-r--r--   0 jafaratili   (501) staff       (20)     3469 2022-08-12 09:23:45.000000 pyswitchbee-1.7.8/README.md
--rw-r--r--   0 jafaratili   (501) staff       (20)      740 2022-12-15 06:51:08.000000 pyswitchbee-1.7.8/pyproject.toml
--rw-r--r--   0 jafaratili   (501) staff       (20)       38 2022-12-15 06:51:53.901218 pyswitchbee-1.7.8/setup.cfg
-drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:51:53.781915 pyswitchbee-1.7.8/src/
-drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:51:53.842760 pyswitchbee-1.7.8/src/pyswitchbee.egg-info/
--rw-r--r--   0 jafaratili   (501) staff       (20)     4099 2022-12-15 06:51:53.000000 pyswitchbee-1.7.8/src/pyswitchbee.egg-info/PKG-INFO
--rw-r--r--   0 jafaratili   (501) staff       (20)      525 2022-12-15 06:51:53.000000 pyswitchbee-1.7.8/src/pyswitchbee.egg-info/SOURCES.txt
--rw-r--r--   0 jafaratili   (501) staff       (20)        1 2022-12-15 06:51:53.000000 pyswitchbee-1.7.8/src/pyswitchbee.egg-info/dependency_links.txt
--rw-r--r--   0 jafaratili   (501) staff       (20)        8 2022-12-15 06:51:53.000000 pyswitchbee-1.7.8/src/pyswitchbee.egg-info/requires.txt
--rw-r--r--   0 jafaratili   (501) staff       (20)       10 2022-12-15 06:51:53.000000 pyswitchbee-1.7.8/src/pyswitchbee.egg-info/top_level.txt
-drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:51:53.876082 pyswitchbee-1.7.8/src/switchbee/
--rw-r--r--   0 jafaratili   (501) staff       (20)      113 2022-12-10 09:05:16.000000 pyswitchbee-1.7.8/src/switchbee/__init__.py
-drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:51:53.885205 pyswitchbee-1.7.8/src/switchbee/api/
--rw-r--r--   0 jafaratili   (501) staff       (20)      271 2022-12-15 06:48:10.000000 pyswitchbee-1.7.8/src/switchbee/api/__init__.py
--rw-r--r--   0 jafaratili   (501) staff       (20)    16702 2022-12-15 06:46:37.000000 pyswitchbee-1.7.8/src/switchbee/api/central_unit.py
--rw-r--r--   0 jafaratili   (501) staff       (20)     3995 2022-12-10 21:47:47.000000 pyswitchbee-1.7.8/src/switchbee/api/polling.py
--rw-r--r--   0 jafaratili   (501) staff       (20)     7987 2022-12-15 06:50:35.000000 pyswitchbee-1.7.8/src/switchbee/api/wsrpc.py
-drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:51:53.892678 pyswitchbee-1.7.8/src/switchbee/central_unit/
--rw-r--r--   0 jafaratili   (501) staff       (20)     4127 2022-12-13 19:44:24.000000 pyswitchbee-1.7.8/src/switchbee/central_unit/__init__.py
--rw-r--r--   0 jafaratili   (501) staff       (20)     2451 2022-12-13 19:44:54.000000 pyswitchbee-1.7.8/src/switchbee/const.py
-drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:51:53.899204 pyswitchbee-1.7.8/src/switchbee/device/
--rw-r--r--   0 jafaratili   (501) staff       (20)     9280 2022-12-10 07:08:50.000000 pyswitchbee-1.7.8/src/switchbee/device/__init__.py
--rw-r--r--   0 jafaratili   (501) staff       (20)        0 2022-09-21 13:55:15.000000 pyswitchbee-1.7.8/src/switchbee/py.typed
--rw-r--r--   0 jafaratili   (501) staff       (20)      151 2022-12-10 07:08:50.000000 pyswitchbee-1.7.8/src/switchbee/utils.py
+drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:57:28.002612 pyswitchbee-1.7.9/
+-rw-r--r--   0 jafaratili   (501) staff       (20)    11357 2022-12-10 07:08:50.000000 pyswitchbee-1.7.9/LICENSE
+-rw-r--r--   0 jafaratili   (501) staff       (20)       30 2022-09-27 17:50:42.000000 pyswitchbee-1.7.9/MANIFEST.in
+-rw-r--r--   0 jafaratili   (501) staff       (20)     4099 2022-12-15 06:57:28.002310 pyswitchbee-1.7.9/PKG-INFO
+-rw-r--r--   0 jafaratili   (501) staff       (20)     3469 2022-08-12 09:23:45.000000 pyswitchbee-1.7.9/README.md
+-rw-r--r--   0 jafaratili   (501) staff       (20)      740 2022-12-15 06:57:05.000000 pyswitchbee-1.7.9/pyproject.toml
+-rw-r--r--   0 jafaratili   (501) staff       (20)       38 2022-12-15 06:57:28.002702 pyswitchbee-1.7.9/setup.cfg
+drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:57:27.957167 pyswitchbee-1.7.9/src/
+drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:57:27.987794 pyswitchbee-1.7.9/src/pyswitchbee.egg-info/
+-rw-r--r--   0 jafaratili   (501) staff       (20)     4099 2022-12-15 06:57:27.000000 pyswitchbee-1.7.9/src/pyswitchbee.egg-info/PKG-INFO
+-rw-r--r--   0 jafaratili   (501) staff       (20)      525 2022-12-15 06:57:27.000000 pyswitchbee-1.7.9/src/pyswitchbee.egg-info/SOURCES.txt
+-rw-r--r--   0 jafaratili   (501) staff       (20)        1 2022-12-15 06:57:27.000000 pyswitchbee-1.7.9/src/pyswitchbee.egg-info/dependency_links.txt
+-rw-r--r--   0 jafaratili   (501) staff       (20)        8 2022-12-15 06:57:27.000000 pyswitchbee-1.7.9/src/pyswitchbee.egg-info/requires.txt
+-rw-r--r--   0 jafaratili   (501) staff       (20)       10 2022-12-15 06:57:27.000000 pyswitchbee-1.7.9/src/pyswitchbee.egg-info/top_level.txt
+drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:57:27.993079 pyswitchbee-1.7.9/src/switchbee/
+-rw-r--r--   0 jafaratili   (501) staff       (20)      113 2022-12-10 09:05:16.000000 pyswitchbee-1.7.9/src/switchbee/__init__.py
+drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:57:27.998854 pyswitchbee-1.7.9/src/switchbee/api/
+-rw-r--r--   0 jafaratili   (501) staff       (20)      271 2022-12-15 06:48:10.000000 pyswitchbee-1.7.9/src/switchbee/api/__init__.py
+-rw-r--r--   0 jafaratili   (501) staff       (20)    16585 2022-12-15 06:56:39.000000 pyswitchbee-1.7.9/src/switchbee/api/central_unit.py
+-rw-r--r--   0 jafaratili   (501) staff       (20)     3995 2022-12-10 21:47:47.000000 pyswitchbee-1.7.9/src/switchbee/api/polling.py
+-rw-r--r--   0 jafaratili   (501) staff       (20)     7987 2022-12-15 06:50:35.000000 pyswitchbee-1.7.9/src/switchbee/api/wsrpc.py
+drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:57:28.000190 pyswitchbee-1.7.9/src/switchbee/central_unit/
+-rw-r--r--   0 jafaratili   (501) staff       (20)     4127 2022-12-13 19:44:24.000000 pyswitchbee-1.7.9/src/switchbee/central_unit/__init__.py
+-rw-r--r--   0 jafaratili   (501) staff       (20)     2451 2022-12-13 19:44:54.000000 pyswitchbee-1.7.9/src/switchbee/const.py
+drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:57:28.001642 pyswitchbee-1.7.9/src/switchbee/device/
+-rw-r--r--   0 jafaratili   (501) staff       (20)     9280 2022-12-10 07:08:50.000000 pyswitchbee-1.7.9/src/switchbee/device/__init__.py
+-rw-r--r--   0 jafaratili   (501) staff       (20)        0 2022-09-21 13:55:15.000000 pyswitchbee-1.7.9/src/switchbee/py.typed
+-rw-r--r--   0 jafaratili   (501) staff       (20)      151 2022-12-10 07:08:50.000000 pyswitchbee-1.7.9/src/switchbee/utils.py
```

### Comparing `pyswitchbee-1.7.8/LICENSE` & `pyswitchbee-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswitchbee-1.7.8/PKG-INFO` & `pyswitchbee-1.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswitchbee
-Version: 1.7.8
+Version: 1.7.9
 Summary: SwitchBee Python Integration.
 Author-email: Jafar Atili <at.jafar@outlook.com>
 Project-URL: homepage, https://pypi.org/project/pyswitchbee/
 Project-URL: repository, https://github.com/jafar-atili/pySwitchbee/
 Keywords: home,automation,switchbee,smart
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pyswitchbee-1.7.8/README.md` & `pyswitchbee-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `pyswitchbee-1.7.8/pyproject.toml` & `pyswitchbee-1.7.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyswitchbee"
-version = "1.7.8"
+version = "1.7.9"
 description = "SwitchBee Python Integration."
 readme = "README.md"
 authors = [{ name = "Jafar Atili", email = "at.jafar@outlook.com" }]
 keywords = [ "home", "automation", "switchbee", "smart" ]
 classifiers = [
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
```

### Comparing `pyswitchbee-1.7.8/src/pyswitchbee.egg-info/PKG-INFO` & `pyswitchbee-1.7.9/src/pyswitchbee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswitchbee
-Version: 1.7.8
+Version: 1.7.9
 Summary: SwitchBee Python Integration.
 Author-email: Jafar Atili <at.jafar@outlook.com>
 Project-URL: homepage, https://pypi.org/project/pyswitchbee/
 Project-URL: repository, https://github.com/jafar-atili/pySwitchbee/
 Keywords: home,automation,switchbee,smart
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pyswitchbee-1.7.8/src/pyswitchbee.egg-info/SOURCES.txt` & `pyswitchbee-1.7.9/src/pyswitchbee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyswitchbee-1.7.8/src/switchbee/api/central_unit.py` & `pyswitchbee-1.7.9/src/switchbee/api/central_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,24 +433,22 @@
 
         if device_id not in self._devices_map:
             logger.debug("Device id %d is not tracked", device_id)
             return
 
         device = self._devices_map[device_id]
 
+        # temp workaround
+        if isinstance(state, float):
+            state = int(state)
+
         if isinstance(device, SwitchBeeDimmer):
-            # temp workaround
-            if isinstance(state, float):
-                state = int(state)
             assert isinstance(state, (str, int))
             device.brightness = state  # type: ignore
         elif isinstance(device, SwitchBeeShutter):
-            # temp workaround
-            if isinstance(state, float):
-                state = int(state)
             assert isinstance(state, (str, int))
             device.position = state  # type: ignore
         elif isinstance(
             device,
             (
                 SwitchBeeSwitch,
                 SwitchBeeGroupSwitch,
```

### Comparing `pyswitchbee-1.7.8/src/switchbee/api/polling.py` & `pyswitchbee-1.7.9/src/switchbee/api/polling.py`

 * *Files identical despite different names*

### Comparing `pyswitchbee-1.7.8/src/switchbee/api/wsrpc.py` & `pyswitchbee-1.7.9/src/switchbee/api/wsrpc.py`

 * *Files identical despite different names*

### Comparing `pyswitchbee-1.7.8/src/switchbee/central_unit/__init__.py` & `pyswitchbee-1.7.9/src/switchbee/central_unit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswitchbee-1.7.8/src/switchbee/const.py` & `pyswitchbee-1.7.9/src/switchbee/const.py`

 * *Files identical despite different names*

### Comparing `pyswitchbee-1.7.8/src/switchbee/device/__init__.py` & `pyswitchbee-1.7.9/src/switchbee/device/__init__.py`

 * *Files identical despite different names*

