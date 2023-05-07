# Comparing `tmp/pyroporn-0.2.8.tar.gz` & `tmp/pyroporn-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroporn-0.2.8.tar", last modified: Sat May  6 09:23:39 2023, max compression
+gzip compressed data, was "pyroporn-0.2.9.tar", last modified: Sun May  7 03:47:00 2023, max compression
```

## Comparing `pyroporn-0.2.8.tar` & `pyroporn-0.2.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:23:39.771304 pyroporn-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-06 09:23:39.771304 pyroporn-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 09:23:22.000000 pyroporn-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:23:39.763304 pyroporn-0.2.8/pyroporn/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20913 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:23:39.767304 pyroporn-0.2.8/pyroporn/database/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/database/bdbDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/database/bubDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/database/othDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/database/papDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/database/pmoDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/database/pobDatabase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:23:39.767304 pyroporn-0.2.8/pyroporn/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/decorators/forcesub.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/decorators/genbuttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/decorators/getjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/decorators/getlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/decorators/oncmd.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/decorators/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:23:39.767304 pyroporn-0.2.8/pyroporn/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/methods/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/methods/getfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/methods/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:23:39.767304 pyroporn-0.2.8/pyroporn/types/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/types/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/types/inlineBdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/types/inlineBub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/types/inlinePob.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/types/inlineVip.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/types/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/types/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:23:39.771304 pyroporn-0.2.8/pyroporn/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/utilities/formater.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/utilities/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/utilities/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 09:23:22.000000 pyroporn-0.2.8/pyroporn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:23:39.767304 pyroporn-0.2.8/pyroporn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-06 09:23:39.000000 pyroporn-0.2.8/pyroporn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-06 09:23:39.000000 pyroporn-0.2.8/pyroporn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 09:23:39.000000 pyroporn-0.2.8/pyroporn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-06 09:23:39.000000 pyroporn-0.2.8/pyroporn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 09:23:39.000000 pyroporn-0.2.8/pyroporn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 09:23:39.771304 pyroporn-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-06 09:23:22.000000 pyroporn-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:47:00.019320 pyroporn-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-07 03:47:00.019320 pyroporn-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-07 03:46:46.000000 pyroporn-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:47:00.007320 pyroporn-0.2.9/pyroporn/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20913 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:47:00.011320 pyroporn-0.2.9/pyroporn/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/database/bdbDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/database/bubDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/database/othDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/database/papDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/database/pmoDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/database/pobDatabase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:47:00.011320 pyroporn-0.2.9/pyroporn/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/decorators/forcesub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/decorators/genbuttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/decorators/getjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/decorators/getlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/decorators/oncmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/decorators/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:47:00.015320 pyroporn-0.2.9/pyroporn/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/methods/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/methods/getfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/methods/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:47:00.015320 pyroporn-0.2.9/pyroporn/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/types/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/types/inlineBdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/types/inlineBub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/types/inlinePob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/types/inlineVip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/types/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/types/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:47:00.019320 pyroporn-0.2.9/pyroporn/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/utilities/formater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/utilities/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/utilities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-07 03:46:46.000000 pyroporn-0.2.9/pyroporn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:47:00.011320 pyroporn-0.2.9/pyroporn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-07 03:46:59.000000 pyroporn-0.2.9/pyroporn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-07 03:47:00.000000 pyroporn-0.2.9/pyroporn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 03:46:59.000000 pyroporn-0.2.9/pyroporn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-07 03:46:59.000000 pyroporn-0.2.9/pyroporn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-07 03:46:59.000000 pyroporn-0.2.9/pyroporn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 03:47:00.019320 pyroporn-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-07 03:46:46.000000 pyroporn-0.2.9/setup.py
```

### Comparing `pyroporn-0.2.8/PKG-INFO` & `pyroporn-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroporn
-Version: 0.2.8
+Version: 0.2.9
 Summary: Best Porn Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyroporn
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram porn bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyroporn-0.2.8/pyroporn/client.py` & `pyroporn-0.2.9/pyroporn/client.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/config.py` & `pyroporn-0.2.9/pyroporn/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 
 class Config:
     API_ID = int(os.environ.get("API_ID", "6092505"))
     API_HASH = os.environ.get("API_HASH", "98d119a0bebd325358589b62461e41a2")
