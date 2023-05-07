# Comparing `tmp/twitch-dl-2.1.2.tar.gz` & `tmp/twitch-dl-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch-dl-2.1.2.tar", last modified: Tue Apr 18 05:12:34 2023, max compression
+gzip compressed data, was "twitch-dl-2.1.3.tar", last modified: Sun May  7 09:51:15 2023, max compression
```

## Comparing `twitch-dl-2.1.2.tar` & `twitch-dl-2.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-04-18 05:12:34.095268 twitch-dl-2.1.2/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      721 2023-04-18 05:12:34.095268 twitch-dl-2.1.2/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1627 2022-08-18 08:06:46.000000 twitch-dl-2.1.2/README.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2023-04-18 05:12:34.095268 twitch-dl-2.1.2/setup.cfg
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1128 2023-04-18 05:08:35.000000 twitch-dl-2.1.2/setup.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-04-18 05:12:34.095268 twitch-dl-2.1.2/twitch_dl.egg-info/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      721 2023-04-18 05:12:33.000000 twitch-dl-2.1.2/twitch_dl.egg-info/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      584 2023-04-18 05:12:34.000000 twitch-dl-2.1.2/twitch_dl.egg-info/SOURCES.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2023-04-18 05:12:33.000000 twitch-dl-2.1.2/twitch_dl.egg-info/dependency_links.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       53 2023-04-18 05:12:33.000000 twitch-dl-2.1.2/twitch_dl.egg-info/entry_points.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       40 2023-04-18 05:12:33.000000 twitch-dl-2.1.2/twitch_dl.egg-info/requires.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2023-04-18 05:12:33.000000 twitch-dl-2.1.2/twitch_dl.egg-info/top_level.txt
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-04-18 05:12:34.095268 twitch-dl-2.1.2/twitchdl/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       68 2023-04-18 05:08:41.000000 twitch-dl-2.1.2/twitchdl/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       42 2020-11-04 07:52:52.000000 twitch-dl-2.1.2/twitchdl/__main__.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-04-18 05:12:34.095268 twitch-dl-2.1.2/twitchdl/commands/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      198 2022-11-20 08:22:41.000000 twitch-dl-2.1.2/twitchdl/commands/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2702 2022-11-20 14:35:33.000000 twitch-dl-2.1.2/twitchdl/commands/clips.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    12820 2022-11-20 14:32:36.000000 twitch-dl-2.1.2/twitchdl/commands/download.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      182 2022-08-09 07:04:30.000000 twitch-dl-2.1.2/twitchdl/commands/env.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2592 2022-11-20 14:35:33.000000 twitch-dl-2.1.2/twitchdl/commands/info.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1892 2022-11-20 14:35:33.000000 twitch-dl-2.1.2/twitchdl/commands/videos.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10603 2022-11-20 14:32:36.000000 twitch-dl-2.1.2/twitchdl/console.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      882 2022-08-20 11:25:04.000000 twitch-dl-2.1.2/twitchdl/download.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      113 2020-04-09 20:48:04.000000 twitch-dl-2.1.2/twitchdl/exceptions.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3892 2022-11-20 14:35:42.000000 twitch-dl-2.1.2/twitchdl/http.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4374 2022-09-10 06:24:28.000000 twitch-dl-2.1.2/twitchdl/output.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4435 2022-08-18 08:06:46.000000 twitch-dl-2.1.2/twitchdl/progress.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9434 2023-04-18 05:05:03.000000 twitch-dl-2.1.2/twitchdl/twitch.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2938 2022-11-20 14:32:36.000000 twitch-dl-2.1.2/twitchdl/utils.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-05-07 09:51:15.511402 twitch-dl-2.1.3/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      721 2023-05-07 09:51:15.511402 twitch-dl-2.1.3/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1627 2022-08-18 08:06:46.000000 twitch-dl-2.1.3/README.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2023-05-07 09:51:15.511402 twitch-dl-2.1.3/setup.cfg
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1128 2023-05-07 09:50:13.000000 twitch-dl-2.1.3/setup.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-05-07 09:51:15.511402 twitch-dl-2.1.3/twitch_dl.egg-info/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      721 2023-05-07 09:51:15.000000 twitch-dl-2.1.3/twitch_dl.egg-info/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      584 2023-05-07 09:51:15.000000 twitch-dl-2.1.3/twitch_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2023-05-07 09:51:15.000000 twitch-dl-2.1.3/twitch_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       53 2023-05-07 09:51:15.000000 twitch-dl-2.1.3/twitch_dl.egg-info/entry_points.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       40 2023-05-07 09:51:15.000000 twitch-dl-2.1.3/twitch_dl.egg-info/requires.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2023-05-07 09:51:15.000000 twitch-dl-2.1.3/twitch_dl.egg-info/top_level.txt
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-05-07 09:51:15.511402 twitch-dl-2.1.3/twitchdl/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       69 2023-05-07 09:50:07.000000 twitch-dl-2.1.3/twitchdl/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       42 2020-11-04 07:52:52.000000 twitch-dl-2.1.3/twitchdl/__main__.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2023-05-07 09:51:15.511402 twitch-dl-2.1.3/twitchdl/commands/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      198 2022-11-20 08:22:41.000000 twitch-dl-2.1.3/twitchdl/commands/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2702 2022-11-20 14:35:33.000000 twitch-dl-2.1.3/twitchdl/commands/clips.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    12820 2022-11-20 14:32:36.000000 twitch-dl-2.1.3/twitchdl/commands/download.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      182 2022-08-09 07:04:30.000000 twitch-dl-2.1.3/twitchdl/commands/env.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2592 2022-11-20 14:35:33.000000 twitch-dl-2.1.3/twitchdl/commands/info.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1892 2022-11-20 14:35:33.000000 twitch-dl-2.1.3/twitchdl/commands/videos.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10603 2022-11-20 14:32:36.000000 twitch-dl-2.1.3/twitchdl/console.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      882 2022-08-20 11:25:04.000000 twitch-dl-2.1.3/twitchdl/download.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      113 2020-04-09 20:48:04.000000 twitch-dl-2.1.3/twitchdl/exceptions.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3892 2022-11-20 14:35:42.000000 twitch-dl-2.1.3/twitchdl/http.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4374 2022-09-10 06:24:28.000000 twitch-dl-2.1.3/twitchdl/output.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4435 2022-08-18 08:06:46.000000 twitch-dl-2.1.3/twitchdl/progress.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9434 2023-04-18 05:05:03.000000 twitch-dl-2.1.3/twitchdl/twitch.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2938 2022-11-20 14:32:36.000000 twitch-dl-2.1.3/twitchdl/utils.py
```

### Comparing `twitch-dl-2.1.2/PKG-INFO` & `twitch-dl-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: twitch-dl
-Version: 2.1.2
+Version: 2.1.3
 Summary: Twitch downloader
 Home-page: https://github.com/ihabunek/twitch-dl/
 Author: Ivan Habunek
 Author-email: ivan@habunek.com
 License: GPLv3
 Project-URL: Documentation, https://twitch-dl.bezdomni.net/
 Description: Quickly download videos from twitch.tv.
