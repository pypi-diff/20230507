# Comparing `tmp/transformgpt-0.1.1.tar.gz` & `tmp/transformgpt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformgpt-0.1.1.tar", last modified: Sat May  6 22:30:19 2023, max compression
+gzip compressed data, was "transformgpt-0.1.2.tar", last modified: Sat May  6 22:42:14 2023, max compression
```

## Comparing `transformgpt-0.1.1.tar` & `transformgpt-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:30:19.084130 transformgpt-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-06 22:30:04.000000 transformgpt-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-05-06 22:30:19.084130 transformgpt-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-06 22:30:04.000000 transformgpt-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-06 22:30:19.084130 transformgpt-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-06 22:30:04.000000 transformgpt-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:30:19.080130 transformgpt-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-06 22:30:04.000000 transformgpt-0.1.1/test/test_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:30:19.080130 transformgpt-0.1.1/transformgpt/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 22:30:04.000000 transformgpt-0.1.1/transformgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-06 22:30:04.000000 transformgpt-0.1.1/transformgpt/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-06 22:30:04.000000 transformgpt-0.1.1/transformgpt/source_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-06 22:30:04.000000 transformgpt-0.1.1/transformgpt/transformgpt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:30:19.084130 transformgpt-0.1.1/transformgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-05-06 22:30:19.000000 transformgpt-0.1.1/transformgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-06 22:30:19.000000 transformgpt-0.1.1/transformgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 22:30:19.000000 transformgpt-0.1.1/transformgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-06 22:30:19.000000 transformgpt-0.1.1/transformgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 22:30:19.000000 transformgpt-0.1.1/transformgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-06 22:30:19.000000 transformgpt-0.1.1/transformgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:42:14.853140 transformgpt-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-06 22:42:01.000000 transformgpt-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-05-06 22:42:14.853140 transformgpt-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-05-06 22:42:01.000000 transformgpt-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-06 22:42:14.853140 transformgpt-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-06 22:42:01.000000 transformgpt-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:42:14.849140 transformgpt-0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-06 22:42:01.000000 transformgpt-0.1.2/test/test_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:42:14.849140 transformgpt-0.1.2/transformgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 22:42:01.000000 transformgpt-0.1.2/transformgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-06 22:42:01.000000 transformgpt-0.1.2/transformgpt/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-06 22:42:01.000000 transformgpt-0.1.2/transformgpt/source_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-06 22:42:01.000000 transformgpt-0.1.2/transformgpt/transformgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:42:14.853140 transformgpt-0.1.2/transformgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-05-06 22:42:14.000000 transformgpt-0.1.2/transformgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-06 22:42:14.000000 transformgpt-0.1.2/transformgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 22:42:14.000000 transformgpt-0.1.2/transformgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-06 22:42:14.000000 transformgpt-0.1.2/transformgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 22:42:14.000000 transformgpt-0.1.2/transformgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-06 22:42:14.000000 transformgpt-0.1.2/transformgpt.egg-info/top_level.txt
```

### Comparing `transformgpt-0.1.1/LICENSE` & `transformgpt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `transformgpt-0.1.1/PKG-INFO` & `transformgpt-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: transformgpt
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for transforming unstructured text into structured data without context/mappings using ChatGPT.
 Home-page: https://github.com/TSavo/transformgpt
-Download-URL: https://github.com/tsavo/transformgpt/tarball/0.1.1
+Download-URL: https://github.com/tsavo/transformgpt/tarball/0.1.2
 Author: T Savo
 Author-email: evilgenius@nefariousplan.com
 License: MIT
 Keywords: openai gpt3 chatgpt nlp chatbot transformers structruing text
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -60,16 +60,19 @@
                     [-k KEY]
                     [-m MODEL]
                     [-t TEMPERATURE]
                     description
 ```
 
 KEY: OpenAI API Token if it's not set as an environment variable.
-MMDEL: OpenAI Model, defaults to 'gpt-3.5-turbo'
+
+MODEL: OpenAI Model, defaults to 'gpt-3.5-turbo'
+
 TEMPERATURE: Temperature for the ChatCompletion, defaults to 0, increase towards 1 to make the answers more creative
