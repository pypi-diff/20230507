# Comparing `tmp/power_analysis-0.1.4.tar.gz` & `tmp/power_analysis-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power_analysis-0.1.4.tar", max compression
+gzip compressed data, was "power_analysis-0.1.5.tar", max compression
```

## Comparing `power_analysis-0.1.4.tar` & `power_analysis-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1092 2023-05-04 03:56:39.000000 power_analysis-0.1.4/LICENSE
--rw-r--r--   0        0        0        0 2023-05-04 03:28:48.000000 power_analysis-0.1.4/power_analysis/__init__.py
--rw-r--r--   0        0        0     1034 2023-05-06 22:45:43.082904 power_analysis-0.1.4/power_analysis/Examples.py
--rw-r--r--   0        0        0     6715 2023-05-07 21:13:52.611023 power_analysis-0.1.4/power_analysis/PanelBoostrapObs.py
--rw-r--r--   0        0        0     3272 2023-05-04 03:35:57.000000 power_analysis-0.1.4/power_analysis/SimpleBootstrap.py
--rw-r--r--   0        0        0      452 2023-05-07 21:22:36.596368 power_analysis-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2268 2023-05-07 21:21:10.300716 power_analysis-0.1.4/README.md
--rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 power_analysis-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-04 03:56:39.000000 power_analysis-0.1.5/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-04 03:28:48.000000 power_analysis-0.1.5/power_analysis/__init__.py
+-rw-r--r--   0        0        0     1034 2023-05-06 22:45:43.082904 power_analysis-0.1.5/power_analysis/Examples.py
+-rw-r--r--   0        0        0     6740 2023-05-07 21:34:39.955708 power_analysis-0.1.5/power_analysis/PanelBoostrapObs.py
+-rw-r--r--   0        0        0     3272 2023-05-04 03:35:57.000000 power_analysis-0.1.5/power_analysis/SimpleBootstrap.py
+-rw-r--r--   0        0        0      452 2023-05-07 21:34:55.167161 power_analysis-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2254 2023-05-07 21:23:47.225015 power_analysis-0.1.5/README.md
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 power_analysis-0.1.5/PKG-INFO
```

### Comparing `power_analysis-0.1.4/LICENSE` & `power_analysis-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `power_analysis-0.1.4/power_analysis/Examples.py` & `power_analysis-0.1.5/power_analysis/Examples.py`

 * *Files identical despite different names*

### Comparing `power_analysis-0.1.4/power_analysis/PanelBoostrapObs.py` & `power_analysis-0.1.5/power_analysis/PanelBoostrapObs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from __future__ import annotations
 import numpy as np
 import pandas as pd
 import statsmodels.api as sm
 from statsmodels.stats.power import TTestIndPower
-from optional import Optional
+from typing import Optional
 
 
 class PowerAnalysis:
     """
     This class conducts power analysis on observational panel data using a clustered bootstrap method.
 
     It calculates statistical power by varying the number of observations (N) and effect sizes.
@@ -46,16 +47,16 @@
         self.data = data
         self.outcome_var = outcome_var
         self.treatment_var = treatment_var
         self.individual_var = individual_var
         if random_seed is not None:
             np.random.seed(random_seed)
 
-    def fit_model(self, data: pd.DataFrame, control_vars: Optional[list[str]] = None,
-                  fixed_effects: Optional[list[str]] = None, cluster_var: Optional[str] = None) -> tuple[float, float]:
+    def fit_model(self, data: pd.DataFrame, control_vars: list[str] | None = None,
+                  fixed_effects: list[str] | None = None, cluster_var: str | None = None) -> tuple[float, float]:
         """
          Fits a linear regression model to the provided data and returns the treatment effect and p-value.
 
          Parameters:
          -----------
          data: pd.DataFrame
              A DataFrame containing the observational panel data.
```

### Comparing `power_analysis-0.1.4/power_analysis/SimpleBootstrap.py` & `power_analysis-0.1.5/power_analysis/SimpleBootstrap.py`

 * *Files identical despite different names*

### Comparing `power_analysis-0.1.4/README.md` & `power_analysis-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,11 +62,7 @@
 ## Contributing 🤝
 
 Contributions to `power-analysis` are welcome! If you find a bug or would like to suggest a new feature, please open an issue on GitHub.
 
 ## License 📜
 
 `power-analysis` is licensed under the MIT license. See `LICENSE` for more information.
-
-```
-
-```
```

### Comparing `power_analysis-0.1.4/PKG-INFO` & `power_analysis-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-analysis
-Version: 0.1.4
+Version: 0.1.5
 Summary: This package allows you to perform power analysis computations
 License: MIT
 Author: Rodrigo Franco
 Author-email: franc703@umn.edu
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -81,11 +81,7 @@
 
 Contributions to `power-analysis` are welcome! If you find a bug or would like to suggest a new feature, please open an issue on GitHub.
 
 ## License 📜
 
 `power-analysis` is licensed under the MIT license. See `LICENSE` for more information.
 
-```
-
-```
-
```

