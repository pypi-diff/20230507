# Comparing `tmp/optimal_loc-0.0.3.tar.gz` & `tmp/optimal_loc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimal_loc-0.0.3.tar", max compression
+gzip compressed data, was "optimal_loc-0.0.4.tar", max compression
```

## Comparing `optimal_loc-0.0.3.tar` & `optimal_loc-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.0.3/LICENSE
--rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.0.3/README.md
--rw-r--r--   0        0        0       72 2023-05-07 13:56:36.839386 optimal_loc-0.0.3/optimal_loc/__init__.py
--rw-r--r--   0        0        0      286 2023-05-07 14:15:30.698685 optimal_loc-0.0.3/optimal_loc/bash_command.py
--rw-r--r--   0        0        0     9612 2023-05-07 14:21:19.853757 optimal_loc-0.0.3/optimal_loc/optimal_loc.py
--rw-r--r--   0        0        0     2676 2023-05-07 14:24:38.799578 optimal_loc-0.0.3/optimal_loc/st_app.py
--rw-r--r--   0        0        0      857 2023-05-07 14:09:07.360707 optimal_loc-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 optimal_loc-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.0.4/LICENSE
+-rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.0.4/README.md
+-rw-r--r--   0        0        0       95 2023-05-07 14:39:16.673492 optimal_loc-0.0.4/optimal_loc/__init__.py
+-rw-r--r--   0        0        0      286 2023-05-07 14:15:30.698685 optimal_loc-0.0.4/optimal_loc/bash_command.py
+-rw-r--r--   0        0        0     9643 2023-05-07 14:38:38.710680 optimal_loc-0.0.4/optimal_loc/optimal_loc.py
+-rw-r--r--   0        0        0     2648 2023-05-07 14:37:48.634589 optimal_loc-0.0.4/optimal_loc/st_app.py
+-rw-r--r--   0        0        0      857 2023-05-07 14:39:16.669752 optimal_loc-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 optimal_loc-0.0.4/PKG-INFO
```

### Comparing `optimal_loc-0.0.3/LICENSE` & `optimal_loc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.0.3/README.md` & `optimal_loc-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.0.3/optimal_loc/optimal_loc.py` & `optimal_loc-0.0.4/optimal_loc/optimal_loc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 import logging
-import numpy as np
-import pandas as pd
+from numpy import array, meshgrid
+from pandas import DataFrame, pivot_table
 from pymongo.mongo_client import MongoClient
-import h3
+from h3 import geo_to_h3, h3_to_geo
 import pickle
 from pulp import LpProblem, LpMinimize, LpVariable, lpSum, PULP_CBC_CMD
 
 
 class OptimalLoc:
     def __init__(self):
         self.supply_data = None
         self.optimal_data = None
         self.hex_distance_data = None
         self.event_frequency_data = None
 
-    def event_frequency(self, raw_data: pd.DataFrame) -> None:
+    def event_frequency(self, raw_data: DataFrame) -> None:
         """
         Calculate the frequency of events in each hexagonal region.
 
         Parameters:
-        event_data: pd.DataFrame containing event data, with columns "latitude" and "longitude".
+        event_data: pandas.DataFrame containing event data, with columns "latitude" and "longitude".
 
         Returns:
         None
         """
-        raw_data["hex_id"] = raw_data.apply(lambda x: h3.geo_to_h3(x["latitude"], x["longitude"], 8), 1)
+        raw_data["hex_id"] = raw_data.apply(lambda x: geo_to_h3(x["latitude"], x["longitude"], 8), 1)
 
         raw_data = raw_data['hex_id'].value_counts().reset_index().rename(columns={"index": "hexagon_id",
                                                                                    "hex_id": "total_event"})
-        raw_data["hex_location"] = raw_data.apply(lambda x: h3.h3_to_geo(h=x["hexagon_id"]), 1)
+        raw_data["hex_location"] = raw_data.apply(lambda x: h3_to_geo(h=x["hexagon_id"]), 1)
         raw_data["hex_lat"] = raw_data.apply(lambda x: x["hex_location"][0], 1)
         raw_data["hex_lon"] = raw_data.apply(lambda x: x["hex_location"][1], 1)
         raw_data = raw_data.drop(columns="hex_location")
 
         self.event_frequency_data = raw_data
 
