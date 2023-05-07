# Comparing `tmp/djangorestframework-verbose-errors-0.0.1.tar.gz` & `tmp/djangorestframework-verbose-errors-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangorestframework-verbose-errors-0.0.1.tar", last modified: Sun May  7 13:52:45 2023, max compression
+gzip compressed data, was "dist/djangorestframework-verbose-errors-0.0.2.tar", last modified: Sun May  7 14:03:59 2023, max compression
```

## Comparing `djangorestframework-verbose-errors-0.0.1.tar` & `djangorestframework-verbose-errors-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mikhaileremeev   (501) staff       (20)        0 2023-05-07 13:52:45.000000 djangorestframework-verbose-errors-0.0.1/
--rw-r--r--   0 mikhaileremeev   (501) staff       (20)      319 2023-05-07 13:52:45.000000 djangorestframework-verbose-errors-0.0.1/PKG-INFO
-drwxr-xr-x   0 mikhaileremeev   (501) staff       (20)        0 2023-05-07 13:52:45.000000 djangorestframework-verbose-errors-0.0.1/djangorestframework_verbose_errors.egg-info/
--rw-r--r--   0 mikhaileremeev   (501) staff       (20)      319 2023-05-07 13:52:45.000000 djangorestframework-verbose-errors-0.0.1/djangorestframework_verbose_errors.egg-info/PKG-INFO
--rw-r--r--   0 mikhaileremeev   (501) staff       (20)      331 2023-05-07 13:52:45.000000 djangorestframework-verbose-errors-0.0.1/djangorestframework_verbose_errors.egg-info/SOURCES.txt
--rw-r--r--   0 mikhaileremeev   (501) staff       (20)       30 2023-05-07 13:52:45.000000 djangorestframework-verbose-errors-0.0.1/djangorestframework_verbose_errors.egg-info/top_level.txt
--rw-r--r--   0 mikhaileremeev   (501) staff       (20)        1 2023-05-07 13:52:45.000000 djangorestframework-verbose-errors-0.0.1/djangorestframework_verbose_errors.egg-info/dependency_links.txt
--rw-r--r--   0 mikhaileremeev   (501) staff       (20)      138 2023-05-07 13:46:38.000000 djangorestframework-verbose-errors-0.0.1/README.md
-drwxr-xr-x   0 mikhaileremeev   (501) staff       (20)        0 2023-05-07 13:52:45.000000 djangorestframework-verbose-errors-0.0.1/rest_framework_verbose_errors/
--rw-r--r--   0 mikhaileremeev   (501) staff       (20)       80 2023-05-04 20:48:20.000000 djangorestframework-verbose-errors-0.0.1/rest_framework_verbose_errors/__init__.py
--rw-r--r--   0 mikhaileremeev   (501) staff       (20)      801 2023-05-07 13:20:45.000000 djangorestframework-verbose-errors-0.0.1/rest_framework_verbose_errors/views.py
--rwxr-xr-x   0 mikhaileremeev   (501) staff       (20)      467 2023-05-07 13:44:47.000000 djangorestframework-verbose-errors-0.0.1/setup.py
--rw-r--r--   0 mikhaileremeev   (501) staff       (20)       38 2023-05-07 13:52:45.000000 djangorestframework-verbose-errors-0.0.1/setup.cfg
+drwxr-xr-x   0 mikhaileremeev   (501) staff       (20)        0 2023-05-07 14:03:59.000000 djangorestframework-verbose-errors-0.0.2/
+-rw-r--r--   0 mikhaileremeev   (501) staff       (20)      562 2023-05-07 14:03:59.000000 djangorestframework-verbose-errors-0.0.2/PKG-INFO
+drwxr-xr-x   0 mikhaileremeev   (501) staff       (20)        0 2023-05-07 14:03:59.000000 djangorestframework-verbose-errors-0.0.2/djangorestframework_verbose_errors.egg-info/
+-rw-r--r--   0 mikhaileremeev   (501) staff       (20)      562 2023-05-07 14:03:59.000000 djangorestframework-verbose-errors-0.0.2/djangorestframework_verbose_errors.egg-info/PKG-INFO
+-rw-r--r--   0 mikhaileremeev   (501) staff       (20)      331 2023-05-07 14:03:59.000000 djangorestframework-verbose-errors-0.0.2/djangorestframework_verbose_errors.egg-info/SOURCES.txt
+-rw-r--r--   0 mikhaileremeev   (501) staff       (20)       30 2023-05-07 14:03:59.000000 djangorestframework-verbose-errors-0.0.2/djangorestframework_verbose_errors.egg-info/top_level.txt
+-rw-r--r--   0 mikhaileremeev   (501) staff       (20)        1 2023-05-07 14:03:59.000000 djangorestframework-verbose-errors-0.0.2/djangorestframework_verbose_errors.egg-info/dependency_links.txt
+-rw-r--r--   0 mikhaileremeev   (501) staff       (20)      138 2023-05-07 13:46:38.000000 djangorestframework-verbose-errors-0.0.2/README.md
+drwxr-xr-x   0 mikhaileremeev   (501) staff       (20)        0 2023-05-07 14:03:59.000000 djangorestframework-verbose-errors-0.0.2/rest_framework_verbose_errors/
+-rw-r--r--   0 mikhaileremeev   (501) staff       (20)       80 2023-05-07 14:02:39.000000 djangorestframework-verbose-errors-0.0.2/rest_framework_verbose_errors/__init__.py
+-rw-r--r--   0 mikhaileremeev   (501) staff       (20)      801 2023-05-07 13:20:45.000000 djangorestframework-verbose-errors-0.0.2/rest_framework_verbose_errors/views.py
+-rwxr-xr-x   0 mikhaileremeev   (501) staff       (20)      565 2023-05-07 14:02:27.000000 djangorestframework-verbose-errors-0.0.2/setup.py
+-rw-r--r--   0 mikhaileremeev   (501) staff       (20)       38 2023-05-07 14:03:59.000000 djangorestframework-verbose-errors-0.0.2/setup.cfg
```

### Comparing `djangorestframework-verbose-errors-0.0.1/rest_framework_verbose_errors/views.py` & `djangorestframework-verbose-errors-0.0.2/rest_framework_verbose_errors/views.py`

 * *Files identical despite different names*

