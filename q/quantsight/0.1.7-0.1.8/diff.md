# Comparing `tmp/quantsight-0.1.7.tar.gz` & `tmp/quantsight-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantsight-0.1.7.tar", last modified: Fri May  5 10:33:04 2023, max compression
+gzip compressed data, was "quantsight-0.1.8.tar", last modified: Sun May  7 12:39:00 2023, max compression
```

## Comparing `quantsight-0.1.7.tar` & `quantsight-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:04.900562 quantsight-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 10:32:54.000000 quantsight-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-05 10:33:04.900562 quantsight-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-05 10:32:54.000000 quantsight-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:04.900562 quantsight-0.1.7/quantsight/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 10:32:54.000000 quantsight-0.1.7/quantsight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-05 10:32:54.000000 quantsight-0.1.7/quantsight/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-05 10:32:54.000000 quantsight-0.1.7/quantsight/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:04.900562 quantsight-0.1.7/quantsight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-05 10:33:04.000000 quantsight-0.1.7/quantsight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-05 10:33:04.000000 quantsight-0.1.7/quantsight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:33:04.000000 quantsight-0.1.7/quantsight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-05 10:33:04.000000 quantsight-0.1.7/quantsight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 10:33:04.000000 quantsight-0.1.7/quantsight.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:33:04.900562 quantsight-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-05 10:32:59.000000 quantsight-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:39:00.324562 quantsight-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 12:38:52.000000 quantsight-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-07 12:39:00.324562 quantsight-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-07 12:38:52.000000 quantsight-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:39:00.324562 quantsight-0.1.8/quantsight/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 12:38:52.000000 quantsight-0.1.8/quantsight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-07 12:38:52.000000 quantsight-0.1.8/quantsight/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-07 12:38:52.000000 quantsight-0.1.8/quantsight/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:39:00.324562 quantsight-0.1.8/quantsight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-07 12:39:00.000000 quantsight-0.1.8/quantsight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-07 12:39:00.000000 quantsight-0.1.8/quantsight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 12:39:00.000000 quantsight-0.1.8/quantsight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-07 12:39:00.000000 quantsight-0.1.8/quantsight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 12:39:00.000000 quantsight-0.1.8/quantsight.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 12:39:00.324562 quantsight-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-07 12:38:58.000000 quantsight-0.1.8/setup.py
```

### Comparing `quantsight-0.1.7/LICENSE` & `quantsight-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `quantsight-0.1.7/PKG-INFO` & `quantsight-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantsight
-Version: 0.1.7
+Version: 0.1.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Publish to PyPI](https://github.com/Unsigned-Research/quantsight-client/actions/workflows/publish-to-pypi.yml/badge.svg?branch=master)](https://github.com/Unsigned-Research/quantsight-client/actions/workflows/publish-to-pypi.yml)
 [![PyPI version](https://badge.fury.io/py/quantsight.svg)](https://badge.fury.io/py/quantsight)
 [![PyPI version](https://img.shields.io/badge/Quantsight-Visit%20Website-blue.svg)](https://www.quantsight.dev/)
```

### Comparing `quantsight-0.1.7/README.md` & `quantsight-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `quantsight-0.1.7/quantsight/agent.py` & `quantsight-0.1.8/quantsight/agent.py`

 * *Files identical despite different names*

### Comparing `quantsight-0.1.7/quantsight/client.py` & `quantsight-0.1.8/quantsight/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 import shutil
 from .agent import QueryAgent
 
 
 class QuantsightClient(QueryAgent):
     def __init__(self, api_key: str, openai_api_key: str = None, cache_path: Path = None, **kwargs):
         super().__init__(openai_api_key, **kwargs)
-        self.base_url = "http://127.0.0.1:8000"
-        # self.base_url = "https://api.quantsight.dev"
+        self.base_url = "https://api.quantsight.dev"
         self.headers = {"Authorization": f"Bearer {api_key}"}
 
         file_location = Path(__file__).resolve().parent
 
         self.cache_path = cache_path
         if self.cache_path is None:
             self.cache_path = file_location
```

### Comparing `quantsight-0.1.7/quantsight.egg-info/PKG-INFO` & `quantsight-0.1.8/quantsight.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantsight
-Version: 0.1.7
+Version: 0.1.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Publish to PyPI](https://github.com/Unsigned-Research/quantsight-client/actions/workflows/publish-to-pypi.yml/badge.svg?branch=master)](https://github.com/Unsigned-Research/quantsight-client/actions/workflows/publish-to-pypi.yml)
 [![PyPI version](https://badge.fury.io/py/quantsight.svg)](https://badge.fury.io/py/quantsight)
 [![PyPI version](https://img.shields.io/badge/Quantsight-Visit%20Website-blue.svg)](https://www.quantsight.dev/)
```

