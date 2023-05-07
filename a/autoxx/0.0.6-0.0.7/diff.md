# Comparing `tmp/autoxx-0.0.6.tar.gz` & `tmp/autoxx-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.6.tar", max compression
+gzip compressed data, was "autoxx-0.0.7.tar", max compression
```

## Comparing `autoxx-0.0.6.tar` & `autoxx-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.6/README.md
--rw-r--r--   0        0        0      310 2023-05-06 05:23:14.108735 autoxx-0.0.6/autoxx/agent/base.py
--rw-r--r--   0        0        0      973 2023-05-06 13:18:45.575572 autoxx-0.0.6/autoxx/agent/researcher.py
--rw-r--r--   0        0        0     4409 2023-05-06 13:18:30.489651 autoxx-0.0.6/autoxx/agi.py
--rw-r--r--   0        0        0      287 2023-04-29 02:02:42.984705 autoxx-0.0.6/autoxx/azure.yaml
--rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.6/autoxx/js/overlay.js
--rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.6/autoxx/requirements.txt
--rw-r--r--   0        0        0     4808 2023-05-06 05:12:53.745943 autoxx-0.0.6/autoxx/search/simple_search.py
--rw-r--r--   0        0        0     4995 2023-05-07 02:59:38.452753 autoxx-0.0.6/autoxx/task_manager.py
--rw-r--r--   0        0        0      633 2023-05-07 02:59:43.391893 autoxx-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 autoxx-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.7/README.md
+-rw-r--r--   0        0        0      310 2023-05-06 05:23:14.108735 autoxx-0.0.7/autoxx/agent/base.py
+-rw-r--r--   0        0        0      973 2023-05-06 13:18:45.575572 autoxx-0.0.7/autoxx/agent/researcher.py
+-rw-r--r--   0        0        0     4125 2023-05-07 04:54:29.318874 autoxx-0.0.7/autoxx/agi.py
+-rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.7/autoxx/js/overlay.js
+-rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.7/autoxx/requirements.txt
+-rw-r--r--   0        0        0     4847 2023-05-07 04:46:57.263699 autoxx-0.0.7/autoxx/search/simple_search.py
+-rw-r--r--   0        0        0     4995 2023-05-07 02:59:38.452753 autoxx-0.0.7/autoxx/task_manager.py
+-rw-r--r--   0        0        0      633 2023-05-07 04:54:24.998675 autoxx-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 autoxx-0.0.7/PKG-INFO
```

### Comparing `autoxx-0.0.6/autoxx/agent/researcher.py` & `autoxx-0.0.7/autoxx/agent/researcher.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.6/autoxx/agi.py` & `autoxx-0.0.7/autoxx/agi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import os, json
+import json
 from collections import deque
 from typing import Dict, List, Dict, Optional
 
-from autoxx.search.simple_search import simple_search, setup_autgpt_config
 from autogpt.llm_utils import create_chat_completion
+from autogpt.config import Config
 
-AZURE_CONFIG_FILE = os.path.join(os.path.dirname(__file__), "azure.yaml")
-CFG = setup_autgpt_config(azure_config_file=AZURE_CONFIG_FILE, only_gpt4=True, debug=True)
 response_format = """[
     {
         "task_id": 1,
         "task_description": "task description"
     },
     {
         "task_id": 2,
@@ -42,15 +40,15 @@
         f"Based on the result, create new tasks to be completed by the AI system that do not overlap with incomplete tasks. Up to {allowed_new_task} new tasks can be created.\n"
         "You should only respond in JSON format as described below \n"
         f"Response Format: \n{response_format} \nEnsure the response can be parsed by Python json.loads"
     )
 
     messages = [create_message(prompt)]
     response = create_chat_completion(
-        model=CFG.fast_llm_model,
+        model=Config().fast_llm_model,
         messages=messages,
     )
 
     new_tasks = json.loads(response)
     return [{"task_description": task["task_description"]} for task in new_tasks]
 
 def prioritization_agent(this_task_id:int, objective:str, task_list:deque) -> deque:
@@ -65,42 +63,39 @@
         "#. First task\n"
         "#. Second task\n"
         f"Start the task list with number {next_task_id}."
     )
 
     messages = [create_message(prompt)]
     response = create_chat_completion(
-        model=CFG.fast_llm_model,
+        model=Config().fast_llm_model,
         messages=messages,
     )
 
     new_tasks = response.split('\n')
     task_list = []
     for task_string in new_tasks:
         task_parts = task_string.strip().split(".", 1)
         if len(task_parts) == 2:
             task_id = task_parts[0].strip()
             task_description = task_parts[1].strip()
             task_list.append({"task_id": task_id, "task_description": task_description})
     return task_list
 
-def execution_agent(objective:str, task: str) -> str:
-    return simple_search(task, 2)
-
 def init_task_list(objective: str, max_tasks_count: Optional[int] = 4) -> List[Dict]:
     task_id_counter = 0
     prompt = (
         f"You are an task creation AI that creates tasks with the following objective: {objective}.\n"
         f"Up to {max_tasks_count - 1} new tasks can be created to complete this objective. "
         "You should only respond in JSON format as described below \n"
         f"Response Format: \n{response_format} \nEnsure the response can be parsed by Python json.loads"
     )
     messages = [create_message(prompt)]
     response = create_chat_completion(
-        model=CFG.fast_llm_model,
+        model=Config().fast_llm_model,
         messages=messages,
     )
 
     new_tasks = json.loads(response)
     task_list = []
     for new_task in new_tasks:
         task_id_counter += 1
```

### Comparing `autoxx-0.0.6/autoxx/js/overlay.js` & `autoxx-0.0.7/autoxx/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.6/autoxx/search/simple_search.py` & `autoxx-0.0.7/autoxx/search/simple_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 CFG = Config()
 
 def setup_autgpt_config(
         azure_config_file:Optional[str] = "",
         only_gpt4:bool = False,
         debug:bool = False,
 ) -> Config:
+    print("xxxxxx", azure_config_file)
     CFG = Config()
     if azure_config_file != "":
         CFG.set_openai_api_key(os.getenv("AZURE_OPENAI_API_KEY", ""))
         CFG.use_azure=True
         CFG.load_azure_config(config_file=azure_config_file)
 
     if only_gpt4:
```

### Comparing `autoxx-0.0.6/autoxx/task_manager.py` & `autoxx-0.0.7/autoxx/task_manager.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.6/pyproject.toml` & `autoxx-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.6"
+version = "0.0.7"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `autoxx-0.0.6/PKG-INFO` & `autoxx-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.6
+Version: 0.0.7
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

