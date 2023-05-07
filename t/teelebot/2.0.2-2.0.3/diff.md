# Comparing `tmp/teelebot-2.0.2-py3-none-any.whl.zip` & `tmp/teelebot-2.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 36587 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat     4126 b- defN 23-May-06 02:35 teelebot/__init__.py
+Zip file size: 36814 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat     4126 b- defN 23-May-07 14:53 teelebot/__init__.py
 -rw-rw-rw-  2.0 fat      159 b- defN 23-May-03 15:15 teelebot/__main__.py
--rw-rw-rw-  2.0 fat    27873 b- defN 23-May-06 02:39 teelebot/bot.py
+-rw-rw-rw-  2.0 fat    27942 b- defN 23-May-07 16:23 teelebot/bot.py
 -rw-rw-rw-  2.0 fat     7366 b- defN 23-May-03 18:10 teelebot/buffer.py
--rw-rw-rw-  2.0 fat    19351 b- defN 23-May-06 02:33 teelebot/handler.py
+-rw-rw-rw-  2.0 fat    19377 b- defN 23-May-07 16:46 teelebot/handler.py
 -rw-rw-rw-  2.0 fat     1807 b- defN 23-May-03 00:00 teelebot/logger.py
 -rw-rw-rw-  2.0 fat      721 b- defN 23-May-03 00:01 teelebot/polling.py
--rw-rw-rw-  2.0 fat     3700 b- defN 23-May-06 02:37 teelebot/request.py
+-rw-rw-rw-  2.0 fat     3700 b- defN 23-May-07 14:53 teelebot/request.py
 -rw-rw-rw-  2.0 fat     3895 b- defN 23-May-06 02:35 teelebot/schedule.py
--rw-rw-rw-  2.0 fat      482 b- defN 23-May-06 02:22 teelebot/version.py
+-rw-rw-rw-  2.0 fat      482 b- defN 23-May-07 16:51 teelebot/version.py
 -rw-rw-rw-  2.0 fat     2665 b- defN 23-May-03 15:18 teelebot/webhook.py
--rw-rw-rw-  2.0 fat    35823 b- defN 23-May-06 03:07 teelebot-2.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     8492 b- defN 23-May-06 03:07 teelebot-2.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 03:07 teelebot-2.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       43 b- defN 23-May-06 03:07 teelebot-2.0.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-06 03:07 teelebot-2.0.2.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-May-06 03:07 teelebot-2.0.2.dist-info/zip-safe
--rw-rw-r--  2.0 fat     1406 b- defN 23-May-06 03:07 teelebot-2.0.2.dist-info/RECORD
-18 files, 118012 bytes uncompressed, 34309 bytes compressed:  70.9%
+-rw-rw-rw-  2.0 fat    35823 b- defN 23-May-07 16:54 teelebot-2.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9052 b- defN 23-May-07 16:54 teelebot-2.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-07 16:54 teelebot-2.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       43 b- defN 23-May-07 16:54 teelebot-2.0.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-07 16:54 teelebot-2.0.3.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-May-07 16:54 teelebot-2.0.3.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     1406 b- defN 23-May-07 16:54 teelebot-2.0.3.dist-info/RECORD
+18 files, 118667 bytes uncompressed, 34536 bytes compressed:  70.9%
```

## zipnote {}

```diff
@@ -27,29 +27,29 @@
 
 Filename: teelebot/version.py
 Comment: 
 
 Filename: teelebot/webhook.py
 Comment: 
 
-Filename: teelebot-2.0.2.dist-info/LICENSE
+Filename: teelebot-2.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: teelebot-2.0.2.dist-info/METADATA
+Filename: teelebot-2.0.3.dist-info/METADATA
 Comment: 
 
-Filename: teelebot-2.0.2.dist-info/WHEEL
+Filename: teelebot-2.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: teelebot-2.0.2.dist-info/entry_points.txt
+Filename: teelebot-2.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: teelebot-2.0.2.dist-info/top_level.txt
+Filename: teelebot-2.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: teelebot-2.0.2.dist-info/zip-safe
+Filename: teelebot-2.0.3.dist-info/zip-safe
 Comment: 
 
