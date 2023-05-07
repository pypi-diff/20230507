# Comparing `tmp/pydlm-0.1.1.8.tar.gz` & `tmp/pydlm-0.1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydlm-0.1.1.8.tar", last modified: Mon May 15 02:14:03 2017, max compression
+gzip compressed data, was "dist/pydlm-0.1.1.9.tar", last modified: Wed Aug 30 01:45:33 2017, max compression
```

## Comparing `pydlm-0.1.1.8.tar` & `pydlm-0.1.1.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/
--rw-r--r--   0 samuel     (501) staff       (20)      714 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/PKG-INFO
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/pydlm/
--rw-r--r--   0 samuel     (501) staff       (20)      413 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/__init__.py
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/pydlm/base/
--rw-r--r--   0 samuel     (501) staff       (20)      182 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/base/__init__.py
--rw-r--r--   0 samuel     (501) staff       (20)     3175 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/base/baseModel.py
--rw-r--r--   0 samuel     (501) staff       (20)    15563 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/base/kalmanFilter.py
--rw-r--r--   0 samuel     (501) staff       (20)     2216 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/base/tools.py
--rw-r--r--   0 samuel     (501) staff       (20)    45784 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/dlm.py
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/pydlm/func/
--rw-r--r--   0 samuel     (501) staff       (20)       53 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/func/__init__.py
--rw-r--r--   0 samuel     (501) staff       (20)    35565 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/func/_dlm.py
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/pydlm/modeler/
--rw-r--r--   0 samuel     (501) staff       (20)      396 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/modeler/__init__.py
--rw-r--r--   0 samuel     (501) staff       (20)     8842 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/modeler/autoReg.py
--rw-r--r--   0 samuel     (501) staff       (20)    14426 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/modeler/builder.py
--rw-r--r--   0 samuel     (501) staff       (20)     2072 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/modeler/component.py
--rw-r--r--   0 samuel     (501) staff       (20)     7185 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/modeler/dynamic.py
--rw-r--r--   0 samuel     (501) staff       (20)     7965 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/modeler/longSeason.py
--rw-r--r--   0 samuel     (501) staff       (20)     1199 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/modeler/matrixTools.py
--rw-r--r--   0 samuel     (501) staff       (20)     5694 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/modeler/seasonality.py
--rw-r--r--   0 samuel     (501) staff       (20)     3795 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/modeler/trends.py
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/pydlm/plot/
--rw-r--r--   0 samuel     (501) staff       (20)       62 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/plot/__init__.py
--rw-r--r--   0 samuel     (501) staff       (20)    17985 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/plot/dlmPlot.py
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/pydlm/tests/
--rw-r--r--   0 samuel     (501) staff       (20)        0 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/tests/__init__.py
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/pydlm/tests/base/
--rw-r--r--   0 samuel     (501) staff       (20)        0 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/tests/base/__init__.py
--rw-r--r--   0 samuel     (501) staff       (20)     5369 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/tests/base/testKalmanFilter.py
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/pydlm/tests/func/
--rw-r--r--   0 samuel     (501) staff       (20)        0 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/tests/func/__init__.py
--rw-r--r--   0 samuel     (501) staff       (20)    14437 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/tests/func/test_dlm.py
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/pydlm/tests/modeler/
--rw-r--r--   0 samuel     (501) staff       (20)        0 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/tests/modeler/__init__.py
--rw-r--r--   0 samuel     (501) staff       (20)     3859 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/tests/modeler/testAutoReg.py
--rw-r--r--   0 samuel     (501) staff       (20)     3852 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/tests/modeler/testBuilder.py
--rw-r--r--   0 samuel     (501) staff       (20)     1509 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/tests/modeler/testDynamic.py
--rw-r--r--   0 samuel     (501) staff       (20)     2746 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/tests/modeler/testLongSeason.py
--rw-r--r--   0 samuel     (501) staff       (20)      335 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/tests/modeler/testSeasonality.py
--rw-r--r--   0 samuel     (501) staff       (20)      297 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/tests/modeler/testTrends.py
--rw-r--r--   0 samuel     (501) staff       (20)    17440 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/tests/testDlm.py
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/pydlm/tuner/
--rw-r--r--   0 samuel     (501) staff       (20)        0 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/tuner/__init__.py
--rw-r--r--   0 samuel     (501) staff       (20)     3604 2017-05-15 02:11:32.000000 pydlm-0.1.1.8/pydlm/tuner/dlmTuner.py
-drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/pydlm.egg-info/
--rw-r--r--   0 samuel     (501) staff       (20)        1 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/pydlm.egg-info/dependency_links.txt
--rw-r--r--   0 samuel     (501) staff       (20)      714 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/pydlm.egg-info/PKG-INFO
--rw-r--r--   0 samuel     (501) staff       (20)       50 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/pydlm.egg-info/requires.txt
--rw-r--r--   0 samuel     (501) staff       (20)     1079 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/pydlm.egg-info/SOURCES.txt
--rw-r--r--   0 samuel     (501) staff       (20)        6 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/pydlm.egg-info/top_level.txt
--rw-r--r--   0 samuel     (501) staff       (20)       67 2017-05-15 02:14:03.000000 pydlm-0.1.1.8/setup.cfg
--rw-r--r--   0 samuel     (501) staff       (20)     1098 2017-05-15 02:13:49.000000 pydlm-0.1.1.8/setup.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/
+-rw-r--r--   0 samuel     (501) staff       (20)      714 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/PKG-INFO
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/pydlm/
+-rw-r--r--   0 samuel     (501) staff       (20)      413 2016-12-29 03:51:04.000000 pydlm-0.1.1.9/pydlm/__init__.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/pydlm/base/
+-rw-r--r--   0 samuel     (501) staff       (20)      182 2016-11-05 01:12:01.000000 pydlm-0.1.1.9/pydlm/base/__init__.py
+-rw-r--r--   0 samuel     (501) staff       (20)     3175 2016-11-05 01:12:01.000000 pydlm-0.1.1.9/pydlm/base/baseModel.py
+-rw-r--r--   0 samuel     (501) staff       (20)    15563 2017-02-07 10:32:11.000000 pydlm-0.1.1.9/pydlm/base/kalmanFilter.py
+-rw-r--r--   0 samuel     (501) staff       (20)     2216 2016-11-05 22:13:43.000000 pydlm-0.1.1.9/pydlm/base/tools.py
+-rw-r--r--   0 samuel     (501) staff       (20)    50735 2017-07-26 06:11:17.000000 pydlm-0.1.1.9/pydlm/dlm.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/pydlm/func/
+-rw-r--r--   0 samuel     (501) staff       (20)       53 2016-11-05 01:12:01.000000 pydlm-0.1.1.9/pydlm/func/__init__.py
+-rw-r--r--   0 samuel     (501) staff       (20)    36054 2017-07-26 06:11:54.000000 pydlm-0.1.1.9/pydlm/func/_dlm.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/pydlm/modeler/
+-rw-r--r--   0 samuel     (501) staff       (20)      396 2016-11-05 01:12:01.000000 pydlm-0.1.1.9/pydlm/modeler/__init__.py
+-rw-r--r--   0 samuel     (501) staff       (20)     8842 2017-02-08 10:29:35.000000 pydlm-0.1.1.9/pydlm/modeler/autoReg.py
+-rw-r--r--   0 samuel     (501) staff       (20)    14426 2017-02-24 09:29:34.000000 pydlm-0.1.1.9/pydlm/modeler/builder.py
+-rw-r--r--   0 samuel     (501) staff       (20)     2072 2016-11-05 01:12:01.000000 pydlm-0.1.1.9/pydlm/modeler/component.py
+-rw-r--r--   0 samuel     (501) staff       (20)     7185 2017-04-30 00:27:47.000000 pydlm-0.1.1.9/pydlm/modeler/dynamic.py
+-rw-r--r--   0 samuel     (501) staff       (20)     7965 2016-11-11 08:24:33.000000 pydlm-0.1.1.9/pydlm/modeler/longSeason.py
+-rw-r--r--   0 samuel     (501) staff       (20)     1199 2016-11-05 01:12:01.000000 pydlm-0.1.1.9/pydlm/modeler/matrixTools.py
+-rw-r--r--   0 samuel     (501) staff       (20)     5694 2017-07-25 10:08:45.000000 pydlm-0.1.1.9/pydlm/modeler/seasonality.py
+-rw-r--r--   0 samuel     (501) staff       (20)     3853 2017-06-15 07:57:33.000000 pydlm-0.1.1.9/pydlm/modeler/trends.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/pydlm/plot/
+-rw-r--r--   0 samuel     (501) staff       (20)       62 2016-11-05 01:12:01.000000 pydlm-0.1.1.9/pydlm/plot/__init__.py
+-rw-r--r--   0 samuel     (501) staff       (20)    19316 2017-07-25 09:23:10.000000 pydlm-0.1.1.9/pydlm/plot/dlmPlot.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/pydlm/tests/
+-rw-r--r--   0 samuel     (501) staff       (20)        0 2016-11-05 01:12:01.000000 pydlm-0.1.1.9/pydlm/tests/__init__.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/pydlm/tests/base/
+-rw-r--r--   0 samuel     (501) staff       (20)        0 2016-11-05 01:12:01.000000 pydlm-0.1.1.9/pydlm/tests/base/__init__.py
+-rw-r--r--   0 samuel     (501) staff       (20)     5448 2017-06-15 07:43:32.000000 pydlm-0.1.1.9/pydlm/tests/base/testKalmanFilter.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/pydlm/tests/func/
+-rw-r--r--   0 samuel     (501) staff       (20)        0 2016-11-05 01:12:01.000000 pydlm-0.1.1.9/pydlm/tests/func/__init__.py
+-rw-r--r--   0 samuel     (501) staff       (20)    15070 2017-06-20 06:41:17.000000 pydlm-0.1.1.9/pydlm/tests/func/test_dlm.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/pydlm/tests/modeler/
+-rw-r--r--   0 samuel     (501) staff       (20)        0 2016-11-05 01:12:01.000000 pydlm-0.1.1.9/pydlm/tests/modeler/__init__.py
+-rw-r--r--   0 samuel     (501) staff       (20)     3859 2017-02-24 07:55:41.000000 pydlm-0.1.1.9/pydlm/tests/modeler/testAutoReg.py
+-rw-r--r--   0 samuel     (501) staff       (20)     3852 2017-06-15 07:37:20.000000 pydlm-0.1.1.9/pydlm/tests/modeler/testBuilder.py
+-rw-r--r--   0 samuel     (501) staff       (20)     1509 2017-04-30 00:27:47.000000 pydlm-0.1.1.9/pydlm/tests/modeler/testDynamic.py
+-rw-r--r--   0 samuel     (501) staff       (20)     2746 2017-02-24 07:55:48.000000 pydlm-0.1.1.9/pydlm/tests/modeler/testLongSeason.py
+-rw-r--r--   0 samuel     (501) staff       (20)      335 2017-02-24 07:55:21.000000 pydlm-0.1.1.9/pydlm/tests/modeler/testSeasonality.py
+-rw-r--r--   0 samuel     (501) staff       (20)      297 2017-02-24 07:55:12.000000 pydlm-0.1.1.9/pydlm/tests/modeler/testTrends.py
+-rw-r--r--   0 samuel     (501) staff       (20)    17952 2017-07-25 10:10:44.000000 pydlm-0.1.1.9/pydlm/tests/testDlm.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/pydlm/tuner/
+-rw-r--r--   0 samuel     (501) staff       (20)        0 2016-12-29 03:53:20.000000 pydlm-0.1.1.9/pydlm/tuner/__init__.py
+-rw-r--r--   0 samuel     (501) staff       (20)     4263 2017-06-20 06:54:50.000000 pydlm-0.1.1.9/pydlm/tuner/dlmTuner.py
+drwxr-xr-x   0 samuel     (501) staff       (20)        0 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/pydlm.egg-info/
+-rw-r--r--   0 samuel     (501) staff       (20)        1 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/pydlm.egg-info/dependency_links.txt
+-rw-r--r--   0 samuel     (501) staff       (20)      714 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/pydlm.egg-info/PKG-INFO
+-rw-r--r--   0 samuel     (501) staff       (20)       50 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/pydlm.egg-info/requires.txt
+-rw-r--r--   0 samuel     (501) staff       (20)     1079 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/pydlm.egg-info/SOURCES.txt
+-rw-r--r--   0 samuel     (501) staff       (20)        6 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/pydlm.egg-info/top_level.txt
+-rw-r--r--   0 samuel     (501) staff       (20)       67 2017-08-30 01:45:33.000000 pydlm-0.1.1.9/setup.cfg
+-rw-r--r--   0 samuel     (501) staff       (20)     1098 2017-08-30 01:40:13.000000 pydlm-0.1.1.9/setup.py
```

### Comparing `pydlm-0.1.1.8/PKG-INFO` & `pydlm-0.1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pydlm
-Version: 0.1.1.8
+Version: 0.1.1.9
 Summary: A python library for the Bayesian dynamic linear model for time series modeling
 Home-page: https://github.com/wwrechard/pydlm
 Author: Xiangyu Wang
 Author-email: wwrechard@gmail.com
 License: BSD
 Description: UNKNOWN
 Keywords: dlm bayes bayesian kalman filter smoothing dynamic model
