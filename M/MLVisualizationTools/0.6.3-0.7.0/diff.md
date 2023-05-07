# Comparing `tmp/MLVisualizationTools-0.6.3.tar.gz` & `tmp/MLVisualizationTools-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLVisualizationTools-0.6.3.tar", last modified: Thu Mar 23 01:40:43 2023, max compression
+gzip compressed data, was "MLVisualizationTools-0.7.0.tar", last modified: Sun May  7 03:37:03 2023, max compression
```

## Comparing `MLVisualizationTools-0.6.3.tar` & `MLVisualizationTools-0.7.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:40:43.569647 MLVisualizationTools-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:40:43.557647 MLVisualizationTools-0.6.3/MLVisualizationTools/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/colorizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/dashbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/datainterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:40:43.561648 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/AnimationDemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/DashDemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/DashKaggleDemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/DashNotebookDemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/DataOverlayDemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:40:43.549647 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:40:43.561648 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Datasets/Titanic/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Datasets/Titanic/TitanicDemoPreprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    22848 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Datasets/Titanic/train.csv
--rw-r--r--   0 runner    (1001) docker     (123)    60302 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Datasets/Titanic/train_orig.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/MatplotlibDemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:40:43.553647 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:40:43.565647 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel/
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel/keras_metadata.pb
--rw-r--r--   0 runner    (1001) docker     (123)    93696 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel/saved_model.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:40:43.565647 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel/variables/variables.data-00000-of-00001
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel/variables/variables.index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:40:43.565647 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel_v2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel_v2.0/keras_metadata.pb
--rw-r--r--   0 runner    (1001) docker     (123)    89084 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel_v2.0/saved_model.pb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:40:43.565647 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/variables.data-00000-of-00001
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/variables.index
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/examples/TrainTitanicModel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:40:43.565647 MLVisualizationTools-0.6.3/MLVisualizationTools/express/
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/express/DashModelVisualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/express/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/graphinterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/modelanalytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/modelinterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:40:43.553647 MLVisualizationTools-0.6.3/MLVisualizationTools/theme_assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:40:43.565647 MLVisualizationTools-0.6.3/MLVisualizationTools/theme_assets/dark_assets/
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/theme_assets/dark_assets/darktheme.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:40:43.565647 MLVisualizationTools-0.6.3/MLVisualizationTools/theme_assets/light_assets/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/theme_assets/light_assets/lighttheme.css
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/MLVisualizationTools/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:40:43.561648 MLVisualizationTools-0.6.3/MLVisualizationTools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-03-23 01:40:43.000000 MLVisualizationTools-0.6.3/MLVisualizationTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-03-23 01:40:43.000000 MLVisualizationTools-0.6.3/MLVisualizationTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 01:40:43.000000 MLVisualizationTools-0.6.3/MLVisualizationTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-23 01:40:43.000000 MLVisualizationTools-0.6.3/MLVisualizationTools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-23 01:40:43.000000 MLVisualizationTools-0.6.3/MLVisualizationTools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-03-23 01:40:43.569647 MLVisualizationTools-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-03-23 01:40:43.569647 MLVisualizationTools-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 01:40:43.569647 MLVisualizationTools-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-23 01:40:33.000000 MLVisualizationTools-0.6.3/tests/testconf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.698009 MLVisualizationTools-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.690009 MLVisualizationTools-0.7.0/MLVisualizationTools/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/colorizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/dashbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/datainterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.694009 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/AnimationDemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/DashDemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/DashKaggleDemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/DashNotebookDemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/DataOverlayDemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.682010 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.694009 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Datasets/Titanic/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Datasets/Titanic/TitanicDemoPreprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22848 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Datasets/Titanic/train.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    60302 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Datasets/Titanic/train_orig.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/MatplotlibDemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.682010 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.694009 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/keras_metadata.pb
+-rw-r--r--   0 runner    (1001) docker     (123)    93696 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/saved_model.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.694009 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/variables/variables.data-00000-of-00001
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/variables/variables.index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.698009 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/keras_metadata.pb
+-rw-r--r--   0 runner    (1001) docker     (123)    89084 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/saved_model.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.698009 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/variables.data-00000-of-00001
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/variables.index
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/SklearnDemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/examples/TrainTitanicModel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.698009 MLVisualizationTools-0.7.0/MLVisualizationTools/express/
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/express/DashModelVisualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/express/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/graphinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/modelanalytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/modelinterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.682010 MLVisualizationTools-0.7.0/MLVisualizationTools/theme_assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.698009 MLVisualizationTools-0.7.0/MLVisualizationTools/theme_assets/dark_assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/theme_assets/dark_assets/darktheme.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.698009 MLVisualizationTools-0.7.0/MLVisualizationTools/theme_assets/light_assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/theme_assets/light_assets/lighttheme.css
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/MLVisualizationTools/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.690009 MLVisualizationTools-0.7.0/MLVisualizationTools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-07 03:37:03.000000 MLVisualizationTools-0.7.0/MLVisualizationTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-07 03:37:03.000000 MLVisualizationTools-0.7.0/MLVisualizationTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 03:37:03.000000 MLVisualizationTools-0.7.0/MLVisualizationTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-07 03:37:03.000000 MLVisualizationTools-0.7.0/MLVisualizationTools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 03:37:03.000000 MLVisualizationTools-0.7.0/MLVisualizationTools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-07 03:37:03.698009 MLVisualizationTools-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-07 03:37:03.698009 MLVisualizationTools-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:37:03.698009 MLVisualizationTools-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-07 03:36:47.000000 MLVisualizationTools-0.7.0/tests/testconf.py
```

### Comparing `MLVisualizationTools-0.6.3/LICENSE` & `MLVisualizationTools-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/backend.py` & `MLVisualizationTools-0.7.0/MLVisualizationTools/backend.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/colorizers.py` & `MLVisualizationTools-0.7.0/MLVisualizationTools/colorizers.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/dashbackend.py` & `MLVisualizationTools-0.7.0/MLVisualizationTools/dashbackend.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/datainterface.py` & `MLVisualizationTools-0.7.0/MLVisualizationTools/datainterface.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/AnimationDemo.py` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/AnimationDemo.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/DashDemo.py` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/DashDemo.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/DashKaggleDemo.py` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/DashKaggleDemo.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/DashNotebookDemo.py` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/DashNotebookDemo.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/DataOverlayDemo.py` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/DataOverlayDemo.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Datasets/Titanic/TitanicDemoPreprocess.py` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Datasets/Titanic/TitanicDemoPreprocess.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Datasets/Titanic/train.csv` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Datasets/Titanic/train.csv`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Datasets/Titanic/train_orig.csv` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Datasets/Titanic/train_orig.csv`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Demo.py` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Demo.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/MatplotlibDemo.py` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/MatplotlibDemo.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel/keras_metadata.pb` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/keras_metadata.pb`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel/saved_model.pb` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/saved_model.pb`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel/variables/variables.data-00000-of-00001` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel/variables/variables.index` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel/variables/variables.index`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel_v2.0/keras_metadata.pb` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/keras_metadata.pb`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel_v2.0/saved_model.pb` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/saved_model.pb`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/variables.data-00000-of-00001` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/variables.index` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/Models/titanicmodel_v2.0/variables/variables.index`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/examples/TrainTitanicModel.py` & `MLVisualizationTools-0.7.0/MLVisualizationTools/examples/TrainTitanicModel.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/express/DashModelVisualizer.py` & `MLVisualizationTools-0.7.0/MLVisualizationTools/express/DashModelVisualizer.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/graphinterface.py` & `MLVisualizationTools-0.7.0/MLVisualizationTools/graphinterface.py`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/modelanalytics.py` & `MLVisualizationTools-0.7.0/MLVisualizationTools/modelanalytics.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,15 +79,16 @@
 
     currentpos = 0
     for name, item in coldata.items():
         for i in range(0, steps):
             preddata[name][i + currentpos] = i * (item['max'] - item['min'])/(steps-1) + item['min']
         currentpos += steps
 
-    predictions = model.predict(preddata)
+
+    predictions = model.predict(preddata.values)
 
     currentpos = 0
     for name in coldata:
         values = predictions[currentpos:currentpos + steps]
         currentpos += steps
         AR.append(name, values.max() - values.min())
     return AR
```

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/modelinterface.py` & `MLVisualizationTools-0.7.0/MLVisualizationTools/modelinterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     preddata[x] = col
 
     col = []
     for pos in range(0, steps):
         col += [round(pos * (coldata[y]['max'] - coldata[y]['min']) / (steps - 1) + coldata[y]['min'], 6)] * steps
     preddata[y] = col
 
