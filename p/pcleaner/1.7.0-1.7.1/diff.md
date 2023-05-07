# Comparing `tmp/pcleaner-1.7.0.tar.gz` & `tmp/pcleaner-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcleaner-1.7.0.tar", last modified: Fri May  5 21:42:16 2023, max compression
+gzip compressed data, was "pcleaner-1.7.1.tar", last modified: Sun May  7 15:40:57 2023, max compression
```

## Comparing `pcleaner-1.7.0.tar` & `pcleaner-1.7.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 21:42:16.000628 pcleaner-1.7.0/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.7.0/LICENSE
--rw-r--r--   0 corbin    (1000) corbin    (1001)    12273 2023-05-05 21:42:16.000628 pcleaner-1.7.0/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)    11599 2023-05-04 21:07:46.000000 pcleaner-1.7.0/README.md
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 21:42:15.993962 pcleaner-1.7.0/pcleaner/
--rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2023-05-05 21:41:58.000000 pcleaner-1.7.0/pcleaner/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    19402 2023-05-04 21:08:14.000000 pcleaner-1.7.0/pcleaner/analytics.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6380 2023-05-04 21:08:14.000000 pcleaner-1.7.0/pcleaner/cli_utils.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 21:42:15.997295 pcleaner-1.7.0/pcleaner/comic_text_detector/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.7.0/pcleaner/comic_text_detector/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.7.0/pcleaner/comic_text_detector/basemodel.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.7.0/pcleaner/comic_text_detector/inference.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 21:42:15.997295 pcleaner-1.7.0/pcleaner/comic_text_detector/models/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.7.0/pcleaner/comic_text_detector/models/__init__.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 21:42:15.997295 pcleaner-1.7.0/pcleaner/comic_text_detector/models/yolov5/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.7.0/pcleaner/comic_text_detector/models/yolov5/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.7.0/pcleaner/comic_text_detector/models/yolov5/common.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.7.0/pcleaner/comic_text_detector/models/yolov5/yolo.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 21:42:15.997295 pcleaner-1.7.0/pcleaner/comic_text_detector/utils/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.7.0/pcleaner/comic_text_detector/utils/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.7.0/pcleaner/comic_text_detector/utils/db_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.7.0/pcleaner/comic_text_detector/utils/export.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.7.0/pcleaner/comic_text_detector/utils/general.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.7.0/pcleaner/comic_text_detector/utils/imgproc_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.7.0/pcleaner/comic_text_detector/utils/io_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.7.0/pcleaner/comic_text_detector/utils/loss.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.7.0/pcleaner/comic_text_detector/utils/textblock.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.7.0/pcleaner/comic_text_detector/utils/textmask.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.7.0/pcleaner/comic_text_detector/utils/weight_init.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.7.0/pcleaner/comic_text_detector/utils/yolov5_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    45416 2023-05-05 16:06:03.000000 pcleaner-1.7.0/pcleaner/config.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6056 2023-04-17 18:08:37.000000 pcleaner-1.7.0/pcleaner/ctd_interface.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 21:42:15.997295 pcleaner-1.7.0/pcleaner/data/
--rw-r--r--   0 corbin    (1000) corbin    (1001)   410712 2021-09-30 18:43:41.000000 pcleaner-1.7.0/pcleaner/data/LiberationSans-Regular.ttf
--rw-r--r--   0 corbin    (1000) corbin    (1001)   107848 2018-04-08 15:54:09.000000 pcleaner-1.7.0/pcleaner/data/NotoMono-Regular.ttf
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-18 19:22:52.000000 pcleaner-1.7.0/pcleaner/data/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     5573 2023-04-14 12:31:20.000000 pcleaner-1.7.0/pcleaner/denoiser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 21:42:16.000628 pcleaner-1.7.0/pcleaner/gui/
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 21:42:16.000628 pcleaner-1.7.0/pcleaner/gui/CustomQ/
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2600 2023-05-05 16:04:17.000000 pcleaner-1.7.0/pcleaner/gui/CustomQ/CColorButton.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3323 2023-05-05 21:26:07.000000 pcleaner-1.7.0/pcleaner/gui/CustomQ/CComboBox.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3234 2023-04-21 15:08:36.000000 pcleaner-1.7.0/pcleaner/gui/CustomQ/CTableWidget.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:59:57.000000 pcleaner-1.7.0/pcleaner/gui/CustomQ/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-1.7.0/pcleaner/gui/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    21094 2023-05-05 16:04:17.000000 pcleaner-1.7.0/pcleaner/gui/file_table.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1094 2023-05-05 20:27:29.000000 pcleaner-1.7.0/pcleaner/gui/gui_utils.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1958 2023-04-22 17:01:16.000000 pcleaner-1.7.0/pcleaner/gui/launcher.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    42594 2023-05-05 21:40:55.000000 pcleaner-1.7.0/pcleaner/gui/mainwindow_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4457 2023-05-05 16:04:17.000000 pcleaner-1.7.0/pcleaner/gui/new_profile_driver.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    16468 2023-05-05 21:36:36.000000 pcleaner-1.7.0/pcleaner/gui/profile_parser.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 21:42:16.000628 pcleaner-1.7.0/pcleaner/gui/rc_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:25:41.000000 pcleaner-1.7.0/pcleaner/gui/rc_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    10008 2023-04-22 16:59:47.000000 pcleaner-1.7.0/pcleaner/gui/rc_generated_files/icons_rc.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    75061 2023-04-22 17:01:02.000000 pcleaner-1.7.0/pcleaner/gui/rc_generated_files/theme_icons_rc.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 21:42:16.000628 pcleaner-1.7.0/pcleaner/gui/ui_generated_files/
--rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 00:09:43.000000 pcleaner-1.7.0/pcleaner/gui/ui_generated_files/__init__.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     6310 2023-04-17 00:10:07.000000 pcleaner-1.7.0/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    29795 2023-05-05 16:04:17.000000 pcleaner-1.7.0/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7464 2023-05-05 16:04:17.000000 pcleaner-1.7.0/pcleaner/gui/ui_generated_files/ui_NewProfile.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     3233 2023-05-05 16:04:17.000000 pcleaner-1.7.0/pcleaner/gui/worker_thread.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1828 2023-04-21 20:13:16.000000 pcleaner-1.7.0/pcleaner/helpers.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    23467 2023-05-05 14:10:21.000000 pcleaner-1.7.0/pcleaner/image_ops.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    27027 2023-05-05 16:00:19.000000 pcleaner-1.7.0/pcleaner/main.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8762 2023-04-18 15:30:06.000000 pcleaner-1.7.0/pcleaner/masker.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     4845 2023-04-14 12:51:27.000000 pcleaner-1.7.0/pcleaner/model_downloader.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     8778 2023-05-04 20:46:40.000000 pcleaner-1.7.0/pcleaner/pre_processor.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)     7581 2023-05-04 21:08:14.000000 pcleaner-1.7.0/pcleaner/profile_cli.py
--rw-r--r--   0 corbin    (1000) corbin    (1001)    14109 2023-04-18 20:03:45.000000 pcleaner-1.7.0/pcleaner/structures.py
-drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-05 21:42:15.997295 pcleaner-1.7.0/pcleaner.egg-info/
--rw-r--r--   0 corbin    (1000) corbin    (1001)    12273 2023-05-05 21:42:15.000000 pcleaner-1.7.0/pcleaner.egg-info/PKG-INFO
--rw-r--r--   0 corbin    (1000) corbin    (1001)     2218 2023-05-05 21:42:15.000000 pcleaner-1.7.0/pcleaner.egg-info/SOURCES.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-05-05 21:42:15.000000 pcleaner-1.7.0/pcleaner.egg-info/dependency_links.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-05-05 21:42:15.000000 pcleaner-1.7.0/pcleaner.egg-info/entry_points.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      188 2023-05-05 21:42:15.000000 pcleaner-1.7.0/pcleaner.egg-info/requires.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-05-05 21:42:15.000000 pcleaner-1.7.0/pcleaner.egg-info/top_level.txt
--rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.7.0/pyproject.toml
--rw-r--r--   0 corbin    (1000) corbin    (1001)     1138 2023-05-05 21:42:16.000628 pcleaner-1.7.0/setup.cfg
--rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.7.0/setup.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.637381 pcleaner-1.7.1/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    35129 2023-01-07 18:56:55.000000 pcleaner-1.7.1/LICENSE
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    12273 2023-05-07 15:40:57.637381 pcleaner-1.7.1/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    11599 2023-05-04 21:07:46.000000 pcleaner-1.7.1/README.md
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.627381 pcleaner-1.7.1/pcleaner/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       82 2023-05-07 15:40:17.000000 pcleaner-1.7.1/pcleaner/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    19402 2023-05-04 21:08:14.000000 pcleaner-1.7.1/pcleaner/analytics.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6380 2023-05-04 21:08:14.000000 pcleaner-1.7.1/pcleaner/cli_utils.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.627381 pcleaner-1.7.1/pcleaner/comic_text_detector/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:00.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10114 2023-01-07 23:20:26.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/basemodel.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8492 2023-01-07 23:33:40.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/inference.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.627381 pcleaner-1.7.1/pcleaner/comic_text_detector/models/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/models/__init__.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.627381 pcleaner-1.7.1/pcleaner/comic_text_detector/models/yolov5/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2022-12-24 01:25:46.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/models/yolov5/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10685 2023-01-07 23:24:30.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/models/yolov5/common.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14770 2023-01-07 23:38:16.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/models/yolov5/yolo.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.630714 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-01-07 23:23:32.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27905 2023-01-07 23:20:26.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/db_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2136 2023-01-07 23:25:33.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/export.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2582 2023-01-07 23:25:33.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/general.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7012 2023-01-07 23:20:26.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/imgproc_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1919 2023-04-13 13:46:43.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/io_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7283 2023-01-07 23:26:33.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/loss.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    20873 2023-01-07 23:27:00.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/textblock.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    13486 2023-01-07 23:27:26.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/textmask.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3181 2023-01-07 23:28:17.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/weight_init.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10727 2023-01-07 23:28:28.000000 pcleaner-1.7.1/pcleaner/comic_text_detector/utils/yolov5_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    45416 2023-05-05 16:06:03.000000 pcleaner-1.7.1/pcleaner/config.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6333 2023-05-07 15:38:48.000000 pcleaner-1.7.1/pcleaner/ctd_interface.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.634048 pcleaner-1.7.1/pcleaner/data/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   410712 2021-09-30 18:43:41.000000 pcleaner-1.7.1/pcleaner/data/LiberationSans-Regular.ttf
+-rw-r--r--   0 corbin    (1000) corbin    (1001)   107848 2018-04-08 15:54:09.000000 pcleaner-1.7.1/pcleaner/data/NotoMono-Regular.ttf
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-18 19:22:52.000000 pcleaner-1.7.1/pcleaner/data/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     5573 2023-04-14 12:31:20.000000 pcleaner-1.7.1/pcleaner/denoiser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.634048 pcleaner-1.7.1/pcleaner/gui/
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.634048 pcleaner-1.7.1/pcleaner/gui/CustomQ/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2600 2023-05-05 16:04:17.000000 pcleaner-1.7.1/pcleaner/gui/CustomQ/CColorButton.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3323 2023-05-05 21:26:07.000000 pcleaner-1.7.1/pcleaner/gui/CustomQ/CComboBox.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3234 2023-04-21 15:08:36.000000 pcleaner-1.7.1/pcleaner/gui/CustomQ/CTableWidget.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:59:57.000000 pcleaner-1.7.1/pcleaner/gui/CustomQ/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-14 12:39:20.000000 pcleaner-1.7.1/pcleaner/gui/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    21094 2023-05-05 16:04:17.000000 pcleaner-1.7.1/pcleaner/gui/file_table.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1094 2023-05-05 20:27:29.000000 pcleaner-1.7.1/pcleaner/gui/gui_utils.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1958 2023-04-22 17:01:16.000000 pcleaner-1.7.1/pcleaner/gui/launcher.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    42594 2023-05-05 21:40:55.000000 pcleaner-1.7.1/pcleaner/gui/mainwindow_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4457 2023-05-05 16:04:17.000000 pcleaner-1.7.1/pcleaner/gui/new_profile_driver.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    16468 2023-05-05 21:36:36.000000 pcleaner-1.7.1/pcleaner/gui/profile_parser.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.634048 pcleaner-1.7.1/pcleaner/gui/rc_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 01:25:41.000000 pcleaner-1.7.1/pcleaner/gui/rc_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    10008 2023-04-22 16:59:47.000000 pcleaner-1.7.1/pcleaner/gui/rc_generated_files/icons_rc.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    75061 2023-04-22 17:01:02.000000 pcleaner-1.7.1/pcleaner/gui/rc_generated_files/theme_icons_rc.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.637381 pcleaner-1.7.1/pcleaner/gui/ui_generated_files/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        0 2023-04-17 00:09:43.000000 pcleaner-1.7.1/pcleaner/gui/ui_generated_files/__init__.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     6310 2023-04-17 00:10:07.000000 pcleaner-1.7.1/pcleaner/gui/ui_generated_files/ui_ImageDetails.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    29795 2023-05-05 16:04:17.000000 pcleaner-1.7.1/pcleaner/gui/ui_generated_files/ui_Mainwindow.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7464 2023-05-05 16:04:17.000000 pcleaner-1.7.1/pcleaner/gui/ui_generated_files/ui_NewProfile.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     3233 2023-05-05 16:04:17.000000 pcleaner-1.7.1/pcleaner/gui/worker_thread.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1828 2023-04-21 20:13:16.000000 pcleaner-1.7.1/pcleaner/helpers.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    23467 2023-05-05 14:10:21.000000 pcleaner-1.7.1/pcleaner/image_ops.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    27027 2023-05-06 17:47:48.000000 pcleaner-1.7.1/pcleaner/main.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8762 2023-05-06 17:47:48.000000 pcleaner-1.7.1/pcleaner/masker.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     4845 2023-04-14 12:51:27.000000 pcleaner-1.7.1/pcleaner/model_downloader.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     8817 2023-05-06 17:51:16.000000 pcleaner-1.7.1/pcleaner/pre_processor.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     7581 2023-05-04 21:08:14.000000 pcleaner-1.7.1/pcleaner/profile_cli.py
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    14109 2023-05-06 17:51:42.000000 pcleaner-1.7.1/pcleaner/structures.py
+drwxr-xr-x   0 corbin    (1000) corbin    (1001)        0 2023-05-07 15:40:57.627381 pcleaner-1.7.1/pcleaner.egg-info/
+-rw-r--r--   0 corbin    (1000) corbin    (1001)    12273 2023-05-07 15:40:57.000000 pcleaner-1.7.1/pcleaner.egg-info/PKG-INFO
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     2218 2023-05-07 15:40:57.000000 pcleaner-1.7.1/pcleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        1 2023-05-07 15:40:57.000000 pcleaner-1.7.1/pcleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       48 2023-05-07 15:40:57.000000 pcleaner-1.7.1/pcleaner.egg-info/entry_points.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      188 2023-05-07 15:40:57.000000 pcleaner-1.7.1/pcleaner.egg-info/requires.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)        9 2023-05-07 15:40:57.000000 pcleaner-1.7.1/pcleaner.egg-info/top_level.txt
+-rw-r--r--   0 corbin    (1000) corbin    (1001)      122 2023-01-23 03:12:00.000000 pcleaner-1.7.1/pyproject.toml
+-rw-r--r--   0 corbin    (1000) corbin    (1001)     1138 2023-05-07 15:40:57.637381 pcleaner-1.7.1/setup.cfg
+-rw-r--r--   0 corbin    (1000) corbin    (1001)       38 2023-01-07 18:56:55.000000 pcleaner-1.7.1/setup.py
```

### Comparing `pcleaner-1.7.0/LICENSE` & `pcleaner-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/PKG-INFO` & `pcleaner-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.7.0
+Version: 1.7.1
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `pcleaner-1.7.0/README.md` & `pcleaner-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/analytics.py` & `pcleaner-1.7.1/pcleaner/analytics.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/cli_utils.py` & `pcleaner-1.7.1/pcleaner/cli_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/comic_text_detector/basemodel.py` & `pcleaner-1.7.1/pcleaner/comic_text_detector/basemodel.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/comic_text_detector/inference.py` & `pcleaner-1.7.1/pcleaner/comic_text_detector/inference.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/comic_text_detector/models/yolov5/common.py` & `pcleaner-1.7.1/pcleaner/comic_text_detector/models/yolov5/common.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/comic_text_detector/models/yolov5/yolo.py` & `pcleaner-1.7.1/pcleaner/comic_text_detector/models/yolov5/yolo.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/comic_text_detector/utils/db_utils.py` & `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/comic_text_detector/utils/export.py` & `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/export.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/comic_text_detector/utils/general.py` & `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/general.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/comic_text_detector/utils/imgproc_utils.py` & `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/imgproc_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/comic_text_detector/utils/io_utils.py` & `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/comic_text_detector/utils/loss.py` & `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/loss.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/comic_text_detector/utils/textblock.py` & `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/textblock.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/comic_text_detector/utils/textmask.py` & `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/textmask.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/comic_text_detector/utils/weight_init.py` & `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/comic_text_detector/utils/yolov5_utils.py` & `pcleaner-1.7.1/pcleaner/comic_text_detector/utils/yolov5_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/config.py` & `pcleaner-1.7.1/pcleaner/config.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/ctd_interface.py` & `pcleaner-1.7.1/pcleaner/ctd_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import json
 import uuid
 from pathlib import Path
 import multiprocessing as mp
 
 from tqdm import tqdm
+from PIL import Image
 import torch
 import numpy as np
 import cv2
 from logzero import logger
 
 import pcleaner.config as cfg
 from .comic_text_detector.inference import TextDetector
@@ -141,16 +142,19 @@
     data = {
         "image_path": img_name,
         "mask_path": maskname,
         "original_path": str(img_path),
         "scale": image_scale,
         "blk_list": blk_dict_list,
     }
-
-    with open(Path(img_name).with_suffix(".json"), "w", encoding="utf8") as f:
+    # Remove the suffix and add _raw.json
+    json_path = Path(img_name).with_suffix(".json")
+    json_path = json_path.with_stem(json_path.stem + "#raw")
+    logger.debug(f"Saving json file to {json_path}")
+    with open(json_path, "w", encoding="utf8") as f:
         json.dump(data, f, ensure_ascii=False, cls=NumpyEncoder, indent=4)
     imwrite(img_name, img)
     imwrite(maskname, mask_refined)
 
 
 def read_image(path: Path | str, scale=1.0) -> np.ndarray:
     """
@@ -158,16 +162,19 @@
     Then return an array of the image.
 
     :param path: Image path
     :param scale: Scale factor
     :return: Image array
     """
 
-    img = cv2.imdecode(np.fromfile(str(path), dtype=np.uint8), cv2.IMREAD_COLOR)
+    img = Image.open(str(path))
+
+    if img.mode == "CMYK":
+        logger.warning(f"Image {path} is in CMYK mode. Converting to RGB.")
+        img = img.convert("RGB")
 
     if scale != 1.0:
-        height, width, channels = img.shape
-        new_width = int(width * scale)
-        new_height = int(height * scale)
-        img = cv2.resize(img, (new_width, new_height))
+        new_width = int(img.width * scale)
+        new_height = int(img.height * scale)
+        img = img.resize((new_width, new_height), Image.ANTIALIAS)
 
-    return img
+    return np.array(img)
```

