# Comparing `tmp/photoprism_client-0.1.1.tar.gz` & `tmp/photoprism_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/photoprism_client-0.1.1.tar", last modified: Mon Nov  7 08:39:14 2022, max compression
+gzip compressed data, was "dist/photoprism_client-0.1.3.tar", last modified: Tue Nov 22 21:37:55 2022, max compression
```

## Comparing `photoprism_client-0.1.1.tar` & `photoprism_client-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mvanleeuwen   (501) staff       (20)        0 2022-11-07 08:39:14.000000 photoprism_client-0.1.1/
-drwxr-xr-x   0 mvanleeuwen   (501) staff       (20)        0 2022-11-07 08:39:14.000000 photoprism_client-0.1.1/photoprism_client.egg-info/
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)     5411 2022-11-07 08:39:14.000000 photoprism_client-0.1.1/photoprism_client.egg-info/PKG-INFO
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)        9 2022-11-07 08:39:14.000000 photoprism_client-0.1.1/photoprism_client.egg-info/requires.txt
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)       11 2022-11-07 08:39:14.000000 photoprism_client-0.1.1/photoprism_client.egg-info/top_level.txt
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)      297 2022-11-07 08:39:14.000000 photoprism_client-0.1.1/photoprism_client.egg-info/SOURCES.txt
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)        1 2022-11-07 08:39:14.000000 photoprism_client-0.1.1/photoprism_client.egg-info/dependency_links.txt
-drwxr-xr-x   0 mvanleeuwen   (501) staff       (20)        0 2022-11-07 08:39:14.000000 photoprism_client-0.1.1/photoprism/
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)      689 2022-11-06 12:24:57.000000 photoprism_client-0.1.1/photoprism/Session.py
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)        0 2022-03-25 19:21:56.000000 photoprism_client-0.1.1/photoprism/__init__.py
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)     5244 2022-11-07 07:24:38.000000 photoprism_client-0.1.1/photoprism/Photo.py
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)     5411 2022-11-07 08:39:14.000000 photoprism_client-0.1.1/PKG-INFO
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)      544 2022-11-07 08:39:13.000000 photoprism_client-0.1.1/setup.py
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)     4515 2022-11-07 07:24:38.000000 photoprism_client-0.1.1/README.md
--rw-r--r--   0 mvanleeuwen   (501) staff       (20)      103 2022-11-07 08:39:14.000000 photoprism_client-0.1.1/setup.cfg
+drwxr-xr-x   0 mvanleeuwen   (501) staff       (20)        0 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/
+drwxr-xr-x   0 mvanleeuwen   (501) staff       (20)        0 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/photoprism_client.egg-info/
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)     5741 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/photoprism_client.egg-info/PKG-INFO
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)        9 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/photoprism_client.egg-info/requires.txt
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)       11 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/photoprism_client.egg-info/top_level.txt
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)      297 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/photoprism_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)        1 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/photoprism_client.egg-info/dependency_links.txt
+drwxr-xr-x   0 mvanleeuwen   (501) staff       (20)        0 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/photoprism/
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)      689 2022-11-06 12:24:57.000000 photoprism_client-0.1.3/photoprism/Session.py
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)        0 2022-03-25 19:21:56.000000 photoprism_client-0.1.3/photoprism/__init__.py
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)     5851 2022-11-22 21:16:32.000000 photoprism_client-0.1.3/photoprism/Photo.py
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)     5741 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/PKG-INFO
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)      544 2022-11-22 21:35:02.000000 photoprism_client-0.1.3/setup.py
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)     4829 2022-11-22 21:29:35.000000 photoprism_client-0.1.3/README.md
+-rw-r--r--   0 mvanleeuwen   (501) staff       (20)      103 2022-11-22 21:37:55.000000 photoprism_client-0.1.3/setup.cfg
```

### Comparing `photoprism_client-0.1.1/photoprism_client.egg-info/PKG-INFO` & `photoprism_client-0.1.3/photoprism_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photoprism-client
-Version: 0.1.1
+Version: 0.1.3
 Summary: A Python client to interact with photoprism. 
 Home-page: https://github.com/mvlnetdev/photoprism_client
 Author: mvlnetdev
 Author-email: maartenvanleeuwen1996@gmail.com
 License: MIT license
 Description: # Python client for PhotoPrism 
         A Python client to interact with photoprism.
