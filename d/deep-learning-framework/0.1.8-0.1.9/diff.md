# Comparing `tmp/deep_learning_framework-0.1.8.tar.gz` & `tmp/deep_learning_framework-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_learning_framework-0.1.8.tar", last modified: Thu Jul 21 08:04:17 2022, max compression
+gzip compressed data, was "deep_learning_framework-0.1.9.tar", last modified: Thu Jul 21 08:06:18 2022, max compression
```

## Comparing `deep_learning_framework-0.1.8.tar` & `deep_learning_framework-0.1.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 theorieken   (501) staff       (20)        0 2022-07-21 08:04:17.712220 deep_learning_framework-0.1.8/
--rw-r--r--   0 theorieken   (501) staff       (20)     1054 2022-07-20 14:55:31.000000 deep_learning_framework-0.1.8/LICENSE.txt
--rw-r--r--   0 theorieken   (501) staff       (20)      293 2022-07-21 08:04:17.712287 deep_learning_framework-0.1.8/PKG-INFO
--rw-r--r--   0 theorieken   (501) staff       (20)     5825 2022-07-20 15:49:59.000000 deep_learning_framework-0.1.8/README.md
--rw-r--r--   0 theorieken   (501) staff       (20)      107 2022-07-21 08:04:17.712509 deep_learning_framework-0.1.8/setup.cfg
--rw-r--r--   0 theorieken   (501) staff       (20)      576 2022-07-21 08:04:14.000000 deep_learning_framework-0.1.8/setup.py
-drwxr-xr-x   0 theorieken   (501) staff       (20)        0 2022-07-21 08:04:17.706055 deep_learning_framework-0.1.8/src/
-drwxr-xr-x   0 theorieken   (501) staff       (20)        0 2022-07-21 08:04:17.707514 deep_learning_framework-0.1.8/src/deep_learning_framework.egg-info/
--rw-r--r--   0 theorieken   (501) staff       (20)      293 2022-07-21 08:04:17.000000 deep_learning_framework-0.1.8/src/deep_learning_framework.egg-info/PKG-INFO
--rw-r--r--   0 theorieken   (501) staff       (20)     1023 2022-07-21 08:04:17.000000 deep_learning_framework-0.1.8/src/deep_learning_framework.egg-info/SOURCES.txt
--rw-r--r--   0 theorieken   (501) staff       (20)        1 2022-07-21 08:04:17.000000 deep_learning_framework-0.1.8/src/deep_learning_framework.egg-info/dependency_links.txt
--rw-r--r--   0 theorieken   (501) staff       (20)       81 2022-07-21 08:04:17.000000 deep_learning_framework-0.1.8/src/deep_learning_framework.egg-info/requires.txt
--rw-r--r--   0 theorieken   (501) staff       (20)       10 2022-07-21 08:04:17.000000 deep_learning_framework-0.1.8/src/deep_learning_framework.egg-info/top_level.txt
-drwxr-xr-x   0 theorieken   (501) staff       (20)        0 2022-07-21 08:04:17.709183 deep_learning_framework-0.1.8/src/deepframe/
-drwxr-xr-x   0 theorieken   (501) staff       (20)        0 2022-07-21 08:04:17.710217 deep_learning_framework-0.1.8/src/deepframe/Dataset/
--rw-r--r--   0 theorieken   (501) staff       (20)     1032 2022-07-20 15:55:33.000000 deep_learning_framework-0.1.8/src/deepframe/Dataset/BaseDataset.py
--rw-r--r--   0 theorieken   (501) staff       (20)       77 2022-07-21 08:04:07.000000 deep_learning_framework-0.1.8/src/deepframe/Dataset/__init__.py
--rw-r--r--   0 theorieken   (501) staff       (20)     8560 2022-07-02 09:51:37.000000 deep_learning_framework-0.1.8/src/deepframe/Dataset/transforms.py
--rw-r--r--   0 theorieken   (501) staff       (20)     3289 2022-07-20 15:25:13.000000 deep_learning_framework-0.1.8/src/deepframe/Dataset/utils.py
-drwxr-xr-x   0 theorieken   (501) staff       (20)        0 2022-07-21 08:04:17.710849 deep_learning_framework-0.1.8/src/deepframe/Evaluator/
--rw-r--r--   0 theorieken   (501) staff       (20)      544 2022-05-24 16:36:15.000000 deep_learning_framework-0.1.8/src/deepframe/Evaluator/BaseEvaluator.py
--rw-r--r--   0 theorieken   (501) staff       (20)       30 2022-07-21 08:04:03.000000 deep_learning_framework-0.1.8/src/deepframe/Evaluator/__init__.py
-drwxr-xr-x   0 theorieken   (501) staff       (20)        0 2022-07-21 08:04:17.711195 deep_learning_framework-0.1.8/src/deepframe/MetricLogger/
--rw-r--r--   0 theorieken   (501) staff       (20)     2097 2022-06-27 12:29:19.000000 deep_learning_framework-0.1.8/src/deepframe/MetricLogger/BaseMetricLogger.py
--rw-r--r--   0 theorieken   (501) staff       (20)       33 2022-07-21 08:04:00.000000 deep_learning_framework-0.1.8/src/deepframe/MetricLogger/__init__.py
-drwxr-xr-x   0 theorieken   (501) staff       (20)        0 2022-07-21 08:04:17.711604 deep_learning_framework-0.1.8/src/deepframe/Model/
--rw-r--r--   0 theorieken   (501) staff       (20)     1253 2022-07-20 14:19:16.000000 deep_learning_framework-0.1.8/src/deepframe/Model/BaseNeuralNetwork.py
-drwxr-xr-x   0 theorieken   (501) staff       (20)        0 2022-07-21 08:04:17.712115 deep_learning_framework-0.1.8/src/deepframe/Model/NeuralNetworks/
--rw-r--r--   0 theorieken   (501) staff       (20)        0 2022-07-20 14:17:30.000000 deep_learning_framework-0.1.8/src/deepframe/Model/NeuralNetworks/Convolutional.py
--rw-r--r--   0 theorieken   (501) staff       (20)     4599 2022-07-20 15:25:13.000000 deep_learning_framework-0.1.8/src/deepframe/Model/NeuralNetworks/FullyConnected.py
--rw-r--r--   0 theorieken   (501) staff       (20)        0 2022-07-20 14:17:36.000000 deep_learning_framework-0.1.8/src/deepframe/Model/NeuralNetworks/Recursive.py
--rw-r--r--   0 theorieken   (501) staff       (20)       87 2022-07-21 08:03:56.000000 deep_learning_framework-0.1.8/src/deepframe/Model/NeuralNetworks/__init__.py
--rw-r--r--   0 theorieken   (501) staff       (20)       87 2022-07-21 08:03:53.000000 deep_learning_framework-0.1.8/src/deepframe/Model/__init__.py
--rw-r--r--   0 theorieken   (501) staff       (20)        0 2022-07-20 14:19:32.000000 deep_learning_framework-0.1.8/src/deepframe/Model/utils.py
--rw-r--r--   0 theorieken   (501) staff       (20)      275 2022-05-14 15:59:58.000000 deep_learning_framework-0.1.8/src/deepframe/MultiRunner.py
--rw-r--r--   0 theorieken   (501) staff       (20)    36305 2022-07-20 15:37:31.000000 deep_learning_framework-0.1.8/src/deepframe/Runner.py
--rw-r--r--   0 theorieken   (501) staff       (20)      197 2022-07-21 08:03:48.000000 deep_learning_framework-0.1.8/src/deepframe/__init__.py
--rw-r--r--   0 theorieken   (501) staff       (20)     2855 2022-07-20 14:20:16.000000 deep_learning_framework-0.1.8/src/deepframe/losses.py
--rw-r--r--   0 theorieken   (501) staff       (20)     8815 2022-07-20 14:20:31.000000 deep_learning_framework-0.1.8/src/deepframe/utils.py
+drwxr-xr-x   0 theorieken   (501) staff       (20)        0 2022-07-21 08:06:18.627073 deep_learning_framework-0.1.9/
+-rw-r--r--   0 theorieken   (501) staff       (20)     1054 2022-07-20 14:55:31.000000 deep_learning_framework-0.1.9/LICENSE.txt
+-rw-r--r--   0 theorieken   (501) staff       (20)      293 2022-07-21 08:06:18.627132 deep_learning_framework-0.1.9/PKG-INFO
+-rw-r--r--   0 theorieken   (501) staff       (20)     5825 2022-07-20 15:49:59.000000 deep_learning_framework-0.1.9/README.md
+-rw-r--r--   0 theorieken   (501) staff       (20)      107 2022-07-21 08:06:18.628112 deep_learning_framework-0.1.9/setup.cfg
+-rw-r--r--   0 theorieken   (501) staff       (20)      576 2022-07-21 08:06:16.000000 deep_learning_framework-0.1.9/setup.py
+drwxr-xr-x   0 theorieken   (501) staff       (20)        0 2022-07-21 08:06:18.620888 deep_learning_framework-0.1.9/src/
+drwxr-xr-x   0 theorieken   (501) staff       (20)        0 2022-07-21 08:06:18.622377 deep_learning_framework-0.1.9/src/deep_learning_framework.egg-info/
+-rw-r--r--   0 theorieken   (501) staff       (20)      293 2022-07-21 08:06:18.000000 deep_learning_framework-0.1.9/src/deep_learning_framework.egg-info/PKG-INFO
+-rw-r--r--   0 theorieken   (501) staff       (20)     1023 2022-07-21 08:06:18.000000 deep_learning_framework-0.1.9/src/deep_learning_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 theorieken   (501) staff       (20)        1 2022-07-21 08:06:18.000000 deep_learning_framework-0.1.9/src/deep_learning_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 theorieken   (501) staff       (20)       81 2022-07-21 08:06:18.000000 deep_learning_framework-0.1.9/src/deep_learning_framework.egg-info/requires.txt
+-rw-r--r--   0 theorieken   (501) staff       (20)       10 2022-07-21 08:06:18.000000 deep_learning_framework-0.1.9/src/deep_learning_framework.egg-info/top_level.txt
+drwxr-xr-x   0 theorieken   (501) staff       (20)        0 2022-07-21 08:06:18.623440 deep_learning_framework-0.1.9/src/deepframe/
+drwxr-xr-x   0 theorieken   (501) staff       (20)        0 2022-07-21 08:06:18.624393 deep_learning_framework-0.1.9/src/deepframe/Dataset/
+-rw-r--r--   0 theorieken   (501) staff       (20)     1032 2022-07-20 15:55:33.000000 deep_learning_framework-0.1.9/src/deepframe/Dataset/BaseDataset.py
+-rw-r--r--   0 theorieken   (501) staff       (20)       77 2022-07-21 08:04:07.000000 deep_learning_framework-0.1.9/src/deepframe/Dataset/__init__.py
+-rw-r--r--   0 theorieken   (501) staff       (20)     8560 2022-07-02 09:51:37.000000 deep_learning_framework-0.1.9/src/deepframe/Dataset/transforms.py
+-rw-r--r--   0 theorieken   (501) staff       (20)     3285 2022-07-21 08:06:09.000000 deep_learning_framework-0.1.9/src/deepframe/Dataset/utils.py
+drwxr-xr-x   0 theorieken   (501) staff       (20)        0 2022-07-21 08:06:18.624820 deep_learning_framework-0.1.9/src/deepframe/Evaluator/
+-rw-r--r--   0 theorieken   (501) staff       (20)      544 2022-05-24 16:36:15.000000 deep_learning_framework-0.1.9/src/deepframe/Evaluator/BaseEvaluator.py
+-rw-r--r--   0 theorieken   (501) staff       (20)       30 2022-07-21 08:04:03.000000 deep_learning_framework-0.1.9/src/deepframe/Evaluator/__init__.py
+drwxr-xr-x   0 theorieken   (501) staff       (20)        0 2022-07-21 08:06:18.625268 deep_learning_framework-0.1.9/src/deepframe/MetricLogger/
+-rw-r--r--   0 theorieken   (501) staff       (20)     2097 2022-06-27 12:29:19.000000 deep_learning_framework-0.1.9/src/deepframe/MetricLogger/BaseMetricLogger.py
+-rw-r--r--   0 theorieken   (501) staff       (20)       33 2022-07-21 08:04:00.000000 deep_learning_framework-0.1.9/src/deepframe/MetricLogger/__init__.py
+drwxr-xr-x   0 theorieken   (501) staff       (20)        0 2022-07-21 08:06:18.626531 deep_learning_framework-0.1.9/src/deepframe/Model/
+-rw-r--r--   0 theorieken   (501) staff       (20)     1253 2022-07-20 14:19:16.000000 deep_learning_framework-0.1.9/src/deepframe/Model/BaseNeuralNetwork.py
+drwxr-xr-x   0 theorieken   (501) staff       (20)        0 2022-07-21 08:06:18.626871 deep_learning_framework-0.1.9/src/deepframe/Model/NeuralNetworks/
+-rw-r--r--   0 theorieken   (501) staff       (20)        0 2022-07-20 14:17:30.000000 deep_learning_framework-0.1.9/src/deepframe/Model/NeuralNetworks/Convolutional.py
+-rw-r--r--   0 theorieken   (501) staff       (20)     4595 2022-07-21 08:06:06.000000 deep_learning_framework-0.1.9/src/deepframe/Model/NeuralNetworks/FullyConnected.py
+-rw-r--r--   0 theorieken   (501) staff       (20)        0 2022-07-20 14:17:36.000000 deep_learning_framework-0.1.9/src/deepframe/Model/NeuralNetworks/Recursive.py
+-rw-r--r--   0 theorieken   (501) staff       (20)       87 2022-07-21 08:03:56.000000 deep_learning_framework-0.1.9/src/deepframe/Model/NeuralNetworks/__init__.py
+-rw-r--r--   0 theorieken   (501) staff       (20)       87 2022-07-21 08:03:53.000000 deep_learning_framework-0.1.9/src/deepframe/Model/__init__.py
+-rw-r--r--   0 theorieken   (501) staff       (20)        0 2022-07-20 14:19:32.000000 deep_learning_framework-0.1.9/src/deepframe/Model/utils.py
+-rw-r--r--   0 theorieken   (501) staff       (20)      275 2022-05-14 15:59:58.000000 deep_learning_framework-0.1.9/src/deepframe/MultiRunner.py
+-rw-r--r--   0 theorieken   (501) staff       (20)    36297 2022-07-21 08:05:56.000000 deep_learning_framework-0.1.9/src/deepframe/Runner.py
+-rw-r--r--   0 theorieken   (501) staff       (20)      197 2022-07-21 08:03:48.000000 deep_learning_framework-0.1.9/src/deepframe/__init__.py
+-rw-r--r--   0 theorieken   (501) staff       (20)     2855 2022-07-20 14:20:16.000000 deep_learning_framework-0.1.9/src/deepframe/losses.py
+-rw-r--r--   0 theorieken   (501) staff       (20)     8815 2022-07-20 14:20:31.000000 deep_learning_framework-0.1.9/src/deepframe/utils.py
```

### Comparing `deep_learning_framework-0.1.8/LICENSE.txt` & `deep_learning_framework-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deep_learning_framework-0.1.8/README.md` & `deep_learning_framework-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `deep_learning_framework-0.1.8/setup.py` & `deep_learning_framework-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='deep_learning_framework',
-    version='0.1.8',
+    version='0.1.9',
     license='MIT',
     author="Theo Rieken",
     author_email='mail@theorieken.de',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/theorieken/deep-learning-framework',
     keywords='deep learning',
```

