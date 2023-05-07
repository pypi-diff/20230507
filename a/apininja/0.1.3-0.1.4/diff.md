# Comparing `tmp/apininja-0.1.3.tar.gz` & `tmp/apininja-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apininja-0.1.3.tar", last modified: Sun May  7 12:01:01 2023, max compression
+gzip compressed data, was "apininja-0.1.4.tar", last modified: Sun May  7 12:07:18 2023, max compression
```

## Comparing `apininja-0.1.3.tar` & `apininja-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 syncster31   (501) staff       (20)        0 2023-05-07 12:01:01.976144 apininja-0.1.3/
--rw-r--r--   0 syncster31   (501) staff       (20)      497 2023-05-07 12:01:01.976003 apininja-0.1.3/PKG-INFO
-drwxr-xr-x   0 syncster31   (501) staff       (20)        0 2023-05-07 12:01:01.975834 apininja-0.1.3/apininja.egg-info/
--rw-r--r--   0 syncster31   (501) staff       (20)      497 2023-05-07 12:01:01.000000 apininja-0.1.3/apininja.egg-info/PKG-INFO
--rw-r--r--   0 syncster31   (501) staff       (20)      183 2023-05-07 12:01:01.000000 apininja-0.1.3/apininja.egg-info/SOURCES.txt
--rw-r--r--   0 syncster31   (501) staff       (20)        1 2023-05-07 12:01:01.000000 apininja-0.1.3/apininja.egg-info/dependency_links.txt
--rw-r--r--   0 syncster31   (501) staff       (20)       43 2023-05-07 12:01:01.000000 apininja-0.1.3/apininja.egg-info/entry_points.txt
--rw-r--r--   0 syncster31   (501) staff       (20)        9 2023-05-07 12:01:01.000000 apininja-0.1.3/apininja.egg-info/top_level.txt
--rw-r--r--   0 syncster31   (501) staff       (20)     1994 2023-05-07 10:52:03.000000 apininja-0.1.3/apininja.py
--rw-r--r--   0 syncster31   (501) staff       (20)       38 2023-05-07 12:01:01.976181 apininja-0.1.3/setup.cfg
--rw-r--r--   0 syncster31   (501) staff       (20)      731 2023-05-07 11:59:41.000000 apininja-0.1.3/setup.py
+drwxr-xr-x   0 syncster31   (501) staff       (20)        0 2023-05-07 12:07:18.246062 apininja-0.1.4/
+-rw-r--r--   0 syncster31   (501) staff       (20)      497 2023-05-07 12:07:18.245908 apininja-0.1.4/PKG-INFO
+drwxr-xr-x   0 syncster31   (501) staff       (20)        0 2023-05-07 12:07:18.245723 apininja-0.1.4/apininja.egg-info/
+-rw-r--r--   0 syncster31   (501) staff       (20)      497 2023-05-07 12:07:18.000000 apininja-0.1.4/apininja.egg-info/PKG-INFO
+-rw-r--r--   0 syncster31   (501) staff       (20)      183 2023-05-07 12:07:18.000000 apininja-0.1.4/apininja.egg-info/SOURCES.txt
+-rw-r--r--   0 syncster31   (501) staff       (20)        1 2023-05-07 12:07:18.000000 apininja-0.1.4/apininja.egg-info/dependency_links.txt
+-rw-r--r--   0 syncster31   (501) staff       (20)       43 2023-05-07 12:07:18.000000 apininja-0.1.4/apininja.egg-info/entry_points.txt
+-rw-r--r--   0 syncster31   (501) staff       (20)        9 2023-05-07 12:07:18.000000 apininja-0.1.4/apininja.egg-info/top_level.txt
+-rw-r--r--   0 syncster31   (501) staff       (20)     1994 2023-05-07 10:52:03.000000 apininja-0.1.4/apininja.py
+-rw-r--r--   0 syncster31   (501) staff       (20)       38 2023-05-07 12:07:18.246102 apininja-0.1.4/setup.cfg
+-rw-r--r--   0 syncster31   (501) staff       (20)      731 2023-05-07 12:06:50.000000 apininja-0.1.4/setup.py
```

### Comparing `apininja-0.1.3/apininja.py` & `apininja-0.1.4/apininja.py`

 * *Files identical despite different names*

### Comparing `apininja-0.1.3/setup.py` & `apininja-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='apininja',
-    version='0.1.3',
+    version='0.1.4',
     author='Alex Academia',
     author_email='alexius.sayco.academia@gmail.com',
     description='An api module generator.',
     long_description='An api module generator.',
     url='https://github.com/alexiusacademia/apininja',
     py_modules=['apininja'],
     entry_points={
```