-Filename: teelebot-2.0.2.dist-info/RECORD
+Filename: teelebot-2.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## teelebot/bot.py

```diff
@@ -1,14 +1,14 @@
 # -*- coding:utf-8 -*-
 """
 @description:基于Telegram Bot Api 的机器人框架
 @creation date: 2019-08-13
-@last modification: 2023-05-06
+@last modification: 2023-05-08
 @author: Pluto (github:plutobell)
-@version: 2.0.2
+@version: 2.0.3
 """
 import time
 import sys
 import os
 import types
 import string
 import random
@@ -209,16 +209,17 @@
 
             for plugin in list(self.__non_plugin_list):
                 if plugin not in list(now_non_plugin_list):
                     _logger.info("The plugin " + plugin + " has been uninstalled")
                     self.__non_plugin_info.pop(plugin)
 
                     if (self.__plugin_dir + plugin) in sys.path:
-                        sys.modules.pop(self.__plugin_dir + plugin)
                         sys.path.remove(self.__plugin_dir + plugin)
+                    if (self.__plugin_dir + plugin) in sys.modules:
+                        sys.modules.pop(self.__plugin_dir + plugin)
 
             self.__non_plugin_list = now_non_plugin_list
 
     def __control_plugin(self, plugin_bridge, chat_type, chat_id):
         if chat_type != "private" and "PluginCTL" in plugin_bridge.keys() \
                 and plugin_bridge["PluginCTL"] == "/pluginctl":
             if os.path.exists(self.path_converter(self.__plugin_dir + "PluginCTL/db/" + str(chat_id) + ".db")):
```

## teelebot/handler.py

```diff
@@ -1,11 +1,11 @@
 # -*- coding:utf-8 -*-
 '''
 @creation date: 2019-08-23
-@last modification: 2023-05-06
+@last modification: 2023-05-08
 '''
 import configparser
 import argparse
 import os
 import sys
 import shutil
 import requests
@@ -17,31 +17,31 @@
 common_pkg_prefix = "~~"
 inline_mode_prefix = "?:"
 
 parser = argparse.ArgumentParser(description="teelebot console command list")
 parser.add_argument("-c", "--config", type=str,
                     help="specify the configuration file")
 parser.add_argument("-k", "--key", type=str,
-                    help="specify the bot key")
+                    help="specify the bot api token")
 parser.add_argument("-r", "--root", type=str,
-                    help="specify the root user id")
+                    help="specify the telegram user user_id of bot admin")
 parser.add_argument("-p", "--plugin", type=str,
                     help="specify the plugin path")
 parser.add_argument("-mp", "--make_plugin", type=str,
                     help="create a plugin template")
 parser.add_argument("-L", "--logout",
-                    help="use it to log out from the cloud Bot API server before launching the bot locally.",
+                    help="use it to log out from the cloud Bot API server before launching the bot locally",
                     action="store_true")
 parser.add_argument("-C", "--close",
-                    help="use it to close the bot instance before moving it from one local server to another.",
+                    help="use it to close the bot instance before moving it from one local server to another",
                     action="store_true")
 parser.add_argument(
     "-d", "--debug", help="run teelebot in debug mode", action="store_true")
 parser.add_argument(
-    "-v", "--version", help="view the current version of teelebot", action="store_true")
+    "-v", "--version", help="show the current version of teelebot", action="store_true")
 args = parser.parse_args()
 
 if len(sys.argv) == 2 and args.version:
     print("\nVersion: " + __version__)
     print("Author: " + __author__)
     print("Project: " + __github__)
     os._exit(0)
```

## teelebot/version.py

