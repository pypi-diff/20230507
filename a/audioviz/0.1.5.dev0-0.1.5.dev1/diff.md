# Comparing `tmp/audioviz-0.1.5.dev0.tar.gz` & `tmp/audioviz-0.1.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioviz-0.1.5.dev0.tar", last modified: Fri May  5 03:26:26 2023, max compression
+gzip compressed data, was "audioviz-0.1.5.dev1.tar", last modified: Sun May  7 03:02:06 2023, max compression
```

## Comparing `audioviz-0.1.5.dev0.tar` & `audioviz-0.1.5.dev1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-05 03:26:26.001868 audioviz-0.1.5.dev0/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      689 2023-05-05 03:26:26.001868 audioviz-0.1.5.dev0/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1258 2023-04-25 05:51:15.000000 audioviz-0.1.5.dev0/README.md
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-05 03:26:25.997868 audioviz-0.1.5.dev0/audioviz/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8548 2023-04-27 03:14:29.000000 audioviz-0.1.5.dev0/audioviz/BeatAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    10474 2023-05-05 03:22:56.000000 audioviz-0.1.5.dev0/audioviz/ChordAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2679 2023-04-30 07:22:36.000000 audioviz-0.1.5.dev0/audioviz/GeneralAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2653 2023-05-05 03:17:01.000000 audioviz-0.1.5.dev0/audioviz/Panel.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9984 2023-04-23 03:57:05.000000 audioviz-0.1.5.dev0/audioviz/PitchAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14126 2023-04-23 04:28:52.000000 audioviz-0.1.5.dev0/audioviz/StructureAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6523 2023-04-23 03:57:05.000000 audioviz-0.1.5.dev0/audioviz/TimbreAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      284 2023-05-05 03:18:02.000000 audioviz-0.1.5.dev0/audioviz/__init__.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1591 2023-04-27 03:14:12.000000 audioviz-0.1.5.dev0/audioviz/colabInterface.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1077 2023-04-30 07:26:37.000000 audioviz-0.1.5.dev0/audioviz/utils.py
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-05 03:26:26.001868 audioviz-0.1.5.dev0/audioviz.egg-info/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      689 2023-05-05 03:26:25.000000 audioviz-0.1.5.dev0/audioviz.egg-info/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      464 2023-05-05 03:26:25.000000 audioviz-0.1.5.dev0/audioviz.egg-info/SOURCES.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-05-05 03:26:25.000000 audioviz-0.1.5.dev0/audioviz.egg-info/dependency_links.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.1.5.dev0/audioviz.egg-info/not-zip-safe
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       69 2023-05-05 03:26:25.000000 audioviz-0.1.5.dev0/audioviz.egg-info/requires.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-05-05 03:26:25.000000 audioviz-0.1.5.dev0/audioviz.egg-info/top_level.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-05-05 03:26:26.001868 audioviz-0.1.5.dev0/setup.cfg
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1197 2023-05-05 03:25:30.000000 audioviz-0.1.5.dev0/setup.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-07 03:02:06.673739 audioviz-0.1.5.dev1/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1772 2023-05-07 03:02:06.673739 audioviz-0.1.5.dev1/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1042 2023-05-07 02:59:39.000000 audioviz-0.1.5.dev1/README.md
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-07 03:02:06.673739 audioviz-0.1.5.dev1/audioviz/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8548 2023-04-27 03:14:29.000000 audioviz-0.1.5.dev1/audioviz/BeatAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    10474 2023-05-05 03:22:56.000000 audioviz-0.1.5.dev1/audioviz/ChordAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2679 2023-04-30 07:22:36.000000 audioviz-0.1.5.dev1/audioviz/GeneralAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2653 2023-05-05 03:17:01.000000 audioviz-0.1.5.dev1/audioviz/Panel.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9984 2023-04-23 03:57:05.000000 audioviz-0.1.5.dev1/audioviz/PitchAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14126 2023-04-23 04:28:52.000000 audioviz-0.1.5.dev1/audioviz/StructureAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6523 2023-04-23 03:57:05.000000 audioviz-0.1.5.dev1/audioviz/TimbreAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      284 2023-05-05 03:18:02.000000 audioviz-0.1.5.dev1/audioviz/__init__.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1591 2023-04-27 03:14:12.000000 audioviz-0.1.5.dev1/audioviz/colabInterface.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1077 2023-04-30 07:26:37.000000 audioviz-0.1.5.dev1/audioviz/utils.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-07 03:02:06.673739 audioviz-0.1.5.dev1/audioviz.egg-info/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1772 2023-05-07 03:02:06.000000 audioviz-0.1.5.dev1/audioviz.egg-info/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      464 2023-05-07 03:02:06.000000 audioviz-0.1.5.dev1/audioviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-05-07 03:02:06.000000 audioviz-0.1.5.dev1/audioviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.1.5.dev1/audioviz.egg-info/not-zip-safe
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       69 2023-05-07 03:02:06.000000 audioviz-0.1.5.dev1/audioviz.egg-info/requires.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-05-07 03:02:06.000000 audioviz-0.1.5.dev1/audioviz.egg-info/top_level.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-05-07 03:02:06.673739 audioviz-0.1.5.dev1/setup.cfg
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1364 2023-05-07 03:01:28.000000 audioviz-0.1.5.dev1/setup.py
```

### Comparing `audioviz-0.1.5.dev0/README.md` & `audioviz-0.1.5.dev1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,18 @@
 # audioviz-colab ##
 
