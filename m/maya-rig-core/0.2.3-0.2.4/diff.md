# Comparing `tmp/maya_rig_core-0.2.3.tar.gz` & `tmp/maya_rig_core-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\maya_rig_core-0.2.3.tar", last modified: Sun May  7 12:09:29 2023, max compression
+gzip compressed data, was "dist\maya_rig_core-0.2.4.tar", last modified: Sun May  7 12:20:33 2023, max compression
```

## Comparing `maya_rig_core-0.2.3.tar` & `maya_rig_core-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 12:09:28.000000 maya_rig_core-0.2.3/
--rw-rw-rw-   0        0        0    11558 2022-09-27 19:48:00.000000 maya_rig_core-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     6010 2023-05-07 12:09:30.000000 maya_rig_core-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     4754 2022-09-28 16:54:34.000000 maya_rig_core-0.2.3/README.md
--rw-rw-rw-   0        0        0     5257 2023-05-07 12:09:28.000000 maya_rig_core-0.2.3/README.rst
--rw-rw-rw-   0        0        0      112 2023-05-07 12:09:30.000000 maya_rig_core-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1907 2023-05-07 11:56:56.000000 maya_rig_core-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 12:09:28.000000 maya_rig_core-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-07 12:09:28.000000 maya_rig_core-0.2.3/src/maya_rig_core.egg-info/
--rw-rw-rw-   0        0        0     6010 2023-05-07 12:09:30.000000 maya_rig_core-0.2.3/src/maya_rig_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2023-05-07 12:09:30.000000 maya_rig_core-0.2.3/src/maya_rig_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 12:09:30.000000 maya_rig_core-0.2.3/src/maya_rig_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-07 12:09:30.000000 maya_rig_core-0.2.3/src/maya_rig_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-07 12:09:30.000000 maya_rig_core-0.2.3/src/maya_rig_core.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-07 12:09:28.000000 maya_rig_core-0.2.3/src/rig_core/
--rw-rw-rw-   0        0        0      294 2022-03-21 21:57:28.000000 maya_rig_core-0.2.3/src/rig_core/__init__.py
--rw-rw-rw-   0        0        0      538 2022-06-25 21:30:36.000000 maya_rig_core-0.2.3/src/rig_core/all.py
--rw-rw-rw-   0        0        0     3613 2022-10-02 15:28:22.000000 maya_rig_core-0.2.3/src/rig_core/contextmanager.py
--rw-rw-rw-   0        0        0    13599 2022-11-27 14:56:44.000000 maya_rig_core-0.2.3/src/rig_core/ctx.py
--rw-rw-rw-   0        0        0     5911 2022-08-24 00:21:54.000000 maya_rig_core-0.2.3/src/rig_core/db.py
--rw-rw-rw-   0        0        0     1465 2022-10-02 15:27:38.000000 maya_rig_core-0.2.3/src/rig_core/filter.py
--rw-rw-rw-   0        0        0     4848 2022-10-02 16:28:52.000000 maya_rig_core-0.2.3/src/rig_core/joint_tree.py
--rw-rw-rw-   0        0        0     1098 2022-10-02 15:27:38.000000 maya_rig_core-0.2.3/src/rig_core/response.py
--rw-rw-rw-   0        0        0     1811 2022-11-27 14:56:44.000000 maya_rig_core-0.2.3/src/rig_core/tag.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:20:29.000000 maya_rig_core-0.2.4/
+-rw-rw-rw-   0        0        0    11558 2022-09-27 19:48:00.000000 maya_rig_core-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     6010 2023-05-07 12:20:34.000000 maya_rig_core-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4754 2022-09-28 16:54:34.000000 maya_rig_core-0.2.4/README.md
+-rw-rw-rw-   0        0        0     5257 2023-05-07 12:20:34.000000 maya_rig_core-0.2.4/README.rst
+-rw-rw-rw-   0        0        0      112 2023-05-07 12:20:34.000000 maya_rig_core-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1907 2023-05-07 12:19:38.000000 maya_rig_core-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:20:29.000000 maya_rig_core-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 12:20:33.000000 maya_rig_core-0.2.4/src/maya_rig_core.egg-info/
+-rw-rw-rw-   0        0        0     6010 2023-05-07 12:20:34.000000 maya_rig_core-0.2.4/src/maya_rig_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2023-05-07 12:20:34.000000 maya_rig_core-0.2.4/src/maya_rig_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 12:20:34.000000 maya_rig_core-0.2.4/src/maya_rig_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-07 12:20:34.000000 maya_rig_core-0.2.4/src/maya_rig_core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-07 12:20:34.000000 maya_rig_core-0.2.4/src/maya_rig_core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 12:20:33.000000 maya_rig_core-0.2.4/src/rig_core/
+-rw-rw-rw-   0        0        0      294 2022-03-21 21:57:28.000000 maya_rig_core-0.2.4/src/rig_core/__init__.py
+-rw-rw-rw-   0        0        0      538 2022-06-25 21:30:36.000000 maya_rig_core-0.2.4/src/rig_core/all.py
+-rw-rw-rw-   0        0        0     3613 2022-10-02 15:28:22.000000 maya_rig_core-0.2.4/src/rig_core/contextmanager.py
+-rw-rw-rw-   0        0        0    13599 2022-11-27 14:56:44.000000 maya_rig_core-0.2.4/src/rig_core/ctx.py
+-rw-rw-rw-   0        0        0     5911 2022-08-24 00:21:54.000000 maya_rig_core-0.2.4/src/rig_core/db.py
+-rw-rw-rw-   0        0        0     1465 2022-10-02 15:27:38.000000 maya_rig_core-0.2.4/src/rig_core/filter.py
+-rw-rw-rw-   0        0        0     4848 2022-10-02 16:28:52.000000 maya_rig_core-0.2.4/src/rig_core/joint_tree.py
+-rw-rw-rw-   0        0        0     1098 2022-10-02 15:27:38.000000 maya_rig_core-0.2.4/src/rig_core/response.py
+-rw-rw-rw-   0        0        0     1811 2022-11-27 14:56:44.000000 maya_rig_core-0.2.4/src/rig_core/tag.py
```

### Comparing `maya_rig_core-0.2.3/LICENSE` & `maya_rig_core-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `maya_rig_core-0.2.3/PKG-INFO` & `maya_rig_core-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maya_rig_core
-Version: 0.2.3
+Version: 0.2.4
 Summary: 一个好用的绑定核心库
 Home-page: https://github.com/cpcgskill/maya_rig_core
 Author: ('cpcgskill',)
 Author-email: cpcgskill@outlook.com
 License: Apache Software License (Apache 2.0)
 Project-URL: Bug Tracker, https://github.com/cpcgskill/maya_rig_core/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `maya_rig_core-0.2.3/README.md` & `maya_rig_core-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `maya_rig_core-0.2.3/README.rst` & `maya_rig_core-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `maya_rig_core-0.2.3/setup.py` & `maya_rig_core-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 import setuptools
 
 lib_name = 'maya_rig_core'
 
 author = 'cpcgskill',
 author_email = 'cpcgskill@outlook.com'
 
