# Comparing `tmp/silobuster-0.1.7.tar.gz` & `tmp/silobuster-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silobuster-0.1.7.tar", last modified: Sun May  7 05:09:33 2023, max compression
+gzip compressed data, was "silobuster-0.1.8.tar", last modified: Sun May  7 05:27:57 2023, max compression
```

## Comparing `silobuster-0.1.7.tar` & `silobuster-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:09:33.814879 silobuster-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 05:09:33.814879 silobuster-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-07 05:09:27.000000 silobuster-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 05:09:33.814879 silobuster-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-07 05:09:28.000000 silobuster-0.1.7/setup_pypi_package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:09:33.814879 silobuster-0.1.7/silobuster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 05:09:28.000000 silobuster-0.1.7/silobuster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:09:33.814879 silobuster-0.1.7/silobuster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 05:09:33.000000 silobuster-0.1.7/silobuster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-07 05:09:33.000000 silobuster-0.1.7/silobuster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 05:09:33.000000 silobuster-0.1.7/silobuster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-07 05:09:33.000000 silobuster-0.1.7/silobuster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 05:09:33.000000 silobuster-0.1.7/silobuster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:27:57.038255 silobuster-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 05:27:57.038255 silobuster-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-07 05:27:50.000000 silobuster-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 05:27:57.038255 silobuster-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-07 05:27:52.000000 silobuster-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:27:57.034255 silobuster-0.1.8/silobuster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 05:27:52.000000 silobuster-0.1.8/silobuster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:27:57.038255 silobuster-0.1.8/silobuster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 05:27:57.000000 silobuster-0.1.8/silobuster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-07 05:27:57.000000 silobuster-0.1.8/silobuster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 05:27:57.000000 silobuster-0.1.8/silobuster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-07 05:27:57.000000 silobuster-0.1.8/silobuster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 05:27:57.000000 silobuster-0.1.8/silobuster.egg-info/top_level.txt
```

### Comparing `silobuster-0.1.7/README.md` & `silobuster-0.1.8/README.md`

 * *Files identical despite different names*

