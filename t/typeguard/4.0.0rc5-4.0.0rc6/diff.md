# Comparing `tmp/typeguard-4.0.0rc5.tar.gz` & `tmp/typeguard-4.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeguard-4.0.0rc5.tar", last modified: Mon May  1 19:38:43 2023, max compression
+gzip compressed data, was "typeguard-4.0.0rc6.tar", last modified: Sun May  7 10:35:57 2023, max compression
```

## Comparing `typeguard-4.0.0rc5.tar` & `typeguard-4.0.0rc6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:43.007793 typeguard-4.0.0rc5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:42.999793 typeguard-4.0.0rc5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:42.999793 typeguard-4.0.0rc5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/.github/ISSUE_TEMPLATE/features_request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:42.999793 typeguard-4.0.0rc5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-01 19:38:43.007793 typeguard-4.0.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:43.003793 typeguard-4.0.0rc5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/docs/extending.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/docs/userguide.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18500 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/docs/versionhistory.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 19:38:43.007793 typeguard-4.0.0rc5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:42.999793 typeguard-4.0.0rc5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:43.003793 typeguard-4.0.0rc5/src/typeguard/
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26071 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_importhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_memo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_suppression.py
--rw-r--r--   0 runner    (1001) docker     (123)    41301 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/src/typeguard/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:43.003793 typeguard-4.0.0rc5/src/typeguard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-01 19:38:42.000000 typeguard-4.0.0rc5/src/typeguard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-01 19:38:42.000000 typeguard-4.0.0rc5/src/typeguard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:38:42.000000 typeguard-4.0.0rc5/src/typeguard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-01 19:38:42.000000 typeguard-4.0.0rc5/src/typeguard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-01 19:38:42.000000 typeguard-4.0.0rc5/src/typeguard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-01 19:38:42.000000 typeguard-4.0.0rc5/src/typeguard.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:43.007793 typeguard-4.0.0rc5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/dummymodule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:38:43.007793 typeguard-4.0.0rc5/tests/mypy/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/mypy/negative.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/mypy/positive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/mypy/test_type_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    31816 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_importhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_instrumentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_suppression.py
--rw-r--r--   0 runner    (1001) docker     (123)    41950 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16646 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_typechecked.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_union_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-01 19:38:29.000000 typeguard-4.0.0rc5/tests/test_warn_on_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.707884 typeguard-4.0.0rc6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.695884 typeguard-4.0.0rc6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.699884 typeguard-4.0.0rc6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/.github/ISSUE_TEMPLATE/features_request.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.699884 typeguard-4.0.0rc6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-07 10:35:57.707884 typeguard-4.0.0rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.699884 typeguard-4.0.0rc6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/docs/extending.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/docs/userguide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/docs/versionhistory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 10:35:57.707884 typeguard-4.0.0rc6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.695884 typeguard-4.0.0rc6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.703884 typeguard-4.0.0rc6/src/typeguard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26071 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_memo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_pytest_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41863 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/src/typeguard/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.703884 typeguard-4.0.0rc6/src/typeguard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-07 10:35:57.000000 typeguard-4.0.0rc6/src/typeguard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-07 10:35:57.000000 typeguard-4.0.0rc6/src/typeguard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 10:35:57.000000 typeguard-4.0.0rc6/src/typeguard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-07 10:35:57.000000 typeguard-4.0.0rc6/src/typeguard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-07 10:35:57.000000 typeguard-4.0.0rc6/src/typeguard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 10:35:57.000000 typeguard-4.0.0rc6/src/typeguard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.707884 typeguard-4.0.0rc6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/dummymodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:35:57.707884 typeguard-4.0.0rc6/tests/mypy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/mypy/negative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/mypy/positive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/mypy/test_type_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31816 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_instrumentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43600 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16646 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_typechecked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_union_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-07 10:35:39.000000 typeguard-4.0.0rc6/tests/test_warn_on_error.py
```

### Comparing `typeguard-4.0.0rc5/.github/ISSUE_TEMPLATE/bug_report.yaml` & `typeguard-4.0.0rc6/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/.github/ISSUE_TEMPLATE/features_request.yaml` & `typeguard-4.0.0rc6/.github/ISSUE_TEMPLATE/features_request.yaml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/.github/workflows/publish.yml` & `typeguard-4.0.0rc6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/.github/workflows/test.yml` & `typeguard-4.0.0rc6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/.pre-commit-config.yaml` & `typeguard-4.0.0rc6/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [ "--fix=lf" ]
       - id: trailing-whitespace
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.262
+    rev: v0.0.263
     hooks:
       - id: ruff
         args: [--fix, --show-fixes]
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
```

### Comparing `typeguard-4.0.0rc5/LICENSE` & `typeguard-4.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/PKG-INFO` & `typeguard-4.0.0rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeguard
-Version: 4.0.0rc5
+Version: 4.0.0rc6
 Summary: Run-time type checker for Python
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://typeguard.readthedocs.io/en/latest/
 Project-URL: Change log, https://typeguard.readthedocs.io/en/latest/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/typeguard
 Project-URL: Issue tracker, https://github.com/agronholm/typeguard/issues
