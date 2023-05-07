# Comparing `tmp/quantsight-0.1.8.tar.gz` & `tmp/quantsight-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantsight-0.1.8.tar", last modified: Sun May  7 12:39:00 2023, max compression
+gzip compressed data, was "quantsight-0.1.9.tar", last modified: Sun May  7 14:24:00 2023, max compression
```

## Comparing `quantsight-0.1.8.tar` & `quantsight-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:39:00.324562 quantsight-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 12:38:52.000000 quantsight-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-07 12:39:00.324562 quantsight-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-07 12:38:52.000000 quantsight-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:39:00.324562 quantsight-0.1.8/quantsight/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 12:38:52.000000 quantsight-0.1.8/quantsight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-07 12:38:52.000000 quantsight-0.1.8/quantsight/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-07 12:38:52.000000 quantsight-0.1.8/quantsight/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:39:00.324562 quantsight-0.1.8/quantsight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-07 12:39:00.000000 quantsight-0.1.8/quantsight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-07 12:39:00.000000 quantsight-0.1.8/quantsight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 12:39:00.000000 quantsight-0.1.8/quantsight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-07 12:39:00.000000 quantsight-0.1.8/quantsight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 12:39:00.000000 quantsight-0.1.8/quantsight.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 12:39:00.324562 quantsight-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-07 12:38:58.000000 quantsight-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:24:00.335892 quantsight-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 14:23:51.000000 quantsight-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-07 14:24:00.335892 quantsight-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-07 14:23:51.000000 quantsight-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:24:00.335892 quantsight-0.1.9/quantsight/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 14:23:51.000000 quantsight-0.1.9/quantsight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-07 14:23:51.000000 quantsight-0.1.9/quantsight/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-07 14:23:51.000000 quantsight-0.1.9/quantsight/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:24:00.335892 quantsight-0.1.9/quantsight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-07 14:24:00.000000 quantsight-0.1.9/quantsight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-07 14:24:00.000000 quantsight-0.1.9/quantsight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 14:24:00.000000 quantsight-0.1.9/quantsight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-07 14:24:00.000000 quantsight-0.1.9/quantsight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 14:24:00.000000 quantsight-0.1.9/quantsight.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 14:24:00.335892 quantsight-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-07 14:23:57.000000 quantsight-0.1.9/setup.py
```

### Comparing `quantsight-0.1.8/LICENSE` & `quantsight-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quantsight-0.1.8/README.md` & `quantsight-0.1.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 This is a Python client for the Quantsight Data API, which allows you to fetch historical funding rates, candle data, and perform custom queries from supported exchanges. The client is easy to use and supports fetching data into a Pandas DataFrame for further analysis.
 
 ### Key features:
 
 
 #### ✅ Pull data from API directly as a pandas DataFrame
 #### ✅ Automatically cached data for faster retrieval and saved credits
-#### ✅ Integrated OpenAI for querying data in natural language prompts
+#### ✅ Integrated OpenAI for querying data using natural language prompts
 
 
 ## Installation
 
 To install the Quantsight Data API Python client, use `pip`:
 
 ```bash
@@ -23,52 +23,101 @@
 ```
 
 ## Usage
 
 First, import the `QuantsightDataAPI` class and create an instance with your API key:
 
 ```python
-from quantsight import Quantsight
+import quantsight as qs
 
 api_key = "your_api_key"
-qs = Quantsight(api_key)
+qs = qs.Quantsight(api_key)
 ```
 
 Then, you can use the following methods to fetch data from the Quantsight Data API:
 
 ### Get funding rate
 
 To fetch historical funding rates from a supported exchange, use the `get_funding_rate` method:
 
 ```python
-funding_rate_df = qs.get_funding_rate("2010-01-01T00:00:00", "2023-05-04T11:47:20.958631", "okx", 100, "BTC-USD-SWAP")
+funding_rate_df = qs.get_funding_rate(
+    exchange="okx",
+    limit=1e6,
+)
 ```
 
 ### Get OHLCV data
 
 To fetch candle data from a supported exchange, use the `get_ohlcv` method:
 
 ```python
-ohlcv_df = qs.get_ohlcv("2010-01-01T00:00:00", "2023-05-04T11:47:20.958631", "okx", "1d", "spot", 100, "BTC-USD-SWAP")
+ohlcv_df = qs.get_ohlcv(
+    period="1d",
+    exchange="okx",
+    limit=1e6,
+)
 ```
 
 ### Get OHLCV data around time
 
 To fetch candle data around a specific point in time, use the `get_ohlcv_around_time` method:
 
 ```python
-ohlcv_around_time_df = qs.get_ohlcv_around_time("2010-01-01T00:00:00+00:00", "2023-05-04T10:47:20.956633+00:00", "okx", "1d", "spot", "00:00:00", 10, 100, "BTC-USD-SWAP")
+ohlcv_around_time_df = qs.get_ohlcv_around_time(
+    period="1d",
+    exchange="okx",
+    target_time=time(9,0,0),
+    sample_count=10,
+    limit=1e6,
+)
 ```
 
