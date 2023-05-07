# Comparing `tmp/pyswitchbee-1.7.9.tar.gz` & `tmp/pyswitchbee-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyswitchbee-1.7.9.tar", last modified: Thu Dec 15 06:57:28 2022, max compression
+gzip compressed data, was "pyswitchbee-1.8.0.tar", last modified: Sun May  7 10:45:51 2023, max compression
```

## Comparing `pyswitchbee-1.7.9.tar` & `pyswitchbee-1.8.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:57:28.002612 pyswitchbee-1.7.9/
--rw-r--r--   0 jafaratili   (501) staff       (20)    11357 2022-12-10 07:08:50.000000 pyswitchbee-1.7.9/LICENSE
--rw-r--r--   0 jafaratili   (501) staff       (20)       30 2022-09-27 17:50:42.000000 pyswitchbee-1.7.9/MANIFEST.in
--rw-r--r--   0 jafaratili   (501) staff       (20)     4099 2022-12-15 06:57:28.002310 pyswitchbee-1.7.9/PKG-INFO
--rw-r--r--   0 jafaratili   (501) staff       (20)     3469 2022-08-12 09:23:45.000000 pyswitchbee-1.7.9/README.md
--rw-r--r--   0 jafaratili   (501) staff       (20)      740 2022-12-15 06:57:05.000000 pyswitchbee-1.7.9/pyproject.toml
--rw-r--r--   0 jafaratili   (501) staff       (20)       38 2022-12-15 06:57:28.002702 pyswitchbee-1.7.9/setup.cfg
-drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:57:27.957167 pyswitchbee-1.7.9/src/
-drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:57:27.987794 pyswitchbee-1.7.9/src/pyswitchbee.egg-info/
--rw-r--r--   0 jafaratili   (501) staff       (20)     4099 2022-12-15 06:57:27.000000 pyswitchbee-1.7.9/src/pyswitchbee.egg-info/PKG-INFO
--rw-r--r--   0 jafaratili   (501) staff       (20)      525 2022-12-15 06:57:27.000000 pyswitchbee-1.7.9/src/pyswitchbee.egg-info/SOURCES.txt
--rw-r--r--   0 jafaratili   (501) staff       (20)        1 2022-12-15 06:57:27.000000 pyswitchbee-1.7.9/src/pyswitchbee.egg-info/dependency_links.txt
--rw-r--r--   0 jafaratili   (501) staff       (20)        8 2022-12-15 06:57:27.000000 pyswitchbee-1.7.9/src/pyswitchbee.egg-info/requires.txt
--rw-r--r--   0 jafaratili   (501) staff       (20)       10 2022-12-15 06:57:27.000000 pyswitchbee-1.7.9/src/pyswitchbee.egg-info/top_level.txt
-drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:57:27.993079 pyswitchbee-1.7.9/src/switchbee/
--rw-r--r--   0 jafaratili   (501) staff       (20)      113 2022-12-10 09:05:16.000000 pyswitchbee-1.7.9/src/switchbee/__init__.py
-drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:57:27.998854 pyswitchbee-1.7.9/src/switchbee/api/
--rw-r--r--   0 jafaratili   (501) staff       (20)      271 2022-12-15 06:48:10.000000 pyswitchbee-1.7.9/src/switchbee/api/__init__.py
--rw-r--r--   0 jafaratili   (501) staff       (20)    16585 2022-12-15 06:56:39.000000 pyswitchbee-1.7.9/src/switchbee/api/central_unit.py
--rw-r--r--   0 jafaratili   (501) staff       (20)     3995 2022-12-10 21:47:47.000000 pyswitchbee-1.7.9/src/switchbee/api/polling.py
--rw-r--r--   0 jafaratili   (501) staff       (20)     7987 2022-12-15 06:50:35.000000 pyswitchbee-1.7.9/src/switchbee/api/wsrpc.py
-drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:57:28.000190 pyswitchbee-1.7.9/src/switchbee/central_unit/
--rw-r--r--   0 jafaratili   (501) staff       (20)     4127 2022-12-13 19:44:24.000000 pyswitchbee-1.7.9/src/switchbee/central_unit/__init__.py
--rw-r--r--   0 jafaratili   (501) staff       (20)     2451 2022-12-13 19:44:54.000000 pyswitchbee-1.7.9/src/switchbee/const.py
-drwxr-xr-x   0 jafaratili   (501) staff       (20)        0 2022-12-15 06:57:28.001642 pyswitchbee-1.7.9/src/switchbee/device/
--rw-r--r--   0 jafaratili   (501) staff       (20)     9280 2022-12-10 07:08:50.000000 pyswitchbee-1.7.9/src/switchbee/device/__init__.py
--rw-r--r--   0 jafaratili   (501) staff       (20)        0 2022-09-21 13:55:15.000000 pyswitchbee-1.7.9/src/switchbee/py.typed
--rw-r--r--   0 jafaratili   (501) staff       (20)      151 2022-12-10 07:08:50.000000 pyswitchbee-1.7.9/src/switchbee/utils.py
+drwxr-xr-x   0 jafar.atili   (502) staff       (20)        0 2023-05-07 10:45:51.938149 pyswitchbee-1.8.0/
+-rw-r--r--   0 jafar.atili   (502) staff       (20)    11357 2023-05-04 14:52:10.000000 pyswitchbee-1.8.0/LICENSE
+-rw-r--r--   0 jafar.atili   (502) staff       (20)       30 2023-05-04 14:52:10.000000 pyswitchbee-1.8.0/MANIFEST.in
+-rw-r--r--   0 jafar.atili   (502) staff       (20)     4099 2023-05-07 10:45:51.937982 pyswitchbee-1.8.0/PKG-INFO
+-rw-r--r--   0 jafar.atili   (502) staff       (20)     3469 2023-05-04 14:52:10.000000 pyswitchbee-1.8.0/README.md
+-rw-r--r--   0 jafar.atili   (502) staff       (20)      757 2023-05-07 10:45:27.000000 pyswitchbee-1.8.0/pyproject.toml
+-rw-r--r--   0 jafar.atili   (502) staff       (20)       38 2023-05-07 10:45:51.938195 pyswitchbee-1.8.0/setup.cfg
+drwxr-xr-x   0 jafar.atili   (502) staff       (20)        0 2023-05-07 10:45:51.933179 pyswitchbee-1.8.0/src/
+drwxr-xr-x   0 jafar.atili   (502) staff       (20)        0 2023-05-07 10:45:51.935288 pyswitchbee-1.8.0/src/pyswitchbee.egg-info/
+-rw-r--r--   0 jafar.atili   (502) staff       (20)     4099 2023-05-07 10:45:51.000000 pyswitchbee-1.8.0/src/pyswitchbee.egg-info/PKG-INFO
+-rw-r--r--   0 jafar.atili   (502) staff       (20)      525 2023-05-07 10:45:51.000000 pyswitchbee-1.8.0/src/pyswitchbee.egg-info/SOURCES.txt
+-rw-r--r--   0 jafar.atili   (502) staff       (20)        1 2023-05-07 10:45:51.000000 pyswitchbee-1.8.0/src/pyswitchbee.egg-info/dependency_links.txt
+-rw-r--r--   0 jafar.atili   (502) staff       (20)       23 2023-05-07 10:45:51.000000 pyswitchbee-1.8.0/src/pyswitchbee.egg-info/requires.txt
+-rw-r--r--   0 jafar.atili   (502) staff       (20)       10 2023-05-07 10:45:51.000000 pyswitchbee-1.8.0/src/pyswitchbee.egg-info/top_level.txt
+drwxr-xr-x   0 jafar.atili   (502) staff       (20)        0 2023-05-07 10:45:51.936375 pyswitchbee-1.8.0/src/switchbee/
+-rw-r--r--   0 jafar.atili   (502) staff       (20)      100 2023-05-04 14:52:10.000000 pyswitchbee-1.8.0/src/switchbee/__init__.py
+drwxr-xr-x   0 jafar.atili   (502) staff       (20)        0 2023-05-07 10:45:51.937260 pyswitchbee-1.8.0/src/switchbee/api/
+-rw-r--r--   0 jafar.atili   (502) staff       (20)      629 2023-05-04 14:52:10.000000 pyswitchbee-1.8.0/src/switchbee/api/__init__.py
+-rw-r--r--   0 jafar.atili   (502) staff       (20)    18133 2023-05-07 10:45:13.000000 pyswitchbee-1.8.0/src/switchbee/api/central_unit.py
+-rw-r--r--   0 jafar.atili   (502) staff       (20)     3995 2023-05-04 14:52:10.000000 pyswitchbee-1.8.0/src/switchbee/api/polling.py
+-rw-r--r--   0 jafar.atili   (502) staff       (20)     8145 2023-05-04 14:52:10.000000 pyswitchbee-1.8.0/src/switchbee/api/wsrpc.py
+drwxr-xr-x   0 jafar.atili   (502) staff       (20)        0 2023-05-07 10:45:51.937474 pyswitchbee-1.8.0/src/switchbee/central_unit/
+-rw-r--r--   0 jafar.atili   (502) staff       (20)     4127 2023-05-05 11:00:15.000000 pyswitchbee-1.8.0/src/switchbee/central_unit/__init__.py
+-rw-r--r--   0 jafar.atili   (502) staff       (20)     2520 2023-05-05 10:31:42.000000 pyswitchbee-1.8.0/src/switchbee/const.py
+drwxr-xr-x   0 jafar.atili   (502) staff       (20)        0 2023-05-07 10:45:51.937757 pyswitchbee-1.8.0/src/switchbee/device/
+-rw-r--r--   0 jafar.atili   (502) staff       (20)     9893 2023-05-07 10:16:36.000000 pyswitchbee-1.8.0/src/switchbee/device/__init__.py
+-rw-r--r--   0 jafar.atili   (502) staff       (20)        0 2023-05-04 14:52:10.000000 pyswitchbee-1.8.0/src/switchbee/py.typed
+-rw-r--r--   0 jafar.atili   (502) staff       (20)      151 2023-05-04 14:52:10.000000 pyswitchbee-1.8.0/src/switchbee/utils.py
```

### Comparing `pyswitchbee-1.7.9/LICENSE` & `pyswitchbee-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyswitchbee-1.7.9/PKG-INFO` & `pyswitchbee-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswitchbee
-Version: 1.7.9
+Version: 1.8.0
 Summary: SwitchBee Python Integration.
 Author-email: Jafar Atili <at.jafar@outlook.com>
 Project-URL: homepage, https://pypi.org/project/pyswitchbee/
 Project-URL: repository, https://github.com/jafar-atili/pySwitchbee/
 Keywords: home,automation,switchbee,smart
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pyswitchbee-1.7.9/README.md` & `pyswitchbee-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pyswitchbee-1.7.9/pyproject.toml` & `pyswitchbee-1.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyswitchbee"
-version = "1.7.9"
+version = "1.8.0"
 description = "SwitchBee Python Integration."
 readme = "README.md"
 authors = [{ name = "Jafar Atili", email = "at.jafar@outlook.com" }]
 keywords = [ "home", "automation", "switchbee", "smart" ]
 classifiers = [
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Home Automation",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Typing :: Typed"
 ]
