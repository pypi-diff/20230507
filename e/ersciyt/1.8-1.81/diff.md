# Comparing `tmp/ersciyt-1.8.tar.gz` & `tmp/ersciyt-1.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ersciyt-1.8.tar", last modified: Sun May  7 12:37:19 2023, max compression
+gzip compressed data, was "ersciyt-1.81.tar", last modified: Sun May  7 12:42:35 2023, max compression
```

## Comparing `ersciyt-1.8.tar` & `ersciyt-1.81.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:37:19.645782 ersciyt-1.8/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-05-07 12:37:13.000000 ersciyt-1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-07 12:37:13.000000 ersciyt-1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      795 2023-05-07 12:37:19.645782 ersciyt-1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      517 2023-05-07 12:37:13.000000 ersciyt-1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:37:19.644782 ersciyt-1.8/ersciyt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 12:37:13.000000 ersciyt-1.8/ersciyt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-07 12:37:13.000000 ersciyt-1.8/ersciyt/admin.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-05-07 12:37:13.000000 ersciyt-1.8/ersciyt/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:37:19.645782 ersciyt-1.8/ersciyt/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 12:37:13.000000 ersciyt-1.8/ersciyt/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-07 12:37:13.000000 ersciyt-1.8/ersciyt/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:37:19.645782 ersciyt-1.8/ersciyt/static/
--rw-r--r--   0 root         (0) root         (0)    11852 2023-05-07 12:37:13.000000 ersciyt-1.8/ersciyt/static/ersci_viddown_tab2.xpi
--rw-r--r--   0 root         (0) root         (0)       60 2023-05-07 12:37:13.000000 ersciyt-1.8/ersciyt/tests.py
--rw-r--r--   0 root         (0) root         (0)      412 2023-05-07 12:37:13.000000 ersciyt-1.8/ersciyt/urls.py
--rw-r--r--   0 root         (0) root         (0)     6902 2023-05-07 12:37:13.000000 ersciyt-1.8/ersciyt/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:37:19.645782 ersciyt-1.8/ersciyt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      795 2023-05-07 12:37:19.000000 ersciyt-1.8/ersciyt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      392 2023-05-07 12:37:19.000000 ersciyt-1.8/ersciyt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 12:37:19.000000 ersciyt-1.8/ersciyt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-07 12:37:19.000000 ersciyt-1.8/ersciyt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-07 12:37:19.000000 ersciyt-1.8/ersciyt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      664 2023-05-07 12:37:19.646782 ersciyt-1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-07 12:37:13.000000 ersciyt-1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:42:35.230172 ersciyt-1.81/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-05-07 12:42:12.000000 ersciyt-1.81/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-07 12:42:12.000000 ersciyt-1.81/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      796 2023-05-07 12:42:35.230172 ersciyt-1.81/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      517 2023-05-07 12:42:12.000000 ersciyt-1.81/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:42:35.228172 ersciyt-1.81/ersciyt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 12:42:12.000000 ersciyt-1.81/ersciyt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-07 12:42:12.000000 ersciyt-1.81/ersciyt/admin.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-07 12:42:12.000000 ersciyt-1.81/ersciyt/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:42:35.229172 ersciyt-1.81/ersciyt/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 12:42:12.000000 ersciyt-1.81/ersciyt/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-07 12:42:12.000000 ersciyt-1.81/ersciyt/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:42:35.230172 ersciyt-1.81/ersciyt/static/
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-05-07 12:42:12.000000 ersciyt-1.81/ersciyt/static/ersci_viddown_tab2.xpi
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-07 12:42:12.000000 ersciyt-1.81/ersciyt/tests.py
+-rw-r--r--   0 root         (0) root         (0)      412 2023-05-07 12:42:12.000000 ersciyt-1.81/ersciyt/urls.py
+-rw-r--r--   0 root         (0) root         (0)     6901 2023-05-07 12:42:12.000000 ersciyt-1.81/ersciyt/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 12:42:35.229172 ersciyt-1.81/ersciyt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      796 2023-05-07 12:42:35.000000 ersciyt-1.81/ersciyt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-07 12:42:35.000000 ersciyt-1.81/ersciyt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 12:42:35.000000 ersciyt-1.81/ersciyt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-07 12:42:35.000000 ersciyt-1.81/ersciyt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-07 12:42:35.000000 ersciyt-1.81/ersciyt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      665 2023-05-07 12:42:35.231173 ersciyt-1.81/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-07 12:42:12.000000 ersciyt-1.81/setup.py
```

### Comparing `ersciyt-1.8/LICENSE` & `ersciyt-1.81/LICENSE`

 * *Files identical despite different names*

### Comparing `ersciyt-1.8/PKG-INFO` & `ersciyt-1.81/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.8
+Version: 1.81
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ersciyt-1.8/README.md` & `ersciyt-1.81/README.md`

 * *Files identical despite different names*

### Comparing `ersciyt-1.8/ersciyt/static/ersci_viddown_tab2.xpi` & `ersciyt-1.81/ersciyt/static/ersci_viddown_tab2.xpi`

 * *Files identical despite different names*

### Comparing `ersciyt-1.8/ersciyt/views.py` & `ersciyt-1.81/ersciyt/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         return response
     except:
         return HttpResponse (video.description)
 '''
 
 def helping(request):
     try:
-        qr_code = pyqrcode.create(request.headers['Host']))
+        qr_code = pyqrcode.create(request.headers['Host'])
         qr_code.svg('a.svg', scale=6)
         return HttpResponse ('''
         <p>Use address of youtube after watch like - for download video -  :<br>
         <b> YourSiteName/ytlink?url=<any video site link></b><br>
         or<br>
         enter Youtube ID after YourSiteName address - for play in firefox -  : <br>
         <b>YourSiteName/xazlZh1lTpM</b><br>
```

### Comparing `ersciyt-1.8/ersciyt.egg-info/PKG-INFO` & `ersciyt-1.81/ersciyt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.8
+Version: 1.81
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ersciyt-1.8/setup.cfg` & `ersciyt-1.81/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ersciyt
-version = 1.8
+version = 1.81
 description = Youtube Downloader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/yt.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

