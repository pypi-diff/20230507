# Comparing `tmp/hagis-0.5.7.tar.gz` & `tmp/hagis-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.5.7.tar", last modified: Sun May  7 11:46:44 2023, max compression
+gzip compressed data, was "hagis-0.6.0.tar", last modified: Sun May  7 12:19:54 2023, max compression
```

## Comparing `hagis-0.5.7.tar` & `hagis-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 11:46:44.806627 hagis-0.5.7/
--rw-rw-rw-   0        0        0      923 2023-05-07 11:46:44.805897 hagis-0.5.7/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.5.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 11:46:44.797569 hagis-0.5.7/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-05-07 11:46:44.000000 hagis-0.5.7/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-05-07 11:46:44.000000 hagis-0.5.7/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 11:46:44.000000 hagis-0.5.7/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-07 11:46:44.000000 hagis-0.5.7/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    22388 2023-05-07 11:44:51.000000 hagis-0.5.7/hagis.py
--rw-rw-rw-   0        0        0      589 2023-05-07 11:46:02.000000 hagis-0.5.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 11:46:44.806627 hagis-0.5.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 12:19:54.608316 hagis-0.6.0/
+-rw-rw-rw-   0        0        0      923 2023-05-07 12:19:54.608316 hagis-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 12:19:54.597082 hagis-0.6.0/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-05-07 12:19:54.000000 hagis-0.6.0/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-05-07 12:19:54.000000 hagis-0.6.0/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 12:19:54.000000 hagis-0.6.0/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-07 12:19:54.000000 hagis-0.6.0/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    22212 2023-05-07 12:18:26.000000 hagis-0.6.0/hagis.py
+-rw-rw-rw-   0        0        0      589 2023-05-07 12:18:38.000000 hagis-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 12:19:54.619452 hagis-0.6.0/setup.cfg
```

### Comparing `hagis-0.5.7/PKG-INFO` & `hagis-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.5.7
+Version: 0.6.0
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.5.7/hagis.egg-info/PKG-INFO` & `hagis-0.6.0/hagis.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.5.7
+Version: 0.6.0
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.5.7/hagis.py` & `hagis-0.6.0/hagis.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,33 +52,31 @@
 
         # List of custom mapping properties that have been handled.
         mapped: List[str] = []
 
         for model_type in reversed(model.mro()):
             if hasattr(model_type, "__annotations__"):
                 for property_name, property_type in model_type.__annotations__.items():
-                    key = property_name.lower()
-
                     if property_name in mapping:
-                        self._fields[key] = mapping[property_name]
+                        self._fields[property_name] = mapping[property_name]
                         mapped.append(property_name)
                     else:
-                        self._fields[key] = property_name
+                        self._fields[property_name] = property_name
 
-                    if key == shape_property_name.lower():
+                    if property_name.lower() == shape_property_name.lower():
                         self._shape_property_name = property_name
                         self._shape_property_type = property_type
 
         self._is_arcgis_gemetry = hasattr(self._shape_property_type, "__module__")\
             and self._shape_property_type.__module__.startswith("arcgis.geometry.")
 
         # Add custom properties that have not been handled as dynamically handled propeties.
         for property_name, field in mapping.items():
             if property_name not in mapped:
-                self._fields[property_name.lower()] = field
+                self._fields[property_name] = field
 
     _token_cache: Dict[Tuple[str, str], Tuple[str, int]] = {}
 
     def set_token_generator(self, username: str, password: str, referer: str = "",
                             token_url: str = "https://www.arcgis.com/sharing/generateToken", **kwargs: Any) -> None:
         """ Sets the token generation parameters.
 
@@ -142,15 +140,15 @@
             return
 
         if self._is_dynamic:
             # If dynamic, request all fields.
             fields = "*"
         else:
             # Otherwise, request only what is used by the model.
-            fields = ",".join([f for (_, f) in self._fields.items() if f != self._shape_property_name.lower()])
+            fields = ",".join([f for f in self._fields.values() if f.lower() != self._shape_property_name.lower()])
             if not self._shape_property_name:
                 kwargs["returnGeometry"] = False
 
         if record_count:
             kwargs["resultRecordCount"] = record_count
 
         if wkid:
@@ -158,17 +156,16 @@
 
         for row in islice(self._query(where_clause, fields, record_count, max_workers, **kwargs), record_count):
             if self._is_dynamic:
                 yield row  # type: ignore
             else:
                 if self._has_parameterless_constructor:
                     item = self._model()
-                    row_dict = {key.lower(): value for key, value in row.__dict__.items()}
                     for property_name, field_name in self._fields.items():
-                        setattr(item, property_name, row_dict[field_name])
+                        setattr(item, property_name, row.__dict__[field_name])
                 else:
                     # Support for data classes and named tuples.
                     item = self._model(*row.__dict__.values())
 
                 yield item
 
     def count(self, where_clause: Union[str, Callable[[T], bool], None] = None) -> int:
@@ -278,17 +275,16 @@
     def _to_dict(self, item: T) -> Dict[str, Any]:
         dictionary: Dict[str, Any] = {}
         attributes: Dict[str, Any] = {}
 
         dictionary["attributes"] = attributes
 
         for key, value in item.__dict__.items():
-            lower_property_name = key.lower()
-            field = self._fields[lower_property_name]
-            if lower_property_name == self._shape_property_name.lower():
+            field = self._fields[key]
+            if key.lower() == self._shape_property_name.lower():
                 if self._is_arcgis_gemetry:
                     dictionary["geometry"] = loads(value.JSON)
                 else:
                     dictionary["geometry"] = value.__dict__
             elif isinstance(value, datetime):
                 attributes[field] = int((value - datetime.utcfromtimestamp(0)).total_seconds() * 1000)
             else:
```

### Comparing `hagis-0.5.7/pyproject.toml` & `hagis-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.5.7"
+version = "0.6.0"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

