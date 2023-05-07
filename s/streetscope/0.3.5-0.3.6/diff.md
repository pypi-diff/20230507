# Comparing `tmp/streetscope-0.3.5.tar.gz` & `tmp/streetscope-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streetscope-0.3.5.tar", max compression
+gzip compressed data, was "streetscope-0.3.6.tar", max compression
```

## Comparing `streetscope-0.3.5.tar` & `streetscope-0.3.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0     1072 2023-04-28 01:06:03.496785 streetscope-0.3.5/LICENSE
--rw-r--r--   0        0        0      689 2023-04-28 01:06:03.507513 streetscope-0.3.5/README.md
--rw-r--r--   0        0        0      672 2023-05-07 05:47:44.054342 streetscope-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      141 2023-04-28 01:35:32.382729 streetscope-0.3.5/src/streetscope/__init__.py
--rw-r--r--   0        0        0       27 2023-04-28 01:36:07.601106 streetscope-0.3.5/src/streetscope/cv/__init__.py
--rw-r--r--   0        0        0       27 2023-04-28 10:12:41.686471 streetscope-0.3.5/src/streetscope/cv/segmentation/__init__.py
--rw-r--r--   0        0        0    39101 2023-05-05 01:28:21.346862 streetscope-0.3.5/src/streetscope/cv/segmentation/segmentation.py
--rw-r--r--   0        0        0       55 2023-04-13 03:44:34.089983 streetscope-0.3.5/src/streetscope/download/__init__.py
--rw-r--r--   0        0        0    11875 2023-05-07 05:42:23.024013 streetscope-0.3.5/src/streetscope/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-04-12 01:36:02.614098 streetscope-0.3.5/src/streetscope/download/utils/UserAgent.csv
--rw-r--r--   0        0        0        0 2023-04-12 07:50:41.918376 streetscope-0.3.5/src/streetscope/download/utils/__init__.py
--rw-r--r--   0        0        0     8754 2023-05-07 05:12:49.772501 streetscope-0.3.5/src/streetscope/download/utils/geoprocess.py
--rw-r--r--   0        0        0     3636 2023-05-07 05:25:22.808345 streetscope-0.3.5/src/streetscope/download/utils/get_pids.py
--rw-r--r--   0        0        0     8108 2023-05-05 23:52:21.840224 streetscope-0.3.5/src/streetscope/download/utils/imtool.py
--rw-r--r--   0        0        0        0 2023-04-28 01:06:03.540992 streetscope-0.3.5/src/streetscope/streetscope.py
--rw-r--r--   0        0        0       30 2023-05-03 02:17:38.864664 streetscope-0.3.5/src/streetscope/transform/__init__.py
--rw-r--r--   0        0        0     6768 2023-04-28 09:51:23.730858 streetscope-0.3.5/src/streetscope/transform/transform_image.py
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 streetscope-0.3.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-04-28 01:06:03.496785 streetscope-0.3.6/LICENSE
+-rw-r--r--   0        0        0      689 2023-04-28 01:06:03.507513 streetscope-0.3.6/README.md
+-rw-r--r--   0        0        0      672 2023-05-07 06:22:50.025105 streetscope-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      141 2023-04-28 01:35:32.382729 streetscope-0.3.6/src/streetscope/__init__.py
+-rw-r--r--   0        0        0       27 2023-04-28 01:36:07.601106 streetscope-0.3.6/src/streetscope/cv/__init__.py
+-rw-r--r--   0        0        0       27 2023-04-28 10:12:41.686471 streetscope-0.3.6/src/streetscope/cv/segmentation/__init__.py
+-rw-r--r--   0        0        0    39101 2023-05-05 01:28:21.346862 streetscope-0.3.6/src/streetscope/cv/segmentation/segmentation.py
+-rw-r--r--   0        0        0       55 2023-04-13 03:44:34.089983 streetscope-0.3.6/src/streetscope/download/__init__.py
+-rw-r--r--   0        0        0    11847 2023-05-07 06:18:13.579525 streetscope-0.3.6/src/streetscope/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-04-12 01:36:02.614098 streetscope-0.3.6/src/streetscope/download/utils/UserAgent.csv
+-rw-r--r--   0        0        0        0 2023-04-12 07:50:41.918376 streetscope-0.3.6/src/streetscope/download/utils/__init__.py
+-rw-r--r--   0        0        0     8527 2023-05-07 06:21:09.842314 streetscope-0.3.6/src/streetscope/download/utils/geoprocess.py
+-rw-r--r--   0        0        0     1730 2023-05-07 06:09:51.861103 streetscope-0.3.6/src/streetscope/download/utils/get_pids.py
+-rw-r--r--   0        0        0     8108 2023-05-05 23:52:21.840224 streetscope-0.3.6/src/streetscope/download/utils/imtool.py
+-rw-r--r--   0        0        0        0 2023-04-28 01:06:03.540992 streetscope-0.3.6/src/streetscope/streetscope.py
+-rw-r--r--   0        0        0       30 2023-05-03 02:17:38.864664 streetscope-0.3.6/src/streetscope/transform/__init__.py
+-rw-r--r--   0        0        0     6768 2023-04-28 09:51:23.730858 streetscope-0.3.6/src/streetscope/transform/transform_image.py
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 streetscope-0.3.6/PKG-INFO
```

### Comparing `streetscope-0.3.5/LICENSE` & `streetscope-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.5/README.md` & `streetscope-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.5/pyproject.toml` & `streetscope-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streetscope"
-version = "0.3.5"
+version = "0.3.6"
 description = "This package handles downloading, cleaning, analyzing street view imagery"
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `streetscope-0.3.5/src/streetscope/cv/segmentation/segmentation.py` & `streetscope-0.3.6/src/streetscope/cv/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.5/src/streetscope/download/streetview_downloader.py` & `streetscope-0.3.6/src/streetscope/download/streetview_downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,23 +9,22 @@
 import cv2
 import pkg_resources
 from pathlib import Path
 import geopandas as gpd
 from tqdm import tqdm
 import warnings
 from shapely.errors import ShapelyDeprecationWarning
-import aiohttp
-import asyncio
 
 warnings.filterwarnings("ignore", category=ShapelyDeprecationWarning)
 
 from streetscope.download.utils.imtool import ImageTool
 from streetscope.download.utils.get_pids import panoids
 from streetscope.download.utils.geoprocess import GeoProcessor
 
+
 class StreetViewDownloader:
     def __init__(self, gsv_api_key = None, log_path = None, nthreads = 5, distance = 1, grid = False, grid_size = 20):
         if gsv_api_key == None:
             warnings.warn("Please provide your Google Street View API key to augment metadata.")
         self._gsv_api_key = gsv_api_key
         self._log_path = log_path
         self._nthreads = nthreads
@@ -140,15 +139,15 @@
 
         def worker(index, row):
             panoid = row['panoid']
             year_month = get_year_month(panoid)
             return index, year_month
         
         with ThreadPoolExecutor() as executor:
-            futures = {executor.submit(worker, i, row): i for i, row in df.iterrows()}
+            futures = {executor.submit(worker, i, row): i for i, row in tqdm(df.iterrows(), total = len(df), desc="Preparing to augment metadata", ncols=100)}
             for future in tqdm(as_completed(futures), total=len(futures), desc="Augmenting timestamp metadata", ncols=100):
                 row_index, year_month = future.result()
                 df.at[row_index, 'year'] = year_month['year']
                 df.at[row_index, 'month'] = year_month['month']
         return df
                     
     def _get_pids_from_csv(self, input_csv_file, closest=False, disp=False):
@@ -174,85 +173,86 @@
                     df.rename(columns={col: 'latitude'}, inplace=True)
 
             return df
         df = standardize_column_names(df)
         results = []
 
         with ThreadPoolExecutor() as executor:
-            futures = {executor.submit(worker, row): (row['longitude'], row['latitude']) for _, row in df.iterrows()}
+            futures = {executor.submit(worker, row): (row['longitude'], row['latitude']) for _, row in tqdm(df.iterrows(), total = len(df), desc="Preparing to get pids", ncols=100)}
             for future in tqdm(as_completed(futures), total=len(futures), desc="Getting pids", ncols=100):
                 (input_longitude, input_latitude), row_results = future.result()
                 for result in row_results:
                     result['input_longitude'] = input_longitude
                     result['input_latitude'] = input_latitude
                     results.append(result)
 
         results_df = pd.DataFrame(results)
         return results_df
     
-    async def _get_pids_from_shp(self, input_shp_file, closest=False, disp=False):  
-        async def get_street_view_info(longitude, latitude):
-            async with aiohttp.ClientSession() as session:
-                results = await panoids(latitude, longitude, closest=closest, disp=disp, session=session)
+    def _get_pids_from_shp(self, input_shp_file, closest=False, disp=False):  
+        def get_street_view_info(longitude, latitude):
+            with requests.Session() as session:
+                results = panoids(latitude, longitude, closest=closest, disp=disp, session=session)
             return results
 
-        async def worker(session, row):
+        def worker(row):
             input_longitude = row['longitude']
             input_latitude = row['latitude']
-            results = await get_street_view_info(input_longitude, input_latitude, session=session)
+            results = get_street_view_info(input_longitude, input_latitude)
             return (input_longitude, input_latitude), results
 
         # read shapefile
         gdf = gpd.read_file(input_shp_file)
-        gp = GeoProcessor(gdf, distance=self.distance, grid = self.grid, grid_size = self.grid_size)
+        gp = GeoProcessor(gdf, distance=self.distance, grid=self.grid, grid_size=self.grid_size)
         df = gp.get_lat_lon()
         results = []
 
-        async with aiohttp.ClientSession() as session:
-            tasks = [worker(session, row) for _, row in df.iterrows()]
-            for future in tqdm(asyncio.as_completed(tasks), total=len(tasks), desc="Getting pids", ncols=100):
-                (input_longitude, input_latitude), row_results = await future
+        with ThreadPoolExecutor() as executor:
+            futures = {executor.submit(worker, row): (row['longitude'], row['latitude']) for _, row in tqdm(df.iterrows(), total = len(df), desc="Preparing to get pids", ncols=100)}
+            for future in tqdm(as_completed(futures), total=len(futures), desc="Getting pids", ncols=100):
+                (input_longitude, input_latitude), row_results = future.result()
                 for result in row_results:
                     result['input_longitude'] = input_longitude
                     result['input_latitude'] = input_latitude
                     results.append(result)
 
         results_df = pd.DataFrame(results)
         return results_df
+
     
-    async def get_pids(self, path_pid, lat = None, lng = None, input_csv_file = "", input_shp_file = "", closest=False, disp=False, augment_metadata=False):
+    def get_pids(self, path_pid, lat = None, lng = None, input_csv_file = "", input_shp_file = "", closest=False, disp=False, augment_metadata=False):
         if lat != None and lng != None:
             pid = panoids(lat, lng, closest=closest, disp=disp)
         elif input_csv_file != "":
             pid = self._get_pids_from_csv(input_csv_file, closest=closest, disp=disp)
         elif input_shp_file != "":
-            pid = await self._get_pids_from_shp(input_shp_file, closest=closest, disp=disp)
+            pid = self._get_pids_from_shp(input_shp_file, closest=closest, disp=disp)
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
     
-    async def download_gsv(self, dir_output, path_pid = None, zoom=2, h_tiles=4, v_tiles=2, cropped=False, full=True, 
+    def download_gsv(self, dir_output, path_pid = None, zoom=2, h_tiles=4, v_tiles=2, cropped=False, full=True, 
                 lat=None, lng=None, input_csv_file="", input_shp_file = "", closest=False, disp=False, augment_metadata=False):
         # set dir_output as attribute and create the directory
         self.dir_output = dir_output
         Path(dir_output).mkdir(parents=True, exist_ok=True)
         
         # If path_pid is None, call get_pids function first
         if path_pid is None:
             print("Getting pids...")
             path_pid = os.path.join(self.dir_output, "pids.csv")
-            await self.get_pids(path_pid, lat=lat, lng=lng,
+            self.get_pids(path_pid, lat=lat, lng=lng,
                         input_csv_file=input_csv_file, input_shp_file = input_shp_file, closest=closest, disp=disp, augment_metadata=augment_metadata)
 
         # Horizontal Google Street View tiles
         # zoom 3: (8, 4); zoom 5: (26, 13) zoom 2: (4, 2) zoom 1: (2, 1);4:(8,16)
         # zoom = 2
         # h_tiles = 4  # 26
         # v_tiles = 2  # 13
@@ -266,21 +266,18 @@
         panoids_rest = self._check_already(panoids)
 
         panoids = self._read_pids(path_pid)
         panoids_rest = self._check_already(panoids)
 
         UAs = random.choices(self.user_agent, k = len(panoids_rest))
         ImageTool.dwl_multiple(panoids_rest, zoom, v_tiles, h_tiles, panorama_output, UAs, cropped, full, log_path=self.log_path)
-    
-    def download_gsv_sync(self, *args, **kwargs):
-            return asyncio.run(self.download_gsv(*args, **kwargs))
-                
+
 if __name__ == "__main__":
     sv_downloader = StreetViewDownloader(gsv_api_key="AIzaSyCPHEaGhci712SM9UsB8f-Mdpl1lsA6VH0", 
                                         log_path = "/Volumes/exfat_archi/streetscope_test/delft",
                                         distance=1
                                         # grid = True, grid_size = 0.1
                                         )
-    sv_downloader.download_gsv_sync("/Volumes/exfat_archi/streetscope_test/delft/images", 
+    sv_downloader.download_gsv("/Volumes/exfat_archi/streetscope_test/delft/images", 
                             # path_pid = "/Volumes/exfat_archi/streetscope_test/delft/images/pids.csv",
                             input_shp_file = "/Volumes/exfat_archi/streetscope_test/delft/Delft/Delft.shp", augment_metadata=True)
     # sv_downloader.download_gsv("/Users/koichiito/Downloads/Delft", lat = 52.004400, lng = 4.342597, augment_metadata=True)
```

