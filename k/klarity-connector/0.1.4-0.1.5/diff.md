# Comparing `tmp/klarity-connector-0.1.4.tar.gz` & `tmp/klarity-connector-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klarity-connector-0.1.4.tar", last modified: Sat May  6 17:53:35 2023, max compression
+gzip compressed data, was "klarity-connector-0.1.5.tar", last modified: Sun May  7 12:00:08 2023, max compression
```

## Comparing `klarity-connector-0.1.4.tar` & `klarity-connector-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:53:35.332884 klarity-connector-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-06 17:53:23.000000 klarity-connector-0.1.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-06 17:53:35.332884 klarity-connector-0.1.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:53:35.332884 klarity-connector-0.1.4/klarity_connector/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-06 17:53:23.000000 klarity-connector-0.1.4/klarity_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-06 17:53:23.000000 klarity-connector-0.1.4/klarity_connector/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:53:35.332884 klarity-connector-0.1.4/klarity_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-06 17:53:35.000000 klarity-connector-0.1.4/klarity_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-06 17:53:35.000000 klarity-connector-0.1.4/klarity_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 17:53:35.000000 klarity-connector-0.1.4/klarity_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 17:53:35.000000 klarity-connector-0.1.4/klarity_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 17:53:35.000000 klarity-connector-0.1.4/klarity_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 17:53:35.332884 klarity-connector-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-06 17:53:23.000000 klarity-connector-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:00:08.122681 klarity-connector-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 11:59:56.000000 klarity-connector-0.1.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-07 12:00:08.122681 klarity-connector-0.1.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:00:08.118681 klarity-connector-0.1.5/klarity_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-07 11:59:56.000000 klarity-connector-0.1.5/klarity_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-07 11:59:56.000000 klarity-connector-0.1.5/klarity_connector/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 12:00:08.122681 klarity-connector-0.1.5/klarity_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-07 12:00:08.000000 klarity-connector-0.1.5/klarity_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-07 12:00:08.000000 klarity-connector-0.1.5/klarity_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 12:00:08.000000 klarity-connector-0.1.5/klarity_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-07 12:00:08.000000 klarity-connector-0.1.5/klarity_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 12:00:08.000000 klarity-connector-0.1.5/klarity_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 12:00:08.122681 klarity-connector-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-07 11:59:56.000000 klarity-connector-0.1.5/setup.py
```

### Comparing `klarity-connector-0.1.4/LICENSE.md` & `klarity-connector-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `klarity-connector-0.1.4/PKG-INFO` & `klarity-connector-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klarity-connector
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python connector to GraphQL API of Klarity
 Home-page: https://github.com/Kacperek0/klarity-connector
 Author: Kacper Szczepanek
 Author-email: pypi@szczepanek.dev
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -34,14 +34,15 @@
 
 from klarity_connector import KlarityConnector
 
 # Create a connector
 connector = KlarityConnector(
     region='eu'
     api_key='YOUR_API_KEY',
+    billing_period='current' | 'previous' # Current is a default billing period
 )
 
 # Sending GraphQL query
 query = """
     query applications{
         applicationsPaginated(limit: 100, page: 0){
             results{
```

### Comparing `klarity-connector-0.1.4/klarity_connector/connector.py` & `klarity-connector-0.1.5/klarity_connector/connector.py`

 * *Files identical despite different names*

### Comparing `klarity-connector-0.1.4/klarity_connector.egg-info/PKG-INFO` & `klarity-connector-0.1.5/klarity_connector.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klarity-connector
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python connector to GraphQL API of Klarity
 Home-page: https://github.com/Kacperek0/klarity-connector
 Author: Kacper Szczepanek
 Author-email: pypi@szczepanek.dev
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -34,14 +34,15 @@
 
 from klarity_connector import KlarityConnector
 
 # Create a connector
 connector = KlarityConnector(
     region='eu'
     api_key='YOUR_API_KEY',
+    billing_period='current' | 'previous' # Current is a default billing period
 )
 
 # Sending GraphQL query
 query = """
     query applications{
         applicationsPaginated(limit: 100, page: 0){
             results{
```

### Comparing `klarity-connector-0.1.4/setup.py` & `klarity-connector-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'readme.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="klarity-connector",
-    version="0.1.4",
+    version="0.1.5",
     description="Python connector to GraphQL API of Klarity",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Kacperek0/klarity-connector",
     author="Kacper Szczepanek",
     author_email="pypi@szczepanek.dev",
     license="MIT",
```

