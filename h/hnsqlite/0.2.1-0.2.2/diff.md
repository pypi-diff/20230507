# Comparing `tmp/hnsqlite-0.2.1.tar.gz` & `tmp/hnsqlite-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnsqlite-0.2.1.tar", last modified: Tue May  2 16:31:40 2023, max compression
+gzip compressed data, was "hnsqlite-0.2.2.tar", last modified: Sun May  7 01:38:27 2023, max compression
```

## Comparing `hnsqlite-0.2.1.tar` & `hnsqlite-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-02 16:31:40.368013 hnsqlite-0.2.1/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-03-20 17:17:48.000000 hnsqlite-0.2.1/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     7584 2023-05-02 16:31:40.367688 hnsqlite-0.2.1/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     6980 2023-05-01 19:05:01.000000 hnsqlite-0.2.1/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-02 16:31:40.365159 hnsqlite-0.2.1/hnsqlite/
--rw-r--r--   0 wsk        (501) staff       (20)      116 2023-03-26 23:42:40.000000 hnsqlite-0.2.1/hnsqlite/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)    27458 2023-05-02 16:29:21.000000 hnsqlite-0.2.1/hnsqlite/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)     4758 2023-03-27 02:41:29.000000 hnsqlite-0.2.1/hnsqlite/filter.py
--rw-r--r--   0 wsk        (501) staff       (20)     1238 2023-03-19 01:38:08.000000 hnsqlite-0.2.1/hnsqlite/util.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-02 16:31:40.366473 hnsqlite-0.2.1/hnsqlite.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     7584 2023-05-02 16:31:40.000000 hnsqlite-0.2.1/hnsqlite.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      346 2023-05-02 16:31:40.000000 hnsqlite-0.2.1/hnsqlite.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-02 16:31:40.000000 hnsqlite-0.2.1/hnsqlite.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       37 2023-05-02 16:31:40.000000 hnsqlite-0.2.1/hnsqlite.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)        9 2023-05-02 16:31:40.000000 hnsqlite-0.2.1/hnsqlite.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      747 2023-05-02 16:21:03.000000 hnsqlite-0.2.1/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-02 16:31:40.368111 hnsqlite-0.2.1/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-02 16:31:40.367292 hnsqlite-0.2.1/test/
--rw-r--r--   0 wsk        (501) staff       (20)    12583 2023-05-01 19:05:01.000000 hnsqlite-0.2.1/test/test_collection.py
--rw-r--r--   0 wsk        (501) staff       (20)     2832 2023-05-01 19:05:01.000000 hnsqlite-0.2.1/test/test_collection_filter.py
--rw-r--r--   0 wsk        (501) staff       (20)    12321 2023-03-20 05:54:20.000000 hnsqlite-0.2.1/test/test_filter.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 01:38:27.316337 hnsqlite-0.2.2/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-03-20 17:17:48.000000 hnsqlite-0.2.2/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     7584 2023-05-07 01:38:27.316063 hnsqlite-0.2.2/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     6980 2023-05-01 19:05:01.000000 hnsqlite-0.2.2/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 01:38:27.313661 hnsqlite-0.2.2/hnsqlite/
+-rw-r--r--   0 wsk        (501) staff       (20)      116 2023-03-26 23:42:40.000000 hnsqlite-0.2.2/hnsqlite/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)    30561 2023-05-07 01:27:15.000000 hnsqlite-0.2.2/hnsqlite/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4758 2023-03-27 02:41:29.000000 hnsqlite-0.2.2/hnsqlite/filter.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1238 2023-03-19 01:38:08.000000 hnsqlite-0.2.2/hnsqlite/util.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 01:38:27.314948 hnsqlite-0.2.2/hnsqlite.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     7584 2023-05-07 01:38:27.000000 hnsqlite-0.2.2/hnsqlite.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      346 2023-05-07 01:38:27.000000 hnsqlite-0.2.2/hnsqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-07 01:38:27.000000 hnsqlite-0.2.2/hnsqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       37 2023-05-07 01:38:27.000000 hnsqlite-0.2.2/hnsqlite.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        9 2023-05-07 01:38:27.000000 hnsqlite-0.2.2/hnsqlite.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      747 2023-05-07 00:12:17.000000 hnsqlite-0.2.2/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-07 01:38:27.316411 hnsqlite-0.2.2/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 01:38:27.315741 hnsqlite-0.2.2/test/
+-rw-r--r--   0 wsk        (501) staff       (20)    12583 2023-05-01 19:05:01.000000 hnsqlite-0.2.2/test/test_collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2832 2023-05-01 19:05:01.000000 hnsqlite-0.2.2/test/test_collection_filter.py
+-rw-r--r--   0 wsk        (501) staff       (20)    12321 2023-03-20 05:54:20.000000 hnsqlite-0.2.2/test/test_filter.py
```

### Comparing `hnsqlite-0.2.1/LICENSE` & `hnsqlite-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hnsqlite-0.2.1/PKG-INFO` & `hnsqlite-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hnsqlite
-Version: 0.2.1
+Version: 0.2.2
 Summary: A minimalist integration of sqlite and hnswlib focused on providing simple embedding persistence and search for text applications.
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/hnsqlite
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/hnsqlite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hnsqlite-0.2.1/README.md` & `hnsqlite-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `hnsqlite-0.2.1/hnsqlite/collection.py` & `hnsqlite-0.2.2/hnsqlite/collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from psutil import cpu_count
 import os
 from json import dumps, loads
 import numpy as np
 from .filter import filter_item
 from .util import md5_file, _is_valid_namestr
 import sqlite3
+from collections import defaultdict
+import glob
 
 CPU_COUNT = cpu_count()
 
 class NoResultError(Exception):
     pass
 
 class dbHnswIndexConfig(SQLModel, table=True):
@@ -162,62 +164,79 @@
 
     def vector_as_array(self) -> np.array:    
         """
         return the stored vector as a numpy array        
         """
         return np.array(self.vector)
 
-        
+
+            
 class SearchResponse(Embedding):
     """
     Return a search result consisting of an embedding and the distance to the query vector
     """
     distance: float
 
 
     
 class Collection :
     """
     A combination of a sqlite database and an hnswlib index that provides a persistent collection of embeddings (strings+vectors+metadata) including hnswlib index configuration.
     """      
     def __init__(self, 
-                 collection_name : str,
-                 dimension       : int,                                  
-                 sqlite_filename : Optional[str] = 'hnsqlite.sqlite',
+                 collection_name : Optional[str] = None,
+                 dimension       : Optional[int] = None,                                  
+                 sqlite_filename : Optional[str] = None,
                  modelname       : Optional[str] = None,
                  description     : Optional[str] = None) -> "Collection":
         """
-        collection_name:    The name of the collection to use.  must be unique with the sqlite database            
-        dimension:          The dimension of the vector space        
+        collection_name:    The name of the collection to use.  must be unique with the sqlite database.  Need not be specified if the sqlite database contains only one collection.
+        dimension:          The dimension of the vector space. Need not be specified if the collection already exists.       
         sqlite_filename:    The name of the sqlite database file to use for the collection
-                            If not specified a default name of 'hnsqlite.sqlite' will be used and the database will be created if it does not exist.
+                            If not specified and a single sqlite file exists in the current directory, that file will be used.
+                            otherwise a new database will be created with the default name of 'hnsqlite.sqlite'.
         modelname:          Optional name of the model used to generate the embeddings
         description:        Optional description of the collection
         
         Create a hnsqlite Collection object from a sqlite collection database file.
         Creates hnsqlite tables within the database if necessary.
         If the specified collection name is found in the database, the collection will be initialized
         from the database.  Otherwise a new collection of the specified name will be created in the database.
         """
-        _is_valid_namestr(collection_name, 'name')
+        if collection_name is not None:   # validate collection_name if specified
+            _is_valid_namestr(collection_name, 'name')
+        if not sqlite_filename:   # find sqlite file if not specified
+            sqlite_files = glob.glob("*.sqlite")
+            if len(sqlite_files) == 1:
+                sqlite_filename = sqlite_files[0]
+                logger.info(f"using sqlite_filename {sqlite_filename}")
+            elif len(sqlite_files) > 1:
+                sqlite_filename = 'hnsqlite.sqlite'  # default name
         if not os.path.exists(sqlite_filename):        
             logger.warning(f"sqlite_filename {sqlite_filename} does not exist; create new database")
         else:
             logger.info(f"sqlite_filename {sqlite_filename} exists; using existing database")
         db_engine = create_engine(f'sqlite:///{sqlite_filename}')
         SQLModel.metadata.create_all(db_engine)                    
         with Session(db_engine) as session:
-            cconfig = session.exec(select(dbCollectionConfig).where(dbCollectionConfig.name == collection_name)).first()
+            if not collection_name:
+                cconfig = session.exec(select(dbCollectionConfig)).one()
+                collection_name = cconfig.name
+            else:
+                cconfig = session.exec(select(dbCollectionConfig).where(dbCollectionConfig.name == collection_name)).first()
             if cconfig:
-                if cconfig.dim != dimension:
+                if dimension and cconfig.dim != dimension:
                     logger.error(f"collection {collection_name} already exists in {sqlite_filename} with dimension {cconfig.dim}")
                     raise ValueError(f"collection {collection_name} already exists in {sqlite_filename} with dimension {cconfig.dim}")
                 else:
                     logger.info(f"using existing collection {collection_name} found in {sqlite_filename}")
             else:
+                if not dimension or not collection_name:
+                    logger.error(f'collection name and dimension must be specified to create a new collection')
+                    raise ValueError(f'collection name and dimension must be specified to create a new collection')
                 logger.warning(f"collection {collection_name} not found in {sqlite_filename}; creating new collection")
                 cconfig = dbCollectionConfig(name=collection_name, 
                                              dim=dimension,
                                              model=modelname, 
                                              description=description)        
                 with Session(db_engine) as session:            
                     session.add(cconfig)
@@ -298,15 +317,15 @@
         with Session(self.db_engine) as session:
             t0 = time()
             count = 0
             BATCH_SIZE = CPU_COUNT*16
             # batches process of embeddings for efficiency
             def process_batch(batch : list[dbEmbedding]):            
                 # add batch of document embeddings to index
-                hnsw_ix.add_items([e.vector for e in batch], [e.id for e in batch])            
+                hnsw_ix.add_items([e.vector_as_array() for e in batch], [e.id for e in batch])            
                 logger.info(f"hnsw_index.add_items   vectors/sec: {count/(time() - t0):.1f} ; total vectors: {count}")            
             batch = []            
             for de in session.exec(select(dbEmbedding).where(dbEmbedding.collection_id == self.config.id )).yield_per(BATCH_SIZE):
                 batch.append(de)
                 if len(batch) == BATCH_SIZE:
                     process_batch(batch)
                     count += len(batch)
@@ -343,14 +362,18 @@
         logger.info(f"load index for {self.config}")        
         with Session(self.db_engine) as session:
             index_config = session.exec(select(dbHnswIndexConfig).where(dbHnswIndexConfig.collection_id == self.config.id).order_by(dbHnswIndexConfig.id.desc())).first()
             if not index_config:
                 self.make_index()   # intialize and load the index
                 return
         logger.info(f"loading index {index_config}")
+        if not os.path.exists(index_config.filename):
+            logger.error(f"index file {index_config.filename} does not exist")
+            self.make_index()
+            return
         md5sum = md5_file(index_config.filename)
         if md5sum != index_config.md5sum:
             logger.error(f"md5sum {md5sum} does not match config.md5sum {index_config.md5sum}")
             self.make_index()   # intialize and load the index from scratch
             return
         else:
             logger.info(f"md5sum matches index.md5sum")
@@ -455,15 +478,45 @@
     def get_embeddings_doc_ids(self, doc_ids : List[str]) ->  List[Embedding]:
         """
         get the embeddings for the specified doc_ids
         """
         with Session(self.db_engine) as session:    
             query = select(dbEmbedding).where(dbEmbedding.collection_id == self.config.id).where(dbEmbedding.doc_id.in_(doc_ids))
             return [Embedding.from_db(e) for e in session.exec(query)]
-        
+
+    def get_embeddings_by_doc(self, index: int, limit: int, reverse :bool, max_per_doc: int = 1) -> Tuple[List[List[Embedding]], int]:
+        """
+        return a tuple containing a list of lists of Embedding objects from the collection and the index of the last item processed.
+        the top level list is per document, the inner list is the embeddings for that document
+        index is is the offset into the list of documents; should be -1 for first item if reverse is True
+        limit is the number of documents to return
+        max_per_doc is the maximum number of embeddings to return per document
+        """
+        docs_dl = defaultdict(list)
+        query = select(dbEmbedding).where(dbEmbedding.collection_id == self.config.id)
+        if reverse:
+            index = index if index >= 0 else 9223372036854775807   # largest 64 bit signed integer
+            query = query.order_by(desc(dbEmbedding.id)).where(dbEmbedding.id < index)
+        else:
+            query = query.order_by(asc(dbEmbedding.id)).where(dbEmbedding.id > index)
+        with Session(self.db_engine) as session:
+            for emb in session.exec(query):
+                index = emb.id  # advance index of last item processed
+                if emb.doc_id not in docs_dl and len (docs_dl) >= limit:
+                    break
+                docs_dl[emb.doc_id].append(Embedding.from_db(emb))
+
+        for doc_id in docs_dl:
+            docs_dl[doc_id].sort(key=lambda e: e.created_at)
+        if max_per_doc is None:
+            docs = [docs_dl[doc_id] for doc_id in docs_dl]
+        else:
+            docs = [docs_dl[doc_id][:max_per_doc] for doc_id in docs_dl]
+        return docs, index
+
     def search(self, vector: np.array, k = 12, filter=None) -> List[SearchResponse]:        
         """
         query the hnsw index for the nearest neighbors of the given vector
         unlike hnswlib which takes a 2D array of vectors, this method takes a single vector
         since the common use case for this in production is searching for a single vector at a time
         """
         if isinstance(vector, list):
```

