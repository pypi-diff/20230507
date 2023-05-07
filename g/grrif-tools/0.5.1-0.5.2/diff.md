# Comparing `tmp/grrif_tools-0.5.1.tar.gz` & `tmp/grrif_tools-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grrif_tools-0.5.1.tar", last modified: Sun May  7 16:00:24 2023, max compression
+gzip compressed data, was "grrif_tools-0.5.2.tar", last modified: Sun May  7 19:06:33 2023, max compression
```

## Comparing `grrif_tools-0.5.1.tar` & `grrif_tools-0.5.2.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxr-xr-x   0 fetzu      (501) staff       (20)        0 2023-05-07 16:00:24.173706 grrif_tools-0.5.1/
--rw-r--r--   0 fetzu      (501) staff       (20)     3099 2023-05-07 11:10:03.000000 grrif_tools-0.5.1/.gitignore
--rw-r--r--   0 fetzu      (501) staff       (20)     1076 2023-05-07 09:42:56.000000 grrif_tools-0.5.1/LICENSE
--rw-r--r--   0 fetzu      (501) staff       (20)       18 2023-05-07 15:22:37.000000 grrif_tools-0.5.1/MANIFEST.in
--rw-r--r--   0 fetzu      (501) staff       (20)     1359 2023-05-07 16:00:24.173560 grrif_tools-0.5.1/PKG-INFO
--rw-r--r--   0 fetzu      (501) staff       (20)      732 2023-05-07 15:20:19.000000 grrif_tools-0.5.1/README.md
-drwxr-xr-x   0 fetzu      (501) staff       (20)        0 2023-05-07 16:00:24.172302 grrif_tools-0.5.1/grrif_tools/
--rw-r--r--   0 fetzu      (501) staff       (20)        0 2023-05-07 13:23:06.000000 grrif_tools-0.5.1/grrif_tools/__init__.py
--rw-r--r--   0 fetzu      (501) staff       (20)     3401 2023-05-07 15:58:08.000000 grrif_tools-0.5.1/grrif_tools/cli.py
--rw-r--r--   0 fetzu      (501) staff       (20)     7758 2023-05-07 15:56:52.000000 grrif_tools-0.5.1/grrif_tools/grrif_archiver.py
-drwxr-xr-x   0 fetzu      (501) staff       (20)        0 2023-05-07 16:00:24.173352 grrif_tools-0.5.1/grrif_tools.egg-info/
--rw-r--r--   0 fetzu      (501) staff       (20)     1359 2023-05-07 16:00:24.000000 grrif_tools-0.5.1/grrif_tools.egg-info/PKG-INFO
--rw-r--r--   0 fetzu      (501) staff       (20)      349 2023-05-07 16:00:24.000000 grrif_tools-0.5.1/grrif_tools.egg-info/SOURCES.txt
--rw-r--r--   0 fetzu      (501) staff       (20)        1 2023-05-07 16:00:24.000000 grrif_tools-0.5.1/grrif_tools.egg-info/dependency_links.txt
--rw-r--r--   0 fetzu      (501) staff       (20)       53 2023-05-07 16:00:24.000000 grrif_tools-0.5.1/grrif_tools.egg-info/entry_points.txt
--rw-r--r--   0 fetzu      (501) staff       (20)       55 2023-05-07 16:00:24.000000 grrif_tools-0.5.1/grrif_tools.egg-info/requires.txt
--rw-r--r--   0 fetzu      (501) staff       (20)       12 2023-05-07 16:00:24.000000 grrif_tools-0.5.1/grrif_tools.egg-info/top_level.txt
--rw-r--r--   0 fetzu      (501) staff       (20)      678 2023-05-07 15:58:03.000000 grrif_tools-0.5.1/pyproject.toml
--rw-r--r--   0 fetzu      (501) staff       (20)       38 2023-05-07 16:00:24.173757 grrif_tools-0.5.1/setup.cfg
--rw-r--r--   0 fetzu      (501) staff       (20)      600 2023-05-07 15:57:58.000000 grrif_tools-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:06:33.595787 grrif_tools-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-07 19:06:27.000000 grrif_tools-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 19:06:27.000000 grrif_tools-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-07 19:06:33.595787 grrif_tools-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-07 19:06:27.000000 grrif_tools-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:06:33.595787 grrif_tools-0.5.2/grrif_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 19:06:27.000000 grrif_tools-0.5.2/grrif_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-07 19:06:27.000000 grrif_tools-0.5.2/grrif_tools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-05-07 19:06:27.000000 grrif_tools-0.5.2/grrif_tools/grrif_archiver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:06:33.595787 grrif_tools-0.5.2/grrif_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-07 19:06:33.000000 grrif_tools-0.5.2/grrif_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-07 19:06:33.000000 grrif_tools-0.5.2/grrif_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 19:06:33.000000 grrif_tools-0.5.2/grrif_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-07 19:06:33.000000 grrif_tools-0.5.2/grrif_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 19:06:33.000000 grrif_tools-0.5.2/grrif_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 19:06:33.000000 grrif_tools-0.5.2/grrif_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 19:06:33.595787 grrif_tools-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-07 19:06:27.000000 grrif_tools-0.5.2/setup.py
```

### Comparing `grrif_tools-0.5.1/LICENSE` & `grrif_tools-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.5.1/README.md` & `grrif_tools-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `grrif_tools-0.5.1/grrif_tools/cli.py` & `grrif_tools-0.5.2/grrif_tools/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ### [ GRRIF Tools by Julien 'fetzu' Bono ]
 ## [ IMPORTS ]
 import sys
 import argparse
 from datetime import date, datetime
 
 ## [ CONFIGURATION ]
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 ## [ Is CLI even cooler with argparse? ]
 parser = argparse.ArgumentParser(
     description="A set of tools for Cool Cats™. Allows you to archive GRRIF's play history and scrobble it to last.fm (upcoming)."
 )
 
 subparsers = parser.add_subparsers(dest="subcommand")
```

### Comparing `grrif_tools-0.5.1/grrif_tools/grrif_archiver.py` & `grrif_tools-0.5.2/grrif_tools/grrif_archiver.py`

 * *Files identical despite different names*

