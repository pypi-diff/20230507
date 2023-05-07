# Comparing `tmp/gama_config-1.14.0.tar.gz` & `tmp/gama_config-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gama_config-1.14.0.tar", last modified: Sun May  7 13:28:20 2023, max compression
+gzip compressed data, was "gama_config-1.9.0.tar", last modified: Sun Apr 16 23:29:11 2023, max compression
```

## Comparing `gama_config-1.14.0.tar` & `gama_config-1.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-05-07 13:28:20.167418 gama_config-1.14.0/
--rw-rw-r--   0 runner    (1000) runner    (1001)     1529 2023-05-07 13:28:20.167418 gama_config-1.14.0/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      886 2023-05-07 13:27:31.000000 gama_config-1.14.0/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-05-07 13:28:20.167418 gama_config-1.14.0/gama_config/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-05-07 13:27:31.000000 gama_config-1.14.0/gama_config/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1657 2023-05-07 13:27:31.000000 gama_config-1.14.0/gama_config/gama_gs.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     3261 2023-05-07 13:27:31.000000 gama_config-1.14.0/gama_config/gama_vessel.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      620 2023-05-07 13:27:31.000000 gama_config-1.14.0/gama_config/generate_schemas.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1406 2023-05-07 13:27:31.000000 gama_config-1.14.0/gama_config/helpers.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-05-07 13:28:20.167418 gama_config-1.14.0/gama_config/schemas/
--rw-rw-r--   0 runner    (1000) runner    (1001)     1844 2023-05-07 13:27:31.000000 gama_config-1.14.0/gama_config/schemas/gama_gs.schema.json
--rw-rw-r--   0 runner    (1000) runner    (1001)     4677 2023-05-07 13:27:31.000000 gama_config-1.14.0/gama_config/schemas/gama_vessel.schema.json
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-05-07 13:28:20.167418 gama_config-1.14.0/gama_config.egg-info/
--rw-rw-r--   0 runner    (1000) runner    (1001)     1529 2023-05-07 13:28:20.000000 gama_config-1.14.0/gama_config.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      445 2023-05-07 13:28:20.000000 gama_config-1.14.0/gama_config.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-05-07 13:28:20.000000 gama_config-1.14.0/gama_config.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       35 2023-05-07 13:28:20.000000 gama_config-1.14.0/gama_config.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       12 2023-05-07 13:28:20.000000 gama_config-1.14.0/gama_config.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-05-07 13:28:06.000000 gama_config-1.14.0/gama_config.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)      864 2023-05-07 13:28:20.167418 gama_config-1.14.0/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-05-07 13:27:31.000000 gama_config-1.14.0/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:11.865756 gama_config-1.9.0/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1470 2023-04-16 23:29:11.865756 gama_config-1.9.0/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      828 2023-04-16 23:28:20.000000 gama_config-1.9.0/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:11.865756 gama_config-1.9.0/gama_config/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2023-04-16 23:28:20.000000 gama_config-1.9.0/gama_config/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1657 2023-04-16 23:28:20.000000 gama_config-1.9.0/gama_config/gama_gs.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2084 2023-04-16 23:28:20.000000 gama_config-1.9.0/gama_config/gama_vessel.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      620 2023-04-16 23:28:20.000000 gama_config-1.9.0/gama_config/generate_schemas.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1340 2023-04-16 23:28:20.000000 gama_config-1.9.0/gama_config/helpers.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:11.865756 gama_config-1.9.0/gama_config/schemas/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1844 2023-04-16 23:28:20.000000 gama_config-1.9.0/gama_config/schemas/gama_gs.schema.json
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2990 2023-04-16 23:28:20.000000 gama_config-1.9.0/gama_config/schemas/gama_vessel.schema.json
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-04-16 23:29:11.865756 gama_config-1.9.0/gama_config.egg-info/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1470 2023-04-16 23:29:11.000000 gama_config-1.9.0/gama_config.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      445 2023-04-16 23:29:11.000000 gama_config-1.9.0/gama_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-16 23:29:11.000000 gama_config-1.9.0/gama_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       35 2023-04-16 23:29:11.000000 gama_config-1.9.0/gama_config.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       12 2023-04-16 23:29:11.000000 gama_config-1.9.0/gama_config.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-04-16 23:28:56.000000 gama_config-1.9.0/gama_config.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)      863 2023-04-16 23:29:11.869756 gama_config-1.9.0/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-04-16 23:28:20.000000 gama_config-1.9.0/setup.py
```

### Comparing `gama_config-1.14.0/PKG-INFO` & `gama_config-1.9.0/gama_config.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gama_config
-Version: 1.14.0
+Name: gama-config
+Version: 1.9.0
 Summary: A library for reading / writing GAMA config files
 Home-page: https://github.com/Greenroom-Robotics/gama
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
@@ -20,15 +20,15 @@
 
 GAMA Config is used to load config stored inside the `.gama` folder.
 
 ## Install
 
 * `pip install -e ./libs/gama_config`
 * or...