### Comparing `streetscope-0.3.5/src/streetscope/download/utils/UserAgent.csv` & `streetscope-0.3.6/src/streetscope/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.5/src/streetscope/download/utils/geoprocess.py` & `streetscope-0.3.6/src/streetscope/download/utils/geoprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,19 +48,14 @@
 
     def process_multipoint(self, gdf):
         gdf = gdf.explode('geometry').reset_index(drop=True)
         gdf['longitude'] = gdf.geometry.x
         gdf['latitude'] = gdf.geometry.y
         return gdf[['longitude', 'latitude']]
 
-    def get_sample_points(self, linestring, distance=20):
-        length = linestring.length
-        count = math.ceil(length / distance)
-        return [linestring.interpolate((i / count) * length) for i in range(count + 1)]
-
     def process_linestring(self, gdf):
         # Project the LineStrings to UTM
         gdf_utm = ox.projection.project_gdf(gdf)
         self.utm_crs = gdf_utm.crs
 
         # Use osmnx.utils_geo.interpolate_points function to interpolate points along LineStrings
         gdf_utm['sample_points'] = gdf_utm['geometry'].progress_apply(lambda geom: list(ox.utils_geo.interpolate_points(geom, dist=self.distance)), desc="Interpolating Points")
```

### Comparing `streetscope-0.3.5/src/streetscope/download/utils/imtool.py` & `streetscope-0.3.6/src/streetscope/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.5/src/streetscope/transform/transform_image.py` & `streetscope-0.3.6/src/streetscope/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.5/PKG-INFO` & `streetscope-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streetscope
-Version: 0.3.5
+Version: 0.3.6
 Summary: This package handles downloading, cleaning, analyzing street view imagery
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

