# Comparing `tmp/katalytic-images-0.3.0.tar.gz` & `tmp/katalytic-images-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-images-0.3.0.tar", last modified: Thu May  4 17:58:36 2023, max compression
+gzip compressed data, was "katalytic-images-0.4.0.tar", last modified: Sun May  7 10:08:38 2023, max compression
```

## Comparing `katalytic-images-0.3.0.tar` & `katalytic-images-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic-images-0.3.0/.coveragerc
--rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic-images-0.3.0/.gitignore
--rw-r--r--   0        0        0     3324 2023-04-30 14:15:39.110597 katalytic-images-0.3.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     1912 2023-05-04 17:58:14.314350 katalytic-images-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic-images-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2130 2023-04-30 14:20:54.475497 katalytic-images-0.3.0/README.md
--rw-r--r--   0        0        0     1551 2023-05-04 17:58:14.298350 katalytic-images-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7582 2023-05-02 05:00:49.687540 katalytic-images-0.3.0/src/katalytic/images.py
--rw-r--r--   0        0        0    13039 2023-05-01 19:23:22.988107 katalytic-images-0.3.0/tests/test_images.py
--rw-r--r--   0        0        0     3608 1970-01-01 00:00:00.000000 katalytic-images-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic-images-0.4.0/.coveragerc
+-rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic-images-0.4.0/.gitignore
+-rw-r--r--   0        0        0     3308 2023-05-05 03:58:55.053635 katalytic-images-0.4.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2111 2023-05-07 10:08:33.713105 katalytic-images-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic-images-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     2130 2023-04-30 14:20:54.475497 katalytic-images-0.4.0/README.md
+-rw-r--r--   0        0        0     1549 2023-05-07 10:08:33.713105 katalytic-images-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    10015 2023-05-07 10:03:19.751524 katalytic-images-0.4.0/src/katalytic/images.py
+-rw-r--r--   0        0        0    14584 2023-05-07 10:06:02.709954 katalytic-images-0.4.0/tests/test_images.py
+-rw-r--r--   0        0        0     3606 1970-01-01 00:00:00.000000 katalytic-images-0.4.0/PKG-INFO
```

### Comparing `katalytic-images-0.3.0/.gitignore` & `katalytic-images-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.3.0/.gitlab-ci.yml` & `katalytic-images-0.4.0/.gitlab-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 include:
 - template: Security/SAST.gitlab-ci.yml
 
-image: python:3.9
+image: python:3.7
 
 stages:
   - coverage
   - test
   - security
   - release
 
 variables:
-  TOX_ENV: py39
   PIP_DISABLE_PIP_VERSION_CHECK: "1"
   PIP_NO_CACHE_DIR: "off"
 
 coverage:
-  image: python:3.6
+  image: python:3.7
   stage: coverage
   script:
     - apt-get update -qq
     - apt-get install -y libgl1-mesa-glx
     - pip install --upgrade pip
     - pip install -e .[dev]
     - python -m pytest --cov-fail-under=100 --cov=src --cov-report=xml --cov-report=term-missing || { echo "Tests failed. Exiting ..." && exit 1; }
