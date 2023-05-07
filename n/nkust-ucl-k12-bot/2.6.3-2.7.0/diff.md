# Comparing `tmp/nkust-ucl-k12-bot-2.6.3.tar.gz` & `tmp/nkust-ucl-k12-bot-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkust-ucl-k12-bot-2.6.3.tar", last modified: Sat May  6 17:53:13 2023, max compression
+gzip compressed data, was "nkust-ucl-k12-bot-2.7.0.tar", last modified: Sun May  7 08:39:51 2023, max compression
```

## Comparing `nkust-ucl-k12-bot-2.6.3.tar` & `nkust-ucl-k12-bot-2.7.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:53:13.216040 nkust-ucl-k12-bot-2.6.3/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.6.3/LICENSE
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     4053 2023-05-06 17:53:13.215781 nkust-ucl-k12-bot-2.6.3/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     3640 2023-05-06 17:52:32.000000 nkust-ucl-k12-bot-2.6.3/README.md
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:53:13.213201 nkust-ucl-k12-bot-2.6.3/nkust_ucl/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     8299 2023-05-06 17:30:29.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl/k12.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:53:13.214825 nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1021 2023-05-06 17:09:58.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/attachment.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/config.py
--rwxr-xr-x   0 zhengshiwen   (501) staff       (20)     3798 2023-05-06 08:05:20.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/handler_sqllite.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/log.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/mqtt_client.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-06 17:53:13.215547 nkust-ucl-k12-bot-2.6.3/nkust_ucl_k12_bot.egg-info/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     4053 2023-05-06 17:53:13.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl_k12_bot.egg-info/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      402 2023-05-06 17:53:13.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl_k12_bot.egg-info/SOURCES.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 17:53:13.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl_k12_bot.egg-info/dependency_links.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-06 17:53:13.000000 nkust-ucl-k12-bot-2.6.3/nkust_ucl_k12_bot.egg-info/top_level.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-06 17:53:13.216156 nkust-ucl-k12-bot-2.6.3/setup.cfg
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      621 2023-05-06 17:52:56.000000 nkust-ucl-k12-bot-2.6.3/setup.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 08:39:51.134932 nkust-ucl-k12-bot-2.7.0/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.7.0/LICENSE
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     4053 2023-05-07 08:39:51.134612 nkust-ucl-k12-bot-2.7.0/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     3640 2023-05-06 17:52:32.000000 nkust-ucl-k12-bot-2.7.0/README.md
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 08:39:51.131396 nkust-ucl-k12-bot-2.7.0/nkust_ucl/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     8517 2023-05-07 08:37:12.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl/k12.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 08:39:51.133472 nkust-ucl-k12-bot-2.7.0/nkust_ucl/utils/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl/utils/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1021 2023-05-06 17:09:58.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl/utils/attachment.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl/utils/config.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl/utils/log.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl/utils/mqtt_client.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 08:39:51.134318 nkust-ucl-k12-bot-2.7.0/nkust_ucl_k12_bot.egg-info/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     4053 2023-05-07 08:39:51.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl_k12_bot.egg-info/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      367 2023-05-07 08:39:51.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl_k12_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-07 08:39:51.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl_k12_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-07 08:39:51.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl_k12_bot.egg-info/top_level.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-07 08:39:51.134990 nkust-ucl-k12-bot-2.7.0/setup.cfg
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      621 2023-05-07 08:39:23.000000 nkust-ucl-k12-bot-2.7.0/setup.py
```

### Comparing `nkust-ucl-k12-bot-2.6.3/LICENSE` & `nkust-ucl-k12-bot-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.6.3/PKG-INFO` & `nkust-ucl-k12-bot-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 2.6.3
+Version: 2.7.0
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nkust-ucl-k12-bot-2.6.3/README.md` & `nkust-ucl-k12-bot-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.6.3/nkust_ucl/k12.py` & `nkust-ucl-k12-bot-2.7.0/nkust_ucl/k12.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from urllib.parse import urlparse
 
 from .utils.config import K12Config
 from .utils.mqtt_client import K12MqttClient
 from .utils.attachment import Attachment
 
 from .utils.log import setup_logger
-from .utils.handler_sqllite import SQLiteHandler
 
 class MsgType:
     Text = "Text"
     Image = "Image"
     Audio = "audio"
     Document = "Document"
     Sticker = "Sticker"
@@ -43,15 +42,16 @@
 
         self.client_msg_history = {}
 
         self.config = K12Config(config_file)
         # 載入設定
         # 這邊是存取資料庫的部分
         bot = self.config.get('bot', {})
-        self.users_db = SQLiteHandler(bot.get('database', 'users.db'))
+        # 防止重複
+        self.duplicate = []
         self.logger.info('K12 database config loaded')
         # 這邊是存取網站的部分
         website = self.config.get('website', {})
         self.host = website['host']
         self.GetMsg = website['GetMsg']
         self.GetMsgHistory = website['GetMsgHistory']
         self.GetContent = website['GetContent']
@@ -187,18 +187,23 @@
 
     def default_on_message(self, client, userdata, msg):
         self.logger.debug(f"Message received: {msg.payload.decode()}")
         data = json.loads(msg.payload.decode())
         self.process_message(data)
     
     def process_message(self, data):
+        _this_msg = ChatMessage(data)
         # 防止重複
-        if self.users_db.add_chat_message(data):
+        if _this_msg.msg_id not in self.duplicate:
+            # 先清空重複訊息的 list，避免 list 過大
+            self.duplicate.clear()
+            # 然後把這個訊息的 msg_id 加入重複訊息的 list，這樣就不會重複處理
+            self.duplicate.append(_this_msg.msg_id)
             self.display_log(data)
-            self.chat_msg = ChatMessage(data)
+            self.chat_msg = _this_msg
             # 當處理完訊息後，呼叫 on_processed_message
             self._on_processed_message(self.chat_msg)
     
     @classmethod
     def on_processed_message(cls, func=None):
         if func:
             cls._on_processed_message = func
```

### Comparing `nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/attachment.py` & `nkust-ucl-k12-bot-2.7.0/nkust_ucl/utils/attachment.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.6.3/nkust_ucl/utils/mqtt_client.py` & `nkust-ucl-k12-bot-2.7.0/nkust_ucl/utils/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.6.3/nkust_ucl_k12_bot.egg-info/PKG-INFO` & `nkust-ucl-k12-bot-2.7.0/nkust_ucl_k12_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 2.6.3
+Version: 2.7.0
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nkust-ucl-k12-bot-2.6.3/setup.py` & `nkust-ucl-k12-bot-2.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nkust-ucl-k12-bot",
-    version="2.6.3",
+    version="2.7.0",
     author="Ethan Cheng",
     author_email="asdewq45445@gmail.com",
     description="一個用於k12的bot包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinbow99/k12-telegram",
     packages=setuptools.find_packages(),
```

