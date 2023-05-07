# Comparing `tmp/py-portfolio-tools-0.0.7.tar.gz` & `tmp/py-portfolio-tools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-portfolio-tools-0.0.7.tar", last modified: Fri May  5 17:32:19 2023, max compression
+gzip compressed data, was "py-portfolio-tools-0.0.8.tar", last modified: Sun May  7 12:12:53 2023, max compression
```

## Comparing `py-portfolio-tools-0.0.7.tar` & `py-portfolio-tools-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 17:32:19.437162 py-portfolio-tools-0.0.7/
--rw-rw-rw-   0        0        0     1075 2023-04-17 11:45:54.000000 py-portfolio-tools-0.0.7/LICENSE.md
--rw-rw-rw-   0        0        0     1198 2023-05-05 17:32:19.437162 py-portfolio-tools-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-04-17 11:54:14.000000 py-portfolio-tools-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 17:32:19.437162 py-portfolio-tools-0.0.7/py-portfolio-tools/
--rw-rw-rw-   0        0        0     2545 2023-04-17 18:42:57.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/DataFetch.py
--rw-rw-rw-   0        0        0      703 2023-04-17 13:42:55.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/Logger.py
--rw-rw-rw-   0        0        0     8330 2023-05-05 17:32:02.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/Portfolio.py
--rw-rw-rw-   0        0        0     3232 2023-04-23 17:24:00.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/PortfolioInputWindow.py
--rw-rw-rw-   0        0        0     8397 2023-05-05 11:08:15.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/PortfolioManager.py
--rw-rw-rw-   0        0        0       30 2023-04-17 14:28:58.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/Predictor.py
--rw-rw-rw-   0        0        0     3151 2023-05-05 11:22:09.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/StocksAllocator.py
--rw-rw-rw-   0        0        0     2076 2023-04-23 17:24:05.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/Tickers.py
--rw-rw-rw-   0        0        0     6864 2023-04-22 07:56:08.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/Utils.py
--rw-rw-rw-   0        0        0      243 2023-04-22 07:44:44.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/__init__.py
--rw-rw-rw-   0        0        0     1397 2023-04-21 18:15:14.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:32:19.437162 py-portfolio-tools-0.0.7/py_portfolio_tools.egg-info/
--rw-rw-rw-   0        0        0     1198 2023-05-05 17:32:19.000000 py-portfolio-tools-0.0.7/py_portfolio_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2023-05-05 17:32:19.000000 py-portfolio-tools-0.0.7/py_portfolio_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 17:32:19.000000 py-portfolio-tools-0.0.7/py_portfolio_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-05-05 17:32:19.000000 py-portfolio-tools-0.0.7/py_portfolio_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-05 17:32:19.000000 py-portfolio-tools-0.0.7/py_portfolio_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 17:32:19.437162 py-portfolio-tools-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1633 2023-05-05 17:32:11.000000 py-portfolio-tools-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:12:53.900237 py-portfolio-tools-0.0.8/
+-rw-rw-rw-   0        0        0     1075 2023-04-17 11:45:54.000000 py-portfolio-tools-0.0.8/LICENSE.md
+-rw-rw-rw-   0        0        0     1198 2023-05-07 12:12:53.899399 py-portfolio-tools-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2023-04-17 11:54:14.000000 py-portfolio-tools-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 12:12:53.875702 py-portfolio-tools-0.0.8/py-portfolio-tools/
+-rw-rw-rw-   0        0        0     2545 2023-04-17 18:42:57.000000 py-portfolio-tools-0.0.8/py-portfolio-tools/DataFetch.py
+-rw-rw-rw-   0        0        0      703 2023-04-17 13:42:55.000000 py-portfolio-tools-0.0.8/py-portfolio-tools/Logger.py
+-rw-rw-rw-   0        0        0     4040 2023-05-07 12:04:47.000000 py-portfolio-tools-0.0.8/py-portfolio-tools/Optimizers.py
+-rw-rw-rw-   0        0        0    10710 2023-05-07 11:54:12.000000 py-portfolio-tools-0.0.8/py-portfolio-tools/Portfolio.py
+-rw-rw-rw-   0        0        0     3232 2023-04-23 17:24:00.000000 py-portfolio-tools-0.0.8/py-portfolio-tools/PortfolioInputWindow.py
+-rw-rw-rw-   0        0        0    10166 2023-05-07 12:06:51.000000 py-portfolio-tools-0.0.8/py-portfolio-tools/PortfolioManager.py
+-rw-rw-rw-   0        0        0       30 2023-04-17 14:28:58.000000 py-portfolio-tools-0.0.8/py-portfolio-tools/Predictor.py
+-rw-rw-rw-   0        0        0     3151 2023-05-05 11:22:09.000000 py-portfolio-tools-0.0.8/py-portfolio-tools/StocksAllocator.py
+-rw-rw-rw-   0        0        0     2076 2023-04-23 17:24:05.000000 py-portfolio-tools-0.0.8/py-portfolio-tools/Tickers.py
+-rw-rw-rw-   0        0        0     6864 2023-04-22 07:56:08.000000 py-portfolio-tools-0.0.8/py-portfolio-tools/Utils.py
+-rw-rw-rw-   0        0        0      436 2023-05-07 12:12:05.000000 py-portfolio-tools-0.0.8/py-portfolio-tools/__init__.py
+-rw-rw-rw-   0        0        0     1399 2023-05-07 12:12:30.000000 py-portfolio-tools-0.0.8/py-portfolio-tools/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:12:53.898402 py-portfolio-tools-0.0.8/py_portfolio_tools.egg-info/
+-rw-rw-rw-   0        0        0     1198 2023-05-07 12:12:53.000000 py-portfolio-tools-0.0.8/py_portfolio_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-05-07 12:12:53.000000 py-portfolio-tools-0.0.8/py_portfolio_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 12:12:53.000000 py-portfolio-tools-0.0.8/py_portfolio_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-05-07 12:12:53.000000 py-portfolio-tools-0.0.8/py_portfolio_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-07 12:12:53.000000 py-portfolio-tools-0.0.8/py_portfolio_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 12:12:53.900237 py-portfolio-tools-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1642 2023-05-07 12:12:25.000000 py-portfolio-tools-0.0.8/setup.py
```

### Comparing `py-portfolio-tools-0.0.7/LICENSE.md` & `py-portfolio-tools-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.7/PKG-INFO` & `py-portfolio-tools-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-portfolio-tools
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python Library and set of GUI tools for Portfolio Management
 Home-page: https://gitlab.com/Jaysmito101/py-portfolio-tools
 Author: Jaysmito Mukherjee
 Author-email: jaysmito101@gmail.com
 License: MIT
 Project-URL: Documentation, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/wikis/Home
 Project-URL: Issue tracker, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/issues
