# Comparing `tmp/pyghostdb-0.0.0.tar.gz` & `tmp/pyghostdb-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyghostdb-0.0.0.tar", last modified: Thu May  4 02:33:00 2023, max compression
+gzip compressed data, was "pyghostdb-0.0.1.tar", last modified: Sat May  6 23:23:09 2023, max compression
```

## Comparing `pyghostdb-0.0.0.tar` & `pyghostdb-0.0.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-04 02:33:00.002790 pyghostdb-0.0.0/
--rw-r--r--   0 fedorshabashev   (501) staff       (20)       53 2023-05-04 02:33:00.002653 pyghostdb-0.0.0/PKG-INFO
--rw-r--r--   0 fedorshabashev   (501) staff       (20)      783 2023-05-04 00:59:20.000000 pyghostdb-0.0.0/README.md
-drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-04 02:33:00.002103 pyghostdb-0.0.0/pyghostdb/
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     1094 2023-05-03 14:29:03.000000 pyghostdb-0.0.0/pyghostdb/ghost_storage.py
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     3072 2023-05-03 01:43:38.000000 pyghostdb-0.0.0/pyghostdb/hnswlib_index.py
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     2020 2023-05-03 14:28:48.000000 pyghostdb-0.0.0/pyghostdb/test_hnsw.py
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     1572 2023-05-03 14:23:30.000000 pyghostdb-0.0.0/pyghostdb/text_storage.py
-drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-04 02:33:00.002522 pyghostdb-0.0.0/pyghostdb.egg-info/
--rw-r--r--   0 fedorshabashev   (501) staff       (20)       53 2023-05-04 02:32:59.000000 pyghostdb-0.0.0/pyghostdb.egg-info/PKG-INFO
--rw-r--r--   0 fedorshabashev   (501) staff       (20)      259 2023-05-04 02:32:59.000000 pyghostdb-0.0.0/pyghostdb.egg-info/SOURCES.txt
--rw-r--r--   0 fedorshabashev   (501) staff       (20)        1 2023-05-04 02:32:59.000000 pyghostdb-0.0.0/pyghostdb.egg-info/dependency_links.txt
--rw-r--r--   0 fedorshabashev   (501) staff       (20)       10 2023-05-04 02:32:59.000000 pyghostdb-0.0.0/pyghostdb.egg-info/top_level.txt
--rw-r--r--   0 fedorshabashev   (501) staff       (20)      392 2023-05-04 02:30:53.000000 pyghostdb-0.0.0/pyproject.toml
--rw-r--r--   0 fedorshabashev   (501) staff       (20)       38 2023-05-04 02:33:00.002821 pyghostdb-0.0.0/setup.cfg
+drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-06 23:23:09.420142 pyghostdb-0.0.1/
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      189 2023-05-06 23:23:09.420013 pyghostdb-0.0.1/PKG-INFO
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      783 2023-05-04 00:59:20.000000 pyghostdb-0.0.1/README.md
+drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-06 23:23:09.419045 pyghostdb-0.0.1/pyghostdb/
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)        0 2023-05-05 14:29:31.000000 pyghostdb-0.0.1/pyghostdb/__init__.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     2000 2023-05-06 23:02:33.000000 pyghostdb-0.0.1/pyghostdb/ghost_storage.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     3072 2023-05-03 01:43:38.000000 pyghostdb-0.0.1/pyghostdb/hnswlib_index.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     2280 2023-05-06 14:54:30.000000 pyghostdb-0.0.1/pyghostdb/parquet_conversion.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     2333 2023-05-05 22:25:22.000000 pyghostdb-0.0.1/pyghostdb/test_hnsw.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     2286 2023-05-06 15:04:20.000000 pyghostdb-0.0.1/pyghostdb/text_storage.py
+drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-06 23:23:09.419863 pyghostdb-0.0.1/pyghostdb.egg-info/
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      189 2023-05-06 23:23:09.000000 pyghostdb-0.0.1/pyghostdb.egg-info/PKG-INFO
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      345 2023-05-06 23:23:09.000000 pyghostdb-0.0.1/pyghostdb.egg-info/SOURCES.txt
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)        1 2023-05-06 23:23:09.000000 pyghostdb-0.0.1/pyghostdb.egg-info/dependency_links.txt
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)       70 2023-05-06 23:23:09.000000 pyghostdb-0.0.1/pyghostdb.egg-info/requires.txt
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)       10 2023-05-06 23:23:09.000000 pyghostdb-0.0.1/pyghostdb.egg-info/top_level.txt
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      363 2023-05-06 23:22:11.000000 pyghostdb-0.0.1/pyproject.toml
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)       38 2023-05-06 23:23:09.420177 pyghostdb-0.0.1/setup.cfg
```

### Comparing `pyghostdb-0.0.0/README.md` & `pyghostdb-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyghostdb-0.0.0/pyghostdb/hnswlib_index.py` & `pyghostdb-0.0.1/pyghostdb/hnswlib_index.py`

 * *Files identical despite different names*

### Comparing `pyghostdb-0.0.0/pyghostdb/test_hnsw.py` & `pyghostdb-0.0.1/pyghostdb/test_hnsw.py`

 * *Files 16% similar despite different names*

```diff
@@ -49,13 +49,20 @@
     gs.add(3, 'hello world 3', np.random.random((3, 1)))
     gs.add(4, 'hello world 4', np.random.random((3, 1)))
     gs.add(5, 'hello world 5', np.random.random((3, 1)))
     gs.add(5, 'hello world 6', np.random.random((3, 1)))
 
     print(gs.search(np.array([1, 2, 3]), k=1))
 
