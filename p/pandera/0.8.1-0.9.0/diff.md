# Comparing `tmp/pandera-0.8.1.tar.gz` & `tmp/pandera-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pandera-0.8.1.tar", last modified: Fri Dec 31 21:44:23 2021, max compression
+gzip compressed data, was "pandera-0.9.0.tar", last modified: Wed Feb  9 00:35:29 2022, max compression
```

## Comparing `pandera-0.8.1.tar` & `pandera-0.9.0.tar`

### file list

```diff
@@ -1,102 +1,107 @@
-drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2021-12-31 21:44:23.766294 pandera-0.8.1/
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     1071 2021-02-23 22:18:56.000000 pandera-0.8.1/LICENSE.txt
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    12683 2021-12-31 21:44:23.766425 pandera-0.8.1/PKG-INFO
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    11416 2021-12-31 15:23:31.000000 pandera-0.8.1/README.md
-drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2021-12-31 21:44:23.752378 pandera-0.8.1/pandera/
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     2867 2021-12-24 18:06:40.000000 pandera-0.8.1/pandera/__init__.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     4950 2021-11-11 18:23:50.000000 pandera-0.8.1/pandera/check_utils.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    35291 2021-11-20 20:32:50.000000 pandera-0.8.1/pandera/checks.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)      107 2021-12-28 14:39:41.000000 pandera-0.8.1/pandera/constants.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)      387 2021-11-11 18:23:50.000000 pandera-0.8.1/pandera/dask_accessor.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    22026 2021-12-26 15:46:53.000000 pandera-0.8.1/pandera/decorators.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     1133 2021-08-26 13:06:23.000000 pandera-0.8.1/pandera/deprecations.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    13608 2021-11-11 18:23:50.000000 pandera-0.8.1/pandera/dtypes.py
-drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2021-12-31 21:44:23.755073 pandera-0.8.1/pandera/engines/
--rw-r--r--   0 nielsbantilan   (501) staff       (20)        0 2021-08-26 13:06:23.000000 pandera-0.8.1/pandera/engines/__init__.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     6986 2021-12-24 18:06:40.000000 pandera-0.8.1/pandera/engines/engine.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    11654 2021-12-24 18:06:40.000000 pandera-0.8.1/pandera/engines/numpy_engine.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    24540 2021-12-24 18:06:40.000000 pandera-0.8.1/pandera/engines/pandas_engine.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)      282 2021-08-26 13:06:23.000000 pandera-0.8.1/pandera/engines/type_aliases.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     4436 2021-11-11 18:23:50.000000 pandera-0.8.1/pandera/engines/utils.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     4446 2021-11-11 18:23:50.000000 pandera-0.8.1/pandera/error_formatters.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     1550 2021-06-26 15:15:54.000000 pandera-0.8.1/pandera/error_handlers.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     8882 2021-12-31 16:55:29.000000 pandera-0.8.1/pandera/errors.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     6178 2021-11-11 05:54:23.000000 pandera-0.8.1/pandera/extensions.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)      850 2021-11-11 18:23:50.000000 pandera-0.8.1/pandera/external_config.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    18500 2021-10-15 12:49:46.000000 pandera-0.8.1/pandera/hypotheses.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     1389 2021-08-26 13:06:23.000000 pandera-0.8.1/pandera/inspection_utils.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    22409 2021-12-08 03:05:35.000000 pandera-0.8.1/pandera/io.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)      392 2021-11-11 18:23:50.000000 pandera-0.8.1/pandera/koalas_accessor.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    18650 2021-12-26 15:46:53.000000 pandera-0.8.1/pandera/model.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    12159 2021-12-24 18:06:40.000000 pandera-0.8.1/pandera/model_components.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     2838 2021-11-11 18:23:50.000000 pandera-0.8.1/pandera/modin_accessor.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     3762 2021-12-24 18:06:40.000000 pandera-0.8.1/pandera/mypy.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     1681 2021-12-08 06:11:45.000000 pandera-0.8.1/pandera/pandas_accessor.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)        0 2021-10-08 13:38:39.000000 pandera-0.8.1/pandera/py.typed
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    28112 2021-11-11 18:23:50.000000 pandera-0.8.1/pandera/schema_components.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     2735 2021-08-26 13:06:23.000000 pandera-0.8.1/pandera/schema_inference.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     7168 2021-09-10 15:12:41.000000 pandera-0.8.1/pandera/schema_statistics.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    82980 2021-12-24 18:06:40.000000 pandera-0.8.1/pandera/schemas.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    42066 2021-11-11 18:23:50.000000 pandera-0.8.1/pandera/strategies.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)      219 2021-10-15 12:49:46.000000 pandera-0.8.1/pandera/system.py
-drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2021-12-31 21:44:23.756541 pandera-0.8.1/pandera/typing/
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     1174 2021-12-26 15:46:53.000000 pandera-0.8.1/pandera/typing/__init__.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     6401 2021-12-24 18:06:40.000000 pandera-0.8.1/pandera/typing/common.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     2133 2021-12-24 18:06:40.000000 pandera-0.8.1/pandera/typing/dask.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     1481 2021-11-11 18:23:50.000000 pandera-0.8.1/pandera/typing/koalas.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     1157 2021-11-11 18:23:50.000000 pandera-0.8.1/pandera/typing/modin.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     3168 2021-12-26 15:46:53.000000 pandera-0.8.1/pandera/typing/pandas.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)       42 2021-12-28 14:29:36.000000 pandera-0.8.1/pandera/version.py
-drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2021-12-31 21:44:23.753576 pandera-0.8.1/pandera.egg-info/
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    12683 2021-12-31 21:44:23.000000 pandera-0.8.1/pandera.egg-info/PKG-INFO
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     2341 2021-12-31 21:44:23.000000 pandera-0.8.1/pandera.egg-info/SOURCES.txt
--rw-r--r--   0 nielsbantilan   (501) staff       (20)        1 2021-12-31 21:44:23.000000 pandera-0.8.1/pandera.egg-info/dependency_links.txt
--rw-r--r--   0 nielsbantilan   (501) staff       (20)      479 2021-12-31 21:44:23.000000 pandera-0.8.1/pandera.egg-info/requires.txt
--rw-r--r--   0 nielsbantilan   (501) staff       (20)       14 2021-12-31 21:44:23.000000 pandera-0.8.1/pandera.egg-info/top_level.txt
--rw-r--r--   0 nielsbantilan   (501) staff       (20)       83 2021-11-11 18:23:50.000000 pandera-0.8.1/pyproject.toml
--rw-r--r--   0 nielsbantilan   (501) staff       (20)      251 2021-12-31 21:44:23.766858 pandera-0.8.1/setup.cfg
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     2229 2021-12-24 18:09:33.000000 pandera-0.8.1/setup.py
-drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2021-12-31 21:44:23.757198 pandera-0.8.1/tests/
--rw-r--r--   0 nielsbantilan   (501) staff       (20)        0 2019-06-06 04:39:12.000000 pandera-0.8.1/tests/__init__.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)      591 2021-10-13 04:51:53.000000 pandera-0.8.1/tests/conftest.py
-drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2021-12-31 21:44:23.763760 pandera-0.8.1/tests/core/
--rw-r--r--   0 nielsbantilan   (501) staff       (20)        0 2021-02-25 19:31:37.000000 pandera-0.8.1/tests/core/__init__.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     1031 2021-07-25 18:12:05.000000 pandera-0.8.1/tests/core/checks_fixtures.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)      143 2021-09-24 18:55:14.000000 pandera-0.8.1/tests/core/conftest.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    13637 2021-09-24 17:14:37.000000 pandera-0.8.1/tests/core/test_checks.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    32000 2021-09-22 13:14:15.000000 pandera-0.8.1/tests/core/test_checks_builtin.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    27951 2021-10-15 12:49:46.000000 pandera-0.8.1/tests/core/test_decorators.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     1556 2021-11-11 18:23:50.000000 pandera-0.8.1/tests/core/test_deprecations.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)      818 2021-08-26 13:06:23.000000 pandera-0.8.1/tests/core/test_docs_setting_column_widths.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    17783 2021-12-24 18:06:40.000000 pandera-0.8.1/tests/core/test_dtypes.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     5565 2021-08-26 13:06:23.000000 pandera-0.8.1/tests/core/test_engine.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     2121 2021-08-26 13:06:23.000000 pandera-0.8.1/tests/core/test_engine_utils.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     9633 2021-12-31 16:55:29.000000 pandera-0.8.1/tests/core/test_errors.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)      477 2021-08-26 13:06:23.000000 pandera-0.8.1/tests/core/test_extension_modules.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     8940 2021-10-18 15:24:14.000000 pandera-0.8.1/tests/core/test_extensions.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    26261 2021-12-16 15:37:33.000000 pandera-0.8.1/tests/core/test_model.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     2445 2021-09-10 15:12:41.000000 pandera-0.8.1/tests/core/test_model_components.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     1471 2021-08-26 13:06:23.000000 pandera-0.8.1/tests/core/test_numpy_engine.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     2223 2021-11-11 18:23:50.000000 pandera-0.8.1/tests/core/test_pandas_accessor.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     1364 2021-11-11 18:23:50.000000 pandera-0.8.1/tests/core/test_pandas_engine.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     4668 2021-11-11 18:23:50.000000 pandera-0.8.1/tests/core/test_pydantic.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    25083 2021-10-18 15:24:24.000000 pandera-0.8.1/tests/core/test_schema_components.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     4075 2021-08-26 13:06:23.000000 pandera-0.8.1/tests/core/test_schema_inference.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    19461 2021-09-10 15:12:41.000000 pandera-0.8.1/tests/core/test_schema_statistics.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    59874 2021-10-15 12:49:46.000000 pandera-0.8.1/tests/core/test_schemas.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    13116 2021-12-24 18:06:40.000000 pandera-0.8.1/tests/core/test_typing.py
-drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2021-12-31 21:44:23.764711 pandera-0.8.1/tests/dask/
--rw-r--r--   0 nielsbantilan   (501) staff       (20)        0 2021-11-11 18:23:50.000000 pandera-0.8.1/tests/dask/__init__.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     4040 2021-11-11 18:23:50.000000 pandera-0.8.1/tests/dask/test_dask.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     1842 2021-11-11 18:23:50.000000 pandera-0.8.1/tests/dask/test_dask_accessor.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     1206 2021-11-11 18:23:50.000000 pandera-0.8.1/tests/dask/test_dask_not_installed.py
-drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2021-12-31 21:44:23.765178 pandera-0.8.1/tests/hypotheses/
--rw-r--r--   0 nielsbantilan   (501) staff       (20)        0 2021-02-25 19:31:37.000000 pandera-0.8.1/tests/hypotheses/__init__.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     9605 2021-02-25 19:31:37.000000 pandera-0.8.1/tests/hypotheses/test_hypotheses.py
-drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2021-12-31 21:44:23.765572 pandera-0.8.1/tests/io/
--rw-r--r--   0 nielsbantilan   (501) staff       (20)        0 2021-02-25 19:31:37.000000 pandera-0.8.1/tests/io/__init__.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    25771 2021-11-11 18:23:50.000000 pandera-0.8.1/tests/io/test_io.py
-drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2021-12-31 21:44:23.766040 pandera-0.8.1/tests/strategies/
--rw-r--r--   0 nielsbantilan   (501) staff       (20)        0 2021-02-25 19:31:37.000000 pandera-0.8.1/tests/strategies/__init__.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)    32540 2021-12-24 18:06:40.000000 pandera-0.8.1/tests/strategies/test_strategies.py
--rw-r--r--   0 nielsbantilan   (501) staff       (20)     2916 2021-08-26 13:06:23.000000 pandera-0.8.1/tests/test_inspection_utils.py
+drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2022-02-09 00:35:29.317079 pandera-0.9.0/
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     1071 2021-02-23 22:18:56.000000 pandera-0.9.0/LICENSE.txt
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    12839 2022-02-09 00:35:29.317233 pandera-0.9.0/PKG-INFO
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    11471 2022-02-08 16:44:29.000000 pandera-0.9.0/README.md
+drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2022-02-09 00:35:29.299623 pandera-0.9.0/pandera/
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     2890 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/__init__.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     4950 2021-11-11 18:23:50.000000 pandera-0.9.0/pandera/check_utils.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    35827 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/checks.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)      107 2021-12-28 14:39:41.000000 pandera-0.9.0/pandera/constants.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)      387 2021-11-11 18:23:50.000000 pandera-0.9.0/pandera/dask_accessor.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    23481 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/decorators.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     1133 2021-08-26 13:06:23.000000 pandera-0.9.0/pandera/deprecations.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    13608 2021-11-11 18:23:50.000000 pandera-0.9.0/pandera/dtypes.py
+drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2022-02-09 00:35:29.302419 pandera-0.9.0/pandera/engines/
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)        0 2021-08-26 13:06:23.000000 pandera-0.9.0/pandera/engines/__init__.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     6986 2021-12-24 18:06:40.000000 pandera-0.9.0/pandera/engines/engine.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    11654 2022-01-10 00:11:52.000000 pandera-0.9.0/pandera/engines/numpy_engine.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    25892 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/engines/pandas_engine.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)      282 2021-08-26 13:06:23.000000 pandera-0.9.0/pandera/engines/type_aliases.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     4436 2021-11-11 18:23:50.000000 pandera-0.9.0/pandera/engines/utils.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     4365 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/error_formatters.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     1550 2021-06-26 15:15:54.000000 pandera-0.9.0/pandera/error_handlers.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     8882 2022-01-13 18:45:51.000000 pandera-0.9.0/pandera/errors.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     6178 2021-11-11 05:54:23.000000 pandera-0.9.0/pandera/extensions.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)      850 2021-11-11 18:23:50.000000 pandera-0.9.0/pandera/external_config.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    18500 2021-10-15 12:49:46.000000 pandera-0.9.0/pandera/hypotheses.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     1389 2021-08-26 13:06:23.000000 pandera-0.9.0/pandera/inspection_utils.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    22409 2021-12-08 03:05:35.000000 pandera-0.9.0/pandera/io.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     1030 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/json_schema.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)      545 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/koalas_accessor.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    18368 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/model.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    12870 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/model_components.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     2838 2022-01-14 02:40:23.000000 pandera-0.9.0/pandera/modin_accessor.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     3762 2022-01-10 00:13:36.000000 pandera-0.9.0/pandera/mypy.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     1681 2021-12-08 06:11:45.000000 pandera-0.9.0/pandera/pandas_accessor.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)        0 2021-10-08 13:38:39.000000 pandera-0.9.0/pandera/py.typed
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    28452 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/schema_components.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     2735 2021-08-26 13:06:23.000000 pandera-0.9.0/pandera/schema_inference.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     7168 2021-09-10 15:12:41.000000 pandera-0.9.0/pandera/schema_statistics.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    84402 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/schemas.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    42144 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/strategies.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)      219 2021-10-15 12:49:46.000000 pandera-0.9.0/pandera/system.py
+drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2022-02-09 00:35:29.304829 pandera-0.9.0/pandera/typing/
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     1330 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/typing/__init__.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     7930 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/typing/common.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     2529 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/typing/config.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     2133 2022-01-23 21:03:51.000000 pandera-0.9.0/pandera/typing/dask.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     2123 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/typing/fastapi.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     1212 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/typing/formats.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)      986 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/typing/geopandas.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     1481 2022-01-12 00:16:41.000000 pandera-0.9.0/pandera/typing/koalas.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     1157 2022-01-12 00:16:46.000000 pandera-0.9.0/pandera/typing/modin.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     5862 2022-02-08 16:44:29.000000 pandera-0.9.0/pandera/typing/pandas.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)       42 2022-02-08 16:45:08.000000 pandera-0.9.0/pandera/version.py
+drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2022-02-09 00:35:29.300844 pandera-0.9.0/pandera.egg-info/
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    12839 2022-02-09 00:35:29.000000 pandera-0.9.0/pandera.egg-info/PKG-INFO
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     2469 2022-02-09 00:35:29.000000 pandera-0.9.0/pandera.egg-info/SOURCES.txt
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)        1 2022-02-09 00:35:29.000000 pandera-0.9.0/pandera.egg-info/dependency_links.txt
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)      564 2022-02-09 00:35:29.000000 pandera-0.9.0/pandera.egg-info/requires.txt
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)        8 2022-02-09 00:35:29.000000 pandera-0.9.0/pandera.egg-info/top_level.txt
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)       83 2021-11-11 18:23:50.000000 pandera-0.9.0/pyproject.toml
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)      251 2022-02-09 00:35:29.317769 pandera-0.9.0/setup.cfg
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     2390 2022-02-08 16:44:29.000000 pandera-0.9.0/setup.py
+drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2022-02-09 00:35:29.305469 pandera-0.9.0/tests/
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)        0 2019-06-06 04:39:12.000000 pandera-0.9.0/tests/__init__.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)      590 2022-02-08 16:44:29.000000 pandera-0.9.0/tests/conftest.py
+drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2022-02-09 00:35:29.314663 pandera-0.9.0/tests/core/
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)        0 2021-02-25 19:31:37.000000 pandera-0.9.0/tests/core/__init__.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     1031 2021-07-25 18:12:05.000000 pandera-0.9.0/tests/core/checks_fixtures.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)      143 2021-09-24 18:55:14.000000 pandera-0.9.0/tests/core/conftest.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    14391 2022-02-08 16:44:29.000000 pandera-0.9.0/tests/core/test_checks.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    32000 2021-09-22 13:14:15.000000 pandera-0.9.0/tests/core/test_checks_builtin.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    27951 2022-01-31 21:13:11.000000 pandera-0.9.0/tests/core/test_decorators.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     1556 2021-11-11 18:23:50.000000 pandera-0.9.0/tests/core/test_deprecations.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)      818 2021-08-26 13:06:23.000000 pandera-0.9.0/tests/core/test_docs_setting_column_widths.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    18652 2022-02-08 16:44:29.000000 pandera-0.9.0/tests/core/test_dtypes.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     5565 2021-08-26 13:06:23.000000 pandera-0.9.0/tests/core/test_engine.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     2121 2021-08-26 13:06:23.000000 pandera-0.9.0/tests/core/test_engine_utils.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     9633 2022-01-10 00:13:36.000000 pandera-0.9.0/tests/core/test_errors.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)      477 2021-08-26 13:06:23.000000 pandera-0.9.0/tests/core/test_extension_modules.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     8940 2021-10-18 15:24:14.000000 pandera-0.9.0/tests/core/test_extensions.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    26541 2022-02-08 16:44:29.000000 pandera-0.9.0/tests/core/test_model.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     2445 2021-09-10 15:12:41.000000 pandera-0.9.0/tests/core/test_model_components.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     1471 2021-08-26 13:06:23.000000 pandera-0.9.0/tests/core/test_numpy_engine.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     2223 2021-11-11 18:23:50.000000 pandera-0.9.0/tests/core/test_pandas_accessor.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     1364 2021-11-11 18:23:50.000000 pandera-0.9.0/tests/core/test_pandas_engine.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     4668 2021-11-11 18:23:50.000000 pandera-0.9.0/tests/core/test_pydantic.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    25083 2021-10-18 15:24:24.000000 pandera-0.9.0/tests/core/test_schema_components.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     4075 2021-08-26 13:06:23.000000 pandera-0.9.0/tests/core/test_schema_inference.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    19461 2021-09-10 15:12:41.000000 pandera-0.9.0/tests/core/test_schema_statistics.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    60087 2022-02-08 16:44:29.000000 pandera-0.9.0/tests/core/test_schemas.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    13116 2021-12-24 18:06:40.000000 pandera-0.9.0/tests/core/test_typing.py
+drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2022-02-09 00:35:29.315549 pandera-0.9.0/tests/dask/
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)        0 2021-11-11 18:23:50.000000 pandera-0.9.0/tests/dask/__init__.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     4040 2021-11-11 18:23:50.000000 pandera-0.9.0/tests/dask/test_dask.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     1842 2021-11-11 18:23:50.000000 pandera-0.9.0/tests/dask/test_dask_accessor.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     1206 2021-11-11 18:23:50.000000 pandera-0.9.0/tests/dask/test_dask_not_installed.py
+drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2022-02-09 00:35:29.315964 pandera-0.9.0/tests/hypotheses/
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)        0 2021-02-25 19:31:37.000000 pandera-0.9.0/tests/hypotheses/__init__.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     9605 2021-02-25 19:31:37.000000 pandera-0.9.0/tests/hypotheses/test_hypotheses.py
+drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2022-02-09 00:35:29.316361 pandera-0.9.0/tests/io/
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)        0 2021-02-25 19:31:37.000000 pandera-0.9.0/tests/io/__init__.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    25771 2021-11-11 18:23:50.000000 pandera-0.9.0/tests/io/test_io.py
+drwxr-xr-x   0 nielsbantilan   (501) staff       (20)        0 2022-02-09 00:35:29.316818 pandera-0.9.0/tests/strategies/
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)        0 2021-02-25 19:31:37.000000 pandera-0.9.0/tests/strategies/__init__.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)    32662 2022-02-08 16:44:29.000000 pandera-0.9.0/tests/strategies/test_strategies.py
+-rw-r--r--   0 nielsbantilan   (501) staff       (20)     2916 2021-08-26 13:06:23.000000 pandera-0.9.0/tests/test_inspection_utils.py
```

### Comparing `pandera-0.8.1/LICENSE.txt` & `pandera-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/PKG-INFO` & `pandera-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandera
-Version: 0.8.1
+Version: 0.9.0
 Summary: A light-weight and flexible data validation and testing tool for dataframes.
 Home-page: https://github.com/pandera-dev/pandera
 Author: Niels Bantilan
 Author-email: niels.bantilan@gmail.com
 License: MIT
 Project-URL: Documentation, https://pandera.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/pandera-dev/pandera/issues
