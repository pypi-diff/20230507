# Comparing `tmp/PySpecies-0.1.1.tar.gz` & `tmp/PySpecies-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySpecies-0.1.1.tar", last modified: Sat May  6 22:34:22 2023, max compression
+gzip compressed data, was "PySpecies-0.1.2.tar", last modified: Sat May  6 23:26:37 2023, max compression
```

## Comparing `PySpecies-0.1.1.tar` & `PySpecies-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-05-06 22:34:22.588324 PySpecies-0.1.1/
--rwxr-xr-x   0 sam       (1000) sam       (1000)     1085 2023-03-26 13:57:19.000000 PySpecies-0.1.1/LICENSE
--rw-r--r--   0 sam       (1000) sam       (1000)     2034 2023-05-06 22:34:22.588324 PySpecies-0.1.1/PKG-INFO
--rwxr-xr-x   0 sam       (1000) sam       (1000)     1530 2023-05-06 22:18:09.000000 PySpecies-0.1.1/README.md
--rw-r--r--   0 sam       (1000) sam       (1000)       38 2023-05-06 22:34:22.588324 PySpecies-0.1.1/setup.cfg
--rw-r--r--   0 sam       (1000) sam       (1000)      763 2023-05-06 22:34:03.000000 PySpecies-0.1.1/setup.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-05-06 22:34:22.584324 PySpecies-0.1.1/src/
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-05-06 22:34:22.588324 PySpecies-0.1.1/src/PySpecies.egg-info/
--rw-r--r--   0 sam       (1000) sam       (1000)     2034 2023-05-06 22:34:22.000000 PySpecies-0.1.1/src/PySpecies.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)      293 2023-05-06 22:34:22.000000 PySpecies-0.1.1/src/PySpecies.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-05-06 22:34:22.000000 PySpecies-0.1.1/src/PySpecies.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       10 2023-05-06 22:34:22.000000 PySpecies-0.1.1/src/PySpecies.egg-info/top_level.txt
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-05-06 22:34:22.588324 PySpecies-0.1.1/src/pyspecies/
--rwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-05-06 22:31:14.000000 PySpecies-0.1.1/src/pyspecies/__init__.py
--rwxr-xr-x   0 sam       (1000) sam       (1000)     4143 2023-05-06 22:31:14.000000 PySpecies-0.1.1/src/pyspecies/_euler.py
--rwxr-xr-x   0 sam       (1000) sam       (1000)     4348 2023-05-06 22:31:14.000000 PySpecies-0.1.1/src/pyspecies/_utils.py
--rwxr-xr-x   0 sam       (1000) sam       (1000)     1919 2023-05-06 22:31:14.000000 PySpecies-0.1.1/src/pyspecies/models.py
--rwxr-xr-x   0 sam       (1000) sam       (1000)     7224 2023-05-06 22:31:14.000000 PySpecies-0.1.1/src/pyspecies/pop.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-05-06 23:26:37.557304 PySpecies-0.1.2/
+-rwxr-xr-x   0 sam       (1000) sam       (1000)     1085 2023-03-26 13:57:19.000000 PySpecies-0.1.2/LICENSE
+-rw-r--r--   0 sam       (1000) sam       (1000)     2193 2023-05-06 23:26:37.557304 PySpecies-0.1.2/PKG-INFO
+-rwxr-xr-x   0 sam       (1000) sam       (1000)     1693 2023-05-06 23:21:51.000000 PySpecies-0.1.2/README.md
+-rw-r--r--   0 sam       (1000) sam       (1000)       38 2023-05-06 23:26:37.557304 PySpecies-0.1.2/setup.cfg
+-rw-r--r--   0 sam       (1000) sam       (1000)      755 2023-05-06 23:25:52.000000 PySpecies-0.1.2/setup.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-05-06 23:26:37.557304 PySpecies-0.1.2/src/
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-05-06 23:26:37.557304 PySpecies-0.1.2/src/PySpecies.egg-info/
+-rw-r--r--   0 sam       (1000) sam       (1000)     2193 2023-05-06 23:26:37.000000 PySpecies-0.1.2/src/PySpecies.egg-info/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)      293 2023-05-06 23:26:37.000000 PySpecies-0.1.2/src/PySpecies.egg-info/SOURCES.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-05-06 23:26:37.000000 PySpecies-0.1.2/src/PySpecies.egg-info/dependency_links.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       10 2023-05-06 23:26:37.000000 PySpecies-0.1.2/src/PySpecies.egg-info/top_level.txt
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-05-06 23:26:37.557304 PySpecies-0.1.2/src/pyspecies/
+-rwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-05-06 22:31:14.000000 PySpecies-0.1.2/src/pyspecies/__init__.py
+-rwxr-xr-x   0 sam       (1000) sam       (1000)     4143 2023-05-06 22:31:14.000000 PySpecies-0.1.2/src/pyspecies/_euler.py
+-rwxr-xr-x   0 sam       (1000) sam       (1000)     4348 2023-05-06 22:31:14.000000 PySpecies-0.1.2/src/pyspecies/_utils.py
+-rwxr-xr-x   0 sam       (1000) sam       (1000)     1919 2023-05-06 22:31:14.000000 PySpecies-0.1.2/src/pyspecies/models.py
+-rwxr-xr-x   0 sam       (1000) sam       (1000)     7224 2023-05-06 22:31:14.000000 PySpecies-0.1.2/src/pyspecies/pop.py
```

### Comparing `PySpecies-0.1.1/LICENSE` & `PySpecies-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PySpecies-0.1.1/PKG-INFO` & `PySpecies-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: PySpecies
-Version: 0.1.1
+Version: 0.1.2
 Summary: Blazing-fast simulation of self-organized patterns in reaction-diffusion systems.