```

### Comparing `katalytic-images-0.3.0/CHANGELOG.md` & `katalytic-images-0.4.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.4.0 (2023-05-07)
+### feat
+- [[`dca7f3e`](https://gitlab.com/katalytic/katalytic-images/commit/dca7f3eb1ee463393fa8c872fcebe8f101b5f73c)] add create_{rectangle,circle,line,text,mask,polylines}
+
+
 ## 0.3.0 (2023-05-04)
 ### feat
 - [[`d824d98`](https://gitlab.com/katalytic/katalytic-images/commit/d824d989ce58efd8ffe644e2527d02952a230a92)] **draw:** add more shape types
 - [[`62be07d`](https://gitlab.com/katalytic/katalytic-images/commit/62be07dfbc5aca96d490732eaa421d6083c5d663)] **draw:** implement 'mask' and 'polylines' shape types
 
 
 ## 0.2.2 (2023-05-01)
```

### Comparing `katalytic-images-0.3.0/LICENSE.txt` & `katalytic-images-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.3.0/README.md` & `katalytic-images-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-images-0.3.0/pyproject.toml` & `katalytic-images-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-images"
-version = "0.3.0"
+version = "0.4.0"
 description = "This plugin adds utilities for working with images and videos to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -24,15 +24,15 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Utilities",
 ]
 authors = [{name="Valentin Neagu", email="vali19th@protonmail.com"}]
 
 requires-python = ">=3.6"
 dependencies = [
-    "katalytic-checks>=0.1.1",
+    "katalytic-data>=0.8.0",
     "katalytic-files>=0.3.0",
     "katalytic-pkg>=0.2.0",
     "numpy>=1.14",
     "opencv-python>=4.0.0",
     "pillow>=8.4.0",
 ]
```

### Comparing `katalytic-images-0.3.0/src/katalytic/images.py` & `katalytic-images-0.4.0/src/katalytic/images.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     ndarray as __np_ndarray
 )
 
 import PIL.Image
 __PIL_Image_open = PIL.Image.open
 __PIL_Image_Image = PIL.Image.Image
 
-from katalytic.checks import is_iterable, is_number, is_sequence
+from katalytic.data.checks import is_iterable, is_number, is_sequence
 from katalytic.pkg import get_version, mark
 
 __version__, __version_info__ = get_version(__name__)
 
 
 def bhwc(arr):
     if arr.shape == (0,):
@@ -59,14 +59,104 @@
 
     if return_PIL:
         return PIL.Image.fromarray(img)
     else:
         return img
 
 
+def create_line(p1, p2, color, *, thickness=3, **kwargs):
+    return {
+        'type': 'line',
+        'p1': tuple(map(int, p1)),
+        'p2': tuple(map(int, p2)),
+        'color': color,
+        'thickness': thickness,
+        **kwargs
+    }
+
+
+def create_circle(center, radius, color, *, thickness=3, **kwargs):
+    return {
+        'type': 'circle',
+        'center': center,
+        'radius': radius,
+        'color': color,
+        'thickness': thickness,
+        **kwargs
+    }
+
+
+def create_rectangle(p1, p2, color, *, thickness=3, **kwargs):
+    return {
+        'type': 'rectangle',
+        'p1': p1,#tuple(map(int, p1)),
+        'p2': tuple(map(int, p2)),
+        'color': color,
+        'thickness': thickness,
+        **kwargs
+    }
+
+
+def create_text(text, origin, color, *, font=cv2.FONT_HERSHEY_SIMPLEX, scale=1.25, thickness=3, bg=None, bg_pad=None, **kwargs):
+    shape = {
+        'type': 'text',
+        'text': text,
+        'origin': tuple(map(int, origin)),
+        'color': color,
+        'font': font,
+        'font_scale': scale,
+        'thickness': thickness,
+        **kwargs
+    }
+
+    if bg is None:
+        if bg_pad is None:
+            return shape
+        else:
+            # bg_pad is set to None by default instead of 5 ot alert the user
+            # when he sets <bg_pad> and forgets <bg>.
+            # Otherwise the mistake would be ignored silently
+            raise ValueError('<bg> is None, even though <bg_pad> is set to a value')
+
+    if bg_pad is None:
+        bg_pad = [5] * 4
+    elif is_number(bg_pad):
+        bg_pad = [bg_pad] * 4
+    elif is_sequence(bg_pad):
+        if len(bg_pad) == 2:
+            bg_pad = [*bg_pad, *bg_pad]
+        elif len(bg_pad) != 4:
+            raise ValueError(f'<bg_pad> expects None, a number or a sequence like (horizontal, vertical) or (left, top, right, bottom). Got a sequence of length {len(bg_pad)}')
+    else:
+        raise TypeError(f'type(bg_pad) = {type(bg_pad)!r}')
+
+    shape['background'] = {'color': bg, 'pad': bg_pad}
+    return shape
+
+
+def create_polylines(pts, color, *, thickness=3, is_closed=True, **kwargs):
+    return {
+        'type': 'polylines',
+        'pts': pts,
+        'color': color,
+        'thickness': thickness,
+        'is_closed': is_closed,
+        **kwargs
+    }
+
+
+def create_mask(pts, color, **kwargs):
+    return {
+        'type': 'mask',
+        'pts': pts,
+        'color': color,
+        **kwargs
+    }
+
+
 def draw(image, data):
     new_image = image.copy()
     draw_inplace(new_image, data)
     return new_image
 
 
 def draw_inplace(image, data):
```

### Comparing `katalytic-images-0.3.0/tests/test_images.py` & `katalytic-images-0.4.0/tests/test_images.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import copy
 from pathlib import Path
 
+import cv2
 import numpy as np
 import PIL.Image
 import pytest
 from PIL import Image
 
 from katalytic.data import all_types_besides
 from katalytic.files import get_unique_path, load, save
-from katalytic.images import bhwc, convert_image, draw, hw, hwc, are_arrays_equal, load_image, save_image
+from katalytic.images import bhwc, convert_image, create_circle, create_line, create_mask, create_polylines, create_rectangle, create_text, draw, hw, hwc, are_arrays_equal, load_image, save_image
 
 
 def _create_RGB(dtype=np.uint8):
     return np.array([
         [[255, 0, 0], [0, 255, 0], [0, 0, 255]],        # RGB
         [[0, 255, 255], [255, 0, 255], [255, 255, 0]],  # CMY
         [[0, 0, 255], [0, 255, 0], [255, 0, 0]],        # BGR
@@ -97,21 +98,21 @@
 
     def test_returns_numpy_if_numpy(self):
         img = _create_RGB()
         img2 = convert_image(img, 'RGB', 'BGR')
         assert isinstance(img2, np.ndarray)
 
     def test_returns_numpy_if_str(self):
-        path = get_unique_path('/tmp/{}.png')
+        path = get_unique_path('{}.png')
         save_image(_create_RGB(), path)
         img2 = convert_image(path, 'RGB', 'BGR')
         assert isinstance(img2, np.ndarray)
 
     def test_returns_numpy_if_Path(self):
-        path = Path(get_unique_path('/tmp/{}.png'))
+        path = Path(get_unique_path('{}.png'))
         save_image(_create_RGB(), path)
         img2 = convert_image(path, 'RGB', 'BGR')
         assert isinstance(img2, np.ndarray)
 
     @pytest.mark.xfail(reason='Not implemented')
     def test_convert_binary(self):
         img = np.array([[[0, 0, 0], [255, 255, 255]]])
@@ -144,27 +145,33 @@
     def test_wrong_type(self, wrong_type):
         with pytest.raises(TypeError):
             draw(np.zeros((5, 5)), wrong_type)
 
     def test_draws_on_a_copy(self):
         img = np.zeros((5, 5, 3), dtype=np.uint8)
         img_copy = img.copy()
-        img = draw(img, {
-            'type': 'line',
-            'pt1': (0, 0),
-            'pt2': (0, 3),
-            'color': (0, 255, 0),
-            'thickness': 1,
-        })
-        assert not are_arrays_equal(img, img_copy)
+        shapes = [
+            create_line((0,0), (0,3), (0, 255, 0), thickness=1),
+            create_rectangle((1,1), (3,3), (255, 0, 0), thickness=-1),
+            create_circle((4,4), 2, (0, 0, 255))
+        ]
+
+        img = draw(img, shapes)
+        assert (img == [255, 0, 0]).all(axis=2).any()
+        assert (img == [0, 255, 0]).all(axis=2).any()
+        assert (img == [0, 0, 255]).all(axis=2).any()
+
+        assert not (img_copy == [255, 0, 0]).all(axis=2).any()
+        assert not (img_copy == [0, 255, 0]).all(axis=2).any()
+        assert not (img_copy == [0, 0, 255]).all(axis=2).any()
 
     def test_maintains_order_if_sequence(self):
         data = [
-            {'type': 'line', 'pt1': (0, 0), 'pt2': (0, 2), 'color': (0, 255, 0), 'thickness': 1},
-            {'type': 'line', 'pt1': (0, 1), 'pt2': (0, 3), 'color': (0, 0, 255), 'thickness': 1},
+            create_line((0,0), (0,2), (0, 255, 0), thickness=1),
+            create_line((0,1), (0,3), (0, 0, 255), thickness=1),
         ]
         expected = np.array([
             [[0, 255, 0]],
             [[0, 0, 255]],
             [[0, 0, 255]],
             [[0, 0, 255]],
         ])
@@ -180,56 +187,82 @@
             [[0, 0, 255]],
         ])
 
         img = np.zeros((4, 1, 3), dtype=np.uint8)
         img = draw(img, data[::-1])
         assert are_arrays_equal(img, expected)
 
-    def test_uses_defaults(self):
-        img = np.zeros((5, 5), dtype=np.uint8)
-        img = draw(img, {'type': 'rectangle', 'p1': (0, 0), 'p2': (3, 3), 'color': 1})
-
-        expected = np.zeros((5, 5), dtype=np.uint8)
-        expected[0:4, 0:4] = 1
-        assert are_arrays_equal(img, expected)
-
     def test_text_with_background_color(self):
         original = 255 * np.ones((100, 100, 3), dtype=np.uint8)
+        shape = create_text('hello', (0, 50), (0, 255, 0), bg=(255, 0, 255), bg_pad=(5, 10, 15, 20))
+
+        processed = draw(original, shape)
+        assert not are_arrays_equal(original, processed)
+        assert (processed == (0, 255, 0)).any()
+        assert (processed == (255, 0, 255)).any()
+
+    def test_text_with_pad_but_without_bg_color(self):
+        with pytest.raises(ValueError):
+            create_text('hello', (0, 50), (0, 255, 0), bg_pad=(5, 10, 15, 20))
+
+    @pytest.mark.parametrize('pad', [(1,2,3), (1,2,3,4,5)])
+    def test_text_with_invalid_pad_values(self, pad):
+        with pytest.raises(ValueError):
+            create_text('hello', (0, 50), (0, 255, 0), bg=(0,0,255), bg_pad=pad)
 
-        text_color = (0, 255, 0)
-        bg_color = (255, 0, 255)
-        shape = {
+    @pytest.mark.parametrize('pad', all_types_besides(['none', 'numbers', 'sequences']))
+    def test_text_with_invalid_pad_types(self, pad):
+        with pytest.raises(TypeError):
+            create_text('hello', (0, 50), (0, 255, 0), bg=(0,0,255), bg_pad=pad)
+
+    @pytest.mark.parametrize('input_pad, expected_pad', [
+        (None, [5,5,5,5]),
+        (1, [1,1,1,1]),
+        ((1,2), [1,2,1,2]),
+        ((1,2,3,4), (1,2,3,4)),
+    ])
+    def test_text_with_different_pad_values(self, input_pad, expected_pad):
+        shape = create_text('hello', (0, 50), (0, 255, 0), bg=(0,0,255), bg_pad=input_pad)
+        assert shape == {
             'type': 'text',
-            'text': "21",
-            'color': text_color,
+            'text': 'hello',
+            'origin': (0, 50),
+            'color': (0, 255, 0),
+            'font': cv2.FONT_HERSHEY_SIMPLEX,
+            'font_scale': 1.25,
+            'thickness': 3,
             'background': {
-                'color': bg_color,
-                'pad': (5, 10, 15, 20),
+                'color': (0, 0, 255),
+                'pad': expected_pad
             },
-            'origin': (0, 50),
         }
 
-        processed = draw(original, shape)
-        assert not are_arrays_equal(original, processed)
-        assert (processed == text_color).any()
-        assert (processed == bg_color).any()
+    def test_text_without_bg_color_or_pad(self):
+        shape = create_text('hello', (0, 50), (0, 255, 0))
+        assert shape == {
+            'type': 'text',
+            'text': 'hello',
+            'origin': (0, 50),
+            'color': (0, 255, 0),
+            'font': cv2.FONT_HERSHEY_SIMPLEX,
+            'font_scale': 1.25,
+            'thickness': 3,
+        }
 
     @pytest.mark.parametrize('shape', [
-        {'type': 'mask', 'pts': [(100,100), (250,250), (250,100), (150,200)]},
-        {'type': 'mask', 'pts': [[(100,100), (250,250), (250,100), (150,200)], ((0,0), (0,1), (1,0), (2,0))]},
-        {'type': 'mask', 'pts': np.array([[(100,100), (250,250), (250,100), (150,200)]])},
-        {'type': 'mask', 'pts': np.array([[(100,100), (250,250), (250,100), (150,200)]], dtype=np.uint8)},
-        {'type': 'polylines', 'pts': [(100,100), (250,250), (250,100), (150,200)]},
-        {'type': 'polylines', 'pts': [[(100,100), (250,250), (250,100), (150,200)], ((0,0), (0,1), (1,0), (2,0))]},
-        {'type': 'polylines', 'pts': np.array([[(100,100), (250,250), (250,100), (150,200)]])},
-        {'type': 'polylines', 'pts': np.array([[(100,100), (250,250), (250,100), (150,200)]], dtype=np.uint8)},
+        create_mask([(100,100), (250,250), (250,100), (150,200)], (0, 255, 0)),
+        create_mask([[(100,100), (250,250), (250,100), (150,200)], ((0,0), (0,1), (1,0), (2,0))], (0, 255, 0)),
+        create_mask(np.array([[(100,100), (250,250), (250,100), (150,200)]]), (0, 255, 0)),
+        create_mask(np.array([[(100,100), (250,250), (250,100), (150,200)]], dtype=np.uint8), (0, 255, 0)),
+        create_polylines([(100,100), (250,250), (250,100), (150,200)], (0, 255, 0)),
+        create_polylines([[(100,100), (250,250), (250,100), (150,200)], ((0,0), (0,1), (1,0), (2,0))], (0, 255, 0)),
+        create_polylines(np.array([[(100,100), (250,250), (250,100), (150,200)]]), (0, 255, 0)),
+        create_polylines(np.array([[(100,100), (250,250), (250,100), (150,200)]], dtype=np.uint8), (0, 255, 0)),
     ])
     def test_masks_and_polylines(self, shape):
-        shape['color'] = (0, 255, 0)
-
         original = 255 * np.ones((1000, 1000, 3), dtype=np.uint8)
         processed = draw(original, shape)
         assert not are_arrays_equal(original, processed)
 
 
 class Test_are_arrays_equal:
     @pytest.mark.parametrize('img_1, img_2', [
@@ -255,77 +288,77 @@
             check_type=True
         )
 
 
 class Test_load_and_save:
     def test_str(self):
         image_1 = _create_RGB()
-        path = get_unique_path('/tmp/{}.png')
+        path = get_unique_path('{}.png')
         save_image(image_1, path)
         assert are_arrays_equal(image_1, load_image(path))
 
     def test_Path(self):
         image_1 = _create_RGB()
-        path = Path(get_unique_path('/tmp/{}.png'))
+        path = Path(get_unique_path('{}.png'))
         save_image(image_1, path)
         assert are_arrays_equal(image_1, load_image(path))
 
     def test_save_PIL_Image(self):
         image_1 = _create_RGB()
-        path = Path(get_unique_path('/tmp/{}.png'))
+        path = Path(get_unique_path('{}.png'))
         save_image(Image.fromarray(image_1), path)
         assert are_arrays_equal(image_1, load_image(path))
 
     def test_load_PIL_Image(self):
         image_1 = _create_RGB()
-        path = Path(get_unique_path('/tmp/{}.png'))
+        path = Path(get_unique_path('{}.png'))
         save_image(image_1, path)
         assert are_arrays_equal(image_1, load_image(Image.fromarray(image_1)))
 
     def test_load_returns_copy(self):
         img = _create_RGB()
         img_copy = load_image(img)
         img[0][0] = [255, 255, 255]
         assert not are_arrays_equal(img, img_copy)
 
     def test_path_exists_replace(self):
-        path = get_unique_path('/tmp/{}.png')
+        path = get_unique_path('{}.png')
         Path(path).touch()
 
         img = _create_RGB()
         save_image(img, path, exists='replace')
         assert are_arrays_equal(load_image(path), img)
 
     def test_save_uses_copy_file(self):
-        path = get_unique_path('/tmp/{}.png')
+        path = get_unique_path('{}.png')
         save_image(_create_RGB(), path)
 
-        path2 = get_unique_path('/tmp/{}.png')
+        path2 = get_unique_path('{}.png')
         save_image(path, path2, exists='replace')
 
         assert are_arrays_equal(load_image(path2), load_image(path))
 
     def test_path_exists_skip(self):
-        path = get_unique_path('/tmp/{}.png')
+        path = get_unique_path('{}.png')
         img = _create_RGB()
         save_image(img, path)
 
         img2 = convert_image(img, 'RGB', 'BGR')
         save_image(img2, path, exists='skip')
         assert not are_arrays_equal(load_image(path), img2)
 
     def test_path_exists_error(self):
-        path = get_unique_path('/tmp/{}.png')
+        path = get_unique_path('{}.png')
         Path(path).touch()
 
         with pytest.raises(FileExistsError):
             save_image(_create_RGB(), path, exists='error')
 
     def test_universal_load_and_save(self):
-        path = get_unique_path('/tmp/{}.png')
+        path = get_unique_path('{}.png')
         img = _create_RGB()
         save(img, path)
         assert are_arrays_equal(load(path), img)
 
     @pytest.mark.parametrize('img', [1, True, None, [], {}, (), object()])
     def test_load_raises_TypeError_for_image(self, img):
         with pytest.raises(TypeError):
@@ -340,18 +373,18 @@
     def test_save_raises_TypeError_for_path(self, path):
         with pytest.raises(TypeError):
             save_image(_create_RGB(), path)
 
     @pytest.mark.parametrize('image', [1, True, None, [], {}, (), object()])
     def test_save_raises_TypeError_for_image(self, image):
         with pytest.raises(TypeError):
-            save_image(image, get_unique_path('/tmp/{}.png'))
+            save_image(image, get_unique_path('{}.png'))
 
     @pytest.mark.parametrize('mode', ['unkonwn', '', 1, True, None, [], {}, (), object()])
     def test_save_raises_ValueError_for_mode(self, mode):
         with pytest.raises(ValueError):
-            save_image(_create_RGB(), get_unique_path('/tmp/{}.png'), mode=mode)
+            save_image(_create_RGB(), get_unique_path('{}.png'), mode=mode)
 
     @pytest.mark.parametrize('exists', ['unkonwn', '', 1, True, None, [], {}, (), object()])
     def test_save_raises_ValueError_for_exists(self, exists):
         with pytest.raises(ValueError):
-            save_image(_create_RGB(), get_unique_path('/tmp/{}.png'), exists=exists)
+            save_image(_create_RGB(), get_unique_path('{}.png'), exists=exists)
```

### Comparing `katalytic-images-0.3.0/PKG-INFO` & `katalytic-images-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-images
-Version: 0.3.0
+Version: 0.4.0
 Summary: This plugin adds utilities for working with images and videos to the katalytic namespace
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Dist: katalytic-checks>=0.1.1
+Requires-Dist: katalytic-data>=0.8.0
 Requires-Dist: katalytic-files>=0.3.0
 Requires-Dist: katalytic-pkg>=0.2.0
 Requires-Dist: numpy>=1.14
 Requires-Dist: opencv-python>=4.0.0
 Requires-Dist: pillow>=8.4.0
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
```

