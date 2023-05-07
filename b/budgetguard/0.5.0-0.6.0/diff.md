# Comparing `tmp/budgetguard-0.5.0.tar.gz` & `tmp/budgetguard-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budgetguard-0.5.0.tar", max compression
+gzip compressed data, was "budgetguard-0.6.0.tar", max compression
```

## Comparing `budgetguard-0.5.0.tar` & `budgetguard-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       23 2023-05-07 16:47:13.284005 budgetguard-0.5.0/budgetguard/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 17:14:30.248599 budgetguard-0.5.0/budgetguard/budgetguard/pipelines/__init__.py
--rw-r--r--   0        0        0      352 2023-05-03 17:14:30.249601 budgetguard-0.5.0/budgetguard/budgetguard/pipelines/base.py
--rw-r--r--   0        0        0        0 2023-05-03 17:14:30.249601 budgetguard-0.5.0/budgetguard/budgetguard/scripts/__init__.py
--rw-r--r--   0        0        0      513 2023-05-05 00:11:56.001550 budgetguard-0.5.0/budgetguard/tests/__init__.py
--rw-r--r--   0        0        0     1022 2023-05-04 23:02:25.622629 budgetguard-0.5.0/budgetguard/tests/test_dummy.py
--rw-r--r--   0        0        0     1235 2023-05-03 11:46:24.500492 budgetguard-0.5.0/LICENSE
--rw-r--r--   0        0        0      671 2023-05-07 16:47:13.285005 budgetguard-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      712 2023-05-06 00:24:12.216445 budgetguard-0.5.0/README.md
--rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 budgetguard-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-05-07 17:09:02.484878 budgetguard-0.6.0/budgetguard/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 17:14:30.248599 budgetguard-0.6.0/budgetguard/budgetguard/pipelines/__init__.py
+-rw-r--r--   0        0        0      352 2023-05-03 17:14:30.249601 budgetguard-0.6.0/budgetguard/budgetguard/pipelines/base.py
+-rw-r--r--   0        0        0        0 2023-05-03 17:14:30.249601 budgetguard-0.6.0/budgetguard/budgetguard/scripts/__init__.py
+-rw-r--r--   0        0        0      513 2023-05-05 00:11:56.001550 budgetguard-0.6.0/budgetguard/tests/__init__.py
+-rw-r--r--   0        0        0     1022 2023-05-04 23:02:25.622629 budgetguard-0.6.0/budgetguard/tests/test_dummy.py
+-rw-r--r--   0        0        0     1235 2023-05-03 11:46:24.500492 budgetguard-0.6.0/LICENSE
+-rw-r--r--   0        0        0      704 2023-05-07 17:09:02.496876 budgetguard-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      712 2023-05-06 00:24:12.216445 budgetguard-0.6.0/README.md
+-rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 budgetguard-0.6.0/PKG-INFO
```

### Comparing `budgetguard-0.5.0/budgetguard/tests/__init__.py` & `budgetguard-0.6.0/budgetguard/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `budgetguard-0.5.0/budgetguard/tests/test_dummy.py` & `budgetguard-0.6.0/budgetguard/tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `budgetguard-0.5.0/LICENSE` & `budgetguard-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `budgetguard-0.5.0/pyproject.toml` & `budgetguard-0.6.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [tool.poetry]
 name = "budgetguard"
-version = "0.5.0"
+version = "0.6.0"
 description = ""
 authors = ["Mateusz Borsuk <mtszborsuk212@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.8"
-requests = "^2.28.2, !=2.30.0"
+requests = "2.30.0"
 pyspark = "3.2.0"
+requests_toolbelt = "1.0"
+urllib3 = "2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 coverage = "^7.2.5"
 flake8 = "^6.0.0"
 black = "^23.3.0"
 isort = "^5.12.0"
```

### Comparing `budgetguard-0.5.0/README.md` & `budgetguard-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `budgetguard-0.5.0/PKG-INFO` & `budgetguard-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: budgetguard
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Author: Mateusz Borsuk
 Author-email: mtszborsuk212@gmail.com
 Requires-Python: >=3.8.8,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyspark (==3.2.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0,!=2.30.0)
+Requires-Dist: requests (==2.30.0)
+Requires-Dist: requests_toolbelt (==1.0)
+Requires-Dist: urllib3 (==2.0)
 Description-Content-Type: text/markdown
 
 
 # BudgetGuard
 [![codecov](https://codecov.io/gh/M-Borsuk/BudgetGuard/branch/main/graph/badge.svg?token=BudgetGuard_token_here)](https://codecov.io/gh/M-Borsuk/BudgetGuard)
 [![CI](https://github.com/M-Borsuk/BudgetGuard/actions/workflows/main.yml/badge.svg)](https://github.com/M-Borsuk/BudgetGuard/actions/workflows/main.yml)
```

