# Comparing `tmp/nonebot-plugin-csgo-case-simulator-0.1.6.tar.gz` & `tmp/nonebot-plugin-csgo-case-simulator-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-csgo-case-simulator-0.1.6.tar", max compression
+gzip compressed data, was "nonebot-plugin-csgo-case-simulator-0.1.7.tar", max compression
```

## Comparing `nonebot-plugin-csgo-case-simulator-0.1.6.tar` & `nonebot-plugin-csgo-case-simulator-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1062 2023-05-06 19:37:08.273216 nonebot-plugin-csgo-case-simulator-0.1.6/LICENSE
--rw-r--r--   0        0        0     3194 2023-05-06 19:37:08.273449 nonebot-plugin-csgo-case-simulator-0.1.6/nonebot-plugin-csgo-case-simulator/__init__.py
--rw-r--r--   0        0        0   274723 2023-05-06 19:37:08.274212 nonebot-plugin-csgo-case-simulator-0.1.6/nonebot-plugin-csgo-case-simulator/background2.png
--rw-r--r--   0        0        0     2442 2023-05-06 19:37:08.274307 nonebot-plugin-csgo-case-simulator-0.1.6/nonebot-plugin-csgo-case-simulator/cases.py
--rw-r--r--   0        0        0  3886748 2023-05-07 01:22:58.975435 nonebot-plugin-csgo-case-simulator-0.1.6/nonebot-plugin-csgo-case-simulator/font/font.ttf
--rw-r--r--   0        0        0     1846 2023-05-06 19:37:08.274385 nonebot-plugin-csgo-case-simulator-0.1.6/nonebot-plugin-csgo-case-simulator/skins.py
--rw-r--r--   0        0        0     3699 2023-05-07 02:08:04.100909 nonebot-plugin-csgo-case-simulator-0.1.6/nonebot-plugin-csgo-case-simulator/utils.py
--rw-r--r--   0        0        0      516 2023-05-07 02:08:17.269924 nonebot-plugin-csgo-case-simulator-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      818 2023-05-07 02:08:39.979017 nonebot-plugin-csgo-case-simulator-0.1.6/setup.py
--rw-r--r--   0        0        0      546 2023-05-07 02:08:39.979143 nonebot-plugin-csgo-case-simulator-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-06 19:37:08.273216 nonebot-plugin-csgo-case-simulator-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3272 2023-05-07 06:37:13.253861 nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/__init__.py
+-rw-r--r--   0        0        0   274723 2023-05-06 19:37:08.274212 nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/background2.png
+-rw-r--r--   0        0        0     2442 2023-05-06 19:37:08.274307 nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/cases.py
+-rw-r--r--   0        0        0  3886748 2023-05-07 01:22:58.975435 nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/font/font.ttf
+-rw-r--r--   0        0        0     1846 2023-05-06 19:37:08.274385 nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/skins.py
+-rw-r--r--   0        0        0     3957 2023-05-07 06:33:57.219273 nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/utils.py
+-rw-r--r--   0        0        0      516 2023-05-07 06:34:57.066286 nonebot-plugin-csgo-case-simulator-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      818 2023-05-07 06:39:19.805570 nonebot-plugin-csgo-case-simulator-0.1.7/setup.py
+-rw-r--r--   0        0        0      546 2023-05-07 06:39:19.805689 nonebot-plugin-csgo-case-simulator-0.1.7/PKG-INFO
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.6/LICENSE` & `nonebot-plugin-csgo-case-simulator-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.6/nonebot-plugin-csgo-case-simulator/__init__.py` & `nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import asyncio
-from enum import Enum
-import os
-import time
 from nonebot import on_command
 from nonebot.params import CommandArg
 from nonebot.adapters.onebot.v11 import Message, MessageSegment, MessageEvent
-import httpx
 from .cases import Cases
 from .skins import Skins
 from .utils import Utils
 
 cases = Cases()
 skins = Skins()
 utils = Utils()
@@ -31,34 +27,34 @@
     "非凡": 6,
 }
 
 rarities_reverse = {value: key for key, value in rarities.items()}
 
 case_opening = on_command("open", priority=5)
 list_cases = on_command("cases", priority=5)
-radom_case = on_command("random", priority=5)
+# radom_case = on_command("random", priority=5)
 search_skin = on_command("s_skin", priority=5)
 
 
 @list_cases.handle()
 async def handle_list_cases():
     cases_list = cases.get_case_name_list()
     cases_list_str = ""
     for case in cases_list:
         cases_list_str += f"{case}\n"
     await list_cases.finish(f"{cases_list_str}")
 
 
