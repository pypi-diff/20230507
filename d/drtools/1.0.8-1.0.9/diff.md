# Comparing `tmp/drtools-1.0.8.tar.gz` & `tmp/drtools-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drtools-1.0.8.tar", last modified: Fri Feb 10 16:48:32 2023, max compression
+gzip compressed data, was "drtools-1.0.9.tar", last modified: Sat Feb 11 04:32:48 2023, max compression
```

## Comparing `drtools-1.0.8.tar` & `drtools-1.0.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:32.434703 drtools-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-10 16:48:22.000000 drtools-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:22.000000 drtools-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-10 16:48:32.434703 drtools-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-10 16:48:22.000000 drtools-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-10 16:48:22.000000 drtools-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-02-10 16:48:32.434703 drtools-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:32.422703 drtools-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:32.426703 drtools-1.0.8/src/drtools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:32.430703 drtools-1.0.8/src/drtools/data_science/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/beyond_linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/data_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/data_load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:32.430703 drtools-1.0.8/src/drtools/data_science/model_selection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/model_selection/dimension_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/model_selection/shrinkage.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/model_selection/subset_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/multiple_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    28368 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:32.430703 drtools-1.0.8/src/drtools/data_science/resampling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/resampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/resampling/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/resampling/cross_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:32.430703 drtools-1.0.8/src/drtools/data_science/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54978 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/resources/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/statistical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/survival_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/test_error_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/tree_based.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/data_science/unsupervised_learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:32.430703 drtools-1.0.8/src/drtools/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:32.430703 drtools-1.0.8/src/drtools/database/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/database/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/database/connection/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/database/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/file_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:32.434703 drtools-1.0.8/src/drtools/geo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/geo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:32.434703 drtools-1.0.8/src/drtools/scrapping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/scrapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/scrapping/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/scrapping/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/scrapping/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/thread_pool_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20856 2023-02-10 16:48:22.000000 drtools-1.0.8/src/drtools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:32.426703 drtools-1.0.8/src/drtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-10 16:48:32.000000 drtools-1.0.8/src/drtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-02-10 16:48:32.000000 drtools-1.0.8/src/drtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 16:48:32.000000 drtools-1.0.8/src/drtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-10 16:48:32.000000 drtools-1.0.8/src/drtools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 16:48:32.434703 drtools-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-02-10 16:48:22.000000 drtools-1.0.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.866935 drtools-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-11 04:32:34.000000 drtools-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-11 04:32:48.870935 drtools-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-11 04:32:34.000000 drtools-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-11 04:32:34.000000 drtools-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-02-11 04:32:48.870935 drtools-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.850936 drtools-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.858935 drtools-1.0.9/src/drtools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.862935 drtools-1.0.9/src/drtools/data_science/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/beyond_linearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/data_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/data_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.862935 drtools-1.0.9/src/drtools/data_science/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/model_selection/dimension_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/model_selection/shrinkage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/model_selection/subset_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/multiple_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28368 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.862935 drtools-1.0.9/src/drtools/data_science/resampling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/resampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/resampling/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/resampling/cross_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.866935 drtools-1.0.9/src/drtools/data_science/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54879 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/resources/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/statistical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/survival_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/test_error_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/tree_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/data_science/unsupervised_learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.866935 drtools-1.0.9/src/drtools/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.866935 drtools-1.0.9/src/drtools/database/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/database/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/database/connection/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/database/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/file_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.866935 drtools-1.0.9/src/drtools/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/geo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.866935 drtools-1.0.9/src/drtools/scrapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/scrapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/scrapping/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/scrapping/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/scrapping/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/thread_pool_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20856 2023-02-11 04:32:34.000000 drtools-1.0.9/src/drtools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.858935 drtools-1.0.9/src/drtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-11 04:32:48.000000 drtools-1.0.9/src/drtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-02-11 04:32:48.000000 drtools-1.0.9/src/drtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 04:32:48.000000 drtools-1.0.9/src/drtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-11 04:32:48.000000 drtools-1.0.9/src/drtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 04:32:48.866935 drtools-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-02-11 04:32:34.000000 drtools-1.0.9/tests/test_utils.py
```

### Comparing `drtools-1.0.8/LICENSE` & `drtools-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/setup.cfg` & `drtools-1.0.9/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = drtools
-version = 1.0.8
+version = 1.0.9
 author = Andrey Malheiros
 author_email = example@email.com
 description = Kit of MY useful tools.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/andreylcj/drtools
 project_urls =
