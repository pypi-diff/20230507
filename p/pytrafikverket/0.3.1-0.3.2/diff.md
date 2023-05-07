# Comparing `tmp/pytrafikverket-0.3.1.tar.gz` & `tmp/pytrafikverket-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrafikverket-0.3.1.tar", last modified: Thu May  4 16:19:48 2023, max compression
+gzip compressed data, was "pytrafikverket-0.3.2.tar", last modified: Sun May  7 18:09:49 2023, max compression
```

## Comparing `pytrafikverket-0.3.1.tar` & `pytrafikverket-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-05-04 16:19:48.750889 pytrafikverket-0.3.1/
--rw-r--r--   0 gjo       (1000) gjo       (1000)     1072 2023-04-07 12:58:54.000000 pytrafikverket-0.3.1/LICENSE
--rw-r--r--   0 gjo       (1000) gjo       (1000)     2675 2023-05-04 16:19:48.750889 pytrafikverket-0.3.1/PKG-INFO
--rw-r--r--   0 gjo       (1000) gjo       (1000)     2138 2023-05-03 19:02:53.000000 pytrafikverket-0.3.1/README.md
-drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-05-04 16:19:48.740889 pytrafikverket-0.3.1/pytrafikverket/
--rw-r--r--   0 gjo       (1000) gjo       (1000)      632 2023-04-07 12:58:54.000000 pytrafikverket-0.3.1/pytrafikverket/__init__.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     6478 2023-05-03 18:52:58.000000 pytrafikverket-0.3.1/pytrafikverket/__main__.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     1327 2023-05-03 20:18:05.000000 pytrafikverket-0.3.1/pytrafikverket/exceptions.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)        0 2023-05-03 18:52:58.000000 pytrafikverket-0.3.1/pytrafikverket/py.typed
--rw-r--r--   0 gjo       (1000) gjo       (1000)     8786 2023-05-03 20:18:05.000000 pytrafikverket-0.3.1/pytrafikverket/trafikverket.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     3717 2023-05-03 19:06:27.000000 pytrafikverket-0.3.1/pytrafikverket/trafikverket_camera.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     9937 2023-05-03 18:52:58.000000 pytrafikverket-0.3.1/pytrafikverket/trafikverket_ferry.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)    12091 2023-05-03 20:07:04.000000 pytrafikverket-0.3.1/pytrafikverket/trafikverket_train.py
--rw-r--r--   0 gjo       (1000) gjo       (1000)     7309 2023-05-04 16:19:35.000000 pytrafikverket-0.3.1/pytrafikverket/trafikverket_weather.py
-drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-05-04 16:19:48.740889 pytrafikverket-0.3.1/pytrafikverket.egg-info/
--rw-r--r--   0 gjo       (1000) gjo       (1000)     2675 2023-05-04 16:19:48.000000 pytrafikverket-0.3.1/pytrafikverket.egg-info/PKG-INFO
--rw-r--r--   0 gjo       (1000) gjo       (1000)      547 2023-05-04 16:19:48.000000 pytrafikverket-0.3.1/pytrafikverket.egg-info/SOURCES.txt
--rw-r--r--   0 gjo       (1000) gjo       (1000)        1 2023-05-04 16:19:48.000000 pytrafikverket-0.3.1/pytrafikverket.egg-info/dependency_links.txt
--rw-r--r--   0 gjo       (1000) gjo       (1000)       27 2023-05-04 16:19:48.000000 pytrafikverket-0.3.1/pytrafikverket.egg-info/requires.txt
--rw-r--r--   0 gjo       (1000) gjo       (1000)       15 2023-05-04 16:19:48.000000 pytrafikverket-0.3.1/pytrafikverket.egg-info/top_level.txt
--rw-r--r--   0 gjo       (1000) gjo       (1000)        1 2023-05-03 20:20:24.000000 pytrafikverket-0.3.1/pytrafikverket.egg-info/zip-safe
--rw-r--r--   0 gjo       (1000) gjo       (1000)      170 2023-05-04 16:19:48.750889 pytrafikverket-0.3.1/setup.cfg
--rw-r--r--   0 gjo       (1000) gjo       (1000)     1067 2023-05-04 16:19:35.000000 pytrafikverket-0.3.1/setup.py
+drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-05-07 18:09:49.306672 pytrafikverket-0.3.2/
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     1072 2023-04-07 12:58:54.000000 pytrafikverket-0.3.2/LICENSE
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     2675 2023-05-07 18:09:49.306672 pytrafikverket-0.3.2/PKG-INFO
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     2138 2023-05-03 19:02:53.000000 pytrafikverket-0.3.2/README.md
+drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-05-07 18:09:49.306672 pytrafikverket-0.3.2/pytrafikverket/
+-rw-r--r--   0 gjo       (1000) gjo       (1000)      632 2023-04-07 12:58:54.000000 pytrafikverket-0.3.2/pytrafikverket/__init__.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     6478 2023-05-06 08:48:37.000000 pytrafikverket-0.3.2/pytrafikverket/__main__.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     1327 2023-05-03 20:18:05.000000 pytrafikverket-0.3.2/pytrafikverket/exceptions.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)        0 2023-05-03 18:52:58.000000 pytrafikverket-0.3.2/pytrafikverket/py.typed
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     8786 2023-05-06 08:48:37.000000 pytrafikverket-0.3.2/pytrafikverket/trafikverket.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     3717 2023-05-03 19:06:27.000000 pytrafikverket-0.3.2/pytrafikverket/trafikverket_camera.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     9937 2023-05-03 18:52:58.000000 pytrafikverket-0.3.2/pytrafikverket/trafikverket_ferry.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)    12091 2023-05-07 18:07:37.000000 pytrafikverket-0.3.2/pytrafikverket/trafikverket_train.py
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     7309 2023-05-04 16:19:35.000000 pytrafikverket-0.3.2/pytrafikverket/trafikverket_weather.py
+drwxr-xr-x   0 gjo       (1000) gjo       (1000)        0 2023-05-07 18:09:49.306672 pytrafikverket-0.3.2/pytrafikverket.egg-info/
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     2675 2023-05-07 18:09:49.000000 pytrafikverket-0.3.2/pytrafikverket.egg-info/PKG-INFO
+-rw-r--r--   0 gjo       (1000) gjo       (1000)      547 2023-05-07 18:09:49.000000 pytrafikverket-0.3.2/pytrafikverket.egg-info/SOURCES.txt
+-rw-r--r--   0 gjo       (1000) gjo       (1000)        1 2023-05-07 18:09:49.000000 pytrafikverket-0.3.2/pytrafikverket.egg-info/dependency_links.txt
+-rw-r--r--   0 gjo       (1000) gjo       (1000)       27 2023-05-07 18:09:49.000000 pytrafikverket-0.3.2/pytrafikverket.egg-info/requires.txt
+-rw-r--r--   0 gjo       (1000) gjo       (1000)       15 2023-05-07 18:09:49.000000 pytrafikverket-0.3.2/pytrafikverket.egg-info/top_level.txt
+-rw-r--r--   0 gjo       (1000) gjo       (1000)        1 2023-05-03 20:20:24.000000 pytrafikverket-0.3.2/pytrafikverket.egg-info/zip-safe
+-rw-r--r--   0 gjo       (1000) gjo       (1000)      170 2023-05-07 18:09:49.306672 pytrafikverket-0.3.2/setup.cfg
+-rw-r--r--   0 gjo       (1000) gjo       (1000)     1067 2023-05-07 18:09:32.000000 pytrafikverket-0.3.2/setup.py
```

### Comparing `pytrafikverket-0.3.1/LICENSE` & `pytrafikverket-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.1/PKG-INFO` & `pytrafikverket-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrafikverket
-Version: 0.3.1
+Version: 0.3.2
 Summary: Retreive values from public API at the Swedish Transport Administration (Trafikverket).
 Home-page: https://github.com/endor-force/pytrafikverket
 Author: Peter Andersson, Jonas Karlsson
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pytrafikverket-0.3.1/README.md` & `pytrafikverket-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.1/pytrafikverket/__init__.py` & `pytrafikverket-0.3.2/pytrafikverket/__init__.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.1/pytrafikverket/__main__.py` & `pytrafikverket-0.3.2/pytrafikverket/__main__.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.1/pytrafikverket/exceptions.py` & `pytrafikverket-0.3.2/pytrafikverket/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.1/pytrafikverket/trafikverket.py` & `pytrafikverket-0.3.2/pytrafikverket/trafikverket.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.1/pytrafikverket/trafikverket_camera.py` & `pytrafikverket-0.3.2/pytrafikverket/trafikverket_camera.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.1/pytrafikverket/trafikverket_ferry.py` & `pytrafikverket-0.3.2/pytrafikverket/trafikverket_ferry.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.1/pytrafikverket/trafikverket_train.py` & `pytrafikverket-0.3.2/pytrafikverket/trafikverket_train.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         location_advertised = node_helper.get_text("Advertised")
         return cls(location_signature, advertised_location_name, location_advertised)
 
 
 class TrainStopStatus(Enum):
     """Contain the different train stop statuses."""
 
