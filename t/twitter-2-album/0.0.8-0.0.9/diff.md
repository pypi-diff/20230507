# Comparing `tmp/twitter_2_album-0.0.8.tar.gz` & `tmp/twitter_2_album-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/twitter_2_album-0.0.8.tar", last modified: Sat May 16 19:06:48 2020, max compression
+gzip compressed data, was "dist/twitter_2_album-0.0.9.tar", last modified: Mon May 18 05:05:43 2020, max compression
```

## Comparing `twitter_2_album-0.0.8.tar` & `twitter_2_album-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-05-16 19:06:48.000000 twitter_2_album-0.0.8/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      847 2020-05-16 19:06:48.000000 twitter_2_album-0.0.8/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      230 2020-03-23 00:07:28.000000 twitter_2_album-0.0.8/README.md
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2020-05-16 19:06:48.000000 twitter_2_album-0.0.8/setup.cfg
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      776 2020-05-16 19:06:46.000000 twitter_2_album-0.0.8/setup.py
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-05-16 19:06:48.000000 twitter_2_album-0.0.8/twitter_2_album/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1514 2020-05-16 18:46:13.000000 twitter_2_album-0.0.8/twitter_2_album/__init__.py
-drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-05-16 19:06:48.000000 twitter_2_album-0.0.8/twitter_2_album.egg-info/
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      847 2020-05-16 19:06:48.000000 twitter_2_album-0.0.8/twitter_2_album.egg-info/PKG-INFO
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      240 2020-05-16 19:06:48.000000 twitter_2_album-0.0.8/twitter_2_album.egg-info/SOURCES.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2020-05-16 19:06:48.000000 twitter_2_album-0.0.8/twitter_2_album.egg-info/dependency_links.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       28 2020-05-16 19:06:48.000000 twitter_2_album-0.0.8/twitter_2_album.egg-info/requires.txt
--rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       16 2020-05-16 19:06:48.000000 twitter_2_album-0.0.8/twitter_2_album.egg-info/top_level.txt
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-05-18 05:05:43.000000 twitter_2_album-0.0.9/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      847 2020-05-18 05:05:43.000000 twitter_2_album-0.0.9/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      230 2020-03-23 00:07:28.000000 twitter_2_album-0.0.9/README.md
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       38 2020-05-18 05:05:43.000000 twitter_2_album-0.0.9/setup.cfg
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      776 2020-05-18 05:05:23.000000 twitter_2_album-0.0.9/setup.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-05-18 05:05:43.000000 twitter_2_album-0.0.9/twitter_2_album/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)     1951 2020-05-18 05:00:08.000000 twitter_2_album-0.0.9/twitter_2_album/__init__.py
+drwxr-xr-x   0 yunzhi   (672583) primarygroup (89939)        0 2020-05-18 05:05:43.000000 twitter_2_album-0.0.9/twitter_2_album.egg-info/
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      847 2020-05-18 05:05:43.000000 twitter_2_album-0.0.9/twitter_2_album.egg-info/PKG-INFO
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)      240 2020-05-18 05:05:43.000000 twitter_2_album-0.0.9/twitter_2_album.egg-info/SOURCES.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)        1 2020-05-18 05:05:43.000000 twitter_2_album-0.0.9/twitter_2_album.egg-info/dependency_links.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       28 2020-05-18 05:05:43.000000 twitter_2_album-0.0.9/twitter_2_album.egg-info/requires.txt
+-rw-r--r--   0 yunzhi   (672583) primarygroup (89939)       16 2020-05-18 05:05:43.000000 twitter_2_album-0.0.9/twitter_2_album.egg-info/top_level.txt
```

### Comparing `twitter_2_album-0.0.8/PKG-INFO` & `twitter_2_album-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter_2_album
-Version: 0.0.8
+Version: 0.0.9
 Summary: Return photo list and caption (markdown format) from twitter.
 Home-page: https://github.com/gaoyunzhi/twitter_2_album
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # twitter_2_album
```

### Comparing `twitter_2_album-0.0.8/setup.py` & `twitter_2_album-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="twitter_2_album",
-    version="0.0.8",
+    version="0.0.9",
     author="Yunzhi Gao",
     author_email="gaoyunzhi@gmail.com",
     description="Return photo list and caption (markdown format) from twitter.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaoyunzhi/twitter_2_album",
     packages=setuptools.find_packages(),
```

### Comparing `twitter_2_album-0.0.8/twitter_2_album/__init__.py` & `twitter_2_album-0.0.9/twitter_2_album/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,22 +40,33 @@
 def getImgs(status):
 	if not status:
 		return []
 	# seems video is not returned in side the json, there is nothing we can do...
 	return [x['media_url'] for x in getEntities(status).get('media', [])
 		if x['type'] == 'photo']
 
+def getVideo(status):
+	if not status:
+		return ''
+	videos = [x for x in getEntities(status).get('media', []) if x['type'] == 'video']
+	if not videos:
+		return ''
+	variants = [x for x in videos[0]['video_info']['variants'] if x['content_type'] == 'video/mp4']
+	variants = [(x.get('bitrate'), x) for x in variants]
+	variants.sort()
+	return variants[-1][1]['url']
 
-def getQuoteImgs(status):
+def getQuote(status, func):
 	try:
 		status.quoted_status
 	except:
-		return []
-	return getImgs(status.quoted_status)
+		return None
+	return func(status.quoted_status)
 
 def get(path):
 	tid = getTid(path)
 	status = twitterApi.get_status(tid, tweet_mode="extended")
 	r = Result()
-	r.imgs = getImgs(status) or getQuoteImgs(status)
+	r.video = getVideo(status) or getQuote(status, getVideo) or ''
+	r.imgs = getImgs(status) or getQuote(status, getImgs) or []
 	r.cap = getCap(status)
 	return r
```

### Comparing `twitter_2_album-0.0.8/twitter_2_album.egg-info/PKG-INFO` & `twitter_2_album-0.0.9/twitter_2_album.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-2-album
-Version: 0.0.8
+Version: 0.0.9
 Summary: Return photo list and caption (markdown format) from twitter.
 Home-page: https://github.com/gaoyunzhi/twitter_2_album
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Description: # twitter_2_album
```

