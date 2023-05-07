# Comparing `tmp/zillionare-trader-client-0.3.9.tar.gz` & `tmp/zillionare_trader_client-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zillionare-trader-client-0.3.9.tar", max compression
+gzip compressed data, was "zillionare_trader_client-0.4.1.tar", max compression
```

## Comparing `zillionare-trader-client-0.3.9.tar` & `zillionare_trader_client-0.4.1.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0     1068 2022-03-16 11:57:48.309626 zillionare-trader-client-0.3.9/LICENSE
--rw-r--r--   0        0        0     1752 2022-06-06 14:56:11.726066 zillionare-trader-client-0.3.9/README.md
--rw-r--r--   0        0        0     2557 2022-06-06 14:48:49.081704 zillionare-trader-client-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     6848 2022-05-27 07:03:09.682619 zillionare-trader-client-0.3.9/tests/__init__.py
--rw-r--r--   0        0        0     2191 2022-03-27 11:33:22.207264 zillionare-trader-client-0.3.9/tests/data/bars_1d.pkl
--rw-r--r--   0        0        0   408697 2022-03-27 11:33:22.211264 zillionare-trader-client-0.3.9/tests/data/bars_1m.pkl
--rw-r--r--   0        0        0      912 2022-03-27 11:33:22.211264 zillionare-trader-client-0.3.9/tests/data/defaults.yaml
--rw-r--r--   0        0        0      931 2022-03-27 11:33:22.211264 zillionare-trader-client-0.3.9/tests/data/hljh_1d.csv
--rw-r--r--   0        0        0   214231 2022-03-27 11:33:22.215264 zillionare-trader-client-0.3.9/tests/data/hljh_1m.csv
--rw-r--r--   0        0        0      303 2022-03-27 11:33:22.215264 zillionare-trader-client-0.3.9/tests/data/hljh_limits.csv
--rw-r--r--   0        0        0      902 2022-03-27 11:33:22.215264 zillionare-trader-client-0.3.9/tests/data/limits.csv
--rw-r--r--   0        0        0     1078 2022-03-27 11:33:22.215264 zillionare-trader-client-0.3.9/tests/data/limits.pkl
--rw-r--r--   0        0        0      438 2022-03-27 11:33:22.215264 zillionare-trader-client-0.3.9/tests/data/readme.md
--rw-r--r--   0        0        0      896 2022-03-27 11:33:22.215264 zillionare-trader-client-0.3.9/tests/data/tyst_1d.csv
--rw-r--r--   0        0        0   207056 2022-03-27 11:33:22.219264 zillionare-trader-client-0.3.9/tests/data/tyst_1m.csv
--rw-r--r--   0        0        0      315 2022-03-27 11:33:22.219264 zillionare-trader-client-0.3.9/tests/data/tyst_limits.csv
--rw-r--r--   0        0        0     8400 2022-06-06 14:45:21.778081 zillionare-trader-client-0.3.9/tests/test_traderclient.py
--rw-r--r--   0        0        0     1636 2022-05-31 08:09:54.569114 zillionare-trader-client-0.3.9/tests/test_transport.py
--rw-r--r--   0        0        0      183 2022-05-31 01:56:08.192026 zillionare-trader-client-0.3.9/traderclient/__init__.py
--rw-r--r--   0        0        0        0 2022-05-27 07:03:09.682619 zillionare-trader-client-0.3.9/traderclient/cli.py
--rw-r--r--   0        0        0    25469 2022-06-06 13:17:56.022864 zillionare-trader-client-0.3.9/traderclient/client.py
--rw-r--r--   0        0        0      487 2022-05-30 14:16:41.141679 zillionare-trader-client-0.3.9/traderclient/datatypes.py
--rw-r--r--   0        0        0     7426 2022-06-06 15:15:42.647186 zillionare-trader-client-0.3.9/traderclient/demo.py
--rw-r--r--   0        0        0      350 2022-05-27 07:03:09.682619 zillionare-trader-client-0.3.9/traderclient/errors.py
--rw-r--r--   0        0        0     3676 2022-06-06 15:12:25.892310 zillionare-trader-client-0.3.9/traderclient/transport.py
--rw-r--r--   0        0        0     1572 2022-05-27 07:03:09.682619 zillionare-trader-client-0.3.9/traderclient/utils.py
--rw-r--r--   0        0        0     3424 2022-06-06 15:18:11.413658 zillionare-trader-client-0.3.9/setup.py
--rw-r--r--   0        0        0     3746 2022-06-06 15:18:11.414239 zillionare-trader-client-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-04 02:55:06.813294 zillionare_trader_client-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1752 2023-04-04 02:55:06.813294 zillionare_trader_client-0.4.1/README.md
+-rw-r--r--   0        0        0     2513 2023-05-06 07:21:53.012380 zillionare_trader_client-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6831 2023-05-05 12:28:42.792689 zillionare_trader_client-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     2191 2023-04-04 02:55:06.817294 zillionare_trader_client-0.4.1/tests/data/bars_1d.pkl
+-rw-r--r--   0        0        0   408697 2023-04-04 02:55:06.825294 zillionare_trader_client-0.4.1/tests/data/bars_1m.pkl
+-rw-r--r--   0        0        0    56389 2023-05-05 09:15:16.952210 zillionare_trader_client-0.4.1/tests/data/calendar.json
+-rw-r--r--   0        0        0      881 2023-05-05 09:05:10.906134 zillionare_trader_client-0.4.1/tests/data/defaults.yaml
+-rw-r--r--   0        0        0      931 2023-04-04 02:55:06.825294 zillionare_trader_client-0.4.1/tests/data/hljh_1d.csv
+-rw-r--r--   0        0        0   214231 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.1/tests/data/hljh_1m.csv
+-rw-r--r--   0        0        0      303 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.1/tests/data/hljh_limits.csv
+-rw-r--r--   0        0        0      902 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.1/tests/data/limits.csv
+-rw-r--r--   0        0        0     1078 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.1/tests/data/limits.pkl
+-rw-r--r--   0        0        0      438 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.1/tests/data/readme.md
+-rw-r--r--   0        0        0      896 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.1/tests/data/tyst_1d.csv
+-rw-r--r--   0        0        0   207056 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.1/tests/data/tyst_1m.csv
+-rw-r--r--   0        0        0      315 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.1/tests/data/tyst_limits.csv
+-rw-r--r--   0        0        0     1339 2023-05-05 09:31:56.254023 zillionare_trader_client-0.4.1/tests/helper.py
+-rw-r--r--   0        0        0     4117 2023-04-04 02:55:06.829294 zillionare_trader_client-0.4.1/tests/performance.py
+-rw-r--r--   0        0        0    10301 2023-05-05 10:59:19.119637 zillionare_trader_client-0.4.1/tests/test_traderclient.py
+-rw-r--r--   0        0        0     1620 2023-05-05 12:07:44.696724 zillionare_trader_client-0.4.1/tests/test_transport.py
+-rw-r--r--   0        0        0      183 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.1/traderclient/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.1/traderclient/cli.py
+-rw-r--r--   0        0        0    29101 2023-05-06 06:53:48.601741 zillionare_trader_client-0.4.1/traderclient/client.py
+-rw-r--r--   0        0        0      487 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.1/traderclient/datatypes.py
+-rw-r--r--   0        0        0     6983 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.1/traderclient/demo.py
+-rw-r--r--   0        0        0      350 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.1/traderclient/errors.py
+-rw-r--r--   0        0        0     3750 2023-05-06 06:54:02.837816 zillionare_trader_client-0.4.1/traderclient/transport.py
+-rw-r--r--   0        0        0     1572 2023-04-04 02:55:06.833294 zillionare_trader_client-0.4.1/traderclient/utils.py
+-rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 zillionare_trader_client-0.4.1/PKG-INFO
```

### Comparing `zillionare-trader-client-0.3.9/LICENSE` & `zillionare_trader_client-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zillionare-trader-client-0.3.9/README.md` & `zillionare_trader_client-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `zillionare-trader-client-0.3.9/pyproject.toml` & `zillionare_trader_client-0.4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "zillionare-trader-client"
-version = "0.3.9"
+version = "0.4.1"
 homepage = "https://github.com/zillionare/trader-client"
 description = "Zillionare Trader Client"
 authors = ["Aaron Yang <code@jieyu.ai>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -23,39 +23,34 @@
 [tool.poetry.dependencies]
 python = ">=3.8,<3.9"
 
 black  = {version = "^22.3.0", optional = true}
 isort  = { version = "5.6.4", optional = true}
 flake8  = { version = "3.8.4", optional = true}
 flake8-docstrings = { version = "^1.6.0", optional = true }
-pytest  = { version = "6.1.2", optional = true}
 pytest-cov  = { version = "2.10.1", optional = true}
 tox  = { version = "^3.20.1", optional = true}
-virtualenv  = { version = "^20.2.2", optional = true}
-pip  = { version = "^20.3.1", optional = true}
 mkdocs  = { version = "^1.2.3", optional = true}
 mkdocs-include-markdown-plugin  = { version = "^3.2.3", optional = true}
 mkdocs-material  = { version = "^8.1.11", optional = true}
 mkdocstrings  = { version = "^0.18.0", optional = true}
 mkdocs-material-extensions  = { version = "^1.0.3", optional = true}
 mkdocs-autorefs = {version = "^0.4.1", optional = true}
 twine  = { version = "^3.3.0", optional = true}
 pre-commit = {version = "^2.12.0", optional = true}
 toml = {version = "^0.10.2", optional = true}
-arrow = "^1.2.2"
 livereload = {version = "^2.6.3", optional = true}
-httpx = "^0.16"
-sanic = {version = "^22.3.2", optional = true}
-fire = "^0.4.0"
-numpy = "^1.22.4"
+httpx = "^0.23"
 mike = {version = "^1.1.2", optional = true}
+sanic = {version = "^23.3.0", optional = true}
+arrow = {version = "^1.2.3"}
+numpy = "^1.24.3"
 
 [tool.poetry.extras]
 test = [
-    "pytest",
     "black",
     "isort",
     "flake8",
     "flake8-docstrings",
     "pytest-cov",
     "sanic"
     ]
@@ -70,14 +65,19 @@
     "mkdocs-material-extension",
     "mkdocs-autorefs",
     "Jinja2",
     "livereload",
     "mike"
     ]
 
+[[tool.poetry.source]]
+name = "tsinghua"
+url = "https://pypi.tuna.tsinghua.edu.cn/simple"
+default = true
+secondary = false
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 bt = 'traderclient.cli:main'
```