```

### Comparing `pydlm-0.1.1.8/pydlm/base/baseModel.py` & `pydlm-0.1.1.9/pydlm/base/baseModel.py`

 * *Files identical despite different names*

### Comparing `pydlm-0.1.1.8/pydlm/base/kalmanFilter.py` & `pydlm-0.1.1.9/pydlm/base/kalmanFilter.py`

 * *Files identical despite different names*

### Comparing `pydlm-0.1.1.8/pydlm/base/tools.py` & `pydlm-0.1.1.9/pydlm/base/tools.py`

 * *Files identical despite different names*

### Comparing `pydlm-0.1.1.8/pydlm/dlm.py` & `pydlm-0.1.1.9/pydlm/dlm.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,17 +28,18 @@
 
 """
 # This is the major class for fitting time series data using the
 # dynamic linear model. dlm is a subclass of builder, with adding the
 # Kalman filter functionality for filtering the data
 
 from copy import deepcopy
+from numpy import matrix
 from pydlm.base.tools import getInterval
-from pydlm.tuner.dlmTuner import modelTuner
 from pydlm.func._dlm import _dlm
+from pydlm.tuner.dlmTuner import modelTuner
 
 class dlm(_dlm):
     """ The main class of the dynamic linear model.
 
 
     This is the main class of the Bayeisan dynamic linear model.
     It provides the modeling, filtering, forecasting and smoothing
@@ -256,19 +257,25 @@
         self.fitForwardFilter()
         self.fitBackwardSmoother()
 
 # =========================== model prediction ==============================
 
     # One day ahead prediction function
     def predict(self, date=None, featureDict=None):
