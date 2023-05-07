# Comparing `tmp/mpb_lib-0.1.84.tar.gz` & `tmp/mpb_lib-0.1.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpb_lib-0.1.84.tar", last modified: Sun May  7 06:57:58 2023, max compression
+gzip compressed data, was "mpb_lib-0.1.85.tar", last modified: Sun May  7 07:02:53 2023, max compression
```

## Comparing `mpb_lib-0.1.84.tar` & `mpb_lib-0.1.85.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:57:58.883883 mpb_lib-0.1.84/
--rw-r--r--   0 ats        (501) staff       (20)      336 2023-05-07 06:57:58.883536 mpb_lib-0.1.84/PKG-INFO
--rw-r--r--   0 ats        (501) staff       (20)        0 2020-12-04 09:04:33.000000 mpb_lib-0.1.84/README.md
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:57:58.859139 mpb_lib-0.1.84/mpb_lib/
--rw-r--r--   0 ats        (501) staff       (20)        0 2020-12-04 09:04:46.000000 mpb_lib-0.1.84/mpb_lib/__init__.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:57:58.860723 mpb_lib-0.1.84/mpb_lib/apis/
--rw-r--r--   0 ats        (501) staff       (20)     4942 2023-04-23 23:04:41.000000 mpb_lib-0.1.84/mpb_lib/apis/__init__.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:57:58.862220 mpb_lib-0.1.84/mpb_lib/cannon/
--rw-r--r--   0 ats        (501) staff       (20)      347 2023-05-07 06:57:46.000000 mpb_lib-0.1.84/mpb_lib/cannon/__init__.py
--rw-r--r--   0 ats        (501) staff       (20)     2050 2023-05-07 06:57:47.000000 mpb_lib-0.1.84/mpb_lib/cannon/cannon.py
--rw-r--r--   0 ats        (501) staff       (20)     9060 2023-02-01 23:05:06.000000 mpb_lib-0.1.84/mpb_lib/cannon/cannon_html.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:57:58.864068 mpb_lib-0.1.84/mpb_lib/face/
--rw-r--r--   0 ats        (501) staff       (20)      157 2023-02-01 23:06:06.000000 mpb_lib-0.1.84/mpb_lib/face/__init__.py
--rw-r--r--   0 ats        (501) staff       (20)     4435 2023-02-01 23:06:15.000000 mpb_lib-0.1.84/mpb_lib/face/face.py
--rw-r--r--   0 ats        (501) staff       (20)     4304 2023-02-01 23:06:36.000000 mpb_lib-0.1.84/mpb_lib/face/face_html.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:57:58.864780 mpb_lib-0.1.84/mpb_lib/maze/
--rw-r--r--   0 ats        (501) staff       (20)     2633 2023-02-02 01:03:43.000000 mpb_lib-0.1.84/mpb_lib/maze/__init__.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:57:58.866657 mpb_lib-0.1.84/mpb_lib/rpg/
--rw-r--r--   0 ats        (501) staff       (20)      185 2021-07-20 02:03:49.000000 mpb_lib-0.1.84/mpb_lib/rpg/__init__.py
--rw-r--r--   0 ats        (501) staff       (20)     9880 2022-06-01 08:47:58.000000 mpb_lib-0.1.84/mpb_lib/rpg/rpg.py
--rw-r--r--   0 ats        (501) staff       (20)     2996 2021-11-26 23:16:54.000000 mpb_lib-0.1.84/mpb_lib/rpg/rpg_html.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:57:58.868182 mpb_lib-0.1.84/mpb_lib/rythmbox/
--rw-r--r--   0 ats        (501) staff       (20)       29 2021-09-06 05:02:03.000000 mpb_lib-0.1.84/mpb_lib/rythmbox/__init__.py
--rw-r--r--   0 ats        (501) staff       (20)     2419 2021-12-27 01:25:09.000000 mpb_lib-0.1.84/mpb_lib/rythmbox/rythmbox.py
--rw-r--r--   0 ats        (501) staff       (20)     5044 2021-09-02 04:33:49.000000 mpb_lib-0.1.84/mpb_lib/rythmbox/rythmbox_html.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:57:58.868612 mpb_lib-0.1.84/mpb_lib/sound/
--rw-r--r--   0 ats        (501) staff       (20)      881 2023-02-01 23:07:24.000000 mpb_lib-0.1.84/mpb_lib/sound/__init__.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:57:58.877066 mpb_lib-0.1.84/mpb_lib/sound/wavs/
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:51.000000 mpb_lib-0.1.84/mpb_lib/sound/wavs/a.wav
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:15.000000 mpb_lib-0.1.84/mpb_lib/sound/wavs/b.wav
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:23.000000 mpb_lib-0.1.84/mpb_lib/sound/wavs/c.wav
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:30.000000 mpb_lib-0.1.84/mpb_lib/sound/wavs/d.wav
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:35.000000 mpb_lib-0.1.84/mpb_lib/sound/wavs/e.wav
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:40.000000 mpb_lib-0.1.84/mpb_lib/sound/wavs/f.wav
--rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:46.000000 mpb_lib-0.1.84/mpb_lib/sound/wavs/g.wav
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:57:58.879970 mpb_lib-0.1.84/mpb_lib/tictactoe/
--rw-r--r--   0 ats        (501) staff       (20)      170 2023-02-01 23:08:05.000000 mpb_lib-0.1.84/mpb_lib/tictactoe/__init__.py
--rw-r--r--   0 ats        (501) staff       (20)      950 2023-02-01 23:08:32.000000 mpb_lib-0.1.84/mpb_lib/tictactoe/tictactoe.py
--rw-r--r--   0 ats        (501) staff       (20)     2415 2023-02-01 23:08:24.000000 mpb_lib-0.1.84/mpb_lib/tictactoe/tictactoe_html.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:57:58.882878 mpb_lib-0.1.84/mpb_lib/vowelgen/
--rw-r--r--   0 ats        (501) staff       (20)     2350 2022-08-18 22:51:31.000000 mpb_lib-0.1.84/mpb_lib/vowelgen/HPF.py
--rw-r--r--   0 ats        (501) staff       (20)      946 2023-02-01 23:02:22.000000 mpb_lib-0.1.84/mpb_lib/vowelgen/__init__.py
--rw-r--r--   0 ats        (501) staff       (20)     3277 2022-08-18 22:51:27.000000 mpb_lib-0.1.84/mpb_lib/vowelgen/glottal.py
--rw-r--r--   0 ats        (501) staff       (20)     6059 2022-08-18 10:39:56.000000 mpb_lib-0.1.84/mpb_lib/vowelgen/threetube.py
--rw-r--r--   0 ats        (501) staff       (20)     5291 2022-08-18 10:39:53.000000 mpb_lib-0.1.84/mpb_lib/vowelgen/twotube.py
-drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 06:57:58.860405 mpb_lib-0.1.84/mpb_lib.egg-info/
--rw-r--r--   0 ats        (501) staff       (20)      336 2023-05-07 06:57:58.000000 mpb_lib-0.1.84/mpb_lib.egg-info/PKG-INFO
--rw-r--r--   0 ats        (501) staff       (20)      962 2023-05-07 06:57:58.000000 mpb_lib-0.1.84/mpb_lib.egg-info/SOURCES.txt
--rw-r--r--   0 ats        (501) staff       (20)        1 2023-05-07 06:57:58.000000 mpb_lib-0.1.84/mpb_lib.egg-info/dependency_links.txt
--rw-r--r--   0 ats        (501) staff       (20)        8 2023-05-07 06:57:58.000000 mpb_lib-0.1.84/mpb_lib.egg-info/top_level.txt
--rw-r--r--   0 ats        (501) staff       (20)       38 2023-05-07 06:57:58.883967 mpb_lib-0.1.84/setup.cfg
--rw-r--r--   0 ats        (501) staff       (20)     1043 2023-05-07 06:57:54.000000 mpb_lib-0.1.84/setup.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 07:02:53.086657 mpb_lib-0.1.85/
+-rw-r--r--   0 ats        (501) staff       (20)      336 2023-05-07 07:02:53.086370 mpb_lib-0.1.85/PKG-INFO
+-rw-r--r--   0 ats        (501) staff       (20)        0 2020-12-04 09:04:33.000000 mpb_lib-0.1.85/README.md
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 07:02:53.059986 mpb_lib-0.1.85/mpb_lib/
+-rw-r--r--   0 ats        (501) staff       (20)        0 2020-12-04 09:04:46.000000 mpb_lib-0.1.85/mpb_lib/__init__.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 07:02:53.061580 mpb_lib-0.1.85/mpb_lib/apis/
+-rw-r--r--   0 ats        (501) staff       (20)     4942 2023-04-23 23:04:41.000000 mpb_lib-0.1.85/mpb_lib/apis/__init__.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 07:02:53.062705 mpb_lib-0.1.85/mpb_lib/cannon/
+-rw-r--r--   0 ats        (501) staff       (20)      319 2023-05-07 07:02:18.000000 mpb_lib-0.1.85/mpb_lib/cannon/__init__.py
+-rw-r--r--   0 ats        (501) staff       (20)     2174 2023-05-07 07:02:38.000000 mpb_lib-0.1.85/mpb_lib/cannon/cannon.py
+-rw-r--r--   0 ats        (501) staff       (20)     9060 2023-02-01 23:05:06.000000 mpb_lib-0.1.85/mpb_lib/cannon/cannon_html.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 07:02:53.065044 mpb_lib-0.1.85/mpb_lib/face/
+-rw-r--r--   0 ats        (501) staff       (20)      157 2023-02-01 23:06:06.000000 mpb_lib-0.1.85/mpb_lib/face/__init__.py
+-rw-r--r--   0 ats        (501) staff       (20)     4435 2023-02-01 23:06:15.000000 mpb_lib-0.1.85/mpb_lib/face/face.py
+-rw-r--r--   0 ats        (501) staff       (20)     4304 2023-02-01 23:06:36.000000 mpb_lib-0.1.85/mpb_lib/face/face_html.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 07:02:53.065689 mpb_lib-0.1.85/mpb_lib/maze/
+-rw-r--r--   0 ats        (501) staff       (20)     2633 2023-02-02 01:03:43.000000 mpb_lib-0.1.85/mpb_lib/maze/__init__.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 07:02:53.067530 mpb_lib-0.1.85/mpb_lib/rpg/
+-rw-r--r--   0 ats        (501) staff       (20)      185 2021-07-20 02:03:49.000000 mpb_lib-0.1.85/mpb_lib/rpg/__init__.py
+-rw-r--r--   0 ats        (501) staff       (20)     9880 2022-06-01 08:47:58.000000 mpb_lib-0.1.85/mpb_lib/rpg/rpg.py
+-rw-r--r--   0 ats        (501) staff       (20)     2996 2021-11-26 23:16:54.000000 mpb_lib-0.1.85/mpb_lib/rpg/rpg_html.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 07:02:53.069661 mpb_lib-0.1.85/mpb_lib/rythmbox/
+-rw-r--r--   0 ats        (501) staff       (20)       29 2021-09-06 05:02:03.000000 mpb_lib-0.1.85/mpb_lib/rythmbox/__init__.py
+-rw-r--r--   0 ats        (501) staff       (20)     2419 2021-12-27 01:25:09.000000 mpb_lib-0.1.85/mpb_lib/rythmbox/rythmbox.py
+-rw-r--r--   0 ats        (501) staff       (20)     5044 2021-09-02 04:33:49.000000 mpb_lib-0.1.85/mpb_lib/rythmbox/rythmbox_html.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 07:02:53.070560 mpb_lib-0.1.85/mpb_lib/sound/
+-rw-r--r--   0 ats        (501) staff       (20)      881 2023-02-01 23:07:24.000000 mpb_lib-0.1.85/mpb_lib/sound/__init__.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 07:02:53.079470 mpb_lib-0.1.85/mpb_lib/sound/wavs/
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:51.000000 mpb_lib-0.1.85/mpb_lib/sound/wavs/a.wav
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:15.000000 mpb_lib-0.1.85/mpb_lib/sound/wavs/b.wav
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:23.000000 mpb_lib-0.1.85/mpb_lib/sound/wavs/c.wav
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:30.000000 mpb_lib-0.1.85/mpb_lib/sound/wavs/d.wav
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:35.000000 mpb_lib-0.1.85/mpb_lib/sound/wavs/e.wav
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:40.000000 mpb_lib-0.1.85/mpb_lib/sound/wavs/f.wav
+-rw-r--r--   0 ats        (501) staff       (20)    88244 2021-09-28 07:08:46.000000 mpb_lib-0.1.85/mpb_lib/sound/wavs/g.wav
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 07:02:53.082295 mpb_lib-0.1.85/mpb_lib/tictactoe/
+-rw-r--r--   0 ats        (501) staff       (20)      170 2023-02-01 23:08:05.000000 mpb_lib-0.1.85/mpb_lib/tictactoe/__init__.py
+-rw-r--r--   0 ats        (501) staff       (20)      950 2023-02-01 23:08:32.000000 mpb_lib-0.1.85/mpb_lib/tictactoe/tictactoe.py
+-rw-r--r--   0 ats        (501) staff       (20)     2415 2023-02-01 23:08:24.000000 mpb_lib-0.1.85/mpb_lib/tictactoe/tictactoe_html.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 07:02:53.085890 mpb_lib-0.1.85/mpb_lib/vowelgen/
+-rw-r--r--   0 ats        (501) staff       (20)     2350 2022-08-18 22:51:31.000000 mpb_lib-0.1.85/mpb_lib/vowelgen/HPF.py
+-rw-r--r--   0 ats        (501) staff       (20)      946 2023-02-01 23:02:22.000000 mpb_lib-0.1.85/mpb_lib/vowelgen/__init__.py
+-rw-r--r--   0 ats        (501) staff       (20)     3277 2022-08-18 22:51:27.000000 mpb_lib-0.1.85/mpb_lib/vowelgen/glottal.py
+-rw-r--r--   0 ats        (501) staff       (20)     6059 2022-08-18 10:39:56.000000 mpb_lib-0.1.85/mpb_lib/vowelgen/threetube.py
+-rw-r--r--   0 ats        (501) staff       (20)     5291 2022-08-18 10:39:53.000000 mpb_lib-0.1.85/mpb_lib/vowelgen/twotube.py
+drwxr-xr-x   0 ats        (501) staff       (20)        0 2023-05-07 07:02:53.061244 mpb_lib-0.1.85/mpb_lib.egg-info/
+-rw-r--r--   0 ats        (501) staff       (20)      336 2023-05-07 07:02:52.000000 mpb_lib-0.1.85/mpb_lib.egg-info/PKG-INFO
+-rw-r--r--   0 ats        (501) staff       (20)      962 2023-05-07 07:02:52.000000 mpb_lib-0.1.85/mpb_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 ats        (501) staff       (20)        1 2023-05-07 07:02:52.000000 mpb_lib-0.1.85/mpb_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 ats        (501) staff       (20)        8 2023-05-07 07:02:52.000000 mpb_lib-0.1.85/mpb_lib.egg-info/top_level.txt
+-rw-r--r--   0 ats        (501) staff       (20)       38 2023-05-07 07:02:53.086738 mpb_lib-0.1.85/setup.cfg
+-rw-r--r--   0 ats        (501) staff       (20)     1043 2023-05-07 07:02:49.000000 mpb_lib-0.1.85/setup.py
```

### Comparing `mpb_lib-0.1.84/mpb_lib/apis/__init__.py` & `mpb_lib-0.1.85/mpb_lib/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/cannon/cannon.py` & `mpb_lib-0.1.85/mpb_lib/cannon/cannon.py`

 * *Files 22% similar despite different names*

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
 
@@ -46,30 +47,33 @@
     html_body = HTML_fook(LOAD_SCRIPT)
     display_hook(html_body)
 
 
 from .cannon_html import HTML_TEMPLATE, SCRIPT, LOAD_SCRIPT
 
 def cannon_game(powder):
+    from string import Template
     html_source = Template(HTML_TEMPLATE)
     args = {"SCRIPT":SCRIPT, "stage":1, "powder":powder, "delta": 0,
             "dist_display": ""}
     html_body = HTML_fook(html_source.substitute(**args))
     display_hook(html_body)
 
 
 def cannon_game2(powder):
+    from string import Template
     html_source = Template(HTML_TEMPLATE)
     args = {"SCRIPT":SCRIPT, "stage":2, "powder":powder, "delta": 0,
             "dist_display": ""}
     html_body = HTML_fook(html_source.substitute(**args))
     display_hook(html_body)
 
 
 def cannon_game3(powder, delta=-1):
+    from string import Template
     global DELTA
     if delta != -1:
         DELTA = delta
     else:
         set_delta()
     html_source = Template(HTML_TEMPLATE)
     args = {"SCRIPT":SCRIPT, "stage":2, "powder":powder, "delta": DELTA,
```

