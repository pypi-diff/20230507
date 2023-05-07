# Comparing `tmp/pyroe-0.9.1.tar.gz` & `tmp/pyroe-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroe-0.9.1.tar", last modified: Mon Apr 17 03:07:00 2023, max compression
+gzip compressed data, was "pyroe-0.9.2.tar", last modified: Sun May  7 14:22:34 2023, max compression
```

## Comparing `pyroe-0.9.1.tar` & `pyroe-0.9.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:00.005496 pyroe-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-17 03:06:48.000000 pyroe-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-17 03:07:00.005496 pyroe-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-17 03:06:48.000000 pyroe-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:00.001496 pyroe-0.9.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10146 2023-04-17 03:06:48.000000 pyroe-0.9.1/bin/pyroe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-17 03:06:48.000000 pyroe-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 03:07:00.005496 pyroe-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:00.001496 pyroe-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:00.005496 pyroe-0.9.1/src/pyroe/
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/ProcessedQuant.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:00.005496 pyroe-0.9.1/src/pyroe/data/
--rw-r--r--   0 runner    (1001) docker     (123)    14989 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/data/available_datasets.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/fetch_processed_quant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/id_to_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/load_fry.py
--rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/load_processed_quant.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24577 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/make_splici_txome.py
--rw-r--r--   0 runner    (1001) docker     (123)    50262 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/make_txome.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-17 03:06:48.000000 pyroe-0.9.1/src/pyroe/pyroe_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:00.005496 pyroe-0.9.1/src/pyroe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-17 03:06:59.000000 pyroe-0.9.1/src/pyroe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-17 03:07:00.000000 pyroe-0.9.1/src/pyroe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 03:06:59.000000 pyroe-0.9.1/src/pyroe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 03:06:59.000000 pyroe-0.9.1/src/pyroe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 03:06:59.000000 pyroe-0.9.1/src/pyroe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 03:07:00.005496 pyroe-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-17 03:06:48.000000 pyroe-0.9.1/tests/test_ProcessedQuant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-17 03:06:48.000000 pyroe-0.9.1/tests/test_fetch_processed_quant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-17 03:06:48.000000 pyroe-0.9.1/tests/test_load_processed_quant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-17 03:06:48.000000 pyroe-0.9.1/tests/test_make_spliceu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-17 03:06:48.000000 pyroe-0.9.1/tests/test_make_splici.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:22:34.415984 pyroe-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-07 14:22:18.000000 pyroe-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-07 14:22:34.415984 pyroe-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-07 14:22:18.000000 pyroe-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:22:34.411984 pyroe-0.9.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10146 2023-05-07 14:22:18.000000 pyroe-0.9.2/bin/pyroe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-07 14:22:18.000000 pyroe-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-07 14:22:34.415984 pyroe-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:22:34.411984 pyroe-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:22:34.411984 pyroe-0.9.2/src/pyroe/
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/ProcessedQuant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:22:34.411984 pyroe-0.9.2/src/pyroe/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14989 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/data/available_datasets.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/fetch_processed_quant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/id_to_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/load_fry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/load_processed_quant.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24577 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/make_splici_txome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50262 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/make_txome.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-07 14:22:18.000000 pyroe-0.9.2/src/pyroe/pyroe_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:22:34.411984 pyroe-0.9.2/src/pyroe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-07 14:22:34.000000 pyroe-0.9.2/src/pyroe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-07 14:22:34.000000 pyroe-0.9.2/src/pyroe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 14:22:34.000000 pyroe-0.9.2/src/pyroe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-07 14:22:34.000000 pyroe-0.9.2/src/pyroe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 14:22:34.000000 pyroe-0.9.2/src/pyroe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:22:34.415984 pyroe-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-07 14:22:18.000000 pyroe-0.9.2/tests/test_ProcessedQuant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-07 14:22:18.000000 pyroe-0.9.2/tests/test_fetch_processed_quant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-07 14:22:18.000000 pyroe-0.9.2/tests/test_load_processed_quant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-07 14:22:18.000000 pyroe-0.9.2/tests/test_make_spliceu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-05-07 14:22:18.000000 pyroe-0.9.2/tests/test_make_splici.py
```

### Comparing `pyroe-0.9.1/LICENSE` & `pyroe-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.1/PKG-INFO` & `pyroe-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroe
-Version: 0.9.1
+Version: 0.9.2
 Summary: utilities of alevin-fry
 Home-page: https://github.com/COMBINE-lab/pyroe
 Author: Dongze He, Rob Patro
 Author-email: dhe17@umd.edu, rob@cs.umd.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyroe-0.9.1/README.md` & `pyroe-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.1/bin/pyroe` & `pyroe-0.9.2/bin/pyroe`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.1/setup.cfg` & `pyroe-0.9.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyroe
-version = 0.9.1
+version = 0.9.2
 author = Dongze He, Rob Patro
 author_email = dhe17@umd.edu, rob@cs.umd.edu
 description = utilities of alevin-fry
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/COMBINE-lab/pyroe
 classifiers = 
@@ -18,15 +18,15 @@
 	= src
 scripts = 
 	bin/pyroe
 python_requires = >=3.7
 include_package_data = True
 install_requires = 
 	pandas >= 1.3.0, < 2.0.0
-	pyranges >= 0.0.120
+	pyranges == 0.0.120
 	biopython >= 1.77
 	packaging >= 21.0
 	scanpy >= 1.8.2
 
 [options.packages.find]
 where = src
```