-        """ One day ahead predict based on the current data for a specific future
-        days.
+        """ One day ahead predict based on the current data.
 
         The predict result is based on all the data before date and predict the
-        observation at date + days.
+        observation at date + days. 
+
+        The prediction could be on the last day and into the future or in 
+        the middle of the time series and ignore the rest. For predicting into
+        the future, the new features must be supplied to featureDict. For 
+        prediction in the middle, the user can still supply the features which
+        will be used priorily. The old features will be used if featureDict is
+        None.
 
         Args:
             date: the index when the prediction based on. Default to the
                   last day.
             featureDict: the feature set for the dynamic Components, in a form
                   of {"component_name": feature}. If the featureDict is not
                   supplied, then the algo reuse those stored in the dynamic
@@ -286,42 +293,99 @@
 
         # check if the data on the date has been filtered
         if date > self.result.filteredSteps[1]:
             raise NameError('Prediction can only be made right' +
                             ' after the filtered date')
 
         return self._oneDayAheadPredict(date=date, featureDict=featureDict)
-
+        
     def continuePredict(self, featureDict=None):
         """ Continue prediction after the one-day ahead predict.
 
         If users want to have a multiple day prediction, they can opt to use
         continuePredict after predict with new features contained in
         featureDict. For example,
 
         >>> # predict 3 days after the last day
         >>> myDLM.predict(featureDict=featureDict_day1)
         >>> myDLM.continuePredict(featureDict=featureDict_day2)
         >>> myDLM.continuePredict(featureDict=featureDict_day3)
 
+        The featureDict acts the same way as in predict().
+
         Args:
             featureDict: the feature set for the dynamic components, stored
-                         in a for of {"component name": feature}. If the set
+                         in a for of {"component name": vector}. If the set
                          was not supplied, then the algo will re-use the old
                          feature. For days beyond the data, the featureDict
                          for every dynamic component must be provided.
 
         Returns:
             A tupe. (predicted observation, variance)
         """
         if self.result.predictStatus is None:
             raise NameError('continuePredict has to come after predict.')
 
         return self._continuePredict(featureDict=featureDict)
 
+    # N day ahead prediction
+    def predictN(self, N=1, date=None, featureDict=None):
+        """ N day ahead prediction based on the current data.
+
+        This function is a convenient wrapper of predict() and
+        continuePredict(). If the prediction is into the future, i.e, > n, 
+        the featureDict has to contain all feature vectors for multiple days
+        for each dynamic component. For example, assume myDLM has a component
+        named 'spy' which posseses two dimensions,
+
+        >>> featureDict_3day = {'spy': [[1, 2],[2, 3],[3, 4]]}
+        >>> myDLM.predictN(N=3, featureDict=featureDict_3day)
+
+        Args:
+            N:    The length of days to predict.
+            date: The index when the prediction based on. Default to the
+                  last day.
+            FeatureDict: The feature set for the dynamic Components, in a form
+                  of {"component_name": feature}, where the feature must have
+                  N elements of feature vectors. If the featureDict is not
+                  supplied, then the algo reuse those stored in the dynamic
+                  components. For dates beyond the last day, featureDict must
+                  be supplied.
+
+        Returns:
+            A tuple of two lists. (Predicted observation, variance of the predicted
+            observation)
+
+        """
+        if N < 1:
+            raise NameError('N has to be greater or equal to 1')
+        # Take care if features are numpy matrix
+        if isinstance(featureDict, matrix):
+            featureDict = featureDict.tolist()
+        predictedObs = []
+        predictedVar = []
+
+        # call predict for the first day
+        getSingleDayFeature = lambda f, i: ({k: v[i] for k, v in f.items()}
+                                            if f is not None else None)
+        # Construct the single day featureDict
+        featureDictOneDay = getSingleDayFeature(featureDict, 0)
+        (obs, var) = self.predict(date=date, featureDict=featureDictOneDay)
+        predictedObs.append(obs)
+        predictedVar.append(var)
+
+        # Continue predicting the remaining days
+        for i in range(1, N):
+            featureDictOneDay = getSingleDayFeature(featureDict, i)
+            (obs, var) = self.continuePredict(featureDict=featureDictOneDay)
+            predictedObs.append(obs)
+            predictedVar.append(var)
+        return (self._1DmatrixToArray(predictedObs),
+                self._1DmatrixToArray(predictedVar))
+
 # =========================== result components =============================
 
     def getAll(self):
         """ get all the _result class which contains all results
 
         Returns:
             The @result object containing all computed results.
@@ -877,15 +941,15 @@
         """ Reset the plotting option for the dlm class
 
         """
         self.options.plotOriginalData = True
         self.options.plotFilteredData = True
         self.options.plotSmoothedData = True
         self.options.plotPredictedData = True
-        self.options.showDataPoint = True
+        self.options.showDataPoint = False
         self.options.showFittedPoint = False
         self.options.showConfidenceInterval = True
         self.options.dataColor = 'black'
         self.options.filteredColor = 'blue'
         self.options.predictedColor = 'green'
         self.options.smoothedColor = 'red'
         self.options.separatePlot = True
@@ -908,14 +972,16 @@
 
         # load the library only when needed
         # import pydlm.plot.dlmPlot as dlmPlot
         self.loadPlotLibrary()
 
         if self.time is None:
             time = range(len(self.data))
+        else:
+            time = self.time
 
         # initialize the figure
         dlmPlot.plotInitialize()
 
         # change option setting if some results are not available
         if not self.initialized:
             raise NameError('The model must be constructed and' +
@@ -988,14 +1054,16 @@
         # load the library only when needed
         # import pydlm.plot.dlmPlot as dlmPlot
         self.loadPlotLibrary()
 
         # provide a fake time for plotting
         if self.time is None:
             time = range(len(self.data))
+        else:
+            time = self.time
 
         # change option setting if some results are not available
         if not self.initialized:
             raise NameError('The model must be constructed and' +
                             ' fitted before ploting.')
 
         # check the filter status and automatically turn off bad plots
@@ -1022,14 +1090,66 @@
                                     result=self.result,
                                     options=self.options,
                                     name=name)
         else:
             raise NameError('No such component.')
 
         dlmPlot.plotout()
+
+    def plotPredictN(self, N=1, date=None, featureDict=None):
+        """
+        Function to plot the N-day prediction results.
+
+        The input is the same as `dlm.predictN`. For details,
+        please refer to that function.
+
+        Args:
+            N:    The length of days to predict.
+            date: The index when the prediction based on. Default to the
+                  last day.
+            FeatureDict: The feature set for the dynamic Components, in a form
+                  of {"component_name": feature}, where the feature must have
+                  N elements of feature vectors. If the featureDict is not
+                  supplied, then the algo reuses those stored in the dynamic
+                  components. For dates beyond the last day, featureDict must
+                  be supplied.
+        """
+        if date is None:
+            date = self.n - 1
+
+        # load the library only when needed
+        # import pydlm.plot.dlmPlot as dlmPlot
+        self.loadPlotLibrary()
+
+        # provide a fake time for plotting
+        if self.time is None:
+            time = range(len(self.data))
+        else:
+            time = self.time
+
+        # change option setting if some results are not available
+        if not self.initialized:
+            raise NameError('The model must be constructed and' +
+                            ' fitted before ploting.')
+
+        # check the filter status and automatically turn off bad plots
+        self._checkPlotOptions()
+
+        predictedTimeRange = range(date, date + N)
+        predictedData, predictedVar = self.predictN(
+            N=N, date=date, featureDict=featureDict)
+        dlmPlot.plotPrediction(
+            time=time, data=self.data,
+            predictedTime=predictedTimeRange,
+            predictedData=predictedData,
+            predictedVar=predictedVar,
+            options=self.options)
+
+        dlmPlot.plotout()
+                               
 # ================================ control options =========================
 
     def showOptions(self):
         """ Print out all the option values
 
         """
         allItems = vars(self.options)
```

### Comparing `pydlm-0.1.1.8/pydlm/func/_dlm.py` & `pydlm-0.1.1.9/pydlm/func/_dlm.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             self.stable = True
             self.innovationType='component'
 
             self.plotOriginalData = True
             self.plotFilteredData = True
             self.plotSmoothedData = True
             self.plotPredictedData = True
-            self.showDataPoint = True
+            self.showDataPoint = False
             self.showFittedPoint = False
             self.showConfidenceInterval = True
             self.dataColor = 'black'
             self.filteredColor = 'blue'
             self.predictedColor = 'green'
             self.smoothedColor = 'red'
             self.separatePlot = True
@@ -363,14 +363,20 @@
     # found, it will fetch the default feature from the component. If
     # it could not find feature for some component, it returns an error
     # The intermediate result will be stored in result.predictStatus as
     # (start_date, next_pred_date, [all_predicted_values]), which will be
     # used by _continuePredict.
     def _oneDayAheadPredict(self, date, featureDict=None):
         """ One day ahead prediction based on the date and the featureDict.
