# Comparing `tmp/pynukibt-0.0.4.tar.gz` & `tmp/pynukibt-0.0.5.tar.gz`

## Comparing `pynukibt-0.0.4.tar` & `pynukibt-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pynukibt-0.0.4/requirements.txt
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pynukibt-0.0.4/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pynukibt-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pynukibt-0.0.4/pyNukiBT/__init__.py
--rw-r--r--   0        0        0    39005 2020-02-02 00:00:00.000000 pynukibt-0.0.4/pyNukiBT/const.py
--rw-r--r--   0        0        0    24728 2020-02-02 00:00:00.000000 pynukibt-0.0.4/pyNukiBT/nuki.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pynukibt-0.0.4/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pynukibt-0.0.4/LICENSE
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 pynukibt-0.0.4/README.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 pynukibt-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 pynukibt-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pynukibt-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pynukibt-0.0.5/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pynukibt-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pynukibt-0.0.5/pyNukiBT/__init__.py
+-rw-r--r--   0        0        0    39005 2020-02-02 00:00:00.000000 pynukibt-0.0.5/pyNukiBT/const.py
+-rw-r--r--   0        0        0    24709 2020-02-02 00:00:00.000000 pynukibt-0.0.5/pyNukiBT/nuki.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pynukibt-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pynukibt-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 pynukibt-0.0.5/README.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 pynukibt-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 pynukibt-0.0.5/PKG-INFO
```

### Comparing `pynukibt-0.0.4/setup.py` & `pynukibt-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyNukiBT",
-    version="0.0.4",
+    version="0.0.5",
     author="Ronen Gruengras",
     author_email="ronengr@gmail.com",
     description="Nuki Bluetooth API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ronengr/pyNukiBT",
     packages=find_packages(),
```

### Comparing `pynukibt-0.0.4/.github/workflows/python-publish.yml` & `pynukibt-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pynukibt-0.0.4/pyNukiBT/const.py` & `pynukibt-0.0.5/pyNukiBT/const.py`

 * *Files identical despite different names*

### Comparing `pynukibt-0.0.4/pyNukiBT/nuki.py` & `pynukibt-0.0.5/pyNukiBT/nuki.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,17 +54,16 @@
         self._device_type = None
 
         self._pairing_handle = None
         self._client = None
         self._expected_response: NukiConst.NukiCommand = None
         self._aggregate_messages = list(),
         self.retry = 5
-        self.connection_timeout = 30
-        self.command_timeout = 30
-        self.command_response_timeout = 10
+        self.connection_timeout = 40
+        self.command_response_timeout = 20
 
         self._send_cmd_lock = asyncio.Lock()
         self._connect_lock = asyncio.Lock()
         self._operation_lock = asyncio.Lock()
         self._update_state_lock = asyncio.Lock()
         self._update_config_lock = asyncio.Lock()
         self._notify_future = None
@@ -334,15 +333,15 @@
             for i in range(1, self.retry + 1):
                 logger.info(f"Trying to send data. Attempt {i}")
                 try:
                     await self.connect()
                     if _characteristic is None:
                         _characteristic = self._const.BLE_CHAR
                     logger.info(f"Sending data to Nuki")
-                    await self._client.write_gatt_char(_characteristic, command)
+                    await self._client.write_gatt_char(_characteristic, command, response=True)
                 except (TimeoutError, CancelledError):
                     logger.error(f"Timeout while sending data on attempt {i}")
                     await asyncio.sleep(0.2)
                 except BleakDBusError as ex:
                     logger.error(f"DBus Error {ex}")
                     await asyncio.sleep(0.2)
                 # except BLEAK_RETRY_EXCEPTIONS as ex:
```

### Comparing `pynukibt-0.0.4/.gitignore` & `pynukibt-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pynukibt-0.0.4/LICENSE` & `pynukibt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pynukibt-0.0.4/README.md` & `pynukibt-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pynukibt-0.0.4/pyproject.toml` & `pynukibt-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyNukiBT"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Ronen Gruengras", email="ronengr@gmail.com" },
 ]
 description = "Nuki Bluetooth API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pynukibt-0.0.4/PKG-INFO` & `pynukibt-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNukiBT
-Version: 0.0.4
+Version: 0.0.5
 Summary: Nuki Bluetooth API
 Project-URL: Homepage, https://github.com/ronengr/pyNukiBT
 Project-URL: Bug Tracker, https://github.com/ronengr/pyNukiBT/issues
 Author-email: Ronen Gruengras <ronengr@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

