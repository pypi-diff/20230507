# Comparing `tmp/nwebclient-1.0.84.tar.gz` & `tmp/nwebclient-1.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.84.tar", last modified: Sun May  7 11:19:09 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.85.tar", last modified: Sun May  7 11:24:55 2023, max compression
```

## Comparing `nwebclient-1.0.84.tar` & `nwebclient-1.0.85.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 11:19:09.176692 nwebclient-1.0.84/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.84/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-07 11:19:09.176692 nwebclient-1.0.84/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.84/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 11:19:09.176692 nwebclient-1.0.84/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     5983 2023-05-07 10:27:03.000000 nwebclient-1.0.84/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.84/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-05 19:49:25.000000 nwebclient-1.0.84/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)    10951 2023-05-06 17:29:25.000000 nwebclient-1.0.84/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.84/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.84/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 11:19:09.176692 nwebclient-1.0.84/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-07 11:19:09.000000 nwebclient-1.0.84/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-05-07 11:19:09.000000 nwebclient-1.0.84/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-07 11:19:09.000000 nwebclient-1.0.84/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-07 11:19:09.000000 nwebclient-1.0.84/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-07 11:19:09.000000 nwebclient-1.0.84/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-07 11:19:09.000000 nwebclient-1.0.84/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-07 11:19:09.176692 nwebclient-1.0.84/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-07 10:00:23.000000 nwebclient-1.0.84/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 11:24:55.421283 nwebclient-1.0.85/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.85/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-07 11:24:55.431283 nwebclient-1.0.85/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.85/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 11:24:55.421283 nwebclient-1.0.85/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     5993 2023-05-07 11:24:11.000000 nwebclient-1.0.85/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.85/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-05 19:49:25.000000 nwebclient-1.0.85/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    10951 2023-05-06 17:29:25.000000 nwebclient-1.0.85/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.85/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.85/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 11:24:55.421283 nwebclient-1.0.85/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-07 11:24:55.000000 nwebclient-1.0.85/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-05-07 11:24:55.000000 nwebclient-1.0.85/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-07 11:24:55.000000 nwebclient-1.0.85/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-07 11:24:55.000000 nwebclient-1.0.85/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-07 11:24:55.000000 nwebclient-1.0.85/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-07 11:24:55.000000 nwebclient-1.0.85/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-07 11:24:55.431283 nwebclient-1.0.85/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-07 11:24:50.000000 nwebclient-1.0.85/setup.py
```

### Comparing `nwebclient-1.0.84/LICENSE` & `nwebclient-1.0.85/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.84/PKG-INFO` & `nwebclient-1.0.85/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.84
+Version: 1.0.85
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.84/README.md` & `nwebclient-1.0.85/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.84/nwebclient/__init__.py` & `nwebclient-1.0.85/nwebclient/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         if self.__user != "":
             params["username"]= self.__user
             params["password"]= self.__pass
         url = self.__url+path
         #print("NWEB-Client: " + url);
         res = requests.post(url, data=params, verify=self.ssl_verify)
         return res.text
-    def upload(self, path, params = {}, name, data):
+    def upload(self, path, params={}, name='file', data=None):
         """ open('file.txt','rb') """
         url = self.__url+path
         if self.__user != "":
             params["username"]= self.__user
             params["password"]= self.__pass
         files = {name: data}
         r = requests.post(url, files=files, data=values)
```

### Comparing `nwebclient-1.0.84/nwebclient/__main__.py` & `nwebclient-1.0.85/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.84/nwebclient/crypt.py` & `nwebclient-1.0.85/nwebclient/crypt.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.84/nwebclient/sd.py` & `nwebclient-1.0.85/nwebclient/sd.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.84/nwebclient/sdb.py` & `nwebclient-1.0.85/nwebclient/sdb.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.84/nwebclient/ticker.py` & `nwebclient-1.0.85/nwebclient/ticker.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.84/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.85/nwebclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.84
+Version: 1.0.85
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.84/setup.py` & `nwebclient-1.0.85/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.84",
+    version="1.0.85",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
```

