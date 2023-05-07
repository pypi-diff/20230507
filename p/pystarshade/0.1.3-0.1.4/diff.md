# Comparing `tmp/pystarshade-0.1.3.tar.gz` & `tmp/pystarshade-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pystarshade-0.1.3.tar", last modified: Sun May  7 20:39:57 2023, max compression
+gzip compressed data, was "dist/pystarshade-0.1.4.tar", last modified: Sun May  7 21:10:56 2023, max compression
```

## Comparing `pystarshade-0.1.3.tar` & `pystarshade-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 20:39:57.000000 pystarshade-0.1.3/
-drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 20:39:57.000000 pystarshade-0.1.3/pystarshade/
-drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 20:39:57.000000 pystarshade-0.1.3/pystarshade/apodization/
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     3163 2023-04-21 21:25:36.000000 pystarshade-0.1.3/pystarshade/apodization/apodization.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-21 21:01:22.000000 pystarshade-0.1.3/pystarshade/apodization/__init__.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)       48 2023-04-18 00:42:34.000000 pystarshade-0.1.3/pystarshade/apodization/sample.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-18 00:42:34.000000 pystarshade-0.1.3/pystarshade/version.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-18 00:42:34.000000 pystarshade-0.1.3/pystarshade/__init__.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     6718 2023-05-06 20:21:18.000000 pystarshade-0.1.3/pystarshade/simulate_field.py
-drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 20:39:57.000000 pystarshade-0.1.3/pystarshade/diffraction/
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     6682 2023-05-06 16:20:58.000000 pystarshade-0.1.3/pystarshade/diffraction/field.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-21 21:01:22.000000 pystarshade-0.1.3/pystarshade/diffraction/__init__.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     2004 2023-05-06 19:54:21.000000 pystarshade-0.1.3/pystarshade/diffraction/bluestein_fft.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     3362 2023-05-06 19:55:46.000000 pystarshade-0.1.3/pystarshade/diffraction/util.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     5953 2023-05-03 22:04:10.000000 pystarshade-0.1.3/pystarshade/diffraction/diffract.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     2257 2023-04-23 21:28:48.000000 pystarshade-0.1.3/README.md
-drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 20:39:57.000000 pystarshade-0.1.3/pystarshade.egg-info/
--rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-05-07 20:39:57.000000 pystarshade-0.1.3/pystarshade.egg-info/dependency_links.txt
--rw-rw-r--   0 ielo      (1000) ielo      (1000)       12 2023-05-07 20:39:57.000000 pystarshade-0.1.3/pystarshade.egg-info/top_level.txt
--rw-rw-r--   0 ielo      (1000) ielo      (1000)      737 2023-05-07 20:39:57.000000 pystarshade-0.1.3/pystarshade.egg-info/PKG-INFO
--rw-rw-r--   0 ielo      (1000) ielo      (1000)       12 2023-05-07 20:39:57.000000 pystarshade-0.1.3/pystarshade.egg-info/requires.txt
--rw-rw-r--   0 ielo      (1000) ielo      (1000)      556 2023-05-07 20:39:57.000000 pystarshade-0.1.3/pystarshade.egg-info/SOURCES.txt
--rw-rw-r--   0 ielo      (1000) ielo      (1000)      869 2023-05-07 17:34:37.000000 pystarshade-0.1.3/setup.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)      737 2023-05-07 20:39:57.000000 pystarshade-0.1.3/PKG-INFO
--rw-rw-r--   0 ielo      (1000) ielo      (1000)       38 2023-05-07 20:39:57.000000 pystarshade-0.1.3/setup.cfg
+drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:10:56.000000 pystarshade-0.1.4/
+drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:10:56.000000 pystarshade-0.1.4/pystarshade/
+drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:10:56.000000 pystarshade-0.1.4/pystarshade/apodization/
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     3163 2023-04-21 21:25:36.000000 pystarshade-0.1.4/pystarshade/apodization/apodization.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-21 21:01:22.000000 pystarshade-0.1.4/pystarshade/apodization/__init__.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)       48 2023-04-18 00:42:34.000000 pystarshade-0.1.4/pystarshade/apodization/sample.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-18 00:42:34.000000 pystarshade-0.1.4/pystarshade/version.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-18 00:42:34.000000 pystarshade-0.1.4/pystarshade/__init__.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     6718 2023-05-07 20:59:15.000000 pystarshade-0.1.4/pystarshade/simulate_field.py
+drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:10:56.000000 pystarshade-0.1.4/pystarshade/diffraction/
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     6682 2023-05-06 16:20:58.000000 pystarshade-0.1.4/pystarshade/diffraction/field.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-21 21:01:22.000000 pystarshade-0.1.4/pystarshade/diffraction/__init__.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     2004 2023-05-06 19:54:21.000000 pystarshade-0.1.4/pystarshade/diffraction/bluestein_fft.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     3362 2023-05-06 19:55:46.000000 pystarshade-0.1.4/pystarshade/diffraction/util.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     5953 2023-05-03 22:04:10.000000 pystarshade-0.1.4/pystarshade/diffraction/diffract.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     2404 2023-05-07 21:09:32.000000 pystarshade-0.1.4/README.md
+drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:10:56.000000 pystarshade-0.1.4/pystarshade.egg-info/
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-05-07 21:10:56.000000 pystarshade-0.1.4/pystarshade.egg-info/dependency_links.txt
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)       12 2023-05-07 21:10:56.000000 pystarshade-0.1.4/pystarshade.egg-info/top_level.txt
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)      737 2023-05-07 21:10:56.000000 pystarshade-0.1.4/pystarshade.egg-info/PKG-INFO
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)       12 2023-05-07 21:10:56.000000 pystarshade-0.1.4/pystarshade.egg-info/requires.txt
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)      556 2023-05-07 21:10:56.000000 pystarshade-0.1.4/pystarshade.egg-info/SOURCES.txt
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)      869 2023-05-07 20:58:19.000000 pystarshade-0.1.4/setup.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)      737 2023-05-07 21:10:56.000000 pystarshade-0.1.4/PKG-INFO
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)       38 2023-05-07 21:10:56.000000 pystarshade-0.1.4/setup.cfg
```

### Comparing `pystarshade-0.1.3/pystarshade/apodization/apodization.py` & `pystarshade-0.1.4/pystarshade/apodization/apodization.py`

 * *Files identical despite different names*

### Comparing `pystarshade-0.1.3/pystarshade/simulate_field.py` & `pystarshade-0.1.4/pystarshade/simulate_field.py`

 * *Files identical despite different names*

### Comparing `pystarshade-0.1.3/pystarshade/diffraction/field.py` & `pystarshade-0.1.4/pystarshade/diffraction/field.py`

 * *Files identical despite different names*

### Comparing `pystarshade-0.1.3/pystarshade/diffraction/bluestein_fft.py` & `pystarshade-0.1.4/pystarshade/diffraction/bluestein_fft.py`

 * *Files identical despite different names*

### Comparing `pystarshade-0.1.3/pystarshade/diffraction/util.py` & `pystarshade-0.1.4/pystarshade/diffraction/util.py`

 * *Files identical despite different names*

### Comparing `pystarshade-0.1.3/pystarshade/diffraction/diffract.py` & `pystarshade-0.1.4/pystarshade/diffraction/diffract.py`

 * *Files identical despite different names*

### Comparing `pystarshade-0.1.3/README.md` & `pystarshade-0.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -38,31 +38,35 @@
 
 Nominal parameters: 
 
 ## Organization
 
 <pre>
 Pystarshade