```

### Comparing `typeguard-4.0.0rc5/README.rst` & `typeguard-4.0.0rc6/README.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/docs/api.rst` & `typeguard-4.0.0rc6/docs/api.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/docs/conf.py` & `typeguard-4.0.0rc6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/docs/contributing.rst` & `typeguard-4.0.0rc6/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/docs/extending.rst` & `typeguard-4.0.0rc6/docs/extending.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/docs/features.rst` & `typeguard-4.0.0rc6/docs/features.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/docs/userguide.rst` & `typeguard-4.0.0rc6/docs/userguide.rst`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/docs/versionhistory.rst` & `typeguard-4.0.0rc6/docs/versionhistory.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 Version history
 ===============
 
 This library adheres to `Semantic Versioning 2.0 <https://semver.org/#semantic-versioning-200>`_.
 
+**4.0.0rc6** (2023-05-07)
+
+- Fixed ``@typechecked`` optimization causing compilation of instrumented code to fail
+  when an ``if`` block was left empty by the AST transformer
+  (`#352 <https://github.com/agronholm/typeguard/issues/352>`_)
+- Fixed the AST transformer trying to parse the second argument of ``typing.Annotated``
+  as a forward reference (`#353 <https://github.com/agronholm/typeguard/issues/353>`_)
+
 **4.0.0rc5** (2023-05-01)
 
 - Added ``InstrumentationWarning`` to the public API
 - Changed ``@typechecked`` to skip instrumentation in optimized mode, as in typeguard
   2.x
 - Avoid type checks where the types in question are shadowed by local variables
 - Fixed instrumentation using ``typing.Optional`` without a subscript when the subscript
```

### Comparing `typeguard-4.0.0rc5/pyproject.toml` & `typeguard-4.0.0rc6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/src/typeguard/__init__.py` & `typeguard-4.0.0rc6/src/typeguard/__init__.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/src/typeguard/_checkers.py` & `typeguard-4.0.0rc6/src/typeguard/_checkers.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/src/typeguard/_config.py` & `typeguard-4.0.0rc6/src/typeguard/_config.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/src/typeguard/_decorators.py` & `typeguard-4.0.0rc6/src/typeguard/_decorators.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/src/typeguard/_exceptions.py` & `typeguard-4.0.0rc6/src/typeguard/_exceptions.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/src/typeguard/_functions.py` & `typeguard-4.0.0rc6/src/typeguard/_functions.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/src/typeguard/_importhook.py` & `typeguard-4.0.0rc6/src/typeguard/_importhook.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/src/typeguard/_memo.py` & `typeguard-4.0.0rc6/src/typeguard/_memo.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/src/typeguard/_pytest_plugin.py` & `typeguard-4.0.0rc6/src/typeguard/_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/src/typeguard/_suppression.py` & `typeguard-4.0.0rc6/src/typeguard/_suppression.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/src/typeguard/_transformer.py` & `typeguard-4.0.0rc6/src/typeguard/_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,18 @@
     "typing.Any",
     "typing_extensions.Any",
 )
 literal_names = (
     "typing.Literal",
     "typing_extensions.Literal",
 )
