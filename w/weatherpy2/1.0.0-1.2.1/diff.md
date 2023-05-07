# Comparing `tmp/weatherpy2-1.0.0.tar.gz` & `tmp/weatherpy2-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weatherpy2-1.0.0.tar", last modified: Sun May  7 18:32:41 2023, max compression
+gzip compressed data, was "weatherpy2-1.2.1.tar", last modified: Thu Mar 30 02:36:54 2023, max compression
```

## Comparing `weatherpy2-1.0.0.tar` & `weatherpy2-1.2.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 18:32:41.187312 weatherpy2-1.0.0/
--rw-rw-rw-   0        0        0      772 2023-05-07 18:32:41.186318 weatherpy2-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-07 18:32:41.156230 weatherpy2-1.0.0/jetbrainsfleetrun/
--rw-rw-rw-   0        0        0       66 2023-05-07 18:29:46.000000 weatherpy2-1.0.0/jetbrainsfleetrun/__init__.py
--rw-rw-rw-   0        0        0      665 2023-05-07 18:25:46.000000 weatherpy2-1.0.0/jetbrainsfleetrun/jetbrainsfleetrun.py
--rw-rw-rw-   0        0        0       42 2023-05-07 18:32:41.187312 weatherpy2-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      948 2023-05-07 18:31:18.000000 weatherpy2-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 18:32:41.184302 weatherpy2-1.0.0/weatherpy2.egg-info/
--rw-rw-rw-   0        0        0      772 2023-05-07 18:32:41.000000 weatherpy2-1.0.0/weatherpy2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-05-07 18:32:41.000000 weatherpy2-1.0.0/weatherpy2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 18:32:41.000000 weatherpy2-1.0.0/weatherpy2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-07 18:32:41.000000 weatherpy2-1.0.0/weatherpy2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-07 18:32:41.000000 weatherpy2-1.0.0/weatherpy2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-30 02:36:54.149339 weatherpy2-1.2.1/
+-rw-rw-rw-   0        0        0      757 2023-03-30 02:36:54.148315 weatherpy2-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-03-30 02:36:54.149339 weatherpy2-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      926 2023-03-30 02:36:23.000000 weatherpy2-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-30 02:36:54.130243 weatherpy2-1.2.1/weatherpy2/
+-rw-rw-rw-   0        0        0       43 2023-03-30 02:12:00.000000 weatherpy2-1.2.1/weatherpy2/__init__.py
+-rw-rw-rw-   0        0        0      925 2023-03-30 02:20:35.000000 weatherpy2-1.2.1/weatherpy2/setup.py
+-rw-rw-rw-   0        0        0     2270 2023-03-30 02:09:21.000000 weatherpy2-1.2.1/weatherpy2/weatherpy2.py
+drwxrwxrwx   0        0        0        0 2023-03-30 02:36:54.146799 weatherpy2-1.2.1/weatherpy2.egg-info/
+-rw-rw-rw-   0        0        0      757 2023-03-30 02:36:54.000000 weatherpy2-1.2.1/weatherpy2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-03-30 02:36:54.000000 weatherpy2-1.2.1/weatherpy2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-30 02:36:54.000000 weatherpy2-1.2.1/weatherpy2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-03-30 02:36:54.000000 weatherpy2-1.2.1/weatherpy2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-03-30 02:36:54.000000 weatherpy2-1.2.1/weatherpy2.egg-info/top_level.txt
```

### Comparing `weatherpy2-1.0.0/PKG-INFO` & `weatherpy2-1.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: weatherpy2
-Version: 1.0.0
-Summary: Easy Python file running in JetBrains Fleet
-Home-page: https://github.com/GamerXZEN/jetbrainsfleetrun
+Version: 1.2.1
+Summary: Easy weather forcasting for Python 3
+Home-page: https://github.com/GamerXZEN/weatherpy2
 Author: GamerXZEN
 Author-email: codspecialops@gmail.com
 Keywords: weather,forecast,python
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `weatherpy2-1.0.0/setup.py` & `weatherpy2-1.2.1/weatherpy2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup
 setup(
     name='weatherpy2',
-    packages=['jetbrainsfleetrun'],
-    version="1.0.0",
+    packages=['weatherpy2'],
+    version="1.2.1",
     liscense="MIT",
-    description="Easy Python file running in JetBrains Fleet",
+    description="Easy weather forcasting for Python 3",
     author="GamerXZEN",
     author_email="codspecialops@gmail.com",
-    url="https://github.com/GamerXZEN/jetbrainsfleetrun",
+    url="https://github.com/GamerXZEN/weatherpy2",
     keywords=["weather", "forecast", "python",],
     install_requires=["requests"],
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python:: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `weatherpy2-1.0.0/weatherpy2.egg-info/PKG-INFO` & `weatherpy2-1.2.1/weatherpy2.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: weatherpy2
-Version: 1.0.0
-Summary: Easy Python file running in JetBrains Fleet
-Home-page: https://github.com/GamerXZEN/jetbrainsfleetrun
+Version: 1.2.1
+Summary: Easy weather forcasting for Python 3
+Home-page: https://github.com/GamerXZEN/weatherpy2
 Author: GamerXZEN
 Author-email: codspecialops@gmail.com
 Keywords: weather,forecast,python
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

