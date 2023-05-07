# Comparing `tmp/audioviz-0.1.5.dev1.tar.gz` & `tmp/audioviz-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioviz-0.1.5.dev1.tar", last modified: Sun May  7 03:02:06 2023, max compression
+gzip compressed data, was "audioviz-0.1.6.tar", last modified: Sun May  7 07:20:50 2023, max compression
```

## Comparing `audioviz-0.1.5.dev1.tar` & `audioviz-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-07 03:02:06.673739 audioviz-0.1.5.dev1/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1772 2023-05-07 03:02:06.673739 audioviz-0.1.5.dev1/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1042 2023-05-07 02:59:39.000000 audioviz-0.1.5.dev1/README.md
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-07 03:02:06.673739 audioviz-0.1.5.dev1/audioviz/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8548 2023-04-27 03:14:29.000000 audioviz-0.1.5.dev1/audioviz/BeatAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    10474 2023-05-05 03:22:56.000000 audioviz-0.1.5.dev1/audioviz/ChordAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2679 2023-04-30 07:22:36.000000 audioviz-0.1.5.dev1/audioviz/GeneralAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2653 2023-05-05 03:17:01.000000 audioviz-0.1.5.dev1/audioviz/Panel.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9984 2023-04-23 03:57:05.000000 audioviz-0.1.5.dev1/audioviz/PitchAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14126 2023-04-23 04:28:52.000000 audioviz-0.1.5.dev1/audioviz/StructureAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6523 2023-04-23 03:57:05.000000 audioviz-0.1.5.dev1/audioviz/TimbreAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      284 2023-05-05 03:18:02.000000 audioviz-0.1.5.dev1/audioviz/__init__.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1591 2023-04-27 03:14:12.000000 audioviz-0.1.5.dev1/audioviz/colabInterface.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1077 2023-04-30 07:26:37.000000 audioviz-0.1.5.dev1/audioviz/utils.py
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-07 03:02:06.673739 audioviz-0.1.5.dev1/audioviz.egg-info/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1772 2023-05-07 03:02:06.000000 audioviz-0.1.5.dev1/audioviz.egg-info/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      464 2023-05-07 03:02:06.000000 audioviz-0.1.5.dev1/audioviz.egg-info/SOURCES.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-05-07 03:02:06.000000 audioviz-0.1.5.dev1/audioviz.egg-info/dependency_links.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.1.5.dev1/audioviz.egg-info/not-zip-safe
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       69 2023-05-07 03:02:06.000000 audioviz-0.1.5.dev1/audioviz.egg-info/requires.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-05-07 03:02:06.000000 audioviz-0.1.5.dev1/audioviz.egg-info/top_level.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-05-07 03:02:06.673739 audioviz-0.1.5.dev1/setup.cfg
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1364 2023-05-07 03:01:28.000000 audioviz-0.1.5.dev1/setup.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-07 07:20:50.626348 audioviz-0.1.6/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1933 2023-05-07 07:20:50.626348 audioviz-0.1.6/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1208 2023-05-07 03:19:43.000000 audioviz-0.1.6/README.md
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-07 07:20:50.622348 audioviz-0.1.6/audioviz/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8548 2023-04-27 03:14:29.000000 audioviz-0.1.6/audioviz/BeatAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    10474 2023-05-05 03:22:56.000000 audioviz-0.1.6/audioviz/ChordAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2679 2023-04-30 07:22:36.000000 audioviz-0.1.6/audioviz/GeneralAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2653 2023-05-05 03:17:01.000000 audioviz-0.1.6/audioviz/Panel.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9984 2023-04-23 03:57:05.000000 audioviz-0.1.6/audioviz/PitchAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14126 2023-04-23 04:28:52.000000 audioviz-0.1.6/audioviz/StructureAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6523 2023-04-23 03:57:05.000000 audioviz-0.1.6/audioviz/TimbreAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      304 2023-05-07 07:11:37.000000 audioviz-0.1.6/audioviz/__init__.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1591 2023-04-27 03:14:12.000000 audioviz-0.1.6/audioviz/colabInterface.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1094 2023-05-07 03:14:17.000000 audioviz-0.1.6/audioviz/utils.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-07 07:20:50.626348 audioviz-0.1.6/audioviz.egg-info/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1933 2023-05-07 07:20:50.000000 audioviz-0.1.6/audioviz.egg-info/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      464 2023-05-07 07:20:50.000000 audioviz-0.1.6/audioviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-05-07 07:20:50.000000 audioviz-0.1.6/audioviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.1.6/audioviz.egg-info/not-zip-safe
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       69 2023-05-07 07:20:50.000000 audioviz-0.1.6/audioviz.egg-info/requires.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-05-07 07:20:50.000000 audioviz-0.1.6/audioviz.egg-info/top_level.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-05-07 07:20:50.626348 audioviz-0.1.6/setup.cfg
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1360 2023-05-07 07:19:43.000000 audioviz-0.1.6/setup.py
```

### Comparing `audioviz-0.1.5.dev1/PKG-INFO` & `audioviz-0.1.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioviz
-Version: 0.1.5.dev1
+Version: 0.1.6
 Summary: An user-friendly music information retrieval tools interfacing with Google Colab
 Home-page: https://github.com/TrangDuLam/audioviz
 Author: ayTrang
 Author-email: andrew.chuang@gapp.nthu.edu.tw
 License: MIT
 Keywords: Music Information Retrieval,Academia Sinica,NTHU
 Classifier: Development Status :: 3 - Alpha
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # audioviz-colab ##
 
 * An user-friendly music information retrieval visualization API interfacing with Google Colab