-    def create_hexagon_distance_data(self, raw_data: pd.DataFrame) -> pd.DataFrame:
+    def create_hexagon_distance_data(self, raw_data: DataFrame) -> DataFrame:
         """
         Create a DataFrame containing the distances between pairs of hexagonal regions.
 
         Parameters:
-        event_data: pd.DataFrame containing event data, with columns "latitude" and "longitude".
+        event_data: pandas.DataFrame containing event data, with columns "latitude" and "longitude".
 
         Returns:
-        A pd.DataFrame containing columns
+        A pandas.DataFrame containing columns
         "fromhex", "tohex", "fromhex_lat", "fromhex_lon", "tohex_lat", "tohex_lon", and "distance".
         """
         self.event_frequency(raw_data)
         event_data = self.event_frequency_data
 
         hexagon_ids = event_data[["hexagon_id", "hex_lat", "hex_lon"]].rename(columns={"hexagon_id": "hexagon"})
-        out_list = np.array(np.meshgrid(hexagon_ids.hexagon, hexagon_ids.hexagon)).T.reshape(-1, 2)
+        out_list = array(meshgrid(hexagon_ids.hexagon, hexagon_ids.hexagon)).T.reshape(-1, 2)
 
-        hex_distance_data = pd.DataFrame(data=out_list, columns=['fromhex', 'tohex'])
+        hex_distance_data = DataFrame(data=out_list, columns=['fromhex', 'tohex'])
 
         hex_distance_data = hex_distance_data.merge(
             hexagon_ids[["hexagon", "hex_lat", "hex_lon"]].rename(
                 columns={"hex_lon": "fromhex_lon", 'hex_lat': 'fromhex_lat'}),
             left_on="fromhex",
             right_on="hexagon",
             how="left").drop(columns=["hexagon"])
@@ -83,22 +83,22 @@
             print("Pinged your deployment. You successfully connected to MongoDB!")
         except Exception as e:
             print(e)
             raise ConnectionError()
 
         db = mongo_client[mongo_database_name]
         col = db[mongo_collection_name]
-        distance_data = pd.DataFrame(list(col.find()))
+        distance_data = DataFrame(list(col.find()))
         self.hex_distance_data = distance_data
 
         return distance_data
 
     def read_distances(self, read_from_dataframe: bool = False,
                        read_from_mongo: bool = False,
-                       distance_dataframe: pd.DataFrame = pd.DataFrame(),
+                       distance_dataframe: DataFrame = DataFrame(),
                        mongo_client: MongoClient = None,
                        mongo_database_name: str = None,
                        mongo_collection_name: str = None):
 
         # raise an error if more than one input is True
         if sum([read_from_dataframe, read_from_mongo]) > 1:
             raise ValueError("You can read the distance from only one source.")
@@ -106,15 +106,15 @@
         if sum([read_from_dataframe, read_from_mongo]) == 0:
             raise ValueError("You need to specify at least one data source to read the real hexagon distances.")
 
         # otherwise, do something with the input that is True
         if read_from_dataframe:
             if len(distance_dataframe) == 0:
                 raise ValueError("""
-                distance_dataframe:pd.DataFrame can not be null if you want to read distances from a data frame.
+                distance_dataframe:pandas.DataFrame can not be null if you want to read distances from a data frame.
                 Please give the distance data as a dataframe where columns should be 
                 'fromhex', 'tohex', 'fromhex_lat', 'fromhex_lon', 'tohex_lat', 'tohex_lon', 'distance'
                 """)
 
             self.hex_distance_data = distance_dataframe
             return distance_dataframe
 
