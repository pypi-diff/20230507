# Comparing `tmp/bosch-control-panel-cc880p-2.3.0.tar.gz` & `tmp/bosch-control-panel-cc880p-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bosch-control-panel-cc880p-2.3.0.tar", last modified: Fri Apr 15 11:45:11 2022, max compression
+gzip compressed data, was "bosch-control-panel-cc880p-3.0.0.tar", last modified: Sun May  7 15:18:32 2023, max compression
```

## Comparing `bosch-control-panel-cc880p-2.3.0.tar` & `bosch-control-panel-cc880p-3.0.0.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 11:45:11.587613 bosch-control-panel-cc880p-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11338 2022-04-15 11:45:00.000000 bosch-control-panel-cc880p-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    22326 2022-04-15 11:45:11.587613 bosch-control-panel-cc880p-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    21606 2022-04-15 11:45:00.000000 bosch-control-panel-cc880p-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-04-15 11:45:00.000000 bosch-control-panel-cc880p-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1468 2022-04-15 11:45:11.587613 bosch-control-panel-cc880p-2.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 11:45:11.583613 bosch-control-panel-cc880p-2.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 11:45:11.583613 bosch-control-panel-cc880p-2.3.0/src/bosch/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 11:45:11.583613 bosch-control-panel-cc880p-2.3.0/src/bosch/control_panel/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 11:45:11.583613 bosch-control-panel-cc880p-2.3.0/src/bosch/control_panel/cc880p/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-15 11:45:00.000000 bosch-control-panel-cc880p-2.3.0/src/bosch/control_panel/cc880p/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 11:45:11.583613 bosch-control-panel-cc880p-2.3.0/src/bosch/control_panel/cc880p/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-15 11:45:00.000000 bosch-control-panel-cc880p-2.3.0/src/bosch/control_panel/cc880p/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2348 2022-04-15 11:45:00.000000 bosch-control-panel-cc880p-2.3.0/src/bosch/control_panel/cc880p/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-04-15 11:45:00.000000 bosch-control-panel-cc880p-2.3.0/src/bosch/control_panel/cc880p/cli/cmds.py
--rw-r--r--   0 runner    (1001) docker     (121)     3605 2022-04-15 11:45:00.000000 bosch-control-panel-cc880p-2.3.0/src/bosch/control_panel/cc880p/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    22800 2022-04-15 11:45:00.000000 bosch-control-panel-cc880p-2.3.0/src/bosch/control_panel/cc880p/cp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-04-15 11:45:00.000000 bosch-control-panel-cc880p-2.3.0/src/bosch/control_panel/cc880p/models.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-04-15 11:45:00.000000 bosch-control-panel-cc880p-2.3.0/src/bosch/control_panel/cc880p/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 11:45:11.587613 bosch-control-panel-cc880p-2.3.0/src/bosch/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-15 11:45:00.000000 bosch-control-panel-cc880p-2.3.0/src/bosch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-04-15 11:45:00.000000 bosch-control-panel-cc880p-2.3.0/src/bosch/utils/bytes_to_str.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 11:45:11.587613 bosch-control-panel-cc880p-2.3.0/src/bosch_control_panel_cc880p.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22326 2022-04-15 11:45:11.000000 bosch-control-panel-cc880p-2.3.0/src/bosch_control_panel_cc880p.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-04-15 11:45:11.000000 bosch-control-panel-cc880p-2.3.0/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-15 11:45:11.000000 bosch-control-panel-cc880p-2.3.0/src/bosch_control_panel_cc880p.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-04-15 11:45:11.000000 bosch-control-panel-cc880p-2.3.0/src/bosch_control_panel_cc880p.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-04-15 11:45:11.000000 bosch-control-panel-cc880p-2.3.0/src/bosch_control_panel_cc880p.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-15 11:45:11.000000 bosch-control-panel-cc880p-2.3.0/src/bosch_control_panel_cc880p.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:32.642022 bosch-control-panel-cc880p-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22289 2023-05-07 15:18:32.642022 bosch-control-panel-cc880p-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21606 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-07 15:18:32.642022 bosch-control-panel-cc880p-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:32.638022 bosch-control-panel-cc880p-3.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:32.638022 bosch-control-panel-cc880p-3.0.0/src/bosch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:32.638022 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:32.638022 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:32.638022 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/cli/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/cp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:32.642022 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/models/cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/models/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/models/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-07 15:18:21.000000 bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:18:32.642022 bosch-control-panel-cc880p-3.0.0/src/bosch_control_panel_cc880p.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22289 2023-05-07 15:18:32.000000 bosch-control-panel-cc880p-3.0.0/src/bosch_control_panel_cc880p.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-07 15:18:32.000000 bosch-control-panel-cc880p-3.0.0/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 15:18:32.000000 bosch-control-panel-cc880p-3.0.0/src/bosch_control_panel_cc880p.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-07 15:18:32.000000 bosch-control-panel-cc880p-3.0.0/src/bosch_control_panel_cc880p.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-07 15:18:32.000000 bosch-control-panel-cc880p-3.0.0/src/bosch_control_panel_cc880p.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 15:18:32.000000 bosch-control-panel-cc880p-3.0.0/src/bosch_control_panel_cc880p.egg-info/top_level.txt
```

### Comparing `bosch-control-panel-cc880p-2.3.0/LICENSE` & `bosch-control-panel-cc880p-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-2.3.0/PKG-INFO` & `bosch-control-panel-cc880p-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: bosch-control-panel-cc880p
-Version: 2.3.0
+Version: 3.0.0
 Summary: Library to interface with the old CC880p Bosch COntrol Panels
 Home-page: https://github.com/hgomes88/bosch-control-panel-cc880p
 Author: Hugo Gomes
 Author-email: hgomes88@gmail.com
