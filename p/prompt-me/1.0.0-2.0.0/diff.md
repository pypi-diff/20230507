# Comparing `tmp/prompt-me-1.0.0.tar.gz` & `tmp/prompt-me-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\prompt-me-1.0.0.tar", last modified: Mon Apr 24 08:08:59 2023, max compression
+gzip compressed data, was "prompt-me-2.0.0.tar", last modified: Sun May  7 12:09:30 2023, max compression
```

## Comparing `prompt-me-1.0.0.tar` & `prompt-me-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 08:08:59.614165 prompt-me-1.0.0/
--rw-rw-rw-   0        0        0     4473 2023-04-24 08:08:59.613192 prompt-me-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2847 2023-04-24 08:04:09.000000 prompt-me-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 08:08:59.601437 prompt-me-1.0.0/prompt_me/
--rw-rw-rw-   0        0        0      819 2023-04-24 06:15:24.000000 prompt-me-1.0.0/prompt_me/__init__.py
--rw-rw-rw-   0        0        0     6107 2023-04-24 07:45:17.000000 prompt-me-1.0.0/prompt_me/_core.py
--rw-rw-rw-   0        0        0     2713 2023-04-24 06:23:20.000000 prompt-me-1.0.0/prompt_me/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:08:59.611162 prompt-me-1.0.0/prompt_me.egg-info/
--rw-rw-rw-   0        0        0     4473 2023-04-24 08:08:59.000000 prompt-me-1.0.0/prompt_me.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-04-24 08:08:59.000000 prompt-me-1.0.0/prompt_me.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 08:08:59.000000 prompt-me-1.0.0/prompt_me.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-24 08:08:59.000000 prompt-me-1.0.0/prompt_me.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 08:08:59.614165 prompt-me-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1785 2023-04-24 08:07:10.000000 prompt-me-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:09:30.052913 prompt-me-2.0.0/
+-rw-rw-rw-   0        0        0    11558 2023-03-08 11:01:44.000000 prompt-me-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     8326 2023-05-07 12:09:30.051909 prompt-me-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7406 2023-05-07 11:55:52.000000 prompt-me-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 12:09:30.006944 prompt-me-2.0.0/prompt_me/
+-rw-rw-rw-   0        0        0     1054 2023-05-07 07:53:11.000000 prompt-me-2.0.0/prompt_me/__init__.py
+-rw-rw-rw-   0        0        0     6378 2023-05-07 08:34:26.000000 prompt-me-2.0.0/prompt_me/chatbot.py
+-rw-rw-rw-   0        0        0     1481 2023-05-07 09:13:07.000000 prompt-me-2.0.0/prompt_me/config.py
+-rw-rw-rw-   0        0        0     5630 2023-05-07 09:13:07.000000 prompt-me-2.0.0/prompt_me/conversation.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:09:30.027350 prompt-me-2.0.0/prompt_me/llm/
+-rw-rw-rw-   0        0        0      796 2023-05-07 09:16:25.000000 prompt-me-2.0.0/prompt_me/llm/__init__.py
+-rw-rw-rw-   0        0        0      940 2023-05-07 11:59:12.000000 prompt-me-2.0.0/prompt_me/llm/base.py
+-rw-rw-rw-   0        0        0     1235 2023-05-07 07:45:37.000000 prompt-me-2.0.0/prompt_me/llm/chat.py
+-rw-rw-rw-   0        0        0      767 2023-05-07 09:13:07.000000 prompt-me-2.0.0/prompt_me/llm/openai.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:09:30.029892 prompt-me-2.0.0/prompt_me/memory/
+-rw-rw-rw-   0        0        0      767 2023-05-07 09:16:25.000000 prompt-me-2.0.0/prompt_me/memory/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:09:30.036901 prompt-me-2.0.0/prompt_me/preset_role/
+-rw-rw-rw-   0        0        0      927 2023-05-07 11:35:24.000000 prompt-me-2.0.0/prompt_me/preset_role/__init__.py
+-rw-rw-rw-   0        0        0     1047 2023-05-07 08:13:28.000000 prompt-me-2.0.0/prompt_me/preset_role/base.py
+-rw-rw-rw-   0        0        0     1858 2023-05-07 11:34:58.000000 prompt-me-2.0.0/prompt_me/preset_role/roles.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:09:30.042947 prompt-me-2.0.0/prompt_me/tools/
+-rw-rw-rw-   0        0        0      767 2023-05-07 09:16:25.000000 prompt-me-2.0.0/prompt_me/tools/__init__.py
+-rw-rw-rw-   0        0        0      767 2023-05-07 09:16:25.000000 prompt-me-2.0.0/prompt_me/tools/duckduckgo.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:09:30.049908 prompt-me-2.0.0/prompt_me/utils/
+-rw-rw-rw-   0        0        0      817 2023-05-07 11:59:12.000000 prompt-me-2.0.0/prompt_me/utils/__init__.py
+-rw-rw-rw-   0        0        0      656 2023-05-07 06:58:01.000000 prompt-me-2.0.0/prompt_me/utils/singleton.py
+-rw-rw-rw-   0        0        0     2649 2023-05-07 11:59:12.000000 prompt-me-2.0.0/prompt_me/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:09:30.016371 prompt-me-2.0.0/prompt_me.egg-info/
+-rw-rw-rw-   0        0        0     8326 2023-05-07 12:09:29.000000 prompt-me-2.0.0/prompt_me.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      605 2023-05-07 12:09:29.000000 prompt-me-2.0.0/prompt_me.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 12:09:29.000000 prompt-me-2.0.0/prompt_me.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-07 12:09:29.000000 prompt-me-2.0.0/prompt_me.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 12:09:30.053907 prompt-me-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1854 2023-05-07 12:08:09.000000 prompt-me-2.0.0/setup.py
```

### Comparing `prompt-me-1.0.0/prompt_me/__init__.py` & `prompt-me-2.0.0/prompt_me/utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 # limitations under the License.
 #
 # Copyright Owner: Zeeland
 # GitHub Link: https://github.com/Undertone0809/
 # Project Link: https://github.com/Undertone0809/prompt-me
 # Contact Email: zeeland@foxmail.com
 