-dependencies = [ "aiohttp" ]
+dependencies = [ "aiohttp", "awesomeversion"]
 requires-python = ">=3.9"
 
 [project.urls]
 homepage = "https://pypi.org/project/pyswitchbee/"
 repository = "https://github.com/jafar-atili/pySwitchbee/"
```

### Comparing `pyswitchbee-1.7.9/src/pyswitchbee.egg-info/PKG-INFO` & `pyswitchbee-1.8.0/src/pyswitchbee.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswitchbee
-Version: 1.7.9
+Version: 1.8.0
 Summary: SwitchBee Python Integration.
 Author-email: Jafar Atili <at.jafar@outlook.com>
 Project-URL: homepage, https://pypi.org/project/pyswitchbee/
 Project-URL: repository, https://github.com/jafar-atili/pySwitchbee/
 Keywords: home,automation,switchbee,smart
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pyswitchbee-1.7.9/src/pyswitchbee.egg-info/SOURCES.txt` & `pyswitchbee-1.8.0/src/pyswitchbee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyswitchbee-1.7.9/src/switchbee/api/central_unit.py` & `pyswitchbee-1.8.0/src/switchbee/api/central_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import re
 from datetime import timedelta
 from logging import getLogger
 from typing import Any, List
 from abc import ABC, abstractmethod
 
 from aiohttp import ClientSession
 from switchbee.const import ApiAttribute, ApiCommand, ApiStatus