-* `pip install gama_config` (Public on [PyPi](https://pypi.org/project/gama-config/))
+* `pip install gama_config`
 
 ## Usage
 
 ### Reading config
 
 ```python
 from gama_config.gama_vessel import read_vessel_config
```

### Comparing `gama_config-1.14.0/gama_config/gama_gs.py` & `gama_config-1.9.0/gama_config/gama_gs.py`

 * *Files identical despite different names*

### Comparing `gama_config-1.14.0/gama_config/gama_vessel.py` & `gama_config-1.9.0/gama_config/gama_vessel.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # IMPORTANT
 # After changing this file, run `python3 -m gama_config.generate_schemas`
 # To re-generate the json schemas
 
 from dataclasses import dataclass
 from enum import Enum
 from dacite import from_dict, Config
-from typing import Optional, Any, List, Annotated
-from gama_config.helpers import write_config, read_config, find_gama_config, join_lines
-from dc_schema import SchemaAnnotation
-
+from typing import Optional, Any
+from gama_config.helpers import write_config, read_config, find_gama_config
 
 GAMA_VESSEL_FILE_NAME = "gama_vessel.yml"
 GAMA_VESSEL_SCHEMA_URL = (
     "https://greenroom-robotics.github.io/gama/schemas/gama_vessel.schema.json"
 )
 
 
@@ -42,64 +40,28 @@
 class GamaVesselConfigExtensions:
     lookout: bool = False
     rviz: bool = False
     groot: bool = False
 
 
 @dataclass
-class Pipeline:
-    # This will become the name of frame-id, ros topic and webrtc steam
-    name: str
-    # Used to order the stream in the UI
-    order: Optional[int]
-    # An array of gstream source / transform elements
-    # eg)
-    # ["v4l2src", "video/x-raw, format=RGB,width=1920,height=1080"]
-    elements: List[str]
-
-
-@dataclass
-class GamaVesselGreenstream:
-    pipeline_overrides: Annotated[
-        Optional[List[Optional[Pipeline]]],
-        SchemaAnnotation(
-            description=join_lines(
-                "A list of greenstream pipelines.",
-                "These will only take affect if the the mode is 'hardware'",
-                "",
-                "Set these to 'null' to ignore the override.",
-            ),
-            examples=[
-                join_lines(
-                    "- null",
-                    "- name: fwd",
-                    "  elements:" "  - v4l2src",
-                    "  - video/x-raw, format=RGB,width=1920,height=1080",
-                )
-            ],
-        ),
-    ] = None
-
-
-@dataclass
 class GamaVesselConfig:
     variant: Variant = Variant.WHISKEY_BRAVO
     mode: Mode = Mode.SIMULATOR
     extensions: GamaVesselConfigExtensions = GamaVesselConfigExtensions()
     network: Network = Network.SHARED
     prod: bool = False
     log_level: LogLevel = LogLevel.INFO
     ubiquity_user: Optional[str] = None
     ubiquity_pass: Optional[str] = None
     ubiquity_ip: Optional[str] = None
     ddsrouter_groundstation_ip: Optional[str] = None
     ddsrouter_groundstation_port: Optional[str] = None
     ddsrouter_vessel_ip: Optional[str] = None
     ddsrouter_vessel_port: Optional[str] = None
-    greenstream: GamaVesselGreenstream = GamaVesselGreenstream()
 
 
 def parse_vessel_config(config: dict[str, Any]) -> GamaVesselConfig:
     return from_dict(
         GamaVesselConfig,
         config,
         config=Config(cast=[Mode, Network, Variant, LogLevel]),
```

### Comparing `gama_config-1.14.0/gama_config/generate_schemas.py` & `gama_config-1.9.0/gama_config/generate_schemas.py`

 * *Files identical despite different names*

### Comparing `gama_config-1.14.0/gama_config/helpers.py` & `gama_config-1.9.0/gama_config/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,18 +4,14 @@
 import os
 from typing import Any, Callable
 from pathlib import Path
 
 type_parse = Callable[[Any], Any]
 
 
-def join_lines(*lines: str) -> str:
-    return "\n".join(lines)
-
-
 def find_gama_config() -> Path:
     """Returns the path to the .gama directory"""
     path = Path.cwd()
     while len(path.parts) > 1:
         if (path / ".gama").exists():
             return path / ".gama"
         else:
```

### Comparing `gama_config-1.14.0/gama_config/schemas/gama_gs.schema.json` & `gama_config-1.9.0/gama_config/schemas/gama_gs.schema.json`

 * *Files identical despite different names*

### Comparing `gama_config-1.14.0/gama_config.egg-info/PKG-INFO` & `gama_config-1.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gama-config
-Version: 1.14.0
+Name: gama_config
+Version: 1.9.0
 Summary: A library for reading / writing GAMA config files
 Home-page: https://github.com/Greenroom-Robotics/gama
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
@@ -20,15 +20,15 @@
 
 GAMA Config is used to load config stored inside the `.gama` folder.
 
 ## Install
 
 * `pip install -e ./libs/gama_config`
 * or...
-* `pip install gama_config` (Public on [PyPi](https://pypi.org/project/gama-config/))
+* `pip install gama_config`
 
 ## Usage
 
 ### Reading config
 
 ```python
 from gama_config.gama_vessel import read_vessel_config
```

### Comparing `gama_config-1.14.0/setup.cfg` & `gama_config-1.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gama_config
-version = 1.14.0
+version = 1.9.0
 url = https://github.com/Greenroom-Robotics/gama
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
```

