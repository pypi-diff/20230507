# Comparing `tmp/ersciyt-1.7.tar.gz` & `tmp/ersciyt-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ersciyt-1.7.tar", last modified: Sat May  6 06:46:30 2023, max compression
+gzip compressed data, was "ersciyt-1.8.tar", last modified: Sun May  7 12:37:19 2023, max compression
```

## Comparing `ersciyt-1.7.tar` & `ersciyt-1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 06:46:30.692298 ersciyt-1.7/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-05-06 06:46:21.000000 ersciyt-1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-06 06:46:21.000000 ersciyt-1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      795 2023-05-06 06:46:30.692298 ersciyt-1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      517 2023-05-06 06:46:21.000000 ersciyt-1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 06:46:30.691298 ersciyt-1.7/ersciyt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-06 06:46:21.000000 ersciyt-1.7/ersciyt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-06 06:46:21.000000 ersciyt-1.7/ersciyt/admin.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-05-06 06:46:21.000000 ersciyt-1.7/ersciyt/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 06:46:30.692298 ersciyt-1.7/ersciyt/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-06 06:46:21.000000 ersciyt-1.7/ersciyt/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-06 06:46:21.000000 ersciyt-1.7/ersciyt/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 06:46:30.692298 ersciyt-1.7/ersciyt/static/
--rw-r--r--   0 root         (0) root         (0)    11852 2023-05-06 06:46:21.000000 ersciyt-1.7/ersciyt/static/ersci_viddown_tab2.xpi
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-06 06:46:21.000000 ersciyt-1.7/ersciyt/tests.py
--rw-r--r--   0 root         (0) root         (0)      412 2023-05-06 06:46:21.000000 ersciyt-1.7/ersciyt/urls.py
--rw-r--r--   0 root         (0) root         (0)     6611 2023-05-06 06:46:21.000000 ersciyt-1.7/ersciyt/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 06:46:30.692298 ersciyt-1.7/ersciyt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      795 2023-05-06 06:46:30.000000 ersciyt-1.7/ersciyt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      392 2023-05-06 06:46:30.000000 ersciyt-1.7/ersciyt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 06:46:30.000000 ersciyt-1.7/ersciyt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-06 06:46:30.000000 ersciyt-1.7/ersciyt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-06 06:46:30.000000 ersciyt-1.7/ersciyt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-06 06:46:30.693298 ersciyt-1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-06 06:46:21.000000 ersciyt-1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:37:19.645782 ersciyt-1.8/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-05-07 12:37:13.000000 ersciyt-1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-07 12:37:13.000000 ersciyt-1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      795 2023-05-07 12:37:19.645782 ersciyt-1.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      517 2023-05-07 12:37:13.000000 ersciyt-1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:37:19.644782 ersciyt-1.8/ersciyt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 12:37:13.000000 ersciyt-1.8/ersciyt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-07 12:37:13.000000 ersciyt-1.8/ersciyt/admin.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-07 12:37:13.000000 ersciyt-1.8/ersciyt/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:37:19.645782 ersciyt-1.8/ersciyt/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 12:37:13.000000 ersciyt-1.8/ersciyt/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-07 12:37:13.000000 ersciyt-1.8/ersciyt/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:37:19.645782 ersciyt-1.8/ersciyt/static/
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-05-07 12:37:13.000000 ersciyt-1.8/ersciyt/static/ersci_viddown_tab2.xpi
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-07 12:37:13.000000 ersciyt-1.8/ersciyt/tests.py
+-rw-r--r--   0 root         (0) root         (0)      412 2023-05-07 12:37:13.000000 ersciyt-1.8/ersciyt/urls.py
+-rw-r--r--   0 root         (0) root         (0)     6902 2023-05-07 12:37:13.000000 ersciyt-1.8/ersciyt/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:37:19.645782 ersciyt-1.8/ersciyt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      795 2023-05-07 12:37:19.000000 ersciyt-1.8/ersciyt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-07 12:37:19.000000 ersciyt-1.8/ersciyt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 12:37:19.000000 ersciyt-1.8/ersciyt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-07 12:37:19.000000 ersciyt-1.8/ersciyt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-07 12:37:19.000000 ersciyt-1.8/ersciyt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      664 2023-05-07 12:37:19.646782 ersciyt-1.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-07 12:37:13.000000 ersciyt-1.8/setup.py
```

### Comparing `ersciyt-1.7/LICENSE` & `ersciyt-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ersciyt-1.7/PKG-INFO` & `ersciyt-1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.7
+Version: 1.8
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ersciyt-1.7/README.md` & `ersciyt-1.8/README.md`

 * *Files identical despite different names*

### Comparing `ersciyt-1.7/ersciyt/static/ersci_viddown_tab2.xpi` & `ersciyt-1.8/ersciyt/static/ersci_viddown_tab2.xpi`

 * *Files identical despite different names*

### Comparing `ersciyt-1.7/ersciyt/views.py` & `ersciyt-1.8/ersciyt/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from django.shortcuts import render
 from django.conf import settings
 #from pytube import YouTube
+import pyqrcode
 import os,subprocess
 from django.http import HttpResponse,FileResponse
 #from youtube_transcript_api import YouTubeTranscriptApi
 #from youtube_transcript_api.formatters import WebVTTFormatter
 #pip install googletrans==4.0.0-rc1
 #from googletrans import Translator
 import re
+from django.contrib.staticfiles import finders
 
 
 def ytdwn(request,link):
     try:        
         #os.system('sudo apt-get install -y ffmpeg') 
         os.system('yt-dlp  -f 18 -o a.mp4 https://www.youtube.com/watch?v={}'.format(link))        
         tmp4=open('a.mp4' , 'rb')
@@ -144,21 +146,25 @@
         return response
     except:
         return HttpResponse (video.description)
 '''
 
 def helping(request):
     try:
+        qr_code = pyqrcode.create(request.headers['Host']))
+        qr_code.svg('a.svg', scale=6)
         return HttpResponse ('''
         <p>Use address of youtube after watch like - for download video -  :<br>
         <b> YourSiteName/ytlink?url=<any video site link></b><br>
         or<br>
-        link name like - for play in firefox -  : <br>
+        enter Youtube ID after YourSiteName address - for play in firefox -  : <br>
         <b>YourSiteName/xazlZh1lTpM</b><br>        
         <a href="/static/ersci_viddown_tab2.xpi">Video download firefox Addon direct link</a><br>
         or<br>
         <a href="https://addons.mozilla.org/en-US/firefox/addon/ersci_viddown_tab2">video download firefox Addon mozilla site link</a>
-        
+        <br>
+        <b>{}</b>
+        <img src='{}' />
         </p>
-        ''')
+        '''.format(request.headers['Host'],finders.find('a.svg')))
     except:
         return HttpResponse ('Youtube Url Is Mistake!!!')
```

### Comparing `ersciyt-1.7/ersciyt.egg-info/PKG-INFO` & `ersciyt-1.8/ersciyt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.7
+Version: 1.8
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ersciyt-1.7/setup.cfg` & `ersciyt-1.8/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ersciyt
-version = 1.7
+version = 1.8
 description = Youtube Downloader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/yt.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
@@ -19,12 +19,13 @@
 [options]
 include_package_data = true
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	django
 	yt-dlp
+	pyqrcode
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

