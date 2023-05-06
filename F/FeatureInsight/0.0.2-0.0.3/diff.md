# Comparing `tmp/FeatureInsight-0.0.2.tar.gz` & `tmp/FeatureInsight-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FeatureInsight-0.0.2.tar", last modified: Sat May  6 22:10:34 2023, max compression
+gzip compressed data, was "FeatureInsight-0.0.3.tar", last modified: Sat May  6 22:17:52 2023, max compression
```

## Comparing `FeatureInsight-0.0.2.tar` & `FeatureInsight-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 22:10:34.159107 FeatureInsight-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-05-06 22:10:34.146148 FeatureInsight-0.0.2/FeatureInsight/
--rw-rw-rw-   0        0        0      113 2023-05-06 22:10:27.000000 FeatureInsight-0.0.2/FeatureInsight/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:10:34.157107 FeatureInsight-0.0.2/FeatureInsight/shell/
--rw-rw-rw-   0        0        0       66 2023-05-06 21:36:44.000000 FeatureInsight-0.0.2/FeatureInsight/shell/__init__.py
--rw-rw-rw-   0        0        0      206 2023-05-06 21:36:44.000000 FeatureInsight-0.0.2/FeatureInsight/shell/usage.py
--rw-rw-rw-   0        0        0     2630 2023-05-06 21:58:44.000000 FeatureInsight-0.0.2/FeatureInsight/structure_Investigation.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:10:34.154106 FeatureInsight-0.0.2/FeatureInsight.egg-info/
--rw-rw-rw-   0        0        0      549 2023-05-06 22:10:34.000000 FeatureInsight-0.0.2/FeatureInsight.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2023-05-06 22:10:34.000000 FeatureInsight-0.0.2/FeatureInsight.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 22:10:34.000000 FeatureInsight-0.0.2/FeatureInsight.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-06 22:10:34.000000 FeatureInsight-0.0.2/FeatureInsight.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-05-06 22:10:34.000000 FeatureInsight-0.0.2/FeatureInsight.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 21:37:38.000000 FeatureInsight-0.0.2/FeatureInsight.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1083 2023-05-06 21:32:28.000000 FeatureInsight-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      181 2023-05-06 21:36:43.000000 FeatureInsight-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      549 2023-05-06 22:10:34.158107 FeatureInsight-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       95 2023-05-06 21:48:28.000000 FeatureInsight-0.0.2/README.md
--rw-rw-rw-   0        0        0        0 2023-05-06 21:32:28.000000 FeatureInsight-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 22:10:34.159107 FeatureInsight-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1864 2023-05-06 21:42:54.000000 FeatureInsight-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:17:52.754242 FeatureInsight-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-05-06 22:17:52.739230 FeatureInsight-0.0.3/FeatureInsight/
+-rw-rw-rw-   0        0        0      390 2023-05-06 22:17:46.000000 FeatureInsight-0.0.3/FeatureInsight/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:17:52.752242 FeatureInsight-0.0.3/FeatureInsight/shell/
+-rw-rw-rw-   0        0        0       66 2023-05-06 21:36:44.000000 FeatureInsight-0.0.3/FeatureInsight/shell/__init__.py
+-rw-rw-rw-   0        0        0      206 2023-05-06 21:36:44.000000 FeatureInsight-0.0.3/FeatureInsight/shell/usage.py
+-rw-rw-rw-   0        0        0     2313 2023-05-06 22:13:08.000000 FeatureInsight-0.0.3/FeatureInsight/structure_Investigation.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:17:52.748242 FeatureInsight-0.0.3/FeatureInsight.egg-info/
+-rw-rw-rw-   0        0        0      621 2023-05-06 22:17:52.000000 FeatureInsight-0.0.3/FeatureInsight.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-05-06 22:17:52.000000 FeatureInsight-0.0.3/FeatureInsight.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 22:17:52.000000 FeatureInsight-0.0.3/FeatureInsight.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-06 22:17:52.000000 FeatureInsight-0.0.3/FeatureInsight.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      157 2023-05-06 22:17:52.000000 FeatureInsight-0.0.3/FeatureInsight.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-06 22:17:52.000000 FeatureInsight-0.0.3/FeatureInsight.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 21:37:38.000000 FeatureInsight-0.0.3/FeatureInsight.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1083 2023-05-06 21:32:28.000000 FeatureInsight-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      181 2023-05-06 21:36:43.000000 FeatureInsight-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      621 2023-05-06 22:17:52.753242 FeatureInsight-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2023-05-06 22:11:31.000000 FeatureInsight-0.0.3/README.md
+-rw-rw-rw-   0        0        0      157 2023-05-06 22:17:29.000000 FeatureInsight-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 22:17:52.754242 FeatureInsight-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1864 2023-05-06 22:10:43.000000 FeatureInsight-0.0.3/setup.py
```

### Comparing `FeatureInsight-0.0.2/LICENSE` & `FeatureInsight-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FeatureInsight-0.0.2/setup.py` & `FeatureInsight-0.0.3/setup.py`

 * *Files identical despite different names*