### Comparing `deep_learning_framework-0.1.8/src/deep_learning_framework.egg-info/SOURCES.txt` & `deep_learning_framework-0.1.9/src/deep_learning_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deep_learning_framework-0.1.8/src/deepframe/Dataset/BaseDataset.py` & `deep_learning_framework-0.1.9/src/deepframe/Dataset/BaseDataset.py`

 * *Files identical despite different names*

### Comparing `deep_learning_framework-0.1.8/src/deepframe/Dataset/transforms.py` & `deep_learning_framework-0.1.9/src/deepframe/Dataset/transforms.py`

 * *Files identical despite different names*

### Comparing `deep_learning_framework-0.1.8/src/deepframe/Dataset/utils.py` & `deep_learning_framework-0.1.9/src/deepframe/Dataset/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This file contains the data transformer, an instance that applies the
 specified transformations to the data samples
 """
 
 import importlib
 import copy
-from src.deepframe.utils import Logger
+from deepframe.utils import Logger
 
 
 class BaseTransform(object):
 
     prior_knowledge = None
 
     def __init__(self):
```

### Comparing `deep_learning_framework-0.1.8/src/deepframe/Evaluator/BaseEvaluator.py` & `deep_learning_framework-0.1.9/src/deepframe/Evaluator/BaseEvaluator.py`

 * *Files identical despite different names*

### Comparing `deep_learning_framework-0.1.8/src/deepframe/MetricLogger/BaseMetricLogger.py` & `deep_learning_framework-0.1.9/src/deepframe/MetricLogger/BaseMetricLogger.py`

 * *Files identical despite different names*

### Comparing `deep_learning_framework-0.1.8/src/deepframe/Model/BaseNeuralNetwork.py` & `deep_learning_framework-0.1.9/src/deepframe/Model/BaseNeuralNetwork.py`

 * *Files identical despite different names*

### Comparing `deep_learning_framework-0.1.8/src/deepframe/Model/NeuralNetworks/FullyConnected.py` & `deep_learning_framework-0.1.9/src/deepframe/Model/NeuralNetworks/FullyConnected.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import importlib
 import sys
 import traceback
 import torch
-from src.deepframe.utils import Logger
+from deepframe.utils import Logger
 from ..BaseNeuralNetwork import BaseNeuralNetwork
 
 
 class AutomaticNetwork(BaseNeuralNetwork):
     """
     This network is fed by the job description files. Please do not change
     this code!
```

### Comparing `deep_learning_framework-0.1.8/src/deepframe/Runner.py` & `deep_learning_framework-0.1.9/src/deepframe/Runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This file contains the runner class which runs jobs (input as path to json)
 """
 import pandas as pd
 
-from src.deepframe.utils import Logger, Timer, bcolors
-from src.deepframe.Model.NeuralNetworks.FullyConnected import AutomaticNetwork
+from deepframe.utils import Logger, Timer, bcolors
+from deepframe.Model.NeuralNetworks.FullyConnected import AutomaticNetwork
 from torch.utils.data import random_split, DataLoader
 from pathlib import Path
 from torch import autograd
 import torch
 import ssl
 import traceback
 import wandb
```

### Comparing `deep_learning_framework-0.1.8/src/deepframe/losses.py` & `deep_learning_framework-0.1.9/src/deepframe/losses.py`

 * *Files identical despite different names*

### Comparing `deep_learning_framework-0.1.8/src/deepframe/utils.py` & `deep_learning_framework-0.1.9/src/deepframe/utils.py`

 * *Files identical despite different names*

