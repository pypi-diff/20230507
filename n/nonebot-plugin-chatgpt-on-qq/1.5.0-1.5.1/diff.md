# Comparing `tmp/nonebot-plugin-chatgpt-on-qq-1.5.0.tar.gz` & `tmp/nonebot-plugin-chatgpt-on-qq-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.5.0.tar", last modified: Tue May  2 17:18:13 2023, max compression
+gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.5.1.tar", last modified: Sun May  7 04:19:54 2023, max compression
```

## Comparing `nonebot-plugin-chatgpt-on-qq-1.5.0.tar` & `nonebot-plugin-chatgpt-on-qq-1.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 17:18:13.434898 nonebot-plugin-chatgpt-on-qq-1.5.0/
--rw-rw-rw-   0        0        0      770 2023-05-02 17:18:13.433916 nonebot-plugin-chatgpt-on-qq-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-02 17:18:13.419764 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/
--rw-rw-rw-   0        0        0    21908 2023-05-02 17:17:29.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/__init__.py
--rw-rw-rw-   0        0        0     1217 2023-05-02 17:17:29.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/config.py
--rw-rw-rw-   0        0        0      876 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py
--rw-rw-rw-   0        0        0     6723 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/loadpresets.py
--rw-rw-rw-   0        0        0    11359 2023-05-02 17:17:29.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/sessions.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:18:13.431780 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq.egg-info/
--rw-rw-rw-   0        0        0      770 2023-05-02 17:18:13.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-05-02 17:18:13.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 17:18:13.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-05-02 17:18:13.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-05-02 17:18:13.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 17:18:13.434898 nonebot-plugin-chatgpt-on-qq-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1220 2023-05-02 17:17:55.000000 nonebot-plugin-chatgpt-on-qq-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 04:19:54.585218 nonebot-plugin-chatgpt-on-qq-1.5.1/
+-rw-rw-rw-   0        0        0      770 2023-05-07 04:19:54.585218 nonebot-plugin-chatgpt-on-qq-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-07 04:19:54.570952 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/
+-rw-rw-rw-   0        0        0    21908 2023-05-07 04:19:18.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/__init__.py
+-rw-rw-rw-   0        0        0     1255 2023-05-07 04:19:18.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/config.py
+-rw-rw-rw-   0        0        0      876 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/custom_errors.py
+-rw-rw-rw-   0        0        0     6723 2023-05-01 06:07:08.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/loadpresets.py
+-rw-rw-rw-   0        0        0    11532 2023-05-07 04:19:18.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/sessions.py
+drwxrwxrwx   0        0        0        0 2023-05-07 04:19:54.583218 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq.egg-info/
+-rw-rw-rw-   0        0        0      770 2023-05-07 04:19:54.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      489 2023-05-07 04:19:54.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 04:19:54.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-05-07 04:19:54.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-05-07 04:19:54.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 04:19:54.586218 nonebot-plugin-chatgpt-on-qq-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2023-05-07 04:19:33.000000 nonebot-plugin-chatgpt-on-qq-1.5.1/setup.py
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.5.0/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.5.0
+Version: 1.5.1
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/__init__.py` & `nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     name="多功能ChatGPT插件",
     description="基于chatGPT-3.5-turbo API的nonebot插件",
     usage=__usage__,
     config=Config,
     extra={
         "License": "BSD License",
         "Author": "颜曦",
-        "version": "1.5.0",
+        "version": "1.5.1",
     },
 )
 
 allow_private: bool = plugin_config.allow_private
 api_keys: List[str] = session_container.api_keys
 temperature: float = plugin_config.temperature
 model: str = plugin_config.model_name
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/config.py` & `nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pydantic import Extra, BaseModel, validator
 
 from .custom_errors import ApiKeyError, NoApiKeyError
 
 
 class Config(BaseModel, extra=Extra.ignore):
     api_key: Union[str, List[str]] = None
+    key_load_balancing: bool = False
     history_save_path: Path = Path("data/ChatHistory").absolute()
     preset_path: Path = Path("data/Presets").absolute()
     openai_proxy: str = None
     openai_api_base: str = None
     chat_memory_max: int = 10
     history_max: int = 100
     temperature: float = 0.5
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py` & `nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/custom_errors.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/loadpresets.py` & `nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/loadpresets.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq/sessions.py` & `nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq/sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,17 +180,19 @@
             model: str = 'gpt-3.5-turbo',
             max_tokens=1024,
     ) -> str:
         if not api_keys:
             logger.error(
                 f'当前不存在api key，请在配置文件里进行配置...')
             return ''
-        random.shuffle(api_keys)
+        if key_load_balancing:
+            random.shuffle(api_keys)
         for num, key in enumerate(api_keys):
             openai.api_key = key
+            logger.debug(f'当前使用 Api Key [{key[:4]}...{key[-4:]}]')
             try:
                 completion: dict = await openai.ChatCompletion.acreate(
                     model=model,
                     messages=self.chat_memory,
                     temperature=temperature,
                     max_tokens=max_tokens,
                     timeout=timeout,
@@ -266,14 +268,15 @@
     def dump2json_str(self) -> str:
         return json.dumps(self.chat_memory, ensure_ascii=False)
 
 
 chat_memory_max = plugin_config.chat_memory_max if plugin_config.chat_memory_max > 2 else 2
 history_max = plugin_config.history_max if plugin_config.history_max > chat_memory_max else 100
 timeout = int(plugin_config.timeout) if plugin_config.timeout and plugin_config.timeout > 0 else 10
+key_load_balancing: bool = plugin_config.key_load_balancing
 
 session_container: SessionContainer = SessionContainer(
     dir_path=plugin_config.history_save_path,
     chat_memory_max=chat_memory_max,
     api_keys=plugin_config.api_key,
     history_max=history_max,
 )
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.5.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.5.1/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.5.0
+Version: 1.5.1
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.5.0/setup.py` & `nonebot-plugin-chatgpt-on-qq-1.5.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding:utf-8
 
 from setuptools import find_packages, setup
 
 setup(
     name='nonebot-plugin-chatgpt-on-qq',
-    version='1.5.0',
+    version='1.5.1',
     description='具有多对话功能的chatGPT聊天插件',
     long_description=open('README.rst').read(),
     author='颜曦',
     author_email='424504326@qq.com',
     maintainer='颜曦',
     maintainer_email='424504326@qq.com',
     packages=find_packages(),
```

