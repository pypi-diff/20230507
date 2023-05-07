# Comparing `tmp/qtex-0.0.5.tar.gz` & `tmp/qtex-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtex-0.0.5.tar", last modified: Sun May  7 02:20:18 2023, max compression
+gzip compressed data, was "qtex-0.0.6.tar", last modified: Sun May  7 02:32:21 2023, max compression
```

## Comparing `qtex-0.0.5.tar` & `qtex-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:20:18.117449 qtex-0.0.5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 02:03:44.000000 qtex-0.0.5/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2023-05-07 02:20:18.117449 qtex-0.0.5/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:20:18.113449 qtex-0.0.5/qtex/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:19:14.000000 qtex-0.0.5/qtex/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:20:18.117449 qtex-0.0.5/qtex/app/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 03:52:06.000000 qtex-0.0.5/qtex/app/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9965 2023-05-04 04:14:21.000000 qtex-0.0.5/qtex/app/persist_universe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      374 2023-04-28 21:57:05.000000 qtex-0.0.5/qtex/env_config.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:20:18.117449 qtex-0.0.5/qtex/jq/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:19:37.000000 qtex-0.0.5/qtex/jq/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:20:18.117449 qtex-0.0.5/qtex/jq/etl/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:54:50.000000 qtex-0.0.5/qtex/jq/etl/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4462 2023-05-07 01:58:29.000000 qtex-0.0.5/qtex/jq/etl/factor_info.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6254 2023-05-07 02:16:55.000000 qtex-0.0.5/qtex/jq/etl/factor_values.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1899 2023-05-02 01:56:55.000000 qtex-0.0.5/qtex/jq/persist_ext.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:20:18.117449 qtex-0.0.5/qtex/jq/sync/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:58:58.000000 qtex-0.0.5/qtex/jq/sync/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1224 2023-05-06 02:37:06.000000 qtex-0.0.5/qtex/jq/sync/position.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1928 2023-05-04 00:04:51.000000 qtex-0.0.5/qtex/jq/univ.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2849 2023-05-07 01:58:58.000000 qtex-0.0.5/qtex/jq/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-05-07 02:20:02.000000 qtex-0.0.5/qtex/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:20:18.117449 qtex-0.0.5/qtex.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2023-05-07 02:20:18.000000 qtex-0.0.5/qtex.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      494 2023-05-07 02:20:18.000000 qtex-0.0.5/qtex.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-07 02:20:18.000000 qtex-0.0.5/qtex.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-02 02:06:42.000000 qtex-0.0.5/qtex.egg-info/not-zip-safe
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       60 2023-05-07 02:20:18.000000 qtex-0.0.5/qtex.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-05-07 02:20:18.000000 qtex-0.0.5/qtex.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-07 02:20:18.117449 qtex-0.0.5/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      698 2023-05-02 02:07:22.000000 qtex-0.0.5/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:32:21.785534 qtex-0.0.6/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 02:03:44.000000 qtex-0.0.6/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2023-05-07 02:32:21.785534 qtex-0.0.6/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:32:21.781533 qtex-0.0.6/qtex/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:19:14.000000 qtex-0.0.6/qtex/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:32:21.781533 qtex-0.0.6/qtex/app/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-04 03:52:06.000000 qtex-0.0.6/qtex/app/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9965 2023-05-04 04:14:21.000000 qtex-0.0.6/qtex/app/persist_universe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      374 2023-04-28 21:57:05.000000 qtex-0.0.6/qtex/env_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:32:21.785534 qtex-0.0.6/qtex/jq/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:19:37.000000 qtex-0.0.6/qtex/jq/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:32:21.785534 qtex-0.0.6/qtex/jq/etl/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:54:50.000000 qtex-0.0.6/qtex/jq/etl/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4462 2023-05-07 01:58:29.000000 qtex-0.0.6/qtex/jq/etl/factor_info.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6259 2023-05-07 02:32:06.000000 qtex-0.0.6/qtex/jq/etl/factor_values.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1899 2023-05-02 01:56:55.000000 qtex-0.0.6/qtex/jq/persist_ext.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:32:21.785534 qtex-0.0.6/qtex/jq/sync/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-02 01:58:58.000000 qtex-0.0.6/qtex/jq/sync/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1224 2023-05-06 02:37:06.000000 qtex-0.0.6/qtex/jq/sync/position.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1928 2023-05-04 00:04:51.000000 qtex-0.0.6/qtex/jq/univ.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2849 2023-05-07 01:58:58.000000 qtex-0.0.6/qtex/jq/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2023-05-07 02:32:16.000000 qtex-0.0.6/qtex/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-07 02:32:21.781533 qtex-0.0.6/qtex.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      151 2023-05-07 02:32:21.000000 qtex-0.0.6/qtex.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      494 2023-05-07 02:32:21.000000 qtex-0.0.6/qtex.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-07 02:32:21.000000 qtex-0.0.6/qtex.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-02 02:06:42.000000 qtex-0.0.6/qtex.egg-info/not-zip-safe
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       60 2023-05-07 02:32:21.000000 qtex-0.0.6/qtex.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-05-07 02:32:21.000000 qtex-0.0.6/qtex.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-07 02:32:21.785534 qtex-0.0.6/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      698 2023-05-02 02:07:22.000000 qtex-0.0.6/setup.py
```

### Comparing `qtex-0.0.5/qtex/app/persist_universe.py` & `qtex-0.0.6/qtex/app/persist_universe.py`

 * *Files identical despite different names*

### Comparing `qtex-0.0.5/qtex/jq/etl/factor_info.py` & `qtex-0.0.6/qtex/jq/etl/factor_info.py`

 * *Files identical despite different names*

### Comparing `qtex-0.0.5/qtex/jq/etl/factor_values.py` & `qtex-0.0.6/qtex/jq/etl/factor_values.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         N = len(factor_names)
         logger.info(f'=== Processing category={category} with #factors={N} ===')
         batch_idx = 0
         while True:
             start_idx = batch_idx * batch_size
             end_idx = min((batch_idx + 1) * batch_size, N)
             if N > batch_size:
-                logger(f'Processing ibatch={batch_idx}, start_idx={start_idx}, end_idx={end_idx}')
+                logger.info(f'Processing ibatch={batch_idx}, start_idx={start_idx}, end_idx={end_idx}')
 
             fd = jqu.load_factor_scores(
                 jq_codes=securities,
                 factors=factor_names[start_idx:end_idx],
                 start_date=datestr, end_date=datestr
             ).T.stack()
```

### Comparing `qtex-0.0.5/qtex/jq/persist_ext.py` & `qtex-0.0.6/qtex/jq/persist_ext.py`

 * *Files identical despite different names*

### Comparing `qtex-0.0.5/qtex/jq/sync/position.py` & `qtex-0.0.6/qtex/jq/sync/position.py`

 * *Files identical despite different names*

### Comparing `qtex-0.0.5/qtex/jq/univ.py` & `qtex-0.0.6/qtex/jq/univ.py`

 * *Files identical despite different names*

### Comparing `qtex-0.0.5/qtex/jq/utils.py` & `qtex-0.0.6/qtex/jq/utils.py`

 * *Files identical despite different names*

### Comparing `qtex-0.0.5/setup.py` & `qtex-0.0.6/setup.py`

 * *Files identical despite different names*

