# Comparing `tmp/pystarshade-0.1.6.tar.gz` & `tmp/pystarshade-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pystarshade-0.1.6.tar", last modified: Sun May  7 21:29:14 2023, max compression
+gzip compressed data, was "dist/pystarshade-0.1.7.tar", last modified: Sun May  7 21:40:34 2023, max compression
```

## Comparing `pystarshade-0.1.6.tar` & `pystarshade-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:29:14.000000 pystarshade-0.1.6/
-drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:29:14.000000 pystarshade-0.1.6/pystarshade/
-drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:29:14.000000 pystarshade-0.1.6/pystarshade/apodization/
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     3165 2023-05-07 21:26:47.000000 pystarshade-0.1.6/pystarshade/apodization/apodize.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-21 21:01:22.000000 pystarshade-0.1.6/pystarshade/apodization/__init__.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-18 00:42:34.000000 pystarshade-0.1.6/pystarshade/__init__.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     6718 2023-05-07 21:27:02.000000 pystarshade-0.1.6/pystarshade/simulate_field.py
-drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:29:14.000000 pystarshade-0.1.6/pystarshade/diffraction/
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     6684 2023-05-07 21:27:27.000000 pystarshade-0.1.6/pystarshade/diffraction/field.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-21 21:01:22.000000 pystarshade-0.1.6/pystarshade/diffraction/__init__.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     2005 2023-05-07 21:27:49.000000 pystarshade-0.1.6/pystarshade/diffraction/bluestein_fft.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     3362 2023-05-06 19:55:46.000000 pystarshade-0.1.6/pystarshade/diffraction/util.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     5955 2023-05-07 21:27:18.000000 pystarshade-0.1.6/pystarshade/diffraction/diffract.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     2404 2023-05-07 21:09:32.000000 pystarshade-0.1.6/README.md
-drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:29:14.000000 pystarshade-0.1.6/pystarshade.egg-info/
--rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-05-07 21:29:14.000000 pystarshade-0.1.6/pystarshade.egg-info/dependency_links.txt
--rw-rw-r--   0 ielo      (1000) ielo      (1000)       12 2023-05-07 21:29:14.000000 pystarshade-0.1.6/pystarshade.egg-info/top_level.txt
--rw-rw-r--   0 ielo      (1000) ielo      (1000)      737 2023-05-07 21:29:14.000000 pystarshade-0.1.6/pystarshade.egg-info/PKG-INFO
--rw-rw-r--   0 ielo      (1000) ielo      (1000)       12 2023-05-07 21:29:14.000000 pystarshade-0.1.6/pystarshade.egg-info/requires.txt
--rw-rw-r--   0 ielo      (1000) ielo      (1000)      495 2023-05-07 21:29:14.000000 pystarshade-0.1.6/pystarshade.egg-info/SOURCES.txt
--rw-rw-r--   0 ielo      (1000) ielo      (1000)      869 2023-05-07 21:28:54.000000 pystarshade-0.1.6/setup.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)      737 2023-05-07 21:29:14.000000 pystarshade-0.1.6/PKG-INFO
--rw-rw-r--   0 ielo      (1000) ielo      (1000)       38 2023-05-07 21:29:14.000000 pystarshade-0.1.6/setup.cfg
+drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:40:34.000000 pystarshade-0.1.7/
+drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:40:34.000000 pystarshade-0.1.7/pystarshade/
+drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:40:34.000000 pystarshade-0.1.7/pystarshade/apodization/
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     3165 2023-05-07 21:26:47.000000 pystarshade-0.1.7/pystarshade/apodization/apodize.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-21 21:01:22.000000 pystarshade-0.1.7/pystarshade/apodization/__init__.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-18 00:42:34.000000 pystarshade-0.1.7/pystarshade/__init__.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     6718 2023-05-07 21:27:02.000000 pystarshade-0.1.7/pystarshade/simulate_field.py
+drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:40:34.000000 pystarshade-0.1.7/pystarshade/diffraction/
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     6660 2023-05-07 21:38:42.000000 pystarshade-0.1.7/pystarshade/diffraction/field.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-21 21:01:22.000000 pystarshade-0.1.7/pystarshade/diffraction/__init__.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     1993 2023-05-07 21:38:52.000000 pystarshade-0.1.7/pystarshade/diffraction/bluestein_fft.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     3362 2023-05-06 19:55:46.000000 pystarshade-0.1.7/pystarshade/diffraction/util.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     5931 2023-05-07 21:39:03.000000 pystarshade-0.1.7/pystarshade/diffraction/diffract.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     2404 2023-05-07 21:09:32.000000 pystarshade-0.1.7/README.md
+drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:40:34.000000 pystarshade-0.1.7/pystarshade.egg-info/
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-05-07 21:40:34.000000 pystarshade-0.1.7/pystarshade.egg-info/dependency_links.txt
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)       12 2023-05-07 21:40:34.000000 pystarshade-0.1.7/pystarshade.egg-info/top_level.txt
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)      737 2023-05-07 21:40:34.000000 pystarshade-0.1.7/pystarshade.egg-info/PKG-INFO
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)       12 2023-05-07 21:40:34.000000 pystarshade-0.1.7/pystarshade.egg-info/requires.txt
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)      495 2023-05-07 21:40:34.000000 pystarshade-0.1.7/pystarshade.egg-info/SOURCES.txt
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)      869 2023-05-07 21:39:58.000000 pystarshade-0.1.7/setup.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)      737 2023-05-07 21:40:34.000000 pystarshade-0.1.7/PKG-INFO
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)       38 2023-05-07 21:40:34.000000 pystarshade-0.1.7/setup.cfg
```

### Comparing `pystarshade-0.1.6/pystarshade/apodization/apodize.py` & `pystarshade-0.1.7/pystarshade/apodization/apodize.py`

 * *Files identical despite different names*

### Comparing `pystarshade-0.1.6/pystarshade/simulate_field.py` & `pystarshade-0.1.7/pystarshade/simulate_field.py`

 * *Files identical despite different names*

### Comparing `pystarshade-0.1.6/pystarshade/diffraction/field.py` & `pystarshade-0.1.7/pystarshade/diffraction/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .diffraction.util import *
-from .diffraction.bluestein_fft import zoom_fft_2d_mod
+from .util import *
+from .bluestein_fft import zoom_fft_2d_mod
 import numpy as np
 
 class SourceField:
     """
     This class returns far-field diffraction for an N_s x N_s source-field, calculated via a Bluestein FFT
     
     Attributes:
```

### Comparing `pystarshade-0.1.6/pystarshade/diffraction/bluestein_fft.py` & `pystarshade-0.1.7/pystarshade/diffraction/bluestein_fft.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from .diffraction.util import trunc_2d
+from .util import trunc_2d
 
 def zoom_fft_2d_mod(x, N_x, N_out, Z_pad):
     """
     MODIFIED VERSION: computes the Bluestein FFT on fftshift(x) (without explicitly shifting x).
     Compute a zoomed 2D FFT using the Bluestein algorithm. 
     The input x is centered. 
     Args:
