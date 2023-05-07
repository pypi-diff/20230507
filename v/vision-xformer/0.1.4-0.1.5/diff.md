# Comparing `tmp/vision_xformer-0.1.4.tar.gz` & `tmp/vision_xformer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_xformer-0.1.4.tar", last modified: Sat May  6 18:57:27 2023, max compression
+gzip compressed data, was "vision_xformer-0.1.5.tar", last modified: Sun May  7 00:19:10 2023, max compression
```

## Comparing `vision_xformer-0.1.4.tar` & `vision_xformer-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 18:57:27.076306 vision_xformer-0.1.4/
--rw-rw-rw-   0        0        0     1072 2023-05-06 01:04:48.000000 vision_xformer-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     3823 2023-05-06 18:57:27.073309 vision_xformer-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3085 2023-05-06 01:04:35.000000 vision_xformer-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 18:57:27.076306 vision_xformer-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1145 2023-05-06 18:57:06.000000 vision_xformer-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:57:26.979368 vision_xformer-0.1.4/vision_xformer/
--rw-rw-rw-   0        0        0      157 2023-05-06 02:12:38.000000 vision_xformer-0.1.4/vision_xformer/__init__.py
--rw-rw-rw-   0        0        0     6497 2023-05-06 18:56:56.000000 vision_xformer-0.1.4/vision_xformer/vision_linformer.py
--rw-rw-rw-   0        0        0     7009 2023-05-06 01:29:58.000000 vision_xformer-0.1.4/vision_xformer/vision_nystromformer.py
--rw-rw-rw-   0        0        0    20185 2023-05-06 01:55:44.000000 vision_xformer-0.1.4/vision_xformer/vision_performer.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:57:27.071293 vision_xformer-0.1.4/vision_xformer.egg-info/
--rw-rw-rw-   0        0        0     3823 2023-05-06 18:57:26.000000 vision_xformer-0.1.4/vision_xformer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-05-06 18:57:26.000000 vision_xformer-0.1.4/vision_xformer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:57:26.000000 vision_xformer-0.1.4/vision_xformer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-06 18:57:26.000000 vision_xformer-0.1.4/vision_xformer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-06 18:57:26.000000 vision_xformer-0.1.4/vision_xformer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 00:19:10.609014 vision_xformer-0.1.5/
+-rw-rw-rw-   0        0        0     1072 2023-05-06 01:04:48.000000 vision_xformer-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     3823 2023-05-07 00:19:10.608015 vision_xformer-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3085 2023-05-06 01:04:35.000000 vision_xformer-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-07 00:19:10.610015 vision_xformer-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1145 2023-05-07 00:18:52.000000 vision_xformer-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 00:19:10.504738 vision_xformer-0.1.5/vision_xformer/
+-rw-rw-rw-   0        0        0      233 2023-05-07 00:18:03.000000 vision_xformer-0.1.5/vision_xformer/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-06 19:02:18.000000 vision_xformer-0.1.5/vision_xformer/fnet.py
+-rw-rw-rw-   0        0        0     1913 2023-05-07 00:12:55.000000 vision_xformer-0.1.5/vision_xformer/fnet2d.py
+-rw-rw-rw-   0        0        0     6497 2023-05-06 18:56:56.000000 vision_xformer-0.1.5/vision_xformer/vision_linformer.py
+-rw-rw-rw-   0        0        0     7009 2023-05-06 01:29:58.000000 vision_xformer-0.1.5/vision_xformer/vision_nystromformer.py
+-rw-rw-rw-   0        0        0    20185 2023-05-06 01:55:44.000000 vision_xformer-0.1.5/vision_xformer/vision_performer.py
+drwxrwxrwx   0        0        0        0 2023-05-07 00:19:10.605016 vision_xformer-0.1.5/vision_xformer.egg-info/
+-rw-rw-rw-   0        0        0     3823 2023-05-07 00:19:10.000000 vision_xformer-0.1.5/vision_xformer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-05-07 00:19:10.000000 vision_xformer-0.1.5/vision_xformer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 00:19:10.000000 vision_xformer-0.1.5/vision_xformer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-07 00:19:10.000000 vision_xformer-0.1.5/vision_xformer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-07 00:19:10.000000 vision_xformer-0.1.5/vision_xformer.egg-info/top_level.txt
```

### Comparing `vision_xformer-0.1.4/LICENSE` & `vision_xformer-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.4/PKG-INFO` & `vision_xformer-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision_xformer
-Version: 0.1.4
+Version: 0.1.5
 Summary: Vision Xformers
 Home-page: https://github.com/pranavphoenix/VisionXformer
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,training,optimizer,machine learning,attention,transformers,computer vision
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vision_xformer-0.1.4/README.md` & `vision_xformer-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.4/setup.py` & `vision_xformer-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
   name = 'vision_xformer',
   packages = find_packages(exclude=['examples']),
-  version = '0.1.4',
+  version = '0.1.5',
   license='MIT',
   description = 'Vision Xformers',
   long_description=long_description,
   long_description_content_type = 'text/markdown',
   author = 'Pranav Jeevan',
   author_email = 'pranav13phoenix@gmail.com',
   url = 'https://github.com/pranavphoenix/VisionXformer',
```

### Comparing `vision_xformer-0.1.4/vision_xformer/vision_linformer.py` & `vision_xformer-0.1.5/vision_xformer/vision_linformer.py`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.4/vision_xformer/vision_nystromformer.py` & `vision_xformer-0.1.5/vision_xformer/vision_nystromformer.py`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.4/vision_xformer/vision_performer.py` & `vision_xformer-0.1.5/vision_xformer/vision_performer.py`

 * *Files identical despite different names*

### Comparing `vision_xformer-0.1.4/vision_xformer.egg-info/PKG-INFO` & `vision_xformer-0.1.5/vision_xformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-xformer
-Version: 0.1.4
+Version: 0.1.5
 Summary: Vision Xformers
 Home-page: https://github.com/pranavphoenix/VisionXformer
 Author: Pranav Jeevan
 Author-email: pranav13phoenix@gmail.com
 License: MIT
 Keywords: artificial intelligence,training,optimizer,machine learning,attention,transformers,computer vision
 Classifier: Development Status :: 4 - Beta
```

