# Comparing `tmp/optimal_loc-0.0.4.tar.gz` & `tmp/optimal_loc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimal_loc-0.0.4.tar", max compression
+gzip compressed data, was "optimal_loc-0.0.5.tar", max compression
```

## Comparing `optimal_loc-0.0.4.tar` & `optimal_loc-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.0.4/LICENSE
--rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.0.4/README.md
--rw-r--r--   0        0        0       95 2023-05-07 14:39:16.673492 optimal_loc-0.0.4/optimal_loc/__init__.py
--rw-r--r--   0        0        0      286 2023-05-07 14:15:30.698685 optimal_loc-0.0.4/optimal_loc/bash_command.py
--rw-r--r--   0        0        0     9643 2023-05-07 14:38:38.710680 optimal_loc-0.0.4/optimal_loc/optimal_loc.py
--rw-r--r--   0        0        0     2648 2023-05-07 14:37:48.634589 optimal_loc-0.0.4/optimal_loc/st_app.py
--rw-r--r--   0        0        0      857 2023-05-07 14:39:16.669752 optimal_loc-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 optimal_loc-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.0.5/LICENSE
+-rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.0.5/README.md
+-rw-r--r--   0        0        0       95 2023-05-07 14:57:52.488420 optimal_loc-0.0.5/optimal_loc/__init__.py
+-rw-r--r--   0        0        0      399 2023-05-07 14:57:38.361508 optimal_loc-0.0.5/optimal_loc/bash_command.py
+-rw-r--r--   0        0        0     9523 2023-05-07 15:00:25.950207 optimal_loc-0.0.5/optimal_loc/optimal_loc.py
+-rw-r--r--   0        0        0     2746 2023-05-07 15:03:26.365727 optimal_loc-0.0.5/optimal_loc/st_app.py
+-rw-r--r--   0        0        0      857 2023-05-07 14:57:52.485594 optimal_loc-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 optimal_loc-0.0.5/PKG-INFO
```

### Comparing `optimal_loc-0.0.4/LICENSE` & `optimal_loc-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.0.4/README.md` & `optimal_loc-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.0.4/optimal_loc/optimal_loc.py` & `optimal_loc-0.0.5/optimal_loc/optimal_loc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 from numpy import array, meshgrid
 from pandas import DataFrame, pivot_table
 from pymongo.mongo_client import MongoClient
 from h3 import geo_to_h3, h3_to_geo
 import pickle
 from pulp import LpProblem, LpMinimize, LpVariable, lpSum, PULP_CBC_CMD
 
@@ -65,18 +64,14 @@
             hexagon_ids[["hexagon", "hex_lat", "hex_lon"]],
             left_on="tohex",
             right_on="hexagon",
             how="left").drop(columns=["hexagon"]).rename(columns={"hex_lon": "tohex_lon", 'hex_lat': 'tohex_lat'})
 
         self.hex_distance_data = hex_distance_data
 
-        logging.info(
-            "Distance data for each hexagons was created. You can read it by object_name.hex_distance_data"
-        )
-
         print("Distance data for each hexagons was created. You can read it by object_name.hex_distance_data")
 
     def read_distances_from_mongodb(self, mongo_client: MongoClient,
                                     mongo_database_name: str,
                                     mongo_collection_name: str):
         try:
             mongo_client.admin.command('ping')
@@ -86,16 +81,14 @@
             raise ConnectionError()
 
         db = mongo_client[mongo_database_name]
         col = db[mongo_collection_name]
         distance_data = DataFrame(list(col.find()))
         self.hex_distance_data = distance_data
 
-        return distance_data
-
     def read_distances(self, read_from_dataframe: bool = False,
                        read_from_mongo: bool = False,
                        distance_dataframe: DataFrame = DataFrame(),
                        mongo_client: MongoClient = None,
                        mongo_database_name: str = None,
                        mongo_collection_name: str = None):
 
@@ -112,22 +105,23 @@
                 raise ValueError("""
                 distance_dataframe:pandas.DataFrame can not be null if you want to read distances from a data frame.
                 Please give the distance data as a dataframe where columns should be 
                 'fromhex', 'tohex', 'fromhex_lat', 'fromhex_lon', 'tohex_lat', 'tohex_lon', 'distance'
                 """)
 
             self.hex_distance_data = distance_dataframe
-            return distance_dataframe
+            print("Successfully read the distance data")
 
         elif read_from_mongo:
             if mongo_client and mongo_database_name and mongo_collection_name:
-                return self.read_distances_from_mongodb(
+                self.read_distances_from_mongodb(
                     mongo_client=mongo_client,
                     mongo_database_name=mongo_database_name,
                     mongo_collection_name=mongo_collection_name)
+                print("Successfully read the distance data")
 
             else:
                 raise ValueError("""
                 mongo_client:MongoClient,
                 mongo_database_name:str
                 mongo_collection_name:str features can not be null if you want to read distances from a MongoDb.
                 """)
@@ -221,15 +215,15 @@
         prob.solve(PULP_CBC_CMD(msg=0))
 
         results = self.prepare_data_tables(prob, frequency_data)
 
         with open('optimal_locations.pickle', 'wb') as handle:
             pickle.dump(results, handle, protocol=pickle.HIGHEST_PROTOCOL)
 
-        logging.info(
+        print(
             """
             You have successfully run the algorithm. To see the optimization results, you can run 
             object_name.supply_data or object_name.optimal_data 
             OR
             You can run optimal_loc.visualize() command to see the results on a map.
             """
         )
```

### Comparing `optimal_loc-0.0.4/optimal_loc/st_app.py` & `optimal_loc-0.0.5/optimal_loc/st_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import os
 import streamlit as st
 from pandas import DataFrame
 from streamlit_folium import folium_static
 from pickle import load as pickle_load
 from folium import plugins, Map, CircleMarker, Marker, Icon
 from PIL import Image
 
-my_algorithm = Image.open('../Modelling Algorithm.png')
+
+PACKAGE_DIR = os.path.dirname(os.path.abspath(__file__))
+my_algorithm = Image.open(os.path.join(PACKAGE_DIR, '..', 'Modelling Algorithm.png'))
 
 st.set_page_config(layout="wide")
 
 my_colours = [
     'darkred',
     'orange',
     'darkgreen',
```

### Comparing `optimal_loc-0.0.4/pyproject.toml` & `optimal_loc-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optimal-loc"
-version = "0.0.4"
+version = "0.0.5"
 description = "A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs."
 
 authors = ["Sinan Demirhan <sdemirhan1320@gmail.com>"]
 readme = "README.md"
 packages = [{include = "optimal_loc"}]
 license = "MIT"
 homepage = "https://github.com/sinan-demirhan/optimal-loc"
```

### Comparing `optimal_loc-0.0.4/PKG-INFO` & `optimal_loc-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimal-loc
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs.
 Home-page: https://github.com/sinan-demirhan/optimal-loc
 License: MIT
 Keywords: optimalLoc,optimal_loc,optimal-loc,optimal,optimal location,optimal location finder
 Author: Sinan Demirhan
 Author-email: sdemirhan1320@gmail.com
 Requires-Python: >=3.7,<4.0
```

