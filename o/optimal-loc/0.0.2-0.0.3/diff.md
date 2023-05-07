# Comparing `tmp/optimal_loc-0.0.2.tar.gz` & `tmp/optimal_loc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimal_loc-0.0.2.tar", max compression
+gzip compressed data, was "optimal_loc-0.0.3.tar", max compression
```

## Comparing `optimal_loc-0.0.2.tar` & `optimal_loc-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.0.2/LICENSE
--rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.0.2/README.md
--rw-r--r--   0        0        0       27 2023-04-30 23:48:01.553355 optimal_loc-0.0.2/optimal_loc/__init__.py
--rw-r--r--   0        0        0     8647 2023-05-06 22:13:25.474844 optimal_loc-0.0.2/optimal_loc/optimal_loc.py
--rw-r--r--   0        0        0      803 2023-05-06 23:00:37.866930 optimal_loc-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 optimal_loc-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.0.3/LICENSE
+-rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.0.3/README.md
+-rw-r--r--   0        0        0       72 2023-05-07 13:56:36.839386 optimal_loc-0.0.3/optimal_loc/__init__.py
+-rw-r--r--   0        0        0      286 2023-05-07 14:15:30.698685 optimal_loc-0.0.3/optimal_loc/bash_command.py
+-rw-r--r--   0        0        0     9612 2023-05-07 14:21:19.853757 optimal_loc-0.0.3/optimal_loc/optimal_loc.py
+-rw-r--r--   0        0        0     2676 2023-05-07 14:24:38.799578 optimal_loc-0.0.3/optimal_loc/st_app.py
+-rw-r--r--   0        0        0      857 2023-05-07 14:09:07.360707 optimal_loc-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 optimal_loc-0.0.3/PKG-INFO
```

### Comparing `optimal_loc-0.0.2/LICENSE` & `optimal_loc-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.0.2/README.md` & `optimal_loc-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.0.2/optimal_loc/optimal_loc.py` & `optimal_loc-0.0.3/optimal_loc/optimal_loc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import logging
 import numpy as np
 import pandas as pd
 from pymongo.mongo_client import MongoClient
 import h3
 import pickle
-from pulp import *
+from pulp import LpProblem, LpMinimize, LpVariable, lpSum, PULP_CBC_CMD
 
 
 class OptimalLoc:
     def __init__(self):
         self.supply_data = None
         self.optimal_data = None
         self.hex_distance_data = None
@@ -64,15 +65,19 @@
             hexagon_ids[["hexagon", "hex_lat", "hex_lon"]],
             left_on="tohex",
             right_on="hexagon",
             how="left").drop(columns=["hexagon"]).rename(columns={"hex_lon": "tohex_lon", 'hex_lat': 'tohex_lat'})
 
         self.hex_distance_data = hex_distance_data
 
-        return hex_distance_data
+        logging.info(
+            "Distance data for each hexagons was created. You can read it by object_name.hex_distance_data"
+        )
+
+        print("Distance data for each hexagons was created. You can read it by object_name.hex_distance_data")
 
     def read_distances_from_mongodb(self, mongo_client: MongoClient,
                                     mongo_database_name: str,
                                     mongo_collection_name: str):
         try:
             mongo_client.admin.command('ping')
             print("Pinged your deployment. You successfully connected to MongoDB!")
@@ -157,22 +162,31 @@
         self.supply_data = supply_data
         
         analysis_result["optimal_data"] = optimal_data.to_dict()
         analysis_result["supply_data"] = supply_data.to_dict()
 
         return analysis_result
 
-    def calculate_optimal_locations(self, 
-                                    distance_data: pd.DataFrame, 
-                                    frequency_data: pd.DataFrame, 
-                                    number_of_loc: int):
-        
+    def calculate_optimal_locations(self, number_of_loc: int,
+                                    distance_data: pd.DataFrame = None,
+                                    frequency_data: pd.DataFrame = None
+                                    ):
+
+        if distance_data is None:
+            distance_data = self.hex_distance_data
+        if frequency_data is None:
+            frequency_data = self.event_frequency_data
+        if distance_data is None or frequency_data is None:
+            raise ValueError("""
+                Please specify distance_data and frequency_data or run related functions.
+            """)
+
         distance_matrix = pd.pivot_table(
             distance_data, 
-            values='haversine_dist', 
+            values='distance',
             index="fromhex",
             columns="tohex"
         )
         
         distance_matrix.columns.name = None
         distance_matrix.index.name = None
 
@@ -207,8 +221,15 @@
         prob.solve(PULP_CBC_CMD(msg=0))
 
         results = self.prepare_data_tables(prob, frequency_data)
 
         with open('optimal_locations.pickle', 'wb') as handle:
             pickle.dump(results, handle, protocol=pickle.HIGHEST_PROTOCOL)
 
-        return results
+        logging.info(
+            """
+            You have successfully run the algorithm. To see the optimization results, you can run 
+            object_name.supply_data or object_name.optimal_data 
+            OR
+            You can run optimal_loc.visualize() command to see the results on a map.
+            """
+        )
```

### Comparing `optimal_loc-0.0.2/pyproject.toml` & `optimal_loc-0.0.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [tool.poetry]
 name = "optimal-loc"
-version = "0.0.2"
+version = "0.0.3"
 description = "A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs."
 
 authors = ["Sinan Demirhan <sdemirhan1320@gmail.com>"]
 readme = "README.md"
 packages = [{include = "optimal_loc"}]
 license = "MIT"
 homepage = "https://github.com/sinan-demirhan/optimal-loc"
 repository = "https://github.com/sinan-demirhan/optimal-loc"
-keywords = ["optimal_loc", "optimal-loc", "optimal", "optimal location", "optimal location finder"]
+keywords = ["optimalLoc","optimal_loc", "optimal-loc", "optimal", "optimal location", "optimal location finder"]
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 numpy = "^1.20.2"
 pandas = "^1.2.4"
 pymongo = "^3.11.0"
 h3 = "^3.7.6"
 pulp = "^2.4"
+folium = "^0.13.0"
+streamlit = "^1.21.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `optimal_loc-0.0.2/PKG-INFO` & `optimal_loc-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: optimal-loc
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs.
 Home-page: https://github.com/sinan-demirhan/optimal-loc
 License: MIT
-Keywords: optimal_loc,optimal-loc,optimal,optimal location,optimal location finder
+Keywords: optimalLoc,optimal_loc,optimal-loc,optimal,optimal location,optimal location finder
 Author: Sinan Demirhan
 Author-email: sdemirhan1320@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: folium (>=0.13.0,<0.14.0)
 Requires-Dist: h3 (>=3.7.6,<4.0.0)
 Requires-Dist: numpy (>=1.20.2,<2.0.0)
 Requires-Dist: pandas (>=1.2.4,<2.0.0)
 Requires-Dist: pulp (>=2.4,<3.0)
 Requires-Dist: pymongo (>=3.11.0,<4.0.0)
+Requires-Dist: streamlit (>=1.21.0,<2.0.0)
 Project-URL: Repository, https://github.com/sinan-demirhan/optimal-loc
 Description-Content-Type: text/markdown
 
 # optimal-loc
 A python project which finds the optimal N locations in a given area according to the given location inputs.
 
 ### Purpose of the Package
```

