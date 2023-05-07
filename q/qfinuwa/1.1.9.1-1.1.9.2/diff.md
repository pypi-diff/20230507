# Comparing `tmp/qfinuwa-1.1.9.1.tar.gz` & `tmp/qfinuwa-1.1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfinuwa-1.1.9.1.tar", last modified: Sat May  6 09:42:16 2023, max compression
+gzip compressed data, was "qfinuwa-1.1.9.2.tar", last modified: Sun May  7 06:36:47 2023, max compression
```

## Comparing `qfinuwa-1.1.9.1.tar` & `qfinuwa-1.1.9.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:42:16.641391 qfinuwa-1.1.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-05-06 09:42:16.641391 qfinuwa-1.1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-06 09:42:16.641391 qfinuwa-1.1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:42:16.637391 qfinuwa-1.1.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:42:16.641391 qfinuwa-1.1.9.1/src/qfinuwa/
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/API.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17211 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/backtester.py
--rw-r--r--   0 runner    (1001) docker     (123)    13962 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/indicators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:42:16.641391 qfinuwa-1.1.9.1/src/qfinuwa/opt/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/opt/_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/opt/_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/opt/_stockdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-06 09:42:05.000000 qfinuwa-1.1.9.1/src/qfinuwa/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:42:16.641391 qfinuwa-1.1.9.1/src/qfinuwa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-05-06 09:42:16.000000 qfinuwa-1.1.9.1/src/qfinuwa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-06 09:42:16.000000 qfinuwa-1.1.9.1/src/qfinuwa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 09:42:16.000000 qfinuwa-1.1.9.1/src/qfinuwa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-06 09:42:16.000000 qfinuwa-1.1.9.1/src/qfinuwa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-06 09:42:16.000000 qfinuwa-1.1.9.1/src/qfinuwa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:36:47.137105 qfinuwa-1.1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-07 06:36:36.000000 qfinuwa-1.1.9.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-05-07 06:36:47.137105 qfinuwa-1.1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-07 06:36:36.000000 qfinuwa-1.1.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-07 06:36:36.000000 qfinuwa-1.1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-07 06:36:47.137105 qfinuwa-1.1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-07 06:36:36.000000 qfinuwa-1.1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:36:47.137105 qfinuwa-1.1.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:36:47.137105 qfinuwa-1.1.9.2/src/qfinuwa/
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-05-07 06:36:36.000000 qfinuwa-1.1.9.2/src/qfinuwa/API.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-07 06:36:36.000000 qfinuwa-1.1.9.2/src/qfinuwa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17211 2023-05-07 06:36:36.000000 qfinuwa-1.1.9.2/src/qfinuwa/backtester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13962 2023-05-07 06:36:36.000000 qfinuwa-1.1.9.2/src/qfinuwa/indicators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:36:47.137105 qfinuwa-1.1.9.2/src/qfinuwa/opt/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-07 06:36:36.000000 qfinuwa-1.1.9.2/src/qfinuwa/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-07 06:36:36.000000 qfinuwa-1.1.9.2/src/qfinuwa/opt/_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-07 06:36:36.000000 qfinuwa-1.1.9.2/src/qfinuwa/opt/_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-07 06:36:36.000000 qfinuwa-1.1.9.2/src/qfinuwa/opt/_stockdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-07 06:36:36.000000 qfinuwa-1.1.9.2/src/qfinuwa/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-07 06:36:36.000000 qfinuwa-1.1.9.2/src/qfinuwa/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:36:47.137105 qfinuwa-1.1.9.2/src/qfinuwa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-05-07 06:36:47.000000 qfinuwa-1.1.9.2/src/qfinuwa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-07 06:36:47.000000 qfinuwa-1.1.9.2/src/qfinuwa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 06:36:47.000000 qfinuwa-1.1.9.2/src/qfinuwa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 06:36:47.000000 qfinuwa-1.1.9.2/src/qfinuwa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-07 06:36:47.000000 qfinuwa-1.1.9.2/src/qfinuwa.egg-info/top_level.txt
```

### Comparing `qfinuwa-1.1.9.1/LICENSE.txt` & `qfinuwa-1.1.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.9.1/PKG-INFO` & `qfinuwa-1.1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qfinuwa
-Version: 1.1.9.1
+Version: 1.1.9.2
 Summary: Framework for backtesting quantitative trading algorithims.
 Home-page: https://github.com/QFinUWA/algo-backtester/issues
 Author: Isaac Bergl
 Author-email: tberg644@gmail.com
 Project-URL: Bug Tracker, https://github.com/QFinUWA/algo-backtester/issues
 Project-URL: repository, https://github.com/QFinUWA/algo-backtester
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qfinuwa-1.1.9.1/README.md` & `qfinuwa-1.1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.9.1/setup.cfg` & `qfinuwa-1.1.9.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = QFinUWA
-version = 1.1.9.1
+version = 1.1.9.2
 author = Isaac Bergl
 author_email = tberg644@gmail.com
 description = A backtesting framework for quantitative finance for QFIN UWA.
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/QFinUWA/algo-backtester/issues
 project_urls =
