# Comparing `tmp/hyper-bump-it-0.4.0.tar.gz` & `tmp/hyper-bump-it-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyper-bump-it-0.4.0.tar", last modified: Mon Feb 27 13:22:51 2023, max compression
+gzip compressed data, was "hyper-bump-it-0.4.1.tar", last modified: Sun May  7 21:42:06 2023, max compression
```

## Comparing `hyper-bump-it-0.4.0.tar` & `hyper-bump-it-0.4.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:22:51.850477 hyper-bump-it-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-02-27 13:22:51.850477 hyper-bump-it-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:22:51.846477 hyper-bump-it-0.4.0/hyper_bump_it/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:22:51.846477 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:22:51.846477 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/cli/by.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/cli/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:22:51.846477 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/cli/interactive/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/cli/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/cli/interactive/file_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/cli/interactive/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/cli/interactive/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/cli/interactive/top_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/cli/to.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:22:51.846477 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/config/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/config/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/config/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10029 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/config/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/config/keystone_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/execution_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:22:51.850477 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/format_pattern/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/format_pattern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/format_pattern/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/format_pattern/matching_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/format_pattern/text_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/planned_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/vcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/hyper_bump_it/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 13:22:51.846477 hyper-bump-it-0.4.0/hyper_bump_it.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-02-27 13:22:51.000000 hyper-bump-it-0.4.0/hyper_bump_it.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-02-27 13:22:51.000000 hyper-bump-it-0.4.0/hyper_bump_it.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 13:22:51.000000 hyper-bump-it-0.4.0/hyper_bump_it.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-27 13:22:51.000000 hyper-bump-it-0.4.0/hyper_bump_it.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-27 13:22:51.000000 hyper-bump-it-0.4.0/hyper_bump_it.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-27 13:22:51.000000 hyper-bump-it-0.4.0/hyper_bump_it.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 13:22:51.850477 hyper-bump-it-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-27 13:22:41.000000 hyper-bump-it-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:42:06.747787 hyper-bump-it-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-07 21:42:06.747787 hyper-bump-it-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:42:06.739787 hyper-bump-it-0.4.1/hyper_bump_it/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:42:06.743787 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:42:06.743787 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:42:06.743787 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/file_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/top_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/to.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:42:06.747787 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/keystone_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/execution_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:42:06.747787 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/format_pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/format_pattern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/format_pattern/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/format_pattern/matching_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/format_pattern/text_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/planned_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:42:06.739787 hyper-bump-it-0.4.1/hyper_bump_it.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-07 21:42:06.000000 hyper-bump-it-0.4.1/hyper_bump_it.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-07 21:42:06.000000 hyper-bump-it-0.4.1/hyper_bump_it.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 21:42:06.000000 hyper-bump-it-0.4.1/hyper_bump_it.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-07 21:42:06.000000 hyper-bump-it-0.4.1/hyper_bump_it.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-07 21:42:06.000000 hyper-bump-it-0.4.1/hyper_bump_it.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-07 21:42:06.000000 hyper-bump-it-0.4.1/hyper_bump_it.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 21:42:06.747787 hyper-bump-it-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/setup.py
```

### Comparing `hyper-bump-it-0.4.0/LICENSE` & `hyper-bump-it-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/PKG-INFO` & `hyper-bump-it-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyper-bump-it
-Version: 0.4.0
+Version: 0.4.1
 Summary: A version bumping tool
 Author-email: Patrick Lannigan <p.lannigan@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/plannigan/hyper-bump-it
 Project-URL: changelog, https://github.com/plannigan/hyper-bump-it/blob/main/CHANGELOG.md
 Project-URL: issues, https://github.com/plannigan/hyper-bump-it/issues
 Keywords: version,bump,command line
@@ -23,24 +23,26 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hyper-bump-it)][pypi]
 [![codecov](https://codecov.io/gh/plannigan/hyper-bump-it/branch/main/graph/badge.svg?token=V4DADJU0BI)][codecov]
 [![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)][mypy-home]
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)][black-home]
 
 # Hyper Bump It
 
-A version bumping tool.
+A command line tool for updating the version in project files needed for the next release.
 
 `hyper-bump-it`'s features include:
+
 * Updating the version to a new fully specified value
-* Increasing the version base on a specific version part
+* Increasing the version based on a specific version part
 * Optional Git integrations:
     * Commit changes
     * Create a new branch or tag
     * Push changes to a remote repository
 * Customizable search and replacement patterns
