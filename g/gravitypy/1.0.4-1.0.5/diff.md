# Comparing `tmp/gravitypy-1.0.4.tar.gz` & `tmp/gravitypy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitypy-1.0.4.tar", last modified: Sun May  7 19:03:58 2023, max compression
+gzip compressed data, was "gravitypy-1.0.5.tar", last modified: Sun May  7 19:21:00 2023, max compression
```

## Comparing `gravitypy-1.0.4.tar` & `gravitypy-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:03:58.016598 gravitypy-1.0.4/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 16:26:56.000000 gravitypy-1.0.4/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 16:26:56.000000 gravitypy-1.0.4/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 19:03:58.016598 gravitypy-1.0.4/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1005 2023-05-07 16:26:56.000000 gravitypy-1.0.4/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:03:58.016598 gravitypy-1.0.4/gravitypy.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 19:03:58.000000 gravitypy-1.0.4/gravitypy.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      377 2023-05-07 19:03:58.000000 gravitypy-1.0.4/gravitypy.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 19:03:58.000000 gravitypy-1.0.4/gravitypy.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       48 2023-05-07 19:03:58.000000 gravitypy-1.0.4/gravitypy.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 19:03:58.000000 gravitypy-1.0.4/gravitypy.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-05-07 19:03:58.000000 gravitypy-1.0.4/gravitypy.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 16:26:56.000000 gravitypy-1.0.4/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 19:03:58.016598 gravitypy-1.0.4/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      957 2023-05-07 19:03:40.000000 gravitypy-1.0.4/setup.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:03:58.016598 gravitypy-1.0.4/src/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 16:26:56.000000 gravitypy-1.0.4/src/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       64 2023-05-07 17:49:44.000000 gravitypy-1.0.4/src/__main__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15390 2023-05-07 19:03:12.000000 gravitypy-1.0.4/src/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:21:00.846722 gravitypy-1.0.5/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 16:26:56.000000 gravitypy-1.0.5/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 16:26:56.000000 gravitypy-1.0.5/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 19:21:00.846722 gravitypy-1.0.5/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1005 2023-05-07 16:26:56.000000 gravitypy-1.0.5/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:21:00.846722 gravitypy-1.0.5/gravitypy/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 16:26:56.000000 gravitypy-1.0.5/gravitypy/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       64 2023-05-07 17:49:44.000000 gravitypy-1.0.5/gravitypy/__main__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15448 2023-05-07 19:20:12.000000 gravitypy-1.0.5/gravitypy/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:21:00.842723 gravitypy-1.0.5/gravitypy/resources/
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:21:00.846722 gravitypy-1.0.5/gravitypy/resources/fonts/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 16:26:56.000000 gravitypy-1.0.5/gravitypy/resources/fonts/minecraft_font.ttf
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:21:00.846722 gravitypy-1.0.5/gravitypy.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 19:21:00.000000 gravitypy-1.0.5/gravitypy.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-05-07 19:21:00.000000 gravitypy-1.0.5/gravitypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 19:21:00.000000 gravitypy-1.0.5/gravitypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       48 2023-05-07 19:21:00.000000 gravitypy-1.0.5/gravitypy.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 19:21:00.000000 gravitypy-1.0.5/gravitypy.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-05-07 19:21:00.000000 gravitypy-1.0.5/gravitypy.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 16:26:56.000000 gravitypy-1.0.5/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 19:21:00.846722 gravitypy-1.0.5/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      899 2023-05-07 19:19:39.000000 gravitypy-1.0.5/setup.py
```

### Comparing `gravitypy-1.0.4/LICENSE` & `gravitypy-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gravitypy-1.0.4/README.md` & `gravitypy-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gravitypy-1.0.4/setup.py` & `gravitypy-1.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,25 +5,24 @@
 req_file = os.path.join(here, 'requirements.txt')
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 LONG_DESCRIPTION = 'Pygame N-Body gravity simulation app'
 
 setup(
    name='gravitypy',
-   version='1.0.4',
+   version='1.0.5',
    description='Particles Gravity',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Particles_Gravity",
    long_description_content_type="text/markdown",
    long_description=LONG_DESCRIPTION,
-   packages=['src'],
-   package_data={'src': ['data/*.dat']},
-   data_files=[('resources/fonts', ['/home/wiktor/Desktop/Particles_Gravity/src/resources/fonts/minecraft_font.ttf'])],
+   packages=['gravitypy'],
+   data_files=[('gravitypy/resources/fonts', ['gravitypy/resources/fonts/minecraft_font.ttf'])],
    install_requires=REQUIREMENTS, 
     entry_points={
         'console_scripts': [
             'gravitypy = src.__main__:main'
         ]
     },
```

### Comparing `gravitypy-1.0.4/src/main.py` & `gravitypy-1.0.5/gravitypy/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 
 pygame.init()
 pygame.display.set_caption("GravityPy")
 
 WIDTH, HEIGHT = 1200, 800
 SCREEN = pygame.display.set_mode((WIDTH, HEIGHT))
 CLOCK = pygame.time.Clock()
+font_path = os.path.join(os.path.dirname(__file__), 'gravitypy/resources/fonts/minecraft_font.ttf')
 
-FONT = pygame.font.Font('Desktop/Particles_Gravity/src/resources/fonts/myfont.ttf', 16)
+FONT = pygame.font.Font(font_path, font_size)
 G = 100
 SCALE = 1.0
 PARTICLES = []
 ADDED_RADIUS = 20
 ADDED_MASS = 20
 ADDED_VELOCITY = pygame.Vector2(0, 0)
 NUM_PARTICLES = 30
```

