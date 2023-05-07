# Comparing `tmp/geopix-0.0.98.tar.gz` & `tmp/geopix-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geopix-0.0.98.tar", max compression
+gzip compressed data, was "geopix-0.0.99.tar", max compression
```

## Comparing `geopix-0.0.98.tar` & `geopix-0.0.99.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1076 2022-12-27 18:38:20.942232 geopix-0.0.98/LICENSE
--rw-r--r--   0        0        0       86 2022-12-27 18:38:20.942232 geopix-0.0.98/README.md
--rw-r--r--   0        0        0        0 2022-12-27 18:38:20.942232 geopix-0.0.98/geopix/__init__.py
--rw-r--r--   0        0        0     4645 2022-12-27 18:38:20.942232 geopix-0.0.98/geopix/geopix.py
--rw-r--r--   0        0        0      916 2022-12-27 18:38:21.510242 geopix-0.0.98/pyproject.toml
--rw-r--r--   0        0        0      822 1970-01-01 00:00:00.000000 geopix-0.0.98/setup.py
--rw-r--r--   0        0        0      915 1970-01-01 00:00:00.000000 geopix-0.0.98/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-12-29 02:06:49.941089 geopix-0.0.99/LICENSE
+-rw-r--r--   0        0        0       86 2022-12-29 02:06:49.941089 geopix-0.0.99/README.md
+-rw-r--r--   0        0        0        0 2022-12-29 02:06:49.941089 geopix-0.0.99/geopix/__init__.py
+-rw-r--r--   0        0        0     4645 2022-12-29 02:06:49.941089 geopix-0.0.99/geopix/geopix.py
+-rw-r--r--   0        0        0      916 2022-12-29 02:06:50.493092 geopix-0.0.99/pyproject.toml
+-rw-r--r--   0        0        0      822 1970-01-01 00:00:00.000000 geopix-0.0.99/setup.py
+-rw-r--r--   0        0        0      915 1970-01-01 00:00:00.000000 geopix-0.0.99/PKG-INFO
```

### Comparing `geopix-0.0.98/LICENSE` & `geopix-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `geopix-0.0.98/geopix/geopix.py` & `geopix-0.0.99/geopix/geopix.py`

 * *Files identical despite different names*

### Comparing `geopix-0.0.98/pyproject.toml` & `geopix-0.0.99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geopix"
-version = "v0.0.98"
+version = "v0.0.99"
 description = "Helper functions to convert geo coords to pixel coords and back."
 authors = ["Michael Mohamed <michael@foundationstack.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/fsai-dev/fsai-cli-tools"
 repository = "https://github.com/fsai-dev/fsai-cli-tools"
```

### Comparing `geopix-0.0.98/setup.py` & `geopix-0.0.99/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['beartype>=0.10.4,<0.11.0', 'loguru>=0.6.0,<0.7.0']
 
 setup_kwargs = {
     'name': 'geopix',
-    'version': '0.0.98',
+    'version': '0.0.99',
     'description': 'Helper functions to convert geo coords to pixel coords and back.',
     'long_description': '# geopix\n\n## Installation\n```sh\npip install geopix\n```\n\n## Getting Started\nSee tests.\n',
     'author': 'Michael Mohamed',
     'author_email': 'michael@foundationstack.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fsai-dev/fsai-cli-tools',
```

### Comparing `geopix-0.0.98/PKG-INFO` & `geopix-0.0.99/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geopix
-Version: 0.0.98
+Version: 0.0.99
 Summary: Helper functions to convert geo coords to pixel coords and back.
 Home-page: https://github.com/fsai-dev/fsai-cli-tools
 License: MIT
 Author: Michael Mohamed
 Author-email: michael@foundationstack.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

