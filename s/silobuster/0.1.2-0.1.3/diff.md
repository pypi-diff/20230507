# Comparing `tmp/silobuster-0.1.2.tar.gz` & `tmp/silobuster-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silobuster-0.1.2.tar", last modified: Sun May  7 04:21:00 2023, max compression
+gzip compressed data, was "silobuster-0.1.3.tar", last modified: Sun May  7 04:30:24 2023, max compression
```

## Comparing `silobuster-0.1.2.tar` & `silobuster-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:21:00.773257 silobuster-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 04:21:00.773257 silobuster-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-07 04:20:52.000000 silobuster-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 04:21:00.773257 silobuster-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-07 04:20:54.000000 silobuster-0.1.2/setup_pypi_package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:21:00.773257 silobuster-0.1.2/silobuster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 04:20:54.000000 silobuster-0.1.2/silobuster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:21:00.773257 silobuster-0.1.2/silobuster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 04:21:00.000000 silobuster-0.1.2/silobuster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-07 04:21:00.000000 silobuster-0.1.2/silobuster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 04:21:00.000000 silobuster-0.1.2/silobuster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-07 04:21:00.000000 silobuster-0.1.2/silobuster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 04:21:00.000000 silobuster-0.1.2/silobuster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:30:24.791459 silobuster-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 04:30:24.791459 silobuster-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-07 04:30:15.000000 silobuster-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 04:30:24.791459 silobuster-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-07 04:30:17.000000 silobuster-0.1.3/setup_pypi_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:30:24.791459 silobuster-0.1.3/silobuster/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 04:30:17.000000 silobuster-0.1.3/silobuster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:30:24.791459 silobuster-0.1.3/silobuster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 04:30:24.000000 silobuster-0.1.3/silobuster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-07 04:30:24.000000 silobuster-0.1.3/silobuster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 04:30:24.000000 silobuster-0.1.3/silobuster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-07 04:30:24.000000 silobuster-0.1.3/silobuster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 04:30:24.000000 silobuster-0.1.3/silobuster.egg-info/top_level.txt
```

### Comparing `silobuster-0.1.2/README.md` & `silobuster-0.1.3/README.md`

 * *Files identical despite different names*

