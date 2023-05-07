# Comparing `tmp/pyghs-0.2.2.tar.gz` & `tmp/pyghs-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyghs-0.2.2.tar", last modified: Thu May  4 10:36:52 2023, max compression
+gzip compressed data, was "pyghs-0.2.3.tar", last modified: Sun May  7 15:30:30 2023, max compression
```

## Comparing `pyghs-0.2.2.tar` & `pyghs-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-05-04 10:36:52.698815 pyghs-0.2.2/
--rw-r--r--   0 chaoying   (501) staff       (20)     1108 2023-05-04 10:36:52.698666 pyghs-0.2.2/PKG-INFO
--rw-r--r--   0 chaoying   (501) staff       (20)      497 2023-05-03 11:47:43.000000 pyghs-0.2.2/README.md
-drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-05-04 10:36:52.696771 pyghs-0.2.2/ghs/
--rw-r--r--   0 chaoying   (501) staff       (20)       94 2023-05-03 11:18:07.000000 pyghs-0.2.2/ghs/__init__.py
--rw-r--r--   0 chaoying   (501) staff       (20)     4421 2023-05-04 09:50:01.000000 pyghs-0.2.2/ghs/async_storage.py
--rw-r--r--   0 chaoying   (501) staff       (20)     1552 2023-05-04 10:19:54.000000 pyghs-0.2.2/ghs/config.py
--rw-r--r--   0 chaoying   (501) staff       (20)     4066 2023-05-04 09:50:01.000000 pyghs-0.2.2/ghs/storage.py
-drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-05-04 10:36:52.697559 pyghs-0.2.2/pyghs.egg-info/
--rw-r--r--   0 chaoying   (501) staff       (20)     1108 2023-05-04 10:36:52.000000 pyghs-0.2.2/pyghs.egg-info/PKG-INFO
--rw-r--r--   0 chaoying   (501) staff       (20)      284 2023-05-04 10:36:52.000000 pyghs-0.2.2/pyghs.egg-info/SOURCES.txt
--rw-r--r--   0 chaoying   (501) staff       (20)        1 2023-05-04 10:36:52.000000 pyghs-0.2.2/pyghs.egg-info/dependency_links.txt
--rw-r--r--   0 chaoying   (501) staff       (20)       63 2023-05-04 10:36:52.000000 pyghs-0.2.2/pyghs.egg-info/requires.txt
--rw-r--r--   0 chaoying   (501) staff       (20)        4 2023-05-04 10:36:52.000000 pyghs-0.2.2/pyghs.egg-info/top_level.txt
--rw-r--r--   0 chaoying   (501) staff       (20)      952 2023-05-04 10:36:40.000000 pyghs-0.2.2/pyproject.toml
--rw-r--r--   0 chaoying   (501) staff       (20)       38 2023-05-04 10:36:52.698855 pyghs-0.2.2/setup.cfg
-drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-05-04 10:36:52.698183 pyghs-0.2.2/tests/
--rw-r--r--   0 chaoying   (501) staff       (20)      691 2023-05-03 11:37:33.000000 pyghs-0.2.2/tests/test_async_storage.py
--rw-r--r--   0 chaoying   (501) staff       (20)      587 2023-05-03 11:49:01.000000 pyghs-0.2.2/tests/test_storage.py
+drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-05-07 15:30:30.516540 pyghs-0.2.3/
+-rw-r--r--   0 chaoying   (501) staff       (20)     1001 2023-05-07 15:30:30.516384 pyghs-0.2.3/PKG-INFO
+-rw-r--r--   0 chaoying   (501) staff       (20)      497 2023-05-03 11:47:43.000000 pyghs-0.2.3/README.md
+drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-05-07 15:30:30.514431 pyghs-0.2.3/ghs/
+-rw-r--r--   0 chaoying   (501) staff       (20)       94 2023-05-03 11:18:07.000000 pyghs-0.2.3/ghs/__init__.py
+-rw-r--r--   0 chaoying   (501) staff       (20)     4421 2023-05-04 09:50:01.000000 pyghs-0.2.3/ghs/async_storage.py
+-rw-r--r--   0 chaoying   (501) staff       (20)     1552 2023-05-04 10:19:54.000000 pyghs-0.2.3/ghs/config.py
+-rw-r--r--   0 chaoying   (501) staff       (20)     4066 2023-05-04 09:50:01.000000 pyghs-0.2.3/ghs/storage.py
+drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-05-07 15:30:30.515410 pyghs-0.2.3/pyghs.egg-info/
+-rw-r--r--   0 chaoying   (501) staff       (20)     1001 2023-05-07 15:30:30.000000 pyghs-0.2.3/pyghs.egg-info/PKG-INFO
+-rw-r--r--   0 chaoying   (501) staff       (20)      284 2023-05-07 15:30:30.000000 pyghs-0.2.3/pyghs.egg-info/SOURCES.txt
+-rw-r--r--   0 chaoying   (501) staff       (20)        1 2023-05-07 15:30:30.000000 pyghs-0.2.3/pyghs.egg-info/dependency_links.txt
+-rw-r--r--   0 chaoying   (501) staff       (20)       63 2023-05-07 15:30:30.000000 pyghs-0.2.3/pyghs.egg-info/requires.txt
+-rw-r--r--   0 chaoying   (501) staff       (20)        4 2023-05-07 15:30:30.000000 pyghs-0.2.3/pyghs.egg-info/top_level.txt
+-rw-r--r--   0 chaoying   (501) staff       (20)      855 2023-05-07 15:29:57.000000 pyghs-0.2.3/pyproject.toml
+-rw-r--r--   0 chaoying   (501) staff       (20)       38 2023-05-07 15:30:30.516585 pyghs-0.2.3/setup.cfg
+drwxr-xr-x   0 chaoying   (501) staff       (20)        0 2023-05-07 15:30:30.516047 pyghs-0.2.3/tests/
+-rw-r--r--   0 chaoying   (501) staff       (20)      691 2023-05-03 11:37:33.000000 pyghs-0.2.3/tests/test_async_storage.py
+-rw-r--r--   0 chaoying   (501) staff       (20)      587 2023-05-03 11:49:01.000000 pyghs-0.2.3/tests/test_storage.py
```

### Comparing `pyghs-0.2.2/PKG-INFO` & `pyghs-0.2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: pyghs
-Version: 0.2.2
+Version: 0.2.3
 Summary: Storage csv file in github repository.
 Author-email: Chaoying <chaoying2022@gmail.com>
 License: MIT
 Keywords: github,storage,pandas
-Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # GHS
 
 Storage csv file in github repository.
 
 ## Installation
```

### Comparing `pyghs-0.2.2/ghs/async_storage.py` & `pyghs-0.2.3/ghs/async_storage.py`

 * *Files identical despite different names*

### Comparing `pyghs-0.2.2/ghs/config.py` & `pyghs-0.2.3/ghs/config.py`

 * *Files identical despite different names*

### Comparing `pyghs-0.2.2/ghs/storage.py` & `pyghs-0.2.3/ghs/storage.py`

 * *Files identical despite different names*

### Comparing `pyghs-0.2.2/pyghs.egg-info/PKG-INFO` & `pyghs-0.2.3/pyghs.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: pyghs
-Version: 0.2.2
+Version: 0.2.3
 Summary: Storage csv file in github repository.
 Author-email: Chaoying <chaoying2022@gmail.com>
 License: MIT
 Keywords: github,storage,pandas
-Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # GHS
 
 Storage csv file in github repository.
 
 ## Installation
```

### Comparing `pyghs-0.2.2/pyproject.toml` & `pyghs-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,33 +4,31 @@
 dev = [
     "pytest-asyncio>=0.21.0",
     "pytest>=7.3.1",
 ]
 
 [project]
 name = "pyghs"
-version = "0.2.2"
+version = "0.2.3"
 description = "Storage csv file in github repository."
 authors = [
     {name = "Chaoying", email = "chaoying2022@gmail.com"},
 ]
 dependencies = [
     "aiohttp>=3.8.4",
     "pandas>=2.0.1",
     "dynaconf>=3.1.12",
     "requests>=2.29.0",
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = {text = "MIT"}
 readme = "README.md"
 keywords = ["github", "storage", "pandas"]
 classifiers = [
-    "Topic :: Software Development :: Build Tools",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.pytest.ini_options]
```

### Comparing `pyghs-0.2.2/tests/test_async_storage.py` & `pyghs-0.2.3/tests/test_async_storage.py`

 * *Files identical despite different names*

### Comparing `pyghs-0.2.2/tests/test_storage.py` & `pyghs-0.2.3/tests/test_storage.py`

 * *Files identical despite different names*

