# Comparing `tmp/tsp_wrapper-1.0.3.tar.gz` & `tmp/tsp_wrapper-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsp_wrapper-1.0.3.tar", last modified: Sun May  7 09:52:59 2023, max compression
+gzip compressed data, was "tsp_wrapper-1.0.4.tar", last modified: Sun May  7 16:34:02 2023, max compression
```

## Comparing `tsp_wrapper-1.0.3.tar` & `tsp_wrapper-1.0.4.tar`

### file list

```diff
@@ -1,52 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:52:59.315012 tsp_wrapper-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-07 09:52:59.315012 tsp_wrapper-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-07 09:52:59.319012 tsp_wrapper-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:52:59.311011 tsp_wrapper-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:52:59.311011 tsp_wrapper-1.0.3/src/tsp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:52:59.315012 tsp_wrapper-1.0.3/src/tsp_wrapper/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:52:59.315012 tsp_wrapper-1.0.3/src/tsp_wrapper/broker/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/broker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/broker/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/broker/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/broker/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/broker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:52:59.315012 tsp_wrapper-1.0.3/src/tsp_wrapper/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/conf/global_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:52:59.315012 tsp_wrapper-1.0.3/src/tsp_wrapper/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:52:59.315012 tsp_wrapper-1.0.3/src/tsp_wrapper/core/management/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/core/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/core/management/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:52:59.315012 tsp_wrapper-1.0.3/src/tsp_wrapper/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/middleware/dict_to_city.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/middleware/euclidean_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/middleware/tsp_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:52:59.315012 tsp_wrapper-1.0.3/src/tsp_wrapper/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/tasks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/tasks/tsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:52:59.315012 tsp_wrapper-1.0.3/src/tsp_wrapper/tsp/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/tsp/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/tsp/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/tsp/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/tsp/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/tsp/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:52:59.315012 tsp_wrapper-1.0.3/src/tsp_wrapper/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-07 09:52:50.000000 tsp_wrapper-1.0.3/src/tsp_wrapper/utils/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:52:59.311011 tsp_wrapper-1.0.3/src/tsp_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-07 09:52:59.000000 tsp_wrapper-1.0.3/src/tsp_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-07 09:52:59.000000 tsp_wrapper-1.0.3/src/tsp_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:52:59.000000 tsp_wrapper-1.0.3/src/tsp_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 09:52:59.000000 tsp_wrapper-1.0.3/src/tsp_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:34:02.303695 tsp_wrapper-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-07 16:34:02.303695 tsp_wrapper-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-07 16:34:02.303695 tsp_wrapper-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:34:02.295694 tsp_wrapper-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:34:02.299695 tsp_wrapper-1.0.4/src/tsp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:34:02.299695 tsp_wrapper-1.0.4/src/tsp_wrapper/broker/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/broker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/broker/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/broker/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/broker/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/broker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:34:02.299695 tsp_wrapper-1.0.4/src/tsp_wrapper/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/conf/global_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:34:02.299695 tsp_wrapper-1.0.4/src/tsp_wrapper/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:34:02.299695 tsp_wrapper-1.0.4/src/tsp_wrapper/core/management/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/core/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/core/management/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:34:02.303695 tsp_wrapper-1.0.4/src/tsp_wrapper/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/middleware/dict_to_city.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/middleware/euclidean_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/middleware/tsp_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:34:02.303695 tsp_wrapper-1.0.4/src/tsp_wrapper/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/tasks/tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:34:02.303695 tsp_wrapper-1.0.4/src/tsp_wrapper/tsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/tsp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/tsp/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/tsp/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/tsp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/tsp/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:34:02.303695 tsp_wrapper-1.0.4/src/tsp_wrapper/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-07 16:33:51.000000 tsp_wrapper-1.0.4/src/tsp_wrapper/utils/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:34:02.299695 tsp_wrapper-1.0.4/src/tsp_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-07 16:34:02.000000 tsp_wrapper-1.0.4/src/tsp_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-07 16:34:02.000000 tsp_wrapper-1.0.4/src/tsp_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 16:34:02.000000 tsp_wrapper-1.0.4/src/tsp_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 16:34:02.000000 tsp_wrapper-1.0.4/src/tsp_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 16:34:02.000000 tsp_wrapper-1.0.4/src/tsp_wrapper.egg-info/top_level.txt
```

### Comparing `tsp_wrapper-1.0.3/PKG-INFO` & `tsp_wrapper-1.0.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsp_wrapper
-Version: 1.0.3
+Version: 1.0.4
 Summary: tsp_wrapper is a pipeline tsp solver
 Home-page: https://github.com/daneah/publishing-python-packages
 Author: AmirBahador
 Author-email: "AmirBahador" <amirbahador.pv@gmail.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `tsp_wrapper-1.0.3/setup.cfg` & `tsp_wrapper-1.0.4/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tsp_wrapper
-version = 1.0.3
+version = 1.0.4
 description = tsp_wrapper is a pipeline tsp solver
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/daneah/publishing-python-packages
 author = AmirBahador
 author_email = "AmirBahador" <amirbahador.pv@gmail.com>
 license = MIT License
@@ -14,14 +14,17 @@
 
 [options]
 python_requires = >=3.9
 package_dir = 
 	=src
 packages = find_namespace:
 include_package_data = True
+install_requires = 
+	ortools>=9.6.2534,<10
+	kombu>=5.2.4,<6
 
 [options.packages.find]
 where = src
 exclude = 
 	test*
 
 [mypy]
```

