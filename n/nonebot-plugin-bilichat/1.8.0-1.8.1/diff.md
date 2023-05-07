# Comparing `tmp/nonebot_plugin_bilichat-1.8.0.tar.gz` & `tmp/nonebot_plugin_bilichat-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-1.8.0.tar", last modified: Fri Apr 28 16:13:20 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-1.8.1.tar", last modified: Sun May  7 17:18:19 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-1.8.0.tar` & `nonebot_plugin_bilichat-1.8.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    34523 2023-04-28 16:13:07.264203 nonebot_plugin_bilichat-1.8.0/LICENSE
--rw-r--r--   0        0        0    11854 2023-04-28 16:13:07.264203 nonebot_plugin_bilichat-1.8.0/README.md
--rw-r--r--   0        0        0     6000 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4809 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6439 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      399 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-04-28 16:13:07.272203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1045 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     5825 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2343 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1068 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/utils.py
--rw-r--r--   0        0        0     1780 2023-04-28 16:13:07.276203 nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1407 2023-04-28 16:13:20.916168 nonebot_plugin_bilichat-1.8.0/pyproject.toml
--rw-r--r--   0        0        0    13143 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-05-07 17:18:04.896358 nonebot_plugin_bilichat-1.8.1/LICENSE
+-rw-r--r--   0        0        0    11854 2023-05-07 17:18:04.896358 nonebot_plugin_bilichat-1.8.1/README.md
+-rw-r--r--   0        0        0     5837 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4809 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6439 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      399 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-05-07 17:18:04.904358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-05-07 17:18:04.908358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1045 2023-05-07 17:18:04.908358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     5825 2023-05-07 17:18:04.908358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-05-07 17:18:04.908358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2343 2023-05-07 17:18:04.908358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-05-07 17:18:04.908358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     2268 2023-05-07 17:18:04.908358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/utils.py
+-rw-r--r--   0        0        0     1780 2023-05-07 17:18:04.908358 nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1407 2023-05-07 17:18:19.236206 nonebot_plugin_bilichat-1.8.1/pyproject.toml
+-rw-r--r--   0        0        0    13143 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.8.1/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-1.8.0/LICENSE` & `nonebot_plugin_bilichat-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/README.md` & `nonebot_plugin_bilichat-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import re
 import shlex
 from itertools import chain
-from typing import Union, cast
+from typing import cast
 
 from nonebot.adapters import MessageSegment
-from nonebot.adapters.onebot.v11 import Bot as V11_Bot
 from nonebot.adapters.onebot.v11 import GroupMessageEvent as V11_GME
-from nonebot.adapters.onebot.v11 import MessageEvent as V11_ME
 from nonebot.adapters.onebot.v11 import PrivateMessageEvent as V11_PME
-from nonebot.adapters.onebot.v12 import Bot as V12_Bot
 from nonebot.adapters.onebot.v12 import GroupMessageEvent as V12_GME
-from nonebot.adapters.onebot.v12 import MessageEvent as V12_ME
 from nonebot.adapters.onebot.v12 import PrivateMessageEvent as V12_PME
 from nonebot.consts import REGEX_GROUP, REGEX_STR
 from nonebot.exception import FinishedException
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.params import Depends
 from nonebot.plugin import PluginMetadata, on_regex
@@ -23,15 +19,15 @@
 
 from .config import __version__, plugin_config
 from .lib.b23_extract import b23_extract
 from .lib.content_resolve import get_column_basic, get_content_cache, get_video_basic
 from .model.arguments import Options, parser
 from .model.exception import AbortError
 from .optional import capture_exception  # type: ignore
-from .utils import get_image, get_reply
+from .utils import BOT, MESSAGE_EVENT, get_image, get_reply
 
 if plugin_config.bilichat_openai_token or plugin_config.bilichat_newbing_cookie:
     ENABLE_SUMMARY = True
     from .summary import summarization
 else:
     ENABLE_SUMMARY = False
 
@@ -48,15 +44,15 @@
         "author": "djkcyl & Well404",
         "version": __version__,
         "priority": 1,
     },
 )
 
 
-async def _bili_check(bot: Union[V11_Bot, V12_Bot], event: Union[V11_ME, V12_ME], state: T_State):
+async def _bili_check(bot: BOT, event: MESSAGE_EVENT, state: T_State):
     if str(event.get_user_id()) == str(bot.self_id):
         return plugin_config.bilichat_enable_self
     elif isinstance(event, (V11_PME, V12_PME)):
         state["_uid_"] = event.user_id
         return plugin_config.bilichat_enable_private
     elif isinstance(event, (V11_GME, V12_GME)):
         state["_uid_"] = event.group_id
@@ -80,15 +76,15 @@
     r"b23.(tv|wtf)[\\/]+(\w+)",
     block=plugin_config.bilichat_block,
     priority=1,
     rule=Rule(_bili_check),
 )
 
 
-def get_args(event: Union[V11_ME, V12_ME]):
+def get_args(event: MESSAGE_EVENT):
     return parser.parse_known_args(
         list(
             chain.from_iterable(
                 shlex.split(str(seg)) if cast(MessageSegment, seg).is_text() else (seg,) for seg in event.get_message()
             )
         ),  # type: ignore
         namespace=Options(),
@@ -98,25 +94,29 @@
 @bili.handle()
 async def get_bili_number_re(state: T_State):
     state["bili_number"] = state[REGEX_STR]
 
 
 @b23.handle()
 async def get_bili_number_b23(state: T_State):
+    bililink = await b23_extract(state[REGEX_GROUP])
     if matched := re.search(
-        r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})|cv(\d{1,16})", await b23_extract(state[REGEX_GROUP])  # type: ignore
+        r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})|cv(\d{1,16})", bililink  # type: ignore
     ):
         state["bili_number"] = matched.group()
+    else:
+        logger.info(f"{bililink} is not video or column")
+        raise FinishedException
 
 
 @bili.handle()
 @b23.handle()
 async def video_info(
-    bot: Union[V11_Bot, V12_Bot],
-    event: Union[V11_ME, V12_ME],
+    bot: BOT,
+    event: MESSAGE_EVENT,
     state: T_State,
     matcher: Matcher,
     options: Options = Depends(get_args),
 ):
     reply = await get_reply(event)
     # basic info
     bili_number, uid = state["bili_number"], state["_uid_"]
```

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-1.8.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.8.0/pyproject.toml` & `nonebot_plugin_bilichat-1.8.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "1.8.0"
+version = "1.8.1"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
```

### Comparing `nonebot_plugin_bilichat-1.8.0/PKG-INFO` & `nonebot_plugin_bilichat-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 1.8.0
+Version: 1.8.1
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.8.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.8.1 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
 Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra" Requires-Dist:
```

