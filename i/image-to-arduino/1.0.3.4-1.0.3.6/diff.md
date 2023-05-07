# Comparing `tmp/image-to-arduino-1.0.3.4.tar.gz` & `tmp/image-to-arduino-1.0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-to-arduino-1.0.3.4.tar", last modified: Sun May  7 08:47:53 2023, max compression
+gzip compressed data, was "image-to-arduino-1.0.3.6.tar", last modified: Sun May  7 09:02:50 2023, max compression
```

## Comparing `image-to-arduino-1.0.3.4.tar` & `image-to-arduino-1.0.3.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 08:47:53.590900 image-to-arduino-1.0.3.4/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image-to-arduino-1.0.3.4/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-07 08:47:53.590900 image-to-arduino-1.0.3.4/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2842 2023-04-23 17:53:08.000000 image-to-arduino-1.0.3.4/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 08:47:53.586899 image-to-arduino-1.0.3.4/image_to_arduino.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-07 08:47:53.000000 image-to-arduino-1.0.3.4/image_to_arduino.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 08:47:53.000000 image-to-arduino-1.0.3.4/image_to_arduino.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 08:47:53.000000 image-to-arduino-1.0.3.4/image_to_arduino.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       60 2023-05-07 08:47:53.000000 image-to-arduino-1.0.3.4/image_to_arduino.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-05-07 08:47:53.000000 image-to-arduino-1.0.3.4/image_to_arduino.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-05-07 08:47:53.000000 image-to-arduino-1.0.3.4/image_to_arduino.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 08:47:53.590900 image-to-arduino-1.0.3.4/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1159 2023-05-07 08:47:28.000000 image-to-arduino-1.0.3.4/setup.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 08:47:53.590900 image-to-arduino-1.0.3.4/src/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 14:35:32.000000 image-to-arduino-1.0.3.4/src/__init__.py
--rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     7724 2023-04-23 17:50:58.000000 image-to-arduino-1.0.3.4/src/image-to-arduino.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 09:02:50.932516 image-to-arduino-1.0.3.6/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image-to-arduino-1.0.3.6/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-07 09:02:50.932516 image-to-arduino-1.0.3.6/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2842 2023-04-23 17:53:08.000000 image-to-arduino-1.0.3.6/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 09:02:50.932516 image-to-arduino-1.0.3.6/image_to_arduino.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-07 09:02:50.000000 image-to-arduino-1.0.3.6/image_to_arduino.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 09:02:50.000000 image-to-arduino-1.0.3.6/image_to_arduino.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 09:02:50.000000 image-to-arduino-1.0.3.6/image_to_arduino.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       54 2023-05-07 09:02:50.000000 image-to-arduino-1.0.3.6/image_to_arduino.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-05-07 09:02:50.000000 image-to-arduino-1.0.3.6/image_to_arduino.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-05-07 09:02:50.000000 image-to-arduino-1.0.3.6/image_to_arduino.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 09:02:50.932516 image-to-arduino-1.0.3.6/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1153 2023-05-07 09:02:40.000000 image-to-arduino-1.0.3.6/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 09:02:50.932516 image-to-arduino-1.0.3.6/src/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 14:35:32.000000 image-to-arduino-1.0.3.6/src/__init__.py
+-rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     7724 2023-04-23 17:50:58.000000 image-to-arduino-1.0.3.6/src/image-to-arduino.py
```

### Comparing `image-to-arduino-1.0.3.4/LICENSE` & `image-to-arduino-1.0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `image-to-arduino-1.0.3.4/README.md` & `image-to-arduino-1.0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `image-to-arduino-1.0.3.4/setup.py` & `image-to-arduino-1.0.3.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,28 +13,28 @@
     def finalize_options(self):
         pass
 
     def run(self):
         os.system('python3 image-to-arduino.py')
 setup(
    name='image-to-arduino',
-   version='1.0.3.4',
+   version='1.0.3.6',
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
-            'mycommand = mypackage.mycommand:MyCommand'
+            'mycommand = src.mycommand:MyCommand'
         ]
     },
    cmdclass={
         'mycommand': MyCommand
     }
 
 )
```

### Comparing `image-to-arduino-1.0.3.4/src/image-to-arduino.py` & `image-to-arduino-1.0.3.6/src/image-to-arduino.py`

 * *Files identical despite different names*

