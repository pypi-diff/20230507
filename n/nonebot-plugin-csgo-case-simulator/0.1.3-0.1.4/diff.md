# Comparing `tmp/nonebot-plugin-csgo-case-simulator-0.1.3.tar.gz` & `tmp/nonebot-plugin-csgo-case-simulator-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-csgo-case-simulator-0.1.3.tar", max compression
+gzip compressed data, was "nonebot-plugin-csgo-case-simulator-0.1.4.tar", max compression
```

## Comparing `nonebot-plugin-csgo-case-simulator-0.1.3.tar` & `nonebot-plugin-csgo-case-simulator-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-05-06 16:52:29.595978 nonebot-plugin-csgo-case-simulator-0.1.3/LICENSE
--rw-r--r--   0        0        0     3194 2023-05-06 19:24:50.184276 nonebot-plugin-csgo-case-simulator-0.1.3/nonebot-plugin-csgo-case-simulator/__init__.py
--rw-r--r--   0        0        0   274723 2023-05-06 15:50:23.752798 nonebot-plugin-csgo-case-simulator-0.1.3/nonebot-plugin-csgo-case-simulator/background2.png
--rw-r--r--   0        0        0     2442 2023-05-06 19:24:19.879469 nonebot-plugin-csgo-case-simulator-0.1.3/nonebot-plugin-csgo-case-simulator/cases.py
--rw-r--r--   0        0        0     1846 2023-05-06 19:24:30.996173 nonebot-plugin-csgo-case-simulator-0.1.3/nonebot-plugin-csgo-case-simulator/skins.py
--rw-r--r--   0        0        0     3649 2023-05-06 19:29:41.725607 nonebot-plugin-csgo-case-simulator-0.1.3/nonebot-plugin-csgo-case-simulator/utils.py
--rw-r--r--   0        0        0      516 2023-05-06 19:29:56.925975 nonebot-plugin-csgo-case-simulator-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      768 2023-05-06 19:30:26.509006 nonebot-plugin-csgo-case-simulator-0.1.3/setup.py
--rw-r--r--   0        0        0      546 2023-05-06 19:30:26.509136 nonebot-plugin-csgo-case-simulator-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-06 19:37:08.273216 nonebot-plugin-csgo-case-simulator-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3194 2023-05-06 19:37:08.273449 nonebot-plugin-csgo-case-simulator-0.1.4/nonebot-plugin-csgo-case-simulator/__init__.py
+-rw-r--r--   0        0        0   274723 2023-05-06 19:37:08.274212 nonebot-plugin-csgo-case-simulator-0.1.4/nonebot-plugin-csgo-case-simulator/background2.png
+-rw-r--r--   0        0        0     2442 2023-05-06 19:37:08.274307 nonebot-plugin-csgo-case-simulator-0.1.4/nonebot-plugin-csgo-case-simulator/cases.py
+-rw-r--r--   0        0        0     1846 2023-05-06 19:37:08.274385 nonebot-plugin-csgo-case-simulator-0.1.4/nonebot-plugin-csgo-case-simulator/skins.py
+-rw-r--r--   0        0        0     3691 2023-05-07 01:34:42.011243 nonebot-plugin-csgo-case-simulator-0.1.4/nonebot-plugin-csgo-case-simulator/utils.py
+-rw-r--r--   0        0        0      516 2023-05-07 01:37:06.693268 nonebot-plugin-csgo-case-simulator-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      768 2023-05-07 01:37:43.641574 nonebot-plugin-csgo-case-simulator-0.1.4/setup.py
+-rw-r--r--   0        0        0      546 2023-05-07 01:37:43.641702 nonebot-plugin-csgo-case-simulator-0.1.4/PKG-INFO
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.3/LICENSE` & `nonebot-plugin-csgo-case-simulator-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.3/nonebot-plugin-csgo-case-simulator/__init__.py` & `nonebot-plugin-csgo-case-simulator-0.1.4/nonebot-plugin-csgo-case-simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.3/nonebot-plugin-csgo-case-simulator/background2.png` & `nonebot-plugin-csgo-case-simulator-0.1.4/nonebot-plugin-csgo-case-simulator/background2.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.3/nonebot-plugin-csgo-case-simulator/cases.py` & `nonebot-plugin-csgo-case-simulator-0.1.4/nonebot-plugin-csgo-case-simulator/cases.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.3/nonebot-plugin-csgo-case-simulator/skins.py` & `nonebot-plugin-csgo-case-simulator-0.1.4/nonebot-plugin-csgo-case-simulator/skins.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.3/nonebot-plugin-csgo-case-simulator/utils.py` & `nonebot-plugin-csgo-case-simulator-0.1.4/nonebot-plugin-csgo-case-simulator/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import asyncio
 import base64
 from io import BytesIO
 import math
 import os
-import time
 from PIL import Image, ImageFont, ImageDraw, ImageFilter
 import httpx
 
 
+FONT = font_path = os.path.join('..', 'font', '仓耳舒圆体W03.ttf')
+
+
 class Utils:
     def __init__(self):
         self.client = httpx.Client()
         self.rarity_color = {
             "工业级": (96, 152, 217),
             "军规级": (76, 105, 255),
             "受限": (136, 70, 255),
             "保密": (177, 46, 194),
             "隐秘": (235, 75, 75),
             "及其罕见的特殊物品": (201, 171, 5),
             "非凡": (201, 171, 5),
         }
 
     async def merge_images(self, items):
-        ttf_path = "仓耳舒圆体W03.ttf"
+        ttf_path = FONT
         font = ImageFont.truetype(ttf_path, 40)
         image_list = []
 
         image_tasks = [self.download_image(item["image"]) for item in items]
         image_list = await asyncio.gather(*image_tasks)
 
         width = image_list[0].width
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.3/pyproject.toml` & `nonebot-plugin-csgo-case-simulator-0.1.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-csgo-case-simulator"
-version = "0.1.3"
+version = "0.1.4"
 description = "a nonebot based csgo case simulator"
 authors = ["Roy <lyt2980999208@gmail.com>"]
 license = "MIT"
 packages = [{ include = "nonebot-plugin-csgo-case-simulator" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.3/setup.py` & `nonebot-plugin-csgo-case-simulator-0.1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['Pillow>=9.5.0,<10.0.0',
  'httpx>=0.24.0,<0.25.0',
  'nonebot-adapter-onebot>=2.2.3,<3.0.0',
  'nonebot2>=2.0.0-rc.4,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-csgo-case-simulator',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'a nonebot based csgo case simulator',
     'long_description': None,
     'author': 'Roy',
     'author_email': 'lyt2980999208@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.3/PKG-INFO` & `nonebot-plugin-csgo-case-simulator-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-csgo-case-simulator
-Version: 0.1.3
+Version: 0.1.4
 Summary: a nonebot based csgo case simulator
 License: MIT
 Author: Roy
 Author-email: lyt2980999208@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

