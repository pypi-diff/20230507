# Comparing `tmp/quantsight-0.1.3.linux-x86_64.tar.gz` & `tmp/quantsight-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantsight-0.1.3.linux-x86_64.tar", last modified: Thu May  4 18:24:35 2023, max compression
+gzip compressed data, was "quantsight-0.1.7.tar", last modified: Fri May  5 10:33:04 2023, max compression
```

## Comparing `quantsight-0.1.3.linux-x86_64.tar` & `quantsight-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.203635 ./
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.203635 ./opt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/Python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/Python/3.11.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/Python/3.11.3/x64/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.215634 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-04 18:24:24.000000 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-04 18:24:35.207635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/__pycache__/client.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-04 18:24:24.000000 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:24:35.215634 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.3-py3.11.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-04 18:24:35.075635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.3-py3.11.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-04 18:24:35.095635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.3-py3.11.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:24:35.075635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.3-py3.11.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 18:24:35.075635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.3-py3.11.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 18:24:35.075635 ./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.3-py3.11.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:04.900562 quantsight-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 10:32:54.000000 quantsight-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-05 10:33:04.900562 quantsight-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-05 10:32:54.000000 quantsight-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:04.900562 quantsight-0.1.7/quantsight/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 10:32:54.000000 quantsight-0.1.7/quantsight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-05 10:32:54.000000 quantsight-0.1.7/quantsight/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-05 10:32:54.000000 quantsight-0.1.7/quantsight/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:33:04.900562 quantsight-0.1.7/quantsight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-05 10:33:04.000000 quantsight-0.1.7/quantsight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-05 10:33:04.000000 quantsight-0.1.7/quantsight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:33:04.000000 quantsight-0.1.7/quantsight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-05 10:33:04.000000 quantsight-0.1.7/quantsight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 10:33:04.000000 quantsight-0.1.7/quantsight.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:33:04.900562 quantsight-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-05 10:32:59.000000 quantsight-0.1.7/setup.py
```

### Comparing `./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight/client.py` & `quantsight-0.1.7/quantsight/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-import os
-
 import requests
 import pandas as pd
 import json
 from typing import Optional
 from datetime import datetime, timezone
-from data_cache import pandas_cache
+from data_cache import pandas_cache, read_metadata
 from pathlib import Path
 import os
+import shutil
+from .agent import QueryAgent
 
 
-class QuantsightClient:
-    def __init__(
-            self,
-            api_key: str,
-            openai_api_key: str = None,
-            cache_path: Path = None
-    ):
-        self.base_url = "https://api.quantsight.dev"
+class QuantsightClient(QueryAgent):
+    def __init__(self, api_key: str, openai_api_key: str = None, cache_path: Path = None, **kwargs):
+        super().__init__(openai_api_key, **kwargs)
+        self.base_url = "http://127.0.0.1:8000"
+        # self.base_url = "https://api.quantsight.dev"
         self.headers = {"Authorization": f"Bearer {api_key}"}
 
         file_location = Path(__file__).resolve().parent
 
-        if cache_path is None:
-            cache_path = file_location
+        self.cache_path = cache_path
+        if self.cache_path is None:
+            self.cache_path = file_location
+        self.cache_path = self.cache_path / "temp"
 
-        os.environ["CACHE_PATH"] = str(cache_path)
+        self.cache_path.mkdir(parents=True, exist_ok=True)
+
+        os.environ["CACHE_PATH"] = str(self.cache_path)
 
     def _request(
             self,
             endpoint: str,
             payload: dict
     ) -> pd.DataFrame:
         url = f"{self.base_url}{endpoint}"
@@ -42,19 +43,25 @@
         df = pd.DataFrame(data)
 
         if "ts" in df.columns:
             df['ts'] = pd.to_datetime(df['ts'])
 
         return df
 
+    def clear_cache(self):
+        os.remove(self.cache_path / "data.h5")
+
+    def read_cache_metadata(self):
+        return read_metadata(str(self.cache_path / "data.h5"))
+
     @pandas_cache
     def get_funding_rate(
             self,
             from_ts: datetime = datetime(2010, 1, 1, tzinfo=timezone.utc),
-            to_ts: datetime = datetime.now(tz=timezone.utc),
+            to_ts: datetime = datetime(2023, 5, 1, tzinfo=timezone.utc),
             exchange: str = "okx",
             limit: int = 100,
             ticker: Optional[str] = None
     ) -> pd.DataFrame:
         payload = {
             "from_ts": from_ts.isoformat(),
             "to_ts": to_ts.isoformat(),
@@ -64,15 +71,15 @@
         }
         return self._request("/get_funding_rate", payload)
 
     @pandas_cache
     def get_ohlcv(
             self,
             from_ts: datetime = datetime(2010, 1, 1, tzinfo=timezone.utc),
-            to_ts: datetime = datetime.now(tz=timezone.utc),
+            to_ts: datetime = datetime(2023, 5, 1, tzinfo=timezone.utc),
             exchange: str = "okx",
             period: str = "1d",
             instrument: str = "swap",
             limit: int = 100,
             ticker: Optional[str] = None
     ) -> pd.DataFrame:
         payload = {
@@ -83,14 +90,28 @@
             "instrument": instrument,
             "limit": limit,
             "ticker": ticker,
         }
         return self._request("/get_ohlcv", payload)
 
     @pandas_cache
+    def custom_query(
+            self,
+            query: str,
+            dry_run: bool = True,
+            use_legacy_sql: bool = False
+    ) -> pd.DataFrame:
+        payload = {
+            "query": query,
+            "dry_run": dry_run,
+            "use_legacy_sql": use_legacy_sql,
+        }
+        return self._request("/custom_query", payload)
+
+    @pandas_cache
     def get_ohlcv_around_time(
             self,
             from_ts: datetime,
             to_ts: datetime,
             exchange: str,
             period: str,
             instrument: str,
@@ -108,20 +129,7 @@
             "target_time": target_time,
             "sample_count": sample_count,
             "limit": limit,
             "ticker": ticker,
         }
         return self._request("/get_ohlcv_around_time", payload)
 
-    @pandas_cache
-    def custom_query(
-            self,
-            query: str,
-            dry_run: bool = True,
-            use_legacy_sql: bool = False
-    ) -> pd.DataFrame:
-        payload = {
-            "query": query,
-            "dry_run": dry_run,
-            "use_legacy_sql": use_legacy_sql,
-        }
-        return self._request("/custom_query", payload)
```

### Comparing `./opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/quantsight-0.1.3-py3.11.egg-info/PKG-INFO` & `quantsight-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantsight
-Version: 0.1.3
+Version: 0.1.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Publish to PyPI](https://github.com/Unsigned-Research/quantsight-client/actions/workflows/publish-to-pypi.yml/badge.svg?branch=master)](https://github.com/Unsigned-Research/quantsight-client/actions/workflows/publish-to-pypi.yml)
 [![PyPI version](https://badge.fury.io/py/quantsight.svg)](https://badge.fury.io/py/quantsight)
 [![PyPI version](https://img.shields.io/badge/Quantsight-Visit%20Website-blue.svg)](https://www.quantsight.dev/)
```

