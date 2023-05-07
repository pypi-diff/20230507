# Comparing `tmp/EvaLLM-1.1.2.tar.gz` & `tmp/EvaLLM-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EvaLLM-1.1.2.tar", last modified: Sat May  6 01:55:04 2023, max compression
+gzip compressed data, was "EvaLLM-1.1.3.tar", last modified: Sun May  7 17:30:50 2023, max compression
```

## Comparing `EvaLLM-1.1.2.tar` & `EvaLLM-1.1.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 01:55:04.367840 EvaLLM-1.1.2/
-drwxrwxrwx   0        0        0        0 2023-05-06 01:55:04.366249 EvaLLM-1.1.2/EvaLLM.egg-info/
--rw-rw-rw-   0        0        0     1725 2023-05-06 01:55:04.000000 EvaLLM-1.1.2/EvaLLM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2023-05-06 01:55:04.000000 EvaLLM-1.1.2/EvaLLM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 01:55:04.000000 EvaLLM-1.1.2/EvaLLM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 01:55:04.000000 EvaLLM-1.1.2/EvaLLM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2023-05-06 01:44:41.000000 EvaLLM-1.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1725 2023-05-06 01:55:04.367275 EvaLLM-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1344 2023-05-06 01:44:39.000000 EvaLLM-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 01:55:04.368352 EvaLLM-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1896 2023-05-06 01:54:53.000000 EvaLLM-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 17:30:50.403595 EvaLLM-1.1.3/
+drwxrwxrwx   0        0        0        0 2023-05-07 17:30:50.401976 EvaLLM-1.1.3/EvaLLM.egg-info/
+-rw-rw-rw-   0        0        0     1795 2023-05-07 17:30:50.000000 EvaLLM-1.1.3/EvaLLM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2023-05-07 17:30:50.000000 EvaLLM-1.1.3/EvaLLM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 17:30:50.000000 EvaLLM-1.1.3/EvaLLM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-07 17:30:50.000000 EvaLLM-1.1.3/EvaLLM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 17:30:50.000000 EvaLLM-1.1.3/EvaLLM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2023-05-06 01:44:41.000000 EvaLLM-1.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1795 2023-05-07 17:30:50.402982 EvaLLM-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1344 2023-05-06 01:44:39.000000 EvaLLM-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-07 17:30:50.404104 EvaLLM-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2039 2023-05-07 17:01:21.000000 EvaLLM-1.1.3/setup.py
```

### Comparing `EvaLLM-1.1.2/EvaLLM.egg-info/PKG-INFO` & `EvaLLM-1.1.3/EvaLLM.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EvaLLM
-Version: 1.1.2
+Version: 1.1.3
 Summary: Speak with an emotional AI Chatbot, 100% free.
 Home-page: 
 Author: CodeSoft
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 
 ## EvaLLM
 A Python Package that incorporates emotional AI into your code.
 
 ## Getting Started
 Getting started is incredibly simple. First, install EvaLLM by using pip.
     `pip install evallm`
-The modules will not install yet, as they install when you first run.
+The models will not install yet, as they install when you first run. This pip install will use about 2GB - 4GB, and models take 2GB to 3GB.
 
 ## Usage
 Now that you've installed, you can use the `respond()` function. There is 1 required parameter, and 1 optional. Prompt is the prompt for Eva. Temperature is a decimal integer between 0 and 1 that determines how creative Eva will be. If you have worked with GPT-3, then it works the same here. An example usage of a chat application with Eva may look like this:
 
 ```
 #Import packages
 import evallm as eva
```

### Comparing `EvaLLM-1.1.2/LICENSE.txt` & `EvaLLM-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EvaLLM-1.1.2/PKG-INFO` & `EvaLLM-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EvaLLM
-Version: 1.1.2
+Version: 1.1.3
 Summary: Speak with an emotional AI Chatbot, 100% free.
 Home-page: 
 Author: CodeSoft
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 
 ## EvaLLM
 A Python Package that incorporates emotional AI into your code.
 
 ## Getting Started
 Getting started is incredibly simple. First, install EvaLLM by using pip.
     `pip install evallm`
-The modules will not install yet, as they install when you first run.
+The models will not install yet, as they install when you first run. This pip install will use about 2GB - 4GB, and models take 2GB to 3GB.
 
 ## Usage
 Now that you've installed, you can use the `respond()` function. There is 1 required parameter, and 1 optional. Prompt is the prompt for Eva. Temperature is a decimal integer between 0 and 1 that determines how creative Eva will be. If you have worked with GPT-3, then it works the same here. An example usage of a chat application with Eva may look like this:
 
 ```
 #Import packages
 import evallm as eva
```

### Comparing `EvaLLM-1.1.2/README.md` & `EvaLLM-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `EvaLLM-1.1.2/setup.py` & `EvaLLM-1.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 ## EvaLLM
 A Python Package that incorporates emotional AI into your code.
 
 ## Getting Started
 Getting started is incredibly simple. First, install EvaLLM by using pip.
     `pip install evallm`
-The modules will not install yet, as they install when you first run.
+The models will not install yet, as they install when you first run. This pip install will use about 2GB - 4GB, and models take 2GB to 3GB.
 
 ## Usage
 Now that you've installed, you can use the `respond()` function. There is 1 required parameter, and 1 optional. Prompt is the prompt for Eva. Temperature is a decimal integer between 0 and 1 that determines how creative Eva will be. If you have worked with GPT-3, then it works the same here. An example usage of a chat application with Eva may look like this:
 
 ```
 #Import packages
 import evallm as eva
@@ -39,21 +39,25 @@
 
 ## Mascot
 Eva has an official mascot. It is a female girl, often depicted in the style of Anime. Here's a picture:
 ![Image of Eva](https://codesoft-assets.codesoftgames.repl.co/eva/transparent.png)'''
 
 setuptools.setup(
     name="EvaLLM",
-    version="1.1.2",
+    version="1.1.3",
     author="CodeSoft",
+    install_requires=[
+        'torch',
+        'transformers',
+    ],
     author_email="",
     description="Speak with an emotional AI Chatbot, 100% free.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-)
+)
```

