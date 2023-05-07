# Comparing `tmp/cluedin-0.2.0.tar.gz` & `tmp/cluedin-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cluedin-0.2.0.tar", max compression
+gzip compressed data, was "cluedin-0.2.1.tar", max compression
```

## Comparing `cluedin-0.2.0.tar` & `cluedin-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-05-02 20:10:19.990177 cluedin-0.2.0/README.md
--rw-r--r--   0        0        0      119 2023-05-07 15:56:18.443909 cluedin-0.2.0/cluedin/__init__.py
--rw-r--r--   0        0        0      664 2023-05-06 19:21:43.490227 cluedin-0.2.0/cluedin/auth.py
--rw-r--r--   0        0        0     1120 2023-05-07 16:45:36.605300 cluedin-0.2.0/cluedin/gql.py
--rw-r--r--   0        0        0      681 2023-05-07 15:56:40.250091 cluedin-0.2.0/cluedin/urls.py
--rw-r--r--   0        0        0      264 2023-05-06 19:41:45.000595 cluedin-0.2.0/cluedin/utils.py
--rw-r--r--   0        0        0      292 2023-05-07 16:51:57.219769 cluedin-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 cluedin-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1927 2023-05-07 18:00:02.022377 cluedin-0.2.1/README.md
+-rw-r--r--   0        0        0      119 2023-05-07 15:56:18.443909 cluedin-0.2.1/cluedin/__init__.py
+-rw-r--r--   0        0        0      664 2023-05-06 19:21:43.490227 cluedin-0.2.1/cluedin/auth.py
+-rw-r--r--   0        0        0     1120 2023-05-07 16:45:36.605300 cluedin-0.2.1/cluedin/gql.py
+-rw-r--r--   0        0        0      681 2023-05-07 15:56:40.250091 cluedin-0.2.1/cluedin/urls.py
+-rw-r--r--   0        0        0      264 2023-05-06 19:41:45.000595 cluedin-0.2.1/cluedin/utils.py
+-rw-r--r--   0        0        0      292 2023-05-07 18:00:27.016967 cluedin-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2372 1970-01-01 00:00:00.000000 cluedin-0.2.1/PKG-INFO
```

### Comparing `cluedin-0.2.0/cluedin/auth.py` & `cluedin-0.2.1/cluedin/auth.py`

 * *Files identical despite different names*

### Comparing `cluedin-0.2.0/cluedin/gql.py` & `cluedin-0.2.1/cluedin/gql.py`

 * *Files identical despite different names*

### Comparing `cluedin-0.2.0/cluedin/urls.py` & `cluedin-0.2.1/cluedin/urls.py`

 * *Files identical despite different names*

