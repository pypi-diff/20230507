# Comparing `tmp/budgetguard-0.1.0.tar.gz` & `tmp/budgetguard-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budgetguard-0.1.0.tar", max compression
+gzip compressed data, was "budgetguard-0.2.1.tar", max compression
```

## Comparing `budgetguard-0.1.0.tar` & `budgetguard-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0        0 2023-05-03 14:54:50.599944 budgetguard-0.1.0/budgetguard/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 17:14:30.248599 budgetguard-0.1.0/budgetguard/budgetguard/pipelines/__init__.py
--rw-r--r--   0        0        0      352 2023-05-03 17:14:30.249601 budgetguard-0.1.0/budgetguard/budgetguard/pipelines/base.py
--rw-r--r--   0        0        0        0 2023-05-03 17:14:30.249601 budgetguard-0.1.0/budgetguard/budgetguard/scripts/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 17:14:30.252602 budgetguard-0.1.0/budgetguard/tests/__init__.py
--rw-r--r--   0        0        0      373 2023-05-03 21:15:49.018397 budgetguard-0.1.0/budgetguard/tests/conftest.py
--rw-r--r--   0        0        0      934 2023-05-03 21:17:12.020318 budgetguard-0.1.0/budgetguard/tests/dummy_tests.py
--rw-r--r--   0        0        0     1235 2023-05-03 11:46:24.500492 budgetguard-0.1.0/LICENSE
--rw-r--r--   0        0        0      599 2023-05-03 21:27:49.039543 budgetguard-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4639 2023-05-03 11:46:24.501492 budgetguard-0.1.0/README.md
--rw-r--r--   0        0        0     4994 1970-01-01 00:00:00.000000 budgetguard-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-05-05 23:37:14.348031 budgetguard-0.2.1/budgetguard/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 17:14:30.248599 budgetguard-0.2.1/budgetguard/budgetguard/pipelines/__init__.py
+-rw-r--r--   0        0        0      352 2023-05-03 17:14:30.249601 budgetguard-0.2.1/budgetguard/budgetguard/pipelines/base.py
+-rw-r--r--   0        0        0        0 2023-05-03 17:14:30.249601 budgetguard-0.2.1/budgetguard/budgetguard/scripts/__init__.py
+-rw-r--r--   0        0        0      513 2023-05-05 00:11:56.001550 budgetguard-0.2.1/budgetguard/tests/__init__.py
+-rw-r--r--   0        0        0     1022 2023-05-04 23:02:25.622629 budgetguard-0.2.1/budgetguard/tests/test_dummy.py
+-rw-r--r--   0        0        0     1235 2023-05-03 11:46:24.500492 budgetguard-0.2.1/LICENSE
+-rw-r--r--   0        0        0      671 2023-05-06 01:01:40.325593 budgetguard-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      712 2023-05-06 00:24:12.216445 budgetguard-0.2.1/README.md
+-rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 budgetguard-0.2.1/PKG-INFO
```

### Comparing `budgetguard-0.1.0/LICENSE` & `budgetguard-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `budgetguard-0.1.0/pyproject.toml` & `budgetguard-0.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [tool.poetry]
 name = "budgetguard"
-version = "0.1.0"
+version = "0.2.1"
 description = ""
 authors = ["Mateusz Borsuk <mtszborsuk212@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.8"
-pyspark = "^3.4.0"
+requests = "^2.28.2, !=2.30.0"
+pyspark = "3.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 coverage = "^7.2.5"
 flake8 = "^6.0.0"
 black = "^23.3.0"
 isort = "^5.12.0"
 pytest-cov = "^4.0.0"
 codecov = "^2.1.13"
 mkdocs = "^1.4.3"
 mypy = "^1.2.0"
 pre-commit = "^3.3.1"
 scriv = {extras = ["toml"], version = "^1.3.1"}
+tox = "^4.5.1"
+bump2version = "^1.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

