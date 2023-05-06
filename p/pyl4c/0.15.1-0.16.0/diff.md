# Comparing `tmp/pyl4c-0.15.1.tar.gz` & `tmp/pyl4c-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyl4c-0.15.1.tar", last modified: Tue Feb 28 21:50:42 2023, max compression
+gzip compressed data, was "pyl4c-0.16.0.tar", last modified: Sat May  6 23:07:00 2023, max compression
```

## Comparing `pyl4c-0.15.1.tar` & `pyl4c-0.16.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 arthur.endsley  (1009) arthur.endsley  (1009)        0 2023-02-28 21:50:42.248492 pyl4c-0.15.1/
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)     1174 2023-02-09 19:42:44.000000 pyl4c-0.15.1/LICENSE
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)     4126 2023-02-28 21:50:42.248492 pyl4c-0.15.1/PKG-INFO
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)     3540 2023-02-09 20:37:28.000000 pyl4c-0.15.1/README.md
-drwxrwxr-x   0 arthur.endsley  (1009) arthur.endsley  (1009)        0 2023-02-28 21:50:42.244491 pyl4c-0.15.1/pyl4c/
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)     5136 2023-02-09 21:24:47.000000 pyl4c-0.15.1/pyl4c/__init__.py
-drwxrwxr-x   0 arthur.endsley  (1009) arthur.endsley  (1009)        0 2023-02-28 21:50:42.244491 pyl4c-0.15.1/pyl4c/apps/
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)      316 2023-02-09 19:42:44.000000 pyl4c-0.15.1/pyl4c/apps/__init__.py
-drwxrwxr-x   0 arthur.endsley  (1009) arthur.endsley  (1009)        0 2023-02-28 21:50:42.244491 pyl4c-0.15.1/pyl4c/apps/calibration/
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)    22571 2023-02-09 19:42:44.000000 pyl4c-0.15.1/pyl4c/apps/calibration/__init__.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)    37841 2023-02-09 19:42:44.000000 pyl4c-0.15.1/pyl4c/apps/calibration/main.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)     6061 2023-02-09 19:42:44.000000 pyl4c-0.15.1/pyl4c/apps/calibration/nature.py
-drwxrwxr-x   0 arthur.endsley  (1009) arthur.endsley  (1009)        0 2023-02-28 21:50:42.244491 pyl4c-0.15.1/pyl4c/apps/l4c/
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)    25025 2023-02-09 20:37:28.000000 pyl4c-0.15.1/pyl4c/apps/l4c/__init__.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)     4039 2023-02-09 20:28:39.000000 pyl4c-0.15.1/pyl4c/apps/l4c/io.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)    23120 2023-02-09 20:37:28.000000 pyl4c-0.15.1/pyl4c/apps/l4c/main.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)    15574 2023-02-28 21:35:23.000000 pyl4c-0.15.1/pyl4c/apps/resample.py
-drwxrwxr-x   0 arthur.endsley  (1009) arthur.endsley  (1009)        0 2023-02-28 21:50:42.244491 pyl4c-0.15.1/pyl4c/data/
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)        0 2023-02-09 19:42:44.000000 pyl4c-0.15.1/pyl4c/data/__init__.py
-drwxrwxr-x   0 arthur.endsley  (1009) arthur.endsley  (1009)        0 2023-02-28 21:50:42.244491 pyl4c-0.15.1/pyl4c/data/files/
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)     2497 2023-02-09 19:42:44.000000 pyl4c-0.15.1/pyl4c/data/files/SMAP_BPLUT_2020-07-31.csv
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)      235 2023-02-09 19:42:44.000000 pyl4c-0.15.1/pyl4c/data/files/config_calibration.json
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)    12201 2023-02-09 19:42:44.000000 pyl4c-0.15.1/pyl4c/data/fixtures.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)     9426 2023-02-09 21:24:55.000000 pyl4c-0.15.1/pyl4c/ease2.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)     3275 2023-02-09 19:42:44.000000 pyl4c-0.15.1/pyl4c/epsg.py
-drwxrwxr-x   0 arthur.endsley  (1009) arthur.endsley  (1009)        0 2023-02-28 21:50:42.244491 pyl4c-0.15.1/pyl4c/lib/
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)       14 2023-02-09 21:25:03.000000 pyl4c-0.15.1/pyl4c/lib/__init__.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)    15544 2023-02-09 19:42:44.000000 pyl4c-0.15.1/pyl4c/lib/cli.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)     9108 2023-02-09 20:37:28.000000 pyl4c-0.15.1/pyl4c/lib/modis.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)    15824 2023-02-09 21:25:13.000000 pyl4c-0.15.1/pyl4c/lib/netcdf.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)    18082 2023-02-09 21:25:18.000000 pyl4c-0.15.1/pyl4c/lib/tcf.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)    17638 2023-02-09 19:42:44.000000 pyl4c-0.15.1/pyl4c/lib/transcom.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)    11426 2023-02-09 19:42:44.000000 pyl4c-0.15.1/pyl4c/lib/transpiration.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)    35690 2023-02-09 20:37:28.000000 pyl4c-0.15.1/pyl4c/science.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)    33119 2023-02-09 21:25:39.000000 pyl4c-0.15.1/pyl4c/spatial.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)    12564 2023-02-09 20:37:28.000000 pyl4c-0.15.1/pyl4c/stats.py
-drwxrwxr-x   0 arthur.endsley  (1009) arthur.endsley  (1009)        0 2023-02-28 21:50:42.244491 pyl4c-0.15.1/pyl4c/tests/
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)       20 2023-02-09 19:42:44.000000 pyl4c-0.15.1/pyl4c/tests/__init__.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)     3342 2023-02-09 19:42:44.000000 pyl4c-0.15.1/pyl4c/tests/calibration.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)     4721 2023-02-09 20:37:28.000000 pyl4c-0.15.1/pyl4c/tests/l4c.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)    20579 2023-02-09 20:37:28.000000 pyl4c-0.15.1/pyl4c/tests/tests.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)     2124 2023-02-09 19:42:44.000000 pyl4c-0.15.1/pyl4c/tests/transpiration.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)     6945 2023-02-09 19:42:44.000000 pyl4c-0.15.1/pyl4c/towers.py
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)    33781 2023-02-28 21:29:06.000000 pyl4c-0.15.1/pyl4c/utils.py
-drwxrwxr-x   0 arthur.endsley  (1009) arthur.endsley  (1009)        0 2023-02-28 21:50:42.244491 pyl4c-0.15.1/pyl4c.egg-info/
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)     4126 2023-02-28 21:50:42.000000 pyl4c-0.15.1/pyl4c.egg-info/PKG-INFO
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)      932 2023-02-28 21:50:42.000000 pyl4c-0.15.1/pyl4c.egg-info/SOURCES.txt
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)        1 2023-02-28 21:50:42.000000 pyl4c-0.15.1/pyl4c.egg-info/dependency_links.txt
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)      259 2023-02-28 21:50:42.000000 pyl4c-0.15.1/pyl4c.egg-info/requires.txt
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)       52 2023-02-28 21:50:42.000000 pyl4c-0.15.1/pyl4c.egg-info/top_level.txt
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)      104 2023-02-09 20:37:28.000000 pyl4c-0.15.1/pyproject.toml
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)     1095 2023-02-28 21:50:42.248492 pyl4c-0.15.1/setup.cfg
--rw-rw-r--   0 arthur.endsley  (1009) arthur.endsley  (1009)      150 2023-02-09 19:42:44.000000 pyl4c-0.15.1/setup.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:07:00.002541 pyl4c-0.16.0/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1174 2023-05-06 23:00:51.000000 pyl4c-0.16.0/LICENSE
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     4126 2023-05-06 23:07:00.002541 pyl4c-0.16.0/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3540 2023-05-06 23:00:51.000000 pyl4c-0.16.0/README.md
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:06:59.998541 pyl4c-0.16.0/pyl4c/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     5136 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/__init__.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:06:59.998541 pyl4c-0.16.0/pyl4c/apps/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      316 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/apps/__init__.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:06:59.998541 pyl4c-0.16.0/pyl4c/apps/calibration/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    22571 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/apps/calibration/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    37841 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/apps/calibration/main.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     6061 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/apps/calibration/nature.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:06:59.998541 pyl4c-0.16.0/pyl4c/apps/l4c/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    25025 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/apps/l4c/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     4039 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/apps/l4c/io.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    23120 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/apps/l4c/main.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    15574 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/apps/resample.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:07:00.002541 pyl4c-0.16.0/pyl4c/data/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/data/__init__.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:07:00.002541 pyl4c-0.16.0/pyl4c/data/files/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2497 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/data/files/SMAP_BPLUT_2020-07-31.csv
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      235 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/data/files/config_calibration.json
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    13075 2023-05-06 23:02:24.000000 pyl4c-0.16.0/pyl4c/data/fixtures.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     9426 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/ease2.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3275 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/epsg.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:07:00.002541 pyl4c-0.16.0/pyl4c/lib/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       14 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/lib/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    15544 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/lib/cli.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     9108 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/lib/modis.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    16110 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/lib/netcdf.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    18082 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/lib/tcf.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    17638 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/lib/transcom.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    11426 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/lib/transpiration.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    34283 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/science.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    33119 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/spatial.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    12564 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/stats.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:07:00.002541 pyl4c-0.16.0/pyl4c/tests/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       20 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/tests/__init__.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     3342 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/tests/calibration.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     4721 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/tests/l4c.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    20579 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/tests/tests.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     2124 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/tests/transpiration.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     6945 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/towers.py
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    33781 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyl4c/utils.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-05-06 23:06:59.998541 pyl4c-0.16.0/pyl4c.egg-info/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     4126 2023-05-06 23:06:59.000000 pyl4c-0.16.0/pyl4c.egg-info/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      932 2023-05-06 23:06:59.000000 pyl4c-0.16.0/pyl4c.egg-info/SOURCES.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-05-06 23:06:59.000000 pyl4c-0.16.0/pyl4c.egg-info/dependency_links.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      259 2023-05-06 23:06:59.000000 pyl4c-0.16.0/pyl4c.egg-info/requires.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       52 2023-05-06 23:06:59.000000 pyl4c-0.16.0/pyl4c.egg-info/top_level.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      104 2023-05-06 23:00:51.000000 pyl4c-0.16.0/pyproject.toml
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)     1095 2023-05-06 23:07:00.006541 pyl4c-0.16.0/setup.cfg
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      150 2023-05-06 23:00:51.000000 pyl4c-0.16.0/setup.py
```

### Comparing `pyl4c-0.15.1/LICENSE` & `pyl4c-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/PKG-INFO` & `pyl4c-0.16.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyl4c
-Version: 0.15.1
+Version: 0.16.0
 Summary: Python tools for working with SMAP L4C data
 Author: K. Arthur Endsley
 Author-email: arthur.endsley@ntsg.umt.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `pyl4c-0.15.1/README.md` & `pyl4c-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/__init__.py` & `pyl4c-0.16.0/pyl4c/__init__.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/apps/calibration/__init__.py` & `pyl4c-0.16.0/pyl4c/apps/calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/apps/calibration/main.py` & `pyl4c-0.16.0/pyl4c/apps/calibration/main.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/apps/calibration/nature.py` & `pyl4c-0.16.0/pyl4c/apps/calibration/nature.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/apps/l4c/__init__.py` & `pyl4c-0.16.0/pyl4c/apps/l4c/__init__.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/apps/l4c/io.py` & `pyl4c-0.16.0/pyl4c/apps/l4c/io.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/apps/l4c/main.py` & `pyl4c-0.16.0/pyl4c/apps/l4c/main.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/apps/resample.py` & `pyl4c-0.16.0/pyl4c/apps/resample.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/data/files/SMAP_BPLUT_2020-07-31.csv` & `pyl4c-0.16.0/pyl4c/data/files/SMAP_BPLUT_2020-07-31.csv`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/data/fixtures.py` & `pyl4c-0.16.0/pyl4c/data/fixtures.py`

 * *Files 3% similar despite different names*

```diff
@@ -198,15 +198,15 @@
     -------
     numpy.ndarray
         Array of same size, shape as pft_array but with parameter values
         in place of PFT codes
     '''
     param = bplut[name]
     # Basically, index the <name> array, in PFT order, by PFT numeric codes
-    return np.asarray(param)[np.ravel(pft_array)].reshape(pft_array.shape)
+    return np.asarray(param)[:,np.ravel(pft_array)].reshape(pft_array.shape)
 
 
 def restore_bplut(csv_file_path, version_id = None):
     '''
     Translates a BPLUT CSV file to a Python internal representation
     (OrderedDict instance).
 
