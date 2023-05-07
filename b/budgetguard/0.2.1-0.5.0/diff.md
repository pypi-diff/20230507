# Comparing `tmp/budgetguard-0.2.1.tar.gz` & `tmp/budgetguard-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budgetguard-0.2.1.tar", max compression
+gzip compressed data, was "budgetguard-0.5.0.tar", max compression
```

## Comparing `budgetguard-0.2.1.tar` & `budgetguard-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       23 2023-05-05 23:37:14.348031 budgetguard-0.2.1/budgetguard/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 17:14:30.248599 budgetguard-0.2.1/budgetguard/budgetguard/pipelines/__init__.py
--rw-r--r--   0        0        0      352 2023-05-03 17:14:30.249601 budgetguard-0.2.1/budgetguard/budgetguard/pipelines/base.py
--rw-r--r--   0        0        0        0 2023-05-03 17:14:30.249601 budgetguard-0.2.1/budgetguard/budgetguard/scripts/__init__.py
--rw-r--r--   0        0        0      513 2023-05-05 00:11:56.001550 budgetguard-0.2.1/budgetguard/tests/__init__.py
--rw-r--r--   0        0        0     1022 2023-05-04 23:02:25.622629 budgetguard-0.2.1/budgetguard/tests/test_dummy.py
--rw-r--r--   0        0        0     1235 2023-05-03 11:46:24.500492 budgetguard-0.2.1/LICENSE
--rw-r--r--   0        0        0      671 2023-05-06 01:01:40.325593 budgetguard-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      712 2023-05-06 00:24:12.216445 budgetguard-0.2.1/README.md
--rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 budgetguard-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-05-07 16:47:13.284005 budgetguard-0.5.0/budgetguard/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 17:14:30.248599 budgetguard-0.5.0/budgetguard/budgetguard/pipelines/__init__.py
+-rw-r--r--   0        0        0      352 2023-05-03 17:14:30.249601 budgetguard-0.5.0/budgetguard/budgetguard/pipelines/base.py
+-rw-r--r--   0        0        0        0 2023-05-03 17:14:30.249601 budgetguard-0.5.0/budgetguard/budgetguard/scripts/__init__.py
+-rw-r--r--   0        0        0      513 2023-05-05 00:11:56.001550 budgetguard-0.5.0/budgetguard/tests/__init__.py
+-rw-r--r--   0        0        0     1022 2023-05-04 23:02:25.622629 budgetguard-0.5.0/budgetguard/tests/test_dummy.py
+-rw-r--r--   0        0        0     1235 2023-05-03 11:46:24.500492 budgetguard-0.5.0/LICENSE
+-rw-r--r--   0        0        0      671 2023-05-07 16:47:13.285005 budgetguard-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      712 2023-05-06 00:24:12.216445 budgetguard-0.5.0/README.md
+-rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 budgetguard-0.5.0/PKG-INFO
```

### Comparing `budgetguard-0.2.1/budgetguard/tests/__init__.py` & `budgetguard-0.5.0/budgetguard/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `budgetguard-0.2.1/budgetguard/tests/test_dummy.py` & `budgetguard-0.5.0/budgetguard/tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `budgetguard-0.2.1/LICENSE` & `budgetguard-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `budgetguard-0.2.1/README.md` & `budgetguard-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `budgetguard-0.2.1/PKG-INFO` & `budgetguard-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budgetguard
-Version: 0.2.1
+Version: 0.5.0
 Summary: 
 Author: Mateusz Borsuk
 Author-email: mtszborsuk212@gmail.com
 Requires-Python: >=3.8.8,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