### Comparing `hnsqlite-0.2.1/hnsqlite/filter.py` & `hnsqlite-0.2.2/hnsqlite/filter.py`

 * *Files identical despite different names*

### Comparing `hnsqlite-0.2.1/hnsqlite/util.py` & `hnsqlite-0.2.2/hnsqlite/util.py`

 * *Files identical despite different names*

### Comparing `hnsqlite-0.2.1/hnsqlite.egg-info/PKG-INFO` & `hnsqlite-0.2.2/hnsqlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hnsqlite
-Version: 0.2.1
+Version: 0.2.2
 Summary: A minimalist integration of sqlite and hnswlib focused on providing simple embedding persistence and search for text applications.
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/hnsqlite
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/hnsqlite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `hnsqlite-0.2.1/pyproject.toml` & `hnsqlite-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hnsqlite"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['sqlmodel', 'hnswlib', 'psutil', 'numpy', 'loguru']
 description = "A minimalist integration of sqlite and hnswlib focused on providing simple embedding persistence and search for text applications."
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `hnsqlite-0.2.1/test/test_collection.py` & `hnsqlite-0.2.2/test/test_collection.py`

 * *Files identical despite different names*

### Comparing `hnsqlite-0.2.1/test/test_collection_filter.py` & `hnsqlite-0.2.2/test/test_collection_filter.py`

 * *Files identical despite different names*

### Comparing `hnsqlite-0.2.1/test/test_filter.py` & `hnsqlite-0.2.2/test/test_filter.py`

 * *Files identical despite different names*

