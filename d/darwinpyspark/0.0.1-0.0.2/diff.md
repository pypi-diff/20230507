# Comparing `tmp/darwinpyspark-0.0.1.tar.gz` & `tmp/darwinpyspark-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "darwinpyspark-0.0.1.tar", last modified: Sun May  7 11:04:55 2023, max compression
+gzip compressed data, was "darwinpyspark-0.0.2.tar", last modified: Sun May  7 12:06:02 2023, max compression
```

## Comparing `darwinpyspark-0.0.1.tar` & `darwinpyspark-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-05-07 11:04:55.638276 darwinpyspark-0.0.1/
--rw-r--r--   0 harry      (501) staff       (20)     1063 2023-05-07 11:04:10.000000 darwinpyspark-0.0.1/LICENSE
--rw-r--r--   0 harry      (501) staff       (20)     2417 2023-05-07 11:04:55.638111 darwinpyspark-0.0.1/PKG-INFO
--rw-r--r--   0 harry      (501) staff       (20)     2033 2023-05-07 11:04:34.000000 darwinpyspark-0.0.1/README.md
-drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-05-07 11:04:55.637967 darwinpyspark-0.0.1/darwinpyspark.egg-info/
--rw-r--r--   0 harry      (501) staff       (20)     2417 2023-05-07 11:04:55.000000 darwinpyspark-0.0.1/darwinpyspark.egg-info/PKG-INFO
--rw-r--r--   0 harry      (501) staff       (20)      210 2023-05-07 11:04:55.000000 darwinpyspark-0.0.1/darwinpyspark.egg-info/SOURCES.txt
--rw-r--r--   0 harry      (501) staff       (20)        1 2023-05-07 11:04:55.000000 darwinpyspark-0.0.1/darwinpyspark.egg-info/dependency_links.txt
--rw-r--r--   0 harry      (501) staff       (20)        9 2023-05-07 11:04:55.000000 darwinpyspark-0.0.1/darwinpyspark.egg-info/requires.txt
--rw-r--r--   0 harry      (501) staff       (20)        1 2023-05-07 11:04:55.000000 darwinpyspark-0.0.1/darwinpyspark.egg-info/top_level.txt
--rw-r--r--   0 harry      (501) staff       (20)       38 2023-05-07 11:04:55.638322 darwinpyspark-0.0.1/setup.cfg
--rw-r--r--   0 harry      (501) staff       (20)      548 2023-05-07 11:02:29.000000 darwinpyspark-0.0.1/setup.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-05-07 12:06:02.099287 darwinpyspark-0.0.2/
+-rw-r--r--   0 harry      (501) staff       (20)     1063 2023-05-07 11:04:10.000000 darwinpyspark-0.0.2/LICENSE
+-rw-r--r--   0 harry      (501) staff       (20)     2417 2023-05-07 12:06:02.099167 darwinpyspark-0.0.2/PKG-INFO
+-rw-r--r--   0 harry      (501) staff       (20)     2033 2023-05-07 11:04:34.000000 darwinpyspark-0.0.2/README.md
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-05-07 12:06:02.098208 darwinpyspark-0.0.2/darwinpyspark/
+-rw-r--r--   0 harry      (501) staff       (20)       40 2023-04-26 09:11:11.000000 darwinpyspark-0.0.2/darwinpyspark/__init__.py
+-rw-r--r--   0 harry      (501) staff       (20)     8554 2023-05-04 16:21:40.000000 darwinpyspark-0.0.2/darwinpyspark/darwinpyspark.py
+drwxr-xr-x   0 harry      (501) staff       (20)        0 2023-05-07 12:06:02.099005 darwinpyspark-0.0.2/darwinpyspark.egg-info/
+-rw-r--r--   0 harry      (501) staff       (20)     2417 2023-05-07 12:06:02.000000 darwinpyspark-0.0.2/darwinpyspark.egg-info/PKG-INFO
+-rw-r--r--   0 harry      (501) staff       (20)      267 2023-05-07 12:06:02.000000 darwinpyspark-0.0.2/darwinpyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 harry      (501) staff       (20)        1 2023-05-07 12:06:02.000000 darwinpyspark-0.0.2/darwinpyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 harry      (501) staff       (20)        9 2023-05-07 12:06:02.000000 darwinpyspark-0.0.2/darwinpyspark.egg-info/requires.txt
+-rw-r--r--   0 harry      (501) staff       (20)       14 2023-05-07 12:06:02.000000 darwinpyspark-0.0.2/darwinpyspark.egg-info/top_level.txt
+-rw-r--r--   0 harry      (501) staff       (20)       38 2023-05-07 12:06:02.099340 darwinpyspark-0.0.2/setup.cfg
+-rw-r--r--   0 harry      (501) staff       (20)      548 2023-05-07 12:03:18.000000 darwinpyspark-0.0.2/setup.py
```

### Comparing `darwinpyspark-0.0.1/LICENSE` & `darwinpyspark-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `darwinpyspark-0.0.1/PKG-INFO` & `darwinpyspark-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darwinpyspark
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for interacting with the V7 platform via Pyspark
 Home-page: https://github.com/v7labs/darwinpyspark
 Author: Harry Hands
 Author-email: harry.hands@v7labs.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `darwinpyspark-0.0.1/README.md` & `darwinpyspark-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `darwinpyspark-0.0.1/darwinpyspark.egg-info/PKG-INFO` & `darwinpyspark-0.0.2/darwinpyspark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darwinpyspark
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for interacting with the V7 platform via Pyspark
 Home-page: https://github.com/v7labs/darwinpyspark
 Author: Harry Hands
 Author-email: harry.hands@v7labs.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `darwinpyspark-0.0.1/setup.py` & `darwinpyspark-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="darwinpyspark",
-    version="0.0.1",
+    version="0.0.2",
     author="Harry Hands",
     author_email="harry.hands@v7labs.com",
     description="A package for interacting with the V7 platform via Pyspark",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/v7labs/darwinpyspark",
     packages=find_packages(),
```

