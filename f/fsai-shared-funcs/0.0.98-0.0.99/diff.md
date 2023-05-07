# Comparing `tmp/fsai_shared_funcs-0.0.98.tar.gz` & `tmp/fsai_shared_funcs-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsai_shared_funcs-0.0.98.tar", max compression
+gzip compressed data, was "fsai_shared_funcs-0.0.99.tar", max compression
```

## Comparing `fsai_shared_funcs-0.0.98.tar` & `fsai_shared_funcs-0.0.99.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1082 2022-12-27 18:38:20.375882 fsai_shared_funcs-0.0.98/LICENSE
--rw-r--r--   0        0        0      121 2022-12-27 18:38:20.375882 fsai_shared_funcs-0.0.98/README.md
--rw-r--r--   0        0        0        0 2022-12-27 18:38:20.375882 fsai_shared_funcs-0.0.98/fsai_shared_funcs/__init__.py
--rw-r--r--   0        0        0      216 2022-12-27 18:38:20.375882 fsai_shared_funcs-0.0.98/fsai_shared_funcs/conversion_helper.py
--rw-r--r--   0        0        0     1565 2022-12-27 18:38:20.375882 fsai_shared_funcs-0.0.98/fsai_shared_funcs/database_helper.py
--rw-r--r--   0        0        0      352 2022-12-27 18:38:20.375882 fsai_shared_funcs-0.0.98/fsai_shared_funcs/dict_helper.py
--rw-r--r--   0        0        0     2234 2022-12-27 18:38:20.375882 fsai_shared_funcs-0.0.98/fsai_shared_funcs/file_helper.py
--rw-r--r--   0        0        0      387 2022-12-27 18:38:20.375882 fsai_shared_funcs-0.0.98/fsai_shared_funcs/geo_helper.py
--rw-r--r--   0        0        0     1044 2022-12-27 18:38:20.375882 fsai_shared_funcs-0.0.98/fsai_shared_funcs/json_helper.py
--rw-r--r--   0        0        0        0 2022-12-27 18:38:20.375882 fsai_shared_funcs-0.0.98/fsai_shared_funcs/proto_helpers/__init__.py
--rw-r--r--   0        0        0    40827 2022-12-27 18:38:20.375882 fsai_shared_funcs-0.0.98/fsai_shared_funcs/proto_helpers/json_format.py
--rw-r--r--   0        0        0      469 2022-12-27 18:38:20.375882 fsai_shared_funcs-0.0.98/fsai_shared_funcs/string_helper.py
--rw-r--r--   0        0        0      852 2022-12-27 18:38:20.375882 fsai_shared_funcs-0.0.98/fsai_shared_funcs/time_helper.py
--rw-r--r--   0        0        0      961 2022-12-27 18:38:20.951889 fsai_shared_funcs-0.0.98/pyproject.toml
--rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 fsai_shared_funcs-0.0.98/setup.py
--rw-r--r--   0        0        0     1058 1970-01-01 00:00:00.000000 fsai_shared_funcs-0.0.98/PKG-INFO
+-rw-r--r--   0        0        0     1082 2022-12-29 02:06:52.700279 fsai_shared_funcs-0.0.99/LICENSE
+-rw-r--r--   0        0        0      121 2022-12-29 02:06:52.700279 fsai_shared_funcs-0.0.99/README.md
+-rw-r--r--   0        0        0        0 2022-12-29 02:06:52.700279 fsai_shared_funcs-0.0.99/fsai_shared_funcs/__init__.py
+-rw-r--r--   0        0        0      216 2022-12-29 02:06:52.700279 fsai_shared_funcs-0.0.99/fsai_shared_funcs/conversion_helper.py
+-rw-r--r--   0        0        0     1565 2022-12-29 02:06:52.700279 fsai_shared_funcs-0.0.99/fsai_shared_funcs/database_helper.py
+-rw-r--r--   0        0        0      352 2022-12-29 02:06:52.700279 fsai_shared_funcs-0.0.99/fsai_shared_funcs/dict_helper.py
+-rw-r--r--   0        0        0     2234 2022-12-29 02:06:52.700279 fsai_shared_funcs-0.0.99/fsai_shared_funcs/file_helper.py
+-rw-r--r--   0        0        0      387 2022-12-29 02:06:52.700279 fsai_shared_funcs-0.0.99/fsai_shared_funcs/geo_helper.py
+-rw-r--r--   0        0        0     1044 2022-12-29 02:06:52.700279 fsai_shared_funcs-0.0.99/fsai_shared_funcs/json_helper.py
+-rw-r--r--   0        0        0        0 2022-12-29 02:06:52.700279 fsai_shared_funcs-0.0.99/fsai_shared_funcs/proto_helpers/__init__.py
+-rw-r--r--   0        0        0    40827 2022-12-29 02:06:52.700279 fsai_shared_funcs-0.0.99/fsai_shared_funcs/proto_helpers/json_format.py
+-rw-r--r--   0        0        0      469 2022-12-29 02:06:52.700279 fsai_shared_funcs-0.0.99/fsai_shared_funcs/string_helper.py
+-rw-r--r--   0        0        0      852 2022-12-29 02:06:52.700279 fsai_shared_funcs-0.0.99/fsai_shared_funcs/time_helper.py
+-rw-r--r--   0        0        0      961 2022-12-29 02:06:53.388311 fsai_shared_funcs-0.0.99/pyproject.toml
+-rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 fsai_shared_funcs-0.0.99/setup.py
+-rw-r--r--   0        0        0     1058 1970-01-01 00:00:00.000000 fsai_shared_funcs-0.0.99/PKG-INFO
```

### Comparing `fsai_shared_funcs-0.0.98/LICENSE` & `fsai_shared_funcs-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `fsai_shared_funcs-0.0.98/fsai_shared_funcs/database_helper.py` & `fsai_shared_funcs-0.0.99/fsai_shared_funcs/database_helper.py`

 * *Files identical despite different names*

