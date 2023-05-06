# Comparing `tmp/spotON_sdk-0.0.1.2.tar.gz` & `tmp/spotON_sdk-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.1.2.tar", last modified: Sat May  6 22:41:49 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.1.3.tar", last modified: Sat May  6 22:45:52 2023, max compression
```

## Comparing `spotON_sdk-0.0.1.2.tar` & `spotON_sdk-0.0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     6171 2023-05-06 14:09:02.618269 spotON_sdk-0.0.1.2/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.1.2/LICENSE
--rw-r--r--   0        0        0      361 2023-05-06 22:41:38.203364 spotON_sdk-0.0.1.2/pyproject.toml
--rw-r--r--   0        0        0      390 2023-05-06 22:35:35.239243 spotON_sdk-0.0.1.2/spotON_sdk/__init__.py
--rw-r--r--   0        0        0     2786 2023-05-06 22:41:04.021539 spotON_sdk-0.0.1.2/spotON_sdk/logic/Config.py
--rw-r--r--   0        0        0      218 1970-01-01 00:00:00.000000 spotON_sdk-0.0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6171 2023-05-06 14:09:02.618269 spotON_sdk-0.0.1.3/.gitignore
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.1.3/LICENSE
+-rw-r--r--   0        0        0      345 2023-05-06 22:45:37.572415 spotON_sdk-0.0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      390 2023-05-06 22:45:45.764197 spotON_sdk-0.0.1.3/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0     2786 2023-05-06 22:41:04.021539 spotON_sdk-0.0.1.3/spotON_sdk/logic/Config.py
+-rw-r--r--   0        0        0      218 1970-01-01 00:00:00.000000 spotON_sdk-0.0.1.3/PKG-INFO
```

### Comparing `spotON_sdk-0.0.1.2/.gitignore` & `spotON_sdk-0.0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.1.2/LICENSE` & `spotON_sdk-0.0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.1.2/spotON_sdk/logic/Config.py` & `spotON_sdk-0.0.1.3/spotON_sdk/logic/Config.py`

 * *Files identical despite different names*