+
 Description: A description of how you want the data to be transformed.
 
 Takes input from STDIN and returns on STDOUT the transformed data.
 
 ### Example:
 ```
 > echo "Hello World.\nHow are you today?\nI am fine.\nIf you don't respond I will blackmail you." | transformgpt "An object with the fields original_message, intent, and response, where intent is one of greeting, inquiry, response, threat, informative."
```

### Comparing `transformgpt-0.1.1/README.md` & `transformgpt-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,19 @@
                     [-k KEY]
                     [-m MODEL]
                     [-t TEMPERATURE]
                     description
 ```
 
 KEY: OpenAI API Token if it's not set as an environment variable.
-MMDEL: OpenAI Model, defaults to 'gpt-3.5-turbo'
+
+MODEL: OpenAI Model, defaults to 'gpt-3.5-turbo'
+
 TEMPERATURE: Temperature for the ChatCompletion, defaults to 0, increase towards 1 to make the answers more creative
+
 Description: A description of how you want the data to be transformed.
 
 Takes input from STDIN and returns on STDOUT the transformed data.
 
 ### Example:
 ```
 > echo "Hello World.\nHow are you today?\nI am fine.\nIf you don't respond I will blackmail you." | transformgpt "An object with the fields original_message, intent, and response, where intent is one of greeting, inquiry, response, threat, informative."
```

### Comparing `transformgpt-0.1.1/setup.py` & `transformgpt-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup
-VERSION='0.1.1'
+VERSION='0.1.2'
 setup(
     name='transformgpt',
     version=VERSION,
     packages=['transformgpt'],
     author='T Savo',
     author_email="evilgenius@nefariousplan.com",
     description="A library for transforming unstructured text into structured data without context/mappings using ChatGPT.",
```

### Comparing `transformgpt-0.1.1/test/test_interpreter.py` & `transformgpt-0.1.2/test/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `transformgpt-0.1.1/transformgpt/main.py` & `transformgpt-0.1.2/transformgpt/main.py`

 * *Files identical despite different names*

### Comparing `transformgpt-0.1.1/transformgpt/source_utils.py` & `transformgpt-0.1.2/transformgpt/source_utils.py`

 * *Files identical despite different names*

### Comparing `transformgpt-0.1.1/transformgpt/transformgpt.py` & `transformgpt-0.1.2/transformgpt/transformgpt.py`

 * *Files identical despite different names*

### Comparing `transformgpt-0.1.1/transformgpt.egg-info/PKG-INFO` & `transformgpt-0.1.2/transformgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: transformgpt
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library for transforming unstructured text into structured data without context/mappings using ChatGPT.
 Home-page: https://github.com/TSavo/transformgpt
-Download-URL: https://github.com/tsavo/transformgpt/tarball/0.1.1
+Download-URL: https://github.com/tsavo/transformgpt/tarball/0.1.2
 Author: T Savo
 Author-email: evilgenius@nefariousplan.com
 License: MIT
 Keywords: openai gpt3 chatgpt nlp chatbot transformers structruing text
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -60,16 +60,19 @@
                     [-k KEY]
                     [-m MODEL]
                     [-t TEMPERATURE]
                     description
 ```
 
 KEY: OpenAI API Token if it's not set as an environment variable.
-MMDEL: OpenAI Model, defaults to 'gpt-3.5-turbo'
+
+MODEL: OpenAI Model, defaults to 'gpt-3.5-turbo'
+
 TEMPERATURE: Temperature for the ChatCompletion, defaults to 0, increase towards 1 to make the answers more creative
+
 Description: A description of how you want the data to be transformed.
 
 Takes input from STDIN and returns on STDOUT the transformed data.
 
 ### Example:
 ```
 > echo "Hello World.\nHow are you today?\nI am fine.\nIf you don't respond I will blackmail you." | transformgpt "An object with the fields original_message, intent, and response, where intent is one of greeting, inquiry, response, threat, informative."
```