### Comparing `pyroe-0.9.1/src/pyroe/ProcessedQuant.py` & `pyroe-0.9.2/src/pyroe/ProcessedQuant.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.1/src/pyroe/convert.py` & `pyroe-0.9.2/src/pyroe/convert.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.1/src/pyroe/data/available_datasets.tsv` & `pyroe-0.9.2/src/pyroe/data/available_datasets.tsv`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.1/src/pyroe/fetch_processed_quant.py` & `pyroe-0.9.2/src/pyroe/fetch_processed_quant.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.1/src/pyroe/id_to_name.py` & `pyroe-0.9.2/src/pyroe/id_to_name.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.1/src/pyroe/load_fry.py` & `pyroe-0.9.2/src/pyroe/load_fry.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.1/src/pyroe/load_processed_quant.py` & `pyroe-0.9.2/src/pyroe/load_processed_quant.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.1/src/pyroe/make_splici_txome.py` & `pyroe-0.9.2/src/pyroe/make_splici_txome.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.1/src/pyroe/make_txome.py` & `pyroe-0.9.2/src/pyroe/make_txome.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.1/src/pyroe/pyroe_utils.py` & `pyroe-0.9.2/src/pyroe/pyroe_utils.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.1/src/pyroe.egg-info/PKG-INFO` & `pyroe-0.9.2/src/pyroe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroe
-Version: 0.9.1
+Version: 0.9.2
 Summary: utilities of alevin-fry
 Home-page: https://github.com/COMBINE-lab/pyroe
 Author: Dongze He, Rob Patro
 Author-email: dhe17@umd.edu, rob@cs.umd.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyroe-0.9.1/src/pyroe.egg-info/SOURCES.txt` & `pyroe-0.9.2/src/pyroe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.1/tests/test_ProcessedQuant.py` & `pyroe-0.9.2/tests/test_ProcessedQuant.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.1/tests/test_fetch_processed_quant.py` & `pyroe-0.9.2/tests/test_fetch_processed_quant.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.1/tests/test_load_processed_quant.py` & `pyroe-0.9.2/tests/test_load_processed_quant.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.1/tests/test_make_spliceu.py` & `pyroe-0.9.2/tests/test_make_spliceu.py`

 * *Files identical despite different names*

### Comparing `pyroe-0.9.1/tests/test_make_splici.py` & `pyroe-0.9.2/tests/test_make_splici.py`

 * *Files identical despite different names*