+        The prediction could be on the last day and into the future or in 
+        the middle of the time series and ignore the rest. For predicting into
+        the future, the new features must be supplied to featureDict. For 
+        prediction in the middle, the user can still supply the features which
+        will be used priorily. The old features will be used if featureDict is
+        None.
 
         Args:
             date: the prediction starts (based on the observation before and
                   on this date)
             featureDict: the new feature value for some dynamic components.
                          must be specified in a form of {component_name: value}
                          if the feature for some dynamic component is not
@@ -401,15 +407,16 @@
 
         return (predictedObs, predictedObsVar)
 
     def _continuePredict(self, featureDict=None):
         """ Continue predicting one day after _oneDayAheadPredict or
         after _continuePredict. After using
         _oneDayAheadPredict, the user can continue predicting by using
-        _continuePredict and the new featureDict.
+        _continuePredict. The featureDict act the same as in
+        _oneDayAheadPredict.
 
         Args:
             featureDict: the new feature value for some dynamic components.
                          see @_oneDayAheadPredict
 
         Returns:
             A tuple of (predicted_mean, predicted_variance)
@@ -432,15 +439,14 @@
                 feature = self.result.predictStatus[2][-comp.d:]
             else:
                 extra = comp.d - len(self.predictStatus[2])
                 feature = self.data[(currentDate - extra + 1):
                                     (currentDate + 1)] + self.result.predictStatus[2]
             if featureDict is None:
                 featureDict = {}
-
             featureDict[name] = feature
 
         self._constructEvaluationForPrediction(featureDict=featureDict,
                                                date=currentDate + 1)
         self.Filter.predict(self.builder.model)
         predictedObs = self.builder.model.prediction.obs
         predictedObsVar = self.builder.model.prediction.obsVar
@@ -481,16 +487,16 @@
         for name in componentCollection:
             if name in featureDict:
                 self.builder.model.evaluation[
                     0, self.builder.componentIndex[name][0]:
                     (self.builder.componentIndex[name][1] + 1)] = featureDict[name]
             else:
                 if date is None:
-                    raise NameError('Both date and featureDict are ' +
-                                    'not provided for component ' + name)
+                    raise NameError('The feature of ' + name + ' is lacking, '
+                                    'but the date is not provided.')
                 comp = componentCollection[name]
                 comp.updateEvaluation(date)
                 self.builder.model.evaluation[
                     0, self.builder.componentIndex[name][0]:
                     (self.builder.componentIndex[name][1] + 1)] = comp.evaluation
 
 # =========================== model helper function ==========================
@@ -807,15 +813,16 @@
 
         if self.result.filteredSteps[1] == -1:
             raise NameError('need to run forward filter first')
 
         mse = 0
         for i in range(self.result.filteredSteps[0],
                        self.result.filteredSteps[1] + 1):
-            mse += (self.data[i] - self.result.predictedObs[i]) ** 2
+            if self.data[i] is not None:
+                mse += (self.data[i] - self.result.predictedObs[i]) ** 2
 
         mse = mse / (self.result.filteredSteps[1] + 1 -
                       self.result.filteredSteps[0])
         return mse[0,0]
 
     # get the discount from the model
     def _getDiscounts(self):
```

### Comparing `pydlm-0.1.1.8/pydlm/modeler/autoReg.py` & `pydlm-0.1.1.9/pydlm/modeler/autoReg.py`

 * *Files identical despite different names*

### Comparing `pydlm-0.1.1.8/pydlm/modeler/builder.py` & `pydlm-0.1.1.9/pydlm/modeler/builder.py`

 * *Files identical despite different names*

### Comparing `pydlm-0.1.1.8/pydlm/modeler/component.py` & `pydlm-0.1.1.9/pydlm/modeler/component.py`

 * *Files identical despite different names*

### Comparing `pydlm-0.1.1.8/pydlm/modeler/dynamic.py` & `pydlm-0.1.1.9/pydlm/modeler/dynamic.py`

 * *Files identical despite different names*

### Comparing `pydlm-0.1.1.8/pydlm/modeler/longSeason.py` & `pydlm-0.1.1.9/pydlm/modeler/longSeason.py`

 * *Files identical despite different names*

### Comparing `pydlm-0.1.1.8/pydlm/modeler/matrixTools.py` & `pydlm-0.1.1.9/pydlm/modeler/matrixTools.py`

 * *Files identical despite different names*

### Comparing `pydlm-0.1.1.8/pydlm/modeler/seasonality.py` & `pydlm-0.1.1.9/pydlm/modeler/seasonality.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     or cos relationship between each state. They can be arbitrarily valued.
 
     Args:
         period: the period of the
         discount: the discount factor
         name: the name of the trend component
         w: the value to set the prior covariance. Default to a diagonal
-           matrix with 1e7 on the diagonal.
+           matrix with 100 on the diagonal.
 
     Examples:
         >>>  # create a 7-day seasonality:
         >>> ctrend = seasonality(period = 7, name = 'weekly', discount = 0.99)
         >>>  # change the ctrend to have covariance with diagonals are 2 and state 1
         >>> ctrend.createCovPrior(cov = 2)
         >>> ctrend.createMeanPrior(mean = 1)
@@ -58,15 +58,15 @@
 
 
     """
     def __init__(self,
                  period = 7,
                  discount = 0.99,
                  name = 'seasonality',
-                 w=1e7):
+                 w=100):
 
         if period <= 1:
             raise NameError('Period has to be greater than 1.')
         self.d = period
         self.componentType = 'seasonality'
         self.name = name
         self.discount = np.ones(self.d) * discount