```

### Comparing `py-portfolio-tools-0.0.7/py-portfolio-tools/DataFetch.py` & `py-portfolio-tools-0.0.8/py-portfolio-tools/DataFetch.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.7/py-portfolio-tools/Logger.py` & `py-portfolio-tools-0.0.8/py-portfolio-tools/Logger.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.7/py-portfolio-tools/Portfolio.py` & `py-portfolio-tools-0.0.8/py-portfolio-tools/Portfolio.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,16 +23,25 @@
         self._weights = weights
         self._predictor = predictor
         self._dataFetch = dataFetch
         self._logger = logger
         self._analysis = None
         self._hasAnalysis = False
         self._stockHistory = None
+        self._hasStockHistory = False
         self._isCompoundingReturns = False
         self._logReturns = False
+        self._riskFreeRate = 0.02
+        self._forceReCalculate = False
+    
+    def SetWeights(self, weights):
+        """Set the weights of the portfolio"""
+        if len(weights) != len(self._stocks):
+            raise RuntimeError("Weights size does not match stocks size")
+        self._weights = weights
     
     def FetchStockHistory(self, startDate, endDate, silent = False):
         # is endDate is None, then set it to today
         if endDate == None:
             endDate = str(datetime.now().strftime("%Y-%m-%d"))
         # check if end date after today
         requirePrediction = False
@@ -49,66 +58,111 @@
             self._stockHistory[stock] = self._dataFetch.GetStockHistory(stock, start = startDate, end = finalEndDate)["Close"]
         
         if requirePrediction:
             self._logger.Log(f'Predicting stock history from {finalEndDate} to {endDate}')
             if self._predictor == None:
                 raise RuntimeError("Predictor is not set")
             self._stockHistory = self._predictor.Predict(self._stockHistory, finalEndDate, endDate)
