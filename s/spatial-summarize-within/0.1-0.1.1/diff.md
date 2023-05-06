# Comparing `tmp/spatial_summarize_within-0.1.tar.gz` & `tmp/spatial_summarize_within-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatial_summarize_within-0.1.tar", last modified: Sat May  6 21:27:46 2023, max compression
+gzip compressed data, was "spatial_summarize_within-0.1.1.tar", last modified: Sat May  6 23:03:24 2023, max compression
```

## Comparing `spatial_summarize_within-0.1.tar` & `spatial_summarize_within-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-06 21:27:46.332877 spatial_summarize_within-0.1/
--rw-r--r--   0 Kenne      (501) staff       (20)       66 2023-05-06 21:27:46.332755 spatial_summarize_within-0.1/PKG-INFO
--rw-r--r--   0 Kenne      (501) staff       (20)       38 2023-05-06 21:27:46.332913 spatial_summarize_within-0.1/setup.cfg
--rw-r--r--   0 Kenne      (501) staff       (20)      250 2023-05-06 21:13:30.000000 spatial_summarize_within-0.1/setup.py
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-06 21:27:46.332024 spatial_summarize_within-0.1/spatial_summarize_within/
--rw-r--r--   0 Kenne      (501) staff       (20)        0 2023-05-06 20:55:18.000000 spatial_summarize_within-0.1/spatial_summarize_within/__init__.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2116 2023-05-06 20:55:51.000000 spatial_summarize_within-0.1/spatial_summarize_within/summarize within.py
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-06 21:27:46.332593 spatial_summarize_within-0.1/spatial_summarize_within.egg-info/
--rw-r--r--   0 Kenne      (501) staff       (20)       66 2023-05-06 21:27:46.000000 spatial_summarize_within-0.1/spatial_summarize_within.egg-info/PKG-INFO
--rw-r--r--   0 Kenne      (501) staff       (20)      329 2023-05-06 21:27:46.000000 spatial_summarize_within-0.1/spatial_summarize_within.egg-info/SOURCES.txt
--rw-r--r--   0 Kenne      (501) staff       (20)        1 2023-05-06 21:27:46.000000 spatial_summarize_within-0.1/spatial_summarize_within.egg-info/dependency_links.txt
--rw-r--r--   0 Kenne      (501) staff       (20)       37 2023-05-06 21:27:46.000000 spatial_summarize_within-0.1/spatial_summarize_within.egg-info/requires.txt
--rw-r--r--   0 Kenne      (501) staff       (20)       25 2023-05-06 21:27:46.000000 spatial_summarize_within-0.1/spatial_summarize_within.egg-info/top_level.txt
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-06 23:03:24.663974 spatial_summarize_within-0.1.1/
+-rw-r--r--   0 Kenne      (501) staff       (20)     1076 2023-05-06 22:57:53.000000 spatial_summarize_within-0.1.1/LICENSE
+-rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-06 23:03:24.663870 spatial_summarize_within-0.1.1/PKG-INFO
+-rw-r--r--   0 Kenne      (501) staff       (20)     2188 2023-05-06 22:57:53.000000 spatial_summarize_within-0.1.1/README.md
+-rw-r--r--   0 Kenne      (501) staff       (20)       38 2023-05-06 23:03:24.664008 spatial_summarize_within-0.1.1/setup.cfg
+-rw-r--r--   0 Kenne      (501) staff       (20)      252 2023-05-06 22:58:09.000000 spatial_summarize_within-0.1.1/setup.py
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-06 23:03:24.663189 spatial_summarize_within-0.1.1/spatial_summarize_within/
+-rw-r--r--   0 Kenne      (501) staff       (20)       46 2023-05-06 23:00:41.000000 spatial_summarize_within-0.1.1/spatial_summarize_within/__init__.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2116 2023-05-06 20:55:51.000000 spatial_summarize_within-0.1.1/spatial_summarize_within/summarize_within.py
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-05-06 23:03:24.663734 spatial_summarize_within-0.1.1/spatial_summarize_within.egg-info/
+-rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-05-06 23:03:24.000000 spatial_summarize_within-0.1.1/spatial_summarize_within.egg-info/PKG-INFO
+-rw-r--r--   0 Kenne      (501) staff       (20)      347 2023-05-06 23:03:24.000000 spatial_summarize_within-0.1.1/spatial_summarize_within.egg-info/SOURCES.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)        1 2023-05-06 23:03:24.000000 spatial_summarize_within-0.1.1/spatial_summarize_within.egg-info/dependency_links.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)       37 2023-05-06 23:03:24.000000 spatial_summarize_within-0.1.1/spatial_summarize_within.egg-info/requires.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)       25 2023-05-06 23:03:24.000000 spatial_summarize_within-0.1.1/spatial_summarize_within.egg-info/top_level.txt
```

### Comparing `spatial_summarize_within-0.1/spatial_summarize_within/summarize within.py` & `spatial_summarize_within-0.1.1/spatial_summarize_within/summarize_within.py`

 * *Files identical despite different names*