```

### Comparing `pydlm-0.1.1.8/pydlm/modeler/trends.py` & `pydlm-0.1.1.9/pydlm/modeler/trends.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,50 +18,50 @@
 
 class trend(component):
     """ The trend component that features the polynomial trending,
     providing one building block for the dynamic linear model.
     It decribes a latent polynomial trending in the time series data.
 
     Args:
-        degree: the degree of the polynomial
+        degree: the degree of the polynomial. 0: constant; 1: linear...
         discount: the discount factor
         name: the name of the trend component
         w: the value to set the prior covariance. Default to a diagonal
            matrix with 1e7 on the diagonal.
 
     Examples:
         >>>  # create a constant trend
         >>> ctrend = trend(degree = 1, name = 'Const', discount = 0.99)
         >>>  # change the ctrend to have covariance with diagonals are 2 and state 1
         >>> ctrend.createCovPrior(cov = 2)
         >>> ctrend.createMeanPrior(mean = 1)
 
     Attributes:
-        d: the degree of the polynomial trend
+        d: the dimension of the latent states of the polynomial trend
         componentType: the type of the component, in this case, 'trend'
         name: the name of the trend component, to be supplied by user
               used in modeling and result extraction
         discount: the discount factor for this component. Details please refer
                   to the @kalmanFilter
         evaluation: the evaluation matrix for this component
         transition: the transition matrix for this component
         covPrior: the prior guess of the covariance matrix of the latent states
         meanPrior: the prior guess of the latent states
 
     """
 
     def __init__(self,
-                 degree = 1,
+                 degree = 0,
                  discount = 0.99,
                  name = 'trend',
                  w=1e7):
 
-        if degree <= 0:
-            raise NameError('degree has to be positive')
-        self.d = degree
+        if degree < 0:
+            raise NameError('degree has to be non-negative')
+        self.d = degree + 1
         self.name = name
         self.componentType = 'trend'
         self.discount = np.ones(self.d) * discount
 
         # Initialize all basic quantities
         self.evaluation = None
         self.transition = None
```

### Comparing `pydlm-0.1.1.8/pydlm/plot/dlmPlot.py` & `pydlm-0.1.1.9/pydlm/plot/dlmPlot.py`

 * *Files 6% similar despite different names*

```diff
@@ -408,14 +408,50 @@
             plotInterval(time=time[start:end],
                          upper=upper, lower=lower,
                          intervalType=options.intervalType,
                          color=options.smoothedColor)
 
         plt.legend(loc='best', shadow=True)
 