### Comparing `pcleaner-1.7.0/pcleaner/data/LiberationSans-Regular.ttf` & `pcleaner-1.7.1/pcleaner/data/LiberationSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/data/NotoMono-Regular.ttf` & `pcleaner-1.7.1/pcleaner/data/NotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/denoiser.py` & `pcleaner-1.7.1/pcleaner/denoiser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/gui/CustomQ/CColorButton.py` & `pcleaner-1.7.1/pcleaner/gui/CustomQ/CColorButton.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/gui/CustomQ/CComboBox.py` & `pcleaner-1.7.1/pcleaner/gui/CustomQ/CComboBox.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/gui/CustomQ/CTableWidget.py` & `pcleaner-1.7.1/pcleaner/gui/CustomQ/CTableWidget.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/gui/file_table.py` & `pcleaner-1.7.1/pcleaner/gui/file_table.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/gui/gui_utils.py` & `pcleaner-1.7.1/pcleaner/gui/gui_utils.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/gui/launcher.py` & `pcleaner-1.7.1/pcleaner/gui/launcher.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/gui/mainwindow_driver.py` & `pcleaner-1.7.1/pcleaner/gui/mainwindow_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/gui/new_profile_driver.py` & `pcleaner-1.7.1/pcleaner/gui/new_profile_driver.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/gui/profile_parser.py` & `pcleaner-1.7.1/pcleaner/gui/profile_parser.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/gui/rc_generated_files/icons_rc.py` & `pcleaner-1.7.1/pcleaner/gui/rc_generated_files/icons_rc.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/gui/rc_generated_files/theme_icons_rc.py` & `pcleaner-1.7.1/pcleaner/gui/rc_generated_files/theme_icons_rc.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/gui/ui_generated_files/ui_ImageDetails.py` & `pcleaner-1.7.1/pcleaner/gui/ui_generated_files/ui_ImageDetails.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/gui/ui_generated_files/ui_Mainwindow.py` & `pcleaner-1.7.1/pcleaner/gui/ui_generated_files/ui_Mainwindow.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/gui/ui_generated_files/ui_NewProfile.py` & `pcleaner-1.7.1/pcleaner/gui/ui_generated_files/ui_NewProfile.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/gui/worker_thread.py` & `pcleaner-1.7.1/pcleaner/gui/worker_thread.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/helpers.py` & `pcleaner-1.7.1/pcleaner/helpers.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/image_ops.py` & `pcleaner-1.7.1/pcleaner/image_ops.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/main.py` & `pcleaner-1.7.1/pcleaner/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,15 @@
 
         if ocr_analytics and not hide_analytics:
             an.show_ocr_analytics(ocr_analytics, profile.pre_processor.ocr_max_size)
 
     if not skip_masking:
         print("Running Masker...")
         # Read the json files in the image directory.