-    predictions = model.predict(preddata)
+    predictions = model.predict(preddata.values)
     if outputkey in preddata.columns:
         warnings.warn(f"Output key '{outputkey}' was already in dataframe. This means that '{outputkey}' "
                       "was a key in your dataset and could result in data being overwritten. "
                       "You can pick a different key in the function call.")
     preddata[outputkey] = predictions
     return GraphData(preddata, GraphDataTypes.Grid, steps, x, y, outputkey=outputkey)
 #endregion grid
@@ -168,15 +168,15 @@
     preddata[y] = col
 
     col = []
     for pos in range(0, steps):
         col += [round(pos * (coldata[anim]['max'] - coldata[anim]['min']) / (steps - 1) + coldata[anim]['min'],6 )] * (steps ** 2)
     preddata[anim] = col
 
-    predictions = model.predict(preddata)
+    predictions = model.predict(preddata.values)
     if outputkey in preddata.columns:
         warnings.warn(f"Output key '{outputkey}' was already in dataframe. This means that '{outputkey}' "
                       "was a key in your dataset and could result in data being overwritten. "
                       "You can pick a different key in the function call.")
     preddata[outputkey] = predictions
     return GraphData(preddata, GraphDataTypes.Animation, steps, x, y, anim, outputkey)
```

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools/theme_assets/dark_assets/darktheme.css` & `MLVisualizationTools-0.7.0/MLVisualizationTools/theme_assets/dark_assets/darktheme.css`

 * *Files identical despite different names*

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools.egg-info/PKG-INFO` & `MLVisualizationTools-0.7.0/MLVisualizationTools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLVisualizationTools
-Version: 0.6.3
+Version: 0.7.0
 Summary: A set of functions and demos to make machine learning projects easier to understand through effective visualizations.
 Home-page: https://github.com/RobertJN64/MLVisualizationTools
 Author: Robert Nies
 Author-email: robertjnies@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -161,7 +161,13 @@
 
 For version 2.0 through 2.4, we load a v2.0 model.
 For version 2.5+ we load a v2.5 model.
 
 If this causes compatibility issues you can still use the main library on your models. 
 If you need an example model, retrain it with 
 [TrainTitanicModel.py](/MLVisualizationTools/examples/TrainTitanicModel.py)
