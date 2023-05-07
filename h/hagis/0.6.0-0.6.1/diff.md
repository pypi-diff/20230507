# Comparing `tmp/hagis-0.6.0.tar.gz` & `tmp/hagis-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagis-0.6.0.tar", last modified: Sun May  7 12:19:54 2023, max compression
+gzip compressed data, was "hagis-0.6.1.tar", last modified: Sun May  7 12:31:58 2023, max compression
```

## Comparing `hagis-0.6.0.tar` & `hagis-0.6.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 12:19:54.608316 hagis-0.6.0/
--rw-rw-rw-   0        0        0      923 2023-05-07 12:19:54.608316 hagis-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 12:19:54.597082 hagis-0.6.0/hagis.egg-info/
--rw-rw-rw-   0        0        0      923 2023-05-07 12:19:54.000000 hagis-0.6.0/hagis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-05-07 12:19:54.000000 hagis-0.6.0/hagis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 12:19:54.000000 hagis-0.6.0/hagis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-07 12:19:54.000000 hagis-0.6.0/hagis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    22212 2023-05-07 12:18:26.000000 hagis-0.6.0/hagis.py
--rw-rw-rw-   0        0        0      589 2023-05-07 12:18:38.000000 hagis-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 12:19:54.619452 hagis-0.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 12:31:58.130229 hagis-0.6.1/
+-rw-rw-rw-   0        0        0      923 2023-05-07 12:31:58.128402 hagis-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2023-05-04 16:02:37.000000 hagis-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 12:31:58.120597 hagis-0.6.1/hagis.egg-info/
+-rw-rw-rw-   0        0        0      923 2023-05-07 12:31:58.000000 hagis-0.6.1/hagis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      149 2023-05-07 12:31:58.000000 hagis-0.6.1/hagis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 12:31:58.000000 hagis-0.6.1/hagis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-07 12:31:58.000000 hagis-0.6.1/hagis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    22308 2023-05-07 12:30:18.000000 hagis-0.6.1/hagis.py
+-rw-rw-rw-   0        0        0      589 2023-05-07 12:30:56.000000 hagis-0.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 12:31:58.130229 hagis-0.6.1/setup.cfg
```

### Comparing `hagis-0.6.0/PKG-INFO` & `hagis-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.6.0
+Version: 0.6.1
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.6.0/hagis.egg-info/PKG-INFO` & `hagis-0.6.1/hagis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagis
-Version: 0.6.0
+Version: 0.6.1
 Summary: A high availability GIS client
 Author-email: Jiro Shirota <jshirota@gmail.com>
 Project-URL: Homepage, https://github.com/jshirota/Hagis
 Project-URL: Bug Tracker, https://github.com/jshirota/Hagis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hagis-0.6.0/hagis.py` & `hagis-0.6.1/hagis.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,16 +156,17 @@
 
         for row in islice(self._query(where_clause, fields, record_count, max_workers, **kwargs), record_count):
             if self._is_dynamic:
                 yield row  # type: ignore
             else:
                 if self._has_parameterless_constructor:
                     item = self._model()
+                    row_dict = {key.lower(): value for key, value in row.__dict__.items()}
                     for property_name, field_name in self._fields.items():
-                        setattr(item, property_name, row.__dict__[field_name])
+                        setattr(item, property_name, row_dict[field_name.lower()])
                 else:
                     # Support for data classes and named tuples.
                     item = self._model(*row.__dict__.values())
 
                 yield item
 
     def count(self, where_clause: Union[str, Callable[[T], bool], None] = None) -> int:
```

### Comparing `hagis-0.6.0/pyproject.toml` & `hagis-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hagis"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "A high availability GIS client"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

