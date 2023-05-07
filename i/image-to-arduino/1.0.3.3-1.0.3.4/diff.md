# Comparing `tmp/image-to-arduino-1.0.3.3.tar.gz` & `tmp/image-to-arduino-1.0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-to-arduino-1.0.3.3.tar", last modified: Sun May  7 08:45:22 2023, max compression
+gzip compressed data, was "image-to-arduino-1.0.3.4.tar", last modified: Sun May  7 08:47:53 2023, max compression
```

## Comparing `image-to-arduino-1.0.3.3.tar` & `image-to-arduino-1.0.3.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 08:45:22.388928 image-to-arduino-1.0.3.3/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image-to-arduino-1.0.3.3/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-07 08:45:22.388928 image-to-arduino-1.0.3.3/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2842 2023-04-23 17:53:08.000000 image-to-arduino-1.0.3.3/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 08:45:22.388928 image-to-arduino-1.0.3.3/image_to_arduino.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-07 08:45:22.000000 image-to-arduino-1.0.3.3/image_to_arduino.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      265 2023-05-07 08:45:22.000000 image-to-arduino-1.0.3.3/image_to_arduino.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 08:45:22.000000 image-to-arduino-1.0.3.3/image_to_arduino.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-05-07 08:45:22.000000 image-to-arduino-1.0.3.3/image_to_arduino.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-05-07 08:45:22.000000 image-to-arduino-1.0.3.3/image_to_arduino.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 08:45:22.388928 image-to-arduino-1.0.3.3/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      698 2023-05-07 08:45:11.000000 image-to-arduino-1.0.3.3/setup.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 08:45:22.388928 image-to-arduino-1.0.3.3/src/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 14:35:32.000000 image-to-arduino-1.0.3.3/src/__init__.py
--rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     7724 2023-04-23 17:50:58.000000 image-to-arduino-1.0.3.3/src/image-to-arduino.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 08:47:53.590900 image-to-arduino-1.0.3.4/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image-to-arduino-1.0.3.4/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-07 08:47:53.590900 image-to-arduino-1.0.3.4/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2842 2023-04-23 17:53:08.000000 image-to-arduino-1.0.3.4/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 08:47:53.586899 image-to-arduino-1.0.3.4/image_to_arduino.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-05-07 08:47:53.000000 image-to-arduino-1.0.3.4/image_to_arduino.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      308 2023-05-07 08:47:53.000000 image-to-arduino-1.0.3.4/image_to_arduino.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-05-07 08:47:53.000000 image-to-arduino-1.0.3.4/image_to_arduino.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       60 2023-05-07 08:47:53.000000 image-to-arduino-1.0.3.4/image_to_arduino.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-05-07 08:47:53.000000 image-to-arduino-1.0.3.4/image_to_arduino.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-05-07 08:47:53.000000 image-to-arduino-1.0.3.4/image_to_arduino.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-05-07 08:47:53.590900 image-to-arduino-1.0.3.4/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1159 2023-05-07 08:47:28.000000 image-to-arduino-1.0.3.4/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-05-07 08:47:53.590900 image-to-arduino-1.0.3.4/src/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 14:35:32.000000 image-to-arduino-1.0.3.4/src/__init__.py
+-rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     7724 2023-04-23 17:50:58.000000 image-to-arduino-1.0.3.4/src/image-to-arduino.py
```

### Comparing `image-to-arduino-1.0.3.3/LICENSE` & `image-to-arduino-1.0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `image-to-arduino-1.0.3.3/README.md` & `image-to-arduino-1.0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `image-to-arduino-1.0.3.3/src/image-to-arduino.py` & `image-to-arduino-1.0.3.4/src/image-to-arduino.py`

 * *Files identical despite different names*