-        
 
-    
-    def NumericalAnalysis(self, startDate, endDate, silent = False):
-        """Do a numerical analysis of the portfolio"""
+        self._hasStockHistory = True
 
-        if not silent:
-            self._logger.Log(f"Starging numerical analysis of portfolio {self._name}")
-            self._logger.Log(f"Stocks: {self._stocks}")
-            self._logger.Log(f"Weights: {self._weights}")
-        
-        if self._analysis == None:
-            self.FetchStockHistory(startDate, endDate, silent)
-            self._analysis = Object()
-            self._analysis.startDate = startDate
-            self._analysis.endDate = endDate
-            self._analysis.stockHistory = self._stockHistory.copy()
-        
+    def CalculateDailyReturns(self):
         # calculate the daily returns
+        if self._analysis == None:
+            raise RuntimeError("Analysis has not been done yet")
         if self._logReturns:
             self._analysis.dailyReturns = np.log(1 + self._stockHistory.pct_change()).dropna(how="all")
         else:
             self._analysis.dailyReturns = self._stockHistory.pct_change().dropna(how="all")
+        return self._analysis.dailyReturns
         
+    def CalculateDailyMeanReturns(self):
+        # calculate the daily mean returns
+        if self._analysis == None:
+            raise RuntimeError("Analysis has not been done yet")
+        if self._forceReCalculate:
+            self.CalculateDailyReturns()
         if self._isCompoundingReturns:
             self._analysis.meanDailyReturns = (self._analysis.dailyReturns + 1).prod() ** (252 / self._analysis.dailyReturns.count) - 1
         else:
             self._analysis.meanDailyReturns = self._analysis.dailyReturns.mean() * 252
+        return self._analysis.meanDailyReturns
+       
+    def CalculatePortfolioCovarianceMatrix(self):
+        if self._analysis == None:
+            raise RuntimeError("Analysis has not been done yet")
+        if self._forceReCalculate:
+            self.CalculateDailyReturns()
         # calculate the covariance matrix
         self._analysis.covarianceMatrix = self._analysis.dailyReturns.cov() * 252
-
+        return self._analysis.covarianceMatrix 
+    
+    def CalculateRisk(self):
+        # calculate the portfolio standard deviation
+        if self._analysis == None:
+            raise RuntimeError("Analysis has not been done yet")
+        if self._forceReCalculate:
+            self.CalculatePortfolioCovarianceMatrix()        
         # calculate the portfolio variance
         self._analysis.portfolioVariance = np.dot(self._weights, np.dot(self._analysis.covarianceMatrix, self._weights))
-
         # calculate the portfolio standard deviation
         self._analysis.portfolioStandardDeviation = np.sqrt(self._analysis.portfolioVariance)
         self._analysis.portfolioRisk = self._analysis.portfolioStandardDeviation
+        return self._analysis.portfolioRisk
 
+    def CalculateExpectedReturn(self):
         # calculate the portfolio expected return
+        if self._analysis == None:
+            raise RuntimeError("Analysis has not been done yet")
         self._analysis.portfolioExpectedReturn = np.dot(self._weights, self._analysis.meanDailyReturns)
-
+        return self._analysis.portfolioExpectedReturn
+    
+    def CalculateSharpeRatio(self, riskFreeRate = 0.02):
         # calculate the portfolio sharpe ratio
-        self._analysis.portfolioSharpeRatio = (self._analysis.portfolioExpectedReturn - 0.02) / self._analysis.portfolioStandardDeviation
+        if self._analysis == None:
+            raise RuntimeError("Analysis has not been done yet")
+        if self._forceReCalculate:
+            self.CalculateExpectedReturn()
+            self.CalculateRisk()
+        self._analysis.portfolioSharpeRatio = (self._analysis.portfolioExpectedReturn - riskFreeRate) / self._analysis.portfolioStandardDeviation
+        return self._analysis.portfolioSharpeRatio
+    
+    def NumericalAnalysis(self, startDate, endDate, silent = False):
+        """Do a numerical analysis of the portfolio"""
 
