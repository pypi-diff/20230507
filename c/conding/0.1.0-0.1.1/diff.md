# Comparing `tmp/conding-0.1.0.tar.gz` & `tmp/conding-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conding-0.1.0.tar", last modified: Sun May  7 18:02:48 2023, max compression
+gzip compressed data, was "conding-0.1.1.tar", last modified: Sun May  7 18:12:21 2023, max compression
```

## Comparing `conding-0.1.0.tar` & `conding-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:02:48.398576 conding-0.1.0/
--rw-rw-r--   0 ygg       (1000) ygg       (1000)    11337 2023-01-20 02:50:04.000000 conding-0.1.0/LICENSE
--rw-rw-r--   0 ygg       (1000) ygg       (1000)      111 2023-01-20 02:50:04.000000 conding-0.1.0/MANIFEST.in
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     6612 2023-05-07 18:02:48.398576 conding-0.1.0/PKG-INFO
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     5713 2023-05-03 21:26:11.000000 conding-0.1.0/README.md
-drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:02:48.398576 conding-0.1.0/conding/
--rw-rw-r--   0 ygg       (1000) ygg       (1000)       22 2023-05-07 17:51:06.000000 conding-0.1.0/conding/__init__.py
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     9858 2023-05-07 17:51:06.000000 conding-0.1.0/conding/_modidx.py
-drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:02:48.398576 conding-0.1.0/conding/dune/
--rw-rw-r--   0 ygg       (1000) ygg       (1000)        0 2023-05-07 17:51:06.000000 conding-0.1.0/conding/dune/__init__.py
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     1299 2023-05-07 17:51:05.000000 conding-0.1.0/conding/dune/dune.py
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     6323 2023-05-07 17:51:06.000000 conding-0.1.0/conding/dune/tec.py
-drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:02:48.398576 conding-0.1.0/conding/pamm/
--rw-rw-r--   0 ygg       (1000) ygg       (1000)        0 2023-05-07 17:51:06.000000 conding-0.1.0/conding/pamm/__init__.py
--rw-rw-r--   0 ygg       (1000) ygg       (1000)      281 2023-05-07 17:51:05.000000 conding-0.1.0/conding/pamm/abc.py
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     6442 2023-05-07 17:51:05.000000 conding-0.1.0/conding/pamm/bancor.py
-drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:02:48.398576 conding-0.1.0/conding/samm/
--rw-rw-r--   0 ygg       (1000) ygg       (1000)        0 2023-05-07 17:51:06.000000 conding-0.1.0/conding/samm/__init__.py
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     4643 2023-05-07 17:51:06.000000 conding-0.1.0/conding/samm/uniswap.py
-drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:02:48.398576 conding-0.1.0/conding.egg-info/
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     6612 2023-05-07 18:02:48.000000 conding-0.1.0/conding.egg-info/PKG-INFO
--rw-rw-r--   0 ygg       (1000) ygg       (1000)      506 2023-05-07 18:02:48.000000 conding-0.1.0/conding.egg-info/SOURCES.txt
--rw-rw-r--   0 ygg       (1000) ygg       (1000)        1 2023-05-07 18:02:48.000000 conding-0.1.0/conding.egg-info/dependency_links.txt
--rw-rw-r--   0 ygg       (1000) ygg       (1000)       36 2023-05-07 18:02:48.000000 conding-0.1.0/conding.egg-info/entry_points.txt
--rw-rw-r--   0 ygg       (1000) ygg       (1000)        1 2023-05-07 18:01:48.000000 conding-0.1.0/conding.egg-info/not-zip-safe
--rw-rw-r--   0 ygg       (1000) ygg       (1000)        7 2023-05-07 18:02:48.000000 conding-0.1.0/conding.egg-info/requires.txt
--rw-rw-r--   0 ygg       (1000) ygg       (1000)        8 2023-05-07 18:02:48.000000 conding-0.1.0/conding.egg-info/top_level.txt
--rw-rw-r--   0 ygg       (1000) ygg       (1000)      614 2023-05-03 17:32:51.000000 conding-0.1.0/pyproject.toml
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     1081 2023-04-28 02:05:55.000000 conding-0.1.0/settings.ini
--rw-rw-r--   0 ygg       (1000) ygg       (1000)       38 2023-05-07 18:02:48.398576 conding-0.1.0/setup.cfg
--rw-rw-r--   0 ygg       (1000) ygg       (1000)     2560 2023-01-20 02:50:04.000000 conding-0.1.0/setup.py
+drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:12:21.222194 conding-0.1.1/
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)    11337 2023-01-20 02:50:04.000000 conding-0.1.1/LICENSE
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)      111 2023-01-20 02:50:04.000000 conding-0.1.1/MANIFEST.in
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     6612 2023-05-07 18:12:21.222194 conding-0.1.1/PKG-INFO
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     5713 2023-05-03 21:26:11.000000 conding-0.1.1/README.md
+drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:12:21.218194 conding-0.1.1/conding/
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)       22 2023-05-07 17:51:06.000000 conding-0.1.1/conding/__init__.py
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     9858 2023-05-07 17:51:06.000000 conding-0.1.1/conding/_modidx.py
+drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:12:21.222194 conding-0.1.1/conding/dune/
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)        0 2023-05-07 17:51:06.000000 conding-0.1.1/conding/dune/__init__.py
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     1299 2023-05-07 17:51:05.000000 conding-0.1.1/conding/dune/dune.py
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     6323 2023-05-07 17:51:06.000000 conding-0.1.1/conding/dune/tec.py
+drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:12:21.222194 conding-0.1.1/conding/pamm/
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)        0 2023-05-07 17:51:06.000000 conding-0.1.1/conding/pamm/__init__.py
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)      281 2023-05-07 17:51:05.000000 conding-0.1.1/conding/pamm/abc.py
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     6442 2023-05-07 17:51:05.000000 conding-0.1.1/conding/pamm/bancor.py
+drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:12:21.222194 conding-0.1.1/conding/samm/
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)        0 2023-05-07 17:51:06.000000 conding-0.1.1/conding/samm/__init__.py
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     4643 2023-05-07 17:51:06.000000 conding-0.1.1/conding/samm/uniswap.py
+drwxrwxr-x   0 ygg       (1000) ygg       (1000)        0 2023-05-07 18:12:21.222194 conding-0.1.1/conding.egg-info/
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     6612 2023-05-07 18:12:21.000000 conding-0.1.1/conding.egg-info/PKG-INFO
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)      506 2023-05-07 18:12:21.000000 conding-0.1.1/conding.egg-info/SOURCES.txt
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)        1 2023-05-07 18:12:21.000000 conding-0.1.1/conding.egg-info/dependency_links.txt
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)       36 2023-05-07 18:12:21.000000 conding-0.1.1/conding.egg-info/entry_points.txt
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)        1 2023-05-07 18:01:48.000000 conding-0.1.1/conding.egg-info/not-zip-safe
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)      190 2023-05-07 18:12:21.000000 conding-0.1.1/conding.egg-info/requires.txt
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)        8 2023-05-07 18:12:21.000000 conding-0.1.1/conding.egg-info/top_level.txt
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)      614 2023-05-03 17:32:51.000000 conding-0.1.1/pyproject.toml
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     1243 2023-05-07 18:11:56.000000 conding-0.1.1/settings.ini
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)       38 2023-05-07 18:12:21.222194 conding-0.1.1/setup.cfg
+-rw-rw-r--   0 ygg       (1000) ygg       (1000)     2560 2023-01-20 02:50:04.000000 conding-0.1.1/setup.py
```

### Comparing `conding-0.1.0/LICENSE` & `conding-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `conding-0.1.0/PKG-INFO` & `conding-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conding
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for analysing and modelling bonding curves. This library is managed using nbdev with application development in python param panel.
 Home-page: https://github.com/bonding-curves/conding
 Author: Shawn Anderson
 Author-email: shawn@longtailfinancial.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: conding Version: 0.1.0 Summary: Python library for
+Metadata-Version: 2.1 Name: conding Version: 0.1.1 Summary: Python library for
 analysing and modelling bonding curves. This library is managed using nbdev
 with application development in python param panel. Home-page: https://
 github.com/bonding-curves/conding Author: Shawn Anderson Author-email:
 shawn@longtailfinancial.com License: Apache Software License 2.0 Keywords:
 nbdev jupyter notebook python Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Natural Language ::
 English Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `conding-0.1.0/README.md` & `conding-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `conding-0.1.0/conding/_modidx.py` & `conding-0.1.1/conding/_modidx.py`

 * *Files identical despite different names*

