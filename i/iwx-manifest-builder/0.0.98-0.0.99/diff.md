# Comparing `tmp/iwx_manifest_builder-0.0.98.tar.gz` & `tmp/iwx_manifest_builder-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iwx_manifest_builder-0.0.98.tar", max compression
+gzip compressed data, was "iwx_manifest_builder-0.0.99.tar", max compression
```

## Comparing `iwx_manifest_builder-0.0.98.tar` & `iwx_manifest_builder-0.0.99.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1082 2022-12-27 18:38:25.825136 iwx_manifest_builder-0.0.98/LICENSE
--rw-r--r--   0        0        0      139 2022-12-27 18:38:25.825136 iwx_manifest_builder-0.0.98/README.md
--rw-r--r--   0        0        0        0 2022-12-27 18:38:25.825136 iwx_manifest_builder-0.0.98/iwx_manifest_builder/__init__.py
--rw-r--r--   0        0        0      281 2022-12-27 18:38:25.825136 iwx_manifest_builder-0.0.98/iwx_manifest_builder/schema/bbox_coord_schema.py
--rw-r--r--   0        0        0      332 2022-12-27 18:38:25.825136 iwx_manifest_builder-0.0.98/iwx_manifest_builder/schema/bbox_pixels_coord_schema.py
--rw-r--r--   0        0        0      206 2022-12-27 18:38:25.825136 iwx_manifest_builder-0.0.98/iwx_manifest_builder/schema/category_schema.py
--rw-r--r--   0        0        0      702 2022-12-27 18:38:25.825136 iwx_manifest_builder-0.0.98/iwx_manifest_builder/schema/document/detection_schema.py
--rw-r--r--   0        0        0      255 2022-12-27 18:38:25.825136 iwx_manifest_builder-0.0.98/iwx_manifest_builder/schema/image_schema.py
--rw-r--r--   0        0        0      296 2022-12-27 18:38:25.825136 iwx_manifest_builder-0.0.98/iwx_manifest_builder/schema/inferred_schema.py
--rw-r--r--   0        0        0     2485 2022-12-27 18:38:25.825136 iwx_manifest_builder-0.0.98/iwx_manifest_builder/schema/maxar_feature_schema.py
--rw-r--r--   0        0        0      219 2022-12-27 18:38:25.825136 iwx_manifest_builder-0.0.98/iwx_manifest_builder/schema/point_coord_schema.py
--rw-r--r--   0        0        0      145 2022-12-27 18:38:25.825136 iwx_manifest_builder-0.0.98/iwx_manifest_builder/schema/polygon_coord_schema.py
--rw-r--r--   0        0        0      211 2022-12-27 18:38:25.825136 iwx_manifest_builder-0.0.98/iwx_manifest_builder/schema/workflow_schema.py
--rw-r--r--   0        0        0      978 2022-12-27 18:38:26.517140 iwx_manifest_builder-0.0.98/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 iwx_manifest_builder-0.0.98/setup.py
--rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 iwx_manifest_builder-0.0.98/PKG-INFO
+-rw-r--r--   0        0        0     1082 2022-12-29 02:06:49.518006 iwx_manifest_builder-0.0.99/LICENSE
+-rw-r--r--   0        0        0      139 2022-12-29 02:06:49.518006 iwx_manifest_builder-0.0.99/README.md
+-rw-r--r--   0        0        0        0 2022-12-29 02:06:49.518006 iwx_manifest_builder-0.0.99/iwx_manifest_builder/__init__.py
+-rw-r--r--   0        0        0      281 2022-12-29 02:06:49.518006 iwx_manifest_builder-0.0.99/iwx_manifest_builder/schema/bbox_coord_schema.py
+-rw-r--r--   0        0        0      332 2022-12-29 02:06:49.518006 iwx_manifest_builder-0.0.99/iwx_manifest_builder/schema/bbox_pixels_coord_schema.py
+-rw-r--r--   0        0        0      206 2022-12-29 02:06:49.518006 iwx_manifest_builder-0.0.99/iwx_manifest_builder/schema/category_schema.py
+-rw-r--r--   0        0        0      702 2022-12-29 02:06:49.518006 iwx_manifest_builder-0.0.99/iwx_manifest_builder/schema/document/detection_schema.py
+-rw-r--r--   0        0        0      255 2022-12-29 02:06:49.518006 iwx_manifest_builder-0.0.99/iwx_manifest_builder/schema/image_schema.py
+-rw-r--r--   0        0        0      296 2022-12-29 02:06:49.518006 iwx_manifest_builder-0.0.99/iwx_manifest_builder/schema/inferred_schema.py
+-rw-r--r--   0        0        0     2485 2022-12-29 02:06:49.518006 iwx_manifest_builder-0.0.99/iwx_manifest_builder/schema/maxar_feature_schema.py
+-rw-r--r--   0        0        0      219 2022-12-29 02:06:49.518006 iwx_manifest_builder-0.0.99/iwx_manifest_builder/schema/point_coord_schema.py
+-rw-r--r--   0        0        0      145 2022-12-29 02:06:49.518006 iwx_manifest_builder-0.0.99/iwx_manifest_builder/schema/polygon_coord_schema.py
+-rw-r--r--   0        0        0      211 2022-12-29 02:06:49.518006 iwx_manifest_builder-0.0.99/iwx_manifest_builder/schema/workflow_schema.py
+-rw-r--r--   0        0        0      978 2022-12-29 02:06:50.058014 iwx_manifest_builder-0.0.99/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 iwx_manifest_builder-0.0.99/setup.py
+-rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 iwx_manifest_builder-0.0.99/PKG-INFO
```

### Comparing `iwx_manifest_builder-0.0.98/LICENSE` & `iwx_manifest_builder-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `iwx_manifest_builder-0.0.98/iwx_manifest_builder/schema/document/detection_schema.py` & `iwx_manifest_builder-0.0.99/iwx_manifest_builder/schema/document/detection_schema.py`

 * *Files identical despite different names*

