# Comparing `tmp/widelearning-0.6.0.tar.gz` & `tmp/widelearning-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widelearning-0.6.0.tar", max compression
+gzip compressed data, was "widelearning-0.7.5.tar", max compression
```

## Comparing `widelearning-0.6.0.tar` & `widelearning-0.7.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      354 2023-04-27 04:21:13.787954 widelearning-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    74117 2023-04-27 04:13:48.010957 widelearning-0.6.0/widelearning.py
--rw-r--r--   0        0        0      505 2023-04-27 04:21:23.242814 widelearning-0.6.0/setup.py
--rw-r--r--   0        0        0      514 2023-04-27 04:21:23.243043 widelearning-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      354 2023-05-07 04:44:44.856843 widelearning-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0    78935 2023-05-07 04:41:00.260607 widelearning-0.7.5/widelearning.py
+-rw-r--r--   0        0        0      505 2023-05-07 04:45:09.419025 widelearning-0.7.5/setup.py
+-rw-r--r--   0        0        0      514 2023-05-07 04:45:09.419279 widelearning-0.7.5/PKG-INFO
```

### Comparing `widelearning-0.6.0/PKG-INFO` & `widelearning-0.7.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widelearning
-Version: 0.6.0
+Version: 0.7.5
 Summary: Library for searching the optimal neural network architecture
 Author: Brinkinvision
 Author-email: brinkinvision@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
```