@@ -132,25 +132,25 @@
                 mongo_collection_name:str features can not be null if you want to read distances from a MongoDb.
                 """)
 
         else:
             # do something with c
             pass
 
-    def prepare_data_tables(self, pulp_solution, frequency_data: pd.DataFrame):
+    def prepare_data_tables(self, pulp_solution, frequency_data: DataFrame):
         analysis_result = {}
 
         wh_loc = []
         hex_loc = []
         assign = []
         for v in pulp_solution.variables()[len(frequency_data):]:
             wh_loc.append(v.name.split("_")[1])
             hex_loc.append(v.name.split("_")[2])
             assign.append(v.varValue)
-        df = pd.DataFrame({"supply_hexagon_id": wh_loc, "hexagon_id": hex_loc, "assign": assign})
+        df = DataFrame({"supply_hexagon_id": wh_loc, "hexagon_id": hex_loc, "assign": assign})
         optimal_data = df[df["assign"] != 0].reset_index(drop=True)
 
         optimal_data = optimal_data.merge(
             frequency_data[["hexagon_id", "hex_lat", "hex_lon"]],
             on="hexagon_id",
             how="left").drop(columns=["assign"])
 
@@ -163,28 +163,28 @@
         
         analysis_result["optimal_data"] = optimal_data.to_dict()
         analysis_result["supply_data"] = supply_data.to_dict()
 
         return analysis_result
 
     def calculate_optimal_locations(self, number_of_loc: int,
-                                    distance_data: pd.DataFrame = None,
-                                    frequency_data: pd.DataFrame = None
+                                    distance_data: DataFrame = None,
+                                    frequency_data: DataFrame = None
                                     ):
 
         if distance_data is None:
             distance_data = self.hex_distance_data
         if frequency_data is None:
             frequency_data = self.event_frequency_data
         if distance_data is None or frequency_data is None:
             raise ValueError("""
                 Please specify distance_data and frequency_data or run related functions.
             """)
 
-        distance_matrix = pd.pivot_table(
+        distance_matrix = pivot_table(
             distance_data, 
             values='distance',
             index="fromhex",
             columns="tohex"
         )
         
         distance_matrix.columns.name = None
```

### Comparing `optimal_loc-0.0.3/optimal_loc/st_app.py` & `optimal_loc-0.0.4/optimal_loc/st_app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import streamlit as st
 from pandas import DataFrame
-import folium
 from streamlit_folium import folium_static
-import pickle
-from folium import plugins
+from pickle import load as pickle_load
+from folium import plugins, Map, CircleMarker, Marker, Icon
 from PIL import Image
 
 my_algorithm = Image.open('../Modelling Algorithm.png')
 
 st.set_page_config(layout="wide")
 
 my_colours = [
@@ -22,15 +21,15 @@
     'black'
 ]
 
 
 @st.cache_data
 def read_data(my_json):
     with open(my_json, 'rb') as handle:
-        output_distances = pickle.load(handle)
+        output_distances = pickle_load(handle)
     return output_distances
 
 
 st.sidebar.text('')
 st.sidebar.text('')
 st.sidebar.text('')
 
@@ -63,25 +62,24 @@
 
 
 def plotting_main_map(optimization_data: DataFrame,
                       optimal_loc_data: DataFrame
                       ):
 
     plot_center = [optimization_data["hex_lat"].median(), optimization_data["hex_lon"].median()]
-    my_map = folium.Map(location=plot_center, zoom_start=12)
+    my_map = Map(location=plot_center, zoom_start=12)
 
     for j, i in optimal_data.iterrows():
-        folium.CircleMarker([i["hex_lat"], i["hex_lon"]],
-                            radius=5,
-                            color=i["my_colours"]).add_to(my_map)
+        CircleMarker([i["hex_lat"], i["hex_lon"]],
+                     radius=5,
+                     color=i["my_colours"]).add_to(my_map)
 
     for j, i in optimal_loc_data.iterrows():
-        folium.Marker([i["hex_lat"], i["hex_lon"]], radius=5,
-                      icon=folium.Icon(color='red', icon='info-sign')
-                      ).add_to(my_map)
+        Marker([i["hex_lat"], i["hex_lon"]], radius=5,
+               icon=Icon(color='red', icon='info-sign')).add_to(my_map)
 
     plugins.Fullscreen(position='topleft').add_to(my_map)
 
     return my_map
 
 
 if not agree:
```

### Comparing `optimal_loc-0.0.3/pyproject.toml` & `optimal_loc-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optimal-loc"
-version = "0.0.3"
+version = "0.0.4"
 description = "A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs."
 
 authors = ["Sinan Demirhan <sdemirhan1320@gmail.com>"]
 readme = "README.md"
 packages = [{include = "optimal_loc"}]
 license = "MIT"
 homepage = "https://github.com/sinan-demirhan/optimal-loc"
```

### Comparing `optimal_loc-0.0.3/PKG-INFO` & `optimal_loc-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimal-loc
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs.
 Home-page: https://github.com/sinan-demirhan/optimal-loc
 License: MIT
 Keywords: optimalLoc,optimal_loc,optimal-loc,optimal,optimal location,optimal location finder
 Author: Sinan Demirhan
 Author-email: sdemirhan1320@gmail.com
 Requires-Python: >=3.7,<4.0
```

