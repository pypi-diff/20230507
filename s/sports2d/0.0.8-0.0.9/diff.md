# Comparing `tmp/sports2d-0.0.8.tar.gz` & `tmp/sports2d-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sports2d-0.0.8.tar", last modified: Sat May  6 00:16:20 2023, max compression
+gzip compressed data, was "sports2d-0.0.9.tar", last modified: Sun May  7 09:28:54 2023, max compression
```

## Comparing `sports2d-0.0.8.tar` & `sports2d-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:16:20.659336 sports2d-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-06 00:16:04.000000 sports2d-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-05-06 00:16:20.659336 sports2d-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11864 2023-05-06 00:16:04.000000 sports2d-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:16:20.651336 sports2d-0.0.8/Sports2D/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:16:20.651336 sports2d-0.0.8/Sports2D/Demo/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-06 00:16:04.000000 sports2d-0.0.8/Sports2D/Demo/Config_demo.toml
--rw-r--r--   0 runner    (1001) docker     (123)  2539508 2023-05-06 00:16:04.000000 sports2d-0.0.8/Sports2D/Demo/demo.mp4
--rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-05-06 00:16:04.000000 sports2d-0.0.8/Sports2D/Sports2D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:16:20.655336 sports2d-0.0.8/Sports2D/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-05-06 00:16:04.000000 sports2d-0.0.8/Sports2D/Utilities/Blazepose_runsave.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-06 00:16:04.000000 sports2d-0.0.8/Sports2D/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-06 00:16:04.000000 sports2d-0.0.8/Sports2D/Utilities/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-06 00:16:04.000000 sports2d-0.0.8/Sports2D/Utilities/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-05-06 00:16:04.000000 sports2d-0.0.8/Sports2D/Utilities/skeletons.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-06 00:16:04.000000 sports2d-0.0.8/Sports2D/Utilities/test_with_blazepose.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-06 00:16:04.000000 sports2d-0.0.8/Sports2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21660 2023-05-06 00:16:04.000000 sports2d-0.0.8/Sports2D/compute_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)    23641 2023-05-06 00:16:04.000000 sports2d-0.0.8/Sports2D/detect_pose.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-06 00:16:04.000000 sports2d-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-06 00:16:20.659336 sports2d-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-06 00:16:04.000000 sports2d-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:16:20.659336 sports2d-0.0.8/sports2d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-05-06 00:16:20.000000 sports2d-0.0.8/sports2d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-06 00:16:20.000000 sports2d-0.0.8/sports2d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:16:20.000000 sports2d-0.0.8/sports2d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:16:20.000000 sports2d-0.0.8/sports2d.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-06 00:16:20.000000 sports2d-0.0.8/sports2d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 00:16:20.000000 sports2d-0.0.8/sports2d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:28:54.448033 sports2d-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-07 09:28:40.000000 sports2d-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14793 2023-05-07 09:28:54.448033 sports2d-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-05-07 09:28:40.000000 sports2d-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:28:54.444033 sports2d-0.0.9/Sports2D/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:28:54.444033 sports2d-0.0.9/Sports2D/Demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/Demo/Config_demo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)  2539508 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/Demo/demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/Sports2D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:28:54.448033 sports2d-0.0.9/Sports2D/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/Utilities/Blazepose_runsave.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/Utilities/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/Utilities/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/Utilities/skeletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/Utilities/test_with_blazepose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21758 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/compute_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23724 2023-05-07 09:28:40.000000 sports2d-0.0.9/Sports2D/detect_pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-07 09:28:40.000000 sports2d-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-07 09:28:54.452033 sports2d-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-07 09:28:40.000000 sports2d-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:28:54.448033 sports2d-0.0.9/sports2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14793 2023-05-07 09:28:54.000000 sports2d-0.0.9/sports2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-07 09:28:54.000000 sports2d-0.0.9/sports2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:28:54.000000 sports2d-0.0.9/sports2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:28:54.000000 sports2d-0.0.9/sports2d.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-07 09:28:54.000000 sports2d-0.0.9/sports2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-07 09:28:54.000000 sports2d-0.0.9/sports2d.egg-info/top_level.txt
```

### Comparing `sports2d-0.0.8/LICENSE` & `sports2d-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.8/PKG-INFO` & `sports2d-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports2d
-Version: 0.0.8
+Version: 0.0.9
 Summary: Detect pose and compute 2D joint angles from a video.
 Home-page: https://github.com/davidpagnon/Sports2D
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
 Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics,sports,sports-analytics
@@ -39,24 +39,23 @@
 -->
 
 
 # Sports2D
 
 **`Sports2D` lets you compute 2D joint and segment angles from a video.**
 
