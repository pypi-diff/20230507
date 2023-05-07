# Comparing `tmp/querytograph-0.0.1.tar.gz` & `tmp/querytograph-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "querytograph-0.0.1.tar", last modified: Sun May  7 16:52:59 2023, max compression
+gzip compressed data, was "querytograph-0.0.2.tar", last modified: Sun May  7 17:04:55 2023, max compression
```

## Comparing `querytograph-0.0.1.tar` & `querytograph-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 simk      (1000) simk      (1000)        0 2023-05-07 16:52:59.211126 querytograph-0.0.1/
--rw-rw-r--   0 simk      (1000) simk      (1000)     1987 2023-05-07 16:52:59.211126 querytograph-0.0.1/PKG-INFO
--rw-rw-r--   0 simk      (1000) simk      (1000)     1734 2023-05-07 16:51:32.000000 querytograph-0.0.1/README.md
-drwxrwxr-x   0 simk      (1000) simk      (1000)        0 2023-05-07 16:52:59.211126 querytograph-0.0.1/querytograph/
--rw-rw-r--   0 simk      (1000) simk      (1000)       50 2023-05-07 08:51:42.000000 querytograph-0.0.1/querytograph/__init__.py
--rw-rw-r--   0 simk      (1000) simk      (1000)     7212 2023-05-07 15:53:56.000000 querytograph-0.0.1/querytograph/querytograph.py
-drwxrwxr-x   0 simk      (1000) simk      (1000)        0 2023-05-07 16:52:59.211126 querytograph-0.0.1/querytograph.egg-info/
--rw-rw-r--   0 simk      (1000) simk      (1000)     1987 2023-05-07 16:52:58.000000 querytograph-0.0.1/querytograph.egg-info/PKG-INFO
--rw-rw-r--   0 simk      (1000) simk      (1000)      251 2023-05-07 16:52:59.000000 querytograph-0.0.1/querytograph.egg-info/SOURCES.txt
--rw-rw-r--   0 simk      (1000) simk      (1000)        1 2023-05-07 16:52:58.000000 querytograph-0.0.1/querytograph.egg-info/dependency_links.txt
--rw-rw-r--   0 simk      (1000) simk      (1000)       71 2023-05-07 16:52:59.000000 querytograph-0.0.1/querytograph.egg-info/requires.txt
--rw-rw-r--   0 simk      (1000) simk      (1000)       13 2023-05-07 16:52:59.000000 querytograph-0.0.1/querytograph.egg-info/top_level.txt
--rw-rw-r--   0 simk      (1000) simk      (1000)       38 2023-05-07 16:52:59.211126 querytograph-0.0.1/setup.cfg
--rw-rw-r--   0 simk      (1000) simk      (1000)      963 2023-05-07 16:27:11.000000 querytograph-0.0.1/setup.py
+drwxrwxr-x   0 simk      (1000) simk      (1000)        0 2023-05-07 17:04:55.155226 querytograph-0.0.2/
+-rw-rw-r--   0 simk      (1000) simk      (1000)     2039 2023-05-07 17:04:55.155226 querytograph-0.0.2/PKG-INFO
+-rw-rw-r--   0 simk      (1000) simk      (1000)     1734 2023-05-07 16:51:32.000000 querytograph-0.0.2/README.md
+drwxrwxr-x   0 simk      (1000) simk      (1000)        0 2023-05-07 17:04:55.151226 querytograph-0.0.2/querytograph/
+-rw-rw-r--   0 simk      (1000) simk      (1000)       50 2023-05-07 08:51:42.000000 querytograph-0.0.2/querytograph/__init__.py
+-rw-rw-r--   0 simk      (1000) simk      (1000)     7212 2023-05-07 15:53:56.000000 querytograph-0.0.2/querytograph/querytograph.py
+drwxrwxr-x   0 simk      (1000) simk      (1000)        0 2023-05-07 17:04:55.155226 querytograph-0.0.2/querytograph.egg-info/
+-rw-rw-r--   0 simk      (1000) simk      (1000)     2039 2023-05-07 17:04:54.000000 querytograph-0.0.2/querytograph.egg-info/PKG-INFO
+-rw-rw-r--   0 simk      (1000) simk      (1000)      251 2023-05-07 17:04:55.000000 querytograph-0.0.2/querytograph.egg-info/SOURCES.txt
+-rw-rw-r--   0 simk      (1000) simk      (1000)        1 2023-05-07 17:04:54.000000 querytograph-0.0.2/querytograph.egg-info/dependency_links.txt
+-rw-rw-r--   0 simk      (1000) simk      (1000)       71 2023-05-07 17:04:54.000000 querytograph-0.0.2/querytograph.egg-info/requires.txt
+-rw-rw-r--   0 simk      (1000) simk      (1000)       13 2023-05-07 17:04:55.000000 querytograph-0.0.2/querytograph.egg-info/top_level.txt
+-rw-rw-r--   0 simk      (1000) simk      (1000)       38 2023-05-07 17:04:55.155226 querytograph-0.0.2/setup.cfg
+-rw-rw-r--   0 simk      (1000) simk      (1000)     1015 2023-05-07 17:04:13.000000 querytograph-0.0.2/setup.py
```

### Comparing `querytograph-0.0.1/PKG-INFO` & `querytograph-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: querytograph
-Version: 0.0.1
+Version: 0.0.2
 Summary: Using ChatGPT to convert your plain English queries into graphs
+Home-page: https://github.com/franziss/querytograph
 Author: franziss
 Author-email: franziss@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # QueryToGraph
```

### Comparing `querytograph-0.0.1/README.md` & `querytograph-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `querytograph-0.0.1/querytograph/querytograph.py` & `querytograph-0.0.2/querytograph/querytograph.py`

 * *Files identical despite different names*

### Comparing `querytograph-0.0.1/querytograph.egg-info/PKG-INFO` & `querytograph-0.0.2/querytograph.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: querytograph
-Version: 0.0.1
+Version: 0.0.2
 Summary: Using ChatGPT to convert your plain English queries into graphs
+Home-page: https://github.com/franziss/querytograph
 Author: franziss
 Author-email: franziss@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # QueryToGraph
```

### Comparing `querytograph-0.0.1/setup.py` & `querytograph-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='querytograph',
     packages=find_packages(include=['querytograph']),
-    version='0.0.1',
+    version='0.0.2',
     description='Using ChatGPT to convert your plain English queries into graphs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='franziss',
     author_email='franziss@gmail.com',
     license='MIT',
+    url="https://github.com/franziss/querytograph",
     install_requires=[
         'pandas',
         'openai',
         'langchain==0.0.160',
         'rapidfuzz==3.0.0',
         'gradio==3.26.0',
         'numpy'
```

