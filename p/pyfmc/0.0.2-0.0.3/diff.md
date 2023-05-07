# Comparing `tmp/pyfmc-0.0.2.tar.gz` & `tmp/pyfmc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfmc-0.0.2.tar", last modified: Sun May  7 07:14:16 2023, max compression
+gzip compressed data, was "pyfmc-0.0.3.tar", last modified: Sun May  7 07:25:26 2023, max compression
```

## Comparing `pyfmc-0.0.2.tar` & `pyfmc-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,11 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 07:14:16.456722 pyfmc-0.0.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1139 2023-05-07 07:14:16.456722 pyfmc-0.0.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      520 2023-05-06 14:11:21.000000 pyfmc-0.0.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 07:14:16.456722 pyfmc-0.0.2/pyfmc/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 07:14:16.456722 pyfmc-0.0.2/pyfmc/common/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      395 2023-05-06 14:11:21.000000 pyfmc-0.0.2/pyfmc/common/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2023-05-06 14:11:21.000000 pyfmc-0.0.2/pyfmc/common/historical_data.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 07:14:16.456722 pyfmc-0.0.2/pyfmc/pyfmc.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1139 2023-05-07 07:14:16.000000 pyfmc-0.0.2/pyfmc/pyfmc.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      314 2023-05-07 07:14:16.000000 pyfmc-0.0.2/pyfmc/pyfmc.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-07 07:14:16.000000 pyfmc-0.0.2/pyfmc/pyfmc.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       54 2023-05-07 07:14:16.000000 pyfmc-0.0.2/pyfmc/pyfmc.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       19 2023-05-07 07:14:16.000000 pyfmc-0.0.2/pyfmc/pyfmc.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 07:14:16.456722 pyfmc-0.0.2/pyfmc/simulations/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      266 2023-05-06 14:11:21.000000 pyfmc-0.0.2/pyfmc/simulations/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2700 2023-05-06 14:11:21.000000 pyfmc-0.0.2/pyfmc/simulations/gbm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-07 07:14:16.460722 pyfmc-0.0.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      745 2023-05-07 07:13:46.000000 pyfmc-0.0.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 07:25:26.299798 pyfmc-0.0.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1190 2023-05-07 07:25:26.299798 pyfmc-0.0.3/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      520 2023-05-06 14:11:21.000000 pyfmc-0.0.3/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 07:25:26.299798 pyfmc-0.0.3/pyfmc.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1190 2023-05-07 07:25:26.000000 pyfmc-0.0.3/pyfmc.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-05-07 07:25:26.000000 pyfmc-0.0.3/pyfmc.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-07 07:25:26.000000 pyfmc-0.0.3/pyfmc.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       54 2023-05-07 07:25:26.000000 pyfmc-0.0.3/pyfmc.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-07 07:25:26.000000 pyfmc-0.0.3/pyfmc.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-07 07:25:26.299798 pyfmc-0.0.3/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      709 2023-05-07 07:24:30.000000 pyfmc-0.0.3/setup.py
```

### Comparing `pyfmc-0.0.2/PKG-INFO` & `pyfmc-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pyfmc
-Version: 0.0.2
+Version: 0.0.3
 Summary: Finance Monte-Carlo Simulation using PyTorch
-Home-page: https://github.com/ethanlee928/pyfmc/archive/refs/tags/v0.0.2.tar.gz
+Home-page: https://github.com/ethanlee928/pyfmc
 Author: Ethan Lee
 Author-email: ethan2000.el@gmail.com
 License: UNKNOWN
+Download-URL: https://github.com/ethanlee928/pyfmc/archive/refs/tags/v0.0.3.tar.gz
 Description: # Finance Monte-Carlo Simulation using PyTorch
         
         - An easy-to-use python package to do Monte-Carlo Simulation on stock prices
         - GPU accelerated Monte-Carlo simulation, that could allow simulation more random walkers without a large time penalty
         
         ## For Development
```

### Comparing `pyfmc-0.0.2/README.md` & `pyfmc-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyfmc-0.0.2/pyfmc/pyfmc.egg-info/PKG-INFO` & `pyfmc-0.0.3/pyfmc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pyfmc
-Version: 0.0.2
+Version: 0.0.3
 Summary: Finance Monte-Carlo Simulation using PyTorch
-Home-page: https://github.com/ethanlee928/pyfmc/archive/refs/tags/v0.0.2.tar.gz
+Home-page: https://github.com/ethanlee928/pyfmc
 Author: Ethan Lee
 Author-email: ethan2000.el@gmail.com
 License: UNKNOWN
+Download-URL: https://github.com/ethanlee928/pyfmc/archive/refs/tags/v0.0.3.tar.gz
 Description: # Finance Monte-Carlo Simulation using PyTorch
         
         - An easy-to-use python package to do Monte-Carlo Simulation on stock prices
         - GPU accelerated Monte-Carlo simulation, that could allow simulation more random walkers without a large time penalty
         
         ## For Development
```

