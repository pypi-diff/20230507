# Comparing `tmp/edit-anything-0.0.4.tar.gz` & `tmp/edit-anything-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edit-anything-0.0.4.tar", last modified: Sat May  6 08:38:04 2023, max compression
+gzip compressed data, was "dist/edit-anything-0.0.5.tar", last modified: Sun May  7 08:57:23 2023, max compression
```

## Comparing `edit-anything-0.0.4.tar` & `edit-anything-0.0.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.557640 edit-anything-0.0.4/
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)       52 2023-05-06 07:21:01.000000 edit-anything-0.0.4/MANIFEST.in
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)      661 2023-05-06 08:38:04.557640 edit-anything-0.0.4/PKG-INFO
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)      361 2023-05-06 07:21:01.000000 edit-anything-0.0.4/README.md
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/edit_anything.egg-info/
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)      661 2023-05-06 08:38:04.000000 edit-anything-0.0.4/edit_anything.egg-info/PKG-INFO
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     1683 2023-05-06 08:38:04.000000 edit-anything-0.0.4/edit_anything.egg-info/SOURCES.txt
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        1 2023-05-06 08:38:04.000000 edit-anything-0.0.4/edit_anything.egg-info/dependency_links.txt
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)       54 2023-05-06 08:38:04.000000 edit-anything-0.0.4/edit_anything.egg-info/entry_points.txt
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        1 2023-05-06 08:34:08.000000 edit-anything-0.0.4/edit_anything.egg-info/not-zip-safe
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)      129 2023-05-06 08:38:04.000000 edit-anything-0.0.4/edit_anything.egg-info/requires.txt
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)       10 2023-05-06 08:38:04.000000 edit-anything-0.0.4/edit_anything.egg-info/top_level.txt
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/__init__.py
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/backend/
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/__init__.py
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/backend/constant/
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/constant/__init__.py
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)      160 2023-05-06 07:42:14.000000 edit-anything-0.0.4/fastmodel/backend/constant/biz_constants.py
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/backend/domain/
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/domain/__init__.py
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/backend/domain/dto/
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/domain/dto/__init__.py
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)      174 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/domain/dto/req_classes.py
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)      124 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/domain/dto/rsp_classes.py
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/backend/exception/
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        1 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/exception/__init__.py
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     1221 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/exception/exceptions.py
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/backend/inference/
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/inference/__init__.py
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     1160 2023-05-06 08:12:38.000000 edit-anything-0.0.4/fastmodel/backend/inference/inference.py
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/backend/process/
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/process/__init__.py
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)       65 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/process/cv_process.py
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/backend/util/
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/util/__init__.py
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     3118 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/util/file.py
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     2066 2023-05-06 08:12:38.000000 edit-anything-0.0.4/fastmodel/backend/util/img_util.py
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     1197 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/util/str_util.py
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/frontend/
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/__init__.py
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.557640 edit-anything-0.0.4/fastmodel/frontend/edit-anything/
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.557640 edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/css/
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)    50507 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/css/801e8f75.css
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)   101568 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/css/db720fc8.css
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.557640 edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/img/
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)    10462 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/img/favicon.ico
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)   163424 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/img/low-salary.de80db91.jpg
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)      697 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/index.html
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.557640 edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)   834928 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/764.d32bc368.js
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     2272 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/764.d32bc368.js.LICENSE.txt
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)    49531 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/antd.a691f5d1.js
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)    39046 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/main.7d537378.js
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     2226 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/runtime~main.0144593e.js
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/frontend/edit-anything/tmp/
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/frontend/edit-anything/tmp/img/
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.557640 edit-anything-0.0.4/fastmodel/frontend/edit-anything/tmp/img/in/
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:12:38.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/tmp/img/in/a.txt
-drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.557640 edit-anything-0.0.4/fastmodel/frontend/edit-anything/tmp/img/out/
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:12:38.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/tmp/img/out/a.txt
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     3425 2023-05-06 08:33:23.000000 edit-anything-0.0.4/fastmodel/main.py
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)       38 2023-05-06 08:38:04.557640 edit-anything-0.0.4/setup.cfg
--rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     1104 2023-05-06 08:36:52.000000 edit-anything-0.0.4/setup.py
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.892284 edit-anything-0.0.5/
+-rw-r--r--   0 arkmon     (501) staff       (20)       52 2023-05-07 03:41:35.000000 edit-anything-0.0.5/MANIFEST.in
+-rw-r--r--   0 arkmon     (501) staff       (20)      929 2023-05-07 08:57:23.891984 edit-anything-0.0.5/PKG-INFO
+-rw-r--r--   0 arkmon     (501) staff       (20)      363 2023-05-07 03:41:35.000000 edit-anything-0.0.5/README.md
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.877708 edit-anything-0.0.5/edit_anything.egg-info/
+-rw-r--r--   0 arkmon     (501) staff       (20)      929 2023-05-07 08:57:23.000000 edit-anything-0.0.5/edit_anything.egg-info/PKG-INFO
+-rw-r--r--   0 arkmon     (501) staff       (20)     1683 2023-05-07 08:57:23.000000 edit-anything-0.0.5/edit_anything.egg-info/SOURCES.txt
+-rw-r--r--   0 arkmon     (501) staff       (20)        1 2023-05-07 08:57:23.000000 edit-anything-0.0.5/edit_anything.egg-info/dependency_links.txt
+-rw-r--r--   0 arkmon     (501) staff       (20)       55 2023-05-07 08:57:23.000000 edit-anything-0.0.5/edit_anything.egg-info/entry_points.txt
+-rw-r--r--   0 arkmon     (501) staff       (20)        1 2023-05-07 08:53:24.000000 edit-anything-0.0.5/edit_anything.egg-info/not-zip-safe
+-rw-r--r--   0 arkmon     (501) staff       (20)      129 2023-05-07 08:57:23.000000 edit-anything-0.0.5/edit_anything.egg-info/requires.txt
+-rw-r--r--   0 arkmon     (501) staff       (20)       10 2023-05-07 08:57:23.000000 edit-anything-0.0.5/edit_anything.egg-info/top_level.txt
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.878206 edit-anything-0.0.5/fastmodel/
+-rw-r--r--   0 arkmon     (501) staff       (20)        0 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/__init__.py
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.878566 edit-anything-0.0.5/fastmodel/backend/
+-rw-r--r--   0 arkmon     (501) staff       (20)        0 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/backend/__init__.py
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.879129 edit-anything-0.0.5/fastmodel/backend/constant/
+-rw-r--r--   0 arkmon     (501) staff       (20)        0 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/backend/constant/__init__.py
+-rw-r--r--   0 arkmon     (501) staff       (20)      160 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/backend/constant/biz_constants.py
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.879595 edit-anything-0.0.5/fastmodel/backend/domain/
+-rw-r--r--   0 arkmon     (501) staff       (20)        0 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/backend/domain/__init__.py
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.881235 edit-anything-0.0.5/fastmodel/backend/domain/dto/
+-rw-r--r--   0 arkmon     (501) staff       (20)        0 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/backend/domain/dto/__init__.py
+-rw-r--r--   0 arkmon     (501) staff       (20)      291 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/backend/domain/dto/req_classes.py
+-rw-r--r--   0 arkmon     (501) staff       (20)      124 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/backend/domain/dto/rsp_classes.py
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.882383 edit-anything-0.0.5/fastmodel/backend/exception/
+-rw-r--r--   0 arkmon     (501) staff       (20)        1 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/backend/exception/__init__.py
+-rw-r--r--   0 arkmon     (501) staff       (20)     1221 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/backend/exception/exceptions.py
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.883043 edit-anything-0.0.5/fastmodel/backend/inference/
+-rw-r--r--   0 arkmon     (501) staff       (20)        0 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/backend/inference/__init__.py
+-rw-r--r--   0 arkmon     (501) staff       (20)     1819 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/backend/inference/inference.py
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.883566 edit-anything-0.0.5/fastmodel/backend/process/
+-rw-r--r--   0 arkmon     (501) staff       (20)        0 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/backend/process/__init__.py
+-rw-r--r--   0 arkmon     (501) staff       (20)       65 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/backend/process/cv_process.py
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.884646 edit-anything-0.0.5/fastmodel/backend/util/
+-rw-r--r--   0 arkmon     (501) staff       (20)        0 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/backend/util/__init__.py
+-rw-r--r--   0 arkmon     (501) staff       (20)     3118 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/backend/util/file.py
+-rw-r--r--   0 arkmon     (501) staff       (20)     2066 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/backend/util/img_util.py
+-rw-r--r--   0 arkmon     (501) staff       (20)     1197 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/backend/util/str_util.py
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.884933 edit-anything-0.0.5/fastmodel/frontend/
+-rw-r--r--   0 arkmon     (501) staff       (20)        0 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/frontend/__init__.py
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.885135 edit-anything-0.0.5/fastmodel/frontend/edit-anything/
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.872233 edit-anything-0.0.5/fastmodel/frontend/edit-anything/assets/
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.885777 edit-anything-0.0.5/fastmodel/frontend/edit-anything/assets/css/
+-rw-r--r--   0 arkmon     (501) staff       (20)    50507 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/frontend/edit-anything/assets/css/801e8f75.css
+-rw-r--r--   0 arkmon     (501) staff       (20)   101568 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/frontend/edit-anything/assets/css/db720fc8.css
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.886503 edit-anything-0.0.5/fastmodel/frontend/edit-anything/assets/img/
+-rw-r--r--   0 arkmon     (501) staff       (20)    10462 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/frontend/edit-anything/assets/img/favicon.ico
+-rw-r--r--   0 arkmon     (501) staff       (20)   163424 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/frontend/edit-anything/assets/img/low-salary.de80db91.jpg
+-rw-r--r--   0 arkmon     (501) staff       (20)      697 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/frontend/edit-anything/index.html
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.890984 edit-anything-0.0.5/fastmodel/frontend/edit-anything/js/
+-rw-r--r--   0 arkmon     (501) staff       (20)   834928 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/frontend/edit-anything/js/764.d32bc368.js
+-rw-r--r--   0 arkmon     (501) staff       (20)     2272 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/frontend/edit-anything/js/764.d32bc368.js.LICENSE.txt
+-rw-r--r--   0 arkmon     (501) staff       (20)    49531 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/frontend/edit-anything/js/antd.a691f5d1.js
+-rw-r--r--   0 arkmon     (501) staff       (20)    39046 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/frontend/edit-anything/js/main.7d537378.js
+-rw-r--r--   0 arkmon     (501) staff       (20)     2226 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/frontend/edit-anything/js/runtime~main.0144593e.js
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.872952 edit-anything-0.0.5/fastmodel/frontend/edit-anything/tmp/
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.873289 edit-anything-0.0.5/fastmodel/frontend/edit-anything/tmp/img/
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.891271 edit-anything-0.0.5/fastmodel/frontend/edit-anything/tmp/img/in/
+-rw-r--r--   0 arkmon     (501) staff       (20)        0 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/frontend/edit-anything/tmp/img/in/a.txt
+drwxr-xr-x   0 arkmon     (501) staff       (20)        0 2023-05-07 08:57:23.891627 edit-anything-0.0.5/fastmodel/frontend/edit-anything/tmp/img/out/
+-rw-r--r--   0 arkmon     (501) staff       (20)        0 2023-05-07 03:41:35.000000 edit-anything-0.0.5/fastmodel/frontend/edit-anything/tmp/img/out/a.txt
+-rw-r--r--   0 arkmon     (501) staff       (20)     4155 2023-05-07 08:52:52.000000 edit-anything-0.0.5/fastmodel/main.py
+-rw-r--r--   0 arkmon     (501) staff       (20)       38 2023-05-07 08:57:23.892385 edit-anything-0.0.5/setup.cfg
+-rw-r--r--   0 arkmon     (501) staff       (20)     1126 2023-05-07 08:57:18.000000 edit-anything-0.0.5/setup.py
```

### Comparing `edit-anything-0.0.4/edit_anything.egg-info/SOURCES.txt` & `edit-anything-0.0.5/edit_anything.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.4/fastmodel/backend/exception/exceptions.py` & `edit-anything-0.0.5/fastmodel/backend/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.4/fastmodel/backend/inference/inference.py` & `edit-anything-0.0.5/fastmodel/backend/inference/inference.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,48 @@
 import numpy as np
