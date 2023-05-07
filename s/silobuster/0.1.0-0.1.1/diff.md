# Comparing `tmp/silobuster-0.1.0.tar.gz` & `tmp/silobuster-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silobuster-0.1.0.tar", last modified: Fri Mar 31 21:36:14 2023, max compression
+gzip compressed data, was "silobuster-0.1.1.tar", last modified: Sun May  7 04:07:32 2023, max compression
```

## Comparing `silobuster-0.1.0.tar` & `silobuster-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:36:14.478387 silobuster-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-31 21:36:14.478387 silobuster-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-03-31 21:36:03.000000 silobuster-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 21:36:14.478387 silobuster-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-31 21:36:05.000000 silobuster-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:36:14.478387 silobuster-0.1.0/silobuster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-31 21:36:14.000000 silobuster-0.1.0/silobuster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-31 21:36:14.000000 silobuster-0.1.0/silobuster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 21:36:14.000000 silobuster-0.1.0/silobuster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-31 21:36:14.000000 silobuster-0.1.0/silobuster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-31 21:36:14.000000 silobuster-0.1.0/silobuster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:07:32.840130 silobuster-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 04:07:32.840130 silobuster-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-07 04:07:22.000000 silobuster-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 04:07:32.840130 silobuster-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-07 04:07:24.000000 silobuster-0.1.1/setup_pypi_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:07:32.840130 silobuster-0.1.1/silobuster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 04:07:32.000000 silobuster-0.1.1/silobuster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-07 04:07:32.000000 silobuster-0.1.1/silobuster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 04:07:32.000000 silobuster-0.1.1/silobuster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-07 04:07:32.000000 silobuster-0.1.1/silobuster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 04:07:32.000000 silobuster-0.1.1/silobuster.egg-info/top_level.txt
```

### Comparing `silobuster-0.1.0/README.md` & `silobuster-0.1.1/README.md`

 * *Files identical despite different names*

