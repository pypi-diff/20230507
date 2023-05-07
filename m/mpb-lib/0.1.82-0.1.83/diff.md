# Comparing `tmp/mpb_lib-0.1.82.tar.gz` & `tmp/mpb_lib-0.1.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpb_lib-0.1.82.tar", last modified: Sun Apr 23 23:06:44 2023, max compression
+gzip compressed data, was "mpb_lib-0.1.83.tar", last modified: Sun May  7 06:28:49 2023, max compression
```

## Comparing `mpb_lib-0.1.82.tar` & `mpb_lib-0.1.83.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-23 23:06:44.831602 mpb_lib-0.1.82/
--rw-r--r--   0 ats        (501) staff       (20)      336 2023-04-23 23:06:44.831142 mpb_lib-0.1.82/PKG-INFO
--rw-r--r--   0 ats        (501) staff       (20)        0 2020-12-04 09:04:33.000000 mpb_lib-0.1.82/README.md
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-23 23:06:44.786991 mpb_lib-0.1.82/mpb_lib/
--rw-r--r--   0 ats        (501) staff       (20)        0 2020-12-04 09:04:46.000000 mpb_lib-0.1.82/mpb_lib/__init__.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-23 23:06:44.789356 mpb_lib-0.1.82/mpb_lib/apis/
--rw-r--r--   0 ats        (501) staff       (20)     4942 2023-04-23 23:04:41.000000 mpb_lib-0.1.82/mpb_lib/apis/__init__.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-23 23:06:44.801090 mpb_lib-0.1.82/mpb_lib/cannon/
--rw-r--r--   0 ats        (501) staff       (20)      319 2023-02-01 23:04:45.000000 mpb_lib-0.1.82/mpb_lib/cannon/__init__.py
--rw-r--r--   0 ats        (501) staff       (20)     2050 2023-02-01 23:05:23.000000 mpb_lib-0.1.82/mpb_lib/cannon/cannon.py
--rw-r--r--   0 ats        (501) staff       (20)     9060 2023-02-01 23:05:06.000000 mpb_lib-0.1.82/mpb_lib/cannon/cannon_html.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-23 23:06:44.803916 mpb_lib-0.1.82/mpb_lib/face/
--rw-r--r--   0 ats        (501) staff       (20)      157 2023-02-01 23:06:06.000000 mpb_lib-0.1.82/mpb_lib/face/__init__.py
--rw-r--r--   0 ats        (501) staff       (20)     4435 2023-02-01 23:06:15.000000 mpb_lib-0.1.82/mpb_lib/face/face.py
--rw-r--r--   0 ats        (501) staff       (20)     4304 2023-02-01 23:06:36.000000 mpb_lib-0.1.82/mpb_lib/face/face_html.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-23 23:06:44.804950 mpb_lib-0.1.82/mpb_lib/maze/
--rw-r--r--   0 ats        (501) staff       (20)     2633 2023-02-02 01:03:43.000000 mpb_lib-0.1.82/mpb_lib/maze/__init__.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-23 23:06:44.807224 mpb_lib-0.1.82/mpb_lib/rpg/
--rw-r--r--   0 ats        (501) staff       (20)      185 2021-07-20 02:03:49.000000 mpb_lib-0.1.82/mpb_lib/rpg/__init__.py
--rw-r--r--   0 ats        (501) staff       (20)     9880 2022-06-01 08:47:58.000000 mpb_lib-0.1.82/mpb_lib/rpg/rpg.py
--rw-r--r--   0 ats        (501) staff       (20)     2996 2021-11-26 23:16:54.000000 mpb_lib-0.1.82/mpb_lib/rpg/rpg_html.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-23 23:06:44.809150 mpb_lib-0.1.82/mpb_lib/rythmbox/
--rw-r--r--   0 ats        (501) staff       (20)       29 2021-09-06 05:02:03.000000 mpb_lib-0.1.82/mpb_lib/rythmbox/__init__.py
--rw-r--r--   0 ats        (501) staff       (20)     2419 2021-12-27 01:25:09.000000 mpb_lib-0.1.82/mpb_lib/rythmbox/rythmbox.py
--rw-r--r--   0 ats        (501) staff       (20)     5044 2021-09-02 04:33:49.000000 mpb_lib-0.1.82/mpb_lib/rythmbox/rythmbox_html.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-23 23:06:44.810019 mpb_lib-0.1.82/mpb_lib/sound/
--rw-r--r--   0 ats        (501) staff       (20)      881 2023-02-01 23:07:24.000000 mpb_lib-0.1.82/mpb_lib/sound/__init__.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-23 23:06:44.822865 mpb_lib-0.1.82/mpb_lib/sound/wavs/
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:51.000000 mpb_lib-0.1.82/mpb_lib/sound/wavs/a.wav
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:15.000000 mpb_lib-0.1.82/mpb_lib/sound/wavs/b.wav
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:23.000000 mpb_lib-0.1.82/mpb_lib/sound/wavs/c.wav
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:30.000000 mpb_lib-0.1.82/mpb_lib/sound/wavs/d.wav
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:35.000000 mpb_lib-0.1.82/mpb_lib/sound/wavs/e.wav
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:40.000000 mpb_lib-0.1.82/mpb_lib/sound/wavs/f.wav
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:46.000000 mpb_lib-0.1.82/mpb_lib/sound/wavs/g.wav
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-23 23:06:44.826704 mpb_lib-0.1.82/mpb_lib/tictactoe/
--rw-r--r--   0 ats        (501) staff       (20)      170 2023-02-01 23:08:05.000000 mpb_lib-0.1.82/mpb_lib/tictactoe/__init__.py
--rw-r--r--   0 ats        (501) staff       (20)      950 2023-02-01 23:08:32.000000 mpb_lib-0.1.82/mpb_lib/tictactoe/tictactoe.py
--rw-r--r--   0 ats        (501) staff       (20)     2415 2023-02-01 23:08:24.000000 mpb_lib-0.1.82/mpb_lib/tictactoe/tictactoe_html.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-23 23:06:44.830511 mpb_lib-0.1.82/mpb_lib/vowelgen/
--rw-r--r--   0 ats        (501) staff       (20)     2350 2022-08-18 22:51:31.000000 mpb_lib-0.1.82/mpb_lib/vowelgen/HPF.py
--rw-r--r--   0 ats        (501) staff       (20)      946 2023-02-01 23:02:22.000000 mpb_lib-0.1.82/mpb_lib/vowelgen/__init__.py
--rw-r--r--   0 ats        (501) staff       (20)     3277 2022-08-18 22:51:27.000000 mpb_lib-0.1.82/mpb_lib/vowelgen/glottal.py
--rw-r--r--   0 ats        (501) staff       (20)     6059 2022-08-18 10:39:56.000000 mpb_lib-0.1.82/mpb_lib/vowelgen/threetube.py
--rw-r--r--   0 ats        (501) staff       (20)     5291 2022-08-18 10:39:53.000000 mpb_lib-0.1.82/mpb_lib/vowelgen/twotube.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-04-23 23:06:44.788698 mpb_lib-0.1.82/mpb_lib.egg-info/
--rw-r--r--   0 ats        (501) staff       (20)      336 2023-04-23 23:06:44.000000 mpb_lib-0.1.82/mpb_lib.egg-info/PKG-INFO
--rw-r--r--   0 ats        (501) staff       (20)      962 2023-04-23 23:06:44.000000 mpb_lib-0.1.82/mpb_lib.egg-info/SOURCES.txt
--rw-r--r--   0 ats        (501) staff       (20)        1 2023-04-23 23:06:44.000000 mpb_lib-0.1.82/mpb_lib.egg-info/dependency_links.txt
--rw-r--r--   0 ats        (501) staff       (20)        8 2023-04-23 23:06:44.000000 mpb_lib-0.1.82/mpb_lib.egg-info/top_level.txt
--rw-r--r--   0 ats        (501) staff       (20)       38 2023-04-23 23:06:44.831678 mpb_lib-0.1.82/setup.cfg
--rw-r--r--   0 ats        (501) staff       (20)     1043 2023-04-23 23:05:02.000000 mpb_lib-0.1.82/setup.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:28:49.078098 mpb_lib-0.1.83/
+-rw-r--r--   0 ats        (501) staff       (20)      336 2023-05-07 06:28:49.077817 mpb_lib-0.1.83/PKG-INFO
+-rw-r--r--   0 ats        (501) staff       (20)        0 2020-12-04 09:04:33.000000 mpb_lib-0.1.83/README.md
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:28:49.053052 mpb_lib-0.1.83/mpb_lib/
+-rw-r--r--   0 ats        (501) staff       (20)        0 2020-12-04 09:04:46.000000 mpb_lib-0.1.83/mpb_lib/__init__.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:28:49.054299 mpb_lib-0.1.83/mpb_lib/apis/
+-rw-r--r--   0 ats        (501) staff       (20)     4942 2023-04-23 23:04:41.000000 mpb_lib-0.1.83/mpb_lib/apis/__init__.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:28:49.055878 mpb_lib-0.1.83/mpb_lib/cannon/
+-rw-r--r--   0 ats        (501) staff       (20)      319 2023-02-01 23:04:45.000000 mpb_lib-0.1.83/mpb_lib/cannon/__init__.py
+-rw-r--r--   0 ats        (501) staff       (20)     2078 2023-05-07 06:28:17.000000 mpb_lib-0.1.83/mpb_lib/cannon/cannon.py
+-rw-r--r--   0 ats        (501) staff       (20)     9060 2023-02-01 23:05:06.000000 mpb_lib-0.1.83/mpb_lib/cannon/cannon_html.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:28:49.057669 mpb_lib-0.1.83/mpb_lib/face/
+-rw-r--r--   0 ats        (501) staff       (20)      157 2023-02-01 23:06:06.000000 mpb_lib-0.1.83/mpb_lib/face/__init__.py
+-rw-r--r--   0 ats        (501) staff       (20)     4435 2023-02-01 23:06:15.000000 mpb_lib-0.1.83/mpb_lib/face/face.py
+-rw-r--r--   0 ats        (501) staff       (20)     4304 2023-02-01 23:06:36.000000 mpb_lib-0.1.83/mpb_lib/face/face_html.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:28:49.058293 mpb_lib-0.1.83/mpb_lib/maze/
+-rw-r--r--   0 ats        (501) staff       (20)     2633 2023-02-02 01:03:43.000000 mpb_lib-0.1.83/mpb_lib/maze/__init__.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:28:49.060308 mpb_lib-0.1.83/mpb_lib/rpg/
+-rw-r--r--   0 ats        (501) staff       (20)      185 2021-07-20 02:03:49.000000 mpb_lib-0.1.83/mpb_lib/rpg/__init__.py
+-rw-r--r--   0 ats        (501) staff       (20)     9880 2022-06-01 08:47:58.000000 mpb_lib-0.1.83/mpb_lib/rpg/rpg.py
+-rw-r--r--   0 ats        (501) staff       (20)     2996 2021-11-26 23:16:54.000000 mpb_lib-0.1.83/mpb_lib/rpg/rpg_html.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:28:49.061858 mpb_lib-0.1.83/mpb_lib/rythmbox/
+-rw-r--r--   0 ats        (501) staff       (20)       29 2021-09-06 05:02:03.000000 mpb_lib-0.1.83/mpb_lib/rythmbox/__init__.py
+-rw-r--r--   0 ats        (501) staff       (20)     2419 2021-12-27 01:25:09.000000 mpb_lib-0.1.83/mpb_lib/rythmbox/rythmbox.py
+-rw-r--r--   0 ats        (501) staff       (20)     5044 2021-09-02 04:33:49.000000 mpb_lib-0.1.83/mpb_lib/rythmbox/rythmbox_html.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:28:49.062428 mpb_lib-0.1.83/mpb_lib/sound/
+-rw-r--r--   0 ats        (501) staff       (20)      881 2023-02-01 23:07:24.000000 mpb_lib-0.1.83/mpb_lib/sound/__init__.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:28:49.071321 mpb_lib-0.1.83/mpb_lib/sound/wavs/
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:51.000000 mpb_lib-0.1.83/mpb_lib/sound/wavs/a.wav
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:15.000000 mpb_lib-0.1.83/mpb_lib/sound/wavs/b.wav
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:23.000000 mpb_lib-0.1.83/mpb_lib/sound/wavs/c.wav
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:30.000000 mpb_lib-0.1.83/mpb_lib/sound/wavs/d.wav
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:35.000000 mpb_lib-0.1.83/mpb_lib/sound/wavs/e.wav
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:40.000000 mpb_lib-0.1.83/mpb_lib/sound/wavs/f.wav
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:46.000000 mpb_lib-0.1.83/mpb_lib/sound/wavs/g.wav
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:28:49.074001 mpb_lib-0.1.83/mpb_lib/tictactoe/
+-rw-r--r--   0 ats        (501) staff       (20)      170 2023-02-01 23:08:05.000000 mpb_lib-0.1.83/mpb_lib/tictactoe/__init__.py
+-rw-r--r--   0 ats        (501) staff       (20)      950 2023-02-01 23:08:32.000000 mpb_lib-0.1.83/mpb_lib/tictactoe/tictactoe.py
+-rw-r--r--   0 ats        (501) staff       (20)     2415 2023-02-01 23:08:24.000000 mpb_lib-0.1.83/mpb_lib/tictactoe/tictactoe_html.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:28:49.077230 mpb_lib-0.1.83/mpb_lib/vowelgen/
+-rw-r--r--   0 ats        (501) staff       (20)     2350 2022-08-18 22:51:31.000000 mpb_lib-0.1.83/mpb_lib/vowelgen/HPF.py
+-rw-r--r--   0 ats        (501) staff       (20)      946 2023-02-01 23:02:22.000000 mpb_lib-0.1.83/mpb_lib/vowelgen/__init__.py
+-rw-r--r--   0 ats        (501) staff       (20)     3277 2022-08-18 22:51:27.000000 mpb_lib-0.1.83/mpb_lib/vowelgen/glottal.py
+-rw-r--r--   0 ats        (501) staff       (20)     6059 2022-08-18 10:39:56.000000 mpb_lib-0.1.83/mpb_lib/vowelgen/threetube.py
+-rw-r--r--   0 ats        (501) staff       (20)     5291 2022-08-18 10:39:53.000000 mpb_lib-0.1.83/mpb_lib/vowelgen/twotube.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:28:49.054031 mpb_lib-0.1.83/mpb_lib.egg-info/
+-rw-r--r--   0 ats        (501) staff       (20)      336 2023-05-07 06:28:48.000000 mpb_lib-0.1.83/mpb_lib.egg-info/PKG-INFO
+-rw-r--r--   0 ats        (501) staff       (20)      962 2023-05-07 06:28:48.000000 mpb_lib-0.1.83/mpb_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 ats        (501) staff       (20)        1 2023-05-07 06:28:48.000000 mpb_lib-0.1.83/mpb_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 ats        (501) staff       (20)        8 2023-05-07 06:28:48.000000 mpb_lib-0.1.83/mpb_lib.egg-info/top_level.txt
+-rw-r--r--   0 ats        (501) staff       (20)       38 2023-05-07 06:28:49.078200 mpb_lib-0.1.83/setup.cfg
+-rw-r--r--   0 ats        (501) staff       (20)     1043 2023-05-07 06:28:22.000000 mpb_lib-0.1.83/setup.py
```

### Comparing `mpb_lib-0.1.82/mpb_lib/apis/__init__.py` & `mpb_lib-0.1.83/mpb_lib/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/cannon/cannon.py` & `mpb_lib-0.1.83/mpb_lib/cannon/cannon.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Copyright (c) 2023 Atsush Shibata(shivata@m-info.co.jp)
 #
 # Released under the MIT license.
 
 
 from random import randint
 from math import floor
