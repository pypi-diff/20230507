# Comparing `tmp/bumbo_shogo-0.0.1.tar.gz` & `tmp/bumbo_shogo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bumbo_shogo-0.0.1.tar", last modified: Sat May  6 14:58:19 2023, max compression
+gzip compressed data, was "bumbo_shogo-0.0.2.tar", last modified: Sun May  7 02:12:45 2023, max compression
```

## Comparing `bumbo_shogo-0.0.1.tar` & `bumbo_shogo-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 Shogo      (501) staff       (20)        0 2023-05-06 14:58:19.658910 bumbo_shogo-0.0.1/
--rw-r--r--   0 Shogo      (501) staff       (20)      396 2023-05-06 14:58:19.658468 bumbo_shogo-0.0.1/PKG-INFO
-drwxr-xr-x   0 Shogo      (501) staff       (20)        0 2023-05-06 14:58:19.646342 bumbo_shogo-0.0.1/bumbo/
--rw-r--r--   0 Shogo      (501) staff       (20)        0 2023-05-06 14:48:44.000000 bumbo_shogo-0.0.1/bumbo/__init__.py
--rw-r--r--   0 Shogo      (501) staff       (20)     3789 2023-05-06 14:48:23.000000 bumbo_shogo-0.0.1/bumbo/api.py
--rw-r--r--   0 Shogo      (501) staff       (20)      674 2023-05-06 11:54:24.000000 bumbo_shogo-0.0.1/bumbo/middleware.py
--rw-r--r--   0 Shogo      (501) staff       (20)      955 2023-05-06 14:40:43.000000 bumbo_shogo-0.0.1/bumbo/response.py
-drwxr-xr-x   0 Shogo      (501) staff       (20)        0 2023-05-06 14:58:19.657755 bumbo_shogo-0.0.1/bumbo_shogo.egg-info/
--rw-r--r--   0 Shogo      (501) staff       (20)      396 2023-05-06 14:58:19.000000 bumbo_shogo-0.0.1/bumbo_shogo.egg-info/PKG-INFO
--rw-r--r--   0 Shogo      (501) staff       (20)      251 2023-05-06 14:58:19.000000 bumbo_shogo-0.0.1/bumbo_shogo.egg-info/SOURCES.txt
--rw-r--r--   0 Shogo      (501) staff       (20)        1 2023-05-06 14:58:19.000000 bumbo_shogo-0.0.1/bumbo_shogo.egg-info/dependency_links.txt
--rw-r--r--   0 Shogo      (501) staff       (20)      106 2023-05-06 14:58:19.000000 bumbo_shogo-0.0.1/bumbo_shogo.egg-info/requires.txt
--rw-r--r--   0 Shogo      (501) staff       (20)        6 2023-05-06 14:58:19.000000 bumbo_shogo-0.0.1/bumbo_shogo.egg-info/top_level.txt
--rw-r--r--   0 Shogo      (501) staff       (20)       38 2023-05-06 14:58:19.659083 bumbo_shogo-0.0.1/setup.cfg
--rw-r--r--   0 Shogo      (501) staff       (20)     1792 2023-05-06 14:51:32.000000 bumbo_shogo-0.0.1/setup.py
+drwxr-xr-x   0 Shogo      (501) staff       (20)        0 2023-05-07 02:12:45.093917 bumbo_shogo-0.0.2/
+-rw-r--r--   0 Shogo      (501) staff       (20)     3828 2023-05-07 02:12:45.093443 bumbo_shogo-0.0.2/PKG-INFO
+-rw-r--r--   0 Shogo      (501) staff       (20)     3486 2023-05-07 02:07:23.000000 bumbo_shogo-0.0.2/README.md
+drwxr-xr-x   0 Shogo      (501) staff       (20)        0 2023-05-07 02:12:45.087940 bumbo_shogo-0.0.2/bumbo/
+-rw-r--r--   0 Shogo      (501) staff       (20)        0 2023-05-06 14:48:44.000000 bumbo_shogo-0.0.2/bumbo/__init__.py
+-rw-r--r--   0 Shogo      (501) staff       (20)     3789 2023-05-06 14:48:23.000000 bumbo_shogo-0.0.2/bumbo/api.py
+-rw-r--r--   0 Shogo      (501) staff       (20)      674 2023-05-06 11:54:24.000000 bumbo_shogo-0.0.2/bumbo/middleware.py
+-rw-r--r--   0 Shogo      (501) staff       (20)      955 2023-05-06 14:40:43.000000 bumbo_shogo-0.0.2/bumbo/response.py
+drwxr-xr-x   0 Shogo      (501) staff       (20)        0 2023-05-07 02:12:45.092058 bumbo_shogo-0.0.2/bumbo_shogo.egg-info/
+-rw-r--r--   0 Shogo      (501) staff       (20)     3828 2023-05-07 02:12:44.000000 bumbo_shogo-0.0.2/bumbo_shogo.egg-info/PKG-INFO
+-rw-r--r--   0 Shogo      (501) staff       (20)      261 2023-05-07 02:12:45.000000 bumbo_shogo-0.0.2/bumbo_shogo.egg-info/SOURCES.txt
+-rw-r--r--   0 Shogo      (501) staff       (20)        1 2023-05-07 02:12:44.000000 bumbo_shogo-0.0.2/bumbo_shogo.egg-info/dependency_links.txt
+-rw-r--r--   0 Shogo      (501) staff       (20)      106 2023-05-07 02:12:44.000000 bumbo_shogo-0.0.2/bumbo_shogo.egg-info/requires.txt
+-rw-r--r--   0 Shogo      (501) staff       (20)        6 2023-05-07 02:12:44.000000 bumbo_shogo-0.0.2/bumbo_shogo.egg-info/top_level.txt
+-rw-r--r--   0 Shogo      (501) staff       (20)       38 2023-05-07 02:12:45.094063 bumbo_shogo-0.0.2/setup.cfg
+-rw-r--r--   0 Shogo      (501) staff       (20)     1792 2023-05-07 02:12:34.000000 bumbo_shogo-0.0.2/setup.py
```

### Comparing `bumbo_shogo-0.0.1/bumbo/api.py` & `bumbo_shogo-0.0.2/bumbo/api.py`

 * *Files identical despite different names*

### Comparing `bumbo_shogo-0.0.1/bumbo/middleware.py` & `bumbo_shogo-0.0.2/bumbo/middleware.py`

 * *Files identical despite different names*

### Comparing `bumbo_shogo-0.0.1/bumbo/response.py` & `bumbo_shogo-0.0.2/bumbo/response.py`

 * *Files identical despite different names*

### Comparing `bumbo_shogo-0.0.1/setup.py` & `bumbo_shogo-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Package meta-data.
 NAME = "bumbo_shogo"
 DESCRIPTION = "Bumbo Python Web Framework built for learning purposes."
 EMAIL = "shougees@gmail.com"
 AUTHOR = "Shogo Okuda"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 # Which packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==2.10.3",
     "parse==1.12.1",
     "requests==2.22.0",
     "requests-wsgi-adapter==0.4.1",
```

