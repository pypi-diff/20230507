# Comparing `tmp/autoxx-0.0.5.tar.gz` & `tmp/autoxx-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.5.tar", max compression
+gzip compressed data, was "autoxx-0.0.6.tar", max compression
```

## Comparing `autoxx-0.0.5.tar` & `autoxx-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.5/README.md
--rw-r--r--   0        0        0      310 2023-05-06 05:23:14.108735 autoxx-0.0.5/autoxx/agent/base.py
--rw-r--r--   0        0        0      973 2023-05-06 13:18:45.575572 autoxx-0.0.5/autoxx/agent/researcher.py
--rw-r--r--   0        0        0     4409 2023-05-06 13:18:30.489651 autoxx-0.0.5/autoxx/agi.py
--rw-r--r--   0        0        0      287 2023-04-29 02:02:42.984705 autoxx-0.0.5/autoxx/azure.yaml
--rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.5/autoxx/js/overlay.js
--rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.5/autoxx/requirements.txt
--rw-r--r--   0        0        0     4808 2023-05-06 05:12:53.745943 autoxx-0.0.5/autoxx/search/simple_search.py
--rw-r--r--   0        0        0     4965 2023-05-07 02:25:10.355024 autoxx-0.0.5/autoxx/task_manager.py
--rw-r--r--   0        0        0      633 2023-05-07 02:26:47.967466 autoxx-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 autoxx-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.6/README.md
+-rw-r--r--   0        0        0      310 2023-05-06 05:23:14.108735 autoxx-0.0.6/autoxx/agent/base.py
+-rw-r--r--   0        0        0      973 2023-05-06 13:18:45.575572 autoxx-0.0.6/autoxx/agent/researcher.py
+-rw-r--r--   0        0        0     4409 2023-05-06 13:18:30.489651 autoxx-0.0.6/autoxx/agi.py
+-rw-r--r--   0        0        0      287 2023-04-29 02:02:42.984705 autoxx-0.0.6/autoxx/azure.yaml
+-rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.6/autoxx/js/overlay.js
+-rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.6/autoxx/requirements.txt
+-rw-r--r--   0        0        0     4808 2023-05-06 05:12:53.745943 autoxx-0.0.6/autoxx/search/simple_search.py
+-rw-r--r--   0        0        0     4995 2023-05-07 02:59:38.452753 autoxx-0.0.6/autoxx/task_manager.py
+-rw-r--r--   0        0        0      633 2023-05-07 02:59:43.391893 autoxx-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 autoxx-0.0.6/PKG-INFO
```

### Comparing `autoxx-0.0.5/autoxx/agent/researcher.py` & `autoxx-0.0.6/autoxx/agent/researcher.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.5/autoxx/agi.py` & `autoxx-0.0.6/autoxx/agi.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.5/autoxx/js/overlay.js` & `autoxx-0.0.6/autoxx/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.5/autoxx/search/simple_search.py` & `autoxx-0.0.6/autoxx/search/simple_search.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.5/autoxx/task_manager.py` & `autoxx-0.0.6/autoxx/task_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
                 result = self.agent.execute(self.objective, task["task_description"])
                 this_task_id = int(task["task_id"])
                 logging.info(f"\033[93m\033[1m TASK RESULT({self.objective}) \033[0m\033[0m {result}")
             except Exception as e:  
                 logging.error(f"An error occurred while executing the task({self.objective}): {e}")
                 self.status = "error"
                 self.error_message = str(e)  
+                return str(e)
                 # You can also handle specific exceptions if needed, e.g., KeyError, ValueError, etc.  
                 # To do this, add additional except blocks for each specific exception type.  
 
             task["data"] = result
             self.task_cur += 1
 
             # Step 2: Create new tasks
```

### Comparing `autoxx-0.0.5/pyproject.toml` & `autoxx-0.0.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.5"
+version = "0.0.6"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `autoxx-0.0.5/PKG-INFO` & `autoxx-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.5
+Version: 0.0.6
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

