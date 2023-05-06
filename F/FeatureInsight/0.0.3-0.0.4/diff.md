# Comparing `tmp/FeatureInsight-0.0.3.tar.gz` & `tmp/FeatureInsight-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FeatureInsight-0.0.3.tar", last modified: Sat May  6 22:17:52 2023, max compression
+gzip compressed data, was "FeatureInsight-0.0.4.tar", last modified: Sat May  6 22:23:53 2023, max compression
```

## Comparing `FeatureInsight-0.0.3.tar` & `FeatureInsight-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 22:17:52.754242 FeatureInsight-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-05-06 22:17:52.739230 FeatureInsight-0.0.3/FeatureInsight/
--rw-rw-rw-   0        0        0      390 2023-05-06 22:17:46.000000 FeatureInsight-0.0.3/FeatureInsight/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:17:52.752242 FeatureInsight-0.0.3/FeatureInsight/shell/
--rw-rw-rw-   0        0        0       66 2023-05-06 21:36:44.000000 FeatureInsight-0.0.3/FeatureInsight/shell/__init__.py
--rw-rw-rw-   0        0        0      206 2023-05-06 21:36:44.000000 FeatureInsight-0.0.3/FeatureInsight/shell/usage.py
--rw-rw-rw-   0        0        0     2313 2023-05-06 22:13:08.000000 FeatureInsight-0.0.3/FeatureInsight/structure_Investigation.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:17:52.748242 FeatureInsight-0.0.3/FeatureInsight.egg-info/
--rw-rw-rw-   0        0        0      621 2023-05-06 22:17:52.000000 FeatureInsight-0.0.3/FeatureInsight.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-05-06 22:17:52.000000 FeatureInsight-0.0.3/FeatureInsight.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 22:17:52.000000 FeatureInsight-0.0.3/FeatureInsight.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-06 22:17:52.000000 FeatureInsight-0.0.3/FeatureInsight.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      157 2023-05-06 22:17:52.000000 FeatureInsight-0.0.3/FeatureInsight.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-06 22:17:52.000000 FeatureInsight-0.0.3/FeatureInsight.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 21:37:38.000000 FeatureInsight-0.0.3/FeatureInsight.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1083 2023-05-06 21:32:28.000000 FeatureInsight-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      181 2023-05-06 21:36:43.000000 FeatureInsight-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      621 2023-05-06 22:17:52.753242 FeatureInsight-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      169 2023-05-06 22:11:31.000000 FeatureInsight-0.0.3/README.md
--rw-rw-rw-   0        0        0      157 2023-05-06 22:17:29.000000 FeatureInsight-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 22:17:52.754242 FeatureInsight-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1864 2023-05-06 22:10:43.000000 FeatureInsight-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:23:53.639645 FeatureInsight-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-05-06 22:23:53.627643 FeatureInsight-0.0.4/FeatureInsight/
+-rw-rw-rw-   0        0        0     2118 2023-05-06 22:23:10.000000 FeatureInsight-0.0.4/FeatureInsight/EDA_Investigation.py
+-rw-rw-rw-   0        0        0      442 2023-05-06 22:23:27.000000 FeatureInsight-0.0.4/FeatureInsight/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:23:53.637645 FeatureInsight-0.0.4/FeatureInsight/shell/
+-rw-rw-rw-   0        0        0       66 2023-05-06 21:36:44.000000 FeatureInsight-0.0.4/FeatureInsight/shell/__init__.py
+-rw-rw-rw-   0        0        0      206 2023-05-06 21:36:44.000000 FeatureInsight-0.0.4/FeatureInsight/shell/usage.py
+-rw-rw-rw-   0        0        0     2313 2023-05-06 22:13:08.000000 FeatureInsight-0.0.4/FeatureInsight/structure_Investigation.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:23:53.635645 FeatureInsight-0.0.4/FeatureInsight.egg-info/
+-rw-rw-rw-   0        0        0      621 2023-05-06 22:23:53.000000 FeatureInsight-0.0.4/FeatureInsight.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      486 2023-05-06 22:23:53.000000 FeatureInsight-0.0.4/FeatureInsight.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 22:23:53.000000 FeatureInsight-0.0.4/FeatureInsight.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-06 22:23:53.000000 FeatureInsight-0.0.4/FeatureInsight.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      157 2023-05-06 22:23:53.000000 FeatureInsight-0.0.4/FeatureInsight.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-06 22:23:53.000000 FeatureInsight-0.0.4/FeatureInsight.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 21:37:38.000000 FeatureInsight-0.0.4/FeatureInsight.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1083 2023-05-06 21:32:28.000000 FeatureInsight-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      181 2023-05-06 21:36:43.000000 FeatureInsight-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      621 2023-05-06 22:23:53.638645 FeatureInsight-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2023-05-06 22:23:15.000000 FeatureInsight-0.0.4/README.md
+-rw-rw-rw-   0        0        0      157 2023-05-06 22:17:29.000000 FeatureInsight-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 22:23:53.639645 FeatureInsight-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1864 2023-05-06 22:10:43.000000 FeatureInsight-0.0.4/setup.py
```

### Comparing `FeatureInsight-0.0.3/FeatureInsight/structure_Investigation.py` & `FeatureInsight-0.0.4/FeatureInsight/structure_Investigation.py`

 * *Files identical despite different names*

### Comparing `FeatureInsight-0.0.3/FeatureInsight.egg-info/PKG-INFO` & `FeatureInsight-0.0.4/FeatureInsight.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeatureInsight
-Version: 0.0.3
+Version: 0.0.4
 Summary: project description
 Home-page: https://github.com/px39n/FeatureInsight
 Author: px39n
 Author-email: isxzl39@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `FeatureInsight-0.0.3/LICENSE` & `FeatureInsight-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FeatureInsight-0.0.3/PKG-INFO` & `FeatureInsight-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeatureInsight
-Version: 0.0.3
+Version: 0.0.4
 Summary: project description
 Home-page: https://github.com/px39n/FeatureInsight
 Author: px39n
 Author-email: isxzl39@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `FeatureInsight-0.0.3/setup.py` & `FeatureInsight-0.0.4/setup.py`

 * *Files identical despite different names*

