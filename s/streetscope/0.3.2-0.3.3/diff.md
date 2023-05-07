# Comparing `tmp/streetscope-0.3.2.tar.gz` & `tmp/streetscope-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streetscope-0.3.2.tar", max compression
+gzip compressed data, was "streetscope-0.3.3.tar", max compression
```

## Comparing `streetscope-0.3.2.tar` & `streetscope-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0     1072 2023-04-28 01:06:03.496785 streetscope-0.3.2/LICENSE
--rw-r--r--   0        0        0      689 2023-04-28 01:06:03.507513 streetscope-0.3.2/README.md
--rw-r--r--   0        0        0      655 2023-05-06 01:02:17.921343 streetscope-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      141 2023-04-28 01:35:32.382729 streetscope-0.3.2/src/streetscope/__init__.py
--rw-r--r--   0        0        0       27 2023-04-28 01:36:07.601106 streetscope-0.3.2/src/streetscope/cv/__init__.py
--rw-r--r--   0        0        0       27 2023-04-28 10:12:41.686471 streetscope-0.3.2/src/streetscope/cv/segmentation/__init__.py
--rw-r--r--   0        0        0    39101 2023-05-05 01:28:21.346862 streetscope-0.3.2/src/streetscope/cv/segmentation/segmentation.py
--rw-r--r--   0        0        0       55 2023-04-13 03:44:34.089983 streetscope-0.3.2/src/streetscope/download/__init__.py
--rw-r--r--   0        0        0    10738 2023-05-05 22:57:18.657057 streetscope-0.3.2/src/streetscope/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-04-12 01:36:02.614098 streetscope-0.3.2/src/streetscope/download/utils/UserAgent.csv
--rw-r--r--   0        0        0        0 2023-04-12 07:50:41.918376 streetscope-0.3.2/src/streetscope/download/utils/__init__.py
--rw-r--r--   0        0        0     5048 2023-05-05 13:59:33.549883 streetscope-0.3.2/src/streetscope/download/utils/geoprocess.py
--rw-r--r--   0        0        0     3553 2023-04-12 01:50:02.108635 streetscope-0.3.2/src/streetscope/download/utils/get_pids.py
--rw-r--r--   0        0        0     8108 2023-05-05 23:52:21.840224 streetscope-0.3.2/src/streetscope/download/utils/imtool.py
--rw-r--r--   0        0        0        0 2023-04-28 01:06:03.540992 streetscope-0.3.2/src/streetscope/streetscope.py
--rw-r--r--   0        0        0       30 2023-05-03 02:17:38.864664 streetscope-0.3.2/src/streetscope/transform/__init__.py
--rw-r--r--   0        0        0     6768 2023-04-28 09:51:23.730858 streetscope-0.3.2/src/streetscope/transform/transform_image.py
--rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 streetscope-0.3.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-04-28 01:06:03.496785 streetscope-0.3.3/LICENSE
+-rw-r--r--   0        0        0      689 2023-04-28 01:06:03.507513 streetscope-0.3.3/README.md
+-rw-r--r--   0        0        0      655 2023-05-07 05:39:36.908242 streetscope-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      141 2023-04-28 01:35:32.382729 streetscope-0.3.3/src/streetscope/__init__.py
+-rw-r--r--   0        0        0       27 2023-04-28 01:36:07.601106 streetscope-0.3.3/src/streetscope/cv/__init__.py
+-rw-r--r--   0        0        0       27 2023-04-28 10:12:41.686471 streetscope-0.3.3/src/streetscope/cv/segmentation/__init__.py
+-rw-r--r--   0        0        0    39101 2023-05-05 01:28:21.346862 streetscope-0.3.3/src/streetscope/cv/segmentation/segmentation.py
+-rw-r--r--   0        0        0       55 2023-04-13 03:44:34.089983 streetscope-0.3.3/src/streetscope/download/__init__.py
+-rw-r--r--   0        0        0    11871 2023-05-07 05:36:40.959962 streetscope-0.3.3/src/streetscope/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-04-12 01:36:02.614098 streetscope-0.3.3/src/streetscope/download/utils/UserAgent.csv
+-rw-r--r--   0        0        0        0 2023-04-12 07:50:41.918376 streetscope-0.3.3/src/streetscope/download/utils/__init__.py
+-rw-r--r--   0        0        0     8754 2023-05-07 05:12:49.772501 streetscope-0.3.3/src/streetscope/download/utils/geoprocess.py
+-rw-r--r--   0        0        0     3636 2023-05-07 05:25:22.808345 streetscope-0.3.3/src/streetscope/download/utils/get_pids.py
+-rw-r--r--   0        0        0     8108 2023-05-05 23:52:21.840224 streetscope-0.3.3/src/streetscope/download/utils/imtool.py
+-rw-r--r--   0        0        0        0 2023-04-28 01:06:03.540992 streetscope-0.3.3/src/streetscope/streetscope.py
+-rw-r--r--   0        0        0       30 2023-05-03 02:17:38.864664 streetscope-0.3.3/src/streetscope/transform/__init__.py
+-rw-r--r--   0        0        0     6768 2023-04-28 09:51:23.730858 streetscope-0.3.3/src/streetscope/transform/transform_image.py
+-rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 streetscope-0.3.3/PKG-INFO
```

### Comparing `streetscope-0.3.2/LICENSE` & `streetscope-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.2/README.md` & `streetscope-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.2/pyproject.toml` & `streetscope-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streetscope"
-version = "0.3.2"
+version = "0.3.3"
 description = "This package handles downloading, cleaning, analyzing street view imagery"
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `streetscope-0.3.2/src/streetscope/cv/segmentation/segmentation.py` & `streetscope-0.3.3/src/streetscope/cv/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.2/src/streetscope/download/streetview_downloader.py` & `streetscope-0.3.3/src/streetscope/download/streetview_downloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,28 +7,36 @@
 import warnings
 import requests
 import cv2
 import pkg_resources
 from pathlib import Path
 import geopandas as gpd
 from tqdm import tqdm
+import warnings
+from shapely.errors import ShapelyDeprecationWarning
+import aiohttp
+import asyncio
+
+warnings.filterwarnings("ignore", category=ShapelyDeprecationWarning)
 
 from streetscope.download.utils.imtool import ImageTool
 from streetscope.download.utils.get_pids import panoids
 from streetscope.download.utils.geoprocess import GeoProcessor
 
 class StreetViewDownloader:
-    def __init__(self, gsv_api_key = None, log_path = None, nthreads = 5, distance = 1):
+    def __init__(self, gsv_api_key = None, log_path = None, nthreads = 5, distance = 1, grid = False, grid_size = 20):
         if gsv_api_key == None:
             warnings.warn("Please provide your Google Street View API key to augment metadata.")
         self._gsv_api_key = gsv_api_key
         self._log_path = log_path
         self._nthreads = nthreads
         self._distance = distance
         self._user_agent = self._get_ua()
+        self._grid = grid
+        self._grid_size = grid_size
 
     @property
     def gsv_api_key(self):
         return self._gsv_api_key    
     @gsv_api_key.setter
     def gsv_api_key(self,gsv_api_key):
         self._gsv_api_key = gsv_api_key
@@ -51,14 +59,28 @@
     def distance(self):
         return self._distance    
     @distance.setter
     def distance(self,distance):
         self._distance = distance
     
     @property
+    def grid(self):
+        return self._grid    
+    @grid.setter
+    def grid(self,grid):
+        self._grid = grid
+        
+    @property
+    def grid_size(self):
+        return self._grid_size    
+    @grid_size.setter
+    def grid_size(self,grid_size):
+        self._grid_size = grid_size
+    
+    @property
     def user_agent(self):
         return self._user_agent  
     
     def _get_ua(self):
         user_agent_file = pkg_resources.resource_filename('streetscope.download.utils', 'UserAgent.csv')
         UA = []
         with open(user_agent_file, 'r') as f:
@@ -163,73 +185,78 @@
                     result['input_longitude'] = input_longitude
                     result['input_latitude'] = input_latitude
                     results.append(result)
 
         results_df = pd.DataFrame(results)
         return results_df
     
-    def _get_pids_from_shp(self, input_shp_file, closest=False, disp=False):
-        def get_street_view_info(longitude, latitude):
-            results = panoids(latitude, longitude, closest=closest, disp=disp)
+    async def _get_pids_from_shp(self, input_shp_file, closest=False, disp=False):  
+        async def get_street_view_info(longitude, latitude):
+            async with aiohttp.ClientSession() as session:
+                results = await panoids(latitude, longitude, closest=closest, disp=disp, session=session)
             return results
 
-        def worker(row):
+        async def worker(session, row):
             input_longitude = row['longitude']
             input_latitude = row['latitude']
-            return (input_longitude, input_latitude), get_street_view_info(input_longitude, input_latitude)
+            results = await get_street_view_info(input_longitude, input_latitude, session=session)
+            return (input_longitude, input_latitude), results
 
         # read shapefile
         gdf = gpd.read_file(input_shp_file)
-        gp = GeoProcessor(gdf, distance=self.distance)
+        gp = GeoProcessor(gdf, distance=self.distance, grid = self.grid, grid_size = self.grid_size)
         df = gp.get_lat_lon()
         results = []
 
-        with ThreadPoolExecutor() as executor:
-            futures = {executor.submit(worker, row): (row['longitude'], row['latitude']) for _, row in df.iterrows()}
-            for future in tqdm(as_completed(futures), total=len(futures), desc="Getting pids", ncols=100):
-                (input_longitude, input_latitude), row_results = future.result()
+        async with aiohttp.ClientSession() as session:
+            tasks = [worker(session, row) for _, row in df.iterrows()]
+            for future in tqdm(asyncio.as_completed(tasks), total=len(tasks), desc="Getting pids", ncols=100):
+                (input_longitude, input_latitude), row_results = await future
                 for result in row_results:
                     result['input_longitude'] = input_longitude
                     result['input_latitude'] = input_latitude
                     results.append(result)
 
         results_df = pd.DataFrame(results)
         return results_df
     
-    def get_pids(self, path_pid, lat = None, lng = None, input_csv_file = "", input_shp_file = "", closest=False, disp=False, augment_metadata=False):
+    async def get_pids(self, path_pid, lat = None, lng = None, input_csv_file = "", input_shp_file = "", closest=False, disp=False, augment_metadata=False):
         if lat != None and lng != None:
             pid = panoids(lat, lng, closest=closest, disp=disp)
         elif input_csv_file != "":
             pid = self._get_pids_from_csv(input_csv_file, closest=closest, disp=disp)
         elif input_shp_file != "":
-            pid = self._get_pids_from_shp(input_shp_file, closest=closest, disp=disp)
+            pid = await self._get_pids_from_shp(input_shp_file, closest=closest, disp=disp)
         else:
             raise ValueError("Please input the lat and lng, csv file, or shapefile.")
         # save the pids
         pid_df = pd.DataFrame(pid)
         pid_df = pid_df.drop_duplicates(subset='panoid')
         if augment_metadata & (self.gsv_api_key != None):
             pid_df = self._augment_metadata(pid_df)
         elif augment_metadata & (self.gsv_api_key == None):
             raise ValueError("Please set the gsv api key by calling the gsv_api_key method.")
         pid_df.to_csv(path_pid, index=False)
         print("The panorama IDs have been saved to {}".format(path_pid))
     
-    def download_gsv(self, dir_output, path_pid = None, zoom=2, h_tiles=4, v_tiles=2, cropped=False, full=True, 
-                    lat=None, lng=None, input_csv_file="", input_shp_file = "", closest=False, disp=False, augment_metadata=False):
+    async def download_gsv(self, dir_output, path_pid = None, zoom=2, h_tiles=4, v_tiles=2, cropped=False, full=True, 
+                lat=None, lng=None, input_csv_file="", input_shp_file = "", closest=False, disp=False, augment_metadata=False):
         # set dir_output as attribute and create the directory
         self.dir_output = dir_output
         Path(dir_output).mkdir(parents=True, exist_ok=True)
         
         # If path_pid is None, call get_pids function first
         if path_pid is None:
             print("Getting pids...")
             path_pid = os.path.join(self.dir_output, "pids.csv")
-            self.get_pids(path_pid, lat=lat, lng=lng,
+            await self.get_pids(path_pid, lat=lat, lng=lng,
                         input_csv_file=input_csv_file, input_shp_file = input_shp_file, closest=closest, disp=disp, augment_metadata=augment_metadata)
+    
+    def download_gsv_sync(self, *args, **kwargs):
+        return asyncio.run(self.download_gsv(*args, **kwargs))
 
         # Horizontal Google Street View tiles
         # zoom 3: (8, 4); zoom 5: (26, 13) zoom 2: (4, 2) zoom 1: (2, 1);4:(8,16)
         # zoom = 2
         # h_tiles = 4  # 26
         # v_tiles = 2  # 13
         # cropped = False
@@ -244,11 +271,16 @@
         panoids = self._read_pids(path_pid)
         panoids_rest = self._check_already(panoids)
 
         UAs = random.choices(self.user_agent, k = len(panoids_rest))
         ImageTool.dwl_multiple(panoids_rest, zoom, v_tiles, h_tiles, panorama_output, UAs, cropped, full, log_path=self.log_path)
                 
 if __name__ == "__main__":
-    sv_downloader = StreetViewDownloader(gsv_api_key="AIzaSyDjIBLaZ-nAWq0RIoOUQUOzCLYzMYAN2aQ", log_path = "/Users/koichiito/Downloads/Delft/log.txt")
-    sv_downloader.download_gsv("/Volumes/exfat_archi/streetscope_test/delft/images", path_pid = "/Volumes/exfat_archi/streetscope_test/delft/images/pids.csv",
+    sv_downloader = StreetViewDownloader(gsv_api_key="AIzaSyCPHEaGhci712SM9UsB8f-Mdpl1lsA6VH0", 
+                                        log_path = "/Volumes/exfat_archi/streetscope_test/delft",
+                                        distance=1
+                                        # grid = True, grid_size = 0.1
+                                        )
+    sv_downloader.download_gsv_sync("/Volumes/exfat_archi/streetscope_test/delft/images", 
+                            # path_pid = "/Volumes/exfat_archi/streetscope_test/delft/images/pids.csv",
                             input_shp_file = "/Volumes/exfat_archi/streetscope_test/delft/Delft/Delft.shp", augment_metadata=True)
     # sv_downloader.download_gsv("/Users/koichiito/Downloads/Delft", lat = 52.004400, lng = 4.342597, augment_metadata=True)
```

