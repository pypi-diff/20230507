# Comparing `tmp/autoxx-0.0.2.tar.gz` & `tmp/autoxx-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoxx-0.0.2.tar", max compression
+gzip compressed data, was "autoxx-0.0.3.tar", max compression
```

## Comparing `autoxx-0.0.2.tar` & `autoxx-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.2/README.md
--rw-r--r--   0        0        0      310 2023-05-06 05:23:14.108735 autoxx-0.0.2/autoxx/agent/base.py
--rw-r--r--   0        0        0      971 2023-05-06 11:43:42.921582 autoxx-0.0.2/autoxx/agent/researcher.py
--rw-r--r--   0        0        0     4408 2023-05-06 10:47:31.935661 autoxx-0.0.2/autoxx/agi.py
--rw-r--r--   0        0        0      287 2023-04-29 02:02:42.984705 autoxx-0.0.2/autoxx/azure.yaml
--rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.2/autoxx/js/overlay.js
--rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.2/autoxx/requirements.txt
--rw-r--r--   0        0        0     4808 2023-05-06 05:12:53.745943 autoxx-0.0.2/autoxx/search/simple_search.py
--rw-r--r--   0        0        0     4058 2023-05-06 11:44:00.910745 autoxx-0.0.2/autoxx/task_manager.py
--rw-r--r--   0        0        0      633 2023-05-06 13:16:22.064642 autoxx-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 autoxx-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-06 12:39:27.568074 autoxx-0.0.3/README.md
+-rw-r--r--   0        0        0      310 2023-05-06 05:23:14.108735 autoxx-0.0.3/autoxx/agent/base.py
+-rw-r--r--   0        0        0      973 2023-05-06 13:18:45.575572 autoxx-0.0.3/autoxx/agent/researcher.py
+-rw-r--r--   0        0        0     4409 2023-05-06 13:18:30.489651 autoxx-0.0.3/autoxx/agi.py
+-rw-r--r--   0        0        0      287 2023-04-29 02:02:42.984705 autoxx-0.0.3/autoxx/azure.yaml
+-rw-r--r--   0        0        0      804 2023-04-29 02:00:35.851451 autoxx-0.0.3/autoxx/js/overlay.js
+-rw-r--r--   0        0        0      406 2023-05-06 12:27:17.236147 autoxx-0.0.3/autoxx/requirements.txt
+-rw-r--r--   0        0        0     4808 2023-05-06 05:12:53.745943 autoxx-0.0.3/autoxx/search/simple_search.py
+-rw-r--r--   0        0        0     4061 2023-05-06 13:18:37.927290 autoxx-0.0.3/autoxx/task_manager.py
+-rw-r--r--   0        0        0      633 2023-05-06 13:19:33.073694 autoxx-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      980 1970-01-01 00:00:00.000000 autoxx-0.0.3/PKG-INFO
```

### Comparing `autoxx-0.0.2/autoxx/agent/researcher.py` & `autoxx-0.0.3/autoxx/agent/researcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from autox.agent.base import BaseAgent
+from autoxx.agent.base import BaseAgent
 from typing import List, Dict
-from autox.search.simple_search import simple_search
+from autoxx.search.simple_search import simple_search
 from autogpt.llm_utils import create_chat_completion
 from autogpt.config import Config
 
 CFG = Config()
 
 class ResearchAgent(BaseAgent):
```

### Comparing `autoxx-0.0.2/autoxx/agi.py` & `autoxx-0.0.3/autoxx/agi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os, json
 from collections import deque
 from typing import Dict, List, Dict, Optional
 
-from autox.search.simple_search import simple_search, setup_autgpt_config
+from autoxx.search.simple_search import simple_search, setup_autgpt_config
 from autogpt.llm_utils import create_chat_completion
 
 AZURE_CONFIG_FILE = os.path.join(os.path.dirname(__file__), "azure.yaml")
 CFG = setup_autgpt_config(azure_config_file=AZURE_CONFIG_FILE, only_gpt4=True, debug=True)
 response_format = """[
     {
         "task_id": 1,
```

### Comparing `autoxx-0.0.2/autoxx/js/overlay.js` & `autoxx-0.0.3/autoxx/js/overlay.js`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.2/autoxx/search/simple_search.py` & `autoxx-0.0.3/autoxx/search/simple_search.py`

 * *Files identical despite different names*

### Comparing `autoxx-0.0.2/autoxx/task_manager.py` & `autoxx-0.0.3/autoxx/task_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging, time, threading
 from typing import Dict, Optional
-from autox.agent.base import BaseAgent
-from autox.agent.researcher import ResearchAgent
-from autox.agi import init_task_list, task_creation_agent, prioritization_agent
+from autoxx.agent.base import BaseAgent
+from autoxx.agent.researcher import ResearchAgent
+from autoxx.agi import init_task_list, task_creation_agent, prioritization_agent
 
 class Task:
     def __init__(self, agent:BaseAgent, objective:str, max_tasks_count: Optional[int] = 3):
         if objective is None or len(objective) <= 1:  
             raise ValueError("Must provide an objective")  
         if agent is None:  
             raise ValueError("Must provide an agent")
```

### Comparing `autoxx-0.0.2/pyproject.toml` & `autoxx-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autoxx"
-version = "0.0.2"
+version = "0.0.3"
 description = "LLM-based autonomous agent"
 authors = ["IANTHEREAL <argregoryian@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `autoxx-0.0.2/PKG-INFO` & `autoxx-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoxx
-Version: 0.0.2
+Version: 0.0.3
 Summary: LLM-based autonomous agent
 License: MIT
 Author: IANTHEREAL
 Author-email: argregoryian@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

