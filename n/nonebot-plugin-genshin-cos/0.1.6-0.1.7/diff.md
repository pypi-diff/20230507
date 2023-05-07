# Comparing `tmp/nonebot_plugin_genshin_cos-0.1.6.tar.gz` & `tmp/nonebot_plugin_genshin_cos-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_genshin_cos-0.1.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_genshin_cos-0.1.7.tar", max compression
```

## Comparing `nonebot_plugin_genshin_cos-0.1.6.tar` & `nonebot_plugin_genshin_cos-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1085 2023-03-28 09:06:05.557316 nonebot_plugin_genshin_cos-0.1.6/LICENSE
--rw-r--r--   0        0        0     8850 2023-04-27 04:40:34.852336 nonebot_plugin_genshin_cos-0.1.6/nonebot_plugin_genshin_cos/__init__.py
--rw-r--r--   0        0        0      269 2023-04-27 05:00:12.292105 nonebot_plugin_genshin_cos-0.1.6/nonebot_plugin_genshin_cos/config.py
--rw-r--r--   0        0        0   459180 2023-04-08 07:01:06.461588 nonebot_plugin_genshin_cos-0.1.6/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF
--rw-r--r--   0        0        0    11030 2023-04-27 04:58:22.298726 nonebot_plugin_genshin_cos-0.1.6/nonebot_plugin_genshin_cos/utils.py
--rw-r--r--   0        0        0      661 2023-04-27 05:06:50.988254 nonebot_plugin_genshin_cos-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3634 2023-04-27 05:19:54.659437 nonebot_plugin_genshin_cos-0.1.6/README.md
--rw-r--r--   0        0        0     4422 1970-01-01 00:00:00.000000 nonebot_plugin_genshin_cos-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-03-28 09:06:05.557316 nonebot_plugin_genshin_cos-0.1.7/LICENSE
+-rw-r--r--   0        0        0     8860 2023-05-07 00:52:02.221268 nonebot_plugin_genshin_cos-0.1.7/nonebot_plugin_genshin_cos/__init__.py
+-rw-r--r--   0        0        0      269 2023-04-27 05:00:12.292105 nonebot_plugin_genshin_cos-0.1.7/nonebot_plugin_genshin_cos/config.py
+-rw-r--r--   0        0        0   459180 2023-04-08 07:01:06.461588 nonebot_plugin_genshin_cos-0.1.7/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF
+-rw-r--r--   0        0        0    11068 2023-05-07 00:51:33.291947 nonebot_plugin_genshin_cos-0.1.7/nonebot_plugin_genshin_cos/utils.py
+-rw-r--r--   0        0        0      661 2023-05-07 00:52:27.173270 nonebot_plugin_genshin_cos-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3634 2023-04-27 05:19:54.659437 nonebot_plugin_genshin_cos-0.1.7/README.md
+-rw-r--r--   0        0        0     4422 1970-01-01 00:00:00.000000 nonebot_plugin_genshin_cos-0.1.7/PKG-INFO
```

### Comparing `nonebot_plugin_genshin_cos-0.1.6/LICENSE` & `nonebot_plugin_genshin_cos-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshin_cos-0.1.6/nonebot_plugin_genshin_cos/__init__.py` & `nonebot_plugin_genshin_cos-0.1.7/nonebot_plugin_genshin_cos/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     description="获取原神coser图片",
     config=Config,
     usage="原神cos",
     extra={
         "unique_name": "genshin_cos",
         "example": "保存cos:保存cos图片至本地文件",
         "author": "divandia <106718176+Cvandia@users.noreply.github.com>",
-        "version": "0.1.6",
+        "version": "0.1.7",
     },
 )
 logo = """<g>
   /$$$$$$                                /$$       /$$                  /$$$$$$                     
  /$$__  $$                              | $$      |__/                 /$$__  $$                    
 | $$  \__/  /$$$$$$  /$$$$$$$   /$$$$$$$| $$$$$$$  /$$ /$$$$$$$       | $$  \__/  /$$$$$$   /$$$$$$$
 | $$ /$$$$ /$$__  $$| $$__  $$ /$$_____/| $$__  $$| $$| $$__  $$      | $$       /$$__  $$ /$$_____/
@@ -157,18 +157,18 @@
     global user_data
     args = list(state['_matched_groups'])
     img = get_cos()
     out_cd, deletime, user_data = check_cd(event.user_id, user_data)
     if out_cd:
         if not args[2]:
             await send_cos.send("获取图片中…请稍等")
-            if not img.randow_cos_img():
+            if not await img.randow_cos_img():
                 await send_cos.finish("未获取到图片")
             try:
-                await send_cos.send(MessageSegment.image(img.randow_cos_img()))
+                await send_cos.send(MessageSegment.image(await img.randow_cos_img()))
             except ActionFailed:
                 await send_cos.finish("账户风控了,发送不了图片", at_sender=True)
         else:
             num = int(re.sub(r"[x|*|X]", "", args[2]))
             num = num if num <= max else max
             msg_list = ['找到最新的一些cos图如下:']
             imgs = await img.get_img_url()
@@ -203,8 +203,8 @@
     if isinstance(event, GroupMessageEvent):
         return await bot.call_api(
             "send_group_forward_msg", group_id=event.group_id, messages=messages
         )
     else:
         return await bot.call_api(
             "send_private_forward_msg", user_id=event.user_id, messages=messages
-        )
+        )
```

### Comparing `nonebot_plugin_genshin_cos-0.1.6/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF` & `nonebot_plugin_genshin_cos-0.1.7/nonebot_plugin_genshin_cos/fonts/CONSOLA.TTF`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshin_cos-0.1.6/nonebot_plugin_genshin_cos/utils.py` & `nonebot_plugin_genshin_cos-0.1.7/nonebot_plugin_genshin_cos/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,36 @@
-from httpx import AsyncClient
-from nonebot.log import logger
+from datetime import datetime, timedelta
 from pathlib import Path
+from typing import List, Tuple
+
+from httpx import AsyncClient
 from nonebot import get_driver
+from nonebot.log import logger
+from nonebot.log import logger as blog
 from PIL import Image, ImageDraw, ImageFont
-from typing import List, Tuple
+
 from .config import Config
-from datetime import datetime, timedelta
-from nonebot.log import logger as blog
+
 try:
     import ujson as json
 except ImportError:
     import json
-import random
-from playwright.async_api import async_playwright
+
 import io
 import os
-import time
+import random
 import re
+import time
+
+from playwright.async_api import async_playwright
 
 cd = Config.parse_obj(get_driver().config.dict()).cos_cd
-font_path = os.path.join(os.path.dirname(__file__), "fonts")+ "/CONSOLA.TTF"
+font_path = os.path.join(os.path.dirname(__file__), "fonts") + "/CONSOLA.TTF"
+
+
 class WriteError(Exception):
     pass
 
 
 class get_cos(object):
     """获取米游社原神cos最新图片"""
 
@@ -64,80 +71,80 @@
 
     async def get_img_name(self) -> list:
         """获取cos图片名称
 
         Returns:
             list: 图片名称列表
         """
-        data = self.parse()
+        data = await self.parse()
         name_list = []
         for k, v in data.items():
             name_list.append(k)
         return name_list
 
     async def save_img(self, save_path: str):
         """保存cos的图片
 
         Args:
             save_path: 保存的路劲
 
         Returns:
             int: 成功保存的数量
         """
-        data = self.parse()
+        data = await self.parse()
         path = Path(save_path)
         if not str(save_path):
             path = Path("./data/genshin_cos")
         if not path.exists():
             path.mkdir(parents=True)
             logger.warning(f"文件夹不存在，正在创建文件夹:{path}")
         N = 0
         for k, v in data.items():
             N += 1
-            k = re.sub(r'^[\w-+.?？|=*]*', '', k)
+            k = re.sub(r"^[\-\+.?？|=*]*", "", k)
             try:
                 with open(path / f"{k}.jpg", 'wb') as f:
                     img = await AsyncClient().get(
                         v, headers=self.headers)  # 发送请求获取图片内容
                     f.write(img.content)
                     logger.success(f"保存成功 --> {k}")
             except Exception as exc:
                 logger.error(exc)
                 raise WriteError(f"出错了请查看详细报错:\n{exc}")
         return N
 
-    def randow_cos_img(self) -> str:
+    async def randow_cos_img(self) -> str:
         """随机cos图链接
 
         Returns:
             str: 图片url
         """
-        return random.choice(self.get_img_url())
+        return random.choice(await self.get_img_url())
 
     async def download_urls(self, urls: list, names: list, save_path: str) -> int:
         """下载特定的图片链接
 
         Args:
             urls (list): 图片链接
             names (list): 图片对应名称
             save_path (str): 保存的路劲
 
         retrun:
             int: 返回成功保存的数量
         """
         path = Path(save_path)
-        if not str(save_path):
+        if not save_path:
             path = Path("./data/genshin_cos")
         if not path.exists():
             path.mkdir(parents=True)
             logger.warning(f"文件夹不存在，正在创建文件夹:{path}")
         N = 0
         for url, name in zip(urls, names):
             N += 1
-            name = re.sub(r'^[\w-+.?？|=*]*', '', name)
+            name = re.sub(r"^[\-\+.?？|=*]*", "", name)
             try:
                 with open(path / f"{name}.jpg", 'wb') as f:
                     img = await AsyncClient().get(url, headers=self.headers)
                     f.write(img.content)
                     logger.success(f"保存成功 --> {name}")
             except Exception as exc:
                 raise WriteError(exc)
@@ -195,31 +202,31 @@
             await self.page.wait_for_selector('//*[@id="__layout"]/div/div[2]/div/div/div[2]')
             # 滑轮向下滚动seconds秒
             start_time = time.time()
             while (time.time() - start_time < seconds):
                 await self.page.mouse.wheel(delta_y=20, delta_x=0)
                 time.sleep(0.01)
             await self.page.wait_for_timeout(2000)
-            guid_image = await self.page.locator('div.mhy-article-list__body').screenshot(quality=50,type='jpeg')
+            guid_image = await self.page.locator('div.mhy-article-list__body').screenshot(quality=50, type='jpeg')
             self.guid_links = await self.page.query_selector_all('.mhy-img-article-card__header a')
             image = Image.open(io.BytesIO(guid_image))
             draw = ImageDraw.Draw(image)
             for m in range(len(self.guid_links)):
                 x = m % 3  # 0,1,2
                 y = m // 3  # 0,1,2,3,4,5
                 draw.text((x*247, y*247), str(m), fill=(255, 0, 0),
-                        font=ImageFont.truetype(font=font_path, size=100))
+                          font=ImageFont.truetype(font=font_path, size=100))
             byes = io.BytesIO()
             image.save(byes, format="JPEG")
             return byes
         except Exception as exc:
             await self.close()
             raise exc
 
-    async def get_img_or_video(self, location:List[int]) -> Tuple[int, list]:
+    async def get_img_or_video(self, location: List[int]) -> Tuple[int, list]:
         """
         获取图片或视频链接
 
         params
         ----
 
         return
