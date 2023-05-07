# Comparing `tmp/cvat_manifest_builder-0.0.98.tar.gz` & `tmp/cvat_manifest_builder-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvat_manifest_builder-0.0.98.tar", max compression
+gzip compressed data, was "cvat_manifest_builder-0.0.99.tar", max compression
```

## Comparing `cvat_manifest_builder-0.0.98.tar` & `cvat_manifest_builder-0.0.99.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1082 2022-12-27 18:38:23.153719 cvat_manifest_builder-0.0.98/LICENSE
--rw-r--r--   0        0        0      626 2022-12-27 18:38:23.153719 cvat_manifest_builder-0.0.98/README.md
--rw-r--r--   0        0        0        0 2022-12-27 18:38:23.153719 cvat_manifest_builder-0.0.98/cvat_manifest_builder/__init__.py
--rw-r--r--   0        0        0     3770 2022-12-27 18:38:23.153719 cvat_manifest_builder-0.0.98/cvat_manifest_builder/cvat_manifest_builder.py
--rw-r--r--   0        0        0     1037 2022-12-27 18:38:23.753723 cvat_manifest_builder-0.0.98/pyproject.toml
--rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 cvat_manifest_builder-0.0.98/setup.py
--rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 cvat_manifest_builder-0.0.98/PKG-INFO
+-rw-r--r--   0        0        0     1082 2022-12-29 02:06:51.071356 cvat_manifest_builder-0.0.99/LICENSE
+-rw-r--r--   0        0        0      626 2022-12-29 02:06:51.071356 cvat_manifest_builder-0.0.99/README.md
+-rw-r--r--   0        0        0        0 2022-12-29 02:06:51.071356 cvat_manifest_builder-0.0.99/cvat_manifest_builder/__init__.py
+-rw-r--r--   0        0        0     3770 2022-12-29 02:06:51.071356 cvat_manifest_builder-0.0.99/cvat_manifest_builder/cvat_manifest_builder.py
+-rw-r--r--   0        0        0     1037 2022-12-29 02:06:51.719363 cvat_manifest_builder-0.0.99/pyproject.toml
+-rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 cvat_manifest_builder-0.0.99/setup.py
+-rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 cvat_manifest_builder-0.0.99/PKG-INFO
```

### Comparing `cvat_manifest_builder-0.0.98/LICENSE` & `cvat_manifest_builder-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cvat_manifest_builder-0.0.98/README.md` & `cvat_manifest_builder-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `cvat_manifest_builder-0.0.98/cvat_manifest_builder/cvat_manifest_builder.py` & `cvat_manifest_builder-0.0.99/cvat_manifest_builder/cvat_manifest_builder.py`

 * *Files identical despite different names*

### Comparing `cvat_manifest_builder-0.0.98/pyproject.toml` & `cvat_manifest_builder-0.0.99/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvat-manifest-builder"
-version = "v0.0.98"
+version = "v0.0.99"
 description = "Builds a CVAT manifest file from a directory of images."
 authors = ["Michael Mohamed <michael@foundationstack.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fsai-dev/fsai-cli-tools"
 repository = "https://github.com/fsai-dev/fsai-cli-tools"
```

### Comparing `cvat_manifest_builder-0.0.98/setup.py` & `cvat_manifest_builder-0.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 entry_points = \
 {'console_scripts': ['cvat-manifest-builder = '
                      'cvat_manifest_builder.cvat_manifest_builder:app']}
 
 setup_kwargs = {
     'name': 'cvat-manifest-builder',
-    'version': '0.0.98',
+    'version': '0.0.99',
     'description': 'Builds a CVAT manifest file from a directory of images.',
     'long_description': '# cvat-manifest-builder\n## Installation & Use\n\n```shell\n# Install cvat-manifest-builder\n> pip install cvat-manifest-builder\n\n> cvat-manifest-builder --help\nusage: cvat-manifest-builder [-h] --output_manifest_file OUTPUT_MANIFEST_FILE --input_data_path\n                             INPUT_DATA_PATH\n\nBuilds a CVAT manifest file from a directory of images.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --output_manifest_file OUTPUT_MANIFEST_FILE\n                        Path to the output manifest file.\n  --input_data_path INPUT_DATA_PATH\n                        Path to the data directory.\n```',
     'author': 'Michael Mohamed',
     'author_email': 'michael@foundationstack.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fsai-dev/fsai-cli-tools',
```

### Comparing `cvat_manifest_builder-0.0.98/PKG-INFO` & `cvat_manifest_builder-0.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvat-manifest-builder
-Version: 0.0.98
+Version: 0.0.99
 Summary: Builds a CVAT manifest file from a directory of images.
 Home-page: https://github.com/fsai-dev/fsai-cli-tools
 License: MIT
 Author: Michael Mohamed
 Author-email: michael@foundationstack.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

