# Comparing `tmp/PyViCare-2.9.0.tar.gz` & `tmp/PyViCare-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyViCare-2.9.0.tar", last modified: Thu Sep 30 15:34:54 2021, max compression
+gzip compressed data, was "PyViCare-2.9.1.tar", last modified: Thu Sep 30 16:44:09 2021, max compression
```

## Comparing `PyViCare-2.9.0.tar` & `PyViCare-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2021-09-30 15:34:54.895755 PyViCare-2.9.0/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     8249 2021-09-30 15:34:54.895755 PyViCare-2.9.0/PKG-INFO
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2021-09-30 15:34:54.891755 PyViCare-2.9.0/PyViCare/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      513 2021-08-07 16:20:15.000000 PyViCare-2.9.0/PyViCare/Feature.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2859 2021-09-05 20:12:27.000000 PyViCare-2.9.0/PyViCare/PyViCare.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3092 2021-09-05 20:12:27.000000 PyViCare-2.9.0/PyViCare/PyViCareAbstractOAuthManager.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     5099 2021-08-16 18:46:32.000000 PyViCare-2.9.0/PyViCare/PyViCareBrowserOAuthManager.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1852 2021-09-09 11:01:07.000000 PyViCare-2.9.0/PyViCare/PyViCareCachedService.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    18790 2021-09-13 17:56:32.000000 PyViCare-2.9.0/PyViCare/PyViCareDevice.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2577 2021-09-05 20:12:27.000000 PyViCare-2.9.0/PyViCare/PyViCareDeviceConfig.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    15756 2021-09-02 18:32:04.000000 PyViCare-2.9.0/PyViCare/PyViCareFuelCell.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     6124 2021-09-30 15:34:37.000000 PyViCare-2.9.0/PyViCare/PyViCareGazBoiler.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2517 2021-09-05 20:12:27.000000 PyViCare-2.9.0/PyViCare/PyViCareHeatPump.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      142 2021-09-05 20:12:27.000000 PyViCare-2.9.0/PyViCare/PyViCareHybrid.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     5302 2021-08-16 18:46:32.000000 PyViCare-2.9.0/PyViCare/PyViCareOAuthManager.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      918 2021-09-30 15:34:37.000000 PyViCare-2.9.0/PyViCare/PyViCareOilBoiler.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     2652 2021-09-30 15:34:37.000000 PyViCare-2.9.0/PyViCare/PyViCarePelletsBoiler.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     1986 2021-08-16 18:46:32.000000 PyViCare-2.9.0/PyViCare/PyViCareService.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     3736 2021-09-09 15:15:45.000000 PyViCare-2.9.0/PyViCare/PyViCareUtils.py
--rw-rw-r--   0 lukas     (1000) lukas     (1000)        0 2021-08-07 16:20:15.000000 PyViCare-2.9.0/PyViCare/__init__.py
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2021-09-30 15:34:54.895755 PyViCare-2.9.0/PyViCare.egg-info/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     8249 2021-09-30 15:34:54.000000 PyViCare-2.9.0/PyViCare.egg-info/PKG-INFO
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      680 2021-09-30 15:34:54.000000 PyViCare-2.9.0/PyViCare.egg-info/SOURCES.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)        1 2021-09-30 15:34:54.000000 PyViCare-2.9.0/PyViCare.egg-info/dependency_links.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)       30 2021-09-30 15:34:54.000000 PyViCare-2.9.0/PyViCare.egg-info/requires.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)        9 2021-09-30 15:34:54.000000 PyViCare-2.9.0/PyViCare.egg-info/top_level.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     6532 2021-09-05 20:12:27.000000 PyViCare-2.9.0/README.md
--rw-rw-r--   0 lukas     (1000) lukas     (1000)       38 2021-09-30 15:34:54.895755 PyViCare-2.9.0/setup.cfg
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      783 2021-08-07 16:20:15.000000 PyViCare-2.9.0/setup.py
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2021-09-30 16:44:09.643934 PyViCare-2.9.1/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     8249 2021-09-30 16:44:09.643934 PyViCare-2.9.1/PKG-INFO
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2021-09-30 16:44:09.639934 PyViCare-2.9.1/PyViCare/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      513 2021-08-07 16:20:15.000000 PyViCare-2.9.1/PyViCare/Feature.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2859 2021-09-05 20:12:27.000000 PyViCare-2.9.1/PyViCare/PyViCare.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3092 2021-09-05 20:12:27.000000 PyViCare-2.9.1/PyViCare/PyViCareAbstractOAuthManager.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     5099 2021-08-16 18:46:32.000000 PyViCare-2.9.1/PyViCare/PyViCareBrowserOAuthManager.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     1852 2021-09-09 11:01:07.000000 PyViCare-2.9.1/PyViCare/PyViCareCachedService.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    18790 2021-09-13 17:56:32.000000 PyViCare-2.9.1/PyViCare/PyViCareDevice.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2577 2021-09-05 20:12:27.000000 PyViCare-2.9.1/PyViCare/PyViCareDeviceConfig.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)    15756 2021-09-02 18:32:04.000000 PyViCare-2.9.1/PyViCare/PyViCareFuelCell.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     6122 2021-09-30 16:43:57.000000 PyViCare-2.9.1/PyViCare/PyViCareGazBoiler.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2517 2021-09-05 20:12:27.000000 PyViCare-2.9.1/PyViCare/PyViCareHeatPump.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      142 2021-09-05 20:12:27.000000 PyViCare-2.9.1/PyViCare/PyViCareHybrid.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     5302 2021-08-16 18:46:32.000000 PyViCare-2.9.1/PyViCare/PyViCareOAuthManager.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      916 2021-09-30 16:43:57.000000 PyViCare-2.9.1/PyViCare/PyViCareOilBoiler.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     2650 2021-09-30 16:43:57.000000 PyViCare-2.9.1/PyViCare/PyViCarePelletsBoiler.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     1986 2021-08-16 18:46:32.000000 PyViCare-2.9.1/PyViCare/PyViCareService.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     3736 2021-09-09 15:15:45.000000 PyViCare-2.9.1/PyViCare/PyViCareUtils.py
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)        0 2021-08-07 16:20:15.000000 PyViCare-2.9.1/PyViCare/__init__.py
+drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2021-09-30 16:44:09.639934 PyViCare-2.9.1/PyViCare.egg-info/
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     8249 2021-09-30 16:44:09.000000 PyViCare-2.9.1/PyViCare.egg-info/PKG-INFO
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      680 2021-09-30 16:44:09.000000 PyViCare-2.9.1/PyViCare.egg-info/SOURCES.txt
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)        1 2021-09-30 16:44:09.000000 PyViCare-2.9.1/PyViCare.egg-info/dependency_links.txt
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)       30 2021-09-30 16:44:09.000000 PyViCare-2.9.1/PyViCare.egg-info/requires.txt
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)        9 2021-09-30 16:44:09.000000 PyViCare-2.9.1/PyViCare.egg-info/top_level.txt
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)     6532 2021-09-05 20:12:27.000000 PyViCare-2.9.1/README.md
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)       38 2021-09-30 16:44:09.643934 PyViCare-2.9.1/setup.cfg
+-rw-rw-r--   0 lukas     (1000) lukas     (1000)      783 2021-08-07 16:20:15.000000 PyViCare-2.9.1/setup.py
```

### Comparing `PyViCare-2.9.0/PKG-INFO` & `PyViCare-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyViCare
-Version: 2.9.0
+Version: 2.9.1
 Summary: Library to communicate with the Viessmann ViCare API
 Home-page: https://github.com/somm15/PyViCare
 Author: Simon Gillet
 Author-email: mail+pyvicare@gillet.ninja
 License: UNKNOWN
 Description: # PyViCare
