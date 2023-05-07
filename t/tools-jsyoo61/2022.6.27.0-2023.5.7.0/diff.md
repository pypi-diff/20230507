# Comparing `tmp/tools-jsyoo61-2022.6.27.0.tar.gz` & `tmp/tools-jsyoo61-2023.5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tools-jsyoo61-2022.6.27.0.tar", last modified: Mon Jun 27 14:32:33 2022, max compression
+gzip compressed data, was "tools-jsyoo61-2023.5.7.0.tar", last modified: Sun May  7 06:27:19 2023, max compression
```

## Comparing `tools-jsyoo61-2022.6.27.0.tar` & `tools-jsyoo61-2023.5.7.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxrwxrwx   0        0        0        0 2022-06-27 14:32:33.809644 tools-jsyoo61-2022.6.27.0/
--rw-rw-rw-   0        0        0     1509 2022-06-27 14:32:33.809644 tools-jsyoo61-2022.6.27.0/PKG-INFO
--rw-rw-rw-   0        0        0      861 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/README.md
--rw-rw-rw-   0        0        0       42 2022-06-27 14:32:33.809644 tools-jsyoo61-2022.6.27.0/setup.cfg
--rw-rw-rw-   0        0        0      821 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-06-27 14:32:33.662642 tools-jsyoo61-2022.6.27.0/tools/
--rw-rw-rw-   0        0        0      293 2022-06-27 14:31:47.000000 tools-jsyoo61-2022.6.27.0/tools/__init__.py
--rw-rw-rw-   0        0        0     1100 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/array.py
--rw-rw-rw-   0        0        0     3207 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/data.py
--rw-rw-rw-   0        0        0     6927 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/exp.py
-drwxrwxrwx   0        0        0        0 2022-06-27 14:32:33.665642 tools-jsyoo61-2022.6.27.0/tools/hydra/
--rw-rw-rw-   0        0        0      143 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/hydra/__init__.py
--rw-rw-rw-   0        0        0     2406 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/modules.py
-drwxrwxrwx   0        0        0        0 2022-06-27 14:32:33.690642 tools-jsyoo61-2022.6.27.0/tools/numpy/
--rw-rw-rw-   0        0        0      235 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/numpy/__init__.py
--rw-rw-rw-   0        0        0     1389 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/numpy/_f.py
--rw-rw-rw-   0        0        0      960 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/numpy/_utils.py
--rw-rw-rw-   0        0        0     2219 2022-05-01 04:19:35.000000 tools-jsyoo61-2022.6.27.0/tools/os.py
-drwxrwxrwx   0        0        0        0 2022-06-27 14:32:33.693643 tools-jsyoo61-2022.6.27.0/tools/pandas/
--rw-rw-rw-   0        0        0       40 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/pandas/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-27 14:32:33.708643 tools-jsyoo61-2022.6.27.0/tools/plot/
--rw-rw-rw-   0        0        0       86 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/plot/__init__.py
--rw-rw-rw-   0        0        0      809 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/plot/sklearn.py
--rw-rw-rw-   0        0        0     2371 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/plot/utils.py
--rw-rw-rw-   0        0        0      834 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/random.py
-drwxrwxrwx   0        0        0        0 2022-06-27 14:32:33.730641 tools-jsyoo61-2022.6.27.0/tools/sklearn/
--rw-rw-rw-   0        0        0       33 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/sklearn/__init__.py
--rw-rw-rw-   0        0        0     4749 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/sklearn/model_selection.py
-drwxrwxrwx   0        0        0        0 2022-06-27 14:32:33.735642 tools-jsyoo61-2022.6.27.0/tools/stats/
--rw-rw-rw-   0        0        0      881 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/stats/__init__.py
--rw-rw-rw-   0        0        0    14598 2022-06-19 15:51:29.000000 tools-jsyoo61-2022.6.27.0/tools/tools.py
-drwxrwxrwx   0        0        0        0 2022-06-27 14:32:33.784643 tools-jsyoo61-2022.6.27.0/tools/torch/
--rw-rw-rw-   0        0        0      460 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/torch/__init__.py
--rw-rw-rw-   0        0        0      333 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/torch/_pandas.py
--rw-rw-rw-   0        0        0     2046 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/torch/estimator.py
--rw-rw-rw-   0        0        0    10951 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/torch/federated_learning.py
--rw-rw-rw-   0        0        0      310 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/torch/layers.py
--rw-rw-rw-   0        0        0    17852 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/torch/model.py
-drwxrwxrwx   0        0        0        0 2022-06-27 14:32:33.793643 tools-jsyoo61-2022.6.27.0/tools/torch/optim/
--rw-rw-rw-   0        0        0       30 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/torch/optim/__init__.py
--rw-rw-rw-   0        0        0     8208 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/torch/optim/lr_scheduler.py
--rw-rw-rw-   0        0        0      266 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/torch/plot.py
--rw-rw-rw-   0        0        0     2880 2022-05-01 04:16:16.000000 tools-jsyoo61-2022.6.27.0/tools/torch/utils.py
-drwxrwxrwx   0        0        0        0 2022-06-27 14:32:33.808643 tools-jsyoo61-2022.6.27.0/tools_jsyoo61.egg-info/
--rw-rw-rw-   0        0        0     1509 2022-06-27 14:32:33.000000 tools-jsyoo61-2022.6.27.0/tools_jsyoo61.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      837 2022-06-27 14:32:33.000000 tools-jsyoo61-2022.6.27.0/tools_jsyoo61.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-27 14:32:33.000000 tools-jsyoo61-2022.6.27.0/tools_jsyoo61.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2022-06-27 14:32:33.000000 tools-jsyoo61-2022.6.27.0/tools_jsyoo61.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-06-27 14:32:33.000000 tools-jsyoo61-2022.6.27.0/tools_jsyoo61.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 06:27:19.678982 tools-jsyoo61-2023.5.7.0/
+-rw-rw-rw-   0        0        0     1089 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1342 2023-05-07 06:27:19.676966 tools-jsyoo61-2023.5.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-07 06:27:19.679977 tools-jsyoo61-2023.5.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      821 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:27:19.527431 tools-jsyoo61-2023.5.7.0/tools/
+-rw-rw-rw-   0        0        0      292 2023-05-07 06:27:06.000000 tools-jsyoo61-2023.5.7.0/tools/__init__.py
+-rw-rw-rw-   0        0        0     1100 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/array.py
+-rw-rw-rw-   0        0        0     3207 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/data.py
+-rw-rw-rw-   0        0        0     6927 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/exp.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:27:19.531922 tools-jsyoo61-2023.5.7.0/tools/hydra/
+-rw-rw-rw-   0        0        0      143 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/hydra/__init__.py
+-rw-rw-rw-   0        0        0     3263 2022-09-12 22:10:08.000000 tools-jsyoo61-2023.5.7.0/tools/modules.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:27:19.546327 tools-jsyoo61-2023.5.7.0/tools/numpy/
+-rw-rw-rw-   0        0        0      235 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/numpy/__init__.py
+-rw-rw-rw-   0        0        0     1389 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/numpy/_f.py
+-rw-rw-rw-   0        0        0      960 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/numpy/_utils.py
+-rw-rw-rw-   0        0        0     2219 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/os.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:27:19.551772 tools-jsyoo61-2023.5.7.0/tools/pandas/
+-rw-rw-rw-   0        0        0       40 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/pandas/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:27:19.564397 tools-jsyoo61-2023.5.7.0/tools/plot/
+-rw-rw-rw-   0        0        0       86 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/plot/__init__.py
+-rw-rw-rw-   0        0        0      809 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/plot/sklearn.py
+-rw-rw-rw-   0        0        0     2371 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/plot/utils.py
+-rw-rw-rw-   0        0        0      834 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/random.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:27:19.571759 tools-jsyoo61-2023.5.7.0/tools/sklearn/
+-rw-rw-rw-   0        0        0       33 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/sklearn/__init__.py
+-rw-rw-rw-   0        0        0     4749 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/sklearn/model_selection.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:27:19.575753 tools-jsyoo61-2023.5.7.0/tools/stats/
+-rw-rw-rw-   0        0        0      881 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/stats/__init__.py
+-rw-rw-rw-   0        0        0    14715 2023-05-07 06:26:42.000000 tools-jsyoo61-2023.5.7.0/tools/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:27:19.615564 tools-jsyoo61-2023.5.7.0/tools/torch/
+-rw-rw-rw-   0        0        0      460 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/torch/__init__.py
+-rw-rw-rw-   0        0        0      333 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/torch/_pandas.py
+-rw-rw-rw-   0        0        0     2046 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/torch/estimator.py
+-rw-rw-rw-   0        0        0    10951 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/torch/federated_learning.py
+-rw-rw-rw-   0        0        0      310 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/torch/layers.py
+-rw-rw-rw-   0        0        0    17852 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/torch/model.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:27:19.622878 tools-jsyoo61-2023.5.7.0/tools/torch/optim/
+-rw-rw-rw-   0        0        0       30 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/torch/optim/__init__.py
+-rw-rw-rw-   0        0        0     8208 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/torch/optim/lr_scheduler.py
+-rw-rw-rw-   0        0        0      266 2022-07-01 04:57:33.000000 tools-jsyoo61-2023.5.7.0/tools/torch/plot.py
+-rw-rw-rw-   0        0        0     2880 2022-08-18 21:12:21.000000 tools-jsyoo61-2023.5.7.0/tools/torch/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:27:19.671860 tools-jsyoo61-2023.5.7.0/tools_jsyoo61.egg-info/
+-rw-rw-rw-   0        0        0     1342 2023-05-07 06:27:18.000000 tools-jsyoo61-2023.5.7.0/tools_jsyoo61.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      849 2023-05-07 06:27:19.000000 tools-jsyoo61-2023.5.7.0/tools_jsyoo61.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 06:27:18.000000 tools-jsyoo61-2023.5.7.0/tools_jsyoo61.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-07 06:27:18.000000 tools-jsyoo61-2023.5.7.0/tools_jsyoo61.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-07 06:27:18.000000 tools-jsyoo61-2023.5.7.0/tools_jsyoo61.egg-info/top_level.txt
```

### Comparing `tools-jsyoo61-2022.6.27.0/PKG-INFO` & `tools-jsyoo61-2023.5.7.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: tools-jsyoo61
-Version: 2022.6.27.0
+Version: 2023.5.7.0
 Summary: personal syntax tool
 Home-page: https://github.com/jsyoo61/tools
 Author: JaeSung Yoo
 Author-email: jsyoo61@korea.ac.kr
 License: UNKNOWN
