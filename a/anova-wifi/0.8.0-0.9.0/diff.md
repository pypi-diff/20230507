# Comparing `tmp/anova_wifi-0.8.0.tar.gz` & `tmp/anova_wifi-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anova_wifi-0.8.0.tar", max compression
+gzip compressed data, was "anova_wifi-0.9.0.tar", max compression
```

## Comparing `anova_wifi-0.8.0.tar` & `anova_wifi-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-04-21 13:12:03.528793 anova_wifi-0.8.0/LICENSE
--rw-r--r--   0        0        0     4360 2023-04-21 13:12:03.528793 anova_wifi-0.8.0/README.md
--rw-r--r--   0        0        0     2220 2023-04-21 13:12:04.352851 anova_wifi-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      483 2023-04-21 13:12:04.312848 anova_wifi-0.8.0/src/anova_wifi/__init__.py
--rw-r--r--   0        0        0      185 2023-04-21 13:12:03.532793 anova_wifi-0.8.0/src/anova_wifi/exceptions.py
--rw-r--r--   0        0        0     4455 2023-04-21 13:12:03.532793 anova_wifi-0.8.0/src/anova_wifi/parser.py
--rw-r--r--   0        0        0     8095 2023-04-21 13:12:03.532793 anova_wifi-0.8.0/src/anova_wifi/precission_cooker.py
--rw-r--r--   0        0        0        0 2023-04-21 13:12:03.532793 anova_wifi-0.8.0/src/anova_wifi/py.typed
--rw-r--r--   0        0        0     5428 1970-01-01 00:00:00.000000 anova_wifi-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-28 18:46:34.209962 anova_wifi-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4360 2023-04-28 18:46:34.209962 anova_wifi-0.9.0/README.md
+-rw-r--r--   0        0        0     2220 2023-04-28 18:46:35.150066 anova_wifi-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      459 2023-04-28 18:46:35.102061 anova_wifi-0.9.0/src/anova_wifi/__init__.py
+-rw-r--r--   0        0        0      185 2023-04-28 18:46:34.209962 anova_wifi-0.9.0/src/anova_wifi/exceptions.py
+-rw-r--r--   0        0        0     4455 2023-04-28 18:46:34.209962 anova_wifi-0.9.0/src/anova_wifi/parser.py
+-rw-r--r--   0        0        0     6657 2023-04-28 18:46:34.209962 anova_wifi-0.9.0/src/anova_wifi/precission_cooker.py
+-rw-r--r--   0        0        0        0 2023-04-28 18:46:34.209962 anova_wifi-0.9.0/src/anova_wifi/py.typed
+-rw-r--r--   0        0        0     5428 1970-01-01 00:00:00.000000 anova_wifi-0.9.0/PKG-INFO
```

### Comparing `anova_wifi-0.8.0/LICENSE` & `anova_wifi-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anova_wifi-0.8.0/README.md` & `anova_wifi-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `anova_wifi-0.8.0/pyproject.toml` & `anova_wifi-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anova-wifi"
-version = "0.8.0"
+version = "0.9.0"
 description = "A package to get read only data from Anova precision cookers with wifi"
 authors = ["Luke <conway220@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/conway220/anova-wifi"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `anova_wifi-0.8.0/src/anova_wifi/parser.py` & `anova_wifi-0.9.0/src/anova_wifi/parser.py`

 * *Files identical despite different names*

### Comparing `anova_wifi-0.8.0/src/anova_wifi/precission_cooker.py` & `anova_wifi-0.9.0/src/anova_wifi/precission_cooker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,73 @@
 import logging
 import secrets
 import string
-from typing import Any
+from dataclasses import dataclass
 
 import aiohttp
-from sensor_state_data.enum import StrEnum
 
 from anova_wifi.exceptions import AnovaException, AnovaOffline
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class AnovaPrecisionCookerSensor(StrEnum):
-    COOK_TIME = "cook_time"
-    MODE = "mode"
-    STATE = "state"
-    TARGET_TEMPERATURE = "target_temperature"
-    COOK_TIME_REMAINING = "cook_time_remaining"
-    FIRMWARE_VERSION = "firmware_version"
-    HEATER_TEMPERATURE = "heater_temperature"
-    TRIAC_TEMPERATURE = "triac_temperature"
-    WATER_TEMPERATURE = "water_temperature"
-
-
-class AnovaPrecisionCookerBinarySensor(StrEnum):
-    COOKING = "cooking"
-    PREHEATING = "preheating"
-    MAINTAINING = "maintaining"
-    DEVICE_SAFE = "device_safe"
-    WATER_LEAK = "water_leak"
-    WATER_LEVEL_CRITICAL = "water_level_critical"
-    WATER_TEMP_TOO_HIGH = "water_temp_too_high"
-
-
 MODE_MAP = {"IDLE": "Idle", "COOK": "Cook", "LOW WATER": "Low water"}
 
 STATE_MAP = {
     "PREHEATING": "Preheating",
     "COOKING": "Cooking",
     "MAINTAINING": "Maintaining",
     "": "No state",
 }
 
 