### Comparing `zillionare-trader-client-0.3.9/tests/__init__.py` & `zillionare_trader_client-0.4.1/tests/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Unit test package for traderclient."""
+
 import multiprocessing
 import os
 import pickle
 import socket
+import subprocess
 import time
 import uuid
 from enum import IntEnum
-from http.client import CONFLICT, FORBIDDEN, UNAUTHORIZED
 from signal import SIGTERM
 
 import arrow
 import httpx
 import numpy as np
 from sanic import HTTPResponse, Sanic
 from sanic import response as r
@@ -200,15 +201,15 @@
         self.port = port
 
         self._server = None
         self._loop = None
         self._process = None
 
     def run(self):
-        mp = multiprocessing.get_context("fork")
+        mp = multiprocessing.get_context("spawn")
         self._process = mp.Process(target=self._run_server)
         self._process.daemon = True
         self._process.start()
         is_ready = False
         while not is_ready:
             try:
                 httpx.get(f"http://localhost:{self.port}")
@@ -216,15 +217,15 @@
                 time.sleep(0.1)
                 continue
             else:
                 is_ready = True
 
     def _run_server(self):
         print("Running server")
-        app.run(host=self.host, port=self.port)
+        app.run(host=self.host, port=self.port, single_process=True)
 
     def stop(self):
         os.kill(self._process.pid, SIGTERM)
         print("Stopping server")
         self._process.join()
         self._process.terminate()
```

### Comparing `zillionare-trader-client-0.3.9/tests/data/bars_1d.pkl` & `zillionare_trader_client-0.4.1/tests/data/bars_1d.pkl`

 * *Files identical despite different names*

### Comparing `zillionare-trader-client-0.3.9/tests/data/bars_1m.pkl` & `zillionare_trader_client-0.4.1/tests/data/bars_1m.pkl`

 * *Files identical despite different names*

### Comparing `zillionare-trader-client-0.3.9/tests/data/defaults.yaml` & `zillionare_trader_client-0.4.1/tests/data/defaults.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -5,37 +5,39 @@
   formatters:
     default:
       format: '%(asctime)s %(levelname)-1.1s %(process)d %(name)s:%(funcName)s:%(lineno)s | %(message)s'
   handlers:
     console:
       class: logging.StreamHandler
       formatter: default
-    file:
-      class: logging.handlers.RotatingFileHandler
-      formatter: default
-      filename: /var/log/backtest/backtest.log
-      maxBytes: 10485760
-      backupCount: 10
-      encoding: utf-8
   loggers:
     apscheduler:
       level: INFO
     sanic:
       level: WARNING
     cfg4py:
       level: WARNING
   root:
     handlers:
       - console
-      - file
     level: INFO
 metrics:
   risk_free_rate: 0.03
   annual_days: 252
 server:
   path: /backtest/api/trade/v0.2/
 
 feed:
   type: file
   filefeed:
     bars_path: /config/bars_1m.pkl
     limits_path: /config/limits.pkl