-Home-page: https://github.com/samuel-boite/pyspecies
+Home-page: https://github.com/samuelbx/pyspecies
 Author: Samuel Boïté, Mathias Grau
 Author-email: boite.samuel@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PySpecies
 
-Blazing-fast simulation of advanced 1D population dynamics.
+[![PyPI version](https://badge.fury.io/py/pyspecies.svg)](https://badge.fury.io/py/pyspecies)
 
-Based on the Shigesada Kawasaki Teramoto (SKT) reaction-diffusion model. [[PubMed '79]](https://pubmed.ncbi.nlm.nih.gov/513804/)
+Blazing-fast simulation of population dynamics, based on the Shigesada-Kawasaki-Teramoto (SKT) reaction-diffusion model. [[PubMed '79]](https://pubmed.ncbi.nlm.nih.gov/513804/)
 
-![Population dynamics simulation](./misc/example.gif)
+![Population dynamics simulation](https://github.com/samuelbx/pyspecies/raw/main/misc/example.gif)
 
 ## Installation
 
 ```bash
 pip install pyspecies
 ```
 
@@ -73,8 +73,8 @@
 p.sim(duration=20, N=200)
 p.sim(duration=100, N=200)
 p.anim()
 ```
 
 ## Theory
 
-The calculations underlying this library are described (in French) in the following document: [Théorie](./misc/theory.pdf).
+The calculations underlying this library are described (in French) in the [following document](https://github.com/samuelbx/pyspecies/blob/main/misc/theory.pdf).
```

### Comparing `PySpecies-0.1.1/README.md` & `PySpecies-0.1.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # PySpecies
 
-Blazing-fast simulation of advanced 1D population dynamics.
+[![PyPI version](https://badge.fury.io/py/pyspecies.svg)](https://badge.fury.io/py/pyspecies)
 
-Based on the Shigesada Kawasaki Teramoto (SKT) reaction-diffusion model. [[PubMed '79]](https://pubmed.ncbi.nlm.nih.gov/513804/)
+Blazing-fast simulation of population dynamics, based on the Shigesada-Kawasaki-Teramoto (SKT) reaction-diffusion model. [[PubMed '79]](https://pubmed.ncbi.nlm.nih.gov/513804/)
 
-![Population dynamics simulation](./misc/example.gif)
+![Population dynamics simulation](https://github.com/samuelbx/pyspecies/raw/main/misc/example.gif)
 
 ## Installation
 
 ```bash
 pip install pyspecies
 ```
 
@@ -59,8 +59,8 @@
 p.sim(duration=20, N=200)
 p.sim(duration=100, N=200)
 p.anim()
 ```
 
 ## Theory
 
-The calculations underlying this library are described (in French) in the following document: [Théorie](./misc/theory.pdf).
+The calculations underlying this library are described (in French) in the [following document](https://github.com/samuelbx/pyspecies/blob/main/misc/theory.pdf).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `PySpecies-0.1.1/setup.py` & `PySpecies-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PySpecies",
-    version="0.1.1",
+    version="0.1.2",
     author="Samuel Boïté, Mathias Grau",
     author_email="boite.samuel@gmail.com",
     description="Blazing-fast simulation of self-organized patterns in reaction-diffusion systems.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/samuel-boite/pyspecies",
-    package_dir = {"": "src"},
-    packages = setuptools.find_packages(where="src"),
+    url="https://github.com/samuelbx/pyspecies",
+    package_dir={"": "src"},
+    packages=setuptools.find_packages(where="src"),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
 )
```

### Comparing `PySpecies-0.1.1/src/PySpecies.egg-info/PKG-INFO` & `PySpecies-0.1.2/src/PySpecies.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: PySpecies
-Version: 0.1.1
+Version: 0.1.2
 Summary: Blazing-fast simulation of self-organized patterns in reaction-diffusion systems.
-Home-page: https://github.com/samuel-boite/pyspecies
+Home-page: https://github.com/samuelbx/pyspecies
 Author: Samuel Boïté, Mathias Grau
 Author-email: boite.samuel@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PySpecies
 
-Blazing-fast simulation of advanced 1D population dynamics.
+[![PyPI version](https://badge.fury.io/py/pyspecies.svg)](https://badge.fury.io/py/pyspecies)
 
-Based on the Shigesada Kawasaki Teramoto (SKT) reaction-diffusion model. [[PubMed '79]](https://pubmed.ncbi.nlm.nih.gov/513804/)
+Blazing-fast simulation of population dynamics, based on the Shigesada-Kawasaki-Teramoto (SKT) reaction-diffusion model. [[PubMed '79]](https://pubmed.ncbi.nlm.nih.gov/513804/)
 
-![Population dynamics simulation](./misc/example.gif)
+![Population dynamics simulation](https://github.com/samuelbx/pyspecies/raw/main/misc/example.gif)
 
 ## Installation
 
 ```bash
 pip install pyspecies
 ```
 
@@ -73,8 +73,8 @@
 p.sim(duration=20, N=200)
 p.sim(duration=100, N=200)
 p.anim()
 ```
 
 ## Theory
 
-The calculations underlying this library are described (in French) in the following document: [Théorie](./misc/theory.pdf).
+The calculations underlying this library are described (in French) in the [following document](https://github.com/samuelbx/pyspecies/blob/main/misc/theory.pdf).
```

### Comparing `PySpecies-0.1.1/src/pyspecies/_euler.py` & `PySpecies-0.1.2/src/pyspecies/_euler.py`

 * *Files identical despite different names*

### Comparing `PySpecies-0.1.1/src/pyspecies/_utils.py` & `PySpecies-0.1.2/src/pyspecies/_utils.py`

 * *Files identical despite different names*

### Comparing `PySpecies-0.1.1/src/pyspecies/models.py` & `PySpecies-0.1.2/src/pyspecies/models.py`

 * *Files identical despite different names*

### Comparing `PySpecies-0.1.1/src/pyspecies/pop.py` & `PySpecies-0.1.2/src/pyspecies/pop.py`

 * *Files identical despite different names*

