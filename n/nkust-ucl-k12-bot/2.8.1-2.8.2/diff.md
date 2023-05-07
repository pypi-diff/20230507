# Comparing `tmp/nkust-ucl-k12-bot-2.8.1.tar.gz` & `tmp/nkust-ucl-k12-bot-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkust-ucl-k12-bot-2.8.1.tar", last modified: Sun May  7 11:29:38 2023, max compression
+gzip compressed data, was "nkust-ucl-k12-bot-2.8.2.tar", last modified: Sun May  7 11:32:02 2023, max compression
```

## Comparing `nkust-ucl-k12-bot-2.8.1.tar` & `nkust-ucl-k12-bot-2.8.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 11:29:38.382881 nkust-ucl-k12-bot-2.8.1/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.8.1/LICENSE
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     4053 2023-05-07 11:29:38.382640 nkust-ucl-k12-bot-2.8.1/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     3640 2023-05-06 17:52:32.000000 nkust-ucl-k12-bot-2.8.1/README.md
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 11:29:38.379603 nkust-ucl-k12-bot-2.8.1/nkust_ucl/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.8.1/nkust_ucl/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)    10504 2023-05-07 11:23:38.000000 nkust-ucl-k12-bot-2.8.1/nkust_ucl/k12.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 11:29:38.381590 nkust-ucl-k12-bot-2.8.1/nkust_ucl/utils/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.8.1/nkust_ucl/utils/__init__.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     1021 2023-05-06 17:09:58.000000 nkust-ucl-k12-bot-2.8.1/nkust_ucl/utils/attachment.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.8.1/nkust_ucl/utils/config.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.8.1/nkust_ucl/utils/log.py
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.8.1/nkust_ucl/utils/mqtt_client.py
-drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 11:29:38.382395 nkust-ucl-k12-bot-2.8.1/nkust_ucl_k12_bot.egg-info/
--rw-r--r--   0 zhengshiwen   (501) staff       (20)     4053 2023-05-07 11:29:38.000000 nkust-ucl-k12-bot-2.8.1/nkust_ucl_k12_bot.egg-info/PKG-INFO
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      367 2023-05-07 11:29:38.000000 nkust-ucl-k12-bot-2.8.1/nkust_ucl_k12_bot.egg-info/SOURCES.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-07 11:29:38.000000 nkust-ucl-k12-bot-2.8.1/nkust_ucl_k12_bot.egg-info/dependency_links.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-07 11:29:38.000000 nkust-ucl-k12-bot-2.8.1/nkust_ucl_k12_bot.egg-info/top_level.txt
--rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-07 11:29:38.382936 nkust-ucl-k12-bot-2.8.1/setup.cfg
--rw-r--r--   0 zhengshiwen   (501) staff       (20)      621 2023-05-07 11:29:10.000000 nkust-ucl-k12-bot-2.8.1/setup.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 11:32:02.940982 nkust-ucl-k12-bot-2.8.2/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1077 2023-05-06 09:22:13.000000 nkust-ucl-k12-bot-2.8.2/LICENSE
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     4053 2023-05-07 11:32:02.940773 nkust-ucl-k12-bot-2.8.2/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     3640 2023-05-06 17:52:32.000000 nkust-ucl-k12-bot-2.8.2/README.md
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 11:32:02.938661 nkust-ucl-k12-bot-2.8.2/nkust_ucl/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       26 2023-05-06 09:17:34.000000 nkust-ucl-k12-bot-2.8.2/nkust_ucl/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)    10504 2023-05-07 11:23:38.000000 nkust-ucl-k12-bot-2.8.2/nkust_ucl/k12.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 11:32:02.939872 nkust-ucl-k12-bot-2.8.2/nkust_ucl/utils/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-06 06:57:47.000000 nkust-ucl-k12-bot-2.8.2/nkust_ucl/utils/__init__.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     1021 2023-05-06 17:09:58.000000 nkust-ucl-k12-bot-2.8.2/nkust_ucl/utils/attachment.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      340 2023-05-06 06:55:39.000000 nkust-ucl-k12-bot-2.8.2/nkust_ucl/utils/config.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      426 2023-05-06 07:51:50.000000 nkust-ucl-k12-bot-2.8.2/nkust_ucl/utils/log.py
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      938 2023-05-06 07:31:05.000000 nkust-ucl-k12-bot-2.8.2/nkust_ucl/utils/mqtt_client.py
+drwxr-xr-x   0 zhengshiwen   (501) staff       (20)        0 2023-05-07 11:32:02.940563 nkust-ucl-k12-bot-2.8.2/nkust_ucl_k12_bot.egg-info/
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)     4053 2023-05-07 11:32:02.000000 nkust-ucl-k12-bot-2.8.2/nkust_ucl_k12_bot.egg-info/PKG-INFO
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      367 2023-05-07 11:32:02.000000 nkust-ucl-k12-bot-2.8.2/nkust_ucl_k12_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)        1 2023-05-07 11:32:02.000000 nkust-ucl-k12-bot-2.8.2/nkust_ucl_k12_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       10 2023-05-07 11:32:02.000000 nkust-ucl-k12-bot-2.8.2/nkust_ucl_k12_bot.egg-info/top_level.txt
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)       38 2023-05-07 11:32:02.941033 nkust-ucl-k12-bot-2.8.2/setup.cfg
+-rw-r--r--   0 zhengshiwen   (501) staff       (20)      621 2023-05-07 11:31:58.000000 nkust-ucl-k12-bot-2.8.2/setup.py
```

### Comparing `nkust-ucl-k12-bot-2.8.1/LICENSE` & `nkust-ucl-k12-bot-2.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.8.1/PKG-INFO` & `nkust-ucl-k12-bot-2.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 2.8.1
+Version: 2.8.2
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nkust-ucl-k12-bot-2.8.1/README.md` & `nkust-ucl-k12-bot-2.8.2/README.md`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.8.1/nkust_ucl/k12.py` & `nkust-ucl-k12-bot-2.8.2/nkust_ucl/k12.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.8.1/nkust_ucl/utils/attachment.py` & `nkust-ucl-k12-bot-2.8.2/nkust_ucl/utils/attachment.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.8.1/nkust_ucl/utils/mqtt_client.py` & `nkust-ucl-k12-bot-2.8.2/nkust_ucl/utils/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `nkust-ucl-k12-bot-2.8.1/nkust_ucl_k12_bot.egg-info/PKG-INFO` & `nkust-ucl-k12-bot-2.8.2/nkust_ucl_k12_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkust-ucl-k12-bot
-Version: 2.8.1
+Version: 2.8.2
 Summary: 一個用於k12的bot包
 Home-page: https://github.com/xinbow99/k12-telegram
 Author: Ethan Cheng
 Author-email: asdewq45445@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nkust-ucl-k12-bot-2.8.1/setup.py` & `nkust-ucl-k12-bot-2.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nkust-ucl-k12-bot",
-    version="2.8.1",
+    version="2.8.2",
     author="Ethan Cheng",
     author_email="asdewq45445@gmail.com",
     description="一個用於k12的bot包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinbow99/k12-telegram",
     packages=setuptools.find_packages(),
```

