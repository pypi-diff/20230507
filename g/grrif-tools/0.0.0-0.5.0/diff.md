# Comparing `tmp/grrif_tools-0.0.0.tar.gz` & `tmp/grrif_tools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grrif_tools-0.0.0.tar", last modified: Sun May  7 15:22:44 2023, max compression
+gzip compressed data, was "grrif_tools-0.5.0.tar", last modified: Sun May  7 15:44:55 2023, max compression
```

## Comparing `grrif_tools-0.0.0.tar` & `grrif_tools-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 fetzu      (501) staff       (20)        0 2023-05-07 15:22:44.916744 grrif_tools-0.0.0/
--rw-r--r--   0 fetzu      (501) staff       (20)     3099 2023-05-07 11:10:03.000000 grrif_tools-0.0.0/.gitignore
--rw-r--r--   0 fetzu      (501) staff       (20)     1076 2023-05-07 09:42:56.000000 grrif_tools-0.0.0/LICENSE
--rw-r--r--   0 fetzu      (501) staff       (20)       18 2023-05-07 15:22:37.000000 grrif_tools-0.0.0/MANIFEST.in
--rw-r--r--   0 fetzu      (501) staff       (20)      287 2023-05-07 15:22:44.916600 grrif_tools-0.0.0/PKG-INFO
--rw-r--r--   0 fetzu      (501) staff       (20)      732 2023-05-07 15:20:19.000000 grrif_tools-0.0.0/README.md
-drwxr-xr-x   0 fetzu      (501) staff       (20)        0 2023-05-07 15:22:44.915159 grrif_tools-0.0.0/grrif_tools/
--rw-r--r--   0 fetzu      (501) staff       (20)        0 2023-05-07 13:23:06.000000 grrif_tools-0.0.0/grrif_tools/__init__.py
--rw-r--r--   0 fetzu      (501) staff       (20)     3402 2023-05-07 15:12:24.000000 grrif_tools-0.0.0/grrif_tools/cli.py
--rw-r--r--   0 fetzu      (501) staff       (20)     7312 2023-05-07 15:14:39.000000 grrif_tools-0.0.0/grrif_tools/grrif_archiver.py
-drwxr-xr-x   0 fetzu      (501) staff       (20)        0 2023-05-07 15:22:44.916389 grrif_tools-0.0.0/grrif_tools.egg-info/
--rw-r--r--   0 fetzu      (501) staff       (20)      287 2023-05-07 15:22:44.000000 grrif_tools-0.0.0/grrif_tools.egg-info/PKG-INFO
--rw-r--r--   0 fetzu      (501) staff       (20)      334 2023-05-07 15:22:44.000000 grrif_tools-0.0.0/grrif_tools.egg-info/SOURCES.txt
--rw-r--r--   0 fetzu      (501) staff       (20)        1 2023-05-07 15:22:44.000000 grrif_tools-0.0.0/grrif_tools.egg-info/dependency_links.txt
--rw-r--r--   0 fetzu      (501) staff       (20)       53 2023-05-07 15:22:44.000000 grrif_tools-0.0.0/grrif_tools.egg-info/entry_points.txt
--rw-r--r--   0 fetzu      (501) staff       (20)       55 2023-05-07 15:22:44.000000 grrif_tools-0.0.0/grrif_tools.egg-info/requires.txt
--rw-r--r--   0 fetzu      (501) staff       (20)       12 2023-05-07 15:22:44.000000 grrif_tools-0.0.0/grrif_tools.egg-info/top_level.txt
--rw-r--r--   0 fetzu      (501) staff       (20)       38 2023-05-07 15:22:44.916784 grrif_tools-0.0.0/setup.cfg
--rw-r--r--   0 fetzu      (501) staff       (20)      600 2023-05-07 14:59:59.000000 grrif_tools-0.0.0/setup.py
+drwxr-xr-x   0 fetzu      (501) staff       (20)        0 2023-05-07 15:44:55.800473 grrif_tools-0.5.0/
+-rw-r--r--   0 fetzu      (501) staff       (20)     3099 2023-05-07 11:10:03.000000 grrif_tools-0.5.0/.gitignore
+-rw-r--r--   0 fetzu      (501) staff       (20)     1076 2023-05-07 09:42:56.000000 grrif_tools-0.5.0/LICENSE
+-rw-r--r--   0 fetzu      (501) staff       (20)       18 2023-05-07 15:22:37.000000 grrif_tools-0.5.0/MANIFEST.in
+-rw-r--r--   0 fetzu      (501) staff       (20)     1359 2023-05-07 15:44:55.800268 grrif_tools-0.5.0/PKG-INFO
+-rw-r--r--   0 fetzu      (501) staff       (20)      732 2023-05-07 15:20:19.000000 grrif_tools-0.5.0/README.md
+drwxr-xr-x   0 fetzu      (501) staff       (20)        0 2023-05-07 15:44:55.799115 grrif_tools-0.5.0/grrif_tools/
+-rw-r--r--   0 fetzu      (501) staff       (20)        0 2023-05-07 13:23:06.000000 grrif_tools-0.5.0/grrif_tools/__init__.py
+-rw-r--r--   0 fetzu      (501) staff       (20)     3402 2023-05-07 15:27:48.000000 grrif_tools-0.5.0/grrif_tools/cli.py
+-rw-r--r--   0 fetzu      (501) staff       (20)     7312 2023-05-07 15:14:39.000000 grrif_tools-0.5.0/grrif_tools/grrif_archiver.py
+drwxr-xr-x   0 fetzu      (501) staff       (20)        0 2023-05-07 15:44:55.800083 grrif_tools-0.5.0/grrif_tools.egg-info/
+-rw-r--r--   0 fetzu      (501) staff       (20)     1359 2023-05-07 15:44:55.000000 grrif_tools-0.5.0/grrif_tools.egg-info/PKG-INFO
+-rw-r--r--   0 fetzu      (501) staff       (20)      349 2023-05-07 15:44:55.000000 grrif_tools-0.5.0/grrif_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 fetzu      (501) staff       (20)        1 2023-05-07 15:44:55.000000 grrif_tools-0.5.0/grrif_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 fetzu      (501) staff       (20)       53 2023-05-07 15:44:55.000000 grrif_tools-0.5.0/grrif_tools.egg-info/entry_points.txt
+-rw-r--r--   0 fetzu      (501) staff       (20)       55 2023-05-07 15:44:55.000000 grrif_tools-0.5.0/grrif_tools.egg-info/requires.txt
+-rw-r--r--   0 fetzu      (501) staff       (20)       12 2023-05-07 15:44:55.000000 grrif_tools-0.5.0/grrif_tools.egg-info/top_level.txt
+-rw-r--r--   0 fetzu      (501) staff       (20)      678 2023-05-07 15:43:33.000000 grrif_tools-0.5.0/pyproject.toml
+-rw-r--r--   0 fetzu      (501) staff       (20)       38 2023-05-07 15:44:55.800513 grrif_tools-0.5.0/setup.cfg
+-rw-r--r--   0 fetzu      (501) staff       (20)      600 2023-05-07 15:27:37.000000 grrif_tools-0.5.0/setup.py
```

### Comparing `grrif_tools-0.0.0/.gitignore` & `grrif_tools-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.0.0/LICENSE` & `grrif_tools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.0.0/README.md` & `grrif_tools-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.0.0/grrif_tools/cli.py` & `grrif_tools-0.5.0/grrif_tools/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ### [ GRRIF Tools by Julien 'fetzu' Bono ]
 ## [ IMPORTS ]
 import sys
 import argparse
 from datetime import date, datetime
 
 ## [ CONFIGURATION ]
-__version__ = "0.0.0"
+__version__ = "0.5.0"
 
 ## [ Is CLI even cooler with argparse? ]
 parser = argparse.ArgumentParser(
     description='A set of tools for Cool Cats™. Allows you to archive GRRIF\'s play history and scrobble it to last.fm (upcoming).'
 )
 
 subparsers = parser.add_subparsers(dest='subcommand')
```

### Comparing `grrif_tools-0.0.0/grrif_tools/grrif_archiver.py` & `grrif_tools-0.5.0/grrif_tools/grrif_archiver.py`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.0.0/setup.py` & `grrif_tools-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="grrif_tools",
     description="An unofficial set of tools for Cool Cats™.",
     author="Julien 'fetzu' Bono", 
     url="https://fetzu.ch/",
-    version="0.0.0",
+    version="0.5.0",
     download_url="https://github.com/fetzu/grrif_tools",
     packages=find_packages(include=['grrif_tools','grrif_tools.*']),
     license="License :: OSI Approved :: MIT License",
     install_requires=[
         "Requests==2.30.0",
         "beautifulsoup4==4.11.1",
         "titlecase==2.4",
```

