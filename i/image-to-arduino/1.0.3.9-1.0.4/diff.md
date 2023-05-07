# Comparing `tmp/image-to-arduino-1.0.3.9.tar.gz` & `tmp/image-to-arduino-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-to-arduino-1.0.3.9.tar", last modified: Sun May  7 12:33:05 2023, max compression
+gzip compressed data, was "image-to-arduino-1.0.4.tar", last modified: Sun May  7 12:36:51 2023, max compression
```

## Comparing `image-to-arduino-1.0.3.9.tar` & `image-to-arduino-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 12:33:05.576532 image-to-arduino-1.0.3.9/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image-to-arduino-1.0.3.9/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 10:45:25.000000 image-to-arduino-1.0.3.9/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-07 12:33:05.576532 image-to-arduino-1.0.3.9/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2842 2023-04-23 17:53:08.000000 image-to-arduino-1.0.3.9/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 12:33:05.576532 image-to-arduino-1.0.3.9/image_to_arduino.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-07 12:33:05.000000 image-to-arduino-1.0.3.9/image_to_arduino.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      351 2023-05-07 12:33:05.000000 image-to-arduino-1.0.3.9/image_to_arduino.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 12:33:05.000000 image-to-arduino-1.0.3.9/image_to_arduino.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       59 2023-05-07 12:33:05.000000 image-to-arduino-1.0.3.9/image_to_arduino.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-05-07 12:33:05.000000 image-to-arduino-1.0.3.9/image_to_arduino.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-05-07 12:33:05.000000 image-to-arduino-1.0.3.9/image_to_arduino.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       77 2023-04-22 13:23:37.000000 image-to-arduino-1.0.3.9/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 12:33:05.576532 image-to-arduino-1.0.3.9/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1154 2023-05-07 12:32:40.000000 image-to-arduino-1.0.3.9/setup.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 12:33:05.576532 image-to-arduino-1.0.3.9/src/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 14:35:32.000000 image-to-arduino-1.0.3.9/src/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       71 2023-05-07 12:29:24.000000 image-to-arduino-1.0.3.9/src/__main__.py
--rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     8329 2023-05-07 12:28:36.000000 image-to-arduino-1.0.3.9/src/imagetoarduino.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 12:36:51.848554 image-to-arduino-1.0.4/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image-to-arduino-1.0.4/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-07 10:45:25.000000 image-to-arduino-1.0.4/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-05-07 12:36:51.848554 image-to-arduino-1.0.4/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2842 2023-04-23 17:53:08.000000 image-to-arduino-1.0.4/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 12:36:51.848554 image-to-arduino-1.0.4/image_to_arduino.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-05-07 12:36:51.000000 image-to-arduino-1.0.4/image_to_arduino.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      351 2023-05-07 12:36:51.000000 image-to-arduino-1.0.4/image_to_arduino.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 12:36:51.000000 image-to-arduino-1.0.4/image_to_arduino.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       53 2023-05-07 12:36:51.000000 image-to-arduino-1.0.4/image_to_arduino.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-05-07 12:36:51.000000 image-to-arduino-1.0.4/image_to_arduino.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-05-07 12:36:51.000000 image-to-arduino-1.0.4/image_to_arduino.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       77 2023-04-22 13:23:37.000000 image-to-arduino-1.0.4/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 12:36:51.848554 image-to-arduino-1.0.4/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1146 2023-05-07 12:36:34.000000 image-to-arduino-1.0.4/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 12:36:51.848554 image-to-arduino-1.0.4/src/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 14:35:32.000000 image-to-arduino-1.0.4/src/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       71 2023-05-07 12:29:24.000000 image-to-arduino-1.0.4/src/__main__.py
+-rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     8329 2023-05-07 12:28:36.000000 image-to-arduino-1.0.4/src/imagetoarduino.py
```

### Comparing `image-to-arduino-1.0.3.9/LICENSE` & `image-to-arduino-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `image-to-arduino-1.0.3.9/README.md` & `image-to-arduino-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `image-to-arduino-1.0.3.9/setup.py` & `image-to-arduino-1.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 # Read the requirements.txt file and split into a list of lines
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 LONG_DESCRIPTION = 'About Image converter GUI App to arduino oled display ssd1306 128x64'
 
 setup(
    name='image-to-arduino',
-   version='1.0.3.9',
+   version='1.0.4',
    description='Image converter to arduino',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Image_Converter_App.git",
    long_description_content_type="text/markdown",
    long_description=LONG_DESCRIPTION,
    packages=['src'],
    package_data={'src': ['data/*.dat']},
    install_requires=REQUIREMENTS, 
     entry_points={
         'console_scripts': [
-            'imagetoarduino = src.imagetoarduino:main'
+            'imagetoarduino = src.__main__:main'
         ]
     },
 
 )
```

### Comparing `image-to-arduino-1.0.3.9/src/imagetoarduino.py` & `image-to-arduino-1.0.4/src/imagetoarduino.py`

 * *Files identical despite different names*