-* Coordinated by Prof. Li Su, Prof. Yufen Huang from Academia Sinica, Taipei, Taiwan
+* Coordinated by Prof. [Li Su](https://homepage.iis.sinica.edu.tw/pages/lisu/index_en.html), Prof. [Yu-Fen Huang](https://yfhuang.info/) from the [Music and Culture Technology Lab](https://sites.google.com/view/mctl/), Academia Sinica, Taipei, Taiwan
 * A collaration project with graduate students from National Tsing Hua University, Hsinchu, Taiwan
 
 ## Introduction to this packages ##
 
 * Custom visualization wrappers for open source module [librosa](https://librosa.org/doc/latest/index.html)
 * Using open source graphing library [Plotly](https://plotly.com/python/) to enhance visualization capabilities
 * Direcctly integrated with Google Colab functions to provide platform-free user experience
```

### Comparing `audioviz-0.1.5.dev1/README.md` & `audioviz-0.1.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # audioviz-colab ##
 
 * An user-friendly music information retrieval visualization API interfacing with Google Colab
-* Coordinated by Prof. Li Su, Prof. Yufen Huang from Academia Sinica, Taipei, Taiwan
+* Coordinated by Prof. [Li Su](https://homepage.iis.sinica.edu.tw/pages/lisu/index_en.html), Prof. [Yu-Fen Huang](https://yfhuang.info/) from the [Music and Culture Technology Lab](https://sites.google.com/view/mctl/), Academia Sinica, Taipei, Taiwan
 * A collaration project with graduate students from National Tsing Hua University, Hsinchu, Taiwan
 
 ## Introduction to this packages ##
 
 * Custom visualization wrappers for open source module [librosa](https://librosa.org/doc/latest/index.html)
 * Using open source graphing library [Plotly](https://plotly.com/python/) to enhance visualization capabilities
 * Direcctly integrated with Google Colab functions to provide platform-free user experience
```

### Comparing `audioviz-0.1.5.dev1/audioviz/BeatAnalysis.py` & `audioviz-0.1.6/audioviz/BeatAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.5.dev1/audioviz/ChordAnalysis.py` & `audioviz-0.1.6/audioviz/ChordAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.5.dev1/audioviz/GeneralAnalysis.py` & `audioviz-0.1.6/audioviz/GeneralAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.5.dev1/audioviz/Panel.py` & `audioviz-0.1.6/audioviz/Panel.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.5.dev1/audioviz/PitchAnalysis.py` & `audioviz-0.1.6/audioviz/PitchAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.5.dev1/audioviz/StructureAnalysis.py` & `audioviz-0.1.6/audioviz/StructureAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.5.dev1/audioviz/TimbreAnalysis.py` & `audioviz-0.1.6/audioviz/TimbreAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.5.dev1/audioviz/colabInterface.py` & `audioviz-0.1.6/audioviz/colabInterface.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.5.dev1/audioviz/utils.py` & `audioviz-0.1.6/audioviz/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import scipy
 import librosa
 
+import IPython.display as ipd
 from IPython.display import Audio
 
 import numpy.typing as npt
 
 def audio_cutter(y: npt.ArrayLike, sr: int, start_time: float, end_time: float) -> npt.ArrayLike :
     '''
     To cut the input signal with start and end time
@@ -30,12 +31,12 @@
 
 def load_example_audio(filename: str) -> None :
     '''
     To load the example audio
 
     '''
     if filename == 'Mozart' :
-        y, sr = librosa.load('./example_audio/Mozart_Turkish_March.wav', duration=30)
+        y, sr = librosa.load('./example/Mozart_Turkish_March.wav', duration=30)
     if filename == 'Brahms' :
-        y, sr = librosa.load('./example_audio/Hungarian_Dance_No_5.wav', duration=30)
+        y, sr = librosa.load('./exampl/Hungarian_Dance_No_5.wav', duration=30)
         
     return y, sr
```

### Comparing `audioviz-0.1.5.dev1/audioviz.egg-info/PKG-INFO` & `audioviz-0.1.6/audioviz.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioviz
-Version: 0.1.5.dev1
+Version: 0.1.6
 Summary: An user-friendly music information retrieval tools interfacing with Google Colab
 Home-page: https://github.com/TrangDuLam/audioviz
 Author: ayTrang
 Author-email: andrew.chuang@gapp.nthu.edu.tw
 License: MIT
 Keywords: Music Information Retrieval,Academia Sinica,NTHU
 Classifier: Development Status :: 3 - Alpha
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # audioviz-colab ##
 
 * An user-friendly music information retrieval visualization API interfacing with Google Colab
-* Coordinated by Prof. Li Su, Prof. Yufen Huang from Academia Sinica, Taipei, Taiwan
+* Coordinated by Prof. [Li Su](https://homepage.iis.sinica.edu.tw/pages/lisu/index_en.html), Prof. [Yu-Fen Huang](https://yfhuang.info/) from the [Music and Culture Technology Lab](https://sites.google.com/view/mctl/), Academia Sinica, Taipei, Taiwan
 * A collaration project with graduate students from National Tsing Hua University, Hsinchu, Taiwan
 
 ## Introduction to this packages ##
 
 * Custom visualization wrappers for open source module [librosa](https://librosa.org/doc/latest/index.html)
 * Using open source graphing library [Plotly](https://plotly.com/python/) to enhance visualization capabilities
 * Direcctly integrated with Google Colab functions to provide platform-free user experience
```

### Comparing `audioviz-0.1.5.dev1/setup.py` & `audioviz-0.1.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='audioviz',
     packages=['audioviz'],
-    version='0.1.5dev1',
+    version='0.1.6',
     
     description='An user-friendly music information retrieval tools interfacing with Google Colab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     
     url='https://github.com/TrangDuLam/audioviz',
     author='ayTrang',
```