+redis:
+  dsn: redis://localhost:6379
+
+influxdb:
+  url: http://localhost:8086
+  token: my-token
+  org: my-org
+  bucket_name: my-bucket
+  enable_compress: true
+  max_query_size: 150000
```

### Comparing `zillionare-trader-client-0.3.9/tests/data/hljh_1d.csv` & `zillionare_trader_client-0.4.1/tests/data/hljh_1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare-trader-client-0.3.9/tests/data/hljh_1m.csv` & `zillionare_trader_client-0.4.1/tests/data/hljh_1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-trader-client-0.3.9/tests/data/limits.csv` & `zillionare_trader_client-0.4.1/tests/data/limits.csv`

 * *Files identical despite different names*

### Comparing `zillionare-trader-client-0.3.9/tests/data/limits.pkl` & `zillionare_trader_client-0.4.1/tests/data/limits.pkl`

 * *Files identical despite different names*

### Comparing `zillionare-trader-client-0.3.9/tests/data/tyst_1d.csv` & `zillionare_trader_client-0.4.1/tests/data/tyst_1d.csv`

 * *Files identical despite different names*

### Comparing `zillionare-trader-client-0.3.9/tests/data/tyst_1m.csv` & `zillionare_trader_client-0.4.1/tests/data/tyst_1m.csv`

 * *Files identical despite different names*

### Comparing `zillionare-trader-client-0.3.9/tests/test_traderclient.py` & `zillionare_trader_client-0.4.1/tests/test_traderclient.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,84 @@
 #!/usr/bin/env python
 """Tests for `traderclient` package."""
 # pylint: disable=redefined-outer-name
 
 import datetime
 import unittest
+import uuid
+from unittest import mock
 
+import arrow
+import httpx
 import numpy as np
 
 from tests import assert_deep_almost_equal
 from traderclient.client import TraderClient
 from traderclient.errors import TradeError
 from traderclient.utils import enable_logging
 
+rsp = httpx.get("http://localhost:3180/")
+endpoint = rsp.json()["endpoint"]
+url = f"http://localhost:3180{endpoint}/"
 
-class TraderClientWithBacktestServerTest(unittest.TestCase):
-    def setUp(self):
+
+class TraderClientWithBacktestServerTest(unittest.IsolatedAsyncioTestCase):
+    async def asyncSetUp(self):
         enable_logging("info")
 
-        self.url = "http://localhost:3180/backtest/api/trade/v0.4"
         start = datetime.date(2022, 3, 1)
         end = datetime.date(2022, 3, 14)
         try:
-            TraderClient.delete_account(self.url, "test", "test")
+            TraderClient.delete_account(url, "test", "test")
         except:
             pass
 
         # this also tested _start_backtest
         self.client = TraderClient(
-            self.url, "test", "test", is_backtest=True, start=start, end=end
+            url,
+            f"test-{uuid.uuid4().hex}",
+            f"{uuid.uuid4().hex}",
+            is_backtest=True,
+            start=start,
+            end=end,
         )
 
-    def tearDown(self) -> None:
-        return super().tearDown()
+    async def asyncTearDown(self):
+        return super().asyncTearDown()
+
+    async def _setup_omicron(self):
+        import os
+
+        import cfg4py
+        import omicron
+        from omicron.core.errors import DataNotReadyError
+
+        from tests.helper import data_populate
+
+        config_dir = os.path.join(os.path.dirname(__file__), "data")
+        cfg4py.init(config_dir)
+
+        try:
+            await omicron.init()
+        except DataNotReadyError:
+            pass
+
+        await data_populate()
 
     def test_buy(self):
         date = datetime.datetime(2022, 3, 1, 10, 4)
         r = self.client.buy("002537.XSHE", 10, 500, order_time=date)
 
         self.assertEqual(r["security"], "002537.XSHE")
         self.assertAlmostEqual(r["price"], 9.420000076293945, 2)
         self.assertEqual(r["filled"], 500)
         self.assertEqual(r["time"], date)
 
         # no excpetion is ok
-        r = self.client.buy("002537.XSHE", 10, 500, order_time=date.isoformat())
+        r = self.client.buy("002537.XSHE", 10, 500, order_time=date)
 
     def test_info(self):
         # this also test available_money, balance
         info = self.client.info()
         self.assertEqual(info["available"], 1_000_000)
         self.assertEqual(info["assets"], 1_000_000)
         self.assertAlmostEqual(info["pnl"], 0, 2)
@@ -78,28 +109,28 @@
         self.assertAlmostEqual(balance["market_value"], 4750, 2)
         self.assertAlmostEqual(balance["assets"], 1000039.528, 2)
         self.assertAlmostEqual(balance["pnl"], 39.5289, 2)
         self.assertAlmostEqual(balance["ppnl"], 39.5289 / 1_000_000, 2)
 
     def test_positions(self):
         # this also test available_shares
-        positions = self.client.positions()
+        positions = self.client.positions
         self.assertEqual(0, positions.size)
 
         self.client.buy(
             "002537.XSHE", 10, 500, order_time=datetime.datetime(2022, 3, 1, 10, 4)
         )
 
-        positions = self.client.positions()
+        positions = self.client.positions
         self.assertListEqual(positions["security"].tolist(), ["002537.XSHE"])
         self.assertListEqual(positions["shares"].tolist(), [500])
         self.assertListEqual(positions["sellable"].tolist(), [0])
         np.testing.assert_array_almost_equal(positions["price"], [9.42], decimal=2)
 
-        positions = self.client.positions(datetime.date(2022, 3, 7))
+        positions = self.client.get_positions(datetime.date(2022, 3, 7))
         self.assertListEqual(positions["security"].tolist(), ["002537.XSHE"])
         self.assertListEqual(positions["shares"].tolist(), [500])
         self.assertListEqual(positions["sellable"].tolist(), [500])
         np.testing.assert_array_almost_equal(positions["price"], [9.42], decimal=2)
 
         # last_tradeday is still 2022, 3, 1, so the available_shares is 0
         r = self.client.available_shares("002537.XSHE")
@@ -160,15 +191,15 @@
             (9.57, 500, "2022-03-08 09:31:00"),
             (9.08, 500, "2022-03-09 09:31:00"),
             (9.1, 500, "2022-03-10 09:31:00"),
             (9.68, 500, "2022-03-11 09:31:00"),
             (9.65, 500, "2022-03-14 09:31:00"),
         ]:
             try:
-                self.client.buy(hljh, price, volume, order_time=tm)
+                self.client.buy(hljh, price, volume, order_time=arrow.get(tm).naive)
             except TradeError:
                 pass
 
         self.client.sell(
             hljh, 9.1, 5000, order_time=datetime.datetime(2022, 3, 14, 15, 0)
         )
 