-        json_files = Path(cache_dir).glob("*_clean.json")
+        json_files = Path(cache_dir).glob("*#clean.json")
 
         # When denoising, we don't immediately output the cleaned image.
         # But when not, we do, since denoising is optional.
         if not skip_denoising:
             masker_output_dir = None
         else:
             masker_output_dir = output_dir
@@ -394,15 +394,15 @@
 
         if not hide_analytics and masker_analytics_raw:
             an.show_masker_analytics(masker_analytics_raw)
 
     if not skip_denoising:
         print("Running Denoiser...")
         # Read the json files in the image directory.
-        json_files = Path(cache_dir).glob("*_mask_data.json")
+        json_files = Path(cache_dir).glob("*#mask_data.json")
 
         # Zip together the json files and the out path thing.
         data = [
             st.DenoiserData(
                 json_file,
                 output_dir,
                 cache_dir,
```

### Comparing `pcleaner-1.7.0/pcleaner/masker.py` & `pcleaner-1.7.1/pcleaner/masker.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,8 +202,8 @@
         m.noise_mask_data for m in mask_fitments if m.analytics_std_deviation <= mask_max_deviation
     ]
 
     # Save the data.
     mask_data = st.MaskData(
         original_path, target_path, base_image_path, mask_path, scale, boxes_with_deviation
     )
-    mask_data.write_json(cache_path.with_name(cache_path.stem + "_mask_data.json"))
+    mask_data.write_json(cache_path.with_name(cache_path.stem + "#mask_data.json"))
```

### Comparing `pcleaner-1.7.0/pcleaner/model_downloader.py` & `pcleaner-1.7.1/pcleaner/model_downloader.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/pre_processor.py` & `pcleaner-1.7.1/pcleaner/pre_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import re
 from dataclasses import asdict
 from pathlib import Path
 from functools import partial
 
 from PIL import Image
 from manga_ocr import MangaOcr
+from logzero import logger
 
 import pcleaner.ctd_interface as ctm
 import pcleaner.structures as st
 import pcleaner.config as cfg
 import pcleaner.helpers as hp
 
 
@@ -42,15 +43,15 @@
     cache_masks_ocr: bool = False,
 ) -> tuple[int, tuple[int, ...], tuple[int, ...], tuple[tuple[str, str], ...]] | None:
     """
     Load the generated json file, and clean the data, leaving only the
     relevant data for the following steps.
 
     Check that this file wasn't already processed, and if it was, skip it.
-    Processed json files have the file name ending with '_clean.json'.
+    Processed json files have the file name ending with '#clean.json'.
 
     If a manga ocr object is given, run ocr on small boxes to determine whether
     they contain mere symbols, in which case these boxes do not need to be cleaned
     and can be removed from the dataset.
     The model must be initialized somewhere else to lessen coupling, and to avoid the long
     initialization time for each page.
 
@@ -59,19 +60,20 @@
     :param json_file_path: Path to the json file.
     :param pre_processor_conf: Pre processor configuration, part of the profile.
     :param cache_masks: Whether to cache the masks.
     :param mocr: [Optional] Manga ocr object.
     :param cache_masks_ocr: [Optional] Whether to cache the masks early for ocr.
     :return: Analytics data if the manga ocr object is given, None otherwise.
     """
