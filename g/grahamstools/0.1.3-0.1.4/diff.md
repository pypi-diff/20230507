# Comparing `tmp/grahamstools-0.1.3.tar.gz` & `tmp/grahamstools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grahamstools-0.1.3.tar", last modified: Sat May  6 22:54:10 2023, max compression
+gzip compressed data, was "grahamstools-0.1.4.tar", last modified: Sat May  6 23:06:23 2023, max compression
```

## Comparing `grahamstools-0.1.3.tar` & `grahamstools-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 22:54:10.151041 grahamstools-0.1.3/
--rw-rw-rw-   0        0        0      653 2023-05-06 22:54:10.147042 grahamstools-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-14 02:09:20.000000 grahamstools-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 22:54:10.124043 grahamstools-0.1.3/grahamstools/
--rw-rw-rw-   0        0        0      355 2023-05-06 22:10:38.000000 grahamstools-0.1.3/grahamstools/__init__.py
--rw-rw-rw-   0        0        0     2016 2023-05-06 22:37:16.000000 grahamstools-0.1.3/grahamstools/module1.py
--rw-rw-rw-   0        0        0     4852 2023-05-06 22:48:38.000000 grahamstools-0.1.3/grahamstools/move_mouse.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:54:10.143043 grahamstools-0.1.3/grahamstools.egg-info/
--rw-rw-rw-   0        0        0      653 2023-05-06 22:54:09.000000 grahamstools-0.1.3/grahamstools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-05-06 22:54:09.000000 grahamstools-0.1.3/grahamstools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 22:54:09.000000 grahamstools-0.1.3/grahamstools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-06 22:54:09.000000 grahamstools-0.1.3/grahamstools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 22:54:10.151041 grahamstools-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1032 2023-05-06 22:54:00.000000 grahamstools-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 23:06:23.418042 grahamstools-0.1.4/
+-rw-rw-rw-   0        0        0      653 2023-05-06 23:06:23.413042 grahamstools-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-14 02:09:20.000000 grahamstools-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 23:06:23.390041 grahamstools-0.1.4/grahamstools/
+-rw-rw-rw-   0        0        0      356 2023-05-06 22:58:48.000000 grahamstools-0.1.4/grahamstools/__init__.py
+-rw-rw-rw-   0        0        0     2016 2023-05-06 22:37:16.000000 grahamstools-0.1.4/grahamstools/module1.py
+-rw-rw-rw-   0        0        0     4852 2023-05-06 22:48:38.000000 grahamstools-0.1.4/grahamstools/move_mouse.py
+drwxrwxrwx   0        0        0        0 2023-05-06 23:06:23.410043 grahamstools-0.1.4/grahamstools.egg-info/
+-rw-rw-rw-   0        0        0      653 2023-05-06 23:06:23.000000 grahamstools-0.1.4/grahamstools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-05-06 23:06:23.000000 grahamstools-0.1.4/grahamstools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 23:06:23.000000 grahamstools-0.1.4/grahamstools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-06 23:06:23.000000 grahamstools-0.1.4/grahamstools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 23:06:23.418042 grahamstools-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2023-05-06 23:06:13.000000 grahamstools-0.1.4/setup.py
```

### Comparing `grahamstools-0.1.3/PKG-INFO` & `grahamstools-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grahamstools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools and resources for Python developers
 Home-page: https://github.com/GrahamboJangles/GrahamsTools
 Download-URL: https://github.com/GrahamboJangles/GrahamsTools/archive/refs/tags/0.1.0.tar.gz
 Author: GrahamboJangles
 Author-email: lafebregraham@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `grahamstools-0.1.3/grahamstools/module1.py` & `grahamstools-0.1.4/grahamstools/module1.py`

 * *Files identical despite different names*

### Comparing `grahamstools-0.1.3/grahamstools/move_mouse.py` & `grahamstools-0.1.4/grahamstools/move_mouse.py`

 * *Files identical despite different names*

### Comparing `grahamstools-0.1.3/grahamstools.egg-info/PKG-INFO` & `grahamstools-0.1.4/grahamstools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grahamstools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools and resources for Python developers
 Home-page: https://github.com/GrahamboJangles/GrahamsTools
 Download-URL: https://github.com/GrahamboJangles/GrahamsTools/archive/refs/tags/0.1.0.tar.gz
 Author: GrahamboJangles
 Author-email: lafebregraham@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `grahamstools-0.1.3/setup.py` & `grahamstools-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='grahamstools',
-    version='0.1.3',
+    version='0.1.4',
     author='GrahamboJangles',
     author_email='lafebregraham@gmail.com',
     description='Tools and resources for Python developers',
     url = "https://github.com/GrahamboJangles/GrahamsTools",
     download_url = "https://github.com/GrahamboJangles/GrahamsTools/archive/refs/tags/0.1.0.tar.gz",
     packages=find_packages(),
     # This is for required dependencies
```