@@ -15,26 +15,29 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: strategies
 Provides-Extra: hypotheses
 Provides-Extra: io
 Provides-Extra: koalas
 Provides-Extra: modin
 Provides-Extra: modin-ray
 Provides-Extra: modin-dask
 Provides-Extra: dask
 Provides-Extra: mypy
+Provides-Extra: fastapi
+Provides-Extra: geopandas
 Provides-Extra: all
 License-File: LICENSE.txt
 
 <br>
 <div align="center"><img src="https://raw.githubusercontent.com/pandera-dev/pandera/master/docs/source/_static/pandera-banner.png" width="400"></div>
 
 <hr>
@@ -113,14 +116,15 @@
 
 Installing additional functionality:
 ```
 pip install pandera[hypotheses]  # hypothesis checks
 pip install pandera[io]          # yaml/script schema io utilities
 pip install pandera[strategies]  # data synthesis strategies
 pip install pandera[mypy]        # enable static type-linting of pandas
+pip install pandera[fastapi]     # fastapi integration
 pip install pandera[dask]        # validate dask dataframes
 pip install pandera[koalas]      # validate koalas dataframes
 pip install pandera[modin]       # validate modin dataframes
 pip install pandera[modin-ray]   # validate modin dataframes with ray
 pip install pandera[modin-dask]  # validate modin dataframes with dask
 pip install pandera[all]         # all packages
 ```