@@ -50,29 +51,50 @@
     DeviceType.Shutter,
     DeviceType.TimedPowerSwitch,
     DeviceType.Thermostat,
     DeviceType.TimedSwitch,
 ]
 
 
+class CUVersion:
+    def __init__(self, version: str) -> None:
+        self.major: int | str = 0
+        self.minor: int = 0
+        self.revision: int = 0
+        self.build: int = 0
+
+        self._initialize(version)
+
+    def _initialize(self, version: str) -> None:
+        if match := re.match(r"(\d+|\S)\.(\d+)\.(\d+)\((\d+)\)$", version):
+            self.major = match.group(1)
+            self.minor = int(match.group(2))
+            self.revision = int(match.group(3))
+            self.build = int(match.group(4))
+
+    def __repr__(self) -> str:
+        return f"{self.major}.{self.minor}.{self.revision}.{self.build}"
+
+
 class CentralUnitAPI(ABC):
     _login_count: int = -1  # we don't count the first login
     _token: str | None = None
     _token_expiration: int = 0
 
     def __init__(
         self, ip_address: str, user: str, password: str, aiohttp_session: ClientSession
     ) -> None:
         self._ip_address: str = ip_address
         self._username: str = user
         self._password: str = password
         self._aiohttp_session: ClientSession = aiohttp_session
 
         self._mac: str | None = None
