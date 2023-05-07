# Comparing `tmp/pyghostdb-0.0.2.tar.gz` & `tmp/pyghostdb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyghostdb-0.0.2.tar", last modified: Sun May  7 02:20:25 2023, max compression
+gzip compressed data, was "pyghostdb-0.0.3.tar", last modified: Sun May  7 03:59:51 2023, max compression
```

## Comparing `pyghostdb-0.0.2.tar` & `pyghostdb-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-07 02:20:25.262378 pyghostdb-0.0.2/
--rw-r--r--   0 fedorshabashev   (501) staff       (20)      189 2023-05-07 02:20:25.262222 pyghostdb-0.0.2/PKG-INFO
--rw-r--r--   0 fedorshabashev   (501) staff       (20)      783 2023-05-04 00:59:20.000000 pyghostdb-0.0.2/README.md
-drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-07 02:20:25.261305 pyghostdb-0.0.2/pyghostdb/
--rw-r--r--   0 fedorshabashev   (501) staff       (20)        0 2023-05-05 14:29:31.000000 pyghostdb-0.0.2/pyghostdb/__init__.py
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     2000 2023-05-06 23:02:33.000000 pyghostdb-0.0.2/pyghostdb/ghost_storage.py
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     3068 2023-05-07 00:07:50.000000 pyghostdb-0.0.2/pyghostdb/hnswlib_index.py
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     2280 2023-05-06 14:54:30.000000 pyghostdb-0.0.2/pyghostdb/parquet_conversion.py
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     2332 2023-05-07 00:07:50.000000 pyghostdb-0.0.2/pyghostdb/test_hnsw.py
--rw-r--r--   0 fedorshabashev   (501) staff       (20)     2283 2023-05-07 00:07:14.000000 pyghostdb-0.0.2/pyghostdb/text_storage.py
-drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-07 02:20:25.262082 pyghostdb-0.0.2/pyghostdb.egg-info/
--rw-r--r--   0 fedorshabashev   (501) staff       (20)      189 2023-05-07 02:20:25.000000 pyghostdb-0.0.2/pyghostdb.egg-info/PKG-INFO
--rw-r--r--   0 fedorshabashev   (501) staff       (20)      345 2023-05-07 02:20:25.000000 pyghostdb-0.0.2/pyghostdb.egg-info/SOURCES.txt
--rw-r--r--   0 fedorshabashev   (501) staff       (20)        1 2023-05-07 02:20:25.000000 pyghostdb-0.0.2/pyghostdb.egg-info/dependency_links.txt
--rw-r--r--   0 fedorshabashev   (501) staff       (20)       58 2023-05-07 02:20:25.000000 pyghostdb-0.0.2/pyghostdb.egg-info/requires.txt
--rw-r--r--   0 fedorshabashev   (501) staff       (20)       10 2023-05-07 02:20:25.000000 pyghostdb-0.0.2/pyghostdb.egg-info/top_level.txt
--rw-r--r--   0 fedorshabashev   (501) staff       (20)      347 2023-05-07 02:19:53.000000 pyghostdb-0.0.2/pyproject.toml
--rw-r--r--   0 fedorshabashev   (501) staff       (20)       38 2023-05-07 02:20:25.262492 pyghostdb-0.0.2/setup.cfg
+drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-07 03:59:51.022441 pyghostdb-0.0.3/
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      189 2023-05-07 03:59:51.022306 pyghostdb-0.0.3/PKG-INFO
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      783 2023-05-04 00:59:20.000000 pyghostdb-0.0.3/README.md
+drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-07 03:59:51.021443 pyghostdb-0.0.3/pyghostdb/
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)        0 2023-05-05 14:29:31.000000 pyghostdb-0.0.3/pyghostdb/__init__.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     2756 2023-05-07 03:58:29.000000 pyghostdb-0.0.3/pyghostdb/ghost_storage.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     3068 2023-05-07 00:07:50.000000 pyghostdb-0.0.3/pyghostdb/hnswlib_index.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     2281 2023-05-07 02:28:04.000000 pyghostdb-0.0.3/pyghostdb/parquet_conversion.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     2376 2023-05-07 02:28:04.000000 pyghostdb-0.0.3/pyghostdb/test_hnsw.py
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)     2284 2023-05-07 02:28:04.000000 pyghostdb-0.0.3/pyghostdb/text_storage.py
+drwxr-xr-x   0 fedorshabashev   (501) staff       (20)        0 2023-05-07 03:59:51.022164 pyghostdb-0.0.3/pyghostdb.egg-info/
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      189 2023-05-07 03:59:51.000000 pyghostdb-0.0.3/pyghostdb.egg-info/PKG-INFO
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      345 2023-05-07 03:59:51.000000 pyghostdb-0.0.3/pyghostdb.egg-info/SOURCES.txt
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)        1 2023-05-07 03:59:51.000000 pyghostdb-0.0.3/pyghostdb.egg-info/dependency_links.txt
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)       58 2023-05-07 03:59:51.000000 pyghostdb-0.0.3/pyghostdb.egg-info/requires.txt
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)       10 2023-05-07 03:59:51.000000 pyghostdb-0.0.3/pyghostdb.egg-info/top_level.txt
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)      347 2023-05-07 03:59:42.000000 pyghostdb-0.0.3/pyproject.toml
+-rw-r--r--   0 fedorshabashev   (501) staff       (20)       38 2023-05-07 03:59:51.022480 pyghostdb-0.0.3/setup.cfg
```

### Comparing `pyghostdb-0.0.2/README.md` & `pyghostdb-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyghostdb-0.0.2/pyghostdb/ghost_storage.py` & `pyghostdb-0.0.3/pyghostdb/ghost_storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,48 +5,66 @@
 import os
 
 
 class GhostStorage:
     hnsw_index = None
     text_storage_db = None
 