```

### Comparing `pandera-0.8.1/README.md` & `pandera-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 
 Installing additional functionality:
 ```
 pip install pandera[hypotheses]  # hypothesis checks
 pip install pandera[io]          # yaml/script schema io utilities
 pip install pandera[strategies]  # data synthesis strategies
 pip install pandera[mypy]        # enable static type-linting of pandas
+pip install pandera[fastapi]     # fastapi integration
 pip install pandera[dask]        # validate dask dataframes
 pip install pandera[koalas]      # validate koalas dataframes
 pip install pandera[modin]       # validate modin dataframes
 pip install pandera[modin-ray]   # validate modin dataframes with ray
 pip install pandera[modin-dask]  # validate modin dataframes with dask
 pip install pandera[all]         # all packages
 ```
```

### Comparing `pandera-0.8.1/pandera/__init__.py` & `pandera-0.9.0/pandera/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from pandera.engines.numpy_engine import Object
 from pandera.engines.pandas_engine import (
     BOOL,
     INT8,
     INT16,
     INT32,
     INT64,
+    PANDAS_1_2_0_PLUS,
     PANDAS_1_3_0_PLUS,
     STRING,
     UINT8,
     UINT16,
     UINT32,
     UINT64,
 )
```

### Comparing `pandera-0.8.1/pandera/check_utils.py` & `pandera-0.9.0/pandera/check_utils.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/checks.py` & `pandera-0.9.0/pandera/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,16 @@
         groupby: Optional[Union[str, List[str], Callable]] = None,
         ignore_na: bool = True,
         element_wise: bool = False,
         name: str = None,
         error: Optional[str] = None,
         raise_warning: bool = False,
         n_failure_cases: Union[int, None] = constants.N_FAILURE_CASES,
+        title: Optional[str] = None,
+        description: Optional[str] = None,
         **check_kwargs,
     ) -> None:
         """Apply a validation function to each element, Series, or DataFrame.
 
         :param check_fn: A function to check pandas data structure. For Column
             or SeriesSchema checks, if element_wise is True, this function
             should have the signature: ``Callable[[pd.Series],
@@ -169,28 +171,37 @@
             check.
         :param raise_warning: if True, raise a UserWarning and do not throw
             exception instead of raising a SchemaError for a specific check.
             This option should be used carefully in cases where a failing
             check is informational and shouldn't stop execution of the program.
         :param n_failure_cases: report the first n unique failure cases. If
             None, report all failure cases.
+        :param title: A human-readable label for the check.
+        :param description: An arbitrary textual description of the check.
         :param check_kwargs: key-word arguments to pass into ``check_fn``
 
         :example:
 
         >>> import pandas as pd
         >>> import pandera as pa
         >>>
         >>>
         >>> # column checks are vectorized by default
         >>> check_positive = pa.Check(lambda s: s > 0)
         >>>
         >>> # define an element-wise check
         >>> check_even = pa.Check(lambda x: x % 2 == 0, element_wise=True)
         >>>
+        >>> # checks can be given human-readable metadata
+        >>> check_with_metadata = pa.Check(
+        ...     lambda x: True,
+        ...     title="Always passes",
+        ...     description="This check always passes."
+        ... )
+        >>>
         >>> # specify assertions across categorical variables using `groupby`,
         >>> # for example, make sure the mean measure for group "A" is always
         >>> # larger than the mean measure for group "B"
         >>> check_by_group = pa.Check(
         ...     lambda measures: measures["A"].mean() > measures["B"].mean(),
         ...     groupby=["group"],
         ... )
@@ -237,14 +248,16 @@
         self.error = error
         self.name = name or getattr(
             self._check_fn, "__name__", self._check_fn.__class__.__name__
         )
         self.ignore_na = ignore_na
         self.raise_warning = raise_warning
         self.n_failure_cases = n_failure_cases
+        self.title = title
+        self.description = description
 
         if groupby is None and groups is not None:
             raise ValueError(
                 "`groupby` argument needs to be provided when `groups` "
                 "argument is defined"
             )
```

### Comparing `pandera-0.8.1/pandera/decorators.py` & `pandera-0.9.0/pandera/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     Union,
     cast,
     overload,
 )
 
 import pandas as pd
 import wrapt
+from pydantic import validate_arguments
 
 from . import errors, schemas
 from .inspection_utils import (
     is_classmethod_from_meta,
     is_decorated_classmethod,
 )
 from .model import SchemaModel
@@ -93,15 +94,15 @@
     raise errors.SchemaError(
         schema,
         arg_df,
         msg,
         failure_cases=schema_error.failure_cases,
         check=schema_error.check,
         check_index=schema_error.check_index,
-    )
+    ) from schema_error
 
 
 def check_input(
     schema: Schemas,
     obj_getter: Optional[InputGetter] = None,
     head: Optional[int] = None,
     tail: Optional[int] = None,
@@ -480,25 +481,29 @@
 ) -> Callable[[F], F]:
     ...  # pragma: no cover
 
 
 def check_types(
     wrapped=None,
     *,
+    with_pydantic=False,
     head: Optional[int] = None,
     tail: Optional[int] = None,
     sample: Optional[int] = None,
     random_state: Optional[int] = None,
     lazy: bool = False,
     inplace: bool = False,
 ) -> Callable:
     """Validate function inputs and output based on type annotations.
 
     See the :ref:`User Guide <schema_models>` for more.
 
+    :param wrapped: the function to decorate.
+    :param with_pydantic: use ``pydantic.validate_arguments`` to validate
+        inputs. This function is still needed to validate function outputs.
     :param head: validate the first n rows. Rows overlapping with `tail` or
         `sample` are de-duplicated.
     :param tail: validate the last n rows. Rows overlapping with `head` or
         `sample` are de-duplicated.
     :param sample: validate a random sample of n rows. Rows overlapping
         with `head` or `tail` are de-duplicated.
     :param random_state: random seed for the ``sample`` argument.
@@ -508,58 +513,84 @@
     :param inplace: if True, applies coercion to the object of validation,
             otherwise creates a copy of the data.
     """
     # pylint: disable=too-many-locals
     if wrapped is None:
         return functools.partial(
             check_types,
+            with_pydantic=with_pydantic,
             head=head,
             tail=tail,
             sample=sample,
             random_state=random_state,
             lazy=lazy,
             inplace=inplace,
         )
 
     # Front-load annotation parsing
-    annotated_schemas: Dict[str, Tuple[schemas.DataFrameSchema, bool]] = {}
+    annotated_schema_models: Dict[str, Tuple[SchemaModel, AnnotationInfo]] = {}
     for arg_name_, annotation in typing.get_type_hints(wrapped).items():
         annotation_info = AnnotationInfo(annotation)
         if not annotation_info.is_generic_df:
             continue
 
-        schema = cast(SchemaModel, annotation_info.arg).to_schema()
-        annotated_schemas[arg_name_] = (schema, annotation_info.optional)
+        schema_model = cast(SchemaModel, annotation_info.arg)
+        annotated_schema_models[arg_name_] = (schema_model, annotation_info)
 
     def _check_arg(arg_name: str, arg_value: Any) -> Any:
         """
         Validate function's argument if annoted with a schema, else
         pass-through.
         """
-        schema, optional = annotated_schemas.get(arg_name, (None, None))
+        schema_model, annotation_info = annotated_schema_models.get(
+            arg_name, (None, None)
+        )
+
+        if schema_model is None:
+            return arg_value
+
         if (
-            schema
-            and not (optional and arg_value is None)
+            annotation_info
+            and not (annotation_info.optional and arg_value is None)
             # the pandera.schema attribute should only be available when
             # schema.validate has been called in the DF. There's probably
             # a better way of doing this
-            and (
+        ):
+            config = schema_model.__config__
+            data_container_type = annotation_info.origin
+            schema = schema_model.to_schema()
+
+            if data_container_type and config and config.from_format:
+                arg_value = data_container_type.from_format(arg_value, config)
+
+            if (
                 arg_value.pandera.schema is None
+                # don't re-validate a dataframe that contains the same exact
+                # schema
                 or arg_value.pandera.schema != schema
-            )
-        ):
-            try:
-                return schema.validate(
-                    arg_value, head, tail, sample, random_state, lazy, inplace
-                )
-            except errors.SchemaError as e:
-                _handle_schema_error(
-                    "check_types", wrapped, schema, arg_value, e
-                )
-        return arg_value
+            ):
+                try:
+                    arg_value = schema.validate(
+                        arg_value,
+                        head,
+                        tail,
+                        sample,
+                        random_state,
+                        lazy,
+                        inplace,
+                    )
+                except errors.SchemaError as e:
+                    _handle_schema_error(
+                        "check_types", wrapped, schema, arg_value, e
+                    )
+
+            if data_container_type and config and config.to_format:
+                arg_value = data_container_type.to_format(arg_value, config)
+
+            return arg_value
 
     sig = inspect.signature(wrapped)
 
     def validate_args(arguments: Dict[str, Any]) -> Dict[str, Any]:
         return {
             arg_name: _check_arg(arg_name, arg_value)
             for arg_name, arg_value in arguments.items()
@@ -591,29 +622,35 @@
         @wrapt.decorator
         async def _wrapper(
             wrapped_: Callable,
             instance: Optional[Any],
             args: Tuple[Any, ...],
             kwargs: Dict[str, Any],
         ):
-            validated_pos, validated_kwd = validate_inputs(
-                instance, args, kwargs
-            )
-            out = await wrapped_(*validated_pos.values(), **validated_kwd)
+            if with_pydantic:
+                out = await validate_arguments(wrapped_)(*args, **kwargs)
+            else:
+                validated_pos, validated_kwd = validate_inputs(
+                    instance, args, kwargs
+                )
+                out = await wrapped_(*validated_pos.values(), **validated_kwd)
             return _check_arg("return", out)
 
     else:
 
         @wrapt.decorator
         def _wrapper(
             wrapped_: Callable,
             instance: Optional[Any],
             args: Tuple[Any, ...],
             kwargs: Dict[str, Any],
         ):
-            validated_pos, validated_kwd = validate_inputs(
-                instance, args, kwargs
-            )
-            out = wrapped_(*validated_pos.values(), **validated_kwd)
+            if with_pydantic:
+                out = validate_arguments(wrapped_)(*args, **kwargs)
+            else:
+                validated_pos, validated_kwd = validate_inputs(
+                    instance, args, kwargs
+                )
+                out = wrapped_(*validated_pos.values(), **validated_kwd)
             return _check_arg("return", out)
 
     return _wrapper(wrapped)  # pylint:disable=no-value-for-parameter
```

### Comparing `pandera-0.8.1/pandera/deprecations.py` & `pandera-0.9.0/pandera/deprecations.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/dtypes.py` & `pandera-0.9.0/pandera/dtypes.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/engines/engine.py` & `pandera-0.9.0/pandera/engines/engine.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/engines/numpy_engine.py` & `pandera-0.9.0/pandera/engines/numpy_engine.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/engines/pandas_engine.py` & `pandera-0.9.0/pandera/engines/pandas_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 def pandas_version():
     """Return the pandas version."""
 
     return version.parse(pd.__version__)
 
 
+PANDAS_1_2_0_PLUS = pandas_version().release >= (1, 2, 0)
 PANDAS_1_3_0_PLUS = pandas_version().release >= (1, 3, 0)
 
 try:
     from typing import Literal  # type: ignore
 except ImportError:
     from typing_extensions import Literal  # type: ignore
 
@@ -350,14 +351,33 @@
 
 _register_numpy_numbers(
     builtin_name="float",
     pandera_name="Float",
     sizes=[128, 64, 32, 16] if FLOAT_128_AVAILABLE else [64, 32, 16],
 )
 
+if PANDAS_1_2_0_PLUS:
+
+    @Engine.register_dtype(equivalents=[pd.Float64Dtype, pd.Float64Dtype()])
+    @immutable
+    class FLOAT64(DataType, dtypes.Float):
+        """Semantic representation of a :class:`pandas.Float64Dtype`."""
+
+        type = pd.Float64Dtype()
+        bit_width: int = 64
+
+    @Engine.register_dtype(equivalents=[pd.Float32Dtype, pd.Float32Dtype()])
+    @immutable
+    class FLOAT32(FLOAT64):
+        """Semantic representation of a :class:`pandas.Float32Dtype`."""
+
+        type = pd.Float32Dtype()
+        bit_width: int = 32
+
+
 # ###############################################################################
 # # complex
 # ###############################################################################
 
 _register_numpy_numbers(
     builtin_name="complex",
     pandera_name="Complex",
@@ -653,14 +673,39 @@
     @classmethod
     def from_parametrized_dtype(cls, pd_dtype: pd.IntervalDtype):
         """Convert a :class:`pandas.IntervalDtype` to
         a Pandera :class:`pandera.engines.pandas_engine.Interval`."""
         return cls(subtype=pd_dtype.subtype)  # type: ignore
 
 
+# ###############################################################################
+# # geopandas
+# ###############################################################################
+
+try:
+    import geopandas as gpd
+
+    GEOPANDAS_INSTALLED = True
+except ImportError:  # pragma: no cover
+    GEOPANDAS_INSTALLED = False
+
+if GEOPANDAS_INSTALLED:
+
+    @Engine.register_dtype(
+        equivalents=[
+            "geometry",
+            gpd.array.GeometryDtype,
+            gpd.array.GeometryDtype(),
+        ]
+    )
+    @dtypes.immutable
+    class Geometry(DataType):
+        type = gpd.array.GeometryDtype()
+
+
 class PandasDtype(Enum):
     # pylint: disable=line-too-long,invalid-name
     """Enumerate all valid pandas data types.
 
     This class simply enumerates the valid numpy dtypes for pandas arrays.
     For convenience ``PandasDtype`` enums can all be accessed in the top-level
     ``pandera`` name space via the same enum name.
