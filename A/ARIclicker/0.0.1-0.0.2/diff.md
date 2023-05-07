# Comparing `tmp/ARIclicker-0.0.1.tar.gz` & `tmp/ARIclicker-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ARIclicker-0.0.1.tar", last modified: Wed May  3 11:09:06 2023, max compression
+gzip compressed data, was "ARIclicker-0.0.2.tar", last modified: Sun May  7 03:51:12 2023, max compression
```

## Comparing `ARIclicker-0.0.1.tar` & `ARIclicker-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 11:09:06.512271 ARIclicker-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-03 11:09:06.461258 ARIclicker-0.0.1/ARIclicker/
--rw-rw-rw-   0        0        0     1725 2023-05-03 11:07:38.000000 ARIclicker-0.0.1/ARIclicker/__init__.py
--rw-rw-rw-   0        0        0        2 2023-05-03 11:07:38.000000 ARIclicker-0.0.1/ARIclicker/file.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:09:06.500236 ARIclicker-0.0.1/ARIclicker.egg-info/
--rw-rw-rw-   0        0        0      360 2023-05-03 11:09:06.000000 ARIclicker-0.0.1/ARIclicker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-05-03 11:09:06.000000 ARIclicker-0.0.1/ARIclicker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:09:06.000000 ARIclicker-0.0.1/ARIclicker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 11:09:06.000000 ARIclicker-0.0.1/ARIclicker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-03 11:09:06.000000 ARIclicker-0.0.1/ARIclicker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      360 2023-05-03 11:09:06.510241 ARIclicker-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1093 2023-05-03 01:46:26.000000 ARIclicker-0.0.1/license.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 11:09:06.512271 ARIclicker-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      533 2023-05-03 10:45:14.000000 ARIclicker-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 03:51:12.813392 ARIclicker-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-05-07 03:51:11.816975 ARIclicker-0.0.2/ARIclicker/
+-rw-rw-rw-   0        0        0     1725 2023-05-03 11:07:38.000000 ARIclicker-0.0.2/ARIclicker/__init__.py
+-rw-rw-rw-   0        0        0        2 2023-05-03 11:07:38.000000 ARIclicker-0.0.2/ARIclicker/file.py
+drwxrwxrwx   0        0        0        0 2023-05-07 03:51:12.686466 ARIclicker-0.0.2/ARIclicker.egg-info/
+-rw-rw-rw-   0        0        0     1198 2023-05-07 03:51:10.000000 ARIclicker-0.0.2/ARIclicker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-07 03:51:10.000000 ARIclicker-0.0.2/ARIclicker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 03:51:10.000000 ARIclicker-0.0.2/ARIclicker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-07 03:51:10.000000 ARIclicker-0.0.2/ARIclicker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-07 03:51:10.000000 ARIclicker-0.0.2/ARIclicker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1198 2023-05-07 03:51:12.783410 ARIclicker-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      845 2023-05-07 03:40:28.000000 ARIclicker-0.0.2/README.md
+-rw-rw-rw-   0        0        0     1093 2023-05-03 01:46:26.000000 ARIclicker-0.0.2/license.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 03:51:12.857367 ARIclicker-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-05-07 03:50:10.000000 ARIclicker-0.0.2/setup.py
```

### Comparing `ARIclicker-0.0.1/ARIclicker/__init__.py` & `ARIclicker-0.0.2/ARIclicker/__init__.py`

 * *Files identical despite different names*

### Comparing `ARIclicker-0.0.1/license.txt` & `ARIclicker-0.0.2/license.txt`

 * *Files identical despite different names*