### Comparing `fsai_shared_funcs-0.0.98/fsai_shared_funcs/file_helper.py` & `fsai_shared_funcs-0.0.99/fsai_shared_funcs/file_helper.py`

 * *Files identical despite different names*

### Comparing `fsai_shared_funcs-0.0.98/fsai_shared_funcs/json_helper.py` & `fsai_shared_funcs-0.0.99/fsai_shared_funcs/json_helper.py`

 * *Files identical despite different names*

### Comparing `fsai_shared_funcs-0.0.98/fsai_shared_funcs/proto_helpers/json_format.py` & `fsai_shared_funcs-0.0.99/fsai_shared_funcs/proto_helpers/json_format.py`

 * *Files identical despite different names*

### Comparing `fsai_shared_funcs-0.0.98/fsai_shared_funcs/time_helper.py` & `fsai_shared_funcs-0.0.99/fsai_shared_funcs/time_helper.py`

 * *Files identical despite different names*

### Comparing `fsai_shared_funcs-0.0.98/pyproject.toml` & `fsai_shared_funcs-0.0.99/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fsai-shared-funcs"
-version = "v0.0.98"
+version = "v0.0.99"
 description = "Simple functions shared across fsai apps."
 authors = ["Michael Mohamed <michael@foundationstack.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fsai-dev/fsai-cli-tools"
 repository = "https://github.com/fsai-dev/fsai-cli-tools"
```

### Comparing `fsai_shared_funcs-0.0.98/setup.py` & `fsai_shared_funcs-0.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'google>=3.0.0,<4.0.0',
  'jsonlines>=3.1.0,<4.0.0',
  'loguru>=0.6.0,<0.7.0',
  'pydash>=5.1.0,<6.0.0']
 
 setup_kwargs = {
     'name': 'fsai-shared-funcs',
-    'version': '0.0.98',
+    'version': '0.0.99',
     'description': 'Simple functions shared across fsai apps.',
     'long_description': '# fsai-shared-funcs\n\nSimple functions shared across fsai apps.\n\n## Installation\n```shell\npoetry add fsai-shared-funcs\n```',
     'author': 'Michael Mohamed',
     'author_email': 'michael@foundationstack.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fsai-dev/fsai-cli-tools',
```

### Comparing `fsai_shared_funcs-0.0.98/PKG-INFO` & `fsai_shared_funcs-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsai-shared-funcs
-Version: 0.0.98
+Version: 0.0.99
 Summary: Simple functions shared across fsai apps.
 Home-page: https://github.com/fsai-dev/fsai-cli-tools
 License: MIT
 Author: Michael Mohamed
 Author-email: michael@foundationstack.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