@@ -212,7 +243,38 @@
 
         assets = self.client.get_assets()
         self.assertEqual(assets[0]["date"], datetime.date(2022, 3, 1))
         self.assertEqual(assets[-1]["date"], datetime.date(2022, 3, 14))
 
     def test_stop_backtest(self):
         self.client.stop_backtest()
+
+    async def test_buy_by_money(self):
+        await self._setup_omicron()
+
+        date = datetime.datetime(2022, 3, 1, 10, 4)
+
+        # fixed priced
+        r = await self.client.buy_by_money("002537.XSHE", 5000, 10, order_time=date)
+
+        self.assertEqual(r["security"], "002537.XSHE")
+        self.assertAlmostEqual(r["price"], 9.42, 2)
+        self.assertEqual(r["filled"], 500)
+        self.assertEqual(r["time"], date)
+
+        # first call, info should be invoked
+        self.assertAlmostEqual(self.client.available_money, 995289.53, 2)
+        self.assertTrue(self.client._is_dirty == False)
+
+        shares = self.client.available_shares("002537.XSHE")
+        self.assertEqual(shares, 0)
+        with mock.patch("traderclient.client.TraderClient.info") as mocked:
+            # 第二次调用，不从远端取
+            self.client.available_money
+            mocked.assert_not_called()
+
+        # no price provided, market buy
+        r = await self.client.buy_by_money("002537.XSHE", 5000, order_time=date)
+        self.assertEqual(r["security"], "002537.XSHE")
+        self.assertAlmostEqual(r["price"], 9.42, 2)
+        self.assertEqual(r["filled"], 500)
+        self.assertEqual(r["time"], date)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zillionare-trader-client-0.3.9/tests/test_transport.py` & `zillionare_trader_client-0.4.1/tests/test_transport.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import datetime
 import unittest
 
 import httpx
 
 from tests import MockServer, get_free_port
 from traderclient.client import TraderClient
 from traderclient.errors import TradeError
```

### Comparing `zillionare-trader-client-0.3.9/traderclient/client.py` & `zillionare_trader_client-0.4.1/traderclient/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 
 class TraderClient:
     """大富翁实盘和回测的客户端。
 
     在使用客户端时，需要先构建客户端实例，再调用其他方法，并处理[traderclient.errors.TradeError][]的异常，可以通过`status_code`和`message`来获取错误信息。如果是回测模式，一般会在回测结束时调用`metrics`方法来查看策略评估结果。如果要进一步查看信息，可以调用`bills`方法来获取历史持仓、交易记录和每日资产数据。
 
+    !!! Warn
+        此类实例既非线程安全，也非异步事件安全。即你不能在多个线程中，或者多个异步队列中使用它。
     """
 
     def __init__(
         self, url: str, acct: str, token: str, is_backtest: bool = False, **kwargs
     ):
         """构建一个交易客户端
 
@@ -45,22 +47,26 @@
         self._account = acct
         self.headers = {"Authorization": self._token}
         self.headers["Account"] = self._account
 
         self._is_backtest = is_backtest
 
         if is_backtest:
-            principal = kwargs.get("principal", 1_000_000)
+            self._principal = kwargs.get("principal", 1_000_000)
             commission = kwargs.get("commission", 1e-4)
             start = kwargs.get("start")
             end = kwargs.get("end")
             if start is None or end is None:
                 raise ValueError("start and end must be specified in backtest mode")
 
-            self._start_backtest(acct, token, principal, commission, start, end)
+            self._start_backtest(acct, token, self._principal, commission, start, end)
+
+        self._is_dirty = False
+        self._cash = None
+        self._positions = None
 
     def _cmd_url(self, cmd: str) -> str:
         return f"{self._url}/{cmd}"
 
     def _start_backtest(
         self,
         acct: str,
@@ -110,15 +116,17 @@
             - market_value: 股票市值
             - pnl: 盈亏(绝对值)
             - ppnl: 盈亏(百分比)，即pnl/principal
             - positions: 当前持仓，dtype为[position_dtype](https://zillionare.github.io/backtesting/0.3.2/api/trade/#backtest.trade.datatypes.position_dtype)的numpy structured array
 
         """
         url = self._cmd_url("info")
-        return get(url, headers=self.headers)
+        r = get(url, headers=self.headers)
+        self._is_dirty = False
+        return r
 
     def balance(self) -> Dict:
         """取该账号对应的账户余额信息
 
         Returns:
             Dict: 账户余额信息
 
@@ -147,17 +155,19 @@
     @property
     def available_money(self) -> float:
         """取当前账户的可用金额。策略函数可能需要这个数据进行仓位计算
 
         Returns:
             float: 账户可用资金
         """
-        url = self._cmd_url("info")
-        r = get(url, headers=self.headers)
-        return r.get("available")
+        if self._is_dirty or self._cash is None:
+            info = self.info()
+            self._cash = info.get("available")
+
+        return self._cash
 
     @property
     def principal(self) -> float:
         """账户本金
 
         Returns:
             本金
@@ -165,15 +175,27 @@
         if self._is_backtest:
             return self._principal
 
         url = self._cmd_url("info")
         r = get(url, headers=self.headers)
         return r.get("principal")
 
-    def positions(self, dt: datetime.date = None) -> np.ndarray:
+    @property
+    def positions(self):
+        """当前账户最新持仓"""
+        if self._is_dirty or self._positions is None:
+            url = self._cmd_url("positions")
+
+            r = get(url, headers=self.headers)
+
+            self._positions = r
+
+        return self._positions
+
+    def get_positions(self, dt: Optional[datetime.date] = None) -> np.ndarray:
         """取该子账户当前持仓信息
 
         Warning:
             在回测模式下，持仓信息不包含alias字段
 
         Args:
             dt: 指定日期，默认为None，表示取当前日期（最新）的持仓信息，trade server暂不支持此参数
@@ -193,25 +215,30 @@
 
         Args:
             security: 股票代码
 
         Returns:
             int: 指定股票今日可卖数量，无可卖即为0
         """
-        url = self._cmd_url("positions")
+        if self._is_dirty or self._positions is None:
+            url = self._cmd_url("positions")
 
-        r = get(url, headers=self.headers)
+            r = get(url, headers=self.headers)
 
-        found = r[r["security"] == security]
+            self._positions = r
+            # 此时持仓虽然同步了，但其它数据，比如cash并未同步，所以不能更改_is_dirty状态
+
+        found = self._positions[self._positions["security"] == security]
         if found.size == 1:
             return found["sellable"][0].item()
         elif found.size == 0:
             return 0
         else:
             logger.warning("found more than one position entry in response: %s", found)
