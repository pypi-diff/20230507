# Comparing `tmp/betanegbinfit-1.9.1.tar.gz` & `tmp/betanegbinfit-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betanegbinfit-1.9.1.tar", last modified: Sat May  6 13:26:08 2023, max compression
+gzip compressed data, was "betanegbinfit-1.9.2.tar", last modified: Sun May  7 14:57:58 2023, max compression
```

## Comparing `betanegbinfit-1.9.1.tar` & `betanegbinfit-1.9.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-06 13:26:08.419722 betanegbinfit-1.9.1/
--rw-r--r--   0 georgy    (1000) georgy    (1001)     4108 2023-05-06 13:26:08.419722 betanegbinfit-1.9.1/PKG-INFO
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3534 2022-01-12 15:51:26.000000 betanegbinfit-1.9.1/README.md
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-06 13:26:08.416389 betanegbinfit-1.9.1/betanegbinfit/
--rw-r--r--   0 georgy    (1000) georgy    (1001)      725 2023-05-06 13:25:32.000000 betanegbinfit-1.9.1/betanegbinfit/__init__.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14720 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/betacdnb.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     2534 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/betainc.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     5146 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/bridge_mixalime.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     6146 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/cdnb.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     5148 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/combine.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14940 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/create.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    38370 2023-05-06 13:24:10.000000 betanegbinfit-1.9.1/betanegbinfit/distributions.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3125 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/hyp.py
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-06 13:26:08.419722 betanegbinfit-1.9.1/betanegbinfit/models/
--rw-r--r--   0 georgy    (1000) georgy    (1001)      258 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/models/__init__.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    15251 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/models/model.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    22116 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/models/model_line.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3341 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/models/model_line_lrt.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14364 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/models/model_mixture.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     8477 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/models/model_mixtures.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    29845 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/models/model_window.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    13557 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/plot.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14689 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/stats.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     6960 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/tests.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    29604 2023-04-24 17:33:25.000000 betanegbinfit-1.9.1/betanegbinfit/utils.py
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-06 13:26:08.419722 betanegbinfit-1.9.1/betanegbinfit.egg-info/
--rw-r--r--   0 georgy    (1000) georgy    (1001)     4108 2023-05-06 13:26:08.000000 betanegbinfit-1.9.1/betanegbinfit.egg-info/PKG-INFO
--rw-r--r--   0 georgy    (1000) georgy    (1001)      777 2023-05-06 13:26:08.000000 betanegbinfit-1.9.1/betanegbinfit.egg-info/SOURCES.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)        1 2023-05-06 13:26:08.000000 betanegbinfit-1.9.1/betanegbinfit.egg-info/dependency_links.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       43 2023-05-06 13:26:08.000000 betanegbinfit-1.9.1/betanegbinfit.egg-info/requires.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       14 2023-05-06 13:26:08.000000 betanegbinfit-1.9.1/betanegbinfit.egg-info/top_level.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       38 2023-05-06 13:26:08.419722 betanegbinfit-1.9.1/setup.cfg
--rw-r--r--   0 georgy    (1000) georgy    (1001)      963 2023-04-16 06:18:26.000000 betanegbinfit-1.9.1/setup.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-07 14:57:58.628431 betanegbinfit-1.9.2/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     4054 2023-05-07 14:57:58.628431 betanegbinfit-1.9.2/PKG-INFO
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3534 2022-01-12 15:51:26.000000 betanegbinfit-1.9.2/README.md
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-07 14:57:58.625098 betanegbinfit-1.9.2/betanegbinfit/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      725 2023-05-07 14:57:11.000000 betanegbinfit-1.9.2/betanegbinfit/__init__.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14720 2023-04-24 17:33:25.000000 betanegbinfit-1.9.2/betanegbinfit/betacdnb.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     2534 2023-04-24 17:33:25.000000 betanegbinfit-1.9.2/betanegbinfit/betainc.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     5146 2023-04-24 17:33:25.000000 betanegbinfit-1.9.2/betanegbinfit/bridge_mixalime.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     6178 2023-05-07 14:27:30.000000 betanegbinfit-1.9.2/betanegbinfit/cdnb.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     5148 2023-04-24 17:33:25.000000 betanegbinfit-1.9.2/betanegbinfit/combine.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14940 2023-04-24 17:33:25.000000 betanegbinfit-1.9.2/betanegbinfit/create.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    38370 2023-05-07 14:29:31.000000 betanegbinfit-1.9.2/betanegbinfit/distributions.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3125 2023-04-24 17:33:25.000000 betanegbinfit-1.9.2/betanegbinfit/hyp.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-07 14:57:58.628431 betanegbinfit-1.9.2/betanegbinfit/models/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      258 2023-04-24 17:33:25.000000 betanegbinfit-1.9.2/betanegbinfit/models/__init__.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    15251 2023-04-24 17:33:25.000000 betanegbinfit-1.9.2/betanegbinfit/models/model.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    22116 2023-04-24 17:33:25.000000 betanegbinfit-1.9.2/betanegbinfit/models/model_line.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3341 2023-04-24 17:33:25.000000 betanegbinfit-1.9.2/betanegbinfit/models/model_line_lrt.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14364 2023-04-24 17:33:25.000000 betanegbinfit-1.9.2/betanegbinfit/models/model_mixture.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     8477 2023-04-24 17:33:25.000000 betanegbinfit-1.9.2/betanegbinfit/models/model_mixtures.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    29845 2023-04-24 17:33:25.000000 betanegbinfit-1.9.2/betanegbinfit/models/model_window.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    13557 2023-04-24 17:33:25.000000 betanegbinfit-1.9.2/betanegbinfit/plot.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14689 2023-04-24 17:33:25.000000 betanegbinfit-1.9.2/betanegbinfit/stats.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     6960 2023-04-24 17:33:25.000000 betanegbinfit-1.9.2/betanegbinfit/tests.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    29604 2023-04-24 17:33:25.000000 betanegbinfit-1.9.2/betanegbinfit/utils.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-05-07 14:57:58.628431 betanegbinfit-1.9.2/betanegbinfit.egg-info/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     4054 2023-05-07 14:57:58.000000 betanegbinfit-1.9.2/betanegbinfit.egg-info/PKG-INFO
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      777 2023-05-07 14:57:58.000000 betanegbinfit-1.9.2/betanegbinfit.egg-info/SOURCES.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)        1 2023-05-07 14:57:58.000000 betanegbinfit-1.9.2/betanegbinfit.egg-info/dependency_links.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       43 2023-05-07 14:57:58.000000 betanegbinfit-1.9.2/betanegbinfit.egg-info/requires.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       14 2023-05-07 14:57:58.000000 betanegbinfit-1.9.2/betanegbinfit.egg-info/top_level.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       38 2023-05-07 14:57:58.628431 betanegbinfit-1.9.2/setup.cfg
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      963 2023-04-16 06:18:26.000000 betanegbinfit-1.9.2/setup.py
```

### Comparing `betanegbinfit-1.9.1/PKG-INFO` & `betanegbinfit-1.9.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 Metadata-Version: 2.1
 Name: betanegbinfit
