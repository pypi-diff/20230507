# Comparing `tmp/snake-opencv-0.1.0.tar.gz` & `tmp/snake-opencv-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snake-opencv-0.1.0.tar", max compression
+gzip compressed data, was "snake-opencv-0.1.1.tar", max compression
```

## Comparing `snake-opencv-0.1.0.tar` & `snake-opencv-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    11358 2023-01-28 18:04:16.471534 snake-opencv-0.1.0/LICENSE
--rw-r--r--   0        0        0      363 2023-01-28 23:51:23.853941 snake-opencv-0.1.0/README.md
--rw-r--r--   0        0        0      556 2023-01-28 18:06:01.961413 snake-opencv-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      161 2023-01-29 23:56:40.336403 snake-opencv-0.1.0/snake_opencv/__init__.py
--rw-r--r--   0        0        0       21 2023-01-16 10:06:58.589904 snake-opencv-0.1.0/snake_opencv/core/__init__.py
--rw-r--r--   0        0        0    24344 2023-01-16 10:05:05.937027 snake-opencv-0.1.0/snake_opencv/core/const.py
--rw-r--r--   0        0        0       44 2023-01-28 20:13:58.958664 snake-opencv-0.1.0/snake_opencv/dnn/__init__.py
--rw-r--r--   0        0        0     3607 2023-01-29 23:41:34.770501 snake-opencv-0.1.0/snake_opencv/dnn/binding.py
--rw-r--r--   0        0        0     1379 2023-01-28 20:36:18.788127 snake-opencv-0.1.0/snake_opencv/dnn/const.py
--rw-r--r--   0        0        0       44 2023-01-16 09:20:16.213259 snake-opencv-0.1.0/snake_opencv/highgui/__init__.py
--rw-r--r--   0        0        0     4949 2023-01-29 23:43:31.524754 snake-opencv-0.1.0/snake_opencv/highgui/binding.py
--rw-r--r--   0        0        0     2912 2023-01-16 09:17:03.779177 snake-opencv-0.1.0/snake_opencv/highgui/const.py
--rw-r--r--   0        0        0       44 2023-01-16 09:19:42.188926 snake-opencv-0.1.0/snake_opencv/imgcodecs/__init__.py
--rw-r--r--   0        0        0     5211 2023-01-28 19:04:32.764488 snake-opencv-0.1.0/snake_opencv/imgcodecs/binding.py
--rw-r--r--   0        0        0     1496 2023-01-16 09:19:46.836972 snake-opencv-0.1.0/snake_opencv/imgcodecs/const.py
--rw-r--r--   0        0        0       44 2023-01-16 09:23:40.099004 snake-opencv-0.1.0/snake_opencv/imgproc/__init__.py
--rw-r--r--   0        0        0    27593 2023-01-28 22:48:45.559226 snake-opencv-0.1.0/snake_opencv/imgproc/binding.py
--rw-r--r--   0        0        0    35343 2023-01-16 09:21:53.794143 snake-opencv-0.1.0/snake_opencv/imgproc/const.py
--rw-r--r--   0        0        0       44 2023-01-29 23:56:52.516276 snake-opencv-0.1.0/snake_opencv/photo/__init__.py
--rw-r--r--   0        0        0     3620 2023-01-30 00:14:06.457314 snake-opencv-0.1.0/snake_opencv/photo/binding.py
--rw-r--r--   0        0        0      854 2023-01-29 00:04:59.607188 snake-opencv-0.1.0/snake_opencv/photo/const.py
--rw-r--r--   0        0        0       44 2023-01-16 09:26:22.996162 snake-opencv-0.1.0/snake_opencv/videoio/__init__.py
--rw-r--r--   0        0        0     7240 2023-01-28 23:53:22.873202 snake-opencv-0.1.0/snake_opencv/videoio/binding.py
--rw-r--r--   0        0        0    29523 2023-01-16 09:25:09.583662 snake-opencv-0.1.0/snake_opencv/videoio/const.py
--rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 snake-opencv-0.1.0/setup.py
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 snake-opencv-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-05 19:37:45.899387 snake-opencv-0.1.1/LICENSE
+-rw-r--r--   0        0        0      460 2023-05-05 22:17:27.044555 snake-opencv-0.1.1/README.md
+-rw-r--r--   0        0        0      686 2023-05-05 22:01:43.402463 snake-opencv-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      161 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-05 22:47:28.939893 snake-opencv-0.1.1/snake_opencv/core/__init__.py
+-rw-r--r--   0        0        0    12427 2023-05-06 23:46:48.811339 snake-opencv-0.1.1/snake_opencv/core/binding.py
+-rw-r--r--   0        0        0    24344 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/core/const.py
+-rw-r--r--   0        0        0       44 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/dnn/__init__.py
+-rw-r--r--   0        0        0     3607 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/dnn/binding.py
+-rw-r--r--   0        0        0     1379 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/dnn/const.py
+-rw-r--r--   0        0        0       44 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/highgui/__init__.py
+-rw-r--r--   0        0        0     4949 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/highgui/binding.py
+-rw-r--r--   0        0        0     2912 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/highgui/const.py
+-rw-r--r--   0        0        0       44 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/imgcodecs/__init__.py
+-rw-r--r--   0        0        0     5211 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/imgcodecs/binding.py
+-rw-r--r--   0        0        0     1496 2023-05-05 19:37:45.903386 snake-opencv-0.1.1/snake_opencv/imgcodecs/const.py
+-rw-r--r--   0        0        0       44 2023-05-05 19:37:45.907386 snake-opencv-0.1.1/snake_opencv/imgproc/__init__.py
+-rw-r--r--   0        0        0    34260 2023-05-06 23:14:06.167539 snake-opencv-0.1.1/snake_opencv/imgproc/binding.py
+-rw-r--r--   0        0        0    35343 2023-05-05 19:37:45.907386 snake-opencv-0.1.1/snake_opencv/imgproc/const.py
+-rw-r--r--   0        0        0       44 2023-05-05 19:37:45.907386 snake-opencv-0.1.1/snake_opencv/photo/__init__.py
+-rw-r--r--   0        0        0     3620 2023-05-05 19:37:45.907386 snake-opencv-0.1.1/snake_opencv/photo/binding.py
+-rw-r--r--   0        0        0      854 2023-05-05 19:37:45.907386 snake-opencv-0.1.1/snake_opencv/photo/const.py
+-rw-r--r--   0        0        0       44 2023-05-05 19:37:45.907386 snake-opencv-0.1.1/snake_opencv/videoio/__init__.py
+-rw-r--r--   0        0        0     7240 2023-05-05 19:37:45.907386 snake-opencv-0.1.1/snake_opencv/videoio/binding.py
+-rw-r--r--   0        0        0    29523 2023-05-05 19:37:45.907386 snake-opencv-0.1.1/snake_opencv/videoio/const.py
+-rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 snake-opencv-0.1.1/setup.py
+-rw-r--r--   0        0        0     1143 1970-01-01 00:00:00.000000 snake-opencv-0.1.1/PKG-INFO
```

### Comparing `snake-opencv-0.1.0/LICENSE` & `snake-opencv-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.0/pyproject.toml` & `snake-opencv-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 [tool.poetry]
 name = "snake-opencv"
