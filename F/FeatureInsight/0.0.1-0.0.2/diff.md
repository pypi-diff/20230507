# Comparing `tmp/FeatureInsight-0.0.1.tar.gz` & `tmp/FeatureInsight-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FeatureInsight-0.0.1.tar", last modified: Sat May  6 21:45:20 2023, max compression
+gzip compressed data, was "FeatureInsight-0.0.2.tar", last modified: Sat May  6 22:10:34 2023, max compression
```

## Comparing `FeatureInsight-0.0.1.tar` & `FeatureInsight-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 21:45:20.094049 FeatureInsight-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-06 21:45:20.084087 FeatureInsight-0.0.1/FeatureInsight/
--rw-rw-rw-   0        0        0      101 2023-05-06 21:36:44.000000 FeatureInsight-0.0.1/FeatureInsight/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 21:45:20.093050 FeatureInsight-0.0.1/FeatureInsight/shell/
--rw-rw-rw-   0        0        0       66 2023-05-06 21:36:44.000000 FeatureInsight-0.0.1/FeatureInsight/shell/__init__.py
--rw-rw-rw-   0        0        0      206 2023-05-06 21:36:44.000000 FeatureInsight-0.0.1/FeatureInsight/shell/usage.py
-drwxrwxrwx   0        0        0        0 2023-05-06 21:45:20.091085 FeatureInsight-0.0.1/FeatureInsight.egg-info/
--rw-rw-rw-   0        0        0     3307 2023-05-06 21:45:20.000000 FeatureInsight-0.0.1/FeatureInsight.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2023-05-06 21:45:20.000000 FeatureInsight-0.0.1/FeatureInsight.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 21:45:20.000000 FeatureInsight-0.0.1/FeatureInsight.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-06 21:45:20.000000 FeatureInsight-0.0.1/FeatureInsight.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-05-06 21:45:20.000000 FeatureInsight-0.0.1/FeatureInsight.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 21:37:38.000000 FeatureInsight-0.0.1/FeatureInsight.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1083 2023-05-06 21:32:28.000000 FeatureInsight-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      181 2023-05-06 21:36:43.000000 FeatureInsight-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3307 2023-05-06 21:45:20.094049 FeatureInsight-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2855 2023-05-06 21:32:28.000000 FeatureInsight-0.0.1/README.md
--rw-rw-rw-   0        0        0        0 2023-05-06 21:32:28.000000 FeatureInsight-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 21:45:20.094049 FeatureInsight-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1864 2023-05-06 21:42:54.000000 FeatureInsight-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:10:34.159107 FeatureInsight-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-06 22:10:34.146148 FeatureInsight-0.0.2/FeatureInsight/
+-rw-rw-rw-   0        0        0      113 2023-05-06 22:10:27.000000 FeatureInsight-0.0.2/FeatureInsight/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:10:34.157107 FeatureInsight-0.0.2/FeatureInsight/shell/
+-rw-rw-rw-   0        0        0       66 2023-05-06 21:36:44.000000 FeatureInsight-0.0.2/FeatureInsight/shell/__init__.py
+-rw-rw-rw-   0        0        0      206 2023-05-06 21:36:44.000000 FeatureInsight-0.0.2/FeatureInsight/shell/usage.py
+-rw-rw-rw-   0        0        0     2630 2023-05-06 21:58:44.000000 FeatureInsight-0.0.2/FeatureInsight/structure_Investigation.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:10:34.154106 FeatureInsight-0.0.2/FeatureInsight.egg-info/
+-rw-rw-rw-   0        0        0      549 2023-05-06 22:10:34.000000 FeatureInsight-0.0.2/FeatureInsight.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-05-06 22:10:34.000000 FeatureInsight-0.0.2/FeatureInsight.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 22:10:34.000000 FeatureInsight-0.0.2/FeatureInsight.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-06 22:10:34.000000 FeatureInsight-0.0.2/FeatureInsight.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-05-06 22:10:34.000000 FeatureInsight-0.0.2/FeatureInsight.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 21:37:38.000000 FeatureInsight-0.0.2/FeatureInsight.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1083 2023-05-06 21:32:28.000000 FeatureInsight-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      181 2023-05-06 21:36:43.000000 FeatureInsight-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      549 2023-05-06 22:10:34.158107 FeatureInsight-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       95 2023-05-06 21:48:28.000000 FeatureInsight-0.0.2/README.md
+-rw-rw-rw-   0        0        0        0 2023-05-06 21:32:28.000000 FeatureInsight-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 22:10:34.159107 FeatureInsight-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1864 2023-05-06 21:42:54.000000 FeatureInsight-0.0.2/setup.py
```

### Comparing `FeatureInsight-0.0.1/LICENSE` & `FeatureInsight-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FeatureInsight-0.0.1/setup.py` & `FeatureInsight-0.0.2/setup.py`

 * *Files identical despite different names*