```

### Comparing `twitch-dl-2.1.2/README.md` & `twitch-dl-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.2/setup.py` & `twitch-dl-2.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Works simliarly to youtube-dl but downloads multiple VODs in parallel which
 makes it faster.
 """
 
 setup(
     name="twitch-dl",
-    version="2.1.2",
+    version="2.1.3",
     description="Twitch downloader",
     long_description=long_description.strip(),
     author="Ivan Habunek",
     author_email="ivan@habunek.com",
     url="https://github.com/ihabunek/twitch-dl/",
     project_urls={
         "Documentation": "https://twitch-dl.bezdomni.net/"
```

### Comparing `twitch-dl-2.1.2/twitch_dl.egg-info/PKG-INFO` & `twitch-dl-2.1.3/twitch_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: twitch-dl
-Version: 2.1.2
+Version: 2.1.3
 Summary: Twitch downloader
 Home-page: https://github.com/ihabunek/twitch-dl/
 Author: Ivan Habunek
 Author-email: ivan@habunek.com
 License: GPLv3
 Project-URL: Documentation, https://twitch-dl.bezdomni.net/
 Description: Quickly download videos from twitch.tv.
```

### Comparing `twitch-dl-2.1.2/twitch_dl.egg-info/SOURCES.txt` & `twitch-dl-2.1.3/twitch_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.2/twitchdl/commands/clips.py` & `twitch-dl-2.1.3/twitchdl/commands/clips.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.2/twitchdl/commands/download.py` & `twitch-dl-2.1.3/twitchdl/commands/download.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.2/twitchdl/commands/info.py` & `twitch-dl-2.1.3/twitchdl/commands/info.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.2/twitchdl/commands/videos.py` & `twitch-dl-2.1.3/twitchdl/commands/videos.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.2/twitchdl/console.py` & `twitch-dl-2.1.3/twitchdl/console.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.2/twitchdl/download.py` & `twitch-dl-2.1.3/twitchdl/download.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.2/twitchdl/http.py` & `twitch-dl-2.1.3/twitchdl/http.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.2/twitchdl/output.py` & `twitch-dl-2.1.3/twitchdl/output.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.2/twitchdl/progress.py` & `twitch-dl-2.1.3/twitchdl/progress.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.2/twitchdl/twitch.py` & `twitch-dl-2.1.3/twitchdl/twitch.py`

 * *Files identical despite different names*

### Comparing `twitch-dl-2.1.2/twitchdl/utils.py` & `twitch-dl-2.1.3/twitchdl/utils.py`

 * *Files identical despite different names*

