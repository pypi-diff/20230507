# Comparing `tmp/FeatureInsight-0.0.6.tar.gz` & `tmp/FeatureInsight-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FeatureInsight-0.0.6.tar", last modified: Sat May  6 22:29:55 2023, max compression
+gzip compressed data, was "FeatureInsight-0.0.7.tar", last modified: Sat May  6 22:34:37 2023, max compression
```

## Comparing `FeatureInsight-0.0.6.tar` & `FeatureInsight-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 22:29:55.316799 FeatureInsight-0.0.6/
-drwxrwxrwx   0        0        0        0 2023-05-06 22:29:55.304798 FeatureInsight-0.0.6/FeatureInsight/
--rw-rw-rw-   0        0        0     2118 2023-05-06 22:23:10.000000 FeatureInsight-0.0.6/FeatureInsight/EDA_Investigation.py
--rw-rw-rw-   0        0        0      442 2023-05-06 22:29:52.000000 FeatureInsight-0.0.6/FeatureInsight/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:29:55.314800 FeatureInsight-0.0.6/FeatureInsight/shell/
--rw-rw-rw-   0        0        0       66 2023-05-06 21:36:44.000000 FeatureInsight-0.0.6/FeatureInsight/shell/__init__.py
--rw-rw-rw-   0        0        0      206 2023-05-06 21:36:44.000000 FeatureInsight-0.0.6/FeatureInsight/shell/usage.py
--rw-rw-rw-   0        0        0     2590 2023-05-06 22:28:33.000000 FeatureInsight-0.0.6/FeatureInsight/structure_Investigation.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:29:55.312800 FeatureInsight-0.0.6/FeatureInsight.egg-info/
--rw-rw-rw-   0        0        0      621 2023-05-06 22:29:55.000000 FeatureInsight-0.0.6/FeatureInsight.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      486 2023-05-06 22:29:55.000000 FeatureInsight-0.0.6/FeatureInsight.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 22:29:55.000000 FeatureInsight-0.0.6/FeatureInsight.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-06 22:29:55.000000 FeatureInsight-0.0.6/FeatureInsight.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      157 2023-05-06 22:29:55.000000 FeatureInsight-0.0.6/FeatureInsight.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-06 22:29:55.000000 FeatureInsight-0.0.6/FeatureInsight.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 21:37:38.000000 FeatureInsight-0.0.6/FeatureInsight.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1083 2023-05-06 21:32:28.000000 FeatureInsight-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      181 2023-05-06 21:36:43.000000 FeatureInsight-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      621 2023-05-06 22:29:55.315799 FeatureInsight-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      169 2023-05-06 22:23:15.000000 FeatureInsight-0.0.6/README.md
--rw-rw-rw-   0        0        0      157 2023-05-06 22:17:29.000000 FeatureInsight-0.0.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 22:29:55.316799 FeatureInsight-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1864 2023-05-06 22:10:43.000000 FeatureInsight-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:34:37.799113 FeatureInsight-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-05-06 22:34:37.787113 FeatureInsight-0.0.7/FeatureInsight/
+-rw-rw-rw-   0        0        0     2394 2023-05-06 22:34:16.000000 FeatureInsight-0.0.7/FeatureInsight/EDA_Investigation.py
+-rw-rw-rw-   0        0        0      442 2023-05-06 22:34:30.000000 FeatureInsight-0.0.7/FeatureInsight/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:34:37.797113 FeatureInsight-0.0.7/FeatureInsight/shell/
+-rw-rw-rw-   0        0        0       66 2023-05-06 21:36:44.000000 FeatureInsight-0.0.7/FeatureInsight/shell/__init__.py
+-rw-rw-rw-   0        0        0      206 2023-05-06 21:36:44.000000 FeatureInsight-0.0.7/FeatureInsight/shell/usage.py
+-rw-rw-rw-   0        0        0     2590 2023-05-06 22:28:33.000000 FeatureInsight-0.0.7/FeatureInsight/structure_Investigation.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:34:37.795113 FeatureInsight-0.0.7/FeatureInsight.egg-info/
+-rw-rw-rw-   0        0        0      621 2023-05-06 22:34:37.000000 FeatureInsight-0.0.7/FeatureInsight.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      486 2023-05-06 22:34:37.000000 FeatureInsight-0.0.7/FeatureInsight.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 22:34:37.000000 FeatureInsight-0.0.7/FeatureInsight.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-06 22:34:37.000000 FeatureInsight-0.0.7/FeatureInsight.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      157 2023-05-06 22:34:37.000000 FeatureInsight-0.0.7/FeatureInsight.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-06 22:34:37.000000 FeatureInsight-0.0.7/FeatureInsight.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 21:37:38.000000 FeatureInsight-0.0.7/FeatureInsight.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1083 2023-05-06 21:32:28.000000 FeatureInsight-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      181 2023-05-06 21:36:43.000000 FeatureInsight-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      621 2023-05-06 22:34:37.798113 FeatureInsight-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2023-05-06 22:23:15.000000 FeatureInsight-0.0.7/README.md
+-rw-rw-rw-   0        0        0      157 2023-05-06 22:17:29.000000 FeatureInsight-0.0.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 22:34:37.799113 FeatureInsight-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1864 2023-05-06 22:10:43.000000 FeatureInsight-0.0.7/setup.py
```

### Comparing `FeatureInsight-0.0.6/FeatureInsight/EDA_Investigation.py` & `FeatureInsight-0.0.7/FeatureInsight/EDA_Investigation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,19 @@
-
+from sklearn.pipeline import Pipeline
+import pandas as pd 
+import numpy as np
+import seaborn as sns
+import matplotlib.pyplot as plt
+import math
+import os
+from PIL import Image
+import cv2
+from tqdm import tqdm
+from tabulate import tabulate
+from feature_engine.encoding import *
 def univar_dis(train_df,collist):
  """plot distribution for a fea list in df.
  Detailed explanation 
  Args:  
      df: train in dataframe
      collist: ['fea1','fea2']
      flag:
```

### Comparing `FeatureInsight-0.0.6/FeatureInsight/structure_Investigation.py` & `FeatureInsight-0.0.7/FeatureInsight/structure_Investigation.py`

 * *Files identical despite different names*

### Comparing `FeatureInsight-0.0.6/FeatureInsight.egg-info/PKG-INFO` & `FeatureInsight-0.0.7/FeatureInsight.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeatureInsight
-Version: 0.0.6
+Version: 0.0.7
 Summary: project description
 Home-page: https://github.com/px39n/FeatureInsight
 Author: px39n
 Author-email: isxzl39@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `FeatureInsight-0.0.6/LICENSE` & `FeatureInsight-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `FeatureInsight-0.0.6/PKG-INFO` & `FeatureInsight-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeatureInsight
-Version: 0.0.6
+Version: 0.0.7
 Summary: project description
 Home-page: https://github.com/px39n/FeatureInsight
 Author: px39n
 Author-email: isxzl39@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `FeatureInsight-0.0.6/setup.py` & `FeatureInsight-0.0.7/setup.py`

 * *Files identical despite different names*