@@ -302,7 +302,36 @@
     # The "kstr" and "kslw" values are really the fraction of kopt
     #   assigned to the second and third pools
     result['decay_rates'][1,:] = np.multiply(
         result['decay_rates'][0,:], result['decay_rates'][1,:])
     result['decay_rates'][2,:] = np.multiply(
         result['decay_rates'][0,:], result['decay_rates'][2,:])
     return result
+
+
+def restore_bplut_flat(csv_file_path, version_id = None):
+    '''
+    Translates a BPLUT CSV file to a Python internal representation
+    (OrderedDict instance). Compare to `restore_bplut()`, this version
+    sets parameter values as flat lists instead of n-dimensional NumPy
+    arrays.
+
+    Parameters
+    ----------
+    csv_file_path : str
+        File path to the CSV representation of the BPLUT
+    version_id : str
+        (Optional) Version identifier for the BPLUT
+
+    Returns
+    -------
+    OrderedDict
+    '''
+    params = restore_bplut(csv_file_path, version_id)
+    result = dict()
+    for key, value in params.items():
+        if key not in ('tmin', 'vpd', 'smsf', 'smrz', 'ft'):
+            result[key] = value
+            continue
+        for i, array in enumerate(value.tolist()):
+            result[f'{key}{i}'] = array
+    return OrderedDict(result)
```

### Comparing `pyl4c-0.15.1/pyl4c/ease2.py` & `pyl4c-0.16.0/pyl4c/ease2.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/epsg.py` & `pyl4c-0.16.0/pyl4c/epsg.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/lib/cli.py` & `pyl4c-0.16.0/pyl4c/lib/cli.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/lib/modis.py` & `pyl4c-0.16.0/pyl4c/lib/modis.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/lib/netcdf.py` & `pyl4c-0.16.0/pyl4c/lib/netcdf.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,17 @@
     '''
     if hasattr(variable, 'ndim'):
         return variable.ndim
     if hasattr(variable, 'dimensions'):
         return len(variable.dimensions)
 
 
-def netcdf_array(nc, keys, cell_size = None, time_idx = 0, x_offset = -180):
+def netcdf_array(
+        nc, keys, cell_size = None, time_idx = 0, x_offset = -180,
+        scale_and_offset = True):
     '''
     Extracts an equirectangular NetCDF data array as a NumPy array, with
     spatial reference system (SRS) information. NOTE: Both `cell_size` elements
     should be positive numbers.
 
     Parameters
     ----------