@@ -239,18 +246,18 @@
                     url_list.extend([await pic.get_attribute('large') for pic in pic_images])
                     await new_page.close()
         except Exception as exp:
             await self.close()
             raise exp
         # 获取图片链接
         if pic_images:
-            return 0,url_list
+            return 0, url_list
         # 如果图片不存在则获取获取视频链接
         else:
-            return 1,url_list
+            return 1, url_list
 
     async def get_all_img(self) -> list:
         """
         获取所有图片链接
 
         return
         ----
@@ -295,23 +302,24 @@
         data[str(user_id)] = datetime.now()
     if datetime.now() < data[f'{user_id}']:
         delta = (data[str(user_id)] - datetime.now()).seconds
         return False, delta, data
     else:
         data[str(user_id)] = datetime.now() + timedelta(seconds=cd)
         return True, 0, data
-    
-def log(front:str,behind:str,*args, **kwargs):
+
+
+def log(front: str, behind: str, *args, **kwargs):
     """
     自定义`nonebot2`的log输出
 
     Args:
         front (str): 前面的文字
         behind (str): 后面的文字
-    
+
     Returns:
         log输出，格式为`[front] behind`
     """
     blog.opt(colors=True).info(f"<u><y>[{front}]</y></u>{behind}")
 
 ##############################################################################################################
 # 别看了，这里能有啥？
```

### Comparing `nonebot_plugin_genshin_cos-0.1.6/pyproject.toml` & `nonebot_plugin_genshin_cos-0.1.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-genshin-cos"
-version = "0.1.6"
+version = "0.1.7"
 description = "米游社原神cos图获取"
 authors = ["Cvandia <106718176+Cvandia@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_genshin_cos"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_genshin_cos-0.1.6/README.md` & `nonebot_plugin_genshin_cos-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_genshin_cos-0.1.6/PKG-INFO` & `nonebot_plugin_genshin_cos-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-genshin-cos
-Version: 0.1.6
+Version: 0.1.7
 Summary: 米游社原神cos图获取
 License: MIT
 Author: Cvandia
 Author-email: 106718176+Cvandia@users.noreply.github.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-genshin-cos Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-genshin-cos Version: 0.1.7 Summary:
 ç±³æ¸¸ç¤¾åç¥coså¾è·å License: MIT Author: Cvandia Author-email:
 106718176+Cvandia@users.noreply.github.com Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=0.7.0) Requires-Dist: httpx (>=0.19.0) Requires-
```