### Comparing `streetscope-0.3.2/src/streetscope/download/utils/UserAgent.csv` & `streetscope-0.3.3/src/streetscope/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.2/src/streetscope/download/utils/get_pids.py` & `streetscope-0.3.3/src/streetscope/download/utils/get_pids.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 import re
 import requests
 from datetime import datetime
+import aiohttp
+import asyncio
 
 def _panoids_url(lat, lon):
     """
     Builds the URL of the script on Google's servers that returns the closest
     panoramas (ids) to a give GPS coordinate.
     """
     url = "https://maps.googleapis.com/maps/api/js/GeoPhotoService.SingleImageSearch?pb=!1m5!1sapiv3!5sUS!11m2!1m1!1b0!2m4!1m2!3d{0:}!4d{1:}!2d50!3m10!2m2!1sen!2sGB!9m1!1e2!11m4!1m3!1e2!2b1!3e2!4m10!1e1!1e2!1e3!1e4!1e8!1e6!5m1!1e2!6m1!1e2&callback=_xdc_._v2mub5"
     return url.format(lat, lon)
 
 
-def _panoids_data(lat, lon, proxies=None):
+async def _panoids_data(session, lat, lon):
     """
     Gets the response of the script on Google's servers that returns the
     closest panoramas (ids) to a give GPS coordinate.
     """
     url = _panoids_url(lat, lon)
-    return requests.get(url, proxies=None)
+    async with session.get(url) as resp:
+        return await resp.text()
 
 
-def panoids(lat, lon, closest=False, disp=False, proxies=None):
+async def panoids(lat, lon, closest=False, disp=False, session=None):
     """
     Gets the closest panoramas (ids) to the GPS coordinates.
     If the 'closest' boolean parameter is set to true, only the closest panorama
     will be gotten (at all the available dates)
     """
 
-    resp = _panoids_data(lat, lon)
+    resp = await _panoids_data(session, lat, lon)
 
     # Get all the panorama ids and coordinates
     # I think the latest panorama should be the first one. And the previous
     # successive ones ought to be in reverse order from bottom to top. The final
     # images don't seem to correspond to a particular year. So if there is one
     # image per year I expect them to be orded like:
     # 2015
```

### Comparing `streetscope-0.3.2/src/streetscope/download/utils/imtool.py` & `streetscope-0.3.3/src/streetscope/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.2/src/streetscope/transform/transform_image.py` & `streetscope-0.3.3/src/streetscope/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.2/PKG-INFO` & `streetscope-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streetscope
-Version: 0.3.2
+Version: 0.3.3
 Summary: This package handles downloading, cleaning, analyzing street view imagery
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