-Description: # tools-jsyoo61
-        
-        My personal tools for python programming.\
-        JaeSung Yoo\
-        jsyoo61@korea.ac.kr
-        
-            pip install tools-jsyoo61
-        
-            import tools as T
-            T.save_pickle(data, 'data.p')
-            data = T.load_pickle('data.p')
-        
-        Most useful functions are in `tools.tools`\
-        API dependent tools are in their corresponding folders: `tools.API_name` (i.e. `tools.torch.optim`)
-        Not documented yet, so you'll have to look at documents written inside the codes. (Most codes contain explanation)
-        
-        `scripts/` folder is not included in pip. It's just a copy-paste format
-        
-        I'm open to using my tools for any purpose, and I would appreciate it if the users let me know.
-        Please email me before using it.
-        
-        If you have any questions or suggestions, I am more than happy to discuss them :smile: \
-        Please contact me via email or pull request. (I prefer email though)
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# tools-jsyoo61
+
+My personal tools for python programming.\
+JaeSung Yoo\
+jsyoo61@korea.ac.kr
+
+    pip install tools-jsyoo61
+
+    import tools as T
+    T.save_pickle(data, 'data.p')
+    data = T.load_pickle('data.p')
+
+Most useful functions are in `tools.tools`\
+API dependent tools are in their corresponding folders: `tools.API_name` (i.e. `tools.torch.optim`)
+Not documented yet, so you'll have to look at documents written inside the codes. (Most codes contain explanation)
+
+`scripts/` folder is not included in pip. It's just a copy-paste format
+
+I'm open to using my tools for any purpose, and I would appreciate it if the users let me know.
+Please email me before using it.
+
+If you have any questions or suggestions, I am more than happy to discuss them :smile: \
+Please contact me via email or pull request. (I prefer email though)
+
+
```

### Comparing `tools-jsyoo61-2022.6.27.0/README.md` & `tools-jsyoo61-2023.5.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2022.6.27.0/setup.py` & `tools-jsyoo61-2023.5.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2022.6.27.0/tools/array.py` & `tools-jsyoo61-2023.5.7.0/tools/array.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2022.6.27.0/tools/data.py` & `tools-jsyoo61-2023.5.7.0/tools/data.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2022.6.27.0/tools/exp.py` & `tools-jsyoo61-2023.5.7.0/tools/exp.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2022.6.27.0/tools/modules.py` & `tools-jsyoo61-2023.5.7.0/tools/modules.py`

 * *Files 18% similar despite different names*

```diff
@@ -63,14 +63,21 @@
         y_smooth = tnp.moving_mean(y, w)
         if ax==None:
             ax = plt.gca()
         ax.plot(x, y, color=color, alpha=0.4)
         ax.plot(x, y_smooth, color=color)
         return ax
 
