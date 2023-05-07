# Comparing `tmp/DeepSearchLite-0.1.0.tar.gz` & `tmp/DeepSearchLite-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepSearchLite-0.1.0.tar", last modified: Sun May  7 02:15:44 2023, max compression
+gzip compressed data, was "DeepSearchLite-0.1.1.tar", last modified: Sun May  7 04:14:21 2023, max compression
```

## Comparing `DeepSearchLite-0.1.0.tar` & `DeepSearchLite-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ibad      (1000) ibad      (1000)        0 2023-05-07 02:15:44.443247 DeepSearchLite-0.1.0/
-drwxrwxr-x   0 ibad      (1000) ibad      (1000)        0 2023-05-07 02:15:44.443247 DeepSearchLite-0.1.0/DeepSearchLite/
--rw-rw-r--   0 ibad      (1000) ibad      (1000)    12329 2023-05-07 02:12:25.000000 DeepSearchLite-0.1.0/DeepSearchLite/DeepSearchLite.py
--rw-rw-r--   0 ibad      (1000) ibad      (1000)       65 2023-05-07 01:07:56.000000 DeepSearchLite-0.1.0/DeepSearchLite/__init__.py
-drwxrwxr-x   0 ibad      (1000) ibad      (1000)        0 2023-05-07 02:15:44.443247 DeepSearchLite-0.1.0/DeepSearchLite.egg-info/
--rw-rw-r--   0 ibad      (1000) ibad      (1000)     3091 2023-05-07 02:15:44.000000 DeepSearchLite-0.1.0/DeepSearchLite.egg-info/PKG-INFO
--rw-rw-r--   0 ibad      (1000) ibad      (1000)      275 2023-05-07 02:15:44.000000 DeepSearchLite-0.1.0/DeepSearchLite.egg-info/SOURCES.txt
--rw-rw-r--   0 ibad      (1000) ibad      (1000)        1 2023-05-07 02:15:44.000000 DeepSearchLite-0.1.0/DeepSearchLite.egg-info/dependency_links.txt
--rw-rw-r--   0 ibad      (1000) ibad      (1000)       35 2023-05-07 02:15:44.000000 DeepSearchLite-0.1.0/DeepSearchLite.egg-info/requires.txt
--rw-rw-r--   0 ibad      (1000) ibad      (1000)       15 2023-05-07 02:15:44.000000 DeepSearchLite-0.1.0/DeepSearchLite.egg-info/top_level.txt
--rw-rw-r--   0 ibad      (1000) ibad      (1000)     1068 2023-05-07 01:06:14.000000 DeepSearchLite-0.1.0/LICENSE
--rw-rw-r--   0 ibad      (1000) ibad      (1000)     3091 2023-05-07 02:15:44.443247 DeepSearchLite-0.1.0/PKG-INFO
--rw-rw-r--   0 ibad      (1000) ibad      (1000)     2363 2023-05-07 02:09:18.000000 DeepSearchLite-0.1.0/README.md
--rw-rw-r--   0 ibad      (1000) ibad      (1000)       38 2023-05-07 02:15:44.443247 DeepSearchLite-0.1.0/setup.cfg
--rw-rw-r--   0 ibad      (1000) ibad      (1000)     1044 2023-05-07 02:14:22.000000 DeepSearchLite-0.1.0/setup.py
+drwxrwxr-x   0 ibad      (1000) ibad      (1000)        0 2023-05-07 04:14:21.233251 DeepSearchLite-0.1.1/
+drwxrwxr-x   0 ibad      (1000) ibad      (1000)        0 2023-05-07 04:14:21.233251 DeepSearchLite-0.1.1/DeepSearchLite/
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)    13903 2023-05-07 03:48:20.000000 DeepSearchLite-0.1.1/DeepSearchLite/DeepSearchLite.py
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)       65 2023-05-07 01:07:56.000000 DeepSearchLite-0.1.1/DeepSearchLite/__init__.py
+drwxrwxr-x   0 ibad      (1000) ibad      (1000)        0 2023-05-07 04:14:21.233251 DeepSearchLite-0.1.1/DeepSearchLite.egg-info/
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)     3091 2023-05-07 04:14:21.000000 DeepSearchLite-0.1.1/DeepSearchLite.egg-info/PKG-INFO
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)      275 2023-05-07 04:14:21.000000 DeepSearchLite-0.1.1/DeepSearchLite.egg-info/SOURCES.txt
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)        1 2023-05-07 04:14:21.000000 DeepSearchLite-0.1.1/DeepSearchLite.egg-info/dependency_links.txt
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)       35 2023-05-07 04:14:21.000000 DeepSearchLite-0.1.1/DeepSearchLite.egg-info/requires.txt
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)       15 2023-05-07 04:14:21.000000 DeepSearchLite-0.1.1/DeepSearchLite.egg-info/top_level.txt
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)     1068 2023-05-07 01:06:14.000000 DeepSearchLite-0.1.1/LICENSE
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)     3091 2023-05-07 04:14:21.233251 DeepSearchLite-0.1.1/PKG-INFO
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)     2363 2023-05-07 02:09:18.000000 DeepSearchLite-0.1.1/README.md
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)       38 2023-05-07 04:14:21.233251 DeepSearchLite-0.1.1/setup.cfg
+-rw-rw-r--   0 ibad      (1000) ibad      (1000)     1044 2023-05-07 02:48:29.000000 DeepSearchLite-0.1.1/setup.py
```

### Comparing `DeepSearchLite-0.1.0/DeepSearchLite/DeepSearchLite.py` & `DeepSearchLite-0.1.1/DeepSearchLite/DeepSearchLite.py`

 * *Files 7% similar despite different names*

```diff
@@ -320,7 +320,47 @@
 
     def load_metadata(self):
         """Loads the metadata and index for search mode."""
         self.image_data = pd.read_pickle(
             image_data_with_features_pkl(self.metadata_dir, self.model_name)
         )
         self.f = len(self.image_data["features"][0])