+
+# =========================== plot for prediction ========================
+def plotPrediction(time, data, predictedTime,
+                   predictedData, predictedVar, options):
+    """
+    Function for ploting N-day ahead prediction
+
+    Args:
+        time: the data time
+        data: the original data
+        predictedTime: the predicted time period
+        predictedData: the predicted data
+        predictedVar: the predicted variance
+        options: options for the plot, for details please refer to @dlm
+    """
+    # plot the original data
+    plotData(time, data, showDataPoint=options.showDataPoint,
+             color=options.dataColor,
+             label='time series')
+    # overlay the predicted data
+    plotData(predictedTime, predictedData,
+             showDataPoint=options.showFittedPoint,
+             color=options.predictedColor,
+             label='N-day prediction')
+    # overlay confidence interval
+    if options.showConfidenceInterval:
+        upper, lower = getInterval(predictedData,
+                                   predictedVar,
+                                   p=options.confidence)
+
+        plotInterval(time=predictedTime,
+                     upper=upper, lower=lower,
+                     intervalType=options.intervalType,
+                     color=options.predictedColor)
+    
+    
 # =========================== basic functions ============================
 
 
 def plotData(time, data, showDataPoint=True, color='black', label='unknown'):
     """
     The function to plot data points.
```

### Comparing `pydlm-0.1.1.8/pydlm/tests/base/testKalmanFilter.py` & `pydlm-0.1.1.9/pydlm/tests/base/testKalmanFilter.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,18 +8,22 @@
 
 class testKalmanFilter(unittest.TestCase):
 
     def setUp(self):
         self.kf1 = kalmanFilter(discount=[1])
         self.kf0 = kalmanFilter(discount=[1e-10])
         self.kf11 = kalmanFilter(discount=[1, 1])
+        self.trend0 = trend(degree=0, discount=1, w=1.0)
+        self.trend0_90 = trend(degree=0, discount=0.9, w=1.0)
+        self.trend0_98 = trend(degree=0, discount=0.98, w=1.0, name='a')
+        self.trend1 = trend(degree=1, discount=1, w=1.0)
 
     def testForwardFilter(self):
         dlm = builder()
-        dlm.add(trend(degree=1, discount=1, w=1.0))
+        dlm.add(self.trend0)
         dlm.initialize()
         self.kf1.predict(dlm.model)
         self.assertAlmostEqual(dlm.model.prediction.obs, 0)
 
         # the prior on the mean is zero, but observe 1, with
         # discount = 1, one should expect the filterd mean to be 0.5
         self.kf1.forwardFilter(dlm.model, 1)
@@ -57,15 +61,15 @@
 
         self.kf11.forwardFilter(dlm.model, -1)
         self.assertAlmostEqual(dlm.model.state[0][0, 0], -0.5)
         self.assertAlmostEqual(dlm.model.state[1][0, 0], 0.5)
 
     def testBackwardSmoother(self):
         dlm = builder()
-        dlm.add(trend(degree=1, discount=1, w=1.0))
+        dlm.add(self.trend0)
         dlm.initialize()
 
         # with mean being 0 and observe 1 and 0 consectively, one shall
         # expect the smoothed mean at 1 will be 1/3, for discount = 1
         self.kf1.forwardFilter(dlm.model, 1)
         self.kf1.forwardFilter(dlm.model, 0)
         self.kf1.backwardSmoother(dlm.model, \
@@ -75,15 +79,15 @@
         self.assertAlmostEqual(dlm.model.sysVar[0, 0], 0.18518519)
 
     # second order trend with discount = 1. The smoothed result should be
     # equal to a direct fit on the three data points, 0, 1, -1. Thus, the
     # smoothed observation should be 0.0
     def testBackwardSmootherMultiDim(self):
         dlm = builder()
-        dlm.add(trend(degree=2, discount=1, w=1.0))
+        dlm.add(self.trend1)
         dlm.initialize()
 
         self.kf11.forwardFilter(dlm.model, 1)
         state1 = dlm.model.state
         cov1 = dlm.model.sysVar
 
         self.kf11.forwardFilter(dlm.model, -1)
@@ -91,15 +95,15 @@
                                    rawState = state1, \
                                    rawSysVar = cov1)
 
         self.assertAlmostEqual(dlm.model.obs[0, 0], 0.0)
 
     def testMissingData(self):
         dlm = builder()
-        dlm.add(trend(degree=1, discount=1, w=1.0))
+        dlm.add(self.trend0)
         dlm.initialize()
 
         self.kf0.forwardFilter(dlm.model, 1)
         self.assertAlmostEqual(dlm.model.obs[0, 0], 1.0)
         self.assertAlmostEqual(dlm.model.obsVar[0, 0], 1.0)
 
         self.kf0.forwardFilter(dlm.model, None)
@@ -111,26 +115,26 @@
         self.assertAlmostEqual(dlm.model.obsVar[0, 0]/1e10, 0.5)
 
         self.kf0.forwardFilter(dlm.model, 0)
         self.assertAlmostEqual(dlm.model.obs[0, 0], 0.0)
 
     def testMissingEvaluation(self):
         dlm = builder()
-        dlm.add(trend(degree=1, discount=1, w=1.0))
+        dlm.add(self.trend0)
         dlm.initialize()
 
         dlm.model.evaluation = np.matrix([[None]])
         self.kf1.forwardFilter(dlm.model, 1.0, dealWithMissingEvaluation = True)
         self.assertAlmostEqual(dlm.model.obs, 0.0)
         self.assertAlmostEqual(dlm.model.transition, 1.0)
 
     def testEvolveMode(self):
         dlm = builder()
-        dlm.add(trend(degree=1, discount=0.9, w=1.0))
-        dlm.add(trend(degree=1, discount=0.98, name='a', w=1.0))
+        dlm.add(self.trend0_90)
+        dlm.add(self.trend0_98)
         dlm.initialize()
 
         kf2 = kalmanFilter(discount=[0.9, 0.98],
                            updateInnovation='component',
                            index=dlm.componentIndex)
         kf2.forwardFilter(dlm.model, 1.0)
         self.assertAlmostEqual(dlm.model.innovation[0, 1], 0.0)
```

### Comparing `pydlm-0.1.1.8/pydlm/tests/func/test_dlm.py` & `pydlm-0.1.1.9/pydlm/tests/func/test_dlm.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,37 +14,41 @@
         self.data = [0] * 9 + [1] + [0] * 10
         self.dlm1 = _dlm(self.data)
         self.dlm2 = _dlm(self.data)
         self.dlm3 = _dlm([-1, 1, -1, 1, -1, 1, -1, 1, -1, 1, -1, 1])
         self.dlm4 = _dlm([0, 0, 0, 0, 0, 1, 1, 1, 1, 1])
         self.dlm5 = _dlm(range(100))
         self.dlm6 = _dlm(range(100))
-        self.dlm1.builder + trend(degree=1, discount=1, w=1.0)
-        self.dlm2.builder + trend(degree=1, discount=1e-12, w=1.0)
+        self.dlm7 = _dlm([0, 1, None, 1, 0, 1, -1])
+        self.dlm1.builder + trend(degree=0, discount=1, w=1.0)
+        self.dlm2.builder + trend(degree=0, discount=1e-12, w=1.0)
         self.dlm3.builder + seasonality(period=2, discount=1, w=1.0)
         self.dlm4.builder + dynamic(features=[[0] for i in range(5)] +
                                     [[1] for i in range(5)], discount=1,
                                     w=1.0)
-        self.dlm5.builder + trend(degree=1, discount=1, w=1.0) + \
+        self.dlm5.builder + trend(degree=0, discount=1, w=1.0) + \
             autoReg(degree=1, data=range(100), discount=1, w=1.0)
-        self.dlm6.builder + trend(degree=1, discount=0.9, w=1.0) + \
+        self.dlm6.builder + trend(degree=0, discount=0.9, w=1.0) + \
             seasonality(period=2, discount=0.8, w=1.0) + \
             autoReg(degree=3, data=range(100), discount=1.0)
+        self.dlm7.builder + trend(degree=0, discount=1, w=1.0)
         self.dlm1._initialize()
         self.dlm2._initialize()
         self.dlm3._initialize()
         self.dlm4._initialize()
         self.dlm5._initialize()
         self.dlm6._initialize()
+        self.dlm7._initialize()
         self.dlm1.options.innovationType='whole'
         self.dlm2.options.innovationType='whole'
         self.dlm3.options.innovationType='whole'
         self.dlm4.options.innovationType='whole'
         self.dlm5.options.innovationType='whole'
         self.dlm6.options.innovationType='whole'
+        self.dlm7.options.innovationType='whole'
 
     def testForwardFilter(self):
         self.dlm1._forwardFilter(start=0, end=19, renew=False)
         self.assertAlmostEqual(np.sum(self.dlm1.result.filteredObs[0:9]), 0)
         self.assertAlmostEqual(self.dlm1.result.filteredObs[9][0, 0], 1.0/11)
         self.assertAlmostEqual(self.dlm1.result.filteredObs[19][0, 0], 1.0/21)
 
@@ -279,30 +283,41 @@
 
         diff = 0.0
         for i in range(len(arTrend)):
             diff += abs(arTrend[i] - trueAr[i])
         self.assertAlmostEqual(diff, 0)
 
     def testComputeMSE(self):
-        self.dlm1._forwardFilter(start = 0, end = 19, renew = False)
-        self.dlm1.result.filteredSteps = (0, 19)
+        self.dlm1._forwardFilter(start=0, end=19, renew=False)
+        self.dlm1.result.filteredSteps=(0, 19)
         mse1 = self.dlm1._getMSE()
         mse_expect = 0
         for i in range(20):
             mse_expect += (self.dlm1.result.predictedObs[i] -
                             self.data[i]) ** 2
         mse_expect /= 20
         self.assertAlmostEqual(mse1, mse_expect)
 
-        self.dlm2._forwardFilter(start = 0, end = 19, renew = False)
-        self.dlm2.result.filteredSteps = (0, 19)
+        self.dlm2._forwardFilter(start=0, end=19, renew=False)
+        self.dlm2.result.filteredSteps=(0, 19)
         mse2 = self.dlm2._getMSE()
         mse_expect = 2.0/20
+        self.assertAlmostEqual(mse2, mse_expect)
 
-        self.assertAlmostEqual(mse2, mse_expect)        
+        # Test missing data
+        self.dlm7._forwardFilter(start=0, end=6, renew=False)
+        self.dlm7.result.filteredSteps=(0, 6)
+        mse3 = self.dlm7._getMSE()
+        mse_expect = 0
+        for i in range(7):
+            if self.dlm7.data[i] is not None:
+                mse_expect += (self.dlm7.result.predictedObs[i] -
+                               self.dlm7.data[i]) ** 2
+        mse_expect /= 7
+        self.assertAlmostEqual(mse3, mse_expect)
 
     def testGetDiscount(self):
         discounts = self.dlm6._getDiscounts()
         self.assertTrue(0.9 in discounts)
         self.assertTrue(0.8 in discounts)
         self.assertTrue(1.0 in discounts)
```

### Comparing `pydlm-0.1.1.8/pydlm/tests/modeler/testAutoReg.py` & `pydlm-0.1.1.9/pydlm/tests/modeler/testAutoReg.py`

 * *Files identical despite different names*

### Comparing `pydlm-0.1.1.8/pydlm/tests/modeler/testBuilder.py` & `pydlm-0.1.1.9/pydlm/tests/modeler/testBuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pydlm.modeler.matrixTools import matrixTools as mt
 
 
 class testBuilder(unittest.TestCase):
 
     def setUp(self):
         self.features = np.random.rand(10, 2).tolist()
-        self.trend = trend(degree=3, w=1.0)
+        self.trend = trend(degree=2, w=1.0)
         self.seasonality = seasonality(period=7, w=1.0)
         self.dynamic = dynamic(self.features, w=1.0)
         self.autoReg = autoReg(degree=3,
                                data=np.random.rand(10).tolist(),
                                w=1.0)
         self.builder1 = builder()
```

### Comparing `pydlm-0.1.1.8/pydlm/tests/modeler/testDynamic.py` & `pydlm-0.1.1.9/pydlm/tests/modeler/testDynamic.py`

 * *Files identical despite different names*

### Comparing `pydlm-0.1.1.8/pydlm/tests/modeler/testLongSeason.py` & `pydlm-0.1.1.9/pydlm/tests/modeler/testLongSeason.py`

 * *Files identical despite different names*

### Comparing `pydlm-0.1.1.8/pydlm/tests/testDlm.py` & `pydlm-0.1.1.9/pydlm/tests/testDlm.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,25 +8,27 @@
 from pydlm.dlm import dlm
 
 class testDlm(unittest.TestCase):
 
     def setUp(self):
         self.data = [0] * 9 + [1] + [0] * 10
         self.features = np.random.random((20, 2)).tolist()
+        self.trend0 = trend(degree=0, discount=1.0, w=1.0)
+        self.trend1 = trend(degree=0, discount=1.0)
         self.dlm1 = dlm(self.data)
         self.dlm2 = dlm(self.data)
         self.dlm3 = dlm([-1, 1, -1, 1, -1, 1, -1, 1, -1, 1, -1, 1])
         self.dlm4 = dlm([0, 0, 0, 0, 0, 1, 1, 1, 1, 1])
         self.dlm5 = dlm(range(100))
-        self.dlm1 + trend(degree=1, discount=1, w=1.0)
-        self.dlm2 + trend(degree=1, discount=1e-12, w=1.0)
+        self.dlm1 + trend(degree=0, discount=1, w=1.0)
+        self.dlm2 + trend(degree=0, discount=1e-12, w=1.0)
         self.dlm3 + seasonality(period=2, discount=1, w=1.0)
         self.dlm4 + dynamic(features=[[0] for i in range(5)] +
                             [[1] for i in range(5)], discount=1, w=1.0)
-        self.dlm5 + trend(degree=1, discount=1, w=1.0) + \
+        self.dlm5 + trend(degree=0, discount=1, w=1.0) + \
             autoReg(degree=1, data=range(100), discount=1, w=1.0)
         self.dlm1.evolveMode('dependent')
         self.dlm2.evolveMode('dependent')
         self.dlm3.evolveMode('dependent')
         self.dlm4.evolveMode('dependent')
         self.dlm5.evolveMode('dependent')
 
@@ -72,107 +74,97 @@
         self.dlm2.fitBackwardSmoother()
         self.assertAlmostEqual(self.dlm2.result.smoothedObs[0][0, 0], 0.0)
         self.assertAlmostEqual(self.dlm2.result.smoothedObs[19][0, 0], 0.0)
         self.assertAlmostEqual(self.dlm2.result.smoothedObs[9][0, 0], 1.0)
 
     def testAppend(self):
         dlm4 = dlm(self.data[0:11])
-        dlm4 + trend(degree=1, discount=1, w=1.0)
+        dlm4 + self.trend0
         dlm4.evolveMode('dependent')
         dlm4.fitForwardFilter()
         self.assertEqual(dlm4.n, 11)
 
         dlm4.append(self.data[11 : 20])
         self.assertEqual(dlm4.n, 20)
         dlm4.fitForwardFilter()
 
         self.dlm1.fitForwardFilter()
-        self.assertAlmostEqual(np.sum(np.array(dlm4.result.filteredObs) - \
+        self.assertAlmostEqual(np.sum(np.array(dlm4.result.filteredObs) -
                                       np.array(self.dlm1.result.filteredObs)), 0.0)
 
     def testAppendDynamic(self):
         # we feed the data to dlm4 via two segments
         dlm4 = dlm(self.data[0:11])
-        dlm4 + trend(degree = 1, discount = 1) + dynamic(features = self.features[0:11], \
-                                                         discount = 1)
+        dlm4 + self.trend1 + dynamic(features = self.features[0:11],
+                                     discount = 1)
         dlm4.fitForwardFilter()
         dlm4.append(self.data[11 : 20])
         dlm4.append(self.features[11 : 20], component = 'dynamic')
         dlm4.fitForwardFilter()
 
         # we feed the data to dlm5 all at once
         dlm5 = dlm(self.data)
-        dlm5 + trend(degree = 1, discount = 1) + dynamic(features = self.features, \
-                                                         discount = 1)
+        dlm5 + self.trend1 + dynamic(features = self.features,
+                                     discount = 1)
         dlm5.fitForwardFilter()
-        self.assertAlmostEqual(np.sum(np.array(dlm4.result.filteredObs) - \
+        self.assertAlmostEqual(np.sum(np.array(dlm4.result.filteredObs) -
                                       np.array(dlm5.result.filteredObs)), 0.0)
 
     def testAppendAutomatic(self):
         # we feed the data to dlm4 via two segments
         dlm4 = dlm(self.data[0:11])
-        dlm4 + trend(degree = 1, discount = 1) + autoReg(degree = 3,
-                                                         data = self.data[0:11],
-                                                         discount = 1)
+        dlm4 + self.trend1 + autoReg(degree = 3, data = self.data[0:11],
+                                     discount = 1)
         dlm4.fitForwardFilter()
         dlm4.append(self.data[11 : 20])
         dlm4.fitForwardFilter()
 
         # we feed the data to dlm5 all at once
         dlm5 = dlm(self.data)
-        dlm5 + trend(degree = 1, discount = 1) + autoReg(degree = 3,
-                                                         data = self.data,
-                                                         discount = 1)
+        dlm5 + self.trend1 + autoReg(degree = 3, data = self.data, discount = 1)
         dlm5.fitForwardFilter()
-        self.assertAlmostEqual(np.sum(np.array(dlm4.result.filteredObs) - \
+        self.assertAlmostEqual(np.sum(np.array(dlm4.result.filteredObs) -
                                       np.array(dlm5.result.filteredObs)), 0.0)
 
     def testPopout(self):
         dlm4 = dlm(self.data)
-        dlm4 + trend(degree = 1, discount = 1) + dynamic(features = \
-                                                         self.features, \
-                                                         discount = 1)
+        dlm4 + self.trend1 + dynamic(features = self.features, discount = 1)
         dlm4.fitForwardFilter()
         # the filtered step range should be (0, 19)
         self.assertEqual(dlm4.result.filteredSteps, [0, 19])
 
         # pop out the first date, the filtered range should be (0, -1)
         dlm4.popout(0)
         self.assertEqual(dlm4.result.filteredSteps, [0, -1])
 
         dlm4.fitForwardFilter()
         dlm5 = dlm(self.data[1 : 20])
-        dlm5 + trend(degree = 1, discount = 1) + dynamic(features = \
-                                                         self.features[1 : 20], \
-                                                         discount = 1)
+        dlm5 + self.trend1 + dynamic(features = self.features[1 : 20],
+                                     discount = 1)
         dlm5.fitForwardFilter()
 
         # The two chain should have the same filtered obs
-        self.assertAlmostEqual(np.sum(np.array(dlm4.result.filteredObs) - \
+        self.assertAlmostEqual(np.sum(np.array(dlm4.result.filteredObs) -
                                       np.array(dlm5.result.filteredObs)), 0.0)
 
     def testAlter(self):
         dlm4 = dlm(self.data)
-        dlm4 + trend(degree = 1, discount = 1) + dynamic(features = \
-                                                         self.features, \
-                                                         discount = 1)
+        dlm4 + self.trend1 + dynamic(features = self.features, discount = 1)
         dlm4.fitForwardFilter()
         # the filtered step range should be (0, 19)
         self.assertEqual(dlm4.result.filteredSteps, [0, 19])
 
         dlm4.alter(date = 15, data = 1, component = 'main')
         self.assertEqual(dlm4.result.filteredSteps, [0, 14])
         dlm4.fitForwardFilter()
 
         newData = [0] * 9 + [1] + [0] * 10
         newData[15] = 1
         dlm5 = dlm(newData)
-        dlm5 + trend(degree = 1, discount = 1) + dynamic(features = \
-                                                         self.features, \
-                                                         discount = 1)
+        dlm5 + self.trend1 + dynamic(features = self.features, discount = 1)
         dlm5.fitForwardFilter()
 
         # The two chain should have the same filtered obs
         self.assertAlmostEqual(np.sum(np.array(dlm4.result.filteredObs) - \
                                       np.array(dlm5.result.filteredObs)), 0.0)
 
         # test alter the feature
@@ -207,32 +199,60 @@
                                [11, 12, [-6.0/7]])
         (obs, var) = self.dlm3.continuePredict()
         self.assertAlmostEqual(self.dlm3.result.predictStatus,
                                [11, 13, [-6.0/7, 6.0/7]])
 
     def testContinuePredictWithDynamic(self):
         self.dlm4.fitForwardFilter()
-        featureDict = {'dynamic': 2.0}
+        featureDict = {'dynamic': [2.0]}
         (obs, var) = self.dlm4.predict(date=9,
                                        featureDict=featureDict)
         self.assertAlmostEqual(self.dlm4.result.predictStatus,
                                [9, 10, [5.0/6 * 2]])
 
-        featureDict = {'dynamic': 3.0}
+        featureDict = {'dynamic': [3.0]}
         (obs, var) = self.dlm4.continuePredict(featureDict=featureDict)
         self.assertAlmostEqual(self.dlm4.result.predictStatus,
                                [9, 11, [5.0/6 * 2, 5.0/6 * 3]])
 
     def testPredictWithAutoReg(self):
         self.dlm5.fitForwardFilter()
         (obs, var) = self.dlm5.predict(date=99)
         self.assertAlmostEqual(obs[0, 0], 100.03682874)
         (obs, var) = self.dlm5.continuePredict()
         self.assertAlmostEqual(obs[0, 0], 101.07480945)
 
+    def testPredictNWithoutDynamic(self):
+        self.dlm3.fitForwardFilter()
+        (obs, var) = self.dlm3.predictN(N=2, date=11)
+        self.assertAlmostEqual(self.dlm3.result.predictStatus,
+                               [11, 13, [-6.0/7, 6.0/7]])
+
+    def testPredictNWithDynamic(self):
+        self.dlm4.fitForwardFilter()
+        featureDict = {'dynamic': [[2.0], [3.0]]}
+        (obs, var) = self.dlm4.predictN(N=2, date=9,
+                                        featureDict=featureDict)
+        self.assertAlmostEqual(self.dlm4.result.predictStatus,
+                               [9, 11, [5.0/6 * 2, 5.0/6 * 3]])
+
+    def testPredictNWithAutoReg(self):
+        self.dlm5.fitForwardFilter()
+        (obs, var) = self.dlm5.predictN(N=2, date=99)
+        self.assertAlmostEqual(obs[0], 100.03682874)
+        self.assertAlmostEqual(obs[1], 101.07480945)
+
+    def testPredictNWithDynamicMatrixInput(self):
+        self.dlm4.fitForwardFilter()
+        featureDict = {'dynamic': np.matrix([[2.0], [3.0]])}
+        (obs, var) = self.dlm4.predictN(N=2, date=9,
+                                        featureDict=featureDict)
+        self.assertAlmostEqual(self.dlm4.result.predictStatus,
+                               [9, 11, [5.0/6 * 2, 5.0/6 * 3]])
+
     def testGetLatentState(self):
         # for forward filter
         self.dlm5.fitForwardFilter()
         filteredTrend = self.dlm5.getLatentState(
             filterType='forwardFilter', name='trend')
         diff = 0.0
         for i in range(len(filteredTrend)):
```

### Comparing `pydlm-0.1.1.8/pydlm/tuner/dlmTuner.py` & `pydlm-0.1.1.9/pydlm/tuner/dlmTuner.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,26 +30,36 @@
     """ The main class for modelTuner
 
     Attributes:
         method: the optimization method. Currently only 'gradient_descent'
                 is supported.
         loss:   the optimization loss function. Currently only 'mse' (one-day
                 ahead prediction) is supported.