```

### Comparing `PyViCare-2.9.0/PyViCare/Feature.py` & `PyViCare-2.9.1/PyViCare/Feature.py`

 * *Files identical despite different names*

### Comparing `PyViCare-2.9.0/PyViCare/PyViCare.py` & `PyViCare-2.9.1/PyViCare/PyViCare.py`

 * *Files identical despite different names*

### Comparing `PyViCare-2.9.0/PyViCare/PyViCareAbstractOAuthManager.py` & `PyViCare-2.9.1/PyViCare/PyViCareAbstractOAuthManager.py`

 * *Files identical despite different names*

### Comparing `PyViCare-2.9.0/PyViCare/PyViCareBrowserOAuthManager.py` & `PyViCare-2.9.1/PyViCare/PyViCareBrowserOAuthManager.py`

 * *Files identical despite different names*

### Comparing `PyViCare-2.9.0/PyViCare/PyViCareCachedService.py` & `PyViCare-2.9.1/PyViCare/PyViCareCachedService.py`

 * *Files identical despite different names*

### Comparing `PyViCare-2.9.0/PyViCare/PyViCareDevice.py` & `PyViCare-2.9.1/PyViCare/PyViCareDevice.py`

 * *Files identical despite different names*

### Comparing `PyViCare-2.9.0/PyViCare/PyViCareDeviceConfig.py` & `PyViCare-2.9.1/PyViCare/PyViCareDeviceConfig.py`

 * *Files identical despite different names*

### Comparing `PyViCare-2.9.0/PyViCare/PyViCareFuelCell.py` & `PyViCare-2.9.1/PyViCare/PyViCareFuelCell.py`

 * *Files identical despite different names*

### Comparing `PyViCare-2.9.0/PyViCare/PyViCareGazBoiler.py` & `PyViCare-2.9.1/PyViCare/PyViCareGazBoiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 class GazBurner(DeviceWithComponent):
 
     @property
     def burner(self) -> str:
         return self.component
 
     @handleNotSupported