```

### Comparing `drtools-1.0.8/src/drtools/data_science/beyond_linearity.py` & `drtools-1.0.9/src/drtools/data_science/beyond_linearity.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/data_science/classification.py` & `drtools-1.0.9/src/drtools/data_science/classification.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/data_science/data_handle.py` & `drtools-1.0.9/src/drtools/data_science/data_handle.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/data_science/data_load.py` & `drtools-1.0.9/src/drtools/data_science/data_load.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/data_science/model_selection/subset_selection.py` & `drtools-1.0.9/src/drtools/data_science/model_selection/subset_selection.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/data_science/multiple_testing.py` & `drtools-1.0.9/src/drtools/data_science/multiple_testing.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/data_science/plot.py` & `drtools-1.0.9/src/drtools/data_science/plot.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/data_science/resources/main.py` & `drtools-1.0.9/src/drtools/data_science/resources/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -495,20 +495,21 @@
 
         Returns
         -------
         str
             Model name combining id, algorithm nickname, model name 
             and model version.
         """
-        return f'{self.id}-{self.algorithm}_{self.name}_{self.version}'
+        # return f'{self.id}-{self.algorithm}_{self.name}_{self.version}'
+        return f'{self.id}-{self.algorithm}'
     
     # @start_end_log('cols_correct_order')        
     def cols_correct_order(
         self
-    ) -> List[str]:        
+    ) -> List[str]:
         """Returns list of all cols of model, including 
         extra columns, in correct order.
 
         Returns
         -------
         List[str]
             Model cols in correct order.
@@ -520,24 +521,24 @@
             + input_features_name \
             + output_features_name
         return pretty_cols
     
     @start_end_log('load_model')
     def load_model(
         self,
-        project_root_path: str,
+        model_file_path: str,
         *args,
         **kwargs
     ) -> Any:
         """Load model from path and return model instance
 
         Parameters
         ----------
-        project_root_path : str
-            The root path of project.
+        model_file_path : str
+            Path of model file.
         args : Tuple, optional
             All args inputs will be passed to load model 
             function, by default ().
         kwargs : Dict, optional
             All args inputs will be passed to load model 
             function, by default {}.
 
@@ -552,26 +553,18 @@
             If model algorithm is invalid
         """
         
         self.LOGGER.info(f'Loading model {self.get_model_name()}...')        
         model = None        
         if self.algorithm == 'lgbm':
             import lightgbm as lgb
-            model = lgb.Booster(
-                model_file=f'{project_root_path}/models/{self.get_model_name()}/model/{self.get_model_name()}.txt',
-                *args,
-                **kwargs
-            )
+            model = lgb.Booster(model_file=model_file_path, *args, **kwargs)
         elif self.algorithm == 'NN':
             from tensorflow import keras