+from string import Template
 
 from IPython.display import display, HTML
 try:
     from google.colab.output import eval_js
     HTML_fook = HTML
     display_hook = display
```

### Comparing `mpb_lib-0.1.82/mpb_lib/cannon/cannon_html.py` & `mpb_lib-0.1.83/mpb_lib/cannon/cannon_html.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/face/face.py` & `mpb_lib-0.1.83/mpb_lib/face/face.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/face/face_html.py` & `mpb_lib-0.1.83/mpb_lib/face/face_html.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/maze/__init__.py` & `mpb_lib-0.1.83/mpb_lib/maze/__init__.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/rpg/rpg.py` & `mpb_lib-0.1.83/mpb_lib/rpg/rpg.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/rpg/rpg_html.py` & `mpb_lib-0.1.83/mpb_lib/rpg/rpg_html.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/rythmbox/rythmbox.py` & `mpb_lib-0.1.83/mpb_lib/rythmbox/rythmbox.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/rythmbox/rythmbox_html.py` & `mpb_lib-0.1.83/mpb_lib/rythmbox/rythmbox_html.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/sound/__init__.py` & `mpb_lib-0.1.83/mpb_lib/sound/__init__.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/sound/wavs/a.wav` & `mpb_lib-0.1.83/mpb_lib/sound/wavs/a.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/sound/wavs/b.wav` & `mpb_lib-0.1.83/mpb_lib/sound/wavs/b.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/sound/wavs/c.wav` & `mpb_lib-0.1.83/mpb_lib/sound/wavs/c.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/sound/wavs/d.wav` & `mpb_lib-0.1.83/mpb_lib/sound/wavs/d.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/sound/wavs/e.wav` & `mpb_lib-0.1.83/mpb_lib/sound/wavs/e.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/sound/wavs/f.wav` & `mpb_lib-0.1.83/mpb_lib/sound/wavs/f.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/sound/wavs/g.wav` & `mpb_lib-0.1.83/mpb_lib/sound/wavs/g.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/tictactoe/tictactoe.py` & `mpb_lib-0.1.83/mpb_lib/tictactoe/tictactoe.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/tictactoe/tictactoe_html.py` & `mpb_lib-0.1.83/mpb_lib/tictactoe/tictactoe_html.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/vowelgen/HPF.py` & `mpb_lib-0.1.83/mpb_lib/vowelgen/HPF.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/vowelgen/__init__.py` & `mpb_lib-0.1.83/mpb_lib/vowelgen/__init__.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/vowelgen/glottal.py` & `mpb_lib-0.1.83/mpb_lib/vowelgen/glottal.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/vowelgen/threetube.py` & `mpb_lib-0.1.83/mpb_lib/vowelgen/threetube.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib/vowelgen/twotube.py` & `mpb_lib-0.1.83/mpb_lib/vowelgen/twotube.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/mpb_lib.egg-info/SOURCES.txt` & `mpb_lib-0.1.83/mpb_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.82/setup.py` & `mpb_lib-0.1.83/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
                        'sound/wavs/d.wav',
                        'sound/wavs/e.wav',
                        'sound/wavs/f.wav',
                        'sound/wavs/g.wav',
                        'sound/wavs/a.wav',
                        'sound/wavs/b.wav' ]},
 
-    version='0.1.82', # バージョン
+    version='0.1.83', # バージョン
 
     license='MIT', # ライセンス
 
     install_requires=[],
 
     author='Atsushi Shibata',
     author_email='shibata@m-info.co.jp',
```