```

### Comparing `pystarshade-0.1.6/pystarshade/diffraction/util.py` & `pystarshade-0.1.7/pystarshade/diffraction/util.py`

 * *Files identical despite different names*

### Comparing `pystarshade-0.1.6/pystarshade/diffraction/diffract.py` & `pystarshade-0.1.7/pystarshade/diffraction/diffract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
-from .diffraction.bluestein_fft import zoom_fft_2d_mod, zoom_fft_2d
-from .diffraction.util import *
+from .bluestein_fft import zoom_fft_2d_mod, zoom_fft_2d
+from .util import *
 
 class Fresnel:
     def __init__(self, d_x, N_in, z, wavelength):
         self.d_x = d_x
         self.N_in = N_in
         self.z = z
         self.wavelength = wavelength
```

### Comparing `pystarshade-0.1.6/README.md` & `pystarshade-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pystarshade-0.1.6/pystarshade.egg-info/PKG-INFO` & `pystarshade-0.1.7/pystarshade.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystarshade
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python package for end-to-end starshade simulation
 Home-page: https://github.com/xiaziyna/PyStarshade
 Author: Jamila Taaki
 Author-email: xiaziyna@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pystarshade-0.1.6/setup.py` & `pystarshade-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pystarshade",
-    version="0.1.6",
+    version="0.1.7",
     description="A python package for end-to-end starshade simulation",
     author="Jamila Taaki",
     author_email="xiaziyna@gmail.com",
     url="https://github.com/xiaziyna/PyStarshade",
     packages=find_packages(),
     install_requires=[
         "numpy",
```

### Comparing `pystarshade-0.1.6/PKG-INFO` & `pystarshade-0.1.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystarshade
-Version: 0.1.6
+Version: 0.1.7
 Summary: A python package for end-to-end starshade simulation
 Home-page: https://github.com/xiaziyna/PyStarshade
 Author: Jamila Taaki
 Author-email: xiaziyna@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

