# Comparing `tmp/gravitypy-1.0.1.tar.gz` & `tmp/gravitypy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitypy-1.0.1.tar", last modified: Sun May  7 17:33:36 2023, max compression
+gzip compressed data, was "gravitypy-1.0.2.tar", last modified: Sun May  7 18:16:14 2023, max compression
```

## Comparing `gravitypy-1.0.1.tar` & `gravitypy-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 17:33:36.562897 gravitypy-1.0.1/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 16:26:56.000000 gravitypy-1.0.1/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 16:26:56.000000 gravitypy-1.0.1/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 17:33:36.562897 gravitypy-1.0.1/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1005 2023-05-07 16:26:56.000000 gravitypy-1.0.1/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 17:33:36.562897 gravitypy-1.0.1/gravitypy.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 17:33:36.000000 gravitypy-1.0.1/gravitypy.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      299 2023-05-07 17:33:36.000000 gravitypy-1.0.1/gravitypy.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 17:33:36.000000 gravitypy-1.0.1/gravitypy.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       48 2023-05-07 17:33:36.000000 gravitypy-1.0.1/gravitypy.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 17:33:36.000000 gravitypy-1.0.1/gravitypy.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-05-07 17:33:36.000000 gravitypy-1.0.1/gravitypy.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 16:26:56.000000 gravitypy-1.0.1/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 17:33:36.562897 gravitypy-1.0.1/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      837 2023-05-07 17:29:56.000000 gravitypy-1.0.1/setup.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 17:33:36.562897 gravitypy-1.0.1/src/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 16:26:56.000000 gravitypy-1.0.1/src/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       64 2023-05-07 17:31:28.000000 gravitypy-1.0.1/src/__main__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15370 2023-05-07 17:31:57.000000 gravitypy-1.0.1/src/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 18:16:14.233126 gravitypy-1.0.2/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 16:26:56.000000 gravitypy-1.0.2/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 16:26:56.000000 gravitypy-1.0.2/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 18:16:14.233126 gravitypy-1.0.2/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1005 2023-05-07 16:26:56.000000 gravitypy-1.0.2/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 18:16:14.233126 gravitypy-1.0.2/gravitypy.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 18:16:14.000000 gravitypy-1.0.2/gravitypy.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      299 2023-05-07 18:16:14.000000 gravitypy-1.0.2/gravitypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 18:16:14.000000 gravitypy-1.0.2/gravitypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       48 2023-05-07 18:16:14.000000 gravitypy-1.0.2/gravitypy.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 18:16:14.000000 gravitypy-1.0.2/gravitypy.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-05-07 18:16:14.000000 gravitypy-1.0.2/gravitypy.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 16:26:56.000000 gravitypy-1.0.2/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 18:16:14.233126 gravitypy-1.0.2/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      837 2023-05-07 18:15:55.000000 gravitypy-1.0.2/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 18:16:14.233126 gravitypy-1.0.2/src/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 16:26:56.000000 gravitypy-1.0.2/src/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       64 2023-05-07 17:49:44.000000 gravitypy-1.0.2/src/__main__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15478 2023-05-07 18:15:19.000000 gravitypy-1.0.2/src/main.py
```

### Comparing `gravitypy-1.0.1/LICENSE` & `gravitypy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gravitypy-1.0.1/README.md` & `gravitypy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gravitypy-1.0.1/setup.py` & `gravitypy-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 req_file = os.path.join(here, 'requirements.txt')
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 LONG_DESCRIPTION = 'Pygame N-Body gravity simulation app'
 
 setup(
    name='gravitypy',
-   version='1.0.1',
+   version='1.0.2',
    description='Particles Gravity',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Particles_Gravity",
    long_description_content_type="text/markdown",
    long_description=LONG_DESCRIPTION,
```

### Comparing `gravitypy-1.0.1/src/main.py` & `gravitypy-1.0.2/src/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import pygame
 import random
 import math
 from pygame.locals import *
+import os
 
 pygame.init()
-pygame.display.set_caption("Gravity Simulation")
+pygame.display.set_caption("GravityPy")
 
 WIDTH, HEIGHT = 1200, 800
 SCREEN = pygame.display.set_mode((WIDTH, HEIGHT))
 CLOCK = pygame.time.Clock()
-FONT = pygame.font.Font('src/resources/fonts/minecraft_font.ttf', 16)
+
+script_dir = os.path.dirname(os.path.abspath(__file__))
+font_path = os.path.join(script_dir, 'resources', 'fonts', 'minecraft_font.ttf')
+FONT = pygame.font.Font(font_path, 16)
 G = 100
 SCALE = 1.0
 PARTICLES = []
 ADDED_RADIUS = 20
 ADDED_MASS = 20
 ADDED_VELOCITY = pygame.Vector2(0, 0)
 NUM_PARTICLES = 30
```

