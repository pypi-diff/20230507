# Comparing `tmp/mnzipcode-0.0.5.tar.gz` & `tmp/mnzipcode-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnzipcode-0.0.5.tar", last modified: Sun May  7 08:02:50 2023, max compression
+gzip compressed data, was "mnzipcode-0.0.6.tar", last modified: Sun May  7 08:07:07 2023, max compression
```

## Comparing `mnzipcode-0.0.5.tar` & `mnzipcode-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-05-07 08:02:50.767988 mnzipcode-0.0.5/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1034 2023-05-07 08:02:50.767988 mnzipcode-0.0.5/PKG-INFO
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      265 2023-03-23 09:39:39.000000 mnzipcode-0.0.5/README.md
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-05-07 08:02:50.767988 mnzipcode-0.0.5/mnzipcode/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       25 2023-05-07 07:52:13.000000 mnzipcode-0.0.5/mnzipcode/__init__.py
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     3510 2023-05-07 08:02:25.000000 mnzipcode-0.0.5/mnzipcode/mnZipCodes.py
-drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-05-07 08:02:50.767988 mnzipcode-0.0.5/mnzipcode.egg-info/
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1034 2023-05-07 08:02:50.000000 mnzipcode-0.0.5/mnzipcode.egg-info/PKG-INFO
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      196 2023-05-07 08:02:50.000000 mnzipcode-0.0.5/mnzipcode.egg-info/SOURCES.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        1 2023-05-07 08:02:50.000000 mnzipcode-0.0.5/mnzipcode.egg-info/dependency_links.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       10 2023-05-07 08:02:50.000000 mnzipcode-0.0.5/mnzipcode.egg-info/top_level.txt
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       38 2023-05-07 08:02:50.767988 mnzipcode-0.0.5/setup.cfg
--rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1131 2023-05-07 08:00:36.000000 mnzipcode-0.0.5/setup.py
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-05-07 08:07:07.798517 mnzipcode-0.0.6/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1034 2023-05-07 08:07:07.798517 mnzipcode-0.0.6/PKG-INFO
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      265 2023-03-23 09:39:39.000000 mnzipcode-0.0.6/README.md
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-05-07 08:07:07.794516 mnzipcode-0.0.6/mnzipcode/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       25 2023-05-07 07:52:13.000000 mnzipcode-0.0.6/mnzipcode/__init__.py
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)   146710 2023-05-07 08:06:42.000000 mnzipcode-0.0.6/mnzipcode/mnZipCodes.py
+drwxrwxr-x   0 bi11y     (1000) bi11y     (1000)        0 2023-05-07 08:07:07.798517 mnzipcode-0.0.6/mnzipcode.egg-info/
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1034 2023-05-07 08:07:07.000000 mnzipcode-0.0.6/mnzipcode.egg-info/PKG-INFO
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)      196 2023-05-07 08:07:07.000000 mnzipcode-0.0.6/mnzipcode.egg-info/SOURCES.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)        1 2023-05-07 08:07:07.000000 mnzipcode-0.0.6/mnzipcode.egg-info/dependency_links.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       10 2023-05-07 08:07:07.000000 mnzipcode-0.0.6/mnzipcode.egg-info/top_level.txt
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)       38 2023-05-07 08:07:07.798517 mnzipcode-0.0.6/setup.cfg
+-rw-rw-r--   0 bi11y     (1000) bi11y     (1000)     1131 2023-05-07 08:06:49.000000 mnzipcode-0.0.6/setup.py
```

### Comparing `mnzipcode-0.0.5/PKG-INFO` & `mnzipcode-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnzipcode
-Version: 0.0.5
+Version: 0.0.6
 Summary: mnzipcodes is a simple library for querying Mongolian zip codes.
 Author: Bekkage
 Description-Content-Type: text/markdown
 
 
 mnzipcodes is a simple library for querying Mongolian zip codes.
```

### Comparing `mnzipcode-0.0.5/mnzipcode.egg-info/PKG-INFO` & `mnzipcode-0.0.6/mnzipcode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnzipcode
-Version: 0.0.5
+Version: 0.0.6
 Summary: mnzipcodes is a simple library for querying Mongolian zip codes.
 Author: Bekkage
 Description-Content-Type: text/markdown
 
 
 mnzipcodes is a simple library for querying Mongolian zip codes.
```

### Comparing `mnzipcode-0.0.5/setup.py` & `mnzipcode-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools 
 
 setuptools.setup(
   name='mnzipcode',
-  version='0.0.5',
+  version='0.0.6',
   author='Bekkage',
   description='mnzipcodes is a simple library for querying Mongolian zip codes.',
   long_description_content_type= 'text/markdown',
   long_description="""
 mnzipcodes is a simple library for querying Mongolian zip codes.
 
 ### Installation
```

