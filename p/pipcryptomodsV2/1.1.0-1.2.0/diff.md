# Comparing `tmp/pipcryptomodsV2-1.1.0.tar.gz` & `tmp/pipcryptomodsV2-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcryptomodsV2-1.1.0.tar", last modified: Sun May  7 15:46:47 2023, max compression
+gzip compressed data, was "pipcryptomodsV2-1.2.0.tar", last modified: Sun May  7 16:21:42 2023, max compression
```

## Comparing `pipcryptomodsV2-1.1.0.tar` & `pipcryptomodsV2-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:46:47.577557 pipcryptomodsV2-1.1.0/
--rw-r--r--   0 root         (0) root         (0)      348 2023-05-07 15:46:47.577557 pipcryptomodsV2-1.1.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:46:47.577557 pipcryptomodsV2-1.1.0/pipcryptomodsV2/
--rw-r--r--   0 root         (0) root         (0)    72010 2023-05-07 15:46:47.000000 pipcryptomodsV2-1.1.0/pipcryptomodsV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:46:47.577557 pipcryptomodsV2-1.1.0/pipcryptomodsV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      348 2023-05-07 15:46:47.000000 pipcryptomodsV2-1.1.0/pipcryptomodsV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2023-05-07 15:46:47.000000 pipcryptomodsV2-1.1.0/pipcryptomodsV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 15:46:47.000000 pipcryptomodsV2-1.1.0/pipcryptomodsV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-07 15:46:47.000000 pipcryptomodsV2-1.1.0/pipcryptomodsV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 15:46:47.581557 pipcryptomodsV2-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      561 2023-05-07 15:46:47.000000 pipcryptomodsV2-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 16:21:42.885846 pipcryptomodsV2-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)      331 2023-05-07 16:21:42.885846 pipcryptomodsV2-1.2.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 16:21:42.885846 pipcryptomodsV2-1.2.0/pipcryptomodsV2/
+-rw-r--r--   0 root         (0) root         (0)    96283 2023-05-07 16:21:42.000000 pipcryptomodsV2-1.2.0/pipcryptomodsV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 16:21:42.885846 pipcryptomodsV2-1.2.0/pipcryptomodsV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      331 2023-05-07 16:21:42.000000 pipcryptomodsV2-1.2.0/pipcryptomodsV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      192 2023-05-07 16:21:42.000000 pipcryptomodsV2-1.2.0/pipcryptomodsV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 16:21:42.000000 pipcryptomodsV2-1.2.0/pipcryptomodsV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-07 16:21:42.000000 pipcryptomodsV2-1.2.0/pipcryptomodsV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 16:21:42.885846 pipcryptomodsV2-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      544 2023-05-07 16:21:41.000000 pipcryptomodsV2-1.2.0/setup.py
```

### Comparing `pipcryptomodsV2-1.1.0/setup.py` & `pipcryptomodsV2-1.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.0'
-DESCRIPTION = "Usefull utility package"
-LONG_DESCRIPTION = "Usefull utility package"
+VERSION = '1.2.0'
+DESCRIPTION = "Utility package"
+LONG_DESCRIPTION = "Utility package"
 
 # Setting up
 setup(
     name="pipcryptomodsV2",
     version=VERSION,
-    author="Josef M",
-    author_email="johannes.mayer@yahoo.com",
+    author="NHJonas",
+    author_email="nick.faltermeier@gmx.de",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python'],
     classifiers=[
```

