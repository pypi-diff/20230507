# Comparing `tmp/nwebclient-1.0.86.tar.gz` & `tmp/nwebclient-1.0.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.86.tar", last modified: Sun May  7 11:35:14 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.87.tar", last modified: Sun May  7 13:57:03 2023, max compression
```

## Comparing `nwebclient-1.0.86.tar` & `nwebclient-1.0.87.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 11:35:14.541928 nwebclient-1.0.86/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.86/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-07 11:35:14.541928 nwebclient-1.0.86/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.86/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 11:35:14.541928 nwebclient-1.0.86/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     6080 2023-05-07 11:34:00.000000 nwebclient-1.0.86/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.86/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-05 19:49:25.000000 nwebclient-1.0.86/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)    10951 2023-05-06 17:29:25.000000 nwebclient-1.0.86/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.86/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.86/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 11:35:14.541928 nwebclient-1.0.86/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-07 11:35:14.000000 nwebclient-1.0.86/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-05-07 11:35:14.000000 nwebclient-1.0.86/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-07 11:35:14.000000 nwebclient-1.0.86/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-07 11:35:14.000000 nwebclient-1.0.86/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-07 11:35:14.000000 nwebclient-1.0.86/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-07 11:35:14.000000 nwebclient-1.0.86/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-07 11:35:14.541928 nwebclient-1.0.86/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-07 11:35:12.000000 nwebclient-1.0.86/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 13:57:03.081592 nwebclient-1.0.87/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.87/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-07 13:57:03.081592 nwebclient-1.0.87/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.87/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 13:57:03.081592 nwebclient-1.0.87/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6475 2023-05-07 13:56:35.000000 nwebclient-1.0.87/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.87/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-05 19:49:25.000000 nwebclient-1.0.87/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    10951 2023-05-06 17:29:25.000000 nwebclient-1.0.87/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.87/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.87/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-07 13:57:03.081592 nwebclient-1.0.87/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-07 13:57:02.000000 nwebclient-1.0.87/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-05-07 13:57:02.000000 nwebclient-1.0.87/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-07 13:57:02.000000 nwebclient-1.0.87/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-07 13:57:02.000000 nwebclient-1.0.87/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-07 13:57:02.000000 nwebclient-1.0.87/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-07 13:57:02.000000 nwebclient-1.0.87/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-07 13:57:03.081592 nwebclient-1.0.87/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-07 13:56:54.000000 nwebclient-1.0.87/setup.py
```

### Comparing `nwebclient-1.0.86/LICENSE` & `nwebclient-1.0.87/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.86/PKG-INFO` & `nwebclient-1.0.87/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.86
+Version: 1.0.87
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.86/README.md` & `nwebclient-1.0.87/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.86/nwebclient/__init__.py` & `nwebclient-1.0.87/nwebclient/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 import json
 # add .parse in python3
 import urllib
+import sys
 import os.path
 
 #import .sdb as sdb
 
 name = "nwebclient"
 
 class NWebGroup:
@@ -60,14 +61,16 @@
         print(self.__data)
         #for key, value in self.__data.iteritems():
         #    print key + ": " + value
     def downloadThumbnail(self, size = 'nn'):
         # TODO imple   
         path = 'image/'+self.id()+'/thumbnail/'+size+'/'+self.id()+'.jpg'
         return 0
+    def save(self, file):
+        self.__client.reqToFile('/w/d/'+str(self.id())+'/download', file)
     def setContent(self, content):
         self.__data['content'] = content
         self.__client.req('api/document/'+self.__data['document_id'], {
             'action': 'update',
             'content': content
         })
 class NWebClient:
@@ -135,14 +138,15 @@
         r = requests.post(url, files=files, data=values)
     def doc(self, id):
         response = self.req("api/document/"+str(id), {format:"json"})
         #print(response)
         data = json.loads(response);
         return NWebDoc(self, data)
     def docs(self, q = ''):
+        """ Syntax: q """
         ja = self.req('w/api/docs?'+q);
         items = json.loads(ja)
         return list(map(lambda x: NWebDoc(self, x), items))
     def group(self, id): 
         data = json.loads(self.req("api/group/"+id, {format:"json"}))
         return NWebGroup(self, data)
     def getOrCreateGroup(self, guid, title):
@@ -151,27 +155,34 @@
         # https://bsnx.net/4.0/w/group/DBCD3638B55EA1ECE7EE1BDEC7E04131/create
         res = self.req("w/group/"+str(group_id)+"/create", {
             "title": name,
             "content": content,
             "kind": kind
         })
         return res
+    def createFileDoc(self, name, group_id, data):
+        """  open('file', 'rb') """
+        self.upload("w/group/"+str(group_id)+"/create", {
+            "title": name,
+            "kind": 'binary'
+        }, 'file', data)
     def deleteDoc(self, id):
-        self.req('w/d/delete', {'confirm': 1})
+        self.req('w/d/'+str(id)+'/delete', {'confirm': 1})
     def downloadImages(self):
         # https://bsnx.net/4.0/w/api/docs?tag=Untertage
         docs = self.docs('kind=image&limit=1000')
         for doc in docs:
            self.reqToFile('image/'+str(doc.id())+'/orginal/web/'+str(doc.id())+'.jpg', str(doc.id())+ '.jpg')
            print("Download Image: " + str(doc.id()))
 
 def metric_val(baseUrl, metricName, val):
     """ baseUrl: string = e.g. https://bsnx.net/metric-endpoint """
     requests.get(url=baseUrl, params= {'metric':metricName, 'val':val})
 
 def main():
     print("nx-c")
     c = NWebClient(None)
+    print(sys.argv)
     print(str(c.docs()))
 
 if __name__ == '__main__': # nx-c vom python-package bereitgestellt
     main()
```

### Comparing `nwebclient-1.0.86/nwebclient/__main__.py` & `nwebclient-1.0.87/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.86/nwebclient/crypt.py` & `nwebclient-1.0.87/nwebclient/crypt.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.86/nwebclient/sd.py` & `nwebclient-1.0.87/nwebclient/sd.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.86/nwebclient/sdb.py` & `nwebclient-1.0.87/nwebclient/sdb.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.86/nwebclient/ticker.py` & `nwebclient-1.0.87/nwebclient/ticker.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.86/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.87/nwebclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.86
+Version: 1.0.87
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.86/setup.py` & `nwebclient-1.0.87/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.86",
+    version="1.0.87",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
```