+    def mean(self):
+        return np.mean(self.y)
+    def min(self):
+        return np.min(self.y)
+    def max(self):
+        return np.max(self.y)
+
 class AverageMeter(object):
     """Computes and stores the average and current value
     Variables
     ---------
     self.val
     self.avg
     self.sum
@@ -88,7 +95,23 @@
         self.count = 0
 
     def step(self, val, n=1):
         self.val = val
         self.sum += val * n
         self.count += n
         self.avg = self.sum / self.count
+
+class DictList(object):
+    """Dictionary of lists"""
+    def __init__(self, keys):
+        self._dict = {}
+
+    def append(self, data):
+        assert type(data) in [list, dict]
+        if type(data)==dict:
+            assert set(self._dict.keys())==set(data.keys()), f'allowed keys are: {self._dict.keys()}, received: {data.keys()}'
+            for key, value in data.items():
+                self._dict[key].append(item)
+        else:
+            warnings.warn('Appending with list is not recommended as this cannot ensure the data are being appended to the right place.')
+            for key, value in zip(self._dict.items(), data):
+                self._dict[key].append(value)
```

### Comparing `tools-jsyoo61-2022.6.27.0/tools/numpy/_f.py` & `tools-jsyoo61-2023.5.7.0/tools/numpy/_f.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2022.6.27.0/tools/numpy/_utils.py` & `tools-jsyoo61-2023.5.7.0/tools/numpy/_utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2022.6.27.0/tools/os.py` & `tools-jsyoo61-2023.5.7.0/tools/os.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2022.6.27.0/tools/plot/sklearn.py` & `tools-jsyoo61-2023.5.7.0/tools/plot/sklearn.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2022.6.27.0/tools/plot/utils.py` & `tools-jsyoo61-2023.5.7.0/tools/plot/utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2022.6.27.0/tools/random.py` & `tools-jsyoo61-2023.5.7.0/tools/random.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2022.6.27.0/tools/sklearn/model_selection.py` & `tools-jsyoo61-2023.5.7.0/tools/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2022.6.27.0/tools/stats/__init__.py` & `tools-jsyoo61-2023.5.7.0/tools/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2022.6.27.0/tools/tools.py` & `tools-jsyoo61-2023.5.7.0/tools/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,14 @@
  'now',
  'reverse_dict',
  'unnest_dict',
  'nestdict_to_list',
  'update_ld',
  'update_keys',
  'merge_dict',
- # 'pprint_dict',
  'prettify_dict',
  'read',
  'readline',
  'readlines',
  'save_pickle',
  'str2bool',
  'write']
@@ -471,53 +470,56 @@
     start
 
     stop
 
     reset
         sets self.elapsed_time = 0
     '''
-    def __init__(self, print = False, return_f = True, auto_reset = True):
-        self.print = print
-        self.return_f = return_f
+    def __init__(self, auto_reset = True):
         self.auto_reset = auto_reset
-        self.elapsed_time = 0
+        self._elapsed_time = 0
         self.running = False
 
+    def __repr__(self):
+        options = ''
+        if self.auto_reset: options += '(auto_reset)'
+
+        if len(options)==0:
+            return f'[Timer][running: {self.running}][elapsed_time: {self.elapsed_time()}]'
+        else:
+            return f'[Timer {options}][running: {self.running}][elapsed_time: {self.elapsed_time()}]'
+
     def __enter__(self):
         self.start()
 
     def __exit__(self):
-        t = self.stop()
-        print(t)
+        self.stop()
 
     def start(self):
         if self.auto_reset:
             # self.reset()
-            self.elapsed_time = 0
+            self._elapsed_time = 0
         self.running = True
         self.start_time = time.time()
 
     def stop(self):
         if self.running:
             self.end_time = time.time()
-            self.elapsed_time += self.end_time - self.start_time
+            self._elapsed_time += self.end_time - self.start_time
             self.running = False
-        if self.print:
-            print(self.elapsed_time)
-        if self.return_f:
-            return self.elapsed_time
+        return self._elapsed_time
 
-    def elapsed(self):
+    def elapsed_time(self):
         if self.running:
-            return time.time() - self.start_time
+            return self._elapsed_time + time.time() - self.start_time
         else:
-            warnings.warn('timer is not running. call start() first')
+            return self._elapsed_time
 
     def reset(self):
-        self.elapsed_time = 0
+        self._elapsed_time = 0
 
 class Wrapper:
     def __repr__(self):
         name = '<wrapper>\n'
         args = 'args: '+' '.join(str(self.args))+'\n'
         kwargs = 'kwargs: '+str(self.kwargs)
         return name+args+kwargs
```

### Comparing `tools-jsyoo61-2022.6.27.0/tools/torch/estimator.py` & `tools-jsyoo61-2023.5.7.0/tools/torch/estimator.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2022.6.27.0/tools/torch/federated_learning.py` & `tools-jsyoo61-2023.5.7.0/tools/torch/federated_learning.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2022.6.27.0/tools/torch/model.py` & `tools-jsyoo61-2023.5.7.0/tools/torch/model.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2022.6.27.0/tools/torch/optim/lr_scheduler.py` & `tools-jsyoo61-2023.5.7.0/tools/torch/optim/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2022.6.27.0/tools/torch/utils.py` & `tools-jsyoo61-2023.5.7.0/tools/torch/utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2022.6.27.0/tools_jsyoo61.egg-info/PKG-INFO` & `tools-jsyoo61-2023.5.7.0/tools_jsyoo61.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: tools-jsyoo61
-Version: 2022.6.27.0
+Version: 2023.5.7.0
 Summary: personal syntax tool
 Home-page: https://github.com/jsyoo61/tools
 Author: JaeSung Yoo
 Author-email: jsyoo61@korea.ac.kr
 License: UNKNOWN
-Description: # tools-jsyoo61
-        
-        My personal tools for python programming.\
-        JaeSung Yoo\
-        jsyoo61@korea.ac.kr
-        
-            pip install tools-jsyoo61
-        
-            import tools as T
-            T.save_pickle(data, 'data.p')
-            data = T.load_pickle('data.p')
-        
-        Most useful functions are in `tools.tools`\
-        API dependent tools are in their corresponding folders: `tools.API_name` (i.e. `tools.torch.optim`)
-        Not documented yet, so you'll have to look at documents written inside the codes. (Most codes contain explanation)
-        
-        `scripts/` folder is not included in pip. It's just a copy-paste format
-        
-        I'm open to using my tools for any purpose, and I would appreciate it if the users let me know.
-        Please email me before using it.
-        
-        If you have any questions or suggestions, I am more than happy to discuss them :smile: \
-        Please contact me via email or pull request. (I prefer email though)
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# tools-jsyoo61
+
+My personal tools for python programming.\
+JaeSung Yoo\
+jsyoo61@korea.ac.kr
+
+    pip install tools-jsyoo61
+
+    import tools as T
+    T.save_pickle(data, 'data.p')
+    data = T.load_pickle('data.p')
+
+Most useful functions are in `tools.tools`\
+API dependent tools are in their corresponding folders: `tools.API_name` (i.e. `tools.torch.optim`)
+Not documented yet, so you'll have to look at documents written inside the codes. (Most codes contain explanation)
+
+`scripts/` folder is not included in pip. It's just a copy-paste format
+
+I'm open to using my tools for any purpose, and I would appreciate it if the users let me know.
+Please email me before using it.
+
+If you have any questions or suggestions, I am more than happy to discuss them :smile: \
+Please contact me via email or pull request. (I prefer email though)
+
+
```

### Comparing `tools-jsyoo61-2022.6.27.0/tools_jsyoo61.egg-info/SOURCES.txt` & `tools-jsyoo61-2023.5.7.0/tools_jsyoo61.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 setup.py
 tools/__init__.py
 tools/array.py
 tools/data.py
 tools/exp.py
 tools/modules.py
```

