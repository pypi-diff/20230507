# Comparing `tmp/dataset-viewer-0.1.1.tar.gz` & `tmp/dataset-viewer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset-viewer-0.1.1.tar", last modified: Sat May  6 08:08:08 2023, max compression
+gzip compressed data, was "dataset-viewer-0.1.2.tar", last modified: Sun May  7 04:30:47 2023, max compression
```

## Comparing `dataset-viewer-0.1.1.tar` & `dataset-viewer-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 08:08:08.144076 dataset-viewer-0.1.1/
--rw-rw-rw-   0        0        0     1081 2023-05-03 02:47:20.000000 dataset-viewer-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      866 2023-05-06 08:08:08.144076 dataset-viewer-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-03 04:41:07.000000 dataset-viewer-0.1.1/README.md
--rw-rw-rw-   0        0        0      746 2023-05-06 08:07:24.000000 dataset-viewer-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 08:08:08.144076 dataset-viewer-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      291 2023-05-03 04:56:59.000000 dataset-viewer-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 08:08:08.121238 dataset-viewer-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 08:08:08.129324 dataset-viewer-0.1.1/src/dataset_viewer/
--rw-rw-rw-   0        0        0      142 2023-05-06 07:14:18.000000 dataset-viewer-0.1.1/src/dataset_viewer/__init__.py
--rw-rw-rw-   0        0        0     1509 2023-05-06 08:03:32.000000 dataset-viewer-0.1.1/src/dataset_viewer/dataset.py
--rw-rw-rw-   0        0        0     1892 2023-05-06 08:07:04.000000 dataset-viewer-0.1.1/src/dataset_viewer/viewer.py
-drwxrwxrwx   0        0        0        0 2023-05-06 08:08:08.143077 dataset-viewer-0.1.1/src/dataset_viewer.egg-info/
--rw-rw-rw-   0        0        0      866 2023-05-06 08:08:08.000000 dataset-viewer-0.1.1/src/dataset_viewer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-05-06 08:08:08.000000 dataset-viewer-0.1.1/src/dataset_viewer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 08:08:08.000000 dataset-viewer-0.1.1/src/dataset_viewer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-06 08:08:08.000000 dataset-viewer-0.1.1/src/dataset_viewer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-06 08:08:08.000000 dataset-viewer-0.1.1/src/dataset_viewer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 04:30:47.169928 dataset-viewer-0.1.2/
+-rw-rw-rw-   0        0        0     1081 2023-05-03 02:47:20.000000 dataset-viewer-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      866 2023-05-07 04:30:47.168928 dataset-viewer-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-03 04:41:07.000000 dataset-viewer-0.1.2/README.md
+-rw-rw-rw-   0        0        0      746 2023-05-07 04:30:31.000000 dataset-viewer-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 04:30:47.169928 dataset-viewer-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      291 2023-05-03 04:56:59.000000 dataset-viewer-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 04:30:47.143957 dataset-viewer-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 04:30:47.150931 dataset-viewer-0.1.2/src/dataset_viewer/
+-rw-rw-rw-   0        0        0      142 2023-05-06 07:14:18.000000 dataset-viewer-0.1.2/src/dataset_viewer/__init__.py
+-rw-rw-rw-   0        0        0     3014 2023-05-07 04:27:15.000000 dataset-viewer-0.1.2/src/dataset_viewer/dataset.py
+-rw-rw-rw-   0        0        0     2518 2023-05-07 04:29:28.000000 dataset-viewer-0.1.2/src/dataset_viewer/viewer.py
+drwxrwxrwx   0        0        0        0 2023-05-07 04:30:47.167926 dataset-viewer-0.1.2/src/dataset_viewer.egg-info/
+-rw-rw-rw-   0        0        0      866 2023-05-07 04:30:47.000000 dataset-viewer-0.1.2/src/dataset_viewer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-05-07 04:30:47.000000 dataset-viewer-0.1.2/src/dataset_viewer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 04:30:47.000000 dataset-viewer-0.1.2/src/dataset_viewer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-07 04:30:47.000000 dataset-viewer-0.1.2/src/dataset_viewer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-07 04:30:47.000000 dataset-viewer-0.1.2/src/dataset_viewer.egg-info/top_level.txt
```

### Comparing `dataset-viewer-0.1.1/LICENSE` & `dataset-viewer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset-viewer-0.1.1/PKG-INFO` & `dataset-viewer-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-viewer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Allow to view a dataset image by image and edit their labels
 Author-email: Hillpro <66534835+Hillpro@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Hillpro/dataset-viewer
 Project-URL: Bug Tracker, https://github.com/Hillpro/dataset-viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dataset-viewer-0.1.1/pyproject.toml` & `dataset-viewer-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataset-viewer"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Hillpro", email="66534835+Hillpro@users.noreply.github.com" },
 ]
 description = "Allow to view a dataset image by image and edit their labels"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dataset-viewer-0.1.1/src/dataset_viewer/dataset.py` & `dataset-viewer-0.1.2/src/dataset_viewer/dataset.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,48 +7,113 @@
 
 
 DEFAULT_PATH = Path('..', '..', 'data')
 VALID_FILE_TYPES = ["jpg", "jpeg", "png"]
 
 
 def image_name(img):
