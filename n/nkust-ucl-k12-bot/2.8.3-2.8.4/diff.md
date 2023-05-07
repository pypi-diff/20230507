# Comparing `tmp/nkust-ucl-k12-bot-2.8.3.tar.gz` & `tmp/nkust-ucl-k12-bot-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkust-ucl-k12-bot-2.8.3.tar", last modified: Sun May  7 11:43:54 2023, max compression
+gzip compressed data, was "nkust-ucl-k12-bot-2.8.4.tar", last modified: Sun May  7 11:45:48 2023, max compression
```

## Comparing `nkust-ucl-k12-bot-2.8.3.tar` & `nkust-ucl-k12-bot-2.8.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 11:43:54.698313 nkust-ucl-k12-bot-2.8.3/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.8.3/LICENSE
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     4964 2023-05-07 11:43:54.698063 nkust-ucl-k12-bot-2.8.3/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     4551 2023-05-07 11:43:44.000000 nkust-ucl-k12-bot-2.8.3/README.md
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 11:43:54.694785 nkust-ucl-k12-bot-2.8.3/nkust_ucl/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.8.3/nkust_ucl/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)    10504 2023-05-07 11:23:38.000000 nkust-ucl-k12-bot-2.8.3/nkust_ucl/k12.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 11:43:54.696820 nkust-ucl-k12-bot-2.8.3/nkust_ucl/utils/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.8.3/nkust_ucl/utils/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1021 2023-05-06 17:09:58.000000 nkust-ucl-k12-bot-2.8.3/nkust_ucl/utils/attachment.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.8.3/nkust_ucl/utils/config.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.8.3/nkust_ucl/utils/log.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.8.3/nkust_ucl/utils/mqtt_client.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 11:43:54.697764 nkust-ucl-k12-bot-2.8.3/nkust_ucl_k12_bot.egg-info/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     4964 2023-05-07 11:43:54.000000 nkust-ucl-k12-bot-2.8.3/nkust_ucl_k12_bot.egg-info/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      367 2023-05-07 11:43:54.000000 nkust-ucl-k12-bot-2.8.3/nkust_ucl_k12_bot.egg-info/SOURCES.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-07 11:43:54.000000 nkust-ucl-k12-bot-2.8.3/nkust_ucl_k12_bot.egg-info/dependency_links.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-07 11:43:54.000000 nkust-ucl-k12-bot-2.8.3/nkust_ucl_k12_bot.egg-info/top_level.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-07 11:43:54.698367 nkust-ucl-k12-bot-2.8.3/setup.cfg
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      621 2023-05-07 11:38:40.000000 nkust-ucl-k12-bot-2.8.3/setup.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 11:45:48.535091 nkust-ucl-k12-bot-2.8.4/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.8.4/LICENSE
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     5377 2023-05-07 11:45:48.534841 nkust-ucl-k12-bot-2.8.4/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     4964 2023-05-07 11:45:37.000000 nkust-ucl-k12-bot-2.8.4/README.md
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 11:45:48.532270 nkust-ucl-k12-bot-2.8.4/nkust_ucl/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.8.4/nkust_ucl/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)    10504 2023-05-07 11:23:38.000000 nkust-ucl-k12-bot-2.8.4/nkust_ucl/k12.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 11:45:48.533573 nkust-ucl-k12-bot-2.8.4/nkust_ucl/utils/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.8.4/nkust_ucl/utils/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1021 2023-05-06 17:09:58.000000 nkust-ucl-k12-bot-2.8.4/nkust_ucl/utils/attachment.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.8.4/nkust_ucl/utils/config.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.8.4/nkust_ucl/utils/log.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.8.4/nkust_ucl/utils/mqtt_client.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 11:45:48.534594 nkust-ucl-k12-bot-2.8.4/nkust_ucl_k12_bot.egg-info/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     5377 2023-05-07 11:45:48.000000 nkust-ucl-k12-bot-2.8.4/nkust_ucl_k12_bot.egg-info/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      367 2023-05-07 11:45:48.000000 nkust-ucl-k12-bot-2.8.4/nkust_ucl_k12_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-07 11:45:48.000000 nkust-ucl-k12-bot-2.8.4/nkust_ucl_k12_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-07 11:45:48.000000 nkust-ucl-k12-bot-2.8.4/nkust_ucl_k12_bot.egg-info/top_level.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-07 11:45:48.535151 nkust-ucl-k12-bot-2.8.4/setup.cfg
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      621 2023-05-07 11:45:45.000000 nkust-ucl-k12-bot-2.8.4/setup.py
```

### Comparing `nkust-ucl-k12-bot-2.8.3/LICENSE` & `nkust-ucl-k12-bot-2.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.8.3/PKG-INFO` & `nkust-ucl-k12-bot-2.8.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 2.8.3
+Version: 2.8.4
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -105,15 +105,23 @@
 
 def reply_chatgpt(message):
     message.reply("test")
 
 
 command_handler.register_command("/chatgpt", MsgType.TEXT, reply_chatgpt)
 ```
-
+我們必須在on_processed_message中呼叫command_handler.handle_command來處理指令，這樣就可以在收到指令時呼叫指定的函式
+```python
+@K12.on_processed_message
+def my_custom_on_processed_message(self, chat_msg: ChatMessage):
+    # ... 自定義的 on_processed 行為 ...
+    if chat_msg.send_user_id == "1234567890987654321":
+        return
+    command_handler.handle_command(chat_msg)
+```
 
 ## v2.8.0以前
 ### **初始化 K12 Bot**
 
 ```python
 from nkust_ucl.k12 import BOT as K12
 from nkust_ucl.k12 import MsgType, CommandHandler
