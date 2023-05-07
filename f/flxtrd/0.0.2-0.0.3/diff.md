# Comparing `tmp/flxtrd-0.0.2.tar.gz` & `tmp/flxtrd-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flxtrd-0.0.2.tar", max compression
+gzip compressed data, was "flxtrd-0.0.3.tar", max compression
```

## Comparing `flxtrd-0.0.2.tar` & `flxtrd-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     9135 2023-05-05 08:04:47.294863 flxtrd-0.0.2/LICENSE
--rw-r--r--   0        0        0     2547 2023-05-07 17:50:02.220036 flxtrd-0.0.2/README.md
--rw-r--r--   0        0        0     1883 2023-05-07 17:55:20.495107 flxtrd-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-07 17:55:35.934823 flxtrd-0.0.2/src/__init__.py
--rw-r--r--   0        0        0     3267 1970-01-01 00:00:00.000000 flxtrd-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     9135 2023-05-05 08:04:47.294863 flxtrd-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2637 2023-05-07 17:59:58.410005 flxtrd-0.0.3/README.md
+-rw-r--r--   0        0        0     1883 2023-05-07 18:00:34.383985 flxtrd-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-07 17:55:35.934823 flxtrd-0.0.3/src/__init__.py
+-rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 flxtrd-0.0.3/PKG-INFO
```

### Comparing `flxtrd-0.0.2/LICENSE` & `flxtrd-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flxtrd-0.0.2/README.md` & `flxtrd-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# flxtrd
+# GLocalFlexTrade Public API 
+
+Trade energy or offer flexible loads to the European energy market.
 
 [![Release](https://img.shields.io/github/v/release/glocalflex/flxtrd)](https://img.shields.io/github/v/release/glocalflex/flxtrd)
 [![Build status](https://img.shields.io/github/actions/workflow/status/glocalflex/flxtrd/main.yml?branch=main)](https://github.com/glocalflex/flxtrd/actions/workflows/main.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/glocalflex/flxtrd/branch/main/graph/badge.svg)](https://codecov.io/gh/glocalflex/flxtrd)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/glocalflex/flxtrd)](https://img.shields.io/github/commit-activity/m/glocalflex/flxtrd)
 [![License](https://img.shields.io/github/license/glocalflex/flxtrd)](https://img.shields.io/github/license/glocalflex/flxtrd)
```

### Comparing `flxtrd-0.0.2/pyproject.toml` & `flxtrd-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flxtrd"
-version = "0.0.2"
+version = "0.0.3"
 description = "Public client API for the flexible energy trading market GLocalFlex."
 authors = ["glocalflex"]
 repository = "https://github.com/glocalflex/flxtrade"
 documentation = "https://glocalflex.github.io/flxtrade/"
 readme = "README.md"
 packages = [
   {include = "src"}
```

### Comparing `flxtrd-0.0.2/PKG-INFO` & `flxtrd-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flxtrd
-Version: 0.0.2
+Version: 0.0.3
 Summary: Public client API for the flexible energy trading market GLocalFlex.
 Home-page: https://github.com/glocalflex/flxtrade
 Author: glocalflex
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -12,15 +12,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pika (>=1.3.1,<2.0.0)
 Requires-Dist: requests (>=2.28.0)
 Project-URL: Documentation, https://glocalflex.github.io/flxtrade/
 Project-URL: Repository, https://github.com/glocalflex/flxtrade
 Description-Content-Type: text/markdown
 
-# flxtrd
+# GLocalFlexTrade Public API 
+
+Trade energy or offer flexible loads to the European energy market.
 
 [![Release](https://img.shields.io/github/v/release/glocalflex/flxtrd)](https://img.shields.io/github/v/release/glocalflex/flxtrd)
 [![Build status](https://img.shields.io/github/actions/workflow/status/glocalflex/flxtrd/main.yml?branch=main)](https://github.com/glocalflex/flxtrd/actions/workflows/main.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/glocalflex/flxtrd/branch/main/graph/badge.svg)](https://codecov.io/gh/glocalflex/flxtrd)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/glocalflex/flxtrd)](https://img.shields.io/github/commit-activity/m/glocalflex/flxtrd)
 [![License](https://img.shields.io/github/license/glocalflex/flxtrd)](https://img.shields.io/github/license/glocalflex/flxtrd)
```

