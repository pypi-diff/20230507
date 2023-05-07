# Comparing `tmp/streetscope-0.3.3.tar.gz` & `tmp/streetscope-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streetscope-0.3.3.tar", max compression
+gzip compressed data, was "streetscope-0.3.4.tar", max compression
```

## Comparing `streetscope-0.3.3.tar` & `streetscope-0.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0     1072 2023-04-28 01:06:03.496785 streetscope-0.3.3/LICENSE
--rw-r--r--   0        0        0      689 2023-04-28 01:06:03.507513 streetscope-0.3.3/README.md
--rw-r--r--   0        0        0      655 2023-05-07 05:39:36.908242 streetscope-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      141 2023-04-28 01:35:32.382729 streetscope-0.3.3/src/streetscope/__init__.py
--rw-r--r--   0        0        0       27 2023-04-28 01:36:07.601106 streetscope-0.3.3/src/streetscope/cv/__init__.py
--rw-r--r--   0        0        0       27 2023-04-28 10:12:41.686471 streetscope-0.3.3/src/streetscope/cv/segmentation/__init__.py
--rw-r--r--   0        0        0    39101 2023-05-05 01:28:21.346862 streetscope-0.3.3/src/streetscope/cv/segmentation/segmentation.py
--rw-r--r--   0        0        0       55 2023-04-13 03:44:34.089983 streetscope-0.3.3/src/streetscope/download/__init__.py
--rw-r--r--   0        0        0    11871 2023-05-07 05:36:40.959962 streetscope-0.3.3/src/streetscope/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-04-12 01:36:02.614098 streetscope-0.3.3/src/streetscope/download/utils/UserAgent.csv
--rw-r--r--   0        0        0        0 2023-04-12 07:50:41.918376 streetscope-0.3.3/src/streetscope/download/utils/__init__.py
--rw-r--r--   0        0        0     8754 2023-05-07 05:12:49.772501 streetscope-0.3.3/src/streetscope/download/utils/geoprocess.py
--rw-r--r--   0        0        0     3636 2023-05-07 05:25:22.808345 streetscope-0.3.3/src/streetscope/download/utils/get_pids.py
--rw-r--r--   0        0        0     8108 2023-05-05 23:52:21.840224 streetscope-0.3.3/src/streetscope/download/utils/imtool.py
--rw-r--r--   0        0        0        0 2023-04-28 01:06:03.540992 streetscope-0.3.3/src/streetscope/streetscope.py
--rw-r--r--   0        0        0       30 2023-05-03 02:17:38.864664 streetscope-0.3.3/src/streetscope/transform/__init__.py
--rw-r--r--   0        0        0     6768 2023-04-28 09:51:23.730858 streetscope-0.3.3/src/streetscope/transform/transform_image.py
--rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 streetscope-0.3.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-04-28 01:06:03.496785 streetscope-0.3.4/LICENSE
+-rw-r--r--   0        0        0      689 2023-04-28 01:06:03.507513 streetscope-0.3.4/README.md
+-rw-r--r--   0        0        0      655 2023-05-07 05:43:00.528988 streetscope-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      141 2023-04-28 01:35:32.382729 streetscope-0.3.4/src/streetscope/__init__.py
+-rw-r--r--   0        0        0       27 2023-04-28 01:36:07.601106 streetscope-0.3.4/src/streetscope/cv/__init__.py
+-rw-r--r--   0        0        0       27 2023-04-28 10:12:41.686471 streetscope-0.3.4/src/streetscope/cv/segmentation/__init__.py
+-rw-r--r--   0        0        0    39101 2023-05-05 01:28:21.346862 streetscope-0.3.4/src/streetscope/cv/segmentation/segmentation.py
+-rw-r--r--   0        0        0       55 2023-04-13 03:44:34.089983 streetscope-0.3.4/src/streetscope/download/__init__.py
+-rw-r--r--   0        0        0    11875 2023-05-07 05:42:23.024013 streetscope-0.3.4/src/streetscope/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-04-12 01:36:02.614098 streetscope-0.3.4/src/streetscope/download/utils/UserAgent.csv
+-rw-r--r--   0        0        0        0 2023-04-12 07:50:41.918376 streetscope-0.3.4/src/streetscope/download/utils/__init__.py
+-rw-r--r--   0        0        0     8754 2023-05-07 05:12:49.772501 streetscope-0.3.4/src/streetscope/download/utils/geoprocess.py
+-rw-r--r--   0        0        0     3636 2023-05-07 05:25:22.808345 streetscope-0.3.4/src/streetscope/download/utils/get_pids.py
+-rw-r--r--   0        0        0     8108 2023-05-05 23:52:21.840224 streetscope-0.3.4/src/streetscope/download/utils/imtool.py
+-rw-r--r--   0        0        0        0 2023-04-28 01:06:03.540992 streetscope-0.3.4/src/streetscope/streetscope.py
+-rw-r--r--   0        0        0       30 2023-05-03 02:17:38.864664 streetscope-0.3.4/src/streetscope/transform/__init__.py
+-rw-r--r--   0        0        0     6768 2023-04-28 09:51:23.730858 streetscope-0.3.4/src/streetscope/transform/transform_image.py
+-rw-r--r--   0        0        0     1750 1970-01-01 00:00:00.000000 streetscope-0.3.4/PKG-INFO
```

### Comparing `streetscope-0.3.3/LICENSE` & `streetscope-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.3/README.md` & `streetscope-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.3/pyproject.toml` & `streetscope-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streetscope"
-version = "0.3.3"
+version = "0.3.4"
 description = "This package handles downloading, cleaning, analyzing street view imagery"
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `streetscope-0.3.3/src/streetscope/cv/segmentation/segmentation.py` & `streetscope-0.3.4/src/streetscope/cv/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.3/src/streetscope/download/streetview_downloader.py` & `streetscope-0.3.4/src/streetscope/download/streetview_downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,17 +246,14 @@
         
         # If path_pid is None, call get_pids function first
         if path_pid is None:
             print("Getting pids...")
             path_pid = os.path.join(self.dir_output, "pids.csv")
             await self.get_pids(path_pid, lat=lat, lng=lng,
                         input_csv_file=input_csv_file, input_shp_file = input_shp_file, closest=closest, disp=disp, augment_metadata=augment_metadata)
-    
-    def download_gsv_sync(self, *args, **kwargs):
-        return asyncio.run(self.download_gsv(*args, **kwargs))
 
         # Horizontal Google Street View tiles
         # zoom 3: (8, 4); zoom 5: (26, 13) zoom 2: (4, 2) zoom 1: (2, 1);4:(8,16)
         # zoom = 2
         # h_tiles = 4  # 26
         # v_tiles = 2  # 13
         # cropped = False
@@ -269,14 +266,17 @@
         panoids_rest = self._check_already(panoids)
 
         panoids = self._read_pids(path_pid)
         panoids_rest = self._check_already(panoids)
 
         UAs = random.choices(self.user_agent, k = len(panoids_rest))
         ImageTool.dwl_multiple(panoids_rest, zoom, v_tiles, h_tiles, panorama_output, UAs, cropped, full, log_path=self.log_path)
+    
+    def download_gsv_sync(self, *args, **kwargs):
+            return asyncio.run(self.download_gsv(*args, **kwargs))
                 
 if __name__ == "__main__":
     sv_downloader = StreetViewDownloader(gsv_api_key="AIzaSyCPHEaGhci712SM9UsB8f-Mdpl1lsA6VH0", 
                                         log_path = "/Volumes/exfat_archi/streetscope_test/delft",
                                         distance=1
                                         # grid = True, grid_size = 0.1
                                         )
```

### Comparing `streetscope-0.3.3/src/streetscope/download/utils/UserAgent.csv` & `streetscope-0.3.4/src/streetscope/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.3/src/streetscope/download/utils/geoprocess.py` & `streetscope-0.3.4/src/streetscope/download/utils/geoprocess.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.3/src/streetscope/download/utils/get_pids.py` & `streetscope-0.3.4/src/streetscope/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.3/src/streetscope/download/utils/imtool.py` & `streetscope-0.3.4/src/streetscope/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.3/src/streetscope/transform/transform_image.py` & `streetscope-0.3.4/src/streetscope/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `streetscope-0.3.3/PKG-INFO` & `streetscope-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streetscope
-Version: 0.3.3
+Version: 0.3.4
 Summary: This package handles downloading, cleaning, analyzing street view imagery
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