@@ -720,14 +765,16 @@
 
     # pandas data types
     Category = "category"  #: pandas ``"categorical"`` datatype
     INT8 = "Int8"  #: ``"Int8"`` pandas dtype:: pandas 0.24.0+
     INT16 = "Int16"  #: ``"Int16"`` pandas dtype: pandas 0.24.0+
     INT32 = "Int32"  #: ``"Int32"`` pandas dtype: pandas 0.24.0+
     INT64 = "Int64"  #: ``"Int64"`` pandas dtype: pandas 0.24.0+
+    FLOAT32 = "Float32"  #: ``"Float32"`` pandas dtype: pandas 1.2.0+
+    FLOAT64 = "Float64"  #: ``"Float64"`` pandas dtype: pandas 1.2.0+
     UINT8 = "UInt8"  #: ``"UInt8"`` pandas dtype: pandas 0.24.0+
     UINT16 = "UInt16"  #: ``"UInt16"`` pandas dtype: pandas 0.24.0+
     UINT32 = "UInt32"  #: ``"UInt32"`` pandas dtype: pandas 0.24.0+
     UINT64 = "UInt64"  #: ``"UInt64"`` pandas dtype: pandas 0.24.0+
     String = "str"  #: ``"str"`` numpy dtype
 
     #: ``"string"`` pandas dtypes: pandas 1.0.0+. For <1.0.0, this enum will
```

### Comparing `pandera-0.8.1/pandera/engines/utils.py` & `pandera-0.9.0/pandera/engines/utils.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/error_formatters.py` & `pandera-0.9.0/pandera/error_formatters.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,21 +114,16 @@
                 index=lambda df: (
                     df.index.to_frame().apply(tuple, axis=1).astype(str)
                 )
             )[["failure_case", "index"]]
             .reset_index(drop=True)
         )
     elif check_utils.is_table(failure_cases):
-        reshaped_failure_cases = (
-            failure_cases.rename_axis("column", axis=1)
-            .rename_axis("index", axis=0)
-            .unstack()
-            .rename("failure_case")
-            .reset_index()
-        )
+        reshaped_failure_cases = failure_cases.unstack().reset_index()
+        reshaped_failure_cases.columns = ["column", "index", "failure_case"]
     elif check_utils.is_field(failure_cases):
         reshaped_failure_cases = failure_cases.rename("failure_case")
         reshaped_failure_cases.index.name = "index"
         reshaped_failure_cases = reshaped_failure_cases.reset_index()
     else:
         raise TypeError(
             "type of failure_cases argument not understood: "
```

### Comparing `pandera-0.8.1/pandera/error_handlers.py` & `pandera-0.9.0/pandera/error_handlers.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/errors.py` & `pandera-0.9.0/pandera/errors.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/extensions.py` & `pandera-0.9.0/pandera/extensions.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/external_config.py` & `pandera-0.9.0/pandera/external_config.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/hypotheses.py` & `pandera-0.9.0/pandera/hypotheses.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/inspection_utils.py` & `pandera-0.9.0/pandera/inspection_utils.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/io.py` & `pandera-0.9.0/pandera/io.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/model.py` & `pandera-0.9.0/pandera/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Class-based api"""
+
 import inspect
 import os
 import re
 import sys
 import typing
 from typing import (
     Any,
@@ -21,25 +22,27 @@
 
 import pandas as pd
 
 from . import schema_components
 from . import strategies as st
 from .checks import Check
 from .errors import SchemaInitError
+from .json_schema import to_json_schema
 from .model_components import (
     CHECK_KEY,
     DATAFRAME_CHECK_KEY,
     CheckInfo,
     Field,
     FieldCheckInfo,
     FieldInfo,
 )
 from .schemas import DataFrameSchema
 from .typing import INDEX_TYPES, SERIES_TYPES, AnnotationInfo
 from .typing.common import DataFrameBase
+from .typing.config import BaseConfig
 
 if sys.version_info[:2] < (3, 9):
     from typing_extensions import get_type_hints
 else:
     from typing import get_type_hints
 
 try:
@@ -65,44 +68,14 @@
 
     def decorator(func: F) -> F:
         return cast(F, pd.util.Substitution(*args, **kwargs)(func))
 
     return decorator
 
 
-class BaseConfig:  # pylint:disable=R0903
-    """Define DataFrameSchema-wide options.
-
-    *new in 0.5.0*
-    """
-
-    name: Optional[str] = None  #: name of schema
-    coerce: bool = False  #: coerce types of all schema components
-
-    #: make sure certain column combinations are unique
-    unique: Optional[Union[str, List[str]]] = None
-
-    #: make sure all specified columns are in the validated dataframe -
-    #: if ``"filter"``, removes columns not specified in the schema
-    strict: Union[bool, str] = False
-
-    ordered: bool = False  #: validate columns order
-    multiindex_name: Optional[str] = None  #: name of multiindex
-
-    #: coerce types of all MultiIndex components
-    multiindex_coerce: bool = False
-
-    #: make sure all specified columns are in validated MultiIndex -
-    #: if ``"filter"``, removes indexes not specified in the schema
-    multiindex_strict: bool = False
-
-    #: validate MultiIndex in order
-    multiindex_ordered: bool = True
-
-
 def _is_field(name: str) -> bool:
     """Ignore private and reserved keywords."""
     return not name.startswith("_") and name != _CONFIG_KEY
 
 
 _config_options = [attr for attr in vars(BaseConfig) if _is_field(attr)]
 
@@ -162,14 +135,15 @@
 
     *new in 0.5.0*
 
     See the :ref:`User Guide <schema_models>` for more.
     """
 
     Config: Type[BaseConfig] = BaseConfig
+    __extras__: Optional[Dict[str, Any]] = None
     __schema__: Optional[DataFrameSchema] = None
     __config__: Optional[Type[BaseConfig]] = None
 
     #: Key according to `FieldInfo.name`
     __fields__: Dict[str, Tuple[AnnotationInfo, FieldInfo]] = {}
     __checks__: Dict[str, List[Check]] = {}
     __dataframe_checks__: List[Check] = []
@@ -188,21 +162,22 @@
         for field_name in subclass_annotations.keys():
             if _is_field(field_name) and field_name not in cls.__dict__:
                 # Field omitted
                 field = Field()
                 field.__set_name__(cls, field_name)
                 setattr(cls, field_name, field)
 
+        cls.__config__, cls.__extras__ = cls._collect_config_and_extras()
+
     @classmethod
     def to_schema(cls) -> DataFrameSchema:
         """Create :class:`~pandera.DataFrameSchema` from the :class:`.SchemaModel`."""
         if cls in MODEL_CACHE:
             return MODEL_CACHE[cls]
 
-        cls.__config__, extras = cls._collect_config_and_extras()
         mi_kwargs = {
             name[len("multiindex_") :]: value
             for name, value in vars(cls.__config__).items()
             if name.startswith("multiindex_")
         }
 
         cls.__fields__ = cls._collect_fields()
@@ -212,29 +187,38 @@
 
         cls.__checks__ = cls._extract_checks(
             check_infos, field_names=list(cls.__fields__.keys())
         )
 
         df_check_infos = cls._collect_check_infos(DATAFRAME_CHECK_KEY)
         df_custom_checks = cls._extract_df_checks(df_check_infos)
-        df_registered_checks = _convert_extras_to_checks(extras)
+        df_registered_checks = _convert_extras_to_checks(
+            {} if cls.__extras__ is None else cls.__extras__
+        )
         cls.__dataframe_checks__ = df_custom_checks + df_registered_checks
 
         columns, index = cls._build_columns_index(
             cls.__fields__, cls.__checks__, **mi_kwargs
         )
+        kwargs = {}
+        if cls.__config__ is not None:
+            kwargs = {
+                "coerce": cls.__config__.coerce,
+                "strict": cls.__config__.strict,
+                "name": cls.__config__.name,
+                "ordered": cls.__config__.ordered,
+                "unique": cls.__config__.unique,
+                "title": cls.__config__.title,
+                "description": cls.__config__.description or cls.__doc__,
+            }
         cls.__schema__ = DataFrameSchema(
             columns,
             index=index,
             checks=cls.__dataframe_checks__,  # type: ignore
-            coerce=cls.__config__.coerce,
-            strict=cls.__config__.strict,
-            name=cls.__config__.name,
-            ordered=cls.__config__.ordered,
-            unique=cls.__config__.unique,
+            **kwargs,
         )
         if cls not in MODEL_CACHE:
             MODEL_CACHE[cls] = cls.__schema__  # type: ignore
         return cls.__schema__  # type: ignore
 
     @classmethod
     def to_yaml(cls, stream: Optional[os.PathLike] = None):
@@ -262,17 +246,15 @@
                 check_obj, head, tail, sample, random_state, lazy, inplace
             ),
         )
 
     @classmethod
     @docstring_substitution(strategy_doc=DataFrameSchema.strategy.__doc__)
     @st.strategy_import_error