@@ -58,14 +60,18 @@
         (Optional) Index of the "time" axis to extract as a raster
         (Default: 0)
     x_offset : int or float
         (Optional) Because of the absurd X-coordinates convention used in some
         NetCDF arrays, it may be necessary to "offset" the X coordinates; this
         is only used if it is detected that the maximum X coordinate value is
         >/= 180 degrees E (Default: -180);
+    scale_and_offset : bool
+        (Optional) True to apply the scale and offset to the data, if the
+        attributes "scale_factor" and "add_offset" are found (Default); False
+        to do nothing
 
     Returns
     -------
     tuple
         Tuple of `(array, gt, wkt)`
     '''
     def infer_cell_size(x_coords, y_coords):
@@ -130,19 +136,19 @@
         arr = np.flip(arr, axis = 1)
 
     # If necessary, re-sort data so west-most longitude is the first column
     if start_idx is not None:
         arr = np.concatenate((arr[...,start_idx:], arr[...,:start_idx]), axis = 2)
 
     scale = 1
-    if hasattr(nc.variables[keys[0]], 'scale_factor'):
+    if scale_and_offset and hasattr(nc.variables[keys[0]], 'scale_factor'):
         scale = nc.variables[keys[0]].scale_factor
 
     offset = 0
-    if hasattr(nc.variables[keys[0]], 'add_offset'):
+    if scale_and_offset and hasattr(nc.variables[keys[0]], 'add_offset'):
         offset = nc.variables[keys[0]].add_offset
 
     return ((arr * scale) + offset, gt0, wkt0.ExportToWkt())
 
 
 def netcdf_raster(
         nc, keys, cell_size = None, time_idx = 0, subset_bbox = None,
```

### Comparing `pyl4c-0.15.1/pyl4c/lib/tcf.py` & `pyl4c-0.16.0/pyl4c/lib/tcf.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/lib/transcom.py` & `pyl4c-0.16.0/pyl4c/lib/transcom.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/lib/transpiration.py` & `pyl4c-0.16.0/pyl4c/lib/transpiration.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/science.py` & `pyl4c-0.16.0/pyl4c/science.py`

 * *Files 2% similar despite different names*

```diff
@@ -492,55 +492,14 @@
     if units == 'years':
         # NOTE: No need to guard against NaNs/ NoData here because of mask
         mrt = np.divide(mrt, 365.0)
     np.place(mrt, mask, nodata) # Put NoData values back in
     return (mrt, xoff, yoff)
 
 
-def npp(
-        hdf, use_subgrid = False, subset_id = None, subset_bbox = None,
-        nodata = -9999):
-    '''
-    Calculates net primary productivity (NPP), based on the carbon use
-    efficiency (CUE) of each plant functional type (PFT). NPP is derived
-    as: `NPP = GPP * CUE`, where `CUE = NPP/GPP`.
-
-    Parameters
-    ----------
-    hdf : h5py.File
-        The HDF5 file / h5py.File object
-    use_subgrid : bool
-        True to use the 1-km subgrid; requires iterating through the PFT means
-    subset_id : str
-        (Optional) Can provide keyword designating the desired subset area
-    subset_bbox : list or tuple
-        (Optional) Can provide a bounding box to define a desired subset area
-    nodata : float
-        The NoData value to mask (Default: -9999)
-
-    Returns
-    -------
-    numpy.ndarray
-        NPP values on an EASE-Grid 2.0 array
-    '''
-    grid = 'M01' if use_subgrid else 'M09'
-    cue_array = cue(get_pft_array(grid, subset_id, subset_bbox))
-    if not use_subgrid:
-        if subset_id is not None or subset_bbox is not None:
-            gpp, _, _ = subset(
-                hdf, 'GPP/gpp_mean', subset_id = subset_id,
-                subset_bbox = subset_bbox)
-        else:
-            gpp = hdf['GPP/gpp_mean'][:]
-    else:
-        raise NotImplementedError('No support for the 1-km subgrid')
-    gpp[gpp == nodata] = np.nan
-    return np.multiply(gpp, cue_array)
-
-
 def ordinals365(dates):
     '''
     Returns a length-T sequence of ordinals on [1,365]. Can be used for
     indexing a 365-day climatology; see `climatology365()`.
 
     Parameters
     ----------
