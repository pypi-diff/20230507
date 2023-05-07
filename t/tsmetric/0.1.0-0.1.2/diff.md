# Comparing `tmp/tsmetric-0.1.0.tar.gz` & `tmp/tsmetric-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsmetric-0.1.0.tar", max compression
+gzip compressed data, was "tsmetric-0.1.2.tar", max compression
```

## Comparing `tsmetric-0.1.0.tar` & `tsmetric-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-07 15:35:11.770478 tsmetric-0.1.0/README.md
--rw-r--r--   0        0        0      283 2023-05-05 20:46:51.976687 tsmetric-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       61 2023-05-05 20:34:15.889910 tsmetric-0.1.0/tsmetric/__init__.py
--rw-r--r--   0        0        0       59 2023-05-05 20:33:38.677561 tsmetric-0.1.0/tsmetric/length.py
--rw-r--r--   0        0        0       59 2023-05-05 20:33:38.681562 tsmetric-0.1.0/tsmetric/temp.py
--rw-r--r--   0        0        0      341 1970-01-01 00:00:00.000000 tsmetric-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-07 15:35:11.770478 tsmetric-0.1.2/README.md
+-rw-r--r--   0        0        0      300 2023-05-07 16:10:10.719249 tsmetric-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-05-07 16:08:18.242049 tsmetric-0.1.2/tsmetric/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-07 16:05:39.560349 tsmetric-0.1.2/tsmetric/length.py
+-rw-r--r--   0        0        0       59 2023-05-05 20:33:38.681562 tsmetric-0.1.2/tsmetric/temp.py
+-rw-r--r--   0        0        0      380 1970-01-01 00:00:00.000000 tsmetric-0.1.2/PKG-INFO
```