-Version: 1.9.1
-Summary: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
+Version: 1.9.2
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
@@ -75,9 +72,7 @@
 
 
 **Please note, that all functions have plenty of optional arguments and they all are documented, so please consider reading through `help(function of interest)`.**
 
 
 ### A note on performance
 As far as we are concerned, **BetaNegBinFit** should work within a manageable amounts of time. For insance, when `ModelLine` with `model='BetaNB'` ran against *chipseq.tsv* dataset, it finishes in 6 minutes when ran at Ryzen 5600U. It does so under 2 minutes with `model='NB'`.
-
-
```

### Comparing `betanegbinfit-1.9.1/README.md` & `betanegbinfit-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/betanegbinfit/__init__.py` & `betanegbinfit-1.9.2/betanegbinfit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.9.1'
+__version__ = '1.9.2'
 
 import warnings
 # This will omit annoying FutureWarnings by JAX and RutimeWarnings caused by
 # estimates being clipped at bounds.
 warnings.simplefilter(action='ignore', category=FutureWarning)
 warnings.simplefilter(action='ignore', category=RuntimeWarning)
```

### Comparing `betanegbinfit-1.9.1/betanegbinfit/betacdnb.py` & `betanegbinfit-1.9.2/betanegbinfit/betacdnb.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/betanegbinfit/betainc.py` & `betanegbinfit-1.9.2/betanegbinfit/betainc.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/betanegbinfit/bridge_mixalime.py` & `betanegbinfit-1.9.2/betanegbinfit/bridge_mixalime.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/betanegbinfit/cdnb.py` & `betanegbinfit-1.9.2/betanegbinfit/cdnb.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,16 @@
         term /= 2.0 ** exp
         mult += exp
         last_pos = cond(res >= 0, lambda: res, lambda: last_pos)
         return last_pos, res, prev_res, mult, term, i + 1
     
     def cond_iter(carry):
         res, prev_res = carry[1:3]