+            raise ValueError(f"found more than one position entry in response: {found}")
 
     def today_entrusts(self) -> List:
         """查询账户当日所有委托，包括失败的委托
 
         此API在回测模式下不可用。
 
         Returns:
@@ -230,49 +257,79 @@
 
         Returns:
             Dict: 被取消的委托的信息，参考`buy`的结果
         """
         url = self._cmd_url("cancel_entrust")
 
         data = {"cid": cid}
+
+        self._is_dirty = True
         return post_json(url, params=data, headers=self.headers)
 
     def cancel_all_entrusts(self) -> List:
         """撤销当前所有未完成的委托，包括部分成交，不同交易系统实现不同
 
         此API在回测模式下不可用。
         Returns:
             List: 所有被撤的委托单信息，每个委托单的信息同buy
         """
         url = self._cmd_url("cancel_all_entrusts")
 
+        self._is_dirty = True
         return post_json(url, headers=self.headers)
 
+    async def buy_by_money(
+        self,
+        security: str,
+        money: float,
+        price: Optional[float] = None,
+        timeout: float = 0.5,
+        order_time: Optional[datetime.datetime] = None,
+        **kwargs,
+    ) -> Dict:
+        """按金额买入股票。
+
+        Returns:
+            参考[buy][traderclient.client.buy]
+        """
+        order_time = order_time or datetime.datetime.now()
+
+        if price is None:
+            price = await self._get_market_buy_price(security, order_time)
+            volume = int(money / price / 100) * 100
+
+            return self.market_buy(
+                security, volume, timeout=timeout, order_time=order_time
+            )
+        else:
+            volume = int(money / price / 100) * 100
+            return self.buy(security, price, volume, timeout, order_time)
+
     def buy(
         self,
         security: str,
         price: float,
         volume: int,
         timeout: float = 0.5,
-        order_time: Union[str, datetime.datetime] = None,
+        order_time: Optional[datetime.datetime] = None,
         **kwargs,
     ) -> Dict:
         """证券买入
 
         Notes:
             注意如果是回测模式，还需要传入order_time，因为回测模式下，服务器是不可能知道下单这一刻的时间的。注意在回测模式下，返回字段少于实盘。
 
             使用回测服务器时，无论成交实际上是在哪些时间点发生的，都使用order_time。在实盘模式下，则会分别返回create_at, recv_at两个字段
 
         Args:
             security (str): 证券代码
             price (float): 买入价格（限价）。在回测时，如果price指定为None，将转换为市价买入
-            volume (int): 买入股票数
+            volume (int): 买入股票数（非手数）
             timeout (float, optional): 默认等待交易反馈的超时为0.5秒
-            order_time Union[str, datetime.datetime]: 下单时间。在回测模式下使用。
+            order_time: 下单时间。在回测模式下使用。
 
         Returns:
             Dict: 成交返回
                 实盘返回以下字段：
 
                 {
                     "cid" : "xxx-xxxx-xxx",    # 券商给出的合同编号，内部名为entrust_no
@@ -317,35 +374,37 @@
             "price": price,
             "volume": volume,
             "timeout": timeout,
             **kwargs,
         }
 
         if self._is_backtest:
-            assert order_time is not None, "order_time is required in backtest mode"
-            if isinstance(order_time, datetime.datetime):
-                order_time = order_time.strftime("%Y-%m-%d %H:%M:%S")
-            parameters["order_time"] = order_time
+            if order_time is None:
+                raise ValueError("order_time is required in backtest mode")
+
+            _order_time = order_time.strftime("%Y-%m-%d %H:%M:%S")
+            parameters["order_time"] = _order_time
 
+        self._is_dirty = True
         r = post_json(url, params=parameters, headers=self.headers)
 
         for key in ("time", "created_at", "recv_at"):
             if key in r:
                 r[key] = arrow.get(r[key]).naive
 
         return r
 
     def market_buy(
         self,
         security: str,
         volume: int,
         order_type: OrderType = OrderType.MARKET,
-        limit_price: float = None,
+        limit_price: Optional[float] = None,
         timeout: float = 0.5,
-        order_time: Union[str, datetime.datetime] = None,
+        order_time: Optional[datetime.datetime] = None,
         **kwargs,
     ) -> Dict:
         """市价买入股票
 
         Notes:
 
             同花顺终端需要改为涨跌停限价，掘金客户端支持市价交易，掘金系统默认五档成交剩撤消。
@@ -355,15 +414,15 @@
 
         Args:
             security (str): 证券代码
             volume (int): 买入数量
             order_type (OrderType, optional): 市价买入类型，缺省为五档成交剩撤.
             limit_price (float, optional): 剩余转限价的模式下，设置的限价
             timeout (float, optional): 默认等待交易反馈的超时为0.5秒
-            order_time Union[str, datetime.datetime]: 下单时间。在回测模式下使用。
+            order_time: 下单时间。在回测模式下使用。
 
         Returns:
             Dict: 成交返回，详见`buy`方法
         """
         if volume != volume // 100 * 100:
             volume = volume // 100 * 100
             logger.warning("买入数量必须是100的倍数, 已取整到%d", volume)
@@ -376,47 +435,49 @@
             "order_type": order_type,
             "timeout": timeout,
             "limit_price": limit_price,
             **kwargs,
         }
 
         if self._is_backtest:
-            assert order_time is not None, "order_time is required in backtest mode"
-            if isinstance(order_time, datetime.datetime):
-                order_time = order_time.strftime("%Y-%m-%d %H:%M:%S")
-            parameters["order_time"] = order_time
+            if order_time is None:
+                raise ValueError("order_time is required in backtest mode")
+
+            _order_time = order_time.strftime("%Y-%m-%d %H:%M:%S")
+            parameters["order_time"] = _order_time
 
+        self._is_dirty = True
         r = post_json(url, params=parameters, headers=self.headers)
 
         for key in ("time", "created_at", "recv_at"):
             if key in r:
                 r[key] = arrow.get(r[key]).naive
 
         return r
 
     def sell(
         self,
         security: str,
         price: float,
         volume: int,
         timeout: float = 0.5,
-        order_time: Union[str, datetime.datetime] = None,
+        order_time: Optional[datetime.datetime] = None,
         **kwargs,
     ) -> Union[List, Dict]:
         """以限价方式卖出股票
 
         Notes:
             如果是回测模式，还需要传入order_time，因为回测模式下，服务器是不可能知道下单这一刻的时间的。如果服务器是回测服务器，则返回的数据为多个成交记录的列表（即使只包含一个数据）
 
         Args:
             security (str): 证券代码
             price (float): 买入价格（限价）。在回测中如果指定为None,将转换为市价卖出
             volume (int): 买入股票数
             timeout (float, optional): 默认等待交易反馈的超时为0.5秒
