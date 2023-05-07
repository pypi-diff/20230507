# Comparing `tmp/mokuro-0.1.6.tar.gz` & `tmp/mokuro-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mokuro-0.1.6.tar", last modified: Thu Dec 29 10:38:11 2022, max compression
+gzip compressed data, was "dist\mokuro-0.1.7.tar", last modified: Sun May  7 20:58:23 2023, max compression
```

## Comparing `mokuro-0.1.6.tar` & `mokuro-0.1.7.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2022-12-29 10:38:11.673886 mokuro-0.1.6/
--rw-rw-rw-   0        0        0    35823 2022-04-16 12:47:37.000000 mokuro-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      106 2022-04-24 18:07:31.000000 mokuro-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1939 2022-12-29 10:38:11.673886 mokuro-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     3389 2022-11-05 16:55:33.000000 mokuro-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2022-12-29 10:38:11.351951 mokuro-0.1.6/comic_text_detector/
--rw-rw-rw-   0        0        0    35823 2022-04-16 13:12:53.000000 mokuro-0.1.6/comic_text_detector/LICENSE
--rw-rw-rw-   0        0        0        0 2022-04-16 15:46:37.000000 mokuro-0.1.6/comic_text_detector/__init__.py
--rw-rw-rw-   0        0        0    11055 2022-11-05 10:30:05.000000 mokuro-0.1.6/comic_text_detector/basemodel.py
--rw-rw-rw-   0        0        0    11890 2022-04-16 15:52:43.000000 mokuro-0.1.6/comic_text_detector/db_dataset.py
--rw-rw-rw-   0        0        0     8925 2022-11-05 10:46:28.000000 mokuro-0.1.6/comic_text_detector/inference.py
-drwxrwxrwx   0        0        0        0 2022-12-29 10:38:11.353939 mokuro-0.1.6/comic_text_detector/models/
--rw-rw-rw-   0        0        0        0 2022-04-16 13:12:53.000000 mokuro-0.1.6/comic_text_detector/models/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-29 10:38:11.381104 mokuro-0.1.6/comic_text_detector/models/yolov5/
--rw-rw-rw-   0        0        0        0 2022-04-16 13:12:53.000000 mokuro-0.1.6/comic_text_detector/models/yolov5/__init__.py
--rw-rw-rw-   0        0        0    10796 2022-11-05 10:29:46.000000 mokuro-0.1.6/comic_text_detector/models/yolov5/common.py
--rw-rw-rw-   0        0        0    14774 2022-04-16 16:28:29.000000 mokuro-0.1.6/comic_text_detector/models/yolov5/yolo.py
--rw-rw-rw-   0        0        0    10599 2022-04-16 15:52:43.000000 mokuro-0.1.6/comic_text_detector/seg_dataset.py
--rw-rw-rw-   0        0        0    24903 2022-04-16 16:28:29.000000 mokuro-0.1.6/comic_text_detector/text_rendering.py
--rw-rw-rw-   0        0        0    10139 2022-04-16 16:28:29.000000 mokuro-0.1.6/comic_text_detector/train_db.py
--rw-rw-rw-   0        0        0     9093 2022-04-16 15:52:43.000000 mokuro-0.1.6/comic_text_detector/train_seg.py
-drwxrwxrwx   0        0        0        0 2022-12-29 10:38:11.560420 mokuro-0.1.6/comic_text_detector/utils/
--rw-rw-rw-   0        0        0        0 2022-04-23 16:34:25.000000 mokuro-0.1.6/comic_text_detector/utils/__init__.py
--rw-rw-rw-   0        0        0    28581 2022-12-29 10:31:12.000000 mokuro-0.1.6/comic_text_detector/utils/db_utils.py
--rw-rw-rw-   0        0        0     2179 2022-11-22 21:36:36.000000 mokuro-0.1.6/comic_text_detector/utils/export.py
--rw-rw-rw-   0        0        0     2472 2022-04-16 13:12:53.000000 mokuro-0.1.6/comic_text_detector/utils/general.py
--rw-rw-rw-   0        0        0     7099 2022-04-16 13:12:53.000000 mokuro-0.1.6/comic_text_detector/utils/imgproc_utils.py
--rw-rw-rw-   0        0        0     1859 2022-04-16 15:52:43.000000 mokuro-0.1.6/comic_text_detector/utils/io_utils.py
--rw-rw-rw-   0        0        0     7397 2022-04-16 15:52:43.000000 mokuro-0.1.6/comic_text_detector/utils/loss.py
--rw-rw-rw-   0        0        0    21790 2022-11-05 10:46:28.000000 mokuro-0.1.6/comic_text_detector/utils/textblock.py
--rw-rw-rw-   0        0        0    13499 2022-04-16 15:52:43.000000 mokuro-0.1.6/comic_text_detector/utils/textmask.py
--rw-rw-rw-   0        0        0     3888 2022-04-16 13:12:53.000000 mokuro-0.1.6/comic_text_detector/utils/weight_init.py
--rw-rw-rw-   0        0        0    10454 2022-04-16 13:12:53.000000 mokuro-0.1.6/comic_text_detector/utils/yolov5_utils.py
-drwxrwxrwx   0        0        0        0 2022-12-29 10:38:11.619837 mokuro-0.1.6/mokuro/
--rw-rw-rw-   0        0        0      128 2022-12-29 10:37:05.000000 mokuro-0.1.6/mokuro/__init__.py
--rw-rw-rw-   0        0        0      124 2022-04-24 16:27:29.000000 mokuro-0.1.6/mokuro/__main__.py
-drwxrwxrwx   0        0        0        0 2022-12-29 10:38:11.642856 mokuro-0.1.6/mokuro/assets/
-drwxrwxrwx   0        0        0        0 2022-12-29 10:38:11.660873 mokuro-0.1.6/mokuro/assets/icons/
--rw-rw-rw-   0        0        0      284 2022-04-24 16:27:29.000000 mokuro-0.1.6/mokuro/assets/icons/chevron-left-double-svgrepo-com.svg
--rw-rw-rw-   0        0        0      229 2022-04-24 16:27:29.000000 mokuro-0.1.6/mokuro/assets/icons/chevron-left-svgrepo-com.svg
--rw-rw-rw-   0        0        0      283 2022-04-24 16:27:29.000000 mokuro-0.1.6/mokuro/assets/icons/chevron-right-double-svgrepo-com.svg
--rw-rw-rw-   0        0        0      228 2022-04-24 16:27:29.000000 mokuro-0.1.6/mokuro/assets/icons/chevron-right-svgrepo-com.svg
--rw-rw-rw-   0        0        0      282 2022-04-24 16:27:29.000000 mokuro-0.1.6/mokuro/assets/icons/cross-svgrepo-com.svg
--rw-rw-rw-   0        0        0      342 2022-04-24 16:27:29.000000 mokuro-0.1.6/mokuro/assets/icons/expand-svgrepo-com.svg
--rw-rw-rw-   0        0        0      378 2022-04-24 16:27:29.000000 mokuro-0.1.6/mokuro/assets/icons/expand-width-svgrepo-com.svg
--rw-rw-rw-   0        0        0      482 2022-04-24 16:27:29.000000 mokuro-0.1.6/mokuro/assets/icons/fullscreen-svgrepo-com.svg
--rw-rw-rw-   0        0        0      282 2022-04-24 16:27:29.000000 mokuro-0.1.6/mokuro/assets/icons/menu-hamburger-svgrepo-com.svg
--rw-rw-rw-   0        0        0    32707 2022-04-24 16:27:29.000000 mokuro-0.1.6/mokuro/assets/panzoom.min.js
--rw-rw-rw-   0        0        0     1048 2022-04-24 16:27:29.000000 mokuro-0.1.6/mokuro/cache.py
--rw-rw-rw-   0        0        0      133 2022-04-24 16:27:29.000000 mokuro-0.1.6/mokuro/env.py
--rw-rw-rw-   0        0        0     3979 2022-12-29 10:06:15.000000 mokuro-0.1.6/mokuro/manga_page_ocr.py
--rw-rw-rw-   0        0        0    12952 2022-12-29 10:06:15.000000 mokuro-0.1.6/mokuro/overlay_generator.py
--rw-rw-rw-   0        0        0     1642 2022-12-29 10:06:15.000000 mokuro-0.1.6/mokuro/run.py
--rw-rw-rw-   0        0        0    16533 2022-12-29 10:06:15.000000 mokuro-0.1.6/mokuro/script.js
--rw-rw-rw-   0        0        0     5520 2022-12-29 10:06:15.000000 mokuro-0.1.6/mokuro/styles.css
--rw-rw-rw-   0        0        0      734 2022-04-24 16:27:29.000000 mokuro-0.1.6/mokuro/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-29 10:38:11.640855 mokuro-0.1.6/mokuro.egg-info/
--rw-rw-rw-   0        0        0     1939 2022-12-29 10:38:10.000000 mokuro-0.1.6/mokuro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1846 2022-12-29 10:38:10.000000 mokuro-0.1.6/mokuro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-29 10:38:10.000000 mokuro-0.1.6/mokuro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2022-12-29 10:38:10.000000 mokuro-0.1.6/mokuro.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      190 2022-12-29 10:38:10.000000 mokuro-0.1.6/mokuro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2022-12-29 10:38:10.000000 mokuro-0.1.6/mokuro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-29 10:38:11.674887 mokuro-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1208 2022-12-29 10:37:05.000000 mokuro-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-29 10:38:11.671884 mokuro-0.1.6/tests/
--rw-rw-rw-   0        0        0        0 2022-11-05 16:55:34.000000 mokuro-0.1.6/tests/__init__.py
--rw-rw-rw-   0        0        0      370 2022-11-05 16:55:34.000000 mokuro-0.1.6/tests/generate_expected_results.py
--rw-rw-rw-   0        0        0     1025 2022-11-05 16:55:34.000000 mokuro-0.1.6/tests/test_mokuro.py
+drwxrwxrwx   0        0        0        0 2023-05-07 20:58:23.000000 mokuro-0.1.7/
+-rw-rw-rw-   0        0        0    35823 2022-04-16 12:47:37.000000 mokuro-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      106 2022-04-24 18:07:31.000000 mokuro-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1939 2023-05-07 20:58:23.000000 mokuro-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3440 2023-05-07 09:34:49.000000 mokuro-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 20:58:23.000000 mokuro-0.1.7/comic_text_detector/
+-rw-rw-rw-   0        0        0    35823 2022-04-16 13:12:53.000000 mokuro-0.1.7/comic_text_detector/LICENSE
+-rw-rw-rw-   0        0        0        0 2022-04-16 15:46:37.000000 mokuro-0.1.7/comic_text_detector/__init__.py
+-rw-rw-rw-   0        0        0    11055 2022-11-05 10:30:05.000000 mokuro-0.1.7/comic_text_detector/basemodel.py
+-rw-rw-rw-   0        0        0    11890 2022-04-16 15:52:43.000000 mokuro-0.1.7/comic_text_detector/db_dataset.py
+-rw-rw-rw-   0        0        0     8925 2022-11-05 10:46:28.000000 mokuro-0.1.7/comic_text_detector/inference.py
+drwxrwxrwx   0        0        0        0 2023-05-07 20:58:23.000000 mokuro-0.1.7/comic_text_detector/models/
+-rw-rw-rw-   0        0        0        0 2022-04-16 13:12:53.000000 mokuro-0.1.7/comic_text_detector/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 20:58:23.000000 mokuro-0.1.7/comic_text_detector/models/yolov5/
+-rw-rw-rw-   0        0        0        0 2022-04-16 13:12:53.000000 mokuro-0.1.7/comic_text_detector/models/yolov5/__init__.py
+-rw-rw-rw-   0        0        0    10796 2022-11-05 10:29:46.000000 mokuro-0.1.7/comic_text_detector/models/yolov5/common.py
+-rw-rw-rw-   0        0        0    14774 2022-04-16 16:28:29.000000 mokuro-0.1.7/comic_text_detector/models/yolov5/yolo.py
+-rw-rw-rw-   0        0        0    10599 2022-04-16 15:52:43.000000 mokuro-0.1.7/comic_text_detector/seg_dataset.py
+-rw-rw-rw-   0        0        0    24903 2022-04-16 16:28:29.000000 mokuro-0.1.7/comic_text_detector/text_rendering.py
+-rw-rw-rw-   0        0        0    10139 2022-04-16 16:28:29.000000 mokuro-0.1.7/comic_text_detector/train_db.py
+-rw-rw-rw-   0        0        0     9093 2022-04-16 15:52:43.000000 mokuro-0.1.7/comic_text_detector/train_seg.py
+drwxrwxrwx   0        0        0        0 2023-05-07 20:58:23.000000 mokuro-0.1.7/comic_text_detector/utils/
+-rw-rw-rw-   0        0        0        0 2022-04-23 16:34:25.000000 mokuro-0.1.7/comic_text_detector/utils/__init__.py
+-rw-rw-rw-   0        0        0    28581 2022-12-29 10:31:12.000000 mokuro-0.1.7/comic_text_detector/utils/db_utils.py
+-rw-rw-rw-   0        0        0     2179 2022-11-22 21:36:36.000000 mokuro-0.1.7/comic_text_detector/utils/export.py
+-rw-rw-rw-   0        0        0     2472 2022-04-16 13:12:53.000000 mokuro-0.1.7/comic_text_detector/utils/general.py
+-rw-rw-rw-   0        0        0     7099 2022-04-16 13:12:53.000000 mokuro-0.1.7/comic_text_detector/utils/imgproc_utils.py
+-rw-rw-rw-   0        0        0     1859 2022-04-16 15:52:43.000000 mokuro-0.1.7/comic_text_detector/utils/io_utils.py
+-rw-rw-rw-   0        0        0     7397 2022-04-16 15:52:43.000000 mokuro-0.1.7/comic_text_detector/utils/loss.py
+-rw-rw-rw-   0        0        0    21790 2022-11-05 10:46:28.000000 mokuro-0.1.7/comic_text_detector/utils/textblock.py
+-rw-rw-rw-   0        0        0    13499 2022-04-16 15:52:43.000000 mokuro-0.1.7/comic_text_detector/utils/textmask.py
+-rw-rw-rw-   0        0        0     3888 2022-04-16 13:12:53.000000 mokuro-0.1.7/comic_text_detector/utils/weight_init.py
+-rw-rw-rw-   0        0        0    10454 2022-04-16 13:12:53.000000 mokuro-0.1.7/comic_text_detector/utils/yolov5_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-07 20:58:23.000000 mokuro-0.1.7/mokuro/
+-rw-rw-rw-   0        0        0      128 2023-05-07 20:57:33.000000 mokuro-0.1.7/mokuro/__init__.py
+-rw-rw-rw-   0        0        0      124 2022-04-24 16:27:29.000000 mokuro-0.1.7/mokuro/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 20:58:23.000000 mokuro-0.1.7/mokuro/assets/
+drwxrwxrwx   0        0        0        0 2023-05-07 20:58:23.000000 mokuro-0.1.7/mokuro/assets/icons/
+-rw-rw-rw-   0        0        0      284 2022-04-24 16:27:29.000000 mokuro-0.1.7/mokuro/assets/icons/chevron-left-double-svgrepo-com.svg
+-rw-rw-rw-   0        0        0      229 2022-04-24 16:27:29.000000 mokuro-0.1.7/mokuro/assets/icons/chevron-left-svgrepo-com.svg
+-rw-rw-rw-   0        0        0      283 2022-04-24 16:27:29.000000 mokuro-0.1.7/mokuro/assets/icons/chevron-right-double-svgrepo-com.svg
+-rw-rw-rw-   0        0        0      228 2022-04-24 16:27:29.000000 mokuro-0.1.7/mokuro/assets/icons/chevron-right-svgrepo-com.svg
+-rw-rw-rw-   0        0        0      282 2022-04-24 16:27:29.000000 mokuro-0.1.7/mokuro/assets/icons/cross-svgrepo-com.svg
+-rw-rw-rw-   0        0        0      342 2022-04-24 16:27:29.000000 mokuro-0.1.7/mokuro/assets/icons/expand-svgrepo-com.svg
+-rw-rw-rw-   0        0        0      378 2022-04-24 16:27:29.000000 mokuro-0.1.7/mokuro/assets/icons/expand-width-svgrepo-com.svg
+-rw-rw-rw-   0        0        0      482 2022-04-24 16:27:29.000000 mokuro-0.1.7/mokuro/assets/icons/fullscreen-svgrepo-com.svg
+-rw-rw-rw-   0        0        0      282 2022-04-24 16:27:29.000000 mokuro-0.1.7/mokuro/assets/icons/menu-hamburger-svgrepo-com.svg
+-rw-rw-rw-   0        0        0    32707 2022-04-24 16:27:29.000000 mokuro-0.1.7/mokuro/assets/panzoom.min.js
+-rw-rw-rw-   0        0        0     1048 2022-04-24 16:27:29.000000 mokuro-0.1.7/mokuro/cache.py
+-rw-rw-rw-   0        0        0      133 2022-04-24 16:27:29.000000 mokuro-0.1.7/mokuro/env.py
+-rw-rw-rw-   0        0        0     3979 2023-05-07 09:34:25.000000 mokuro-0.1.7/mokuro/manga_page_ocr.py
+-rw-rw-rw-   0        0        0    13282 2023-05-07 11:34:53.000000 mokuro-0.1.7/mokuro/overlay_generator.py
+-rw-rw-rw-   0        0        0     1642 2023-05-07 09:34:25.000000 mokuro-0.1.7/mokuro/run.py
+-rw-rw-rw-   0        0        0    16994 2023-05-07 11:34:53.000000 mokuro-0.1.7/mokuro/script.js
+-rw-rw-rw-   0        0        0     5520 2023-05-07 09:34:25.000000 mokuro-0.1.7/mokuro/styles.css
+-rw-rw-rw-   0        0        0      734 2022-04-24 16:27:29.000000 mokuro-0.1.7/mokuro/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-07 20:58:23.000000 mokuro-0.1.7/mokuro.egg-info/
+-rw-rw-rw-   0        0        0     1939 2023-05-07 20:58:22.000000 mokuro-0.1.7/mokuro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1846 2023-05-07 20:58:22.000000 mokuro-0.1.7/mokuro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 20:58:22.000000 mokuro-0.1.7/mokuro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-07 20:58:22.000000 mokuro-0.1.7/mokuro.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      197 2023-05-07 20:58:22.000000 mokuro-0.1.7/mokuro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-05-07 20:58:22.000000 mokuro-0.1.7/mokuro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 20:58:23.000000 mokuro-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1215 2023-05-07 20:57:33.000000 mokuro-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 20:58:23.000000 mokuro-0.1.7/tests/
+-rw-rw-rw-   0        0        0        0 2022-11-05 16:55:34.000000 mokuro-0.1.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      370 2022-11-05 16:55:34.000000 mokuro-0.1.7/tests/generate_expected_results.py
+-rw-rw-rw-   0        0        0     1025 2022-11-05 16:55:34.000000 mokuro-0.1.7/tests/test_mokuro.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `mokuro-0.1.6/LICENSE` & `mokuro-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/PKG-INFO` & `mokuro-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mokuro
-Version: 0.1.6
+Version: 0.1.7
 Summary: Browser reader for manga with selectable text
 Home-page: https://github.com/kha-white/mokuro
 Author: Maciej Budyś
 Author-email: kha-white@mail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `mokuro-0.1.6/README.md` & `mokuro-0.1.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 See also:
 - [Mokuro2Pdf](https://github.com/Kartoffel0/Mokuro2Pdf), cli Ruby script to generate pdf files with selectable text from Mokuro's html overlay
 - [Xelieu's guide](https://rentry.co/lazyXel), a comprehensive guide on setting up a reading and mining workflow with manga-ocr/mokuro (and many other useful tips)
 
 # Installation
 
-You need Python 3.6, 3.7, 3.8 or 3.9. Unfortunately, PyTorch does not support Python 3.10 yet.
+You need Python 3.6, 3.7, 3.8, 3.9, or 3.10. As of April 2023, PyTorch unfortunately does not support Python 3.11 yet, see pytorch/pytorch#86566.
 
 Some users have reported problems with Python installed from Microsoft Store. If you see an error:
 `ImportError: DLL load failed while importing fugashi: The specified module could not be found.`,
 try installing Python from the [official site](https://www.python.org/downloads).
 
 If you want to run with GPU, install PyTorch as described [here](https://pytorch.org/get-started/locally/#start-locally),
 otherwise this step can be skipped.
```

### Comparing `mokuro-0.1.6/comic_text_detector/LICENSE` & `mokuro-0.1.7/comic_text_detector/LICENSE`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/basemodel.py` & `mokuro-0.1.7/comic_text_detector/basemodel.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/db_dataset.py` & `mokuro-0.1.7/comic_text_detector/db_dataset.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/inference.py` & `mokuro-0.1.7/comic_text_detector/inference.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/models/yolov5/common.py` & `mokuro-0.1.7/comic_text_detector/models/yolov5/common.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/models/yolov5/yolo.py` & `mokuro-0.1.7/comic_text_detector/models/yolov5/yolo.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/seg_dataset.py` & `mokuro-0.1.7/comic_text_detector/seg_dataset.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/text_rendering.py` & `mokuro-0.1.7/comic_text_detector/text_rendering.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/train_db.py` & `mokuro-0.1.7/comic_text_detector/train_db.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/train_seg.py` & `mokuro-0.1.7/comic_text_detector/train_seg.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/utils/db_utils.py` & `mokuro-0.1.7/comic_text_detector/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/utils/export.py` & `mokuro-0.1.7/comic_text_detector/utils/export.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/utils/general.py` & `mokuro-0.1.7/comic_text_detector/utils/general.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/utils/imgproc_utils.py` & `mokuro-0.1.7/comic_text_detector/utils/imgproc_utils.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/utils/io_utils.py` & `mokuro-0.1.7/comic_text_detector/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/utils/loss.py` & `mokuro-0.1.7/comic_text_detector/utils/loss.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/utils/textblock.py` & `mokuro-0.1.7/comic_text_detector/utils/textblock.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/utils/textmask.py` & `mokuro-0.1.7/comic_text_detector/utils/textmask.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/utils/weight_init.py` & `mokuro-0.1.7/comic_text_detector/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/comic_text_detector/utils/yolov5_utils.py` & `mokuro-0.1.7/comic_text_detector/utils/yolov5_utils.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/mokuro/assets/panzoom.min.js` & `mokuro-0.1.7/mokuro/assets/panzoom.min.js`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/mokuro/cache.py` & `mokuro-0.1.7/mokuro/cache.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/mokuro/manga_page_ocr.py` & `mokuro-0.1.7/mokuro/manga_page_ocr.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/mokuro/overlay_generator.py` & `mokuro-0.1.7/mokuro/overlay_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,20 @@
             with tag('label', klass='dropdown-option'):
                 text(text_content)
                 with tag('select', id=id_):
                     for value in values:
                         with tag('option', value=value):
                             text(value)
 
+        def option_color(id_, text_content, value):
+            with tag('label', klass='dropdown-option'):
+                text(text_content)
+                with tag('input', type='color',  value=value, id=id_):
+                    pass
+
         with tag('div', klass='dropdown'):
             with tag('button', id='dropbtn', klass='menuButton'):
                 doc.asis(self.get_icon('menu-hamburger-svgrepo-com'))
 
             with tag('div', klass='dropdown-content'):
                 with tag('div', klass='buttonRow'):
                     with tag('button', id='menuFitToScreen', klass='menuButton'):
@@ -246,14 +252,15 @@
                 option_toggle('menuDisplayOCR', 'OCR enabled ')
                 option_toggle('menuTextBoxBorders', 'display boxes outlines ')
                 option_toggle('menuEditableText', 'editable text ')
                 option_select('menuFontSize', 'font size: ',
                               ['auto', 9, 10, 11, 12, 14, 16, 18, 20, 24, 32, 40, 48, 60])
                 option_toggle('menuEInkMode', 'e-ink mode ')
                 option_toggle('menuToggleOCRTextBoxes', 'toggle OCR text boxes on click')
+                option_color('menuBackgroundColor', 'background color', '#C4C3D0')
                 option_click('menuReset', 'reset settings')
                 option_click('menuAbout', 'about/help')
 
     def get_page_html(self, result, img_path):
         doc, tag, text = Doc().tagtext()
 
         # assign z-index ordering from largest to smallest boxes,
```

### Comparing `mokuro-0.1.6/mokuro/run.py` & `mokuro-0.1.7/mokuro/run.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/mokuro/script.js` & `mokuro-0.1.7/mokuro/script.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -16,14 +16,15 @@
     textBoxBorders: false,
     editableText: false,
     displayOCR: true,
     fontSize: "auto",
     eInkMode: false,
     defaultZoomMode: "fit to screen",
     toggleOCRTextBoxes: false,
+    backgroundColor: '#C4C3D0',
 };
 
 let state = JSON.parse(JSON.stringify(defaultState));
 
 function saveState() {
     localStorage.setItem(storageKey, JSON.stringify(state));
 }
@@ -47,14 +48,15 @@
     document.getElementById("menuTextBoxBorders").checked = state.textBoxBorders;
     document.getElementById("menuEditableText").checked = state.editableText;
     document.getElementById("menuDisplayOCR").checked = state.displayOCR;
     document.getElementById('menuFontSize').value = state.fontSize;
     document.getElementById('menuEInkMode').checked = state.eInkMode;
     document.getElementById('menuDefaultZoom').value = state.defaultZoomMode;
     document.getElementById('menuToggleOCRTextBoxes').checked = state.toggleOCRTextBoxes;
+    document.getElementById('menuBackgroundColor').value = state.backgroundColor;
 }
 
 document.addEventListener('DOMContentLoaded', function() {
     loadState();
     num_pages = document.getElementsByClassName("page").length;
 
     pz = panzoom(pc, {
@@ -160,14 +162,18 @@
     }
 
     if (state.eInkMode) {
         document.getElementById('topMenu').classList.add("notransition");
     } else {
         document.getElementById('topMenu').classList.remove("notransition");
     }
+
+    if (state.backgroundColor) {
+        r.style.setProperty('--colorBackground', state.backgroundColor)
+    }
 }
 
 document.getElementById('menuR2l').addEventListener('click', function() {
     state.r2l = document.getElementById("menuR2l").checked;
     saveState();
     updatePage(state.page_idx);
 }, false);
@@ -218,14 +224,24 @@
 
 document.getElementById('menuToggleOCRTextBoxes').addEventListener('click', function() {
     state.toggleOCRTextBoxes = document.getElementById("menuToggleOCRTextBoxes").checked;
     saveState();
     updateProperties();
 }, false);
 
+document.getElementById('menuBackgroundColor').addEventListener(
+    'input',
+    function(event) {
+        state.backgroundColor = event.target.value;
+        saveState();
+        updateProperties();
+    },
+    false
+);
+
 document.getElementById('menuOriginalSize').addEventListener('click', zoomOriginal, false);
 document.getElementById('menuFitToWidth').addEventListener('click', zoomFitToWidth, false);
 document.getElementById('menuFitToScreen').addEventListener('click', zoomFitToScreen, false);
 document.getElementById('menuFullScreen').addEventListener('click', toggleFullScreen, false);
 
 document.getElementById('menuAbout').addEventListener('click', function() {
     document.getElementById('popupAbout').style.display = 'block';
```

### Comparing `mokuro-0.1.6/mokuro/styles.css` & `mokuro-0.1.7/mokuro/styles.css`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/mokuro/utils.py` & `mokuro-0.1.7/mokuro/utils.py`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/mokuro.egg-info/PKG-INFO` & `mokuro-0.1.7/mokuro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mokuro
-Version: 0.1.6
+Version: 0.1.7
 Summary: Browser reader for manga with selectable text
 Home-page: https://github.com/kha-white/mokuro
 Author: Maciej Budyś
 Author-email: kha-white@mail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `mokuro-0.1.6/mokuro.egg-info/SOURCES.txt` & `mokuro-0.1.7/mokuro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mokuro-0.1.6/setup.py` & `mokuro-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 long_description = (Path(__file__).parent / "README.md").read_text('utf-8').split('# Installation')[0]
 
 setup(
     name="mokuro",
-    version='0.1.6',
+    version='0.1.7',
     description="Browser reader for manga with selectable text",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kha-white/mokuro",
     author="Maciej Budyś",
     author_email="kha-white@mail.com",
     license="GPLv3",
@@ -26,19 +26,19 @@
         "natsort",
         "numpy",
         "opencv-python>=4.1.2",
         "Pillow>=7.1.2",
         "pyclipper",
         "requests",
         "scipy",
-        "sentencepiece",
         "shapely",
         "torch>=1.7.0",
         "torchsummary",
         "torchvision>=0.8.1",
+        "transformers>=4.25.0",
         "tqdm>=4.41.0",
         "yattag",
     ],
     entry_points={
         "console_scripts": [
             "mokuro=mokuro.__main__:main",
         ]
```

### Comparing `mokuro-0.1.6/tests/test_mokuro.py` & `mokuro-0.1.7/tests/test_mokuro.py`

 * *Files identical despite different names*

