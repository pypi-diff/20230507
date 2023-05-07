# Comparing `tmp/dataset-viewer-0.1.2.tar.gz` & `tmp/dataset-viewer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset-viewer-0.1.2.tar", last modified: Sun May  7 04:30:47 2023, max compression
+gzip compressed data, was "dataset-viewer-1.0.0.tar", last modified: Sun May  7 04:35:34 2023, max compression
```

## Comparing `dataset-viewer-0.1.2.tar` & `dataset-viewer-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 04:30:47.169928 dataset-viewer-0.1.2/
--rw-rw-rw-   0        0        0     1081 2023-05-03 02:47:20.000000 dataset-viewer-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      866 2023-05-07 04:30:47.168928 dataset-viewer-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-03 04:41:07.000000 dataset-viewer-0.1.2/README.md
--rw-rw-rw-   0        0        0      746 2023-05-07 04:30:31.000000 dataset-viewer-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 04:30:47.169928 dataset-viewer-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      291 2023-05-03 04:56:59.000000 dataset-viewer-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 04:30:47.143957 dataset-viewer-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-07 04:30:47.150931 dataset-viewer-0.1.2/src/dataset_viewer/
--rw-rw-rw-   0        0        0      142 2023-05-06 07:14:18.000000 dataset-viewer-0.1.2/src/dataset_viewer/__init__.py
--rw-rw-rw-   0        0        0     3014 2023-05-07 04:27:15.000000 dataset-viewer-0.1.2/src/dataset_viewer/dataset.py
--rw-rw-rw-   0        0        0     2518 2023-05-07 04:29:28.000000 dataset-viewer-0.1.2/src/dataset_viewer/viewer.py
-drwxrwxrwx   0        0        0        0 2023-05-07 04:30:47.167926 dataset-viewer-0.1.2/src/dataset_viewer.egg-info/
--rw-rw-rw-   0        0        0      866 2023-05-07 04:30:47.000000 dataset-viewer-0.1.2/src/dataset_viewer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-05-07 04:30:47.000000 dataset-viewer-0.1.2/src/dataset_viewer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 04:30:47.000000 dataset-viewer-0.1.2/src/dataset_viewer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-07 04:30:47.000000 dataset-viewer-0.1.2/src/dataset_viewer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-07 04:30:47.000000 dataset-viewer-0.1.2/src/dataset_viewer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 04:35:34.194184 dataset-viewer-1.0.0/
+-rw-rw-rw-   0        0        0     1081 2023-05-03 02:47:20.000000 dataset-viewer-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      866 2023-05-07 04:35:34.194184 dataset-viewer-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-03 04:41:07.000000 dataset-viewer-1.0.0/README.md
+-rw-rw-rw-   0        0        0      746 2023-05-07 04:35:00.000000 dataset-viewer-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 04:35:34.195201 dataset-viewer-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      291 2023-05-03 04:56:59.000000 dataset-viewer-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 04:35:34.171671 dataset-viewer-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 04:35:34.179185 dataset-viewer-1.0.0/src/dataset_viewer/
+-rw-rw-rw-   0        0        0      142 2023-05-06 07:14:18.000000 dataset-viewer-1.0.0/src/dataset_viewer/__init__.py
+-rw-rw-rw-   0        0        0     3014 2023-05-07 04:27:15.000000 dataset-viewer-1.0.0/src/dataset_viewer/dataset.py
+-rw-rw-rw-   0        0        0     2844 2023-05-07 04:34:26.000000 dataset-viewer-1.0.0/src/dataset_viewer/viewer.py
+drwxrwxrwx   0        0        0        0 2023-05-07 04:35:34.193184 dataset-viewer-1.0.0/src/dataset_viewer.egg-info/
+-rw-rw-rw-   0        0        0      866 2023-05-07 04:35:34.000000 dataset-viewer-1.0.0/src/dataset_viewer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-05-07 04:35:34.000000 dataset-viewer-1.0.0/src/dataset_viewer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 04:35:34.000000 dataset-viewer-1.0.0/src/dataset_viewer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-07 04:35:34.000000 dataset-viewer-1.0.0/src/dataset_viewer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-07 04:35:34.000000 dataset-viewer-1.0.0/src/dataset_viewer.egg-info/top_level.txt
```

### Comparing `dataset-viewer-0.1.2/LICENSE` & `dataset-viewer-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset-viewer-0.1.2/PKG-INFO` & `dataset-viewer-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-viewer
-Version: 0.1.2
+Version: 1.0.0
 Summary: Allow to view a dataset image by image and edit their labels
 Author-email: Hillpro <66534835+Hillpro@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Hillpro/dataset-viewer
 Project-URL: Bug Tracker, https://github.com/Hillpro/dataset-viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dataset-viewer-0.1.2/pyproject.toml` & `dataset-viewer-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataset-viewer"
-version = "0.1.2"
+version = "1.0.0"
 authors = [
   { name="Hillpro", email="66534835+Hillpro@users.noreply.github.com" },
 ]
 description = "Allow to view a dataset image by image and edit their labels"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dataset-viewer-0.1.2/src/dataset_viewer/dataset.py` & `dataset-viewer-1.0.0/src/dataset_viewer/dataset.py`

 * *Files identical despite different names*

### Comparing `dataset-viewer-0.1.2/src/dataset_viewer/viewer.py` & `dataset-viewer-1.0.0/src/dataset_viewer/viewer.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,30 @@
 from napari import Viewer as NapariViewer, layers
 import numpy as np
 
 from dataset_viewer.dataset import Dataset
 
 
 class Viewer():
+    '''
+    A class used to represent a Dataset to show in the Viewer
+
+    Attributes
+    ----------
+    viewer : Viewer
+        The viewer gui instance
+    dataset : Dataset
+        The current viewer dataset
+
+    Methods
+    -------
+    start()
+        Start the viewer gui with the current dataset
+    '''
+
     __image_idx = 0
 
     def __init__(self, dataset: Dataset = None):
         self.viewer = NapariViewer()
         self.dataset = dataset if dataset is not None else Dataset()
 
         self.labels_layer = None
```

### Comparing `dataset-viewer-0.1.2/src/dataset_viewer.egg-info/PKG-INFO` & `dataset-viewer-1.0.0/src/dataset_viewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-viewer
-Version: 0.1.2
+Version: 1.0.0
 Summary: Allow to view a dataset image by image and edit their labels
 Author-email: Hillpro <66534835+Hillpro@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Hillpro/dataset-viewer
 Project-URL: Bug Tracker, https://github.com/Hillpro/dataset-viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