+    * Match based on the current version or arbitrary dates
 * Safe by default, but can be overridden:
     * Request confirmation before editing files
     * Explicit configuration need to push changes
     * Won't run if the current branch is not the default
     * Won't run if there are unstaged changes
 * TOML configuration file (can be part of `pyproject.toml`)
```

### Comparing `hyper-bump-it-0.4.0/README.md` & `hyper-bump-it-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hyper-bump-it)][pypi]
 [![codecov](https://codecov.io/gh/plannigan/hyper-bump-it/branch/main/graph/badge.svg?token=V4DADJU0BI)][codecov]
 [![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)][mypy-home]
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)][black-home]
 
 # Hyper Bump It
 
-A version bumping tool.
+A command line tool for updating the version in project files needed for the next release.
 
 `hyper-bump-it`'s features include:
+
 * Updating the version to a new fully specified value
-* Increasing the version base on a specific version part
+* Increasing the version based on a specific version part
 * Optional Git integrations:
     * Commit changes
     * Create a new branch or tag
     * Push changes to a remote repository
 * Customizable search and replacement patterns
+    * Match based on the current version or arbitrary dates
 * Safe by default, but can be overridden:
     * Request confirmation before editing files
     * Explicit configuration need to push changes
     * Won't run if the current branch is not the default
     * Won't run if there are unstaged changes
 * TOML configuration file (can be part of `pyproject.toml`)
