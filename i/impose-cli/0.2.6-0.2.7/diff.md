# Comparing `tmp/impose-cli-0.2.6.tar.gz` & `tmp/impose_cli-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impose-cli-0.2.6.tar", last modified: Sun May  7 15:33:53 2023, max compression
+gzip compressed data, was "impose_cli-0.2.7.tar", last modified: Sun May  7 15:49:01 2023, max compression
```

## Comparing `impose-cli-0.2.6.tar` & `impose_cli-0.2.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 samuelchai   (501) staff       (20)        0 2023-05-07 15:33:53.668153 impose-cli-0.2.6/
--rw-r--r--   0 samuelchai   (501) staff       (20)      201 2023-05-07 15:33:53.668056 impose-cli-0.2.6/PKG-INFO
-drwxr-xr-x   0 samuelchai   (501) staff       (20)        0 2023-05-07 15:33:53.667884 impose-cli-0.2.6/impose_cli.egg-info/
--rw-r--r--   0 samuelchai   (501) staff       (20)      201 2023-05-07 15:33:53.000000 impose-cli-0.2.6/impose_cli.egg-info/PKG-INFO
--rw-r--r--   0 samuelchai   (501) staff       (20)      177 2023-05-07 15:33:53.000000 impose-cli-0.2.6/impose_cli.egg-info/SOURCES.txt
--rw-r--r--   0 samuelchai   (501) staff       (20)        1 2023-05-07 15:33:53.000000 impose-cli-0.2.6/impose_cli.egg-info/dependency_links.txt
--rw-r--r--   0 samuelchai   (501) staff       (20)        6 2023-05-07 15:33:53.000000 impose-cli-0.2.6/impose_cli.egg-info/requires.txt
--rw-r--r--   0 samuelchai   (501) staff       (20)        1 2023-05-07 15:33:53.000000 impose-cli-0.2.6/impose_cli.egg-info/top_level.txt
--rw-r--r--   0 samuelchai   (501) staff       (20)       38 2023-05-07 15:33:53.668186 impose-cli-0.2.6/setup.cfg
--rw-r--r--   0 samuelchai   (501) staff       (20)      327 2023-05-07 15:33:51.000000 impose-cli-0.2.6/setup.py
+drwxr-xr-x   0 samuelchai   (501) staff       (20)        0 2023-05-07 15:49:01.504074 impose_cli-0.2.7/
+-rw-r--r--   0 samuelchai   (501) staff       (20)      201 2023-05-07 15:49:01.503977 impose_cli-0.2.7/PKG-INFO
+drwxr-xr-x   0 samuelchai   (501) staff       (20)        0 2023-05-07 15:49:01.503818 impose_cli-0.2.7/impose_cli.egg-info/
+-rw-r--r--   0 samuelchai   (501) staff       (20)      201 2023-05-07 15:49:01.000000 impose_cli-0.2.7/impose_cli.egg-info/PKG-INFO
+-rw-r--r--   0 samuelchai   (501) staff       (20)      177 2023-05-07 15:49:01.000000 impose_cli-0.2.7/impose_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 samuelchai   (501) staff       (20)        1 2023-05-07 15:49:01.000000 impose_cli-0.2.7/impose_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 samuelchai   (501) staff       (20)        6 2023-05-07 15:49:01.000000 impose_cli-0.2.7/impose_cli.egg-info/requires.txt
+-rw-r--r--   0 samuelchai   (501) staff       (20)        1 2023-05-07 15:49:01.000000 impose_cli-0.2.7/impose_cli.egg-info/top_level.txt
+-rw-r--r--   0 samuelchai   (501) staff       (20)       38 2023-05-07 15:49:01.504107 impose_cli-0.2.7/setup.cfg
+-rw-r--r--   0 samuelchai   (501) staff       (20)      327 2023-05-07 15:44:36.000000 impose_cli-0.2.7/setup.py
```

