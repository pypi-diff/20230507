# Comparing `tmp/getMultiPrimerSet-1.0.0.tar.gz` & `tmp/getMultiPrimerSet-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getMultiPrimerSet-1.0.0.tar", last modified: Sun May  7 03:51:23 2023, max compression
+gzip compressed data, was "getMultiPrimerSet-1.0.1.tar", last modified: Sun May  7 04:01:21 2023, max compression
```

## Comparing `getMultiPrimerSet-1.0.0.tar` & `getMultiPrimerSet-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 03:51:23.171411 getMultiPrimerSet-1.0.0/
--rw-r--r--   0 semiquant   (502) staff       (20)     2423 2023-05-07 03:51:23.171267 getMultiPrimerSet-1.0.0/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)     2578 2023-05-07 03:49:19.000000 getMultiPrimerSet-1.0.0/README.md
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 03:51:23.170349 getMultiPrimerSet-1.0.0/getMultiPrimerSet/
--rw-r--r--   0 semiquant   (502) staff       (20)    11590 2023-05-07 03:49:25.000000 getMultiPrimerSet-1.0.0/getMultiPrimerSet/getMultiPrimerSet.py
-drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 03:51:23.171074 getMultiPrimerSet-1.0.0/getMultiPrimerSet.egg-info/
--rw-r--r--   0 semiquant   (502) staff       (20)     2423 2023-05-07 03:51:22.000000 getMultiPrimerSet-1.0.0/getMultiPrimerSet.egg-info/PKG-INFO
--rw-r--r--   0 semiquant   (502) staff       (20)      305 2023-05-07 03:51:23.000000 getMultiPrimerSet-1.0.0/getMultiPrimerSet.egg-info/SOURCES.txt
--rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-07 03:51:22.000000 getMultiPrimerSet-1.0.0/getMultiPrimerSet.egg-info/dependency_links.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       79 2023-05-07 03:51:22.000000 getMultiPrimerSet-1.0.0/getMultiPrimerSet.egg-info/entry_points.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       34 2023-05-07 03:51:23.000000 getMultiPrimerSet-1.0.0/getMultiPrimerSet.egg-info/requires.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       18 2023-05-07 03:51:23.000000 getMultiPrimerSet-1.0.0/getMultiPrimerSet.egg-info/top_level.txt
--rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-07 03:51:23.171467 getMultiPrimerSet-1.0.0/setup.cfg
--rw-r--r--   0 semiquant   (502) staff       (20)     2779 2023-05-07 03:51:03.000000 getMultiPrimerSet-1.0.0/setup.py
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 04:01:21.406588 getMultiPrimerSet-1.0.1/
+-rw-r--r--   0 semiquant   (502) staff       (20)     2423 2023-05-07 04:01:21.406432 getMultiPrimerSet-1.0.1/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)     2686 2023-05-07 03:54:39.000000 getMultiPrimerSet-1.0.1/README.md
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 04:01:21.405489 getMultiPrimerSet-1.0.1/getMultiPrimerSet/
+-rw-r--r--   0 semiquant   (502) staff       (20)    11592 2023-05-07 03:59:38.000000 getMultiPrimerSet-1.0.1/getMultiPrimerSet/getMultiPrimerSet.py
+drwxr-xr-x   0 semiquant   (502) staff       (20)        0 2023-05-07 04:01:21.406253 getMultiPrimerSet-1.0.1/getMultiPrimerSet.egg-info/
+-rw-r--r--   0 semiquant   (502) staff       (20)     2423 2023-05-07 04:01:21.000000 getMultiPrimerSet-1.0.1/getMultiPrimerSet.egg-info/PKG-INFO
+-rw-r--r--   0 semiquant   (502) staff       (20)      305 2023-05-07 04:01:21.000000 getMultiPrimerSet-1.0.1/getMultiPrimerSet.egg-info/SOURCES.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)        1 2023-05-07 04:01:21.000000 getMultiPrimerSet-1.0.1/getMultiPrimerSet.egg-info/dependency_links.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       79 2023-05-07 04:01:21.000000 getMultiPrimerSet-1.0.1/getMultiPrimerSet.egg-info/entry_points.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       34 2023-05-07 04:01:21.000000 getMultiPrimerSet-1.0.1/getMultiPrimerSet.egg-info/requires.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       18 2023-05-07 04:01:21.000000 getMultiPrimerSet-1.0.1/getMultiPrimerSet.egg-info/top_level.txt
+-rw-r--r--   0 semiquant   (502) staff       (20)       38 2023-05-07 04:01:21.406637 getMultiPrimerSet-1.0.1/setup.cfg
+-rw-r--r--   0 semiquant   (502) staff       (20)     2779 2023-05-07 03:59:47.000000 getMultiPrimerSet-1.0.1/setup.py
```

### Comparing `getMultiPrimerSet-1.0.0/PKG-INFO` & `getMultiPrimerSet-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getMultiPrimerSet
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for generating multiplex PCR primer sets
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `getMultiPrimerSet-1.0.0/README.md` & `getMultiPrimerSet-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 This program designs PCR primers for a multiplex of given target regions of a DNA sequence in a FASTA file.
 
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7903629.svg)](https://doi.org/10.5281/zenodo.7903629)
+
+
 The script takes several arguments:
 
 | Parameter | Description |
 | --- | --- |
 | region_file (required) | The path to the primer design region file. This file should have three columns: name, start position, and end position (1-based). It can be in either tsv or xlxs format. |
 | input_file (required) | The path to the input FASTA file. |
 | target_tm | The desired melting temperature (Tm) for the primers. Default is 60. |
```

### Comparing `getMultiPrimerSet-1.0.0/getMultiPrimerSet/getMultiPrimerSet.py` & `getMultiPrimerSet-1.0.1/getMultiPrimerSet/getMultiPrimerSet.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy as np
 import concurrent.futures
 import sys
 import random
 
 parser = argparse.ArgumentParser(description='PCR primer design')
 
-from getMultiPrimerSet.getMultiPrimerSet import main
+# from getMultiPrimerSet.getMultiPrimerSet import main
 
 # Define input arguments
 # parser.add_argument('--cpus', type=int, help='number of threads (even though it says cpus)', default=1000)
 parser.add_argument('--region_file', type=str, help='The path to the primer design region file. Two columns, start position and end position (1-based). tsv or xlxs', required=True)
 parser.add_argument('--input_file', type=str, help='The path to the input FASTA file.', required=True)
 parser.add_argument('--target_tm', type=float, help='The desired melting temperature (Tm) for the primers.', default=65)
 parser.add_argument('--primer_len', type=int, help='The desired length of the primers.', default=20)
```

### Comparing `getMultiPrimerSet-1.0.0/getMultiPrimerSet.egg-info/PKG-INFO` & `getMultiPrimerSet-1.0.1/getMultiPrimerSet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getMultiPrimerSet
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for generating multiplex PCR primer sets
 Author: Jason D Limberis
 Author-email: Jason.Limberis@ucsf.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `getMultiPrimerSet-1.0.0/setup.py` & `getMultiPrimerSet-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='getMultiPrimerSet',
-    version='1.0.0',
+    version='1.0.1',
     description='A package for generating multiplex PCR primer sets',
     author='Jason D Limberis',
     author_email='Jason.Limberis@ucsf.edu',
     long_description='''
 This program designs PCR primers for a multiplex of given target regions of a DNA sequence in a FASTA file.
 
 The script takes several arguments:
```

