# Comparing `tmp/xiaogpt-1.43.tar.gz` & `tmp/xiaogpt-1.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-1.43.tar", last modified: Wed Apr 26 00:15:07 2023, max compression
+gzip compressed data, was "xiaogpt-1.44.tar", last modified: Sun May  7 13:13:46 2023, max compression
```

## Comparing `xiaogpt-1.43.tar` & `xiaogpt-1.44.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-04-26 00:14:50.347124 xiaogpt-1.43/LICENSE
--rw-r--r--   0        0        0    11110 2023-04-26 00:14:50.347124 xiaogpt-1.43/README.md
--rw-r--r--   0        0        0      919 2023-04-26 00:15:07.655227 xiaogpt-1.43/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/__main__.py
--rw-r--r--   0        0        0      639 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0      554 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3275 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     1605 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/bot/gpt3_bot.py
--rw-r--r--   0        0        0     1996 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/bot/newbing_bot.py
--rw-r--r--   0        0        0     3415 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/cli.py
--rw-r--r--   0        0        0     5263 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/config.py
--rw-r--r--   0        0        0     2071 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/utils.py
--rw-r--r--   0        0        0    18548 2023-04-26 00:14:50.351124 xiaogpt-1.43/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    11696 1970-01-01 00:00:00.000000 xiaogpt-1.43/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-07 13:13:38.724300 xiaogpt-1.44/LICENSE
+-rw-r--r--   0        0        0    11110 2023-05-07 13:13:38.724300 xiaogpt-1.44/README.md
+-rw-r--r--   0        0        0      919 2023-05-07 13:13:46.828448 xiaogpt-1.44/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/__main__.py
+-rw-r--r--   0        0        0      639 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0      554 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3275 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     1605 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/bot/gpt3_bot.py
+-rw-r--r--   0        0        0     1996 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/bot/newbing_bot.py
+-rw-r--r--   0        0        0     3415 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/cli.py
+-rw-r--r--   0        0        0     5263 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/config.py
+-rw-r--r--   0        0        0     2071 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/utils.py
+-rw-r--r--   0        0        0    18548 2023-05-07 13:13:38.728300 xiaogpt-1.44/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    11696 1970-01-01 00:00:00.000000 xiaogpt-1.44/PKG-INFO
```

### Comparing `xiaogpt-1.43/LICENSE` & `xiaogpt-1.44/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.43/README.md` & `xiaogpt-1.44/README.md`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.43/pyproject.toml` & `xiaogpt-1.44/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "openai",
     "aiohttp",
     "rich",
     "edge-tts>=6.1.3",
     "EdgeGPT==0.1.26",
 ]
 dynamic = []
-version = "1.43"
+version = "1.44"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
```

### Comparing `xiaogpt-1.43/xiaogpt/bot/__init__.py` & `xiaogpt-1.44/xiaogpt/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.43/xiaogpt/bot/base_bot.py` & `xiaogpt-1.44/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.43/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-1.44/xiaogpt/bot/chatgptapi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.43/xiaogpt/bot/gpt3_bot.py` & `xiaogpt-1.44/xiaogpt/bot/gpt3_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.43/xiaogpt/bot/newbing_bot.py` & `xiaogpt-1.44/xiaogpt/bot/newbing_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.43/xiaogpt/cli.py` & `xiaogpt-1.44/xiaogpt/cli.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.43/xiaogpt/config.py` & `xiaogpt-1.44/xiaogpt/config.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.43/xiaogpt/utils.py` & `xiaogpt-1.44/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.43/xiaogpt/xiaogpt.py` & `xiaogpt-1.44/xiaogpt/xiaogpt.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-1.43/PKG-INFO` & `xiaogpt-1.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 1.43
+Version: 1.44
 Summary: Play ChatGPT with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
```

