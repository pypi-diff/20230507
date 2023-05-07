# Comparing `tmp/ukmon_meteortools-2023.5.7.tar.gz` & `tmp/ukmon_meteortools-2023.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukmon_meteortools-2023.5.7.tar", last modified: Thu May  4 20:28:53 2023, max compression
+gzip compressed data, was "ukmon_meteortools-2023.5.8.tar", last modified: Sun May  7 14:40:23 2023, max compression
```

## Comparing `ukmon_meteortools-2023.5.7.tar` & `ukmon_meteortools-2023.5.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 20:28:53.152884 ukmon_meteortools-2023.5.7/
--rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.5.7/LICENSE
--rw-rw-rw-   0        0        0    42659 2023-05-04 20:28:53.151883 ukmon_meteortools-2023.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.5.7/README.md
--rw-rw-rw-   0        0        0     2185 2023-05-04 20:28:30.000000 ukmon_meteortools-2023.5.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 20:28:53.152884 ukmon_meteortools-2023.5.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-04 20:28:53.056884 ukmon_meteortools-2023.5.7/ukmon_meteortools/
--rw-rw-rw-   0        0        0      756 2023-05-02 21:24:36.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 20:28:53.093883 ukmon_meteortools-2023.5.7/ukmon_meteortools/fileformats/
--rw-rw-rw-   0        0        0     2372 2023-05-04 20:03:03.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/fileformats/ECSVhandler.py
--rw-rw-rw-   0        0        0    10159 2023-05-02 20:41:26.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/fileformats/UFOAnalyzerXML.py
--rw-rw-rw-   0        0        0     6742 2023-05-02 20:41:44.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/fileformats/UFOCapXML.py
--rw-rw-rw-   0        0        0      520 2023-05-04 19:41:10.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/fileformats/__init__.py
--rw-rw-rw-   0        0        0    19245 2023-05-04 20:26:21.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/fileformats/ftpDetectInfo.py
--rw-rw-rw-   0        0        0     7393 2023-05-02 21:34:25.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/fileformats/imoWorkingShowerList.py
--rw-rw-rw-   0        0        0     3642 2023-05-04 19:26:25.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/fileformats/kmlHandlers.py
--rw-rw-rw-   0        0        0     2948 2023-05-02 20:46:56.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/fileformats/platepar.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:28:53.106883 ukmon_meteortools-2023.5.7/ukmon_meteortools/rmsutils/
--rw-rw-rw-   0        0        0      720 2023-05-04 19:42:49.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/rmsutils/__init__.py
--rw-rw-rw-   0        0        0     1909 2023-05-02 20:41:57.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
--rw-rw-rw-   0        0        0     6077 2023-05-02 20:34:59.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/rmsutils/multiDayRadiant.py
--rw-rw-rw-   0        0        0     3763 2023-05-02 20:35:34.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/rmsutils/multiEventGroundMap.py
--rw-rw-rw-   0        0        0     5242 2023-05-03 14:21:56.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/rmsutils/multiTrackStack.py
--rw-rw-rw-   0        0        0     2297 2023-05-02 20:31:43.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
--rw-rw-rw-   0        0        0     2281 2023-05-02 20:31:31.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/rmsutils/plotRMSOrbits.py
--rw-rw-rw-   0        0        0     1439 2023-05-04 19:30:59.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/rmsutils/trajPickle.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:28:53.111885 ukmon_meteortools-2023.5.7/ukmon_meteortools/share/
--rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
--rw-rw-rw-   0        0        0      525 2023-05-02 21:29:15.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/share/__init__.py
--rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/share/streamfulldata.npy
-drwxrwxrwx   0        0        0        0 2023-05-04 20:28:53.134885 ukmon_meteortools-2023.5.7/ukmon_meteortools/usertools/
--rw-rw-rw-   0        0        0      444 2023-05-04 19:36:38.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/usertools/__init__.py
--rw-rw-rw-   0        0        0     2945 2023-05-04 15:03:26.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/usertools/apiExampleCode.py
--rw-rw-rw-   0        0        0     1420 2023-03-08 12:49:12.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/usertools/findNearDuplicates.py
--rw-rw-rw-   0        0        0     4372 2023-05-04 16:56:04.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/usertools/getLiveImages.py
--rw-rw-rw-   0        0        0     3244 2023-05-04 19:33:10.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/usertools/getOverlappingFovs.py
--rw-rw-rw-   0        0        0     3589 2023-05-02 20:20:03.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/usertools/plotTrack.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:28:53.149883 ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/
--rw-rw-rw-   0        0        0    13798 2023-05-02 20:57:25.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/Math.py
--rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/VectorMaths.py
--rw-rw-rw-   0        0        0     1296 2023-05-04 20:12:42.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/__init__.py
--rw-rw-rw-   0        0        0     2519 2023-05-02 21:35:02.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/annotateImage.py
--rw-rw-rw-   0        0        0     1313 2023-05-02 21:35:22.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/convertSolLon.py
--rw-rw-rw-   0        0        0     2476 2023-05-02 20:12:42.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/drawFTPfile.py
--rw-rw-rw-   0        0        0     2114 2023-05-02 21:35:49.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/getActiveShowers.py
--rw-rw-rw-   0        0        0     3937 2023-05-02 21:41:36.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/getShowerDates.py
--rw-rw-rw-   0        0        0     3699 2023-05-02 20:49:10.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/sendAnEmail.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:28:53.082886 ukmon_meteortools-2023.5.7/ukmon_meteortools.egg-info/
--rw-rw-rw-   0        0        0    42659 2023-05-04 20:28:53.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1752 2023-05-04 20:28:53.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 20:28:53.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      257 2023-05-04 20:28:53.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-04 20:28:53.000000 ukmon_meteortools-2023.5.7/ukmon_meteortools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 14:40:23.810953 ukmon_meteortools-2023.5.8/
+-rw-rw-rw-   0        0        0    35149 2020-04-29 17:18:36.000000 ukmon_meteortools-2023.5.8/LICENSE
+-rw-rw-rw-   0        0        0    42725 2023-05-07 14:40:23.806938 ukmon_meteortools-2023.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1063 2023-04-12 22:46:43.000000 ukmon_meteortools-2023.5.8/README.md
+-rw-rw-rw-   0        0        0     2364 2023-05-07 14:39:47.000000 ukmon_meteortools-2023.5.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 14:40:23.810953 ukmon_meteortools-2023.5.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 14:40:23.577939 ukmon_meteortools-2023.5.8/ukmon_meteortools/
+-rw-rw-rw-   0        0        0      819 2023-05-07 12:44:14.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 14:40:23.676939 ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/
+-rw-rw-rw-   0        0        0     2043 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/ECSVhandler.py
+-rw-rw-rw-   0        0        0     8691 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/UFOAnalyzerXML.py
+-rw-rw-rw-   0        0        0     6742 2023-05-02 20:41:44.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/UFOCapXML.py
+-rw-rw-rw-   0        0        0      520 2023-05-04 19:41:10.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/__init__.py
+-rw-rw-rw-   0        0        0    18716 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/ftpDetectInfo.py
+-rw-rw-rw-   0        0        0     7393 2023-05-02 21:34:25.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/imoWorkingShowerList.py
+-rw-rw-rw-   0        0        0     4018 2023-05-05 17:15:20.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/kmlHandlers.py
+-rw-rw-rw-   0        0        0     2815 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/platepar.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:40:23.712940 ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/
+-rw-rw-rw-   0        0        0      733 2023-05-05 16:11:22.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/__init__.py
+-rw-rw-rw-   0        0        0     1909 2023-05-02 20:41:57.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py
+-rw-rw-rw-   0        0        0     6077 2023-05-05 15:40:18.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/multiDayRadiant.py
+-rw-rw-rw-   0        0        0     3763 2023-05-02 20:35:34.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/multiEventGroundMap.py
+-rw-rw-rw-   0        0        0     5242 2023-05-05 16:20:15.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/multiTrackStack.py
+-rw-rw-rw-   0        0        0     2297 2023-05-02 20:31:43.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/plotCAMSOrbits.py
+-rw-rw-rw-   0        0        0     2281 2023-05-02 20:31:31.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/plotRMSOrbits.py
+-rw-rw-rw-   0        0        0     3187 2023-05-05 17:16:29.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/trajPickle.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:40:23.718939 ukmon_meteortools-2023.5.8/ukmon_meteortools/share/
+-rw-rw-rw-   0        0        0     8977 2023-04-18 21:24:56.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml
+-rw-rw-rw-   0        0        0      525 2023-05-02 21:29:15.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/share/__init__.py
+-rw-rw-rw-   0        0        0  5702528 2023-04-18 21:40:34.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/share/streamfulldata.npy
+drwxrwxrwx   0        0        0        0 2023-05-07 14:40:23.769945 ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/
+-rw-rw-rw-   0        0        0      444 2023-05-04 19:36:38.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/__init__.py
+-rw-rw-rw-   0        0        0     3164 2023-05-06 20:43:49.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/apiExampleCode.py
+-rw-rw-rw-   0        0        0     1420 2023-03-08 12:49:12.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/findNearDuplicates.py
+-rw-rw-rw-   0        0        0     4298 2023-05-06 21:27:34.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/getLiveImages.py
+-rw-rw-rw-   0        0        0     3085 2023-05-06 21:17:26.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/getOverlappingFovs.py
+-rw-rw-rw-   0        0        0     3429 2023-05-06 20:51:39.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/plotTrack.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:40:23.804949 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/
+-rw-rw-rw-   0        0        0    13798 2023-05-02 20:57:25.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/Math.py
+-rw-rw-rw-   0        0        0      512 2023-04-29 16:53:34.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/VectorMaths.py
+-rw-rw-rw-   0        0        0     1296 2023-05-04 20:12:42.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/__init__.py
+-rw-rw-rw-   0        0        0     2519 2023-05-02 21:35:02.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/annotateImage.py
+-rw-rw-rw-   0        0        0     1313 2023-05-02 21:35:22.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/convertSolLon.py
+-rw-rw-rw-   0        0        0     2393 2023-05-07 12:29:44.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/drawFTPfile.py
+-rw-rw-rw-   0        0        0     2105 2023-05-07 14:36:01.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/getActiveShowers.py
+-rw-rw-rw-   0        0        0     3937 2023-05-02 21:41:36.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/getShowerDates.py
+-rw-rw-rw-   0        0        0     3699 2023-05-02 20:49:10.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/sendAnEmail.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:40:23.646941 ukmon_meteortools-2023.5.8/ukmon_meteortools.egg-info/
+-rw-rw-rw-   0        0        0    42725 2023-05-07 14:40:23.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1752 2023-05-07 14:40:23.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 14:40:23.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      353 2023-05-07 14:40:23.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-07 14:40:23.000000 ukmon_meteortools-2023.5.8/ukmon_meteortools.egg-info/top_level.txt
```

### Comparing `ukmon_meteortools-2023.5.7/LICENSE` & `ukmon_meteortools-2023.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/PKG-INFO` & `ukmon_meteortools-2023.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon_meteortools
-Version: 2023.5.7
+Version: 2023.5.8
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,15 +674,15 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://github.com/markmac99/UKMon-shared/ukmon_meteortools/
+Project-URL: Homepage, https://markmac99.github.io/UKmon-shared/ukmon_meteortools.html
 Project-URL: Bug Tracker, https://github.com/markmac99/UKMon-shared/issues
 Keywords: meteors,ukmon
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
@@ -690,25 +690,26 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # ukmon_meteortools
 
 Python tools and utilities to work with meteor data from the UK Meteor Network
 