+
+## scikit-learn Compatibility
+
+See [SklearnDemo.py](/MLVisualizationTools/examples/SklearnDemo.py)
+
+Sklearn can be used exactly like TF because it has the same `.predict(X, Y)` interface.
```

### Comparing `MLVisualizationTools-0.6.3/MLVisualizationTools.egg-info/SOURCES.txt` & `MLVisualizationTools-0.7.0/MLVisualizationTools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 MLVisualizationTools/examples/AnimationDemo.py
 MLVisualizationTools/examples/DashDemo.py
 MLVisualizationTools/examples/DashKaggleDemo.py
 MLVisualizationTools/examples/DashNotebookDemo.py
 MLVisualizationTools/examples/DataOverlayDemo.py
 MLVisualizationTools/examples/Demo.py
 MLVisualizationTools/examples/MatplotlibDemo.py
+MLVisualizationTools/examples/SklearnDemo.py
 MLVisualizationTools/examples/TrainTitanicModel.py
 MLVisualizationTools/examples/Datasets/Titanic/TitanicDemoPreprocess.py
 MLVisualizationTools/examples/Datasets/Titanic/train.csv
 MLVisualizationTools/examples/Datasets/Titanic/train_orig.csv
 MLVisualizationTools/examples/Models/titanicmodel/keras_metadata.pb
 MLVisualizationTools/examples/Models/titanicmodel/saved_model.pb
 MLVisualizationTools/examples/Models/titanicmodel/variables/variables.data-00000-of-00001
