# Comparing `tmp/pipcryptomodsV2-1.0.0.tar.gz` & `tmp/pipcryptomodsV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcryptomodsV2-1.0.0.tar", last modified: Sun May  7 15:44:42 2023, max compression
+gzip compressed data, was "pipcryptomodsV2-1.1.0.tar", last modified: Sun May  7 15:46:47 2023, max compression
```

## Comparing `pipcryptomodsV2-1.0.0.tar` & `pipcryptomodsV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:44:42.922912 pipcryptomodsV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      348 2023-05-07 15:44:42.922912 pipcryptomodsV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:44:42.922912 pipcryptomodsV2-1.0.0/pipcryptomodsV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-07 15:44:42.000000 pipcryptomodsV2-1.0.0/pipcryptomodsV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:44:42.922912 pipcryptomodsV2-1.0.0/pipcryptomodsV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      348 2023-05-07 15:44:42.000000 pipcryptomodsV2-1.0.0/pipcryptomodsV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2023-05-07 15:44:42.000000 pipcryptomodsV2-1.0.0/pipcryptomodsV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 15:44:42.000000 pipcryptomodsV2-1.0.0/pipcryptomodsV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-07 15:44:42.000000 pipcryptomodsV2-1.0.0/pipcryptomodsV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 15:44:42.922912 pipcryptomodsV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      561 2023-05-07 15:44:42.000000 pipcryptomodsV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:46:47.577557 pipcryptomodsV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-05-07 15:46:47.577557 pipcryptomodsV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:46:47.577557 pipcryptomodsV2-1.1.0/pipcryptomodsV2/
+-rw-r--r--   0 root         (0) root         (0)    72010 2023-05-07 15:46:47.000000 pipcryptomodsV2-1.1.0/pipcryptomodsV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:46:47.577557 pipcryptomodsV2-1.1.0/pipcryptomodsV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-05-07 15:46:47.000000 pipcryptomodsV2-1.1.0/pipcryptomodsV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      192 2023-05-07 15:46:47.000000 pipcryptomodsV2-1.1.0/pipcryptomodsV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 15:46:47.000000 pipcryptomodsV2-1.1.0/pipcryptomodsV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-07 15:46:47.000000 pipcryptomodsV2-1.1.0/pipcryptomodsV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 15:46:47.581557 pipcryptomodsV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      561 2023-05-07 15:46:47.000000 pipcryptomodsV2-1.1.0/setup.py
```

### Comparing `pipcryptomodsV2-1.0.0/setup.py` & `pipcryptomodsV2-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pipcryptomodsV2",
     version=VERSION,
```