```diff
@@ -1,17 +1,17 @@
 # -*- coding:utf-8 -*-
 """
 @description:基于Telegram Bot Api 的机器人框架
 @creation date: 2019-11-15
-@last modification: 2023-05-06
+@last modification: 2023-05-08
 @author: Pluto (github:plutobell)
-@version: 2.0.2
+@version: 2.0.3
 """
 
-__version__ = "2.0.2"
+__version__ = "2.0.3"
 __author__ = "Pluto"
 __email__ = "hi@ojoll.com"
 __blog__ = "https://ojoll.com"
 __github__ = "https://github.com/plutobell/teelebot"
 __description__ = "teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend."
```

## Comparing `teelebot-2.0.2.dist-info/LICENSE` & `teelebot-2.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `teelebot-2.0.2.dist-info/METADATA` & `teelebot-2.0.3.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teelebot
-Version: 2.0.2
+Version: 2.0.3
 Summary: teelebot is a robot framework based on Telegram Bot API, with plug-in system, easy to extend.
 Home-page: https://ojoll.com
 Author: Pluto
 Author-email: hi@ojoll.com
 License: GPLv3
 Keywords: teelebot telegram bot telegram bot api telegram
 Classifier: Programming Language :: Python :: 3
@@ -183,14 +183,16 @@
 
 
 
 #### 一、运行模式
 
 `teelebot` 支持以 `Webhook` 模式和 `Polling` 模式运行。生产环境推荐使用 `Webhook` 模式，而 `Polling` 则仅用于开发环境。
 
+
+
 ##### 1、Webhook 模式
 
 要以 `Webhook` 模式运行，请将配置文件字段 `webhook` 设置为 `True` ，此模式涉及的配置文件字段如下：
 
 ```python
 [config]
 webhook=True
@@ -201,28 +203,28 @@
 server_port=your server port
 local_address=webhook local address
 local_port=webhook local port
 ```
 
 `self_signed` 用于设置是否使用自签名证书，而 `cert_key` 和 `cert_pub` 则是你的证书路径(绝对路径)，`server_address` 为你的服务器公网IP, `server_port` 为服务器的端口(目前 telegram 官方仅支持 443,  80,  88,  8443)，`local_address` 为Webhook 本地监听地址， `local_port` 为 Webhook 本地运行的端口。
 