-License: UNKNOWN
 Project-URL: Tracker, https://github.com/hgomes88/bosch-control-panel-cc880p/issues
 Project-URL: Download, https://pypi.org/project/bosch-control-panel-cc880p/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
@@ -590,9 +588,7 @@
 [level-shifter-website]: https://randomnerdtutorials.com/how-to-level-shift-5v-to-3-3v/
 [elfin-ew10-dev]: http://www.hi-flying.com/elfin-ew10-elfin-ew11
 
 [product-screenshot]: images/screenshot.png
 [a-link-plus-usb-diagram]: images/a-link-plus-usb-diagram.png
 [elfin-ew10-diagram]: images/elfin-ew10-diagram.png
 [esp8266-diagram]: images/esp8266-diagram.png
-
-
```

#### html2text {}

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 2.3.0 Summary:
+Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.0.0 Summary:
 Library to interface with the old CC880p Bosch COntrol Panels Home-page: https:
 //github.com/hgomes88/bosch-control-panel-cc880p Author: Hugo Gomes Author-
-email: hgomes88@gmail.com License: UNKNOWN Project-URL: Tracker, https://
-github.com/hgomes88/bosch-control-panel-cc880p/issues Project-URL: Download,
-https://pypi.org/project/bosch-control-panel-cc880p/ Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
-Provides-Extra: dev License-File: LICENSE
+email: hgomes88@gmail.com Project-URL: Tracker, https://github.com/hgomes88/
+bosch-control-panel-cc880p/issues Project-URL: Download, https://pypi.org/
+project/bosch-control-panel-cc880p/ Classifier: Programming Language :: Python
+:: 3 Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
+Type: text/markdown Provides-Extra: dev License-File: LICENSE
  [![Release][release-shield]][release-url] [![Build][build-shield]][build-url]
 [![MIT License][license-shield]][license-url] [![Contributors][contributors-
 shield]][contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers]
 [stars-shield]][stars-url] [![Issues][issues-shield]][issues-url] [![LinkedIn]
 [linkedin-shield]][linkedin-url]
                                    [CC880P]
                      **** Bosch Control Panel CC880P ****
```

### Comparing `bosch-control-panel-cc880p-2.3.0/README.md` & `bosch-control-panel-cc880p-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `bosch-control-panel-cc880p-2.3.0/setup.cfg` & `bosch-control-panel-cc880p-3.0.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 [options.extras_require]
 dev = 
 	twine==4.0.0
 	build==0.7.0
 	pytest==7.1.1
 	pytest-asyncio==0.18.3
