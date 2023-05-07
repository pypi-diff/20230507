# Comparing `tmp/autoxx-0.0.7.tar.gz` & `tmp/autoxx-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.7.tar", max compression
+gzip compressed data, was "autoxx-0.0.8.tar", max compression
```

## Comparing `autoxx-0.0.7.tar` & `autoxx-0.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.7/README.md
--rw-r--r--   0        0        0      310 2023-05-06 05:23:14.108735 autoxx-0.0.7/autoxx/agent/base.py
--rw-r--r--   0        0        0      973 2023-05-06 13:18:45.575572 autoxx-0.0.7/autoxx/agent/researcher.py
--rw-r--r--   0        0        0     4125 2023-05-07 04:54:29.318874 autoxx-0.0.7/autoxx/agi.py
--rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.7/autoxx/js/overlay.js
--rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.7/autoxx/requirements.txt
--rw-r--r--   0        0        0     4847 2023-05-07 04:46:57.263699 autoxx-0.0.7/autoxx/search/simple_search.py
--rw-r--r--   0        0        0     4995 2023-05-07 02:59:38.452753 autoxx-0.0.7/autoxx/task_manager.py
--rw-r--r--   0        0        0      633 2023-05-07 04:54:24.998675 autoxx-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 autoxx-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.8/README.md
+-rw-r--r--   0        0        0      310 2023-05-06 05:23:14.108735 autoxx-0.0.8/autoxx/agent/base.py
+-rw-r--r--   0        0        0      973 2023-05-06 13:18:45.575572 autoxx-0.0.8/autoxx/agent/researcher.py
+-rw-r--r--   0        0        0     4125 2023-05-07 04:54:29.318874 autoxx-0.0.8/autoxx/agi.py
+-rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.8/autoxx/js/overlay.js
+-rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.8/autoxx/requirements.txt
+-rw-r--r--   0        0        0     4808 2023-05-07 05:09:39.925805 autoxx-0.0.8/autoxx/search/simple_search.py
+-rw-r--r--   0        0        0     4995 2023-05-07 02:59:38.452753 autoxx-0.0.8/autoxx/task_manager.py
+-rw-r--r--   0        0        0      633 2023-05-07 05:09:36.133882 autoxx-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 autoxx-0.0.8/PKG-INFO
```

### Comparing `autoxx-0.0.7/autoxx/agent/researcher.py` & `autoxx-0.0.8/autoxx/agent/researcher.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.7/autoxx/agi.py` & `autoxx-0.0.8/autoxx/agi.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.7/autoxx/js/overlay.js` & `autoxx-0.0.8/autoxx/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.7/autoxx/search/simple_search.py` & `autoxx-0.0.8/autoxx/search/simple_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 CFG = Config()
 
 def setup_autgpt_config(
         azure_config_file:Optional[str] = "",
         only_gpt4:bool = False,
         debug:bool = False,
 ) -> Config:
-    print("xxxxxx", azure_config_file)
     CFG = Config()
     if azure_config_file != "":
         CFG.set_openai_api_key(os.getenv("AZURE_OPENAI_API_KEY", ""))
         CFG.use_azure=True
         CFG.load_azure_config(config_file=azure_config_file)
 
     if only_gpt4:
```

### Comparing `autoxx-0.0.7/autoxx/task_manager.py` & `autoxx-0.0.8/autoxx/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.7/pyproject.toml` & `autoxx-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.7"
+version = "0.0.8"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `autoxx-0.0.7/PKG-INFO` & `autoxx-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.7
+Version: 0.0.8
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