+@dataclass
+class APCUpdateBinary:
+    cooking: bool
+    preheating: bool
+    maintaining: bool
+    device_safe: bool
+    water_leak: bool
+    water_level_critical: bool
+    water_temp_too_high: bool
+
+
+@dataclass
+class APCUpdateSensor:
+    cook_time: int
+    mode: str
+    state: str
+    target_temperature: float
+    cook_time_remaining: int
+    firmware_version: str
+    heater_temperature: float
+    triac_temperature: float
+    water_temperature: float
+
+
+@dataclass
+class APCUpdate:
+    binary_sensor: APCUpdateBinary
+    sensor: APCUpdateSensor
+
+
 class AnovaPrecisionCooker:
     def __init__(
         self, session: aiohttp.ClientSession, device_key: str, type: str, jwt: str
     ) -> None:
         self.session = session
         self.device_key = device_key
         self.type = type
         self._jwt = jwt
-        self.cook_time: float | None = None
-        self.mode: str | None = None
-        self.target_temperature: float | None = None
-        self.temperature_unit: float | None = None
+        self.status: APCUpdate | None = None
+        self.temperature_unit: str = "C"
 
     async def update(
         self,
-    ) -> dict[str, dict[str, Any]]:
+    ) -> APCUpdate:
         """Updates the Sous vide's data with a non-authenticated api call"""
         try:
             http_response = await self.session.get(
                 f"https://anovaculinary.io/devices/{self.device_key}/states/?limit=1"
             )
             anova_status_json = await http_response.json()
             anova_status = anova_status_json[0].get("body")
@@ -72,104 +77,68 @@
                 "Cannot connect to sous vide - perhaps it is not online?"
             )
         system_info = "system-info"
         for key in anova_status.keys():
             if "system-info" in key and "details" not in key and "nxp" not in key:
                 system_info = key
                 break
-        self.mode = anova_status["job"]["mode"]
-        self.cook_time = anova_status["job"]["cook-time-seconds"]
-        self.target_temperature = anova_status["job"]["target-temperature"]
-        self.temperature_unit = anova_status["job"]["temperature-unit"]
-        return {
-            "sensors": {
-                AnovaPrecisionCookerSensor.COOK_TIME: anova_status["job"][
-                    "cook-time-seconds"
-                ],
-                AnovaPrecisionCookerSensor.MODE: MODE_MAP.get(
-                    anova_status["job"]["mode"]
-                ),
-                AnovaPrecisionCookerSensor.STATE: STATE_MAP.get(
-                    anova_status["job-status"]["state"],
-                ),
-                AnovaPrecisionCookerSensor.TARGET_TEMPERATURE: anova_status["job"][
-                    "target-temperature"
-                ],
-                AnovaPrecisionCookerSensor.COOK_TIME_REMAINING: anova_status[
-                    "job-status"
-                ]["cook-time-remaining"],
-                AnovaPrecisionCookerSensor.FIRMWARE_VERSION: anova_status[system_info][
-                    "firmware-version"
-                ],
-                AnovaPrecisionCookerSensor.HEATER_TEMPERATURE: anova_status[
-                    "temperature-info"
-                ]["heater-temperature"],
-                AnovaPrecisionCookerSensor.TRIAC_TEMPERATURE: anova_status[
-                    "temperature-info"
-                ]["triac-temperature"],
-                AnovaPrecisionCookerSensor.WATER_TEMPERATURE: anova_status[
-                    "temperature-info"
-                ]["water-temperature"],
-            },
-            "binary_sensors": {
-                AnovaPrecisionCookerBinarySensor.COOKING: anova_status["job-status"][
-                    "state"
-                ]
-                == "COOKING",
-                AnovaPrecisionCookerBinarySensor.PREHEATING: anova_status["job-status"][
-                    "state"
-                ]
-                == "PREHEATING",
-                AnovaPrecisionCookerBinarySensor.MAINTAINING: anova_status[
-                    "job-status"
-                ]["state"]
-                == "MAINTAINING",
-                AnovaPrecisionCookerBinarySensor.DEVICE_SAFE: anova_status["pin-info"][
-                    "device-safe"
-                ]
-                == 1,
-                AnovaPrecisionCookerBinarySensor.WATER_LEAK: anova_status["pin-info"][
-                    "water-leak"
-                ]
-                == 1,
-                AnovaPrecisionCookerBinarySensor.WATER_LEVEL_CRITICAL: anova_status[
-                    "pin-info"
-                ]["water-level-critical"]
-                == 1,
-                AnovaPrecisionCookerBinarySensor.WATER_TEMP_TOO_HIGH: anova_status[
-                    "pin-info"
-                ]["water-temp-too-high"]
-                == 1
-                if "water-temp-too-high" in anova_status["pin-info"]
-                else None,
-            },
-        }
+        binary_sensor = APCUpdateBinary(
+            cooking=anova_status["job-status"]["state"] == "COOKING",
+            preheating=anova_status["job-status"]["state"] == "PREHEATING",
+            maintaining=anova_status["job-status"]["state"] == "MAINTAINING",
+            device_safe=anova_status["pin-info"]["device-safe"] == 1,
+            water_leak=anova_status["pin-info"]["water-leak"] == 1,
+            water_level_critical=anova_status["pin-info"]["water-level-critical"] == 1,
+            water_temp_too_high=anova_status["pin-info"]["water-temp-too-high"] == 1
+            if "water-temp-too-high" in anova_status["pin-info"]
+            else None,
+        )
+        sensor = APCUpdateSensor(
+            cook_time=anova_status["job"]["cook-time-seconds"],
+            mode=MODE_MAP.get(anova_status["job"]["mode"], "Unknown"),
+            state=STATE_MAP.get(anova_status["job-status"]["state"], "No state"),
+            target_temperature=anova_status["job"]["target-temperature"],
+            cook_time_remaining=anova_status["job-status"]["cook-time-remaining"],
+            firmware_version=anova_status[system_info]["firmware-version"],
+            heater_temperature=anova_status["temperature-info"]["heater-temperature"],
+            triac_temperature=anova_status["temperature-info"]["triac-temperature"],
+            water_temperature=anova_status["temperature-info"]["water-temperature"],
+        )
+        self.status = APCUpdate(
+            binary_sensor=binary_sensor,
+            sensor=sensor,
+        )
+        return self.status
 
     async def build_request(
         self,
         cook_time: int | None = None,
         mode: str | None = None,
         target_temperature: float | None = None,
         temperature_unit: str | None = None,
     ) -> None:
         """Builds an api call for the sous vide"""
         if self._jwt is None:
             raise AnovaException("No JWT - ")
