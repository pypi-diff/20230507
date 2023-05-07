# Comparing `tmp/alpha_trader_python-0.2.0.tar.gz` & `tmp/alpha_trader_python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpha_trader_python-0.2.0.tar", max compression
+gzip compressed data, was "alpha_trader_python-0.2.1.tar", max compression
```

## Comparing `alpha_trader_python-0.2.0.tar` & `alpha_trader_python-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      255 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/README.md
--rw-r--r--   0        0        0       22 2023-05-07 11:23:54.033893 alpha_trader_python-0.2.0/alpha_trader/__init__.py
--rw-r--r--   0        0        0     2074 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/achievement/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/authentication/__init__.py
--rw-r--r--   0        0        0      961 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/bank_account/__init__.py
--rw-r--r--   0        0        0     5117 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/bonds/__init__.py
--rw-r--r--   0        0        0     9181 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/client/__init__.py
--rw-r--r--   0        0        0     3017 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/company/__init__.py
--rw-r--r--   0        0        0      776 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/filter/__init__.py
--rw-r--r--   0        0        0     1155 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/listing/__init__.py
--rw-r--r--   0        0        0      387 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/logging/__init__.py
--rw-r--r--   0        0        0     4276 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/miner/__init__.py
--rw-r--r--   0        0        0     6091 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/order/__init__.py
--rw-r--r--   0        0        0      470 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/owner/__init__.py
--rw-r--r--   0        0        0       71 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/partner/__init__.py
--rw-r--r--   0        0        0     1629 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/portfolio/__init__.py
--rw-r--r--   0        0        0     1895 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/portfolio/position.py
--rw-r--r--   0        0        0        0 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/price/__init__.py
--rw-r--r--   0        0        0      405 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/price/price.py
--rw-r--r--   0        0        0     2790 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/price/price_spread.py
--rw-r--r--   0        0        0     2771 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/securities_account/__init__.py
--rw-r--r--   0        0        0     8216 2023-05-07 11:23:53.233885 alpha_trader_python-0.2.0/alpha_trader/user/__init__.py
--rw-r--r--   0        0        0      929 2023-05-07 11:23:54.033893 alpha_trader_python-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 alpha_trader_python-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      255 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/README.md
+-rw-r--r--   0        0        0       22 2023-05-07 12:19:09.225540 alpha_trader_python-0.2.1/alpha_trader/__init__.py
+-rw-r--r--   0        0        0     2074 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/achievement/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/authentication/__init__.py
+-rw-r--r--   0        0        0      961 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/bank_account/__init__.py
+-rw-r--r--   0        0        0     5117 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/bonds/__init__.py
+-rw-r--r--   0        0        0     9225 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/client/__init__.py
+-rw-r--r--   0        0        0     3017 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/company/__init__.py
+-rw-r--r--   0        0        0      776 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/filter/__init__.py
+-rw-r--r--   0        0        0     1155 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/listing/__init__.py
+-rw-r--r--   0        0        0      387 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/logging/__init__.py
+-rw-r--r--   0        0        0     4276 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/miner/__init__.py
+-rw-r--r--   0        0        0     6091 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/order/__init__.py
+-rw-r--r--   0        0        0      470 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/owner/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/partner/__init__.py
+-rw-r--r--   0        0        0     1629 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/portfolio/__init__.py
+-rw-r--r--   0        0        0     1895 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/portfolio/position.py
+-rw-r--r--   0        0        0        0 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/price/__init__.py
+-rw-r--r--   0        0        0      405 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/price/price.py
+-rw-r--r--   0        0        0     2790 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/price/price_spread.py
+-rw-r--r--   0        0        0     2771 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/securities_account/__init__.py
+-rw-r--r--   0        0        0     8216 2023-05-07 12:19:08.257531 alpha_trader_python-0.2.1/alpha_trader/user/__init__.py
+-rw-r--r--   0        0        0      929 2023-05-07 12:19:09.225540 alpha_trader_python-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 alpha_trader_python-0.2.1/PKG-INFO
```

### Comparing `alpha_trader_python-0.2.0/alpha_trader/achievement/__init__.py` & `alpha_trader_python-0.2.1/alpha_trader/achievement/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.2.0/alpha_trader/bank_account/__init__.py` & `alpha_trader_python-0.2.1/alpha_trader/bank_account/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.2.0/alpha_trader/bonds/__init__.py` & `alpha_trader_python-0.2.1/alpha_trader/bonds/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.2.0/alpha_trader/client/__init__.py` & `alpha_trader_python-0.2.1/alpha_trader/client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,14 +287,16 @@
             password: Password
             email: Email
             locale: Locale
 
         Returns:
             User
         """
+        from alpha_trader.user import User
+
         data = {
             "username": username,
             "password": password,
             "emailAddress": email,
             "locale": locale,
         }
```

### Comparing `alpha_trader_python-0.2.0/alpha_trader/company/__init__.py` & `alpha_trader_python-0.2.1/alpha_trader/company/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.2.0/alpha_trader/filter/__init__.py` & `alpha_trader_python-0.2.1/alpha_trader/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.2.0/alpha_trader/listing/__init__.py` & `alpha_trader_python-0.2.1/alpha_trader/listing/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.2.0/alpha_trader/miner/__init__.py` & `alpha_trader_python-0.2.1/alpha_trader/miner/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.2.0/alpha_trader/order/__init__.py` & `alpha_trader_python-0.2.1/alpha_trader/order/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.2.0/alpha_trader/portfolio/__init__.py` & `alpha_trader_python-0.2.1/alpha_trader/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.2.0/alpha_trader/portfolio/position.py` & `alpha_trader_python-0.2.1/alpha_trader/portfolio/position.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.2.0/alpha_trader/price/price_spread.py` & `alpha_trader_python-0.2.1/alpha_trader/price/price_spread.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.2.0/alpha_trader/securities_account/__init__.py` & `alpha_trader_python-0.2.1/alpha_trader/securities_account/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.2.0/alpha_trader/user/__init__.py` & `alpha_trader_python-0.2.1/alpha_trader/user/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.2.0/pyproject.toml` & `alpha_trader_python-0.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alpha-trader-python"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python SDK for https://alpha-trader.com"
 authors = ["maltemelzer"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "alpha_trader"}]
 
 [tool.poetry.dependencies]
```

### Comparing `alpha_trader_python-0.2.0/PKG-INFO` & `alpha_trader_python-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpha-trader-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python SDK for https://alpha-trader.com
 License: MIT
 Author: maltemelzer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