-from diffusers import StableDiffusionInpaintPipeline
+from diffusers import StableDiffusionInpaintPipeline, StableDiffusionPipeline, EulerDiscreteScheduler
 import torch
 from fastmodel.backend.util.img_util import img_preprocess_sd_inpaint
 from PIL import Image
 from fastmodel.backend.constant.biz_constants import app_abs_path
 
 
 def inference_sd_inpaint(image: str, mask: str, prompt: str, device: str, out_img: str):
     print(image, mask, prompt)
     pipe = StableDiffusionInpaintPipeline.from_pretrained(
         "stabilityai/stable-diffusion-2-inpainting",
         torch_dtype=torch.float,
     )
     pipe.to(device)
-    #image and mask_image should be PIL images.
-    #The mask structure is white for inpainting and black for keeping as s
+    # image and mask_image should be PIL images.
+    # The mask structure is white for inpainting and black for keeping as s
     ori_img, mask_img, o_w, o_h = img_preprocess_sd_inpaint(
         image,
         mask
     )
-    print(o_w,o_h)
     image = pipe(prompt=prompt, image=ori_img, mask_image=mask_img).images[0]
     image = np.array(image)
     image = Image.fromarray(image)
     image = image.resize((o_w, o_h))
     base_path = app_abs_path()
     out_img_path = f'{base_path}/frontend/edit-anything/tmp/img/out/{out_img}.png'
     image.save(out_img_path)
 
     return f'{out_img}.png'
 