+        if not silent:
+            self._logger.Log(f"Starting numerical analysis of portfolio {self._name}")
+            self._logger.Log(f"Stocks: {self._stocks}")
+            self._logger.Log(f"Weights: {self._weights}")
+        
+        if not self._hasStockHistory:
+            self.FetchStockHistory(startDate, endDate, silent)
+
+        if self._analysis == None:
+            self._analysis = Object()
+            self._analysis.startDate = startDate
+            self._analysis.endDate = endDate
+            self._analysis.stockHistory = self._stockHistory.copy()
+
+        self.CalculateDailyReturns() 
+        self.CalculateDailyMeanReturns()
+        self.CalculatePortfolioCovarianceMatrix()
+        self.CalculateRisk()
+        self.CalculateExpectedReturn()
+        self.CalculateSharpeRatio(self._riskFreeRate)
    
 
     def Analyse(self, startDate, endDate):
         """Analyse the portfolio from the start date to the end date"""
         self._logger.Log(f'Calculating portfolio history from {startDate} to {endDate}')
         
-        if self._analysis == None:
+        if not self._hasStockHistory:
             self.FetchStockHistory(startDate, endDate, False)
+        
+        if self._analysis == None:
             self._analysis = Object()
             self._analysis.startDate = startDate
             self._analysis.endDate = endDate
             self._analysis.stockHistory = self._stockHistory.copy()
 
         self._analysis.stockHistoryPlots = []
```

### Comparing `py-portfolio-tools-0.0.7/py-portfolio-tools/PortfolioInputWindow.py` & `py-portfolio-tools-0.0.8/py-portfolio-tools/PortfolioInputWindow.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.7/py-portfolio-tools/PortfolioManager.py` & `py-portfolio-tools-0.0.8/py-portfolio-tools/PortfolioManager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .Utils import *
 from .Logger import *
 from .DataFetch import *
 from .Portfolio import *
 from .StocksAllocator import *
+from .Optimizers import *
 import pandas as pd
 import numpy as np
 import json
 import os
 import imgui
 
 class PortfolioManager:
@@ -20,14 +21,15 @@
         self._stockHistoryComparisonTexture = None
         self._stocksBasedDistributionPlotTexture = None
         self._countryBasedDistributionPlotTexture = None
         self._sectorBasedDistributionPlotTexture = None
         self._allocator = StocksAllocator()
         self._allocatedWithStocks = None
         self._allocatorTotalBudget = 100000
+        self._optimizedPortfolios = []
     
     def Show(self):
         """Show the portfolio in a imgui window"""
         if not self._showWindow:
             return
         
         windowExpanded, self._showWindow = imgui.begin(f"Portfolio {self._portfolio._name}", True)
@@ -80,15 +82,39 @@
                 self._allocatedWithStocks = self._allocator.Allocate(self._portfolio._weights, prices, self._allocatorTotalBudget, "greedy")
             imgui.same_line()
             if imgui.button("Allocate Random"):
                 prices = [self._portfolio._analysis.stockHistory[stock].iloc[-1] for stock in self._portfolio._stocks]
                 self._allocatedWithStocks = self._allocator.Allocate(self._portfolio._weights, prices, self._allocatorTotalBudget, "random")
         elif expanded:
             imgui.text("No analysis has been done yet")
-
+        
+        expanded, visible = imgui.collapsing_header("Portfolio Optimization")
+        if expanded:
+            if imgui.button("Optimize (Monte Carlo)"):
+                optimizer = MonteCarloOptimizer(self._portfolio, self._portfolio._logger)
+                self._optimizedPortfolios = optimizer.Optimize(self._startDate, self._endDate, 10000)
+            imgui.same_line()
+            if imgui.button("Optimize (Mean Variance)"):
+                optimizer = MeanVarianceOptimizer(self._portfolio, self._portfolio._logger)
+                self._optimizedPortfolios = optimizer.Optimize(self._startDate, self._endDate)
+            if len(self._optimizedPortfolios) > 0:
+                imgui.text("Optimized Portfolios:")
+                with imgui.begin_child("##OptimizedPortfolios", 0, 300):
+                    for i in range(len(self._optimizedPortfolios)):
+                        imgui.text(f"Expected Return: {(self._optimizedPortfolios[i][1] * 100):.2f}%")
+                        imgui.text(f"Risk: {(self._optimizedPortfolios[i][0] * 100):.2f}%")
+                        imgui.text(f"Sharpe Ratio: {self._optimizedPortfolios[i][2]:.2f}")
+                        imgui.text(f"Weights: " + str(self._optimizedPortfolios[i][3]))
+                        if imgui.button("Load & Analyse##OptimizedPortfolio_" + str(i)):
+                            self._portfolio._weights = self._optimizedPortfolios[i][3]
+                            self._portfolio.Analyse(self._startDate, self._endDate)
+                            self.LoadAnalysis()
+                        imgui.separator()
+            else:
+                imgui.text("No optimization has been done yet")
         
     def ShowAnalysisTab(self):
         expanded, visible = imgui.collapsing_header("Stocks History")
         if expanded:
             imgui.push_id("StocksHistoryTab")
             for i in range(len(self._portfolio._stocks)):
                 imgui.text(f"{self._portfolio._stocks[i]}")