+def test_add_multiple():
+    gs = GhostStorage(dim=3, max_elements=100)
+    gs.add_multiple([1, 2, 3, 4, 5, 6], ['hello world', 'hello world 2', 'hello world 3', 'hello world 4', 'hello world 5', 'hello world 6'], np.random.random((6, 3)))
+    print(gs.search(np.array([1, 2, 3]), k=1))
+
+
 if __name__ == '__main__':
     test_hnsw()
     test_small_vectors2()
     test_text_storage()
     test_ghostdb()
+    test_add_multiple()
```

### Comparing `pyghostdb-0.0.0/pyghostdb/text_storage.py` & `pyghostdb-0.0.1/pyghostdb/text_storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,68 @@
 import duckdb
 import os
+from pyghostdb.parquet_conversion import write_to_parquet, from_parquet_to_duckdb
 
 
 class TextStorage:
     def __init__(self, db_path: str):
         self.db_path = db_path
 
     def add(self, id_: str, text: str, embedding: list[float]):
         connection = duckdb.connect(self.db_path)
         cursor = connection.cursor()
 
         # Create a table with an ARRAY column to store the vector
-        cursor.execute("CREATE TABLE IF NOT EXISTS vectors (id_ INTEGER PRIMARY KEY, text TEXT, vector_data DOUBLE[])")
+        cursor.execute("CREATE TABLE IF NOT EXISTS vectors (id_ INTEGER PRIMARY KEY, text TEXT, embedding DOUBLE[])")
 
         # remove the old vector from the table if it exists
         cursor.execute("DELETE FROM vectors WHERE id_ = ?", (id_,))
         # Insert the vector into the table
         cursor.execute("""
-            INSERT INTO vectors (id_, text, vector_data) 
+            INSERT INTO vectors (id_, text, embedding) 
             VALUES (?, ?, ?) 
         """, (id_, text, embedding))
 
         connection.commit()
 
+    def add_multiple(self, ids: list[int], texts: list[str], embeddings: list[list[float]]):
+        # write to parquet
+        parquet_filepath = f"{self.db_path}_tmp.parquet"
+        write_to_parquet(ids, texts, embeddings, parquet_filepath)
+        from_parquet_to_duckdb(parquet_filepath, self.db_path, "vectors")
+
+
     def get(self, id_):
         connection = duckdb.connect(self.db_path)
         cursor = connection.cursor()
 
         id_int = int(id_)
         # Load the vector from the table
-        cursor.execute("SELECT id_, text, vector_data FROM vectors WHERE id_ = ?", (id_int,))
+        cursor.execute("SELECT id_, text, embedding FROM vectors WHERE id_ = ?", (id_int,))
         id_, text, vector_data = cursor.fetchone()
 
         return id_, text, vector_data
 
+    def get_text(self, id_):
+        connection = duckdb.connect(self.db_path)
+        cursor = connection.cursor()
+
+        id_int = int(id_)
+        # Load the vector from the table
+        cursor.execute("SELECT id_, text FROM vectors WHERE id_ = ?", (id_int,))
+        text = cursor.fetchone()
+
+        return text
+
     def load(self, id_: str):
         connection = duckdb.connect(self.db_path)
         cursor = connection.cursor()
 
         # Load the vector from the table
-        cursor.execute("SELECT id_, text, vector_data FROM vectors WHERE id_ = ?", (id_,))
+        cursor.execute("SELECT id_, text, embedding FROM vectors WHERE id_ = ?", (id_,))
         id_, text, vector_data = cursor.fetchone()
 
         return id_, text, vector_data
 
     def remove_db(self):
         os.remove(self.db_path)
```

