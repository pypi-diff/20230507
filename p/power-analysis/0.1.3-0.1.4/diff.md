# Comparing `tmp/power_analysis-0.1.3.tar.gz` & `tmp/power_analysis-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power_analysis-0.1.3.tar", max compression
+gzip compressed data, was "power_analysis-0.1.4.tar", max compression
```

## Comparing `power_analysis-0.1.3.tar` & `power_analysis-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1092 2023-05-04 03:56:39.000000 power_analysis-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2023-05-04 03:28:48.000000 power_analysis-0.1.3/power_analysis/__init__.py
--rw-r--r--   0        0        0     1034 2023-05-06 22:45:43.082904 power_analysis-0.1.3/power_analysis/Examples.py
--rw-r--r--   0        0        0     6715 2023-05-07 21:02:22.160905 power_analysis-0.1.3/power_analysis/PanelBoostrapObs.py
--rw-r--r--   0        0        0     3272 2023-05-04 03:35:57.000000 power_analysis-0.1.3/power_analysis/SimpleBootstrap.py
--rw-r--r--   0        0        0      452 2023-05-07 21:10:22.452065 power_analysis-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2153 2023-05-06 22:47:13.219818 power_analysis-0.1.3/README.md
--rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 power_analysis-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-04 03:56:39.000000 power_analysis-0.1.4/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-04 03:28:48.000000 power_analysis-0.1.4/power_analysis/__init__.py
+-rw-r--r--   0        0        0     1034 2023-05-06 22:45:43.082904 power_analysis-0.1.4/power_analysis/Examples.py
+-rw-r--r--   0        0        0     6715 2023-05-07 21:13:52.611023 power_analysis-0.1.4/power_analysis/PanelBoostrapObs.py
+-rw-r--r--   0        0        0     3272 2023-05-04 03:35:57.000000 power_analysis-0.1.4/power_analysis/SimpleBootstrap.py
+-rw-r--r--   0        0        0      452 2023-05-07 21:22:36.596368 power_analysis-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2268 2023-05-07 21:21:10.300716 power_analysis-0.1.4/README.md
+-rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 power_analysis-0.1.4/PKG-INFO
```

### Comparing `power_analysis-0.1.3/LICENSE` & `power_analysis-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `power_analysis-0.1.3/power_analysis/Examples.py` & `power_analysis-0.1.4/power_analysis/Examples.py`

 * *Files identical despite different names*

### Comparing `power_analysis-0.1.3/power_analysis/PanelBoostrapObs.py` & `power_analysis-0.1.4/power_analysis/PanelBoostrapObs.py`

 * *Files identical despite different names*

### Comparing `power_analysis-0.1.3/power_analysis/SimpleBootstrap.py` & `power_analysis-0.1.4/power_analysis/SimpleBootstrap.py`

 * *Files identical despite different names*