```

### Comparing `pyl4c-0.15.1/pyl4c/spatial.py` & `pyl4c-0.16.0/pyl4c/spatial.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/stats.py` & `pyl4c-0.16.0/pyl4c/stats.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/tests/calibration.py` & `pyl4c-0.16.0/pyl4c/tests/calibration.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/tests/l4c.py` & `pyl4c-0.16.0/pyl4c/tests/l4c.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/tests/tests.py` & `pyl4c-0.16.0/pyl4c/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/tests/transpiration.py` & `pyl4c-0.16.0/pyl4c/tests/transpiration.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/towers.py` & `pyl4c-0.16.0/pyl4c/towers.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c/utils.py` & `pyl4c-0.16.0/pyl4c/utils.py`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/pyl4c.egg-info/PKG-INFO` & `pyl4c-0.16.0/pyl4c.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyl4c
-Version: 0.15.1
+Version: 0.16.0
 Summary: Python tools for working with SMAP L4C data
 Author: K. Arthur Endsley
 Author-email: arthur.endsley@ntsg.umt.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `pyl4c-0.15.1/pyl4c.egg-info/SOURCES.txt` & `pyl4c-0.16.0/pyl4c.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyl4c-0.15.1/setup.cfg` & `pyl4c-0.16.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyl4c
-version = 0.15.1
+version = 0.16.0
 author = K. Arthur Endsley
 author_email = arthur.endsley@ntsg.umt.edu
 description = Python tools for working with SMAP L4C data
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

