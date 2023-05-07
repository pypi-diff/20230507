# Comparing `tmp/async_pipeline-0.1.0.tar.gz` & `tmp/async_pipeline-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/async_pipeline-0.1.0.tar", last modified: Sun May  7 09:05:54 2023, max compression
+gzip compressed data, was "dist/async_pipeline-0.1.1.tar", last modified: Sun May  7 09:19:59 2023, max compression
```

## Comparing `async_pipeline-0.1.0.tar` & `async_pipeline-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,57 @@
-drwxr-xr-x   0 rockey     (501) staff       (20)        0 2023-05-07 09:05:54.000000 async_pipeline-0.1.0/
--rw-r--r--   0 rockey     (501) staff       (20)     1066 2023-05-04 06:59:02.000000 async_pipeline-0.1.0/LICENSE
--rw-r--r--   0 rockey     (501) staff       (20)    10098 2023-05-07 09:05:54.000000 async_pipeline-0.1.0/PKG-INFO
--rw-r--r--   0 rockey     (501) staff       (20)     9346 2023-05-07 05:59:44.000000 async_pipeline-0.1.0/README.md
-drwxr-xr-x   0 rockey     (501) staff       (20)        0 2023-05-07 09:05:54.000000 async_pipeline-0.1.0/async_pipeline/
--rw-r--r--   0 rockey     (501) staff       (20)       56 2023-05-06 07:22:37.000000 async_pipeline-0.1.0/async_pipeline/__init__.py
--rw-r--r--   0 rockey     (501) staff       (20)      809 2023-05-06 06:49:53.000000 async_pipeline-0.1.0/async_pipeline/pipe.py
--rw-r--r--   0 rockey     (501) staff       (20)      624 2023-05-05 12:53:08.000000 async_pipeline-0.1.0/async_pipeline/queue.py
--rw-r--r--   0 rockey     (501) staff       (20)      103 2023-05-04 06:23:05.000000 async_pipeline-0.1.0/async_pipeline/signal.py
--rw-r--r--   0 rockey     (501) staff       (20)     2264 2023-05-06 05:32:24.000000 async_pipeline-0.1.0/async_pipeline/stage.py
-drwxr-xr-x   0 rockey     (501) staff       (20)        0 2023-05-07 09:05:54.000000 async_pipeline-0.1.0/async_pipeline.egg-info/
--rw-r--r--   0 rockey     (501) staff       (20)    10098 2023-05-07 09:05:54.000000 async_pipeline-0.1.0/async_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 rockey     (501) staff       (20)      625 2023-05-07 09:05:54.000000 async_pipeline-0.1.0/async_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 rockey     (501) staff       (20)        1 2023-05-07 09:05:54.000000 async_pipeline-0.1.0/async_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 rockey     (501) staff       (20)       15 2023-05-07 09:05:54.000000 async_pipeline-0.1.0/async_pipeline.egg-info/top_level.txt
--rw-r--r--   0 rockey     (501) staff       (20)       38 2023-05-07 09:05:54.000000 async_pipeline-0.1.0/setup.cfg
--rw-r--r--   0 rockey     (501) staff       (20)     1322 2023-05-06 02:28:50.000000 async_pipeline-0.1.0/setup.py
-drwxr-xr-x   0 rockey     (501) staff       (20)        0 2023-05-07 09:05:54.000000 async_pipeline-0.1.0/tests/
--rw-r--r--   0 rockey     (501) staff       (20)     9437 2023-05-06 07:56:20.000000 async_pipeline-0.1.0/tests/test_complex.py
--rw-r--r--   0 rockey     (501) staff       (20)     5918 2023-05-07 04:06:20.000000 async_pipeline-0.1.0/tests/test_concat.py
--rw-r--r--   0 rockey     (501) staff       (20)     2679 2023-05-06 07:56:20.000000 async_pipeline-0.1.0/tests/test_data.py
--rw-r--r--   0 rockey     (501) staff       (20)     2498 2023-05-06 07:56:19.000000 async_pipeline-0.1.0/tests/test_distinct.py
--rw-r--r--   0 rockey     (501) staff       (20)     2620 2023-05-06 07:56:19.000000 async_pipeline-0.1.0/tests/test_duplicate.py
--rw-r--r--   0 rockey     (501) staff       (20)     3223 2023-05-06 07:56:19.000000 async_pipeline-0.1.0/tests/test_each.py
--rw-r--r--   0 rockey     (501) staff       (20)      930 2023-05-06 07:56:19.000000 async_pipeline-0.1.0/tests/test_exception.py
--rw-r--r--   0 rockey     (501) staff       (20)     2072 2023-05-06 07:56:20.000000 async_pipeline-0.1.0/tests/test_filter.py
--rw-r--r--   0 rockey     (501) staff       (20)     2120 2023-05-06 07:56:20.000000 async_pipeline-0.1.0/tests/test_filter_not.py
--rw-r--r--   0 rockey     (501) staff       (20)     1947 2023-05-06 07:56:19.000000 async_pipeline-0.1.0/tests/test_flatten.py
--rw-r--r--   0 rockey     (501) staff       (20)     1308 2023-05-06 07:56:20.000000 async_pipeline-0.1.0/tests/test_limit.py
--rw-r--r--   0 rockey     (501) staff       (20)     2623 2023-05-06 07:56:20.000000 async_pipeline-0.1.0/tests/test_map.py
--rw-r--r--   0 rockey     (501) staff       (20)     3525 2023-05-06 07:56:20.000000 async_pipeline-0.1.0/tests/test_multiply.py
--rw-r--r--   0 rockey     (501) staff       (20)     5384 2023-05-06 07:56:20.000000 async_pipeline-0.1.0/tests/test_partition.py
--rw-r--r--   0 rockey     (501) staff       (20)     3261 2023-05-06 07:56:19.000000 async_pipeline-0.1.0/tests/test_peek.py
+drwxr-xr-x   0 rockey     (501) staff       (20)        0 2023-05-07 09:19:59.000000 async_pipeline-0.1.1/
+-rw-r--r--   0 rockey     (501) staff       (20)     1066 2023-05-04 06:59:02.000000 async_pipeline-0.1.1/LICENSE
+-rw-r--r--   0 rockey     (501) staff       (20)    10098 2023-05-07 09:19:59.000000 async_pipeline-0.1.1/PKG-INFO
+-rw-r--r--   0 rockey     (501) staff       (20)     9346 2023-05-07 05:59:44.000000 async_pipeline-0.1.1/README.md
+drwxr-xr-x   0 rockey     (501) staff       (20)        0 2023-05-07 09:19:59.000000 async_pipeline-0.1.1/async_pipeline/
+-rw-r--r--   0 rockey     (501) staff       (20)       56 2023-05-06 07:22:37.000000 async_pipeline-0.1.1/async_pipeline/__init__.py
+drwxr-xr-x   0 rockey     (501) staff       (20)        0 2023-05-07 09:19:59.000000 async_pipeline-0.1.1/async_pipeline/api/
+-rw-r--r--   0 rockey     (501) staff       (20)     1639 2023-05-06 07:56:52.000000 async_pipeline-0.1.1/async_pipeline/api/__init__.py
+-rw-r--r--   0 rockey     (501) staff       (20)      594 2023-05-05 12:53:08.000000 async_pipeline-0.1.1/async_pipeline/api/concat.py
+-rw-r--r--   0 rockey     (501) staff       (20)      557 2023-05-06 07:49:57.000000 async_pipeline-0.1.1/async_pipeline/api/data.py
+drwxr-xr-x   0 rockey     (501) staff       (20)        0 2023-05-07 09:19:59.000000 async_pipeline-0.1.1/async_pipeline/api/distribute/
+-rw-r--r--   0 rockey     (501) staff       (20)      159 2023-05-06 07:56:52.000000 async_pipeline-0.1.1/async_pipeline/api/distribute/__init__.py
+-rw-r--r--   0 rockey     (501) staff       (20)     1230 2023-05-06 07:56:52.000000 async_pipeline-0.1.1/async_pipeline/api/distribute/multiply.py
+-rw-r--r--   0 rockey     (501) staff       (20)     2043 2023-05-06 05:32:24.000000 async_pipeline-0.1.1/async_pipeline/api/distribute/partition.py
+-rw-r--r--   0 rockey     (501) staff       (20)      504 2023-05-05 12:53:08.000000 async_pipeline-0.1.1/async_pipeline/api/flatten.py
+-rw-r--r--   0 rockey     (501) staff       (20)      319 2023-05-06 07:36:58.000000 async_pipeline-0.1.1/async_pipeline/api/result.py
+drwxr-xr-x   0 rockey     (501) staff       (20)        0 2023-05-07 09:19:59.000000 async_pipeline-0.1.1/async_pipeline/api/select/
+-rw-r--r--   0 rockey     (501) staff       (20)      177 2023-05-06 07:56:52.000000 async_pipeline-0.1.1/async_pipeline/api/select/__init__.py
+-rw-r--r--   0 rockey     (501) staff       (20)      205 2023-05-05 12:53:08.000000 async_pipeline-0.1.1/async_pipeline/api/select/each.py
+-rw-r--r--   0 rockey     (501) staff       (20)       68 2023-05-05 12:53:08.000000 async_pipeline-0.1.1/async_pipeline/api/select/map.py
+-rw-r--r--   0 rockey     (501) staff       (20)      201 2023-05-05 12:53:08.000000 async_pipeline-0.1.1/async_pipeline/api/select/peek.py
+drwxr-xr-x   0 rockey     (501) staff       (20)        0 2023-05-07 09:19:59.000000 async_pipeline-0.1.1/async_pipeline/api/where/
+-rw-r--r--   0 rockey     (501) staff       (20)      339 2023-05-06 07:56:52.000000 async_pipeline-0.1.1/async_pipeline/api/where/__init__.py
+-rw-r--r--   0 rockey     (501) staff       (20)      479 2023-05-05 12:53:08.000000 async_pipeline-0.1.1/async_pipeline/api/where/distinct.py
+-rw-r--r--   0 rockey     (501) staff       (20)      494 2023-05-05 12:53:08.000000 async_pipeline-0.1.1/async_pipeline/api/where/duplicate.py
+-rw-r--r--   0 rockey     (501) staff       (20)      280 2023-05-05 12:53:08.000000 async_pipeline-0.1.1/async_pipeline/api/where/filter.py
+-rw-r--r--   0 rockey     (501) staff       (20)      287 2023-05-05 12:53:08.000000 async_pipeline-0.1.1/async_pipeline/api/where/filter_not.py
+-rw-r--r--   0 rockey     (501) staff       (20)      463 2023-05-05 12:53:08.000000 async_pipeline-0.1.1/async_pipeline/api/where/limit.py
+-rw-r--r--   0 rockey     (501) staff       (20)      809 2023-05-06 06:49:53.000000 async_pipeline-0.1.1/async_pipeline/pipe.py
+-rw-r--r--   0 rockey     (501) staff       (20)      624 2023-05-05 12:53:08.000000 async_pipeline-0.1.1/async_pipeline/queue.py
+-rw-r--r--   0 rockey     (501) staff       (20)      103 2023-05-04 06:23:05.000000 async_pipeline-0.1.1/async_pipeline/signal.py
+-rw-r--r--   0 rockey     (501) staff       (20)     2264 2023-05-06 05:32:24.000000 async_pipeline-0.1.1/async_pipeline/stage.py
+drwxr-xr-x   0 rockey     (501) staff       (20)        0 2023-05-07 09:19:59.000000 async_pipeline-0.1.1/async_pipeline.egg-info/
+-rw-r--r--   0 rockey     (501) staff       (20)    10098 2023-05-07 09:19:59.000000 async_pipeline-0.1.1/async_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 rockey     (501) staff       (20)     1292 2023-05-07 09:19:59.000000 async_pipeline-0.1.1/async_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 rockey     (501) staff       (20)        1 2023-05-07 09:19:59.000000 async_pipeline-0.1.1/async_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 rockey     (501) staff       (20)       21 2023-05-07 09:19:59.000000 async_pipeline-0.1.1/async_pipeline.egg-info/top_level.txt
+-rw-r--r--   0 rockey     (501) staff       (20)       38 2023-05-07 09:19:59.000000 async_pipeline-0.1.1/setup.cfg
+-rw-r--r--   0 rockey     (501) staff       (20)     1334 2023-05-07 09:19:42.000000 async_pipeline-0.1.1/setup.py
+drwxr-xr-x   0 rockey     (501) staff       (20)        0 2023-05-07 09:19:59.000000 async_pipeline-0.1.1/tests/
+-rw-r--r--   0 rockey     (501) staff       (20)      240 2023-05-06 06:19:13.000000 async_pipeline-0.1.1/tests/__init__.py
+-rw-r--r--   0 rockey     (501) staff       (20)      122 2023-05-06 06:55:03.000000 async_pipeline-0.1.1/tests/hp_conf.py
+-rw-r--r--   0 rockey     (501) staff       (20)     9437 2023-05-06 07:56:20.000000 async_pipeline-0.1.1/tests/test_complex.py
+-rw-r--r--   0 rockey     (501) staff       (20)     5918 2023-05-07 04:06:20.000000 async_pipeline-0.1.1/tests/test_concat.py
+-rw-r--r--   0 rockey     (501) staff       (20)     2679 2023-05-06 07:56:20.000000 async_pipeline-0.1.1/tests/test_data.py
+-rw-r--r--   0 rockey     (501) staff       (20)     2498 2023-05-06 07:56:19.000000 async_pipeline-0.1.1/tests/test_distinct.py
+-rw-r--r--   0 rockey     (501) staff       (20)     2620 2023-05-06 07:56:19.000000 async_pipeline-0.1.1/tests/test_duplicate.py
+-rw-r--r--   0 rockey     (501) staff       (20)     3223 2023-05-06 07:56:19.000000 async_pipeline-0.1.1/tests/test_each.py
+-rw-r--r--   0 rockey     (501) staff       (20)      930 2023-05-06 07:56:19.000000 async_pipeline-0.1.1/tests/test_exception.py
+-rw-r--r--   0 rockey     (501) staff       (20)     2072 2023-05-06 07:56:20.000000 async_pipeline-0.1.1/tests/test_filter.py
+-rw-r--r--   0 rockey     (501) staff       (20)     2120 2023-05-06 07:56:20.000000 async_pipeline-0.1.1/tests/test_filter_not.py
+-rw-r--r--   0 rockey     (501) staff       (20)     1947 2023-05-06 07:56:19.000000 async_pipeline-0.1.1/tests/test_flatten.py
+-rw-r--r--   0 rockey     (501) staff       (20)     1308 2023-05-06 07:56:20.000000 async_pipeline-0.1.1/tests/test_limit.py
+-rw-r--r--   0 rockey     (501) staff       (20)     2623 2023-05-06 07:56:20.000000 async_pipeline-0.1.1/tests/test_map.py
+-rw-r--r--   0 rockey     (501) staff       (20)     3525 2023-05-06 07:56:20.000000 async_pipeline-0.1.1/tests/test_multiply.py
+-rw-r--r--   0 rockey     (501) staff       (20)     5384 2023-05-06 07:56:20.000000 async_pipeline-0.1.1/tests/test_partition.py
+-rw-r--r--   0 rockey     (501) staff       (20)     3261 2023-05-06 07:56:19.000000 async_pipeline-0.1.1/tests/test_peek.py
```

### Comparing `async_pipeline-0.1.0/LICENSE` & `async_pipeline-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/PKG-INFO` & `async_pipeline-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_pipeline
-Version: 0.1.0
+Version: 0.1.1
 Summary: Async pipeline with functional methods
 Home-page: https://github.com/RockeyDon/async_pipeline
 Author: Rockey Don
 Author-email: bjxdrj@gmail.com
 Keywords: async,pipeline,functional
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `async_pipeline-0.1.0/README.md` & `async_pipeline-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/async_pipeline/pipe.py` & `async_pipeline-0.1.1/async_pipeline/pipe.py`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/async_pipeline/queue.py` & `async_pipeline-0.1.1/async_pipeline/queue.py`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/async_pipeline/stage.py` & `async_pipeline-0.1.1/async_pipeline/stage.py`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/async_pipeline.egg-info/PKG-INFO` & `async_pipeline-0.1.1/async_pipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-pipeline
-Version: 0.1.0
+Version: 0.1.1
 Summary: Async pipeline with functional methods
 Home-page: https://github.com/RockeyDon/async_pipeline
 Author: Rockey Don
 Author-email: bjxdrj@gmail.com
 Keywords: async,pipeline,functional
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `async_pipeline-0.1.0/setup.py` & `async_pipeline-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 from os import path
 
 DIR = path.dirname(path.abspath(__file__))
 with open(path.join(DIR, 'requirements/release.txt')) as f:
     INSTALL_PACKAGES = f.read().splitlines()
 with open(path.join(DIR, 'requirements/test.txt')) as f:
     TEST_PACKAGES = f.read().splitlines()
 with open(path.join(DIR, 'README.md')) as f:
     README = f.read()
 
 setup(
     name='async_pipeline',
-    version='0.1.0',
+    version='0.1.1',
     author='Rockey Don',
     author_email='bjxdrj@gmail.com',
     description="Async pipeline with functional methods",
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/RockeyDon/async_pipeline',
-    packages=['async_pipeline'],
+    packages=find_packages(),
     keywords=['async', 'pipeline', 'functional'],
 
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: MIT License',
```