-            order_time Union[str, datetime.datetime]: 下单时间。在回测模式下使用。
+            order_time: 下单时间。在回测模式下使用。
 
         Returns:
             Union[List, Dict]: 成交返回，详见`buy`方法，trade server只返回一个委托单信息
         """
         # todo: check return type?
         url = self._cmd_url("sell")
         parameters = {
@@ -424,37 +485,40 @@
             "price": price,
             "volume": volume,
             "timeout": timeout,
             **kwargs,
         }
 
         if self._is_backtest:
-            assert order_time is not None, "order_time is required in backtest mode"
-            if isinstance(order_time, datetime.datetime):
-                order_time = order_time.strftime("%Y-%m-%d %H:%M:%S")
-            parameters["order_time"] = order_time
+            if order_time is None:
+                raise ValueError("order_time is required in backtest mode")
+
+            _order_time = order_time.strftime("%Y-%m-%d %H:%M:%S")
+            parameters["order_time"] = _order_time
 
+        self._is_dirty = True
         r = post_json(url, params=parameters, headers=self.headers)
         for key in ("created_at", "recv_at"):
             if key in r:
                 r[key] = arrow.get(r[key]).naive
 
-        for rec in r:
-            rec["time"] = arrow.get(rec["time"]).naive
+        if self._is_backtest:
+            for rec in r:
+                rec["time"] = arrow.get(rec["time"]).naive
 
         return r
 
     def market_sell(
         self,
         security: str,
         volume: int,
         order_type: OrderType = OrderType.MARKET,
-        limit_price: float = None,
+        limit_price: Optional[float] = None,
         timeout: float = 0.5,
-        order_time: Union[str, datetime.datetime] = None,
+        order_time: Optional[datetime.datetime] = None,
         **kwargs,
     ) -> Union[List, Dict]:
         """市价卖出股票
 
         Notes:
             同花顺终端需要改为涨跌停限价，掘金客户端支持市价交易，掘金系统默认五档成交剩撤
 
@@ -464,15 +528,15 @@
 
         Args:
             security (str): 证券代码
             volume (int): 卖出数量
             order_type (OrderType, optional): 市价卖出类型，缺省为五档成交剩撤.
             limit_price (float, optional): 剩余转限价的模式下，设置的限价
             timeout (float, optional): 默认等待交易反馈的超时为0.5秒
-            order_time Union[str, datetime.datetime]: 下单时间。在回测模式下使用。
+            order_time: 下单时间。在回测模式下使用。
         Returns:
             Union[List, Dict]: 成交返回，详见`buy`方法，trade server只返回一个委托单信息
         """
         url = self._cmd_url("market_sell")
         parameters = {
             "security": security,
             "price": 0,
@@ -480,33 +544,79 @@
             "order_type": order_type,
             "timeout": timeout,
             "limit_price": limit_price,
             **kwargs,
         }
 
         if self._is_backtest:
-            assert order_time is not None, "order_time is required in backtest mode"
-            if isinstance(order_time, datetime.datetime):
-                order_time = order_time.strftime("%Y-%m-%d %H:%M:%S")
-            parameters["order_time"] = order_time
+            if order_time is None:
+                raise ValueError("order_time is required in backtest mode")
+
+            _order_time = order_time.strftime("%Y-%m-%d %H:%M:%S")
+            parameters["order_time"] = _order_time
 
+        self._is_dirty = True
         r = post_json(url, params=parameters, headers=self.headers)
         for key in ("time", "created_at", "recv_at"):
             if key in r:
                 r[key] = arrow.get(r[key]).naive
 
         return r
 
+    async def _get_market_sell_price(
+        self, sec: str, order_time: Optional[datetime.datetime] = None
+    ) -> float:
+        """获取当前股票的市价卖出价格
+
+        如果无法取得跌停价，则以当前价卖出。
+        """
+        from coretypes import FrameType
+        from omicron.models.stock import Stock
+
+        order_time = order_time or datetime.datetime.now()
+        frame = order_time.date()
+        limit_prices = await Stock.get_trade_price_limits(sec, frame, frame)
+        if len(limit_prices) >= 0:
+            price = limit_prices["low_limit"][0]
+        else:
+            price = (await Stock.get_bars(sec, 1, FrameType.MIN1, end=order_time))[
+                "close"
+            ][0]
+
+        return price.item()
+
+    async def _get_market_buy_price(
+        self, sec: str, order_time: Optional[datetime.datetime] = None
+    ) -> float:
+        """获取当前股票的市价买入价格
+
+        如果无法取得涨停价，则以当前价买入。
+        """
+        from coretypes import FrameType
+        from omicron.models.stock import Stock
+
+        order_time = order_time or datetime.datetime.now()
+        frame = order_time.date()
+        limit_prices = await Stock.get_trade_price_limits(sec, frame, frame)
+        if len(limit_prices) >= 0:
+            price = limit_prices["high_limit"][0]
+        else:
+            price = (await Stock.get_bars(sec, 1, FrameType.MIN1, end=order_time))[
+                "close"
+            ][0]
+
+        return price.item()
+
     def sell_percent(
         self,
         security: str,
         price: float,
         percent: float,
-        timeout: int = 0.5,
-        order_time: Union[str, datetime.datetime] = None,
+        timeout: float = 0.5,
+        order_time: Optional[datetime.datetime] = None,
         **kwargs,
     ) -> Union[List, Dict]:
         """按比例卖出特定的股票（基于可卖股票数），比例的数字由调用者提供
 
         Notes:
             注意实现中存在取整问题。比如某支股票当前有500股可卖，如果percent=0.3，则要求卖出150股。实际上卖出的将是100股。
 
@@ -517,32 +627,34 @@
             time_out (int, optional): 缺省超时为0.5秒
             order_time: 下单时间。在回测模式下使用。
 
         Returns:
             Union[List, Dict]: 股票卖出委托单的详细信息，于sell指令相同
         """
         if percent <= 0 or percent > 1:
-            return None
+            raise ValueError(f"percent should between [0, 1]")
         if len(security) < 6:
-            return None
+            raise ValueError(f"wrong security format {security}")
 
         url = self._cmd_url("sell_percent")
         parameters = {
             "security": security,
             "price": price,
             "timeout": timeout,
             "percent": percent,
         }
 
         if self._is_backtest:
-            assert order_time is not None, "order_time is required in backtest mode"
-            if isinstance(order_time, datetime.datetime):
-                order_time = order_time.strftime("%Y-%m-%d %H:%M:%S")
-            parameters["order_time"] = order_time
+            if order_time is None:
+                raise ValueError("order_time is required in backtest mode")
+
+            _order_time = order_time.strftime("%Y-%m-%d %H:%M:%S")
+            parameters["order_time"] = _order_time
 
+        self._is_dirty = True
         r = post_json(url, params=parameters, headers=self.headers)
         for key in ("time", "created_at", "recv_at"):
             if key in r:
                 r[key] = arrow.get(r[key]).naive
 
         return r
 
@@ -555,26 +667,27 @@
             percent (float): 调用者给出的百分比，(0, 1]
             time_out (int, optional): 缺省超时为0.5秒
 
         Returns:
             List: 所有卖出股票的委托单信息，于sell指令相同
         """
         if percent <= 0 or percent > 1:
