# Comparing `tmp/dxsp-2.0.3.tar.gz` & `tmp/dxsp-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.0.3.tar", max compression
+gzip compressed data, was "dxsp-2.0.4.tar", max compression
```

## Comparing `dxsp-2.0.3.tar` & `dxsp-2.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-07 19:57:35.733774 dxsp-2.0.3/LICENSE
--rw-r--r--   0        0        0     3349 2023-05-07 19:57:35.733774 dxsp-2.0.3/README.md
--rw-r--r--   0        0        0       86 2023-05-07 19:57:36.397783 dxsp-2.0.3/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-07 19:57:35.733774 dxsp-2.0.3/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-07 19:57:35.733774 dxsp-2.0.3/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-07 19:57:35.733774 dxsp-2.0.3/dxsp/config.py
--rw-r--r--   0        0        0     2967 2023-05-07 19:57:35.733774 dxsp-2.0.3/dxsp/default_settings.toml
--rw-r--r--   0        0        0    26224 2023-05-07 19:57:35.733774 dxsp-2.0.3/dxsp/main.py
--rw-r--r--   0        0        0     1769 2023-05-07 19:57:36.397783 dxsp-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 dxsp-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-07 20:04:55.556050 dxsp-2.0.4/LICENSE
+-rw-r--r--   0        0        0     3349 2023-05-07 20:04:55.556050 dxsp-2.0.4/README.md
+-rw-r--r--   0        0        0       86 2023-05-07 20:04:56.360065 dxsp-2.0.4/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-07 20:04:55.556050 dxsp-2.0.4/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-07 20:04:55.556050 dxsp-2.0.4/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-07 20:04:55.556050 dxsp-2.0.4/dxsp/config.py
+-rw-r--r--   0        0        0     2967 2023-05-07 20:04:55.556050 dxsp-2.0.4/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    26224 2023-05-07 20:04:55.556050 dxsp-2.0.4/dxsp/main.py
+-rw-r--r--   0        0        0     1790 2023-05-07 20:04:56.360065 dxsp-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 dxsp-2.0.4/PKG-INFO
```

### Comparing `dxsp-2.0.3/LICENSE` & `dxsp-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.3/README.md` & `dxsp-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.3/dxsp/assets/blockchains.py` & `dxsp-2.0.4/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.3/dxsp/default_settings.toml` & `dxsp-2.0.4/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.3/dxsp/main.py` & `dxsp-2.0.4/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.0.3/pyproject.toml` & `dxsp-2.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.0.3"
+version = "2.0.4"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
@@ -25,14 +25,15 @@
 # apollox-connector-python = "*"
 
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "*"
 pytest = "*"
 pytest-cov = "*"
+pytest-asyncio = "*"
 
 [tool.pytest.ini_options]
 testpaths = "tests/"
 python_classes = [
   "Test*",
   "*Test"
 ]
```

### Comparing `dxsp-2.0.3/PKG-INFO` & `dxsp-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.0.3
+Version: 2.0.4
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