-    def __init__(self, dim=1024, max_elements=10**5, persist_dir="ghost_dir"):
+    def __init__(self, dim=1536, max_elements=10**5, persist_dir="ghost_dir"):
         self.hnsw_index = HNSWIndex(dim=dim, max_elements=max_elements, ef=200, M=16)
         self.hnsw_index.init_index()
         self.persist_dir = persist_dir
         if not os.path.exists(self.persist_dir):
             os.makedirs(self.persist_dir)
-        self.text_storage_db = TextStorage(os.path.join(self.persist_dir, "text_storage.db"))
+        self.text_storage_db = TextStorbuiage(self.text_storage_filepath())
+        if self.hnws_index_filepath_exists():
+            self.load()
 
     def add(self, text_id, text, embedding):
-        assert isinstance(embedding, np.ndarray)
-        assert embedding.shape[0] == self.hnsw_index.dim
-        assert self.hnsw_index is not None
+        if not isinstance(embedding, np.ndarray):
+            try:
+                embedding = np.array(embedding)
+            except Exception as e:
+                print(e)
+                raise TypeError("embedding must be a numpy array or a list")
+        if not embedding.shape[0] == self.hnsw_index.dim:
+            raise ValueError("embedding must have the same dimension as the hnsw index")
+        if self.hnsw_index is None:
+            raise AttributeError("HNSW index is not initialized, please call load method")
         # convert numpy array to list of floats
         embedding = [float(x) for x in list(embedding.reshape(-1))]
         self.text_storage_db.add(text_id, text, embedding)
         self.hnsw_index.add_items(embedding, [text_id])
 
     def add_multiple(self, ids: list[int], texts: list[str], embeddings: np.ndarray):
         # convert numpy array to list of floats
         self.hnsw_index.add_items(embeddings, ids)
         embeddings = [list(embedding) for embedding in embeddings]
         self.text_storage_db.add_multiple(ids, texts, embeddings)
 
     def search(self, embedding, k=1):
+        # check if embedding is a list
+        if isinstance(embedding, list):
+            embedding = np.array(embedding)
         ids, distance = self.hnsw_index.knn_query(embedding, k=k)
         # convert ids to list of ints
         ids = [int(id_) for id_ in ids.flatten().tolist()]
         return [self.text_storage_db.get(id_) for id_ in ids]
 
     def clear(self):
         self.hnsw_index = None
         self.text_storage_db.remove_db()
 
     def hnws_index_filepath(self):
         return os.path.join(self.persist_dir, "index.ghostdb")
 
