# Comparing `tmp/grrif_tools-0.6.0.tar.gz` & `tmp/grrif_tools-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grrif_tools-0.6.0.tar", last modified: Sun May  7 20:49:57 2023, max compression
+gzip compressed data, was "grrif_tools-0.6.1.tar", last modified: Sun May  7 21:12:53 2023, max compression
```

## Comparing `grrif_tools-0.6.0.tar` & `grrif_tools-0.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:49:57.690024 grrif_tools-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-07 20:49:50.000000 grrif_tools-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 20:49:50.000000 grrif_tools-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-07 20:49:57.690024 grrif_tools-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-07 20:49:50.000000 grrif_tools-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:49:57.690024 grrif_tools-0.6.0/grrif_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:49:50.000000 grrif_tools-0.6.0/grrif_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-07 20:49:50.000000 grrif_tools-0.6.0/grrif_tools/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-07 20:49:50.000000 grrif_tools-0.6.0/grrif_tools/grrif_archiver.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-07 20:49:50.000000 grrif_tools-0.6.0/grrif_tools/grrif_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:49:57.690024 grrif_tools-0.6.0/grrif_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-07 20:49:57.000000 grrif_tools-0.6.0/grrif_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-07 20:49:57.000000 grrif_tools-0.6.0/grrif_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:49:57.000000 grrif_tools-0.6.0/grrif_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-07 20:49:57.000000 grrif_tools-0.6.0/grrif_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 20:49:57.000000 grrif_tools-0.6.0/grrif_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 20:49:57.000000 grrif_tools-0.6.0/grrif_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-07 20:49:50.000000 grrif_tools-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 20:49:57.690024 grrif_tools-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-07 20:49:50.000000 grrif_tools-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:12:53.754684 grrif_tools-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-07 21:12:48.000000 grrif_tools-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 21:12:48.000000 grrif_tools-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-07 21:12:53.754684 grrif_tools-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-07 21:12:48.000000 grrif_tools-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:12:53.754684 grrif_tools-0.6.1/grrif_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:12:48.000000 grrif_tools-0.6.1/grrif_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-07 21:12:48.000000 grrif_tools-0.6.1/grrif_tools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-07 21:12:48.000000 grrif_tools-0.6.1/grrif_tools/grrif_archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-07 21:12:48.000000 grrif_tools-0.6.1/grrif_tools/grrif_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:12:53.754684 grrif_tools-0.6.1/grrif_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-07 21:12:53.000000 grrif_tools-0.6.1/grrif_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-07 21:12:53.000000 grrif_tools-0.6.1/grrif_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 21:12:53.000000 grrif_tools-0.6.1/grrif_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-07 21:12:53.000000 grrif_tools-0.6.1/grrif_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 21:12:53.000000 grrif_tools-0.6.1/grrif_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 21:12:53.000000 grrif_tools-0.6.1/grrif_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-07 21:12:48.000000 grrif_tools-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 21:12:53.754684 grrif_tools-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-07 21:12:48.000000 grrif_tools-0.6.1/setup.py
```

### Comparing `grrif_tools-0.6.0/LICENSE` & `grrif_tools-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.6.0/PKG-INFO` & `grrif_tools-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grrif_tools
-Version: 0.6.0
+Version: 0.6.1
 Summary: An unofficial set of tools for Cool Cats™.
 Home-page: https://github.com/fetzu/grrif_tools
 Download-URL: https://github.com/fetzu/grrif_tools/releases/latest
 Author: Julien 'fetzu' Bono
 License: MIT License
         
         Copyright (c) 2023 Julien 'fetzu' Bono
```

### Comparing `grrif_tools-0.6.0/README.md` & `grrif_tools-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.6.0/grrif_tools/cli.py` & `grrif_tools-0.6.1/grrif_tools/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ### [ GRRIF Tools by Julien 'fetzu' Bono ]
 ## [ IMPORTS ]
 import sys
 import argparse
 from datetime import date, datetime
 
 ## [ CONFIGURATION ]
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 ## [ Is CLI even cooler with argparse? ]
 parser = argparse.ArgumentParser(
     description="A set of tools for Cool Cats™. Allows you to archive GRRIF's play history and scrobble it to last.fm (upcoming)."
 )
 
 subparsers = parser.add_subparsers(dest="command")
```

### Comparing `grrif_tools-0.6.0/grrif_tools/grrif_archiver.py` & `grrif_tools-0.6.1/grrif_tools/grrif_archiver.py`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.6.0/grrif_tools/grrif_stats.py` & `grrif_tools-0.6.1/grrif_tools/grrif_stats.py`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.6.0/grrif_tools.egg-info/PKG-INFO` & `grrif_tools-0.6.1/grrif_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grrif-tools
-Version: 0.6.0
+Version: 0.6.1
 Summary: An unofficial set of tools for Cool Cats™.
 Home-page: https://github.com/fetzu/grrif_tools
 Download-URL: https://github.com/fetzu/grrif_tools/releases/latest
 Author: Julien 'fetzu' Bono
 License: MIT License
         
         Copyright (c) 2023 Julien 'fetzu' Bono
```

### Comparing `grrif_tools-0.6.0/pyproject.toml` & `grrif_tools-0.6.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "grrif_tools"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
   { name="Julien 'fetzu' Bono" },
 ]
 description = "An unofficial set of tools for Cool Cats™."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
@@ -15,13 +15,13 @@
 ]
 dependencies = [
     "Requests==2.30.0",
     "beautifulsoup4==4.11.1",
     "titlecase==2.4",
 ]
 
-[project.entry-points]
-grrif_tools = { console_scripts= "grrif_tools.cli:main" }
+[project.entry-points.'console_scripts']
+grrif_tools = "grrif_tools.cli:main"
 
 [project.urls]
 "Homepage" = "https://github.com/fetzu/grrif_tools"
 "Bug Tracker" = "https://github.com/fetzu/grrif_tools/issues"
```

### Comparing `grrif_tools-0.6.0/setup.py` & `grrif_tools-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 setup(
     name="grrif_tools",
     description="An unofficial set of tools for Cool Cats™.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Julien 'fetzu' Bono",
     url="https://github.com/fetzu/grrif_tools",
-    version="0.6.0",
+    version="0.6.1",
     download_url="https://github.com/fetzu/grrif_tools/releases/latest",
     packages=find_packages(include=["grrif_tools", "grrif_tools.*"]),
     license="License :: OSI Approved :: MIT License",
     install_requires=[
         "Requests==2.30.0",
         "beautifulsoup4==4.11.1",
         "titlecase==2.4",
```