-            return None
+            raise ValueError(f"percent should between [0, 1]")
 
         url = self._cmd_url("sell_all")
         parameters = {"percent": percent, "timeout": timeout}
 
+        self._is_dirty = True
         return post_json(url, params=parameters, headers=self.headers)
 
     def metrics(
         self,
-        start: datetime.date = None,
-        end: datetime.date = None,
-        baseline: str = None,
+        start: Optional[datetime.date] = None,
+        end: Optional[datetime.date] = None,
+        baseline: Optional[str] = None,
     ) -> Dict:
         """获取指定时间段[start, end]间的账户指标评估数据
 
         Args:
             start: 起始日期
             end: 结束日期
             baseline: the security code for baseline
@@ -626,30 +739,32 @@
             - tx
         """
         url = self._cmd_url("bills")
         return get(url, headers=self.headers)
 
     def get_assets(
         self,
-        start: Union[str, datetime.date] = None,
-        end: Union[str, datetime.date] = None,
+        start: Optional[datetime.date] = None,
+        end: Optional[datetime.date] = None,
     ) -> np.ndarray:
         """获取账户在[start, end]时间段内的资产信息。
 
         此数据可用以资产曲线的绘制。
 
         Args:
             start: 起始日期
             end: 结束日期
 
         Returns:
             np.ndarray: 账户在[start, end]时间段内的资产信息，是一个dtype为[rich_assets_dtype](https://zillionare.github.io/backtesting/0.4.0/api/trade/#backtest.trade.datatypes.rich_assets_dtype)的numpy structured array
         """
         url = self._cmd_url("assets")
-        return get(url, headers=self.headers, params={"start": start, "end": end})
+        _start = start.strftime("%Y-%m-%d") if start else None
+        _end = end.strftime("%Y-%m-%d") if end else None
+        return get(url, headers=self.headers, params={"start": _start, "end": _end})
 
     def stop_backtest(self):
         """停止回测。
 
         此API仅在回测模式下可用。其作用是冻结回测账户，并计算回测的各项指标。在未调用本API前，调用`metrics`也能同样获取到回测的各项指标，但如果需要多次调用`metrics`，则账户在冻结之后，由于指标不再需要更新，因而速度会更快。
 
         另外，在[zillionare-backtest](https://zillionare.github.io/backtesting/)的未来版本中,将可能使用本方法来实现回测数据的持久化保存，因此，建议您从现在起就确保在回测后调用本方法。
```

### Comparing `zillionare-trader-client-0.3.9/traderclient/demo.py` & `zillionare_trader_client-0.4.1/traderclient/demo.py`

 * *Files 8% similar despite different names*

```diff
@@ -111,26 +111,28 @@
 
     print("\n------------- cancel_entrust --------------")
     result = client.cancel_entrust("50f5aaee-6fa8-470c-a630-39b43bc9dda7")
     if result is None:
         return None
     print(result)
 
+
 def test_trade_cancel_all():
     url = "http://192.168.100.133:8000/api/trade/v0.1"
     acct = "henry"
     token = "29b7cce7-e9bb-4510-9231-6d492750b4db"
 
     # initialize client instance
     client = TraderClient(url, acct, token)
 
     print("\n------------- cancel_all_entrust --------------")
     result = client.cancel_all_entrusts()
     print(result)
 
+
 def test_trade_buy():
     url = "http://192.168.100.133:8000/api/trade/v0.1"
     acct = "henry"
     token = "29b7cce7-e9bb-4510-9231-6d492750b4db"
 
     # initialize client instance
     client = TraderClient(url, acct, token)
@@ -143,26 +145,45 @@
     print(result)
     # buy for cancel
     result = client.buy(security="002537.XSHE", price=6.97, volume=600)
     if result is None:
         return None
     print(result)
 
+
 def test_trade_market_buy():
     url = "http://192.168.100.133:8000/api/trade/v0.1"
     acct = "henry"
     token = "29b7cce7-e9bb-4510-9231-6d492750b4db"
 
     # initialize client instance
     client = TraderClient(url, acct, token)
 
     print("\n------------- market_buy --------------")
     rsp = client.market_buy(security="002537.XSHE", price=7.8, volume=500)
     print(rsp)
 
+
+def test_for_nginx():
+    url = "http://203.189.206.225:9100/api/trade/v0.1"
+    acct = "guobotest"
+    token = "b1733675-f525-49e9-82c4-a91360ec36e6"
+
+    # initialize client instance
+    client = TraderClient(url, acct, token)
+
+    try:
+        result = client.info()
+        if result is None:
+            logger.error("failed to get information")
+        print(result)
+    except Exception as e:
+        print(e)
+
+
 def test_trade_sell():
     url = "http://192.168.100.133:8000/api/trade/v0.1"
     acct = "henry"
     token = "29b7cce7-e9bb-4510-9231-6d492750b4db"
 
     # initialize client instance
     client = TraderClient(url, acct, token)
@@ -234,46 +255,14 @@
     end = datetime.datetime(2022, 3, 10, 9, 35)
     result = client.get_entrusts_in_range(start=start, end=end)
     if result is None:
         return None
 
     print(result)
 
+
 def trade_test_entry():
     test_trade_market_buy()
 
-# the following fits backtesting server only
-
-
-def backtest_trade():
-    import uuid
-
-    url = "http://192.168.100.114:7080/backtest/api/trade/v0.3/"
-
-    token = uuid.uuid4().hex
-    account = f"my-great-strategy-v1-{token[-4:]}"
-    start = datetime.date(2022, 5, 18)
-    end = datetime.date(2022, 5, 25)
-    client: TraderClient = TraderClient(
-        url, account, token, is_backtest=True, start=start, end=end
-    )
-
-    code = "000001.XSHE"
-
-    buy = client.buy(code, 16, 200, order_time="2022-05-20 09:31:00")
-    print(buy)
-
-    sell = client.sell_percent(
-        code, 10.1, 0.5, order_time=datetime.datetime(2022, 5, 23, 14, 57)
-    )
-    print(sell)
-    sell = client.sell(code, 10.1, 1000, order_time="2022-05-23 14:57:00")
-    print(sell)
-
-    print(client.metrics())
-    print(client.bills())
-    print(client.get_assets())
-
 
 if __name__ == "__main__":
-    #backtest_trade()
-    trade_test_entry()
+    test_for_nginx()
```

### Comparing `zillionare-trader-client-0.3.9/traderclient/transport.py` & `zillionare_trader_client-0.4.1/traderclient/transport.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import logging
 import os
 import pickle
 import uuid
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 import httpx
 
 from traderclient.utils import get_cmd, status_ok
 
 from .errors import TradeError
 
 logger = logging.getLogger(__name__)
 
 
-def timeout(params: dict = None) -> int:
+def timeout(params: Optional[dict] = None) -> int:
     """determine timeout value for httpx request
 
     if there's envar "TRADER_CLIENT_TIMEOUT", it will precedes, then the max of user timeout and default 30
 
     Args:
         params : user specified in request
 
     Returns:
         timeout
     """
     if os.environ.get("TRADER_CLIENT_TIMEOUT"):
-        return int(os.environ.get("TRADER_CLIENT_TIMEOUT"))
+        return int(os.environ.get("TRADER_CLIENT_TIMEOUT", "5"))
 
     if params is None or params.get("timeout") is None:
         return 30
 
-    return max(params.get("timeout"), 30)
+    return max(params.get("timeout", 5), 30)
 
 
-def process_response_result(rsp: httpx.Response, cmd: str = None) -> Any:
+def process_response_result(rsp: httpx.Response, cmd: Optional[str] = None) -> Any:
     """获取响应中的数据，并检查结果合法性
 
     Args:
         rsp (response): HTTP response object
         cmd (str, optional): trade instuction
 
     Raises:
