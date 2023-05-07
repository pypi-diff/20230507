# Comparing `tmp/basal_and_bark-0.0.6.tar.gz` & `tmp/basal_and_bark-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basal_and_bark-0.0.6.tar", last modified: Sun May  7 01:14:37 2023, max compression
+gzip compressed data, was "basal_and_bark-0.0.7.tar", last modified: Sun May  7 03:33:17 2023, max compression
```

## Comparing `basal_and_bark-0.0.6.tar` & `basal_and_bark-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:14:37.494269 basal_and_bark-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-07 01:14:20.000000 basal_and_bark-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-07 01:14:20.000000 basal_and_bark-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-07 01:14:37.494269 basal_and_bark-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-07 01:14:20.000000 basal_and_bark-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:14:37.490269 basal_and_bark-0.0.6/basal_and_bark/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-07 01:14:20.000000 basal_and_bark-0.0.6/basal_and_bark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20679 2023-05-07 01:14:20.000000 basal_and_bark-0.0.6/basal_and_bark/basal_and_bark.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-07 01:14:20.000000 basal_and_bark-0.0.6/basal_and_bark/basal_and_bark_folium.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:14:37.494269 basal_and_bark-0.0.6/basal_and_bark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-07 01:14:37.000000 basal_and_bark-0.0.6/basal_and_bark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-07 01:14:37.000000 basal_and_bark-0.0.6/basal_and_bark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 01:14:37.000000 basal_and_bark-0.0.6/basal_and_bark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 01:14:37.000000 basal_and_bark-0.0.6/basal_and_bark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 01:14:37.000000 basal_and_bark-0.0.6/basal_and_bark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 01:14:37.000000 basal_and_bark-0.0.6/basal_and_bark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-07 01:14:20.000000 basal_and_bark-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-07 01:14:37.494269 basal_and_bark-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-07 01:14:20.000000 basal_and_bark-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:33:17.100953 basal_and_bark-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-07 03:33:07.000000 basal_and_bark-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-07 03:33:07.000000 basal_and_bark-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-07 03:33:17.100953 basal_and_bark-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-07 03:33:07.000000 basal_and_bark-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:33:17.100953 basal_and_bark-0.0.7/basal_and_bark/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-07 03:33:07.000000 basal_and_bark-0.0.7/basal_and_bark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20677 2023-05-07 03:33:07.000000 basal_and_bark-0.0.7/basal_and_bark/basal_and_bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-07 03:33:07.000000 basal_and_bark-0.0.7/basal_and_bark/basal_and_bark_folium.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 03:33:17.100953 basal_and_bark-0.0.7/basal_and_bark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-07 03:33:17.000000 basal_and_bark-0.0.7/basal_and_bark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-07 03:33:17.000000 basal_and_bark-0.0.7/basal_and_bark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 03:33:17.000000 basal_and_bark-0.0.7/basal_and_bark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 03:33:17.000000 basal_and_bark-0.0.7/basal_and_bark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 03:33:17.000000 basal_and_bark-0.0.7/basal_and_bark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 03:33:17.000000 basal_and_bark-0.0.7/basal_and_bark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-07 03:33:07.000000 basal_and_bark-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-07 03:33:17.100953 basal_and_bark-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-07 03:33:07.000000 basal_and_bark-0.0.7/setup.py
```

### Comparing `basal_and_bark-0.0.6/LICENSE` & `basal_and_bark-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `basal_and_bark-0.0.6/PKG-INFO` & `basal_and_bark-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basal_and_bark
-Version: 0.0.6
+Version: 0.0.7
 Summary: Welcome to Basal and Bark, a spatial python package for working with forest data.
 Home-page: https://github.com/ZachDorm/basal_and_bark
 Author: Zach Dorminey
 Author-email: zach.dorminey@gmail.com
 License: MIT license
 Keywords: basal_and_bark
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `basal_and_bark-0.0.6/README.md` & `basal_and_bark-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `basal_and_bark-0.0.6/basal_and_bark/basal_and_bark.py` & `basal_and_bark-0.0.7/basal_and_bark/basal_and_bark.py`

 * *Files 3% similar despite different names*

```diff
@@ -328,29 +328,29 @@
             # if basemap_ctrl not in leaflet_map.controls:
                     output_widget.display(close_button)
         
         close_button.observe(close_basemap, "value")
 
 
 
-    def makeStateDict():
-        states = {"AL": "01",
-        "AR": "05",
-        "FL": "12",
-        "GA": "13",
-        "KY": "21",
-        "LA": "22",
-        "MS": "28",
-        "NC": "37",
-        "OK": "40",
-        "SC": "45",
-        "TN": "47",
-        "TX": "48",
-        "VA": "51"
-        }
+    # def makeStateDict():
+    #     states = {"AL": "01",
+    #     "AR": "05",
+    #     "FL": "12",
+    #     "GA": "13",
+    #     "KY": "21",
+    #     "LA": "22",
+    #     "MS": "28",
+    #     "NC": "37",
+    #     "OK": "40",
+    #     "SC": "45",
+    #     "TN": "47",
+    #     "TX": "48",
+    #     "VA": "51"
+    #     }
 
     # def createWidgetA4API(self):
     #     output_widget = widgets.Output(layout={'border': '1px solid black'})
     #     output_widget.clear_output()
     #     basemap_ctrl = WidgetControl(widget=output_widget, position='bottomright')
     #     self.add_control(basemap_ctrl)
 
@@ -577,31 +577,31 @@
         lst = list(list(df.values()))#.values())
 
         df = pandas.DataFrame(lst)
         df.index = ['max', 'mean', 'min', 'std', 'sum']
         df.columns = ['GEEMap Data']
         return df
     
-    def findInt(self, tn_counties_gd, gdf):
+    def findInt(self, states, gdf):
         """Find the interesection between the first geometry (must have attribute "USPS") and the second.
 
         Args:
             tn_counties_gd (GeoDataFrame): geometry 1
             gdf (GeoDataFrame): geometry 2
 
         Returns:
             The name of the intersection from field "STUSPS"
         """        
-        for i in range(1,len(tn_counties_gd['geometry']),1):
-            test = tn_counties_gd['geometry'][i].contains(gdf['geometry'])
+        for i in range(1,len(states['geometry']),1):
+            test = states['geometry'][i].contains(gdf['geometry'])
 
             county = 'name'
 
             if test[0]:
-                return tn_counties_gd['STUSPS'][i]
+                return states['STUSPS'][i]
```

### Comparing `basal_and_bark-0.0.6/basal_and_bark/basal_and_bark_folium.py` & `basal_and_bark-0.0.7/basal_and_bark/basal_and_bark_folium.py`

 * *Files identical despite different names*

### Comparing `basal_and_bark-0.0.6/basal_and_bark.egg-info/PKG-INFO` & `basal_and_bark-0.0.7/basal_and_bark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basal-and-bark
-Version: 0.0.6
+Version: 0.0.7
 Summary: Welcome to Basal and Bark, a spatial python package for working with forest data.
 Home-page: https://github.com/ZachDorm/basal_and_bark
 Author: Zach Dorminey
 Author-email: zach.dorminey@gmail.com
 License: MIT license
 Keywords: basal_and_bark
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `basal_and_bark-0.0.6/setup.py` & `basal_and_bark-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='basal_and_bark',
     name='basal_and_bark',
     packages=find_packages(include=['basal_and_bark', 'basal_and_bark.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ZachDorm/basal_and_bark',
-    version='0.0.6',
+    version='0.0.7',
     zip_safe=False,
 )
```