+
+def inference_sd_generate(prompt: str, width: int, height: int, device: str, out_img: str):
+    # todo
+    model_id = "stabilityai/stable-diffusion-2"
+    # Use the Euler scheduler here instead
+    scheduler = EulerDiscreteScheduler.from_pretrained(model_id, subfolder="scheduler")
+    pipe = StableDiffusionPipeline.from_pretrained(model_id, scheduler=scheduler, torch_dtype=torch.float16)
+    pipe = pipe.to(device)
+    image = pipe(prompt).images[0]
+    base_path = app_abs_path()
+    out_img_path = f'{base_path}/frontend/edit-anything/tmp/img/out/{out_img}.png'
+    image.save(out_img_path)
+    return f'{out_img}.png'
+
+
 if __name__ == '__main__':
     pass
```

### Comparing `edit-anything-0.0.4/fastmodel/backend/util/file.py` & `edit-anything-0.0.5/fastmodel/backend/util/file.py`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.4/fastmodel/backend/util/img_util.py` & `edit-anything-0.0.5/fastmodel/backend/util/img_util.py`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.4/fastmodel/backend/util/str_util.py` & `edit-anything-0.0.5/fastmodel/backend/util/str_util.py`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/css/801e8f75.css` & `edit-anything-0.0.5/fastmodel/frontend/edit-anything/assets/css/801e8f75.css`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/css/db720fc8.css` & `edit-anything-0.0.5/fastmodel/frontend/edit-anything/assets/css/db720fc8.css`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/img/favicon.ico` & `edit-anything-0.0.5/fastmodel/frontend/edit-anything/assets/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/img/low-salary.de80db91.jpg` & `edit-anything-0.0.5/fastmodel/frontend/edit-anything/assets/img/low-salary.de80db91.jpg`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.4/fastmodel/frontend/edit-anything/index.html` & `edit-anything-0.0.5/fastmodel/frontend/edit-anything/index.html`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/764.d32bc368.js` & `edit-anything-0.0.5/fastmodel/frontend/edit-anything/js/764.d32bc368.js`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/764.d32bc368.js.LICENSE.txt` & `edit-anything-0.0.5/fastmodel/frontend/edit-anything/js/764.d32bc368.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/antd.a691f5d1.js` & `edit-anything-0.0.5/fastmodel/frontend/edit-anything/js/antd.a691f5d1.js`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/main.7d537378.js` & `edit-anything-0.0.5/fastmodel/frontend/edit-anything/js/main.7d537378.js`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/runtime~main.0144593e.js` & `edit-anything-0.0.5/fastmodel/frontend/edit-anything/js/runtime~main.0144593e.js`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.4/fastmodel/main.py` & `edit-anything-0.0.5/fastmodel/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from fastapi import FastAPI
 import uvicorn
 from fastapi.responses import FileResponse
 from starlette.responses import HTMLResponse
 from fastapi.staticfiles import StaticFiles
-from fastmodel.backend.domain.dto.req_classes import SdInpaintReqDto
+from fastmodel.backend.domain.dto.req_classes import SdInpaintReqDto, SdGenerateReqDto
 from fastmodel.backend.util.str_util import safe_join, generate_random_string
-from fastmodel.backend.inference.inference import inference_sd_inpaint
+from fastmodel.backend.inference.inference import inference_sd_inpaint, inference_sd_generate
 from fastmodel.backend.util.img_util import img_base64_to_file
 from fastmodel.backend.constant.biz_constants import app_abs_path
 import argparse
 
 base_dir = app_abs_path()  # 获取当前脚本所在的目录
 print(base_dir)
 static_resource_dir = os.path.join(base_dir, "frontend/edit-anything")  # 静态文件所在的目录
@@ -46,29 +46,44 @@
     image_base64 = body.image
     mask_base64 = body.mask
     image = img_base64_to_file(image_base64, generate_random_string(6))
     mask = img_base64_to_file(mask_base64, generate_random_string(6))
     prompt = body.prompt
     args = parse_args()
     device = args.device
-
-
     inpaint_img_path = inference_sd_inpaint(image, mask, prompt, device, generate_random_string(7))
 
+    return {
+        "msg": "ok",
+        "msgCode": "10000",
+        "success": True,
+        "total": 1,
+        "data": {
+            "imgBase64": None,
+            "imgUrl": inpaint_img_path
+        }
+    }
 
-    # todo base64 to image
 
+@app.post('/gw/edit-anything/api/v1/bff/sd/generate')
+async def sd_generate(body: SdGenerateReqDto):
+    prompt = body.prompt
+    width = body.width
+    height = body.height
+    args = parse_args()
+    device = args.device
+    generate_img_path = inference_sd_generate(prompt, width, height, device, generate_random_string(9))
     return {
         "msg": "ok",
         "msgCode": "10000",
         "success": True,
         "total": 1,
         "data": {
             "imgBase64": None,
-            "imgUrl": inpaint_img_path
+            "imgUrl": generate_img_path
         }
     }
 
 
 @app.get("/favicon.ico")
 async def favicon():
     ico_file = safe_join(IMG_PATH_LIB, 'favicon.ico')
@@ -78,35 +93,38 @@
 @app.get("/{path:path}")
 async def img_outputs(path: str):
     img_file = safe_join(OUT_IMG_PATH_LIB, path)
     return FileResponse(img_file)
 
 
 def parse_args():
-    parser = argparse.ArgumentParser(description='')
+    parser = argparse.ArgumentParser(description='Light Up Your Imagination From Edit-Anything')
     parser.add_argument(
-        '--host',
         '-H',
+        '--host',
         type=str,
         required=False,
-        default='0.0.0.0'
+        default='0.0.0.0',
+        help='web server url, default=0.0.0.0'
     )
     parser.add_argument(
-        '--port',
         '-P',
+        '--port',
         type=int,
         required=False,
-        default=9911
+        default=9911,
+        help='web server port, default=9911'
     )
     parser.add_argument(
-        '--device',
         '-D',
+        '--device',
         type=str,
         required=False,
-        default='cpu'
+        default='cpu',
+        help='device type: cpu or cuda'
     )
     return parser.parse_args()
 
 
 # init:
 # 1. create tmp dirs to store temp files
 def init():
```

### Comparing `edit-anything-0.0.4/setup.py` & `edit-anything-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     for dirpath, dirnames, filenames in os.walk(base_dir):
         for filename in filenames:
             file_list.append(os.path.join(dirpath, filename))
     return file_list
 
 setup(
     name='edit-anything',
-    version='0.0.4',
+    version='0.0.5',
     description='EditAnything',
-    long_description=utils.get_file_content("README.md"),
+    long_description=utils.get_file_content("README_OUT.md"),
     long_description_content_type='text/markdown',
-    author='wfbi',
-    author_email='myname@example.com',
+    author='edit-anything',
+    author_email='edit-anything@openmmlab.com',
     keywords='EditAnything',
     url='https://github.com/xxx/xxxx',
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         'Development Status :: 3 - Alpha',
```