@@ -18,15 +18,15 @@
         - requests (latest)
         
         ## Setup
         To start interacting with Photoprism set up a session. You always need to do this if you start the script. Otherwise there is no session for the client to interact with PhotoPrism.
         ``` python
         from photoprism.Session import Session
         pp_session = Session("admin", "changethis", "demo.photoprism.app")
-        pp.session.create()
+        pp_session.create()
         ```
         
         ## Searching
         To search for photos. With this example it will return the first 100 results. You can change this with `count=1000`.
         
         ```python
         from photoprism.Photo import Photo
@@ -47,14 +47,16 @@
         | Photo.get_album_uid_by_name() | Get the UID of an album using the name of the album. Be aware, it uses the list_albums function that is limited to 100000 albums | name: string | String of uid, None if it does not exist |
         | Photo.get_uid_list_of_search() | Return a list of UIDs based upon the search | query: string, count: int (default is 100) | list of uids |
         | Photo.list_albums() | Provide a list of all albums within the photoprism instance, with a max of 100000 | None | Dict object with all albums and their metadata (max of 100000 results) |
         | Photo.raw_call() | Function to perform a request to the photoprism server (usually not needed by a user) | endpoint: string, type: string (default="GET"), data: string (default=False) | requests object |
         | Photo.search() | Create the session | query: string, count: int (default=100) | Dict object of the results of the search |
         | Photo.start_import() | Start an import job, default path is upload. It returns True when the import started, not when finished | path: string (default="upload"), move: Bool (default=False) | True if successfully started |
         | Photo.stop_import() | Stop an import job | None | True if successfully stopped |
+        | Photo.remove_photos_from_album() | Remove photos from an album, Returns True if successfull | albumname: string, photos: bool (default=False), count: int (default=1000000) | True if succesfull |
+        | Photo.remove_album() | Remove album based on album name | albumname: string | Dict data returned from the server |
         
         ## License 
         MIT License
         
         Copyright (c) 2022 maartenvl
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `photoprism_client-0.1.1/photoprism/Session.py` & `photoprism_client-0.1.3/photoprism/Session.py`

 * *Files identical despite different names*

### Comparing `photoprism_client-0.1.1/photoprism/Photo.py` & `photoprism_client-0.1.3/photoprism/Photo.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 
 from photoprism import Session
 import requests, json
 
 class Photo():
     def __init__(self, session):
         """Initialize based upon a session"""
-        if type(session) == Session.Session:
-            self.session = session
-        else:
-            TypeError(f"session variable is not of type photoprism.Session.Session, but {type(session)}")
+        if type(session) != Session.Session:
+            raise TypeError(f"session variable is not of type photoprism.Session.Session, but {type(session)}")
 
+        self.session = session
         self.header = {
             "X-Session-ID": self.session.session_id}
 
 
     def search(self, query, count=100):
         """Basic search function. Returns a Dict object based upon the returned JSON"""
 
@@ -39,117 +38,137 @@
         r = requests.get(url, headers=self.header)
         return json.loads(r.text)
 
     def check_if_album_exists(self, name, create_if_not=False):
         """Small function to check if an album exists"""
 
         data = self.list_albums()
-        exists = False
         for d in data:
             if name == d["Title"]:
-                exists = True
+                return True
 
-        if exists == False:
-            if create_if_not:
-                self.create_album(name)
+        if create_if_not:
+            self.create_album(name)
 
-        return exists
+        return False
 
     def get_album_uid_by_name(self, name):
         """Get the UID of an album using the name of the album. Be aware, it uses the list_albums function that is limited to 100000 albums"""
 
         data = self.list_albums()
         uid = None
         for d in data:
             if name == d["Title"]:
-                uid = d["UID"]
-        if uid == None:
-            return False
-        else:
-            return uid
+                return d["UID"]
+        
+        return False
 
     def create_album(self, title):
         """Create an album, returns a boolean if it worked"""
 
         url = f"{self.session.url}/albums"
         data = {"Title":title,"Favorite":False}
         r = requests.post(url=url, data=json.dumps(data), headers=self.header)
-        result = False
+        
         if r.status_code == 200:
-            result = True
-        return result
+            return True
+        
+        return False
 
     def add_photos_to_album(self, photos, album_uid):
         """Add photos to an album, you will need to provide a list of UIDs of the photos you want to add. Returns True if successfull"""
 
         url = f"{self.session.url}/albums/{album_uid}/photos"
         data = {
             "photos":photos
         }
         r = requests.post(url, data=json.dumps(data), headers=self.header)
-        result = False
+        
         if r.status_code == 200:
-            result = True
-        return result
+            return True
+
+        return False
 
     def add_to_album_from_query(self, query, albumname):
         """Provide a search query and add all photos that are returned into an album. Provide the albumname, not the UID of the album."""
 
         self.check_if_album_exists(albumname, create_if_not=True)
         album_uid = self.get_album_uid_by_name(albumname)
         photolist = self.get_uid_list_of_search(query, count=1000000)
         result = self.add_photos_to_album(photolist, album_uid)
-        print(result)
+        return result
 
     def get_album(self, uid):
         """Get all information of an album based upon the UID of the album"""
 
         url = f"{self.session.url}/albums/{uid}"
         r = requests.get(url, headers=self.header)
+        
+        if r.status_code == 200:
+            return json.loads(r.text)
+        
+        return False
+
+    def remove_photos_from_album(self,albumname, photos=False, count=1000000):
+        """Remove photos from an album, Returns True if successfull"""
+        album_uid = self.get_album_uid_by_name(albumname)
+        if photos == False:
+            query = f"album:\"{albumname}\""
+            photos = self.get_uid_list_of_search(query,count=count)
+
+        url = f"{self.session.url}/albums/{album_uid}/photos"
+        data = {
+            "photos":photos
+        }
+        r = requests.delete(url, data=json.dumps(data), headers=self.header)
+        result = False
+        if r.status_code == 200:
+            result = True
+        return result
+
+    def remove_album(self, albumname):
+        """Remove album based on album name"""
+        album_uid = self.get_album_uid_by_name(albumname)
+        url = f"{self.session.url}/albums/{album_uid}"
+        r = requests.delete(url, headers=self.header)
         result = False
         if r.status_code == 200:
             result = json.loads(r.text)
         return result
 
     def start_import(self, path="upload", move=False):
         """Start an import job, default path is upload. It returns True when the import started, not when finished"""
 
         url = f"{self.session.url}/import"
         data = {
             "path": path,
             "move": move
         }
         r = requests.post(url, data=json.dumps(data), headers=self.header)
-        result = False
+        
         if r.status_code == 200:
-            result = True
-        return result
+            return True
+        
+        return False
 
     def stop_import(self):
         """Stop an import job"""
         url = f"{self.session.url}/import"
         r = requests.delete(url, headers=self.header)
-        result = False
+
         if r.status_code == 200:
-            result = True
-        return result
+            return True
+        
+        return False
 
-    def raw_call(self, endpoint, type="GET", data=False):
+    def raw_call(self, endpoint, type="GET", data=None):
         """Function to perform a request to the photoprism server"""
 
         url = f"{self.session.url}/{endpoint}"
         if type == "GET":
-            if data:
-                r = requests.get(url, data = json.dumps(data), headers=self.header)
-            else:
-                r = requests.get(url, headers=self.header)
+            return requests.get(url, headers=self.header)
         elif type == "POST":
-            if data:
-                r = requests.post(url, data = json.dumps(data), headers=self.header)
-            else:
-                r = requests.post(url, headers=self.header)
+            return requests.post(url, data=json.dumps(data) if data else None, headers=self.header)
         elif type == "DELETE":
-            r = requests.delete(url, headers=self.header)
-        else:
-            r = False
-
-        return r
+            return requests.delete(url, headers=self.header)
+        
+        return False
```

### Comparing `photoprism_client-0.1.1/PKG-INFO` & `photoprism_client-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photoprism_client
-Version: 0.1.1
+Version: 0.1.3
 Summary: A Python client to interact with photoprism. 
 Home-page: https://github.com/mvlnetdev/photoprism_client
 Author: mvlnetdev
 Author-email: maartenvanleeuwen1996@gmail.com
 License: MIT license
 Description: # Python client for PhotoPrism 
         A Python client to interact with photoprism.