-from ._core import ChatBot
 from .utils import *
+from .singleton import *
```

### Comparing `prompt-me-1.0.0/prompt_me/_core.py` & `prompt-me-2.0.0/prompt_me/chatbot.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,47 +13,49 @@
 # limitations under the License.
 #
 # Copyright Owner: Zeeland
 # GitHub Link: https://github.com/Undertone0809/
 # Project Link: https://github.com/Undertone0809/prompt-me
 # Contact Email: zeeland@foxmail.com
 
-
+import os
 import time
 import requests
-from prompt_me import utils
 from typing import Optional, List
 
-__all__ = ['ChatBot']
+from prompt_me import utils
+from prompt_me.config import Config
+from prompt_me.preset_role import BaseRole
 
-OPENAI_URL = 'https://chatgpt-api.shn.hk/v1/'
-PROXY_URL = 'https://chatgpt-api.shn.hk/v1/'  # FREE API
+__all__ = ['ChatBot']
 
 cache = utils.get_cache()
 logger = utils.get_logger()
-
-
-# utils.enable_log_no_file()
+CFG = Config()
 
 
 class ChatBot:
-    def __init__(self, key: str, enable_proxy: bool = True):
-        self.key = key
-        if enable_proxy:
-            self.base_url = PROXY_URL
-        else:
-            self.base_url = OPENAI_URL
+    def __init__(self, key: Optional[str] = None, enable_proxy: bool = True):
+        if not key and "OPENAI_API_KEY" not in os.environ.keys():
+            raise ValueError('OPENAI API key is not provided')
+        self.key = key if key else os.getenv('OPENAI_API_KEY')
+
+        CFG.set_enable_proxy(enable_proxy)
 
     def ask(self, msg: str, conversation_id: Optional[str] = None) -> Optional[tuple]:
         """
         ask him a question, return his answer and a conversation_id. You can
         continue your session when you input your conversation_id.
-        :param msg: the message you can to ask
-        :param conversation_id: conversation_id to keep session
-        :return: a tuple like ->(his_answer: str, conversation_id: str)
+
+        Args:
+            msg: the message you can to ask
+            conversation_id: conversation id
+
+        Returns:
+            a tuple like ->(his_answer: str, conversation_id: str)
         """
 
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.key}"
         }
 
@@ -61,38 +63,46 @@
         cache[conversation_id] = messages
         body = {
             "model": "gpt-3.5-turbo",
             "messages": messages
         }
         logger.debug(body)
 
-        response = requests.post(url=self.base_url, headers=headers, json=body)
+        response = requests.post(url=CFG.get_request_url(), headers=headers, json=body)
         if response.status_code == 200:
             ret_data = response.json()
             logger.debug(ret_data)
             ret_msg = ret_data['choices'][0]['message']['content']
             logger.debug(ret_msg)
             self._append_message_to_cache(ret_msg, 'assistant', conversation_id)
             return ret_msg, conversation_id
 
         logger.error("Failed to get data")
         return None
 
     def _get_message_from_cache(self, msg: str, conversation_id: Optional[str] = None) -> tuple:
         """
-        get a complete messages. A message is as follows:
+        Get a complete conversation messages.
+
+        Args:
+            msg:
+            conversation_id:
+
+        Returns:
+            conversation_id, messages
+
+        Examples:
+             A message is as follows:
         ---------------------------------------------------------------
         [
-            {"role": "system", "content": "You are a helpful assistant."},
-            {"role": "user", "content": "Hello, Who are you?"}
-            {"role": "assistant", "content": "I am AI."}
+            {"preset_role": "system", "content": "You are a helpful assistant."},
+            {"preset_role": "user", "content": "Hello, Who are you?"}
+            {"preset_role": "assistant", "content": "I am AI."}
         ]
         ---------------------------------------------------------------
-        :param conversation_id:
-        :return: conversation_id, messages
         """
         messages = [
             {"role": "system", "content": "You are a helpful assistant."},
             {"role": "user", "content": msg}
         ]
         if self._is_old_conversation(conversation_id):
             messages = self._append_message_to_cache(msg, 'user', conversation_id)