-version = '0.2.3'
+version = '0.2.4'
 
 description = '一个好用的绑定核心库'
 with open("README.md", "rb") as f:
     long_description = f.read().decode(encoding='utf-8')
 
 project_homepage = 'https://github.com/cpcgskill/maya_rig_core'
 project_urls = {
     'Bug Tracker': 'https://github.com/cpcgskill/maya_rig_core/issues',
 }
 license = 'Apache Software License (Apache 2.0)'
 
 python_requires = '>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*'
 install_requires = [
-    'maya-test-tools==0.1.0',
-    'cpmel==3',
+    'maya-test-tools>=0.1.0',
+    'cpmel>=3',
 ]
 
 setuptools.setup(
     name=lib_name,
     version=version,
     author=author,
     author_email=author_email,
```

### Comparing `maya_rig_core-0.2.3/src/maya_rig_core.egg-info/PKG-INFO` & `maya_rig_core-0.2.4/src/maya_rig_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maya-rig-core
-Version: 0.2.3
+Version: 0.2.4
 Summary: 一个好用的绑定核心库
 Home-page: https://github.com/cpcgskill/maya_rig_core
 Author: ('cpcgskill',)
 Author-email: cpcgskill@outlook.com
 License: Apache Software License (Apache 2.0)
 Project-URL: Bug Tracker, https://github.com/cpcgskill/maya_rig_core/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `maya_rig_core-0.2.3/src/rig_core/all.py` & `maya_rig_core-0.2.4/src/rig_core/all.py`

 * *Files identical despite different names*

### Comparing `maya_rig_core-0.2.3/src/rig_core/contextmanager.py` & `maya_rig_core-0.2.4/src/rig_core/contextmanager.py`

 * *Files identical despite different names*

### Comparing `maya_rig_core-0.2.3/src/rig_core/ctx.py` & `maya_rig_core-0.2.4/src/rig_core/ctx.py`

 * *Files identical despite different names*

### Comparing `maya_rig_core-0.2.3/src/rig_core/db.py` & `maya_rig_core-0.2.4/src/rig_core/db.py`

 * *Files identical despite different names*

### Comparing `maya_rig_core-0.2.3/src/rig_core/filter.py` & `maya_rig_core-0.2.4/src/rig_core/filter.py`

 * *Files identical despite different names*

### Comparing `maya_rig_core-0.2.3/src/rig_core/joint_tree.py` & `maya_rig_core-0.2.4/src/rig_core/joint_tree.py`

 * *Files identical despite different names*

### Comparing `maya_rig_core-0.2.3/src/rig_core/response.py` & `maya_rig_core-0.2.4/src/rig_core/response.py`

 * *Files identical despite different names*

### Comparing `maya_rig_core-0.2.3/src/rig_core/tag.py` & `maya_rig_core-0.2.4/src/rig_core/tag.py`

 * *Files identical despite different names*