-    def strategy(
-        cls: Type[TSchemaModel], *, size: Optional[int] = None
-    ) -> DataFrameBase[TSchemaModel]:
+    def strategy(cls: Type[TSchemaModel], *, size: Optional[int] = None):
         """%(strategy_doc)s"""
         return cls.to_schema().strategy(size=size)
 
     @classmethod
     @docstring_substitution(example_doc=DataFrameSchema.strategy.__doc__)
     @st.strategy_import_error
     def example(
@@ -310,14 +292,16 @@
                     raise TypeError(
                         "Cannot specify redundant 'dtype_kwargs' "
                         + f"for {annotation.raw_annotation}."
                         + "\n Usage Tip: Drop 'typing.Annotated'."
                     )
                 dtype_kwargs = _get_dtype_kwargs(annotation)
                 dtype = annotation.arg(**dtype_kwargs)  # type: ignore
+            elif annotation.default_dtype:
+                dtype = annotation.default_dtype
             else:
                 dtype = annotation.arg
 
             dtype = None if dtype is Any else dtype
 
             if (
                 annotation.origin in SERIES_TYPES
@@ -508,14 +492,19 @@
                 "SchemaModel cannot be converted to a DataFrameSchema.\n"
                 f"Please revisit the model to address the following errors:"
                 f"\n{exc}"
             ) from exc
 
         return cast("SchemaModel", schema_model)
 
+    @classmethod
+    def __modify_schema__(cls, field_schema):
+        """Update pydantic field schema."""
+        field_schema.update(to_json_schema(cls.to_schema()))
+
 
 def _build_schema_index(
     indices: List[schema_components.Index], **multiindex_kwargs: Any
 ) -> Optional[SchemaIndex]:
     index: Optional[SchemaIndex] = None
     if indices:
         if len(indices) == 1:
```

### Comparing `pandera-0.8.1/pandera/model_components.py` & `pandera-0.9.0/pandera/model_components.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,38 +52,44 @@
         "allow_duplicates",
         "coerce",
         "regex",
         "check_name",
         "alias",
         "original_name",
         "dtype_kwargs",
+        "title",
+        "description",
     )
 
     def __init__(
         self,
         checks: Optional[_CheckList] = None,
         nullable: bool = False,
         unique: bool = False,
         allow_duplicates: Optional[bool] = None,
         coerce: bool = False,
         regex: bool = False,
         alias: Any = None,
         check_name: Optional[bool] = None,
         dtype_kwargs: Optional[Dict[str, Any]] = None,
+        title: Optional[str] = None,
+        description: Optional[str] = None,
     ) -> None:
         self.checks = _to_checklist(checks)
         self.nullable = nullable
         self.unique = unique
         self.allow_duplicates = allow_duplicates
         self.coerce = coerce
         self.regex = regex
         self.alias = alias
         self.check_name = check_name
         self.original_name = cast(str, None)  # always set by SchemaModel
         self.dtype_kwargs = dtype_kwargs
+        self.title = title
+        self.description = description
 
     @property
     def name(self) -> str:
         """Return the name of the field used in the DataFrame"""
         if self.alias is not None:
             return self.alias
         return self.original_name
@@ -143,14 +149,16 @@
             unique=self.unique,
             allow_duplicates=self.allow_duplicates,
             coerce=self.coerce,
             regex=self.regex,
             required=required,
             name=name,
             checks=checks,
+            title=self.title,
+            description=self.description,
         )
 
     def to_index(
         self,
         pandas_dtype: PandasDtypeInputTypes,
         checks: _CheckList = None,
         name: str = None,
@@ -161,14 +169,16 @@
             Index,
             nullable=self.nullable,
             unique=self.unique,
             allow_duplicates=self.allow_duplicates,
             coerce=self.coerce,
             name=name,
             checks=checks,
+            title=self.title,
+            description=self.description,
         )
 
 
 def Field(
     *,
     eq: Any = None,
     ne: Any = None,
@@ -191,25 +201,27 @@
     regex: bool = False,
     ignore_na: bool = True,
     raise_warning: bool = False,
     n_failure_cases: int = 10,
     alias: Any = None,
     check_name: Optional[bool] = None,
     dtype_kwargs: Optional[Dict[str, Any]] = None,
+    title: Optional[str] = None,
+    description: Optional[str] = None,
     **kwargs,
 ) -> Any:
     """Used to provide extra information about a field of a SchemaModel.
 
     *new in 0.5.0*
 
     Some arguments apply only to numeric dtypes and some apply only to ``str``.
     See the :ref:`User Guide <schema_models>` for more information.
 
     The keyword-only arguments from ``eq`` to ``str_startswith`` are dispatched
-    to the built-in `~pandera.checks.Check` methods.
+    to the built-in :py:class:`~pandera.checks.Check` methods.
 
     :param nullable: Whether or not the column/index can contain null values.
     :param unique: Whether column values should be unique.
     :param allow_duplicates: Whether or not column can contain duplicate
         values.
 
         .. warning::
@@ -225,14 +237,16 @@
         report all failure cases.
     :param alias: The public name of the column/index.
     :param check_name: Whether to check the name of the column/index during
         validation. `None` is the default behavior, which translates to `True`
         for columns and multi-index, and to `False` for a single index.
     :param dtype_kwargs: The parameters to be forwarded to the type of the
         field.
+    :param title: A human-readable label for the field.
+    :param description: An arbitrary textual description of the field.
     :param kwargs: Specify custom checks that have been registered with the
         :class:`~pandera.extensions.register_check_method` decorator.
     """
     # pylint:disable=C0103,W0613,R0914
     check_kwargs = {
         "ignore_na": ignore_na,
         "raise_warning": raise_warning,
@@ -265,14 +279,16 @@
         nullable=nullable,
         unique=unique,
         allow_duplicates=allow_duplicates,
         coerce=coerce,
         regex=regex,
         check_name=check_name,
         alias=alias,
+        title=title,
+        description=description,
         dtype_kwargs=dtype_kwargs,
     )
 
 
 def _check_dispatch():
     return {
         "eq": Check.equal_to,
@@ -358,14 +374,15 @@
 
     :param _fn: Method to decorate.
     :param check_kwargs: Keywords arguments forwarded to Check.
     """
 
     def _wrapper(fn: Union[classmethod, AnyCallable]) -> classmethod:
         check_fn, check_method = _to_function_and_classmethod(fn)
+        check_kwargs.setdefault("description", fn.__doc__)
         setattr(
             check_method,
             CHECK_KEY,
             FieldCheckInfo(set(fields), check_fn, regex, **check_kwargs),
         )
         return check_method
 
@@ -384,14 +401,15 @@
     more.
 
     :param check_kwargs: Keywords arguments forwarded to Check.
     """
 
     def _wrapper(fn: Union[classmethod, AnyCallable]) -> classmethod:
         check_fn, check_method = _to_function_and_classmethod(fn)
+        check_kwargs.setdefault("description", fn.__doc__)
         setattr(
             check_method,
             DATAFRAME_CHECK_KEY,
             CheckInfo(check_fn, **check_kwargs),
         )
         return check_method
```

### Comparing `pandera-0.8.1/pandera/modin_accessor.py` & `pandera-0.9.0/pandera/modin_accessor.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/mypy.py` & `pandera-0.9.0/pandera/mypy.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/pandas_accessor.py` & `pandera-0.9.0/pandera/pandas_accessor.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/schema_components.py` & `pandera-0.9.0/pandera/schema_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         unique: bool = False,
         allow_duplicates: Optional[bool] = None,
         coerce: bool = False,
         required: bool = True,
         name: Union[str, Tuple[str, ...], None] = None,
         regex: bool = False,
         pandas_dtype: PandasDtypeInputTypes = None,
+        title: Optional[str] = None,
+        description: Optional[str] = None,
     ) -> None:
         """Create column validator object.
 
         :param dtype: datatype of the column. A ``PandasDtype`` for
             type-checking dataframe. If a string is specified, then assumes
             one of the valid pandas string values:
             http://pandas.pydata.org/pandas-docs/stable/basics.html#dtypes
@@ -65,14 +67,17 @@
         :param name: column name in dataframe to validate.
         :param regex: whether the ``name`` attribute should be treated as a
             regex pattern to apply to multiple columns in a dataframe.
         :param pandas_dtype: alias of ``dtype`` for backwards compatibility.
 
             .. warning:: This option will be deprecated in 0.8.0
 
+        :param title: A human-readable label for the column.
+        :param description: An arbitrary textual description of the column.
+
         :raises SchemaInitError: if impossible to build schema from parameters
 
         :example:
 
         >>> import pandas as pd
         >>> import pandera as pa
         >>>
@@ -93,14 +98,16 @@
             checks,
             nullable,
             unique,
             allow_duplicates,
             coerce,
             name,
             pandas_dtype,
+            title,
+            description,
         )
         if (
             name is not None
             and not isinstance(name, str)
             and not _is_valid_multiindex_tuple_str(name)
             and regex
         ):
@@ -129,14 +136,16 @@
             "checks": self._checks,
             "nullable": self._nullable,
             "unique": self._unique,
             "coerce": self._coerce,
             "required": self.required,
             "name": self._name,
             "regex": self._regex,
+            "title": self.title,
+            "description": self.description,
         }
 
     def set_name(self, name: str):
         """Used to set or modify the name of a column object.
 
         :param str name: the name of the column object
```

### Comparing `pandera-0.8.1/pandera/schema_inference.py` & `pandera-0.9.0/pandera/schema_inference.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/schema_statistics.py` & `pandera-0.9.0/pandera/schema_statistics.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/schemas.py` & `pandera-0.9.0/pandera/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,16 @@
         transformer: Callable = None,
         coerce: bool = False,
         strict: Union[bool, str] = False,
         name: Optional[str] = None,
         ordered: bool = False,
         pandas_dtype: PandasDtypeInputTypes = None,
         unique: Optional[Union[str, List[str]]] = None,
