# Comparing `tmp/recursive_validator-0.0.98.tar.gz` & `tmp/recursive_validator-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recursive_validator-0.0.98.tar", max compression
+gzip compressed data, was "recursive_validator-0.0.99.tar", max compression
```

## Comparing `recursive_validator-0.0.98.tar` & `recursive_validator-0.0.99.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1082 2022-12-27 18:38:22.821406 recursive_validator-0.0.98/LICENSE
--rw-r--r--   0        0        0      158 2022-12-27 18:38:22.821406 recursive_validator-0.0.98/README.md
--rw-r--r--   0        0        0      972 2022-12-27 18:38:23.389403 recursive_validator-0.0.98/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-27 18:38:22.821406 recursive_validator-0.0.98/recursive_validator/__init__.py
--rw-r--r--   0        0        0      709 2022-12-27 18:38:22.821406 recursive_validator-0.0.98/recursive_validator/helpers/data_helpers.py
--rw-r--r--   0        0        0     1268 2022-12-27 18:38:22.821406 recursive_validator-0.0.98/recursive_validator/helpers/file_helpers.py
--rw-r--r--   0        0        0      965 2022-12-27 18:38:22.821406 recursive_validator-0.0.98/recursive_validator/helpers/log_helpers.py
--rw-r--r--   0        0        0     2823 2022-12-27 18:38:22.821406 recursive_validator-0.0.98/recursive_validator/recursive_validator.py
--rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 recursive_validator-0.0.98/setup.py
--rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 recursive_validator-0.0.98/PKG-INFO
+-rw-r--r--   0        0        0     1082 2022-12-29 02:06:50.414983 recursive_validator-0.0.99/LICENSE
+-rw-r--r--   0        0        0      158 2022-12-29 02:06:50.414983 recursive_validator-0.0.99/README.md
+-rw-r--r--   0        0        0      972 2022-12-29 02:06:50.970979 recursive_validator-0.0.99/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-29 02:06:50.414983 recursive_validator-0.0.99/recursive_validator/__init__.py
+-rw-r--r--   0        0        0      709 2022-12-29 02:06:50.414983 recursive_validator-0.0.99/recursive_validator/helpers/data_helpers.py
+-rw-r--r--   0        0        0     1268 2022-12-29 02:06:50.414983 recursive_validator-0.0.99/recursive_validator/helpers/file_helpers.py
+-rw-r--r--   0        0        0      965 2022-12-29 02:06:50.414983 recursive_validator-0.0.99/recursive_validator/helpers/log_helpers.py
+-rw-r--r--   0        0        0     2823 2022-12-29 02:06:50.418983 recursive_validator-0.0.99/recursive_validator/recursive_validator.py
+-rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 recursive_validator-0.0.99/setup.py
+-rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 recursive_validator-0.0.99/PKG-INFO
```

### Comparing `recursive_validator-0.0.98/LICENSE` & `recursive_validator-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `recursive_validator-0.0.98/pyproject.toml` & `recursive_validator-0.0.99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "recursive-validator"
-version = "v0.0.98"
+version = "v0.0.99"
 description = ""
 authors = ["Michael Mohamed <michael@foundationstack.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fsai-dev/fsai-cli-tools"
 repository = "https://github.com/fsai-dev/fsai-cli-tools"
```

### Comparing `recursive_validator-0.0.98/recursive_validator/helpers/data_helpers.py` & `recursive_validator-0.0.99/recursive_validator/helpers/data_helpers.py`

 * *Files identical despite different names*

### Comparing `recursive_validator-0.0.98/recursive_validator/helpers/file_helpers.py` & `recursive_validator-0.0.99/recursive_validator/helpers/file_helpers.py`

 * *Files identical despite different names*

### Comparing `recursive_validator-0.0.98/recursive_validator/helpers/log_helpers.py` & `recursive_validator-0.0.99/recursive_validator/helpers/log_helpers.py`

 * *Files identical despite different names*

### Comparing `recursive_validator-0.0.98/recursive_validator/recursive_validator.py` & `recursive_validator-0.0.99/recursive_validator/recursive_validator.py`

 * *Files identical despite different names*

### Comparing `recursive_validator-0.0.98/setup.py` & `recursive_validator-0.0.99/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 entry_points = \
 {'console_scripts': ['recursive-validator = '
                      'recursive_validator.recursive_validator:app']}
 
 setup_kwargs = {
     'name': 'recursive-validator',
-    'version': '0.0.98',
+    'version': '0.0.99',
     'description': '',
     'long_description': "```shell\npython main.py \\\n--include_patterns '*.yml,*.yaml' \\\n--exclude_patterns '*/backups/*' \\\n--loaders_path ./loaders \\\n--input_directory ./my-project\n```",
     'author': 'Michael Mohamed',
     'author_email': 'michael@foundationstack.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fsai-dev/fsai-cli-tools',
```

### Comparing `recursive_validator-0.0.98/PKG-INFO` & `recursive_validator-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recursive-validator
-Version: 0.0.98
+Version: 0.0.99
 Summary: 
 Home-page: https://github.com/fsai-dev/fsai-cli-tools
 License: MIT
 Author: Michael Mohamed
 Author-email: michael@foundationstack.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

