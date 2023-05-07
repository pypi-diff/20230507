# Comparing `tmp/asciicards-0.0.3.tar.gz` & `tmp/asciicards-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asciicards-0.0.3.tar", last modified: Sun May  7 00:05:45 2023, max compression
+gzip compressed data, was "asciicards-0.0.4.tar", last modified: Sun May  7 00:18:49 2023, max compression
```

## Comparing `asciicards-0.0.3.tar` & `asciicards-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 00:05:45.909740 asciicards-0.0.3/
--rw-rw-rw-   0        0        0    35149 2023-05-06 18:11:30.000000 asciicards-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      495 2023-05-07 00:05:45.908738 asciicards-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-05-06 18:11:30.000000 asciicards-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 00:05:45.907743 asciicards-0.0.3/asciicards.egg-info/
--rw-rw-rw-   0        0        0      495 2023-05-07 00:05:45.000000 asciicards-0.0.3/asciicards.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-05-07 00:05:45.000000 asciicards-0.0.3/asciicards.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 00:05:45.000000 asciicards-0.0.3/asciicards.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 00:05:45.000000 asciicards-0.0.3/asciicards.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       92 2023-05-06 18:24:32.000000 asciicards-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 00:05:45.909740 asciicards-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      489 2023-05-07 00:04:54.000000 asciicards-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 00:18:49.415159 asciicards-0.0.4/
+-rw-rw-rw-   0        0        0    35149 2023-05-06 18:11:30.000000 asciicards-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      495 2023-05-07 00:18:49.415159 asciicards-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-05-06 18:11:30.000000 asciicards-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 00:18:49.401146 asciicards-0.0.4/asciicards/
+-rw-rw-rw-   0        0        0     1483 2023-05-06 21:01:27.000000 asciicards-0.0.4/asciicards/asciicards.py
+drwxrwxrwx   0        0        0        0 2023-05-07 00:18:49.413157 asciicards-0.0.4/asciicards.egg-info/
+-rw-rw-rw-   0        0        0      495 2023-05-07 00:18:49.000000 asciicards-0.0.4/asciicards.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-05-07 00:18:49.000000 asciicards-0.0.4/asciicards.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 00:18:49.000000 asciicards-0.0.4/asciicards.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-07 00:18:49.000000 asciicards-0.0.4/asciicards.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       92 2023-05-06 18:24:32.000000 asciicards-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 00:18:49.416160 asciicards-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      520 2023-05-07 00:18:23.000000 asciicards-0.0.4/setup.py
```

### Comparing `asciicards-0.0.3/LICENSE` & `asciicards-0.0.4/LICENSE`

 * *Files identical despite different names*

