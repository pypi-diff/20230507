# Comparing `tmp/mistacheeselib-0.0.2.tar.gz` & `tmp/mistacheeselib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistacheeselib-0.0.2.tar", last modified: Wed Apr  5 19:19:54 2023, max compression
+gzip compressed data, was "mistacheeselib-0.0.3.tar", last modified: Sun May  7 08:05:13 2023, max compression
```

## Comparing `mistacheeselib-0.0.2.tar` & `mistacheeselib-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mistacheese   (501) staff       (20)        0 2023-04-05 19:19:54.807599 mistacheeselib-0.0.2/
--rw-r--r--   0 mistacheese   (501) staff       (20)      147 2023-04-05 19:19:23.000000 mistacheeselib-0.0.2/CHANGELOG.txt
--rw-r--r--   0 mistacheese   (501) staff       (20)     1060 2023-03-25 16:19:24.000000 mistacheeselib-0.0.2/LICENSE.txt
--rw-r--r--   0 mistacheese   (501) staff       (20)       25 2023-03-25 16:19:24.000000 mistacheeselib-0.0.2/MANIFEST.in
--rw-r--r--   0 mistacheese   (501) staff       (20)      704 2023-04-05 19:19:54.807491 mistacheeselib-0.0.2/PKG-INFO
--rw-r--r--   0 mistacheese   (501) staff       (20)       64 2023-03-25 16:19:24.000000 mistacheeselib-0.0.2/README.txt
--rw-r--r--   0 mistacheese   (501) staff       (20)      294 2023-03-25 16:19:24.000000 mistacheeselib-0.0.2/__init__.py
-drwxr-xr-x   0 mistacheese   (501) staff       (20)        0 2023-04-05 19:19:54.807342 mistacheeselib-0.0.2/mistacheeselib.egg-info/
--rw-r--r--   0 mistacheese   (501) staff       (20)      704 2023-04-05 19:19:54.000000 mistacheeselib-0.0.2/mistacheeselib.egg-info/PKG-INFO
--rw-r--r--   0 mistacheese   (501) staff       (20)      221 2023-04-05 19:19:54.000000 mistacheeselib-0.0.2/mistacheeselib.egg-info/SOURCES.txt
--rw-r--r--   0 mistacheese   (501) staff       (20)        1 2023-04-05 19:19:54.000000 mistacheeselib-0.0.2/mistacheeselib.egg-info/dependency_links.txt
--rw-r--r--   0 mistacheese   (501) staff       (20)        1 2023-04-05 19:19:54.000000 mistacheeselib-0.0.2/mistacheeselib.egg-info/top_level.txt
--rw-r--r--   0 mistacheese   (501) staff       (20)       38 2023-04-05 19:19:54.807635 mistacheeselib-0.0.2/setup.cfg
--rw-r--r--   0 mistacheese   (501) staff       (20)      677 2023-04-05 19:19:23.000000 mistacheeselib-0.0.2/setup.py
+drwxr-xr-x   0 mistacheese   (501) staff       (20)        0 2023-05-07 08:05:13.937139 mistacheeselib-0.0.3/
+-rw-r--r--   0 mistacheese   (501) staff       (20)      213 2023-05-07 07:59:58.000000 mistacheeselib-0.0.3/CHANGELOG.txt
+-rw-r--r--   0 mistacheese   (501) staff       (20)     1060 2023-03-25 16:19:24.000000 mistacheeselib-0.0.3/LICENSE.txt
+-rw-r--r--   0 mistacheese   (501) staff       (20)       25 2023-03-25 16:19:24.000000 mistacheeselib-0.0.3/MANIFEST.in
+-rw-r--r--   0 mistacheese   (501) staff       (20)      750 2023-05-07 08:05:13.937039 mistacheeselib-0.0.3/PKG-INFO
+-rw-r--r--   0 mistacheese   (501) staff       (20)       64 2023-03-25 16:19:24.000000 mistacheeselib-0.0.3/README.txt
+-rw-r--r--   0 mistacheese   (501) staff       (20)      294 2023-05-07 07:59:56.000000 mistacheeselib-0.0.3/__init__.py
+drwxr-xr-x   0 mistacheese   (501) staff       (20)        0 2023-05-07 08:05:13.936880 mistacheeselib-0.0.3/mistacheeselib.egg-info/
+-rw-r--r--   0 mistacheese   (501) staff       (20)      750 2023-05-07 08:05:13.000000 mistacheeselib-0.0.3/mistacheeselib.egg-info/PKG-INFO
+-rw-r--r--   0 mistacheese   (501) staff       (20)      221 2023-05-07 08:05:13.000000 mistacheeselib-0.0.3/mistacheeselib.egg-info/SOURCES.txt
+-rw-r--r--   0 mistacheese   (501) staff       (20)        1 2023-05-07 08:05:13.000000 mistacheeselib-0.0.3/mistacheeselib.egg-info/dependency_links.txt
+-rw-r--r--   0 mistacheese   (501) staff       (20)        1 2023-05-07 08:05:13.000000 mistacheeselib-0.0.3/mistacheeselib.egg-info/top_level.txt
+-rw-r--r--   0 mistacheese   (501) staff       (20)       38 2023-05-07 08:05:13.937173 mistacheeselib-0.0.3/setup.cfg
+-rw-r--r--   0 mistacheese   (501) staff       (20)      657 2023-05-07 08:05:02.000000 mistacheeselib-0.0.3/setup.py
```

### Comparing `mistacheeselib-0.0.2/LICENSE.txt` & `mistacheeselib-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mistacheeselib-0.0.2/PKG-INFO` & `mistacheeselib-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mistacheeselib
-Version: 0.0.2
+Version: 0.0.3
 Summary: some extra functions
 Home-page: 
 Author: Mate Chocheli
 Author-email: matechocheli2@gmail.com
 License: MIT
 Keywords: mistacheeselib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
 
 This is a library that adds some usefull/not usefull fucnctions.
 
 Change log
@@ -21,8 +21,12 @@
 
 0.0.1(25/03/2023)
 -----------------
  - First release
 
 0.0.2(5/04/2023)
 -----------------
- - the First one didn't work
+ - the first one didn't work
+
+0.0.3(7/05/2023)
+-----------------
+ - the second one didn't work
```

### Comparing `mistacheeselib-0.0.2/mistacheeselib.egg-info/PKG-INFO` & `mistacheeselib-0.0.3/mistacheeselib.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mistacheeselib
-Version: 0.0.2
+Version: 0.0.3
 Summary: some extra functions
 Home-page: 
 Author: Mate Chocheli
 Author-email: matechocheli2@gmail.com
 License: MIT
 Keywords: mistacheeselib
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.txt
 
 This is a library that adds some usefull/not usefull fucnctions.
 
 Change log
@@ -21,8 +21,12 @@
 
 0.0.1(25/03/2023)
 -----------------
  - First release
 
 0.0.2(5/04/2023)
 -----------------
- - the First one didn't work
+ - the first one didn't work
+
+0.0.3(7/05/2023)
+-----------------
+ - the second one didn't work
```

### Comparing `mistacheeselib-0.0.2/setup.py` & `mistacheeselib-0.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 classifiers = [
   'Development Status :: 5 - Production/Stable',
   'Intended Audience :: Education',
-  'Operating System :: Microsoft :: Windows :: Windows 10',
+  'Operating System :: OS Independent',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='mistacheeselib',
-  version='0.0.2',
+  version='0.0.3',
   description='some extra functions',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Mate Chocheli',
   author_email='matechocheli2@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