+        title: Optional[str] = None,
+        description: Optional[str] = None,
     ) -> None:
         """Initialize DataFrameSchema validator.
 
         :param columns: a dict where keys are column names and values are
             Column objects specifying the datatypes and properties of a
             particular column.
         :type columns: mapping of column names and column schema component.
@@ -132,14 +134,16 @@
         :param name: name of the schema.
         :param ordered: whether or not to validate the columns order.
         :param pandas_dtype: alias of ``dtype`` for backwards compatibility.
 
             .. warning:: This option will be deprecated in 0.8.0
 
         :param unique: a list of columns that should be jointly unique.
+        :param title: A human-readable label for the schema.
+        :param description: An arbitrary textual description of the schema.
 
         :raises SchemaInitError: if impossible to build schema from parameters
         :raises SchemaInitError: if ``dtype`` and ``pandas_dtype`` are both
             supplied.
 
         :examples:
 
@@ -203,14 +207,16 @@
         self.index = index
         self.strict: Union[bool, str] = strict
         self.name: Optional[str] = name
         self.dtype: PandasDtypeInputTypes = dtype or pandas_dtype  # type: ignore
         self._coerce = coerce
         self._ordered = ordered
         self._unique = unique
+        self._title = title
+        self._description = description
         self._validate_schema()
         self._set_column_names()
 
         # this attribute is not meant to be accessed by users and is explicitly
         # set to True in the case that a schema is created by infer_schema.
         self._IS_INFERRED = False
 
@@ -240,14 +246,24 @@
         return self._ordered
 
     @ordered.setter
     def ordered(self, value: bool) -> None:
         """Set ordered attribute"""
         self._ordered = value
 
+    @property
+    def title(self):
+        """A human-readable label for the schema."""
+        return self._title
+
+    @property
+    def description(self):
+        """An arbitrary textual description of the schema."""
+        return self._description
+
     # the _is_inferred getter and setter methods are not public
     @property
     def _is_inferred(self) -> bool:
         return self._IS_INFERRED
 
     @_is_inferred.setter
     def _is_inferred(self, value: bool) -> None:
@@ -689,14 +705,16 @@
                         self, check_index, check, df_to_validate
                     )
                 )
             except errors.SchemaError as err:
                 error_handler.collect_error("dataframe_check", err)
 
         if self.unique:
+            # NOTE: fix this pylint error
+            # pylint: disable=not-an-iterable
             temp_unique: List[List] = (
                 [self.unique]
                 if all(isinstance(x, str) for x in self.unique)
                 else self.unique
             )
             for lst in temp_unique:
                 duplicates = df_to_validate.duplicated(subset=lst, keep=False)
@@ -1411,15 +1429,15 @@
 
         # if there is already an index, append or replace according to
         # parameters
         ind_list: List = (
             []
             if new_schema.index is None or not append
             else list(new_schema.index.indexes)
-            if check_utils.is_multiindex(new_schema.index) and append
+            if isinstance(new_schema.index, MultiIndex) and append
             else [new_schema.index]
         )
 
         for col in keys_temp:
             ind_list.append(
                 Index(
                     dtype=new_schema.columns[col].dtype,
@@ -1616,14 +1634,16 @@
         checks: CheckList = None,
         nullable: bool = False,
         unique: bool = False,
         allow_duplicates: Optional[bool] = None,
         coerce: bool = False,
         name: Any = None,
         pandas_dtype: PandasDtypeInputTypes = None,
+        title: Optional[str] = None,
+        description: Optional[str] = None,
     ) -> None:
         """Initialize series schema base object.
 
         :param dtype: datatype of the column. If a string is specified,
             then assumes one of the valid pandas string values:
             http://pandas.pydata.org/pandas-docs/stable/basics.html#dtypes
         :param checks: If element_wise is True, then callable signature should
@@ -1647,14 +1667,16 @@
             be coerced into the specified dtype. This has no effect on columns
             where ``dtype=None``.
         :param name: column name in dataframe to validate.
         :param pandas_dtype: alias of ``dtype`` for backwards compatibility.
 
             .. warning:: This option will be deprecated in 0.8.0
 
+        :param title: A human-readable label for the series.
+        :param description: An arbitrary textual description of the series.
         :type nullable: bool
         """
         if checks is None:
             checks = []
         if isinstance(checks, (Check, Hypothesis)):
             checks = [checks]
 
@@ -1670,14 +1692,16 @@
 
         self.dtype = dtype or pandas_dtype  # type: ignore
         self._nullable = nullable
         self._coerce = coerce
         self._checks = checks
         self._name = name
         self._unique = unique
+        self._title = title
+        self._description = description
 
         for check in self.checks:
             if check.groupby is not None and not self._allow_groupby:
                 raise errors.SchemaInitError(
                     f"Cannot use groupby checks with type {type(self)}"
                 )
 
@@ -1754,14 +1778,24 @@
 
     @property
     def name(self) -> Union[str, None]:
         """Get SeriesSchema name."""
         return self._name
 
     @property
+    def title(self):
+        """A human-readable label for the series."""
+        return self._title
+
+    @property
+    def description(self):
+        """An arbitrary textual description of the series."""
+        return self._description
+
+    @property
     def dtype(
         self,
     ) -> DataType:
         """Get the pandas dtype"""
         return self._dtype  # type: ignore
 
     @dtype.setter
@@ -2072,14 +2106,16 @@
         index=None,
         nullable: bool = False,
         unique: bool = False,
         allow_duplicates: Optional[bool] = None,
         coerce: bool = False,
         name: str = None,
         pandas_dtype: PandasDtypeInputTypes = None,
+        title: Optional[str] = None,
+        description: Optional[str] = None,
     ) -> None:
         """Initialize series schema base object.
 
         :param dtype: datatype of the column. If a string is specified,
             then assumes one of the valid pandas string values:
             http://pandas.pydata.org/pandas-docs/stable/basics.html#dtypes
         :param checks: If element_wise is True, then callable signature should
@@ -2101,27 +2137,31 @@
             argument instead.
 
         :param coerce: If True, when schema.validate is called the column will
             be coerced into the specified dtype. This has no effect on columns
             where ``pandas_dtype=None``.
         :param name: series name.
         :param pandas_dtype: alias of ``dtype`` for backwards compatibility.
+        :param title: A human-readable label for the series.
+        :param description: An arbitrary textual description of the series.
 
             .. warning:: This option will be deprecated in 0.8.0
 
         """
         super().__init__(
             dtype,
             checks,
             nullable,
             unique,
             allow_duplicates,
             coerce,
             name,
             pandas_dtype,
+            title,
+            description,
         )
         self.index = index
 
     @property
     def _allow_groupby(self) -> bool:
         """Whether the schema or schema component allows groupby operations."""
         return False
```

### Comparing `pandera-0.8.1/pandera/strategies.py` & `pandera-0.9.0/pandera/strategies.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,16 @@
 
 
 def _mask(
     val: Union[pd.Series, pd.Index], null_mask: List[bool]
 ) -> Union[pd.Series, pd.Index]:
     if pd.api.types.is_timedelta64_dtype(val):
         return val.mask(null_mask, pd.NaT)
+    elif val.dtype == pd.StringDtype():
+        return val.mask(null_mask, pd.NA)
     return val.mask(null_mask)
 
 
 @composite
 def null_field_masks(draw, strategy: Optional[SearchStrategy]):
     """Strategy for masking a column/index with null values.
 
@@ -207,16 +209,16 @@
 
     return register_check_strategy_decorator
 
 
 # pylint: disable=line-too-long
 # Values taken from
 # https://hypothesis.readthedocs.io/en/latest/_modules/hypothesis/extra/numpy.html#from_dtype  # noqa
-MIN_DT_VALUE = -(2 ** 63)
-MAX_DT_VALUE = 2 ** 63 - 1
+MIN_DT_VALUE = -(2**63)
+MAX_DT_VALUE = 2**63 - 1
 
 
 def _is_datetime_tz(pandera_dtype: DataType) -> bool:
     native_type = getattr(pandera_dtype, "type", None)
     return isinstance(native_type, pd.DatetimeTZDtype)
```

### Comparing `pandera-0.8.1/pandera/typing/__init__.py` & `pandera-0.9.0/pandera/typing/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Typing module.
 
 For backwards compatibility, pandas types are exposed to the top-level scope of
 the typing module.
 """
 
-from . import dask, koalas, modin
+from . import dask, fastapi, geopandas, koalas, modin
 from .common import (
     BOOL,
     INT8,
     INT16,
     INT32,
     INT64,
     STRING,
@@ -55,12 +55,17 @@
 
 if koalas.KOALAS_INSTALLED:
     DATAFRAME_TYPES.update({koalas.DataFrame})
     SERIES_TYPES.update({koalas.Series})
     INDEX_TYPES.update({koalas.Index})
 
 
+if geopandas.GEOPANDAS_INSTALLED:
+    DATAFRAME_TYPES.update({geopandas.GeoDataFrame})
+    SERIES_TYPES.update({geopandas.GeoSeries})
+
+
 __all__ = [
     "DataFrame",
     "Series",
     "Index",
 ]
```

### Comparing `pandera-0.8.1/pandera/typing/common.py` & `pandera-0.9.0/pandera/typing/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Common typing functionality."""
 # pylint:disable=abstract-method,disable=too-many-ancestors
 
 import inspect
-from typing import TYPE_CHECKING, Any, Generic, Type, TypeVar
+from typing import TYPE_CHECKING, Any, Generic, Optional, Type, TypeVar
 
 import pandas as pd
 import typing_inspect
 
 from .. import dtypes
 from ..engines import numpy_engine, pandas_engine
 
@@ -38,52 +38,98 @@
 Object = numpy_engine.Object  #: ``"object"`` numpy dtype
 String = dtypes.String  #: ``"str"`` numpy dtype
 #: ``"string"`` pandas dtypes: pandas 1.0.0+. For <1.0.0, this enum will
 #: fall back on the str-as-object-array representation.
 STRING = pandas_engine.STRING  #: ``"str"`` numpy dtype
 BOOL = pandas_engine.BOOL  #: ``"str"`` numpy dtype
 
