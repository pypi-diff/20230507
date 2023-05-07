# Comparing `tmp/scratchattach-1.1.4.tar.gz` & `tmp/scratchattach-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.1.4.tar", last modified: Thu May  4 17:47:55 2023, max compression
+gzip compressed data, was "scratchattach-1.1.5.tar", last modified: Sun May  7 17:33:08 2023, max compression
```

## Comparing `scratchattach-1.1.4.tar` & `scratchattach-1.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 17:47:55.286839 scratchattach-1.1.4/
--rw-rw-rw-   0        0        0    21811 2023-05-04 17:47:55.285838 scratchattach-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    20499 2023-05-04 17:45:21.000000 scratchattach-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 17:47:55.214501 scratchattach-1.1.4/scratchattach/
--rw-rw-rw-   0        0        0      167 2023-05-04 16:19:46.000000 scratchattach-1.1.4/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    12798 2023-05-04 17:35:55.000000 scratchattach-1.1.4/scratchattach/_cloud.py
--rw-rw-rw-   0        0        0    15496 2023-05-04 17:24:58.000000 scratchattach-1.1.4/scratchattach/_cloud_requests.py
--rw-rw-rw-   0        0        0     1797 2023-05-04 16:19:46.000000 scratchattach-1.1.4/scratchattach/_encoder.py
--rw-rw-rw-   0        0        0      779 2023-05-04 16:19:46.000000 scratchattach-1.1.4/scratchattach/_exceptions.py
--rw-rw-rw-   0        0        0     6542 2023-05-04 16:19:46.000000 scratchattach-1.1.4/scratchattach/_forum.py
--rw-rw-rw-   0        0        0    18152 2023-05-04 16:19:46.000000 scratchattach-1.1.4/scratchattach/_project.py
--rw-rw-rw-   0        0        0    17923 2023-05-04 16:19:46.000000 scratchattach-1.1.4/scratchattach/_session.py
--rw-rw-rw-   0        0        0     9651 2023-05-04 16:19:46.000000 scratchattach-1.1.4/scratchattach/_studio.py
--rw-rw-rw-   0        0        0    25071 2023-05-04 16:19:46.000000 scratchattach-1.1.4/scratchattach/_user.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:47:55.281296 scratchattach-1.1.4/scratchattach.egg-info/
--rw-rw-rw-   0        0        0    21811 2023-05-04 17:47:54.000000 scratchattach-1.1.4/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-05-04 17:47:55.000000 scratchattach-1.1.4/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 17:47:54.000000 scratchattach-1.1.4/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-04 17:47:54.000000 scratchattach-1.1.4/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-04 17:47:54.000000 scratchattach-1.1.4/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 17:47:55.287210 scratchattach-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-05-04 16:38:08.000000 scratchattach-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 17:33:08.802517 scratchattach-1.1.5/
+-rw-rw-rw-   0        0        0    22055 2023-05-07 17:33:08.800522 scratchattach-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    20740 2023-05-07 17:32:19.000000 scratchattach-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 17:33:08.764230 scratchattach-1.1.5/scratchattach/
+-rw-rw-rw-   0        0        0      167 2023-05-04 16:19:46.000000 scratchattach-1.1.5/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    12798 2023-05-04 17:35:55.000000 scratchattach-1.1.5/scratchattach/_cloud.py
+-rw-rw-rw-   0        0        0    15496 2023-05-04 17:24:58.000000 scratchattach-1.1.5/scratchattach/_cloud_requests.py
+-rw-rw-rw-   0        0        0     1797 2023-05-04 16:19:46.000000 scratchattach-1.1.5/scratchattach/_encoder.py
+-rw-rw-rw-   0        0        0      888 2023-05-07 17:01:33.000000 scratchattach-1.1.5/scratchattach/_exceptions.py
+-rw-rw-rw-   0        0        0     6542 2023-05-04 16:19:46.000000 scratchattach-1.1.5/scratchattach/_forum.py
+-rw-rw-rw-   0        0        0    18157 2023-05-07 17:16:17.000000 scratchattach-1.1.5/scratchattach/_project.py
+-rw-rw-rw-   0        0        0    17923 2023-05-04 16:19:46.000000 scratchattach-1.1.5/scratchattach/_session.py
+-rw-rw-rw-   0        0        0     9646 2023-05-07 17:16:12.000000 scratchattach-1.1.5/scratchattach/_studio.py
+-rw-rw-rw-   0        0        0    25434 2023-05-07 17:30:43.000000 scratchattach-1.1.5/scratchattach/_user.py
+drwxrwxrwx   0        0        0        0 2023-05-07 17:33:08.797518 scratchattach-1.1.5/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0    22055 2023-05-07 17:33:08.000000 scratchattach-1.1.5/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-05-07 17:33:08.000000 scratchattach-1.1.5/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 17:33:08.000000 scratchattach-1.1.5/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-07 17:33:08.000000 scratchattach-1.1.5/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-07 17:33:08.000000 scratchattach-1.1.5/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 17:33:08.802517 scratchattach-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-05-07 17:32:47.000000 scratchattach-1.1.5/setup.py
```

### Comparing `scratchattach-1.1.4/PKG-INFO` & `scratchattach-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.1.4
+Version: 1.1.5
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -252,14 +252,17 @@
 user.follower_count()
 user.following_count()
 user.project_count()
 user.favorites_count() #Returns the amount of projects the user has favorited
 user.studio_count() #Returns the amount of studios the user is curating
 user.studio_following_count()
 