@@ -61,15 +61,15 @@
     if rsp.status_code == 499:
         logger.warning("%s failed: %s, %s", cmd, rsp.status_code, rsp.text)
         raise TradeError(rsp.status_code, rsp.text)
     else:
         rsp.raise_for_status()
 
 
-def get(url, params=None, headers=None) -> Any:
+def get(url, params: Optional[dict] = None, headers=None) -> Any:
     """发送GET请求到上游服务接口
 
     Args:
         url : 目标URL，带服务器信息
         params : JSON格式的参数清单
         headers : 额外的header选项
 
@@ -105,15 +105,15 @@
 
     action = get_cmd(url)
     result = process_response_result(rsp, action)
 
     return result
 
 
-def delete(url, params=None, headers=None) -> Any:
+def delete(url, params: Optional[Dict] = None, headers=None) -> Any:
     """从服务器上删除资源
 
     Args:
         url : 目标URL，带服务器信息
         params : 查询参数
         headers : 额外的header选项
```

### Comparing `zillionare-trader-client-0.3.9/traderclient/utils.py` & `zillionare_trader_client-0.4.1/traderclient/utils.py`

 * *Files identical despite different names*

### Comparing `zillionare-trader-client-0.3.9/PKG-INFO` & `zillionare_trader_client-0.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 Metadata-Version: 2.1
 Name: zillionare-trader-client
-Version: 0.3.9
+Version: 0.4.1
 Summary: Zillionare Trader Client
 Home-page: https://github.com/zillionare/trader-client
 License: MIT
 Author: Aaron Yang
 Author-email: code@jieyu.ai
 Requires-Python: >=3.8,<3.9
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
-Requires-Dist: arrow (>=1.2.2,<2.0.0)
-Requires-Dist: black (>=22.3.0,<23.0.0); extra == "test"
-Requires-Dist: fire (>=0.4.0,<0.5.0)
-Requires-Dist: flake8 (==3.8.4); extra == "test"
-Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0); extra == "test"
-Requires-Dist: httpx (>=0.16,<0.17)
-Requires-Dist: isort (==5.6.4); extra == "test"
-Requires-Dist: livereload (>=2.6.3,<3.0.0); extra == "doc"
-Requires-Dist: mike (>=1.1.2,<2.0.0); extra == "doc"
-Requires-Dist: mkdocs (>=1.2.3,<2.0.0); extra == "doc"
-Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0); extra == "doc"
-Requires-Dist: mkdocs-include-markdown-plugin (>=3.2.3,<4.0.0); extra == "doc"
-Requires-Dist: mkdocs-material (>=8.1.11,<9.0.0); extra == "doc"
+Requires-Dist: arrow (>=1.2.3,<2.0.0)
+Requires-Dist: black (>=22.3.0,<23.0.0) ; extra == "test"
+Requires-Dist: flake8 (==3.8.4) ; extra == "test"
+Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "test"
+Requires-Dist: httpx (>=0.23,<0.24)
+Requires-Dist: isort (==5.6.4) ; extra == "test"
+Requires-Dist: livereload (>=2.6.3,<3.0.0) ; extra == "doc"
+Requires-Dist: mike (>=1.1.2,<2.0.0) ; extra == "doc"
+Requires-Dist: mkdocs (>=1.2.3,<2.0.0) ; extra == "doc"
+Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0) ; extra == "doc"
+Requires-Dist: mkdocs-include-markdown-plugin (>=3.2.3,<4.0.0) ; extra == "doc"
+Requires-Dist: mkdocs-material (>=8.1.11,<9.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material-extensions (>=1.0.3,<2.0.0)
-Requires-Dist: mkdocstrings (>=0.18.0,<0.19.0); extra == "doc"
-Requires-Dist: numpy (>=1.22.4,<2.0.0)
-Requires-Dist: pip (>=20.3.1,<21.0.0); extra == "dev"
-Requires-Dist: pre-commit (>=2.12.0,<3.0.0); extra == "dev"
-Requires-Dist: pytest (==6.1.2); extra == "test"
-Requires-Dist: pytest-cov (==2.10.1); extra == "test"
-Requires-Dist: sanic (>=22.3.2,<23.0.0); extra == "test"
-Requires-Dist: toml (>=0.10.2,<0.11.0); extra == "dev"
-Requires-Dist: tox (>=3.20.1,<4.0.0); extra == "dev"
-Requires-Dist: twine (>=3.3.0,<4.0.0); extra == "dev"
-Requires-Dist: virtualenv (>=20.2.2,<21.0.0); extra == "dev"
+Requires-Dist: mkdocstrings (>=0.18.0,<0.19.0) ; extra == "doc"
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Requires-Dist: pre-commit (>=2.12.0,<3.0.0) ; extra == "dev"
+Requires-Dist: pytest-cov (==2.10.1) ; extra == "test"
+Requires-Dist: sanic (>=23.3.0,<24.0.0) ; extra == "test"
+Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev"
+Requires-Dist: tox (>=3.20.1,<4.0.0) ; extra == "dev"
+Requires-Dist: twine (>=3.3.0,<4.0.0) ; extra == "dev"
 Description-Content-Type: text/markdown
 
 # 大富翁交易客户端
 
 trade-client是大富翁量化框架中用来交易的客户端。它对回测和实盘提供了几乎相同的接口，从而使得经过回测的策略，可以无缝切换到实盘环境中。
 
 ## 功能
```

