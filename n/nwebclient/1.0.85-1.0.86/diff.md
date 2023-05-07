# Comparing `tmp/nwebclient-1.0.85.tar.gz` & `tmp/nwebclient-1.0.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.85.tar", last modified: Sun May  7 11:24:55 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.86.tar", last modified: Sun May  7 11:35:14 2023, max compression
```

## Comparing `nwebclient-1.0.85.tar` & `nwebclient-1.0.86.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 11:24:55.421283 nwebclient-1.0.85/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.85/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-07 11:24:55.431283 nwebclient-1.0.85/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.85/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 11:24:55.421283 nwebclient-1.0.85/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     5993 2023-05-07 11:24:11.000000 nwebclient-1.0.85/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.85/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-05 19:49:25.000000 nwebclient-1.0.85/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)    10951 2023-05-06 17:29:25.000000 nwebclient-1.0.85/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.85/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.85/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 11:24:55.421283 nwebclient-1.0.85/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-07 11:24:55.000000 nwebclient-1.0.85/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-05-07 11:24:55.000000 nwebclient-1.0.85/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-07 11:24:55.000000 nwebclient-1.0.85/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-07 11:24:55.000000 nwebclient-1.0.85/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-07 11:24:55.000000 nwebclient-1.0.85/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-07 11:24:55.000000 nwebclient-1.0.85/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-07 11:24:55.431283 nwebclient-1.0.85/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-07 11:24:50.000000 nwebclient-1.0.85/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 11:35:14.541928 nwebclient-1.0.86/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.86/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-07 11:35:14.541928 nwebclient-1.0.86/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.86/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 11:35:14.541928 nwebclient-1.0.86/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6080 2023-05-07 11:34:00.000000 nwebclient-1.0.86/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.86/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-05 19:49:25.000000 nwebclient-1.0.86/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    10951 2023-05-06 17:29:25.000000 nwebclient-1.0.86/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.86/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.86/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 11:35:14.541928 nwebclient-1.0.86/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-07 11:35:14.000000 nwebclient-1.0.86/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-05-07 11:35:14.000000 nwebclient-1.0.86/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-07 11:35:14.000000 nwebclient-1.0.86/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-07 11:35:14.000000 nwebclient-1.0.86/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-07 11:35:14.000000 nwebclient-1.0.86/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-07 11:35:14.000000 nwebclient-1.0.86/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-07 11:35:14.541928 nwebclient-1.0.86/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-07 11:35:12.000000 nwebclient-1.0.86/setup.py
```

### Comparing `nwebclient-1.0.85/LICENSE` & `nwebclient-1.0.86/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.85/PKG-INFO` & `nwebclient-1.0.86/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.85
+Version: 1.0.86
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.85/README.md` & `nwebclient-1.0.86/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.85/nwebclient/__init__.py` & `nwebclient-1.0.86/nwebclient/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,18 @@
 class NWebClient:
     __url = ""
     __user = ""
     __pass = ""
     __cfg = {}
     ssl_verify = False
     def __init__(self, url, username = '', password = ''):
-        """ Anstatt url kann auch ein Pfad zur einer JSON-Datei, die die Schluessel enthaelt, angegeben werden. """
+        """
+          Anstatt url kann auch ein Pfad zur einer JSON-Datei, die die Schluessel enthaelt, angegeben werden. 
+          url https://bsnx.net/4.0/
+        """
         if url is None:
             if os.path.isfile('/etc/nweb.json'):
                 url = '/etc/nweb.json'
             if os.path.isfile('nweb.json'):
                 url = 'nweb.json'
         if url[0] == '/' or url.endswith('nweb.json'):
             self.__cfg = json.loads(self.file_get_contents(url))
@@ -134,25 +137,26 @@
         response = self.req("api/document/"+str(id), {format:"json"})
         #print(response)
         data = json.loads(response);
         return NWebDoc(self, data)
     def docs(self, q = ''):
         ja = self.req('w/api/docs?'+q);
         items = json.loads(ja)
-        return map(lambda x: NWebDoc(self, x), items)
+        return list(map(lambda x: NWebDoc(self, x), items))
     def group(self, id): 
         data = json.loads(self.req("api/group/"+id, {format:"json"}))
         return NWebGroup(self, data)
     def getOrCreateGroup(self, guid, title):
         return "TODO"
     def createDoc(self, name, content, group_id, kind='markup'):
         # https://bsnx.net/4.0/w/group/DBCD3638B55EA1ECE7EE1BDEC7E04131/create
         res = self.req("w/group/"+str(group_id)+"/create", {
             "title": name,
-            "content": content
+            "content": content,
+            "kind": kind
         })
         return res
     def deleteDoc(self, id):
         self.req('w/d/delete', {'confirm': 1})
     def downloadImages(self):
         # https://bsnx.net/4.0/w/api/docs?tag=Untertage
         docs = self.docs('kind=image&limit=1000')
```

### Comparing `nwebclient-1.0.85/nwebclient/__main__.py` & `nwebclient-1.0.86/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.85/nwebclient/crypt.py` & `nwebclient-1.0.86/nwebclient/crypt.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.85/nwebclient/sd.py` & `nwebclient-1.0.86/nwebclient/sd.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.85/nwebclient/sdb.py` & `nwebclient-1.0.86/nwebclient/sdb.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.85/nwebclient/ticker.py` & `nwebclient-1.0.86/nwebclient/ticker.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.85/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.86/nwebclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.85
+Version: 1.0.86
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.85/setup.py` & `nwebclient-1.0.86/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.85",
+    version="1.0.86",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
```