+	pytest-mock==3.10.0
 	pre-commit==2.18.1
 	autopep8==1.6.0
 	flake8==4.0.1
 	mypy==0.942
 
 [options.entry_points]
 console_scripts =
```

### Comparing `bosch-control-panel-cc880p-2.3.0/src/bosch/control_panel/cc880p/cli/cli.py` & `bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/cli/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,46 @@
+"""Control panel command line interface."""
 import asyncio
 import logging
 
 from bosch.control_panel.cc880p.cli.cmds import handle_command
 from bosch.control_panel.cc880p.cli.parser import Args
 from bosch.control_panel.cc880p.cli.parser import get_args
 from bosch.control_panel.cc880p.cp import CP
-from bosch.control_panel.cc880p.models import Area
-from bosch.control_panel.cc880p.models import Availability
-from bosch.control_panel.cc880p.models import ControlPanelModel
-from bosch.control_panel.cc880p.models import Id
-from bosch.control_panel.cc880p.models import Output
-from bosch.control_panel.cc880p.models import Siren
-from bosch.control_panel.cc880p.models import Zone
-from bosch.utils.bytes_to_str import to_hex
+from bosch.control_panel.cc880p.models.cp import Area
+from bosch.control_panel.cc880p.models.cp import Availability
+from bosch.control_panel.cc880p.models.cp import ControlPanelEntity
+from bosch.control_panel.cc880p.models.cp import CpVersion
+from bosch.control_panel.cc880p.models.cp import Id
+from bosch.control_panel.cc880p.models.cp import Output
+from bosch.control_panel.cc880p.models.cp import Siren
+from bosch.control_panel.cc880p.models.cp import Zone
+from bosch.control_panel.cc880p.utils import to_hex
 
 logging.basicConfig(level=logging.WARNING)
 
 prev_data = None
 
 
 async def data_listener(data: bytes) -> bool:
+    """Listen of any control panel change."""
     global prev_data
     if prev_data and prev_data[:-2] != data[:-2]:
         print('\nDifference:')
         print(f'\tBefore:\t{to_hex(prev_data)}')
         print(f'\tAfter:\t{to_hex(data)}')
     else:
         print('\nNo Changes:')
         print(to_hex(data))
     prev_data = data
     return True
 
 
-async def cp_listener(id: Id, cp: ControlPanelModel) -> bool:
+async def cp_listener(id: Id, cp: ControlPanelEntity) -> bool:
+    """Control panel listener."""
     if isinstance(cp, Zone):
         print(f'Zone {id} updated: {cp}')
     elif isinstance(cp, Output):
         print(f'Output {id} updated: {cp}')
     elif isinstance(cp, Siren):
         print(f'Siren updated: {cp}')
     elif isinstance(cp, Area):
@@ -44,50 +48,50 @@
     elif isinstance(cp, Availability):
         print(f'Control Panel availability is: {cp}')
 
     return True
 
 
 async def run_listen_mode(cp: CP):
+    """Run the control panel in listen mode."""
     cp.add_data_listener(data_listener)
     cp.add_control_panel_listener(cp_listener)
     while True:
+        await cp.get_status()
         await asyncio.sleep(1)
 
 
 async def run_cmd_mode(cp: CP, args):
+    """Run mode command."""
     await handle_command(cp, args)
 
 
 async def run(loop):
-
+    """Run the control panel command line."""
     args: Args = get_args()
 
-    if args.cmd:
-        get_status_period_s = 0
-    else:
-        get_status_period_s = 2
-
     cp = CP(
         ip=args.connect,
         port=args.port,
+        model=CpVersion.S16_V14.model(),
+        installer_code=args.code,
         loop=loop,
-        get_status_period_s=get_status_period_s
     )
 
     await cp.start()
 
     if args.cmd:
         await run_cmd_mode(cp, args)
     else:
         await run_listen_mode(cp)
 
     await cp.stop()
 
 
 def main():