-@radom_case.handle()
-async def handle_random_case():
-    case = cases.get_random_case()
-    await radom_case.send(f"正在开启{case['name']}...")
-    item = cases.open_case(case["id"])
-    skin = skins.get_skins(item["id"])
-    await radom_case.finish(get_skink_message(skin))
+# @radom_case.handle()
+# async def handle_random_case():
+#     case = cases.get_random_case()
+#     await radom_case.send(f"正在开启{case['name']}...")
+#     item = cases.open_case(case["id"])
+#     skin = skins.get_skins(item["id"])
+#     await radom_case.finish(get_skink_message(skin))
 
 
 @case_opening.handle()
 async def handle_open_case(event: MessageEvent, args: Message = CommandArg()):
     arg_list = args.extract_plain_text().split(" ")
     if len(arg_list) > 0:
         if len(arg_list) == 2:
@@ -67,38 +63,39 @@
             case_name = arg_list[1]
         else:
             amount = 1
             case_name = arg_list[0]
 
         case = cases.get_case_by_name(case_name)
         if case:
-            await case_opening.send(MessageSegment.image(case["image"])+f"正在开启{case['name']}...")
+            img_base64 = await utils.url_to_b64(case["image"])
+            await case_opening.send(MessageSegment.image(img_base64)+f"正在开启{case['name']}...")
             items = cases.open_case_multiple(case["id"], amount)
             opened_skins = []
             for item in items:
                 skin = skins.get_skins(item["name"])
                 opened_skins.append(skin)
 
             image = await utils.merge_images(opened_skins)
-
             await case_opening.finish(MessageSegment.image(image))
         else:
             await case_opening.finish("箱子不存在")
     else:
         await case_opening.finish("请输入箱子名称")
 
 
 @search_skin.handle()
 async def handle_search_skin(args: Message = CommandArg()):
     if skin_name := args.extract_plain_text().strip():
         found_skin_list = skins.search_skin(skin_name)
         if len(found_skin_list) == 0:
             await search_skin.finish("没找到捏")
         for skin in found_skin_list:
-            await search_skin.send(MessageSegment.image(skin["image"])+f"找到饰品{skin['name']}")
+            img_base64 = await utils.url_to_b64(skin["image"])
+            await search_skin.send(MessageSegment.image(img_base64)+f"找到饰品{skin['name']}")
     else:
         await search_skin.finish("请输入皮肤名称")
 
 
 def get_skink_message(skin: dict):
     return (MessageSegment.image(skin["image"]) +
             f"""获得 {skin['rarity']}\n{skin['name']}\n磨损度{skin['wear_rating']}""")
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.6/nonebot-plugin-csgo-case-simulator/background2.png` & `nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/background2.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.6/nonebot-plugin-csgo-case-simulator/cases.py` & `nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/cases.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.6/nonebot-plugin-csgo-case-simulator/font/font.ttf` & `nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/font/font.ttf`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.6/nonebot-plugin-csgo-case-simulator/skins.py` & `nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/skins.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.6/nonebot-plugin-csgo-case-simulator/utils.py` & `nonebot-plugin-csgo-case-simulator-0.1.7/nonebot-plugin-csgo-case-simulator/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,7 +110,13 @@
             return img
 
     def img_to_b64(self, pic: Image.Image) -> str:
         buf = BytesIO()
         pic.save(buf, format="PNG")
         base64_str = base64.b64encode(buf.getbuffer()).decode()
         return "base64://" + base64_str
+    
+    async def url_to_b64(self,url:str)->str:
+        async with httpx.AsyncClient() as client:
+            response = await client.get(url)
+            base64_str = base64.b64encode(response.content).decode()
+            return "base64://" + base64_str
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.6/pyproject.toml` & `nonebot-plugin-csgo-case-simulator-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-csgo-case-simulator"
-version = "0.1.6"
+version = "0.1.7"
 description = "a nonebot based csgo case simulator"
 authors = ["Roy <lyt2980999208@gmail.com>"]
 license = "MIT"
 packages = [{ include = "nonebot-plugin-csgo-case-simulator" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.6/setup.py` & `nonebot-plugin-csgo-case-simulator-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['Pillow>=9.5.0,<10.0.0',
  'httpx>=0.24.0,<0.25.0',
  'nonebot-adapter-onebot>=2.2.3,<3.0.0',
  'nonebot2>=2.0.0-rc.4,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-csgo-case-simulator',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'a nonebot based csgo case simulator',
     'long_description': None,
     'author': 'Roy',
     'author_email': 'lyt2980999208@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `nonebot-plugin-csgo-case-simulator-0.1.6/PKG-INFO` & `nonebot-plugin-csgo-case-simulator-0.1.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-csgo-case-simulator
-Version: 0.1.6
+Version: 0.1.7
 Summary: a nonebot based csgo case simulator
 License: MIT
 Author: Roy
 Author-email: lyt2980999208@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