```

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/cli/common.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,72 +18,72 @@
 ERROR_PANEL_BORDER_STYLE = "red"
 ERROR_PANEL_TILE_ALIGN_: AlignMethod = "left"
 EXAMPLE_FILE_GLOB = "version.txt"
 
 
 class OptionFactory(Protocol):
     def __call__(  # type: ignore[misc]
-        self, default: object = ..., panel_name: str = ...
+        self, panel_name: str = ..., show_default: bool = ...
     ) -> Any:
         ...
 
 
 def _create_option_factory(description: str, *param_decls: str) -> OptionFactory:
     def _create_option(  # type: ignore[misc]
-        default: object = None, panel_name: str = OVERRIDE_PANEL_NAME
+        panel_name: str = OVERRIDE_PANEL_NAME, show_default: bool = False
     ) -> Any:
         return typer.Option(
-            default,
             *param_decls,
             help=description,
-            show_default=default is not None,
+            show_default=show_default,
             rich_help_panel=panel_name,
         )
 
     return _create_option
 
 
 CONFIG_FILE = typer.Option(
-    None,
     help="Path to dedicated configuration file to use instead of normal file discovery",
     show_default=False,
 )
-PROJECT_ROOT = typer.Option(
-    Path.cwd(),
+CONFIG_FILE_DEFAULT: Optional[Path] = None
+PROJECT_ROOT = typer.Option(  # type: ignore[call-overload]
     help="Path to directory containing the project",
-    show_default="Use current directory",  # type: ignore[arg-type]
+    show_default="Use current directory",
 )
+PROJECT_ROOT_DEFAULT = Path.cwd()
 DRY_RUN = typer.Option(
-    False,
     "--no",
     "-n",
     "--dry-run/--no-dry-run",
     help="Answer no to the confirmation prompt. "
     "Only displaying the operations that would be performed",
     show_default=False,
 )
+DRY_RUN_DEFAULT = False
 PATCH = typer.Option(
-    False,
     "--patch/--no-patch",
     help="Like --dry-run, but only display the unified diff output for the planned changes",
     show_default=False,
 )
+PATCH_DEFAULT = False
 SKIP_CONFIRM_PROMPT = typer.Option(
-    None,
     "--yes/--interactive",
     "-y",
     help="Answer yes to the confirmation prompt and run non-interactively",
     show_default=False,
 )
+SKIP_CONFIRM_PROMPT_DEFAULT: Optional[bool] = None
 CURRENT_VERSION = typer.Option(
-    None,
     help="Override the current version",
     show_default=False,
     rich_help_panel=OVERRIDE_PANEL_NAME,
+    parser=Version.parse,
 )
+CURRENT_VERSION_DEFAULT: Optional[Version] = None
 
 commit = _create_option_factory("Control commit Git action")
 branch = _create_option_factory("Control branch Git action")
 tag = _create_option_factory("Control tag Git action")
 remote = _create_option_factory("Name of remote to use when pushing changes")
 commit_format_pattern = _create_option_factory(
     "Format pattern to use for commit message"
@@ -97,43 +97,21 @@
 )
 allow_any_init_branch = _create_option_factory(
     "Disable any initial branch restrictions. (takes precedence over --allowed-init-branch)",
     "--allow-any-init-branch",
 )
 
 
-@overload
-def parse_version(version: str, parameter_name: str) -> Version:
-    ...
-
-
-@overload
-def parse_version(version: Optional[str], parameter_name: str) -> Optional[Version]:
-    ...
-
-
-def parse_version(version: Optional[str], parameter_name: str) -> Optional[Version]:
-    if version is None:
-        return None
-    else:
-        try:
-            return Version.parse(version)
-        except ValueError:
-            raise typer.BadParameter(
-                f"'{version}' is not a valid version", param_hint=parameter_name
-            )
-
-
 def allowed_init_branches(
-    allowed_branches_arg: list[str],
+    allowed_branches_arg: Optional[list[str]],
     allow_any_init_branch_arg: Optional[bool],
 ) -> Optional[frozenset[str]]:
     if allow_any_init_branch_arg is True:
         return frozenset()
-    if len(allowed_branches_arg) == 0:
+    if allowed_branches_arg is None or len(allowed_branches_arg) == 0:
         return None
 
     unique_names = frozenset(allowed_branches_arg)
     if len(unique_names) == len(allowed_branches_arg):
         return unique_names
 
     for value in unique_names:
```

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/cli/init.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/init.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Initialize configuration command.
 """
 from pathlib import Path
-from typing import Mapping
+from typing import Annotated, Mapping
 
 import tomlkit
 import typer
 from pydantic import ValidationError
 from tomlkit.exceptions import TOMLKitError
 
 from .. import ui
@@ -26,69 +26,90 @@
     ConfigFile,
     FileDefinition,
     GitAction,
     GitActionsConfigFile,
     GitConfigFile,
 )
 from ..error import ConfigurationFileReadError, first_error_message
+from ..version import Version
 from . import common, interactive
 
 GIT_PANEL_NAME = "Git Configuration Options"
 
 
 def init_command(
-    current_version: str = typer.Argument(
-        ..., help="Current version for the project", show_default=False
-    ),
-    config_file_name: str = typer.Option(
-        HYPER_CONFIG_FILE_NAME,
-        help="Custom file name for dedicated configuration file",
-    ),
-    project_root: Path = common.PROJECT_ROOT,
-    pyproject: bool = typer.Option(
-        False,
-        help=f"Write config to {PYPROJECT_FILE_NAME}",
-        show_default="Use dedicated configuration file",  # type: ignore[arg-type]
-    ),
-    non_interactive: bool = typer.Option(
-        False,
-        "--non-interactive/--interactive",
-        help="Write out a configuration without prompting for additional information "
-        "(will need manual edits)",
-    ),
-    commit: GitAction = common.commit(DEFAULT_COMMIT_ACTION.value, GIT_PANEL_NAME),
-    branch: GitAction = common.branch(DEFAULT_BRANCH_ACTION.value, GIT_PANEL_NAME),
-    tag: GitAction = common.tag(DEFAULT_TAG_ACTION.value, GIT_PANEL_NAME),
-    remote: str = common.remote(DEFAULT_REMOTE, GIT_PANEL_NAME),
-    commit_format_pattern: str = common.commit_format_pattern(
-        DEFAULT_COMMIT_FORMAT_PATTERN, GIT_PANEL_NAME
-    ),
-    branch_format_pattern: str = common.branch_format_pattern(
-        DEFAULT_BRANCH_FORMAT_PATTERN, GIT_PANEL_NAME
-    ),
-    tag_format_pattern: str = common.tag_format_pattern(
-        DEFAULT_TAG_FORMAT_PATTERN, GIT_PANEL_NAME
-    ),
-    allowed_init_branch: list[str] = common.allowed_init_branch(
-        list(DEFAULT_ALLOWED_INITIAL_BRANCHES), GIT_PANEL_NAME
-    ),
-    allow_any_init_branch: bool = common.allow_any_init_branch(False, GIT_PANEL_NAME),
+    current_version: Annotated[
+        Version,
+        typer.Argument(
+            help="Current version for the project",
+            show_default=False,
+            parser=Version.parse,
+        ),
+    ],
+    config_file_name: Annotated[
+        str,
+        typer.Option(
+            help="Custom file name for dedicated configuration file",
+        ),
+    ] = HYPER_CONFIG_FILE_NAME,
+    project_root: Annotated[Path, common.PROJECT_ROOT] = common.PROJECT_ROOT_DEFAULT,
+    pyproject: Annotated[
+        bool,
+        typer.Option(
+            help=f"Write config to {PYPROJECT_FILE_NAME}",
+            show_default="Use dedicated configuration file",
+        ),
+    ] = False,
+    non_interactive: Annotated[
+        bool,
+        typer.Option(
+            "--non-interactive/--interactive",
+            help="Write out a configuration without prompting for additional information "
+            "(will need manual edits)",
+        ),
+    ] = False,
+    commit: Annotated[
+        GitAction, common.commit(GIT_PANEL_NAME, show_default=True)
+    ] = DEFAULT_COMMIT_ACTION,
+    branch: Annotated[
+        GitAction, common.branch(GIT_PANEL_NAME, show_default=True)
+    ] = DEFAULT_BRANCH_ACTION,
+    tag: Annotated[
+        GitAction, common.tag(GIT_PANEL_NAME, show_default=True)
+    ] = DEFAULT_TAG_ACTION,
+    remote: Annotated[
+        str, common.remote(GIT_PANEL_NAME, show_default=True)
+    ] = DEFAULT_REMOTE,
+    commit_format_pattern: Annotated[
+        str, common.commit_format_pattern(GIT_PANEL_NAME, show_default=True)
+    ] = DEFAULT_COMMIT_FORMAT_PATTERN,
+    branch_format_pattern: Annotated[
+        str, common.branch_format_pattern(GIT_PANEL_NAME, show_default=True)
+    ] = DEFAULT_BRANCH_FORMAT_PATTERN,
+    tag_format_pattern: Annotated[
+        str, common.tag_format_pattern(GIT_PANEL_NAME, show_default=True)
+    ] = DEFAULT_TAG_FORMAT_PATTERN,
+    allowed_init_branch: Annotated[
+        list[str], common.allowed_init_branch(GIT_PANEL_NAME, show_default=True)
+    ] = list(DEFAULT_ALLOWED_INITIAL_BRANCHES),
+    allow_any_init_branch: Annotated[
+        bool, common.allow_any_init_branch(GIT_PANEL_NAME)
+    ] = False,
 ) -> None:
-    version = common.parse_version(current_version, "CURRENT_VERSION")
     try:
         actions = GitActionsConfigFile(commit=commit, branch=branch, tag=tag)
     except ValidationError as ex:
         common.display_and_exit(first_error_message(ex), exit_code=2)
 
     if allow_any_init_branch:
         allowed_init_branch = []
 
     project_root = common.resolve(project_root)
     config = ConfigFile(
-        current_version=version,
+        current_version=current_version,
         files=[FileDefinition(file_glob=common.EXAMPLE_FILE_GLOB)],
         git=GitConfigFile(
             remote=remote,
             commit_format_pattern=commit_format_pattern,
             branch_format_pattern=branch_format_pattern,
             tag_format_pattern=tag_format_pattern,
             allowed_initial_branches=frozenset(allowed_init_branch),
```

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/cli/interactive/file_validation.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/file_validation.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/cli/interactive/files.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/files.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/cli/interactive/git.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/git.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/cli/interactive/top_level.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/top_level.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/compat.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/compat.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/config/__init__.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/__init__.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/config/application.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/application.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/config/cli.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/cli.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/config/core.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/core.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/config/file.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import dataclasses
 from collections.abc import Sequence
 from pathlib import Path
-from typing import Callable, Iterator, Optional, Union, cast
+from typing import Optional, Union, cast
 
 import tomlkit
 from pydantic import (
     BaseModel,
     Field,
     StrictBool,
     StrictStr,
     ValidationError,
     root_validator,
+    validator,
 )
 from tomlkit import TOMLDocument
 from tomlkit.exceptions import TOMLKitError
 
 from ..compat import TypeAlias
 from ..error import (
     ConfigurationFileNotFoundError,
@@ -83,36 +84,32 @@
 
 
 HyperConfigFileValues: TypeAlias = dict[
     str, Union[list[File], Optional[StrictStr], Git]
 ]
 
 
-class ValidVersion(Version):
-    @classmethod
-    def __get_validators__(cls) -> Iterator[Callable[[object], "ValidVersion"]]:
-        yield cls._validate
+class ConfigFile(HyperBaseMode):
+    files: list[File] = Field(..., min_items=1)
+    current_version: Optional[Version] = None
+    show_confirm_prompt: StrictBool = True
+    git: Git = Git()
 
-    @classmethod
-    def _validate(cls, value: object) -> "ValidVersion":
+    @validator("current_version", pre=True)
+    def _check_version(cls, value: Optional[object]) -> Optional[Version]:
+        if value is None:
+            return None
         if isinstance(value, Version):
-            return cast(ValidVersion, dataclasses.replace(value))
+            return dataclasses.replace(value)
         if isinstance(value, str):
-            return cast(ValidVersion, Version.parse(value))
+            return Version.parse(value)
         raise TypeError(
             "Value must be a version or a string that can be parsed into a version"
         )
 
-
-class ConfigFile(HyperBaseMode):
-    files: list[File] = Field(..., min_items=1)
-    current_version: Optional[ValidVersion] = None
-    show_confirm_prompt: StrictBool = True
-    git: Git = Git()
-
     @root_validator(skip_on_failure=True)
     def _check_keystone_files(
         cls,
         values: HyperConfigFileValues,
     ) -> HyperConfigFileValues:
         files = cast(list[File], values["files"])
         keystone_file_count = sum(1 for file in files if file.keystone)
```

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/config/keystone_parser.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/keystone_parser.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/core.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/core.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/error.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/error.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/execution_plan.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/execution_plan.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/files.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/files.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/format_pattern/keys.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/format_pattern/keys.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/format_pattern/matching_pattern.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/format_pattern/matching_pattern.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/format_pattern/text_formatter.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/format_pattern/text_formatter.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/planned_changes.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/planned_changes.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/ui.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/ui.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/vcs.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/vcs.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it/_hyper_bump_it/version.py` & `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/version.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it.egg-info/PKG-INFO` & `hyper-bump-it-0.4.1/hyper_bump_it.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyper-bump-it
-Version: 0.4.0
+Version: 0.4.1
 Summary: A version bumping tool
 Author-email: Patrick Lannigan <p.lannigan@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/plannigan/hyper-bump-it
 Project-URL: changelog, https://github.com/plannigan/hyper-bump-it/blob/main/CHANGELOG.md
 Project-URL: issues, https://github.com/plannigan/hyper-bump-it/issues
 Keywords: version,bump,command line
@@ -23,24 +23,26 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hyper-bump-it)][pypi]
 [![codecov](https://codecov.io/gh/plannigan/hyper-bump-it/branch/main/graph/badge.svg?token=V4DADJU0BI)][codecov]
 [![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)][mypy-home]
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)][black-home]
 
 # Hyper Bump It
 
-A version bumping tool.
+A command line tool for updating the version in project files needed for the next release.
 
 `hyper-bump-it`'s features include:
+
 * Updating the version to a new fully specified value
-* Increasing the version base on a specific version part
+* Increasing the version based on a specific version part
 * Optional Git integrations:
     * Commit changes
     * Create a new branch or tag
     * Push changes to a remote repository
 * Customizable search and replacement patterns
+    * Match based on the current version or arbitrary dates
 * Safe by default, but can be overridden:
     * Request confirmation before editing files
     * Explicit configuration need to push changes
     * Won't run if the current branch is not the default
     * Won't run if there are unstaged changes
 * TOML configuration file (can be part of `pyproject.toml`)
```

### Comparing `hyper-bump-it-0.4.0/hyper_bump_it.egg-info/SOURCES.txt` & `hyper-bump-it-0.4.1/hyper_bump_it.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.0/pyproject.toml` & `hyper-bump-it-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "hyper-bump-it"
-version = "0.4.0"
+version = "0.4.1"
 description = "A version bumping tool"
 readme = "README.md"
 requires-python = ">=3.9,<4.0"
 license = {text = "MIT"}
 dependencies = [
     "GitPython>=3.1.29,<4",
     "tomlkit>=0.11.6,<1.0",
-    "typer>=0.7.0,<1.0",
+    "typer>=0.9.0,<1.0",
     "pydantic>=1.10.2,<2",
     "rich>=12.6.0,<14",
     "typing-extensions>=4.4.0,<5; python_version < '3.11'",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
```

