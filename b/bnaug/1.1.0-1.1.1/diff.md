# Comparing `tmp/bnaug-1.1.0.tar.gz` & `tmp/bnaug-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnaug-1.1.0.tar", last modified: Tue Nov 22 06:04:23 2022, max compression
+gzip compressed data, was "bnaug-1.1.1.tar", last modified: Sun May  7 04:04:03 2023, max compression
```

## Comparing `bnaug-1.1.0.tar` & `bnaug-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 06:04:23.638520 bnaug-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     3997 2022-11-22 06:04:23.638520 bnaug-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3560 2022-11-22 06:04:12.000000 bnaug-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 06:04:23.634520 bnaug-1.1.0/bnaug/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-22 06:04:12.000000 bnaug-1.1.0/bnaug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-11-22 06:04:12.000000 bnaug-1.1.0/bnaug/randaug.py
--rw-r--r--   0 runner    (1001) docker     (121)     6559 2022-11-22 06:04:12.000000 bnaug-1.1.0/bnaug/sentence.py
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-11-22 06:04:12.000000 bnaug-1.1.0/bnaug/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-22 06:04:23.634520 bnaug-1.1.0/bnaug.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3997 2022-11-22 06:04:23.000000 bnaug-1.1.0/bnaug.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-11-22 06:04:23.000000 bnaug-1.1.0/bnaug.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-22 06:04:23.000000 bnaug-1.1.0/bnaug.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-22 06:04:23.000000 bnaug-1.1.0/bnaug.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-22 06:04:23.000000 bnaug-1.1.0/bnaug.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-22 06:04:23.638520 bnaug-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-11-22 06:04:12.000000 bnaug-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:04:03.949963 bnaug-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-07 04:04:03.949963 bnaug-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-05-07 04:03:50.000000 bnaug-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:04:03.945963 bnaug-1.1.1/bnaug/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 04:03:50.000000 bnaug-1.1.1/bnaug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-07 04:03:50.000000 bnaug-1.1.1/bnaug/randaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-05-07 04:03:50.000000 bnaug-1.1.1/bnaug/sentence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-07 04:03:50.000000 bnaug-1.1.1/bnaug/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:04:03.945963 bnaug-1.1.1/bnaug.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-07 04:04:03.000000 bnaug-1.1.1/bnaug.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-07 04:04:03.000000 bnaug-1.1.1/bnaug.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 04:04:03.000000 bnaug-1.1.1/bnaug.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-07 04:04:03.000000 bnaug-1.1.1/bnaug.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 04:04:03.000000 bnaug-1.1.1/bnaug.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 04:04:03.949963 bnaug-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-07 04:03:50.000000 bnaug-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:04:03.949963 bnaug-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-05-07 04:03:50.000000 bnaug-1.1.1/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-07 04:03:50.000000 bnaug-1.1.1/tests/test_randaug.py
```

### Comparing `bnaug-1.1.0/PKG-INFO` & `bnaug-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnaug
-Version: 1.1.0
+Version: 1.1.1
 Summary: bnaug is a text augmentation tool for Bangla text.
 Home-page: https://github.com/sagorbrur/bnaug
 Author: Sagor Sarker
 Author-email: sagorhem3532@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,17 @@
 
 ## Installation
 ```
 pip install bnaug
 ```
 - Dependencies
     - pytorch >=1.7.0
+    
+## Demo Notebook
+- [bnaug demo](https://github.com/sagorbrur/bnaug/blob/main/notebook/bnaug_demo.ipynb)
 
 ## Necessary Model Links
 - [word2vec](https://huggingface.co/sagorsarker/bangla_word2vec/resolve/main/bangla_word2vec_gen4.zip)
 - [glove vector](https://huggingface.co/sagorsarker/bangla-glove-vectors/resolve/main/bn_glove.300d.zip)
 
 ## Sentence Augmentation
 ### Token Replacement
```

### Comparing `bnaug-1.1.0/README.md` & `bnaug-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 
 ## Installation
 ```
 pip install bnaug
 ```
 - Dependencies
     - pytorch >=1.7.0
+    
+## Demo Notebook
+- [bnaug demo](https://github.com/sagorbrur/bnaug/blob/main/notebook/bnaug_demo.ipynb)
 
 ## Necessary Model Links
 - [word2vec](https://huggingface.co/sagorsarker/bangla_word2vec/resolve/main/bangla_word2vec_gen4.zip)
 - [glove vector](https://huggingface.co/sagorsarker/bangla-glove-vectors/resolve/main/bn_glove.300d.zip)
 
 ## Sentence Augmentation
 ### Token Replacement
@@ -112,8 +115,8 @@
     text = "আমি ১০০ বাকি দিলাম"
     randaug.remove_random_char(text)
     print(output)
     ```
 
 ## Inspired from
 - [nlpaug](https://github.com/makcedward/nlpaug)
-- [amitness blog post](https://amitness.com/2020/05/data-augmentation-for-nlp/)
+- [amitness blog post](https://amitness.com/2020/05/data-augmentation-for-nlp/)
```

### Comparing `bnaug-1.1.0/bnaug/randaug.py` & `bnaug-1.1.1/bnaug/randaug.py`

 * *Files identical despite different names*

### Comparing `bnaug-1.1.0/bnaug/sentence.py` & `bnaug-1.1.1/bnaug/sentence.py`

 * *Files identical despite different names*

### Comparing `bnaug-1.1.0/bnaug.egg-info/PKG-INFO` & `bnaug-1.1.1/bnaug.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnaug
-Version: 1.1.0
+Version: 1.1.1
 Summary: bnaug is a text augmentation tool for Bangla text.
 Home-page: https://github.com/sagorbrur/bnaug
 Author: Sagor Sarker
 Author-email: sagorhem3532@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,17 @@
 
 ## Installation
 ```
 pip install bnaug
 ```
 - Dependencies
     - pytorch >=1.7.0
+    
+## Demo Notebook
+- [bnaug demo](https://github.com/sagorbrur/bnaug/blob/main/notebook/bnaug_demo.ipynb)
 
 ## Necessary Model Links
 - [word2vec](https://huggingface.co/sagorsarker/bangla_word2vec/resolve/main/bangla_word2vec_gen4.zip)
 - [glove vector](https://huggingface.co/sagorsarker/bangla-glove-vectors/resolve/main/bn_glove.300d.zip)
 
 ## Sentence Augmentation
 ### Token Replacement
```

### Comparing `bnaug-1.1.0/setup.py` & `bnaug-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import codecs
 import setuptools
 
 
 setuptools.setup(
     name="bnaug",
-    version="1.1.0",
+    version="1.1.1",
     author="Sagor Sarker",
     author_email="sagorhem3532@gmail.com",
     description="bnaug is a text augmentation tool for Bangla text.",
     long_description=codecs.open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/sagorbrur/bnaug",
     license="MIT",
@@ -16,11 +16,11 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
     install_requires=[
-        "bnlp_toolkit==3.2.0",
+        "bnlp_toolkit",
         "transformers==4.24.0"
     ]
 )
```

