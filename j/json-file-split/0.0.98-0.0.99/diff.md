# Comparing `tmp/json_file_split-0.0.98.tar.gz` & `tmp/json_file_split-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_file_split-0.0.98.tar", max compression
+gzip compressed data, was "json_file_split-0.0.99.tar", max compression
```

## Comparing `json_file_split-0.0.98.tar` & `json_file_split-0.0.99.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1076 2022-12-27 18:38:27.622148 json_file_split-0.0.98/LICENSE
--rw-r--r--   0        0        0      319 2022-12-27 18:38:27.622148 json_file_split-0.0.98/README.md
--rw-r--r--   0        0        0        0 2022-12-27 18:38:27.622148 json_file_split-0.0.98/json_file_split/__init__.py
--rw-r--r--   0        0        0     3310 2022-12-27 18:38:27.622148 json_file_split-0.0.98/json_file_split/main.py
--rw-r--r--   0        0        0     1931 2022-12-27 18:38:27.622148 json_file_split-0.0.98/json_file_split/split_libs/jsonl_split.py
--rw-r--r--   0        0        0     1004 2022-12-27 18:38:28.374156 json_file_split-0.0.98/pyproject.toml
--rw-r--r--   0        0        0     1255 1970-01-01 00:00:00.000000 json_file_split-0.0.98/setup.py
--rw-r--r--   0        0        0     1190 1970-01-01 00:00:00.000000 json_file_split-0.0.98/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-12-29 02:06:47.930551 json_file_split-0.0.99/LICENSE
+-rw-r--r--   0        0        0      319 2022-12-29 02:06:47.930551 json_file_split-0.0.99/README.md
+-rw-r--r--   0        0        0        0 2022-12-29 02:06:47.930551 json_file_split-0.0.99/json_file_split/__init__.py
+-rw-r--r--   0        0        0     3310 2022-12-29 02:06:47.930551 json_file_split-0.0.99/json_file_split/main.py
+-rw-r--r--   0        0        0     1931 2022-12-29 02:06:47.930551 json_file_split-0.0.99/json_file_split/split_libs/jsonl_split.py
+-rw-r--r--   0        0        0     1004 2022-12-29 02:06:48.486549 json_file_split-0.0.99/pyproject.toml
+-rw-r--r--   0        0        0     1255 1970-01-01 00:00:00.000000 json_file_split-0.0.99/setup.py
+-rw-r--r--   0        0        0     1190 1970-01-01 00:00:00.000000 json_file_split-0.0.99/PKG-INFO
```

### Comparing `json_file_split-0.0.98/LICENSE` & `json_file_split-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `json_file_split-0.0.98/json_file_split/main.py` & `json_file_split-0.0.99/json_file_split/main.py`

 * *Files identical despite different names*

### Comparing `json_file_split-0.0.98/json_file_split/split_libs/jsonl_split.py` & `json_file_split-0.0.99/json_file_split/split_libs/jsonl_split.py`

 * *Files identical despite different names*

### Comparing `json_file_split-0.0.98/pyproject.toml` & `json_file_split-0.0.99/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "json-file-split"
-version = "v0.0.98"
+version = "v0.0.99"
 description = "Split a json or jsonl file into equal chunks."
 authors = ["Michael Mohamed <michael@foundationstack.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/fsai-dev/fsai-cli-tools"
 repository = "https://github.com/fsai-dev/fsai-cli-tools"
```

### Comparing `json_file_split-0.0.98/setup.py` & `json_file_split-0.0.99/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'loguru>=0.6.0,<0.7.0']
 
 entry_points = \
 {'console_scripts': ['json-file-split = json_file_split.main:app']}
 
 setup_kwargs = {
     'name': 'json-file-split',
-    'version': '0.0.98',
+    'version': '0.0.99',
     'description': 'Split a json or jsonl file into equal chunks.',
     'long_description': '# json-file-split\nSplit a json or jsonl file into different chunks.\n\n## Installation \n```shell\npip install json-file-split\n```\n\n## Usage\n```shell\njson-file-split \\\n--input_file_path ./tests/data/test.jsonl \\\n--save_to_dir /tmp/output/ \\\n--output_file_name test.jsonl \\\n--split_by number_of_buckets \\\n--batch_size 10\n```',
     'author': 'Michael Mohamed',
     'author_email': 'michael@foundationstack.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fsai-dev/fsai-cli-tools',
```

### Comparing `json_file_split-0.0.98/PKG-INFO` & `json_file_split-0.0.99/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-file-split
-Version: 0.0.98
+Version: 0.0.99
 Summary: Split a json or jsonl file into equal chunks.
 Home-page: https://github.com/fsai-dev/fsai-cli-tools
 License: MIT
 Author: Michael Mohamed
 Author-email: michael@foundationstack.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

