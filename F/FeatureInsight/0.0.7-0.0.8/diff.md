# Comparing `tmp/FeatureInsight-0.0.7.tar.gz` & `tmp/FeatureInsight-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FeatureInsight-0.0.7.tar", last modified: Sat May  6 22:34:37 2023, max compression
+gzip compressed data, was "FeatureInsight-0.0.8.tar", last modified: Sun May  7 00:03:11 2023, max compression
```

## Comparing `FeatureInsight-0.0.7.tar` & `FeatureInsight-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 22:34:37.799113 FeatureInsight-0.0.7/
-drwxrwxrwx   0        0        0        0 2023-05-06 22:34:37.787113 FeatureInsight-0.0.7/FeatureInsight/
--rw-rw-rw-   0        0        0     2394 2023-05-06 22:34:16.000000 FeatureInsight-0.0.7/FeatureInsight/EDA_Investigation.py
--rw-rw-rw-   0        0        0      442 2023-05-06 22:34:30.000000 FeatureInsight-0.0.7/FeatureInsight/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:34:37.797113 FeatureInsight-0.0.7/FeatureInsight/shell/
--rw-rw-rw-   0        0        0       66 2023-05-06 21:36:44.000000 FeatureInsight-0.0.7/FeatureInsight/shell/__init__.py
--rw-rw-rw-   0        0        0      206 2023-05-06 21:36:44.000000 FeatureInsight-0.0.7/FeatureInsight/shell/usage.py
--rw-rw-rw-   0        0        0     2590 2023-05-06 22:28:33.000000 FeatureInsight-0.0.7/FeatureInsight/structure_Investigation.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:34:37.795113 FeatureInsight-0.0.7/FeatureInsight.egg-info/
--rw-rw-rw-   0        0        0      621 2023-05-06 22:34:37.000000 FeatureInsight-0.0.7/FeatureInsight.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      486 2023-05-06 22:34:37.000000 FeatureInsight-0.0.7/FeatureInsight.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 22:34:37.000000 FeatureInsight-0.0.7/FeatureInsight.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-06 22:34:37.000000 FeatureInsight-0.0.7/FeatureInsight.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      157 2023-05-06 22:34:37.000000 FeatureInsight-0.0.7/FeatureInsight.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-06 22:34:37.000000 FeatureInsight-0.0.7/FeatureInsight.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 21:37:38.000000 FeatureInsight-0.0.7/FeatureInsight.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1083 2023-05-06 21:32:28.000000 FeatureInsight-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      181 2023-05-06 21:36:43.000000 FeatureInsight-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      621 2023-05-06 22:34:37.798113 FeatureInsight-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      169 2023-05-06 22:23:15.000000 FeatureInsight-0.0.7/README.md
--rw-rw-rw-   0        0        0      157 2023-05-06 22:17:29.000000 FeatureInsight-0.0.7/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 22:34:37.799113 FeatureInsight-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1864 2023-05-06 22:10:43.000000 FeatureInsight-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 00:03:11.505610 FeatureInsight-0.0.8/
+drwxrwxrwx   0        0        0        0 2023-05-07 00:03:11.486610 FeatureInsight-0.0.8/FeatureInsight/
+-rw-rw-rw-   0        0        0     4287 2023-05-06 23:52:10.000000 FeatureInsight-0.0.8/FeatureInsight/EDA_Investigation.py
+-rw-rw-rw-   0        0        0      442 2023-05-07 00:01:56.000000 FeatureInsight-0.0.8/FeatureInsight/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 00:03:11.503610 FeatureInsight-0.0.8/FeatureInsight/shell/
+-rw-rw-rw-   0        0        0       66 2023-05-06 21:36:44.000000 FeatureInsight-0.0.8/FeatureInsight/shell/__init__.py
+-rw-rw-rw-   0        0        0      206 2023-05-06 21:36:44.000000 FeatureInsight-0.0.8/FeatureInsight/shell/usage.py
+-rw-rw-rw-   0        0        0     2590 2023-05-06 22:28:33.000000 FeatureInsight-0.0.8/FeatureInsight/structure_Investigation.py
+-rw-rw-rw-   0        0        0     1498 2023-05-06 23:06:50.000000 FeatureInsight-0.0.8/FeatureInsight/untitled.py
+drwxrwxrwx   0        0        0        0 2023-05-07 00:03:11.500610 FeatureInsight-0.0.8/FeatureInsight.egg-info/
+-rw-rw-rw-   0        0        0      854 2023-05-07 00:03:11.000000 FeatureInsight-0.0.8/FeatureInsight.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      513 2023-05-07 00:03:11.000000 FeatureInsight-0.0.8/FeatureInsight.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 00:03:11.000000 FeatureInsight-0.0.8/FeatureInsight.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-07 00:03:11.000000 FeatureInsight-0.0.8/FeatureInsight.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      162 2023-05-07 00:03:11.000000 FeatureInsight-0.0.8/FeatureInsight.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-07 00:03:11.000000 FeatureInsight-0.0.8/FeatureInsight.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 21:37:38.000000 FeatureInsight-0.0.8/FeatureInsight.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1083 2023-05-06 21:32:28.000000 FeatureInsight-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      181 2023-05-06 21:36:43.000000 FeatureInsight-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      854 2023-05-07 00:03:11.504610 FeatureInsight-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-05-07 00:03:06.000000 FeatureInsight-0.0.8/README.md
+-rw-rw-rw-   0        0        0      161 2023-05-06 22:52:29.000000 FeatureInsight-0.0.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 00:03:11.505610 FeatureInsight-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1864 2023-05-06 22:10:43.000000 FeatureInsight-0.0.8/setup.py
```

### Comparing `FeatureInsight-0.0.7/FeatureInsight/EDA_Investigation.py` & `FeatureInsight-0.0.8/FeatureInsight/untitled.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-from sklearn.pipeline import Pipeline
-import pandas as pd 
-import numpy as np
-import seaborn as sns
-import matplotlib.pyplot as plt
-import math
-import os
-from PIL import Image
-import cv2
-from tqdm import tqdm
-from tabulate import tabulate
-from feature_engine.encoding import *
 def univar_dis(train_df,collist):
  """plot distribution for a fea list in df.
  Detailed explanation 
  Args:  
      df: train in dataframe
      collist: ['fea1','fea2']
      flag: 
@@ -46,32 +34,7 @@
        df=encoder.fit_transform(df)
        sns.countplot(x=cat_list[i], data=df,ax=ax[i])
        ax[i].axvline(x = df[cat_list[i]].quantile(.1), color = 'r', label = '10%')
        ax[i].axvline(x = df[cat_list[i]].quantile(.9), color = 'r', label = '90%')
        ax[i].legend() 
        ax[i].set_title(cat_list[i]+"("+str(train_df[cat_list[i]].nunique())+")")
    plt.show()
-
-
-
-
-def bivar_dis(df,fea_list):
-    """plot bivar_dis for a fea list in df.
-    Detailed explanation 
-    Args:  
-        df: train in dataframe
-        fea_list: [['fea1','fea2'],['fea1','fea2'],['fea1','fea2']]
-        
-    Returns:
-       nothing
-        
-    """   
-    #build figure, set size
-    r_n=math.ceil(len(fea_list)/3)
-    fig, ax =plt.subplots(figsize = (18, 6*r_n), nrows = r_n, ncols = 3)
-    ax=ax.reshape(-1)
-    for i,coup in enumerate(fea_list):
-        
-        #plot data
-        sns.histplot(x=coup[0],hue=coup[1], data=df,ax=ax[i])
-        ax[i].set_title(coup[0]+" vs "+coup[1])
-    plt.show()
```

### Comparing `FeatureInsight-0.0.7/FeatureInsight/structure_Investigation.py` & `FeatureInsight-0.0.8/FeatureInsight/structure_Investigation.py`

 * *Files identical despite different names*

### Comparing `FeatureInsight-0.0.7/LICENSE` & `FeatureInsight-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `FeatureInsight-0.0.7/setup.py` & `FeatureInsight-0.0.8/setup.py`

 * *Files identical despite different names*