-推荐搭配 `nginx` 使用，自签名证书生成请参考：[Generating a self-signed certificate pair (PEM)](https://core.telegram.org/bots/self-signed#generating-a-self-signed-certificate-pair-pem)
+自签名证书生成请参考：[Generating a self-signed certificate pair (PEM)](https://core.telegram.org/bots/self-signed#generating-a-self-signed-certificate-pair-pem)
 
 
 
 ##### 2、Polling 模式
 
 要以 Polling 模式运行，只需要保证配置文件 `webhook` 字段为 `False` 即可。此模式最基本的配置文件如下:
 
 ```
 [config]
 key=bot key
+root_id=your user id
 pool_size=40
 webhook=False
-root_id=your user id
 debug=False
 plugin_dir=your plugin dir
 ```
 
 
 
 
@@ -235,48 +237,74 @@
 
 - 对于使用程序配置文件默认路径的：
 
   输入`teelebot` 回车,正常情况下你应该能看见屏幕提示机器人开始运行。
 
 - 对于命令行手动指定配置文件路径的：
 
-  输入`teelebot -c/--config <configure file path>` 回车,正常情况下你应该能看见屏幕提示机器人开始运行。**(更多指令请通过 `-h/--help` 查看)**
-
+  输入`teelebot -c/--config <configure file path>` 回车,正常情况下你应该能看见屏幕提示机器人开始运行。
+  
+  **更多指令请通过 `-h/--help` 查看：**
+  
+  ```bash
+  usage: -m [-h] [-c CONFIG] [-k KEY] [-r ROOT] [-p PLUGIN] [-mp MAKE_PLUGIN]
+            [-L] [-C] [-d] [-v]
+  
+  teelebot console command list
+  
+  options:
+    -h, --help            show this help message and exit
+    -c CONFIG, --config CONFIG
+                          specify the configuration file
+    -k KEY, --key KEY     specify the bot api token
+    -r ROOT, --root ROOT  specify the telegram user user_id of bot admin
+    -p PLUGIN, --plugin PLUGIN
+                          specify the plugin path
+    -mp MAKE_PLUGIN, --make_plugin MAKE_PLUGIN
+                          create a plugin template
+    -L, --logout          use it to log out from the cloud Bot API server before
+                          launching the bot locally
+    -C, --close           use it to close the bot instance before moving it from
+                          one local server to another
+    -d, --debug           run teelebot in debug mode
+    -v, --version         show the current version of teelebot
+  ```
+  
+  
 
 
-可配合`supervisor`使用。
 
 
 
 
 
 #### 三、配置文件
 
 **完整的配置文件**如下所示:
 
 ```python
 [config]
 key=bot key
+root_id=your user id
 plugin_dir=your plugin dir
 pool_size=40 # the thread pool size, default 40, range(1, 101)
 buffer_size=16 # the buffer area size, default 16(MB)
 webhook=False
 self_signed=False # Optional while webhook is False
 cert_key=your private cert path # Optional while webhook is False
 cert_pub=your public cert path # Optional while webhook is False
 server_ip=your server ip address # Optional while webhook is False
 server_port=your server port # Optional while webhook is False
 local_address=webhook local address # Optional while webhook is False
 local_port=webhook local port # Optional while webhook is False
-root_id=your user id
 debug=False
 drop_pending_updates=False
 local_api_server=local api server address # [Optional]
 updates_chat_member=False # [Optional]
-proxy = socks5h://user:pass@host:port # [Optional]
+proxy=socks5h://user:pass@host:port # [Optional]
 ```
 
 **在 `1.13.0` 及以上版本，支持自动生成配置文件。（默认为Polling模式）**
 
 1.在命令行未指定配置文件路径的情况下，会在默认配置文件路径下不存在配置文件时自动生成配置文件 `config.cfg`。
 
 * 在Linux下，会自动在用户目录下创建文件夹 `.teelebot` ，并生成配置文件 `config.cfg`
@@ -287,25 +315,15 @@
 
 Linux 和 Windows 都可在命令行通过参数手动指定配置文件路径，命令格式：
 
 ```
 teelebot -c/--config <configure file path>
 ```
 
-路径必须为绝对路径，此情况下也会在指定路径上不存在配置文件时自动生成配置文件 ，配置文件命名由指定的路径决定。
-
-**Tip: 自动生成的配置文件未设置这几个字段值：`key`、`root_id`、`plugin_dir`，key 和 root_id 为必须，但我们仍然可以通过命令行设置他们：**
-
-```
-teelebot -c/--config <config file path> -k/--key <bot key> -r/--root <your user id>
-```
-
-**使用以上命令会以Polling模式运行框架，而无需困扰于处理配置文件。**
-
-**之后请手动设置 ``plugin_dir``** 。
+路径必须为绝对路径，并且配置文件名也应当包含在路径内，此情况下会在指定的配置文件不存在时自动生成配置文件 。
 
 
 
 
 
 ## 联系我
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: teelebot Version: 2.0.2 Summary: teelebot is a
+Metadata-Version: 2.1 Name: teelebot Version: 2.0.3 Summary: teelebot is a
 robot framework based on Telegram Bot API, with plug-in system, easy to extend.
 Home-page: https://ojoll.com Author: Pluto Author-email: hi@ojoll.com License:
 GPLv3 Keywords: teelebot telegram bot telegram bot api telegram Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Requires-Python: >=3.6 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests
@@ -60,53 +60,56 @@
 server_port=your server port local_address=webhook local address
 local_port=webhook local port ``` `self_signed`
 ç¨äºè®¾ç½®æ¯å¦ä½¿ç¨èªç­¾åè¯ä¹¦ï¼è `cert_key` å `cert_pub`
 åæ¯ä½ çè¯ä¹¦è·¯å¾(ç»å¯¹è·¯å¾)ï¼`server_address`
 ä¸ºä½ çæå¡å¨å¬ç½IP, `server_port` ä¸ºæå¡å¨çç«¯å£(ç®å telegram
 å®æ¹ä»æ¯æ 443, 80, 88, 8443)ï¼`local_address` ä¸ºWebhook
 æ¬å°çå¬å°åï¼ `local_port` ä¸º Webhook æ¬å°è¿è¡çç«¯å£ã
-æ¨èæ­é `nginx` ä½¿ç¨ï¼èªç­¾åè¯ä¹¦çæè¯·åèï¼[Generating a
-self-signed certificate pair (PEM)](https://core.telegram.org/bots/self-
-signed#generating-a-self-signed-certificate-pair-pem) ##### 2ãPolling æ¨¡å¼
-è¦ä»¥ Polling æ¨¡å¼è¿è¡ï¼åªéè¦ä¿è¯éç½®æä»¶ `webhook` å­æ®µä¸º
-`False` å³å¯ãæ­¤æ¨¡å¼æåºæ¬çéç½®æä»¶å¦ä¸: ``` [config] key=bot
-key pool_size=40 webhook=False root_id=your user id debug=False plugin_dir=your
+èªç­¾åè¯ä¹¦çæè¯·åèï¼[Generating a self-signed certificate pair
+(PEM)](https://core.telegram.org/bots/self-signed#generating-a-self-signed-
+certificate-pair-pem) ##### 2ãPolling æ¨¡å¼ è¦ä»¥ Polling
+æ¨¡å¼è¿è¡ï¼åªéè¦ä¿è¯éç½®æä»¶ `webhook` å­æ®µä¸º `False`
+å³å¯ãæ­¤æ¨¡å¼æåºæ¬çéç½®æä»¶å¦ä¸: ``` [config] key=bot key
+root_id=your user id pool_size=40 webhook=False debug=False plugin_dir=your
 plugin dir ``` #### äºãè¿è¡
 ä»»æè·¯å¾æå¼ç»ç«¯ï¼è¾å¥ä»¥ä¸å½ä»¤ï¼ -
 å¯¹äºä½¿ç¨ç¨åºéç½®æä»¶é»è®¤è·¯å¾çï¼ è¾å¥`teelebot`
 åè½¦,æ­£å¸¸æåµä¸ä½ åºè¯¥è½çè§å±å¹æç¤ºæºå¨äººå¼å§è¿è¡ã -
 å¯¹äºå½ä»¤è¡æå¨æå®éç½®æä»¶è·¯å¾çï¼ è¾å¥`teelebot -c/--config
-`
-åè½¦,æ­£å¸¸æåµä¸ä½ åºè¯¥è½çè§å±å¹æç¤ºæºå¨äººå¼å§è¿è¡ã**
-(æ´å¤æä»¤è¯·éè¿ `-h/--help` æ¥ç)** å¯éå`supervisor`ä½¿ç¨ã
-#### ä¸ãéç½®æä»¶ **å®æ´çéç½®æä»¶**å¦ä¸æç¤º: ```python
-[config] key=bot key plugin_dir=your plugin dir pool_size=40 # the thread pool
+` åè½¦,æ­£å¸¸æåµä¸ä½ åºè¯¥è½çè§å±å¹æç¤ºæºå¨äººå¼å§è¿è¡ã
+**æ´å¤æä»¤è¯·éè¿ `-h/--help` æ¥çï¼** ```bash usage: -m [-h] [-
+c CONFIG] [-k KEY] [-r ROOT] [-p PLUGIN] [-mp MAKE_PLUGIN] [-L] [-C] [-d] [-v]
+teelebot console command list options: -h, --help show this help message and
+exit -c CONFIG, --config CONFIG specify the configuration file -k KEY, --key
+KEY specify the bot api token -r ROOT, --root ROOT specify the telegram user
+user_id of bot admin -p PLUGIN, --plugin PLUGIN specify the plugin path -mp
+MAKE_PLUGIN, --make_plugin MAKE_PLUGIN create a plugin template -L, --logout
+use it to log out from the cloud Bot API server before launching the bot
+locally -C, --close use it to close the bot instance before moving it from one
+local server to another -d, --debug run teelebot in debug mode -v, --version
+show the current version of teelebot ``` #### ä¸ãéç½®æä»¶
+**å®æ´çéç½®æä»¶**å¦ä¸æç¤º: ```python [config] key=bot key
+root_id=your user id plugin_dir=your plugin dir pool_size=40 # the thread pool
 size, default 40, range(1, 101) buffer_size=16 # the buffer area size, default
 16(MB) webhook=False self_signed=False # Optional while webhook is False
 cert_key=your private cert path # Optional while webhook is False cert_pub=your
 public cert path # Optional while webhook is False server_ip=your server ip
 address # Optional while webhook is False server_port=your server port #
 Optional while webhook is False local_address=webhook local address # Optional
 while webhook is False local_port=webhook local port # Optional while webhook
-is False root_id=your user id debug=False drop_pending_updates=False
-local_api_server=local api server address # [Optional]
-updates_chat_member=False # [Optional] proxy = socks5h://user:pass@host:port #
-[Optional] ``` **å¨ `1.13.0`
+is False debug=False drop_pending_updates=False local_api_server=local api
+server address # [Optional] updates_chat_member=False # [Optional]
+proxy=socks5h://user:pass@host:port # [Optional] ``` **å¨ `1.13.0`
 åä»¥ä¸çæ¬ï¼æ¯æèªå¨çæéç½®æä»¶ãï¼é»è®¤ä¸ºPollingæ¨¡å¼ï¼**
 1.å¨å½ä»¤è¡æªæå®éç½®æä»¶è·¯å¾çæåµä¸ï¼ä¼å¨é»è®¤éç½®æä»¶è·¯å¾ä¸ä¸å­å¨éç½®æä»¶æ¶èªå¨çæéç½®æä»¶
 `config.cfg`ã * å¨Linuxä¸ï¼ä¼èªå¨å¨ç¨æ·ç®å½ä¸åå»ºæä»¶å¤¹
 `.teelebot` ï¼å¹¶çæéç½®æä»¶ `config.cfg` * å¨Windowsä¸ï¼åä¼å¨
 `C:\Users\` ç®å½ä¸åå»ºæä»¶å¤¹ `.teelebot` ï¼å¹¶çæéç½®æä»¶
 `config.cfg` 2.æå®éç½®æä»¶ Linux å Windows
 é½å¯å¨å½ä»¤è¡éè¿åæ°æå¨æå®éç½®æä»¶è·¯å¾ï¼å½ä»¤æ ¼å¼ï¼
 ``` teelebot -c/--config  ```
-è·¯å¾å¿é¡»ä¸ºç»å¯¹è·¯å¾ï¼æ­¤æåµä¸ä¹ä¼å¨æå®è·¯å¾ä¸ä¸å­å¨éç½®æä»¶æ¶èªå¨çæéç½®æä»¶
-ï¼éç½®æä»¶å½åç±æå®çè·¯å¾å³å®ã **Tip:
-èªå¨çæçéç½®æä»¶æªè®¾ç½®è¿å ä¸ªå­æ®µå¼ï¼`key`ã`root_id`ã`plugin_dir`ï¼key
-å root_id ä¸ºå¿é¡»ï¼ä½æä»¬ä»ç¶å¯ä»¥éè¿å½ä»¤è¡è®¾ç½®ä»ä»¬ï¼**
-``` teelebot -c/--config  -k/--key  -r/--root  ```
-**ä½¿ç¨ä»¥ä¸å½ä»¤ä¼ä»¥Pollingæ¨¡å¼è¿è¡æ¡æ¶ï¼èæ éå°æ°äºå¤çéç½®æä»¶ã**
-**ä¹åè¯·æå¨è®¾ç½® ``plugin_dir``** ã ## èç³»æ *
-Emailï¼hi#ojoll.com ( # == @ ) * Blog: [åå](https://ojoll.com) * Telegram
-Groupï¼[teelebot official](https://t.me/teelebot_official)ï¼t.me/
-teelebot_officialï¼ * ~~Telegram Groupï¼[teelebotä½éªç¾¤](http://t.me/
-teelebot_chat)ï¼t.me/teelebot_chatï¼~~ * å¶ä»ï¼æ¬repo ç Issue
+è·¯å¾å¿é¡»ä¸ºç»å¯¹è·¯å¾ï¼å¹¶ä¸éç½®æä»¶åä¹åºå½åå«å¨è·¯å¾åï¼æ­¤æåµä¸ä¼å¨æå®çéç½®æä»¶ä¸å­å¨æ¶èªå¨çæéç½®æä»¶
+ã ## èç³»æ * Emailï¼hi#ojoll.com ( # == @ ) * Blog: [åå](https://
+ojoll.com) * Telegram Groupï¼[teelebot official](https://t.me/
+teelebot_official)ï¼t.me/teelebot_officialï¼ * ~~Telegram Groupï¼
+[teelebotä½éªç¾¤](http://t.me/teelebot_chat)ï¼t.me/teelebot_chatï¼~~ *
+å¶ä»ï¼æ¬repo ç Issue
```

## Comparing `teelebot-2.0.2.dist-info/RECORD` & `teelebot-2.0.3.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 teelebot/__init__.py,sha256=_RulqeVSYAqRhTaljCZfWctBfVdmjCIC8Qp-ewpeOY4,4126
 teelebot/__main__.py,sha256=s_E7-RSOfVOZx7c84WupirrRB3zuMwtNDqi6o2Ij0Ko,159
-teelebot/bot.py,sha256=4DGnew7P4Wj9uleJ-L5vANucdJ9BBf5RqDrGXwsln-g,27873
+teelebot/bot.py,sha256=C8eLh2B3l1GxjnHpQtObZL0vqcFkBEcxRJC6y4fkwzs,27942
 teelebot/buffer.py,sha256=yn0CBGUbPBbXmERjMTuCeKZaM_y7H0gPsJbrxiRKliY,7366
-teelebot/handler.py,sha256=FcyTT6iOMrCCrfaaJAuBunsMlmAqWkVbD5zCGJrVPhc,19351
+teelebot/handler.py,sha256=ZPVuqeat6bIenPQL9AjAcYbyQ190ElELecKuVdznwX4,19377
 teelebot/logger.py,sha256=_QWA2Kbj-JWNYDtgeK6IE7q34Brxrq6cUgHEH4YTu2M,1807
 teelebot/polling.py,sha256=7lPDDeVInhk8MH-ZQhzGXYW-uI5t-F0XtMYkMrcEDEU,721
 teelebot/request.py,sha256=aYrdPV-IRJPdiZgZlIjU4es8QokOzs8Jn_bZVd_aI3I,3700
 teelebot/schedule.py,sha256=zMozNsMfsm__ss7samHDmpjXuAyrdBxTQOU1f5wcXXo,3895
-teelebot/version.py,sha256=GG5q0QfBrXWWYc4hLvoftH8p-V8k9MZoSnl6zfXLGAo,482
+teelebot/version.py,sha256=POwd5wx29VzhhtkRfLzgojqDv4-6vjVKIL_FafJfhK8,482
 teelebot/webhook.py,sha256=IomyaLxak_caDNYKNnLaTLtqkFToYq4sHWsD7kahV4Y,2665
-teelebot-2.0.2.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
-teelebot-2.0.2.dist-info/METADATA,sha256=eZ8fmu4OoAe_kQrMLXOPI41Uk_JCYlHoIoCqr67m_Qk,8492
-teelebot-2.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-teelebot-2.0.2.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
-teelebot-2.0.2.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
-teelebot-2.0.2.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-teelebot-2.0.2.dist-info/RECORD,,
+teelebot-2.0.3.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
+teelebot-2.0.3.dist-info/METADATA,sha256=NTpVnOuWUtZTfOj4tfTmlyyFOEI_Oq7APIKCwUUXbFI,9052
+teelebot-2.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+teelebot-2.0.3.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
+teelebot-2.0.3.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
+teelebot-2.0.3.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+teelebot-2.0.3.dist-info/RECORD,,
```