+    """Run main."""
     loop = asyncio.new_event_loop()
     loop.run_until_complete(run(loop))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `bosch-control-panel-cc880p-2.3.0/src/bosch/control_panel/cc880p/models.py` & `bosch-control-panel-cc880p-3.0.0/src/bosch/control_panel/cc880p/models/cp.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,111 @@
+"""Control panel models."""
 import datetime
 from dataclasses import dataclass
 from enum import Enum
-from typing import Callable
 from typing import Dict
 
-Id = int
+from bosch.control_panel.cc880p.models.constants import Id
 
 
 @dataclass
-class ControlPanelModel:
-    pass
+class CpModel:
+    """Control Panel model properties."""
 
+    n_zones: int
+    n_areas: int
+    n_outputs: int
 
-@dataclass
-class Siren(ControlPanelModel):
-    """ Dataclass to store the Siren of the alarm
+
+class CpVersion(Enum):
+    """Control Panel Version to be used.
+
+    Returns a Control Panel model object with the properties referred to
+    the selected version
     """
 
+    S16_V14 = CpModel(
+        n_zones=16,
+        n_areas=1,
+        n_outputs=5
+    )
+
+    def model(self) -> CpModel:
+        """Return the CpModel object."""
+        return self.value
+
+
+@dataclass
+class ControlPanelEntity:
+    """Model representing a Control Panel entity."""
+
+
+@dataclass
+class Siren(ControlPanelEntity):
+    """Dataclass to store the Siren of the alarm."""
+
     on: bool = False
 
 
 @dataclass
-class Zone(ControlPanelModel):
-    """ Dataclass to store the zones of the alarm
-    """
+class Zone(ControlPanelEntity):
+    """Dataclass to store the zones of the alarm."""
 
     triggered: bool = False
     enabled: bool = False
 
 
 @dataclass
-class Output(ControlPanelModel):
-    """Dataclass to store the varios alarm output states
-    """
+class Output(ControlPanelEntity):
+    """Dataclass to store the various alarm output states."""
 
     on: bool = False
 
 
 @dataclass
-class Availability(ControlPanelModel):
-    """Dataclass to store the varios alarm output states
-    """
+class Availability(ControlPanelEntity):
+    """Dataclass to store the various alarm output states."""
 
     available: bool = False
 
 
 class ArmingMode(Enum):
-    """Enumerator with all the alarm states
-    """
+    """Enumerator with all the alarm states."""
 
     DISARMED = 0
     ARMED_AWAY = 1
     ARMED_STAY = 2
 
 
 @dataclass
-class Area(ControlPanelModel):
-    """Dataclass representing the alarm area
-    """
+class Area(ControlPanelEntity):
+    """Dataclass representing the alarm area."""
 
     mode: ArmingMode = ArmingMode.DISARMED
 
 
 class Time(datetime.time):
-    pass
+    """Datetime."""
 
 
 @dataclass
-class ControlPanel(ControlPanelModel):
-    """Dataclass representing the control panel object
-    """
+class ControlPanel(ControlPanelEntity):
+    """Dataclass representing the control panel object."""
+
     siren: Siren
     areas: Dict[Id, Area]
     zones: Dict[Id, Zone]
     outputs: Dict[Id, Output]
     time_utc: Time
     availability: Availability
 
-
-ControlPanelListener = Callable[[Id, ControlPanelModel], bool]
-DataListener = Callable[[bytes], bool]
+    @staticmethod
+    def build(model: CpModel) -> 'ControlPanel':
+        """Build a control panel object."""
+        return ControlPanel(
+            siren=Siren(),
+            outputs={i + 1: Output() for i in range(model.n_outputs)},
+            areas={i + 1: Area() for i in range(model.n_areas)},
+            zones={i + 1: Zone() for i in range(model.n_zones)},
+            time_utc=Time(),
+            availability=Availability()
+        )
```

### Comparing `bosch-control-panel-cc880p-2.3.0/src/bosch_control_panel_cc880p.egg-info/PKG-INFO` & `bosch-control-panel-cc880p-3.0.0/src/bosch_control_panel_cc880p.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: bosch-control-panel-cc880p
-Version: 2.3.0
+Version: 3.0.0
 Summary: Library to interface with the old CC880p Bosch COntrol Panels
 Home-page: https://github.com/hgomes88/bosch-control-panel-cc880p
 Author: Hugo Gomes
 Author-email: hgomes88@gmail.com
