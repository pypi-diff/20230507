# Comparing `tmp/silobuster-0.1.5.tar.gz` & `tmp/silobuster-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silobuster-0.1.5.tar", last modified: Sun May  7 04:51:54 2023, max compression
+gzip compressed data, was "silobuster-0.1.6.tar", last modified: Sun May  7 04:58:26 2023, max compression
```

## Comparing `silobuster-0.1.5.tar` & `silobuster-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:51:54.481650 silobuster-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 04:51:54.481650 silobuster-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-07 04:51:47.000000 silobuster-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 04:51:54.481650 silobuster-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-07 04:51:49.000000 silobuster-0.1.5/setup_pypi_package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:51:54.481650 silobuster-0.1.5/silobuster/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-07 04:51:49.000000 silobuster-0.1.5/silobuster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:51:54.481650 silobuster-0.1.5/silobuster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 04:51:54.000000 silobuster-0.1.5/silobuster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-07 04:51:54.000000 silobuster-0.1.5/silobuster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 04:51:54.000000 silobuster-0.1.5/silobuster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-07 04:51:54.000000 silobuster-0.1.5/silobuster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 04:51:54.000000 silobuster-0.1.5/silobuster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:58:26.525481 silobuster-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 04:58:26.525481 silobuster-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-07 04:58:19.000000 silobuster-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 04:58:26.525481 silobuster-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-07 04:58:21.000000 silobuster-0.1.6/setup_pypi_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:58:26.521481 silobuster-0.1.6/silobuster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 04:58:21.000000 silobuster-0.1.6/silobuster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:58:26.525481 silobuster-0.1.6/silobuster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 04:58:26.000000 silobuster-0.1.6/silobuster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-07 04:58:26.000000 silobuster-0.1.6/silobuster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 04:58:26.000000 silobuster-0.1.6/silobuster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-07 04:58:26.000000 silobuster-0.1.6/silobuster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 04:58:26.000000 silobuster-0.1.6/silobuster.egg-info/top_level.txt
```

### Comparing `silobuster-0.1.5/README.md` & `silobuster-0.1.6/README.md`

 * *Files identical despite different names*