-version = "0.1.0"
+version = "0.1.1"
+repository = "https://github.com/cospectrum/snake-opencv"
 description = "Snake case opencv with type annotations"
 license = "Apache-2.0"
 authors = ["cospectrum <severinalexeyv@gmail.com>"]
 readme = "README.md"
 packages = [{include = "snake_opencv"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 opencv-python = "^4.0"
+typing-extensions = "^4.5.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^0.991"
 flake8 = "^6.0.0"
 pytest = "^7.2.0"
+pre-commit = "^3.3.1"
+pyright = "^1.1.306"
 
 [tool.mypy]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `snake-opencv-0.1.0/snake_opencv/core/const.py` & `snake-opencv-0.1.1/snake_opencv/core/const.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.0/snake_opencv/dnn/binding.py` & `snake-opencv-0.1.1/snake_opencv/dnn/binding.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.0/snake_opencv/dnn/const.py` & `snake-opencv-0.1.1/snake_opencv/dnn/const.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.0/snake_opencv/highgui/binding.py` & `snake-opencv-0.1.1/snake_opencv/highgui/binding.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.0/snake_opencv/highgui/const.py` & `snake-opencv-0.1.1/snake_opencv/highgui/const.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.0/snake_opencv/imgcodecs/binding.py` & `snake-opencv-0.1.1/snake_opencv/imgcodecs/binding.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.0/snake_opencv/imgcodecs/const.py` & `snake-opencv-0.1.1/snake_opencv/imgcodecs/const.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.0/snake_opencv/imgproc/binding.py` & `snake-opencv-0.1.1/snake_opencv/imgproc/binding.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import cv2
 import numpy as np
 
 from typing import Tuple, Optional, List, Literal, Union
+from typing_extensions import TypeAlias
+
 
 from .const import INTER_LINEAR
 from ..core import (
     BORDER_CONSTANT,
     BORDER_DEFAULT,
     CV_PI,
+    CV_32S,
     DECOMP_LU,
 )
 
 
 __all__ = [
     'resize',
     'cvt_color',
@@ -28,14 +31,17 @@
     'hough_lines_p',
     'min_area_rect',
     'box_points',
     'get_perspective_transform',
     'warp_perspective',
     'laplacian',
     'threshold',
+    'connected_components_with_stats',
+    'connected_components',
+    'match_template',
 ]
 
 
 LineType = Literal[-1, 4, 8, 16]
 
 
 Width = int
@@ -366,15 +372,15 @@
         edges=edges,
         apertureSize=aperture_size,
         L2gradient=l2gradient,
     )
 
 
 Contours = Tuple[np.ndarray, ...]
-Hierarchy = np.ndarray
+Hierarchy: TypeAlias = np.ndarray
 
 
 def find_contours(
     image: np.ndarray,
     mode: int,
     method: int,
     offset: Optional[Tuple[X, Y]] = None,
@@ -802,7 +808,155 @@
     return cv2.threshold(
         src,
         thresh,
         maxval,
         type=type,
         dst=dst,
     )
+
+
+Labels: TypeAlias = np.ndarray
+Stats: TypeAlias = np.ndarray
+Centroids: TypeAlias = np.ndarray
+
+
+def connected_components_with_stats(
+    image: np.ndarray,
+    labels: Optional[np.ndarray] = None,
+    stats: Optional[np.ndarray] = None,
+    centroids: Optional[np.ndarray] = None,
+    connectivity: Literal[4, 8] = 8,
+    ltype: int = CV_32S,
+) -> Tuple[int, Labels, Stats, Centroids]:
+    """computes the connected components labeled image of boolean image and
+    also produces a statistics output for each label
+
+    image with 4 or 8 way connectivity - returns N, the total number of labels
+    [0, N-1] where 0 represents the background label. ltype specifies the
+    output label image type, an important consideration based on the total
+    number of labels or alternatively the total number of pixels in the source
+    image. ccltype specifies the connected components labeling algorithm to
+    use, currently Bolelli (Spaghetti) Bolelli2019, Grana (BBDT) Grana2010 and
+    Wu’s (SAUF) Wu2009 algorithms are supported, see the
+    #ConnectedComponentsAlgorithmsTypes for details. Note that SAUF algorithm
+    forces a row major ordering of labels while Spaghetti and BBDT do not. This
+    function uses parallel version of the algorithms (statistics included) if
+    at least one allowed parallel framework is enabled and if the rows of the
+    image are at least twice the number returned by #getNumberOfCPUs.
+
+    Args:
+        image: the 8-bit single-channel image to be labeled
+        labels: destination labeled image
+        stats:
+            statistics output for each label, including the background label.
+            Statistics are accessed via stats(label, COLUMN) where COLUMN is
+            one of #ConnectedComponentsTypes, selecting the statistic. The data
+            type is CV_32S.
+        centroids:
+            centroid output for each label, including the background label.
+            Centroids are accessed via centroids(label, 0) for x and
+            centroids(label, 1) for y. The data type CV_64F.
+        connectivity: 8 or 4 for 8-way or 4-way connectivity respectively
+        ltype:
+            output image label type. Currently CV_32S and CV_16U are supported.
+    """
+    return cv2.connectedComponentsWithStats(
+        image,
+        labels=labels,
+        stats=stats,
+        centroids=centroids,
+        connectivity=connectivity,
+        ltype=ltype,
+    )
+
+
+def connected_components(
+    image: np.ndarray,
+    labels: Optional[np.ndarray] = None,
+    connectivity: Literal[4, 8] = 8,
+    ltype: int = CV_32S,
+) -> Tuple[int, Labels]:
+    """computes the connected components labeled image of boolean image
+
+    image with 4 or 8 way connectivity - returns N, the total number of labels
+    [0, N-1] where 0 represents the background label. ltype specifies the
+    output label image type, an important consideration based on the total
+    number of labels or alternatively the total number of pixels in the source
+    image. ccltype specifies the connected components labeling algorithm to
+    use, currently Bolelli (Spaghetti) Bolelli2019, Grana (BBDT) Grana2010 and
+    Wu’s (SAUF) Wu2009 algorithms are supported, see the
+    #ConnectedComponentsAlgorithmsTypes for details. Note that SAUF algorithm
+    forces a row major ordering of labels while Spaghetti and BBDT do not.
+    This function uses parallel version of the algorithms if at least one
+    allowed parallel framework is enabled and if the rows of the image are at
+    least twice the number returned by #getNumberOfCPUs.
+
+    Args:
+        image: the 8-bit single-channel image to be labeled
+        labels: destination labeled image
+        connectivity: 8 or 4 for 8-way or 4-way connectivity respectively
+        ltype:
+            output image label type. Currently CV_32S and CV_16U are supported.
+    """
+    return cv2.connectedComponents(
+        image,
+        labels=labels,
+        connectivity=connectivity,
+        ltype=ltype,
+    )
+
+
+def match_template(
+    image: np.ndarray,
+    templ: np.ndarray,
+    method: int,
+    result: Optional[np.ndarray] = None,
+    mask: Optional[np.ndarray] = None,
+) -> np.ndarray:
+    """Compares a template against overlapped image regions.
+
+    The function slides through image , compares the overlapped patches of size
+    w×h against templ using the specified method and stores the comparison
+    results in result . TemplateMatchModes describes the formulae for the
+    available comparison methods ( I denotes image, T template, R result, M the
+    optional mask ). The summation is done over template and/or the image
+    patch: x′=0...w−1,y′=0...h−1
+
+    After the function finishes the comparison, the best matches can be found
+    as global minimums (when TM_SQDIFF was used) or maximums (when TM_CCORR or
+    TM_CCOEFF was used) using the minMaxLoc function. In case of a color image,
+    template summation in the numerator and each sum in the denominator is done
+    over all of the channels and separate mean values are used for each
+    channel. That is, the function can take a color template and a color image.
+    The result will still be a single-channel image, which is easier to
+    analyze.
+
+    Args:
+        image:
+            Image where the search is running. It must be 8-bit or 32-bit
+            floating-point.
+        templ:
+            Searched template. It must be not greater than the source image and
+            have the same data type.
+        result:
+            Map of comparison results. It must be single-channel 32-bit
+            floating-point. If image is W×H and templ is w×h, then result is
+            (W−w+1)×(H−h+1).
+        method:
+            Parameter specifying the comparison method, see TemplateMatchModes
+        mask:
+            Optional mask. It must have the same size as templ. It must either
+            have the same number of channels as template or only one channel,
+            which is then used for all template and image channels. If the data
+            type is CV_8U, the mask is interpreted as a binary mask, meaning
+            only elements where mask is nonzero are used and are kept unchanged
+            independent of the actual mask value (weight equals 1). For data
+            tpye CV_32F, the mask values are used as weights. The exact
+            formulas are documented in TemplateMatchModes.
+    """
+    return cv2.matchTemplate(
+        image,
+        templ=templ,
+        method=method,
+        result=result,
+        mask=mask,
+    )
```

### Comparing `snake-opencv-0.1.0/snake_opencv/imgproc/const.py` & `snake-opencv-0.1.1/snake_opencv/imgproc/const.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.0/snake_opencv/photo/binding.py` & `snake-opencv-0.1.1/snake_opencv/photo/binding.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.0/snake_opencv/photo/const.py` & `snake-opencv-0.1.1/snake_opencv/photo/const.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.0/snake_opencv/videoio/binding.py` & `snake-opencv-0.1.1/snake_opencv/videoio/binding.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.0/snake_opencv/videoio/const.py` & `snake-opencv-0.1.1/snake_opencv/videoio/const.py`

 * *Files identical despite different names*

### Comparing `snake-opencv-0.1.0/PKG-INFO` & `snake-opencv-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 Metadata-Version: 2.1
 Name: snake-opencv
-Version: 0.1.0
+Version: 0.1.1
 Summary: Snake case opencv with type annotations
+Home-page: https://github.com/cospectrum/snake-opencv
 License: Apache-2.0
 Author: cospectrum
 Author-email: severinalexeyv@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: opencv-python (>=4.0,<5.0)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Project-URL: Repository, https://github.com/cospectrum/snake-opencv
 Description-Content-Type: text/markdown
 
 # Snake-OpenCV
 Snake case OpenCV with type annotations for Python.
 
-Note: Still in early development
+Note: still in early development
 
 ## Install
 
+Stable version
 ```sh
-git clone https://github.com/cospectrum/snake-opencv.git
-cd snake-opencv && pip install .
+pip install snake-opencv
+```
+
+Latest version from git
+```sh
+pip install git+https://github.com/cospectrum/snake-opencv.git
 ```
 
 ## Usage
 ```py
 import snake_opencv as cv
 
+path = '...'
 image = cv.imread(path)
-image = cv.cvt_color(image, cv.COLOR_BGR2RGB)
+assert image is not None
+gray_image = cv.cvt_color(image, cv.COLOR_BGR2GRAY)
 
-cv.imshow(window_name, image) 
+cv.imshow(window_name, gray_image) 
 ```
```