@@ -18,15 +18,15 @@
         - requests (latest)
         
         ## Setup
         To start interacting with Photoprism set up a session. You always need to do this if you start the script. Otherwise there is no session for the client to interact with PhotoPrism.
         ``` python
         from photoprism.Session import Session
         pp_session = Session("admin", "changethis", "demo.photoprism.app")
-        pp.session.create()
+        pp_session.create()
         ```
         
         ## Searching
         To search for photos. With this example it will return the first 100 results. You can change this with `count=1000`.
         
         ```python
         from photoprism.Photo import Photo
@@ -47,14 +47,16 @@
         | Photo.get_album_uid_by_name() | Get the UID of an album using the name of the album. Be aware, it uses the list_albums function that is limited to 100000 albums | name: string | String of uid, None if it does not exist |
         | Photo.get_uid_list_of_search() | Return a list of UIDs based upon the search | query: string, count: int (default is 100) | list of uids |
         | Photo.list_albums() | Provide a list of all albums within the photoprism instance, with a max of 100000 | None | Dict object with all albums and their metadata (max of 100000 results) |
         | Photo.raw_call() | Function to perform a request to the photoprism server (usually not needed by a user) | endpoint: string, type: string (default="GET"), data: string (default=False) | requests object |
         | Photo.search() | Create the session | query: string, count: int (default=100) | Dict object of the results of the search |
         | Photo.start_import() | Start an import job, default path is upload. It returns True when the import started, not when finished | path: string (default="upload"), move: Bool (default=False) | True if successfully started |
         | Photo.stop_import() | Stop an import job | None | True if successfully stopped |
+        | Photo.remove_photos_from_album() | Remove photos from an album, Returns True if successfull | albumname: string, photos: bool (default=False), count: int (default=1000000) | True if succesfull |
+        | Photo.remove_album() | Remove album based on album name | albumname: string | Dict data returned from the server |
         
         ## License 
         MIT License
         
         Copyright (c) 2022 maartenvl
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `photoprism_client-0.1.1/setup.py` & `photoprism_client-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name='photoprism_client',
-    version='0.1.1',
+    version='0.1.3',
     packages=['photoprism'],
     url='https://github.com/mvlnetdev/photoprism_client',
     license='MIT license',
     author='mvlnetdev',
     author_email='maartenvanleeuwen1996@gmail.com',
     description='A Python client to interact with photoprism. ',
     long_description=readme,
```

### Comparing `photoprism_client-0.1.1/README.md` & `photoprism_client-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 - requests (latest)
 
 ## Setup
 To start interacting with Photoprism set up a session. You always need to do this if you start the script. Otherwise there is no session for the client to interact with PhotoPrism.
 ``` python
 from photoprism.Session import Session
 pp_session = Session("admin", "changethis", "demo.photoprism.app")
-pp.session.create()
+pp_session.create()
 ```
 
 ## Searching
 To search for photos. With this example it will return the first 100 results. You can change this with `count=1000`.
 
 ```python
 from photoprism.Photo import Photo
@@ -39,14 +39,16 @@
 | Photo.get_album_uid_by_name() | Get the UID of an album using the name of the album. Be aware, it uses the list_albums function that is limited to 100000 albums | name: string | String of uid, None if it does not exist |
 | Photo.get_uid_list_of_search() | Return a list of UIDs based upon the search | query: string, count: int (default is 100) | list of uids |
 | Photo.list_albums() | Provide a list of all albums within the photoprism instance, with a max of 100000 | None | Dict object with all albums and their metadata (max of 100000 results) |
 | Photo.raw_call() | Function to perform a request to the photoprism server (usually not needed by a user) | endpoint: string, type: string (default="GET"), data: string (default=False) | requests object |
 | Photo.search() | Create the session | query: string, count: int (default=100) | Dict object of the results of the search |
 | Photo.start_import() | Start an import job, default path is upload. It returns True when the import started, not when finished | path: string (default="upload"), move: Bool (default=False) | True if successfully started |
 | Photo.stop_import() | Stop an import job | None | True if successfully stopped |
+| Photo.remove_photos_from_album() | Remove photos from an album, Returns True if successfull | albumname: string, photos: bool (default=False), count: int (default=1000000) | True if succesfull |
+| Photo.remove_album() | Remove album based on album name | albumname: string | Dict data returned from the server |
 
 ## License 
 MIT License
 
 Copyright (c) 2022 maartenvl
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