```

### Comparing `nkust-ucl-k12-bot-2.8.3/README.md` & `nkust-ucl-k12-bot-2.8.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,23 @@
 
 def reply_chatgpt(message):
     message.reply("test")
 
 
 command_handler.register_command("/chatgpt", MsgType.TEXT, reply_chatgpt)
 ```
-
+我們必須在on_processed_message中呼叫command_handler.handle_command來處理指令，這樣就可以在收到指令時呼叫指定的函式
+```python
+@K12.on_processed_message
+def my_custom_on_processed_message(self, chat_msg: ChatMessage):
+    # ... 自定義的 on_processed 行為 ...
+    if chat_msg.send_user_id == "1234567890987654321":
+        return
+    command_handler.handle_command(chat_msg)
+```
 
 ## v2.8.0以前
 ### **初始化 K12 Bot**
 
 ```python
 from nkust_ucl.k12 import BOT as K12
 from nkust_ucl.k12 import MsgType, CommandHandler
```

### Comparing `nkust-ucl-k12-bot-2.8.3/nkust_ucl/k12.py` & `nkust-ucl-k12-bot-2.8.4/nkust_ucl/k12.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.8.3/nkust_ucl/utils/attachment.py` & `nkust-ucl-k12-bot-2.8.4/nkust_ucl/utils/attachment.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.8.3/nkust_ucl/utils/mqtt_client.py` & `nkust-ucl-k12-bot-2.8.4/nkust_ucl/utils/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.8.3/nkust_ucl_k12_bot.egg-info/PKG-INFO` & `nkust-ucl-k12-bot-2.8.4/nkust_ucl_k12_bot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 2.8.3
+Version: 2.8.4
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -105,15 +105,23 @@
 
 def reply_chatgpt(message):
     message.reply("test")
 
 
 command_handler.register_command("/chatgpt", MsgType.TEXT, reply_chatgpt)
 ```
-
+我們必須在on_processed_message中呼叫command_handler.handle_command來處理指令，這樣就可以在收到指令時呼叫指定的函式
+```python
+@K12.on_processed_message
+def my_custom_on_processed_message(self, chat_msg: ChatMessage):
+    # ... 自定義的 on_processed 行為 ...
+    if chat_msg.send_user_id == "1234567890987654321":
+        return
+    command_handler.handle_command(chat_msg)
+```
 
 ## v2.8.0以前
 ### **初始化 K12 Bot**
 
 ```python
 from nkust_ucl.k12 import BOT as K12
 from nkust_ucl.k12 import MsgType, CommandHandler
```

### Comparing `nkust-ucl-k12-bot-2.8.3/setup.py` & `nkust-ucl-k12-bot-2.8.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nkust-ucl-k12-bot",
-    version="2.8.3",
+    version="2.8.4",
     author="Ethan Cheng",
     author_email="asdewq45445@gmail.com",
     description="一個用於k12的bot包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinbow99/k12-telegram",
     packages=setuptools.find_packages(),
```

