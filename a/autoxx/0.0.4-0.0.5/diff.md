# Comparing `tmp/autoxx-0.0.4.tar.gz` & `tmp/autoxx-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.4.tar", max compression
+gzip compressed data, was "autoxx-0.0.5.tar", max compression
```

## Comparing `autoxx-0.0.4.tar` & `autoxx-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.4/README.md
--rw-r--r--   0        0        0      310 2023-05-06 05:23:14.108735 autoxx-0.0.4/autoxx/agent/base.py
--rw-r--r--   0        0        0      973 2023-05-06 13:18:45.575572 autoxx-0.0.4/autoxx/agent/researcher.py
--rw-r--r--   0        0        0     4409 2023-05-06 13:18:30.489651 autoxx-0.0.4/autoxx/agi.py
--rw-r--r--   0        0        0      287 2023-04-29 02:02:42.984705 autoxx-0.0.4/autoxx/azure.yaml
--rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.4/autoxx/js/overlay.js
--rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.4/autoxx/requirements.txt
--rw-r--r--   0        0        0     4808 2023-05-06 05:12:53.745943 autoxx-0.0.4/autoxx/search/simple_search.py
--rw-r--r--   0        0        0     4965 2023-05-07 02:05:05.272563 autoxx-0.0.4/autoxx/task_manager.py
--rw-r--r--   0        0        0      633 2023-05-07 02:07:44.026486 autoxx-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 autoxx-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.5/README.md
+-rw-r--r--   0        0        0      310 2023-05-06 05:23:14.108735 autoxx-0.0.5/autoxx/agent/base.py
+-rw-r--r--   0        0        0      973 2023-05-06 13:18:45.575572 autoxx-0.0.5/autoxx/agent/researcher.py
+-rw-r--r--   0        0        0     4409 2023-05-06 13:18:30.489651 autoxx-0.0.5/autoxx/agi.py
+-rw-r--r--   0        0        0      287 2023-04-29 02:02:42.984705 autoxx-0.0.5/autoxx/azure.yaml
+-rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.5/autoxx/js/overlay.js
+-rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.5/autoxx/requirements.txt
+-rw-r--r--   0        0        0     4808 2023-05-06 05:12:53.745943 autoxx-0.0.5/autoxx/search/simple_search.py
+-rw-r--r--   0        0        0     4965 2023-05-07 02:25:10.355024 autoxx-0.0.5/autoxx/task_manager.py
+-rw-r--r--   0        0        0      633 2023-05-07 02:26:47.967466 autoxx-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 autoxx-0.0.5/PKG-INFO
```

### Comparing `autoxx-0.0.4/autoxx/agent/researcher.py` & `autoxx-0.0.5/autoxx/agent/researcher.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.4/autoxx/agi.py` & `autoxx-0.0.5/autoxx/agi.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.4/autoxx/js/overlay.js` & `autoxx-0.0.5/autoxx/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.4/autoxx/search/simple_search.py` & `autoxx-0.0.5/autoxx/search/simple_search.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.4/autoxx/task_manager.py` & `autoxx-0.0.5/autoxx/task_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
   
 class TaskManager:  
     def __init__(self):  
         self.tasks = {}  
   
     def create_task(self, objective: str, max_tasks_count: Optional[int] = 3):  
         if objective in self.tasks:
-            if self.tasks[objective].status != "error":
+            if self.tasks[objective].status == "error":
                 task = self.tasks[objective]
                 task_thread = threading.Thread(target=task.execute)  
                 task_thread.start()
                 return
             else:
                 raise ValueError(f"Task found with objective: {objective}")
```

### Comparing `autoxx-0.0.4/pyproject.toml` & `autoxx-0.0.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.4"
+version = "0.0.5"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `autoxx-0.0.4/PKG-INFO` & `autoxx-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.4
+Version: 0.0.5
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