```

### Comparing `qfinuwa-1.1.9.1/src/qfinuwa/API.py` & `qfinuwa-1.1.9.2/src/qfinuwa/API.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.9.1/src/qfinuwa/backtester.py` & `qfinuwa-1.1.9.2/src/qfinuwa/backtester.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.9.1/src/qfinuwa/indicators.py` & `qfinuwa-1.1.9.2/src/qfinuwa/indicators.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.9.1/src/qfinuwa/opt/_portfolio.py` & `qfinuwa-1.1.9.2/src/qfinuwa/opt/_portfolio.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     @curr_prices.setter
     def curr_prices(self, prices: dict):
         self._i += 1
         self._curr_prices = prices
 
         for s in self._stocks:
-            self._value[s].append((self._delta[s]*self._curr_prices[s] + self._capital[s], self._fees_paid[s]))
+            self._value[s].append((self._delta[s]*self._curr_prices[s], self._capital[s], self._fees_paid[s]))
 
     #---------------[Public Methods]-----------------#
 
     def order(self, stock: str, quantity: Union[int, float]) -> bool:
         
         if abs(self._delta[stock] + quantity) > self._delta_limits[stock]:
             return False 
@@ -68,14 +68,15 @@
         self._trades.append((self._i, stock, quantity))
         return True
     
         
     def wrap_up(self):
         for stock in self._stocks:
             self.order(stock, -self._delta[stock])
+        self.curr_prices = self.curr_prices
         return (self._value,  self._trades)
     
 
     #---------------[Internal Methods]-----------------#
     def __str__(self):
         table = str(tabulate(list(self._delta.items()), 
                                 headers = ['Stock', 'Delta'],
```

### Comparing `qfinuwa-1.1.9.1/src/qfinuwa/opt/_result.py` & `qfinuwa-1.1.9.2/src/qfinuwa/opt/_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
         datetimeindex = datetimeindex[self._start: self._end]
 
         self.buys = [(i,s,q) for i, s,q in trades if q > 0]
         self.sells = [(i, s,-q) for i,s,q in trades if q < 0]
 
         self.n_buys = {stock: len([q for i,s,q in self.buys if s == stock]) for stock in stocks}
         self.n_sells = {stock: len([-q for i,s,q in self.sells if s == stock]) for stock in stocks}
-        self.gross_pnl = {stock: value[stock][-1][0] for stock in stocks}
-        self.fees_paid = {stock: value[stock][-1][1] for stock in stocks}
-        self.net_pnl = {stock: value[stock][-1][0] - value[stock][-1][1]  for stock in stocks}
+        self.gross_pnl = {stock: value[stock][-1][1] for stock in stocks}
+        self.fees_paid = {stock: value[stock][-1][2] for stock in stocks}
+        self.net_pnl = {stock: value[stock][-1][1] - value[stock][-1][2]  for stock in stocks}
 
         self.value = value
         self._datetimeindex = datetimeindex.reset_index(drop=True)
         self._stocks = stocks
 
         self._stockdata = stockdata._stock_df
```

### Comparing `qfinuwa-1.1.9.1/src/qfinuwa/opt/_stockdata.py` & `qfinuwa-1.1.9.2/src/qfinuwa/opt/_stockdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,18 +52,17 @@
                 self._index = pd.to_datetime(_df['time'])
 
             # if stock == 'SPY':
             #     self.spy = _df['close'].to_numpy()
 
             self._stock_df[stock] = _df[self._measurement]
         self._data = self._compress_data()
-
         # pre calcualte the price at every iteration for efficiency
         self._prices = np.array([{stock: self._data[i, 1 + s*5]
-                                for s, stock in enumerate(stocks)} for i in range(self._L)])
+                                for s, stock in enumerate(self._stocks)} for i in range(self._L)])
 
         self.sinames = [(measurement, stock , i) for i, (stock, measurement) in 
                         enumerate(product(self._stocks, self._measurement))]
     
     #---------------[Properties]-----------------#
     @property
     def stocks(self):
```

### Comparing `qfinuwa-1.1.9.1/src/qfinuwa/plotting.py` & `qfinuwa-1.1.9.2/src/qfinuwa/plotting.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.9.1/src/qfinuwa/strategy.py` & `qfinuwa-1.1.9.2/src/qfinuwa/strategy.py`

 * *Files identical despite different names*

### Comparing `qfinuwa-1.1.9.1/src/qfinuwa.egg-info/PKG-INFO` & `qfinuwa-1.1.9.2/src/qfinuwa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qfinuwa
-Version: 1.1.9.1
+Version: 1.1.9.2
 Summary: Framework for backtesting quantitative trading algorithims.
 Home-page: https://github.com/QFinUWA/algo-backtester/issues
 Author: Isaac Bergl
 Author-email: tberg644@gmail.com
 Project-URL: Bug Tracker, https://github.com/QFinUWA/algo-backtester/issues
 Project-URL: repository, https://github.com/QFinUWA/algo-backtester
 Classifier: Programming Language :: Python :: 3
```