-        return (prev_res != res)
+        i = carry[-1]
+        return (prev_res != res) & (i < x)
     term = 1.0
     res = 1.0
     mult = jnp.log(n) + jnp.log1p(-p) * 2 + jnp.log(p) * (n + x - 1) - jnp.log1p(-p ** n)
     carry = while_loop(cond_iter, sum_iter, (res, res, 0, 0, term, 1))
     return jnp.log(carry[0]) + mult + carry[3] * jnp.log(2) + pfaff
```

### Comparing `betanegbinfit-1.9.1/betanegbinfit/combine.py` & `betanegbinfit-1.9.2/betanegbinfit/combine.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/betanegbinfit/create.py` & `betanegbinfit-1.9.2/betanegbinfit/create.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/betanegbinfit/distributions.py` & `betanegbinfit-1.9.2/betanegbinfit/distributions.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/betanegbinfit/hyp.py` & `betanegbinfit-1.9.2/betanegbinfit/hyp.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/betanegbinfit/models/model.py` & `betanegbinfit-1.9.2/betanegbinfit/models/model.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/betanegbinfit/models/model_line.py` & `betanegbinfit-1.9.2/betanegbinfit/models/model_line.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/betanegbinfit/models/model_line_lrt.py` & `betanegbinfit-1.9.2/betanegbinfit/models/model_line_lrt.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/betanegbinfit/models/model_mixture.py` & `betanegbinfit-1.9.2/betanegbinfit/models/model_mixture.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/betanegbinfit/models/model_mixtures.py` & `betanegbinfit-1.9.2/betanegbinfit/models/model_mixtures.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/betanegbinfit/models/model_window.py` & `betanegbinfit-1.9.2/betanegbinfit/models/model_window.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/betanegbinfit/plot.py` & `betanegbinfit-1.9.2/betanegbinfit/plot.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/betanegbinfit/stats.py` & `betanegbinfit-1.9.2/betanegbinfit/stats.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/betanegbinfit/tests.py` & `betanegbinfit-1.9.2/betanegbinfit/tests.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/betanegbinfit/utils.py` & `betanegbinfit-1.9.2/betanegbinfit/utils.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/betanegbinfit.egg-info/PKG-INFO` & `betanegbinfit-1.9.2/betanegbinfit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 Metadata-Version: 2.1
 Name: betanegbinfit
-Version: 1.9.1
-Summary: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
+Version: 1.9.2
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
@@ -75,9 +72,7 @@
 
 
 **Please note, that all functions have plenty of optional arguments and they all are documented, so please consider reading through `help(function of interest)`.**
 
 
 ### A note on performance
 As far as we are concerned, **BetaNegBinFit** should work within a manageable amounts of time. For insance, when `ModelLine` with `model='BetaNB'` ran against *chipseq.tsv* dataset, it finishes in 6 minutes when ran at Ryzen 5600U. It does so under 2 minutes with `model='NB'`.
-
-
```

### Comparing `betanegbinfit-1.9.1/betanegbinfit.egg-info/SOURCES.txt` & `betanegbinfit-1.9.2/betanegbinfit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.9.1/setup.py` & `betanegbinfit-1.9.2/setup.py`

 * *Files identical despite different names*