+    '''Gets the image name without extension'''
     return Path(img.filename).name
 
 
+def image_stem(img):
+    '''Gets the image name without extension'''
+    return Path(img.filename).stem
+
+
 def empty_image(img):
+    '''Gets an empty image'''
     return fromarray(np.full(img.size[::-1], 0))
 
 
 class Dataset():
+    '''
+    A class used to represent a Dataset to show in the Viewer
+
+    Attributes
+    ----------
+    images : list
+        List of all loaded images
+
+    Raises
+    -------
+    Exception
+        If no images can be found
+    '''
+
     def __init__(self, data_path: Path = None):
+        '''
+        Parameters
+        ----------
+        data_path : Path
+            The path for images and labels
+        '''
+
         if data_path is None:
             data_path = DEFAULT_PATH
 
         self.images_path = data_path / 'images'
         self.labels_path = data_path / 'labels'
 
         _images = [glob(f'{self.images_path}/*.{ext}') for ext in VALID_FILE_TYPES]
         self.images = [open(item) for i in _images for item in i]
 
         if len(self.images) == 0:
             raise Exception('No images were found')
 
+
     def get(self, index: int) -> tuple[Image, str]:
+        '''Gets a image by index
+
+        Parameters
+        ----------
+        index: int
+            The index of the image
+
+        Returns
+        -------
+        Image
+            The image at the index
+        str
+            The name of the image
+        '''
         index %= len(self.images)
         image = self.images[index]
         return image, image_name(image)
 
     def get_labels_for(self, image):
+        '''Gets the labels image for a specified image
+
+        Parameters
+        ----------
+        img: Image
+            The image to get the labels from
+
+        Returns
+        -------
+        Image
+            the labels image, or an empty image if no labels exists
+        '''
         try:
-            return open(f'{self.labels_path}/{image_name(image)}')
+            # We need to save as png since other formats are using compression
+            return open(f'{self.labels_path}/{image_stem(image)}.png')
         except IOError:
             return empty_image(image)
 
     def save_labels(self, index: int, data):
+        '''Save the labels for the image
+
+        Parameters
+        ----------
+        index: int
+            Index of the image to save the labels for
+        data: Any
+            the numpy array containing the labels data
+        '''
         im = fromarray(data.astype(np.uint8))
-        _, name = self.get(index)
-        save_path = f'{self.labels_path}/{name}'
+        image, _ = self.get(index)
+        save_path = f'{self.labels_path}/{image_stem(image)}.png'
 
         if np.sum(im) > 0:
             im.save(save_path)
         elif os.path.exists(save_path):
             os.remove(save_path)
```

### Comparing `dataset-viewer-0.1.1/src/dataset_viewer/viewer.py` & `dataset-viewer-0.1.2/src/dataset_viewer/viewer.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,45 +12,63 @@
         self.viewer = NapariViewer()
         self.dataset = dataset if dataset is not None else Dataset()
 
         self.labels_layer = None
         self.__set_bindings()
 
     def start(self):
+        '''Starts the viewer gui with the first image in the dataset'''
         self.__show_image(0)
         napari.run()
 
     def __set_bindings(self):
-        # Add reset option ('r')
+        '''Set the current viewer key bindings'''
+        # TODO: Add reset option ('r')
         self.__bind_key('l', self.__current_label_name)
         self.__bind_key('Escape', self.__exit)
         self.__bind_key('Left', self.__previous)
         self.__bind_key('Right', self.__next)
 
     def __bind_key(self, key, func):
+        '''Set a key binding the the viewer'''
         self.viewer.bind_key(key, func)
 
     def __previous(self, viewer: NapariViewer):
         self.__show_image(-1)
 
     def __next(self, viewer: NapariViewer):
         self.__show_image(1)
 
     def __show_image(self, move=0):
+        '''Save current image labels and goes to the next image
+
+        Parameters
+        ----------
+        move : int
+            movement applied to the current image index.
+            0 to show the current image, 1 to show next, -1 to show previous
+        '''
         if self.labels_layer is not None:
             self.dataset.save_labels(self.__image_idx, self.labels_layer.data)
 
         self.__image_idx += move
         self.viewer.layers.clear()
 
         image, name = self.dataset.get(self.__image_idx)
         self.viewer.add_image(np.array(image), name=name)
         self.__set_labels_layer(image)
 
     def __set_labels_layer(self, image):
+        '''Set the labels layer for an image
+
+        Parameters
+        ----------
+        image : Image
+            Image to set the labels layer from
+        '''
         labels = self.dataset.get_labels_for(image)
         self.labels_layer = self.viewer.add_labels(np.array(labels), name='segmentation')
         self.labels_layer.mode = 'PAINT'
 
     def __current_label_name(self, viewer: NapariViewer):
         active_layer = viewer.layers.selection.active
```

### Comparing `dataset-viewer-0.1.1/src/dataset_viewer.egg-info/PKG-INFO` & `dataset-viewer-0.1.2/src/dataset_viewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-viewer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Allow to view a dataset image by image and edit their labels
 Author-email: Hillpro <66534835+Hillpro@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/Hillpro/dataset-viewer
 Project-URL: Bug Tracker, https://github.com/Hillpro/dataset-viewer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