### Comparing `conding-0.1.0/conding/dune/dune.py` & `conding-0.1.1/conding/dune/dune.py`

 * *Files identical despite different names*

### Comparing `conding-0.1.0/conding/dune/tec.py` & `conding-0.1.1/conding/dune/tec.py`

 * *Files identical despite different names*

### Comparing `conding-0.1.0/conding/pamm/bancor.py` & `conding-0.1.1/conding/pamm/bancor.py`

 * *Files identical despite different names*

### Comparing `conding-0.1.0/conding/samm/uniswap.py` & `conding-0.1.1/conding/samm/uniswap.py`

 * *Files identical despite different names*

### Comparing `conding-0.1.0/conding.egg-info/PKG-INFO` & `conding-0.1.1/conding.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conding
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for analysing and modelling bonding curves. This library is managed using nbdev with application development in python param panel.
 Home-page: https://github.com/bonding-curves/conding
 Author: Shawn Anderson
 Author-email: shawn@longtailfinancial.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: conding Version: 0.1.0 Summary: Python library for
+Metadata-Version: 2.1 Name: conding Version: 0.1.1 Summary: Python library for
 analysing and modelling bonding curves. This library is managed using nbdev
 with application development in python param panel. Home-page: https://
 github.com/bonding-curves/conding Author: Shawn Anderson Author-email:
 shawn@longtailfinancial.com License: Apache Software License 2.0 Keywords:
 nbdev jupyter notebook python Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Natural Language ::
 English Classifier: Programming Language :: Python :: 3.7 Classifier:
```

### Comparing `conding-0.1.0/pyproject.toml` & `conding-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `conding-0.1.0/settings.ini` & `conding-0.1.1/settings.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = conding
 lib_name = %(repo)s
-version = 0.1.0
+version = 0.1.1
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = conding
@@ -34,10 +34,10 @@
 description = Python library for analysing and modelling bonding curves. This library is managed using nbdev with application development in python param panel.
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = bonding-curves
 
 ### Optional ###
-# requirements = fastcore pandas
-# dev_requirements = 
+requirements = pandas>=1.5.3 hvplot>=0.8.3 python-dotenv>=1.0.0 dune-client>=1.0.0 diskcache>=5.6.1 pyparsing>=3.0.9 yfinance>=0.2.18
+dev_requirements = nbdev>=2.3.12 jupyterlab==3.6.0 ipython>=8.12.0 icecream>=2.1.3
 # console_scripts =
```

### Comparing `conding-0.1.0/setup.py` & `conding-0.1.1/setup.py`

 * *Files identical despite different names*

