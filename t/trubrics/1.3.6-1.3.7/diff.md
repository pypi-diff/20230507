# Comparing `tmp/trubrics-1.3.6.tar.gz` & `tmp/trubrics-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trubrics-1.3.6.tar", last modified: Wed May  3 06:41:48 2023, max compression
+gzip compressed data, was "trubrics-1.3.7.tar", last modified: Sun May  7 11:02:28 2023, max compression
```

## Comparing `trubrics-1.3.6.tar` & `trubrics-1.3.7.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.977897 trubrics-1.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-05-03 06:41:38.000000 trubrics-1.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-03 06:41:48.977897 trubrics-1.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-05-03 06:41:38.000000 trubrics-1.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.965897 trubrics-1.3.6/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:38.000000 trubrics-1.3.6/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.965897 trubrics-1.3.6/examples/classification_titanic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:38.000000 trubrics-1.3.6/examples/classification_titanic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-03 06:41:38.000000 trubrics-1.3.6/examples/classification_titanic/custom_scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-03 06:41:38.000000 trubrics-1.3.6/examples/classification_titanic/custom_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-03 06:41:38.000000 trubrics-1.3.6/examples/classification_titanic/slicing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-03 06:41:38.000000 trubrics-1.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-03 06:41:38.000000 trubrics-1.3.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-03 06:41:48.977897 trubrics-1.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.965897 trubrics-1.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-03 06:41:38.000000 trubrics-1.3.6/tests/test_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.965897 trubrics-1.3.6/trubrics/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.969897 trubrics-1.3.6/trubrics/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.969897 trubrics-1.3.6/trubrics/example/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/example/app_titanic_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/example/app_titanic_gradio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/example/app_titanic_streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/example/my_first_trubric.json
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/example/titanic.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/example/titanic_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    61194 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/example/titanic_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/example/trubric_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.969897 trubrics-1.3.6/trubrics/feedback/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/feedback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/feedback/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/feedback/dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.969897 trubrics-1.3.6/trubrics/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.969897 trubrics-1.3.6/trubrics/integrations/dash/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/dash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/dash/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.973897 trubrics-1.3.6/trubrics/integrations/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/gradio/collect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.973897 trubrics-1.3.6/trubrics/integrations/mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/mlflow/trubrics_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.973897 trubrics-1.3.6/trubrics/integrations/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/streamlit/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/integrations/streamlit/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.973897 trubrics-1.3.6/trubrics/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/ui/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/ui/firestore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/ui/trubrics_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.973897 trubrics-1.3.6/trubrics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/utils/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.973897 trubrics-1.3.6/trubrics/validations/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/validations/dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.977897 trubrics-1.3.6/trubrics/validations/model/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/validations/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/validations/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/validations/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-03 06:41:38.000000 trubrics-1.3.6/trubrics/validations/validation_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:41:48.969897 trubrics-1.3.6/trubrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-03 06:41:48.000000 trubrics-1.3.6/trubrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-03 06:41:48.000000 trubrics-1.3.6/trubrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:41:48.000000 trubrics-1.3.6/trubrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-03 06:41:48.000000 trubrics-1.3.6/trubrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-03 06:41:48.000000 trubrics-1.3.6/trubrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 06:41:48.000000 trubrics-1.3.6/trubrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.611936 trubrics-1.3.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-05-07 11:02:18.000000 trubrics-1.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-07 11:02:28.611936 trubrics-1.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-05-07 11:02:18.000000 trubrics-1.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.599936 trubrics-1.3.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:18.000000 trubrics-1.3.7/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.603936 trubrics-1.3.7/examples/classification_titanic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:18.000000 trubrics-1.3.7/examples/classification_titanic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-07 11:02:18.000000 trubrics-1.3.7/examples/classification_titanic/custom_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-07 11:02:18.000000 trubrics-1.3.7/examples/classification_titanic/custom_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-07 11:02:18.000000 trubrics-1.3.7/examples/classification_titanic/slicing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-07 11:02:18.000000 trubrics-1.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-07 11:02:18.000000 trubrics-1.3.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-07 11:02:28.611936 trubrics-1.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.603936 trubrics-1.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-07 11:02:18.000000 trubrics-1.3.7/tests/test_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.603936 trubrics-1.3.7/trubrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.603936 trubrics-1.3.7/trubrics/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.607936 trubrics-1.3.7/trubrics/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/example/app_titanic_dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/example/app_titanic_gradio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/example/app_titanic_streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/example/my_first_trubric.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/example/titanic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/example/titanic_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61194 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/example/titanic_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/example/trubric_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.607936 trubrics-1.3.7/trubrics/feedback/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/feedback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/feedback/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/feedback/dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.607936 trubrics-1.3.7/trubrics/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.607936 trubrics-1.3.7/trubrics/integrations/dash/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/dash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/dash/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.607936 trubrics-1.3.7/trubrics/integrations/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/gradio/collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.607936 trubrics-1.3.7/trubrics/integrations/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/mlflow/trubrics_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.607936 trubrics-1.3.7/trubrics/integrations/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/streamlit/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/integrations/streamlit/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.611936 trubrics-1.3.7/trubrics/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/ui/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/ui/firestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/ui/trubrics_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.611936 trubrics-1.3.7/trubrics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/utils/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.611936 trubrics-1.3.7/trubrics/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/validations/dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.611936 trubrics-1.3.7/trubrics/validations/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/validations/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/validations/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/validations/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-07 11:02:18.000000 trubrics-1.3.7/trubrics/validations/validation_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:02:28.603936 trubrics-1.3.7/trubrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-07 11:02:28.000000 trubrics-1.3.7/trubrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-07 11:02:28.000000 trubrics-1.3.7/trubrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 11:02:28.000000 trubrics-1.3.7/trubrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-07 11:02:28.000000 trubrics-1.3.7/trubrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-07 11:02:28.000000 trubrics-1.3.7/trubrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 11:02:28.000000 trubrics-1.3.7/trubrics.egg-info/top_level.txt
```

### Comparing `trubrics-1.3.6/LICENSE` & `trubrics-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/README.md` & `trubrics-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/examples/classification_titanic/custom_validator.py` & `trubrics-1.3.7/examples/classification_titanic/custom_validator.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/setup.cfg` & `trubrics-1.3.7/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trubrics
-version = 1.3.6
+version = 1.3.7
 description = Combine data science knowledge with business user feedback to validate machine learning.
 long_description = Full documentation available at https://trubrics.github.io/trubrics-sdk/.
 
 [options]
 packages = find:
 install_requires = file: requirements.txt
 