+annotated_names = (
+    "typing.Annotated",
+    "typing_extensions.Annotated",
+)
 ignore_decorators = (
     "typing.no_type_check",
     "typeguard.typeguard_ignore",
 )
 aug_assign_functions = {
     Add: "iadd",
     Sub: "isub",
@@ -384,15 +388,20 @@
             if isinstance(node.slice, Index):
                 # Python 3.7 and 3.8
                 slice_value = node.slice.value  # type: ignore[attr-defined]
             else:
                 slice_value = node.slice
 
             if isinstance(slice_value, Tuple):
-                items = [self.visit(item) for item in slice_value.elts]
+                if self._memo.name_matches(node.value, *annotated_names):
+                    # Only treat the first argument to typing.Annotated as a potential
+                    # forward reference
+                    items = [self.visit(slice_value.elts[0])] + slice_value.elts[1:]
+                else:
+                    items = [self.visit(item) for item in slice_value.elts]
 
                 # If this is a Union and any of the items is None, erase the entire
                 # annotation
                 if self._memo.name_matches(node.value, "typing.Union") and any(
                     item is None for item in items
                 ):
                     return None
@@ -1123,14 +1132,20 @@
     def visit_If(self, node: If) -> Any:
         """
         This blocks names from being collected from a module-level
         "if typing.TYPE_CHECKING:" block, so that they won't be type checked.
 
         """
         self.generic_visit(node)
+
+        # Fix empty node body (caused by removal of classes/functions not on the target
+        # path)
+        if not node.body:
+            node.body.append(Pass())
+
         if (
             self._memo is self._module_memo
             and isinstance(node.test, Name)
             and self._memo.name_matches(node.test, "typing.TYPE_CHECKING")
         ):
             collector = NameCollector()
             collector.visit(node)
```

### Comparing `typeguard-4.0.0rc5/src/typeguard/_union_transformer.py` & `typeguard-4.0.0rc6/src/typeguard/_union_transformer.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/src/typeguard/_utils.py` & `typeguard-4.0.0rc6/src/typeguard/_utils.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/src/typeguard.egg-info/PKG-INFO` & `typeguard-4.0.0rc6/src/typeguard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeguard
-Version: 4.0.0rc5
+Version: 4.0.0rc6
 Summary: Run-time type checker for Python
 Author-email: Alex Grönholm <alex.gronholm@nextday.fi>
 License: MIT
 Project-URL: Documentation, https://typeguard.readthedocs.io/en/latest/
 Project-URL: Change log, https://typeguard.readthedocs.io/en/latest/versionhistory.html
 Project-URL: Source code, https://github.com/agronholm/typeguard
 Project-URL: Issue tracker, https://github.com/agronholm/typeguard/issues
```

### Comparing `typeguard-4.0.0rc5/src/typeguard.egg-info/SOURCES.txt` & `typeguard-4.0.0rc6/src/typeguard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/tests/__init__.py` & `typeguard-4.0.0rc6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/tests/conftest.py` & `typeguard-4.0.0rc6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/tests/dummymodule.py` & `typeguard-4.0.0rc6/tests/dummymodule.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/tests/mypy/negative.py` & `typeguard-4.0.0rc6/tests/mypy/negative.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/tests/mypy/positive.py` & `typeguard-4.0.0rc6/tests/mypy/positive.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/tests/mypy/test_type_annotations.py` & `typeguard-4.0.0rc6/tests/mypy/test_type_annotations.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/tests/test_checkers.py` & `typeguard-4.0.0rc6/tests/test_checkers.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/tests/test_importhook.py` & `typeguard-4.0.0rc6/tests/test_importhook.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/tests/test_instrumentation.py` & `typeguard-4.0.0rc6/tests/test_instrumentation.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/tests/test_plugins.py` & `typeguard-4.0.0rc6/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/tests/test_suppression.py` & `typeguard-4.0.0rc6/tests/test_suppression.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/tests/test_transformer.py` & `typeguard-4.0.0rc6/tests/test_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1452,7 +1452,72 @@
             def foo() -> int:
                 if (int := 6):
                     pass
                 return int
             """
         ).strip()
     )
+
+
+def test_dont_leave_empty_ast_container_nodes() -> None:
+    # Regression test for #352
+    node = parse(
+        dedent(
+            """
+            if True:
+
+                class A:
+                    ...
+
+                def func():
+                    ...
+
+            def foo(x: str) -> None:
+                pass
+            """
+        )
+    )
+    TypeguardTransformer(["foo"]).visit(node)
+    assert (
+        unparse(node)
+        == dedent(
+            """
+            if True:
+                pass
+
+            def foo(x: str) -> None:
+                from typeguard import TypeCheckMemo
+                from typeguard._functions import check_argument_types
+                memo = TypeCheckMemo(globals(), locals())
+                check_argument_types('foo', {'x': (x, str)}, memo)
+            """
+        ).strip()
+    )
+
+
+def test_dont_parse_annotated_2nd_arg() -> None:
+    # Regression test for #352
+    node = parse(
+        dedent(
+            """
+            from typing import Annotated
+
+            def foo(x: Annotated[str, 'foo bar']) -> None:
+                pass
+            """
+        )
+    )
+    TypeguardTransformer(["foo"]).visit(node)
+    assert (
+        unparse(node)
+        == dedent(
+            """
+            from typing import Annotated
+
+            def foo(x: Annotated[str, 'foo bar']) -> None:
+                from typeguard import TypeCheckMemo
+                from typeguard._functions import check_argument_types
+                memo = TypeCheckMemo(globals(), locals())
+                check_argument_types('foo', {'x': (x, Annotated[str, 'foo bar'])}, memo)
+            """
+        ).strip()
+    )
```

### Comparing `typeguard-4.0.0rc5/tests/test_typechecked.py` & `typeguard-4.0.0rc6/tests/test_typechecked.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/tests/test_union_transformer.py` & `typeguard-4.0.0rc6/tests/test_union_transformer.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/tests/test_utils.py` & `typeguard-4.0.0rc6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `typeguard-4.0.0rc5/tests/test_warn_on_error.py` & `typeguard-4.0.0rc6/tests/test_warn_on_error.py`

 * *Files identical despite different names*

