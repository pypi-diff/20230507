# Comparing `tmp/impose-cli-0.2.4.tar.gz` & `tmp/impose-cli-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impose-cli-0.2.4.tar", last modified: Sun May  7 15:23:28 2023, max compression
+gzip compressed data, was "impose-cli-0.2.5.tar", last modified: Sun May  7 15:26:20 2023, max compression
```

## Comparing `impose-cli-0.2.4.tar` & `impose-cli-0.2.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 samuelchai   (501) staff       (20)        0 2023-05-07 15:23:28.991737 impose-cli-0.2.4/
--rw-r--r--   0 samuelchai   (501) staff       (20)      201 2023-05-07 15:23:28.991635 impose-cli-0.2.4/PKG-INFO
-drwxr-xr-x   0 samuelchai   (501) staff       (20)        0 2023-05-07 15:23:28.991459 impose-cli-0.2.4/impose_cli.egg-info/
--rw-r--r--   0 samuelchai   (501) staff       (20)      201 2023-05-07 15:23:28.000000 impose-cli-0.2.4/impose_cli.egg-info/PKG-INFO
--rw-r--r--   0 samuelchai   (501) staff       (20)      177 2023-05-07 15:23:28.000000 impose-cli-0.2.4/impose_cli.egg-info/SOURCES.txt
--rw-r--r--   0 samuelchai   (501) staff       (20)        1 2023-05-07 15:23:28.000000 impose-cli-0.2.4/impose_cli.egg-info/dependency_links.txt
--rw-r--r--   0 samuelchai   (501) staff       (20)        6 2023-05-07 15:23:28.000000 impose-cli-0.2.4/impose_cli.egg-info/requires.txt
--rw-r--r--   0 samuelchai   (501) staff       (20)        1 2023-05-07 15:23:28.000000 impose-cli-0.2.4/impose_cli.egg-info/top_level.txt
--rw-r--r--   0 samuelchai   (501) staff       (20)       38 2023-05-07 15:23:28.991783 impose-cli-0.2.4/setup.cfg
--rw-r--r--   0 samuelchai   (501) staff       (20)      327 2023-05-07 15:23:25.000000 impose-cli-0.2.4/setup.py
+drwxr-xr-x   0 samuelchai   (501) staff       (20)        0 2023-05-07 15:26:20.725919 impose-cli-0.2.5/
+-rw-r--r--   0 samuelchai   (501) staff       (20)      201 2023-05-07 15:26:20.725822 impose-cli-0.2.5/PKG-INFO
+drwxr-xr-x   0 samuelchai   (501) staff       (20)        0 2023-05-07 15:26:20.725669 impose-cli-0.2.5/impose_cli.egg-info/
+-rw-r--r--   0 samuelchai   (501) staff       (20)      201 2023-05-07 15:26:20.000000 impose-cli-0.2.5/impose_cli.egg-info/PKG-INFO
+-rw-r--r--   0 samuelchai   (501) staff       (20)      177 2023-05-07 15:26:20.000000 impose-cli-0.2.5/impose_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 samuelchai   (501) staff       (20)        1 2023-05-07 15:26:20.000000 impose-cli-0.2.5/impose_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 samuelchai   (501) staff       (20)        6 2023-05-07 15:26:20.000000 impose-cli-0.2.5/impose_cli.egg-info/requires.txt
+-rw-r--r--   0 samuelchai   (501) staff       (20)        1 2023-05-07 15:26:20.000000 impose-cli-0.2.5/impose_cli.egg-info/top_level.txt
+-rw-r--r--   0 samuelchai   (501) staff       (20)       38 2023-05-07 15:26:20.725952 impose-cli-0.2.5/setup.cfg
+-rw-r--r--   0 samuelchai   (501) staff       (20)      327 2023-05-07 15:26:12.000000 impose-cli-0.2.5/setup.py
```