+> Endpoint is useful for execution optimisation or seasonality analysis
+
 ### Custom query (BETA)
 
 To perform a custom query, use the `custom_query` method:
 
 ```python
-custom_query_df = qs.custom_query("SELECT close FROM {{okx.ohlcv.swap.1d}} LIMIT 10", dry_run=True, use_legacy_sql=False)
+custom_query_df = qs.custom_query(
+    "SELECT close FROM {{okx.ohlcv.swap.1d}} LIMIT 10", 
+    dry_run=True, 
+    use_legacy_sql=False
+)
 ```
 
 Each method returns a Pandas DataFrame containing the fetched data.
 
+### Caching
+
+Queries are cached both in BigQuery and on the client side in order to maximise your data allowance.
+
+By default the local cache location is stored next to the clien.py file but you may change it when initialising the 
+client:
+
+```python
+qs = qs.Quantsight(
+    api_key=api_key,
+    cache_path=Path("root/your/custom/cache/location")
+)
+```
+
+You can retrieve cache metadata like so:
+```python
+qs.read_cache_metadata()
+```
+
+You can delete all cache like so:
+```python
+qs.clear_cache()
+```
+
+> Pandas cache is handled by the [data-cache](https://pypi.org/project/data-cache/) library.
+
+## Documentation
+
+The documentation for each endpoints can be found here: https://api.quantsight.dev/docs
+
 ## License
 
 This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```

### Comparing `quantsight-0.1.8/quantsight/agent.py` & `quantsight-0.1.9/quantsight/agent.py`

 * *Files identical despite different names*

### Comparing `quantsight-0.1.8/quantsight/client.py` & `quantsight-0.1.9/quantsight/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import pandas as pd
 import json
 from typing import Optional
-from datetime import datetime, timezone
+from datetime import datetime, timezone, time
 from data_cache import pandas_cache, read_metadata
 from pathlib import Path
 import os
 import shutil
 from .agent import QueryAgent
 
 
@@ -105,21 +105,21 @@
             "use_legacy_sql": use_legacy_sql,
         }
         return self._request("/custom_query", payload)
 
     @pandas_cache
     def get_ohlcv_around_time(
             self,
-            from_ts: datetime,
-            to_ts: datetime,
-            exchange: str,
-            period: str,
-            instrument: str,
-            target_time: str,
-            sample_count: int,
+            from_ts: datetime = datetime(2010, 1, 1, tzinfo=timezone.utc),
+            to_ts: datetime = datetime(2023, 5, 1, tzinfo=timezone.utc),
+            exchange: str = "okx",
+            period: str = "1h",
+            instrument: str = "swap",
+            target_time: str = time(10, 0, 0),
+            sample_count: int = 10,
             limit: int = 100,
             ticker: Optional[str] = None
     ) -> pd.DataFrame:
         payload = {
             "from_ts": from_ts.isoformat(),
             "to_ts": to_ts.isoformat(),
             "exchange": exchange,
@@ -127,8 +127,7 @@
             "instrument": instrument,
             "target_time": target_time,
             "sample_count": sample_count,
             "limit": limit,
             "ticker": ticker,
         }
         return self._request("/get_ohlcv_around_time", payload)
-
```