+    def hnws_index_filepath_exists(self):
+        return os.path.exists(self.hnws_index_filepath())
+
+    def text_storage_filepath(self):
+        return os.path.join(self.persist_dir, "text_storage.db")
+
     def persist(self):
         self.hnsw_index.save_to_file(self.hnws_index_filepath())
 
     def load(self):
         self.hnsw_index.load_from_file(self.hnws_index_filepath())
```

### Comparing `pyghostdb-0.0.2/pyghostdb/hnswlib_index.py` & `pyghostdb-0.0.3/pyghostdb/hnswlib_index.py`

 * *Files identical despite different names*

### Comparing `pyghostdb-0.0.2/pyghostdb/parquet_conversion.py` & `pyghostdb-0.0.3/pyghostdb/parquet_conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import duckdb
 import pyarrow as pa
 import pyarrow.parquet
-import duckdb
 
 
 def write_to_parquet(text_ids: list[int], texts: list[str], embeddings: list[list[float]], output_file: str):
     schema = pa.schema([
         ('id_', pa.int32()),
         ('text', pa.string()),
         ('embedding', pa.list_(pa.float32())),
@@ -44,14 +44,15 @@
     conn.execute(f'''
         COPY {table_name} FROM '{parquet_file}' (FORMAT 'parquet');
     ''')
 
     # Close the connection
     conn.close()
 
+
 # (id_, text, vector_data)
 
 
 if __name__ == "__main__":
     # Define your dictionary
     data = {
         'text': ['sample text 1', 'sample text 2'],
```

### Comparing `pyghostdb-0.0.2/pyghostdb/test_hnsw.py` & `pyghostdb-0.0.3/pyghostdb/test_hnsw.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from hnswlib_index import HNSWIndex
 import numpy as np
-from text_storage import TextStorage
+
 from ghost_storage import GhostStorage
+from hnswlib_index import HNSWIndex
+from text_storage import TextStorage
+
 
 def test_hnsw():
     n_elements = 100
     index = HNSWIndex(dim=1024, max_elements=n_elements)
     index.build_index(np.float32(np.random.random((n_elements, 1024))))
     test_data = np.float32(np.random.random((100, 1024)))
     labels1, distances = index.knn_query(test_data, k=1)
@@ -49,17 +51,20 @@
     gs.add(3, 'hello world 3', np.random.random((3, 1)))
     gs.add(4, 'hello world 4', np.random.random((3, 1)))
     gs.add(5, 'hello world 5', np.random.random((3, 1)))
     gs.add(5, 'hello world 6', np.random.random((3, 1)))
 
     print(gs.search(np.array([1, 2, 3]), k=1))
 
+
 def test_add_multiple():
     gs = GhostStorage(dim=3, max_elements=100)
-    gs.add_multiple([1, 2, 3, 4, 5, 6], ['hello world', 'hello world 2', 'hello world 3', 'hello world 4', 'hello world 5', 'hello world 6'], np.random.random((6, 3)))
+    gs.add_multiple([1, 2, 3, 4, 5, 6],
+                    ['hello world', 'hello world 2', 'hello world 3', 'hello world 4', 'hello world 5',
+                     'hello world 6'], np.random.random((6, 3)))
     print(gs.search(np.array([1, 2, 3]), k=1))
 
 
 if __name__ == '__main__':
     test_hnsw()
     test_small_vectors2()
     test_text_storage()
```

### Comparing `pyghostdb-0.0.2/pyghostdb/text_storage.py` & `pyghostdb-0.0.3/pyghostdb/text_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-import duckdb
 import os
+
+import duckdb
+
 from pyghostdb.parquet_conversion import write_to_parquet, from_parquet_to_duckdb
 
 
 class TextStorage:
     def __init__(self, db_path: str):
         self.db_path = db_path
 
@@ -26,15 +28,14 @@
 
     def add_multiple(self, ids: list[int], texts: list[str], embeddings: list[list[float]]):
         # write to parquet
         parquet_filepath = f"{self.db_path}_tmp.parquet"
         write_to_parquet(ids, texts, embeddings, parquet_filepath)
         from_parquet_to_duckdb(parquet_filepath, self.db_path, "vectors")
 
-
     def get(self, id_):
         connection = duckdb.connect(self.db_path)
         cursor = connection.cursor()
 
         id_int = int(id_)
         # Load the vector from the table
         cursor.execute("SELECT id_, text, embedding FROM vectors WHERE id_ = ?", (id_int,))
```

