# Comparing `tmp/gravitypy-1.0.6.tar.gz` & `tmp/gravitypy-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitypy-1.0.6.tar", last modified: Sun May  7 19:23:55 2023, max compression
+gzip compressed data, was "gravitypy-1.0.7.tar", last modified: Sun May  7 19:25:44 2023, max compression
```

## Comparing `gravitypy-1.0.6.tar` & `gravitypy-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:23:55.306415 gravitypy-1.0.6/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 16:26:56.000000 gravitypy-1.0.6/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 16:26:56.000000 gravitypy-1.0.6/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 19:23:55.306415 gravitypy-1.0.6/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1005 2023-05-07 16:26:56.000000 gravitypy-1.0.6/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:23:55.306415 gravitypy-1.0.6/gravitypy/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 16:26:56.000000 gravitypy-1.0.6/gravitypy/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-07 19:23:07.000000 gravitypy-1.0.6/gravitypy/__main__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15448 2023-05-07 19:20:12.000000 gravitypy-1.0.6/gravitypy/main.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:23:55.306415 gravitypy-1.0.6/gravitypy/resources/
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:23:55.306415 gravitypy-1.0.6/gravitypy/resources/fonts/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 16:26:56.000000 gravitypy-1.0.6/gravitypy/resources/fonts/minecraft_font.ttf
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:23:55.306415 gravitypy-1.0.6/gravitypy.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 19:23:55.000000 gravitypy-1.0.6/gravitypy.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-05-07 19:23:55.000000 gravitypy-1.0.6/gravitypy.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 19:23:55.000000 gravitypy-1.0.6/gravitypy.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       48 2023-05-07 19:23:55.000000 gravitypy-1.0.6/gravitypy.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 19:23:55.000000 gravitypy-1.0.6/gravitypy.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-05-07 19:23:55.000000 gravitypy-1.0.6/gravitypy.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 16:26:56.000000 gravitypy-1.0.6/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 19:23:55.306415 gravitypy-1.0.6/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      899 2023-05-07 19:23:44.000000 gravitypy-1.0.6/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:25:44.486248 gravitypy-1.0.7/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 16:26:56.000000 gravitypy-1.0.7/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 16:26:56.000000 gravitypy-1.0.7/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 19:25:44.486248 gravitypy-1.0.7/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1005 2023-05-07 16:26:56.000000 gravitypy-1.0.7/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:25:44.486248 gravitypy-1.0.7/gravitypy/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 16:26:56.000000 gravitypy-1.0.7/gravitypy/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       70 2023-05-07 19:25:11.000000 gravitypy-1.0.7/gravitypy/__main__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15448 2023-05-07 19:20:12.000000 gravitypy-1.0.7/gravitypy/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:25:44.482248 gravitypy-1.0.7/gravitypy/resources/
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:25:44.486248 gravitypy-1.0.7/gravitypy/resources/fonts/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15700 2023-05-07 16:26:56.000000 gravitypy-1.0.7/gravitypy/resources/fonts/minecraft_font.ttf
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 19:25:44.486248 gravitypy-1.0.7/gravitypy.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 19:25:44.000000 gravitypy-1.0.7/gravitypy.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-05-07 19:25:44.000000 gravitypy-1.0.7/gravitypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 19:25:44.000000 gravitypy-1.0.7/gravitypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       48 2023-05-07 19:25:44.000000 gravitypy-1.0.7/gravitypy.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 19:25:44.000000 gravitypy-1.0.7/gravitypy.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       10 2023-05-07 19:25:44.000000 gravitypy-1.0.7/gravitypy.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 16:26:56.000000 gravitypy-1.0.7/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 19:25:44.486248 gravitypy-1.0.7/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      899 2023-05-07 19:25:33.000000 gravitypy-1.0.7/setup.py
```

### Comparing `gravitypy-1.0.6/LICENSE` & `gravitypy-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gravitypy-1.0.6/README.md` & `gravitypy-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gravitypy-1.0.6/gravitypy/main.py` & `gravitypy-1.0.7/gravitypy/main.py`

 * *Files identical despite different names*

### Comparing `gravitypy-1.0.6/gravitypy/resources/fonts/minecraft_font.ttf` & `gravitypy-1.0.7/gravitypy/resources/fonts/minecraft_font.ttf`

 * *Files identical despite different names*

### Comparing `gravitypy-1.0.6/setup.py` & `gravitypy-1.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 req_file = os.path.join(here, 'requirements.txt')
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 LONG_DESCRIPTION = 'Pygame N-Body gravity simulation app'
 
 setup(
    name='gravitypy',
-   version='1.0.6',
+   version='1.0.7',
    description='Particles Gravity',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Particles_Gravity",
    long_description_content_type="text/markdown",
    long_description=LONG_DESCRIPTION,
```