```

### Comparing `py-portfolio-tools-0.0.7/py-portfolio-tools/StocksAllocator.py` & `py-portfolio-tools-0.0.8/py-portfolio-tools/StocksAllocator.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.7/py-portfolio-tools/Tickers.py` & `py-portfolio-tools-0.0.8/py-portfolio-tools/Tickers.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.7/py-portfolio-tools/Utils.py` & `py-portfolio-tools-0.0.8/py-portfolio-tools/Utils.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.7/py-portfolio-tools/__main__.py` & `py-portfolio-tools-0.0.8/py-portfolio-tools/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     # print(df.GetStockHistory("GOOG", "1d", "2005-01-01", "2022-12-31"))
     # pf = Portfolio("Test", ["GOOG", "MSFT", "AAPL", "NVDA"])
     # pf.Analyse("2020-01-01", "2022-12-31")
 
     portfolioInputWindow = PortfolioInputWindow()
 
     InitializeGLFW()
-    window = CreateWindow(500, 500, "Portfolio Tools 2.0 - Jaysmito Mukherjee")
+    window = CreateWindow(500, 500, "Portfolio Tools 0.0.8 - Jaysmito Mukherjee")
     gl.glClearColor(0.2, 0.2, 0.2, 1.0)
     imgui.create_context()
     SetupImGuiTheme()
     impl = GlfwRenderer(window)
     while not glfw.window_should_close(window):
         window_size = glfw.get_window_size(window)
         gl.glViewport(0, 0, window_size[0], window_size[1])
```

### Comparing `py-portfolio-tools-0.0.7/py_portfolio_tools.egg-info/PKG-INFO` & `py-portfolio-tools-0.0.8/py_portfolio_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-portfolio-tools
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python Library and set of GUI tools for Portfolio Management
 Home-page: https://gitlab.com/Jaysmito101/py-portfolio-tools
 Author: Jaysmito Mukherjee
 Author-email: jaysmito101@gmail.com
 License: MIT
 Project-URL: Documentation, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/wikis/Home
 Project-URL: Issue tracker, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/issues
```

### Comparing `py-portfolio-tools-0.0.7/py_portfolio_tools.egg-info/SOURCES.txt` & `py-portfolio-tools-0.0.8/py_portfolio_tools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE.md
 README.md
 setup.py
 py-portfolio-tools/DataFetch.py
 py-portfolio-tools/Logger.py
+py-portfolio-tools/Optimizers.py
 py-portfolio-tools/Portfolio.py
 py-portfolio-tools/PortfolioInputWindow.py
 py-portfolio-tools/PortfolioManager.py
 py-portfolio-tools/Predictor.py
 py-portfolio-tools/StocksAllocator.py
 py-portfolio-tools/Tickers.py
 py-portfolio-tools/Utils.py
```

### Comparing `py-portfolio-tools-0.0.7/setup.py` & `py-portfolio-tools-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import re
 
-requirements = ['numpy', 'pandas', 'matplotlib', 'yfinance', "PyOpenGL", "glfw", "imgui[glfw]", "Pillow"] 
+requirements = ['numpy', 'pandas', 'matplotlib', 'yfinance', "PyOpenGL", "glfw", "imgui[glfw]", "Pillow", "scipy"] 
 
-version = '0.0.7'
+version = '0.0.8'
 
 if not version:
     raise RuntimeError('version is not set')
 
 readme = 'Coming Soon ...'
 
 setup(
```