-GenericDtype = TypeVar(  # type: ignore
-    "GenericDtype",
-    bool,
-    int,
-    str,
-    float,
-    pd.core.dtypes.base.ExtensionDtype,
-    Bool,
-    DateTime,
-    Timedelta,
-    Category,
-    Float,
-    Float16,
-    Float32,
-    Float64,
-    Int,
-    Int8,
-    Int16,
-    Int32,
-    Int64,
-    UInt8,
-    UInt16,
-    UInt32,
-    UInt64,
-    INT8,
-    INT16,
-    INT32,
-    INT64,
-    UINT8,
-    UINT16,
-    UINT32,
-    UINT64,
-    Object,
-    String,
-    STRING,
-    BOOL,
-    covariant=True,
-)
+try:
+    Geometry = pandas_engine.Geometry  # : ``"geometry"`` geopandas dtype
+    GEOPANDAS_INSTALLED = True
+except AttributeError:
+    GEOPANDAS_INSTALLED = False
+
+if GEOPANDAS_INSTALLED:
+    GenericDtype = TypeVar(  # type: ignore
+        "GenericDtype",
+        bool,
+        int,
+        str,
+        float,
+        pd.core.dtypes.base.ExtensionDtype,
+        Bool,
+        DateTime,
+        Timedelta,
+        Category,
+        Float,
+        Float16,
+        Float32,
+        Float64,
+        Int,
+        Int8,
+        Int16,
+        Int32,
+        Int64,
+        UInt8,
+        UInt16,
+        UInt32,
+        UInt64,
+        INT8,
+        INT16,
+        INT32,
+        INT64,
+        UINT8,
+        UINT16,
+        UINT32,
+        UINT64,
+        Object,
+        String,
+        STRING,
+        Geometry,
+        covariant=True,
+    )
+else:
+    GenericDtype = TypeVar(  # type: ignore
+        "GenericDtype",
+        bool,
+        int,
+        str,
+        float,
+        pd.core.dtypes.base.ExtensionDtype,
+        Bool,
+        DateTime,
+        Timedelta,
+        Category,
+        Float,
+        Float16,
+        Float32,
+        Float64,
+        Int,
+        Int8,
+        Int16,
+        Int32,
+        Int64,
+        UInt8,
+        UInt16,
+        UInt32,
+        UInt64,
+        INT8,
+        INT16,
+        INT32,
+        INT64,
+        UINT8,
+        UINT16,
+        UINT32,
+        UINT64,
+        Object,
+        String,
+        STRING,
+        covariant=True,
+    )
+
 Schema = TypeVar("Schema", bound="SchemaModel")  # type: ignore
 
 
 # pylint:disable=invalid-name
 if TYPE_CHECKING:
     T = TypeVar("T")  # pragma: no cover
 else:
@@ -93,14 +139,16 @@
 class DataFrameBase(Generic[T]):
     # pylint: disable=too-few-public-methods
     """
     Pandera Dataframe base class for validating dataframes on
     initialization.
     """
 