-* An user-friendly music information retrieval visualization API
-* Coordinated by Prof. Li Su, Prof. Yufen Huang from Academia Sinica
-* A collaration project with graduate students from National Tsing Hua University
-
-## Progress Update ##
-
-| Stage |     Date     |    Description   |
-| :---: |     :---:    |       :---:      |
-| Dev 7 | Feb. 12 2023 | Adapting Plotly Functionalities |
-| Dev 8 | Feb. 14 2023 | Packaging Configuration |
-| Alpha 1 | Mar. 2 2023 | Plotly-based Visualization |
-| Alpha 2 | Mar. 17 2023 | Colab Interfacing Completed |
-| Alpha 3 | Apr. 3 2023 | Colab Interfacing Revamped |
+* An user-friendly music information retrieval visualization API interfacing with Google Colab
+* Coordinated by Prof. Li Su, Prof. Yufen Huang from Academia Sinica, Taipei, Taiwan
+* A collaration project with graduate students from National Tsing Hua University, Hsinchu, Taiwan
 
-
-## Introduction to this repository ##
+## Introduction to this packages ##
 
 * Custom visualization wrappers for open source module [librosa](https://librosa.org/doc/latest/index.html)
-* Using open source graphing library [Plotly](https://plotly.com/python/) to enhance user experience
+* Using open source graphing library [Plotly](https://plotly.com/python/) to enhance visualization capabilities
+* Direcctly integrated with Google Colab functions to provide platform-free user experience
 * Please refer to [official page](https://grace1287986s-organization.gitbook.io/musicai-ui-space-v2/) for more details
 
 ## Installation and Dependency ##
 
 ### Installation ###
 
 * PyPi installation
@@ -30,15 +20,14 @@
   ```bash
   pip install audioviz
   ```
 
 * setup.py
 
 ## Developer Demo ##
-
-## Demo Notebook ##
+![alt text](panel.png "Title")
 
 ## Future Works ##
 
 * Colab upload solution
   * Direct instruction
 * Programming Copilot
```

### Comparing `audioviz-0.1.5.dev0/audioviz/BeatAnalysis.py` & `audioviz-0.1.5.dev1/audioviz/BeatAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.5.dev0/audioviz/ChordAnalysis.py` & `audioviz-0.1.5.dev1/audioviz/ChordAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.5.dev0/audioviz/GeneralAnalysis.py` & `audioviz-0.1.5.dev1/audioviz/GeneralAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.5.dev0/audioviz/Panel.py` & `audioviz-0.1.5.dev1/audioviz/Panel.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.5.dev0/audioviz/PitchAnalysis.py` & `audioviz-0.1.5.dev1/audioviz/PitchAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.5.dev0/audioviz/StructureAnalysis.py` & `audioviz-0.1.5.dev1/audioviz/StructureAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.5.dev0/audioviz/TimbreAnalysis.py` & `audioviz-0.1.5.dev1/audioviz/TimbreAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.5.dev0/audioviz/colabInterface.py` & `audioviz-0.1.5.dev1/audioviz/colabInterface.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.5.dev0/audioviz/utils.py` & `audioviz-0.1.5.dev1/audioviz/utils.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.5.dev0/setup.py` & `audioviz-0.1.5.dev1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from setuptools import setup, find_packages
 
+with open("README.md", "r") as f:
+    long_description = f.read()
+
 setup(
     name='audioviz',
     packages=['audioviz'],
-    version='0.1.5dev',
+    version='0.1.5dev1',
+    
     description='An user-friendly music information retrieval tools interfacing with Google Colab',
-
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    
     url='https://github.com/TrangDuLam/audioviz',
     author='ayTrang',
     author_email='andrew.chuang@gapp.nthu.edu.tw',
     license='MIT',
     zip_safe=False,
     keywords=['Music Information Retrieval', "Academia Sinica", "NTHU"],
```

