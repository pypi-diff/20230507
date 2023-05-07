# Comparing `tmp/syssqlitedbpackageV1-1.0.0.tar.gz` & `tmp/syssqlitedbpackageV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syssqlitedbpackageV1-1.0.0.tar", last modified: Sun May  7 17:03:44 2023, max compression
+gzip compressed data, was "syssqlitedbpackageV1-1.1.0.tar", last modified: Sun May  7 17:05:51 2023, max compression
```

## Comparing `syssqlitedbpackageV1-1.0.0.tar` & `syssqlitedbpackageV1-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 17:03:44.322357 syssqlitedbpackageV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      353 2023-05-07 17:03:44.322357 syssqlitedbpackageV1-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 17:03:44.322357 syssqlitedbpackageV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      566 2023-05-07 17:03:44.000000 syssqlitedbpackageV1-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 17:03:44.322357 syssqlitedbpackageV1-1.0.0/syssqlitedbpackageV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-07 17:03:44.000000 syssqlitedbpackageV1-1.0.0/syssqlitedbpackageV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 17:03:44.322357 syssqlitedbpackageV1-1.0.0/syssqlitedbpackageV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2023-05-07 17:03:44.000000 syssqlitedbpackageV1-1.0.0/syssqlitedbpackageV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2023-05-07 17:03:44.000000 syssqlitedbpackageV1-1.0.0/syssqlitedbpackageV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 17:03:44.000000 syssqlitedbpackageV1-1.0.0/syssqlitedbpackageV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-07 17:03:44.000000 syssqlitedbpackageV1-1.0.0/syssqlitedbpackageV1.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 17:05:51.168995 syssqlitedbpackageV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-05-07 17:05:51.168995 syssqlitedbpackageV1-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 17:05:51.168995 syssqlitedbpackageV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      566 2023-05-07 17:05:50.000000 syssqlitedbpackageV1-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 17:05:51.168995 syssqlitedbpackageV1-1.1.0/syssqlitedbpackageV1/
+-rw-r--r--   0 root         (0) root         (0)    96279 2023-05-07 17:05:50.000000 syssqlitedbpackageV1-1.1.0/syssqlitedbpackageV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 17:05:51.168995 syssqlitedbpackageV1-1.1.0/syssqlitedbpackageV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-05-07 17:05:51.000000 syssqlitedbpackageV1-1.1.0/syssqlitedbpackageV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2023-05-07 17:05:51.000000 syssqlitedbpackageV1-1.1.0/syssqlitedbpackageV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 17:05:51.000000 syssqlitedbpackageV1-1.1.0/syssqlitedbpackageV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-07 17:05:51.000000 syssqlitedbpackageV1-1.1.0/syssqlitedbpackageV1.egg-info/top_level.txt
```

### Comparing `syssqlitedbpackageV1-1.0.0/setup.py` & `syssqlitedbpackageV1-1.1.0/setup.py`

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
     name="syssqlitedbpackageV1",
     version=VERSION,
```