```

### Comparing `MLVisualizationTools-0.6.3/PKG-INFO` & `MLVisualizationTools-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLVisualizationTools
-Version: 0.6.3
+Version: 0.7.0
 Summary: A set of functions and demos to make machine learning projects easier to understand through effective visualizations.
 Home-page: https://github.com/RobertJN64/MLVisualizationTools
 Author: Robert Nies
 Author-email: robertjnies@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -161,7 +161,13 @@
 
 For version 2.0 through 2.4, we load a v2.0 model.
 For version 2.5+ we load a v2.5 model.
 
 If this causes compatibility issues you can still use the main library on your models. 
 If you need an example model, retrain it with 
 [TrainTitanicModel.py](/MLVisualizationTools/examples/TrainTitanicModel.py)
+
+## scikit-learn Compatibility
+
+See [SklearnDemo.py](/MLVisualizationTools/examples/SklearnDemo.py)
+
+Sklearn can be used exactly like TF because it has the same `.predict(X, Y)` interface.
```

### Comparing `MLVisualizationTools-0.6.3/README.md` & `MLVisualizationTools-0.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -137,8 +137,14 @@
 to make running examples quick and easy. It is not needed for main library functions.
 
 For version 2.0 through 2.4, we load a v2.0 model.
 For version 2.5+ we load a v2.5 model.
 
 If this causes compatibility issues you can still use the main library on your models. 
 If you need an example model, retrain it with 
-[TrainTitanicModel.py](/MLVisualizationTools/examples/TrainTitanicModel.py)
+[TrainTitanicModel.py](/MLVisualizationTools/examples/TrainTitanicModel.py)
+
+## scikit-learn Compatibility
+
+See [SklearnDemo.py](/MLVisualizationTools/examples/SklearnDemo.py)
+
+Sklearn can be used exactly like TF because it has the same `.predict(X, Y)` interface.
```

### Comparing `MLVisualizationTools-0.6.3/setup.cfg` & `MLVisualizationTools-0.7.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = MLVisualizationTools
 description = A set of functions and demos to make machine learning projects easier to understand through effective visualizations.
 author = Robert Nies
 license = MIT
 license_file = LICENSE
 url = https://github.com/RobertJN64/MLVisualizationTools
 author_email = robertjnies@gmail.com
-version = 0.6.3
+version = 0.7.0
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
```

### Comparing `MLVisualizationTools-0.6.3/tests/test_basic.py` & `MLVisualizationTools-0.7.0/tests/test_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,18 @@
 
     import MLVisualizationTools.examples.AnimationDemo as AnimationDemo
     AnimationDemo.main(show=False)
 
     import MLVisualizationTools.examples.DataOverlayDemo as DODemo
     DODemo.main(show=False)
 
+    import MLVisualizationTools.examples.SklearnDemo as SKDemo
+    SKDemo.main(show=False)
+
+
 def test_mpl():
     import matplotlib
     matplotlib.use('Agg')  # disables UI rendering
     import warnings
     warnings.filterwarnings(
         action='ignore',
         category=UserWarning,
```

