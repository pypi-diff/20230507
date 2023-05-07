# Comparing `tmp/ImageMagic-0.1.7.tar.gz` & `tmp/ImageMagic-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ImageMagic-0.1.7.tar", last modified: Sun May  7 01:24:37 2023, max compression
+gzip compressed data, was "ImageMagic-0.1.8.tar", last modified: Sun May  7 01:47:02 2023, max compression
```

## Comparing `ImageMagic-0.1.7.tar` & `ImageMagic-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 01:24:37.957534 ImageMagic-0.1.7/
-drwxrwxrwx   0        0        0        0 2023-05-07 01:24:37.941909 ImageMagic-0.1.7/ImageMagic/
--rw-rw-rw-   0        0        0     6237 2023-05-07 00:54:28.000000 ImageMagic-0.1.7/ImageMagic/Aocr.py
--rw-rw-rw-   0        0        0    13766 2023-05-07 01:13:22.000000 ImageMagic-0.1.7/ImageMagic/Image.py
--rw-rw-rw-   0        0        0    12963 2023-05-04 09:07:20.000000 ImageMagic-0.1.7/ImageMagic/_Atesseract.py
--rw-rw-rw-   0        0        0      260 2023-05-04 12:55:21.000000 ImageMagic-0.1.7/ImageMagic/__init__.py
--rw-rw-rw-   0        0        0       85 2023-05-07 01:24:05.000000 ImageMagic-0.1.7/ImageMagic/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-07 01:24:37.957534 ImageMagic-0.1.7/ImageMagic.egg-info/
--rw-rw-rw-   0        0        0      500 2023-05-07 01:24:37.000000 ImageMagic-0.1.7/ImageMagic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-05-07 01:24:37.000000 ImageMagic-0.1.7/ImageMagic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 01:24:37.000000 ImageMagic-0.1.7/ImageMagic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-07 01:24:37.000000 ImageMagic-0.1.7/ImageMagic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 01:24:37.000000 ImageMagic-0.1.7/ImageMagic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2023-05-02 08:31:43.000000 ImageMagic-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      500 2023-05-07 01:24:37.957534 ImageMagic-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1231 2023-05-06 11:02:24.000000 ImageMagic-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-05-07 01:24:37.957534 ImageMagic-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      793 2023-05-06 05:17:18.000000 ImageMagic-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 01:24:37.957534 ImageMagic-0.1.7/test/
--rw-rw-rw-   0        0        0     1286 2023-05-07 01:21:31.000000 ImageMagic-0.1.7/test/test.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:47:02.358485 ImageMagic-0.1.8/
+drwxrwxrwx   0        0        0        0 2023-05-07 01:47:02.342857 ImageMagic-0.1.8/ImageMagic/
+-rw-rw-rw-   0        0        0     6237 2023-05-07 00:54:28.000000 ImageMagic-0.1.8/ImageMagic/Aocr.py
+-rw-rw-rw-   0        0        0    13766 2023-05-07 01:13:22.000000 ImageMagic-0.1.8/ImageMagic/Image.py
+-rw-rw-rw-   0        0        0    12963 2023-05-04 09:07:20.000000 ImageMagic-0.1.8/ImageMagic/_Atesseract.py
+-rw-rw-rw-   0        0        0      260 2023-05-04 12:55:21.000000 ImageMagic-0.1.8/ImageMagic/__init__.py
+-rw-rw-rw-   0        0        0       85 2023-05-07 01:46:11.000000 ImageMagic-0.1.8/ImageMagic/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:47:02.358485 ImageMagic-0.1.8/ImageMagic.egg-info/
+-rw-rw-rw-   0        0        0      500 2023-05-07 01:47:02.000000 ImageMagic-0.1.8/ImageMagic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-05-07 01:47:02.000000 ImageMagic-0.1.8/ImageMagic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 01:47:02.000000 ImageMagic-0.1.8/ImageMagic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-07 01:47:02.000000 ImageMagic-0.1.8/ImageMagic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-07 01:47:02.000000 ImageMagic-0.1.8/ImageMagic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2023-05-02 08:31:43.000000 ImageMagic-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      500 2023-05-07 01:47:02.358485 ImageMagic-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1231 2023-05-06 11:02:24.000000 ImageMagic-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-07 01:47:02.358485 ImageMagic-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      792 2023-05-07 01:41:00.000000 ImageMagic-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 01:47:02.358485 ImageMagic-0.1.8/test/
+-rw-rw-rw-   0        0        0       26 2023-05-06 05:17:57.000000 ImageMagic-0.1.8/test/__init__.py
+-rw-rw-rw-   0        0        0     1286 2023-05-07 01:21:31.000000 ImageMagic-0.1.8/test/test.py
```

### Comparing `ImageMagic-0.1.7/ImageMagic/Aocr.py` & `ImageMagic-0.1.8/ImageMagic/Aocr.py`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.7/ImageMagic/Image.py` & `ImageMagic-0.1.8/ImageMagic/Image.py`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.7/ImageMagic/_Atesseract.py` & `ImageMagic-0.1.8/ImageMagic/_Atesseract.py`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.7/LICENSE` & `ImageMagic-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.7/README.md` & `ImageMagic-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ImageMagic-0.1.7/setup.py` & `ImageMagic-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup,find_packages
 from ImageMagic import _version
 
 setup(
     name='ImageMagic',
     version=_version.__version__,
-    packages=find_packages(exclude='test*'),
+    packages=find_packages(exclude='test'),
     url='https://github.com/asxez/ImageMagic',
     license='GNU GPL 3.0',
     author='asxe',
     author_email='2973918177@qq.com',
     description='图像处理库（包括但不限于图像）【Image processing libraries (including but not limited to images)】',
     long_description='It is a neat image processing library, and you can even achieve what you want with just one line of code, such as text-to-image or image content recognition (OCR), and more!',
     install_requires=[
```

### Comparing `ImageMagic-0.1.7/test/test.py` & `ImageMagic-0.1.8/test/test.py`

 * *Files identical despite different names*