### Comparing `async_pipeline-0.1.0/tests/test_complex.py` & `async_pipeline-0.1.1/tests/test_complex.py`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/tests/test_concat.py` & `async_pipeline-0.1.1/tests/test_concat.py`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/tests/test_data.py` & `async_pipeline-0.1.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/tests/test_distinct.py` & `async_pipeline-0.1.1/tests/test_distinct.py`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/tests/test_duplicate.py` & `async_pipeline-0.1.1/tests/test_duplicate.py`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/tests/test_each.py` & `async_pipeline-0.1.1/tests/test_each.py`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/tests/test_exception.py` & `async_pipeline-0.1.1/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/tests/test_filter.py` & `async_pipeline-0.1.1/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/tests/test_filter_not.py` & `async_pipeline-0.1.1/tests/test_filter_not.py`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/tests/test_flatten.py` & `async_pipeline-0.1.1/tests/test_flatten.py`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/tests/test_limit.py` & `async_pipeline-0.1.1/tests/test_limit.py`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/tests/test_map.py` & `async_pipeline-0.1.1/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/tests/test_multiply.py` & `async_pipeline-0.1.1/tests/test_multiply.py`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/tests/test_partition.py` & `async_pipeline-0.1.1/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `async_pipeline-0.1.0/tests/test_peek.py` & `async_pipeline-0.1.1/tests/test_peek.py`

 * *Files identical despite different names*