-    ON_TIME = "scheduled to arrive on schedule"
+    ON_TIME = "on_time"
     DELAYED = "delayed"
     CANCELED = "canceled"
 
 
 class TrainStop:
     """Contain information about a train stop."""
 
@@ -95,28 +95,28 @@
         self.deviations = deviations
         self.modified_time = modified_time
         self.product_description = product_description
 
     def get_state(self) -> TrainStopStatus:
         """Retrieve the state of the departure."""
         if self.canceled:
-            return TrainStopStatus.CANCELED
+            return TrainStopStatus.CANCELED.value
         if (
             self.advertised_time_at_location is not None
             and self.time_at_location is not None
             and self.advertised_time_at_location != self.time_at_location
         ):
-            return TrainStopStatus.DELAYED
+            return TrainStopStatus.DELAYED.value
         if (
             self.advertised_time_at_location is not None
             and self.estimated_time_at_location is not None
             and self.advertised_time_at_location != self.estimated_time_at_location
         ):
-            return TrainStopStatus.DELAYED
-        return TrainStopStatus.ON_TIME
+            return TrainStopStatus.DELAYED.value
+        return TrainStopStatus.ON_TIME.value
 
     def get_delay_time(self) -> timedelta | None:
         """Calculate the delay of a departure."""
         if self.canceled:
             return None
         if (
             self.advertised_time_at_location is not None
```

### Comparing `pytrafikverket-0.3.1/pytrafikverket/trafikverket_weather.py` & `pytrafikverket-0.3.2/pytrafikverket/trafikverket_weather.py`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.1/pytrafikverket.egg-info/PKG-INFO` & `pytrafikverket-0.3.2/pytrafikverket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrafikverket
-Version: 0.3.1
+Version: 0.3.2
 Summary: Retreive values from public API at the Swedish Transport Administration (Trafikverket).
 Home-page: https://github.com/endor-force/pytrafikverket
 Author: Peter Andersson, Jonas Karlsson
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `pytrafikverket-0.3.1/pytrafikverket.egg-info/SOURCES.txt` & `pytrafikverket-0.3.2/pytrafikverket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytrafikverket-0.3.1/setup.py` & `pytrafikverket-0.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="UTF-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pytrafikverket",
-    version="0.3.1",
+    version="0.3.2",
     description="Retreive values from public API at the Swedish Transport Administration (Trafikverket).",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/endor-force/pytrafikverket",
     author="Peter Andersson, Jonas Karlsson",
     license="MIT",
     classifiers=[
```

