# Comparing `tmp/pyaipersonality-0.0.8.tar.gz` & `tmp/pyaipersonality-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaipersonality-0.0.8.tar", last modified: Sat May  6 19:23:06 2023, max compression
+gzip compressed data, was "pyaipersonality-0.0.9.tar", last modified: Sat May  6 19:24:28 2023, max compression
```

## Comparing `pyaipersonality-0.0.8.tar` & `pyaipersonality-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 19:23:06.849302 pyaipersonality-0.0.8/
--rw-rw-rw-   0        0        0    11558 2023-04-29 07:11:51.000000 pyaipersonality-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     9394 2023-05-06 19:23:06.849302 pyaipersonality-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     8901 2023-05-06 19:20:42.000000 pyaipersonality-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 19:23:06.834299 pyaipersonality-0.0.8/pyaipersonality/
--rw-rw-rw-   0        0        0     8636 2023-05-06 19:04:20.000000 pyaipersonality-0.0.8/pyaipersonality/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 19:23:06.847298 pyaipersonality-0.0.8/pyaipersonality.egg-info/
--rw-rw-rw-   0        0        0     9394 2023-05-06 19:23:06.000000 pyaipersonality-0.0.8/pyaipersonality.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-05-06 19:23:06.000000 pyaipersonality-0.0.8/pyaipersonality.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 19:23:06.000000 pyaipersonality-0.0.8/pyaipersonality.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-05-06 19:23:06.000000 pyaipersonality-0.0.8/pyaipersonality.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-06 19:23:06.000000 pyaipersonality-0.0.8/pyaipersonality.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 19:23:06.850296 pyaipersonality-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-05-06 19:22:31.000000 pyaipersonality-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 19:24:28.451794 pyaipersonality-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2023-04-29 07:11:51.000000 pyaipersonality-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     9394 2023-05-06 19:24:28.451794 pyaipersonality-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8901 2023-05-06 19:24:03.000000 pyaipersonality-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 19:24:28.437278 pyaipersonality-0.0.9/pyaipersonality/
+-rw-rw-rw-   0        0        0     8636 2023-05-06 19:04:20.000000 pyaipersonality-0.0.9/pyaipersonality/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 19:24:28.450794 pyaipersonality-0.0.9/pyaipersonality.egg-info/
+-rw-rw-rw-   0        0        0     9394 2023-05-06 19:24:28.000000 pyaipersonality-0.0.9/pyaipersonality.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-05-06 19:24:28.000000 pyaipersonality-0.0.9/pyaipersonality.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 19:24:28.000000 pyaipersonality-0.0.9/pyaipersonality.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-06 19:24:28.000000 pyaipersonality-0.0.9/pyaipersonality.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-06 19:24:28.000000 pyaipersonality-0.0.9/pyaipersonality.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 19:24:28.452796 pyaipersonality-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-05-06 19:23:53.000000 pyaipersonality-0.0.9/setup.py
```

### Comparing `pyaipersonality-0.0.8/LICENSE` & `pyaipersonality-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaipersonality-0.0.8/PKG-INFO` & `pyaipersonality-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaipersonality
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/PyAIPersonality
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 ![GitHub forks](https://img.shields.io/github/forks/ParisNeo/PyAIPersonality)
 [![Discord](https://img.shields.io/discord/1092918764925882418?color=7289da&label=Discord&logo=discord&logoColor=ffffff)](https://discord.gg/4rR282WJb6)
 [![Follow me on Twitter](https://img.shields.io/twitter/follow/SpaceNerduino?style=social)](https://twitter.com/SpaceNerduino)
 [![Follow Me on YouTube](https://img.shields.io/badge/Follow%20Me%20on-YouTube-red?style=flat&logo=youtube)](https://www.youtube.com/user/Parisneo)
 
 [![PyPI](https://img.shields.io/pypi/v/pyaipersonality.svg)](https://pypi.org/project/pyaipersonality/)
 
-## Current version : 0.0.6 (GLaDOS)
+## Current version : 0.0.9 (GLaDOS)
 ## Main developer [ParisNeo](https://github.com/ParisNeo)
 
 PyAIPersonality is a Python library for defining AI personalities for AI-based models. With PyAIPersonality, you can define a file format, assets, and personalized scripts to create unique AI personalities.
 
 ## Installation
 
 You can install PyAIPersonality using pip:
```

### Comparing `pyaipersonality-0.0.8/README.md` & `pyaipersonality-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ![GitHub forks](https://img.shields.io/github/forks/ParisNeo/PyAIPersonality)
 [![Discord](https://img.shields.io/discord/1092918764925882418?color=7289da&label=Discord&logo=discord&logoColor=ffffff)](https://discord.gg/4rR282WJb6)
 [![Follow me on Twitter](https://img.shields.io/twitter/follow/SpaceNerduino?style=social)](https://twitter.com/SpaceNerduino)
 [![Follow Me on YouTube](https://img.shields.io/badge/Follow%20Me%20on-YouTube-red?style=flat&logo=youtube)](https://www.youtube.com/user/Parisneo)
 
 [![PyPI](https://img.shields.io/pypi/v/pyaipersonality.svg)](https://pypi.org/project/pyaipersonality/)
 
-## Current version : 0.0.6 (GLaDOS)
+## Current version : 0.0.9 (GLaDOS)
 ## Main developer [ParisNeo](https://github.com/ParisNeo)
 
 PyAIPersonality is a Python library for defining AI personalities for AI-based models. With PyAIPersonality, you can define a file format, assets, and personalized scripts to create unique AI personalities.
 
 ## Installation
 
 You can install PyAIPersonality using pip:
```

### Comparing `pyaipersonality-0.0.8/pyaipersonality/__init__.py` & `pyaipersonality-0.0.9/pyaipersonality/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaipersonality-0.0.8/pyaipersonality.egg-info/PKG-INFO` & `pyaipersonality-0.0.9/pyaipersonality.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaipersonality
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/PyAIPersonality
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,15 @@
 ![GitHub forks](https://img.shields.io/github/forks/ParisNeo/PyAIPersonality)
 [![Discord](https://img.shields.io/discord/1092918764925882418?color=7289da&label=Discord&logo=discord&logoColor=ffffff)](https://discord.gg/4rR282WJb6)
 [![Follow me on Twitter](https://img.shields.io/twitter/follow/SpaceNerduino?style=social)](https://twitter.com/SpaceNerduino)
 [![Follow Me on YouTube](https://img.shields.io/badge/Follow%20Me%20on-YouTube-red?style=flat&logo=youtube)](https://www.youtube.com/user/Parisneo)
 
 [![PyPI](https://img.shields.io/pypi/v/pyaipersonality.svg)](https://pypi.org/project/pyaipersonality/)
 
-## Current version : 0.0.6 (GLaDOS)
+## Current version : 0.0.9 (GLaDOS)
 ## Main developer [ParisNeo](https://github.com/ParisNeo)
 
 PyAIPersonality is a Python library for defining AI personalities for AI-based models. With PyAIPersonality, you can define a file format, assets, and personalized scripts to create unique AI personalities.
 
 ## Installation
 
 You can install PyAIPersonality using pip:
```

### Comparing `pyaipersonality-0.0.8/setup.py` & `pyaipersonality-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 requirements = read_requirements("requirements.txt")
 requirements_dev = read_requirements("requirements_dev.txt")
 
 setuptools.setup(
     name="pyaipersonality",
-    version="0.0.8",
+    version="0.0.9",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/PyAIPersonality",
     packages=setuptools.find_packages(),
```

