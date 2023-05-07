# Comparing `tmp/cvxsimulator-0.1.3.tar.gz` & `tmp/cvxsimulator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.1.3.tar", max compression
+gzip compressed data, was "cvxsimulator-0.2.0.tar", max compression
```

## Comparing `cvxsimulator-0.1.3.tar` & `cvxsimulator-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1102 2023-05-05 04:02:45.893140 cvxsimulator-0.1.3/LICENSE
--rw-r--r--   0        0        0     4477 2023-05-05 04:02:45.893140 cvxsimulator-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-05-05 04:02:45.929141 cvxsimulator-0.1.3/cvx/simulator/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-05 04:02:45.929141 cvxsimulator-0.1.3/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     4917 2023-05-05 04:02:45.929141 cvxsimulator-0.1.3/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      464 2023-05-05 04:02:45.929141 cvxsimulator-0.1.3/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      537 2023-05-05 04:03:08.787907 cvxsimulator-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5037 1970-01-01 00:00:00.000000 cvxsimulator-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-05-07 03:49:46.163568 cvxsimulator-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4473 2023-05-07 03:49:46.163568 cvxsimulator-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 03:49:46.167568 cvxsimulator-0.2.0/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-07 03:49:46.167568 cvxsimulator-0.2.0/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     1520 2023-05-07 03:49:46.167568 cvxsimulator-0.2.0/cvx/simulator/month.py
+-rw-r--r--   0        0        0     5814 2023-05-07 03:49:46.167568 cvxsimulator-0.2.0/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      464 2023-05-07 03:49:46.167568 cvxsimulator-0.2.0/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      541 2023-05-07 03:50:40.831761 cvxsimulator-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5033 1970-01-01 00:00:00.000000 cvxsimulator-0.2.0/PKG-INFO
```

### Comparing `cvxsimulator-0.1.3/LICENSE` & `cvxsimulator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.1.3/README.md` & `cvxsimulator-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 ```python
 for _, now, state in portfolio:
     # each day we invest a quarter of the capital in the assets
     portfolio[now] = 0.25 * state.nav / state.prices
 ```
 
 Note that we update the position at time `now` using a series of actual stocks rather than weights or cashpositions.
-Future versions of this package may support such conventions, too.
+The portfolio class also exposes setters for such conventions.
 
 ### Analyse results
 
 The loop above is filling up the desired positions. The portfolio object is now ready for further analysis.
 It is possible dive into the data, e.g.
 
 ```python
```

### Comparing `cvxsimulator-0.1.3/cvx/simulator/metrics.py` & `cvxsimulator-0.2.0/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.1.3/cvx/simulator/portfolio.py` & `cvxsimulator-0.2.0/cvx/simulator/portfolio.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 import pandas as pd
 
 from cvx.simulator.trading_costs import LinearCostModel, TradingCostModel
 
 
 @dataclass
 class _State:
@@ -55,38 +55,67 @@
 
 @dataclass(frozen=True)
 class _EquityPortfolio:
     prices: pd.DataFrame
     stocks: pd.DataFrame
     trading_cost_model: TradingCostModel
     initial_cash: float = 1e6
-    _state: _State = _State()
+    _state: _State = field(default_factory=_State)
 
     def __post_init__(self):
         self._state.position = self.stocks.loc[self.index[0]]
         self._state.prices = self.prices.loc[self.index[0]]
         self._state.cash = self.initial_cash - self._state.value
 
     @property
     def index(self):
         return self.prices.index
 
     @property
     def assets(self):
         return self.prices.columns
 
+    def set_weights(self, time, weights):
+        """
+        Set the position via weights (e.g. fractions of the nav)
+
+        :param time: time
+        :param weights: series of weights
+        """
+        self[time] = (self._state.nav * weights) / self._state.prices
+
+    def set_cashposition(self, time, cashposition):
+        """
+        Set the position via cash positions (e.g. USD invested per asset)
+
+        :param time: time
+        :param cashposition: series of cash positions
+        """
+        self[time] = cashposition / self._state.prices
+
+    def set_position(self, time, position):
+        """
+        Set the position via number of assets (e.g. number of stocks)
+
+        :param time: time
+        :param position: series of number of stocks
+        """
+        self[time] = position
+
     def __iter__(self):
         for before, now in zip(self.index[:-1], self.index[1:]):
             # valuation of the current position
             self._state.prices = self.prices.loc[now]
 
             yield before, now, self._state
 
     def __setitem__(self, key, position):
         assert isinstance(position, pd.Series)
+        assert set(position.index).issubset(set(self.assets))
+
         self.stocks.loc[key, position.index] = position
         self._state.update(position, model=self.trading_cost_model)
 
     def __getitem__(self, item):
         assert item in self.index
         return self.stocks.loc[item]
```

### Comparing `cvxsimulator-0.1.3/PKG-INFO` & `cvxsimulator-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.1.3
+Version: 0.2.0
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -79,15 +79,15 @@
 ```python
 for _, now, state in portfolio:
     # each day we invest a quarter of the capital in the assets
     portfolio[now] = 0.25 * state.nav / state.prices
 ```
 
 Note that we update the position at time `now` using a series of actual stocks rather than weights or cashpositions.
-Future versions of this package may support such conventions, too.
+The portfolio class also exposes setters for such conventions.
 
 ### Analyse results
 
 The loop above is filling up the desired positions. The portfolio object is now ready for further analysis.
 It is possible dive into the data, e.g.
 
 ```python
```

