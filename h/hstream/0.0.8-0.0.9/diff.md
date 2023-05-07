# Comparing `tmp/hstream-0.0.8.tar.gz` & `tmp/hstream-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstream-0.0.8.tar", last modified: Thu Nov 10 08:16:10 2022, max compression
+gzip compressed data, was "hstream-0.0.9.tar", last modified: Thu Nov 10 08:17:21 2022, max compression
```

## Comparing `hstream-0.0.8.tar` & `hstream-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2022-11-10 08:16:10.373987 hstream-0.0.8/
--rw-r--r--   0 conrad     (501) staff       (20)     2068 2022-11-10 08:16:10.373861 hstream-0.0.8/PKG-INFO
--rw-r--r--   0 conrad     (501) staff       (20)     1649 2022-11-10 08:10:39.000000 hstream-0.0.8/README
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2022-11-10 08:16:10.371243 hstream-0.0.8/hstream.egg-info/
--rw-r--r--   0 conrad     (501) staff       (20)     2068 2022-11-10 08:16:10.000000 hstream-0.0.8/hstream.egg-info/PKG-INFO
--rw-r--r--   0 conrad     (501) staff       (20)      413 2022-11-10 08:16:10.000000 hstream-0.0.8/hstream.egg-info/SOURCES.txt
--rw-r--r--   0 conrad     (501) staff       (20)        1 2022-11-10 08:16:10.000000 hstream-0.0.8/hstream.egg-info/dependency_links.txt
--rw-r--r--   0 conrad     (501) staff       (20)       51 2022-11-10 08:16:10.000000 hstream-0.0.8/hstream.egg-info/entry_points.txt
--rw-r--r--   0 conrad     (501) staff       (20)      126 2022-11-10 08:16:10.000000 hstream-0.0.8/hstream.egg-info/requires.txt
--rw-r--r--   0 conrad     (501) staff       (20)       12 2022-11-10 08:16:10.000000 hstream-0.0.8/hstream.egg-info/top_level.txt
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2022-11-10 08:16:10.373102 hstream-0.0.8/hyperstream/
--rw-r--r--   0 conrad     (501) staff       (20)       28 2022-11-10 06:45:33.000000 hstream-0.0.8/hyperstream/__init__.py
--rw-r--r--   0 conrad     (501) staff       (20)       61 2022-11-10 06:58:34.000000 hstream-0.0.8/hyperstream/__main__.py
--rw-r--r--   0 conrad     (501) staff       (20)    12112 2022-11-10 05:45:41.000000 hstream-0.0.8/hyperstream/components.py
--rw-r--r--   0 conrad     (501) staff       (20)     1799 2022-11-09 12:51:35.000000 hstream-0.0.8/hyperstream/hstag.py
--rw-r--r--   0 conrad     (501) staff       (20)    15375 2022-11-10 07:38:29.000000 hstream-0.0.8/hyperstream/hyperstream.py
--rw-r--r--   0 conrad     (501) staff       (20)      457 2022-11-10 06:49:13.000000 hstream-0.0.8/hyperstream/runner.py
-drwxr-xr-x   0 conrad     (501) staff       (20)        0 2022-11-10 08:16:10.373522 hstream-0.0.8/hyperstream/templates/
--rw-r--r--   0 conrad     (501) staff       (20)      498 2022-11-10 05:07:06.000000 hstream-0.0.8/hyperstream/templates/header.html
--rw-r--r--   0 conrad     (501) staff       (20)      797 2022-11-10 03:39:04.000000 hstream-0.0.8/hyperstream/templates/main.html
--rw-r--r--   0 conrad     (501) staff       (20)       38 2022-11-10 08:16:10.374022 hstream-0.0.8/setup.cfg
--rw-r--r--   0 conrad     (501) staff       (20)     1146 2022-11-10 08:16:04.000000 hstream-0.0.8/setup.py
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2022-11-10 08:17:21.510389 hstream-0.0.9/
+-rw-r--r--   0 conrad     (501) staff       (20)     2069 2022-11-10 08:17:21.510231 hstream-0.0.9/PKG-INFO
+-rw-r--r--   0 conrad     (501) staff       (20)     1650 2022-11-10 08:17:04.000000 hstream-0.0.9/README
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2022-11-10 08:17:21.507982 hstream-0.0.9/hstream.egg-info/
+-rw-r--r--   0 conrad     (501) staff       (20)     2069 2022-11-10 08:17:21.000000 hstream-0.0.9/hstream.egg-info/PKG-INFO
+-rw-r--r--   0 conrad     (501) staff       (20)      413 2022-11-10 08:17:21.000000 hstream-0.0.9/hstream.egg-info/SOURCES.txt
+-rw-r--r--   0 conrad     (501) staff       (20)        1 2022-11-10 08:17:21.000000 hstream-0.0.9/hstream.egg-info/dependency_links.txt
+-rw-r--r--   0 conrad     (501) staff       (20)       51 2022-11-10 08:17:21.000000 hstream-0.0.9/hstream.egg-info/entry_points.txt
+-rw-r--r--   0 conrad     (501) staff       (20)      126 2022-11-10 08:17:21.000000 hstream-0.0.9/hstream.egg-info/requires.txt
+-rw-r--r--   0 conrad     (501) staff       (20)       12 2022-11-10 08:17:21.000000 hstream-0.0.9/hstream.egg-info/top_level.txt
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2022-11-10 08:17:21.509493 hstream-0.0.9/hyperstream/
+-rw-r--r--   0 conrad     (501) staff       (20)       28 2022-11-10 06:45:33.000000 hstream-0.0.9/hyperstream/__init__.py
+-rw-r--r--   0 conrad     (501) staff       (20)       61 2022-11-10 06:58:34.000000 hstream-0.0.9/hyperstream/__main__.py
+-rw-r--r--   0 conrad     (501) staff       (20)    12112 2022-11-10 05:45:41.000000 hstream-0.0.9/hyperstream/components.py
+-rw-r--r--   0 conrad     (501) staff       (20)     1799 2022-11-09 12:51:35.000000 hstream-0.0.9/hyperstream/hstag.py
+-rw-r--r--   0 conrad     (501) staff       (20)    15375 2022-11-10 07:38:29.000000 hstream-0.0.9/hyperstream/hyperstream.py
+-rw-r--r--   0 conrad     (501) staff       (20)      457 2022-11-10 06:49:13.000000 hstream-0.0.9/hyperstream/runner.py
+drwxr-xr-x   0 conrad     (501) staff       (20)        0 2022-11-10 08:17:21.509942 hstream-0.0.9/hyperstream/templates/
+-rw-r--r--   0 conrad     (501) staff       (20)      498 2022-11-10 05:07:06.000000 hstream-0.0.9/hyperstream/templates/header.html
+-rw-r--r--   0 conrad     (501) staff       (20)      797 2022-11-10 03:39:04.000000 hstream-0.0.9/hyperstream/templates/main.html
+-rw-r--r--   0 conrad     (501) staff       (20)       38 2022-11-10 08:17:21.510425 hstream-0.0.9/setup.cfg
+-rw-r--r--   0 conrad     (501) staff       (20)     1146 2022-11-10 08:17:10.000000 hstream-0.0.9/setup.py
```

### Comparing `hstream-0.0.8/PKG-INFO` & `hstream-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstream
-Version: 0.0.8
+Version: 0.0.9
 Summary: Create python webapps with ease
 Home-page: http://packages.python.org/hyperstream
 Author: Conrad Bezuidenhout
 Author-email: conradbez1@gmail.com
 License: BSD
 Keywords: streamlit htmx fastapi
 Classifier: Development Status :: 3 - Alpha
