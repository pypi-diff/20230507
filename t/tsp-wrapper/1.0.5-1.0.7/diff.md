# Comparing `tmp/tsp_wrapper-1.0.5.tar.gz` & `tmp/tsp_wrapper-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsp_wrapper-1.0.5.tar", last modified: Sun May  7 18:13:44 2023, max compression
+gzip compressed data, was "tsp_wrapper-1.0.7.tar", last modified: Sun May  7 19:34:43 2023, max compression
```

## Comparing `tsp_wrapper-1.0.5.tar` & `tsp_wrapper-1.0.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:13:44.011498 tsp_wrapper-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-07 18:13:44.011498 tsp_wrapper-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-07 18:13:44.011498 tsp_wrapper-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:13:44.007498 tsp_wrapper-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:13:44.007498 tsp_wrapper-1.0.5/src/tsp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:13:44.007498 tsp_wrapper-1.0.5/src/tsp_wrapper/broker/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/broker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/broker/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/broker/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/broker/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/broker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:13:44.007498 tsp_wrapper-1.0.5/src/tsp_wrapper/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/conf/global_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:13:44.007498 tsp_wrapper-1.0.5/src/tsp_wrapper/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:13:44.011498 tsp_wrapper-1.0.5/src/tsp_wrapper/core/management/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/core/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/core/management/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:13:44.011498 tsp_wrapper-1.0.5/src/tsp_wrapper/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/middleware/dict_to_city.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/middleware/euclidean_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/middleware/tsp_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:13:44.011498 tsp_wrapper-1.0.5/src/tsp_wrapper/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/tasks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/tasks/tsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:13:44.011498 tsp_wrapper-1.0.5/src/tsp_wrapper/tsp/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/tsp/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/tsp/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/tsp/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/tsp/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/tsp/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:13:44.011498 tsp_wrapper-1.0.5/src/tsp_wrapper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-07 18:13:32.000000 tsp_wrapper-1.0.5/src/tsp_wrapper/utils/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:13:44.007498 tsp_wrapper-1.0.5/src/tsp_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-07 18:13:43.000000 tsp_wrapper-1.0.5/src/tsp_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-07 18:13:44.000000 tsp_wrapper-1.0.5/src/tsp_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 18:13:43.000000 tsp_wrapper-1.0.5/src/tsp_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 18:13:43.000000 tsp_wrapper-1.0.5/src/tsp_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 18:13:43.000000 tsp_wrapper-1.0.5/src/tsp_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:34:43.470799 tsp_wrapper-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-07 19:34:43.470799 tsp_wrapper-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-07 19:34:43.470799 tsp_wrapper-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:34:43.466799 tsp_wrapper-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:34:43.466799 tsp_wrapper-1.0.7/src/tsp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:34:43.470799 tsp_wrapper-1.0.7/src/tsp_wrapper/broker/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/broker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/broker/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/broker/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/broker/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/broker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:34:43.470799 tsp_wrapper-1.0.7/src/tsp_wrapper/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/conf/global_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:34:43.470799 tsp_wrapper-1.0.7/src/tsp_wrapper/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:34:43.470799 tsp_wrapper-1.0.7/src/tsp_wrapper/core/management/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/core/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/core/management/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:34:43.470799 tsp_wrapper-1.0.7/src/tsp_wrapper/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/middleware/dict_to_city.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/middleware/euclidean_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/middleware/tsp_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:34:43.470799 tsp_wrapper-1.0.7/src/tsp_wrapper/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/tasks/tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:34:43.470799 tsp_wrapper-1.0.7/src/tsp_wrapper/tsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/tsp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/tsp/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/tsp/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/tsp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/tsp/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:34:43.470799 tsp_wrapper-1.0.7/src/tsp_wrapper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-07 19:34:34.000000 tsp_wrapper-1.0.7/src/tsp_wrapper/utils/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:34:43.466799 tsp_wrapper-1.0.7/src/tsp_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-07 19:34:43.000000 tsp_wrapper-1.0.7/src/tsp_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-07 19:34:43.000000 tsp_wrapper-1.0.7/src/tsp_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 19:34:43.000000 tsp_wrapper-1.0.7/src/tsp_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 19:34:43.000000 tsp_wrapper-1.0.7/src/tsp_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 19:34:43.000000 tsp_wrapper-1.0.7/src/tsp_wrapper.egg-info/top_level.txt
```

### Comparing `tsp_wrapper-1.0.5/PKG-INFO` & `tsp_wrapper-1.0.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsp_wrapper
-Version: 1.0.5
+Version: 1.0.7
 Summary: tsp_wrapper is a pipeline tsp solver
 Home-page: https://github.com/daneah/publishing-python-packages
 Author: AmirBahador
 Author-email: "AmirBahador" <amirbahador.pv@gmail.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `tsp_wrapper-1.0.5/setup.cfg` & `tsp_wrapper-1.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tsp_wrapper
-version = 1.0.5
+version = 1.0.7
 description = tsp_wrapper is a pipeline tsp solver
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/daneah/publishing-python-packages
 author = AmirBahador
 author_email = "AmirBahador" <amirbahador.pv@gmail.com>
 license = MIT License
```

### Comparing `tsp_wrapper-1.0.5/src/tsp_wrapper/broker/connection.py` & `tsp_wrapper-1.0.7/src/tsp_wrapper/broker/connection.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.5/src/tsp_wrapper/broker/queues.py` & `tsp_wrapper-1.0.7/src/tsp_wrapper/broker/queues.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.5/src/tsp_wrapper/broker/worker.py` & `tsp_wrapper-1.0.7/src/tsp_wrapper/broker/worker.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.5/src/tsp_wrapper/core/management/commands.py` & `tsp_wrapper-1.0.7/src/tsp_wrapper/core/management/commands.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.5/src/tsp_wrapper/middleware/euclidean_distance.py` & `tsp_wrapper-1.0.7/src/tsp_wrapper/middleware/euclidean_distance.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.5/src/tsp_wrapper/middleware/tsp_solver.py` & `tsp_wrapper-1.0.7/src/tsp_wrapper/middleware/tsp_solver.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.5/src/tsp_wrapper/tasks/base.py` & `tsp_wrapper-1.0.7/src/tsp_wrapper/tasks/base.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.5/src/tsp_wrapper/tasks/tsp.py` & `tsp_wrapper-1.0.7/src/tsp_wrapper/tasks/tsp.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.5/src/tsp_wrapper/tsp/factory.py` & `tsp_wrapper-1.0.7/src/tsp_wrapper/tsp/factory.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.5/src/tsp_wrapper/tsp/loader.py` & `tsp_wrapper-1.0.7/src/tsp_wrapper/tsp/loader.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.5/src/tsp_wrapper.egg-info/PKG-INFO` & `tsp_wrapper-1.0.7/src/tsp_wrapper.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsp-wrapper
-Version: 1.0.5
+Version: 1.0.7
 Summary: tsp_wrapper is a pipeline tsp solver
 Home-page: https://github.com/daneah/publishing-python-packages
 Author: AmirBahador
 Author-email: "AmirBahador" <amirbahador.pv@gmail.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `tsp_wrapper-1.0.5/src/tsp_wrapper.egg-info/SOURCES.txt` & `tsp_wrapper-1.0.7/src/tsp_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

