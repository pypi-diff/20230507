# Comparing `tmp/steamcrawl-0.1.6.tar.gz` & `tmp/steamcrawl-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steamcrawl-0.1.6.tar", last modified: Sun May  7 13:51:55 2023, max compression
+gzip compressed data, was "steamcrawl-0.1.7.tar", last modified: Sun May  7 13:53:09 2023, max compression
```

## Comparing `steamcrawl-0.1.6.tar` & `steamcrawl-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 13:51:55.677339 steamcrawl-0.1.6/
--rw-rw-rw-   0        0        0     1085 2023-05-06 17:48:49.000000 steamcrawl-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      724 2023-05-07 13:51:55.677339 steamcrawl-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-05-07 13:50:42.000000 steamcrawl-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-07 13:51:55.677339 steamcrawl-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      655 2023-05-07 13:51:33.000000 steamcrawl-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 13:51:55.663376 steamcrawl-0.1.6/steamcrawl/
--rw-rw-rw-   0        0        0       28 2023-05-07 13:37:24.000000 steamcrawl-0.1.6/steamcrawl/__init__.py
--rw-rw-rw-   0        0        0      543 2023-05-05 21:51:45.000000 steamcrawl-0.1.6/steamcrawl/exceptions.py
--rw-rw-rw-   0        0        0    16867 2023-05-07 13:48:49.000000 steamcrawl-0.1.6/steamcrawl/request.py
--rw-rw-rw-   0        0        0        0 2023-05-07 11:37:40.000000 steamcrawl-0.1.6/steamcrawl/requestCounter.py
-drwxrwxrwx   0        0        0        0 2023-05-07 13:51:55.676355 steamcrawl-0.1.6/steamcrawl.egg-info/
--rw-rw-rw-   0        0        0      724 2023-05-07 13:51:55.000000 steamcrawl-0.1.6/steamcrawl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-05-07 13:51:55.000000 steamcrawl-0.1.6/steamcrawl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 13:51:55.000000 steamcrawl-0.1.6/steamcrawl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-07 13:51:55.000000 steamcrawl-0.1.6/steamcrawl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-07 13:51:55.000000 steamcrawl-0.1.6/steamcrawl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 13:53:09.144461 steamcrawl-0.1.7/
+-rw-rw-rw-   0        0        0     1085 2023-05-06 17:48:49.000000 steamcrawl-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      724 2023-05-07 13:53:09.144461 steamcrawl-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-05-07 13:50:42.000000 steamcrawl-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-07 13:53:09.144461 steamcrawl-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      656 2023-05-07 13:52:49.000000 steamcrawl-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 13:53:09.138476 steamcrawl-0.1.7/steamcrawl/
+-rw-rw-rw-   0        0        0       28 2023-05-07 13:37:24.000000 steamcrawl-0.1.7/steamcrawl/__init__.py
+-rw-rw-rw-   0        0        0      543 2023-05-05 21:51:45.000000 steamcrawl-0.1.7/steamcrawl/exceptions.py
+-rw-rw-rw-   0        0        0    16867 2023-05-07 13:48:49.000000 steamcrawl-0.1.7/steamcrawl/request.py
+-rw-rw-rw-   0        0        0        0 2023-05-07 11:37:40.000000 steamcrawl-0.1.7/steamcrawl/requestCounter.py
+drwxrwxrwx   0        0        0        0 2023-05-07 13:53:09.143464 steamcrawl-0.1.7/steamcrawl.egg-info/
+-rw-rw-rw-   0        0        0      724 2023-05-07 13:53:09.000000 steamcrawl-0.1.7/steamcrawl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-07 13:53:09.000000 steamcrawl-0.1.7/steamcrawl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 13:53:09.000000 steamcrawl-0.1.7/steamcrawl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-07 13:53:09.000000 steamcrawl-0.1.7/steamcrawl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-07 13:53:09.000000 steamcrawl-0.1.7/steamcrawl.egg-info/top_level.txt
```

### Comparing `steamcrawl-0.1.6/LICENSE` & `steamcrawl-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `steamcrawl-0.1.6/PKG-INFO` & `steamcrawl-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steamcrawl
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package that helps extract Steam store and community market data as pandas DataFrame for better readabilty and usability.
 Home-page: https://github.com/Hungreeee/steamcrawl
 Author: Hungreeee
 Author-email: hungmnguyen13102003@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `steamcrawl-0.1.6/setup.py` & `steamcrawl-0.1.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='steamcrawl',
-    version='0.1.6',
+    version='0.1.7',
     description='A package that helps extract Steam store and community market data as pandas DataFrame for better readabilty and usability.',
     packages=["steamcrawl"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Hungreeee',
     author_email='hungmnguyen13102003@gmail.com',
     license='MIT',
     url='https://github.com/Hungreeee/steamcrawl',
-    install_requires=['requests', 'pandas', 'seleniumwire'],
+    install_requires=['requests', 'pandas', 'selenium-wire'],
     classifiers = []
 )
```

### Comparing `steamcrawl-0.1.6/steamcrawl/exceptions.py` & `steamcrawl-0.1.7/steamcrawl/exceptions.py`

 * *Files identical despite different names*

### Comparing `steamcrawl-0.1.6/steamcrawl/request.py` & `steamcrawl-0.1.7/steamcrawl/request.py`

 * *Files identical despite different names*

### Comparing `steamcrawl-0.1.6/steamcrawl.egg-info/PKG-INFO` & `steamcrawl-0.1.7/steamcrawl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steamcrawl
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package that helps extract Steam store and community market data as pandas DataFrame for better readabilty and usability.
 Home-page: https://github.com/Hungreeee/steamcrawl
 Author: Hungreeee
 Author-email: hungmnguyen13102003@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

