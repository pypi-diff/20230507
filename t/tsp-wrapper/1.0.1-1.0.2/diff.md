# Comparing `tmp/tsp_wrapper-1.0.1.tar.gz` & `tmp/tsp_wrapper-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsp_wrapper-1.0.1.tar", last modified: Sat May  6 20:27:56 2023, max compression
+gzip compressed data, was "tsp_wrapper-1.0.2.tar", last modified: Sun May  7 08:31:03 2023, max compression
```

## Comparing `tsp_wrapper-1.0.1.tar` & `tsp_wrapper-1.0.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.184827 tsp_wrapper-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-06 20:27:56.188828 tsp_wrapper-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-06 20:27:56.188828 tsp_wrapper-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.176827 tsp_wrapper-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.180827 tsp_wrapper-1.0.1/src/tsp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.180827 tsp_wrapper-1.0.1/src/tsp_wrapper/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.180827 tsp_wrapper-1.0.1/src/tsp_wrapper/broker/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/broker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/broker/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/broker/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/broker/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/broker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.184827 tsp_wrapper-1.0.1/src/tsp_wrapper/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/conf/global_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.184827 tsp_wrapper-1.0.1/src/tsp_wrapper/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.184827 tsp_wrapper-1.0.1/src/tsp_wrapper/core/management/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/core/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/core/management/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.184827 tsp_wrapper-1.0.1/src/tsp_wrapper/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/middleware/dict_to_city.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/middleware/euclidean_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/middleware/tsp_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.184827 tsp_wrapper-1.0.1/src/tsp_wrapper/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/tasks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/tasks/tsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.184827 tsp_wrapper-1.0.1/src/tsp_wrapper/tsp/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/tsp/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/tsp/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/tsp/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/tsp/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/tsp/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.184827 tsp_wrapper-1.0.1/src/tsp_wrapper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-06 20:27:45.000000 tsp_wrapper-1.0.1/src/tsp_wrapper/utils/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 20:27:56.180827 tsp_wrapper-1.0.1/src/tsp_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-06 20:27:56.000000 tsp_wrapper-1.0.1/src/tsp_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-06 20:27:56.000000 tsp_wrapper-1.0.1/src/tsp_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 20:27:56.000000 tsp_wrapper-1.0.1/src/tsp_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-06 20:27:56.000000 tsp_wrapper-1.0.1/src/tsp_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:31:03.406554 tsp_wrapper-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-07 08:31:03.406554 tsp_wrapper-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-07 08:31:03.406554 tsp_wrapper-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:31:03.402554 tsp_wrapper-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:31:03.402554 tsp_wrapper-1.0.2/src/tsp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:31:03.402554 tsp_wrapper-1.0.2/src/tsp_wrapper/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:31:03.402554 tsp_wrapper-1.0.2/src/tsp_wrapper/broker/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/broker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/broker/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/broker/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/broker/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/broker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:31:03.406554 tsp_wrapper-1.0.2/src/tsp_wrapper/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/conf/global_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:31:03.406554 tsp_wrapper-1.0.2/src/tsp_wrapper/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:31:03.406554 tsp_wrapper-1.0.2/src/tsp_wrapper/core/management/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/core/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/core/management/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:31:03.406554 tsp_wrapper-1.0.2/src/tsp_wrapper/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/middleware/dict_to_city.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/middleware/euclidean_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/middleware/tsp_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:31:03.406554 tsp_wrapper-1.0.2/src/tsp_wrapper/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/tasks/tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:31:03.406554 tsp_wrapper-1.0.2/src/tsp_wrapper/tsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/tsp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/tsp/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/tsp/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/tsp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/tsp/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:31:03.406554 tsp_wrapper-1.0.2/src/tsp_wrapper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-07 08:30:51.000000 tsp_wrapper-1.0.2/src/tsp_wrapper/utils/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:31:03.402554 tsp_wrapper-1.0.2/src/tsp_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-07 08:31:03.000000 tsp_wrapper-1.0.2/src/tsp_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-07 08:31:03.000000 tsp_wrapper-1.0.2/src/tsp_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 08:31:03.000000 tsp_wrapper-1.0.2/src/tsp_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 08:31:03.000000 tsp_wrapper-1.0.2/src/tsp_wrapper.egg-info/top_level.txt
```

### Comparing `tsp_wrapper-1.0.1/PKG-INFO` & `tsp_wrapper-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsp_wrapper
-Version: 1.0.1
+Version: 1.0.2
 Summary: tsp_wrapper is a pipeline tsp solver
 Home-page: https://github.com/daneah/publishing-python-packages
 Author: AmirBahador
 Author-email: "AmirBahador" <amirbahador.pv@gmail.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `tsp_wrapper-1.0.1/setup.cfg` & `tsp_wrapper-1.0.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tsp_wrapper
-version = 1.0.1
+version = 1.0.2
 description = tsp_wrapper is a pipeline tsp solver
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/daneah/publishing-python-packages
 author = AmirBahador
 author_email = "AmirBahador" <amirbahador.pv@gmail.com>
 license = MIT License
```

### Comparing `tsp_wrapper-1.0.1/src/tsp_wrapper/broker/connection.py` & `tsp_wrapper-1.0.2/src/tsp_wrapper/broker/connection.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.1/src/tsp_wrapper/broker/queues.py` & `tsp_wrapper-1.0.2/src/tsp_wrapper/broker/queues.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.1/src/tsp_wrapper/broker/worker.py` & `tsp_wrapper-1.0.2/src/tsp_wrapper/broker/worker.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.1/src/tsp_wrapper/core/management/commands.py` & `tsp_wrapper-1.0.2/src/tsp_wrapper/core/management/commands.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.1/src/tsp_wrapper/middleware/euclidean_distance.py` & `tsp_wrapper-1.0.2/src/tsp_wrapper/middleware/euclidean_distance.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.1/src/tsp_wrapper/middleware/tsp_solver.py` & `tsp_wrapper-1.0.2/src/tsp_wrapper/middleware/tsp_solver.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.1/src/tsp_wrapper/tasks/base.py` & `tsp_wrapper-1.0.2/src/tsp_wrapper/tasks/base.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.1/src/tsp_wrapper/tasks/tsp.py` & `tsp_wrapper-1.0.2/src/tsp_wrapper/tasks/tsp.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.1/src/tsp_wrapper/tsp/factory.py` & `tsp_wrapper-1.0.2/src/tsp_wrapper/tsp/factory.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.1/src/tsp_wrapper/tsp/loader.py` & `tsp_wrapper-1.0.2/src/tsp_wrapper/tsp/loader.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.1/src/tsp_wrapper.egg-info/PKG-INFO` & `tsp_wrapper-1.0.2/src/tsp_wrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsp-wrapper
-Version: 1.0.1
+Version: 1.0.2
 Summary: tsp_wrapper is a pipeline tsp solver
 Home-page: https://github.com/daneah/publishing-python-packages
 Author: AmirBahador
 Author-email: "AmirBahador" <amirbahador.pv@gmail.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `tsp_wrapper-1.0.1/src/tsp_wrapper.egg-info/SOURCES.txt` & `tsp_wrapper-1.0.2/src/tsp_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

