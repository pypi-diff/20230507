# Comparing `tmp/marshy-4.0.2.tar.gz` & `tmp/marshy-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marshy-4.0.2.tar", last modified: Sun May  7 16:11:02 2023, max compression
+gzip compressed data, was "marshy-4.0.3.tar", last modified: Sun May  7 16:21:06 2023, max compression
```

## Comparing `marshy-4.0.2.tar` & `marshy-4.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:11:02.670094 marshy-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-07 16:10:53.000000 marshy-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-07 16:10:53.000000 marshy-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-05-07 16:11:02.670094 marshy-4.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:11:02.666094 marshy-4.0.2/marshy/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:11:02.666094 marshy-4.0.2/marshy/factory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/dataclass_marshaller_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/enum_marshaller_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/factory_marshaller_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/impl_marshaller_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/list_marshaller_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/marshaller_factory_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/optional_marshaller_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/tuple_marshaller_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/factory/union_marshaller_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:11:02.670094 marshy-4.0.2/marshy/marshaller/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/as_str_marshaller.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/bool_marshaller.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/datetime_marshaller.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/deferred_marshaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/enum_marshaller.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/iterable_marshaller.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/json_str_marshaller.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/marshaller_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/no_op_marshaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/obj_marshaller.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/optional_marshaller.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/primitive_marshaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/property_marshaller.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/tuple_marshaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/type_marshaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller/union_marshaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/marshaller_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:11:02.666094 marshy-4.0.2/marshy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-05-07 16:11:02.000000 marshy-4.0.2/marshy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-07 16:11:02.000000 marshy-4.0.2/marshy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 16:11:02.000000 marshy-4.0.2/marshy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-07 16:11:02.000000 marshy-4.0.2/marshy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 16:11:02.000000 marshy-4.0.2/marshy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:11:02.670094 marshy-4.0.2/marshy_config_default/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-07 16:10:53.000000 marshy-4.0.2/marshy_config_default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 16:11:02.670094 marshy-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-07 16:10:53.000000 marshy-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:21:06.802556 marshy-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-07 16:20:57.000000 marshy-4.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-07 16:20:57.000000 marshy-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-05-07 16:21:06.802556 marshy-4.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:21:06.798556 marshy-4.0.3/marshy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:21:06.802556 marshy-4.0.3/marshy/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/factory/dataclass_marshaller_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/factory/enum_marshaller_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/factory/factory_marshaller_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/factory/impl_marshaller_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/factory/list_marshaller_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/factory/marshaller_factory_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/factory/optional_marshaller_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/factory/tuple_marshaller_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/factory/union_marshaller_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:21:06.802556 marshy-4.0.3/marshy/marshaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/marshaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/marshaller/as_str_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/marshaller/bool_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/marshaller/datetime_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/marshaller/deferred_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/marshaller/enum_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/marshaller/iterable_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/marshaller/json_str_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/marshaller/marshaller_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/marshaller/no_op_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/marshaller/obj_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/marshaller/optional_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/marshaller/primitive_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/marshaller/property_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/marshaller/tuple_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/marshaller/type_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/marshaller/union_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/marshaller_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:21:06.798556 marshy-4.0.3/marshy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-05-07 16:21:06.000000 marshy-4.0.3/marshy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-07 16:21:06.000000 marshy-4.0.3/marshy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 16:21:06.000000 marshy-4.0.3/marshy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-07 16:21:06.000000 marshy-4.0.3/marshy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 16:21:06.000000 marshy-4.0.3/marshy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:21:06.802556 marshy-4.0.3/marshy_config_default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-07 16:20:57.000000 marshy-4.0.3/marshy_config_default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 16:21:06.802556 marshy-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-07 16:20:57.000000 marshy-4.0.3/setup.py
```

### Comparing `marshy-4.0.2/LICENSE` & `marshy-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/PKG-INFO` & `marshy-4.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marshy
-Version: 4.0.2
+Version: 4.0.3
 Summary: A convention over configuration approach to object marshalling.
 Home-page: https://github.com/tofarr/marshy
 Author: Tim O'Farrell
 Author-email: tofarr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -289,20 +289,10 @@
 
 
 ## Release Proceedure
 
 ![status](https://github.com/tofarr/marshy/actions/workflows/quality.yml/badge.svg?branch=main)
 
 The typical process here is:
-* Create a PR with changes. Merge these to main (The `Quality` workflows make sure that styling, linting, and code
-  code coverage standards are met).
+* Create a PR with changes. Merge these to main (The `Quality` workflows make sure that your PR
+  meets the styling, linting, and code coverage standards).
 * New releases created in github are automatically uploaded to pypi
-
-
-You need an account on pypi before this will work:
-
-```
-pip install setuptools wheel
-python setup.py sdist bdist_wheel
-pip install twine
-python -m twine upload dist/*
-```
```

### Comparing `marshy-4.0.2/marshy/__init__.py` & `marshy-4.0.3/marshy/__init__.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/factory/dataclass_marshaller_factory.py` & `marshy-4.0.3/marshy/factory/dataclass_marshaller_factory.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/factory/enum_marshaller_factory.py` & `marshy-4.0.3/marshy/factory/enum_marshaller_factory.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/factory/factory_marshaller_factory.py` & `marshy-4.0.3/marshy/factory/factory_marshaller_factory.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/factory/impl_marshaller_factory.py` & `marshy-4.0.3/marshy/factory/impl_marshaller_factory.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/factory/list_marshaller_factory.py` & `marshy-4.0.3/marshy/factory/list_marshaller_factory.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/factory/marshaller_factory_abc.py` & `marshy-4.0.3/marshy/factory/marshaller_factory_abc.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/factory/optional_marshaller_factory.py` & `marshy-4.0.3/marshy/factory/optional_marshaller_factory.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/factory/tuple_marshaller_factory.py` & `marshy-4.0.3/marshy/factory/tuple_marshaller_factory.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/factory/union_marshaller_factory.py` & `marshy-4.0.3/marshy/factory/union_marshaller_factory.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/marshaller/__init__.py` & `marshy-4.0.3/marshy/marshaller/__init__.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/marshaller/datetime_marshaller.py` & `marshy-4.0.3/marshy/marshaller/datetime_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/marshaller/deferred_marshaller.py` & `marshy-4.0.3/marshy/marshaller/deferred_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/marshaller/enum_marshaller.py` & `marshy-4.0.3/marshy/marshaller/enum_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/marshaller/iterable_marshaller.py` & `marshy-4.0.3/marshy/marshaller/iterable_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/marshaller/json_str_marshaller.py` & `marshy-4.0.3/marshy/marshaller/json_str_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/marshaller/obj_marshaller.py` & `marshy-4.0.3/marshy/marshaller/obj_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/marshaller/optional_marshaller.py` & `marshy-4.0.3/marshy/marshaller/optional_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/marshaller/property_marshaller.py` & `marshy-4.0.3/marshy/marshaller/property_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/marshaller/tuple_marshaller.py` & `marshy-4.0.3/marshy/marshaller/tuple_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/marshaller/type_marshaller.py` & `marshy-4.0.3/marshy/marshaller/type_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/marshaller/union_marshaller.py` & `marshy-4.0.3/marshy/marshaller/union_marshaller.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/marshaller_context.py` & `marshy-4.0.3/marshy/marshaller_context.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy/utils.py` & `marshy-4.0.3/marshy/utils.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy.egg-info/PKG-INFO` & `marshy-4.0.3/marshy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marshy
-Version: 4.0.2
+Version: 4.0.3
 Summary: A convention over configuration approach to object marshalling.
 Home-page: https://github.com/tofarr/marshy
 Author: Tim O'Farrell
 Author-email: tofarr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -289,20 +289,10 @@
 
 
 ## Release Proceedure
 
 ![status](https://github.com/tofarr/marshy/actions/workflows/quality.yml/badge.svg?branch=main)
 
 The typical process here is:
-* Create a PR with changes. Merge these to main (The `Quality` workflows make sure that styling, linting, and code
-  code coverage standards are met).
+* Create a PR with changes. Merge these to main (The `Quality` workflows make sure that your PR
+  meets the styling, linting, and code coverage standards).
 * New releases created in github are automatically uploaded to pypi
-
-
-You need an account on pypi before this will work:
-
-```
-pip install setuptools wheel
-python setup.py sdist bdist_wheel
-pip install twine
-python -m twine upload dist/*
-```
```

### Comparing `marshy-4.0.2/marshy.egg-info/SOURCES.txt` & `marshy-4.0.3/marshy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/marshy_config_default/__init__.py` & `marshy-4.0.3/marshy_config_default/__init__.py`

 * *Files identical despite different names*

### Comparing `marshy-4.0.2/setup.py` & `marshy-4.0.3/setup.py`

 * *Files identical despite different names*