@@ -24,15 +24,15 @@
 [flake8]
 max-line-length = 120
 
 [isort]
 profile = black
 
 [options.extras_require]
-streamlit = streamlit>=1.11.1,<1.18.0
+streamlit = streamlit>=1.18.0
 dash = dash>=2.6.2; dash-bootstrap-components>=1.2.1
 gradio = gradio>=3.8.1
 mlflow = mlflow>=2.0.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `trubrics-1.3.6/tests/test_context.py` & `trubrics-1.3.7/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/cli/main.py` & `trubrics-1.3.7/trubrics/cli/main.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/cli/run.py` & `trubrics-1.3.7/trubrics/cli/run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/context.py` & `trubrics-1.3.7/trubrics/context.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/example/app_titanic_streamlit.py` & `trubrics-1.3.7/trubrics/example/app_titanic_streamlit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,33 @@
+import os
 from typing import Optional
 
 import streamlit as st
 import typer
 
+from trubrics.cli.main import init
 from trubrics.context import DataContext
 from trubrics.example import get_titanic_data_and_model
 from trubrics.example import titanic_config as tc
 from trubrics.integrations.streamlit import (
     FeedbackCollector,
     generate_what_if_streamlit,
 )
 
 cli = typer.Typer()
 
 
-@st.cache(allow_output_mutation=True)
+@st.cache_resource
 def init_trubrics(trubrics_platform_auth):
+    if trubrics_platform_auth:
+        with st.spinner("Connecting to the Trubrics platform..."):
+            project_name = os.environ.get("TRUBRICS_PROJECT_NAME")
+            if project_name is None:
+                raise KeyError("Environment variable TRUBRICS_PROJECT_NAME is not set.")
+            init(project_name=project_name)
     _, test_df, model = get_titanic_data_and_model()
 
     data_context = DataContext(
         testing_data=test_df,
         target="Survived",
         categorical_columns=tc.CATEGORICAL_COLUMNS,
         business_columns=tc.BUSINESS_COLUMNS,
@@ -63,14 +71,16 @@
             """
         )
     st.markdown("***")
 
 
 @cli.command()
 def main(trubrics_platform_auth: Optional[str] = None):
+    if trubrics_platform_auth is None:
+        trubrics_platform_auth = os.environ.get("TRUBRICS_PLATFORM_AUTH")
     model, data_context, collector = init_trubrics(trubrics_platform_auth)
 
     st.title("Titanic Demo App")
     with st.expander("Notes on the demo"):
         st.markdown(
             """
         The sidebar of features and the '**Model prediction**' section below are not a part
```

### Comparing `trubrics-1.3.6/trubrics/example/my_first_trubric.json` & `trubrics-1.3.7/trubrics/example/my_first_trubric.json`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/example/titanic.py` & `trubrics-1.3.7/trubrics/example/titanic.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/example/titanic_data.csv` & `trubrics-1.3.7/trubrics/example/titanic_data.csv`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/example/trubric_run.py` & `trubrics-1.3.7/trubrics/example/trubric_run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/exceptions.py` & `trubrics-1.3.7/trubrics/exceptions.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/feedback/config.py` & `trubrics-1.3.7/trubrics/feedback/config.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/feedback/dataclass.py` & `trubrics-1.3.7/trubrics/feedback/dataclass.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/integrations/dash/collect.py` & `trubrics-1.3.7/trubrics/integrations/dash/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/integrations/gradio/collect.py` & `trubrics-1.3.7/trubrics/integrations/gradio/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/integrations/mlflow/trubrics_validator.py` & `trubrics-1.3.7/trubrics/integrations/mlflow/trubrics_validator.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/integrations/streamlit/collect.py` & `trubrics-1.3.7/trubrics/integrations/streamlit/collect.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/integrations/streamlit/experiment.py` & `trubrics-1.3.7/trubrics/integrations/streamlit/experiment.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/ui/auth.py` & `trubrics-1.3.7/trubrics/ui/auth.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/ui/firestore.py` & `trubrics-1.3.7/trubrics/ui/firestore.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/ui/trubrics_config.py` & `trubrics-1.3.7/trubrics/ui/trubrics_config.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/validations/dataclass.py` & `trubrics-1.3.7/trubrics/validations/dataclass.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/validations/model/base.py` & `trubrics-1.3.7/trubrics/validations/model/base.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/validations/run.py` & `trubrics-1.3.7/trubrics/validations/run.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics/validations/validation_output.py` & `trubrics-1.3.7/trubrics/validations/validation_output.py`

 * *Files identical despite different names*

### Comparing `trubrics-1.3.6/trubrics.egg-info/SOURCES.txt` & `trubrics-1.3.7/trubrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

