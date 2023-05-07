# Comparing `tmp/schemey-6.0.1.tar.gz` & `tmp/schemey-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/schemey-6.0.1.tar", last modified: Tue Apr 18 21:32:51 2023, max compression
+gzip compressed data, was "schemey-6.0.2.tar", last modified: Sun May  7 17:03:16 2023, max compression
```

## Comparing `schemey-6.0.1.tar` & `schemey-6.0.2.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:32:51.000000 schemey-6.0.1/
--rw-r--r--   0 tofarr     (501) staff       (20)     3879 2023-04-18 21:32:51.000000 schemey-6.0.1/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)     3441 2023-01-15 16:34:55.000000 schemey-6.0.1/README.md
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:32:51.000000 schemey-6.0.1/marshy_config_schemey/
--rw-r--r--   0 tofarr     (501) staff       (20)      225 2022-07-28 13:03:35.000000 schemey-6.0.1/marshy_config_schemey/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey/
--rw-r--r--   0 tofarr     (501) staff       (20)     1414 2022-07-28 21:35:38.000000 schemey-6.0.1/schemey/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey/factory/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-07-27 21:59:06.000000 schemey-6.0.1/schemey/factory/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1398 2023-01-15 15:35:44.000000 schemey-6.0.1/schemey/factory/any_of_schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2926 2023-01-15 15:27:56.000000 schemey-6.0.1/schemey/factory/array_schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     5118 2023-01-15 15:35:53.000000 schemey-6.0.1/schemey/factory/dataclass_schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1036 2023-01-15 15:27:52.000000 schemey-6.0.1/schemey/factory/datetime_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1260 2023-04-18 21:19:24.000000 schemey-6.0.1/schemey/factory/enum_schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1216 2023-01-15 15:28:00.000000 schemey-6.0.1/schemey/factory/external_type_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      874 2022-12-23 00:16:46.000000 schemey-6.0.1/schemey/factory/factory_schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2695 2023-01-15 15:27:40.000000 schemey-6.0.1/schemey/factory/impl_schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      767 2022-12-23 00:16:46.000000 schemey-6.0.1/schemey/factory/ref_schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1052 2022-12-22 23:47:30.000000 schemey-6.0.1/schemey/factory/schema_factory_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      960 2023-01-15 15:27:44.000000 schemey-6.0.1/schemey/factory/simple_type_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1744 2023-01-15 15:27:47.000000 schemey-6.0.1/schemey/factory/tuple_schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1003 2023-01-15 15:27:49.000000 schemey-6.0.1/schemey/factory/uuid_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey/json_schema/
--rw-r--r--   0 tofarr     (501) staff       (20)      291 2023-01-15 15:42:18.000000 schemey-6.0.1/schemey/json_schema/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1185 2023-01-15 16:41:29.000000 schemey-6.0.1/schemey/json_schema/ranges.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1943 2023-01-15 17:25:49.000000 schemey-6.0.1/schemey/json_schema/timestamp.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3707 2023-03-11 00:43:10.000000 schemey-6.0.1/schemey/schema.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1831 2023-01-15 15:13:45.000000 schemey-6.0.1/schemey/schema_context.py
--rw-r--r--   0 tofarr     (501) staff       (20)      653 2022-07-29 12:27:06.000000 schemey-6.0.1/schemey/schema_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      459 2022-11-30 22:21:30.000000 schemey-6.0.1/schemey/schemey_format_checker.py
--rw-r--r--   0 tofarr     (501) staff       (20)      230 2022-07-15 12:34:09.000000 schemey-6.0.1/schemey/string_format.py
--rw-r--r--   0 tofarr     (501) staff       (20)      109 2022-07-28 13:07:38.000000 schemey-6.0.1/schemey/util.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3016 2022-12-23 00:16:46.000000 schemey-6.0.1/schemey/validated.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1755 2022-07-28 21:44:55.000000 schemey-6.0.1/schemey/validator.py
--rw-r--r--   0 tofarr     (501) staff       (20)       22 2023-04-18 21:32:19.000000 schemey-6.0.1/schemey/version.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey.egg-info/
--rw-r--r--   0 tofarr     (501) staff       (20)     3879 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey.egg-info/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)     1102 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey.egg-info/SOURCES.txt
--rw-r--r--   0 tofarr     (501) staff       (20)        1 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey.egg-info/dependency_links.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       28 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey.egg-info/requires.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       53 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey.egg-info/top_level.txt
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey_config_default/
--rw-r--r--   0 tofarr     (501) staff       (20)     2079 2023-01-15 15:58:18.000000 schemey-6.0.1/schemey_config_default/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)       38 2023-04-18 21:32:51.000000 schemey-6.0.1/setup.cfg
--rw-r--r--   0 tofarr     (501) staff       (20)      763 2023-04-18 21:32:19.000000 schemey-6.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:03:16.991970 schemey-6.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-07 17:03:06.000000 schemey-6.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-07 17:03:16.987970 schemey-6.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:03:16.983970 schemey-6.0.2/marshy_config_schemey/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-07 17:03:06.000000 schemey-6.0.2/marshy_config_schemey/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:03:16.987970 schemey-6.0.2/schemey/
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:03:16.987970 schemey-6.0.2/schemey/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/factory/any_of_schema_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/factory/array_schema_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/factory/dataclass_schema_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/factory/datetime_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/factory/enum_schema_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/factory/external_type_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/factory/factory_schema_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/factory/impl_schema_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/factory/ref_schema_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/factory/schema_factory_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/factory/simple_type_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/factory/tuple_schema_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/factory/uuid_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:03:16.987970 schemey-6.0.2/schemey/json_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/json_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/json_schema/ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/json_schema/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/schema_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/schema_marshaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/schemey_format_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/string_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/validated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:03:16.987970 schemey-6.0.2/schemey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-07 17:03:16.000000 schemey-6.0.2/schemey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-07 17:03:16.000000 schemey-6.0.2/schemey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 17:03:16.000000 schemey-6.0.2/schemey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-07 17:03:16.000000 schemey-6.0.2/schemey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-07 17:03:16.000000 schemey-6.0.2/schemey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:03:16.987970 schemey-6.0.2/schemey_config_default/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-07 17:03:06.000000 schemey-6.0.2/schemey_config_default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 17:03:16.991970 schemey-6.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-07 17:03:06.000000 schemey-6.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `schemey-6.0.1/PKG-INFO` & `schemey-6.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: schemey
-Version: 6.0.1
+Version: 6.0.2
 Summary: Convention over configuration Object Schemas for python
 Home-page: https://github.com/tofarr/schemey
 Author: Tim O'Farrell
 Author-email: tofarr@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 
 # Schemey - Json Schemas for Python.
 
 This project allows for generation of json schemas based on python
 classes, or python classes based on json schemas. It also allows for
 generation of validated dataclasses, where setters cannot violate
 the invariants established in a schema.
@@ -93,18 +93,21 @@
     context.factories = [
         f for f in context.factories 
         if 'uuid' not in f.__class__.__name__.lower()
     ]
 
 ```
 