-    SESSION = os.environ.get("SESSION", "BQAhIHQAsQdv8Qr5YTH8_KIAKeEmEoGGY1I-zozu5Nmirp2FUWKdkOetbMEhDun-PkPDLxM3t8Qok_cxY5zK63Zzh3ofPLkEt7pP_o_99a6ZuUhtgmo05oxTaX-3b1ayMqAvcGcAnLIHwIRda0OnwaMTvnL7ZIdX5SqucmRHJW-4BMjg4gl-3B5NNe_5xaLb_hMq04hMycKGfQrv4pgbROV_ZVH-M9E1hoCLR_ZNXAvnaZNLQREG46JkqlKfKGD0QUaSSzpNMvZvGTSIlPWorH5yFwA-zlvYjTGMTRNsqEoDVFI3fLftHCWKZPke_-ud8J93qvoco0X0dMiM5_B8X0wl1f_6mAAAAAEtwrv4AA")
+    SESSION = os.environ.get("SESSION", "BQAhIHQAEoL_7FPGYKwO-MoNWLhRu03lPa7n4y8OMWl67JRWL4cKOuXC6rVbOKjUacqztyNDIOV_IpGq-8zlmISK1DcPuD0jWPvAv99tE6WZBxHuYZuiS7NlQ8PT8pZTXgWwWsquT3B08u6vQ3TXccz_Xw4Vg2l8yQLiuuuI9ukiUQD3t5C_ELqDVMmVcc635qD1V5DUUZsEdBJvh2DFQeKjc3strdNCO9GlVsLx0hGs19JFrfiR2Pj0t5k7pq8inqSMU14bEmlqfd5ZJN6nYIwXLBFIT73Ypl50oA1S6X6sip8hvHuZI-6kWcDr7pafwpuFTdv7OYX8N7C-wuLYDUYbxGWAAAAAEtwrv4AA")
     
     # OTHXBot 
     BOT_TOKEN = os.environ.get("BOT_TOKEN", "5203604736:AAHmhfx42hbMbI7hZZXeQDtm89-dd2ZvIgY")
     # OTHIndexBot 
     BOT_TOKEN2 = os.environ.get("BOT_TOKEN2", "5746206262:AAFzpItUK-qITDs7TcOGyZmHcW_KoLxp3_k")
     # PobBot 
     BOT_TOKEN3 = os.environ.get("BOT_TOKEN3", "6273114809:AAGVPIROv-YQE3YSVn4I7gApeNtcdilO40k")
```

### Comparing `pyroporn-0.2.8/pyroporn/database/bdbDatabase.py` & `pyroporn-0.2.9/pyroporn/database/bdbDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/database/bubDatabase.py` & `pyroporn-0.2.9/pyroporn/database/bubDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/database/othDatabase.py` & `pyroporn-0.2.9/pyroporn/database/othDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/database/papDatabase.py` & `pyroporn-0.2.9/pyroporn/database/papDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/database/pmoDatabase.py` & `pyroporn-0.2.9/pyroporn/database/pmoDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/database/pobDatabase.py` & `pyroporn-0.2.9/pyroporn/database/pobDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/decorators/forcesub.py` & `pyroporn-0.2.9/pyroporn/decorators/forcesub.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/decorators/genbuttons.py` & `pyroporn-0.2.9/pyroporn/decorators/genbuttons.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/decorators/getlink.py` & `pyroporn-0.2.9/pyroporn/decorators/getlink.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/decorators/oncmd.py` & `pyroporn-0.2.9/pyroporn/decorators/oncmd.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/methods/content.py` & `pyroporn-0.2.9/pyroporn/methods/content.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/methods/getfile.py` & `pyroporn-0.2.9/pyroporn/methods/getfile.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/methods/message.py` & `pyroporn-0.2.9/pyroporn/methods/message.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/methods/thumbnail.py` & `pyroporn-0.2.9/pyroporn/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/types/inline.py` & `pyroporn-0.2.9/pyroporn/types/inline.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/types/inlineBdb.py` & `pyroporn-0.2.9/pyroporn/types/inlineBdb.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/types/inlineBub.py` & `pyroporn-0.2.9/pyroporn/types/inlineBub.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/types/inlinePob.py` & `pyroporn-0.2.9/pyroporn/types/inlinePob.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/types/inlineVip.py` & `pyroporn-0.2.9/pyroporn/types/inlineVip.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/types/text.py` & `pyroporn-0.2.9/pyroporn/types/text.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/utilities/formater.py` & `pyroporn-0.2.9/pyroporn/utilities/formater.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/utilities/logger.py` & `pyroporn-0.2.9/pyroporn/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/utilities/mongo.py` & `pyroporn-0.2.9/pyroporn/utilities/mongo.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn/utilities/utils.py` & `pyroporn-0.2.9/pyroporn/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/pyroporn.egg-info/PKG-INFO` & `pyroporn-0.2.9/pyroporn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroporn
-Version: 0.2.8
+Version: 0.2.9
 Summary: Best Porn Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyroporn
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram porn bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyroporn-0.2.8/pyroporn.egg-info/SOURCES.txt` & `pyroporn-0.2.9/pyroporn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroporn-0.2.8/setup.py` & `pyroporn-0.2.9/setup.py`

 * *Files identical despite different names*