-To get more information about the submodules and functions use Python's built-in help capability
+To get more information about the submodules and functions use Python's built-in help capability, for example
+as shown here. 
 
 ``` python
 from ukmon_meteortools import utils
 help(utils)
 help(utils.sendAnEmail)
 ```
 
 Example usage 
 ```python
->>>from ukmon_meteortools.utils import date2JD, jd2LST
+>>>from ukmon_meteortools.utils import date2JD, jd2LST, getActiveShowers, getShowerDets
 >>> date2JD(2023,4,11,12,45,9)
 2460046.0313541666
 >>>import numpy as np
 >>> jd2LST(2460046.0313541666, lon=np.radians(-1.31))
 (30.741774823384617, 30.76463863658577)
 >>> import datetime
 >>> getActiveShowers(datetime.datetime.now())
```

### Comparing `ukmon_meteortools-2023.5.7/README.md` & `ukmon_meteortools-2023.5.8/README.md`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/pyproject.toml` & `ukmon_meteortools-2023.5.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ukmon_meteortools"
-version = "2023.05.7"
+version = "2023.05.8"
 description = "Python Tools for Meteor Data Analysis"
 readme = "ukmon_meteortools/README.md"
 authors = [{ name = "Mark McIntyre", email = "ukmon@markmcintyreastro.co.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -35,23 +35,33 @@
     "Shapely",
     "simplekml",
     "s3fs",
     "xmltodict",
     "requests",
     "pyproj",
     "pdoc",
-    "Cython"
+    "Cython",
+    "opencv-python",
+    "imageio",
+    "scipy",
+    "jplephem",
+    "pyephem",
+    "gitpython",
+    "astropy",
+    "pyqt5",
+    "basemap",
+    "basemap-data-hires"
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 dev = ["bumpver", "gitpython", "behave", "pytest", "pip-tools"]
 
 [project.urls]
-"Homepage" = "https://github.com/markmac99/UKMon-shared/ukmon_meteortools/"
+"Homepage" = "https://markmac99.github.io/UKmon-shared/ukmon_meteortools.html"
 "Bug Tracker" = "https://github.com/markmac99/UKMon-shared/issues"
 
 #[project.scripts]
 #realpython = "reader.__main__:main"
 
 [tool.setuptools]
 #package-dir = {"" = "ukmon_pylib"}
@@ -62,15 +72,15 @@
 #[tool.setuptools.packages.find]
 #where = ["ukmon_meteortools"]
 
 [tool.setuptools.package-data]
 "*" = ["*.npy", "*.xml"]
 
 [tool.bumpver]
-current_version = "2023.05.7"
+current_version = "2023.05.8"
 version_pattern = "YYYY.0M.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/fileformats/ECSVhandler.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/ECSVhandler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 
 import requests
-import sys
 import os
 
 
 def getECSVs(stationID, dateStr, savefiles=False, outdir='.'):
     """
     Retrieve a detection in ECSV format for the specified date  
 
@@ -44,22 +43,7 @@
                             print('saving to ', fnamebase + f'_M{j:03d}.ecsv')
                         outf.write(f'{ecsvlines[i]}\n')
         else:
             print('no error, but no data returned')
     else:
         print(res.status_code)
     return ecsvlines
-
-
-if __name__ == '__main__':
-    sav = True
-    if len(sys.argv) < 3:
-        stat ='UK0025'
-        dt = '2021-07-17T02:41:05.05'
-    else:
-        stat = sys.argv[1]
-        dt = sys.argv[2]
-        if len(sys.argv) == 4:
-            if int(sys.argv[3]) ==0:
-                sav = False
-
-    getECSVs(stat, dt, sav)
```

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/fileformats/UFOAnalyzerXML.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/UFOAnalyzerXML.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #  A class to handle UFO Analyser xml files
 # Copyright (C) 2018-2023 Mark McIntyre
 
-import sys
 import xmltodict
 import datetime
 import math
 import numpy
 from ukmon_meteortools.utils import datetime2JD, altAz2RADec
 
 
@@ -227,43 +226,7 @@
         pp = pp + '    "Ho": 0,\n'
         pp = pp + '    "UT_corr": 0,\n'
         pp = pp + '    "F_scale": 0,\n'
         pp = pp + '    "version": 2\n'
         pp = pp + '}'
 
         return pp
-
-
-if __name__ == '__main__':
-    dd = UAXml(sys.argv[1])
-
-    dtim = dd.getDateTime()
-
-    station, lid, sid, lat, lng, alti = dd.getStationDetails()
-    fps, cx, cy, isintl = dd.getCameraDetails()
-    print('location', station, lat, lng, alti)
-    print('date ', dtim, '\nand path')
-    if isintl == 1:
-        fps = fps * 2
-    # print('camera', fps, cx, cy)
-    # az, ev, rot, fovh, yx, dx, dy, lnk = dd.getProfDetails()
-    # print('profile', az, ev, rot, fovh, yx, dx, dy, lnk)
-
-    pp = dd.makePlateParEntry('XX0000')
-    print(pp)
-    nobjs = dd.getObjectCount()
-    for i in range(nobjs):
-        sec, av, pix, bmax, mag, fcount = dd.getObjectBasics(i)
-        ra1, dc1, h1, dist1, lng1, lat1, az1, ev1, fs = dd.getObjectStart(i)
-        ra2, dc2, h2, dist2, lng2, lat2, fe = dd.getObjectEnd(i)
-        print(sec, ra1, dc1, h1, dist1, lng1, lat1, ra2, dc2, h2, dist2, lng2, lat2)
-        print(fcount)
-        print('fno', 'ra', 'dec', 'mag', 'az', 'ev', 'lsum', 'b')
-        for j in range(fcount):
-            fno, ra, dec, mag, az, ev, lsum, b = dd.getObjectFrameDetails(i, j)
-            us = int(fno / fps * 1000000)
-            tt = dtim + datetime.timedelta(microseconds=us)
-            print(tt, fno, ra, dec, mag, az, ev, lsum, b)
-        fno, tt, ra, dec, mag, fcount, alt, az, b, lsum = dd.getPathVector(i)
-        for j in range(fcount):
-            print(datetime.datetime.fromtimestamp(tt[j]), ra[j], dec[j], fno[j])
-    print('done')
```

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/fileformats/UFOCapXML.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/UFOCapXML.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/fileformats/__init__.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/fileformats/ftpDetectInfo.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/ftpDetectInfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #
 # Load an FTPdetectInfo file - copied from RMS
 #
 # Copyright (C) 2018-2023 Mark McIntyre
 
-import sys
 import os
 import numpy as np
 import configparser as crp
 import json
 import datetime
 
 from ukmon_meteortools.utils import date2JD, angleBetweenSphericalCoords
@@ -500,21 +499,7 @@
             thisfn = fno[i]
             thisx = x[i]
             thisy = y[i]
         li = f'{thisfn:.4f} {thisx:07.2f} {thisy:07.2f} '
         li = li + f'{ra[i]:8.4f} {dec[i]:+7.4f} {az[i]:8.4f} '
         li = li + f'{alt[i]:+7.4f} {bri:06d} {mag[i]:.02f}\n'
         ftpf.write(li)
-
-
-if __name__ == '__main__':
-    if len(sys.argv) < 1:
-        print('usage: python ftpDetectInfo.py ftpfile')
-        print('note: requires .config and platepar to be in the same folder')
-        exit(0)
-        
-    ftpname = sys.argv[1]
-    metlist = loadFTPDetectInfo(sys.argv[1])
-    m1 = metlist[0]
-    print(m1.jdt_ref, m1.ff_name)
-    for f,t,r,d,a,e,x,y,m in zip(m1.frames,m1.time_data, m1.ra_data, m1.dec_data, m1.azim_data, m1.elev_data, m1.x_data, m1.y_data, m1.mag_data):
-        print(f,t,r,d,a,e,x,y,m)
```

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/fileformats/imoWorkingShowerList.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/imoWorkingShowerList.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/fileformats/kmlHandlers.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/kmlHandlers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import xmltodict
 from shapely.geometry import Polygon
 import csv
 import simplekml
 import numpy as np
 import pandas as pd
+import os
 
 
 def munchKML(kmlFilename, return_poly=False):
     """ Load a KML file and return either a list of lats and longs, or a Shapely polygon  
     
     Arguments:  
         kmlFilename:    [string] full path to the KML file to consume   
@@ -39,40 +40,48 @@
             for lin in coords:
                 s = lin.split(',')
                 ptsarr.append((float(s[0]), float(s[1])))
             polyg = Polygon(ptsarr)
             return cname, polyg 
 
 
-def trackCsvtoKML(trackcsvfile, trackdata=None, saveOutput=True):
+def trackCsvtoKML(trackcsvfile, trackdata=None, saveOutput=True, outdir=None):
     """ 
-    Either reads a CSV file containing lat, long, height, time of an event and 
+    Either reads a CSV file containing lat, long, height of an event and 
     creates a 3d KML file from it or, if trackdata is populated, converts a Pandas dataframe containing 
     the same data. Output is written to disk unless saveOutput is false.  
     
     Arguments:  
         trackcsvfile:   [string] full path to the file to read from  
         trackdata:      [array] pandas dataframe containing the data. Default None  
         saveOutput:     [bool] write the KML file to disk. Default true  
+        outdir:         [string] where to save the file. Default same folder as the source file
 
     Returns:  
         the KML file as a tuple  
         """
     kml=simplekml.Kml()
     kml.document.name = trackcsvfile
     if trackdata is None:
         inputfile = csv.reader(open(trackcsvfile))
         for row in inputfile:
             #columns are lat, long, height, times
             kml.newpoint(name='', coords=[(row[1], row[0], row[2])])
     else:
         for i,r in trackdata.iterrows():
             kml.newpoint(name='', coords=[(r[1], r[0], r[2])], extrude=1, altitudemode='absolute')
-    outname = trackcsvfile.replace('.csv','.kml')
+    if 'csv' in trackcsvfile:
+        outname = trackcsvfile.replace('.csv','.kml')
+    else:
+        outname = f'{trackcsvfile}.kml'
     if saveOutput:
+        if outdir is None:
+            outdir, _ = os.path.split(trackcsvfile)
+        os.makedirs(outdir, exist_ok=True)
+        outname = os.path.join(outdir, outname)
         kml.save(outname)
     return kml
 
 
 def getTrackDetails(traj):
     """ Get track details from a WMPL trajectory object
```

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/fileformats/platepar.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/fileformats/platepar.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,14 +78,7 @@
             if len(platepars) > 1: # and pp != pps[-1]:
                 platepars = platepars + ','
             platepars = platepars + '"' + thispl.id +'": '+ json.dumps(thispl.jsd)
     platepars = platepars + '}'
     #print(platepars)
     ppjson = json.loads(platepars)
     return ppjson
-
-
-if __name__ == '__main__':
-    p = loadPlatepars('c:/temp/platepars')
-    #print(p)
-    for pp in p:
-        print(p[pp]['fov_h'])
```

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/rmsutils/__init__.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,9 +19,8 @@
 
 from .multiDayRadiant import multiDayRadiant
 from .multiTrackStack import multiTrackStack
 from .analyseUFOwithRMS import analyseUFOwithRMS
 from .multiEventGroundMap import multiEventGroundMap
 from .plotCAMSOrbits import plotCAMSOrbits
 from .plotRMSOrbits import plotRMSOrbits
-from .trajPickle import getTrajPickle
-
+from .trajPickle import getTrajPickle, trajectoryKML
```

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/analyseUFOwithRMS.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/rmsutils/multiDayRadiant.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/multiDayRadiant.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/rmsutils/multiEventGroundMap.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/multiEventGroundMap.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/rmsutils/multiTrackStack.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/multiTrackStack.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/rmsutils/plotCAMSOrbits.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/plotCAMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/rmsutils/plotRMSOrbits.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/rmsutils/plotRMSOrbits.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/share/IMO_Working_Meteor_Shower_List.xml`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/share/__init__.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/share/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/share/streamfulldata.npy` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/share/streamfulldata.npy`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/usertools/apiExampleCode.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/apiExampleCode.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,57 +2,65 @@
 # Example showing how to use the matchdata API from Python
 #
 # Copyright (C) 2018-2023 Mark McIntyre
 
 """
 Examples showing how to use the APIs. 
 """
-
+import json
+import requests 
 import pandas as pd
 
 
 def matchApiCall(reqtyp, reqval):
     """get names of all matches for a given date"""
     apiurl = 'https://api.ukmeteornetwork.co.uk/matches'
-    apicall = '{}?reqtyp={}&reqval={}'.format(apiurl, reqtyp, reqval)
+    apicall = f'{apiurl}?reqtyp={reqtyp}&reqval={reqval}'
     matchlist = pd.read_json(apicall, lines=True)
     return matchlist
 
 
 def getMatchPickle(patt):
     """
     get the pickled trajectory for a given matched event   
     Returns a json object containing the pickled data
     
     Example pattern 20230501_002536.754_UK
     """
     apiurl = 'https://api.ukmeteornetwork.co.uk/pickle/getpickle'
     apicall = f'{apiurl}?reqval={patt}'
-    matchpickle = pd.read_json(apicall, lines=True)
-    return matchpickle
+    res = requests.get(apicall, stream=True)
+    if res.status_code == 200:
+        data=b''
+        for chunk in res.iter_content(chunk_size=4096):
+            data = data + chunk
+        jsd = json.loads(data)  
+    else:
+        jsd = None  
+    return jsd
 
 
 def detailApiCall1(reqtyp, reqval):
     """ get details of one event """
     apiurl = 'https://api.ukmeteornetwork.co.uk/matches'
-    apicall = '{}?reqtyp={}&reqval={}'.format(apiurl, reqtyp, reqval)
+    apicall = f'{apiurl}?reqtyp={reqtyp}&reqval={reqval}'
     evtdetail = pd.read_json(apicall, typ='series')
     return evtdetail
 
 
 def detailApiCall2(reqtyp, matchlist):
     """
     get details for the first five events in the match list 
     and put them in a pandas dataframe, then sort by brightest
     """
     apiurl = 'https://api.ukmeteornetwork.co.uk/matches'
     details = []
     for id in matchlist.head(5).orbname:
         reqval = id
-        apicall = '{}?reqtyp={}&reqval={}'.format(apiurl, reqtyp, reqval)
+        apicall = f'{apiurl}?reqtyp={reqtyp}&reqval={reqval}'
         details.append(pd.read_json(apicall, typ='series'))
     df = pd.DataFrame(details)
     df = df.sort_values(by=['_mag'])
     return df
 
 
 def getLiveimageList(dtstr):
@@ -76,22 +84,20 @@
 
     """
     apiurl = 'https://api.ukmeteornetwork.co.uk/fireballs/getfb'
     fbfiles = pd.read_json(f'{apiurl}?pattern={patt}')
     return fbfiles
 
 
-if __name__ == '__main__':
-    # get all matched events for a given date
-    reqtyp = 'matches'
-    reqval = '20211121'
-    matchlist = matchApiCall(reqtyp, reqval)
-    print(matchlist)
-
-    reqtyp = 'detail'
-    reqval = '20211121_032219.699_UK'
-    evtlist = detailApiCall1(reqtyp, reqval)
-    print(evtlist)
-
-    reqtyp = 'detail'
-    evt = detailApiCall2(reqtyp, matchlist)
-    print(evt)
+def trajectoryAPI(trajname):
+    apiurl = 'https://api.ukmeteornetwork.co.uk/pickle/getpickle'
+    fmt = 'json'
+    apicall = f'{apiurl}?reqval={trajname}&format={fmt}'
+    res = requests.get(apicall, stream=True)
+    if res.status_code == 200:
+        data=b''
+        for chunk in res.iter_content(chunk_size=4096):
+            data = data + chunk
+        jsd = json.loads(data)  
+    else:
+        jsd = None  
+    return jsd
```

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/usertools/findNearDuplicates.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/findNearDuplicates.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/usertools/getLiveImages.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/getLiveImages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 #
 # python script to get all live JPGs for a specified time
 #
 import os
-import sys
 import pandas as pd
 import requests
 
 
 def getLiveJpgs(dtstr, outdir=None, create_txt=False):
     """
     Retrieve live images from the ukmon website that match a pattern  
@@ -120,11 +119,7 @@
     get_response = requests.get(url, stream=True)
     if fname is None:
         fname = url.split("/")[-1]
     with open(os.path.join(outdir, fname), 'wb') as f:
         for chunk in get_response.iter_content(chunk_size=4096):
             if chunk: # filter out keep-alive new chunks
                 f.write(chunk)
-
-
-if __name__ == '__main__':
-    getLiveJpgs(sys.argv[1])
```

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/usertools/getOverlappingFovs.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/getOverlappingFovs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 # 
 #
 import os
-import sys
 import glob
 
 
 from ukmon_meteortools.fileformats import munchKML
 from shapely.geometry import Point
 
 
@@ -97,14 +96,7 @@
             if testkml != refkml:
                 testcam,_ = os.path.splitext(testkml)
                 #print('comparing to ', testcam)
                 if checkKMLOverlap(os.path.join(srcfolder, refkml), os.path.join(srcfolder, testkml)) is True:
                     currmatches.append(testcam[:6])
         matches.append(currmatches)
     return matches
-
-
-if __name__ == '__main__':
-    src = sys.argv[1]
-    targ = sys.argv[2]
-    matches = getOverlappingCameras(src, '*-25km.kml')
-    print(matches)
```

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/usertools/plotTrack.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/usertools/plotTrack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 
-import sys
 import csv
 from matplotlib import pyplot as plt
 import numpy as np
 
 from ukmon_meteortools.utils import greatCircleDistance
 
 
@@ -108,13 +107,7 @@
         tims.append(float(row[3]))
         alts.append(float(row[2])/1000)
     plt.clf()
     plt.plot(tims,alts)
     outname = trackcsvfile.replace('.csv','_time_alt.png')
     plt.savefig(outname)
     plt.close()
-
-
-if __name__ == '__main__':
-    trackToTimevsHeight(sys.argv[1])
-    trackToDistvsHeight(sys.argv[1])
-    trackToTimevsVelocity(sys.argv[1])
```

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/Math.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/Math.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/VectorMaths.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/VectorMaths.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/__init__.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/annotateImage.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/annotateImage.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/convertSolLon.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/convertSolLon.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/drawFTPfile.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/drawFTPfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright (C) 2018-2023 Mark McIntyre
 #
 # python code to read in an FTPdetect file and plot all the detections
 #
 
-import sys 
 import os
 import configparser as cr 
 from matplotlib import pyplot as plt
 
 
 def _readFTPfile(filename, h):
     """ Internal function to load ftpfile into arrays """
@@ -47,28 +46,25 @@
     Its like a stack of the night's detections but in a much simpler format. Useful for diagnosing false detections.   
 
     Arguments:  
         ftpfile:   [str] full path to the FTPdetect file.  
         cfgfile:   [str] full path to RMS config file to read image dimensions. Default is 1280x720.  
     """
     config = cr.ConfigParser()
-    config.read(cfgfile)
-    if len(config) == 1: 
+    if cfgfile is None: 
         width=1280
         height=720
     else:
+        config.read(cfgfile)
         width = int(config['Capture']['width'])
         height = int(config['Capture']['height'])
+
     print('plotting field of view {}x{}'.format(width, height))
     events = _readFTPfile(ftpfile, height)
     for ev in events: 
         plt.plot(ev['x'],ev['y'])
     pth, ftpf = os.path.split(ftpfile)
     spls = ftpf.split('_')
     outfname = f'{spls[1]}_{spls[2]}_{spls[3]}_{spls[3]}_ftpmap.png'
     plt.savefig(os.path.join(pth, outfname))
     plt.close()
     return 
-
-
-if __name__ == '__main__':
-    drawFTPFile(sys.argv[1], sys.argv[2])
```

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/getActiveShowers.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/getActiveShowers.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
         inclMinor:  [bool] include minor showers or only return major showers  
 
     Returns:  
         If retlist is true, returns a python list of shower short-codes eg ['PER','LYR']  
 
     """
     sl = iwsl.IMOshowerList()
-    listofshowers=sl.getActiveShowers(targdate,True, inclMinor=inclMinor)
+    testdate = datetime.datetime.strptime(targdate, '%Y%m%d')
+    listofshowers=sl.getActiveShowers(testdate,True, inclMinor=inclMinor)
     if retlist is False:
         for shwr in listofshowers:
             print(shwr)
     else:
         return listofshowers
 
 
@@ -54,12 +55,10 @@
         formatter_class=argparse.RawTextHelpFormatter)
     arg_parser.add_argument('-d', '--targdate', metavar='TARGDATE', type=str,
         help='Date to run for (default is today)')
     arg_parser.add_argument('-m', '--includeminor', action="store_true",
         help='include minor showers')
 
     cml_args = arg_parser.parse_args()
-    if cml_args.targdate is not None:
-        targdate = datetime.datetime.strptime(cml_args.targdate, '%Y%m%d')
-    else:
-        targdate = datetime.datetime.now()
+    if cml_args.targdate is None:
+        targdate = datetime.datetime.now().strftime('%Y%m%d')
     getActiveShowers(targdate, inclMinor=cml_args.includeminor)
```

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/getShowerDates.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/getShowerDates.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools/utils/sendAnEmail.py` & `ukmon_meteortools-2023.5.8/ukmon_meteortools/utils/sendAnEmail.py`

 * *Files identical despite different names*

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools.egg-info/PKG-INFO` & `ukmon_meteortools-2023.5.8/ukmon_meteortools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ukmon-meteortools
-Version: 2023.5.7
+Version: 2023.5.8
 Summary: Python Tools for Meteor Data Analysis
 Author-email: Mark McIntyre <ukmon@markmcintyreastro.co.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -674,15 +674,15 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://github.com/markmac99/UKMon-shared/ukmon_meteortools/
+Project-URL: Homepage, https://markmac99.github.io/UKmon-shared/ukmon_meteortools.html
 Project-URL: Bug Tracker, https://github.com/markmac99/UKMon-shared/issues
 Keywords: meteors,ukmon
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7
@@ -690,25 +690,26 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # ukmon_meteortools
 
 Python tools and utilities to work with meteor data from the UK Meteor Network
 
-To get more information about the submodules and functions use Python's built-in help capability
+To get more information about the submodules and functions use Python's built-in help capability, for example
+as shown here. 
 
 ``` python
 from ukmon_meteortools import utils
 help(utils)
 help(utils.sendAnEmail)
 ```
 
 Example usage 
 ```python
->>>from ukmon_meteortools.utils import date2JD, jd2LST
+>>>from ukmon_meteortools.utils import date2JD, jd2LST, getActiveShowers, getShowerDets
 >>> date2JD(2023,4,11,12,45,9)
 2460046.0313541666
 >>>import numpy as np
 >>> jd2LST(2460046.0313541666, lon=np.radians(-1.31))
 (30.741774823384617, 30.76463863658577)
 >>> import datetime
 >>> getActiveShowers(datetime.datetime.now())
```

### Comparing `ukmon_meteortools-2023.5.7/ukmon_meteortools.egg-info/SOURCES.txt` & `ukmon_meteortools-2023.5.8/ukmon_meteortools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

