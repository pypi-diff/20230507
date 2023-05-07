# Comparing `tmp/mysqlcipher-0.1.2.tar.gz` & `tmp/mysqlcipher-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysqlcipher-0.1.2.tar", last modified: Sun May  7 16:25:03 2023, max compression
+gzip compressed data, was "mysqlcipher-0.1.3.tar", last modified: Sun May  7 18:17:13 2023, max compression
```

## Comparing `mysqlcipher-0.1.2.tar` & `mysqlcipher-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jo-project  (1000) jo-project  (1000)        0 2023-05-07 16:25:03.701385 mysqlcipher-0.1.2/
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)    26526 2023-05-07 12:43:59.000000 mysqlcipher-0.1.2/LICENSE
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)      780 2023-05-07 16:25:03.701385 mysqlcipher-0.1.2/PKG-INFO
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)       13 2023-05-07 12:43:59.000000 mysqlcipher-0.1.2/README.md
-drwxr-xr-x   0 jo-project  (1000) jo-project  (1000)        0 2023-05-07 16:25:03.701385 mysqlcipher-0.1.2/mysqlcipher/
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)     1021 2023-05-07 16:24:43.000000 mysqlcipher-0.1.2/mysqlcipher/__init__.py
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)     2728 2023-05-07 12:55:23.000000 mysqlcipher-0.1.2/mysqlcipher/dbapi2.py
-drwxr-xr-x   0 jo-project  (1000) jo-project  (1000)        0 2023-05-07 16:25:03.701385 mysqlcipher-0.1.2/mysqlcipher.egg-info/
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)      780 2023-05-07 16:25:03.000000 mysqlcipher-0.1.2/mysqlcipher.egg-info/PKG-INFO
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)      384 2023-05-07 16:25:03.000000 mysqlcipher-0.1.2/mysqlcipher.egg-info/SOURCES.txt
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)        1 2023-05-07 16:25:03.000000 mysqlcipher-0.1.2/mysqlcipher.egg-info/dependency_links.txt
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)       12 2023-05-07 16:25:03.000000 mysqlcipher-0.1.2/mysqlcipher.egg-info/top_level.txt
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)      274 2023-05-07 16:24:26.000000 mysqlcipher-0.1.2/pyproject.toml
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)      103 2023-05-07 16:25:03.701385 mysqlcipher-0.1.2/setup.cfg
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)     6450 2023-05-07 16:24:21.000000 mysqlcipher-0.1.2/setup.py
-drwxr-xr-x   0 jo-project  (1000) jo-project  (1000)        0 2023-05-07 16:25:03.701385 mysqlcipher-0.1.2/src/
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)    17810 2021-05-14 15:12:50.000000 mysqlcipher-0.1.2/src/blob.c
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)    12679 2020-11-08 02:22:30.000000 mysqlcipher-0.1.2/src/cache.c
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)    61784 2022-09-21 18:11:46.000000 mysqlcipher-0.1.2/src/connection.c
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)    29823 2021-08-06 23:58:58.000000 mysqlcipher-0.1.2/src/cursor.c
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)     4551 2019-06-03 15:14:16.000000 mysqlcipher-0.1.2/src/microprotocols.c
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)    18325 2021-08-23 15:49:08.000000 mysqlcipher-0.1.2/src/module.c
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)     4363 2022-09-21 18:11:46.000000 mysqlcipher-0.1.2/src/prepare_protocol.c
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)     9515 2019-09-28 13:31:34.000000 mysqlcipher-0.1.2/src/row.c
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)    17339 2019-07-23 18:05:14.000000 mysqlcipher-0.1.2/src/statement.c
--rw-r--r--   0 jo-project  (1000) jo-project  (1000)     4812 2021-05-14 15:12:50.000000 mysqlcipher-0.1.2/src/util.c
+drwxr-xr-x   0 jo-project  (1000) jo-project  (1000)        0 2023-05-07 18:17:13.606799 mysqlcipher-0.1.3/
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)    26526 2023-05-07 12:43:59.000000 mysqlcipher-0.1.3/LICENSE
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)      780 2023-05-07 18:17:13.606799 mysqlcipher-0.1.3/PKG-INFO
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)       13 2023-05-07 12:43:59.000000 mysqlcipher-0.1.3/README.md
+drwxr-xr-x   0 jo-project  (1000) jo-project  (1000)        0 2023-05-07 18:17:13.596799 mysqlcipher-0.1.3/mysqlcipher/
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)     1021 2023-05-07 16:24:43.000000 mysqlcipher-0.1.3/mysqlcipher/__init__.py
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)     2728 2023-05-07 12:55:23.000000 mysqlcipher-0.1.3/mysqlcipher/dbapi2.py
+drwxr-xr-x   0 jo-project  (1000) jo-project  (1000)        0 2023-05-07 18:17:13.596799 mysqlcipher-0.1.3/mysqlcipher.egg-info/
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)      780 2023-05-07 18:17:13.000000 mysqlcipher-0.1.3/mysqlcipher.egg-info/PKG-INFO
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)      384 2023-05-07 18:17:13.000000 mysqlcipher-0.1.3/mysqlcipher.egg-info/SOURCES.txt
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)        1 2023-05-07 18:17:13.000000 mysqlcipher-0.1.3/mysqlcipher.egg-info/dependency_links.txt
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)       12 2023-05-07 18:17:13.000000 mysqlcipher-0.1.3/mysqlcipher.egg-info/top_level.txt
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)      274 2023-05-07 18:14:06.000000 mysqlcipher-0.1.3/pyproject.toml
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)      103 2023-05-07 18:17:13.606799 mysqlcipher-0.1.3/setup.cfg
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)     6450 2023-05-07 18:14:12.000000 mysqlcipher-0.1.3/setup.py
+drwxr-xr-x   0 jo-project  (1000) jo-project  (1000)        0 2023-05-07 18:17:13.606799 mysqlcipher-0.1.3/src/
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)    17810 2021-05-14 15:12:50.000000 mysqlcipher-0.1.3/src/blob.c
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)    12679 2020-11-08 02:22:30.000000 mysqlcipher-0.1.3/src/cache.c
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)    61784 2022-09-21 18:11:46.000000 mysqlcipher-0.1.3/src/connection.c
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)    29823 2021-08-06 23:58:58.000000 mysqlcipher-0.1.3/src/cursor.c
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)     4551 2019-06-03 15:14:16.000000 mysqlcipher-0.1.3/src/microprotocols.c
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)    18325 2021-08-23 15:49:08.000000 mysqlcipher-0.1.3/src/module.c
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)     4363 2022-09-21 18:11:46.000000 mysqlcipher-0.1.3/src/prepare_protocol.c
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)     9515 2019-09-28 13:31:34.000000 mysqlcipher-0.1.3/src/row.c
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)    17339 2019-07-23 18:05:14.000000 mysqlcipher-0.1.3/src/statement.c
+-rw-r--r--   0 jo-project  (1000) jo-project  (1000)     4812 2021-05-14 15:12:50.000000 mysqlcipher-0.1.3/src/util.c
```

### Comparing `mysqlcipher-0.1.2/LICENSE` & `mysqlcipher-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlcipher-0.1.2/PKG-INFO` & `mysqlcipher-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlcipher
-Version: 0.1.2
+Version: 0.1.3
 Summary: DB-API 2.0 interface for SQLCipher 4.x
 Home-page: https://github.com/jo-project/mysqlcipher
 Author: jo-project
 Author-email: jo.project.0911@gmail.com
 License: zlib/libpng
 Platform: ALL
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mysqlcipher-0.1.2/mysqlcipher/__init__.py` & `mysqlcipher-0.1.3/mysqlcipher/__init__.py`

 * *Files identical despite different names*

### Comparing `mysqlcipher-0.1.2/mysqlcipher/dbapi2.py` & `mysqlcipher-0.1.3/mysqlcipher/dbapi2.py`

 * *Files identical despite different names*

### Comparing `mysqlcipher-0.1.2/mysqlcipher.egg-info/PKG-INFO` & `mysqlcipher-0.1.3/mysqlcipher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlcipher
-Version: 0.1.2
+Version: 0.1.3
 Summary: DB-API 2.0 interface for SQLCipher 4.x
 Home-page: https://github.com/jo-project/mysqlcipher
 Author: jo-project
 Author-email: jo.project.0911@gmail.com
 License: zlib/libpng
 Platform: ALL
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mysqlcipher-0.1.2/setup.py` & `mysqlcipher-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from distutils import log
 from distutils.command.build_ext import build_ext
 from setuptools import Extension
 
 # If you need to change anything, it should be enough to change setup.cfg.
 
 PACKAGE_NAME = 'mysqlcipher'
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 
 # define sqlite sources
 sources = [os.path.join('src', source)
            for source in ["module.c", "connection.c", "cursor.c", "cache.c",
                           "microprotocols.c", "prepare_protocol.c",
                           "statement.c", "util.c", "row.c", "blob.c"]]