-## Building The Project
-
-You need an account on pypi before this will work:
+## Installing local development dependencies
 
 ```
-pip install setuptools wheel
-python setup.py sdist bdist_wheel
-pip install twine
-python -m twine upload dist/*
+python setup.py install easy_install "schemey[dev]"
 ```
 
+## Release Procedure
+
+![status](https://github.com/tofarr/schemey/actions/workflows/quality.yml/badge.svg?branch=main)
+
+The typical process here is:
+* Create a PR with changes. Merge these to main (The `Quality` workflows make sure that your PR
+  meets the styling, linting, and code coverage standards).
+* New releases created in github are automatically uploaded to pypi
```

### Comparing `schemey-6.0.1/README.md` & `schemey-6.0.2/schemey.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: schemey
+Version: 6.0.2
+Summary: Convention over configuration Object Schemas for python
+Home-page: https://github.com/tofarr/schemey
+Author: Tim O'Farrell
+Author-email: tofarr@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
 # Schemey - Json Schemas for Python.
 
 This project allows for generation of json schemas based on python
 classes, or python classes based on json schemas. It also allows for
 generation of validated dataclasses, where setters cannot violate
 the invariants established in a schema.
 
@@ -79,17 +93,21 @@
     context.factories = [
         f for f in context.factories 
         if 'uuid' not in f.__class__.__name__.lower()
     ]
 
 ```
 
-## Building The Project
-
-You need an account on pypi before this will work:
+## Installing local development dependencies
 
 ```
-pip install setuptools wheel
-python setup.py sdist bdist_wheel
-pip install twine
-python -m twine upload dist/*
-```
+python setup.py install easy_install "schemey[dev]"
+```
+
+## Release Procedure
+
+![status](https://github.com/tofarr/schemey/actions/workflows/quality.yml/badge.svg?branch=main)
+
+The typical process here is:
+* Create a PR with changes. Merge these to main (The `Quality` workflows make sure that your PR
+  meets the styling, linting, and code coverage standards).
+* New releases created in github are automatically uploaded to pypi
```

### Comparing `schemey-6.0.1/schemey/__init__.py` & `schemey-6.0.2/schemey/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from schemey.schema import Schema
 from schemey.schema_context import SchemaContext
 
 _default_context = None
 CONFIG_MODULE_PREFIX = "schemey_config_"
 
 
+# pylint: disable=W0603
 def get_default_schema_context() -> SchemaContext:
     global _default_context
     if not _default_context:
         _default_context = new_default_schema_context()
     return _default_context
```

### Comparing `schemey-6.0.1/schemey/factory/any_of_schema_factory.py` & `schemey-6.0.2/schemey/factory/any_of_schema_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.1/schemey/factory/array_schema_factory.py` & `schemey-6.0.2/schemey/factory/array_schema_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         self,
         type_: Type,
         context: SchemaContext,
         path: str,
         ref_schemas: Dict[Type, Schema],
     ) -> Optional[Schema]:
         array_type = self.get_array_type(type_)
+        # pylint: disable=W0125
         if array_type:
             schema = {"type": "array"}
             args = typing_inspect.get_args(type_)
             if args:
                 item_type = resolve_forward_refs(args[0])
                 if item_type and not typing_inspect.is_typevar(item_type):
                     item_schema = context.schema_from_type(
```

### Comparing `schemey-6.0.1/schemey/factory/dataclass_schema_factory.py` & `schemey-6.0.2/schemey/factory/dataclass_schema_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
             "required": required,
         }
         if type_.__doc__:
             schema["description"] = type_.__doc__.strip()
         schema = Schema(schema, type_)
         return schema
 
+    # pylint: disable=R0914
     def from_json(
         self,
         item: ExternalItemType,
         context: SchemaContext,
         path: str,
         ref_schemas: Dict[str, Schema],
     ) -> Optional[Schema]:
```

### Comparing `schemey-6.0.1/schemey/factory/datetime_factory.py` & `schemey-6.0.2/schemey/factory/datetime_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.1/schemey/factory/enum_schema_factory.py` & `schemey-6.0.2/schemey/factory/enum_schema_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         type_: Type,
         context: SchemaContext,
         path: str,
         ref_schemas: Dict[Type, Schema],
     ) -> Optional[Schema]:
         if isclass(type_) and issubclass(type_, Enum):
             # noinspection PyTypeChecker
-            schema = dict(name=type_.__name__, enum=[e.name for e in type_])
+            schema = {"name": type_.__name__, "enum": [e.name for e in type_]}
             return Schema(schema, type_)
 
     def from_json(
         self,
         item: ExternalItemType,
         context: SchemaContext,
         path: str,
```

### Comparing `schemey-6.0.1/schemey/factory/external_type_factory.py` & `schemey-6.0.2/schemey/factory/external_type_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         type_: Type,
         context: SchemaContext,
         path: str,
         ref_schemas: Dict[Type, Schema],
     ) -> Optional[Schema]:
         if type_ == ExternalItemType:
             return Schema({"type": "object", "additionalProperties": True}, type_)
-        elif type_ == ExternalType:
+        if type_ == ExternalType:
             return Schema({}, type_)
 
     def from_json(
         self,
         item: ExternalItemType,
         context: SchemaContext,
         path: str,
```

### Comparing `schemey-6.0.1/schemey/factory/factory_schema_factory.py` & `schemey-6.0.2/schemey/factory/factory_schema_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.1/schemey/factory/impl_schema_factory.py` & `schemey-6.0.2/schemey/factory/impl_schema_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.1/schemey/factory/ref_schema_factory.py` & `schemey-6.0.2/schemey/factory/ref_schema_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.1/schemey/factory/schema_factory_abc.py` & `schemey-6.0.2/schemey/factory/schema_factory_abc.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.1/schemey/factory/simple_type_factory.py` & `schemey-6.0.2/schemey/factory/simple_type_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.1/schemey/factory/tuple_schema_factory.py` & `schemey-6.0.2/schemey/factory/tuple_schema_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.1/schemey/factory/uuid_factory.py` & `schemey-6.0.2/schemey/factory/uuid_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.1/schemey/json_schema/ranges.py` & `schemey-6.0.2/schemey/json_schema/ranges.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,25 +18,26 @@
 """
 from jsonschema import ValidationError
 
 
 def ranges(validator, aP, instance, schema):
     if not validator.is_type(instance, "object"):
         return
-    ranges_ = schema.get('ranges') or []
+    ranges_ = schema.get("ranges") or []
     for range_ in ranges_:
-        min_property = range_['minProperty']
-        max_property = range_['maxProperty']
-        allow_equal = range_.get('allowEqual')
+        min_property = range_["minProperty"]
+        max_property = range_["maxProperty"]
+        allow_equal = range_.get("allowEqual")
         min_value = instance.get(min_property)
         max_value = instance.get(max_property)
         if min_value < max_value:
             continue
         if allow_equal and min_value == max_value:
             continue
+        # pylint: disable=R0801
         yield ValidationError(
             f"Value not in future: {instance}",
             validator=validator,
             validator_value=aP,
             instance=instance,
             schema=schema,
         )
```

### Comparing `schemey-6.0.1/schemey/json_schema/timestamp.py` & `schemey-6.0.2/schemey/json_schema/timestamp.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,48 +25,49 @@
 from jsonschema import ValidationError
 
 
 def timestamp(validator, aP, instance, schema):
     """
     Check a timestamp. If times are not specified, it is assumed to be utc.
     """
-    format_ = schema.get('format')
-    if format_ not in ('date-time', 'date'):
+    format_ = schema.get("format")
+    if format_ not in ("date-time", "date"):
         yield ValidationError(
             f"Not a date / date-time: {schema}",
             validator=validator,
             validator_value=aP,
             instance=instance,
             schema=schema,
         )
         return
-    timestamp_ = schema['timestamp']
+    timestamp_ = schema["timestamp"]
     now = datetime.now(tz=timezone.utc)
     value = datetime.fromisoformat(instance)
     if not value.tzinfo:
         value = value.replace(tzinfo=timezone.utc)
-    if format_ == 'date':
+    if format_ == "date":
         now.replace(hour=0, minute=0, second=0, microsecond=0)
         value.replace(hour=0, minute=0, second=0, microsecond=0)
     now = now.timestamp()
     value = value.timestamp()
 
-    grace_period_seconds = timestamp_.get('gracePeriodSeconds') or 0
-    past = timestamp_.get('past')
+    grace_period_seconds = timestamp_.get("gracePeriodSeconds") or 0
+    past = timestamp_.get("past")
     if past:
         if value > (now + grace_period_seconds):
             yield ValidationError(
                 f"Value not in past: {instance}",
                 validator=validator,
                 validator_value=aP,
                 instance=instance,
                 schema=schema,
             )
     else:
         if value < (now - grace_period_seconds):
+            # pylint: disable=R0801
             yield ValidationError(
                 f"Value not in future: {instance}",
                 validator=validator,
                 validator_value=aP,
                 instance=instance,
                 schema=schema,
             )
```

### Comparing `schemey-6.0.1/schemey/schema.py` & `schemey-6.0.2/schemey/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,19 +101,21 @@
 
 
 def datetime_schema():
     return Schema({"type": "string", "format": "date-time"}, datetime)
 
 
 def optional_schema(schema: Schema):
-    """ Wrap a simple schema in an optional schema. Does NOT work for schemas which contain refs. """
-    json_schema = dict(anyOf=[
-        {"type": "null"},
-        schema.schema,
-    ])
+    """Wrap a simple schema in an optional schema. Does NOT work for schemas which contain refs."""
+    json_schema = {
+        "anyOf": [
+            {"type": "null"},
+            schema.schema,
+        ]
+    }
     return Schema(json_schema, Optional[schema.python_type])
 
 
 def update_refs(schema: ExternalType, from_location: str, to_location: str):
     """Swap a referenced schema from one location to another"""
     if isinstance(schema, dict):
         schema = {
```

### Comparing `schemey-6.0.1/schemey/schema_context.py` & `schemey-6.0.2/schemey/schema_context.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.1/schemey/schema_marshaller.py` & `schemey-6.0.2/schemey/schema_marshaller.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.1/schemey/validated.py` & `schemey-6.0.2/schemey/validated.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 
 
 def validated(cls: Type[T], schema_context: Optional[SchemaContext] = None):
     if schema_context is None:
         schema_context = get_default_schema_context()
 
     def wrap(cls_):
+        # pylint: disable=C0415,R0401
         from schemey.validator import Validator
 
         if not dataclasses.is_dataclass(cls_):
             cls_ = dataclass(cls_)
         marshaller_context = schema_context.marshaller_context
         schema = schema_context.schema_from_type(cls_)
         properties = schema.schema["properties"]
```

### Comparing `schemey-6.0.1/schemey/validator.py` & `schemey-6.0.2/schemey/validator.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.1/schemey.egg-info/SOURCES.txt` & `schemey-6.0.2/schemey.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-README.md
+MANIFEST.in
 setup.py
 marshy_config_schemey/__init__.py
 schemey/__init__.py
 schemey/schema.py
 schemey/schema_context.py
 schemey/schema_marshaller.py
 schemey/schemey_format_checker.py
 schemey/string_format.py
 schemey/util.py
 schemey/validated.py
 schemey/validator.py
-schemey/version.py
 schemey.egg-info/PKG-INFO
 schemey.egg-info/SOURCES.txt
 schemey.egg-info/dependency_links.txt
 schemey.egg-info/requires.txt
 schemey.egg-info/top_level.txt
 schemey/factory/__init__.py
 schemey/factory/any_of_schema_factory.py
```

### Comparing `schemey-6.0.1/schemey_config_default/__init__.py` & `schemey-6.0.2/schemey_config_default/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,9 +32,9 @@
     context.register_factory(ExternalTypeFactory())
     context.register_factory(DataclassSchemaFactory())
     context.register_factory(EnumSchemaFactory())
     context.register_factory(FactorySchemaFactory())
     context.register_factory(ImplSchemaFactory())
     context.register_factory(AnyOfSchemaFactory())
 
-    register_custom_json_schema_validator('timestamp', timestamp)
-    register_custom_json_schema_validator('ranges', ranges)
+    register_custom_json_schema_validator("timestamp", timestamp)
+    register_custom_json_schema_validator("ranges", ranges)
```

