# Comparing `tmp/grahamstools-0.1.2.tar.gz` & `tmp/grahamstools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grahamstools-0.1.2.tar", last modified: Sat May  6 22:29:50 2023, max compression
+gzip compressed data, was "grahamstools-0.1.3.tar", last modified: Sat May  6 22:54:10 2023, max compression
```

## Comparing `grahamstools-0.1.2.tar` & `grahamstools-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 22:29:50.928041 grahamstools-0.1.2/
--rw-rw-rw-   0        0        0      653 2023-05-06 22:29:50.923041 grahamstools-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-14 02:09:20.000000 grahamstools-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 22:29:50.897043 grahamstools-0.1.2/grahamstools/
--rw-rw-rw-   0        0        0      355 2023-05-06 22:10:38.000000 grahamstools-0.1.2/grahamstools/__init__.py
--rw-rw-rw-   0        0        0     2009 2023-05-06 22:23:28.000000 grahamstools-0.1.2/grahamstools/module1.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:29:50.919041 grahamstools-0.1.2/grahamstools.egg-info/
--rw-rw-rw-   0        0        0      653 2023-05-06 22:29:50.000000 grahamstools-0.1.2/grahamstools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-05-06 22:29:50.000000 grahamstools-0.1.2/grahamstools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 22:29:50.000000 grahamstools-0.1.2/grahamstools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-06 22:29:50.000000 grahamstools-0.1.2/grahamstools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 22:29:50.929041 grahamstools-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1032 2023-05-06 22:28:53.000000 grahamstools-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:54:10.151041 grahamstools-0.1.3/
+-rw-rw-rw-   0        0        0      653 2023-05-06 22:54:10.147042 grahamstools-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-14 02:09:20.000000 grahamstools-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 22:54:10.124043 grahamstools-0.1.3/grahamstools/
+-rw-rw-rw-   0        0        0      355 2023-05-06 22:10:38.000000 grahamstools-0.1.3/grahamstools/__init__.py
+-rw-rw-rw-   0        0        0     2016 2023-05-06 22:37:16.000000 grahamstools-0.1.3/grahamstools/module1.py
+-rw-rw-rw-   0        0        0     4852 2023-05-06 22:48:38.000000 grahamstools-0.1.3/grahamstools/move_mouse.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:54:10.143043 grahamstools-0.1.3/grahamstools.egg-info/
+-rw-rw-rw-   0        0        0      653 2023-05-06 22:54:09.000000 grahamstools-0.1.3/grahamstools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-05-06 22:54:09.000000 grahamstools-0.1.3/grahamstools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 22:54:09.000000 grahamstools-0.1.3/grahamstools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-06 22:54:09.000000 grahamstools-0.1.3/grahamstools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 22:54:10.151041 grahamstools-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2023-05-06 22:54:00.000000 grahamstools-0.1.3/setup.py
```

### Comparing `grahamstools-0.1.2/PKG-INFO` & `grahamstools-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grahamstools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools and resources for Python developers
 Home-page: https://github.com/GrahamboJangles/GrahamsTools
 Download-URL: https://github.com/GrahamboJangles/GrahamsTools/archive/refs/tags/0.1.0.tar.gz
 Author: GrahamboJangles
 Author-email: lafebregraham@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `grahamstools-0.1.2/grahamstools/module1.py` & `grahamstools-0.1.3/grahamstools/module1.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             session.SimpleAudioVolume.SetMasterVolume(volume, None)
 
 def system_tray_icon(tooltip, image_path):
     # Create an image for the system tray icon
     image = Image.open(image_path)
     # Create a system tray icon with the specified image and menu
     global tray_icon
-    tray_icon = icon(tooltip, image, tooltip, menu)
+    tray_icon = icon(tooltip, image, tooltip, menu=menu())
 
 def create_function_in_thread(function):
     # Create a thread for the system tray icon
     global tray_thread
     tray_thread = threading.Thread(target=function)
 
 def run_thread(thread):
```

### Comparing `grahamstools-0.1.2/grahamstools.egg-info/PKG-INFO` & `grahamstools-0.1.3/grahamstools.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grahamstools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools and resources for Python developers
 Home-page: https://github.com/GrahamboJangles/GrahamsTools
 Download-URL: https://github.com/GrahamboJangles/GrahamsTools/archive/refs/tags/0.1.0.tar.gz
 Author: GrahamboJangles
 Author-email: lafebregraham@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `grahamstools-0.1.2/setup.py` & `grahamstools-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='grahamstools',
-    version='0.1.2',
+    version='0.1.3',
     author='GrahamboJangles',
     author_email='lafebregraham@gmail.com',
     description='Tools and resources for Python developers',
     url = "https://github.com/GrahamboJangles/GrahamsTools",
     download_url = "https://github.com/GrahamboJangles/GrahamsTools/archive/refs/tags/0.1.0.tar.gz",
     packages=find_packages(),
     # This is for required dependencies
```

