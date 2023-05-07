# Comparing `tmp/cityscapesScripts-2.2.1.tar.gz` & `tmp/cityscapesScripts-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cityscapesScripts-2.2.1.tar", last modified: Sat Oct 22 06:08:52 2022, max compression
+gzip compressed data, was "cityscapesScripts-2.2.2.tar", last modified: Sun May  7 12:21:16 2023, max compression
```

## Comparing `cityscapesScripts-2.2.1.tar` & `cityscapesScripts-2.2.2.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2022-10-22 06:08:52.738552 cityscapesScripts-2.2.1/
--rw-r--r--   0 mcordts    (501) staff       (20)    10533 2022-10-22 06:08:52.738800 cityscapesScripts-2.2.1/PKG-INFO
--rw-r--r--   0 mcordts    (501) staff       (20)     9182 2022-10-21 15:37:54.000000 cityscapesScripts-2.2.1/README.md
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2022-10-22 06:08:52.652551 cityscapesScripts-2.2.1/cityscapesScripts.egg-info/
--rw-r--r--   0 mcordts    (501) staff       (20)    10533 2022-10-22 06:08:51.000000 cityscapesScripts-2.2.1/cityscapesScripts.egg-info/PKG-INFO
--rw-r--r--   0 mcordts    (501) staff       (20)     3417 2022-10-22 06:08:51.000000 cityscapesScripts-2.2.1/cityscapesScripts.egg-info/SOURCES.txt
--rw-r--r--   0 mcordts    (501) staff       (20)        1 2022-10-22 06:08:51.000000 cityscapesScripts-2.2.1/cityscapesScripts.egg-info/dependency_links.txt
--rw-r--r--   0 mcordts    (501) staff       (20)      940 2022-10-22 06:08:51.000000 cityscapesScripts-2.2.1/cityscapesScripts.egg-info/entry_points.txt
--rw-r--r--   0 mcordts    (501) staff       (20)       82 2022-10-22 06:08:51.000000 cityscapesScripts-2.2.1/cityscapesScripts.egg-info/requires.txt
--rw-r--r--   0 mcordts    (501) staff       (20)       18 2022-10-22 06:08:51.000000 cityscapesScripts-2.2.1/cityscapesScripts.egg-info/top_level.txt
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2022-10-22 06:08:52.653498 cityscapesScripts-2.2.1/cityscapesscripts/
--rw-r--r--   0 mcordts    (501) staff       (20)        6 2022-10-21 15:37:28.000000 cityscapesScripts-2.2.1/cityscapesscripts/VERSION
--rw-r--r--   0 mcordts    (501) staff       (20)        0 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.1/cityscapesscripts/__init__.py
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2022-10-22 06:08:52.654174 cityscapesScripts-2.2.1/cityscapesscripts/annotation/
--rw-r--r--   0 mcordts    (501) staff       (20)        0 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/__init__.py
--rw-r--r--   0 mcordts    (501) staff       (20)   110764 2020-08-29 16:30:00.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/cityscapesLabelTool.py
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2022-10-22 06:08:52.708577 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/
--rw-r--r--   0 mcordts    (501) staff       (20)     6124 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/back.png
--rw-r--r--   0 mcordts    (501) staff       (20)    12493 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/checked6.png
--rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/checked6_red.png
--rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/clearpolygon.png
--rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/deleteobject.png
--rw-r--r--   0 mcordts    (501) staff       (20)     3391 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/exit.png
--rw-r--r--   0 mcordts    (501) staff       (20)    14178 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/filepath.png
--rw-r--r--   0 mcordts    (501) staff       (20)    13163 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/help19.png
--rw-r--r--   0 mcordts    (501) staff       (20)    11772 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/highlight.png
--rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/layerdown.png
--rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/layerup.png
--rw-r--r--   0 mcordts    (501) staff       (20)     2355 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/minus.png
--rw-r--r--   0 mcordts    (501) staff       (20)     9477 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/modify.png
--rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/newobject.png
--rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/next.png
--rw-r--r--   0 mcordts    (501) staff       (20)     4992 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/open.png
--rw-r--r--   0 mcordts    (501) staff       (20)    10655 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/play.png
--rw-r--r--   0 mcordts    (501) staff       (20)     4004 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/plus.png
--rw-r--r--   0 mcordts    (501) staff       (20)     2739 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/save.png
--rw-r--r--   0 mcordts    (501) staff       (20)     9938 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/screenshot.png
--rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/screenshotToggle.png
--rw-r--r--   0 mcordts    (501) staff       (20)     6454 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/shuffle.png
--rw-r--r--   0 mcordts    (501) staff       (20)     5765 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/undo.png
--rw-r--r--   0 mcordts    (501) staff       (20)    12237 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/zoom.png
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2022-10-22 06:08:52.710386 cityscapesScripts-2.2.1/cityscapesscripts/download/
--rw-r--r--   0 mcordts    (501) staff       (20)        1 2020-02-26 20:37:16.000000 cityscapesScripts-2.2.1/cityscapesscripts/download/__init__.py
--rw-r--r--   0 mcordts    (501) staff       (20)     5931 2020-05-31 12:37:37.000000 cityscapesScripts-2.2.1/cityscapesscripts/download/downloader.py
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2022-10-22 06:08:52.716635 cityscapesScripts-2.2.1/cityscapesscripts/evaluation/
--rw-r--r--   0 mcordts    (501) staff       (20)        0 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/evaluation/__init__.py
--rw-r--r--   0 mcordts    (501) staff       (20)    30177 2020-01-19 19:22:15.000000 cityscapesScripts-2.2.1/cityscapesscripts/evaluation/evalInstanceLevelSemanticLabeling.py
--rw-r--r--   0 mcordts    (501) staff       (20)    49118 2020-10-17 11:45:02.000000 cityscapesScripts-2.2.1/cityscapesscripts/evaluation/evalObjectDetection3D.py
--rw-r--r--   0 mcordts    (501) staff       (20)    15701 2021-01-11 19:50:04.000000 cityscapesScripts-2.2.1/cityscapesscripts/evaluation/evalPanopticSemanticLabeling.py
--rw-r--r--   0 mcordts    (501) staff       (20)    28237 2020-02-16 07:50:37.000000 cityscapesScripts-2.2.1/cityscapesscripts/evaluation/evalPixelLevelSemanticLabeling.py
--rw-r--r--   0 mcordts    (501) staff       (20)     1441 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/evaluation/instance.py
--rw-r--r--   0 mcordts    (501) staff       (20)     1613 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/evaluation/instances2dict.py
--rw-r--r--   0 mcordts    (501) staff       (20)     4963 2020-10-17 08:52:07.000000 cityscapesScripts-2.2.1/cityscapesscripts/evaluation/objectDetectionHelpers.py
--rw-r--r--   0 mcordts    (501) staff       (20)    17475 2020-09-26 16:51:47.000000 cityscapesScripts-2.2.1/cityscapesscripts/evaluation/plot3DResults.py
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2022-10-22 06:08:52.720345 cityscapesScripts-2.2.1/cityscapesscripts/helpers/
--rw-r--r--   0 mcordts    (501) staff       (20)        0 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/helpers/__init__.py
--rw-r--r--   0 mcordts    (501) staff       (20)    14057 2020-10-17 11:45:02.000000 cityscapesScripts-2.2.1/cityscapesscripts/helpers/annotation.py
--rw-r--r--   0 mcordts    (501) staff       (20)    15536 2020-10-02 17:58:21.000000 cityscapesScripts-2.2.1/cityscapesscripts/helpers/box3dImageTransform.py
--rw-r--r--   0 mcordts    (501) staff       (20)     3506 2020-08-29 16:30:00.000000 cityscapesScripts-2.2.1/cityscapesscripts/helpers/csHelpers.py
--rw-r--r--   0 mcordts    (501) staff       (20)    10663 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/helpers/labels.py
--rw-r--r--   0 mcordts    (501) staff       (20)     2550 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/helpers/labels_cityPersons.py
--rw-r--r--   0 mcordts    (501) staff       (20)      186 2020-08-29 16:30:00.000000 cityscapesScripts-2.2.1/cityscapesscripts/helpers/version.py
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2022-10-22 06:08:52.723841 cityscapesScripts-2.2.1/cityscapesscripts/preparation/
--rw-r--r--   0 mcordts    (501) staff       (20)        0 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/preparation/__init__.py
--rw-r--r--   0 mcordts    (501) staff       (20)     7428 2021-01-11 19:50:04.000000 cityscapesScripts-2.2.1/cityscapesscripts/preparation/createPanopticImgs.py
--rw-r--r--   0 mcordts    (501) staff       (20)     2926 2020-01-19 19:22:15.000000 cityscapesScripts-2.2.1/cityscapesscripts/preparation/createTrainIdInstanceImgs.py
--rw-r--r--   0 mcordts    (501) staff       (20)     2757 2020-01-19 19:22:15.000000 cityscapesScripts-2.2.1/cityscapesscripts/preparation/createTrainIdLabelImgs.py
--rw-r--r--   0 mcordts    (501) staff       (20)     7247 2020-01-19 19:22:15.000000 cityscapesScripts-2.2.1/cityscapesscripts/preparation/json2instanceImg.py
--rw-r--r--   0 mcordts    (501) staff       (20)     5069 2020-01-19 19:22:15.000000 cityscapesScripts-2.2.1/cityscapesscripts/preparation/json2labelImg.py
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2022-10-22 06:08:52.724590 cityscapesScripts-2.2.1/cityscapesscripts/viewer/
--rw-r--r--   0 mcordts    (501) staff       (20)        0 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/viewer/__init__.py
--rw-r--r--   0 mcordts    (501) staff       (20)    55045 2020-08-29 16:30:00.000000 cityscapesScripts-2.2.1/cityscapesscripts/viewer/cityscapesViewer.py
-drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2022-10-22 06:08:52.737775 cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/
--rw-r--r--   0 mcordts    (501) staff       (20)     6124 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/back.png
--rw-r--r--   0 mcordts    (501) staff       (20)     7530 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/disp.png
--rw-r--r--   0 mcordts    (501) staff       (20)     3391 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/exit.png
--rw-r--r--   0 mcordts    (501) staff       (20)    14178 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/filepath.png
--rw-r--r--   0 mcordts    (501) staff       (20)    13163 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/help19.png
--rw-r--r--   0 mcordts    (501) staff       (20)    13349 2020-08-29 16:30:00.000000 cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/label.png
--rw-r--r--   0 mcordts    (501) staff       (20)     2355 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/minus.png
--rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/next.png
--rw-r--r--   0 mcordts    (501) staff       (20)     4992 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/open.png
--rw-r--r--   0 mcordts    (501) staff       (20)    10655 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/play.png
--rw-r--r--   0 mcordts    (501) staff       (20)     4004 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/plus.png
--rw-r--r--   0 mcordts    (501) staff       (20)     6454 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/shuffle.png
--rw-r--r--   0 mcordts    (501) staff       (20)    12237 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/zoom.png
--rw-r--r--   0 mcordts    (501) staff       (20)       79 2022-10-22 06:08:52.739231 cityscapesScripts-2.2.1/setup.cfg
--rw-r--r--   0 mcordts    (501) staff       (20)     2889 2022-10-21 15:37:16.000000 cityscapesScripts-2.2.1/setup.py
+drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.138107 cityscapesScripts-2.2.2/
+-rw-r--r--   0 mcordts    (501) staff       (20)     1082 2022-10-21 15:36:58.000000 cityscapesScripts-2.2.2/LICENSE
+-rw-r--r--   0 mcordts    (501) staff       (20)     9564 2023-05-07 12:21:16.138365 cityscapesScripts-2.2.2/PKG-INFO
+-rw-r--r--   0 mcordts    (501) staff       (20)     9182 2022-10-21 15:37:54.000000 cityscapesScripts-2.2.2/README.md
+drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.028571 cityscapesScripts-2.2.2/cityscapesScripts.egg-info/
+-rw-r--r--   0 mcordts    (501) staff       (20)     9564 2023-05-07 12:21:15.000000 cityscapesScripts-2.2.2/cityscapesScripts.egg-info/PKG-INFO
+-rw-r--r--   0 mcordts    (501) staff       (20)     3425 2023-05-07 12:21:15.000000 cityscapesScripts-2.2.2/cityscapesScripts.egg-info/SOURCES.txt
+-rw-r--r--   0 mcordts    (501) staff       (20)        1 2023-05-07 12:21:15.000000 cityscapesScripts-2.2.2/cityscapesScripts.egg-info/dependency_links.txt
+-rw-r--r--   0 mcordts    (501) staff       (20)      939 2023-05-07 12:21:15.000000 cityscapesScripts-2.2.2/cityscapesScripts.egg-info/entry_points.txt
+-rw-r--r--   0 mcordts    (501) staff       (20)       82 2023-05-07 12:21:15.000000 cityscapesScripts-2.2.2/cityscapesScripts.egg-info/requires.txt
+-rw-r--r--   0 mcordts    (501) staff       (20)       18 2023-05-07 12:21:15.000000 cityscapesScripts-2.2.2/cityscapesScripts.egg-info/top_level.txt
+drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.029780 cityscapesScripts-2.2.2/cityscapesscripts/
+-rw-r--r--   0 mcordts    (501) staff       (20)        6 2023-05-07 12:19:22.000000 cityscapesScripts-2.2.2/cityscapesscripts/VERSION
+-rw-r--r--   0 mcordts    (501) staff       (20)        0 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/__init__.py
+drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.030603 cityscapesScripts-2.2.2/cityscapesscripts/annotation/
+-rw-r--r--   0 mcordts    (501) staff       (20)        0 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/__init__.py
+-rw-r--r--   0 mcordts    (501) staff       (20)   110764 2020-08-29 16:30:00.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/cityscapesLabelTool.py
+drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.098692 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/
+-rw-r--r--   0 mcordts    (501) staff       (20)     6124 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/back.png
+-rw-r--r--   0 mcordts    (501) staff       (20)    12493 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/checked6.png
+-rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/checked6_red.png
+-rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/clearpolygon.png
+-rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/deleteobject.png
+-rw-r--r--   0 mcordts    (501) staff       (20)     3391 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/exit.png
+-rw-r--r--   0 mcordts    (501) staff       (20)    14178 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/filepath.png
+-rw-r--r--   0 mcordts    (501) staff       (20)    13163 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/help19.png
+-rw-r--r--   0 mcordts    (501) staff       (20)    11772 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/highlight.png
+-rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/layerdown.png
+-rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/layerup.png
+-rw-r--r--   0 mcordts    (501) staff       (20)     2355 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/minus.png
+-rw-r--r--   0 mcordts    (501) staff       (20)     9477 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/modify.png
+-rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/newobject.png
+-rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/next.png
+-rw-r--r--   0 mcordts    (501) staff       (20)     4992 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/open.png
+-rw-r--r--   0 mcordts    (501) staff       (20)    10655 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/play.png
+-rw-r--r--   0 mcordts    (501) staff       (20)     4004 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/plus.png
+-rw-r--r--   0 mcordts    (501) staff       (20)     2739 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/save.png
+-rw-r--r--   0 mcordts    (501) staff       (20)     9938 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/screenshot.png
+-rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/screenshotToggle.png
+-rw-r--r--   0 mcordts    (501) staff       (20)     6454 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/shuffle.png
+-rw-r--r--   0 mcordts    (501) staff       (20)     5765 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/undo.png
+-rw-r--r--   0 mcordts    (501) staff       (20)    12237 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/zoom.png
+drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.100647 cityscapesScripts-2.2.2/cityscapesscripts/download/
+-rw-r--r--   0 mcordts    (501) staff       (20)        1 2020-02-26 20:37:16.000000 cityscapesScripts-2.2.2/cityscapesscripts/download/__init__.py
+-rw-r--r--   0 mcordts    (501) staff       (20)     5931 2020-05-31 12:37:37.000000 cityscapesScripts-2.2.2/cityscapesscripts/download/downloader.py
+drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.108624 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/
+-rw-r--r--   0 mcordts    (501) staff       (20)        0 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/__init__.py
+-rw-r--r--   0 mcordts    (501) staff       (20)    30171 2023-05-07 12:19:22.000000 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/evalInstanceLevelSemanticLabeling.py
+-rw-r--r--   0 mcordts    (501) staff       (20)    49118 2020-10-17 11:45:02.000000 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/evalObjectDetection3D.py
+-rw-r--r--   0 mcordts    (501) staff       (20)    15701 2021-01-11 19:50:04.000000 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/evalPanopticSemanticLabeling.py
+-rw-r--r--   0 mcordts    (501) staff       (20)    28237 2020-02-16 07:50:37.000000 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/evalPixelLevelSemanticLabeling.py
+-rw-r--r--   0 mcordts    (501) staff       (20)     1441 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/instance.py
+-rw-r--r--   0 mcordts    (501) staff       (20)     1613 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/instances2dict.py
+-rw-r--r--   0 mcordts    (501) staff       (20)     4963 2020-10-17 08:52:07.000000 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/objectDetectionHelpers.py
+-rw-r--r--   0 mcordts    (501) staff       (20)    17475 2020-09-26 16:51:47.000000 cityscapesScripts-2.2.2/cityscapesscripts/evaluation/plot3DResults.py
+drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.117740 cityscapesScripts-2.2.2/cityscapesscripts/helpers/
+-rw-r--r--   0 mcordts    (501) staff       (20)        0 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/helpers/__init__.py
+-rw-r--r--   0 mcordts    (501) staff       (20)    14057 2020-10-17 11:45:02.000000 cityscapesScripts-2.2.2/cityscapesscripts/helpers/annotation.py
+-rw-r--r--   0 mcordts    (501) staff       (20)    15536 2020-10-02 17:58:21.000000 cityscapesScripts-2.2.2/cityscapesscripts/helpers/box3dImageTransform.py
+-rw-r--r--   0 mcordts    (501) staff       (20)     3506 2020-08-29 16:30:00.000000 cityscapesScripts-2.2.2/cityscapesscripts/helpers/csHelpers.py
+-rw-r--r--   0 mcordts    (501) staff       (20)    10663 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/helpers/labels.py
+-rw-r--r--   0 mcordts    (501) staff       (20)     2550 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/helpers/labels_cityPersons.py
+-rw-r--r--   0 mcordts    (501) staff       (20)      186 2020-08-29 16:30:00.000000 cityscapesScripts-2.2.2/cityscapesscripts/helpers/version.py
+drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.122834 cityscapesScripts-2.2.2/cityscapesscripts/preparation/
+-rw-r--r--   0 mcordts    (501) staff       (20)        0 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/preparation/__init__.py
+-rw-r--r--   0 mcordts    (501) staff       (20)     7428 2021-01-11 19:50:04.000000 cityscapesScripts-2.2.2/cityscapesscripts/preparation/createPanopticImgs.py
+-rw-r--r--   0 mcordts    (501) staff       (20)     2926 2020-01-19 19:22:15.000000 cityscapesScripts-2.2.2/cityscapesscripts/preparation/createTrainIdInstanceImgs.py
+-rw-r--r--   0 mcordts    (501) staff       (20)     2757 2020-01-19 19:22:15.000000 cityscapesScripts-2.2.2/cityscapesscripts/preparation/createTrainIdLabelImgs.py
+-rw-r--r--   0 mcordts    (501) staff       (20)     7247 2020-01-19 19:22:15.000000 cityscapesScripts-2.2.2/cityscapesscripts/preparation/json2instanceImg.py
+-rw-r--r--   0 mcordts    (501) staff       (20)     5069 2020-01-19 19:22:15.000000 cityscapesScripts-2.2.2/cityscapesscripts/preparation/json2labelImg.py
+drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.124060 cityscapesScripts-2.2.2/cityscapesscripts/viewer/
+-rw-r--r--   0 mcordts    (501) staff       (20)        0 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/__init__.py
+-rw-r--r--   0 mcordts    (501) staff       (20)    55045 2020-08-29 16:30:00.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/cityscapesViewer.py
+drwxr-xr-x   0 mcordts    (501) staff       (20)        0 2023-05-07 12:21:16.137388 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/
+-rw-r--r--   0 mcordts    (501) staff       (20)     6124 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/back.png
+-rw-r--r--   0 mcordts    (501) staff       (20)     7530 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/disp.png
+-rw-r--r--   0 mcordts    (501) staff       (20)     3391 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/exit.png
+-rw-r--r--   0 mcordts    (501) staff       (20)    14178 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/filepath.png
+-rw-r--r--   0 mcordts    (501) staff       (20)    13163 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/help19.png
+-rw-r--r--   0 mcordts    (501) staff       (20)    13349 2020-08-29 16:30:00.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/label.png
+-rw-r--r--   0 mcordts    (501) staff       (20)     2355 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/minus.png
+-rw-r--r--   0 mcordts    (501) staff       (20)  1050910 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/next.png
+-rw-r--r--   0 mcordts    (501) staff       (20)     4992 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/open.png
+-rw-r--r--   0 mcordts    (501) staff       (20)    10655 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/play.png
+-rw-r--r--   0 mcordts    (501) staff       (20)     4004 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/plus.png
+-rw-r--r--   0 mcordts    (501) staff       (20)     6454 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/shuffle.png
+-rw-r--r--   0 mcordts    (501) staff       (20)    12237 2018-10-14 12:05:08.000000 cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/zoom.png
+-rw-r--r--   0 mcordts    (501) staff       (20)       79 2023-05-07 12:21:16.139241 cityscapesScripts-2.2.2/setup.cfg
+-rw-r--r--   0 mcordts    (501) staff       (20)     2889 2022-10-21 15:37:16.000000 cityscapesScripts-2.2.2/setup.py
```

### Comparing `cityscapesScripts-2.2.1/PKG-INFO` & `cityscapesScripts-2.2.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,132 +1,120 @@
-Metadata-Version: 2.1
-Name: cityscapesScripts
-Version: 2.2.1
-Summary: Scripts for the Cityscapes Dataset
-Home-page: https://github.com/mcordts/cityscapesScripts
-Author: Marius Cordts
-Author-email: mail@cityscapes-dataset.net
-License: https://github.com/mcordts/cityscapesScripts/blob/master/LICENSE
-Description: # The Cityscapes Dataset
-        
-        This repository contains scripts for inspection, preparation, and evaluation of the Cityscapes dataset. This large-scale dataset contains a diverse set of stereo video sequences recorded in street scenes from 50 different cities, with high quality pixel-level annotations of 5 000 frames in addition to a larger set of 20 000 weakly annotated frames.
-        
-        Details and download are available at: www.cityscapes-dataset.com
-        
-        
-        ## Dataset Structure
-        
-        The folder structure of the Cityscapes dataset is as follows:
-        ```
-        {root}/{type}{video}/{split}/{city}/{city}_{seq:0>6}_{frame:0>6}_{type}{ext}
-        ```
-        
-        The meaning of the individual elements is:
-         - `root`  the root folder of the Cityscapes dataset. Many of our scripts check if an environment variable `CITYSCAPES_DATASET` pointing to this folder exists and use this as the default choice.
-         - `type`  the type/modality of data, e.g. `gtFine` for fine ground truth, or `leftImg8bit` for left 8-bit images.
-         - `split` the split, i.e. train/val/test/train_extra/demoVideo. Note that not all kinds of data exist for all splits. Thus, do not be surprised to occasionally find empty folders.
-         - `city`  the city in which this part of the dataset was recorded.
-         - `seq`   the sequence number using 6 digits.
-         - `frame` the frame number using 6 digits. Note that in some cities very few, albeit very long sequences were recorded, while in some cities many short sequences were recorded, of which only the 19th frame is annotated.
-         - `ext`   the extension of the file and optionally a suffix, e.g. `_polygons.json` for ground truth files
-        
-        Possible values of `type`
-         - `gtFine`       the fine annotations, 2975 training, 500 validation, and 1525 testing. This type of annotations is used for validation, testing, and optionally for training. Annotations are encoded using `json` files containing the individual polygons. Additionally, we provide `png` images, where pixel values encode labels. Please refer to `helpers/labels.py` and the scripts in `preparation` for details.
-         - `gtCoarse`     the coarse annotations, available for all training and validation images and for another set of 19998 training images (`train_extra`). These annotations can be used for training, either together with gtFine or alone in a weakly supervised setup.
-         - `gtBbox3d`     3D bounding box annotations of vehicles. Please refer to [Cityscapes 3D (Gählert et al., CVPRW '20)](https://arxiv.org/abs/2006.07864) for details.
-         - `gtBboxCityPersons` pedestrian bounding box annotations, available for all training and validation images. Please refer to `helpers/labels_cityPersons.py` as well as [CityPersons (Zhang et al., CVPR '17)](https://bitbucket.org/shanshanzhang/citypersons) for more details. The four values of a bounding box are (x, y, w, h), where (x, y) is its top-left corner and (w, h) its width and height.
-         - `leftImg8bit`  the left images in 8-bit LDR format. These are the standard annotated images.
-         - `leftImg8bit_blurred`  the left images in 8-bit LDR format with faces and license plates blurred. Please compute results on the original images but use the blurred ones for visualization. We thank [Mapillary](https://www.mapillary.com/) for blurring the images.
-         - `leftImg16bit` the left images in 16-bit HDR format. These images offer 16 bits per pixel of color depth and contain more information, especially in very dark or bright parts of the scene. Warning: The images are stored as 16-bit pngs, which is non-standard and not supported by all libraries.
-         - `rightImg8bit`  the right stereo views in 8-bit LDR format.
-         - `rightImg16bit` the right stereo views in 16-bit HDR format.
-         - `timestamp`     the time of recording in ns. The first frame of each sequence always has a timestamp of 0.
-         - `disparity`     precomputed disparity depth maps. To obtain the disparity values, compute for each pixel p with p > 0: d = ( float(p) - 1. ) / 256., while a value p = 0 is an invalid measurement. Warning: the images are stored as 16-bit pngs, which is non-standard and not supported by all libraries.
-         - `camera`        internal and external camera calibration. For details, please refer to [csCalibration.pdf](docs/csCalibration.pdf)
-         - `vehicle`       vehicle odometry, GPS coordinates, and outside temperature. For details, please refer to [csCalibration.pdf](docs/csCalibration.pdf)
-        
-        More types might be added over time and also not all types are initially available. Please let us know if you need any other meta-data to run your approach.
-        
-        Possible values of `split`
-         - `train`       usually used for training, contains 2975 images with fine and coarse annotations
-         - `val`         should be used for validation of hyper-parameters, contains 500 image with fine and coarse annotations. Can also be used for training.
-         - `test`        used for testing on our evaluation server. The annotations are not public, but we include annotations of ego-vehicle and rectification border for convenience.
-         - `train_extra` can be optionally used for training, contains 19998 images with coarse annotations
-         - `demoVideo`   video sequences that could be used for qualitative evaluation, no annotations are available for these videos
-        
-        
-        ## Scripts
-        
-        ### Installation
-        
-        Install `cityscapesscripts` with `pip`
-        ```
-        python -m pip install cityscapesscripts
-        ```
-        
-        Graphical tools (viewer and label tool) are based on Qt5 and can be installed via
-        ```
-        python -m pip install cityscapesscripts[gui]
-        ```
-        
-        ### Usage
-        
-        The installation installs the cityscapes scripts as a python module named `cityscapesscripts` and exposes the following tools
-        - `csDownload`: Download the cityscapes packages via command line.
-        - `csViewer`: View the images and overlay the annotations.
-        - `csLabelTool`: Tool that we used for labeling.
-        - `csEvalPixelLevelSemanticLabeling`: Evaluate pixel-level semantic labeling results on the validation set. This tool is also used to evaluate the results on the test set.
-        - `csEvalInstanceLevelSemanticLabeling`: Evaluate instance-level semantic labeling results on the validation set. This tool is also used to evaluate the results on the test set.
-        - `csEvalPanopticSemanticLabeling`: Evaluate panoptic segmentation results on the validation set. This tool is also used to evaluate the results on the test set.
-        - `csEvalObjectDetection3d`: Evaluate 3D object detection on the validation set. This tool is also used to evaluate the results on the test set.
-        - `csCreateTrainIdLabelImgs`: Convert annotations in polygonal format to png images with label IDs, where pixels encode "train IDs" that you can define in `labels.py`.
-        - `csCreateTrainIdInstanceImgs`: Convert annotations in polygonal format to png images with instance IDs, where pixels encode instance IDs composed of "train IDs".
-        - `csCreatePanopticImgs`: Convert annotations in standard png format to [COCO panoptic segmentation format](http://cocodataset.org/#format-data).
-        - `csPlot3dDetectionResults`: Visualize 3D object detection evaluation results stored in .json format.
-        
-        
-        ### Package Content
-        
-        The package is structured as follows
-         - `helpers`: helper files that are included by other scripts
-         - `viewer`: view the images and the annotations
-         - `preparation`: convert the ground truth annotations into a format suitable for your approach
-         - `evaluation`: validate your approach
-         - `annotation`: the annotation tool used for labeling the dataset
-         - `download`: downloader for Cityscapes packages
-        
-        Note that all files have a small documentation at the top. Most important files
-         - `helpers/labels.py`: central file defining the IDs of all semantic classes and providing mapping between various class properties.
-         - `helpers/labels_cityPersons.py`: file defining the IDs of all CityPersons pedestrian classes and providing mapping between various class properties.
-         - `setup.py`: run `CYTHONIZE_EVAL= python setup.py build_ext --inplace` to enable cython plugin for faster evaluation. Only tested for Ubuntu.
-        
-        
-        ## Evaluation
-        
-        Once you want to test your method on the test set, please run your approach on the provided test images and submit your results:
-        [Submission Page](www.cityscapes-dataset.com/submit)
-        
-        The result format is described at the top of our evaluation scripts:
-        - [Pixel Level Semantic Labeling](cityscapesscripts/evaluation/evalPixelLevelSemanticLabeling.py)
-        - [Instance Level Semantic Labeling](cityscapesscripts/evaluation/evalInstanceLevelSemanticLabeling.py)
-        - [Panoptic Semantic Labeling](cityscapesscripts/evaluation/evalPanopticSemanticLabeling.py)
-        - [3D Object Detection](cityscapesscripts/evaluation/evalObjectDetection3d.py)
-        
-        Note that our evaluation scripts are included in the scripts folder and can be used to test your approach on the validation set. For further details regarding the submission process, please consult our website.
-        
-        ## License
-        
-        The dataset itself is released under custom [terms and conditions](https://www.cityscapes-dataset.com/license/).
-        
-        The Cityscapes Scripts are released under MIT license as found in the [license file](LICENSE).
-        
-        ## Contact
-        
-        Please feel free to contact us with any questions, suggestions or comments:
-        
-        * Marius Cordts, Mohamed Omran
-        * mail@cityscapes-dataset.net
-        * www.cityscapes-dataset.com
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Provides-Extra: gui
+# The Cityscapes Dataset
+
+This repository contains scripts for inspection, preparation, and evaluation of the Cityscapes dataset. This large-scale dataset contains a diverse set of stereo video sequences recorded in street scenes from 50 different cities, with high quality pixel-level annotations of 5 000 frames in addition to a larger set of 20 000 weakly annotated frames.
+
+Details and download are available at: www.cityscapes-dataset.com
+
+
+## Dataset Structure
+
+The folder structure of the Cityscapes dataset is as follows:
+```
+{root}/{type}{video}/{split}/{city}/{city}_{seq:0>6}_{frame:0>6}_{type}{ext}
+```
+
+The meaning of the individual elements is:
+ - `root`  the root folder of the Cityscapes dataset. Many of our scripts check if an environment variable `CITYSCAPES_DATASET` pointing to this folder exists and use this as the default choice.
+ - `type`  the type/modality of data, e.g. `gtFine` for fine ground truth, or `leftImg8bit` for left 8-bit images.
+ - `split` the split, i.e. train/val/test/train_extra/demoVideo. Note that not all kinds of data exist for all splits. Thus, do not be surprised to occasionally find empty folders.
+ - `city`  the city in which this part of the dataset was recorded.
+ - `seq`   the sequence number using 6 digits.
+ - `frame` the frame number using 6 digits. Note that in some cities very few, albeit very long sequences were recorded, while in some cities many short sequences were recorded, of which only the 19th frame is annotated.
+ - `ext`   the extension of the file and optionally a suffix, e.g. `_polygons.json` for ground truth files
+
+Possible values of `type`
+ - `gtFine`       the fine annotations, 2975 training, 500 validation, and 1525 testing. This type of annotations is used for validation, testing, and optionally for training. Annotations are encoded using `json` files containing the individual polygons. Additionally, we provide `png` images, where pixel values encode labels. Please refer to `helpers/labels.py` and the scripts in `preparation` for details.
+ - `gtCoarse`     the coarse annotations, available for all training and validation images and for another set of 19998 training images (`train_extra`). These annotations can be used for training, either together with gtFine or alone in a weakly supervised setup.
+ - `gtBbox3d`     3D bounding box annotations of vehicles. Please refer to [Cityscapes 3D (Gählert et al., CVPRW '20)](https://arxiv.org/abs/2006.07864) for details.
+ - `gtBboxCityPersons` pedestrian bounding box annotations, available for all training and validation images. Please refer to `helpers/labels_cityPersons.py` as well as [CityPersons (Zhang et al., CVPR '17)](https://bitbucket.org/shanshanzhang/citypersons) for more details. The four values of a bounding box are (x, y, w, h), where (x, y) is its top-left corner and (w, h) its width and height.
+ - `leftImg8bit`  the left images in 8-bit LDR format. These are the standard annotated images.
+ - `leftImg8bit_blurred`  the left images in 8-bit LDR format with faces and license plates blurred. Please compute results on the original images but use the blurred ones for visualization. We thank [Mapillary](https://www.mapillary.com/) for blurring the images.
+ - `leftImg16bit` the left images in 16-bit HDR format. These images offer 16 bits per pixel of color depth and contain more information, especially in very dark or bright parts of the scene. Warning: The images are stored as 16-bit pngs, which is non-standard and not supported by all libraries.
+ - `rightImg8bit`  the right stereo views in 8-bit LDR format.
+ - `rightImg16bit` the right stereo views in 16-bit HDR format.
+ - `timestamp`     the time of recording in ns. The first frame of each sequence always has a timestamp of 0.
+ - `disparity`     precomputed disparity depth maps. To obtain the disparity values, compute for each pixel p with p > 0: d = ( float(p) - 1. ) / 256., while a value p = 0 is an invalid measurement. Warning: the images are stored as 16-bit pngs, which is non-standard and not supported by all libraries.
+ - `camera`        internal and external camera calibration. For details, please refer to [csCalibration.pdf](docs/csCalibration.pdf)
+ - `vehicle`       vehicle odometry, GPS coordinates, and outside temperature. For details, please refer to [csCalibration.pdf](docs/csCalibration.pdf)
+
+More types might be added over time and also not all types are initially available. Please let us know if you need any other meta-data to run your approach.
+
+Possible values of `split`
+ - `train`       usually used for training, contains 2975 images with fine and coarse annotations
+ - `val`         should be used for validation of hyper-parameters, contains 500 image with fine and coarse annotations. Can also be used for training.
+ - `test`        used for testing on our evaluation server. The annotations are not public, but we include annotations of ego-vehicle and rectification border for convenience.
+ - `train_extra` can be optionally used for training, contains 19998 images with coarse annotations
+ - `demoVideo`   video sequences that could be used for qualitative evaluation, no annotations are available for these videos
+
+
+## Scripts
+
+### Installation
+
+Install `cityscapesscripts` with `pip`
+```
+python -m pip install cityscapesscripts
+```
+
+Graphical tools (viewer and label tool) are based on Qt5 and can be installed via
+```
+python -m pip install cityscapesscripts[gui]
+```
+
+### Usage
+
+The installation installs the cityscapes scripts as a python module named `cityscapesscripts` and exposes the following tools
+- `csDownload`: Download the cityscapes packages via command line.
+- `csViewer`: View the images and overlay the annotations.
+- `csLabelTool`: Tool that we used for labeling.
+- `csEvalPixelLevelSemanticLabeling`: Evaluate pixel-level semantic labeling results on the validation set. This tool is also used to evaluate the results on the test set.
+- `csEvalInstanceLevelSemanticLabeling`: Evaluate instance-level semantic labeling results on the validation set. This tool is also used to evaluate the results on the test set.
+- `csEvalPanopticSemanticLabeling`: Evaluate panoptic segmentation results on the validation set. This tool is also used to evaluate the results on the test set.
+- `csEvalObjectDetection3d`: Evaluate 3D object detection on the validation set. This tool is also used to evaluate the results on the test set.
+- `csCreateTrainIdLabelImgs`: Convert annotations in polygonal format to png images with label IDs, where pixels encode "train IDs" that you can define in `labels.py`.
+- `csCreateTrainIdInstanceImgs`: Convert annotations in polygonal format to png images with instance IDs, where pixels encode instance IDs composed of "train IDs".
+- `csCreatePanopticImgs`: Convert annotations in standard png format to [COCO panoptic segmentation format](http://cocodataset.org/#format-data).
+- `csPlot3dDetectionResults`: Visualize 3D object detection evaluation results stored in .json format.
+
+
+### Package Content
+
+The package is structured as follows
+ - `helpers`: helper files that are included by other scripts
+ - `viewer`: view the images and the annotations
+ - `preparation`: convert the ground truth annotations into a format suitable for your approach
+ - `evaluation`: validate your approach
+ - `annotation`: the annotation tool used for labeling the dataset
+ - `download`: downloader for Cityscapes packages
+
+Note that all files have a small documentation at the top. Most important files
+ - `helpers/labels.py`: central file defining the IDs of all semantic classes and providing mapping between various class properties.
+ - `helpers/labels_cityPersons.py`: file defining the IDs of all CityPersons pedestrian classes and providing mapping between various class properties.
+ - `setup.py`: run `CYTHONIZE_EVAL= python setup.py build_ext --inplace` to enable cython plugin for faster evaluation. Only tested for Ubuntu.
+
+
+## Evaluation
+
+Once you want to test your method on the test set, please run your approach on the provided test images and submit your results:
+[Submission Page](www.cityscapes-dataset.com/submit)
+
+The result format is described at the top of our evaluation scripts:
+- [Pixel Level Semantic Labeling](cityscapesscripts/evaluation/evalPixelLevelSemanticLabeling.py)
+- [Instance Level Semantic Labeling](cityscapesscripts/evaluation/evalInstanceLevelSemanticLabeling.py)
+- [Panoptic Semantic Labeling](cityscapesscripts/evaluation/evalPanopticSemanticLabeling.py)
+- [3D Object Detection](cityscapesscripts/evaluation/evalObjectDetection3d.py)
+
+Note that our evaluation scripts are included in the scripts folder and can be used to test your approach on the validation set. For further details regarding the submission process, please consult our website.
+
+## License
+
+The dataset itself is released under custom [terms and conditions](https://www.cityscapes-dataset.com/license/).
+
+The Cityscapes Scripts are released under MIT license as found in the [license file](LICENSE).
+
+## Contact
+
+Please feel free to contact us with any questions, suggestions or comments:
+
+* Marius Cordts, Mohamed Omran
+* mail@cityscapes-dataset.net
+* www.cityscapes-dataset.com
```

### Comparing `cityscapesScripts-2.2.1/README.md` & `cityscapesScripts-2.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: cityscapesScripts
+Version: 2.2.2
+Summary: Scripts for the Cityscapes Dataset
+Home-page: https://github.com/mcordts/cityscapesScripts
+Author: Marius Cordts
+Author-email: mail@cityscapes-dataset.net
+License: https://github.com/mcordts/cityscapesScripts/blob/master/LICENSE
+Description-Content-Type: text/markdown
+Provides-Extra: gui
+License-File: LICENSE
+
 # The Cityscapes Dataset
 
 This repository contains scripts for inspection, preparation, and evaluation of the Cityscapes dataset. This large-scale dataset contains a diverse set of stereo video sequences recorded in street scenes from 50 different cities, with high quality pixel-level annotations of 5 000 frames in addition to a larger set of 20 000 weakly annotated frames.
 
 Details and download are available at: www.cityscapes-dataset.com
```

### Comparing `cityscapesScripts-2.2.1/cityscapesScripts.egg-info/PKG-INFO` & `cityscapesScripts-2.2.2/cityscapesScripts.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,132 +1,132 @@
 Metadata-Version: 2.1
 Name: cityscapesScripts
-Version: 2.2.1
+Version: 2.2.2
 Summary: Scripts for the Cityscapes Dataset
 Home-page: https://github.com/mcordts/cityscapesScripts
 Author: Marius Cordts
 Author-email: mail@cityscapes-dataset.net
 License: https://github.com/mcordts/cityscapesScripts/blob/master/LICENSE
-Description: # The Cityscapes Dataset
-        
-        This repository contains scripts for inspection, preparation, and evaluation of the Cityscapes dataset. This large-scale dataset contains a diverse set of stereo video sequences recorded in street scenes from 50 different cities, with high quality pixel-level annotations of 5 000 frames in addition to a larger set of 20 000 weakly annotated frames.
-        
-        Details and download are available at: www.cityscapes-dataset.com
-        
-        
-        ## Dataset Structure
-        
-        The folder structure of the Cityscapes dataset is as follows:
-        ```
-        {root}/{type}{video}/{split}/{city}/{city}_{seq:0>6}_{frame:0>6}_{type}{ext}
-        ```
-        
-        The meaning of the individual elements is:
-         - `root`  the root folder of the Cityscapes dataset. Many of our scripts check if an environment variable `CITYSCAPES_DATASET` pointing to this folder exists and use this as the default choice.
-         - `type`  the type/modality of data, e.g. `gtFine` for fine ground truth, or `leftImg8bit` for left 8-bit images.
-         - `split` the split, i.e. train/val/test/train_extra/demoVideo. Note that not all kinds of data exist for all splits. Thus, do not be surprised to occasionally find empty folders.
-         - `city`  the city in which this part of the dataset was recorded.
-         - `seq`   the sequence number using 6 digits.
-         - `frame` the frame number using 6 digits. Note that in some cities very few, albeit very long sequences were recorded, while in some cities many short sequences were recorded, of which only the 19th frame is annotated.
-         - `ext`   the extension of the file and optionally a suffix, e.g. `_polygons.json` for ground truth files
-        
-        Possible values of `type`
-         - `gtFine`       the fine annotations, 2975 training, 500 validation, and 1525 testing. This type of annotations is used for validation, testing, and optionally for training. Annotations are encoded using `json` files containing the individual polygons. Additionally, we provide `png` images, where pixel values encode labels. Please refer to `helpers/labels.py` and the scripts in `preparation` for details.
-         - `gtCoarse`     the coarse annotations, available for all training and validation images and for another set of 19998 training images (`train_extra`). These annotations can be used for training, either together with gtFine or alone in a weakly supervised setup.
-         - `gtBbox3d`     3D bounding box annotations of vehicles. Please refer to [Cityscapes 3D (Gählert et al., CVPRW '20)](https://arxiv.org/abs/2006.07864) for details.
-         - `gtBboxCityPersons` pedestrian bounding box annotations, available for all training and validation images. Please refer to `helpers/labels_cityPersons.py` as well as [CityPersons (Zhang et al., CVPR '17)](https://bitbucket.org/shanshanzhang/citypersons) for more details. The four values of a bounding box are (x, y, w, h), where (x, y) is its top-left corner and (w, h) its width and height.
-         - `leftImg8bit`  the left images in 8-bit LDR format. These are the standard annotated images.
-         - `leftImg8bit_blurred`  the left images in 8-bit LDR format with faces and license plates blurred. Please compute results on the original images but use the blurred ones for visualization. We thank [Mapillary](https://www.mapillary.com/) for blurring the images.
-         - `leftImg16bit` the left images in 16-bit HDR format. These images offer 16 bits per pixel of color depth and contain more information, especially in very dark or bright parts of the scene. Warning: The images are stored as 16-bit pngs, which is non-standard and not supported by all libraries.
-         - `rightImg8bit`  the right stereo views in 8-bit LDR format.
-         - `rightImg16bit` the right stereo views in 16-bit HDR format.
-         - `timestamp`     the time of recording in ns. The first frame of each sequence always has a timestamp of 0.
-         - `disparity`     precomputed disparity depth maps. To obtain the disparity values, compute for each pixel p with p > 0: d = ( float(p) - 1. ) / 256., while a value p = 0 is an invalid measurement. Warning: the images are stored as 16-bit pngs, which is non-standard and not supported by all libraries.
-         - `camera`        internal and external camera calibration. For details, please refer to [csCalibration.pdf](docs/csCalibration.pdf)
-         - `vehicle`       vehicle odometry, GPS coordinates, and outside temperature. For details, please refer to [csCalibration.pdf](docs/csCalibration.pdf)
-        
-        More types might be added over time and also not all types are initially available. Please let us know if you need any other meta-data to run your approach.
-        
-        Possible values of `split`
-         - `train`       usually used for training, contains 2975 images with fine and coarse annotations
-         - `val`         should be used for validation of hyper-parameters, contains 500 image with fine and coarse annotations. Can also be used for training.
-         - `test`        used for testing on our evaluation server. The annotations are not public, but we include annotations of ego-vehicle and rectification border for convenience.
-         - `train_extra` can be optionally used for training, contains 19998 images with coarse annotations
-         - `demoVideo`   video sequences that could be used for qualitative evaluation, no annotations are available for these videos
-        
-        
-        ## Scripts
-        
-        ### Installation
-        
-        Install `cityscapesscripts` with `pip`
-        ```
-        python -m pip install cityscapesscripts
-        ```
-        
-        Graphical tools (viewer and label tool) are based on Qt5 and can be installed via
-        ```
-        python -m pip install cityscapesscripts[gui]
-        ```
-        
-        ### Usage
-        
-        The installation installs the cityscapes scripts as a python module named `cityscapesscripts` and exposes the following tools
-        - `csDownload`: Download the cityscapes packages via command line.
-        - `csViewer`: View the images and overlay the annotations.
-        - `csLabelTool`: Tool that we used for labeling.
-        - `csEvalPixelLevelSemanticLabeling`: Evaluate pixel-level semantic labeling results on the validation set. This tool is also used to evaluate the results on the test set.
-        - `csEvalInstanceLevelSemanticLabeling`: Evaluate instance-level semantic labeling results on the validation set. This tool is also used to evaluate the results on the test set.
-        - `csEvalPanopticSemanticLabeling`: Evaluate panoptic segmentation results on the validation set. This tool is also used to evaluate the results on the test set.
-        - `csEvalObjectDetection3d`: Evaluate 3D object detection on the validation set. This tool is also used to evaluate the results on the test set.
-        - `csCreateTrainIdLabelImgs`: Convert annotations in polygonal format to png images with label IDs, where pixels encode "train IDs" that you can define in `labels.py`.
-        - `csCreateTrainIdInstanceImgs`: Convert annotations in polygonal format to png images with instance IDs, where pixels encode instance IDs composed of "train IDs".
-        - `csCreatePanopticImgs`: Convert annotations in standard png format to [COCO panoptic segmentation format](http://cocodataset.org/#format-data).
-        - `csPlot3dDetectionResults`: Visualize 3D object detection evaluation results stored in .json format.
-        
-        
-        ### Package Content
-        
-        The package is structured as follows
-         - `helpers`: helper files that are included by other scripts
-         - `viewer`: view the images and the annotations
-         - `preparation`: convert the ground truth annotations into a format suitable for your approach
-         - `evaluation`: validate your approach
-         - `annotation`: the annotation tool used for labeling the dataset
-         - `download`: downloader for Cityscapes packages
-        
-        Note that all files have a small documentation at the top. Most important files
-         - `helpers/labels.py`: central file defining the IDs of all semantic classes and providing mapping between various class properties.
-         - `helpers/labels_cityPersons.py`: file defining the IDs of all CityPersons pedestrian classes and providing mapping between various class properties.
-         - `setup.py`: run `CYTHONIZE_EVAL= python setup.py build_ext --inplace` to enable cython plugin for faster evaluation. Only tested for Ubuntu.
-        
-        
-        ## Evaluation
-        
-        Once you want to test your method on the test set, please run your approach on the provided test images and submit your results:
-        [Submission Page](www.cityscapes-dataset.com/submit)
-        
-        The result format is described at the top of our evaluation scripts:
-        - [Pixel Level Semantic Labeling](cityscapesscripts/evaluation/evalPixelLevelSemanticLabeling.py)
-        - [Instance Level Semantic Labeling](cityscapesscripts/evaluation/evalInstanceLevelSemanticLabeling.py)
-        - [Panoptic Semantic Labeling](cityscapesscripts/evaluation/evalPanopticSemanticLabeling.py)
-        - [3D Object Detection](cityscapesscripts/evaluation/evalObjectDetection3d.py)
-        
-        Note that our evaluation scripts are included in the scripts folder and can be used to test your approach on the validation set. For further details regarding the submission process, please consult our website.
-        
-        ## License
-        
-        The dataset itself is released under custom [terms and conditions](https://www.cityscapes-dataset.com/license/).
-        
-        The Cityscapes Scripts are released under MIT license as found in the [license file](LICENSE).
-        
-        ## Contact
-        
-        Please feel free to contact us with any questions, suggestions or comments:
-        
-        * Marius Cordts, Mohamed Omran
-        * mail@cityscapes-dataset.net
-        * www.cityscapes-dataset.com
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: gui
+License-File: LICENSE
+
+# The Cityscapes Dataset
+
+This repository contains scripts for inspection, preparation, and evaluation of the Cityscapes dataset. This large-scale dataset contains a diverse set of stereo video sequences recorded in street scenes from 50 different cities, with high quality pixel-level annotations of 5 000 frames in addition to a larger set of 20 000 weakly annotated frames.
+
+Details and download are available at: www.cityscapes-dataset.com
+
+
+## Dataset Structure
+
+The folder structure of the Cityscapes dataset is as follows:
+```
+{root}/{type}{video}/{split}/{city}/{city}_{seq:0>6}_{frame:0>6}_{type}{ext}
+```
+
+The meaning of the individual elements is:
+ - `root`  the root folder of the Cityscapes dataset. Many of our scripts check if an environment variable `CITYSCAPES_DATASET` pointing to this folder exists and use this as the default choice.
+ - `type`  the type/modality of data, e.g. `gtFine` for fine ground truth, or `leftImg8bit` for left 8-bit images.
+ - `split` the split, i.e. train/val/test/train_extra/demoVideo. Note that not all kinds of data exist for all splits. Thus, do not be surprised to occasionally find empty folders.
+ - `city`  the city in which this part of the dataset was recorded.
+ - `seq`   the sequence number using 6 digits.
+ - `frame` the frame number using 6 digits. Note that in some cities very few, albeit very long sequences were recorded, while in some cities many short sequences were recorded, of which only the 19th frame is annotated.
+ - `ext`   the extension of the file and optionally a suffix, e.g. `_polygons.json` for ground truth files
+
+Possible values of `type`
+ - `gtFine`       the fine annotations, 2975 training, 500 validation, and 1525 testing. This type of annotations is used for validation, testing, and optionally for training. Annotations are encoded using `json` files containing the individual polygons. Additionally, we provide `png` images, where pixel values encode labels. Please refer to `helpers/labels.py` and the scripts in `preparation` for details.
+ - `gtCoarse`     the coarse annotations, available for all training and validation images and for another set of 19998 training images (`train_extra`). These annotations can be used for training, either together with gtFine or alone in a weakly supervised setup.
+ - `gtBbox3d`     3D bounding box annotations of vehicles. Please refer to [Cityscapes 3D (Gählert et al., CVPRW '20)](https://arxiv.org/abs/2006.07864) for details.
+ - `gtBboxCityPersons` pedestrian bounding box annotations, available for all training and validation images. Please refer to `helpers/labels_cityPersons.py` as well as [CityPersons (Zhang et al., CVPR '17)](https://bitbucket.org/shanshanzhang/citypersons) for more details. The four values of a bounding box are (x, y, w, h), where (x, y) is its top-left corner and (w, h) its width and height.
+ - `leftImg8bit`  the left images in 8-bit LDR format. These are the standard annotated images.
+ - `leftImg8bit_blurred`  the left images in 8-bit LDR format with faces and license plates blurred. Please compute results on the original images but use the blurred ones for visualization. We thank [Mapillary](https://www.mapillary.com/) for blurring the images.
+ - `leftImg16bit` the left images in 16-bit HDR format. These images offer 16 bits per pixel of color depth and contain more information, especially in very dark or bright parts of the scene. Warning: The images are stored as 16-bit pngs, which is non-standard and not supported by all libraries.
+ - `rightImg8bit`  the right stereo views in 8-bit LDR format.
+ - `rightImg16bit` the right stereo views in 16-bit HDR format.
+ - `timestamp`     the time of recording in ns. The first frame of each sequence always has a timestamp of 0.
+ - `disparity`     precomputed disparity depth maps. To obtain the disparity values, compute for each pixel p with p > 0: d = ( float(p) - 1. ) / 256., while a value p = 0 is an invalid measurement. Warning: the images are stored as 16-bit pngs, which is non-standard and not supported by all libraries.
+ - `camera`        internal and external camera calibration. For details, please refer to [csCalibration.pdf](docs/csCalibration.pdf)
+ - `vehicle`       vehicle odometry, GPS coordinates, and outside temperature. For details, please refer to [csCalibration.pdf](docs/csCalibration.pdf)
+
+More types might be added over time and also not all types are initially available. Please let us know if you need any other meta-data to run your approach.
+
+Possible values of `split`
+ - `train`       usually used for training, contains 2975 images with fine and coarse annotations
+ - `val`         should be used for validation of hyper-parameters, contains 500 image with fine and coarse annotations. Can also be used for training.
+ - `test`        used for testing on our evaluation server. The annotations are not public, but we include annotations of ego-vehicle and rectification border for convenience.
+ - `train_extra` can be optionally used for training, contains 19998 images with coarse annotations
+ - `demoVideo`   video sequences that could be used for qualitative evaluation, no annotations are available for these videos
+
+
+## Scripts
+
+### Installation
+
+Install `cityscapesscripts` with `pip`
+```
+python -m pip install cityscapesscripts
+```
+
+Graphical tools (viewer and label tool) are based on Qt5 and can be installed via
+```
+python -m pip install cityscapesscripts[gui]
+```
+
+### Usage
+
+The installation installs the cityscapes scripts as a python module named `cityscapesscripts` and exposes the following tools
+- `csDownload`: Download the cityscapes packages via command line.
+- `csViewer`: View the images and overlay the annotations.
+- `csLabelTool`: Tool that we used for labeling.
+- `csEvalPixelLevelSemanticLabeling`: Evaluate pixel-level semantic labeling results on the validation set. This tool is also used to evaluate the results on the test set.
+- `csEvalInstanceLevelSemanticLabeling`: Evaluate instance-level semantic labeling results on the validation set. This tool is also used to evaluate the results on the test set.
+- `csEvalPanopticSemanticLabeling`: Evaluate panoptic segmentation results on the validation set. This tool is also used to evaluate the results on the test set.
+- `csEvalObjectDetection3d`: Evaluate 3D object detection on the validation set. This tool is also used to evaluate the results on the test set.
+- `csCreateTrainIdLabelImgs`: Convert annotations in polygonal format to png images with label IDs, where pixels encode "train IDs" that you can define in `labels.py`.
+- `csCreateTrainIdInstanceImgs`: Convert annotations in polygonal format to png images with instance IDs, where pixels encode instance IDs composed of "train IDs".
+- `csCreatePanopticImgs`: Convert annotations in standard png format to [COCO panoptic segmentation format](http://cocodataset.org/#format-data).
+- `csPlot3dDetectionResults`: Visualize 3D object detection evaluation results stored in .json format.
+
+
+### Package Content
+
+The package is structured as follows
+ - `helpers`: helper files that are included by other scripts
+ - `viewer`: view the images and the annotations
+ - `preparation`: convert the ground truth annotations into a format suitable for your approach
+ - `evaluation`: validate your approach
+ - `annotation`: the annotation tool used for labeling the dataset
+ - `download`: downloader for Cityscapes packages
+
+Note that all files have a small documentation at the top. Most important files
+ - `helpers/labels.py`: central file defining the IDs of all semantic classes and providing mapping between various class properties.
+ - `helpers/labels_cityPersons.py`: file defining the IDs of all CityPersons pedestrian classes and providing mapping between various class properties.
+ - `setup.py`: run `CYTHONIZE_EVAL= python setup.py build_ext --inplace` to enable cython plugin for faster evaluation. Only tested for Ubuntu.
+
+
+## Evaluation
+
+Once you want to test your method on the test set, please run your approach on the provided test images and submit your results:
+[Submission Page](www.cityscapes-dataset.com/submit)
+
+The result format is described at the top of our evaluation scripts:
+- [Pixel Level Semantic Labeling](cityscapesscripts/evaluation/evalPixelLevelSemanticLabeling.py)
+- [Instance Level Semantic Labeling](cityscapesscripts/evaluation/evalInstanceLevelSemanticLabeling.py)
+- [Panoptic Semantic Labeling](cityscapesscripts/evaluation/evalPanopticSemanticLabeling.py)
+- [3D Object Detection](cityscapesscripts/evaluation/evalObjectDetection3d.py)
+
+Note that our evaluation scripts are included in the scripts folder and can be used to test your approach on the validation set. For further details regarding the submission process, please consult our website.
+
+## License
+
+The dataset itself is released under custom [terms and conditions](https://www.cityscapes-dataset.com/license/).
+
+The Cityscapes Scripts are released under MIT license as found in the [license file](LICENSE).
+
+## Contact
+
+Please feel free to contact us with any questions, suggestions or comments:
+
+* Marius Cordts, Mohamed Omran
+* mail@cityscapes-dataset.net
+* www.cityscapes-dataset.com
```

### Comparing `cityscapesScripts-2.2.1/cityscapesScripts.egg-info/SOURCES.txt` & `cityscapesScripts-2.2.2/cityscapesScripts.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 cityscapesScripts.egg-info/PKG-INFO
 cityscapesScripts.egg-info/SOURCES.txt
 cityscapesScripts.egg-info/dependency_links.txt
 cityscapesScripts.egg-info/entry_points.txt
```

### Comparing `cityscapesScripts-2.2.1/cityscapesScripts.egg-info/entry_points.txt` & `cityscapesScripts-2.2.2/cityscapesScripts.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 csEvalPanopticSemanticLabeling = cityscapesscripts.evaluation.evalPanopticSemanticLabeling:main
 csEvalPixelLevelSemanticLabeling = cityscapesscripts.evaluation.evalPixelLevelSemanticLabeling:main
 csPlot3dDetectionResults = cityscapesscripts.evaluation.plot3dResults:main
 
 [gui_scripts]
 csLabelTool = cityscapesscripts.annotation.cityscapesLabelTool:main [gui]
 csViewer = cityscapesscripts.viewer.cityscapesViewer:main [gui]
-
```

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/cityscapesLabelTool.py` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/cityscapesLabelTool.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/back.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/back.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/checked6.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/checked6.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/checked6_red.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/checked6_red.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/clearpolygon.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/clearpolygon.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/deleteobject.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/deleteobject.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/exit.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/exit.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/filepath.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/filepath.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/help19.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/help19.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/highlight.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/highlight.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/layerdown.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/layerdown.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/layerup.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/layerup.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/minus.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/minus.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/modify.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/modify.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/newobject.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/newobject.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/next.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/next.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/open.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/open.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/play.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/play.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/plus.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/plus.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/save.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/save.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/screenshot.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/screenshot.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/screenshotToggle.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/screenshotToggle.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/shuffle.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/shuffle.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/undo.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/undo.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/annotation/icons/zoom.png` & `cityscapesScripts-2.2.2/cityscapesscripts/annotation/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/download/downloader.py` & `cityscapesScripts-2.2.2/cityscapesscripts/download/downloader.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/evaluation/evalInstanceLevelSemanticLabeling.py` & `cityscapesScripts-2.2.2/cityscapesscripts/evaluation/evalInstanceLevelSemanticLabeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,15 +387,15 @@
     if len(distThs) != len(minRegionSizes):
         printError("Number of distance thresholds and region sizes different")
     if len(distThs) != len(distConfs):
         printError("Number of distance thresholds and confidences different")
 
     # Here we hold the results
     # First dimension is class, second overlap
-    ap = np.zeros( (len(distThs) , len(args.instLabels) , len(overlaps)) , np.float )
+    ap = np.zeros( (len(distThs) , len(args.instLabels) , len(overlaps)) , float )
 
     for dI,(minRegionSize,distanceTh,distanceConf) in enumerate(zip(minRegionSizes,distThs,distConfs)):
         for (oI,overlapTh) in enumerate(overlaps):
             for (lI,labelName) in enumerate(args.instLabels):
                 y_true   = np.empty( 0 )
                 y_score  = np.empty( 0 )
                 # count hard false negatives
@@ -413,15 +413,15 @@
                     if gtInstances:
                         haveGt = True
                     if predInstances:
                         havePred = True
 
                     curTrue  = np.ones ( len(gtInstances) )
                     curScore = np.ones ( len(gtInstances) ) * (-float("inf"))
-                    curMatch = np.zeros( len(gtInstances) , dtype=np.bool )
+                    curMatch = np.zeros( len(gtInstances) , dtype=bool )
 
                     # collect matches
                     for (gtI,gt) in enumerate(gtInstances):
                         foundMatch = False
                         for pred in gt["matchedPred"]:
                             overlap = float(pred["intersection"]) / (gt["pixelCount"]+pred["pixelCount"]-pred["intersection"])
                             if overlap > overlapTh:
```

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/evaluation/evalObjectDetection3D.py` & `cityscapesScripts-2.2.2/cityscapesscripts/evaluation/evalObjectDetection3D.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/evaluation/evalPanopticSemanticLabeling.py` & `cityscapesScripts-2.2.2/cityscapesscripts/evaluation/evalPanopticSemanticLabeling.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/evaluation/evalPixelLevelSemanticLabeling.py` & `cityscapesScripts-2.2.2/cityscapesscripts/evaluation/evalPixelLevelSemanticLabeling.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/evaluation/instance.py` & `cityscapesScripts-2.2.2/cityscapesscripts/evaluation/instance.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/evaluation/instances2dict.py` & `cityscapesScripts-2.2.2/cityscapesscripts/evaluation/instances2dict.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/evaluation/objectDetectionHelpers.py` & `cityscapesScripts-2.2.2/cityscapesscripts/evaluation/objectDetectionHelpers.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/evaluation/plot3DResults.py` & `cityscapesScripts-2.2.2/cityscapesscripts/evaluation/plot3DResults.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/helpers/annotation.py` & `cityscapesScripts-2.2.2/cityscapesscripts/helpers/annotation.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/helpers/box3dImageTransform.py` & `cityscapesScripts-2.2.2/cityscapesscripts/helpers/box3dImageTransform.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/helpers/csHelpers.py` & `cityscapesScripts-2.2.2/cityscapesscripts/helpers/csHelpers.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/helpers/labels.py` & `cityscapesScripts-2.2.2/cityscapesscripts/helpers/labels.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/helpers/labels_cityPersons.py` & `cityscapesScripts-2.2.2/cityscapesscripts/helpers/labels_cityPersons.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/preparation/createPanopticImgs.py` & `cityscapesScripts-2.2.2/cityscapesscripts/preparation/createPanopticImgs.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/preparation/createTrainIdInstanceImgs.py` & `cityscapesScripts-2.2.2/cityscapesscripts/preparation/createTrainIdInstanceImgs.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/preparation/createTrainIdLabelImgs.py` & `cityscapesScripts-2.2.2/cityscapesscripts/preparation/createTrainIdLabelImgs.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/preparation/json2instanceImg.py` & `cityscapesScripts-2.2.2/cityscapesscripts/preparation/json2instanceImg.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/preparation/json2labelImg.py` & `cityscapesScripts-2.2.2/cityscapesscripts/preparation/json2labelImg.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/viewer/cityscapesViewer.py` & `cityscapesScripts-2.2.2/cityscapesscripts/viewer/cityscapesViewer.py`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/back.png` & `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/back.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/disp.png` & `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/disp.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/exit.png` & `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/exit.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/filepath.png` & `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/filepath.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/help19.png` & `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/help19.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/label.png` & `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/label.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/minus.png` & `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/minus.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/next.png` & `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/next.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/open.png` & `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/open.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/play.png` & `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/play.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/plus.png` & `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/plus.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/shuffle.png` & `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/shuffle.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/cityscapesscripts/viewer/icons/zoom.png` & `cityscapesScripts-2.2.2/cityscapesscripts/viewer/icons/zoom.png`

 * *Files identical despite different names*

### Comparing `cityscapesScripts-2.2.1/setup.py` & `cityscapesScripts-2.2.2/setup.py`

 * *Files identical despite different names*