@@ -102,45 +112,55 @@
     def _is_old_conversation(self, conversation_id: Optional[str]) -> bool:
         return conversation_id == self._get_conversation_id(conversation_id)
 
     def _get_conversation_id(self, conversation_id: Optional[str] = None) -> str:
         """
         This function has two functions. Generating a new conversation_id if it
         doesn't exist, otherwise the same conversation_id as the input is returned.
-        :return: conversation_id
+
+        Args:
+            conversation_id:
+
+        Returns:
+            conversation_id
         """
         if conversation_id and conversation_id in cache:
             return conversation_id
         return str(time.time())
 
     def get_history(self, conversation_id: str) -> Optional[List[dict]]:
         """
         get conversation from cache
-        :param conversation_id: when did you talk to him?
-        :return: conversation
+
+        Returns:
+            conversation
         """
         if conversation_id in cache:
             return cache[conversation_id]
         return None
 
     def output(self, conversation_id: str, output_type: str = 'text', file_path: str = "output.md") -> Optional[str]:
         """
-        export conversation to markdown
-        :param conversation_id: conversation to export
-        :param output_type: text or file, default is text
-        :param file_path: output file path
-        :return: conversation in markdown
+        Export conversation to markdown
+
+        Args:
+            conversation_id: conversation to export
+            output_type: text or file, default is text
+            file_path:  output file path
+
+        Returns:
+            conversation in markdown
         """
         conversation = self.get_history(conversation_id)
         if conversation is None:
             return None
 
         ret = "# Chat record\n"
         for message in conversation:
-            role = message.get('role')
+            role = message.get('preset_role')
             content = message.get('content').replace('"', '\\"')
             if role == 'assistant':
                 ret += f"## Bot said\n\n{content}\n\n"
             else:
                 ret += f"## You said\n\n{content}\n\n"
         if output_type == 'text':
             return ret
@@ -150,10 +170,10 @@
         else:
             raise ValueError("Invalid output destination specified. Please choose either 'text' or 'file'.")
         return ret
 
     def _append_message_to_cache(self, msg: str, role: str, conversation_id: str) -> List[dict]:
         messages: List[dict] = cache[conversation_id]
         if role in ['user', 'assistant']:
-            messages.append({"role": role, "content": msg})
+            messages.append({"preset_role": role, "content": msg})
             cache[conversation_id] = messages
         return messages
```

### Comparing `prompt-me-1.0.0/prompt_me/utils.py` & `prompt-me-2.0.0/prompt_me/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,23 @@
 #
 # Copyright Owner: Zeeland
 # GitHub Link: https://github.com/Undertone0809/
 # Project Link: https://github.com/Undertone0809/prompt-me
 # Contact Email: zeeland@foxmail.com
 
 import os
-import sys
 import logging
 import platform
 import datetime
 from functools import wraps
 from cushy_storage import CushyDict
 
 __all__ = ['get_cache', 'get_logger', 'enable_log', 'enable_log_no_file']
 logger = logging.getLogger(__name__)
 
-
 def get_cache():
     return cache
 
 
 def get_logger():
     return logger
 
@@ -59,15 +57,14 @@
     _check_log_path()
     cur_time = datetime.datetime.now().strftime('%Y%m%d_%H%M%S')
     return f"{get_project_root_path()}/log/log_{cur_time}.log"
 
 
 def enable_log():
     if platform.system() == 'Windows':
-        # todo 检查日志输出为空的问题
         logging.basicConfig(
             level=logging.DEBUG,
             format='[%(levelname)s] %(asctime)s %(message)s',
             datefmt='%Y-%m-%d %H:%M:%S',
             handlers=[
                 logging.FileHandler(f"{get_log_name()}", mode='w', encoding='utf-8'),
                 logging.StreamHandler()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prompt-me-1.0.0/setup.py` & `prompt-me-2.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,31 +16,32 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="prompt-me",
-    version="1.0.0",
+    version="2.0.0",
     author="Zeeland",
     author_email="zeeland@foxmail.com",
-    description="A lightweight ChatGPT ChatBot framework",
+    description="A lightweight LLM Prompt Layer framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Undertone0809/prompt-me",
     packages=setuptools.find_packages(),
     license="Apache 2.0",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
 
     ],
-    keywords="prompt-me, prompt, chatgpt, gpt, chatbot",
+    keywords="prompt-me, prompt, chatgpt, gpt, chatbot, llm",
 )
```