-        self._version: str | None = None
+        self._unique_id: str | None = None
+        self._version: CUVersion | None = None
         self._name: str | None = None
         self._last_conf_change: int = 0
         self._devices_map: dict[
             int,
             SwitchBeeSwitch
             | SwitchBeeGroupSwitch
             | SwitchBeeTimedSwitch
@@ -89,22 +111,26 @@
         self._modules_map: dict[int, set] = {}
 
     @property
     def name(self) -> str | None:
         return self._name
 
     @property
-    def version(self) -> str | None:
+    def version(self) -> CUVersion | None:
         return self._version
 
     @property
     def mac(self) -> str | None:
         return self._mac
 
     @property
+    def unique_id(self) -> str | None:
+        return self._unique_id
+
+    @property
     def devices(
         self,
     ) -> dict[
         int,
         SwitchBeeSwitch
         | SwitchBeeGroupSwitch
         | SwitchBeeTimedSwitch
@@ -162,29 +188,30 @@
         raise NotImplementedError
 
     @abstractmethod
     async def _login(self) -> None:
         raise NotImplementedError
 
     def _update_login(self, resp: dict[str, Any]) -> None:
-
         self._login_count += 1
         self._token = resp[ApiAttribute.DATA][ApiAttribute.TOKEN]
         # instead of dealing with time synchronization issue, we
         # calculate one hour from now and set it to be the expiration time of the token
         # self._token_expiration = resp[ApiAttribute.DATA][ApiAttribute.EXPIRATION]
         self._token_expiration = timestamp_now() + TOKEN_EXPIRATION
 
     async def get_configuration(self) -> dict:
         await self.login_if_needed()
         return await self._send_request(ApiCommand.GET_CONF)
 
     async def get_multiple_states(self, ids: list) -> dict:
         """returns JSON {'status': 'OK', 'data': [{'id': 212, 'state': 'OFF'}, {'id': 343, 'state': 'OFF'}]}"""
         await self.login_if_needed()
+        if not len(ids):
+            return {}
         return await self._send_request(ApiCommand.GET_MULTI_STATES, ids)
 
     async def get_state(self, id: int) -> dict:
         """returns JSON {'status': 'OK', 'data': 'OFF'}"""
         await self.login_if_needed()
         return await self._send_request(ApiCommand.GET_STATE, id)
 
@@ -209,23 +236,26 @@
         if data[ApiAttribute.STATUS] != ApiStatus.OK:
             raise SwitchBeeError
 
         # clear the old fetched devices
         self._devices_map.clear()
         self._modules_map.clear()
         self._name = data[ApiAttribute.DATA][ApiAttribute.NAME]
-        self._version = data[ApiAttribute.DATA][ApiAttribute.VERSION]
+        self._version = CUVersion(data[ApiAttribute.DATA][ApiAttribute.VERSION])
         self._mac = data[ApiAttribute.DATA][ApiAttribute.MAC]
-
+        self._unique_id = (
+            None
+            if ApiAttribute.CU_CODE not in data[ApiAttribute.DATA]
+            else data[ApiAttribute.DATA][ApiAttribute.CU_CODE]
+        )
         if include is None:
             return
 
         for zone in data[ApiAttribute.DATA][ApiAttribute.ZONES]:
             for item in zone[ApiAttribute.ITEMS]:
-
                 try:
                     device_type = DeviceType(item[ApiAttribute.TYPE])
                 except ValueError:
                     logger.warning(
                         "Unknown device type %s (%s), Skipping",
                         item[ApiAttribute.TYPE],
                         item[ApiAttribute.NAME],
@@ -332,23 +362,23 @@
                         id=device_id,
                         name=device_name,
                         zone=zone[ApiAttribute.NAME],
                         hardware=device_hw,
                         type=device_type,
                     )
 
-                elif device_type == DeviceType.Thermostat:
+                elif device_type in [DeviceType.Thermostat, DeviceType.VRFAC]:
                     self._devices_map[item[ApiAttribute.ID]] = SwitchBeeThermostat(
                         id=device_id,
                         name=device_name,
                         zone=zone[ApiAttribute.NAME],
                         hardware=device_hw,
                         type=device_type,
                         modes=item[ApiAttribute.MODES],
-                        unit=item[ApiAttribute.TEMPERATURE_UNITS],
+                        temperature_unit=item[ApiAttribute.TEMPERATURE_UNITS],
                     )
 
                 # add rolling scenario
                 elif device_type == DeviceType.RollingScenario:
                     self._devices_map[item[ApiAttribute.ID]] = SwitchBeeRollingScenario(
                         id=device_id,
                         name=device_name,
@@ -400,80 +430,96 @@
                 self._modules_map[unit_id].add(
                     self._devices_map[item[ApiAttribute.ID]].hardware.display
                 )
 
     async def fetch_states(
         self,
     ) -> None:
-
         states = await self.get_multiple_states(
             [
                 dev
                 for dev in self._devices_map.keys()
-                if self._devices_map[dev].hardware != HardwareType.Virtual
+                if (self._devices_map[dev].hardware != HardwareType.Virtual
+                    or self._devices_map[dev].type == DeviceType.VRFAC)
                 and self._devices_map[dev].type
                 in [
                     DeviceType.Switch,
                     DeviceType.GroupSwitch,
                     DeviceType.Dimmer,
                     DeviceType.Shutter,
                     DeviceType.TimedPowerSwitch,
                     DeviceType.Thermostat,
                     DeviceType.TimedSwitch,
+                    DeviceType.VRFAC,
                 ]
             ]
         )
 
+        if not states:
+            logger.debug('get_multiple_states returned empty dict')
+            return
+
+
         for device_state in states[ApiAttribute.DATA]:
             device_id = device_state[ApiAttribute.ID]
-
             self.update_device_state(device_id, device_state[ApiAttribute.STATE])
 
-    def update_device_state(self, device_id: int, state: str | int | dict) -> None:
+    def update_device_state(self, device_id: int, new_state: str | int | dict) -> bool:
         """Update device state."""
 
         if device_id not in self._devices_map:
             logger.debug("Device id %d is not tracked", device_id)
-            return
+            return False
 
         device = self._devices_map[device_id]
 
-        # temp workaround
-        if isinstance(state, float):
-            state = int(state)
-
         if isinstance(device, SwitchBeeDimmer):
-            assert isinstance(state, (str, int))
-            device.brightness = state  # type: ignore
+            assert isinstance(new_state, (str, int))
+            device.brightness = new_state  # type: ignore
+
         elif isinstance(device, SwitchBeeShutter):
-            assert isinstance(state, (str, int))
-            device.position = state  # type: ignore
+            assert isinstance(new_state, (str, int))
+            device.position = new_state  # type: ignore
+
         elif isinstance(
             device,
             (
                 SwitchBeeSwitch,
                 SwitchBeeGroupSwitch,
                 SwitchBeeTimedSwitch,
                 SwitchBeeTimerSwitch,
             ),
         ):
-
-            assert isinstance(state, (int, str))
-            device.state = state
+            assert isinstance(new_state, (int, str))
+            device.state = new_state
 
         elif isinstance(device, SwitchBeeThermostat):
+            
+            if not isinstance(new_state, dict):
+                logger.warning(
+                    "%s: Received invalid state from CU, keeping the old one: %s",
+                    device.name,
+                    new_state,
+                )
+
+                return False
+
             try:
-                assert isinstance(state, dict)
-                device.state = state[ApiAttribute.POWER]
+                device.state = new_state[ApiAttribute.POWER]
             except TypeError:
-                logger.error(
+                logger.warning(
                     "%s: Received invalid state from CU, keeping the old one: %s",
                     device.name,
-                    state,
+                    new_state,
                 )
-                return
+                return False
+
+            device.mode = new_state[ApiAttribute.MODE]
+            device.fan = new_state[ApiAttribute.FAN]
+
+            device.target_temperature = new_state[ApiAttribute.CONFIGURED_TEMPERATURE]
+            device.temperature = new_state[ApiAttribute.ROOM_TEMPERATURE]
 
-            device.mode = state[ApiAttribute.MODE]
-            device.fan = state[ApiAttribute.FAN]
+        else:
+            return False
 
-            device.target_temperature = state[ApiAttribute.CONFIGURED_TEMPERATURE]
-            device.temperature = state[ApiAttribute.ROOM_TEMPERATURE]
+        return True
```

### Comparing `pyswitchbee-1.7.9/src/switchbee/api/polling.py` & `pyswitchbee-1.8.0/src/switchbee/api/polling.py`

 * *Files identical despite different names*

### Comparing `pyswitchbee-1.7.9/src/switchbee/api/wsrpc.py` & `pyswitchbee-1.8.0/src/switchbee/api/wsrpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         return self._call_id
 
     def subscribe_updates(self, callback: Callable) -> None:
         self._on_notification = callback
 
     async def connect(self) -> None:
         if self.connected:
-            raise RuntimeError("Already connected")        
+            raise RuntimeError("Already connected")
 
         logger.debug("Trying to connect to device at %s", self._ip_address)
         try:
             self._client = await self._aiohttp_session.ws_connect(
                 f"http://{self._ip_address}:7891"
             )
         except (
@@ -201,14 +201,16 @@
             if not call.resolve.cancelled():
                 call.resolve.set_result(frame)
 
         else:
             if notification_type := frame.get("notificationType"):
                 # this is a notification
                 logger.debug("Notification %s %s", notification_type, frame)
+                # update the devices states based on the event
+                self.update_device_state_from_event(frame)
                 if self._on_notification:
                     self._on_notification(frame)
             else:
                 logger.warning("Invalid frame: %s", frame)
 
     async def call(
         self,
@@ -253,11 +255,14 @@
         )
 
         super()._update_login(resp)
 
     def update_device_state_from_event(self, push_data: dict) -> None:
         """Update device state from notification data."""
 
-        if dev_id := push_data.get(ApiAttribute.ID):
-            return self.update_device_state(dev_id, push_data[ApiAttribute.NEW_VALUE])
+        if ApiAttribute.ID not in push_data:
+            logger.error("Received update with no device id: %s", push_data)
+            return
 
-        logger.warning("Received update with no device id: %s", push_data)
+        self.update_device_state(
+            push_data[ApiAttribute.ID], push_data[ApiAttribute.NEW_VALUE]
+        )
```

### Comparing `pyswitchbee-1.7.9/src/switchbee/central_unit/__init__.py` & `pyswitchbee-1.8.0/src/switchbee/central_unit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyswitchbee-1.7.9/src/switchbee/const.py` & `pyswitchbee-1.8.0/src/switchbee/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,19 +42,21 @@
     MODES = "modes"
     POWER = "power"
     MODE = "mode"
     FAN = "fan"
     CONFIGURED_TEMPERATURE = "configuredTemperature"
     ROOM_TEMPERATURE = "roomTemperature"
     NEW_VALUE = "newValue"
+    CU_CODE = "cuCode"
 
 
 class ApiStateCommand:
     ON = "ON"
     OFF = "OFF"
+    OFFLINE = "OFFLINE"
 
 
 # SwitchBee device hardware
 class ApiDeviceHardware:
     DIMMABLE_SWITCH = "DIMMABLE_SWITCH"
     SHUTTER = "SHUTTER"
     VIRTUAL = "VIRTUAL"
@@ -82,14 +84,15 @@
     IR_DEVICE = "IR_DEVICE"
     THERMOSTAT = "THERMOSTAT"
     LOCK_GROUP = "LOCK_GROUP"
     TIMED_SWITCH = "TIMED_SWITCH"
     LOUVERED_SHUTTER = "LOUVERED_SHUTTER"
     SOMFY = "SOMFY"
     ROLLING_SCENARIO = "ROLLING_SCENARIO"
+    VRF_AC = "VRF_AC"
 
 
 class ThermostatMode:
     HEAT = "HEAT"
     COOL = "COOL"
     FAN = "FAN"
```

### Comparing `pyswitchbee-1.7.9/src/switchbee/device/__init__.py` & `pyswitchbee-1.8.0/src/switchbee/device/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     TimedPowerSwitch = ApiDeviceType.TIMED_POWER, "Timed Power Switch"
     Thermostat = ApiDeviceType.THERMOSTAT, "Thermostat"
     LockGroup = ApiDeviceType.LOCK_GROUP, "Lock Group"
     TimedSwitch = ApiDeviceType.TIMED_SWITCH, "Timed Switch"
     Somfy = ApiDeviceType.SOMFY, "Somfy"
     IrDevice = ApiDeviceType.IR_DEVICE, "Infra Red Device"
     RollingScenario = ApiDeviceType.ROLLING_SCENARIO, "Rolling Scenario"
+    VRFAC = ApiDeviceType.VRF_AC, "VRF Unit"
 
     def __new__(cls, *args: Any, **kwds: Any):  # type: ignore
         obj = object.__new__(cls)
         obj._value_ = args[0]
         return obj
 
     # ignore the first param since it's already set by __new__
@@ -91,75 +92,83 @@
 
     def __hash__(self) -> int:
         return self.id
 
 
 @dataclass
 class SwitchBeeBaseSwitch(ABC):
-    _state: str | None = field(init=False, default=None)
+    _state: str | int | None = field(init=False, default=None)
 
     @property
-    def state(self) -> str | None:
+    def state(self) -> str | int | None:
         return self._state
 
     @state.setter
-    def state(self, value: str) -> None:
-        self._state = value
+    def state(self, value: str | int) -> None:
+        if value in [ApiStateCommand.OFF, 0]:
+            self._state = ApiStateCommand.OFF
+        elif value in [ApiStateCommand.ON, 100]:
+            self._state = ApiStateCommand.ON
+        else:  # OFFLINE
+            self._state = -1
 
 
 @dataclass
 class SwitchBeeBaseShutter(ABC):
-    _position: int | None = field(init=False, repr=False, default=None)
+    _position: int | None = field(init=False, default=None)
 
     @property
     def position(self) -> int | None:
         return self._position
 
     @position.setter
     def position(self, value: str | int) -> None:
-
-        if value == ApiStateCommand.OFF:
-            self._position = 0
-        elif value == ApiStateCommand.ON:
-            self._position = 100
-        else:
+        if isinstance(value, int):
             self._position = int(value)
+        else:
+            if value == ApiStateCommand.ON:
+                self._position = 100
+            elif value == ApiStateCommand.OFF:
+                self._position = 0
+            else:  # OFFLINE
+                self._position = -1
 
 
 @dataclass
 class SwitchBeeBaseDimmer(ABC):
-
-    _brightness: int = field(init=False)
+    _brightness: int = field(init=False, repr=False)
 
     @property
     def brightness(self) -> int:
         return self._brightness
 
     @brightness.setter
     def brightness(self, value: str | int) -> None:
-        if value == ApiStateCommand.OFF:
-            self._brightness = 0
-        elif value == ApiStateCommand.ON:
-            self._brightness = 100
-        else:
+        if isinstance(value, int):
             self._brightness = int(value)
+        else:
+            if value == ApiStateCommand.ON:
+                self._brightness = 100
+            elif value == ApiStateCommand.OFF:
+                self._brightness = 0
+            else:  # OFFLINE
+                self._brightness = -1
 
 
 @dataclass
 class SwitchBeeBaseTimer(ABC):
-    _minutes_left: int = field(init=False)
-    _state: str | int = field(init=False)
+    _minutes_left: int = field(init=False, repr=False)
+    _state: str | int = field(init=False, repr=False)
 
     @property
     def state(self) -> str | int:
         return self._state
 
     @state.setter
     def state(self, value: str | int) -> None:
-
         if value:
             if value == ApiStateCommand.OFF:
                 self._minutes_left = 0
                 self._state = value
             else:
                 self._minutes_left = int(value)
                 self._state = ApiStateCommand.ON
@@ -167,21 +176,20 @@
     @property
     def minutes_left(self) -> int:
         return self._minutes_left
 
 
 @dataclass
 class SwitchBeeBaseThermostat(ABC):
-
     modes: List[str]
-    unit: str
-    mode: str = field(init=False)
-    fan: str = field(init=False)
-    target_temperature: int = field(init=False)
-    temperature: int = field(init=False)
+    temperature_unit: str
+    mode: str = field(init=False, repr=False)
+    fan: str = field(init=False, repr=False)
+    target_temperature: int = field(init=False, repr=False)
+    temperature: int = field(init=False, repr=False)
     max_temperature: int = 31
     min_temperature: int = 16
 
 
 @final
 @dataclass
 class SwitchBeeSwitch(SwitchBeeBaseSwitch, SwitchBeeBaseDevice):
@@ -265,15 +273,15 @@
 @final
 @dataclass
 class SwitchBeeThermostat(
     SwitchBeeBaseThermostat, SwitchBeeBaseSwitch, SwitchBeeBaseDevice
 ):
     def __post_init__(self) -> None:
         """Post initialization validate device type category as Thermostat."""
-        if self.type != DeviceType.Thermostat:
+        if self.type not in [DeviceType.Thermostat, DeviceType.VRFAC]:
             raise ValueError("only Thermostat are allowed")
         super().__post_init__()
 
 
 @final
 @dataclass
 class SwitchBeeLockGroup(SwitchBeeBaseSwitch, SwitchBeeBaseDevice):
```

