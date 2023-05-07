# Comparing `tmp/pointclass-1.2.tar.gz` & `tmp/pointclass-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointclass-1.2.tar", last modified: Sat May  6 16:29:22 2023, max compression
+gzip compressed data, was "pointclass-1.4.tar", last modified: Sat May  6 17:57:48 2023, max compression
```

## Comparing `pointclass-1.2.tar` & `pointclass-1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 16:29:22.370464 pointclass-1.2/
--rw-rw-rw-   0        0        0      177 2023-05-06 16:29:22.370464 pointclass-1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-25 10:31:30.000000 pointclass-1.2/licence.txt.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 16:29:22.347040 pointclass-1.2/pointclass/
--rw-rw-rw-   0        0        0     1045 2023-05-06 16:29:07.000000 pointclass-1.2/pointclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 16:29:22.368515 pointclass-1.2/pointclass.egg-info/
--rw-rw-rw-   0        0        0      177 2023-05-06 16:29:22.000000 pointclass-1.2/pointclass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-05-06 16:29:22.000000 pointclass-1.2/pointclass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 16:29:22.000000 pointclass-1.2/pointclass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-06 16:29:22.000000 pointclass-1.2/pointclass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 16:29:22.370464 pointclass-1.2/setup.cfg
--rw-rw-rw-   0        0        0      247 2023-05-06 16:27:31.000000 pointclass-1.2/setup1.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:57:48.106597 pointclass-1.4/
+-rw-rw-rw-   0        0        0      177 2023-05-06 17:57:48.104289 pointclass-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-25 10:31:30.000000 pointclass-1.4/licence.txt.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 17:57:48.066909 pointclass-1.4/pointclass/
+-rw-rw-rw-   0        0        0     1905 2023-05-06 17:57:35.000000 pointclass-1.4/pointclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:57:48.102295 pointclass-1.4/pointclass.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-05-06 17:57:47.000000 pointclass-1.4/pointclass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-05-06 17:57:47.000000 pointclass-1.4/pointclass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 17:57:47.000000 pointclass-1.4/pointclass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 17:57:47.000000 pointclass-1.4/pointclass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 17:57:48.107489 pointclass-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      247 2023-05-06 17:57:21.000000 pointclass-1.4/setup1.py
```