+user.follower_names(limit=40, offset=0) #Returns the followers as list of usernames (strings). New in v1.1.5
+user.following_names(limit=40, offset=0) #Returns the people the user is following as a list of usernames (strings). New in v1.1.5
+
 user.followers(limit=40, offset=0) #Returns the followers as list of scratch3.User objects
 user.following(limit=40, offset=0) #Returns the people the user is following as list of scratch3.User objects
 user.projects(limit=None, offset=0) #Returns the projects the user has shared as list of scratch3.Project objects
 user.favorites(limit=None, offset=0) #Returns the projects the user has favorited as list of scratch3.Project objects
 user.studios(limit=None, offset=0) #Returns the studios the user is curating as list of dicts
 
 user.viewed_projects(limit=24, offset=0) #To use this you need to be logged in as the user. Returns the projects the user has recently viewed as list of scratch3.Project objects
```

### Comparing `scratchattach-1.1.4/README.md` & `scratchattach-1.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -236,14 +236,17 @@
 user.follower_count()
 user.following_count()
 user.project_count()
 user.favorites_count() #Returns the amount of projects the user has favorited
 user.studio_count() #Returns the amount of studios the user is curating
 user.studio_following_count()
 
+user.follower_names(limit=40, offset=0) #Returns the followers as list of usernames (strings). New in v1.1.5
+user.following_names(limit=40, offset=0) #Returns the people the user is following as a list of usernames (strings). New in v1.1.5
+
 user.followers(limit=40, offset=0) #Returns the followers as list of scratch3.User objects
 user.following(limit=40, offset=0) #Returns the people the user is following as list of scratch3.User objects
 user.projects(limit=None, offset=0) #Returns the projects the user has shared as list of scratch3.Project objects
 user.favorites(limit=None, offset=0) #Returns the projects the user has favorited as list of scratch3.Project objects
 user.studios(limit=None, offset=0) #Returns the studios the user is curating as list of dicts
 
 user.viewed_projects(limit=24, offset=0) #To use this you need to be logged in as the user. Returns the projects the user has recently viewed as list of scratch3.Project objects
```

### Comparing `scratchattach-1.1.4/scratchattach/_cloud.py` & `scratchattach-1.1.5/scratchattach/_cloud.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.4/scratchattach/_cloud_requests.py` & `scratchattach-1.1.5/scratchattach/_cloud_requests.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.4/scratchattach/_encoder.py` & `scratchattach-1.1.5/scratchattach/_encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.4/scratchattach/_exceptions.py` & `scratchattach-1.1.5/scratchattach/_exceptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -41,7 +41,13 @@
     pass
 
 class Response429(Exception):
     pass
 
 class RequestNotFound(Exception):
     pass
+
+class CommentPostFailure(Exception):
+    """
+    Raised when a comment fails to post
+    """
+    pass
```

### Comparing `scratchattach-1.1.4/scratchattach/_forum.py` & `scratchattach-1.1.5/scratchattach/_forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.4/scratchattach/_project.py` & `scratchattach-1.1.5/scratchattach/_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
 
     def post_comment(self, content, *, parent_id="", commentee_id=""):
         if self._headers is None:
             raise(_exceptions.Unauthenticated)
             return
         data = {
             "commentee_id": commentee_id,
-            "content": content,
+            "content": str(content),
             "parent_id": parent_id,
         }
         headers = self._json_headers
         headers["referer"] = "https://scratch.mit.edu/projects/" + str(self.id) + "/"
         return json.loads(requests.post(
             f"https://api.scratch.mit.edu/proxy/comments/project/{self.id}/",
             headers = headers,
```

### Comparing `scratchattach-1.1.4/scratchattach/_session.py` & `scratchattach-1.1.5/scratchattach/_session.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.1.4/scratchattach/_studio.py` & `scratchattach-1.1.5/scratchattach/_studio.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,25 +98,25 @@
 
     def post_comment(self, content, *, parent_id="", commentee_id=""):
         if self._headers is None:
             raise(_exceptions.Unauthenticated)
             return
         data = {
             "commentee_id": commentee_id,
-            "content": content,
+            "content": str(content),
             "parent_id": parent_id,
         }
         headers = self._json_headers
         headers["referer"] = "https://scratch.mit.edu/projects/" + str(self.id) + "/"
-        return json.loads(requests.post(
+        return requests.post(
             f"https://api.scratch.mit.edu/proxy/comments/studio/{self.id}/",
             headers = headers,
             cookies = self._cookies,
             data=json.dumps(data),
-        ).text)
+        ).json()
 
 
     def reply_comment(self, content, *, parent_id, commentee_id=""):
         return self.post_comment(content, parent_id=parent_id, commentee_id=commentee_id)
 
     def projects(self, limit=40, offset=0):
         return requests.get(f"https://api.scratch.mit.edu/studios/{self.id}/projects/?limit={limit}&offset={offset}").json()
```

### Comparing `scratchattach-1.1.4/scratchattach/_user.py` & `scratchattach-1.1.5/scratchattach/_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,17 @@
                     bio = follower["profile"]["bio"],
                     country = follower["profile"]["country"]
                 ))
             except Exception:
                 print("Failed to parse ", follower)
         return followers
 