```

### Comparing `mysqlcipher-0.1.2/src/blob.c` & `mysqlcipher-0.1.3/src/blob.c`

 * *Files identical despite different names*

### Comparing `mysqlcipher-0.1.2/src/cache.c` & `mysqlcipher-0.1.3/src/cache.c`

 * *Files identical despite different names*

### Comparing `mysqlcipher-0.1.2/src/connection.c` & `mysqlcipher-0.1.3/src/connection.c`

 * *Files identical despite different names*

### Comparing `mysqlcipher-0.1.2/src/cursor.c` & `mysqlcipher-0.1.3/src/cursor.c`

 * *Files identical despite different names*

### Comparing `mysqlcipher-0.1.2/src/microprotocols.c` & `mysqlcipher-0.1.3/src/microprotocols.c`

 * *Files identical despite different names*

### Comparing `mysqlcipher-0.1.2/src/module.c` & `mysqlcipher-0.1.3/src/module.c`

 * *Files identical despite different names*

### Comparing `mysqlcipher-0.1.2/src/prepare_protocol.c` & `mysqlcipher-0.1.3/src/prepare_protocol.c`

 * *Files identical despite different names*

### Comparing `mysqlcipher-0.1.2/src/row.c` & `mysqlcipher-0.1.3/src/row.c`

 * *Files identical despite different names*

### Comparing `mysqlcipher-0.1.2/src/statement.c` & `mysqlcipher-0.1.3/src/statement.c`

 * *Files identical despite different names*

### Comparing `mysqlcipher-0.1.2/src/util.c` & `mysqlcipher-0.1.3/src/util.c`

 * *Files identical despite different names*