@@ -24,15 +24,15 @@
 
 ```
 # main.py
 
 from hyperstream import hs
 
 hs.text_input('What's your name?', default_value = 'friend')
-hs.markdown(f"Welcome {visitor_name})
+hs.markdown(f"Welcome {visitor_name}")
 ```
 
 `python -m hstream main.py`
 
 ![hstream demo](docs/hello_hstream.png)
 
 # Motivation
```

### Comparing `hstream-0.0.8/README` & `hstream-0.0.9/README`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ```
 # main.py
 
 from hyperstream import hs
 
 hs.text_input('What's your name?', default_value = 'friend')
-hs.markdown(f"Welcome {visitor_name})
+hs.markdown(f"Welcome {visitor_name}")
 ```
 
 `python -m hstream main.py`
 
 ![hstream demo](docs/hello_hstream.png)
 
 # Motivation
```

### Comparing `hstream-0.0.8/hstream.egg-info/PKG-INFO` & `hstream-0.0.9/hstream.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstream
-Version: 0.0.8
+Version: 0.0.9
 Summary: Create python webapps with ease
 Home-page: http://packages.python.org/hyperstream
 Author: Conrad Bezuidenhout
 Author-email: conradbez1@gmail.com
 License: BSD
 Keywords: streamlit htmx fastapi
 Classifier: Development Status :: 3 - Alpha
@@ -24,15 +24,15 @@
 
 ```
 # main.py
 
 from hyperstream import hs
 
 hs.text_input('What's your name?', default_value = 'friend')
-hs.markdown(f"Welcome {visitor_name})
+hs.markdown(f"Welcome {visitor_name}")
 ```
 
 `python -m hstream main.py`
 
 ![hstream demo](docs/hello_hstream.png)
 
 # Motivation
```

### Comparing `hstream-0.0.8/hyperstream/components.py` & `hstream-0.0.9/hyperstream/components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.0.8/hyperstream/hstag.py` & `hstream-0.0.9/hyperstream/hstag.py`

 * *Files identical despite different names*

### Comparing `hstream-0.0.8/hyperstream/hyperstream.py` & `hstream-0.0.9/hyperstream/hyperstream.py`

 * *Files identical despite different names*

### Comparing `hstream-0.0.8/hyperstream/templates/main.html` & `hstream-0.0.9/hyperstream/templates/main.html`

 * *Files identical despite different names*

### Comparing `hstream-0.0.8/setup.py` & `hstream-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "hstream",
-    version = "0.0.8",
+    version = "0.0.9",
     author = "Conrad Bezuidenhout",
     author_email = "conradbez1@gmail.com",
     description = ("Create python webapps with ease"),
     license = "BSD",
     keywords = "streamlit htmx fastapi",
     url = "http://packages.python.org/hyperstream",
     long_description=read('README'),
```

