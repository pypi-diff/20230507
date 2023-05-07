# Comparing `tmp/maya-rig-operation-graph-0.6.1.tar.gz` & `tmp/maya-rig-operation-graph-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\maya-rig-operation-graph-0.6.1.tar", last modified: Sun May  7 12:14:19 2023, max compression
+gzip compressed data, was "dist\maya-rig-operation-graph-0.6.2.tar", last modified: Sun May  7 12:21:50 2023, max compression
```

## Comparing `maya-rig-operation-graph-0.6.1.tar` & `maya-rig-operation-graph-0.6.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 12:14:19.000000 maya-rig-operation-graph-0.6.1/
--rw-rw-rw-   0        0        0    11558 2022-10-23 14:57:04.000000 maya-rig-operation-graph-0.6.1/LICENSE
--rw-rw-rw-   0        0        0     3819 2023-05-07 12:14:20.000000 maya-rig-operation-graph-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     2622 2023-05-07 12:14:18.000000 maya-rig-operation-graph-0.6.1/README.rst
--rw-rw-rw-   0        0        0      112 2023-05-07 12:14:20.000000 maya-rig-operation-graph-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1907 2023-05-07 12:13:32.000000 maya-rig-operation-graph-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 12:14:19.000000 maya-rig-operation-graph-0.6.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-07 12:14:19.000000 maya-rig-operation-graph-0.6.1/src/maya_rig_operation_graph.egg-info/
--rw-rw-rw-   0        0        0     3819 2023-05-07 12:14:20.000000 maya-rig-operation-graph-0.6.1/src/maya_rig_operation_graph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      910 2023-05-07 12:14:20.000000 maya-rig-operation-graph-0.6.1/src/maya_rig_operation_graph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 12:14:20.000000 maya-rig-operation-graph-0.6.1/src/maya_rig_operation_graph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-07 12:14:20.000000 maya-rig-operation-graph-0.6.1/src/maya_rig_operation_graph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-07 12:14:20.000000 maya-rig-operation-graph-0.6.1/src/maya_rig_operation_graph.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-07 12:14:19.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/
--rw-rw-rw-   0        0        0      297 2022-05-11 13:52:18.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/__init__.py
--rw-rw-rw-   0        0        0     3219 2023-05-06 17:11:50.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/_utils.py
--rw-rw-rw-   0        0        0     1423 2022-10-06 03:06:38.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/additional.py
--rw-rw-rw-   0        0        0     1250 2023-05-02 01:39:06.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/all.py
--rw-rw-rw-   0        0        0     1271 2022-10-06 03:11:24.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/blend.py
--rw-rw-rw-   0        0        0     1243 2022-10-06 03:26:24.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/clamp.py
--rw-rw-rw-   0        0        0      858 2022-08-04 14:52:14.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/distance.py
--rw-rw-rw-   0        0        0      800 2022-06-12 18:38:00.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/drive.py
--rw-rw-rw-   0        0        0     2267 2022-09-27 19:50:48.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/logic.py
--rw-rw-rw-   0        0        0     4858 2022-09-27 19:50:48.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/math.py
--rw-rw-rw-   0        0        0     1180 2022-08-04 17:29:44.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/math.pyi
--rw-rw-rw-   0        0        0     5757 2023-05-06 17:21:16.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/math3d.py
--rw-rw-rw-   0        0        0     1737 2023-05-02 11:47:16.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/math3d.pyi
--rw-rw-rw-   0        0        0     4714 2023-05-02 03:35:42.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/matrix.py
--rw-rw-rw-   0        0        0     3817 2023-05-06 16:50:06.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/quaternion.py
--rw-rw-rw-   0        0        0     2034 2022-08-23 07:56:04.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/random.py
--rw-rw-rw-   0        0        0      591 2022-06-12 18:38:00.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/reverse.py
--rw-rw-rw-   0        0        0      566 2022-08-22 02:24:00.000000 maya-rig-operation-graph-0.6.1/src/rig_operation_graph/time.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:21:50.000000 maya-rig-operation-graph-0.6.2/
+-rw-rw-rw-   0        0        0    11558 2022-10-23 14:57:04.000000 maya-rig-operation-graph-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0     3819 2023-05-07 12:21:52.000000 maya-rig-operation-graph-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2622 2023-05-07 12:21:50.000000 maya-rig-operation-graph-0.6.2/README.rst
+-rw-rw-rw-   0        0        0      112 2023-05-07 12:21:52.000000 maya-rig-operation-graph-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1914 2023-05-07 12:21:24.000000 maya-rig-operation-graph-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:21:50.000000 maya-rig-operation-graph-0.6.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 12:21:50.000000 maya-rig-operation-graph-0.6.2/src/maya_rig_operation_graph.egg-info/
+-rw-rw-rw-   0        0        0     3819 2023-05-07 12:21:50.000000 maya-rig-operation-graph-0.6.2/src/maya_rig_operation_graph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      910 2023-05-07 12:21:50.000000 maya-rig-operation-graph-0.6.2/src/maya_rig_operation_graph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 12:21:50.000000 maya-rig-operation-graph-0.6.2/src/maya_rig_operation_graph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-07 12:21:50.000000 maya-rig-operation-graph-0.6.2/src/maya_rig_operation_graph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-07 12:21:50.000000 maya-rig-operation-graph-0.6.2/src/maya_rig_operation_graph.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 12:21:50.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/
+-rw-rw-rw-   0        0        0      297 2022-05-11 13:52:18.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/__init__.py
+-rw-rw-rw-   0        0        0     3219 2023-05-06 17:11:50.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/_utils.py
+-rw-rw-rw-   0        0        0     1423 2022-10-06 03:06:38.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/additional.py
+-rw-rw-rw-   0        0        0     1250 2023-05-02 01:39:06.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/all.py
+-rw-rw-rw-   0        0        0     1271 2022-10-06 03:11:24.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/blend.py
+-rw-rw-rw-   0        0        0     1243 2022-10-06 03:26:24.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/clamp.py
+-rw-rw-rw-   0        0        0      858 2022-08-04 14:52:14.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/distance.py
+-rw-rw-rw-   0        0        0      800 2022-06-12 18:38:00.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/drive.py
+-rw-rw-rw-   0        0        0     2267 2022-09-27 19:50:48.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/logic.py
+-rw-rw-rw-   0        0        0     4858 2022-09-27 19:50:48.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/math.py
+-rw-rw-rw-   0        0        0     1180 2022-08-04 17:29:44.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/math.pyi
+-rw-rw-rw-   0        0        0     5757 2023-05-06 17:21:16.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/math3d.py
+-rw-rw-rw-   0        0        0     1737 2023-05-02 11:47:16.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/math3d.pyi
+-rw-rw-rw-   0        0        0     4714 2023-05-02 03:35:42.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/matrix.py
+-rw-rw-rw-   0        0        0     3817 2023-05-06 16:50:06.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/quaternion.py
+-rw-rw-rw-   0        0        0     2034 2022-08-23 07:56:04.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/random.py
+-rw-rw-rw-   0        0        0      591 2022-06-12 18:38:00.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/reverse.py
+-rw-rw-rw-   0        0        0      566 2022-08-22 02:24:00.000000 maya-rig-operation-graph-0.6.2/src/rig_operation_graph/time.py
```

### Comparing `maya-rig-operation-graph-0.6.1/LICENSE` & `maya-rig-operation-graph-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/PKG-INFO` & `maya-rig-operation-graph-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maya-rig-operation-graph
-Version: 0.6.1
+Version: 0.6.2
 Summary: maya计算图的实现
 Home-page: https://github.com/cpcgskill/maya-rig-operation-graph
 Author: ('cpcgskill',)
 Author-email: cpcgskill@outlook.com
 License: Apache Software License (Apache 2.0)
 Project-URL: Bug Tracker, https://github.com/cpcgskill/maya-rig-operation-graph/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `maya-rig-operation-graph-0.6.1/README.rst` & `maya-rig-operation-graph-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/setup.py` & `maya-rig-operation-graph-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 import setuptools
 
 lib_name = 'maya-rig-operation-graph'
 
 author = 'cpcgskill',
 author_email = 'cpcgskill@outlook.com'
 
