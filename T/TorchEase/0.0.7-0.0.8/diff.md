# Comparing `tmp/TorchEase-0.0.7.tar.gz` & `tmp/TorchEase-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchEase-0.0.7.tar", last modified: Sat May  6 10:29:24 2023, max compression
+gzip compressed data, was "TorchEase-0.0.8.tar", last modified: Sat May  6 10:35:51 2023, max compression
```

## Comparing `TorchEase-0.0.7.tar` & `TorchEase-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:29:24.280668 TorchEase-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-06 10:29:24.280668 TorchEase-0.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:29:24.276668 TorchEase-0.0.7/TorchEase/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-06 10:29:10.000000 TorchEase-0.0.7/TorchEase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-05-06 10:29:10.000000 TorchEase-0.0.7/TorchEase/fuser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-06 10:29:10.000000 TorchEase-0.0.7/TorchEase/modelbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-05-06 10:29:10.000000 TorchEase-0.0.7/TorchEase/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-06 10:29:10.000000 TorchEase-0.0.7/TorchEase/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-06 10:29:10.000000 TorchEase-0.0.7/TorchEase/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:29:24.280668 TorchEase-0.0.7/TorchEase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-06 10:29:24.000000 TorchEase-0.0.7/TorchEase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-06 10:29:24.000000 TorchEase-0.0.7/TorchEase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 10:29:24.000000 TorchEase-0.0.7/TorchEase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-06 10:29:24.000000 TorchEase-0.0.7/TorchEase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 10:29:24.000000 TorchEase-0.0.7/TorchEase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 10:29:24.280668 TorchEase-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-06 10:29:10.000000 TorchEase-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:35:51.458398 TorchEase-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-06 10:35:51.454398 TorchEase-0.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:35:51.454398 TorchEase-0.0.8/TorchEase/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-06 10:35:40.000000 TorchEase-0.0.8/TorchEase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-05-06 10:35:40.000000 TorchEase-0.0.8/TorchEase/fuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-06 10:35:40.000000 TorchEase-0.0.8/TorchEase/modelbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-05-06 10:35:40.000000 TorchEase-0.0.8/TorchEase/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-06 10:35:40.000000 TorchEase-0.0.8/TorchEase/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-06 10:35:40.000000 TorchEase-0.0.8/TorchEase/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 10:35:51.454398 TorchEase-0.0.8/TorchEase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-06 10:35:51.000000 TorchEase-0.0.8/TorchEase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-06 10:35:51.000000 TorchEase-0.0.8/TorchEase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 10:35:51.000000 TorchEase-0.0.8/TorchEase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-06 10:35:51.000000 TorchEase-0.0.8/TorchEase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 10:35:51.000000 TorchEase-0.0.8/TorchEase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 10:35:51.458398 TorchEase-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-06 10:35:40.000000 TorchEase-0.0.8/setup.py
```

### Comparing `TorchEase-0.0.7/PKG-INFO` & `TorchEase-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchEase
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simplifying working with PyTorch
 Author: Philipp Steigerwald
 Author-email: info@b-stream.info
 Keywords: python,torch,pytorch,early stop,trainer,tensor
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TorchEase-0.0.7/TorchEase/fuser.py` & `TorchEase-0.0.8/TorchEase/fuser.py`

 * *Files identical despite different names*

### Comparing `TorchEase-0.0.7/TorchEase/modelbase.py` & `TorchEase-0.0.8/TorchEase/modelbase.py`

 * *Files identical despite different names*

### Comparing `TorchEase-0.0.7/TorchEase/trainer.py` & `TorchEase-0.0.8/TorchEase/trainer.py`

 * *Files identical despite different names*

### Comparing `TorchEase-0.0.7/TorchEase/user.py` & `TorchEase-0.0.8/TorchEase/user.py`

 * *Files identical despite different names*

### Comparing `TorchEase-0.0.7/TorchEase/utilities.py` & `TorchEase-0.0.8/TorchEase/utilities.py`

 * *Files identical despite different names*

### Comparing `TorchEase-0.0.7/TorchEase.egg-info/PKG-INFO` & `TorchEase-0.0.8/TorchEase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchEase
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simplifying working with PyTorch
 Author: Philipp Steigerwald
 Author-email: info@b-stream.info
 Keywords: python,torch,pytorch,early stop,trainer,tensor
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TorchEase-0.0.7/setup.py` & `TorchEase-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 DESCRIPTION = 'Simplifying working with PyTorch'
 LONG_DESCRIPTION = 'TorchEase is a Python package that simplifies working with PyTorch, a popular deep learning framework. It provides a set of easy-to-use tools for training, testing, and deploying machine learning models. TorchEase includes features like early stopping, model fusing, and model evaluation, among others, which help streamline the model development process. Additionally, TorchEase is designed to be highly modular, making it easy to integrate into existing PyTorch projects.'
 
 #with open(os.path.join(os.path.dirname(__file__), "TorchEase", "VERSION")) as version_file:
 #    version = version_file.read().strip()
-version = "0.0.7"
+version = "0.0.8"
 
 # Setting up
 setup(
     name="TorchEase",
     version=version,
     author="Philipp Steigerwald",
     author_email="info@b-stream.info",
```