- </br>
- </br>
-
 <img src='Content/demo_gif.gif' title='Demonstration of Sports2D with OpenPose.'  width="760">
 
 `Warning:` Angle estimation is only as good as the pose estimation algorithm, i.e., it is not perfect.\
 `Warning:` Results are acceptable only if the persons move in the 2D plane, from right to left or from left to right.\
 If you need research-grade markerless joint kinematics, consider using several cameras, and constraining angles to a biomechanically accurate model. See [Pose2Sim](https://github.com/perfanalytics/pose2sim) for example.
 
-`Announcement:` Apps with GUI will be released for Windows, Linux, MacOS, as well as Android and iOS.
+`Know issue`: Results won't be good with some iPhone videos in portrait mode. This is solved by priorly converting them with `ffmpeg -i video_input.mov video_output.mp4`, or even more simply with any random online video converter such as https://video-converter.com.
+
+`Announcement:` Apps with GUI will soon be released for Windows, Linux, MacOS, as well as Android and iOS.
 Mobile versions will only support simple exploratory analysis. This involves single-person angle computation, in a potentially less accurate and tunable way.
 
 
 ## Contents
 1. [Installation and Demonstration](#installation-and-demonstration)
    1. [Installation](#installation)
    2. [Demonstration: Detect pose and compute 2D angles](#demonstration-detect-pose-and-compute-2d-angles)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sports2d Version: 0.0.8 Summary: Detect pose and
+Metadata-Version: 2.1 Name: sports2d Version: 0.0.9 Summary: Detect pose and
 compute 2D joint angles from a video. Home-page: https://github.com/
 davidpagnon/Sports2D Author: David Pagnon Author-email: contact@david-
 pagnon.com License: BSD 3-Clause License Project-URL: Bug Tracker, https://
 github.com/davidpagnon/Sports2D/issues Keywords:
 markerless,kinematics,OpenPose,BlazePose,joint
 angles,2D,biomechanics,sports,sports-analytics Platform: any Classifier:
 Programming Language :: Python :: 3 Classifier: Development Status :: 3 - Alpha
@@ -17,46 +17,49 @@
 [Continuous integration](https://github.com/davidpagnon/sports2d/actions/
 workflows/continuous-integration.yml/badge.svg?branch=main)](https://
 github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
 [![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/
 py/Sports2D)\ [![License](https://img.shields.io/badge/License-BSD_3--Clause-
 blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\ [Open_In_Colab]  #
 Sports2D **`Sports2D` lets you compute 2D joint and segment angles from a
-video.**   [Content/demo_gif.gif] `Warning:` Angle estimation is only as good
-as the pose estimation algorithm, i.e., it is not perfect.\ `Warning:` Results
-are acceptable only if the persons move in the 2D plane, from right to left or
-from left to right.\ If you need research-grade markerless joint kinematics,
+video.** [Content/demo_gif.gif] `Warning:` Angle estimation is only as good as
+the pose estimation algorithm, i.e., it is not perfect.\ `Warning:` Results are
+acceptable only if the persons move in the 2D plane, from right to left or from
+left to right.\ If you need research-grade markerless joint kinematics,
 consider using several cameras, and constraining angles to a biomechanically
 accurate model. See [Pose2Sim](https://github.com/perfanalytics/pose2sim) for
-example. `Announcement:` Apps with GUI will be released for Windows, Linux,
-MacOS, as well as Android and iOS. Mobile versions will only support simple
-exploratory analysis. This involves single-person angle computation, in a
-potentially less accurate and tunable way. ## Contents 1. [Installation and
-Demonstration](#installation-and-demonstration) 1. [Installation]
-(#installation) 2. [Demonstration: Detect pose and compute 2D angles]
-(#demonstration-detect-pose-and-compute-2d-angles) 2. [Go further](#go-further)
-1. [Use on your own videos](#use-on-your-own-videos) 2. [Use OpenPose for
-multi-person, more accurate analysis](#use-openpose-for-multi-person-more-
-accurate-analysis) 3. [Advanced-settings](#advanced-settings) 4. [How it works]
-(#how-it-works) 3. [How to cite and how to contribute](#how-to-cite-and-how-to-
-contribute) ## Installation and Demonstration ### Installation - OPTION 1:
-**Quick install** \ Open a terminal. Type `python -V` to make sure python
-'>=3.7 <=3.10' is installed, and then: ``` pip install sports2d ``` - OPTION 2:
-**Safer install with Anaconda**\ Install [Miniconda](https://docs.conda.io/en/
-latest/miniconda.html):\ Open an Anaconda prompt and create a virtual
-environment by typing: ``` conda create -n Sports2D python<=3.10 conda activate
-Sports2D pip install sports2d ``` - OPTION 3: **Build from source and test the
-last changes**\ Open a terminal in the directory of your choice and clone the
-Sports2D repository. ``` git clone https://github.com/davidpagnon/sports2d.git
-cd sports2d pip install . ``` ### Demonstration: Detect pose and compute 2D
-angles Open a terminal, enter `pip show sports2d`, check sports2d package
-location. \ Copy this path and go to the Demo folder by typing `cd
-\Sports2D\Demo`. \ Type `ipython`, and test the following code: ``` from
-Sports2D import Sports2D Sports2D.detect_pose('Config_demo.toml')
-Sports2D.compute_angles('Config_demo.toml') ``` [Content/
+example. `Know issue`: Results won't be good with some iPhone videos in
+portrait mode. This is solved by priorly converting them with `ffmpeg -
+i video_input.mov video_output.mp4`, or even more simply with any random online
+video converter such as https://video-converter.com. `Announcement:` Apps with
+GUI will soon be released for Windows, Linux, MacOS, as well as Android and
+iOS. Mobile versions will only support simple exploratory analysis. This
+involves single-person angle computation, in a potentially less accurate and
+tunable way. ## Contents 1. [Installation and Demonstration](#installation-and-
+demonstration) 1. [Installation](#installation) 2. [Demonstration: Detect pose
+and compute 2D angles](#demonstration-detect-pose-and-compute-2d-angles) 2. [Go
+further](#go-further) 1. [Use on your own videos](#use-on-your-own-videos) 2.
+[Use OpenPose for multi-person, more accurate analysis](#use-openpose-for-
+multi-person-more-accurate-analysis) 3. [Advanced-settings](#advanced-settings)
+4. [How it works](#how-it-works) 3. [How to cite and how to contribute](#how-
+to-cite-and-how-to-contribute) ## Installation and Demonstration ###
+Installation - OPTION 1: **Quick install** \ Open a terminal. Type `python -V`
+to make sure python '>=3.7 <=3.10' is installed, and then: ``` pip install
+sports2d ``` - OPTION 2: **Safer install with Anaconda**\ Install [Miniconda]
+(https://docs.conda.io/en/latest/miniconda.html):\ Open an Anaconda prompt and
+create a virtual environment by typing: ``` conda create -n Sports2D
+python<=3.10 conda activate Sports2D pip install sports2d ``` - OPTION 3:
+**Build from source and test the last changes**\ Open a terminal in the
+directory of your choice and clone the Sports2D repository. ``` git clone
+https://github.com/davidpagnon/sports2d.git cd sports2d pip install . ``` ###
+Demonstration: Detect pose and compute 2D angles Open a terminal, enter `pip
+show sports2d`, check sports2d package location. \ Copy this path and go to the
+Demo folder by typing `cd \Sports2D\Demo`. \ Type `ipython`, and test the
+following code: ``` from Sports2D import Sports2D Sports2D.detect_pose
+('Config_demo.toml') Sports2D.compute_angles('Config_demo.toml') ``` [Content/
 demo_blazepose_terminal.png] You should obtain a video with the overlaid 2D
 joint positions, and angle text values. This output is also provided as an
 image folder.\ You should additionally obtain the same information as time
 series, stored in .csv files. These files can be opened with any spreadsheet
 software, or with the Pandas Python library for example.\ In addition, you will
 get the original OpenPose-like json coordinates files. [Content/
 demo_blazepose_results.png] ## Go further ### Use on your own videos 1. Copy-
```

### Comparing `sports2d-0.0.8/README.md` & `sports2d-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,24 +12,23 @@
 -->
 
 
 # Sports2D
 
 **`Sports2D` lets you compute 2D joint and segment angles from a video.**
 
- </br>
- </br>
-
 <img src='Content/demo_gif.gif' title='Demonstration of Sports2D with OpenPose.'  width="760">
 
 `Warning:` Angle estimation is only as good as the pose estimation algorithm, i.e., it is not perfect.\
 `Warning:` Results are acceptable only if the persons move in the 2D plane, from right to left or from left to right.\
 If you need research-grade markerless joint kinematics, consider using several cameras, and constraining angles to a biomechanically accurate model. See [Pose2Sim](https://github.com/perfanalytics/pose2sim) for example.
 
-`Announcement:` Apps with GUI will be released for Windows, Linux, MacOS, as well as Android and iOS.
+`Know issue`: Results won't be good with some iPhone videos in portrait mode. This is solved by priorly converting them with `ffmpeg -i video_input.mov video_output.mp4`, or even more simply with any random online video converter such as https://video-converter.com.
+
+`Announcement:` Apps with GUI will soon be released for Windows, Linux, MacOS, as well as Android and iOS.
 Mobile versions will only support simple exploratory analysis. This involves single-person angle computation, in a potentially less accurate and tunable way.
 
 
 ## Contents
 1. [Installation and Demonstration](#installation-and-demonstration)
    1. [Installation](#installation)
    2. [Demonstration: Detect pose and compute 2D angles](#demonstration-detect-pose-and-compute-2d-angles)
```

#### html2text {}

```diff
@@ -1,46 +1,49 @@
  [![Continuous integration](https://github.com/davidpagnon/sports2d/actions/
 workflows/continuous-integration.yml/badge.svg?branch=main)](https://
 github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
 [![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/
 py/Sports2D)\ [![License](https://img.shields.io/badge/License-BSD_3--Clause-
 blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\ [Open_In_Colab]  #
 Sports2D **`Sports2D` lets you compute 2D joint and segment angles from a
-video.**   [Content/demo_gif.gif] `Warning:` Angle estimation is only as good
-as the pose estimation algorithm, i.e., it is not perfect.\ `Warning:` Results
-are acceptable only if the persons move in the 2D plane, from right to left or
-from left to right.\ If you need research-grade markerless joint kinematics,
+video.** [Content/demo_gif.gif] `Warning:` Angle estimation is only as good as
+the pose estimation algorithm, i.e., it is not perfect.\ `Warning:` Results are
+acceptable only if the persons move in the 2D plane, from right to left or from
+left to right.\ If you need research-grade markerless joint kinematics,
 consider using several cameras, and constraining angles to a biomechanically
 accurate model. See [Pose2Sim](https://github.com/perfanalytics/pose2sim) for
-example. `Announcement:` Apps with GUI will be released for Windows, Linux,
-MacOS, as well as Android and iOS. Mobile versions will only support simple
-exploratory analysis. This involves single-person angle computation, in a
-potentially less accurate and tunable way. ## Contents 1. [Installation and
-Demonstration](#installation-and-demonstration) 1. [Installation]
-(#installation) 2. [Demonstration: Detect pose and compute 2D angles]
-(#demonstration-detect-pose-and-compute-2d-angles) 2. [Go further](#go-further)
-1. [Use on your own videos](#use-on-your-own-videos) 2. [Use OpenPose for
-multi-person, more accurate analysis](#use-openpose-for-multi-person-more-
-accurate-analysis) 3. [Advanced-settings](#advanced-settings) 4. [How it works]
-(#how-it-works) 3. [How to cite and how to contribute](#how-to-cite-and-how-to-
-contribute) ## Installation and Demonstration ### Installation - OPTION 1:
-**Quick install** \ Open a terminal. Type `python -V` to make sure python
-'>=3.7 <=3.10' is installed, and then: ``` pip install sports2d ``` - OPTION 2:
-**Safer install with Anaconda**\ Install [Miniconda](https://docs.conda.io/en/
-latest/miniconda.html):\ Open an Anaconda prompt and create a virtual
-environment by typing: ``` conda create -n Sports2D python<=3.10 conda activate
-Sports2D pip install sports2d ``` - OPTION 3: **Build from source and test the
-last changes**\ Open a terminal in the directory of your choice and clone the
-Sports2D repository. ``` git clone https://github.com/davidpagnon/sports2d.git
-cd sports2d pip install . ``` ### Demonstration: Detect pose and compute 2D
-angles Open a terminal, enter `pip show sports2d`, check sports2d package
-location. \ Copy this path and go to the Demo folder by typing `cd
-\Sports2D\Demo`. \ Type `ipython`, and test the following code: ``` from
-Sports2D import Sports2D Sports2D.detect_pose('Config_demo.toml')
-Sports2D.compute_angles('Config_demo.toml') ``` [Content/
+example. `Know issue`: Results won't be good with some iPhone videos in
+portrait mode. This is solved by priorly converting them with `ffmpeg -
+i video_input.mov video_output.mp4`, or even more simply with any random online
+video converter such as https://video-converter.com. `Announcement:` Apps with
+GUI will soon be released for Windows, Linux, MacOS, as well as Android and
+iOS. Mobile versions will only support simple exploratory analysis. This
+involves single-person angle computation, in a potentially less accurate and
+tunable way. ## Contents 1. [Installation and Demonstration](#installation-and-
+demonstration) 1. [Installation](#installation) 2. [Demonstration: Detect pose
+and compute 2D angles](#demonstration-detect-pose-and-compute-2d-angles) 2. [Go
+further](#go-further) 1. [Use on your own videos](#use-on-your-own-videos) 2.
+[Use OpenPose for multi-person, more accurate analysis](#use-openpose-for-
+multi-person-more-accurate-analysis) 3. [Advanced-settings](#advanced-settings)
+4. [How it works](#how-it-works) 3. [How to cite and how to contribute](#how-
+to-cite-and-how-to-contribute) ## Installation and Demonstration ###
+Installation - OPTION 1: **Quick install** \ Open a terminal. Type `python -V`
+to make sure python '>=3.7 <=3.10' is installed, and then: ``` pip install
+sports2d ``` - OPTION 2: **Safer install with Anaconda**\ Install [Miniconda]
+(https://docs.conda.io/en/latest/miniconda.html):\ Open an Anaconda prompt and
+create a virtual environment by typing: ``` conda create -n Sports2D
+python<=3.10 conda activate Sports2D pip install sports2d ``` - OPTION 3:
+**Build from source and test the last changes**\ Open a terminal in the
+directory of your choice and clone the Sports2D repository. ``` git clone
+https://github.com/davidpagnon/sports2d.git cd sports2d pip install . ``` ###
+Demonstration: Detect pose and compute 2D angles Open a terminal, enter `pip
+show sports2d`, check sports2d package location. \ Copy this path and go to the
+Demo folder by typing `cd \Sports2D\Demo`. \ Type `ipython`, and test the
+following code: ``` from Sports2D import Sports2D Sports2D.detect_pose
+('Config_demo.toml') Sports2D.compute_angles('Config_demo.toml') ``` [Content/
 demo_blazepose_terminal.png] You should obtain a video with the overlaid 2D
 joint positions, and angle text values. This output is also provided as an
 image folder.\ You should additionally obtain the same information as time
 series, stored in .csv files. These files can be opened with any spreadsheet
 software, or with the Pandas Python library for example.\ In addition, you will
 get the original OpenPose-like json coordinates files. [Content/
 demo_blazepose_results.png] ## Go further ### Use on your own videos 1. Copy-
```

### Comparing `sports2d-0.0.8/Sports2D/Demo/Config_demo.toml` & `sports2d-0.0.9/Sports2D/Demo/Config_demo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
    	
 	
 
 # ADVANCED CONFIGURATION
 	
 [pose_advanced] # only for OPENPOSE
-load_pose = false # else proceed to detection
+load_pose = true # proceeds to detection only if pose files not found
 save_vid = true
 save_img = true
 interp_gap_smaller_than = 5 # do not interpolate bigger gaps
 filter = true
 show_plots = false
 filter_type = 'butterworth' # butterworth, gaussian, LOESS, median
    [pose_advanced.butterworth]
```

### Comparing `sports2d-0.0.8/Sports2D/Demo/demo.mp4` & `sports2d-0.0.9/Sports2D/Demo/demo.mp4`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.8/Sports2D/Sports2D.py` & `sports2d-0.0.9/Sports2D/Sports2D.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,19 @@
 
     video_dir = Path(config_dict.get('project').get('video_dir')).resolve()
     if video_dir == '': video_dir = os.getcwd()
     video_file = Path(config_dict.get('project').get('video_file'))
     
     video = cv2.VideoCapture(str(video_dir / video_file))
     frame_rate = video.get(cv2.CAP_PROP_FPS)
+    try:
+        1/frame_rate
+    except ZeroDivisionError:
+        print('Frame rate could not be retrieved: check that your video exists at the correct path')
+        raise
     video.release()
 
     return video_dir, video_file, frame_rate
 
 
 def detect_pose(config='Config_demo.toml'):
     '''
```

### Comparing `sports2d-0.0.8/Sports2D/Utilities/Blazepose_runsave.py` & `sports2d-0.0.9/Sports2D/Utilities/Blazepose_runsave.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.8/Sports2D/Utilities/common.py` & `sports2d-0.0.9/Sports2D/Utilities/common.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.8/Sports2D/Utilities/filter.py` & `sports2d-0.0.9/Sports2D/Utilities/filter.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.8/Sports2D/Utilities/skeletons.py` & `sports2d-0.0.9/Sports2D/Utilities/skeletons.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.0.8/Sports2D/compute_angles.py` & `sports2d-0.0.9/Sports2D/compute_angles.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,22 +294,24 @@
                 (np.array(cmap((i+1)/len(df_angles_list_frame)))*255).tolist(), 
                 1, 
                 cv2.LINE_4)
             # Progress bar
             x_ang = int(angles_frame_person[ang_nb]*50/180)
             if x_ang > 0:
                 sub_frame = frame[ 1+15*ang_nb : 16+15*ang_nb , 170+250*i : 170+250*i+x_ang ]
-                white_rect = np.ones(sub_frame.shape, dtype=np.uint8) * 255
-                res = cv2.addWeighted(sub_frame, 0.6, white_rect, 0.4, 1.0)
-                frame[ 1+15*ang_nb : 16+15*ang_nb , 170+250*i : 170+250*i+x_ang ] = res
+                if sub_frame.size>0:
+                    white_rect = np.ones(sub_frame.shape, dtype=np.uint8) * 255
+                    res = cv2.addWeighted(sub_frame, 0.6, white_rect, 0.4, 1.0)
+                    frame[ 1+15*ang_nb : 16+15*ang_nb , 170+250*i : 170+250*i+x_ang ] = res
             elif x_ang < 0:
                 sub_frame = frame[ 1+15*ang_nb : 16+15*ang_nb , 170+250*i+x_ang : 170+250*i ]
-                white_rect = np.ones(sub_frame.shape, dtype=np.uint8) * 255
-                res = cv2.addWeighted(sub_frame, 0.6, white_rect, 0.4, 1.0)
-                frame[ 1+15*ang_nb : 16+15*ang_nb , 170+250*i+x_ang : 170+250*i ] = res
+                if sub_frame.size>0:
+                    white_rect = np.ones(sub_frame.shape, dtype=np.uint8) * 255
+                    res = cv2.addWeighted(sub_frame, 0.6, white_rect, 0.4, 1.0)
+                    frame[ 1+15*ang_nb : 16+15*ang_nb , 170+250*i+x_ang : 170+250*i ] = res
         
     return frame
     
     
 def compute_angles_fun(config_dict):
     '''
     Compute joint and segment angles from csv position files.
```

### Comparing `sports2d-0.0.8/Sports2D/detect_pose.py` & `sports2d-0.0.9/Sports2D/detect_pose.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     - video_path: Path of the video to analyze
     - json_path: Path of the directory where to save json files
     - pose_model: string. "BODY_25B", "BODY_25", or others.
           
     OUTPUTS:
     - json files in json_path
     '''
-
+    
     subprocess.run(["./build/examples/openpose/openpose.bin", "--video", video_path, \
     "--model_pose", pose_model, \
     "--write_json", json_path, \
     "--render_pose", "0", "--display", "0"])
 
 
 def run_openpose_mac(video_path, json_path, pose_model):
@@ -281,15 +281,15 @@
         
     # Retrieve keypoint names from model
     model = eval(pose_model)
     keypoints_ids = [node.id for _, _, node in RenderTree(model) if node.id!=None]
     keypoints_names = [node.name for _, _, node in RenderTree(model) if node.id!=None]
     keypoints_names_rearranged = [y for x,y in sorted(zip(keypoints_ids,keypoints_names))]
     keypoints_nb = len(keypoints_ids)
-       
+
     # Retrieve coordinates
     logging.info('Sorting people across frames.')
     json_fnames = list(json_path.glob('*.json'))
     nb_persons_to_detect = max([len(json.load(open(json_fname))['people']) for json_fname in json_fnames])
     Coords = [np.array([]).reshape(0,keypoints_nb*3)] * nb_persons_to_detect
     for json_fname in json_fnames:    # for each frame
         with open(json_fname) as json_f:
@@ -298,15 +298,15 @@
             # Retrieve coords for this frame 
             for ppl in range(len(json_file['people'])):  # for each detected person
                 keypt += [np.asarray(json_file['people'][ppl]['pose_keypoints_2d']).reshape(-1,3)]
             keypt = np.array(keypt)
             # Make sure keypt is as large as the number of persons that need to be detected
             if len(keypt) < nb_persons_to_detect:
                 empty_keypt_to_add = np.concatenate( [[ np.zeros([25,3]) ]] * (nb_persons_to_detect-len(keypt)) )
-                keypt = np.concatenate([keypt, empty_keypt_to_add])
+                keypt = [np.concatenate([keypt, empty_keypt_to_add]) if keypt!=[] else empty_keypt_to_add][0]
             if 'keyptpre' not in locals():
                 keyptpre = keypt
             # Associate persons across frames
             keypt = sort_people(keyptpre, keypt, nb_persons_to_detect)
             # Concatenate to coordinates of previous frames
             for i in range(nb_persons_to_detect): 
                 Coords[i] = np.vstack([Coords[i], keypt[i].reshape(-1)])
@@ -376,23 +376,23 @@
     
     # Draw rectangles
     [cv2.rectangle(img, 
         (np.nanmin(x).astype(int)-25, np.nanmin(y).astype(int)-25), 
         (np.nanmax(x).astype(int)+25, np.nanmax(y).astype(int)+25), 
         (np.array(cmap((i+1)/len(X)))*255).tolist(), 
         2) 
-        for i,(x,y) in enumerate(zip(X,Y))]
+        for i,(x,y) in enumerate(zip(X,Y)) if not np.isnan(x).all()]
  
     # Write person ID
     [cv2.putText(img, str(i),
         (np.nanmin(x).astype(int), np.nanmin(y).astype(int)), 
         cv2.FONT_HERSHEY_SIMPLEX, 1,
         (np.array(cmap((i+1)/len(X)))*255).tolist(),
         2, cv2.LINE_AA) 
-        for i,(x,y) in enumerate(zip(X,Y))]
+        for i,(x,y) in enumerate(zip(X,Y)) if not np.isnan(x).all()]
     
     return img
 
 
 def draw_keypts_skel(X, Y, img, *pose_model):
     '''
     Draws keypoints and optionally skeleton for each person
@@ -556,20 +556,20 @@
     butterworth_filter_cutoff = config_dict.get('pose_advanced').get('butterworth').get('cut_off_frequency')
     gaussian_filter_kernel = config_dict.get('pose_advanced').get('gaussian').get('sigma_kernel')
     loess_filter_kernel = config_dict.get('pose_advanced').get('loess').get('nb_values_used')
     median_filter_kernel = config_dict.get('pose_advanced').get('median').get('kernel_size')
     filter_options = (do_filter, filter_type, butterworth_filter_order, butterworth_filter_cutoff, frame_rate, gaussian_filter_kernel, loess_filter_kernel, median_filter_kernel)
     
     video_file_stem = video_file.stem
-    video_path = video_dir / video_file
+    video_path = (video_dir / video_file)
 
     if pose_algo == 'OPENPOSE':
         pose_model = config_dict.get('pose').get('OPENPOSE').get('openpose_model')
         json_path = video_dir / '_'.join((video_file_stem,pose_model,'json'))
-        
+
         # Pose detection skipped if load existing json files
         if load_pose and len(list(json_path.glob('*')))>0:
             pass
         else:
             logging.info(f'Detecting 2D joint positions with OpenPose model {pose_model}, for {video_file}.')
             json_path.mkdir(parents=True, exist_ok=True)
             openpose_path = config_dict.get('pose').get('OPENPOSE').get('openpose_path')
```

### Comparing `sports2d-0.0.8/setup.cfg` & `sports2d-0.0.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sports2d
-version = 0.0.8
+version = 0.0.9
 author = David Pagnon
 author_email = contact@david-pagnon.com
 description = Detect pose and compute 2D joint angles from a video.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/davidpagnon/Sports2D
 keywords = markerless, kinematics, OpenPose, BlazePose, joint angles, 2D, biomechanics, sports, sports-analytics
```

### Comparing `sports2d-0.0.8/sports2d.egg-info/PKG-INFO` & `sports2d-0.0.9/sports2d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports2d
-Version: 0.0.8
+Version: 0.0.9
 Summary: Detect pose and compute 2D joint angles from a video.
 Home-page: https://github.com/davidpagnon/Sports2D
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
 Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics,sports,sports-analytics
@@ -39,24 +39,23 @@
 -->
 
 
 # Sports2D
 
 **`Sports2D` lets you compute 2D joint and segment angles from a video.**
 
- </br>
- </br>
-
 <img src='Content/demo_gif.gif' title='Demonstration of Sports2D with OpenPose.'  width="760">
 
 `Warning:` Angle estimation is only as good as the pose estimation algorithm, i.e., it is not perfect.\
 `Warning:` Results are acceptable only if the persons move in the 2D plane, from right to left or from left to right.\
 If you need research-grade markerless joint kinematics, consider using several cameras, and constraining angles to a biomechanically accurate model. See [Pose2Sim](https://github.com/perfanalytics/pose2sim) for example.
 
-`Announcement:` Apps with GUI will be released for Windows, Linux, MacOS, as well as Android and iOS.
+`Know issue`: Results won't be good with some iPhone videos in portrait mode. This is solved by priorly converting them with `ffmpeg -i video_input.mov video_output.mp4`, or even more simply with any random online video converter such as https://video-converter.com.
+
+`Announcement:` Apps with GUI will soon be released for Windows, Linux, MacOS, as well as Android and iOS.
 Mobile versions will only support simple exploratory analysis. This involves single-person angle computation, in a potentially less accurate and tunable way.
 
 
 ## Contents
 1. [Installation and Demonstration](#installation-and-demonstration)
    1. [Installation](#installation)
    2. [Demonstration: Detect pose and compute 2D angles](#demonstration-detect-pose-and-compute-2d-angles)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sports2d Version: 0.0.8 Summary: Detect pose and
+Metadata-Version: 2.1 Name: sports2d Version: 0.0.9 Summary: Detect pose and
 compute 2D joint angles from a video. Home-page: https://github.com/
 davidpagnon/Sports2D Author: David Pagnon Author-email: contact@david-
 pagnon.com License: BSD 3-Clause License Project-URL: Bug Tracker, https://
 github.com/davidpagnon/Sports2D/issues Keywords:
 markerless,kinematics,OpenPose,BlazePose,joint
 angles,2D,biomechanics,sports,sports-analytics Platform: any Classifier:
 Programming Language :: Python :: 3 Classifier: Development Status :: 3 - Alpha
@@ -17,46 +17,49 @@
 [Continuous integration](https://github.com/davidpagnon/sports2d/actions/
 workflows/continuous-integration.yml/badge.svg?branch=main)](https://
 github.com/davidpagnon/sports2d/actions/workflows/continuous-integration.yml)
 [![PyPI version](https://badge.fury.io/py/Sports2D.svg)](https://badge.fury.io/
 py/Sports2D)\ [![License](https://img.shields.io/badge/License-BSD_3--Clause-
 blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\ [Open_In_Colab]  #
 Sports2D **`Sports2D` lets you compute 2D joint and segment angles from a
-video.**   [Content/demo_gif.gif] `Warning:` Angle estimation is only as good
-as the pose estimation algorithm, i.e., it is not perfect.\ `Warning:` Results
-are acceptable only if the persons move in the 2D plane, from right to left or
-from left to right.\ If you need research-grade markerless joint kinematics,
+video.** [Content/demo_gif.gif] `Warning:` Angle estimation is only as good as
+the pose estimation algorithm, i.e., it is not perfect.\ `Warning:` Results are
+acceptable only if the persons move in the 2D plane, from right to left or from
+left to right.\ If you need research-grade markerless joint kinematics,
 consider using several cameras, and constraining angles to a biomechanically
 accurate model. See [Pose2Sim](https://github.com/perfanalytics/pose2sim) for
-example. `Announcement:` Apps with GUI will be released for Windows, Linux,
-MacOS, as well as Android and iOS. Mobile versions will only support simple
-exploratory analysis. This involves single-person angle computation, in a
-potentially less accurate and tunable way. ## Contents 1. [Installation and
-Demonstration](#installation-and-demonstration) 1. [Installation]
-(#installation) 2. [Demonstration: Detect pose and compute 2D angles]
-(#demonstration-detect-pose-and-compute-2d-angles) 2. [Go further](#go-further)
-1. [Use on your own videos](#use-on-your-own-videos) 2. [Use OpenPose for
-multi-person, more accurate analysis](#use-openpose-for-multi-person-more-
-accurate-analysis) 3. [Advanced-settings](#advanced-settings) 4. [How it works]
-(#how-it-works) 3. [How to cite and how to contribute](#how-to-cite-and-how-to-
-contribute) ## Installation and Demonstration ### Installation - OPTION 1:
-**Quick install** \ Open a terminal. Type `python -V` to make sure python
-'>=3.7 <=3.10' is installed, and then: ``` pip install sports2d ``` - OPTION 2:
-**Safer install with Anaconda**\ Install [Miniconda](https://docs.conda.io/en/
-latest/miniconda.html):\ Open an Anaconda prompt and create a virtual
-environment by typing: ``` conda create -n Sports2D python<=3.10 conda activate
-Sports2D pip install sports2d ``` - OPTION 3: **Build from source and test the
-last changes**\ Open a terminal in the directory of your choice and clone the
-Sports2D repository. ``` git clone https://github.com/davidpagnon/sports2d.git
-cd sports2d pip install . ``` ### Demonstration: Detect pose and compute 2D
-angles Open a terminal, enter `pip show sports2d`, check sports2d package
-location. \ Copy this path and go to the Demo folder by typing `cd
-\Sports2D\Demo`. \ Type `ipython`, and test the following code: ``` from
-Sports2D import Sports2D Sports2D.detect_pose('Config_demo.toml')
-Sports2D.compute_angles('Config_demo.toml') ``` [Content/
+example. `Know issue`: Results won't be good with some iPhone videos in
+portrait mode. This is solved by priorly converting them with `ffmpeg -
+i video_input.mov video_output.mp4`, or even more simply with any random online
+video converter such as https://video-converter.com. `Announcement:` Apps with
+GUI will soon be released for Windows, Linux, MacOS, as well as Android and
+iOS. Mobile versions will only support simple exploratory analysis. This
+involves single-person angle computation, in a potentially less accurate and
+tunable way. ## Contents 1. [Installation and Demonstration](#installation-and-
+demonstration) 1. [Installation](#installation) 2. [Demonstration: Detect pose
+and compute 2D angles](#demonstration-detect-pose-and-compute-2d-angles) 2. [Go
+further](#go-further) 1. [Use on your own videos](#use-on-your-own-videos) 2.
+[Use OpenPose for multi-person, more accurate analysis](#use-openpose-for-
+multi-person-more-accurate-analysis) 3. [Advanced-settings](#advanced-settings)
+4. [How it works](#how-it-works) 3. [How to cite and how to contribute](#how-
+to-cite-and-how-to-contribute) ## Installation and Demonstration ###
+Installation - OPTION 1: **Quick install** \ Open a terminal. Type `python -V`
+to make sure python '>=3.7 <=3.10' is installed, and then: ``` pip install
+sports2d ``` - OPTION 2: **Safer install with Anaconda**\ Install [Miniconda]
+(https://docs.conda.io/en/latest/miniconda.html):\ Open an Anaconda prompt and
+create a virtual environment by typing: ``` conda create -n Sports2D
+python<=3.10 conda activate Sports2D pip install sports2d ``` - OPTION 3:
+**Build from source and test the last changes**\ Open a terminal in the
+directory of your choice and clone the Sports2D repository. ``` git clone
+https://github.com/davidpagnon/sports2d.git cd sports2d pip install . ``` ###
+Demonstration: Detect pose and compute 2D angles Open a terminal, enter `pip
+show sports2d`, check sports2d package location. \ Copy this path and go to the
+Demo folder by typing `cd \Sports2D\Demo`. \ Type `ipython`, and test the
+following code: ``` from Sports2D import Sports2D Sports2D.detect_pose
+('Config_demo.toml') Sports2D.compute_angles('Config_demo.toml') ``` [Content/
 demo_blazepose_terminal.png] You should obtain a video with the overlaid 2D
 joint positions, and angle text values. This output is also provided as an
 image folder.\ You should additionally obtain the same information as time
 series, stored in .csv files. These files can be opened with any spreadsheet
 software, or with the Pandas Python library for example.\ In addition, you will
 get the original OpenPose-like json coordinates files. [Content/
 demo_blazepose_results.png] ## Go further ### Use on your own videos 1. Copy-
```

### Comparing `sports2d-0.0.8/sports2d.egg-info/SOURCES.txt` & `sports2d-0.0.9/sports2d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

