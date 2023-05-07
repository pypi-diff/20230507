# Comparing `tmp/nkust-ucl-k12-bot-2.7.0.tar.gz` & `tmp/nkust-ucl-k12-bot-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkust-ucl-k12-bot-2.7.0.tar", last modified: Sun May  7 08:39:51 2023, max compression
+gzip compressed data, was "nkust-ucl-k12-bot-2.7.1.tar", last modified: Sun May  7 09:02:24 2023, max compression
```

## Comparing `nkust-ucl-k12-bot-2.7.0.tar` & `nkust-ucl-k12-bot-2.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 08:39:51.134932 nkust-ucl-k12-bot-2.7.0/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.7.0/LICENSE
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     4053 2023-05-07 08:39:51.134612 nkust-ucl-k12-bot-2.7.0/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     3640 2023-05-06 17:52:32.000000 nkust-ucl-k12-bot-2.7.0/README.md
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 08:39:51.131396 nkust-ucl-k12-bot-2.7.0/nkust_ucl/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     8517 2023-05-07 08:37:12.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl/k12.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 08:39:51.133472 nkust-ucl-k12-bot-2.7.0/nkust_ucl/utils/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl/utils/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1021 2023-05-06 17:09:58.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl/utils/attachment.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl/utils/config.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl/utils/log.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl/utils/mqtt_client.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 08:39:51.134318 nkust-ucl-k12-bot-2.7.0/nkust_ucl_k12_bot.egg-info/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     4053 2023-05-07 08:39:51.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl_k12_bot.egg-info/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      367 2023-05-07 08:39:51.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl_k12_bot.egg-info/SOURCES.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-07 08:39:51.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl_k12_bot.egg-info/dependency_links.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-07 08:39:51.000000 nkust-ucl-k12-bot-2.7.0/nkust_ucl_k12_bot.egg-info/top_level.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-07 08:39:51.134990 nkust-ucl-k12-bot-2.7.0/setup.cfg
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      621 2023-05-07 08:39:23.000000 nkust-ucl-k12-bot-2.7.0/setup.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 09:02:24.373062 nkust-ucl-k12-bot-2.7.1/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.7.1/LICENSE
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     4053 2023-05-07 09:02:24.372824 nkust-ucl-k12-bot-2.7.1/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     3640 2023-05-06 17:52:32.000000 nkust-ucl-k12-bot-2.7.1/README.md
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 09:02:24.370303 nkust-ucl-k12-bot-2.7.1/nkust_ucl/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.7.1/nkust_ucl/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     8868 2023-05-07 09:01:46.000000 nkust-ucl-k12-bot-2.7.1/nkust_ucl/k12.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 09:02:24.371693 nkust-ucl-k12-bot-2.7.1/nkust_ucl/utils/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.7.1/nkust_ucl/utils/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1021 2023-05-06 17:09:58.000000 nkust-ucl-k12-bot-2.7.1/nkust_ucl/utils/attachment.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.7.1/nkust_ucl/utils/config.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.7.1/nkust_ucl/utils/log.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.7.1/nkust_ucl/utils/mqtt_client.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 09:02:24.372567 nkust-ucl-k12-bot-2.7.1/nkust_ucl_k12_bot.egg-info/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     4053 2023-05-07 09:02:24.000000 nkust-ucl-k12-bot-2.7.1/nkust_ucl_k12_bot.egg-info/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      367 2023-05-07 09:02:24.000000 nkust-ucl-k12-bot-2.7.1/nkust_ucl_k12_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-07 09:02:24.000000 nkust-ucl-k12-bot-2.7.1/nkust_ucl_k12_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-07 09:02:24.000000 nkust-ucl-k12-bot-2.7.1/nkust_ucl_k12_bot.egg-info/top_level.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-07 09:02:24.373117 nkust-ucl-k12-bot-2.7.1/setup.cfg
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      621 2023-05-07 09:02:22.000000 nkust-ucl-k12-bot-2.7.1/setup.py
```

### Comparing `nkust-ucl-k12-bot-2.7.0/LICENSE` & `nkust-ucl-k12-bot-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.7.0/PKG-INFO` & `nkust-ucl-k12-bot-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 2.7.0
+Version: 2.7.1
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nkust-ucl-k12-bot-2.7.0/README.md` & `nkust-ucl-k12-bot-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.7.0/nkust_ucl/k12.py` & `nkust-ucl-k12-bot-2.7.1/nkust_ucl/k12.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,27 @@
 
 from .utils.config import K12Config
 from .utils.mqtt_client import K12MqttClient
 from .utils.attachment import Attachment
 
 from .utils.log import setup_logger
 
+class CommandHandler:
+    def __init__(self):
+        self.commands = {}
+
+    def register_command(self, command, func):
+        self.commands[command] = func
+
+    def handle_command(self, command, *args, **kwargs):
+        if command in self.commands:
+            return self.commands[command](*args, **kwargs)
+        else:
+            return None
+
 class MsgType:
     Text = "Text"
     Image = "Image"
     Audio = "audio"
     Document = "Document"
     Sticker = "Sticker"
```

### Comparing `nkust-ucl-k12-bot-2.7.0/nkust_ucl/utils/attachment.py` & `nkust-ucl-k12-bot-2.7.1/nkust_ucl/utils/attachment.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.7.0/nkust_ucl/utils/mqtt_client.py` & `nkust-ucl-k12-bot-2.7.1/nkust_ucl/utils/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.7.0/nkust_ucl_k12_bot.egg-info/PKG-INFO` & `nkust-ucl-k12-bot-2.7.1/nkust_ucl_k12_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 2.7.0
+Version: 2.7.1
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nkust-ucl-k12-bot-2.7.0/setup.py` & `nkust-ucl-k12-bot-2.7.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nkust-ucl-k12-bot",
-    version="2.7.0",
+    version="2.7.1",
     author="Ethan Cheng",
     author_email="asdewq45445@gmail.com",
     description="一個用於k12的bot包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinbow99/k12-telegram",
     packages=setuptools.find_packages(),
```