-            model = keras.models.load_model(
-                f'{project_root_path}/models/{self.get_model_name()}/model/{self.get_model_name()}',
-                *args,
-                **kwargs
-            )
+            model = keras.models.load_model(model_file_path, *args, **kwargs)
         else:
             raise Exception(f'Algorithm {self.algorithm} is invalid.')        
         self.LOGGER.info(f'Loading model {self.get_model_name()}... Done!')        
         return model
     
     @start_end_log('save_model')
     def save_model(
@@ -660,26 +653,25 @@
             return model_instance, history
         else:
             raise Exception(f'Algorithm {self.algorithm} is invalid.')
     
     @start_end_log('predict')
     def predict(
         self,
-        # model_instance: Any,
-        project_root_path: str,
+        model_file_path: str,
         X: Any,
         *args,
         **kwargs
     ) -> Any:    
         """Predict data.
 
         Parameters
         ----------
-        model_instance : Any
-            Instance of desired model to train.
+        model_file_path : str
+            Path of model file.
         X : Any
             X data to predict.
         args : Tuple, optional
             All args inputs will be passed to predict 
             function, by default ().
         kwargs : Dict, optional
             All kwargs inputs will be passed to predict 
@@ -692,15 +684,15 @@
 
         Raises
         ------
         Exception
             If model algorithm is invalid
         """    
         self.LOGGER.info(f'Predicting data for model {self.get_model_name()}...')  
-        model_instance = self.load_model(project_root_path)              
+        model_instance = self.load_model(model_file_path)
         if self.algorithm == 'lgbm':
             y_pred = model_instance.predict(X, *args, **kwargs)
         elif self.algorithm == 'NN':
             y_pred = model_instance.predict(X, *args, **kwargs)
             y_pred = y_pred.reshape(1, -1)[0]
         else:
             raise Exception(f'Algorithm {self.algorithm} is invalid.')        
@@ -846,15 +838,18 @@
         ------
         Exception
             If "description" fielf of Feature is invalid.
         """
         
         df = dataframe.copy()
         
-        self.LOGGER.set_verbosity(verbosity)
+        try:
+            self.LOGGER.set_verbosity(verbosity)
+        except:
+            pass
         
         all_features = self.input_features + self.output_features
         
         filter_features = all_features
         if custom is not None:
             filter_features = custom
             
@@ -978,15 +973,18 @@
             to_shape = df.shape
                 
             self.LOGGER.debug(f'Col <{feature["name"]}> filter from shape ({from_shape[0]:,}, {from_shape[1]:,}) to shape ({to_shape[0]:,}, {to_shape[1]:,})')                    
             self.LOGGER.debug(f'({count:,}/{categorical_features_len:,}) Filtering {feature["name"]}... Done!')
             
         self.LOGGER.debug('Transforming and filtering Categorical variables... Done!')
             
-        self.LOGGER.reset_verbosity()
+        try:
+            self.LOGGER.reset_verbosity()
+        except:
+            pass
             
         return df
     
     @start_end_log('typeraze')
     def typeraze(
         self,
         dataframe: DataFrame,
@@ -1220,27 +1218,33 @@
             {'name': col.name, 'type': col.type} 
             for col in self.table.columns 
             if col.name in useful_cols
         ]
         
         custom_treatment = self.CONFIG.get('typeraze_customTreatment', [])
         
-        self.LOGGER.set_verbosity(verbosity)
+        try:
+            self.LOGGER.set_verbosity(verbosity)
+        except:
+            pass
         
         df = typeraze(
             dataframe=df,
             features=features,
             dtypes=dtypes,
             ignore_dtypes=ignore_dtypes,
             custom_treatment=custom_treatment,
             LOGGER=self.LOGGER,
             **kwargs
         )
         
-        self.LOGGER.reset_verbosity()
+        try:
+            self.LOGGER.reset_verbosity()
+        except:
+            pass
         
         return df
         
     # @start_end_log('load_db_as_df')
     def load_db_as_df(
         self, 
         typeraze: bool=False,
```

### Comparing `drtools-1.0.8/src/drtools/data_science/statistical_test.py` & `drtools-1.0.9/src/drtools/data_science/statistical_test.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/data_science/time_series.py` & `drtools-1.0.9/src/drtools/data_science/time_series.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/data_science/transformation.py` & `drtools-1.0.9/src/drtools/data_science/transformation.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/database/connection/postgresql.py` & `drtools-1.0.9/src/drtools/database/connection/postgresql.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/database/utils.py` & `drtools-1.0.9/src/drtools/database/utils.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/file_manager.py` & `drtools-1.0.9/src/drtools/file_manager.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/geo/common.py` & `drtools-1.0.9/src/drtools/geo/common.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/logs.py` & `drtools-1.0.9/src/drtools/logs.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/scrapping/authentication.py` & `drtools-1.0.9/src/drtools/scrapping/authentication.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/scrapping/config.py` & `drtools-1.0.9/src/drtools/scrapping/config.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/scrapping/interaction.py` & `drtools-1.0.9/src/drtools/scrapping/interaction.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/thread_pool_executor.py` & `drtools-1.0.9/src/drtools/thread_pool_executor.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools/utils.py` & `drtools-1.0.9/src/drtools/utils.py`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/src/drtools.egg-info/SOURCES.txt` & `drtools-1.0.9/src/drtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drtools-1.0.8/tests/test_utils.py` & `drtools-1.0.9/tests/test_utils.py`

 * *Files identical despite different names*

