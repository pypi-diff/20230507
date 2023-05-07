# Comparing `tmp/sry-0.0.1.tar.gz` & `tmp/sry-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sry-0.0.1.tar", last modified: Fri May  5 11:41:37 2023, max compression
+gzip compressed data, was "sry-0.0.2.tar", last modified: Sun May  7 02:32:58 2023, max compression
```

## Comparing `sry-0.0.1.tar` & `sry-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 11:41:37.517508 sry-0.0.1/
--rw-rw-rw-   0        0        0       70 2023-05-05 11:41:37.516508 sry-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-05 11:41:37.517508 sry-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      204 2023-05-05 11:37:10.000000 sry-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 11:41:37.512507 sry-0.0.1/sry.egg-info/
--rw-rw-rw-   0        0        0       70 2023-05-05 11:41:37.000000 sry-0.0.1/sry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      123 2023-05-05 11:41:37.000000 sry-0.0.1/sry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 11:41:37.000000 sry-0.0.1/sry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 11:41:37.000000 sry-0.0.1/sry.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1895 2023-05-05 11:31:32.000000 sry-0.0.1/sry.py
+drwxrwxrwx   0        0        0        0 2023-05-07 02:32:58.446681 sry-0.0.2/
+-rw-rw-rw-   0        0        0       70 2023-05-07 02:32:58.446681 sry-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-07 02:32:58.446681 sry-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      204 2023-05-07 01:52:14.000000 sry-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 02:32:58.446681 sry-0.0.2/sry.egg-info/
+-rw-rw-rw-   0        0        0       70 2023-05-07 02:32:58.000000 sry-0.0.2/sry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      123 2023-05-07 02:32:58.000000 sry-0.0.2/sry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 02:32:58.000000 sry-0.0.2/sry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 02:32:58.000000 sry-0.0.2/sry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2349 2023-05-07 02:32:16.000000 sry-0.0.2/sry.py
```