+    def follower_names(self, *, limit=40, offset=0):
+        return [i.name for i in self.followers(limit=limit, offset=offset)]
+
     def following(self, *, limit=40, offset=0):
         if limit>40:
             limit=40
         followers = []
         response = requests.get(
             f"https://api.scratch.mit.edu/users/{self.username}/following/?limit={limit}&offset={offset}").json()
         for follower in response:
@@ -165,14 +168,17 @@
                     bio = follower["profile"]["bio"],
                     country = follower["profile"]["country"]
                 ))
             except Exception:
                 print("Failed to parse ", follower)
         return followers
 
+    def following_names(self, *, limit=40, offset=0):
+        return [i.name for i in self.following(limit=limit, offset=offset)]
+
     '''def get_comments(self, *, page=1):
         response = requests.get(f"https://scratch.mit.edu/site-api/comments/user/{self.z}/?page=1")'''
 
     def is_following(self, user):
         return requests.get(f"https://following-check.1tim.repl.co/api/{self.username}/?following={user}").json()["following"]
 
     def is_followed_by(self, user):
@@ -426,24 +432,27 @@
             cookies = self._cookies,
             data = json.dumps({"featured_project":int(project_id),"featured_project_label":label})
         )
 
 
     def post_comment(self, content, *, parent_id="", commentee_id=""):
         data = {
-            "commentee_id": commentee_id,
-            "content": content,
-            "parent_id": parent_id,
+        "commentee_id": commentee_id,
+        "content": str(content),
+        "parent_id": parent_id,
         }
-        return requests.post(
+        r = requests.post(
             f"https://scratch.mit.edu/site-api/comments/user/{self.username}/add/",
             headers = headers,
             cookies = self._cookies,
             data=json.dumps(data),
         )
+        if r.status_code != 200:
+            raise _exceptions.CommentPostFailure(r.text)
+        return r.text
 
     def reply_comment(self, content, *, parent_id, commentee_id=""):
         return self.post_comment(content, parent_id=parent_id, commentee_id=commentee_id)
 
     def activity_html(self, *, limit=1000):
         return requests.get(f"https://scratch.mit.edu/messages/ajax/user-activity/?user={self.username}&max={limit}").text
```

### Comparing `scratchattach-1.1.4/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.1.5/scratchattach.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.1.4
+Version: 1.1.5
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -252,14 +252,17 @@
 user.follower_count()
 user.following_count()
 user.project_count()
 user.favorites_count() #Returns the amount of projects the user has favorited
 user.studio_count() #Returns the amount of studios the user is curating
 user.studio_following_count()
 
+user.follower_names(limit=40, offset=0) #Returns the followers as list of usernames (strings). New in v1.1.5
+user.following_names(limit=40, offset=0) #Returns the people the user is following as a list of usernames (strings). New in v1.1.5
+
 user.followers(limit=40, offset=0) #Returns the followers as list of scratch3.User objects
 user.following(limit=40, offset=0) #Returns the people the user is following as list of scratch3.User objects
 user.projects(limit=None, offset=0) #Returns the projects the user has shared as list of scratch3.Project objects
 user.favorites(limit=None, offset=0) #Returns the projects the user has favorited as list of scratch3.Project objects
 user.studios(limit=None, offset=0) #Returns the studios the user is curating as list of dicts
 
 user.viewed_projects(limit=24, offset=0) #To use this you need to be logged in as the user. Returns the projects the user has recently viewed as list of scratch3.Project objects
```

### Comparing `scratchattach-1.1.4/setup.py` & `scratchattach-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.1.4'
+VERSION = '1.1.5'
 DESCRIPTION = 'An Scratch API Wrapper for scratch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```