+├── examples
+│   ├── haystacks_model.py
+│   └── star_exo.py
 ├── images
-│   └── contrast_.gif
+│   └── contrast_.gif
+├── __init__.py
+├── pystarshade
+│   ├── apodization
+│   │   ├── apodization.py
+│   │   ├── __init__.py
+│   │   └── sample.py
+│   ├── diffraction
+│   │   ├── bluestein_fft.py
+│   │   ├── diffract.py
+│   │   ├── field.py
+│   │   ├── __init__.py
+│   │   └── util.py
+│   ├── __init__.py
+│   ├── simulate_field.py
+│   └── version.py
 ├── README.md
-├── setup.py
-└── starshade
-    ├── apodization
-    │   ├── apodization.py
-    │   ├── __init__.py
-    │   └── sample.py
-    ├── diffraction
-    │   ├── bluestein_fft.py
-    │   ├── diffract.py
-    │   ├── field.py
-    │   ├── __init__.py
-    │   └── util.py
-    ├── example_star_exo.py
-    ├── __init__.py
-    ├── simulate_field.py
-    └── version.py
+└── setup.py
+
 </pre>
 
 ## License
 
 [PyStarshade] is released under the [GNU General Public License v3.0](LICENSE).
```

### Comparing `pystarshade-0.1.3/pystarshade.egg-info/PKG-INFO` & `pystarshade-0.1.4/pystarshade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystarshade
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python package for end-to-end starshade simulation
 Home-page: https://github.com/xiaziyna/PyStarshade
 Author: Jamila Taaki
 Author-email: xiaziyna@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pystarshade-0.1.3/pystarshade.egg-info/SOURCES.txt` & `pystarshade-0.1.4/pystarshade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystarshade-0.1.3/setup.py` & `pystarshade-0.1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pystarshade",
-    version="0.1.3",
+    version="0.1.4",
     description="A python package for end-to-end starshade simulation",
     author="Jamila Taaki",
     author_email="xiaziyna@gmail.com",
     url="https://github.com/xiaziyna/PyStarshade",
     packages=find_packages(),
     install_requires=[
         "numpy",
```

### Comparing `pystarshade-0.1.3/PKG-INFO` & `pystarshade-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystarshade
-Version: 0.1.3
+Version: 0.1.4
 Summary: A python package for end-to-end starshade simulation
 Home-page: https://github.com/xiaziyna/PyStarshade
 Author: Jamila Taaki
 Author-email: xiaziyna@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

