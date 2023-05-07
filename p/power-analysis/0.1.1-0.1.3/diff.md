# Comparing `tmp/power_analysis-0.1.1.tar.gz` & `tmp/power_analysis-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power_analysis-0.1.1.tar", max compression
+gzip compressed data, was "power_analysis-0.1.3.tar", max compression
```

## Comparing `power_analysis-0.1.1.tar` & `power_analysis-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1092 2023-05-04 03:56:39.960574 power_analysis-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2023-05-04 03:28:48.248048 power_analysis-0.1.1/power_analysis/__init__.py
--rw-r--r--   0        0        0     3272 2023-05-04 03:35:57.988674 power_analysis-0.1.1/power_analysis/modules.py
--rw-r--r--   0        0        0      411 2023-05-04 04:41:32.486209 power_analysis-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2153 2023-05-04 04:29:40.389936 power_analysis-0.1.1/README.md
--rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 power_analysis-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-04 03:56:39.000000 power_analysis-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-04 03:28:48.000000 power_analysis-0.1.3/power_analysis/__init__.py
+-rw-r--r--   0        0        0     1034 2023-05-06 22:45:43.082904 power_analysis-0.1.3/power_analysis/Examples.py
+-rw-r--r--   0        0        0     6715 2023-05-07 21:02:22.160905 power_analysis-0.1.3/power_analysis/PanelBoostrapObs.py
+-rw-r--r--   0        0        0     3272 2023-05-04 03:35:57.000000 power_analysis-0.1.3/power_analysis/SimpleBootstrap.py
+-rw-r--r--   0        0        0      452 2023-05-07 21:10:22.452065 power_analysis-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2153 2023-05-06 22:47:13.219818 power_analysis-0.1.3/README.md
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 power_analysis-0.1.3/PKG-INFO
```

### Comparing `power_analysis-0.1.1/LICENSE` & `power_analysis-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `power_analysis-0.1.1/power_analysis/modules.py` & `power_analysis-0.1.3/power_analysis/SimpleBootstrap.py`

 * *Files identical despite different names*

### Comparing `power_analysis-0.1.1/README.md` & `power_analysis-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `power_analysis-0.1.1/PKG-INFO` & `power_analysis-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: power-analysis
-Version: 0.1.1
+Version: 0.1.3
 Summary: This package allows you to perform power analysis computations
 License: MIT
 Author: Rodrigo Franco
 Author-email: franc703@umn.edu
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (>=1.24.3,<2.0.0)
-Requires-Dist: scipy (>=1.10.1,<2.0.0)
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: numpy (>=1.16.5,<1.23.0)
+Requires-Dist: optional-py (>=1.3.2,<2.0.0)
+Requires-Dist: scipy (>=1.7.0,<=1.7.1)
 Description-Content-Type: text/markdown
 
 # power-analysis 💪🔍
 
 `power-analysis` is a Python package for performing power analysis and calculating sample sizes for statistical models. The package provides classes for defining statistical models, performing power analysis, and calculating sample sizes for two-sample t-tests.
 
 ## Installation 📥
```