+    logger.debug(f"Processing json file: {json_file_path}")
 
     # Check if the file was already processed.
-    if json_file_path.name.endswith("_clean.json"):
+    if json_file_path.name.endswith("#clean.json"):
         return
-    if json_file_path.name.endswith("_mask_data.json"):
+    if json_file_path.name.endswith("#mask_data.json"):
         return
 
     json_data = json.loads(json_file_path.read_text())
 
     image_path = json_data["image_path"]
     mask_path = json_data["mask_path"]
     original_path = json_data["original_path"]
@@ -136,15 +138,15 @@
     # Copy the merged extended boxes to the reference boxes and grow them once again.
     page_data.reference_boxes = page_data.merged_extended_boxes.copy()
     page_data.grow_boxes(
         scale_len(pre_processor_conf.box_reference_padding), st.BoxType.REFERENCE_BOX
     )
 
     # Write the json file with the cleaned data.
-    json_out_path = json_file_path.parent / f"{json_file_path.stem}_clean.json"
+    json_out_path = json_file_path.parent / f"{json_file_path.stem}#clean.json"
     # Remove the _image_size attribute, because it's a cached value that may be unset.
     page_data_dict = asdict(page_data)
     del page_data_dict["_image_size"]
     json_out_path.write_text(json.dumps(page_data_dict, indent=4))
 
     # Draw the boxes on the image and save it.
     if cache_masks and not cache_masks_ocr:
