# Comparing `tmp/gravitypy-1.0.0.tar.gz` & `tmp/gravitypy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitypy-1.0.0.tar", last modified: Sun May  7 14:11:47 2023, max compression
+gzip compressed data, was "gravitypy-1.0.1.tar", last modified: Sun May  7 17:33:36 2023, max compression
```

## Comparing `gravitypy-1.0.0.tar` & `gravitypy-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 14:11:47.170602 gravitypy-1.0.0/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-01 16:37:53.000000 gravitypy-1.0.0/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 13:54:04.000000 gravitypy-1.0.0/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 14:11:47.170602 gravitypy-1.0.0/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1005 2023-05-07 08:09:59.000000 gravitypy-1.0.0/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 14:11:47.166602 gravitypy-1.0.0/gravitypy.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 14:11:47.000000 gravitypy-1.0.0/gravitypy.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      283 2023-05-07 14:11:47.000000 gravitypy-1.0.0/gravitypy.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 14:11:47.000000 gravitypy-1.0.0/gravitypy.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       44 2023-05-07 14:11:47.000000 gravitypy-1.0.0/gravitypy.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 14:11:47.000000 gravitypy-1.0.0/gravitypy.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-05-07 14:11:47.000000 gravitypy-1.0.0/gravitypy.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-06 17:12:58.000000 gravitypy-1.0.0/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 14:11:47.170602 gravitypy-1.0.0/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      833 2023-05-07 14:11:38.000000 gravitypy-1.0.0/setup.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 14:11:47.166602 gravitypy-1.0.0/src/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-06 16:22:33.000000 gravitypy-1.0.0/src/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    13613 2023-05-07 13:52:51.000000 gravitypy-1.0.0/src/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 17:33:36.562897 gravitypy-1.0.1/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-07 16:26:56.000000 gravitypy-1.0.1/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 16:26:56.000000 gravitypy-1.0.1/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 17:33:36.562897 gravitypy-1.0.1/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1005 2023-05-07 16:26:56.000000 gravitypy-1.0.1/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 17:33:36.562897 gravitypy-1.0.1/gravitypy.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 17:33:36.000000 gravitypy-1.0.1/gravitypy.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      299 2023-05-07 17:33:36.000000 gravitypy-1.0.1/gravitypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 17:33:36.000000 gravitypy-1.0.1/gravitypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       48 2023-05-07 17:33:36.000000 gravitypy-1.0.1/gravitypy.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 17:33:36.000000 gravitypy-1.0.1/gravitypy.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-05-07 17:33:36.000000 gravitypy-1.0.1/gravitypy.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       14 2023-05-07 16:26:56.000000 gravitypy-1.0.1/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 17:33:36.562897 gravitypy-1.0.1/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      837 2023-05-07 17:29:56.000000 gravitypy-1.0.1/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 17:33:36.562897 gravitypy-1.0.1/src/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 16:26:56.000000 gravitypy-1.0.1/src/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       64 2023-05-07 17:31:28.000000 gravitypy-1.0.1/src/__main__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)    15370 2023-05-07 17:31:57.000000 gravitypy-1.0.1/src/main.py
```

### Comparing `gravitypy-1.0.0/LICENSE` & `gravitypy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gravitypy-1.0.0/README.md` & `gravitypy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gravitypy-1.0.0/setup.py` & `gravitypy-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 req_file = os.path.join(here, 'requirements.txt')
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 LONG_DESCRIPTION = 'Pygame N-Body gravity simulation app'
 
 setup(
    name='gravitypy',
-   version='1.0.0',
+   version='1.0.1',
    description='Particles Gravity',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Particles_Gravity",
    long_description_content_type="text/markdown",
    long_description=LONG_DESCRIPTION,
    packages=['src'],
    package_data={'src': ['data/*.dat']},
    install_requires=REQUIREMENTS, 
     entry_points={
         'console_scripts': [
-            'gravitypy = src.main:main'
+            'gravitypy = src.__main__:main'
         ]
     },
 
 )
```

