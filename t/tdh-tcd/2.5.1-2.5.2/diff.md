# Comparing `tmp/tdh-tcd-2.5.1.tar.gz` & `tmp/tdh-tcd-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdh-tcd-2.5.1.tar", last modified: Fri May  5 21:28:06 2023, max compression
+gzip compressed data, was "tdh-tcd-2.5.2.tar", last modified: Sat May  6 23:39:46 2023, max compression
```

## Comparing `tdh-tcd-2.5.1.tar` & `tdh-tcd-2.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:28:06.516397 tdh-tcd-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-05 21:27:55.000000 tdh-tcd-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-05 21:28:06.516397 tdh-tcd-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-05 21:27:55.000000 tdh-tcd-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:28:06.516397 tdh-tcd-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-05 21:27:55.000000 tdh-tcd-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:28:06.512397 tdh-tcd-2.5.1/tcd/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-05 21:27:55.000000 tdh-tcd-2.5.1/tcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-05 21:27:55.000000 tdh-tcd-2.5.1/tcd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-05 21:27:55.000000 tdh-tcd-2.5.1/tcd/example.settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-05-05 21:27:55.000000 tdh-tcd-2.5.1/tcd/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-05 21:27:55.000000 tdh-tcd-2.5.1/tcd/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-05-05 21:27:55.000000 tdh-tcd-2.5.1/tcd/twitch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:28:06.512397 tdh-tcd-2.5.1/tdh_tcd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-05 21:28:06.000000 tdh-tcd-2.5.1/tdh_tcd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-05 21:28:06.000000 tdh-tcd-2.5.1/tdh_tcd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:28:06.000000 tdh-tcd-2.5.1/tdh_tcd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 21:28:06.000000 tdh-tcd-2.5.1/tdh_tcd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 21:28:06.000000 tdh-tcd-2.5.1/tdh_tcd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-05 21:28:06.000000 tdh-tcd-2.5.1/tdh_tcd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:39:46.579510 tdh-tcd-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-06 23:39:34.000000 tdh-tcd-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-06 23:39:46.579510 tdh-tcd-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-06 23:39:34.000000 tdh-tcd-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 23:39:46.579510 tdh-tcd-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-06 23:39:34.000000 tdh-tcd-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:39:46.579510 tdh-tcd-2.5.2/tcd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-06 23:39:34.000000 tdh-tcd-2.5.2/tcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-06 23:39:34.000000 tdh-tcd-2.5.2/tcd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-06 23:39:34.000000 tdh-tcd-2.5.2/tcd/example.settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-05-06 23:39:34.000000 tdh-tcd-2.5.2/tcd/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-06 23:39:34.000000 tdh-tcd-2.5.2/tcd/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-05-06 23:39:34.000000 tdh-tcd-2.5.2/tcd/twitch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:39:46.579510 tdh-tcd-2.5.2/tdh_tcd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-06 23:39:46.000000 tdh-tcd-2.5.2/tdh_tcd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-06 23:39:46.000000 tdh-tcd-2.5.2/tdh_tcd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 23:39:46.000000 tdh-tcd-2.5.2/tdh_tcd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-06 23:39:46.000000 tdh-tcd-2.5.2/tdh_tcd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-06 23:39:46.000000 tdh-tcd-2.5.2/tdh_tcd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-06 23:39:46.000000 tdh-tcd-2.5.2/tdh_tcd.egg-info/top_level.txt
```

### Comparing `tdh-tcd-2.5.1/LICENSE` & `tdh-tcd-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.1/PKG-INFO` & `tdh-tcd-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdh-tcd
-Version: 2.5.1
+Version: 2.5.2
 Summary: Twitch Chat Downloader
 Home-page: https://github.com/TheDrHax/Twitch-Chat-Downloader
 Author: Dmitry Karikh
 Author-email: the.dr.hax@gmail.com
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `tdh-tcd-2.5.1/README.md` & `tdh-tcd-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.1/setup.py` & `tdh-tcd-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open('README.md', 'r') as fi:
     long_description = fi.read()
 
 
 setup(
     name='tdh-tcd',
-    version='2.5.1',
+    version='2.5.2',
 
     author='Dmitry Karikh',
     author_email='the.dr.hax@gmail.com',
 
     description='Twitch Chat Downloader',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `tdh-tcd-2.5.1/tcd/__init__.py` & `tdh-tcd-2.5.2/tcd/__init__.py`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.1/tcd/example.settings.json` & `tdh-tcd-2.5.2/tcd/example.settings.json`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.1/tcd/settings.py` & `tdh-tcd-2.5.2/tcd/settings.py`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.1/tcd/subtitles.py` & `tdh-tcd-2.5.2/tcd/subtitles.py`

 * *Files identical despite different names*

### Comparing `tdh-tcd-2.5.1/tcd/twitch.py` & `tdh-tcd-2.5.2/tcd/twitch.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,22 +142,22 @@
         self.creator_id = video['data']['video']['creator']['id']
 
         if settings.get('display_progress') in [None, True]:
             self.progressbar = ProgressBar(max_value=self.duration)
     
     def __iter__(self):
         hasNextPage = True
-        cursor = None
+        cursor = 0
         hashes = set()
 
         while hasNextPage:
             res = gql(f'''
                 query {{
                     video(id: "{self.video_id}") {{
-                        comments{f'(contentOffsetSeconds: {cursor})' if cursor else ''} {{
+                        comments{f'(contentOffsetSeconds: {cursor})' if cursor > 0 else ''} {{
                             edges {{
                                 cursor
                                 node {{
                                     commenter {{
                                         displayName
                                         login
                                         displayBadges(channelID: {self.creator_id}) {{
@@ -182,17 +182,23 @@
                     }}
                 }}
             ''')
 
             comments = res['data']['video']['comments']
             hasNextPage = comments['pageInfo']['hasNextPage']
 
-            for comment in comments['edges']:
-                cursor = comment['node']['contentOffsetSeconds']
+            # Avoid infinite loops
+            new_cursor = comments['edges'][-1]['node']['contentOffsetSeconds']
+            if new_cursor <= cursor:
+                cursor += 1
+                continue
+            else:
+                cursor = new_cursor
 
+            for comment in comments['edges']:
                 # Calculate more accurate offset
                 ts = parse8601(comment['node']['createdAt'])
                 offset = (ts - self.created_at).total_seconds()
                 comment['node']['contentOffsetSeconds'] = offset
 
                 try:
                     msg = Message(comment['node'])
```

### Comparing `tdh-tcd-2.5.1/tdh_tcd.egg-info/PKG-INFO` & `tdh-tcd-2.5.2/tdh_tcd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdh-tcd
-Version: 2.5.1
+Version: 2.5.2
 Summary: Twitch Chat Downloader
 Home-page: https://github.com/TheDrHax/Twitch-Chat-Downloader
 Author: Dmitry Karikh
 Author-email: the.dr.hax@gmail.com
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Intended Audience :: End Users/Desktop
```