-    def getIsActive(self):
+    def getActive(self):
         return self.service.getProperty(f"heating.burners.{self.burner}")["properties"]["active"]["value"]
 
     @handleNotSupported
     def getHours(self):
         return self.service.getProperty(f"heating.burners.{self.burner}.statistics")["properties"]["hours"]["value"]
 
     @handleNotSupported
```

### Comparing `PyViCare-2.9.0/PyViCare/PyViCareHeatPump.py` & `PyViCare-2.9.1/PyViCare/PyViCareHeatPump.py`

 * *Files identical despite different names*

### Comparing `PyViCare-2.9.0/PyViCare/PyViCareOAuthManager.py` & `PyViCare-2.9.1/PyViCare/PyViCareOAuthManager.py`

 * *Files identical despite different names*

### Comparing `PyViCare-2.9.0/PyViCare/PyViCareOilBoiler.py` & `PyViCare-2.9.1/PyViCare/PyViCareOilBoiler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from PyViCare.PyViCareDevice import Device
 from PyViCare.PyViCareUtils import handleNotSupported
 
 
 class OilBoiler(Device):
 
     @handleNotSupported
-    def getIsActive(self):
+    def getActive(self):
         return self.service.getProperty("heating.burner")["properties"]["active"]["value"]
 
     @handleNotSupported
     def getBurnerModulation(self):
         return self.service.getProperty('heating.burner.modulation')["properties"]["value"]["value"]
 
     @handleNotSupported
```

### Comparing `PyViCare-2.9.0/PyViCare/PyViCarePelletsBoiler.py` & `PyViCare-2.9.1/PyViCare/PyViCarePelletsBoiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from PyViCare.PyViCareDevice import Device
 from PyViCare.PyViCareUtils import handleNotSupported
 
 
 class PelletsBoiler(Device):
 
     @handleNotSupported
-    def getIsActive(self):
+    def getActive(self):
         return self.service.getProperty("heating.burner")["properties"]["active"]["value"]
 
     @handleNotSupported
     def getBurnerModulation(self):
         return self.service.getProperty('heating.burner.modulation')["properties"]["value"]["value"]
 
     @handleNotSupported
```

### Comparing `PyViCare-2.9.0/PyViCare/PyViCareService.py` & `PyViCare-2.9.1/PyViCare/PyViCareService.py`

 * *Files identical despite different names*

### Comparing `PyViCare-2.9.0/PyViCare/PyViCareUtils.py` & `PyViCare-2.9.1/PyViCare/PyViCareUtils.py`

 * *Files identical despite different names*

### Comparing `PyViCare-2.9.0/PyViCare.egg-info/PKG-INFO` & `PyViCare-2.9.1/PyViCare.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyViCare
-Version: 2.9.0
+Version: 2.9.1
 Summary: Library to communicate with the Viessmann ViCare API
 Home-page: https://github.com/somm15/PyViCare
 Author: Simon Gillet
 Author-email: mail+pyvicare@gillet.ninja
 License: UNKNOWN
 Description: # PyViCare
```

### Comparing `PyViCare-2.9.0/PyViCare.egg-info/SOURCES.txt` & `PyViCare-2.9.1/PyViCare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyViCare-2.9.0/README.md` & `PyViCare-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `PyViCare-2.9.0/setup.py` & `PyViCare-2.9.1/setup.py`

 * *Files identical despite different names*