+    
     """
 
     def __init__(self, method='gradient_descent', loss='mse'):
 
         self.method = method
         self.loss = loss
         self.current_mse = None
         self.err = 1e-4
         self.discounts = None
 
     def tune(self, untunedDLM, maxit=100, step = 1.0):
+        """ Main function for tuning the DLM model.
 
+        Args:
+            untunedDLM: The DLM object that needs tuning
+            maxit: The maximum number of iteractions for gradient descent.
+            step: the moving length at each iteraction.
+
+        Returns:
+            A tuned DLM object in unintialized status.
+        """
         # make a deep copy of the original dlm
         tunedDLM = deepcopy(untunedDLM)
         tunedDLM.showInternalMessage(False)
 
         if not tunedDLM.initialized:
             tunedDLM.fitForwardFilter()
         discounts = array(tunedDLM._getDiscounts())
@@ -65,25 +75,31 @@
                 tunedDLM.fitForwardFilter()
                 self.current_mse = tunedDLM._getMSE()
 
             if i < maxit - 1:
                 print('Converge successfully!')
             else:
                 print('The algorithm stops without converging.')
-                if min(discounts) <= 0.1 + self.err or max(discounts) >= 1 - 2 * self.err:
-                    print('Possible reason: some discount is too close to 1 or 0.1')
+                if min(discounts) <= 0.7 + self.err or max(discounts) >= 1 - 2 * self.err:
+                    print('Possible reason: some discount is too close to 1 or 0.7' +
+                          ' (0.7 is smallest discount that is permissible.')
                 else:
                     print('It might require more step to converge.' +
                           ' Use tune(..., maixt = <a larger number>) instead.')
 
         self.discounts = discounts
         tunedDLM._setDiscounts(discounts, change_component=True)
         return tunedDLM
 
     def getDiscounts(self):
+        """ Get the tuned discounting factors. One for each component (even the
+            component being multi-dimensional, only one discounting factor will
+            be assigned to one component). Initialized to None.
+
+        """
         return self.discounts
 
     def find_gradient(self, discounts, DLM):
         if self.current_mse is None:
             self.current_mse = DLM._getMSE()
 
         gradient = array([0.0] * len(discounts))
@@ -95,14 +111,14 @@
             DLM._setDiscounts(discounts_err)
             DLM.fitForwardFilter()
             gradient[i] = (DLM._getMSE() - self.current_mse) / self.err
 
         return gradient
 
     def cutoff(self, a):
-        if a < 0.1:
-            return 0.1
+        if a < 0.7:
+            return 0.7
 
         if a >= 1:
             return 0.99999
 
         return a
```

### Comparing `pydlm-0.1.1.8/pydlm.egg-info/PKG-INFO` & `pydlm-0.1.1.9/pydlm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pydlm
-Version: 0.1.1.8
+Version: 0.1.1.9
 Summary: A python library for the Bayesian dynamic linear model for time series modeling
 Home-page: https://github.com/wwrechard/pydlm
 Author: Xiangyu Wang
 Author-email: wwrechard@gmail.com
 License: BSD
 Description: UNKNOWN
 Keywords: dlm bayes bayesian kalman filter smoothing dynamic model
```

### Comparing `pydlm-0.1.1.8/pydlm.egg-info/SOURCES.txt` & `pydlm-0.1.1.9/pydlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydlm-0.1.1.8/setup.py` & `pydlm-0.1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'pydlm',
-    version = '0.1.1.8',
+    version = '0.1.1.9',
     author = 'Xiangyu Wang',
     author_email = 'wwrechard@gmail.com',
     description = ('A python library for the Bayesian dynamic linear ' +
       'model for time series modeling'),
     license = 'BSD',
     keywords = 'dlm bayes bayesian kalman filter smoothing dynamic model',
     url = 'https://github.com/wwrechard/pydlm',
```

