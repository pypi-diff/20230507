# Comparing `tmp/cuboxGPT-0.1.0.tar.gz` & `tmp/cuboxgpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuboxGPT-0.1.0.tar", last modified: Sun May  7 17:24:00 2023, max compression
+gzip compressed data, was "cuboxgpt-0.1.1.tar", last modified: Sun May  7 17:22:46 2023, max compression
```

## Comparing `cuboxGPT-0.1.0.tar` & `cuboxgpt-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 glaze      (501) staff       (20)        0 2023-05-07 17:24:00.621572 cuboxGPT-0.1.0/
--rw-r--r--   0 glaze      (501) staff       (20)     2574 2023-05-07 17:24:00.621405 cuboxGPT-0.1.0/PKG-INFO
--rw-r--r--   0 glaze      (501) staff       (20)     1865 2023-05-07 16:56:41.000000 cuboxGPT-0.1.0/README.md
--rw-r--r--   0 glaze      (501) staff       (20)     2977 2023-05-07 16:56:07.000000 cuboxGPT-0.1.0/chatFromDB.py
-drwxr-xr-x   0 glaze      (501) staff       (20)        0 2023-05-07 17:24:00.620905 cuboxGPT-0.1.0/cuboxGPT.egg-info/
--rw-r--r--   0 glaze      (501) staff       (20)     2574 2023-05-07 17:24:00.000000 cuboxGPT-0.1.0/cuboxGPT.egg-info/PKG-INFO
--rw-r--r--   0 glaze      (501) staff       (20)      466 2023-05-07 17:24:00.000000 cuboxGPT-0.1.0/cuboxGPT.egg-info/SOURCES.txt
--rw-r--r--   0 glaze      (501) staff       (20)        1 2023-05-07 17:24:00.000000 cuboxGPT-0.1.0/cuboxGPT.egg-info/dependency_links.txt
--rw-r--r--   0 glaze      (501) staff       (20)       42 2023-05-07 17:24:00.000000 cuboxGPT-0.1.0/cuboxGPT.egg-info/entry_points.txt
--rw-r--r--   0 glaze      (501) staff       (20)       59 2023-05-07 17:24:00.000000 cuboxGPT-0.1.0/cuboxGPT.egg-info/requires.txt
--rw-r--r--   0 glaze      (501) staff       (20)       33 2023-05-07 17:24:00.000000 cuboxGPT-0.1.0/cuboxGPT.egg-info/top_level.txt
--rw-r--r--   0 glaze      (501) staff       (20)      576 2023-05-07 16:25:32.000000 cuboxGPT-0.1.0/cuboxGPT.py
--rw-r--r--   0 glaze      (501) staff       (20)     1566 2023-05-07 16:04:33.000000 cuboxGPT-0.1.0/db.py
--rw-r--r--   0 glaze      (501) staff       (20)      316 2023-05-07 17:01:22.000000 cuboxGPT-0.1.0/pyproject.toml
--rw-r--r--   0 glaze      (501) staff       (20)       38 2023-05-07 17:24:00.621613 cuboxGPT-0.1.0/setup.cfg
--rw-r--r--   0 glaze      (501) staff       (20)     1346 2023-05-07 17:23:04.000000 cuboxGPT-0.1.0/setup.py
--rw-r--r--   0 glaze      (501) staff       (20)     3531 2023-05-07 04:15:58.000000 cuboxGPT-0.1.0/webParser.py
+drwxr-xr-x   0 glaze      (501) staff       (20)        0 2023-05-07 17:22:46.338823 cuboxgpt-0.1.1/
+-rw-r--r--   0 glaze      (501) staff       (20)     2574 2023-05-07 17:22:46.338685 cuboxgpt-0.1.1/PKG-INFO
+-rw-r--r--   0 glaze      (501) staff       (20)     1865 2023-05-07 16:56:41.000000 cuboxgpt-0.1.1/README.md
+-rw-r--r--   0 glaze      (501) staff       (20)     2977 2023-05-07 16:56:07.000000 cuboxgpt-0.1.1/chatFromDB.py
+drwxr-xr-x   0 glaze      (501) staff       (20)        0 2023-05-07 17:22:46.338167 cuboxgpt-0.1.1/cuboxGPT.egg-info/
+-rw-r--r--   0 glaze      (501) staff       (20)     2574 2023-05-07 17:22:46.000000 cuboxgpt-0.1.1/cuboxGPT.egg-info/PKG-INFO
+-rw-r--r--   0 glaze      (501) staff       (20)      466 2023-05-07 17:22:46.000000 cuboxgpt-0.1.1/cuboxGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 glaze      (501) staff       (20)        1 2023-05-07 17:22:46.000000 cuboxgpt-0.1.1/cuboxGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 glaze      (501) staff       (20)       42 2023-05-07 17:22:46.000000 cuboxgpt-0.1.1/cuboxGPT.egg-info/entry_points.txt
+-rw-r--r--   0 glaze      (501) staff       (20)       59 2023-05-07 17:22:46.000000 cuboxgpt-0.1.1/cuboxGPT.egg-info/requires.txt
+-rw-r--r--   0 glaze      (501) staff       (20)       33 2023-05-07 17:22:46.000000 cuboxgpt-0.1.1/cuboxGPT.egg-info/top_level.txt
+-rw-r--r--   0 glaze      (501) staff       (20)      576 2023-05-07 16:25:32.000000 cuboxgpt-0.1.1/cuboxGPT.py
+-rw-r--r--   0 glaze      (501) staff       (20)     1566 2023-05-07 16:04:33.000000 cuboxgpt-0.1.1/db.py
+-rw-r--r--   0 glaze      (501) staff       (20)      316 2023-05-07 17:01:22.000000 cuboxgpt-0.1.1/pyproject.toml
+-rw-r--r--   0 glaze      (501) staff       (20)       38 2023-05-07 17:22:46.338859 cuboxgpt-0.1.1/setup.cfg
+-rw-r--r--   0 glaze      (501) staff       (20)     1346 2023-05-07 17:22:42.000000 cuboxgpt-0.1.1/setup.py
+-rw-r--r--   0 glaze      (501) staff       (20)     3531 2023-05-07 04:15:58.000000 cuboxgpt-0.1.1/webParser.py
```

### Comparing `cuboxGPT-0.1.0/PKG-INFO` & `cuboxgpt-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cuboxGPT
-Version: 0.1.0
+Name: cuboxgpt
+Version: 0.1.1
 Summary: Use GPT to chat/search your large Cubox datasets
 Home-page: https://github.com/glazec/cuboxGPT
 Author: Glaze
 License: MIT
 Keywords: Cubox,search,AI,GPT,langchain
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cuboxGPT-0.1.0/README.md` & `cuboxgpt-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cuboxGPT-0.1.0/chatFromDB.py` & `cuboxgpt-0.1.1/chatFromDB.py`

 * *Files identical despite different names*

### Comparing `cuboxGPT-0.1.0/cuboxGPT.egg-info/PKG-INFO` & `cuboxgpt-0.1.1/cuboxGPT.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cuboxGPT
-Version: 0.1.0
+Name: cuboxgpt
+Version: 0.1.1
 Summary: Use GPT to chat/search your large Cubox datasets
 Home-page: https://github.com/glazec/cuboxGPT
 Author: Glaze
 License: MIT
 Keywords: Cubox,search,AI,GPT,langchain
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cuboxGPT-0.1.0/cuboxGPT.py` & `cuboxgpt-0.1.1/cuboxGPT.py`

 * *Files identical despite different names*

### Comparing `cuboxGPT-0.1.0/db.py` & `cuboxgpt-0.1.1/db.py`

 * *Files identical despite different names*

### Comparing `cuboxGPT-0.1.0/setup.py` & `cuboxgpt-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 import os
 # Read the contents of the README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
-    name='cuboxGPT',
-    version='0.1.0',
+    name='cuboxgpt',
+    version='0.1.1',
     author='Glaze',
     description='Use GPT to chat/search your large Cubox datasets',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     readme='README.md',
     keywords=['Cubox', 'search', 'AI', 'GPT', 'langchain'],
```

### Comparing `cuboxGPT-0.1.0/webParser.py` & `cuboxgpt-0.1.1/webParser.py`

 * *Files identical despite different names*

