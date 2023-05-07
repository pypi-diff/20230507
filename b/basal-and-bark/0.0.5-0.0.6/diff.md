# Comparing `tmp/basal_and_bark-0.0.5.tar.gz` & `tmp/basal_and_bark-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basal_and_bark-0.0.5.tar", last modified: Thu Apr 27 15:48:18 2023, max compression
+gzip compressed data, was "basal_and_bark-0.0.6.tar", last modified: Sun May  7 01:14:37 2023, max compression
```

## Comparing `basal_and_bark-0.0.5.tar` & `basal_and_bark-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:48:18.244647 basal_and_bark-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 15:47:57.000000 basal_and_bark-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-27 15:47:57.000000 basal_and_bark-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-27 15:48:18.244647 basal_and_bark-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-27 15:47:57.000000 basal_and_bark-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:48:18.244647 basal_and_bark-0.0.5/basal_and_bark/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-27 15:47:57.000000 basal_and_bark-0.0.5/basal_and_bark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-27 15:47:57.000000 basal_and_bark-0.0.5/basal_and_bark/basal_and_bark.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-04-27 15:47:57.000000 basal_and_bark-0.0.5/basal_and_bark/basal_and_bark_folium.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:48:18.244647 basal_and_bark-0.0.5/basal_and_bark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-27 15:48:18.000000 basal_and_bark-0.0.5/basal_and_bark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-27 15:48:18.000000 basal_and_bark-0.0.5/basal_and_bark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 15:48:18.000000 basal_and_bark-0.0.5/basal_and_bark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:48:18.000000 basal_and_bark-0.0.5/basal_and_bark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 15:48:18.000000 basal_and_bark-0.0.5/basal_and_bark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 15:48:18.000000 basal_and_bark-0.0.5/basal_and_bark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 15:47:58.000000 basal_and_bark-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-27 15:48:18.244647 basal_and_bark-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-27 15:47:58.000000 basal_and_bark-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:14:37.494269 basal_and_bark-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-07 01:14:20.000000 basal_and_bark-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-07 01:14:20.000000 basal_and_bark-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-07 01:14:37.494269 basal_and_bark-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-07 01:14:20.000000 basal_and_bark-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:14:37.490269 basal_and_bark-0.0.6/basal_and_bark/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-07 01:14:20.000000 basal_and_bark-0.0.6/basal_and_bark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20679 2023-05-07 01:14:20.000000 basal_and_bark-0.0.6/basal_and_bark/basal_and_bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-07 01:14:20.000000 basal_and_bark-0.0.6/basal_and_bark/basal_and_bark_folium.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:14:37.494269 basal_and_bark-0.0.6/basal_and_bark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-07 01:14:37.000000 basal_and_bark-0.0.6/basal_and_bark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-07 01:14:37.000000 basal_and_bark-0.0.6/basal_and_bark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 01:14:37.000000 basal_and_bark-0.0.6/basal_and_bark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 01:14:37.000000 basal_and_bark-0.0.6/basal_and_bark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 01:14:37.000000 basal_and_bark-0.0.6/basal_and_bark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 01:14:37.000000 basal_and_bark-0.0.6/basal_and_bark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-07 01:14:20.000000 basal_and_bark-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-07 01:14:37.494269 basal_and_bark-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-07 01:14:20.000000 basal_and_bark-0.0.6/setup.py
```

### Comparing `basal_and_bark-0.0.5/LICENSE` & `basal_and_bark-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `basal_and_bark-0.0.5/PKG-INFO` & `basal_and_bark-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basal_and_bark
-Version: 0.0.5
+Version: 0.0.6
 Summary: Welcome to Basal and Bark, a spatial python package for working with forest data.
 Home-page: https://github.com/ZachDorm/basal_and_bark
 Author: Zach Dorminey
 Author-email: zach.dorminey@gmail.com
 License: MIT license
 Keywords: basal_and_bark
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `basal_and_bark-0.0.5/README.md` & `basal_and_bark-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `basal_and_bark-0.0.5/basal_and_bark/basal_and_bark_folium.py` & `basal_and_bark-0.0.6/basal_and_bark/basal_and_bark_folium.py`

 * *Files identical despite different names*

### Comparing `basal_and_bark-0.0.5/basal_and_bark.egg-info/PKG-INFO` & `basal_and_bark-0.0.6/basal_and_bark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basal-and-bark
-Version: 0.0.5
+Version: 0.0.6
 Summary: Welcome to Basal and Bark, a spatial python package for working with forest data.
 Home-page: https://github.com/ZachDorm/basal_and_bark
 Author: Zach Dorminey
 Author-email: zach.dorminey@gmail.com
 License: MIT license
 Keywords: basal_and_bark
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `basal_and_bark-0.0.5/setup.py` & `basal_and_bark-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='basal_and_bark',
     name='basal_and_bark',
     packages=find_packages(include=['basal_and_bark', 'basal_and_bark.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ZachDorm/basal_and_bark',
-    version='0.0.5',
+    version='0.0.6',
     zip_safe=False,
 )
```

