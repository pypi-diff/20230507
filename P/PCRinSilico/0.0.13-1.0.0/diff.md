# Comparing `tmp/PCRinSilico-0.0.13.tar.gz` & `tmp/PCRinSilico-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PCRinSilico-0.0.13.tar", last modified: Mon May  1 20:55:50 2023, max compression
+gzip compressed data, was "PCRinSilico-1.0.0.tar", last modified: Sun May  7 07:00:42 2023, max compression
```

## Comparing `PCRinSilico-0.0.13.tar` & `PCRinSilico-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-01 20:55:50.164571 PCRinSilico-0.0.13/
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-01 20:55:50.164209 PCRinSilico-0.0.13/PCRinSilico.egg-info/
--rw-r--r--   0 semiquant   (502) staff       (20)     2812 2023-05-01 20:55:49.000000 PCRinSilico-0.0.13/PCRinSilico.egg-info/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)      209 2023-05-01 20:55:50.000000 PCRinSilico-0.0.13/PCRinSilico.egg-info/SOURCES.txt
--rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-01 20:55:49.000000 PCRinSilico-0.0.13/PCRinSilico.egg-info/dependency_links.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       17 2023-05-01 20:55:50.000000 PCRinSilico-0.0.13/PCRinSilico.egg-info/requires.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       14 2023-05-01 20:55:50.000000 PCRinSilico-0.0.13/PCRinSilico.egg-info/top_level.txt
--rw-r--r--   0 semiquant   (502) staff       (20)     2812 2023-05-01 20:55:50.164407 PCRinSilico-0.0.13/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)     2365 2023-05-01 16:19:04.000000 PCRinSilico-0.0.13/README.md
--rw-rw-r--   0 semiquant   (502) staff       (20)     6382 2023-05-01 19:58:12.000000 PCRinSilico-0.0.13/in_silico_pcr.py
--rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-01 20:55:50.164627 PCRinSilico-0.0.13/setup.cfg
--rw-r--r--   0 semiquant   (502) staff       (20)     1347 2023-05-01 20:55:36.000000 PCRinSilico-0.0.13/setup.py
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 07:00:42.187438 PCRinSilico-1.0.0/
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 07:00:42.186363 PCRinSilico-1.0.0/PCRinSilico/
+-rw-r--r--   0 semiquant   (502) staff       (20)    10153 2023-05-05 22:30:45.000000 PCRinSilico-1.0.0/PCRinSilico/inSilicoPCR.py
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 07:00:42.187100 PCRinSilico-1.0.0/PCRinSilico.egg-info/
+-rw-r--r--   0 semiquant   (502) staff       (20)     3898 2023-05-07 07:00:41.000000 PCRinSilico-1.0.0/PCRinSilico.egg-info/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)      257 2023-05-07 07:00:42.000000 PCRinSilico-1.0.0/PCRinSilico.egg-info/SOURCES.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-07 07:00:41.000000 PCRinSilico-1.0.0/PCRinSilico.egg-info/dependency_links.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       61 2023-05-07 07:00:41.000000 PCRinSilico-1.0.0/PCRinSilico.egg-info/entry_points.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       17 2023-05-07 07:00:42.000000 PCRinSilico-1.0.0/PCRinSilico.egg-info/requires.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       12 2023-05-07 07:00:42.000000 PCRinSilico-1.0.0/PCRinSilico.egg-info/top_level.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)     3898 2023-05-07 07:00:42.187288 PCRinSilico-1.0.0/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)     3452 2023-05-07 06:59:51.000000 PCRinSilico-1.0.0/README.md
+-rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-07 07:00:42.187488 PCRinSilico-1.0.0/setup.cfg
+-rw-r--r--   0 semiquant   (502) staff       (20)     1955 2023-05-07 06:59:44.000000 PCRinSilico-1.0.0/setup.py
```

