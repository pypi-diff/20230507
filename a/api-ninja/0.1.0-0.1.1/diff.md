# Comparing `tmp/api_ninja-0.1.0.tar.gz` & `tmp/api_ninja-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_ninja-0.1.0.tar", last modified: Sun May  7 11:15:05 2023, max compression
+gzip compressed data, was "api_ninja-0.1.1.tar", last modified: Sun May  7 11:29:31 2023, max compression
```

## Comparing `api_ninja-0.1.0.tar` & `api_ninja-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 syncster31   (501) staff       (20)        0 2023-05-07 11:15:05.247074 api_ninja-0.1.0/
--rw-r--r--   0 syncster31   (501) staff       (20)      498 2023-05-07 11:15:05.246941 api_ninja-0.1.0/PKG-INFO
-drwxr-xr-x   0 syncster31   (501) staff       (20)        0 2023-05-07 11:15:05.246537 api_ninja-0.1.0/api_ninja.egg-info/
--rw-r--r--   0 syncster31   (501) staff       (20)      498 2023-05-07 11:15:05.000000 api_ninja-0.1.0/api_ninja.egg-info/PKG-INFO
--rw-r--r--   0 syncster31   (501) staff       (20)      176 2023-05-07 11:15:05.000000 api_ninja-0.1.0/api_ninja.egg-info/SOURCES.txt
--rw-r--r--   0 syncster31   (501) staff       (20)        1 2023-05-07 11:15:05.000000 api_ninja-0.1.0/api_ninja.egg-info/dependency_links.txt
--rw-r--r--   0 syncster31   (501) staff       (20)       39 2023-05-07 11:15:05.000000 api_ninja-0.1.0/api_ninja.egg-info/entry_points.txt
--rw-r--r--   0 syncster31   (501) staff       (20)       10 2023-05-07 11:15:05.000000 api_ninja-0.1.0/api_ninja.egg-info/top_level.txt
--rw-r--r--   0 syncster31   (501) staff       (20)       38 2023-05-07 11:15:05.247114 api_ninja-0.1.0/setup.cfg
--rw-r--r--   0 syncster31   (501) staff       (20)      729 2023-05-07 11:11:26.000000 api_ninja-0.1.0/setup.py
+drwxr-xr-x   0 syncster31   (501) staff       (20)        0 2023-05-07 11:29:31.188360 api_ninja-0.1.1/
+-rw-r--r--   0 syncster31   (501) staff       (20)      498 2023-05-07 11:29:31.188232 api_ninja-0.1.1/PKG-INFO
+drwxr-xr-x   0 syncster31   (501) staff       (20)        0 2023-05-07 11:29:31.188069 api_ninja-0.1.1/api_ninja.egg-info/
+-rw-r--r--   0 syncster31   (501) staff       (20)      498 2023-05-07 11:29:31.000000 api_ninja-0.1.1/api_ninja.egg-info/PKG-INFO
+-rw-r--r--   0 syncster31   (501) staff       (20)      176 2023-05-07 11:29:31.000000 api_ninja-0.1.1/api_ninja.egg-info/SOURCES.txt
+-rw-r--r--   0 syncster31   (501) staff       (20)        1 2023-05-07 11:29:31.000000 api_ninja-0.1.1/api_ninja.egg-info/dependency_links.txt
+-rw-r--r--   0 syncster31   (501) staff       (20)       39 2023-05-07 11:29:31.000000 api_ninja-0.1.1/api_ninja.egg-info/entry_points.txt
+-rw-r--r--   0 syncster31   (501) staff       (20)        9 2023-05-07 11:29:31.000000 api_ninja-0.1.1/api_ninja.egg-info/top_level.txt
+-rw-r--r--   0 syncster31   (501) staff       (20)       38 2023-05-07 11:29:31.188399 api_ninja-0.1.1/setup.cfg
+-rw-r--r--   0 syncster31   (501) staff       (20)      728 2023-05-07 11:27:09.000000 api_ninja-0.1.1/setup.py
```

### Comparing `api_ninja-0.1.0/setup.py` & `api_ninja-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 setup(
     name='api_ninja',
-    version='0.1.0',
+    version='0.1.1',
     author='Alex Academia',
     author_email='alexius.sayco.academia@gmail.com',
     description='An api module generator.',
     long_description='An api module generator.',
     url='https://github.com/alexiusacademia/apininja',
-    py_modules=['api_ninja'],
+    py_modules=['apininja'],
     entry_points={
         'console_scripts': [
             'apininja = main:main',
         ],
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
```

