# Comparing `tmp/hikari_bot-0.3.8.1.tar.gz` & `tmp/hikari_bot-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_bot-0.3.8.1.tar", max compression
+gzip compressed data, was "hikari_bot-0.3.9.tar", max compression
```

## Comparing `hikari_bot-0.3.8.1.tar` & `hikari_bot-0.3.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1084 2022-05-26 18:22:32.043723 hikari_bot-0.3.8.1/LICENSE
--rw-r--r--   0        0        0     1531 2023-04-26 12:52:08.193863 hikari_bot-0.3.8.1/pyproject.toml
--rw-r--r--   0        0        0    26005 2023-04-14 08:32:32.990647 hikari_bot-0.3.8.1/README.md
--rw-r--r--   0        0        0    13663 2023-04-26 12:51:48.315823 hikari_bot-0.3.8.1/src/plugins/hikari_bot/__init__.py
--rw-r--r--   0        0        0     3147 2023-04-08 18:23:09.590414 hikari_bot-0.3.8.1/src/plugins/hikari_bot/command_select.py
--rw-r--r--   0        0        0    12100 2023-04-03 20:34:11.614042 hikari_bot-0.3.8.1/src/plugins/hikari_bot/data_source.py
--rw-r--r--   0        0        0     3956 2023-04-08 18:23:09.591425 hikari_bot-0.3.8.1/src/plugins/hikari_bot/game/ban_search.py
--rw-r--r--   0        0        0     4098 2023-02-20 07:47:11.425737 hikari_bot-0.3.8.1/src/plugins/hikari_bot/game/box_check.py
--rw-r--r--   0        0        0     3574 2023-03-01 07:15:08.148850 hikari_bot-0.3.8.1/src/plugins/hikari_bot/game/ocr.py
--rw-r--r--   0        0        0      798 2023-02-20 07:47:11.427209 hikari_bot-0.3.8.1/src/plugins/hikari_bot/game/pupu.py
--rw-r--r--   0        0        0     2302 2023-02-20 07:47:11.427209 hikari_bot-0.3.8.1/src/plugins/hikari_bot/game/roll.py
--rw-r--r--   0        0        0     4085 2023-02-20 07:47:11.428271 hikari_bot-0.3.8.1/src/plugins/hikari_bot/game/sx.py
--rw-r--r--   0        0        0     3334 2023-02-20 07:47:11.429266 hikari_bot-0.3.8.1/src/plugins/hikari_bot/mqtt.py
--rw-r--r--   0        0        0     9092 2023-04-03 20:34:11.615043 hikari_bot-0.3.8.1/src/plugins/hikari_bot/publicAPI.py
--rw-r--r--   0        0        0   173077 2023-04-26 12:50:29.054661 hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/Chart.min.js
--rw-r--r--   0        0        0    13279 2023-04-26 12:50:29.006715 hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/chartjs-plugin-datalabels@1.0.0.js
--rw-r--r--   0        0        0     3710 2023-04-26 12:50:29.023346 hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/select-ship.html
--rw-r--r--   0        0        0     5109 2023-04-26 12:50:29.020328 hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/ship-rank.html
--rw-r--r--   0        0        0      225 2023-04-26 12:50:29.021326 hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/text-help.css
--rw-r--r--   0        0        0     7284 2023-04-26 12:50:29.015783 hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-ban.html
--rw-r--r--   0        0        0    16757 2023-04-26 12:50:29.034971 hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-box-christmas.html
--rw-r--r--   0        0        0    18454 2023-04-26 12:50:29.040015 hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-clan.html
--rw-r--r--   0        0        0    23627 2023-04-26 12:50:29.010745 hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-info-recent.html
--rw-r--r--   0        0        0    25496 2023-04-26 12:50:29.039009 hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-info.html
--rw-r--r--   0        0        0     2396 2023-04-26 12:50:29.025368 hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-personalRecord.html
--rw-r--r--   0        0        0     6301 2022-09-02 06:25:22.613704 hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-realTime.html
--rw-r--r--   0        0        0    21658 2023-04-26 12:50:29.024350 hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-ship-recent.html
--rw-r--r--   0        0        0    20751 2023-04-26 12:50:29.052651 hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-ship.html
--rw-r--r--   0        0        0     9446 2023-04-26 12:50:29.011751 hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-sx.html
--rw-r--r--   0        0        0     5784 2023-04-26 12:50:29.013763 hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-unban.html
--rw-r--r--   0        0        0     3084 2023-02-20 07:47:11.431310 hikari_bot-0.3.8.1/src/plugins/hikari_bot/utils.py
--rw-r--r--   0        0        0    13665 2023-04-26 12:48:00.125481 hikari_bot-0.3.8.1/src/plugins/hikari_bot/wws_bind.py
--rw-r--r--   0        0        0     6390 2023-04-26 12:51:11.166963 hikari_bot-0.3.8.1/src/plugins/hikari_bot/wws_clan.py
--rw-r--r--   0        0        0     4303 2023-04-26 12:47:05.903980 hikari_bot-0.3.8.1/src/plugins/hikari_bot/wws_info.py
--rw-r--r--   0        0        0     3663 2023-02-20 07:47:11.434332 hikari_bot-0.3.8.1/src/plugins/hikari_bot/wws_realTime.py
--rw-r--r--   0        0        0     5269 2023-04-26 12:46:50.805409 hikari_bot-0.3.8.1/src/plugins/hikari_bot/wws_recent.py
--rw-r--r--   0        0        0    10118 2023-02-20 07:47:11.436344 hikari_bot-0.3.8.1/src/plugins/hikari_bot/wws_record.py
--rw-r--r--   0        0        0    17498 2023-04-26 12:51:32.608006 hikari_bot-0.3.8.1/src/plugins/hikari_bot/wws_ship.py
--rw-r--r--   0        0        0     9515 2023-04-26 12:51:39.101171 hikari_bot-0.3.8.1/src/plugins/hikari_bot/wws_shiprank.py
--rw-r--r--   0        0        0    38826 1970-01-01 00:00:00.000000 hikari_bot-0.3.8.1/setup.py
--rw-r--r--   0        0        0    26666 1970-01-01 00:00:00.000000 hikari_bot-0.3.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-05-26 18:22:32.043723 hikari_bot-0.3.9/LICENSE
+-rw-r--r--   0        0        0     1527 2023-05-07 05:01:54.090915 hikari_bot-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0    26078 2023-05-07 05:02:48.526232 hikari_bot-0.3.9/README.md
+-rw-r--r--   0        0        0    13484 2023-05-07 05:02:02.140074 hikari_bot-0.3.9/src/plugins/hikari_bot/__init__.py
+-rw-r--r--   0        0        0     3203 2023-05-06 07:16:22.601839 hikari_bot-0.3.9/src/plugins/hikari_bot/command_select.py
+-rw-r--r--   0        0        0    12164 2023-05-06 07:13:44.481628 hikari_bot-0.3.9/src/plugins/hikari_bot/data_source.py
+-rw-r--r--   0        0        0     3726 2023-05-06 07:56:32.594072 hikari_bot-0.3.9/src/plugins/hikari_bot/game/ban_search.py
+-rw-r--r--   0        0        0     3752 2023-05-06 07:57:33.212108 hikari_bot-0.3.9/src/plugins/hikari_bot/game/box_check.py
+-rw-r--r--   0        0        0     3137 2023-05-06 08:18:04.267056 hikari_bot-0.3.9/src/plugins/hikari_bot/game/ocr.py
+-rw-r--r--   0        0        0      811 2023-05-06 08:03:25.972231 hikari_bot-0.3.9/src/plugins/hikari_bot/game/pupu.py
+-rw-r--r--   0        0        0     2302 2023-02-20 07:47:11.427209 hikari_bot-0.3.9/src/plugins/hikari_bot/game/roll.py
+-rw-r--r--   0        0        0     3739 2023-05-06 08:04:56.505548 hikari_bot-0.3.9/src/plugins/hikari_bot/game/sx.py
+-rw-r--r--   0        0        0      882 2023-05-06 08:05:36.794049 hikari_bot-0.3.9/src/plugins/hikari_bot/HttpClient_pool.py
+-rw-r--r--   0        0        0     7446 2023-05-06 07:31:00.349608 hikari_bot-0.3.9/src/plugins/hikari_bot/moudle/publicAPI.py
+-rw-r--r--   0        0        0    12004 2023-05-06 07:55:01.396408 hikari_bot-0.3.9/src/plugins/hikari_bot/moudle/wws_bind.py
+-rw-r--r--   0        0        0     6155 2023-05-06 07:55:07.049323 hikari_bot-0.3.9/src/plugins/hikari_bot/moudle/wws_clan.py
+-rw-r--r--   0        0        0     3928 2023-05-06 07:44:16.265070 hikari_bot-0.3.9/src/plugins/hikari_bot/moudle/wws_info.py
+-rw-r--r--   0        0        0     3769 2023-05-06 07:37:32.342013 hikari_bot-0.3.9/src/plugins/hikari_bot/moudle/wws_realTime.py
+-rw-r--r--   0        0        0     4923 2023-05-06 07:38:53.480353 hikari_bot-0.3.9/src/plugins/hikari_bot/moudle/wws_recent.py
+-rw-r--r--   0        0        0     9775 2023-05-06 07:55:13.603058 hikari_bot-0.3.9/src/plugins/hikari_bot/moudle/wws_record.py
+-rw-r--r--   0        0        0    16544 2023-05-06 07:49:48.702392 hikari_bot-0.3.9/src/plugins/hikari_bot/moudle/wws_ship.py
+-rw-r--r--   0        0        0     8141 2023-05-06 07:55:18.162016 hikari_bot-0.3.9/src/plugins/hikari_bot/moudle/wws_shiprank.py
+-rw-r--r--   0        0        0   173077 2023-05-06 20:00:04.998177 hikari_bot-0.3.9/src/plugins/hikari_bot/template/Chart.min.js
+-rw-r--r--   0        0        0    13279 2023-05-06 20:00:04.974415 hikari_bot-0.3.9/src/plugins/hikari_bot/template/chartjs-plugin-datalabels@1.0.0.js
+-rw-r--r--   0        0        0     3710 2023-05-06 20:00:04.970402 hikari_bot-0.3.9/src/plugins/hikari_bot/template/select-ship.html
+-rw-r--r--   0        0        0     5109 2023-05-06 20:00:04.939544 hikari_bot-0.3.9/src/plugins/hikari_bot/template/ship-rank.html
+-rw-r--r--   0        0        0      225 2023-05-06 20:00:04.950173 hikari_bot-0.3.9/src/plugins/hikari_bot/template/text-help.css
+-rw-r--r--   0        0        0     7284 2023-05-06 20:00:04.964839 hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-ban.html
+-rw-r--r--   0        0        0    16757 2023-05-06 20:00:04.962820 hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-box-christmas.html
+-rw-r--r--   0        0        0    18454 2023-05-06 20:00:04.952166 hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-clan.html
+-rw-r--r--   0        0        0    23627 2023-05-06 20:00:04.948141 hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-info-recent.html
+-rw-r--r--   0        0        0    25496 2023-05-06 20:00:04.986010 hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-info.html
+-rw-r--r--   0        0        0     2396 2023-05-06 20:00:04.972408 hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-personalRecord.html
+-rw-r--r--   0        0        0     6301 2022-09-02 06:25:22.613704 hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-realTime.html
+-rw-r--r--   0        0        0    21658 2023-05-06 20:00:04.967857 hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-ship-recent.html
+-rw-r--r--   0        0        0    20751 2023-05-06 20:00:04.985494 hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-ship.html
+-rw-r--r--   0        0        0     9446 2023-05-06 20:00:04.971398 hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-sx.html
+-rw-r--r--   0        0        0     5784 2023-05-06 20:00:04.973418 hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-unban.html
+-rw-r--r--   0        0        0     3084 2023-02-20 07:47:11.431310 hikari_bot-0.3.9/src/plugins/hikari_bot/utils.py
+-rw-r--r--   0        0        0    38916 1970-01-01 00:00:00.000000 hikari_bot-0.3.9/setup.py
+-rw-r--r--   0        0        0    26731 1970-01-01 00:00:00.000000 hikari_bot-0.3.9/PKG-INFO
```

### Comparing `hikari_bot-0.3.8.1/LICENSE` & `hikari_bot-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.8.1/pyproject.toml` & `hikari_bot-0.3.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hikari-bot"
-version = "0.3.8.1"
+version = "0.3.9"
 description = "Nonebot2 HikariBot,支持战舰世界水表查询"
 authors = ["benx1n <shirakamikanade@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/benx1n/HikariBot"
 repository = "https://github.com/benx1n/HikariBot"
 keywords = ["nonebot", "nonebot2", "qqbot", "wows", "wws","bot","stats"]
@@ -19,15 +19,15 @@
 nonebot-plugin-htmlrender = "^0.2.0.1"
 nonebot-plugin-apscheduler = "^0.2.0"
 nonebot_plugin_guild_patch = "^0.2.1"
 nonebot-plugin-reboot = "^0.1.3"
 httpx = ">=0.20.0"
 Jinja2 = "^3.0.0"
 beautifulsoup4 = "^4.11.1"
-paho-mqtt = "^1.6.1"
+orjson = "^3.8.11"
 
 [tool.poetry.group.dev.dependencies]
 nb-cli = "^0.6.0"
 nonebot-plugin-gocqhttp = "^0.6.2"
 black = {version = "^23.1a1", allow-prereleases = true}
 isort = "^5.12.0"
```

### Comparing `hikari_bot-0.3.8.1/README.md` & `hikari_bot-0.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -263,14 +263,18 @@
     - 如果没有更新到最新版请等待一会儿，镜像站一般每五分钟同步
     - 从0.3.2.2版本开始，您没有填写的配置将按.env文件中的默认配置执行，具体逻辑为
       - 私聊、频道默认禁用
       - 群聊默认开启，默认屏蔽官方交流群
 
 ## 最近的更新日志
 
+### 23-05-07    v0.3.9
+- [+]重构代码
+- [#]替换默认OCR接口
+
 ### 23-04-07    v0.3.8
 - [+]新增国服封号记录查询，指令wws ban/wws 封号记录
 - [#]修复了上次修复排行榜新产生的bug
 
 ### 23-04-04    v0.3.7
 - [+]添加获取随机表情包，指令wws 随机表情包
 - [+]更新船只选择界面
```

#### html2text {}

```diff
@@ -164,17 +164,18 @@
 installç»æåä¼æå°å½åçæ¬ - æ¨ä¹å¯ä»¥éè¿`pip show hikari-
 bot`æ¥çå½åHikariçæ¬ -
 å¦ææ²¡ææ´æ°å°ææ°çè¯·ç­å¾ä¸ä¼å¿ï¼éåç«ä¸è¬æ¯äºåéåæ­¥
 -
 ä»0.3.2.2çæ¬å¼å§ï¼æ¨æ²¡æå¡«åçéç½®å°æ.envæä»¶ä¸­çé»è®¤éç½®æ§è¡ï¼å·ä½é»è¾ä¸º
 - ç§èãé¢éé»è®¤ç¦ç¨ -
 ç¾¤èé»è®¤å¼å¯ï¼é»è®¤å±è½å®æ¹äº¤æµç¾¤ ## æè¿çæ´æ°æ¥å¿ ###
-23-04-07 v0.3.8 - [+]æ°å¢å½æå°å·è®°å½æ¥è¯¢ï¼æä»¤wws ban/wws
-å°å·è®°å½ - [#]ä¿®å¤äºä¸æ¬¡ä¿®å¤æè¡æ¦æ°äº§ççbug ### 23-04-04
-v0.3.7 - [+]æ·»å è·åéæºè¡¨æåï¼æä»¤wws éæºè¡¨æå -
+23-05-07 v0.3.9 - [+]éæä»£ç  - [#]æ¿æ¢é»è®¤OCRæ¥å£ ### 23-04-07
+v0.3.8 - [+]æ°å¢å½æå°å·è®°å½æ¥è¯¢ï¼æä»¤wws ban/wws å°å·è®°å½ -
+[#]ä¿®å¤äºä¸æ¬¡ä¿®å¤æè¡æ¦æ°äº§ççbug ### 23-04-04 v0.3.7 -
+[+]æ·»å è·åéæºè¡¨æåï¼æä»¤wws éæºè¡¨æå -
 [+]æ´æ°è¹åªéæ©çé¢ - [#]æ´æ°Linuxèæ¬æç®¡ ### 23-02-22 v0.3.6.4
 - [+]æ·»å éæºå´è­ï¼æ¦çååä¹ä¸ - [+]æ·»å ocrå¯å¨æ¥éæç¤º -
 [#]ä¿®å¤ä¸é®ååDockerä¾èµé®é¢ [@94Bo](https://github.com/94Bo)
 [@12hydrogen](https://github.com/12hydrogen) ### 22-11-18 v0.3.6
 åå«éç½®é¡¹æ´æ°ï¼è¯·æ·»å `env.prod-example`ä¸­æ°å¢çéç½® -
 [+]æ°å¢ååï¼å·²äº0.3.5.2å®è£ï¼ -
 [+]æ°å¢OCRï¼å·²äº0.3.5.5å®è£ï¼ -
```

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/__init__.py` & `hikari_bot-0.3.9/src/plugins/hikari_bot/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import asyncio
 import html
-import json
 import os
 import platform
 import random
 import re
 import sys
 import traceback
-from pathlib import Path
 
 import httpx
+import orjson
 from loguru import logger
 from nonebot import get_driver, on_command, on_fullmatch, on_message, require
 from nonebot.adapters.onebot.v11 import (
     ActionFailed,
     Bot,
     GroupMessageEvent,
     Message,
@@ -24,32 +23,30 @@
 from nonebot.log import logger
 from nonebot.params import CommandArg
 from nonebot.permission import SUPERUSER
 from nonebot_plugin_guild_patch import GuildMessageEvent
 from nonebot_plugin_htmlrender import text_to_pic
 
 from .command_select import select_command
-from .data_source import nb2_file
+from .data_source import nb2_file, template_path
 from .game.ocr import downlod_OcrResult, pic2txt_byOCR, upload_OcrResult
 from .game.pupu import get_pupu_msg
-from .mqtt import mqtt_run
+from .HttpClient_pool import client_default, client_yuyuko
+from .moudle.wws_clan import ClanSecletProcess
+from .moudle.wws_ship import ShipSecletProcess
 from .utils import DailyNumberLimiter, FreqLimiter, download, get_bot
-from .wws_clan import ClanSecletProcess
-from .wws_ship import ShipSecletProcess
 
 scheduler = require("nonebot_plugin_apscheduler").scheduler
 
 _max = 100
 EXCEED_NOTICE = f"您今天已经冲过{_max}次了，请明早5点后再来！"
 is_first_run = True
 _nlmt = DailyNumberLimiter(_max)
 _flmt = FreqLimiter(3)
-__version__ = "0.3.8.1"
-dir_path = Path(__file__).parent
-template_path = dir_path / "template"
+__version__ = "0.3.9"
 
 bot = on_command("wws", block=False, aliases={"WWS"}, priority=54)
 bot_pupu = on_fullmatch("噗噗", block=False, priority=5)
 bot_checkversion = on_command("wws 检查更新", priority=5, block=False)
 bot_update = on_command("wws 更新Hikari", priority=5, block=False, permission=SUPERUSER)
 bot_listen = on_message(priority=5, block=False)
 ocr_listen = on_message(priority=6, block=False)
@@ -131,22 +128,20 @@
         logger.error(traceback.format_exc())
         await bot.send(ev, "呜呜呜发生了错误，可能是网络问题，如果过段时间不能恢复请联系麻麻哦~")
 
 
 async def send_bot_help():
     try:
         url = "https://benx1n.oss-cn-beijing.aliyuncs.com/version.json"
-        async with httpx.AsyncClient() as client:
-            resp = await client.get(url, timeout=10)
-            result = json.loads(resp.text)
+        resp = await client_default.get(url, timeout=10)
+        result = orjson.loads(resp.text)
         latest_version = result["latest_version"]
         url = "https://benx1n.oss-cn-beijing.aliyuncs.com/wws_help.txt"
-        async with httpx.AsyncClient() as client:
-            resp = await client.get(url, timeout=10)
-            result = resp.text
+        resp = await client_default.get(url, timeout=10)
+        result = resp.text
         result = f"""帮助列表                                                当前版本{__version__}  最新版本{latest_version}\n{result}"""
         img = await text_to_pic(
             text=result, css_path=str(template_path / "text-help.css"), width=800
         )
         return img
     except Exception:
         logger.warning(traceback.format_exc())
@@ -253,17 +248,16 @@
 
 
 @bot_checkversion.handle()
 async def check_version():
     try:
         bot = get_bot()
         url = "https://benx1n.oss-cn-beijing.aliyuncs.com/version.json"
-        async with httpx.AsyncClient() as client:
-            resp = await client.get(url, timeout=10)
-            result = json.loads(resp.text)
+        resp = await client_default.get(url, timeout=10)
+        result = orjson.loads(resp.text)
         superid = driver.config.superusers
         match, msg = False, f"发现新版本"
         for each in result["data"]:
             if each["version"] > __version__:
                 match = True
                 msg += f"\n{each['date']} v{each['version']}\n"
                 for i in each["description"]:
@@ -295,15 +289,15 @@
 async def startup():
     try:
         tasks = []
         loop = asyncio.get_running_loop()
         url = "https://benx1n.oss-cn-beijing.aliyuncs.com/template_Hikari_Latest/template.json"
         async with httpx.AsyncClient() as client:
             resp = await client.get(url, timeout=20)
-            result = resp.json()
+            result = orjson.loads(resp.content)
             for each in result:
                 for name, url in each.items():
                     tasks.append(asyncio.ensure_future(startup_download(url, name)))
         await asyncio.gather(*tasks)
         if driver.config.ocr_on:
             await downlod_OcrResult()
     except Exception:
@@ -323,15 +317,15 @@
     # if is_first_run:
     #    mqtt_run(bot_info['user_id'])
     #    is_first_run = False
 
 
 async def startup_download(url, name):
     async with httpx.AsyncClient() as client:
-        resp = resp = await client.get(url, timeout=20)
+        resp = await client.get(url, timeout=20)
         with open(template_path / name, "wb+") as file:
             file.write(resp.content)
 
 
 scheduler.add_job(
     check_version,
     "cron",
```

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/command_select.py` & `hikari_bot-0.3.9/src/plugins/hikari_bot/command_select.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from dataclasses import dataclass
 from typing import Protocol, Tuple
 
+from .game.ban_search import get_BanInfo
 from .game.box_check import check_christmas_box
 from .game.ocr import get_Random_Ocr_Pic
 from .game.roll import roll_ship
 from .game.sx import get_sx_info
-from .game.ban_search import get_BanInfo
-from .publicAPI import get_ship_name
-from .wws_bind import (
+from .moudle.publicAPI import get_ship_name
+from .moudle.wws_bind import (
     change_BindInfo,
     delete_BindInfo,
     get_BindInfo,
     set_BindInfo,
     set_special_BindInfo,
 )
-from .wws_clan import get_ClanInfo
-from .wws_info import get_AccountInfo
-from .wws_recent import get_RecentInfo
-from .wws_record import get_record
-from .wws_ship import get_ShipInfo, get_ShipInfoRecent
-from .wws_shiprank import get_ShipRank
+from .moudle.wws_clan import get_ClanInfo
+from .moudle.wws_info import get_AccountInfo
+from .moudle.wws_recent import get_RecentInfo
+from .moudle.wws_record import get_record
+from .moudle.wws_ship import get_ShipInfo, get_ShipInfoRecent
+from .moudle.wws_shiprank import get_ShipRank
 
 
 class Func(Protocol):
     async def __call__(self, **kwargs):
         ...
```

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/data_source.py` & `hikari_bot-0.3.9/src/plugins/hikari_bot/data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import re
 import traceback
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Tuple
 
+from nonebot import get_driver
+
 dir_path = Path(__file__).parent
 template_path = dir_path / "template"
+config = get_driver().config
 
 
 @dataclass
 class matching:
     keywords: Tuple[str, ...]
     match_keywords: str
```

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/game/ban_search.py` & `hikari_bot-0.3.9/src/plugins/hikari_bot/game/ban_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,28 @@
 import re
-import time
 import traceback
 from asyncio.exceptions import TimeoutError
-from pathlib import Path
 from typing import List
 
-import httpx
 import jinja2
+import orjson
 from httpx import ConnectTimeout
-from nonebot import get_driver
 from nonebot.log import logger
 from nonebot_plugin_htmlrender import html_to_pic
 
-from ..data_source import servers
-from ..publicAPI import  get_AccountIdByName
+from ..data_source import servers, template_path
+from ..HttpClient_pool import client_yuyuko
+from ..moudle.publicAPI import get_AccountIdByName
+from ..moudle.wws_bind import get_DefaultBindInfo
 from ..utils import match_keywords
-from ..wws_bind import get_DefaultBindInfo
 
-dir_path = Path(__file__).parent.parent
-template_path = dir_path / "template"
 env = jinja2.Environment(
     loader=jinja2.FileSystemLoader(template_path), enable_async=True
 )
 
-headers = {"Authorization": get_driver().config.api_token}
-
-
 async def get_BanInfo(server_type, info, bot, ev):
     try:
         url, params = "", ""
         if isinstance(info, List):
             for i in info:
                 if str(i).lower() == "me":
                     params = {"server": server_type, "accountId": int(ev.user_id)}
@@ -58,19 +51,17 @@
                 else:
                     return "目前仅支持国服查询"
             else:
                 return "您似乎准备用游戏昵称查询，请检查参数中是否包含服务器和游戏昵称，以空格区分"
         else:
             return "参数似乎出了问题呢"
         url = 'https://api.wows.shinoaki.com/public/wows/ban/cn/user'
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.post(url, json={"accountId":param_accountid}, timeout=None)
-            result = resp.json()
-            logger.success(f"本次请求返回的状态码:{result['code']}")
-            logger.success(f"本次请求服务器计算时间:{result['queryTime']}")
+        resp = await client_yuyuko.post(url, json={"accountId":param_accountid}, timeout=None)
+        result = orjson.loads(resp.content)
+        logger.success(f"本次请求总耗时{resp.elapsed.total_seconds()*1000}，服务器计算耗时:{result['queryTime']}")
         if result["code"] == 200 and result["data"]:
             template = env.get_template("wws-ban.html")
             template_data = {"data": result["data"]}
             content = await template.render_async(template_data)
             return await html_to_pic(
                 content, wait=0, viewport={"width": 900, "height": 100}
             )
```

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/game/box_check.py` & `hikari_bot-0.3.9/src/plugins/hikari_bot/game/sx.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 import re
 import time
 import traceback
 from asyncio.exceptions import TimeoutError
-from pathlib import Path
 from typing import List
 
-import httpx
 import jinja2
+import orjson
 from httpx import ConnectTimeout
 from nonebot import get_driver
 from nonebot.log import logger
 from nonebot_plugin_htmlrender import html_to_pic
 
 from ..data_source import (
     servers,
     set_damageColor,
     set_infoparams,
     set_upinfo_color,
     set_winColor,
+    template_path,
 )
-from ..publicAPI import get_AccountIdByName
+from ..HttpClient_pool import client_yuyuko
+from ..moudle.publicAPI import get_AccountIdByName
 from ..utils import match_keywords
 
-dir_path = Path(__file__).parent.parent
-template_path = dir_path / "template"
 env = jinja2.Environment(
     loader=jinja2.FileSystemLoader(template_path), enable_async=True
 )
 env.globals.update(
     set_damageColor=set_damageColor,
     set_winColor=set_winColor,
     set_upinfo_color=set_upinfo_color,
     time=time,
     int=int,
     abs=abs,
     enumerate=enumerate,
 )
 
-headers = {"Authorization": get_driver().config.api_token}
-
-
-async def check_christmas_box(server_type, info, bot, ev):
+async def get_sx_info(server_type, info, bot, ev):
     try:
         url, params = "", ""
         if isinstance(info, List):
             if len(info) == 0:
                 params = {"server": "QQ", "accountId": int(ev.user_id)}
             for i in info:
                 if str(i).lower() == "me":
@@ -68,23 +64,20 @@
                     return "服务器参数似乎输错了呢"
             elif params:
                 logger.success(f"{params}")
             else:
                 return "您似乎准备用游戏昵称查询，请检查参数中是否包含服务器和游戏昵称，以空格区分，如果您准备查询单船战绩，请带上ship参数"
         else:
             return "参数似乎出了问题呢"
-        url = "https://api.wows.shinoaki.com/public/wows/christmas/ship/box"
-        logger.success(f"下面是本次请求的参数，如果遇到了问题，请将这部分连同报错日志一起发送给麻麻哦\n{url}\n{params}")
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            result = resp.json()
-            logger.success(f"本次请求返回的状态码:{result['code']}")
-            logger.success(f"本次请求服务器计算时间:{result['queryTime']}")
+        url = "https://api.wows.shinoaki.com/public/wows/christmas/ship/christmas"
+        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        result = orjson.loads(resp.content)
+        logger.success(f"本次请求总耗时{resp.elapsed.total_seconds()*1000}，服务器计算耗时:{result['queryTime']}")
         if result["code"] == 200 and result["data"]:
-            template = env.get_template("wws-box-christmas.html")
+            template = env.get_template("wws-sx.html")
             template_data = await set_infoparams(result["data"])
             content = await template.render_async(template_data)
             return await html_to_pic(
                 content, wait=0, viewport={"width": 920, "height": 1000}
             )
         elif result["code"] == 403:
             return f"{result['message']}\n请先绑定账号"
```

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/game/ocr.py` & `hikari_bot-0.3.9/src/plugins/hikari_bot/game/ocr.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,98 +1,87 @@
-import json
 import time
 import traceback
 from base64 import b64decode, b64encode
 from pathlib import Path
 
-import httpx
-from nonebot import get_driver
+import orjson
 from nonebot.log import logger
 
-config = get_driver().config
+from ..data_source import config
+from ..HttpClient_pool import client_default, client_yuyuko
+
 ocr_url = config.ocr_url
 dir_path = Path(__file__).parent.parent
 game_path = Path(__file__).parent
 ocr_data_path = game_path / "ocr_data.json"
 upload_url = "https://api.wows.shinoaki.com/api/wows/cache/image/ocr"
 download_url = "https://api.wows.shinoaki.com/api/wows/cache/image/ocr"
 
-headers = {"Authorization": config.api_token}
-
-
 async def pic2txt_byOCR(img_path, filename):
     try:
         global ocr_filename_data
         if filename in ocr_filename_data:
             logger.success(f"filename匹配，跳过OCR:{filename}")
             return b64decode(ocr_filename_data[filename]).decode("utf-8")
         if config.ocr_offline:
             return ""
-        async with httpx.AsyncClient() as client:
-            # logger.success(f"图片地址{img_path}")
-            # resp = await client.get(img_path)
-            # img_base64 = str(b64encode(resp.content),encoding='utf-8')
-            start = time.time()
-            # params = {
-            #    "image":img_base64
-            # }
-            params = {"url": img_path}
-            resp = await client.post(
-                ocr_url, data=params, timeout=5, follow_redirects=True
-            )
+        start = time.time()
+        params = {"url": img_path}
+        resp = await client_default.post(
+            f"{ocr_url}/OCR/", data=params, timeout=5, follow_redirects=True
+        )
         end = time.time()
-        logger.success(f"OCR结果：{resp.text},耗时{end-start:.4f}s\n图片url:{img_path}")
-        return resp.text
+        result = orjson.loads(resp.content)
+        if result['code'] == 200:
+            logger.success(f"OCR结果：{result['data']['msg']},耗时{end-start:.4f}s\n图片url:{img_path}")
+            return result['data']['msg']
     except:
         logger.error(traceback.format_exc())
         return ""
 
 
 async def upload_OcrResult(result_text, filename):
     try:
         params = {
             "md5": filename,
             "text": b64encode(result_text.encode("utf-8")).decode("utf-8"),
         }
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.post(upload_url, json=params)
-            result = resp.json()
+        resp = await client_yuyuko.post(upload_url, json=params)
+        result = orjson.loads(resp.content)
         if result["code"] == 200:
             await downlod_OcrResult()
     except:
         logger.error(traceback.format_exc())
 
 
 async def downlod_OcrResult():
     try:
         global ocr_filename_data
-        async with httpx.AsyncClient(headers=headers, timeout=None) as client:
-            resp = await client.get(download_url)
-            result = resp.json()
-            with open(ocr_data_path, "w", encoding="UTF-8") as f:
-                if result["code"] == 200 and result["data"]:
-                    json.dump(result["data"], f)
-                    ocr_filename_data = result["data"]
-                else:
-                    ocr_filename_data = json.load(
-                        open(ocr_data_path, "r", encoding="utf8")
-                    )
+        resp = await client_yuyuko.get(download_url)
+        result = orjson.loads(resp.content)
+        with open(ocr_data_path, "w", encoding="UTF-8") as f:
+            if result["code"] == 200 and result["data"]:
+                f.write(orjson.dumps(result['data']).decode())
+                ocr_filename_data = result["data"]
+            else:
+                with open(ocr_data_path, "rb") as f:    
+                    ocr_filename_data = orjson.loads(f.read())
         return
     except:
         logger.error("请检查token是否配置正确，如无问题请尝试重启，可能是网络波动或服务器原因")
         logger.error(traceback.format_exc())
         try:
-            ocr_filename_data = json.load(open(ocr_data_path, "r", encoding="utf8"))
+            with open(ocr_data_path, "rb") as f:    
+                ocr_filename_data = orjson.loads(f.read())
         except:
             ocr_filename_data = None
 
 
 async def get_Random_Ocr_Pic(server_type, info, bot, ev):
     try:
-        async with httpx.AsyncClient(headers=headers, timeout=None) as client:
-            resp = await client.post('http://mc.youthnp.cn:23338/ImageRandom/')
-            img = b64decode(resp.text)
+        resp = await client_default.post(f"{ocr_url}/ImageRandom/")
+        img = b64decode(resp.text)
         return img
     except:
         logger.error(traceback.format_exc())  
         return 'OCR服务器出了点问题，请稍后再试哦'
```

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/game/pupu.py` & `hikari_bot-0.3.9/src/plugins/hikari_bot/game/pupu.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import traceback
 from asyncio.exceptions import TimeoutError
 from pathlib import Path
 
-import httpx
+import orjson
 from httpx import ConnectTimeout
 from nonebot.log import logger
 
+from ..HttpClient_pool import client_default
+
 dir_path = Path(__file__).parent
 
 
 async def get_pupu_msg():
     try:
         url = "https://v1.hitokoto.cn"
         params = {}
-        async with httpx.AsyncClient() as client:
-            resp = await client.get(url, params=params, timeout=5)
-            result = resp.json()
+        resp = await client_default.get(url, params=params, timeout=5)
+        result = orjson.loads(resp.content)
         if resp.status_code == 200:
             return result["hitokoto"]
         else:
             return "噗噗出问题了>_<"
     except (TimeoutError, ConnectTimeout):
         logger.warning(traceback.format_exc())
     except Exception:
```

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/game/roll.py` & `hikari_bot-0.3.9/src/plugins/hikari_bot/game/roll.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/game/sx.py` & `hikari_bot-0.3.9/src/plugins/hikari_bot/game/box_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 import re
 import time
 import traceback
 from asyncio.exceptions import TimeoutError
-from pathlib import Path
 from typing import List
 
-import httpx
 import jinja2
+import orjson
 from httpx import ConnectTimeout
 from nonebot import get_driver
 from nonebot.log import logger
 from nonebot_plugin_htmlrender import html_to_pic
 
 from ..data_source import (
     servers,
     set_damageColor,
     set_infoparams,
     set_upinfo_color,
     set_winColor,
+    template_path,
 )
-from ..publicAPI import get_AccountIdByName
+from ..HttpClient_pool import client_yuyuko
+from ..moudle.publicAPI import get_AccountIdByName
 from ..utils import match_keywords
 
-dir_path = Path(__file__).parent.parent
-template_path = dir_path / "template"
 env = jinja2.Environment(
     loader=jinja2.FileSystemLoader(template_path), enable_async=True
 )
 env.globals.update(
     set_damageColor=set_damageColor,
     set_winColor=set_winColor,
     set_upinfo_color=set_upinfo_color,
     time=time,
     int=int,
     abs=abs,
     enumerate=enumerate,
 )
 
-headers = {"Authorization": get_driver().config.api_token}
-
-
-async def get_sx_info(server_type, info, bot, ev):
+async def check_christmas_box(server_type, info, bot, ev):
     try:
         url, params = "", ""
         if isinstance(info, List):
             if len(info) == 0:
                 params = {"server": "QQ", "accountId": int(ev.user_id)}
             for i in info:
                 if str(i).lower() == "me":
@@ -68,23 +64,20 @@
                     return "服务器参数似乎输错了呢"
             elif params:
                 logger.success(f"{params}")
             else:
                 return "您似乎准备用游戏昵称查询，请检查参数中是否包含服务器和游戏昵称，以空格区分，如果您准备查询单船战绩，请带上ship参数"
         else:
             return "参数似乎出了问题呢"
-        url = "https://api.wows.shinoaki.com/public/wows/christmas/ship/christmas"
-        logger.success(f"下面是本次请求的参数，如果遇到了问题，请将这部分连同报错日志一起发送给麻麻哦\n{url}\n{params}")
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            result = resp.json()
-            logger.success(f"本次请求返回的状态码:{result['code']}")
-            logger.success(f"本次请求服务器计算时间:{result['queryTime']}")
+        url = "https://api.wows.shinoaki.com/public/wows/christmas/ship/box"
+        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        result = orjson.loads(resp.content)
+        logger.success(f"本次请求总耗时{resp.elapsed.total_seconds()*1000}，服务器计算耗时:{result['queryTime']}")
         if result["code"] == 200 and result["data"]:
-            template = env.get_template("wws-sx.html")
+            template = env.get_template("wws-box-christmas.html")
             template_data = await set_infoparams(result["data"])
             content = await template.render_async(template_data)
             return await html_to_pic(
                 content, wait=0, viewport={"width": 920, "height": 1000}
             )
         elif result["code"] == 403:
             return f"{result['message']}\n请先绑定账号"
```

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/publicAPI.py` & `hikari_bot-0.3.9/src/plugins/hikari_bot/moudle/wws_record.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,218 +1,225 @@
-import asyncio
-import gzip
-import json
+import re
+import time
 import traceback
-from asyncio.exceptions import TimeoutError
-from base64 import b64encode
+from pathlib import Path
 from typing import List
 
 import httpx
-from httpx import ConnectTimeout
+import jinja2
+import orjson
+from bs4 import BeautifulSoup
 from nonebot import get_driver
-from nonebot.log import logger
+from nonebot_plugin_htmlrender import html_to_pic
 
-from .data_source import levels, nations, shiptypes
-from .utils import match_keywords
+from ..data_source import servers, template_path
+from ..HttpClient_pool import client_default, client_yuyuko
+from ..utils import match_keywords
+from .publicAPI import get_AccountIdByName
+
+env = jinja2.Environment(
+    loader=jinja2.FileSystemLoader(template_path), enable_async=True
+)
 
-headers = {"Authorization": get_driver().config.api_token}
-if get_driver().config.proxy_on:
-    proxy = {"https://": get_driver().config.proxy}
-else:
-    proxy = {}
 
 
-async def get_nation_list():
-    try:
-        msg = ""
-        url = "https://api.wows.shinoaki.com/public/wows/encyclopedia/nation/list"
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, timeout=None)
-            result = resp.json()
-        for nation in result["data"]:
-            msg: str = msg + f"{nation['cn']}：{nation['nation']}\n"
-        return msg
-    except Exception:
-        logger.error(traceback.format_exc())
-
-
-async def get_ship_name(server_type, infolist: List, bot, ev):
-    msg = ""
-    try:
-        param_nation, infolist = await match_keywords(infolist, nations)
-        if not param_nation:
-            return "请检查国家名是否正确"
-
-        param_shiptype, infolist = await match_keywords(infolist, shiptypes)
-        if not param_shiptype:
-            return "请检查船只类别是否正确"
-
-        param_level, infolist = await match_keywords(infolist, levels)
-        if not param_level:
-            return "请检查船只等级是否正确"
-        params = {
-            "county": param_nation,
-            "level": param_level,
-            "shipName": "",
-            "shipType": param_shiptype,
-        }
-        url = "https://api.wows.shinoaki.com/public/wows/encyclopedia/ship/search"
-        logger.success(f"下面是本次请求的参数，如果遇到了问题，请将这部分连同报错日志一起发送给麻麻哦\n{url}\n{params}")
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            logger.success(f"本次请求返回的状态码:{resp.status_code}")
-            result = resp.json()
-        if result["data"]:
-            for ship in result["data"]:
-                msg += f"{ship['shipNameCn']}：{ship['shipNameNumbers']}\n"
+async def get_record(server_type, info, bot, ev):
+    try:
+        params = None
+        if isinstance(info, List):
+            for i in info:
+                if i == "me":
+                    params = {"server": server_type, "accountId": int(ev.user_id)}
+                    break
+                match = re.search(r"CQ:at,qq=(\d+)", i)
+                if match:
+                    params = {"server": server_type, "accountId": int(match.group(1))}
+                    break
+            if not params and len(info) == 2:
+                param_server, info = await match_keywords(info, servers)
+                if param_server and param_server != "cn":
+                    param_accountid = await get_AccountIdByName(
+                        param_server, str(info[0])
+                    )
+                    if isinstance(param_accountid, int):
+                        params = {"server": param_server, "accountId": param_accountid}
+                    else:
+                        return f"{param_accountid}"
+                elif param_server == "cn":
+                    return "暂不支持国服"
+                else:
+                    return "服务器参数似乎输错了呢"
+            elif params:
+                pass
+            else:
+                return (
+                    "您似乎准备用游戏昵称查询公会进出记录，请检查参数中时候包含服务器和游戏昵称，以空格区分，如果您准备查询单船战绩，请带上ship参数"
+                )
         else:
-            msg = "没有符合的船只"
-        return msg
-    except (TimeoutError, ConnectTimeout):
-        logger.warning(traceback.format_exc())
-    except Exception:
-        logger.error(traceback.format_exc())
-        return "wuwuwu出了点问题，请联系麻麻解决"
-
-
-async def get_ship_byName(shipname: str):
-    try:
-        url = "https://api.wows.shinoaki.com/public/wows/encyclopedia/ship/search"
-        params = {"county": "", "level": "", "shipName": shipname, "shipType": ""}
-        logger.success(f"下面是本次请求的参数，如果遇到了问题，请将这部分连同报错日志一起发送给麻麻哦\n{url}\n{params}")
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            logger.success(f"本次请求返回的状态码:{resp.status_code}")
-            result = resp.json()
-        List = []
-        if result["code"] == 200 and result["data"]:
-            for each in result["data"]:
-                List.append(
-                    [
-                        each["id"],
-                        each["shipNameCn"],
-                        each["shipNameNumbers"],
-                        each["tier"],
-                        each['shipType']
-                    ]
+            return "参数似乎出了问题呢"
+        print(params)
+        if type == "personal":
+            url = "https://api.wows.shinoaki.com/upload/numbers/data/upload/user/clan/record"
+            resp = await client_yuyuko.get(url, params=params, timeout=None)
+            result = orjson.loads(resp.content)
+            if result["code"] == 200 and result["data"]:
+                template = env.get_template("wws-personalRecord.html")
+                template_data = {"data": result["data"]}
+                content = await template.render_async(template_data)
+                return await html_to_pic(
+                    content, wait=0, viewport={"width": 920, "height": 100}
+                )
+            elif result["code"] == 403:
+                return f"{result['message']}\n请检查昵称或绑定账号"
+            elif result["code"] == 404:
+                template = env.get_template("wws-personalRecord.html")
+                template_data = await get_personalRecord_Numbers(
+                    result["data"][0]["httpUrl"], params
+                )
+                print(template_data)
+                if template_data:
+                    template_data = {"data": template_data}
+                else:
+                    return "查询失败了呢，可能是没有进出记录"
+                content = await template.render_async(template_data)
+                return await html_to_pic(
+                    content, wait=0, viewport={"width": 920, "height": 100}
                 )
-            return List
+            elif result["code"] == 500:
+                return f"{result['message']}\n这是服务器问题，请联系雨季麻麻"
+            else:
+                return f"{result['message']}"
         else:
-            return None
-    except (TimeoutError, ConnectTimeout):
-        logger.warning(traceback.format_exc())
+            url = ""
+            resp = await client_yuyuko.get(url, params=params, timeout=None)
+            result = orjson.loads(resp.content)
+            if result["code"] == 200 and result["data"]:
+                template = env.get_template("wws-clanRecord.html")
+                template_data = {"data": result["data"]}
+                content = await template.render_async(template_data)
+                return await html_to_pic(
+                    content, wait=0, viewport={"width": 920, "height": 100}
+                )
+            elif result["code"] == 403:
+                return f"{result['message']}\n请检查昵称或绑定账号"
+            elif result["code"] == 404:
+                template = env.get_template("wws-clanRecord.html")
+                template_data = await get_ClanRecord_Numbers(
+                    result["data"][0]["httpUrl"], params["server"], params["accountId"]
+                )
+                print(template_data)
+                if template_data:
+                    template_data = {"data": template_data}
+                else:
+                    return "查询失败了呢，可能是没有进出记录"
+                content = await template.render_async(template_data)
+                return await html_to_pic(
+                    content, wait=0, viewport={"width": 920, "height": 100}
+                )
+            elif result["code"] == 500:
+                return f"{result['message']}\n这是服务器问题，请联系雨季麻麻"
+            else:
+                return f"{result['message']}"
+
     except Exception:
-        logger.error(traceback.format_exc())
-        return None
+        traceback.print_exc()
+        return "wuwuwu出了点问题，请联系麻麻解决，目前不支持国服哦"
 
 
-async def get_all_shipList():
+async def get_personalRecord_Numbers(url, server, accountId):
     try:
-        url = "https://api.wows.shinoaki.com/public/wows/encyclopedia/ship/search"
-        params = {"county": "", "level": "", "shipName": "", "shipType": ""}
+        data = None
         async with httpx.AsyncClient() as client:
-            resp = await client.get(url, params=params, timeout=None)
-            result = resp.json()
-        if result["code"] == 200 and result["data"]:
-            return result["data"]
-        else:
-            return None
+            resp = await client.get(url, timeout=None)
+            soup = BeautifulSoup(resp.content, "html.parser")
+            data = soup.select(f'table[id="moreTransfers"]')
+            if data:
+                data = data.select(f"tr")
+            else:
+                data = soup.select(
+                    f'table[class="table table-styled table-bordered cells-middle"]'
+                )
+                data = data[len(data) - 1].select(f"tr")
+            info, info_list, clan_list = {}, [], []
+            for each in data:
+                class_list = each.select("td span")[0].attrs["class"]
+                if class_list[2] == "transfer-out":
+                    status = 1
+                else:
+                    status = 0
+                timeGroup = re.match(
+                    r"(.*?)\.(.*?)\.(.*?)$", each.select("td")[1].string
+                )
+                dt = f"{timeGroup.group(3)}-{timeGroup.group(2)}-{timeGroup.group(1)} 12:00:00"
+                timestamp = int(time.mktime(time.strptime(dt, r"%Y-%m-%d %H:%M:%S")))
+                clanId = re.match(
+                    r"\/clan\/(.*?),", each.select("td a")[0].attrs["href"]
+                ).group(1)
+                clanName = each.select("td a")[0].string
+                info["server"] = server
+                info["accountId"] = accountId
+                info["clanId"] = int(clanId)
+                info["status"] = status
+                info["time"] = timestamp
+                info["clanName"] = clanName
+                if clanId not in clan_list:
+                    clan_list.append(clanId)
+                info_list.append(info.copy())
+            print(clan_list)
+            clan_url = re.match(r"(.*?)player", url).group(1)
+            for each in clan_list:
+                await get_ClanRecord_Numbers(
+                    f"{clan_url}clan/transfers/{each},111/", each
+                )
+            # result = await post_personalRecord_yuyuko(info_list)
+            # if result:
+            #    return result
+            # else:
+            #    return None
     except Exception:
+        traceback.print_exc()
         return None
 
 
-async def get_AccountIdByName(server: str, name: str):
-    try:
-        url = "https://api.wows.shinoaki.com/public/wows/account/search/user"
-        params = {"server": server, "userName": name}
-        logger.success(f"下面是本次请求的参数，如果遇到了问题，请将这部分连同报错日志一起发送给麻麻哦\n{url}\n{params}")
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            logger.success(f"本次请求返回的状态码:{resp.status_code}")
-            result = resp.json()
-        if result["code"] == 200 and result["data"]:
-            return result["data"]["accountId"]
-        else:
-            return result["message"]
-    except (TimeoutError, ConnectTimeout):
-        logger.warning(traceback.format_exc())
-        return "请求超时了，请过一会儿重试哦~"
-    except Exception:
-        logger.error(traceback.format_exc())
-        return "好像出了点问题呢，可能是网络问题，如果重试几次还不行的话，请联系麻麻解决"
-
-
-async def get_ClanIdByName(server: str, tag: str):
-    try:
-        url = "https://api.wows.shinoaki.com/public/wows/clan/search"
-        params = {"server": server, "tag": tag, "type": 1}
-        print(f"下面是本次请求的参数，如果遇到了问题，请将这部分连同报错日志一起发送给麻麻哦\n{params}")
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            result = resp.json()
-        List = []
+async def get_ClanRecord_Numbers(url, clanId):
+    async with httpx.AsyncClient() as client:
+        resp = await client.get(url, timeout=None)
+        soup = BeautifulSoup(resp.content, "html.parser")
+        data = soup.select(f"tr")
+        info, info_list = {}, []
+        for each_data in data[2:]:
+            class_list = each_data.select("td span")[0].attrs["class"]
+            if class_list[2] == "transfer-out":
+                status = 1
+            else:
+                status = 0
+            timeGroup = re.match(
+                r"(.*?)\.(.*?)\.(.*?)$", each_data.select("td")[1].string
+            )
+            dt = f"{timeGroup.group(3)}-{timeGroup.group(2)}-{timeGroup.group(1)} 12:00:00"
+            timestamp = int(time.mktime(time.strptime(dt, r"%Y-%m-%d %H:%M:%S")))
+            accountMacthGroup = re.match(
+                r"\/player\/(.*?),(.*?)\/", each_data.select("td a")[0].attrs["href"]
+            )
+            if accountMacthGroup:
+                accountId = accountMacthGroup.group(1)
+                accountName = accountMacthGroup.group(2)
+            info["clanId"] = clanId
+            info["status"] = status
+            info["time"] = timestamp
+            info["accountId"] = accountId
+            info["accountName"] = accountName
+            info_list.append(info.copy())
+
+
+async def post_personalRecord_yuyuko(post_data):
+    try:
+        url = "https://api.wows.shinoaki.com/upload/numbers/data/upload/user/clan/record"
+        resp = await client_yuyuko.post(url, json=post_data, timeout=None)
+        result = orjson.loads(resp.content)
         if result["code"] == 200 and result["data"]:
-            # for each in result['data']:
-            #    List.append([each['clanId'],each['name'],each['serverName'],each['tag']])
             return result["data"]
         else:
             return None
     except Exception:
-        logger.error(traceback.format_exc())
+        traceback.print_exc()
         return None
-
-
-async def check_yuyuko_cache(server, id):
-    try:
-        if get_driver().config.check_cache:
-            yuyuko_cache_url = "https://api.wows.shinoaki.com/api/wows/cache/check"
-            params = {"accountId": id, "server": server}
-            print(f"下面是本次请求的参数，如果遇到了问题，请将这部分连同报错日志一起发送给麻麻哦\n{params}")
-            async with httpx.AsyncClient(headers=headers) as client:
-                resp = await client.post(yuyuko_cache_url, json=params, timeout=5)
-                result = resp.json()
-            cache_data = {}
-            if result["code"] == 201:
-                if "DEV" in result["data"]:
-                    await get_wg_info(cache_data, "DEV", result["data"]["DEV"])
-                elif "pvp" in result["data"]:
-                    tasks = []
-                    loop = asyncio.get_running_loop()
-                    for key in result["data"]:
-                        tasks.append(
-                            asyncio.ensure_future(
-                                get_wg_info(cache_data, key, result["data"][key])
-                            )
-                        )
-                    await asyncio.gather(*tasks)
-                if not cache_data:
-                    return False
-                data_base64 = b64encode(
-                    gzip.compress(json.dumps(cache_data).encode("utf-8"))
-                ).decode()
-                params["data"] = data_base64
-                async with httpx.AsyncClient(headers=headers) as client:
-                    resp = await client.post(yuyuko_cache_url, json=params, timeout=5)
-                    result = resp.json()
-                    logger.success(result)
-                if result["code"] == 200:
-                    return True
-                else:
-                    return False
-            return False
-        return False
-    except Exception:
-        logger.error(traceback.format_exc())
-        return False
-
-
-async def get_wg_info(params, key, url):
-    try:
-        async with httpx.AsyncClient(headers=headers, proxies=proxy) as client:
-            resp = await client.get(url, timeout=5, follow_redirects=True)
-            wg_result = resp.json()
-        if resp.status_code == 200 and wg_result["status"] == "ok":
-            params[key] = resp.text
-    except Exception:
-        logger.error(traceback.format_exc())
-        logger.error(f"上报url：{url}")
-        return
```

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/Chart.min.js` & `hikari_bot-0.3.9/src/plugins/hikari_bot/template/Chart.min.js`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/chartjs-plugin-datalabels@1.0.0.js` & `hikari_bot-0.3.9/src/plugins/hikari_bot/template/chartjs-plugin-datalabels@1.0.0.js`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/select-ship.html` & `hikari_bot-0.3.9/src/plugins/hikari_bot/template/select-ship.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/ship-rank.html` & `hikari_bot-0.3.9/src/plugins/hikari_bot/template/ship-rank.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-ban.html` & `hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-ban.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-box-christmas.html` & `hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-box-christmas.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-clan.html` & `hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-clan.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-info-recent.html` & `hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-info-recent.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-info.html` & `hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-info.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-personalRecord.html` & `hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-personalRecord.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-realTime.html` & `hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-realTime.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-ship-recent.html` & `hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-ship-recent.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-ship.html` & `hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-ship.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-sx.html` & `hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-sx.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/template/wws-unban.html` & `hikari_bot-0.3.9/src/plugins/hikari_bot/template/wws-unban.html`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/utils.py` & `hikari_bot-0.3.9/src/plugins/hikari_bot/utils.py`

 * *Files identical despite different names*

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/wws_bind.py` & `hikari_bot-0.3.9/src/plugins/hikari_bot/moudle/wws_bind.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import re
 import traceback
 from asyncio.exceptions import TimeoutError
 from typing import List
 
-import httpx
+import orjson
 from httpx import ConnectTimeout
-from nonebot import get_driver
+from nonebot.adapters.onebot.v11 import ActionFailed, Bot, MessageSegment
 from nonebot.log import logger
-from nonebot.adapters.onebot.v11 import ActionFailed, MessageSegment,Bot
 
-from .data_source import servers
+from ..data_source import servers
+from ..HttpClient_pool import client_yuyuko
+from ..utils import match_keywords
 from .publicAPI import get_AccountIdByName
-from .utils import match_keywords
-
-headers = {"Authorization": get_driver().config.api_token}
 
 
 async def get_BindInfo(server_type, info, bot:Bot, ev):
     try:
         url, params = "", ""
         if isinstance(info, List) and len(info) == 1:
             for i in info:  # 是否包含me或@
@@ -35,19 +33,16 @@
                         "platformId": match.group(1),
                     }
                     break
             if not url or not params:
                 return "参数似乎出了问题呢，请使用me或@群友"
         else:
             return "参数似乎出了问题呢，请使用me或@群友"
-        logger.success(f"下面是本次请求的参数，如果遇到了问题，请将这部分连同报错日志一起发送给麻麻哦\n{url}\n{params}")
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            result = resp.json()
-            logger.success(f"本次请求返回的状态码:{result['code']}")
+        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        result = orjson.loads(resp.content)
         if result["code"] == 200 and result["message"] == "success":
             if result["data"]:
                 msg1 = f"当前绑定账号\n"
                 msg2 = f"绑定账号列表\n"
                 flag = 1
                 for bindinfo in result["data"]:
                     msg2 += f"{flag}：{bindinfo['serverType']} {bindinfo['userName']}\n"
@@ -91,19 +86,16 @@
                         return f"{param_accountid}"
                 else:
                     return "服务器参数似乎输错了呢"
             else:
                 return "参数似乎输错了呢，请确保后面跟随服务器+游戏昵称"
         else:
             return "参数似乎输错了呢，请确保后面跟随服务器+游戏昵称"
-        logger.success(f"下面是本次请求的参数，如果遇到了问题，请将这部分连同报错日志一起发送给麻麻哦\n{url}\n{params}")
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            result = resp.json()
-            logger.success(f"本次请求返回的状态码:{result['code']}")
+        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        result = orjson.loads(resp.content)
         if result["code"] == 200 and result["message"] == "success":
             return "绑定成功"
         elif result["code"] == 500:
             return f"{result['message']}\n这是服务器问题，请联系雨季麻麻"
         else:
             return f"{result['message']}"
     except (TimeoutError, ConnectTimeout):
@@ -120,19 +112,16 @@
             url = "https://api.wows.shinoaki.com/public/wows/bind/account/platform/bind/list"
             params = {
                 "platformType": server_type,
                 "platformId": ev.user_id,
             }
         else:
             return "参数似乎出了问题呢，请跟随要切换的序号"
-        logger.success(f"下面是本次请求的参数，如果遇到了问题，请将这部分连同报错日志一起发送给麻麻哦\n{url}\n{params}")
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            result = resp.json()
-            logger.success(f"本次请求返回的状态码:{result['code']}")
+        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        result = orjson.loads(resp.content)
         if result["code"] == 200 and result["message"] == "success":
             if result["data"] and len(result["data"]) >= int(info[0]):
                 account_name = result["data"][int(info[0]) - 1]["userName"]
                 param_server = result["data"][int(info[0]) - 1]["serverType"]
                 param_accountid = result["data"][int(info[0]) - 1]["accountId"]
                 url = "https://api.wows.shinoaki.com/api/wows/bind/account/platform/bind/put"
                 params = {
@@ -142,17 +131,16 @@
                 }
             else:
                 return "没有对应序号的绑定记录"
         elif result["code"] == 500:
             return f"{result['message']}\n这是服务器问题，请联系雨季麻麻"
         else:
             return f"{result['message']}"
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            result = resp.json()
+        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        result = orjson.loads(resp.content)
         if result["code"] == 200 and result["message"] == "success":
             return f"切换绑定成功,当前绑定账号{param_server}：{account_name}"
         elif result["code"] == 403:
             return f"{result['message']}\n请先绑定账号"
         elif result["code"] == 500:
             return f"{result['message']}\n这是服务器问题，请联系雨季麻麻"
         else:
@@ -183,19 +171,16 @@
                         return "特殊绑定只能使用网页查询到的AccountID哦"
                 else:
                     return "服务器参数似乎输错了呢"
             else:
                 return "参数似乎输错了呢，请确保后面跟随服务器+网页查询到的AccountID"
         else:
             return "参数似乎输错了呢，请确保后面跟随服务器+游戏昵称"
-        logger.success(f"下面是本次请求的参数，如果遇到了问题，请将这部分连同报错日志一起发送给麻麻哦\n{url}\n{params}")
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            result = resp.json()
-            logger.success(f"本次请求返回的状态码:{result['code']}")
+        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        result = orjson.loads(resp.content)
         if result["code"] == 200 and result["message"] == "success":
             return "绑定成功"
         elif result["code"] == 500:
             return f"{result['message']}\n这是服务器问题，请联系雨季麻麻"
         else:
             return f"{result['message']}"
     except (TimeoutError, ConnectTimeout):
@@ -212,17 +197,16 @@
             url = "https://api.wows.shinoaki.com/public/wows/bind/account/platform/bind/list"
             params = {
                 "platformType": server_type,
                 "platformId": ev.user_id,
             }
         else:
             return "参数似乎出了问题呢，请跟随要切换的序号"
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            result = resp.json()
+        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        result = orjson.loads(resp.content)
         if result["code"] == 200 and result["message"] == "success":
             if result["data"] and len(result["data"]) >= int(info[0]):
                 account_name = result["data"][int(info[0]) - 1]["userName"]
                 param_server = result["data"][int(info[0]) - 1]["serverType"]
                 param_accountid = result["data"][int(info[0]) - 1]["accountId"]
                 url = "https://api.wows.shinoaki.com/api/wows/bind/account/platform/bind/remove"
                 params = {
@@ -232,19 +216,16 @@
                 }
             else:
                 return "没有对应序号的绑定记录"
         elif result["code"] == 500:
             return f"{result['message']}\n这是服务器问题，请联系雨季麻麻"
         else:
             return f"{result['message']}"
-        logger.success(f"下面是本次请求的参数，如果遇到了问题，请将这部分连同报错日志一起发送给麻麻哦\n{url}\n{params}")
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            result = resp.json()
-            logger.success(f"本次请求返回的状态码:{result['code']}")
+        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        result = orjson.loads(resp.content)
         if result["code"] == 200 and result["message"] == "success":
             return f"删除绑定成功,删除的账号为{param_server}：{account_name}"
         elif result["code"] == 500:
             return f"{result['message']}\n这是服务器问题，请联系雨季麻麻"
         else:
             return f"{result['message']}"
     except (TimeoutError, ConnectTimeout):
@@ -258,17 +239,16 @@
 async def get_DefaultBindInfo(platformType,platformId):
     try:
         url = 'https://api.wows.shinoaki.com/public/wows/bind/account/platform/bind/list'
         params = {
             "platformType": platformType,
             "platformId": platformId,
         }
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            result = resp.json()
+        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        result = orjson.loads(resp.content)
         if result['code'] == 200 and result['message'] == "success":
             if result['data']:
                 for each in result['data']:
                     if each['defaultId']:
                         return each
             else:
                 return None
```

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/wws_clan.py` & `hikari_bot-0.3.9/src/plugins/hikari_bot/moudle/wws_clan.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 import asyncio
 import re
 import traceback
 from asyncio.exceptions import TimeoutError
 from collections import defaultdict, namedtuple
-from pathlib import Path
 from typing import List
 
 import httpx
 import jinja2
 from httpx import ConnectTimeout
 from nonebot import get_driver
-from nonebot.adapters.onebot.v11 import ActionFailed, MessageSegment,Bot
+from nonebot.adapters.onebot.v11 import ActionFailed, Bot, MessageSegment
 from nonebot.log import logger
 from nonebot_plugin_htmlrender import text_to_pic
 
-from .data_source import servers
+from ..data_source import servers, template_path
+from ..utils import match_keywords
 from .publicAPI import get_ClanIdByName
-from .utils import  match_keywords
 
-dir_path = Path(__file__).parent
-template_path = dir_path / "template"
 env = jinja2.Environment(
     loader=jinja2.FileSystemLoader(template_path), enable_async=True
 )
 
 headers = {"Authorization": get_driver().config.api_token}
 
 ClanSlectState = namedtuple("ClanSlectState", ["state", "SlectIndex", "SelectList"])
@@ -104,15 +101,14 @@
                         return "发生了错误，有可能是网络波动，请稍后再试"
                 else:
                     return "服务器参数似乎输错了呢"
             else:
                 return "您似乎准备用军团名查询军团详情，请检查参数中是否包含服务器、军团名，以空格区分"
         else:
             return "参数似乎出了问题呢"
-        logger.success(f"下面是本次请求的参数，如果遇到了问题，请将这部分连同报错日志一起发送给麻麻哦\n{params}")
         async with httpx.AsyncClient(headers=headers) as client:
             resp = await client.get(url, params=params, timeout=20)
             result = resp.json()
         if result["code"] == 200 and result["data"]:
             template = env.get_template("wws-clan.html")
             # template_data = await set_clanparams(result['data'])
             # content = await template.render_async(template_data)
```

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/wws_info.py` & `hikari_bot-0.3.9/src/plugins/hikari_bot/moudle/wws_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,45 @@
 import re
 import time
 import traceback
 from asyncio.exceptions import TimeoutError
-from pathlib import Path
 from typing import List
 
-import httpx
 import jinja2
+import orjson
 from httpx import ConnectTimeout
-from nonebot import get_driver
+from nonebot.adapters.onebot.v11 import ActionFailed, Bot, MessageSegment
 from nonebot.log import logger
-from nonebot.adapters.onebot.v11 import ActionFailed, MessageSegment,Bot
 from nonebot_plugin_htmlrender import html_to_pic
 
-from .data_source import (
+from ..data_source import (
     servers,
     set_damageColor,
     set_infoparams,
     set_upinfo_color,
     set_winColor,
+    template_path,
 )
+from ..HttpClient_pool import client_yuyuko
+from ..utils import match_keywords
 from .publicAPI import check_yuyuko_cache, get_AccountIdByName
-from .utils import match_keywords
 
-dir_path = Path(__file__).parent
-template_path = dir_path / "template"
 env = jinja2.Environment(
     loader=jinja2.FileSystemLoader(template_path), enable_async=True
 )
 env.globals.update(
     set_damageColor=set_damageColor,
     set_winColor=set_winColor,
     set_upinfo_color=set_upinfo_color,
     time=time,
     int=int,
     abs=abs,
     enumerate=enumerate,
 )
 
-headers = {"Authorization": get_driver().config.api_token}
-
-
 async def get_AccountInfo(server_type, info, bot:Bot, ev):
     try:
         url, params = "", ""
         if isinstance(info, List):
             for i in info:
                 if str(i).lower() == "me":
                     params = {"server": server_type, "accountId": int(ev.user_id)}
@@ -73,20 +68,17 @@
             return "参数似乎出了问题呢"
         is_cache = await check_yuyuko_cache(params["server"], params["accountId"])
         if is_cache:
             logger.success("上报数据成功")
         else:
             logger.success("跳过上报数据，直接请求")
         url = "https://api.wows.shinoaki.com/public/wows/account/user/info"
-        logger.success(f"下面是本次请求的参数，如果遇到了问题，请将这部分连同报错日志一起发送给麻麻哦\n{url}\n{params}")
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            result = resp.json()
-            logger.success(f"本次请求返回的状态码:{result['code']}")
-            logger.success(f"本次请求服务器计算时间:{result['queryTime']}")
+        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        result = orjson.loads(resp.content)
+        logger.success(f"本次请求总耗时{resp.elapsed.total_seconds()*1000}，服务器计算耗时:{result['queryTime']}")
         if result["code"] == 200 and result["data"]:
             template = env.get_template("wws-info.html")
             template_data = await set_infoparams(result["data"])
             content = await template.render_async(template_data)
             return await html_to_pic(
                 content, wait=0, viewport={"width": 920, "height": 1000}
             )
```

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/wws_realTime.py` & `hikari_bot-0.3.9/src/plugins/hikari_bot/moudle/wws_realTime.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-import time
-import traceback
-from os import getcwd
-from pathlib import Path
-
-import jinja2
-from nonebot import get_driver
-from nonebot.adapters.onebot.v11 import MessageSegment
-from nonebot.log import logger
-from nonebot_plugin_htmlrender import html_to_pic
-from playwright.async_api import async_playwright
-
-from .data_source import (
-    select_prvalue_and_color,
-    set_damageColor,
-    set_upinfo_color,
-    set_winColor,
-)
-from .publicAPI import get_all_shipList
-from .utils import get_bot
-
-dir_path = Path(__file__).parent
-template_path = dir_path / "template"
-env = jinja2.Environment(
-    loader=jinja2.FileSystemLoader(template_path), enable_async=True
-)
-env.globals.update(
-    set_damageColor=set_damageColor,
-    set_winColor=set_winColor,
-    set_upinfo_color=set_upinfo_color,
-    time=time,
-    int=int,
-    abs=abs,
-    enumerate=enumerate,
-)
-
-headers = {"Authorization": get_driver().config.api_token}
-
-# all_shipList = asyncio.run(get_all_shipList())
-
-
-async def send_realTime_message(data):
-    try:
-        global all_shipList
-        if not all_shipList:
-            all_shipList = await get_all_shipList()
-        bot = get_bot()
-        template = env.get_template("wws-realTime.html")
-        template_data = await set_realTime_params(data)
-        content = await template.render_async(template_data)
-        print(content)
-        async with async_playwright() as p:
-            browser = await p.chromium.launch()
-            page = await browser.new_page()
-            await page.goto(f"file://{getcwd()}")
-            await page.set_content(content, wait_until="networkidle")
-            img = await page.screenshot(full_page=True)
-            await browser.close()
-        await bot.send_group_msg(
-            group_id=639178962,
-            message=f"[测试功能]雨季刚刚进入了一场战斗\n{MessageSegment.image(img)}",
-        )
-    except Exception:
-        logger.error(traceback.format_exc())
-        return
-
-
-async def set_realTime_params(data):
-    try:
-        player_count = len(data["infoList"])
-        for each_player in data["infoList"]:
-            each_player["shipImgSmall"] = None
-            for each_ship in all_shipList:
-                if each_ship["id"] == each_player["shipId"]:
-                    if each_ship["shipNameCn"]:
-                        each_player["shipName"] = each_ship["shipNameCn"]
-                    else:
-                        each_player["shipName"] = each_ship["name"]
-                    each_player["shipImgSmall"] = each_ship["imgSmall"]
-                    each_player["shipIdValue"] = f"{each_ship['shipIdValue']}"
-                    break
-            if each_player["pvp"]:
-                (
-                    each_player["pvp"]["pr_name"],
-                    each_player["pvp"]["pr_color"],
-                ) = await select_prvalue_and_color(each_player["pvp"]["pr"])
-            if each_player["ship"]:
-                (
-                    each_player["ship"]["pr_name"],
-                    each_player["ship"]["pr_color"],
-                ) = await select_prvalue_and_color(each_player["ship"]["pr"])
-        data["player_count"] = player_count
-        data["template_path"] = template_path
-        logger.success(data)
-        return data
-    except Exception:
-        logger.error(traceback.format_exc())
-        return None
-
-
-async def send_message(content):
-    bot = get_bot()
-    img = await html_to_pic(content, wait=0, viewport={"width": 1800, "height": 1000})
-    await bot.send_group_msg(group_id=574432871, message=MessageSegment.image(img))
+#import time
+#import traceback
+#from os import getcwd
+#from pathlib import Path
+#
+#import jinja2
+#from nonebot import get_driver
+#from nonebot.adapters.onebot.v11 import MessageSegment
+#from nonebot.log import logger
+#from nonebot_plugin_htmlrender import html_to_pic
+#from playwright.async_api import async_playwright
+#
+#from ..data_source import (
+#    select_prvalue_and_color,
+#    set_damageColor,
+#    set_upinfo_color,
+#    set_winColor,
+#)
+#from .publicAPI import get_all_shipList
+#from ..utils import get_bot
+#
+#dir_path = Path(__file__).parent
+#template_path = dir_path / "template"
+#env = jinja2.Environment(
+#    loader=jinja2.FileSystemLoader(template_path), enable_async=True
+#)
+#env.globals.update(
+#    set_damageColor=set_damageColor,
+#    set_winColor=set_winColor,
+#    set_upinfo_color=set_upinfo_color,
+#    time=time,
+#    int=int,
+#    abs=abs,
+#    enumerate=enumerate,
+#)
+#
+#headers = {"Authorization": get_driver().config.api_token}
+#
+## all_shipList = asyncio.run(get_all_shipList())
+#
+#
+#async def send_realTime_message(data):
+#    try:
+#        global all_shipList
+#        if not all_shipList:
+#            all_shipList = await get_all_shipList()
+#        bot = get_bot()
+#        template = env.get_template("wws-realTime.html")
+#        template_data = await set_realTime_params(data)
+#        content = await template.render_async(template_data)
+#        print(content)
+#        async with async_playwright() as p:
+#            browser = await p.chromium.launch()
+#            page = await browser.new_page()
+#            await page.goto(f"file://{getcwd()}")
+#            await page.set_content(content, wait_until="networkidle")
+#            img = await page.screenshot(full_page=True)
+#            await browser.close()
+#        await bot.send_group_msg(
+#            group_id=639178962,
+#            message=f"[测试功能]雨季刚刚进入了一场战斗\n{MessageSegment.image(img)}",
+#        )
+#    except Exception:
+#        logger.error(traceback.format_exc())
+#        return
+#
+#
+#async def set_realTime_params(data):
+#    try:
+#        player_count = len(data["infoList"])
+#        for each_player in data["infoList"]:
+#            each_player["shipImgSmall"] = None
+#            for each_ship in all_shipList:
+#                if each_ship["id"] == each_player["shipId"]:
+#                    if each_ship["shipNameCn"]:
+#                        each_player["shipName"] = each_ship["shipNameCn"]
+#                    else:
+#                        each_player["shipName"] = each_ship["name"]
+#                    each_player["shipImgSmall"] = each_ship["imgSmall"]
+#                    each_player["shipIdValue"] = f"{each_ship['shipIdValue']}"
+#                    break
+#            if each_player["pvp"]:
+#                (
+#                    each_player["pvp"]["pr_name"],
+#                    each_player["pvp"]["pr_color"],
+#                ) = await select_prvalue_and_color(each_player["pvp"]["pr"])
+#            if each_player["ship"]:
+#                (
+#                    each_player["ship"]["pr_name"],
+#                    each_player["ship"]["pr_color"],
+#                ) = await select_prvalue_and_color(each_player["ship"]["pr"])
+#        data["player_count"] = player_count
+#        data["template_path"] = template_path
+#        logger.success(data)
+#        return data
+#    except Exception:
+#        logger.error(traceback.format_exc())
+#        return None
+#
+#
+#async def send_message(content):
+#    bot = get_bot()
+#    img = await html_to_pic(content, wait=0, viewport={"width": 1800, "height": 1000})
+#    await bot.send_group_msg(group_id=574432871, message=MessageSegment.image(img))
```

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/wws_recent.py` & `hikari_bot-0.3.9/src/plugins/hikari_bot/moudle/wws_recent.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,48 +4,46 @@
 from asyncio.exceptions import TimeoutError
 from datetime import datetime
 from pathlib import Path
 from typing import List
 
 import httpx
 import jinja2
+import orjson
 from httpx import ConnectTimeout
 from nonebot import get_driver
+from nonebot.adapters.onebot.v11 import ActionFailed, Bot, MessageSegment
 from nonebot.log import logger
-from nonebot.adapters.onebot.v11 import ActionFailed, MessageSegment,Bot
 from nonebot_plugin_htmlrender import html_to_pic
 
-from .data_source import (
+from ..data_source import (
     servers,
     set_damageColor,
     set_recentparams,
     set_upinfo_color,
     set_winColor,
+    template_path,
 )
+from ..HttpClient_pool import client_yuyuko
+from ..utils import match_keywords
 from .publicAPI import check_yuyuko_cache, get_AccountIdByName
-from .utils import match_keywords
 
-dir_path = Path(__file__).parent
-template_path = dir_path / "template"
 env = jinja2.Environment(
     loader=jinja2.FileSystemLoader(template_path), enable_async=True
 )
 env.globals.update(
     set_damageColor=set_damageColor,
     set_winColor=set_winColor,
     set_upinfo_color=set_upinfo_color,
     time=time,
     int=int,
     abs=abs,
     enumerate=enumerate,
 )
 
-headers = {"Authorization": get_driver().config.api_token}
-
-
 async def get_RecentInfo(server_type, info, bot:Bot, ev):
     try:
         params, day = None, 0
         if datetime.now().hour < 7:
             day = 1
         if isinstance(info, List):
             for i in info:  # 查找日期,没找到默认一天
@@ -94,19 +92,16 @@
             return "参数似乎出了问题呢"
         is_cache = await check_yuyuko_cache(params["server"], params["accountId"])
         if is_cache:
             logger.success("上报数据成功")
         else:
             logger.success("跳过上报数据，直接请求")
         url = "https://api.wows.shinoaki.com//api/wows/recent/v2/recent/info"
-        logger.success(f"下面是本次请求的参数，如果遇到了问题，请将这部分连同报错日志一起发送给麻麻哦\n{url}\n{params}")
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            result = resp.json()
-            logger.success(f"本次请求返回的状态码:{result['code']}")
+        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        result = orjson.loads(resp.content)
         if result["code"] == 200:
             if result["data"]["shipData"][0]["shipData"]:
                 template = env.get_template("wws-info-recent.html")
                 template_data = await set_recentparams(result["data"])
                 content = await template.render_async(template_data)
                 return await html_to_pic(
                     content, wait=0, viewport={"width": 1200, "height": 100}
```

### Comparing `hikari_bot-0.3.8.1/src/plugins/hikari_bot/wws_ship.py` & `hikari_bot-0.3.9/src/plugins/hikari_bot/moudle/wws_ship.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 import asyncio
 import re
 import time
 import traceback
 from asyncio.exceptions import TimeoutError
 from collections import defaultdict, namedtuple
 from datetime import datetime
-from pathlib import Path
 from typing import List
 
-import httpx
 import jinja2
+import orjson
 from bs4 import BeautifulSoup
 from httpx import ConnectTimeout
-from nonebot import get_driver
-from nonebot.adapters.onebot.v11 import ActionFailed, MessageSegment,Bot
+from nonebot.adapters.onebot.v11 import ActionFailed, Bot, MessageSegment
 from nonebot.log import logger
 from nonebot_plugin_htmlrender import html_to_pic, text_to_pic
 
-from .data_source import (
+from ..data_source import (
     number_url_homes,
     servers,
     set_damageColor,
     set_shipparams,
     set_shipRecentparams,
+    set_shipSelectparams,
     set_upinfo_color,
     set_winColor,
-    set_shipSelectparams,
+    template_path,
     tiers,
 )
+from ..HttpClient_pool import client_default, client_yuyuko
+from ..utils import match_keywords
 from .publicAPI import check_yuyuko_cache, get_AccountIdByName, get_ship_byName
-from .utils import match_keywords
 
-dir_path = Path(__file__).parent
-template_path = dir_path / "template"
 env = jinja2.Environment(
     loader=jinja2.FileSystemLoader(template_path), enable_async=True
 )
 env.globals.update(
     set_damageColor=set_damageColor,
     set_winColor=set_winColor,
     set_upinfo_color=set_upinfo_color,
     time=time,
     int=int,
     abs=abs,
     enumerate=enumerate,
 )
-
-headers = {"Authorization": get_driver().config.api_token}
-
 ShipSlectState = namedtuple("ShipSlectState", ["state", "SlectIndex", "SelectList"])
 ShipSecletProcess = defaultdict(lambda: ShipSlectState(False, None, None))
 
 
 async def get_ShipInfo(server_type, info, bot:Bot, ev):
     try:
         url, params = "", ""
@@ -135,21 +130,18 @@
             return "参数似乎出了问题呢"
         is_cache = await check_yuyuko_cache(params["server"], params["accountId"])
         if is_cache:
             logger.success("上报数据成功")
         else:
             logger.success("跳过上报数据，直接请求")
         url = "https://api.wows.shinoaki.com/public/wows/account/ship/info"
-        logger.success(f"下面是本次请求的参数，如果遇到了问题，请将这部分连同报错日志一起发送给麻麻哦\n{url}\n{params}")
         ranking = await get_MyShipRank_yuyuko(params)
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            result = resp.json()
-            logger.success(f"本次请求返回的状态码:{result['code']}")
-            logger.success(f"本次请求服务器计算时间:{result['queryTime']}")
+        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        result = orjson.loads(resp.content)
+        logger.success(f"本次请求总耗时{resp.elapsed.total_seconds()*1000}，服务器计算耗时:{result['queryTime']}")
         if result["code"] == 200 and result["data"]:
             if (
                 not result["data"]["shipInfo"]["battles"]
                 and not result["data"]["rankSolo"]["battles"]
             ):
                 return "查询不到战绩数据"
             template = env.get_template("wws-ship.html")
@@ -178,84 +170,80 @@
         ShipSecletProcess[ev.user_id] = ShipSlectState(False, None, None)
         return "wuwuu好像出了点问题，过一会儿还是不行的话请联系麻麻~"
 
 
 async def get_MyShipRank_yuyuko(params):
     try:
         url = "https://api.wows.shinoaki.com/upload/numbers/data/upload/user/ship/rank"
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            result = resp.json()
-            if result["code"] == 200 and result["data"]:
-                if result["data"]["ranking"]:
-                    return result["data"]["ranking"]
-                elif (
-                    not result["data"]["ranking"]
-                    and not result["data"]["serverId"] == "cn"
-                ):
-                    ranking = await get_MyShipRank_Numbers(
-                        result["data"]["httpUrl"], result["data"]["serverId"]
+        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        result = orjson.loads(resp.content)
+        if result["code"] == 200 and result["data"]:
+            if result["data"]["ranking"]:
+                return result["data"]["ranking"]
+            elif (
+                not result["data"]["ranking"]
+                and not result["data"]["serverId"] == "cn"
+            ):
+                ranking = await get_MyShipRank_Numbers(
+                    result["data"]["httpUrl"], result["data"]["serverId"]
+                )
+                if ranking:
+                    await post_MyShipRank_yuyuko(
+                        result["data"]["accountId"],
+                        ranking,
+                        result["data"]["serverId"],
+                        result["data"]["shipId"],
                     )
-                    if ranking:
-                        await post_MyShipRank_yuyuko(
-                            result["data"]["accountId"],
-                            ranking,
-                            result["data"]["serverId"],
-                            result["data"]["shipId"],
-                        )
-                    return ranking
-                else:
-                    return None
+                return ranking
             else:
                 return None
+        else:
+            return None
     except Exception:
         logger.error(traceback.format_exc())
         return None
 
 
 async def get_MyShipRank_Numbers(url, server):
     try:
         data = None
-        async with httpx.AsyncClient() as client:
-            resp = await client.get(url, timeout=10)
-            if resp.content:
-                result = resp.json()
-                page_url = str(result["url"]).replace("\\", "")
-                nickname = str(result["nickname"])
-                my_rank_url = f"{number_url_homes[server]}{page_url}"
-                async with httpx.AsyncClient() as client:
-                    resp = await client.get(my_rank_url, timeout=10)
-                    soup = BeautifulSoup(resp.content, "html.parser")
-                    data = (
-                        soup.select_one(f'tr[data-nickname="{nickname}"]')
-                        .select_one("td")
-                        .string
-                    )
+        resp = await client_default.get(url, timeout=10)
+        if resp.content:
+            result = orjson.loads(resp.content)
+            page_url = str(result["url"]).replace("\\", "")
+            nickname = str(result["nickname"])
+            my_rank_url = f"{number_url_homes[server]}{page_url}"
+            resp = await client_default.get(my_rank_url, timeout=10)
+            soup = BeautifulSoup(resp.content, "html.parser")
+            data = (
+                soup.select_one(f'tr[data-nickname="{nickname}"]')
+                .select_one("td")
+                .string
+            )
         if data and data.isdigit():
             return data
         else:
             return None
     except Exception:
         logger.error(traceback.format_exc())
         return None
 
 
 async def post_MyShipRank_yuyuko(accountId, ranking, serverId, shipId):
     try:
-        async with httpx.AsyncClient(headers=headers) as client:
-            url = "https://api.wows.shinoaki.com/upload/numbers/data/upload/user/ship/rank"
-            post_data = {
-                "accountId": int(accountId),
-                "ranking": int(ranking),
-                "serverId": serverId,
-                "shipId": int(shipId),
-            }
-            resp = await client.post(url, json=post_data, timeout=None)
-            result = resp.json()
-            return
+        url = "https://api.wows.shinoaki.com/upload/numbers/data/upload/user/ship/rank"
+        post_data = {
+            "accountId": int(accountId),
+            "ranking": int(ranking),
+            "serverId": serverId,
+            "shipId": int(shipId),
+        }
+        resp = await client_yuyuko.post(url, json=post_data, timeout=None)
+        result = orjson.loads(resp.content)
+        return
     except Exception:
         logger.error(traceback.format_exc())
         return
 
 
 async def get_ShipInfoRecent(server_type, info, bot:Bot, ev):
     try:
@@ -352,18 +340,16 @@
             return "参数似乎出了问题呢"
         is_cache = await check_yuyuko_cache(params["server"], params["accountId"])
         if is_cache:
             logger.success("上报数据成功")
         else:
             logger.success("跳过上报数据，直接请求")
         url = "https://api.wows.shinoaki.com/api/wows/recent/v2/recent/info/ship"
-        logger.success(f"下面是本次请求的参数，如果遇到了问题，请将这部分连同报错日志一起发送给麻麻哦\n{url}\n{params}")
-        async with httpx.AsyncClient(headers=headers) as client:
-            resp = await client.get(url, params=params, timeout=None)
-            result = resp.json()
+        resp = await client_yuyuko.get(url, params=params, timeout=None)
+        result = orjson.loads(resp.content)
         if result["code"] == 200 and result["data"]:
             template = env.get_template("wws-ship-recent.html")
             template_data = await set_shipRecentparams(result["data"])
             content = await template.render_async(template_data)
             return await html_to_pic(
                 content, wait=0, viewport={"width": 800, "height": 100}
             )
```

### Comparing `hikari_bot-0.3.8.1/setup.py` & `hikari_bot-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src\\plugins'}
 
 packages = \
-['hikari_bot', 'hikari_bot.game']
+['hikari_bot', 'hikari_bot.game', 'hikari_bot.moudle']
 
 package_data = \
 {'': ['*'],
  'hikari_bot': ['template/Chart.min.js',
                 'template/Chart.min.js',
                 'template/Chart.min.js',
                 'template/Chart.min.js',
@@ -272,21 +272,21 @@
  'httpx>=0.20.0',
  'nonebot-adapter-onebot>=2.1.0,<3.0.0',
  'nonebot-plugin-apscheduler>=0.2.0,<0.3.0',
  'nonebot-plugin-htmlrender>=0.2.0.1,<0.3.0.0',
  'nonebot-plugin-reboot>=0.1.3,<0.2.0',
  'nonebot2[fastapi]>=2.0.0-beta.1,<3.0.0',
  'nonebot_plugin_guild_patch>=0.2.1,<0.3.0',
- 'paho-mqtt>=1.6.1,<2.0.0']
+ 'orjson>=3.8.11,<4.0.0']
 
 setup_kwargs = {
     'name': 'hikari-bot',
-    'version': '0.3.8.1',
+    'version': '0.3.9',
     'description': 'Nonebot2 HikariBot,支持战舰世界水表查询',
-    'long_description': '<!-- markdownlint-disable MD033 MD041 -->\n<p align="center">\n  <a href="https://github.com/benx1n/HikariBot"><img src="https://s2.loli.net/2022/05/28/SFsER8m6TL7jwJ2.png" alt="Hikari " style="width:200px; height:200px" ></a>\n</p>\n\n<div align="center">\n\n# Hikari\n\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable-next-line MD036 -->\n战舰世界水表BOT\n<!-- prettier-ignore-end -->\n\n\n\n<p align="center">\n  <a href="https://pypi.python.org/pypi/hikari-bot">\n    <img src="https://img.shields.io/pypi/v/hikari-bot" alt="pypi">\n  </a>\n  <img src="https://img.shields.io/badge/python-3.8.0+-blue" alt="python">\n  <a href="https://jq.qq.com/?_wv=1027&k=S2WcTKi5">\n    <img src="https://img.shields.io/badge/QQ%E7%BE%A4-967546463-orange?style=flat-square" alt="QQ Chat Group">\n  </a>\n  <a href="https://qun.qq.com/qqweb/qunpro/share?_wv=3&_wwv=128&appChannel=share&inviteCode=1W4NX2S&from=181074&biz=ka#/pc">\n    <img src="https://img.shields.io/badge/QQ%E9%A2%91%E9%81%93-yuyuko助手-5492ff?style=flat-square" alt="QQ Channel">\n  </a>\n\n# 💘您不打算给可爱的Hikari点个Star吗QAQ\n</p>\n</div>\n\n## 简介\n\n战舰世界水表BOT，基于Nonebot2  \n水表人，出击！wws me recent！！！  \nQQ频道官方机器人已上线，请点击上方链接加入体验~  \n[Hoshino版插件](https://github.com/benx1n/wows-stats-bot)\n\n\n## 特色\n\n- [x] 账号总体、单船、近期战绩\n- [x] 全指令支持参数乱序\n- [x] 快速切换绑定账号\n- [x] 实时推送对局信息\n- [x] 支持@快速查询\n- [x] 全异步，高并发下性能更优\n- [x] 支持频道（非官方bot类型）\n\n  <details>\n  <summary>点我查看功能列表</summary>\n\n  - 绑定账号：wws bind/set/绑定 [服务器+游戏昵称]：\n  - 查询账号绑定列表：wws [查询/查]绑定/绑定列表 [me/@群友]：\n  - 切换删除绑定账号：wws [切换/删除]绑定 [序号]\n  - 查询账号总体战绩：wws [(服务器+游戏昵称)/@群友/me]\n  - 查询账号历史记录：wws [(服务器+游戏昵称)/@群友/me] record\n  - 查询账号近期战绩：wws [(服务器+游戏昵称)/@群友/me] recent [日期]\n  - 查询单船总体战绩：wws [(服务器+游戏昵称)/@群友/me] ship [船名]\n  - 查询单船近期战绩：wws [(服务器+游戏昵称)/@群友/me] ship [船名] recent [日期]\n  - 查询服务器排行榜：wws [服务器+战舰名] rank/ship.rank\n  - 查询军团详细信息：wws [(服务器+军团名)/@群友/me] clan\n  - 查询军团历史记录：wws [(服务器+军团名)/@群友/me] clan record\n  - 查询舰船中英文名：wws [搜/查船名] [国家][等级][类型]\n  - 检查版本更新：wws 检查更新\n  - 更新：wws 更新Hikari\n  - 查看帮助：wws help\n  - 噗噗：一言\n\n  </details>\n  <details>\n  <summary>点我查看与Hoshino版的区别</summary>\n\n  - Hikari所使用的Nonebot2框架相比Hoshino更易部署，且两者在单环境下不兼容\n  - 一些功能比如频道目前仅支持Hikari\n  - Hoshino的插件生态更偏向PCR，具体可以查看[Nonebot2商店](https://v2.nonebot.dev/store)和[Hoshino插件索引](https://github.com/pcrbot/HoshinoBot-plugins-index)\n  - 由于个人精力原因，主要功能开发和维护面向Hikari，Hoshino版仅做最低限度功能适配\n\n  </details>\n  <details>\n  <summary>点我查看遇到问题如何解决</summary>\n\n  - [ ] 请确认您已按文档中部署流程进行\n  - [ ] 请确认您已完整浏览[可能会遇到的问题](https://github.com/benx1n/HikariBot#%E5%8F%AF%E8%83%BD%E4%BC%9A%E9%81%87%E5%88%B0%E7%9A%84%E9%97%AE%E9%A2%98)，且仍无法自行解决\n  - [ ] [提问的智慧](https://github.com/ryanhanwu/How-To-Ask-Questions-The-Smart-Way/blob/main/README-zh_CN.md)\n  - [ ] 提供系统环境和bot版本，以及出现问题前后至少 10 秒的完整日志内容。请自行删除日志内存在的个人信息及敏感内容\n\n  </details>\n## 在Windows系统上快速部署\n>点我查看[视频教程](https://www.bilibili.com/video/BV1XP411U7rC)\n\n  `windows安装python版本请勿大于3.11,建议版本3.9`\n\n1. 下载Hikari的[最新Release](https://github.com/benx1n/HikariBot/releases/download/Latest/release_windows.zip)并解压到合适文件夹\n2. 复制一份`.env.prod-example`文件，并将其重命名为`.env.prod`,打开并按其中注释编辑\n    >只显示了.env，没有后面的后缀？请百度`windows如何显示文件后缀名`\n    ```\n    API_TOKEN = xxxxxxxx #无需引号，TOKEN即回复您的邮件所带的一串由[数字+冒号+英文/数字]组成的字符串\n    SUPERUSERS=["QQ号"]\n    ```\n   - 最后TOKEN应该长这样 `API_TOKEN = 123764323:ba1f2511fc30423bdbb183fe33`\n   - 从0.3.2.2版本开始，您没有填写的配置将按.env文件中的默认配置执行，具体逻辑为\n      - 私聊、频道默认禁用\n      - 群聊默认开启，默认屏蔽官方交流群\n      - 默认WEB登录账号密码为admin/admin，如有需要请自行修改，无需设置密码请删除env.prod中的配置项\n\n3. 双击`启动.bat`\n    - 页面加载不出请尝试刷新一下，已知IE浏览器可能存在一些问题\n    - 此时若没有报错，您可以在打开的页面`http://127.0.0.1:8080/go-cqhttp/`中\n      点击左侧添加账号，重启bot即可在网页上看到相应信息（大概率需要扫码）\n    - 如果重启后go-cqhhtp一直卡在扫码或无限重启，请跳转[无法使用内嵌go-cqhttp登录](https://github.com/benx1n/HikariBot#%E6%97%A0%E6%B3%95%E4%BD%BF%E7%94%A8%E5%86%85%E5%B5%8Cgo-cqhttp%E7%99%BB%E5%BD%95bot)\n\n## Linux一键脚本\n> 仅支持Debian、CentOS、Ubuntu\n```\nwget -qO - https://fastly.jsdelivr.net/gh/benx1n/HikariBot@master/install.sh | bash\n```\n\n\n## 使用Docker部署\n- Docker目录下是一个简单的Dockerfile，可以基于官方的Python容器封装一个完整的HikariBot\n  - 以`12hydrogen/hikari-bot:latest`上线官方仓库\n- 注意需要将内部的8080端口映射出来\n  ```\n  docker run -d -P 12hydrogen/hikari-bot:latest -t [token] -i [qqid] # 首次使用需输入token和qqid，-P表示将8080端口随机映射至主机\n  docker run -d -p 12345:8080 12hydrogen/hikari-bot:latest -t [token] -i [qqid] # 使用-p以指定映射在外的端口\n  ```\n- 运行上述指令后会在终端显示一串字符，即Docker容器的标识符，一般使用前几位即可唯一确定一个容器\n  ```\n  1a2b3c4d5e..... # 标识符\n  docker stop 1a2b # 使用前四位确定，stop即停止容器\n  1a2b3c4d5e.....\n  docker start 1a2b # start即启动容器\n  1a2b3c4d5e.....\n  docker restart 1a2b # restart即重启容器\n  1a2b3c4d5e.....\n  ```\n- 在更新后即上传新版本容器\n  ```\n  docker pull 12hydrogen/hikari-bot:latest # 更新\n  docker stop 1a2b\n  1a2b...\n  docker run -d --volumes-from 1a2b -P 12hydrogen/hikari-bot:latest -t [token] -i [qqid] # 随机映射\n  or\n  docker run -d --volumes-from 1a2b -p 12345:8080 12hydrogen/hikari-bot:latest -t [token] -i [qqid] # 指定映射\n  9z8y... # 注意标识符变化了\n  docker rm 1a2b # 删除旧容器，\n  1a2b...\n  ```\n- 将配置文件与容器分离\n  使用volume在宿主机保存相关账号信息，更新时按照相关步骤继承volume即可\n\n## 在Windows系统上完整部署\n1. 下载[Git](https://git-scm.com/download/win)、[Python](https://www.python.org/downloads/windows/)并安装\n    >Python版本需>3.8，或参考[Hoshino版插件](https://github.com/benx1n/wows-stats-bot)中使用Conda虚拟环境\n    >\n    >请注意python安装时勾选或点击`添加到环境变量`，可以安装后cmd中输入`python --version`来验证是否成功\n    >\n    >否则请自行百度如何添加python到环境变量\n\n3. 打开一个合适的文件夹，鼠标右键——Git Bash here，输入以下命令（任选一条）克隆本Hikari仓库\n    ```\n    git clone https://github.com/benx1n/HikariBot.git\n\n    git clone https://gitee.com/benx1n/HikariBot.git\n    ```\n3. 以管理员身份运行`一键安装.bat`\n    >等效于在cmd中执行如下代码\n    ```\n    python -m pip install nb-cli hikari-bot nonebot-plugin-apscheduler nonebot-plugin-gocqhttp -i https://pypi.tuna.tsinghua.edu.cn/simple\n    ```\n\n4. 复制一份`.env.prod-example`文件，并将其重命名为`.env.prod`,打开并按其中注释编辑\n    >只显示了.env，没有后面的后缀？请百度`windows如何显示文件后缀名`\n    ```\n    API_TOKEN = xxxxxxxx #无需引号，TOKEN即回复您的邮件所带的一串由[数字+冒号+英文/数字]组成的字符串\n    SUPERUSERS=["QQ号"]\n    ```\n   - 最后TOKEN应该长这样 `API_TOKEN = 123764323:ba1f2511fc30423bdbb183fe33`\n   - 从0.3.2.2版本开始，您没有填写的配置将按.env文件中的默认配置执行，具体逻辑为\n      - 私聊、频道默认禁用\n      - 群聊默认开启，默认屏蔽官方交流群`\n      - 默认WEB登录账号密码为admin/admin，如有需要请自行修改，无需设置密码请删除env.prod中的配置项\n      - 默认开启噗噗\n      - 默认开启缓存上报\n      - 默认关闭代理\n\n5. 双击`启动.bat`，在打开的浏览器中添加bot账号密码，重新启动Hikari\n    - 页面加载不出请尝试刷新一下，已知IE浏览器可能存在一些问题\n    - 此时若没有报错，您可以在打开的页面`http://127.0.0.1:8080/go-cqhttp/`中\n      点击左侧添加账号，重启bot即可在网页上看到相应信息（大概率需要扫码）\n    - 如果重启后go-cqhhtp一直卡在扫码或无限重启，请跳转[无法使用内嵌go-cqhttp登录](https://github.com/benx1n/HikariBot#%E6%97%A0%E6%B3%95%E4%BD%BF%E7%94%A8%E5%86%85%E5%B5%8Cgo-cqhttp%E7%99%BB%E5%BD%95bot)\n\n\n## ~~在Linux上完整部署~~\n- 需要Python基本环境\n- Clone本仓库\n- 使用`./manage.sh`，基于原有批处理脚本\n- 无参数调用以获取使用帮助\n1. `install`\n    - 安装必须的依赖与bot本体\n2. `update`\n    - 更新bot\n3. `start [-t/--token] [token] [-i/--id] [qqid]`\n    - 运行bot\n    - 在当前目录下不存在`.env.prod`的情况下从参数获取token和qqid以创建相应文件，否则直接运行\n    - 考虑到使用Linux部署时多数情况下本地不存在图形界面，有风险的向公网开放访问\n    - 加入验证机制（listed）\n\n\n## 作为已有Bot的插件部署（如真寻、Haruka）\n1. 如果您已经有了一个基于Nonebot2的机器人（例如真寻），您可以直接\n    ```\n    pip install hikari-bot\n    ```\n2. 在bot的bot.py中加入\n    ```\n    nonebot.load_plugin(\'nonebot_plugin_htmlrender\')\n    nonebot.load_plugin(\'hikari_bot\')\n    ```\n3. 在环境文件中加入以下配置项\n    ```\n    API_TOKEN = xxxxxxxxxxxx\n    SUPERUSERS=["QQ号"]\n    private = false                 #开启私聊\n    group = true                    #开启群聊\n    channel = false                 #开启频道\n    all_channel = false             #是否全频道生效，无论此项配置如何，channel_list中的频道一定会开启\n    channel_list = []               #频道列表白名单，数组形式，可在控制台中获取相应的channel_id\n    ban_group_list = [967546463]    #群列表黑名单，默认屏蔽了开发者交流群\n    pupu = true                     #是否开启噗噗\n    check_cache = true              #是否开启缓存上报,可降低高峰期延迟,如果错误日志中频繁报错上报url:XXXXXXXX,请关闭此项或配置代理\n    proxy_on = false                #是否启用代理\n    proxy = http://localhost:7890   #代理地址，如果上面选项开启，这边替换为你本地的\n    ocr_on = true                   #是否开启ocr(识图指令)\n    ocr_offline = false             #是否只使用hash验证，即设置为true后只能识别服务器已记录的图片，如果群较多(>300)导致响应延迟较高可以开启\n    ocr_url = http://mc.youthnp.cn:23338/OCR/           #默认ocr地址，一般不用动\n    ```\n    >一般来说该文件为.env.dev\n    >也有可能是.env.pord，具体需要看.env中是否有指定\n4.   重启bot\n\n## 更新\n实验性更新指令：`wws 更新Hikari`\n请确保在能登录上服务器的情况下使用\n以下是旧更新方法\n1. 按不同版本\n   - Windows一键包：下载最新一键包，复制旧版本中`accounts`文件夹和`env.prod`文件替换至新版文件夹中即可\n   - 完整版：以管理员身份运行`更新.bat`或执行`./manage.sh update`\n      >等效于在cmd中执行如下代码\n      ```\n      pip install --upgrade hikari-bot\n      git pull\n      ```\n   - 插件版：在cmd中执行如下代码\n      ```\n      pip install --upgrade hikari-bot\n      ```\n2. **对比`.env.prod-example`中新增的配置项，并同步至你本地的`env.prod`**\n    - install结束后会打印当前版本\n    - 您也可以通过`pip show hikari-bot`查看当前Hikari版本\n    - 如果没有更新到最新版请等待一会儿，镜像站一般每五分钟同步\n    - 从0.3.2.2版本开始，您没有填写的配置将按.env文件中的默认配置执行，具体逻辑为\n      - 私聊、频道默认禁用\n      - 群聊默认开启，默认屏蔽官方交流群\n\n## 最近的更新日志\n\n### 23-04-07    v0.3.8\n- [+]新增国服封号记录查询，指令wws ban/wws 封号记录\n- [#]修复了上次修复排行榜新产生的bug\n\n### 23-04-04    v0.3.7\n- [+]添加获取随机表情包，指令wws 随机表情包\n- [+]更新船只选择界面\n- [#]更新Linux脚本托管\n\n### 23-02-22    v0.3.6.4\n- [+]添加随机嘴臭，概率千分之一\n- [+]添加ocr启动报错提示\n- [#]修复一键包及Docker依赖问题 [@94Bo](https://github.com/94Bo) [@12hydrogen](https://github.com/12hydrogen)\n\n### 22-11-18    v0.3.6  包含配置项更新，请添加`env.prod-example`中新增的配置\n- [+]新增噗噗（已于0.3.5.2实装）\n- [+]新增OCR（已于0.3.5.5实装）\n- [+]新增扫雪统计和圣诞船池检查\n- [+]新增国服排行榜\n- [#]大幅优化高峰期响应速度（已于0.3.5.3实装）\n- [#]Linux下支持微软雅黑(已热更新)\n\n### 22-10-29    v0.3.5.5  添加测试功能OCR，支持图片指令\n### 22-10-27    v0.3.5.4  修复一键更新指令bug\n### 22-10-26    v0.3.5.3  添加缓存上报机制，修复噗噗误触发的bug\n### 22-10-25    v0.3.5.2  新增噗噗\n### 22-07-24    v0.3.5  适配nontbo2 v2.0.0rc1  \n### 22-07-24    v0.3.4  **配置项及入口文件更新**  请完整拉取最新仓库，并同步添加`env.prod-example`中新增的配置\n- 重要更新，完整版安装请拉取最新仓库代码，一键包请下载最新版本\n- [+]新增一键更新指令，指令wws 更新Hikari\n- [+]新增Linux一键脚本 [@94Bo](https://github.com/94Bo)\n- [#]修改部分依赖版本\n- [#]大幅改动了模板以适配后续功能\n- [#]修改框架\n- [#]修改接口url\n- [#]修复了没有完全修复的兼容性问题[#11](https://github.com/benx1n/HikariBot/issues/11)\n- [#]修改日志输出等级，现在控制台只会打印SUCCESS级以上的日志\n\n\n\n### 22-07-14    v0.3.3  积累更新\n- [+]新增群聊黑名单，默认屏蔽开发者群"\n- [+]docker添加CI/CD构建发布 [@12hydrogen](https://github.com/12hydrogen)\n- [#]修复与其他插件的兼容性问题\n- [#]更改了请求域名\n- [#]修复manage.sh会更改toml的问题\n- [#]修复了hoshino排行榜选择船只样式问题\n- [#]修复仅打过PVE的单船仍会显示战绩详情的问题\n- [#]info适配v4接口\n- [+]新增配置项ban_group_list\n\n<details>\n<summary><b>更以前的更新日志</b></summary>\n\n### 22-07-05    v0.3.2.2  一些修复\n- [#]修复切换、删除绑定的bug\n- [#]默认配置改为不启用WEB登陆验证\n- [#]修复.bat的环境变量问题 [@94Bo](https://github.com/94Bo)\n\n### 22-07-04    v0.3.2.1  **配置项及入口文件更新**  请完整拉取最新仓库，并同步添加`env.prod-example`中新增的配置\n- [+]新增对QQ频道的适配（非官方bot接入，官方版bot已上线yuyuko频道）\n- [+]新增自定义开启群聊、私聊、QQ频道\n- [+]新增web登录密码\n- [+]新增默认配置项\n- [+]新增PR彩蛋\n- [#]info适配V3接口\n- [#]recent显示时间区间\n\n### 22-06-23    v0.3.1  **重要功能更新**\n- [+]新增单船近期战绩，可显示每日详细信息，指令`wws ship recent`\n- [+]新增docker部署 [@12hydrogen](https://github.com/12hydrogen)\n- [#]修复国服特殊字符ID无法查询的bug\n- [#]修复船只选择过期后发送数字序号仍被识别的bug\n\n### 22-06-15    v0.3.0.1  **重要功能更新**\n- [+]支持显示军团评级颜色\n- [#]排行榜内部逻辑改动，现在仅显示前十，不更新将无法使用\n- [#]\\(hotfix)`wws recent`现在无随机战绩不会显示PR和上方战斗信息\n\n### 22-06-08    v0.2.9.4  **重要功能更新**\n- [+]新增单船的服务器排行，显示在`wws ship`的详情页面下\n- [#]修复0.2.9后无法启动的bug\n- [#]js依赖改为本地\n- [#]修改recent样式，不更新可能会导致错位\n- [#]优化报错提示\n\n### 22-06-03    v0.2.8  一些修复\n- [+]新增删除绑定功能\n- [#]修复`wws ship`总览经验和胜率不上色的bug\n- [#]修复`wws ship`详情只有单野场均被上色的bug\n- [#]修复`wws 查船名`中搜不到德国船的bug\n\n### 22-06-03    v0.2.6  [#]修复`wws recent`胜率颜色的bug\n\n### 22-06-03    v0.2.5  [#]修复`wws recent`击杀显示成命中的bug\n\n### 22-06-03    v0.2.4  **重要功能更新** 否则您将无法使用`wws recent`功能\n- [+]全指令在游戏名外带上括号即可强制指定昵称，以适配一些带有空格、特殊字符、指令字符的昵称\n- [+]新增特殊绑定，请配合网页端食用，复制后发送给Hikari即可一键绑定\n- [+]新增部分报错提示\n- [#]更改ship,rank,recent样式，现在没有战斗场次的类型不会被显示\n- [#]优化Hikari的部署流程\n- [#]修复me大写不被识别的问题\n\n\n### 22-06-02    v0.2.3  一些修复\n- [+]全指令支持大写\n- [#]修复Linux上可能出现的报错\n- [#]修改部分图片的样式\n\n### 22-06-01    v0.2.2  修复了一个VSC导致的依赖错误\n\n### 22-06-01    v0.2.1  修复问题\n\n### 22-06-01    v0.2.0  **重要功能更新**\n- [+]新增排位数据\n- [+]支持国服\n- [+]单船战绩显示单野、自行车、三轮车\n- [+]启用gzip，试图改善请求Timeout\n- [+]增加3s指令CD和每日100次上限\n- [#]修复图片内字符不对称的bug（强迫症）\n- [#]修改未绑定账号时的返回\n- [#]修复网络问题与找不到游戏名时相同返回的bug\n- [#]适配HarukaBot\n\n\n### 22-05-31    v0.1.9  一些修复\n- [#]解决由于QQ风控导致的船只选择列表无法发送的问题\n- [#]修复带非me/@参数查询绑定时引起的报错\n\n### 22-05-30    v0.1.8  **重要更新**\n- [+]所有带请求参数的部分添加log输出以方便查找问题\n- [+]添加平台报错时返回以和Hikari内部错误区分\n- [#]移除bat脚本中的utf8以支持部分英文服务器\n- [#]试图减少因网络导致的报错问题\n\n### 22-05-30    v0.1.7  一些修复\n- [#]修复排行榜查询报错\n- [#]修复部分环境可能出现的单船查询无法选择问题\n\n### 22-05-28    v0.1.6  **重要功能更新**\n- [+]新增排行榜查询 指令`wws rank/ship.rank`\n- [+]新增是否开启内置go-cqhttp，默认开启\n\n### 22-05-28    v0.1.5  一些功能更新\n- [+]添加等级显示，适配新舰船数据\n- [+]新增wws 检查更新\n- [+]配置项添加Bot管理员\n- [#]修复定时任务不触发的bug\n\n### 22-05-27    v0.1.4  一些功能优化\n- [+]添加在windows下的一键安装、更新、启动脚本\n- [#]修复数字ID的recent匹配问题\n- [#]优化提示逻辑\n\n### 22-05-27    v0.1.3  一些修复和适配\n- [+]适配包括真寻等大部分Nonebot2机器人\n- [#]修复自动更新的bug\n\n### 22-05-27    v0.1.2  **调整info接口，不更新无法使用**\n\n### 22-05-27    v0.1.1  一些小改动\n\n### 22-05-27    v0.1.0  一些更新\n- [+]新增定时检查更新\n- [+]新增部署教程\n- [+]添加11级战绩信息\n- [#]优化账号总体和单船图片样式\n\n</details>\n\n## 可能会遇到的问题\n\n### go-cqhttp扫码后提示异地无法登录\n- 一般提示需要扫码，扫码后提示异地无法登录\n- 关于该问题，您可以查看[这里](https://github.com/Mrs4s/go-cqhttp/issues/1469)获得相应解决办法，这里简单列举三种办法\n  - 启动时登录方式选择`浏览器滑条`，按后续提示登录\n  - 手机下载`爱加速`等代理，连接到服务器对应市级地区\n  - 在本地电脑使用go-cqhttp登录成功后，将会在exe同级目录下生成`session.token`和`device.json`两个文件\n  将这两个文件复制到服务器对应目录下并重启\n    - 内嵌go-cqhttp为`account\\QQ号`\n    - 独立go-cqhttp为exe所在同级目录下，请注意使用独立go-cqhttp时需要将`.env.prod`的`USE_PLUGIN_GO_CQHTTP`的值改为`false`\n\n### 无法使用内嵌go-cqhttp登录bot\n\n1. 下载 go-cqhttp 至合适的文件夹\n\n    - github 发布页：https://github.com/Mrs4s/go-cqhttp/releases/latest\n\n    > 您需要根据自己的机器架构选择版本，Windows一般为x86/64架构，通常选择[go-cqhttp_windows_amd64.exe](https://github.com/Mrs4s/go-cqhttp/releases/latest/download/go-cqhttp_windows_amd64.exe)\n\n2. 双击go-cqhttp，提示释出bat，重新运行bat，选择websocket反向代理，go-cqhttp将会在同文件夹内自动创建一个`config.yml`，右键使用notepad++打开，根据注释填写QQ账号密码，并将以下内容写入文件结尾（需替换原有的ws-reverse节点）：\n\n    ```yaml\n      - ws-reverse:\n          universal: ws://127.0.0.1:8080/onebot/v11/ws\n          reconnect-interval: 5000\n          middlewares:\n            <<: *default\n    ```\n\n    > 关于go-cqhttp的配置，你可以在[这里](https://docs.go-cqhttp.org/guide/config.html#%E9%85%8D%E7%BD%AE%E4%BF%A1%E6%81%AF)找到更多说明。\n\n3. 启动go-cqhttp，按照提示登录。\n\n    > 此处如出现异地登陆保护，请尝试\n    > - 在本地电脑使用go-cqhttp登录成功后，将会在exe同级目录下生成`session.token`和`device.json`两个文件\n    > - 将这两个文件复制到服务器对应go-cqhttp目录下并重启\n\n4. 修改Hikari文件夹下.env.prod中`USE_PLUGIN_GO_CQHTTP`的值为`false`\n    ```\n    USE_PLUGIN_GO_CQHTTP = false\n    ```\n5. 在文件夹下打开终端，输入`python bot.py`启动bot\n    - 一键包双击`启动.bat`即可\n\n\n### 出现ZoneInfoNotFoundError报错\n>\n>您可以在[这里](https://github.com/nonebot/nonebot2/issues/78)找到相关解决办法\n>\n### Recent和绑定提示\'鉴权失败\'\n1. 检查Token是否配置正确，token格式为`XXXXX:XXXXXX`\n2. 如果配置正确可能是Token失效了，请重新申请\n\n### \'Config\' Object has no attribute XXXX\n1. 检查视力，重新阅读[更新](https://github.com/benx1n/HikariBot#更新)章节\n\n### Failed to import "nonebot_plugin_guild_patch"\n以下方法任选一种\n- 更新python版本至3.9+\n- 降低Hikari版本至3.1，等待后续版本修复\n- 使用Hikari一键包，其中自带了3.10的python虚拟环境\n- 修改依赖包代码，见[这里](https://github.com/mnixry/nonebot-plugin-guild-patch/pull/6/files)\n\n### Ubuntu系统下部署字体不正常(针对一些云服务器的Ubuntu镜像，不保证成功，只是提供一个解决方案)\n  1. 执行以下命令，完善字体库并将中文设置成默认语言（部分Ubuntu可能不需要该步骤，可直接从第二步开始）\n  ```\n  sudo apt install fonts-noto  \n  sudo locale-gen zh_CN zh_CN.UTF-8  \n  sudo update-locale LC_ALL=zh_CN.UTF-8 LANG=zh_CN.UTF-8  \n  sudo fc-cache -fv\n  ```\n  \n  2. 在你的Windows电脑上打开`C:\\Windows\\fonts`文件夹，找到里面的微软雅黑字体，将其复制出来，放在任意目录，应该会得到`msyh.ttc`，`mshybd.ttc`，`msyhl.ttc`三个文件。（不会有人还用Win7吧？）\n\n  3. 进入到`/usr/share/fonts`文件夹下，创建一个文件夹命名为`msyh`，然后进入其中\n  ```\n  cd /usr/share/fonts \n  sudo mkdir msyh \n  cd msyh\n  ```\n  \n  4. 将三个字体文件上传到`msyh`文件夹中(过程中遇到的问题请自行解决)\n\n  5. 执行以下命令（此时你应该是在`msyh`文件夹下），加载字体\n  ```\n  sudo mkfontscale \n  sudo mkfontdir \n  sudo fc-cache -fv\n  ```\n  \n  6. （可选，若不正常可尝试）重启Hikari。\n\n### 首次启动时plugin-gocqhttp的startup方法报错(traceback中一般还有ssl的错误)\n\n1. 下载 go-cqhttp\n\n    - github 发布页：https://github.com/Mrs4s/go-cqhttp/releases/latest\n\n    > 您需要根据自己的机器架构选择版本，Windows一般为x86/64架构，通常选择[go-cqhttp_windows_amd64.exe](https://github.com/Mrs4s/go-cqhttp/releases/latest/download/go-cqhttp_windows_amd64.exe)\n\n2. 重命名为`go-cqhttp.*`(*为所选择版本后缀,如windowx就是go-cqhttp.exe)并放入`HikariBot\\accounts\\binary`文件夹下\n\n3. 重新启动Hikari\n\n## 贡献代码\n\n请向dev分支提交PR\n\n## 鸣谢\n\n感谢以下开发者及项目做出的贡献与支持\n\n<a href="https://github.com//benx1n/HikariBot/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=benx1n/HikariBot" />\n</a>\n\n[Nonebot2](https://github.com/nonebot/nonebot2)  \n[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)  \n[战舰世界API平台](https://wows.shinoaki.com/)  \n\n## 开源相关\nMIT\n修改、分发代码时请保留原作者相关信息\n',
+    'long_description': '<!-- markdownlint-disable MD033 MD041 -->\n<p align="center">\n  <a href="https://github.com/benx1n/HikariBot"><img src="https://s2.loli.net/2022/05/28/SFsER8m6TL7jwJ2.png" alt="Hikari " style="width:200px; height:200px" ></a>\n</p>\n\n<div align="center">\n\n# Hikari\n\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable-next-line MD036 -->\n战舰世界水表BOT\n<!-- prettier-ignore-end -->\n\n\n\n<p align="center">\n  <a href="https://pypi.python.org/pypi/hikari-bot">\n    <img src="https://img.shields.io/pypi/v/hikari-bot" alt="pypi">\n  </a>\n  <img src="https://img.shields.io/badge/python-3.8.0+-blue" alt="python">\n  <a href="https://jq.qq.com/?_wv=1027&k=S2WcTKi5">\n    <img src="https://img.shields.io/badge/QQ%E7%BE%A4-967546463-orange?style=flat-square" alt="QQ Chat Group">\n  </a>\n  <a href="https://qun.qq.com/qqweb/qunpro/share?_wv=3&_wwv=128&appChannel=share&inviteCode=1W4NX2S&from=181074&biz=ka#/pc">\n    <img src="https://img.shields.io/badge/QQ%E9%A2%91%E9%81%93-yuyuko助手-5492ff?style=flat-square" alt="QQ Channel">\n  </a>\n\n# 💘您不打算给可爱的Hikari点个Star吗QAQ\n</p>\n</div>\n\n## 简介\n\n战舰世界水表BOT，基于Nonebot2  \n水表人，出击！wws me recent！！！  \nQQ频道官方机器人已上线，请点击上方链接加入体验~  \n[Hoshino版插件](https://github.com/benx1n/wows-stats-bot)\n\n\n## 特色\n\n- [x] 账号总体、单船、近期战绩\n- [x] 全指令支持参数乱序\n- [x] 快速切换绑定账号\n- [x] 实时推送对局信息\n- [x] 支持@快速查询\n- [x] 全异步，高并发下性能更优\n- [x] 支持频道（非官方bot类型）\n\n  <details>\n  <summary>点我查看功能列表</summary>\n\n  - 绑定账号：wws bind/set/绑定 [服务器+游戏昵称]：\n  - 查询账号绑定列表：wws [查询/查]绑定/绑定列表 [me/@群友]：\n  - 切换删除绑定账号：wws [切换/删除]绑定 [序号]\n  - 查询账号总体战绩：wws [(服务器+游戏昵称)/@群友/me]\n  - 查询账号历史记录：wws [(服务器+游戏昵称)/@群友/me] record\n  - 查询账号近期战绩：wws [(服务器+游戏昵称)/@群友/me] recent [日期]\n  - 查询单船总体战绩：wws [(服务器+游戏昵称)/@群友/me] ship [船名]\n  - 查询单船近期战绩：wws [(服务器+游戏昵称)/@群友/me] ship [船名] recent [日期]\n  - 查询服务器排行榜：wws [服务器+战舰名] rank/ship.rank\n  - 查询军团详细信息：wws [(服务器+军团名)/@群友/me] clan\n  - 查询军团历史记录：wws [(服务器+军团名)/@群友/me] clan record\n  - 查询舰船中英文名：wws [搜/查船名] [国家][等级][类型]\n  - 检查版本更新：wws 检查更新\n  - 更新：wws 更新Hikari\n  - 查看帮助：wws help\n  - 噗噗：一言\n\n  </details>\n  <details>\n  <summary>点我查看与Hoshino版的区别</summary>\n\n  - Hikari所使用的Nonebot2框架相比Hoshino更易部署，且两者在单环境下不兼容\n  - 一些功能比如频道目前仅支持Hikari\n  - Hoshino的插件生态更偏向PCR，具体可以查看[Nonebot2商店](https://v2.nonebot.dev/store)和[Hoshino插件索引](https://github.com/pcrbot/HoshinoBot-plugins-index)\n  - 由于个人精力原因，主要功能开发和维护面向Hikari，Hoshino版仅做最低限度功能适配\n\n  </details>\n  <details>\n  <summary>点我查看遇到问题如何解决</summary>\n\n  - [ ] 请确认您已按文档中部署流程进行\n  - [ ] 请确认您已完整浏览[可能会遇到的问题](https://github.com/benx1n/HikariBot#%E5%8F%AF%E8%83%BD%E4%BC%9A%E9%81%87%E5%88%B0%E7%9A%84%E9%97%AE%E9%A2%98)，且仍无法自行解决\n  - [ ] [提问的智慧](https://github.com/ryanhanwu/How-To-Ask-Questions-The-Smart-Way/blob/main/README-zh_CN.md)\n  - [ ] 提供系统环境和bot版本，以及出现问题前后至少 10 秒的完整日志内容。请自行删除日志内存在的个人信息及敏感内容\n\n  </details>\n## 在Windows系统上快速部署\n>点我查看[视频教程](https://www.bilibili.com/video/BV1XP411U7rC)\n\n  `windows安装python版本请勿大于3.11,建议版本3.9`\n\n1. 下载Hikari的[最新Release](https://github.com/benx1n/HikariBot/releases/download/Latest/release_windows.zip)并解压到合适文件夹\n2. 复制一份`.env.prod-example`文件，并将其重命名为`.env.prod`,打开并按其中注释编辑\n    >只显示了.env，没有后面的后缀？请百度`windows如何显示文件后缀名`\n    ```\n    API_TOKEN = xxxxxxxx #无需引号，TOKEN即回复您的邮件所带的一串由[数字+冒号+英文/数字]组成的字符串\n    SUPERUSERS=["QQ号"]\n    ```\n   - 最后TOKEN应该长这样 `API_TOKEN = 123764323:ba1f2511fc30423bdbb183fe33`\n   - 从0.3.2.2版本开始，您没有填写的配置将按.env文件中的默认配置执行，具体逻辑为\n      - 私聊、频道默认禁用\n      - 群聊默认开启，默认屏蔽官方交流群\n      - 默认WEB登录账号密码为admin/admin，如有需要请自行修改，无需设置密码请删除env.prod中的配置项\n\n3. 双击`启动.bat`\n    - 页面加载不出请尝试刷新一下，已知IE浏览器可能存在一些问题\n    - 此时若没有报错，您可以在打开的页面`http://127.0.0.1:8080/go-cqhttp/`中\n      点击左侧添加账号，重启bot即可在网页上看到相应信息（大概率需要扫码）\n    - 如果重启后go-cqhhtp一直卡在扫码或无限重启，请跳转[无法使用内嵌go-cqhttp登录](https://github.com/benx1n/HikariBot#%E6%97%A0%E6%B3%95%E4%BD%BF%E7%94%A8%E5%86%85%E5%B5%8Cgo-cqhttp%E7%99%BB%E5%BD%95bot)\n\n## Linux一键脚本\n> 仅支持Debian、CentOS、Ubuntu\n```\nwget -qO - https://fastly.jsdelivr.net/gh/benx1n/HikariBot@master/install.sh | bash\n```\n\n\n## 使用Docker部署\n- Docker目录下是一个简单的Dockerfile，可以基于官方的Python容器封装一个完整的HikariBot\n  - 以`12hydrogen/hikari-bot:latest`上线官方仓库\n- 注意需要将内部的8080端口映射出来\n  ```\n  docker run -d -P 12hydrogen/hikari-bot:latest -t [token] -i [qqid] # 首次使用需输入token和qqid，-P表示将8080端口随机映射至主机\n  docker run -d -p 12345:8080 12hydrogen/hikari-bot:latest -t [token] -i [qqid] # 使用-p以指定映射在外的端口\n  ```\n- 运行上述指令后会在终端显示一串字符，即Docker容器的标识符，一般使用前几位即可唯一确定一个容器\n  ```\n  1a2b3c4d5e..... # 标识符\n  docker stop 1a2b # 使用前四位确定，stop即停止容器\n  1a2b3c4d5e.....\n  docker start 1a2b # start即启动容器\n  1a2b3c4d5e.....\n  docker restart 1a2b # restart即重启容器\n  1a2b3c4d5e.....\n  ```\n- 在更新后即上传新版本容器\n  ```\n  docker pull 12hydrogen/hikari-bot:latest # 更新\n  docker stop 1a2b\n  1a2b...\n  docker run -d --volumes-from 1a2b -P 12hydrogen/hikari-bot:latest -t [token] -i [qqid] # 随机映射\n  or\n  docker run -d --volumes-from 1a2b -p 12345:8080 12hydrogen/hikari-bot:latest -t [token] -i [qqid] # 指定映射\n  9z8y... # 注意标识符变化了\n  docker rm 1a2b # 删除旧容器，\n  1a2b...\n  ```\n- 将配置文件与容器分离\n  使用volume在宿主机保存相关账号信息，更新时按照相关步骤继承volume即可\n\n## 在Windows系统上完整部署\n1. 下载[Git](https://git-scm.com/download/win)、[Python](https://www.python.org/downloads/windows/)并安装\n    >Python版本需>3.8，或参考[Hoshino版插件](https://github.com/benx1n/wows-stats-bot)中使用Conda虚拟环境\n    >\n    >请注意python安装时勾选或点击`添加到环境变量`，可以安装后cmd中输入`python --version`来验证是否成功\n    >\n    >否则请自行百度如何添加python到环境变量\n\n3. 打开一个合适的文件夹，鼠标右键——Git Bash here，输入以下命令（任选一条）克隆本Hikari仓库\n    ```\n    git clone https://github.com/benx1n/HikariBot.git\n\n    git clone https://gitee.com/benx1n/HikariBot.git\n    ```\n3. 以管理员身份运行`一键安装.bat`\n    >等效于在cmd中执行如下代码\n    ```\n    python -m pip install nb-cli hikari-bot nonebot-plugin-apscheduler nonebot-plugin-gocqhttp -i https://pypi.tuna.tsinghua.edu.cn/simple\n    ```\n\n4. 复制一份`.env.prod-example`文件，并将其重命名为`.env.prod`,打开并按其中注释编辑\n    >只显示了.env，没有后面的后缀？请百度`windows如何显示文件后缀名`\n    ```\n    API_TOKEN = xxxxxxxx #无需引号，TOKEN即回复您的邮件所带的一串由[数字+冒号+英文/数字]组成的字符串\n    SUPERUSERS=["QQ号"]\n    ```\n   - 最后TOKEN应该长这样 `API_TOKEN = 123764323:ba1f2511fc30423bdbb183fe33`\n   - 从0.3.2.2版本开始，您没有填写的配置将按.env文件中的默认配置执行，具体逻辑为\n      - 私聊、频道默认禁用\n      - 群聊默认开启，默认屏蔽官方交流群`\n      - 默认WEB登录账号密码为admin/admin，如有需要请自行修改，无需设置密码请删除env.prod中的配置项\n      - 默认开启噗噗\n      - 默认开启缓存上报\n      - 默认关闭代理\n\n5. 双击`启动.bat`，在打开的浏览器中添加bot账号密码，重新启动Hikari\n    - 页面加载不出请尝试刷新一下，已知IE浏览器可能存在一些问题\n    - 此时若没有报错，您可以在打开的页面`http://127.0.0.1:8080/go-cqhttp/`中\n      点击左侧添加账号，重启bot即可在网页上看到相应信息（大概率需要扫码）\n    - 如果重启后go-cqhhtp一直卡在扫码或无限重启，请跳转[无法使用内嵌go-cqhttp登录](https://github.com/benx1n/HikariBot#%E6%97%A0%E6%B3%95%E4%BD%BF%E7%94%A8%E5%86%85%E5%B5%8Cgo-cqhttp%E7%99%BB%E5%BD%95bot)\n\n\n## ~~在Linux上完整部署~~\n- 需要Python基本环境\n- Clone本仓库\n- 使用`./manage.sh`，基于原有批处理脚本\n- 无参数调用以获取使用帮助\n1. `install`\n    - 安装必须的依赖与bot本体\n2. `update`\n    - 更新bot\n3. `start [-t/--token] [token] [-i/--id] [qqid]`\n    - 运行bot\n    - 在当前目录下不存在`.env.prod`的情况下从参数获取token和qqid以创建相应文件，否则直接运行\n    - 考虑到使用Linux部署时多数情况下本地不存在图形界面，有风险的向公网开放访问\n    - 加入验证机制（listed）\n\n\n## 作为已有Bot的插件部署（如真寻、Haruka）\n1. 如果您已经有了一个基于Nonebot2的机器人（例如真寻），您可以直接\n    ```\n    pip install hikari-bot\n    ```\n2. 在bot的bot.py中加入\n    ```\n    nonebot.load_plugin(\'nonebot_plugin_htmlrender\')\n    nonebot.load_plugin(\'hikari_bot\')\n    ```\n3. 在环境文件中加入以下配置项\n    ```\n    API_TOKEN = xxxxxxxxxxxx\n    SUPERUSERS=["QQ号"]\n    private = false                 #开启私聊\n    group = true                    #开启群聊\n    channel = false                 #开启频道\n    all_channel = false             #是否全频道生效，无论此项配置如何，channel_list中的频道一定会开启\n    channel_list = []               #频道列表白名单，数组形式，可在控制台中获取相应的channel_id\n    ban_group_list = [967546463]    #群列表黑名单，默认屏蔽了开发者交流群\n    pupu = true                     #是否开启噗噗\n    check_cache = true              #是否开启缓存上报,可降低高峰期延迟,如果错误日志中频繁报错上报url:XXXXXXXX,请关闭此项或配置代理\n    proxy_on = false                #是否启用代理\n    proxy = http://localhost:7890   #代理地址，如果上面选项开启，这边替换为你本地的\n    ocr_on = true                   #是否开启ocr(识图指令)\n    ocr_offline = false             #是否只使用hash验证，即设置为true后只能识别服务器已记录的图片，如果群较多(>300)导致响应延迟较高可以开启\n    ocr_url = http://mc.youthnp.cn:23338/OCR/           #默认ocr地址，一般不用动\n    ```\n    >一般来说该文件为.env.dev\n    >也有可能是.env.pord，具体需要看.env中是否有指定\n4.   重启bot\n\n## 更新\n实验性更新指令：`wws 更新Hikari`\n请确保在能登录上服务器的情况下使用\n以下是旧更新方法\n1. 按不同版本\n   - Windows一键包：下载最新一键包，复制旧版本中`accounts`文件夹和`env.prod`文件替换至新版文件夹中即可\n   - 完整版：以管理员身份运行`更新.bat`或执行`./manage.sh update`\n      >等效于在cmd中执行如下代码\n      ```\n      pip install --upgrade hikari-bot\n      git pull\n      ```\n   - 插件版：在cmd中执行如下代码\n      ```\n      pip install --upgrade hikari-bot\n      ```\n2. **对比`.env.prod-example`中新增的配置项，并同步至你本地的`env.prod`**\n    - install结束后会打印当前版本\n    - 您也可以通过`pip show hikari-bot`查看当前Hikari版本\n    - 如果没有更新到最新版请等待一会儿，镜像站一般每五分钟同步\n    - 从0.3.2.2版本开始，您没有填写的配置将按.env文件中的默认配置执行，具体逻辑为\n      - 私聊、频道默认禁用\n      - 群聊默认开启，默认屏蔽官方交流群\n\n## 最近的更新日志\n\n### 23-05-07    v0.3.9\n- [+]重构代码\n- [#]替换默认OCR接口\n\n### 23-04-07    v0.3.8\n- [+]新增国服封号记录查询，指令wws ban/wws 封号记录\n- [#]修复了上次修复排行榜新产生的bug\n\n### 23-04-04    v0.3.7\n- [+]添加获取随机表情包，指令wws 随机表情包\n- [+]更新船只选择界面\n- [#]更新Linux脚本托管\n\n### 23-02-22    v0.3.6.4\n- [+]添加随机嘴臭，概率千分之一\n- [+]添加ocr启动报错提示\n- [#]修复一键包及Docker依赖问题 [@94Bo](https://github.com/94Bo) [@12hydrogen](https://github.com/12hydrogen)\n\n### 22-11-18    v0.3.6  包含配置项更新，请添加`env.prod-example`中新增的配置\n- [+]新增噗噗（已于0.3.5.2实装）\n- [+]新增OCR（已于0.3.5.5实装）\n- [+]新增扫雪统计和圣诞船池检查\n- [+]新增国服排行榜\n- [#]大幅优化高峰期响应速度（已于0.3.5.3实装）\n- [#]Linux下支持微软雅黑(已热更新)\n\n### 22-10-29    v0.3.5.5  添加测试功能OCR，支持图片指令\n### 22-10-27    v0.3.5.4  修复一键更新指令bug\n### 22-10-26    v0.3.5.3  添加缓存上报机制，修复噗噗误触发的bug\n### 22-10-25    v0.3.5.2  新增噗噗\n### 22-07-24    v0.3.5  适配nontbo2 v2.0.0rc1  \n### 22-07-24    v0.3.4  **配置项及入口文件更新**  请完整拉取最新仓库，并同步添加`env.prod-example`中新增的配置\n- 重要更新，完整版安装请拉取最新仓库代码，一键包请下载最新版本\n- [+]新增一键更新指令，指令wws 更新Hikari\n- [+]新增Linux一键脚本 [@94Bo](https://github.com/94Bo)\n- [#]修改部分依赖版本\n- [#]大幅改动了模板以适配后续功能\n- [#]修改框架\n- [#]修改接口url\n- [#]修复了没有完全修复的兼容性问题[#11](https://github.com/benx1n/HikariBot/issues/11)\n- [#]修改日志输出等级，现在控制台只会打印SUCCESS级以上的日志\n\n\n\n### 22-07-14    v0.3.3  积累更新\n- [+]新增群聊黑名单，默认屏蔽开发者群"\n- [+]docker添加CI/CD构建发布 [@12hydrogen](https://github.com/12hydrogen)\n- [#]修复与其他插件的兼容性问题\n- [#]更改了请求域名\n- [#]修复manage.sh会更改toml的问题\n- [#]修复了hoshino排行榜选择船只样式问题\n- [#]修复仅打过PVE的单船仍会显示战绩详情的问题\n- [#]info适配v4接口\n- [+]新增配置项ban_group_list\n\n<details>\n<summary><b>更以前的更新日志</b></summary>\n\n### 22-07-05    v0.3.2.2  一些修复\n- [#]修复切换、删除绑定的bug\n- [#]默认配置改为不启用WEB登陆验证\n- [#]修复.bat的环境变量问题 [@94Bo](https://github.com/94Bo)\n\n### 22-07-04    v0.3.2.1  **配置项及入口文件更新**  请完整拉取最新仓库，并同步添加`env.prod-example`中新增的配置\n- [+]新增对QQ频道的适配（非官方bot接入，官方版bot已上线yuyuko频道）\n- [+]新增自定义开启群聊、私聊、QQ频道\n- [+]新增web登录密码\n- [+]新增默认配置项\n- [+]新增PR彩蛋\n- [#]info适配V3接口\n- [#]recent显示时间区间\n\n### 22-06-23    v0.3.1  **重要功能更新**\n- [+]新增单船近期战绩，可显示每日详细信息，指令`wws ship recent`\n- [+]新增docker部署 [@12hydrogen](https://github.com/12hydrogen)\n- [#]修复国服特殊字符ID无法查询的bug\n- [#]修复船只选择过期后发送数字序号仍被识别的bug\n\n### 22-06-15    v0.3.0.1  **重要功能更新**\n- [+]支持显示军团评级颜色\n- [#]排行榜内部逻辑改动，现在仅显示前十，不更新将无法使用\n- [#]\\(hotfix)`wws recent`现在无随机战绩不会显示PR和上方战斗信息\n\n### 22-06-08    v0.2.9.4  **重要功能更新**\n- [+]新增单船的服务器排行，显示在`wws ship`的详情页面下\n- [#]修复0.2.9后无法启动的bug\n- [#]js依赖改为本地\n- [#]修改recent样式，不更新可能会导致错位\n- [#]优化报错提示\n\n### 22-06-03    v0.2.8  一些修复\n- [+]新增删除绑定功能\n- [#]修复`wws ship`总览经验和胜率不上色的bug\n- [#]修复`wws ship`详情只有单野场均被上色的bug\n- [#]修复`wws 查船名`中搜不到德国船的bug\n\n### 22-06-03    v0.2.6  [#]修复`wws recent`胜率颜色的bug\n\n### 22-06-03    v0.2.5  [#]修复`wws recent`击杀显示成命中的bug\n\n### 22-06-03    v0.2.4  **重要功能更新** 否则您将无法使用`wws recent`功能\n- [+]全指令在游戏名外带上括号即可强制指定昵称，以适配一些带有空格、特殊字符、指令字符的昵称\n- [+]新增特殊绑定，请配合网页端食用，复制后发送给Hikari即可一键绑定\n- [+]新增部分报错提示\n- [#]更改ship,rank,recent样式，现在没有战斗场次的类型不会被显示\n- [#]优化Hikari的部署流程\n- [#]修复me大写不被识别的问题\n\n\n### 22-06-02    v0.2.3  一些修复\n- [+]全指令支持大写\n- [#]修复Linux上可能出现的报错\n- [#]修改部分图片的样式\n\n### 22-06-01    v0.2.2  修复了一个VSC导致的依赖错误\n\n### 22-06-01    v0.2.1  修复问题\n\n### 22-06-01    v0.2.0  **重要功能更新**\n- [+]新增排位数据\n- [+]支持国服\n- [+]单船战绩显示单野、自行车、三轮车\n- [+]启用gzip，试图改善请求Timeout\n- [+]增加3s指令CD和每日100次上限\n- [#]修复图片内字符不对称的bug（强迫症）\n- [#]修改未绑定账号时的返回\n- [#]修复网络问题与找不到游戏名时相同返回的bug\n- [#]适配HarukaBot\n\n\n### 22-05-31    v0.1.9  一些修复\n- [#]解决由于QQ风控导致的船只选择列表无法发送的问题\n- [#]修复带非me/@参数查询绑定时引起的报错\n\n### 22-05-30    v0.1.8  **重要更新**\n- [+]所有带请求参数的部分添加log输出以方便查找问题\n- [+]添加平台报错时返回以和Hikari内部错误区分\n- [#]移除bat脚本中的utf8以支持部分英文服务器\n- [#]试图减少因网络导致的报错问题\n\n### 22-05-30    v0.1.7  一些修复\n- [#]修复排行榜查询报错\n- [#]修复部分环境可能出现的单船查询无法选择问题\n\n### 22-05-28    v0.1.6  **重要功能更新**\n- [+]新增排行榜查询 指令`wws rank/ship.rank`\n- [+]新增是否开启内置go-cqhttp，默认开启\n\n### 22-05-28    v0.1.5  一些功能更新\n- [+]添加等级显示，适配新舰船数据\n- [+]新增wws 检查更新\n- [+]配置项添加Bot管理员\n- [#]修复定时任务不触发的bug\n\n### 22-05-27    v0.1.4  一些功能优化\n- [+]添加在windows下的一键安装、更新、启动脚本\n- [#]修复数字ID的recent匹配问题\n- [#]优化提示逻辑\n\n### 22-05-27    v0.1.3  一些修复和适配\n- [+]适配包括真寻等大部分Nonebot2机器人\n- [#]修复自动更新的bug\n\n### 22-05-27    v0.1.2  **调整info接口，不更新无法使用**\n\n### 22-05-27    v0.1.1  一些小改动\n\n### 22-05-27    v0.1.0  一些更新\n- [+]新增定时检查更新\n- [+]新增部署教程\n- [+]添加11级战绩信息\n- [#]优化账号总体和单船图片样式\n\n</details>\n\n## 可能会遇到的问题\n\n### go-cqhttp扫码后提示异地无法登录\n- 一般提示需要扫码，扫码后提示异地无法登录\n- 关于该问题，您可以查看[这里](https://github.com/Mrs4s/go-cqhttp/issues/1469)获得相应解决办法，这里简单列举三种办法\n  - 启动时登录方式选择`浏览器滑条`，按后续提示登录\n  - 手机下载`爱加速`等代理，连接到服务器对应市级地区\n  - 在本地电脑使用go-cqhttp登录成功后，将会在exe同级目录下生成`session.token`和`device.json`两个文件\n  将这两个文件复制到服务器对应目录下并重启\n    - 内嵌go-cqhttp为`account\\QQ号`\n    - 独立go-cqhttp为exe所在同级目录下，请注意使用独立go-cqhttp时需要将`.env.prod`的`USE_PLUGIN_GO_CQHTTP`的值改为`false`\n\n### 无法使用内嵌go-cqhttp登录bot\n\n1. 下载 go-cqhttp 至合适的文件夹\n\n    - github 发布页：https://github.com/Mrs4s/go-cqhttp/releases/latest\n\n    > 您需要根据自己的机器架构选择版本，Windows一般为x86/64架构，通常选择[go-cqhttp_windows_amd64.exe](https://github.com/Mrs4s/go-cqhttp/releases/latest/download/go-cqhttp_windows_amd64.exe)\n\n2. 双击go-cqhttp，提示释出bat，重新运行bat，选择websocket反向代理，go-cqhttp将会在同文件夹内自动创建一个`config.yml`，右键使用notepad++打开，根据注释填写QQ账号密码，并将以下内容写入文件结尾（需替换原有的ws-reverse节点）：\n\n    ```yaml\n      - ws-reverse:\n          universal: ws://127.0.0.1:8080/onebot/v11/ws\n          reconnect-interval: 5000\n          middlewares:\n            <<: *default\n    ```\n\n    > 关于go-cqhttp的配置，你可以在[这里](https://docs.go-cqhttp.org/guide/config.html#%E9%85%8D%E7%BD%AE%E4%BF%A1%E6%81%AF)找到更多说明。\n\n3. 启动go-cqhttp，按照提示登录。\n\n    > 此处如出现异地登陆保护，请尝试\n    > - 在本地电脑使用go-cqhttp登录成功后，将会在exe同级目录下生成`session.token`和`device.json`两个文件\n    > - 将这两个文件复制到服务器对应go-cqhttp目录下并重启\n\n4. 修改Hikari文件夹下.env.prod中`USE_PLUGIN_GO_CQHTTP`的值为`false`\n    ```\n    USE_PLUGIN_GO_CQHTTP = false\n    ```\n5. 在文件夹下打开终端，输入`python bot.py`启动bot\n    - 一键包双击`启动.bat`即可\n\n\n### 出现ZoneInfoNotFoundError报错\n>\n>您可以在[这里](https://github.com/nonebot/nonebot2/issues/78)找到相关解决办法\n>\n### Recent和绑定提示\'鉴权失败\'\n1. 检查Token是否配置正确，token格式为`XXXXX:XXXXXX`\n2. 如果配置正确可能是Token失效了，请重新申请\n\n### \'Config\' Object has no attribute XXXX\n1. 检查视力，重新阅读[更新](https://github.com/benx1n/HikariBot#更新)章节\n\n### Failed to import "nonebot_plugin_guild_patch"\n以下方法任选一种\n- 更新python版本至3.9+\n- 降低Hikari版本至3.1，等待后续版本修复\n- 使用Hikari一键包，其中自带了3.10的python虚拟环境\n- 修改依赖包代码，见[这里](https://github.com/mnixry/nonebot-plugin-guild-patch/pull/6/files)\n\n### Ubuntu系统下部署字体不正常(针对一些云服务器的Ubuntu镜像，不保证成功，只是提供一个解决方案)\n  1. 执行以下命令，完善字体库并将中文设置成默认语言（部分Ubuntu可能不需要该步骤，可直接从第二步开始）\n  ```\n  sudo apt install fonts-noto  \n  sudo locale-gen zh_CN zh_CN.UTF-8  \n  sudo update-locale LC_ALL=zh_CN.UTF-8 LANG=zh_CN.UTF-8  \n  sudo fc-cache -fv\n  ```\n  \n  2. 在你的Windows电脑上打开`C:\\Windows\\fonts`文件夹，找到里面的微软雅黑字体，将其复制出来，放在任意目录，应该会得到`msyh.ttc`，`mshybd.ttc`，`msyhl.ttc`三个文件。（不会有人还用Win7吧？）\n\n  3. 进入到`/usr/share/fonts`文件夹下，创建一个文件夹命名为`msyh`，然后进入其中\n  ```\n  cd /usr/share/fonts \n  sudo mkdir msyh \n  cd msyh\n  ```\n  \n  4. 将三个字体文件上传到`msyh`文件夹中(过程中遇到的问题请自行解决)\n\n  5. 执行以下命令（此时你应该是在`msyh`文件夹下），加载字体\n  ```\n  sudo mkfontscale \n  sudo mkfontdir \n  sudo fc-cache -fv\n  ```\n  \n  6. （可选，若不正常可尝试）重启Hikari。\n\n### 首次启动时plugin-gocqhttp的startup方法报错(traceback中一般还有ssl的错误)\n\n1. 下载 go-cqhttp\n\n    - github 发布页：https://github.com/Mrs4s/go-cqhttp/releases/latest\n\n    > 您需要根据自己的机器架构选择版本，Windows一般为x86/64架构，通常选择[go-cqhttp_windows_amd64.exe](https://github.com/Mrs4s/go-cqhttp/releases/latest/download/go-cqhttp_windows_amd64.exe)\n\n2. 重命名为`go-cqhttp.*`(*为所选择版本后缀,如windowx就是go-cqhttp.exe)并放入`HikariBot\\accounts\\binary`文件夹下\n\n3. 重新启动Hikari\n\n## 贡献代码\n\n请向dev分支提交PR\n\n## 鸣谢\n\n感谢以下开发者及项目做出的贡献与支持\n\n<a href="https://github.com//benx1n/HikariBot/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=benx1n/HikariBot" />\n</a>\n\n[Nonebot2](https://github.com/nonebot/nonebot2)  \n[go-cqhttp](https://github.com/Mrs4s/go-cqhttp)  \n[战舰世界API平台](https://wows.shinoaki.com/)  \n\n## 开源相关\nMIT\n修改、分发代码时请保留原作者相关信息\n',
     'author': 'benx1n',
     'author_email': 'shirakamikanade@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/benx1n/HikariBot',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `hikari_bot-0.3.8.1/PKG-INFO` & `hikari_bot-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-bot
-Version: 0.3.8.1
+Version: 0.3.9
 Summary: Nonebot2 HikariBot,支持战舰世界水表查询
 Home-page: https://github.com/benx1n/HikariBot
 License: MIT
 Keywords: nonebot,nonebot2,qqbot,wows,wws,bot,stats
 Author: benx1n
 Author-email: shirakamikanade@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -19,15 +19,15 @@
 Requires-Dist: httpx (>=0.20.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.0,<3.0.0)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0.1,<0.3.0.0)
 Requires-Dist: nonebot-plugin-reboot (>=0.1.3,<0.2.0)
 Requires-Dist: nonebot2[fastapi] (>=2.0.0-beta.1,<3.0.0)
 Requires-Dist: nonebot_plugin_guild_patch (>=0.2.1,<0.3.0)
-Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
+Requires-Dist: orjson (>=3.8.11,<4.0.0)
 Project-URL: Repository, https://github.com/benx1n/HikariBot
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD041 -->
 <p align="center">
   <a href="https://github.com/benx1n/HikariBot"><img src="https://s2.loli.net/2022/05/28/SFsER8m6TL7jwJ2.png" alt="Hikari " style="width:200px; height:200px" ></a>
 </p>
@@ -292,14 +292,18 @@
     - 如果没有更新到最新版请等待一会儿，镜像站一般每五分钟同步
     - 从0.3.2.2版本开始，您没有填写的配置将按.env文件中的默认配置执行，具体逻辑为
       - 私聊、频道默认禁用
       - 群聊默认开启，默认屏蔽官方交流群
 
 ## 最近的更新日志
 
+### 23-05-07    v0.3.9
+- [+]重构代码
+- [#]替换默认OCR接口
+
 ### 23-04-07    v0.3.8
 - [+]新增国服封号记录查询，指令wws ban/wws 封号记录
 - [#]修复了上次修复排行榜新产生的bug
 
 ### 23-04-04    v0.3.7
 - [+]添加获取随机表情包，指令wws 随机表情包
 - [+]更新船只选择界面
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: hikari-bot Version: 0.3.8.1 Summary: Nonebot2
+Metadata-Version: 2.1 Name: hikari-bot Version: 0.3.9 Summary: Nonebot2
 HikariBot,æ¯ææè°ä¸çæ°´è¡¨æ¥è¯¢ Home-page: https://github.com/benx1n/
 HikariBot License: MIT Keywords: nonebot,nonebot2,qqbot,wows,wws,bot,stats
 Author: benx1n Author-email: shirakamikanade@gmail.com Requires-Python:
 >=3.8.0,<4.0.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: Jinja2 (>=3.0.0,<4.0.0) Requires-Dist:
 beautifulsoup4 (>=4.11.1,<5.0.0) Requires-Dist: httpx (>=0.20.0) Requires-Dist:
 nonebot-adapter-onebot (>=2.1.0,<3.0.0) Requires-Dist: nonebot-plugin-
 apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot-plugin-htmlrender
 (>=0.2.0.1,<0.3.0.0) Requires-Dist: nonebot-plugin-reboot (>=0.1.3,<0.2.0)
 Requires-Dist: nonebot2[fastapi] (>=2.0.0-beta.1,<3.0.0) Requires-Dist:
-nonebot_plugin_guild_patch (>=0.2.1,<0.3.0) Requires-Dist: paho-mqtt
-(>=1.6.1,<2.0.0) Project-URL: Repository, https://github.com/benx1n/HikariBot
+nonebot_plugin_guild_patch (>=0.2.1,<0.3.0) Requires-Dist: orjson
+(>=3.8.11,<4.0.0) Project-URL: Repository, https://github.com/benx1n/HikariBot
 Description-Content-Type: text/markdown
                                    [Hikari_]
                        # Hikari   æè°ä¸çæ°´è¡¨BOT
                 [pypi] [python] [QQ_Chat_Group] [QQ_Channel] #
               ðæ¨ä¸æç®ç»å¯ç±çHikariç¹ä¸ªStaråQAQ
 ## ç®ä» æè°ä¸çæ°´è¡¨BOTï¼åºäºNonebot2 æ°´è¡¨äººï¼åºå»ï¼wws me
 recentï¼ï¼ï¼
@@ -181,17 +181,18 @@
 installç»æåä¼æå°å½åçæ¬ - æ¨ä¹å¯ä»¥éè¿`pip show hikari-
 bot`æ¥çå½åHikariçæ¬ -
 å¦ææ²¡ææ´æ°å°ææ°çè¯·ç­å¾ä¸ä¼å¿ï¼éåç«ä¸è¬æ¯äºåéåæ­¥
 -
 ä»0.3.2.2çæ¬å¼å§ï¼æ¨æ²¡æå¡«åçéç½®å°æ.envæä»¶ä¸­çé»è®¤éç½®æ§è¡ï¼å·ä½é»è¾ä¸º
 - ç§èãé¢éé»è®¤ç¦ç¨ -
 ç¾¤èé»è®¤å¼å¯ï¼é»è®¤å±è½å®æ¹äº¤æµç¾¤ ## æè¿çæ´æ°æ¥å¿ ###
-23-04-07 v0.3.8 - [+]æ°å¢å½æå°å·è®°å½æ¥è¯¢ï¼æä»¤wws ban/wws
-å°å·è®°å½ - [#]ä¿®å¤äºä¸æ¬¡ä¿®å¤æè¡æ¦æ°äº§ççbug ### 23-04-04
-v0.3.7 - [+]æ·»å è·åéæºè¡¨æåï¼æä»¤wws éæºè¡¨æå -
+23-05-07 v0.3.9 - [+]éæä»£ç  - [#]æ¿æ¢é»è®¤OCRæ¥å£ ### 23-04-07
+v0.3.8 - [+]æ°å¢å½æå°å·è®°å½æ¥è¯¢ï¼æä»¤wws ban/wws å°å·è®°å½ -
+[#]ä¿®å¤äºä¸æ¬¡ä¿®å¤æè¡æ¦æ°äº§ççbug ### 23-04-04 v0.3.7 -
+[+]æ·»å è·åéæºè¡¨æåï¼æä»¤wws éæºè¡¨æå -
 [+]æ´æ°è¹åªéæ©çé¢ - [#]æ´æ°Linuxèæ¬æç®¡ ### 23-02-22 v0.3.6.4
 - [+]æ·»å éæºå´è­ï¼æ¦çååä¹ä¸ - [+]æ·»å ocrå¯å¨æ¥éæç¤º -
 [#]ä¿®å¤ä¸é®ååDockerä¾èµé®é¢ [@94Bo](https://github.com/94Bo)
 [@12hydrogen](https://github.com/12hydrogen) ### 22-11-18 v0.3.6
 åå«éç½®é¡¹æ´æ°ï¼è¯·æ·»å `env.prod-example`ä¸­æ°å¢çéç½® -
 [+]æ°å¢ååï¼å·²äº0.3.5.2å®è£ï¼ -
 [+]æ°å¢OCRï¼å·²äº0.3.5.5å®è£ï¼ -
```