### Comparing `tsp_wrapper-1.0.3/src/tsp_wrapper/broker/connection.py` & `tsp_wrapper-1.0.4/src/tsp_wrapper/broker/connection.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.3/src/tsp_wrapper/broker/queues.py` & `tsp_wrapper-1.0.4/src/tsp_wrapper/broker/queues.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.3/src/tsp_wrapper/broker/worker.py` & `tsp_wrapper-1.0.4/src/tsp_wrapper/broker/worker.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.3/src/tsp_wrapper/core/management/commands.py` & `tsp_wrapper-1.0.4/src/tsp_wrapper/core/management/commands.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from tsp_wrapper import broker
 from tsp_wrapper.tasks.tsp import tsp_solver_task, get_ans
 
 import typer
-
+import secrets
 
 app = typer.Typer()
 
 
 @app.command()
 def reciver() -> None:
     worker = broker.Worker(connection=broker.get_broker(), handler=get_ans, type="outbound")
@@ -26,14 +26,15 @@
             {"name": "Nagoya", "lat": 35.1833, "lng": 136.9000},
             {"name": "Taipei", "lat": 25.0375, "lng": 121.5625},
             {"name": "Tongshan", "lat": 34.2610, "lng": 117.1859},
             {"name": "Luanda", "lat": -8.8383, "lng": 13.2344},
         ],
         "num_vehicles": 1,
         "depot": 0,
+        "id": secrets.token_hex(5),
     }
     broker.send_data(connection=broker.get_broker(), message=my_data, routing_key="inbound")
 
 
 @app.command()
 def shell() -> None:
     from IPython import start_ipython
```

### Comparing `tsp_wrapper-1.0.3/src/tsp_wrapper/middleware/euclidean_distance.py` & `tsp_wrapper-1.0.4/src/tsp_wrapper/middleware/euclidean_distance.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.3/src/tsp_wrapper/middleware/tsp_solver.py` & `tsp_wrapper-1.0.4/src/tsp_wrapper/middleware/tsp_solver.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             result.append(data[manager.IndexToNode(index)].name)
             previous_index = index
             index = solution.Value(routing.NextVar(index))
             route_distance += routing.GetArcCostForVehicle(previous_index, index, 0)
         result.append(data[manager.IndexToNode(index)].name)
         return result
 
-    def convert(self, data: dict) -> None:
+    def convert(self, data: dict) -> dict:
         # Instantiate the data problem.
 
         # Create the routing index manager.
         manager = pywrapcp.RoutingIndexManager(len(data["locations"]), data["num_vehicles"], data["depot"])
 
         # Create Routing Model.
         routing = pywrapcp.RoutingModel(manager)
@@ -46,14 +46,16 @@
         # Setting first solution heuristic.
         search_parameters = pywrapcp.DefaultRoutingSearchParameters()
         search_parameters.first_solution_strategy = routing_enums_pb2.FirstSolutionStrategy.PATH_CHEAPEST_ARC
 
         # Solve the problem.
         solution = routing.SolveWithParameters(search_parameters)
 
+        result: dict = {"id": data.get("id"), "locations": []}
+
         if solution:
-            # print_solution(manager, routing, solution, locations)
-            return self.return_solution(manager, routing, solution, data["cities"])
+            result["locations"] = (self.return_solution(manager, routing, solution, data["cities"]),)
+        return result
 
 
 def register() -> None:
     factory.register("tsp_solver", TSPSolverMiddleware)
```

### Comparing `tsp_wrapper-1.0.3/src/tsp_wrapper/tasks/base.py` & `tsp_wrapper-1.0.4/src/tsp_wrapper/tasks/base.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.3/src/tsp_wrapper/tasks/tsp.py` & `tsp_wrapper-1.0.4/src/tsp_wrapper/tasks/tsp.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.3/src/tsp_wrapper/tsp/factory.py` & `tsp_wrapper-1.0.4/src/tsp_wrapper/tsp/factory.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.3/src/tsp_wrapper/tsp/loader.py` & `tsp_wrapper-1.0.4/src/tsp_wrapper/tsp/loader.py`

 * *Files identical despite different names*

### Comparing `tsp_wrapper-1.0.3/src/tsp_wrapper.egg-info/PKG-INFO` & `tsp_wrapper-1.0.4/src/tsp_wrapper.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsp-wrapper
-Version: 1.0.3
+Version: 1.0.4
 Summary: tsp_wrapper is a pipeline tsp solver
 Home-page: https://github.com/daneah/publishing-python-packages
 Author: AmirBahador
 Author-email: "AmirBahador" <amirbahador.pv@gmail.com>
 License: MIT License
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
```

### Comparing `tsp_wrapper-1.0.3/src/tsp_wrapper.egg-info/SOURCES.txt` & `tsp_wrapper-1.0.4/src/tsp_wrapper.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 setup.cfg
 setup.py
 src/tsp_wrapper/__init__.py
 src/tsp_wrapper/__main__.py
 src/tsp_wrapper.egg-info/PKG-INFO
 src/tsp_wrapper.egg-info/SOURCES.txt
 src/tsp_wrapper.egg-info/dependency_links.txt
+src/tsp_wrapper.egg-info/requires.txt
 src/tsp_wrapper.egg-info/top_level.txt
-src/tsp_wrapper/app/__init__.py
 src/tsp_wrapper/broker/__init__.py
 src/tsp_wrapper/broker/connection.py
 src/tsp_wrapper/broker/producer.py
 src/tsp_wrapper/broker/queues.py
 src/tsp_wrapper/broker/worker.py
 src/tsp_wrapper/conf/__init__.py
 src/tsp_wrapper/conf/global_settings.py
```