-License: UNKNOWN
 Project-URL: Tracker, https://github.com/hgomes88/bosch-control-panel-cc880p/issues
 Project-URL: Download, https://pypi.org/project/bosch-control-panel-cc880p/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
@@ -590,9 +588,7 @@
 [level-shifter-website]: https://randomnerdtutorials.com/how-to-level-shift-5v-to-3-3v/
 [elfin-ew10-dev]: http://www.hi-flying.com/elfin-ew10-elfin-ew11
 
 [product-screenshot]: images/screenshot.png
 [a-link-plus-usb-diagram]: images/a-link-plus-usb-diagram.png
 [elfin-ew10-diagram]: images/elfin-ew10-diagram.png
 [esp8266-diagram]: images/esp8266-diagram.png
-
-
```

#### html2text {}

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 2.3.0 Summary:
+Metadata-Version: 2.1 Name: bosch-control-panel-cc880p Version: 3.0.0 Summary:
 Library to interface with the old CC880p Bosch COntrol Panels Home-page: https:
 //github.com/hgomes88/bosch-control-panel-cc880p Author: Hugo Gomes Author-
-email: hgomes88@gmail.com License: UNKNOWN Project-URL: Tracker, https://
-github.com/hgomes88/bosch-control-panel-cc880p/issues Project-URL: Download,
-https://pypi.org/project/bosch-control-panel-cc880p/ Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
-Provides-Extra: dev License-File: LICENSE
+email: hgomes88@gmail.com Project-URL: Tracker, https://github.com/hgomes88/
+bosch-control-panel-cc880p/issues Project-URL: Download, https://pypi.org/
+project/bosch-control-panel-cc880p/ Classifier: Programming Language :: Python
+:: 3 Classifier: License :: OSI Approved :: Apache Software License Classifier:
+Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
+Type: text/markdown Provides-Extra: dev License-File: LICENSE
  [![Release][release-shield]][release-url] [![Build][build-shield]][build-url]
 [![MIT License][license-shield]][license-url] [![Contributors][contributors-
 shield]][contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers]
 [stars-shield]][stars-url] [![Issues][issues-shield]][issues-url] [![LinkedIn]
 [linkedin-shield]][linkedin-url]
                                    [CC880P]
                      **** Bosch Control Panel CC880P ****
```

### Comparing `bosch-control-panel-cc880p-2.3.0/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt` & `bosch-control-panel-cc880p-3.0.0/src/bosch_control_panel_cc880p.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/bosch/control_panel/cc880p/__init__.py
 src/bosch/control_panel/cc880p/cp.py
-src/bosch/control_panel/cc880p/models.py
+src/bosch/control_panel/cc880p/utils.py
 src/bosch/control_panel/cc880p/version.py
 src/bosch/control_panel/cc880p/cli/__init__.py
 src/bosch/control_panel/cc880p/cli/cli.py
 src/bosch/control_panel/cc880p/cli/cmds.py
 src/bosch/control_panel/cc880p/cli/parser.py
-src/bosch/utils/__init__.py
-src/bosch/utils/bytes_to_str.py
+src/bosch/control_panel/cc880p/models/__init__.py
+src/bosch/control_panel/cc880p/models/callbacks.py
+src/bosch/control_panel/cc880p/models/constants.py
+src/bosch/control_panel/cc880p/models/cp.py
+src/bosch/control_panel/cc880p/models/requests.py
+src/bosch/control_panel/cc880p/models/responses.py
 src/bosch_control_panel_cc880p.egg-info/PKG-INFO
 src/bosch_control_panel_cc880p.egg-info/SOURCES.txt
 src/bosch_control_panel_cc880p.egg-info/dependency_links.txt
 src/bosch_control_panel_cc880p.egg-info/entry_points.txt
 src/bosch_control_panel_cc880p.egg-info/requires.txt
 src/bosch_control_panel_cc880p.egg-info/top_level.txt
```