+
+
+    def _get_query_vector_from_image(self, image: Image) -> np.ndarray:
+        query_vector = self._extract(image)
+        return query_vector
+    
+    def get_similar_images_from_image(
+        self, image: Image, number_of_images: int = 10
+    ) -> Dict[int, str]:
+        """
+        Returns the most similar images to a given query image according to the indexed image features.
+
+        Parameters:
+        -----------
+        image : Image
+            The query image.
+        number_of_images : int, optional (default=10)
+            The number of most similar images to the query image to be returned.
+        """
+        query_vector = self._get_query_vector_from_image(image)
+        img_dict = self._search_by_vector(query_vector, number_of_images)
+        return img_dict
+    
+    def get_similar_images_list_from_image(
+        self, image: Image, number_of_images: int = 10
+    ) -> List[str]:
+        """
+        Returns the most similar images to a given query image according to the indexed image features.
+
+        Parameters:
+        -----------
+        image : Image
+            The query image.
+        number_of_images : int, optional (default=10)
+            The number of most similar images to the query image to be returned.
+        """
+        img_dict = self.get_similar_images_from_image(image, number_of_images)
+        similar_n_images =  list(img_dict.values())
+        similar_n_images_names = [os.path.basename(image_path) for image_path in similar_n_images]
+        return similar_n_images_names
```

### Comparing `DeepSearchLite-0.1.0/DeepSearchLite.egg-info/PKG-INFO` & `DeepSearchLite-0.1.1/DeepSearchLite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepSearchLite
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for image similarity search
 Home-page: https://github.com/ibadrather/DeepSearchLite
 Author: Ibad Rather
 Author-email: ibad.rather.ir@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `DeepSearchLite-0.1.0/LICENSE` & `DeepSearchLite-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepSearchLite-0.1.0/PKG-INFO` & `DeepSearchLite-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepSearchLite
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for image similarity search
 Home-page: https://github.com/ibadrather/DeepSearchLite
 Author: Ibad Rather
 Author-email: ibad.rather.ir@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `DeepSearchLite-0.1.0/README.md` & `DeepSearchLite-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `DeepSearchLite-0.1.0/setup.py` & `DeepSearchLite-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="DeepSearchLite",
-    version="0.1.0",
+    version="0.1.1",
     author="Ibad Rather",
     author_email="ibad.rather.ir@gmail.com",
     description="A package for image similarity search",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ibadrather/DeepSearchLite",
     packages=find_packages(),
```

