# Comparing `tmp/impose-cli-0.2.1.tar.gz` & `tmp/impose-cli-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impose-cli-0.2.1.tar", last modified: Sun May  7 15:04:49 2023, max compression
+gzip compressed data, was "impose-cli-0.2.2.tar", last modified: Sun May  7 15:11:56 2023, max compression
```

## Comparing `impose-cli-0.2.1.tar` & `impose-cli-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 samuelchai   (501) staff       (20)        0 2023-05-07 15:04:49.481529 impose-cli-0.2.1/
--rw-r--r--   0 samuelchai   (501) staff       (20)      201 2023-05-07 15:04:49.481423 impose-cli-0.2.1/PKG-INFO
--rw-r--r--   0 samuelchai   (501) staff       (20)      379 2023-05-07 14:14:59.000000 impose-cli-0.2.1/README.md
-drwxr-xr-x   0 samuelchai   (501) staff       (20)        0 2023-05-07 15:04:49.481255 impose-cli-0.2.1/impose_cli.egg-info/
--rw-r--r--   0 samuelchai   (501) staff       (20)      201 2023-05-07 15:04:49.000000 impose-cli-0.2.1/impose_cli.egg-info/PKG-INFO
--rw-r--r--   0 samuelchai   (501) staff       (20)      187 2023-05-07 15:04:49.000000 impose-cli-0.2.1/impose_cli.egg-info/SOURCES.txt
--rw-r--r--   0 samuelchai   (501) staff       (20)        1 2023-05-07 15:04:49.000000 impose-cli-0.2.1/impose_cli.egg-info/dependency_links.txt
--rw-r--r--   0 samuelchai   (501) staff       (20)        6 2023-05-07 15:04:49.000000 impose-cli-0.2.1/impose_cli.egg-info/requires.txt
--rw-r--r--   0 samuelchai   (501) staff       (20)        1 2023-05-07 15:04:49.000000 impose-cli-0.2.1/impose_cli.egg-info/top_level.txt
--rw-r--r--   0 samuelchai   (501) staff       (20)       38 2023-05-07 15:04:49.481564 impose-cli-0.2.1/setup.cfg
--rw-r--r--   0 samuelchai   (501) staff       (20)      327 2023-05-07 15:04:17.000000 impose-cli-0.2.1/setup.py
+drwxr-xr-x   0 samuelchai   (501) staff       (20)        0 2023-05-07 15:11:56.534235 impose-cli-0.2.2/
+-rw-r--r--   0 samuelchai   (501) staff       (20)      201 2023-05-07 15:11:56.534144 impose-cli-0.2.2/PKG-INFO
+-rw-r--r--   0 samuelchai   (501) staff       (20)      379 2023-05-07 14:14:59.000000 impose-cli-0.2.2/README.md
+drwxr-xr-x   0 samuelchai   (501) staff       (20)        0 2023-05-07 15:11:56.533980 impose-cli-0.2.2/impose_cli.egg-info/
+-rw-r--r--   0 samuelchai   (501) staff       (20)      201 2023-05-07 15:11:56.000000 impose-cli-0.2.2/impose_cli.egg-info/PKG-INFO
+-rw-r--r--   0 samuelchai   (501) staff       (20)      187 2023-05-07 15:11:56.000000 impose-cli-0.2.2/impose_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 samuelchai   (501) staff       (20)        1 2023-05-07 15:11:56.000000 impose-cli-0.2.2/impose_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 samuelchai   (501) staff       (20)        6 2023-05-07 15:11:56.000000 impose-cli-0.2.2/impose_cli.egg-info/requires.txt
+-rw-r--r--   0 samuelchai   (501) staff       (20)        1 2023-05-07 15:11:56.000000 impose-cli-0.2.2/impose_cli.egg-info/top_level.txt
+-rw-r--r--   0 samuelchai   (501) staff       (20)       38 2023-05-07 15:11:56.534268 impose-cli-0.2.2/setup.cfg
+-rw-r--r--   0 samuelchai   (501) staff       (20)      327 2023-05-07 15:11:49.000000 impose-cli-0.2.2/setup.py
```