@@ -180,15 +182,14 @@
     :param mocr: Manga ocr object.
     :param max_box_size: Maximum size of a box in pixels, to consider it for ocr.
     :param ocr_blacklist_pattern: Regex pattern to match against the ocr result.
     :param box_padding: [Optional] Padding to add to the box before running ocr.
     :return: The modified page data and Analytics data.
     """
     base_image = Image.open(page_data.image_path)
-    image_width, image_height = base_image.size
     candidate_small_bubbles = [
         box for box in page_data.boxes if page_data.box_size(box) < max_box_size
     ]
     if not candidate_small_bubbles:
         return page_data, (len(page_data.boxes), (), (), ())
     # Check if the small bubbles only contain symbols.
     # If they do, then they are probably not text.
```

### Comparing `pcleaner-1.7.0/pcleaner/profile_cli.py` & `pcleaner-1.7.1/pcleaner/profile_cli.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner/structures.py` & `pcleaner-1.7.1/pcleaner/structures.py`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/pcleaner.egg-info/PKG-INFO` & `pcleaner-1.7.1/pcleaner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcleaner
-Version: 1.7.0
+Version: 1.7.1
 Summary: An AI-powered tool to clean manga panels.
 Home-page: https://github.com/VoxelCubes/PanelCleaner
 Keywords: image processing,cleaning,text removal,manga,ai,machine learning
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `pcleaner-1.7.0/pcleaner.egg-info/SOURCES.txt` & `pcleaner-1.7.1/pcleaner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcleaner-1.7.0/setup.cfg` & `pcleaner-1.7.1/setup.cfg`

 * *Files identical despite different names*