### Comparing `mpb_lib-0.1.84/mpb_lib/cannon/cannon_html.py` & `mpb_lib-0.1.85/mpb_lib/cannon/cannon_html.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/face/face.py` & `mpb_lib-0.1.85/mpb_lib/face/face.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/face/face_html.py` & `mpb_lib-0.1.85/mpb_lib/face/face_html.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/maze/__init__.py` & `mpb_lib-0.1.85/mpb_lib/maze/__init__.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/rpg/rpg.py` & `mpb_lib-0.1.85/mpb_lib/rpg/rpg.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/rpg/rpg_html.py` & `mpb_lib-0.1.85/mpb_lib/rpg/rpg_html.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/rythmbox/rythmbox.py` & `mpb_lib-0.1.85/mpb_lib/rythmbox/rythmbox.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/rythmbox/rythmbox_html.py` & `mpb_lib-0.1.85/mpb_lib/rythmbox/rythmbox_html.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/sound/__init__.py` & `mpb_lib-0.1.85/mpb_lib/sound/__init__.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/sound/wavs/a.wav` & `mpb_lib-0.1.85/mpb_lib/sound/wavs/a.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/sound/wavs/b.wav` & `mpb_lib-0.1.85/mpb_lib/sound/wavs/b.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/sound/wavs/c.wav` & `mpb_lib-0.1.85/mpb_lib/sound/wavs/c.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/sound/wavs/d.wav` & `mpb_lib-0.1.85/mpb_lib/sound/wavs/d.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/sound/wavs/e.wav` & `mpb_lib-0.1.85/mpb_lib/sound/wavs/e.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/sound/wavs/f.wav` & `mpb_lib-0.1.85/mpb_lib/sound/wavs/f.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/sound/wavs/g.wav` & `mpb_lib-0.1.85/mpb_lib/sound/wavs/g.wav`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/tictactoe/tictactoe.py` & `mpb_lib-0.1.85/mpb_lib/tictactoe/tictactoe.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/tictactoe/tictactoe_html.py` & `mpb_lib-0.1.85/mpb_lib/tictactoe/tictactoe_html.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/vowelgen/HPF.py` & `mpb_lib-0.1.85/mpb_lib/vowelgen/HPF.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/vowelgen/__init__.py` & `mpb_lib-0.1.85/mpb_lib/vowelgen/__init__.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/vowelgen/glottal.py` & `mpb_lib-0.1.85/mpb_lib/vowelgen/glottal.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/vowelgen/threetube.py` & `mpb_lib-0.1.85/mpb_lib/vowelgen/threetube.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib/vowelgen/twotube.py` & `mpb_lib-0.1.85/mpb_lib/vowelgen/twotube.py`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/mpb_lib.egg-info/SOURCES.txt` & `mpb_lib-0.1.85/mpb_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpb_lib-0.1.84/setup.py` & `mpb_lib-0.1.85/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
                        'sound/wavs/d.wav',
                        'sound/wavs/e.wav',
                        'sound/wavs/f.wav',
                        'sound/wavs/g.wav',
                        'sound/wavs/a.wav',
                        'sound/wavs/b.wav' ]},
 
-    version='0.1.84', # バージョン
+    version='0.1.85', # バージョン
 
     license='MIT', # ライセンス
 
     install_requires=[],
 
     author='Atsushi Shibata',
     author_email='shibata@m-info.co.jp',
```

