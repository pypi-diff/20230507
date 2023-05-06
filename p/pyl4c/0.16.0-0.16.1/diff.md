# Comparing `tmp/pyl4c-0.16.0.tar.gz` & `tmp/pyl4c-0.16.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyl4c-0.16.0.tar", last modified: Sat May  6 23:07:00 2023, max compression
+gzip compressed data, was "pyl4c-0.16.1.tar", last modified: Sat May  6 23:35:44 2023, max compression
```

## Comparing `pyl4c-0.16.0.tar` & `pyl4c-0.16.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:07:00.002541 pyl4c-0.16.0/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1174 2023-05-06 23:00:51.000000 pyl4c-0.16.0/LICENSE
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     4126 2023-05-06 23:07:00.002541 pyl4c-0.16.0/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     3540 2023-05-06 23:00:51.000000 pyl4c-0.16.0/README.md
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:06:59.998541 pyl4c-0.16.0/pyl4c/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     5136 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/__init__.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:06:59.998541 pyl4c-0.16.0/pyl4c/apps/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      316 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/apps/__init__.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:06:59.998541 pyl4c-0.16.0/pyl4c/apps/calibration/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    22571 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/apps/calibration/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    37841 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/apps/calibration/main.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     6061 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/apps/calibration/nature.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:06:59.998541 pyl4c-0.16.0/pyl4c/apps/l4c/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    25025 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/apps/l4c/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     4039 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/apps/l4c/io.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    23120 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/apps/l4c/main.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    15574 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/apps/resample.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:07:00.002541 pyl4c-0.16.0/pyl4c/data/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/data/__init__.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:07:00.002541 pyl4c-0.16.0/pyl4c/data/files/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2497 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/data/files/SMAP_BPLUT_2020-07-31.csv
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      235 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/data/files/config_calibration.json
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    13075 2023-05-06 23:02:24.000000 pyl4c-0.16.0/pyl4c/data/fixtures.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     9426 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/ease2.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     3275 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/epsg.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:07:00.002541 pyl4c-0.16.0/pyl4c/lib/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       14 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/lib/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    15544 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/lib/cli.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     9108 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/lib/modis.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    16110 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/lib/netcdf.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    18082 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/lib/tcf.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    17638 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/lib/transcom.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    11426 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/lib/transpiration.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    34283 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/science.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    33119 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/spatial.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    12564 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/stats.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:07:00.002541 pyl4c-0.16.0/pyl4c/tests/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       20 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/tests/__init__.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     3342 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/tests/calibration.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     4721 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/tests/l4c.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    20579 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/tests/tests.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     2124 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/tests/transpiration.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     6945 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/towers.py
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    33781 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/utils.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:06:59.998541 pyl4c-0.16.0/pyl4c.egg-info/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     4126 2023-05-06 23:06:59.000000 pyl4c-0.16.0/pyl4c.egg-info/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      932 2023-05-06 23:06:59.000000 pyl4c-0.16.0/pyl4c.egg-info/SOURCES.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-05-06 23:06:59.000000 pyl4c-0.16.0/pyl4c.egg-info/dependency_links.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      259 2023-05-06 23:06:59.000000 pyl4c-0.16.0/pyl4c.egg-info/requires.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       52 2023-05-06 23:06:59.000000 pyl4c-0.16.0/pyl4c.egg-info/top_level.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      104 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyproject.toml
--rw-rw-r--   0 arthur    (1000) arthur    (1000)     1095 2023-05-06 23:07:00.006541 pyl4c-0.16.0/setup.cfg
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      150 2023-05-06 23:00:51.000000 pyl4c-0.16.0/setup.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:35:44.894527 pyl4c-0.16.1/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1174 2023-05-06 23:00:51.000000 pyl4c-0.16.1/LICENSE
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     4126 2023-05-06 23:35:44.894527 pyl4c-0.16.1/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3540 2023-05-06 23:00:51.000000 pyl4c-0.16.1/README.md
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:35:44.886527 pyl4c-0.16.1/pyl4c/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     5136 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/__init__.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:35:44.890527 pyl4c-0.16.1/pyl4c/apps/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      316 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/apps/__init__.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:35:44.890527 pyl4c-0.16.1/pyl4c/apps/calibration/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    22571 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/apps/calibration/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    37841 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/apps/calibration/main.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     6061 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/apps/calibration/nature.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:35:44.890527 pyl4c-0.16.1/pyl4c/apps/l4c/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    25025 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/apps/l4c/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     4039 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/apps/l4c/io.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    23120 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/apps/l4c/main.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    15574 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/apps/resample.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:35:44.890527 pyl4c-0.16.1/pyl4c/data/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/data/__init__.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:35:44.890527 pyl4c-0.16.1/pyl4c/data/files/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2497 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/data/files/SMAP_BPLUT_2020-07-31.csv
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      235 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/data/files/config_calibration.json
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    13109 2023-05-06 23:34:12.000000 pyl4c-0.16.1/pyl4c/data/fixtures.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     9426 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/ease2.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3275 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/epsg.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:35:44.894527 pyl4c-0.16.1/pyl4c/lib/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       14 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/lib/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    15544 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/lib/cli.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     9108 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/lib/modis.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    16110 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/lib/netcdf.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    18082 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/lib/tcf.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    17638 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/lib/transcom.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    11426 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/lib/transpiration.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    34283 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/science.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    33119 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/spatial.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    12564 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/stats.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:35:44.894527 pyl4c-0.16.1/pyl4c/tests/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       20 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/tests/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3342 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/tests/calibration.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     4721 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/tests/l4c.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    20579 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/tests/tests.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2124 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/tests/transpiration.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     6945 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/towers.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    33781 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyl4c/utils.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:35:44.890527 pyl4c-0.16.1/pyl4c.egg-info/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     4126 2023-05-06 23:35:44.000000 pyl4c-0.16.1/pyl4c.egg-info/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      932 2023-05-06 23:35:44.000000 pyl4c-0.16.1/pyl4c.egg-info/SOURCES.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-05-06 23:35:44.000000 pyl4c-0.16.1/pyl4c.egg-info/dependency_links.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      259 2023-05-06 23:35:44.000000 pyl4c-0.16.1/pyl4c.egg-info/requires.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       52 2023-05-06 23:35:44.000000 pyl4c-0.16.1/pyl4c.egg-info/top_level.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      104 2023-05-06 23:00:51.000000 pyl4c-0.16.1/pyproject.toml
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1095 2023-05-06 23:35:44.894527 pyl4c-0.16.1/setup.cfg
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      150 2023-05-06 23:00:51.000000 pyl4c-0.16.1/setup.py
```

### Comparing `pyl4c-0.16.0/LICENSE` & `pyl4c-0.16.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/PKG-INFO` & `pyl4c-0.16.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyl4c
-Version: 0.16.0
+Version: 0.16.1
 Summary: Python tools for working with SMAP L4C data
 Author: K. Arthur Endsley
 Author-email: arthur.endsley@ntsg.umt.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `pyl4c-0.16.0/README.md` & `pyl4c-0.16.1/README.md`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/__init__.py` & `pyl4c-0.16.1/pyl4c/__init__.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/apps/calibration/__init__.py` & `pyl4c-0.16.1/pyl4c/apps/calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/apps/calibration/main.py` & `pyl4c-0.16.1/pyl4c/apps/calibration/main.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/apps/calibration/nature.py` & `pyl4c-0.16.1/pyl4c/apps/calibration/nature.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/apps/l4c/__init__.py` & `pyl4c-0.16.1/pyl4c/apps/l4c/__init__.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/apps/l4c/io.py` & `pyl4c-0.16.1/pyl4c/apps/l4c/io.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/apps/l4c/main.py` & `pyl4c-0.16.1/pyl4c/apps/l4c/main.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/apps/resample.py` & `pyl4c-0.16.1/pyl4c/apps/resample.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/data/files/SMAP_BPLUT_2020-07-31.csv` & `pyl4c-0.16.1/pyl4c/data/files/SMAP_BPLUT_2020-07-31.csv`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/data/fixtures.py` & `pyl4c-0.16.1/pyl4c/data/fixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,9 +329,9 @@
     params = restore_bplut(csv_file_path, version_id)
     result = dict()
     for key, value in params.items():
         if key not in ('tmin', 'vpd', 'smsf', 'smrz', 'ft'):
             result[key] = value
             continue
         for i, array in enumerate(value.tolist()):
-            result[f'{key}{i}'] = array
+            result[f'{key}{i}'] = np.array(array).reshape((1,len(array)))
     return OrderedDict(result)
```

