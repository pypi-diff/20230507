# Comparing `tmp/audioviz-0.1.7.tar.gz` & `tmp/audioviz-0.1.8.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioviz-0.1.7.tar", last modified: Sun May  7 08:14:13 2023, max compression
+gzip compressed data, was "audioviz-0.1.8.dev0.tar", last modified: Sun May  7 08:34:37 2023, max compression
```

## Comparing `audioviz-0.1.7.tar` & `audioviz-0.1.8.dev0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-07 08:14:13.067033 audioviz-0.1.7/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1941 2023-05-07 08:14:13.067033 audioviz-0.1.7/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1208 2023-05-07 03:19:43.000000 audioviz-0.1.7/README.md
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-07 08:14:13.067033 audioviz-0.1.7/audioviz/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8548 2023-04-27 03:14:29.000000 audioviz-0.1.7/audioviz/BeatAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    10474 2023-05-05 03:22:56.000000 audioviz-0.1.7/audioviz/ChordAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2679 2023-04-30 07:22:36.000000 audioviz-0.1.7/audioviz/GeneralAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2653 2023-05-05 03:17:01.000000 audioviz-0.1.7/audioviz/Panel.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9984 2023-04-23 03:57:05.000000 audioviz-0.1.7/audioviz/PitchAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14126 2023-04-23 04:28:52.000000 audioviz-0.1.7/audioviz/StructureAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6523 2023-04-23 03:57:05.000000 audioviz-0.1.7/audioviz/TimbreAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      304 2023-05-07 07:11:37.000000 audioviz-0.1.7/audioviz/__init__.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1591 2023-04-27 03:14:12.000000 audioviz-0.1.7/audioviz/colabInterface.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1094 2023-05-07 03:14:17.000000 audioviz-0.1.7/audioviz/utils.py
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-07 08:14:13.067033 audioviz-0.1.7/audioviz.egg-info/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1941 2023-05-07 08:14:13.000000 audioviz-0.1.7/audioviz.egg-info/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      464 2023-05-07 08:14:13.000000 audioviz-0.1.7/audioviz.egg-info/SOURCES.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-05-07 08:14:13.000000 audioviz-0.1.7/audioviz.egg-info/dependency_links.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.1.7/audioviz.egg-info/not-zip-safe
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       69 2023-05-07 08:14:13.000000 audioviz-0.1.7/audioviz.egg-info/requires.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-05-07 08:14:13.000000 audioviz-0.1.7/audioviz.egg-info/top_level.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-05-07 08:14:13.067033 audioviz-0.1.7/setup.cfg
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1368 2023-05-07 08:13:43.000000 audioviz-0.1.7/setup.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-07 08:34:37.845638 audioviz-0.1.8.dev0/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1938 2023-05-07 08:34:37.845638 audioviz-0.1.8.dev0/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1208 2023-05-07 03:19:43.000000 audioviz-0.1.8.dev0/README.md
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-07 08:34:37.845638 audioviz-0.1.8.dev0/audioviz/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8548 2023-04-27 03:14:29.000000 audioviz-0.1.8.dev0/audioviz/BeatAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    10474 2023-05-05 03:22:56.000000 audioviz-0.1.8.dev0/audioviz/ChordAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2679 2023-04-30 07:22:36.000000 audioviz-0.1.8.dev0/audioviz/GeneralAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2653 2023-05-05 03:17:01.000000 audioviz-0.1.8.dev0/audioviz/Panel.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9984 2023-04-23 03:57:05.000000 audioviz-0.1.8.dev0/audioviz/PitchAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14126 2023-04-23 04:28:52.000000 audioviz-0.1.8.dev0/audioviz/StructureAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6523 2023-04-23 03:57:05.000000 audioviz-0.1.8.dev0/audioviz/TimbreAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      304 2023-05-07 07:11:37.000000 audioviz-0.1.8.dev0/audioviz/__init__.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1591 2023-04-27 03:14:12.000000 audioviz-0.1.8.dev0/audioviz/colabInterface.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1094 2023-05-07 03:14:17.000000 audioviz-0.1.8.dev0/audioviz/utils.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-07 08:34:37.845638 audioviz-0.1.8.dev0/audioviz.egg-info/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1938 2023-05-07 08:34:37.000000 audioviz-0.1.8.dev0/audioviz.egg-info/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      464 2023-05-07 08:34:37.000000 audioviz-0.1.8.dev0/audioviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-05-07 08:34:37.000000 audioviz-0.1.8.dev0/audioviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.1.8.dev0/audioviz.egg-info/not-zip-safe
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       80 2023-05-07 08:34:37.000000 audioviz-0.1.8.dev0/audioviz.egg-info/requires.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-05-07 08:34:37.000000 audioviz-0.1.8.dev0/audioviz.egg-info/top_level.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-05-07 08:34:37.845638 audioviz-0.1.8.dev0/setup.cfg
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1375 2023-05-07 08:34:06.000000 audioviz-0.1.8.dev0/setup.py
```

### Comparing `audioviz-0.1.7/PKG-INFO` & `audioviz-0.1.8.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: audioviz
-Version: 0.1.7
+Version: 0.1.8.dev0
 Summary: An user-friendly music information retrieval tools interfacing with Google Colab
 Home-page: https://github.com/TrangDuLam/audioviz
 Author: ayTrang
 Author-email: andrew.chuang@gapp.nthu.edu.tw
 License: MIT
 Keywords: Music Information Retrieval,Academia Sinica,NTHU
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Topic :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.9, !=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # audioviz-colab ##
 
 * An user-friendly music information retrieval visualization API interfacing with Google Colab
 * Coordinated by Prof. [Li Su](https://homepage.iis.sinica.edu.tw/pages/lisu/index_en.html), Prof. [Yu-Fen Huang](https://yfhuang.info/) from the [Music and Culture Technology Lab](https://sites.google.com/view/mctl/), Academia Sinica, Taipei, Taiwan
 * A collaration project with graduate students from National Tsing Hua University, Hsinchu, Taiwan
```

### Comparing `audioviz-0.1.7/README.md` & `audioviz-0.1.8.dev0/README.md`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.7/audioviz/BeatAnalysis.py` & `audioviz-0.1.8.dev0/audioviz/BeatAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.7/audioviz/ChordAnalysis.py` & `audioviz-0.1.8.dev0/audioviz/ChordAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.7/audioviz/GeneralAnalysis.py` & `audioviz-0.1.8.dev0/audioviz/GeneralAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.7/audioviz/Panel.py` & `audioviz-0.1.8.dev0/audioviz/Panel.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.7/audioviz/PitchAnalysis.py` & `audioviz-0.1.8.dev0/audioviz/PitchAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.7/audioviz/StructureAnalysis.py` & `audioviz-0.1.8.dev0/audioviz/StructureAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.7/audioviz/TimbreAnalysis.py` & `audioviz-0.1.8.dev0/audioviz/TimbreAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.7/audioviz/colabInterface.py` & `audioviz-0.1.8.dev0/audioviz/colabInterface.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.7/audioviz/utils.py` & `audioviz-0.1.8.dev0/audioviz/utils.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.7/audioviz.egg-info/PKG-INFO` & `audioviz-0.1.8.dev0/audioviz.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: audioviz
-Version: 0.1.7
+Version: 0.1.8.dev0
 Summary: An user-friendly music information retrieval tools interfacing with Google Colab
 Home-page: https://github.com/TrangDuLam/audioviz
 Author: ayTrang
 Author-email: andrew.chuang@gapp.nthu.edu.tw
 License: MIT
 Keywords: Music Information Retrieval,Academia Sinica,NTHU
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
 Classifier: Topic :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.9, !=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # audioviz-colab ##
 
 * An user-friendly music information retrieval visualization API interfacing with Google Colab
 * Coordinated by Prof. [Li Su](https://homepage.iis.sinica.edu.tw/pages/lisu/index_en.html), Prof. [Yu-Fen Huang](https://yfhuang.info/) from the [Music and Culture Technology Lab](https://sites.google.com/view/mctl/), Academia Sinica, Taipei, Taiwan
 * A collaration project with graduate students from National Tsing Hua University, Hsinchu, Taiwan
```

### Comparing `audioviz-0.1.7/setup.py` & `audioviz-0.1.8.dev0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='audioviz',
     packages=['audioviz'],
-    version='0.1.7',
+    version='0.1.8.dev0',
     
     description='An user-friendly music information retrieval tools interfacing with Google Colab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     
     url='https://github.com/TrangDuLam/audioviz',
     author='ayTrang',
@@ -20,15 +20,15 @@
     keywords=['Music Information Retrieval', "Academia Sinica", "NTHU"],
 
     install_requires = ["numpy", 
                         "matplotlib",
                         "pandas",
                         "scipy", 
                         "librosa", 
-                        "madmom", 
+                        "madmom==0.17.dev0", 
                         "libfmp", 
                         "plotly",
                         "soundfile",
                         ],
 
     classifiers=[
         'Development Status :: 3 - Alpha',
@@ -36,10 +36,10 @@
         'Topic :: Multimedia :: Sound/Audio :: Analysis',
         'Topic :: Education',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     
-    python_requires='>=3.9, !=3.10',
+    python_requires='>=3.9'
 
 )
```