### Comparing `iwx_manifest_builder-0.0.98/iwx_manifest_builder/schema/maxar_feature_schema.py` & `iwx_manifest_builder-0.0.99/iwx_manifest_builder/schema/maxar_feature_schema.py`

 * *Files identical despite different names*

### Comparing `iwx_manifest_builder-0.0.98/pyproject.toml` & `iwx_manifest_builder-0.0.99/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iwx-manifest-builder"
-version = "v0.0.98"
+version = "v0.0.99"
 description = "Validates data used in building an iwx manifest file."
 authors = ["Michael Mohamed <michael@foundationstack.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fsai-dev/fsai-cli-tools"
 repository = "https://github.com/fsai-dev/fsai-cli-tools"
```

### Comparing `iwx_manifest_builder-0.0.98/setup.py` & `iwx_manifest_builder-0.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ['beartype>=0.10.4,<0.11.0',
  'loguru>=0.6.0,<0.7.0',
  'marshmallow-jsonschema>=0.13.0,<0.14.0',
  'marshmallow>=3.15.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'iwx-manifest-builder',
-    'version': '0.0.98',
+    'version': '0.0.99',
     'description': 'Validates data used in building an iwx manifest file.',
     'long_description': '# iwx-manifest-builder\n\nThs Internal Workflow Exchange library provides schemas needed to validate the data passed between FSAI workflows. ',
     'author': 'Michael Mohamed',
     'author_email': 'michael@foundationstack.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fsai-dev/fsai-cli-tools',
```

### Comparing `iwx_manifest_builder-0.0.98/PKG-INFO` & `iwx_manifest_builder-0.0.99/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iwx-manifest-builder
-Version: 0.0.98
+Version: 0.0.99
 Summary: Validates data used in building an iwx manifest file.
 Home-page: https://github.com/fsai-dev/fsai-cli-tools
 License: MIT
 Author: Michael Mohamed
 Author-email: michael@foundationstack.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

