# Comparing `tmp/hagis-0.5.5.tar.gz` & `tmp/hagis-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.5.5.tar", last modified: Sat May  6 10:56:22 2023, max compression
+gzip compressed data, was "hagis-0.5.6.tar", last modified: Sun May  7 10:50:24 2023, max compression
```

## Comparing `hagis-0.5.5.tar` & `hagis-0.5.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 10:56:22.379643 hagis-0.5.5/
--rw-rw-rw-   0        0        0      923 2023-05-06 10:56:22.377826 hagis-0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.5.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 10:56:22.368994 hagis-0.5.5/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-05-06 10:56:22.000000 hagis-0.5.5/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-05-06 10:56:22.000000 hagis-0.5.5/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 10:56:22.000000 hagis-0.5.5/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-06 10:56:22.000000 hagis-0.5.5/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    22398 2023-05-06 10:55:25.000000 hagis-0.5.5/hagis.py
--rw-rw-rw-   0        0        0      589 2023-05-06 10:54:02.000000 hagis-0.5.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 10:56:22.379643 hagis-0.5.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 10:50:24.436859 hagis-0.5.6/
+-rw-rw-rw-   0        0        0      923 2023-05-07 10:50:24.432139 hagis-0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.5.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 10:50:24.421668 hagis-0.5.6/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-05-07 10:50:24.000000 hagis-0.5.6/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-05-07 10:50:24.000000 hagis-0.5.6/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 10:50:24.000000 hagis-0.5.6/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-07 10:50:24.000000 hagis-0.5.6/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    22495 2023-05-07 10:42:56.000000 hagis-0.5.6/hagis.py
+-rw-rw-rw-   0        0        0      589 2023-05-07 10:49:11.000000 hagis-0.5.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 10:50:24.437352 hagis-0.5.6/setup.cfg
```

### Comparing `hagis-0.5.5/PKG-INFO` & `hagis-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.5.5
+Version: 0.5.6
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.5.5/hagis.egg-info/PKG-INFO` & `hagis-0.5.6/hagis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.5.5
+Version: 0.5.6
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.5.5/hagis.py` & `hagis-0.5.6/hagis.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,27 +336,29 @@
         return (obj.features, obj.exceededTransferLimit if hasattr(obj, "exceededTransferLimit") else False)
 
     def _get_oids(self, where_clause: str) -> List[int]:
         obj = self._call("query", where=where_clause, returnIdsOnly="true")
         return obj.objectIds
 
     def _map(self, row: SimpleNamespace) -> SimpleNamespace:
+        attributes = {key.lower(): value for key, value in row.attributes.__dict__.items()}
+
         if not hasattr(row, "geometry"):
-            return row.attributes
+            return SimpleNamespace(**attributes)
 
         if self._shape_property_type is None or self._shape_property_type in self._unknown_shape_types:
             shape = row.geometry
         else:
             if self._is_arcgis_gemetry:
                 shape = self._shape_property_type(row.geometry.__dict__)
             else:
                 shape = self._shape_property_type()
                 shape.__dict__ = row.geometry.__dict__
 
-        return SimpleNamespace(**row.attributes.__dict__, **{self._shape_property_name: shape})
+        return SimpleNamespace(**attributes, **{self._shape_property_name: shape})
 
     def _query(self, where_clause: str, fields: str, record_count: Optional[int], max_workers: Optional[int],
                **kwargs: Any) -> Iterator[SimpleNamespace]:
         def get_rows(where_clause: str):
             return self._get_rows(where_clause, fields, **kwargs)
 
         rows, exceeded_transfer_limit = get_rows(where_clause)
```

### Comparing `hagis-0.5.5/pyproject.toml` & `hagis-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.5.5"
+version = "0.5.6"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

