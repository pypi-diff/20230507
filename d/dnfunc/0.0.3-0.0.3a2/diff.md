# Comparing `tmp/dnfunc-0.0.3.tar.gz` & `tmp/dnfunc-0.0.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnfunc-0.0.3.tar", max compression
+gzip compressed data, was "dnfunc-0.0.3a2.tar", max compression
```

## Comparing `dnfunc-0.0.3.tar` & `dnfunc-0.0.3a2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2023-05-07 14:46:07.796520 dnfunc-0.0.3/LICENSE
--rw-r--r--   0        0        0      553 2023-05-07 14:46:07.796520 dnfunc-0.0.3/README.md
--rw-r--r--   0        0        0     2655 2023-05-07 14:46:20.704563 dnfunc-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    49969 2023-05-07 14:46:07.796520 dnfunc-0.0.3/src/dnfunc/__init__.py
--rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 dnfunc-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-05 08:20:19.643067 dnfunc-0.0.3a2/LICENSE
+-rw-r--r--   0        0        0      472 2023-05-05 08:20:19.643067 dnfunc-0.0.3a2/README.md
+-rw-r--r--   0        0        0     2663 2023-05-05 08:20:33.743370 dnfunc-0.0.3a2/pyproject.toml
+-rw-r--r--   0        0        0    49969 2023-05-05 08:20:19.647066 dnfunc-0.0.3a2/src/dnfunc/__init__.py
+-rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 dnfunc-0.0.3a2/PKG-INFO
```

### Comparing `dnfunc-0.0.3/LICENSE` & `dnfunc-0.0.3a2/LICENSE`

 * *Files identical despite different names*

### Comparing `dnfunc-0.0.3/pyproject.toml` & `dnfunc-0.0.3a2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "dnfunc"
-version = "0.0.3"
+version = "0.0.3-alpha.2"
 description = "A collection of Vapoursynth functions and wrapperspoetr"
 authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/dnfunc"
 repository = "https://github.com/DeadNews/dnfunc"
 keywords = ["vapoursynth", "vapoursynth-functions", "video-encoding"]
@@ -26,15 +26,15 @@
 vstools = "^2.1.0"
 vsutil = "^0.8.0"
 
 [tool.poetry.group.ci.dependencies]
 black = "^23.3.0"
 mypy = "^1.2.0"
 poethepoet = "^0.20.0"
-ruff = "^0.0.265"
+ruff = "^0.0.264"
 types-pyyaml = "^6.0.12.9"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 
 [tool.poe.tasks]
```

### Comparing `dnfunc-0.0.3/src/dnfunc/__init__.py` & `dnfunc-0.0.3a2/src/dnfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `dnfunc-0.0.3/PKG-INFO` & `dnfunc-0.0.3a2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnfunc
-Version: 0.0.3
+Version: 0.0.3a2
 Summary: A collection of Vapoursynth functions and wrapperspoetr
 Home-page: https://github.com/DeadNews/dnfunc
 License: MIT
 Keywords: vapoursynth,vapoursynth-functions,video-encoding
 Author: DeadNews
 Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.10,<4.0
@@ -27,11 +27,7 @@
 
 > A collection of Vapoursynth functions and wrappers
 
 [![PyPI version](https://img.shields.io/pypi/v/dnfunc)](https://pypi.org/project/dnfunc)
 [![CI/CD](https://github.com/DeadNews/dnfunc/actions/workflows/python-vs-app.yml/badge.svg)](https://github.com/DeadNews/dnfunc/actions/workflows/python-vs-app.yml)
 [![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/dnfunc/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/dnfunc/main)
 
-## Deps
-
-<https://github.com/DeadNews/zsh-scripts/blob/main/src/vs-plugins.zsh>
-
```

