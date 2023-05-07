# Comparing `tmp/searchbook-1.0.tar.gz` & `tmp/searchbook-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchbook-1.0.tar", last modified: Sun May  7 16:56:19 2023, max compression
+gzip compressed data, was "searchbook-1.0.1.tar", last modified: Sun May  7 19:44:38 2023, max compression
```

## Comparing `searchbook-1.0.tar` & `searchbook-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 16:56:19.549656 searchbook-1.0/
--rw-rw-rw-   0        0        0      260 2023-05-07 16:56:19.548654 searchbook-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-07 16:56:19.546654 searchbook-1.0/searchbook.egg-info/
--rw-rw-rw-   0        0        0      260 2023-05-07 16:56:19.000000 searchbook-1.0/searchbook.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-05-07 16:56:19.000000 searchbook-1.0/searchbook.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 16:56:19.000000 searchbook-1.0/searchbook.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-07 16:56:19.000000 searchbook-1.0/searchbook.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 16:56:19.000000 searchbook-1.0/searchbook.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 16:56:19.549656 searchbook-1.0/setup.cfg
--rw-rw-rw-   0        0        0      795 2023-05-07 16:55:00.000000 searchbook-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 19:44:38.268876 searchbook-1.0.1/
+-rw-rw-rw-   0        0        0      262 2023-05-07 19:44:38.267876 searchbook-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-07 19:44:38.265875 searchbook-1.0.1/searchbook.egg-info/
+-rw-rw-rw-   0        0        0      262 2023-05-07 19:44:38.000000 searchbook-1.0.1/searchbook.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-05-07 19:44:38.000000 searchbook-1.0.1/searchbook.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 19:44:38.000000 searchbook-1.0.1/searchbook.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-07 19:44:38.000000 searchbook-1.0.1/searchbook.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 19:44:38.000000 searchbook-1.0.1/searchbook.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 19:44:38.268876 searchbook-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      691 2023-05-07 19:43:19.000000 searchbook-1.0.1/setup.py
```