### Comparing `pyl4c-0.16.0/pyl4c/ease2.py` & `pyl4c-0.16.1/pyl4c/ease2.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/epsg.py` & `pyl4c-0.16.1/pyl4c/epsg.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/lib/cli.py` & `pyl4c-0.16.1/pyl4c/lib/cli.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/lib/modis.py` & `pyl4c-0.16.1/pyl4c/lib/modis.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/lib/netcdf.py` & `pyl4c-0.16.1/pyl4c/lib/netcdf.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/lib/tcf.py` & `pyl4c-0.16.1/pyl4c/lib/tcf.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/lib/transcom.py` & `pyl4c-0.16.1/pyl4c/lib/transcom.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/lib/transpiration.py` & `pyl4c-0.16.1/pyl4c/lib/transpiration.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/science.py` & `pyl4c-0.16.1/pyl4c/science.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/spatial.py` & `pyl4c-0.16.1/pyl4c/spatial.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/stats.py` & `pyl4c-0.16.1/pyl4c/stats.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/tests/calibration.py` & `pyl4c-0.16.1/pyl4c/tests/calibration.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/tests/l4c.py` & `pyl4c-0.16.1/pyl4c/tests/l4c.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/tests/tests.py` & `pyl4c-0.16.1/pyl4c/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/tests/transpiration.py` & `pyl4c-0.16.1/pyl4c/tests/transpiration.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/towers.py` & `pyl4c-0.16.1/pyl4c/towers.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c/utils.py` & `pyl4c-0.16.1/pyl4c/utils.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/pyl4c.egg-info/PKG-INFO` & `pyl4c-0.16.1/pyl4c.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyl4c
-Version: 0.16.0
+Version: 0.16.1
 Summary: Python tools for working with SMAP L4C data
 Author: K. Arthur Endsley
 Author-email: arthur.endsley@ntsg.umt.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `pyl4c-0.16.0/pyl4c.egg-info/SOURCES.txt` & `pyl4c-0.16.1/pyl4c.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyl4c-0.16.0/setup.cfg` & `pyl4c-0.16.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyl4c
-version = 0.16.0
+version = 0.16.1
 author = K. Arthur Endsley
 author_email = arthur.endsley@ntsg.umt.edu
 description = Python tools for working with SMAP L4C data
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