+    default_dtype: Optional[Type] = None
+
     def __setattr__(self, name: str, value: Any) -> None:
         # pylint: disable=no-member
         object.__setattr__(self, name, value)
         if name == "__orig_class__":
             orig_class = getattr(self, "__orig_class__")
             class_args = getattr(orig_class, "__args__", None)
             if class_args is not None and any(
@@ -121,22 +169,36 @@
                 pandera.add_schema(schema_model.to_schema())
 
 
 # pylint:disable=too-few-public-methods
 class SeriesBase(Generic[GenericDtype]):
     """Pandera Series base class to use for all pandas-like APIs."""
 
+    default_dtype: Optional[Type] = None
+
+    def __get__(
+        self, instance: object, owner: Type
+    ) -> str:  # pragma: no cover
+        raise AttributeError("Series should resolve to Field-s")
+
 
 # pylint:disable=too-few-public-methods
 class IndexBase(Generic[GenericDtype]):
     """Representation of pandas.Index, only used for type annotation.
 
     *new in 0.5.0*
     """
 
+    default_dtype: Optional[Type] = None
+
+    def __get__(
+        self, instance: object, owner: Type
+    ) -> str:  # pragma: no cover
+        raise AttributeError("Indexes should resolve to pa.Index-s")
+
 
 class AnnotationInfo:  # pylint:disable=too-few-public-methods
     """Captures extra information about an annotation.
 
     Attributes:
         origin: The non-parameterized generic class.
         arg: The first generic type (SchemaModel does not support more than
@@ -183,7 +245,9 @@
         self.metadata = getattr(self.arg, "__metadata__", None)
         if self.metadata:
             self.arg = typing_inspect.get_args(self.arg)[0]
 
         self.literal = typing_inspect.is_literal_type(self.arg)
         if self.literal:
             self.arg = typing_inspect.get_args(self.arg)[0]
+
+        self.default_dtype = getattr(raw_annotation, "default_dtype", None)
```

### Comparing `pandera-0.8.1/pandera/typing/dask.py` & `pandera-0.9.0/pandera/typing/dask.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/typing/koalas.py` & `pandera-0.9.0/pandera/typing/koalas.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera/typing/modin.py` & `pandera-0.9.0/pandera/typing/modin.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/pandera.egg-info/PKG-INFO` & `pandera-0.9.0/pandera.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandera
-Version: 0.8.1
+Version: 0.9.0
 Summary: A light-weight and flexible data validation and testing tool for dataframes.
 Home-page: https://github.com/pandera-dev/pandera
 Author: Niels Bantilan
 Author-email: niels.bantilan@gmail.com
 License: MIT
 Project-URL: Documentation, https://pandera.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/pandera-dev/pandera/issues
@@ -15,26 +15,29 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: strategies
 Provides-Extra: hypotheses
 Provides-Extra: io
 Provides-Extra: koalas
 Provides-Extra: modin
 Provides-Extra: modin-ray
 Provides-Extra: modin-dask
 Provides-Extra: dask
 Provides-Extra: mypy
+Provides-Extra: fastapi
+Provides-Extra: geopandas
 Provides-Extra: all
 License-File: LICENSE.txt
 
 <br>
 <div align="center"><img src="https://raw.githubusercontent.com/pandera-dev/pandera/master/docs/source/_static/pandera-banner.png" width="400"></div>
 
 <hr>
@@ -113,14 +116,15 @@
 
 Installing additional functionality:
 ```
 pip install pandera[hypotheses]  # hypothesis checks
 pip install pandera[io]          # yaml/script schema io utilities
 pip install pandera[strategies]  # data synthesis strategies
 pip install pandera[mypy]        # enable static type-linting of pandas
+pip install pandera[fastapi]     # fastapi integration
 pip install pandera[dask]        # validate dask dataframes
 pip install pandera[koalas]      # validate koalas dataframes
 pip install pandera[modin]       # validate modin dataframes
 pip install pandera[modin-ray]   # validate modin dataframes with ray
 pip install pandera[modin-dask]  # validate modin dataframes with dask
 pip install pandera[all]         # all packages
 ```
```

### Comparing `pandera-0.8.1/pandera.egg-info/SOURCES.txt` & `pandera-0.9.0/pandera.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 pandera/error_handlers.py
 pandera/errors.py
 pandera/extensions.py
 pandera/external_config.py
 pandera/hypotheses.py
 pandera/inspection_utils.py
 pandera/io.py
+pandera/json_schema.py
 pandera/koalas_accessor.py
 pandera/model.py
 pandera/model_components.py
 pandera/modin_accessor.py
 pandera/mypy.py
 pandera/pandas_accessor.py
 pandera/py.typed
@@ -42,15 +43,19 @@
 pandera/engines/engine.py
 pandera/engines/numpy_engine.py
 pandera/engines/pandas_engine.py
 pandera/engines/type_aliases.py
 pandera/engines/utils.py
 pandera/typing/__init__.py
 pandera/typing/common.py
+pandera/typing/config.py
 pandera/typing/dask.py
+pandera/typing/fastapi.py
+pandera/typing/formats.py
+pandera/typing/geopandas.py
 pandera/typing/koalas.py
 pandera/typing/modin.py
 pandera/typing/pandas.py
 tests/__init__.py
 tests/conftest.py
 tests/test_inspection_utils.py
 tests/core/__init__.py
```

### Comparing `pandera-0.8.1/setup.py` & `pandera-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,18 @@
     "io": ["pyyaml >= 5.1", "black", "frictionless"],
     "koalas": ["koalas", "pyspark"],
     "modin": ["modin", "ray <= 1.7.0", "dask"],
     "modin-ray": ["modin", "ray <= 1.7.0"],
     "modin-dask": ["modin", "dask"],
     "dask": ["dask"],
     "mypy": ["pandas-stubs"],
+    "fastapi": ["fastapi"],
+    "geopandas": ["geopandas", "shapely"],
 }
+
 extras_require = {
     **_extras_require,
     "all": list(set(x for y in _extras_require.values() for x in y)),
 }
 
 setup(
     name="pandera",
@@ -35,21 +38,22 @@
     project_urls={
         "Documentation": "https://pandera.readthedocs.io",
         "Issue Tracker": "https://github.com/pandera-dev/pandera/issues",
     },
     keywords=["pandas", "validation", "data-structures"],
     license="MIT",
     data_files=[("", ["LICENSE.txt"])],
-    packages=find_packages(),
+    packages=find_packages(include=["pandera*"]),
     package_data={"pandera": ["py.typed"]},
     install_requires=[
         "packaging >= 20.0",
         "numpy >= 1.9.0",
         "pandas >= 1.0",
-        "typing_extensions >= 3.7.4.3 ; python_version<'3.8'",
+        "pydantic",
+        "typing_extensions >= 3.7.4.3; python_version<'3.8'",
         "typing_inspect >= 0.6.0",
         "wrapt",
         "pyarrow",
     ],
     extras_require=extras_require,
     python_requires=">=3.7",
     platforms="any",
@@ -59,10 +63,11 @@
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering",
     ],
 )
```

### Comparing `pandera-0.8.1/tests/conftest.py` & `pandera-0.9.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,10 +12,10 @@
     HAS_HYPOTHESIS = True
 
 # ignore test files associated with hypothesis strategies
 collect_ignore = []
 if not HAS_HYPOTHESIS:
     collect_ignore.append("test_strategies.py")
 else:
-    settings.register_profile("ci", max_examples=100, deadline=None)
+    settings.register_profile("ci", max_examples=20, deadline=None)
     settings.register_profile("dev", max_examples=10, deadline=None)
     settings.load_profile(os.getenv("HYPOTHESIS_PROFILE", "dev"))
```

### Comparing `pandera-0.8.1/tests/core/checks_fixtures.py` & `pandera-0.9.0/tests/core/checks_fixtures.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/core/test_checks.py` & `pandera-0.9.0/tests/core/test_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -424,7 +424,37 @@
     schema_check_return_series = DataFrameSchema(
         checks=Check(lambda df: df[0] < 10)
     )
     assert isinstance(schema_check_return_series.validate(data), pd.DataFrame)
 
     schema_check_return_df = DataFrameSchema(checks=Check(lambda df: df < 10))
     assert isinstance(schema_check_return_df.validate(data), pd.DataFrame)
+
+
+def test_dataframe_check_schema_error() -> None:
+    """Test that DataFramSchema-level checks raises errors."""
+
+    schema = DataFrameSchema(
+        checks=Check(
+            lambda df: df["a"].isna() | ~df["b"].isna(), ignore_na=False
+        )
+    )
+    df = pd.DataFrame(
+        {
+            "a": [1, 2, 3, 1],
+            "b": [1, 2, None, None],
+        }
+    )
+
+    try:
+        schema(df, lazy=True)
+    except errors.SchemaErrors as exc:
+        assert pd.isna(
+            exc.failure_cases.query(
+                "index == 2 & column == 'b'"
+            ).failure_case.iloc[0]
+        )
+        assert pd.isna(
+            exc.failure_cases.query(
+                "index == 3 & column == 'b'"
+            ).failure_case.iloc[0]
+        )
```

### Comparing `pandera-0.8.1/tests/core/test_checks_builtin.py` & `pandera-0.9.0/tests/core/test_checks_builtin.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/core/test_decorators.py` & `pandera-0.9.0/tests/core/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/core/test_deprecations.py` & `pandera-0.9.0/tests/core/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/core/test_docs_setting_column_widths.py` & `pandera-0.9.0/tests/core/test_docs_setting_column_widths.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/core/test_dtypes.py` & `pandera-0.9.0/tests/core/test_dtypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,28 +19,29 @@
 import pandera as pa
 from pandera.engines import pandas_engine
 from pandera.system import FLOAT_128_AVAILABLE
 
 # List dtype classes and associated pandas alias,
 # except for parameterizable dtypes that should also list examples of
 # instances.
+from pandera.typing.geopandas import GEOPANDAS_INSTALLED
+
 int_dtypes = {
     int: "int64",
     pa.Int: "int64",
     pa.Int8: "int8",
     pa.Int16: "int16",
     pa.Int32: "int32",
     pa.Int64: "int64",
     np.int8: "int8",
     np.int16: "int16",
     np.int32: "int32",
     np.int64: "int64",
 }
 
-
 nullable_int_dtypes = {
     pandas_engine.INT8: "Int8",
     pandas_engine.INT16: "Int16",
     pandas_engine.INT32: "Int32",
     pandas_engine.INT64: "Int64",
 }
 
@@ -70,37 +71,42 @@
     pa.Float32: "float32",
     pa.Float64: "float64",
     np.float16: "float16",
     np.float32: "float32",
     np.float64: "float64",
 }
 
-
 complex_dtypes = {
     complex: "complex",
     pa.Complex: "complex128",
     pa.Complex64: "complex64",
     pa.Complex128: "complex128",
 }
 
-
 if FLOAT_128_AVAILABLE:
     float_dtypes.update(
         {
             pa.Float128: "float128",
             np.float128: "float128",
         }
     )
     complex_dtypes.update(
         {
             pa.Complex256: "complex256",
             np.complex256: "complex256",
         }
     )
 
+NULLABLE_FLOAT_DTYPES = None
+if pa.PANDAS_1_2_0_PLUS:
+    NULLABLE_FLOAT_DTYPES = {
+        pandas_engine.FLOAT32: "Float32",
+        pandas_engine.FLOAT64: "Float64",
+    }
+
 boolean_dtypes = {bool: "bool", pa.Bool: "bool", np.bool_: "bool"}
 nullable_boolean_dtypes = {pd.BooleanDtype: "boolean", pa.BOOL: "boolean"}
 
 string_dtypes = {
     str: "str",
     pa.String: "str",
     np.str_: "str",
@@ -150,14 +156,19 @@
 
 dtype_fixtures: List[Tuple[Dict, List]] = [
     (int_dtypes, [-1]),
     (nullable_int_dtypes, [-1, None]),
     (uint_dtypes, [1]),
     (nullable_uint_dtypes, [1, None]),
     (float_dtypes, [1.0]),
+    *(
+        []
+        if NULLABLE_FLOAT_DTYPES is None
+        else [(NULLABLE_FLOAT_DTYPES, [1.0, None])]
+    ),
     (complex_dtypes, [complex(1)]),
     (boolean_dtypes, [True, False]),
     (nullable_boolean_dtypes, [True, None]),
     (string_dtypes, ["A", "B"]),
     (object_dtypes, ["A", "B"]),
     (nullable_string_dtypes, [1, 2, None]),
     (category_dtypes, [1, 2, None]),
@@ -172,14 +183,26 @@
         .to_series(),
     ),
     (sparse_dtypes, pd.Series([1, None], dtype=pd.SparseDtype(float))),
     (interval_dtypes, pd.interval_range(-10.0, 10.0).to_series()),
 ]
 
 
+if GEOPANDAS_INSTALLED:
+    from shapely.geometry import Polygon
+
+    # pylint:disable=ungrouped-imports
+    from pandera.engines.pandas_engine import Geometry
+
+    geometry_dtypes = {Geometry: "geometry"}
+    dtype_fixtures.append(
+        (geometry_dtypes, [Polygon(((0, 0), (0, 1), (1, 1)))])
+    )
+
+
 def pretty_param(*values: Any, **kw: Any) -> ParameterSet:
     """Return a pytest parameter with a human-readable id."""
     id_ = kw.pop("id", None)
     if not id_:
         id_ = "-".join(
             f"{val.__module__}.{val.__name__}"
             if inspect.isclass(val)
@@ -320,20 +343,24 @@
     int_dtypes,
     uint_dtypes,
     float_dtypes,
     complex_dtypes,
     boolean_dtypes,
 )
 
+
 nullable_numeric_dtypes = _flatten_dtypesdict(
     nullable_int_dtypes,
     nullable_uint_dtypes,
+    NULLABLE_FLOAT_DTYPES,
     nullable_boolean_dtypes,
+    *([NULLABLE_FLOAT_DTYPES] if NULLABLE_FLOAT_DTYPES else []),
 )
 
+
 nominal_dtypes = _flatten_dtypesdict(
     string_dtypes,
     nullable_string_dtypes,
     category_dtypes,
 )
 
 
@@ -501,15 +528,22 @@
     """Test is_uint."""
     pandera_dtype = pandas_engine.Engine.dtype(uint_dtype)
     assert pa.dtypes.is_uint(pandera_dtype) == expected
 
 
 @pytest.mark.parametrize(
     "float_dtype, expected",
-    [(dtype, True) for dtype in float_dtypes] + [("string", False)],  # type: ignore
+    [
+        (dtype, True)
+        for dtype in (
+            *float_dtypes,
+            *(NULLABLE_FLOAT_DTYPES if NULLABLE_FLOAT_DTYPES else []),
+        )
+    ]
+    + [("string", False)],  # type: ignore
 )
 def test_is_float(float_dtype: Any, expected: bool):
     """Test is_float."""
     pandera_dtype = pandas_engine.Engine.dtype(float_dtype)
     assert pa.dtypes.is_float(pandera_dtype) == expected
```

### Comparing `pandera-0.8.1/tests/core/test_engine.py` & `pandera-0.9.0/tests/core/test_engine.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/core/test_engine_utils.py` & `pandera-0.9.0/tests/core/test_engine_utils.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/core/test_errors.py` & `pandera-0.9.0/tests/core/test_errors.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/core/test_extensions.py` & `pandera-0.9.0/tests/core/test_extensions.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/core/test_model.py` & `pandera-0.9.0/tests/core/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -669,32 +669,45 @@
     class Child(Base):
         b: Series[int]
 
         class Config:
             name = "Child schema"
             strict = True
             multiindex_strict = False
+            description = "foo"
+            title = "bar"
 
     expected = pa.DataFrameSchema(
         columns={"a": pa.Column(int), "b": pa.Column(int)},
         index=pa.MultiIndex(
             [pa.Index(str, name="idx_1"), pa.Index(str, name="idx_2")],
             coerce=True,
             strict=False,
             name="mi",
         ),
         name="Child schema",
         coerce=True,
         strict=True,
         ordered=True,
+        description="foo",
+        title="bar",
     )
 
     assert expected == Child.to_schema()
 
 
+def test_config_docstrings() -> None:
+    class Model(pa.SchemaModel):
+        """foo"""
+
+        a: Series[int]
+
+    assert Model.__doc__ == Model.to_schema().description
+
+
 class Input(pa.SchemaModel):
     a: Series[int]
     b: Series[int]
     idx: Index[str]
 
 
 class Output(Input):
```

### Comparing `pandera-0.8.1/tests/core/test_model_components.py` & `pandera-0.9.0/tests/core/test_model_components.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/core/test_numpy_engine.py` & `pandera-0.9.0/tests/core/test_numpy_engine.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/core/test_pandas_accessor.py` & `pandera-0.9.0/tests/core/test_pandas_accessor.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/core/test_pandas_engine.py` & `pandera-0.9.0/tests/core/test_pandas_engine.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/core/test_pydantic.py` & `pandera-0.9.0/tests/core/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/core/test_schema_components.py` & `pandera-0.9.0/tests/core/test_schema_components.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/core/test_schema_inference.py` & `pandera-0.9.0/tests/core/test_schema_inference.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/core/test_schema_statistics.py` & `pandera-0.9.0/tests/core/test_schema_statistics.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/core/test_schemas.py` & `pandera-0.9.0/tests/core/test_schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1591,25 +1591,33 @@
 @pytest.mark.parametrize("append", [True, False])
 def test_set_index_append(
     append: bool, schema_simple: DataFrameSchema
 ) -> None:
     """
     Test that setting index correctly handles appending to existing index.
     """
-    test_schema = schema_simple.set_index(keys=["col1"], append=append)
-    if append is True:
-        assert isinstance(test_schema.index, MultiIndex)
-        assert list(test_schema.index.columns.keys()) == ["ind0", "col1"]
-        assert (
-            test_schema.index.columns["col1"].dtype
-            == schema_simple.columns["col1"].dtype
-        )
-    else:
-        assert isinstance(test_schema.index, Index)
-        assert test_schema.index.name == "col1"
+
+    expected_index_names = ["ind0"]
+    test_schema = schema_simple
+
+    for key in ["col1", "col2"]:
+        expected_index_names.append(key)
+        test_schema = test_schema.set_index(keys=[key], append=append)
+        if append is True:
+            assert isinstance(test_schema.index, MultiIndex)
+            assert [
+                x.name for x in test_schema.index.indexes
+            ] == expected_index_names
+            assert (
+                test_schema.index.columns[key].dtype
+                == schema_simple.columns[key].dtype
+            )
+        else:
+            assert isinstance(test_schema.index, Index)
+            assert test_schema.index.name == key
 
 
 @pytest.mark.parametrize("drop", [True, False])
 def test_reset_index_drop(drop: bool, schema_simple: DataFrameSchema) -> None:
     """Test that resetting index correctly handles dropping index levels."""
     test_schema = schema_simple.reset_index(drop=drop)
     if drop:
```

### Comparing `pandera-0.8.1/tests/core/test_typing.py` & `pandera-0.9.0/tests/core/test_typing.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/dask/test_dask.py` & `pandera-0.9.0/tests/dask/test_dask.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/dask/test_dask_accessor.py` & `pandera-0.9.0/tests/dask/test_dask_accessor.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/dask/test_dask_not_installed.py` & `pandera-0.9.0/tests/dask/test_dask_not_installed.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/hypotheses/test_hypotheses.py` & `pandera-0.9.0/tests/hypotheses/test_hypotheses.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/io/test_io.py` & `pandera-0.9.0/tests/io/test_io.py`

 * *Files identical despite different names*

### Comparing `pandera-0.8.1/tests/strategies/test_strategies.py` & `pandera-0.9.0/tests/strategies/test_strategies.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,21 @@
 SUPPORTED_DTYPES = set()
 for data_type in pandas_engine.Engine.get_registered_dtypes():
     if (
         # valid hypothesis.strategies.floats <=64
         getattr(data_type, "bit_width", -1) > 64
         or is_category(data_type)
         or data_type in UNSUPPORTED_DTYPE_CLS
+        or (
+            pandas_engine.GEOPANDAS_INSTALLED
+            and data_type == pandas_engine.Geometry
+        )
     ):
         continue
+
     SUPPORTED_DTYPES.add(pandas_engine.Engine.dtype(data_type))
 
 SUPPORTED_DTYPES.add(pandas_engine.Engine.dtype("datetime64[ns, UTC]"))
 
 NUMERIC_DTYPES = [
     data_type for data_type in SUPPORTED_DTYPES if data_type.continuous
 ]
```

### Comparing `pandera-0.8.1/tests/test_inspection_utils.py` & `pandera-0.9.0/tests/test_inspection_utils.py`

 * *Files identical despite different names*

