# Comparing `tmp/pyghostdb-0.0.1.tar.gz` & `tmp/pyghostdb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyghostdb-0.0.1.tar", last modified: Sat May  6 23:23:09 2023, max compression
+gzip compressed data, was "pyghostdb-0.0.2.tar", last modified: Sun May  7 02:20:25 2023, max compression
```

## Comparing `pyghostdb-0.0.1.tar` & `pyghostdb-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-06 23:23:09.420142 pyghostdb-0.0.1/
--rw-r--r--   0 fedorshabashev   (501) staff       (20)      189 2023-05-06 23:23:09.420013 pyghostdb-0.0.1/PKG-INFO
--rw-r--r--   0 fedorshabashev   (501) staff       (20)      783 2023-05-04 00:59:20.000000 pyghostdb-0.0.1/README.md
-drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-06 23:23:09.419045 pyghostdb-0.0.1/pyghostdb/
--rw-r--r--   0 fedorshabashev   (501) staff       (20)        0 2023-05-05 14:29:31.000000 pyghostdb-0.0.1/pyghostdb/__init__.py
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     2000 2023-05-06 23:02:33.000000 pyghostdb-0.0.1/pyghostdb/ghost_storage.py
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     3072 2023-05-03 01:43:38.000000 pyghostdb-0.0.1/pyghostdb/hnswlib_index.py
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     2280 2023-05-06 14:54:30.000000 pyghostdb-0.0.1/pyghostdb/parquet_conversion.py
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     2333 2023-05-05 22:25:22.000000 pyghostdb-0.0.1/pyghostdb/test_hnsw.py
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     2286 2023-05-06 15:04:20.000000 pyghostdb-0.0.1/pyghostdb/text_storage.py
-drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-06 23:23:09.419863 pyghostdb-0.0.1/pyghostdb.egg-info/
--rw-r--r--   0 fedorshabashev   (501) staff       (20)      189 2023-05-06 23:23:09.000000 pyghostdb-0.0.1/pyghostdb.egg-info/PKG-INFO
--rw-r--r--   0 fedorshabashev   (501) staff       (20)      345 2023-05-06 23:23:09.000000 pyghostdb-0.0.1/pyghostdb.egg-info/SOURCES.txt
--rw-r--r--   0 fedorshabashev   (501) staff       (20)        1 2023-05-06 23:23:09.000000 pyghostdb-0.0.1/pyghostdb.egg-info/dependency_links.txt
--rw-r--r--   0 fedorshabashev   (501) staff       (20)       70 2023-05-06 23:23:09.000000 pyghostdb-0.0.1/pyghostdb.egg-info/requires.txt
--rw-r--r--   0 fedorshabashev   (501) staff       (20)       10 2023-05-06 23:23:09.000000 pyghostdb-0.0.1/pyghostdb.egg-info/top_level.txt
--rw-r--r--   0 fedorshabashev   (501) staff       (20)      363 2023-05-06 23:22:11.000000 pyghostdb-0.0.1/pyproject.toml
--rw-r--r--   0 fedorshabashev   (501) staff       (20)       38 2023-05-06 23:23:09.420177 pyghostdb-0.0.1/setup.cfg
+drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-07 02:20:25.262378 pyghostdb-0.0.2/
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      189 2023-05-07 02:20:25.262222 pyghostdb-0.0.2/PKG-INFO
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      783 2023-05-04 00:59:20.000000 pyghostdb-0.0.2/README.md
+drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-07 02:20:25.261305 pyghostdb-0.0.2/pyghostdb/
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)        0 2023-05-05 14:29:31.000000 pyghostdb-0.0.2/pyghostdb/__init__.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     2000 2023-05-06 23:02:33.000000 pyghostdb-0.0.2/pyghostdb/ghost_storage.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     3068 2023-05-07 00:07:50.000000 pyghostdb-0.0.2/pyghostdb/hnswlib_index.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     2280 2023-05-06 14:54:30.000000 pyghostdb-0.0.2/pyghostdb/parquet_conversion.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     2332 2023-05-07 00:07:50.000000 pyghostdb-0.0.2/pyghostdb/test_hnsw.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     2283 2023-05-07 00:07:14.000000 pyghostdb-0.0.2/pyghostdb/text_storage.py
+drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-07 02:20:25.262082 pyghostdb-0.0.2/pyghostdb.egg-info/
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      189 2023-05-07 02:20:25.000000 pyghostdb-0.0.2/pyghostdb.egg-info/PKG-INFO
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      345 2023-05-07 02:20:25.000000 pyghostdb-0.0.2/pyghostdb.egg-info/SOURCES.txt
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)        1 2023-05-07 02:20:25.000000 pyghostdb-0.0.2/pyghostdb.egg-info/dependency_links.txt
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)       58 2023-05-07 02:20:25.000000 pyghostdb-0.0.2/pyghostdb.egg-info/requires.txt
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)       10 2023-05-07 02:20:25.000000 pyghostdb-0.0.2/pyghostdb.egg-info/top_level.txt
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      347 2023-05-07 02:19:53.000000 pyghostdb-0.0.2/pyproject.toml
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)       38 2023-05-07 02:20:25.262492 pyghostdb-0.0.2/setup.cfg
```

### Comparing `pyghostdb-0.0.1/README.md` & `pyghostdb-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyghostdb-0.0.1/pyghostdb/ghost_storage.py` & `pyghostdb-0.0.2/pyghostdb/ghost_storage.py`

 * *Files identical despite different names*

### Comparing `pyghostdb-0.0.1/pyghostdb/hnswlib_index.py` & `pyghostdb-0.0.2/pyghostdb/hnswlib_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,11 +68,7 @@
         self.index.save_index(path)
 
     def load_from_file(self, path):
         """
         Load the index from disk
         """
         self.index.load_index(path)
-
-
-
-
```

### Comparing `pyghostdb-0.0.1/pyghostdb/parquet_conversion.py` & `pyghostdb-0.0.2/pyghostdb/parquet_conversion.py`

 * *Files identical despite different names*

### Comparing `pyghostdb-0.0.1/pyghostdb/test_hnsw.py` & `pyghostdb-0.0.2/pyghostdb/test_hnsw.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,8 +61,7 @@
 
 if __name__ == '__main__':
     test_hnsw()
     test_small_vectors2()
     test_text_storage()
     test_ghostdb()
     test_add_multiple()
-
```

### Comparing `pyghostdb-0.0.1/pyghostdb/text_storage.py` & `pyghostdb-0.0.2/pyghostdb/text_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,10 +61,7 @@
         cursor.execute("SELECT id_, text, embedding FROM vectors WHERE id_ = ?", (id_,))
         id_, text, vector_data = cursor.fetchone()
 
         return id_, text, vector_data
 
     def remove_db(self):
         os.remove(self.db_path)
-
-
-
```