-version = '0.6.1'
+version = '0.6.2'
 
 description = 'maya计算图的实现'
 with open("README.rst", "rb") as f:
     long_description = f.read().decode(encoding='utf-8')
 
 project_homepage = 'https://github.com/cpcgskill/maya-rig-operation-graph'
 project_urls = {
     'Bug Tracker': 'https://github.com/cpcgskill/maya-rig-operation-graph/issues',
 }
 license = 'Apache Software License (Apache 2.0)'
 
 packages = ['rig_operation_graph']
 python_requires = '>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*'
 install_requires = [
-    'maya-rig-core',
+    'maya-rig-core>=0.2.4',
 ]
 
 setuptools.setup(
     name=lib_name,
     version=version,
     author=author,
     author_email=author_email,
```

### Comparing `maya-rig-operation-graph-0.6.1/src/maya_rig_operation_graph.egg-info/PKG-INFO` & `maya-rig-operation-graph-0.6.2/src/maya_rig_operation_graph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maya-rig-operation-graph
-Version: 0.6.1
+Version: 0.6.2
 Summary: maya计算图的实现
 Home-page: https://github.com/cpcgskill/maya-rig-operation-graph
 Author: ('cpcgskill',)
 Author-email: cpcgskill@outlook.com
 License: Apache Software License (Apache 2.0)
 Project-URL: Bug Tracker, https://github.com/cpcgskill/maya-rig-operation-graph/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `maya-rig-operation-graph-0.6.1/src/maya_rig_operation_graph.egg-info/SOURCES.txt` & `maya-rig-operation-graph-0.6.2/src/maya_rig_operation_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/src/rig_operation_graph/_utils.py` & `maya-rig-operation-graph-0.6.2/src/rig_operation_graph/_utils.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/src/rig_operation_graph/additional.py` & `maya-rig-operation-graph-0.6.2/src/rig_operation_graph/additional.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/src/rig_operation_graph/all.py` & `maya-rig-operation-graph-0.6.2/src/rig_operation_graph/all.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/src/rig_operation_graph/blend.py` & `maya-rig-operation-graph-0.6.2/src/rig_operation_graph/blend.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/src/rig_operation_graph/clamp.py` & `maya-rig-operation-graph-0.6.2/src/rig_operation_graph/clamp.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/src/rig_operation_graph/distance.py` & `maya-rig-operation-graph-0.6.2/src/rig_operation_graph/distance.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/src/rig_operation_graph/drive.py` & `maya-rig-operation-graph-0.6.2/src/rig_operation_graph/drive.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/src/rig_operation_graph/logic.py` & `maya-rig-operation-graph-0.6.2/src/rig_operation_graph/logic.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/src/rig_operation_graph/math.py` & `maya-rig-operation-graph-0.6.2/src/rig_operation_graph/math.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/src/rig_operation_graph/math.pyi` & `maya-rig-operation-graph-0.6.2/src/rig_operation_graph/math.pyi`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/src/rig_operation_graph/math3d.py` & `maya-rig-operation-graph-0.6.2/src/rig_operation_graph/math3d.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/src/rig_operation_graph/math3d.pyi` & `maya-rig-operation-graph-0.6.2/src/rig_operation_graph/math3d.pyi`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/src/rig_operation_graph/matrix.py` & `maya-rig-operation-graph-0.6.2/src/rig_operation_graph/matrix.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/src/rig_operation_graph/quaternion.py` & `maya-rig-operation-graph-0.6.2/src/rig_operation_graph/quaternion.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/src/rig_operation_graph/random.py` & `maya-rig-operation-graph-0.6.2/src/rig_operation_graph/random.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/src/rig_operation_graph/reverse.py` & `maya-rig-operation-graph-0.6.2/src/rig_operation_graph/reverse.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.6.1/src/rig_operation_graph/time.py` & `maya-rig-operation-graph-0.6.2/src/rig_operation_graph/time.py`

 * *Files identical despite different names*

