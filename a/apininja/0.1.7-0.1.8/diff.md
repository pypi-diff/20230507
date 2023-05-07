# Comparing `tmp/apininja-0.1.7.tar.gz` & `tmp/apininja-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apininja-0.1.7.tar", last modified: Sun May  7 12:29:34 2023, max compression
+gzip compressed data, was "apininja-0.1.8.tar", last modified: Sun May  7 12:38:25 2023, max compression
```

## Comparing `apininja-0.1.7.tar` & `apininja-0.1.8.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxr-xr-x   0 syncster31   (501) staff       (20)        0 2023-05-07 12:29:34.841079 apininja-0.1.7/
--rw-r--r--   0 syncster31   (501) staff       (20)     1413 2023-05-07 12:29:34.840945 apininja-0.1.7/PKG-INFO
-drwxr-xr-x   0 syncster31   (501) staff       (20)        0 2023-05-07 12:29:34.840785 apininja-0.1.7/apininja.egg-info/
--rw-r--r--   0 syncster31   (501) staff       (20)     1413 2023-05-07 12:29:34.000000 apininja-0.1.7/apininja.egg-info/PKG-INFO
--rw-r--r--   0 syncster31   (501) staff       (20)      183 2023-05-07 12:29:34.000000 apininja-0.1.7/apininja.egg-info/SOURCES.txt
--rw-r--r--   0 syncster31   (501) staff       (20)        1 2023-05-07 12:29:34.000000 apininja-0.1.7/apininja.egg-info/dependency_links.txt
--rw-r--r--   0 syncster31   (501) staff       (20)       43 2023-05-07 12:29:34.000000 apininja-0.1.7/apininja.egg-info/entry_points.txt
--rw-r--r--   0 syncster31   (501) staff       (20)        9 2023-05-07 12:29:34.000000 apininja-0.1.7/apininja.egg-info/top_level.txt
--rw-r--r--   0 syncster31   (501) staff       (20)     1994 2023-05-07 10:52:03.000000 apininja-0.1.7/apininja.py
--rw-r--r--   0 syncster31   (501) staff       (20)       38 2023-05-07 12:29:34.841218 apininja-0.1.7/setup.cfg
--rw-r--r--   0 syncster31   (501) staff       (20)      839 2023-05-07 12:29:01.000000 apininja-0.1.7/setup.py
+drwxr-xr-x   0 syncster31   (501) staff       (20)        0 2023-05-07 12:38:25.259353 apininja-0.1.8/
+-rw-r--r--   0 syncster31   (501) staff       (20)       17 2023-05-07 12:28:41.000000 apininja-0.1.8/MANIFEST.in
+-rw-r--r--   0 syncster31   (501) staff       (20)     1413 2023-05-07 12:38:25.259191 apininja-0.1.8/PKG-INFO
+drwxr-xr-x   0 syncster31   (501) staff       (20)        0 2023-05-07 12:38:25.259021 apininja-0.1.8/apininja.egg-info/
+-rw-r--r--   0 syncster31   (501) staff       (20)     1413 2023-05-07 12:38:25.000000 apininja-0.1.8/apininja.egg-info/PKG-INFO
+-rw-r--r--   0 syncster31   (501) staff       (20)      205 2023-05-07 12:38:25.000000 apininja-0.1.8/apininja.egg-info/SOURCES.txt
+-rw-r--r--   0 syncster31   (501) staff       (20)        1 2023-05-07 12:38:25.000000 apininja-0.1.8/apininja.egg-info/dependency_links.txt
+-rw-r--r--   0 syncster31   (501) staff       (20)       43 2023-05-07 12:38:25.000000 apininja-0.1.8/apininja.egg-info/entry_points.txt
+-rw-r--r--   0 syncster31   (501) staff       (20)        9 2023-05-07 12:38:25.000000 apininja-0.1.8/apininja.egg-info/top_level.txt
+-rw-r--r--   0 syncster31   (501) staff       (20)     1994 2023-05-07 10:52:03.000000 apininja-0.1.8/apininja.py
+-rw-r--r--   0 syncster31   (501) staff       (20)      901 2023-05-07 12:21:29.000000 apininja-0.1.8/readme.md
+-rw-r--r--   0 syncster31   (501) staff       (20)       38 2023-05-07 12:38:25.259399 apininja-0.1.8/setup.cfg
+-rw-r--r--   0 syncster31   (501) staff       (20)      839 2023-05-07 12:34:50.000000 apininja-0.1.8/setup.py
```

### Comparing `apininja-0.1.7/PKG-INFO` & `apininja-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apininja
-Version: 0.1.7
+Version: 0.1.8
 Summary: An api module generator.
 Home-page: https://github.com/alexiusacademia/apininja
 Author: Alex Academia
 Author-email: alexius.sayco.academia@gmail.com
 Keywords: api generator
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `apininja-0.1.7/apininja.egg-info/PKG-INFO` & `apininja-0.1.8/apininja.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apininja
-Version: 0.1.7
+Version: 0.1.8
 Summary: An api module generator.
 Home-page: https://github.com/alexiusacademia/apininja
 Author: Alex Academia
 Author-email: alexius.sayco.academia@gmail.com
 Keywords: api generator
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `apininja-0.1.7/apininja.py` & `apininja-0.1.8/apininja.py`

 * *Files identical despite different names*

### Comparing `apininja-0.1.7/setup.py` & `apininja-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('readme.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='apininja',
-    version='0.1.7',
+    version='0.1.8',
     author='Alex Academia',
     author_email='alexius.sayco.academia@gmail.com',
     description='An api module generator.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/alexiusacademia/apininja',
     py_modules=['apininja'],
```