+        if self.status is None:
+            raise AnovaException("No status - cannot build request")
         json_req = {
-            "cook-time-seconds": cook_time if cook_time is not None else self.cook_time,
+            "cook-time-seconds": cook_time
+            if cook_time is not None
+            else self.status.sensor.cook_time,
             "id": "".join(
                 secrets.choice(string.ascii_lowercase + string.digits)
                 for _ in range(22)
             ),
             # 22 digit random job ID for a new job at every save
-            "mode": mode if mode is not None else self.mode,
+            "mode": mode if mode is not None else self.status.sensor.mode,
             "ota-url": "",
             "target-temperature": target_temperature
             if target_temperature is not None
-            else self.target_temperature,
+            else self.status.sensor.target_temperature,
             "temperature-unit": temperature_unit
             if temperature_unit is not None
             else self.temperature_unit,
         }
         anova_req_headers = {"authorization": "Bearer " + self._jwt}
         _LOGGER.debug(
             "Sending https://anovaculinary.io/devices/%s/current-job with json %s and headers %s",
@@ -183,17 +152,19 @@
             headers=anova_req_headers,
         )
         if not resp.ok:
             raise Exception(f"{await resp.text()}")
         else:
             sous_vide_state = await resp.json()
             _LOGGER.debug("Got response %s", sous_vide_state)
-            self.cook_time = sous_vide_state["cook-time-seconds"]
-            self.mode = sous_vide_state["mode"]
-            self.target_temperature = sous_vide_state["target-temperature"]
+            self.status.sensor.cook_time = sous_vide_state["cook-time-seconds"]
+            self.status.sensor.mode = sous_vide_state["mode"]
+            self.status.sensor.target_temperature = sous_vide_state[
+                "target-temperature"
+            ]
             self.temperature_unit = sous_vide_state["temperature-unit"]
 
     async def set_cook_time(self, seconds: int) -> None:
         """Sets how long you want the cook to be"""
         await self.build_request(cook_time=seconds)
 
     async def set_mode(self, mode: str) -> None:
```

### Comparing `anova_wifi-0.8.0/PKG-INFO` & `anova_wifi-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anova-wifi
-Version: 0.8.0
+Version: 0.9.0
 Summary: A package to get read only data from Anova precision cookers with wifi
 Home-page: https://github.com/conway220/anova-wifi
 License: MIT
 Author: Luke
 Author-email: conway220@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anova-wifi Version: 0.8.0 Summary: A package to get
+Metadata-Version: 2.1 Name: anova-wifi Version: 0.9.0 Summary: A package to get
 read only data from Anova precision cookers with wifi Home-page: https://
 github.com/conway220/anova-wifi License: MIT Author: Luke Author-email:
 conway220@gmail.com Requires-Python: >=3.10,<4.0 Classifier: Development Status
 :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

