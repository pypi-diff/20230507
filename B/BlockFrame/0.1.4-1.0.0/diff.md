# Comparing `tmp/BlockFrame-0.1.4.tar.gz` & `tmp/BlockFrame-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlockFrame-0.1.4.tar", last modified: Sun Apr 30 06:50:31 2023, max compression
+gzip compressed data, was "BlockFrame-1.0.0.tar", last modified: Sun May  7 18:27:48 2023, max compression
```

## Comparing `BlockFrame-0.1.4.tar` & `BlockFrame-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 06:50:31.534530 BlockFrame-0.1.4/
-drwxrwxrwx   0        0        0        0 2023-04-30 06:50:31.484920 BlockFrame-0.1.4/BlockFrame/
--rw-rw-rw-   0        0        0        0 2023-04-01 11:41:46.000000 BlockFrame-0.1.4/BlockFrame/__init__.py
--rw-rw-rw-   0        0        0     4424 2023-04-30 06:46:47.000000 BlockFrame-0.1.4/BlockFrame/block_frame.py
-drwxrwxrwx   0        0        0        0 2023-04-30 06:50:31.526537 BlockFrame-0.1.4/BlockFrame/chunking_service/
--rw-rw-rw-   0        0        0        0 2023-04-01 11:41:46.000000 BlockFrame-0.1.4/BlockFrame/chunking_service/__init__.py
--rw-rw-rw-   0        0        0     7285 2023-04-30 06:46:40.000000 BlockFrame-0.1.4/BlockFrame/chunking_service/chunking.py
--rw-rw-rw-   0        0        0      691 2023-04-28 14:22:04.000000 BlockFrame-0.1.4/BlockFrame/chunking_service/config.py
-drwxrwxrwx   0        0        0        0 2023-04-30 06:50:31.532538 BlockFrame-0.1.4/BlockFrame/database_service/
--rw-rw-rw-   0        0        0        0 2023-04-01 11:35:37.000000 BlockFrame-0.1.4/BlockFrame/database_service/__init__.py
--rw-rw-rw-   0        0        0      744 2023-04-28 14:05:46.000000 BlockFrame-0.1.4/BlockFrame/database_service/database.py
--rw-rw-rw-   0        0        0     1599 2023-04-30 05:33:57.000000 BlockFrame-0.1.4/BlockFrame/database_service/defaultmodel.py
--rw-rw-rw-   0        0        0      377 2023-04-28 14:26:18.000000 BlockFrame-0.1.4/BlockFrame/database_service/getters.py
--rw-rw-rw-   0        0        0     1345 2023-04-30 04:36:05.000000 BlockFrame-0.1.4/BlockFrame/database_service/initalisation.py
--rw-rw-rw-   0        0        0      241 2023-03-26 14:17:13.000000 BlockFrame-0.1.4/BlockFrame/database_service/setters.py
-drwxrwxrwx   0        0        0        0 2023-04-30 06:50:31.493175 BlockFrame-0.1.4/BlockFrame.egg-info/
--rw-rw-rw-   0        0        0      268 2023-04-30 06:50:31.000000 BlockFrame-0.1.4/BlockFrame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      591 2023-04-30 06:50:31.000000 BlockFrame-0.1.4/BlockFrame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 06:50:31.000000 BlockFrame-0.1.4/BlockFrame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-30 06:50:31.000000 BlockFrame-0.1.4/BlockFrame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-30 06:50:31.000000 BlockFrame-0.1.4/BlockFrame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      268 2023-04-30 06:50:31.534530 BlockFrame-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-30 06:50:31.534530 BlockFrame-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      458 2023-04-30 06:50:26.000000 BlockFrame-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 18:27:48.765260 BlockFrame-1.0.0/
+drwxrwxrwx   0        0        0        0 2023-05-07 18:27:48.722927 BlockFrame-1.0.0/BlockFrame/
+-rw-rw-rw-   0        0        0       75 2023-05-07 16:54:53.000000 BlockFrame-1.0.0/BlockFrame/__init__.py
+-rw-rw-rw-   0        0        0      832 2023-05-07 18:26:27.000000 BlockFrame-1.0.0/BlockFrame/block_frame.py
+drwxrwxrwx   0        0        0        0 2023-05-07 18:27:48.754733 BlockFrame-1.0.0/BlockFrame/chunking_service/
+-rw-rw-rw-   0        0        0        0 2023-04-01 11:41:46.000000 BlockFrame-1.0.0/BlockFrame/chunking_service/__init__.py
+-rw-rw-rw-   0        0        0     8233 2023-05-07 18:26:27.000000 BlockFrame-1.0.0/BlockFrame/chunking_service/chunking.py
+-rw-rw-rw-   0        0        0     1095 2023-05-07 18:26:27.000000 BlockFrame-1.0.0/BlockFrame/chunking_service/config.py
+-rw-rw-rw-   0        0        0     1657 2023-05-07 15:14:26.000000 BlockFrame-1.0.0/BlockFrame/chunking_service/fetcher.py
+drwxrwxrwx   0        0        0        0 2023-05-07 18:27:48.763245 BlockFrame-1.0.0/BlockFrame/database_service/
+-rw-rw-rw-   0        0        0        0 2023-04-01 11:35:37.000000 BlockFrame-1.0.0/BlockFrame/database_service/__init__.py
+-rw-rw-rw-   0        0        0     1061 2023-05-07 17:47:32.000000 BlockFrame-1.0.0/BlockFrame/database_service/database.py
+-rw-rw-rw-   0        0        0     1599 2023-05-07 11:12:22.000000 BlockFrame-1.0.0/BlockFrame/database_service/defaultmodel.py
+-rw-rw-rw-   0        0        0      377 2023-04-30 09:16:12.000000 BlockFrame-1.0.0/BlockFrame/database_service/getters.py
+-rw-rw-rw-   0        0        0     1518 2023-05-07 17:44:18.000000 BlockFrame-1.0.0/BlockFrame/database_service/initalisation.py
+-rw-rw-rw-   0        0        0      241 2023-03-26 14:17:13.000000 BlockFrame-1.0.0/BlockFrame/database_service/setters.py
+drwxrwxrwx   0        0        0        0 2023-05-07 18:27:48.750630 BlockFrame-1.0.0/BlockFrame.egg-info/
+-rw-rw-rw-   0        0        0     5161 2023-05-07 18:27:48.000000 BlockFrame-1.0.0/BlockFrame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2023-05-07 18:27:48.000000 BlockFrame-1.0.0/BlockFrame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 18:27:48.000000 BlockFrame-1.0.0/BlockFrame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-07 18:27:48.000000 BlockFrame-1.0.0/BlockFrame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-07 18:27:48.000000 BlockFrame-1.0.0/BlockFrame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5161 2023-05-07 18:27:48.764253 BlockFrame-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-07 18:27:48.765260 BlockFrame-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1310 2023-05-07 18:27:21.000000 BlockFrame-1.0.0/setup.py
```

### Comparing `BlockFrame-0.1.4/BlockFrame/chunking_service/chunking.py` & `BlockFrame-1.0.0/BlockFrame/chunking_service/chunking.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 import hashlib
 import math
 import os
 import pathlib
 import uuid
 from datetime import datetime, timedelta
 
-import psutil
-
 from ..database_service.defaultmodel import ChunkHashes, DefaultChunkModel
 
 
+class ChunksExistsError(Exception):
+    pass
+
+
 class ChunkHandler:
     def __init__(self, *args, **kwargs) -> None:
         self.config = kwargs.get("config")
         self.path = self.config["file-storage-path"]
         self.option = kwargs.get("option")
         self.chunking_method: str = ""
         self.db = kwargs.get("db")
         self.chunk_size_estimate = 1024 * 1024
         self.chunk_counter = 0
         self.window_size = 10
         self.chunk_time_estimate = timedelta(seconds=1)
 
-    def target(self, file_name, size, files: list = None):
+    def target(
+        self, file_name, size=None, files: list = None, custom_chunker: callable = None
+    ):
         self.file_name = file_name
         self.size = size
         self.primary_uuid = uuid.uuid4()
         self.original_file_hash = ""
         self.chunk_file_hashes = []
         self.chunk_file_uid = []
-        return "correctly targetted"
-
-    def __dir(self):
-        try:
-            return (
-                pathlib.Path(self.config.get("file-storage-path"))
-                if pathlib.Path(self.config.get("file-storage-path"))
-                is pathlib.Path(self.config.get("file-storage-path")).exists
-                else pathlib.Path(self.config.get("file-storage-path")).mkdir()
-            )
-        except FileExistsError:
-            return pathlib.Path(self.config.get("file-storage-path"))
+        self.files = files
+        self.custom_chunker = custom_chunker
+        if not pathlib.Path(self.file_name) or not pathlib.Path(self.file_name).exists:
+            raise FileNotFoundError
+        return "correctly targeted"
 
     def generic_chunks(self):
         _size = os.stat(self.file_name).st_size // self.size
         with open(self.file_name, "rb") as f:
             while content := f.read(_size):
                 yield content
 
@@ -85,15 +82,25 @@
                             ),
                             1,
                         )
                     )
 
     def secure_chunks(self):
         with open(self.file_name, "rb") as f:
-            while content := f.read(self.chunk_size_estimate):
+            file_size = os.stat(self.file_name).st_size
+            while True:
+                chunk_size = self.chunk_size_estimate
+                num_chunks = math.ceil(file_size / chunk_size)
+                if num_chunks >= 4:
+                    break
+                chunk_size = math.ceil(file_size / 4)
+                num_chunks = 4
+                self.chunk_size_estimate = chunk_size
+
+            while content := f.read(chunk_size):
                 yield content
                 self.chunk_counter += 1
                 if self.chunk_counter % self.window_size == 0:
                     # use a sliding window to estimate the collision probability
                     past_hashes = self.hasher.digest() * self.window_size
                     self.hasher = hashlib.sha256()
                     self.hasher.update(past_hashes)
@@ -110,30 +117,51 @@
                                 ),
                             ),
                             1,
                         )
                     )
 
     def produce_chunks(self):
-        if self.option == "generic":
-            split_files = self.generic_chunks()
-        if self.option == "hardware":
-            split_files = self.hardware_chunks()
-        if self.option == "time":
-            split_files = self.time_based_chunks()
-        if self.option == "secure":
-            split_files = self.secure_chunks()
+        if self.option == "custom":
+            split_files = self.custom_chunker(self.file_name, self.size)
+
+        else:
+            match self.option:
+                case "generic":
+                    split_files = self.generic_chunks()
+                case "hardware":
+                    split_files = self.hardware_chunks()
+                case "time":
+                    split_files = self.time_based_chunks()
+                case "secure":
+                    split_files = self.secure_chunks()
+        [
+            x
+            for x in os.listdir(self.path)
+            if x.startswith(f"{self.primary_uuid}_chunk_")
+        ]
+
+        with self.db as session:
+            if existing_models := (
+                session.query(DefaultChunkModel)
+                .filter_by(file_name=self.file_name)
+                .all()
+            ):
+                raise ChunksExistsError("file is already chunked")
 
         count = 0
         for chunk in split_files:
             _hash = hashlib.sha256()
             _file_chunk_uid = uuid.uuid4()
+            chunk_name = f"{self.primary_uuid}_chunk_{_file_chunk_uid}_{count}.chunk"
+            if not pathlib.Path(self.path).is_dir():
+                pathlib.Path(self.path).mkdir()
 
             with open(
-                f"{pathlib.Path(self.path).absolute()}/{self.primary_uuid}_chunk_{_file_chunk_uid}_{count}.chunk",
+                f"{pathlib.Path(self.path).absolute()}/{chunk_name}",
                 "wb+",
             ) as f:
                 _hash.update(f.read())
                 count += 1
                 f.write(bytes(chunk))
             self.chunk_file_uid.append(_file_chunk_uid)
             self.chunk_file_hashes.append(_hash.hexdigest())
```

### Comparing `BlockFrame-0.1.4/BlockFrame/database_service/defaultmodel.py` & `BlockFrame-1.0.0/BlockFrame/database_service/defaultmodel.py`

 * *Files identical despite different names*

### Comparing `BlockFrame-0.1.4/BlockFrame/database_service/initalisation.py` & `BlockFrame-1.0.0/BlockFrame/database_service/initalisation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from sqlalchemy.engine import create_engine
 from sqlalchemy.orm import declarative_base, sessionmaker
+from abc import ABC
 
 
-class DatabaseInterface:
+class DatabaseInterface(ABC):
     Base = declarative_base()
     db_engine = create_engine("sqlite:///block_frame.db")
     sync_session = sessionmaker(autocommit=False, autoflush=False, bind=db_engine)
 
-    def custom_uri(self: str):
-        create_engine(self)
-
-    def return_engine(self):
-        return self.db_engine
+    @classmethod
+    def custom_uri(cls, uri: str):
+        cls.db_engine = create_engine(uri)
+        cls.sync_session = sessionmaker(
+            autocommit=False, autoflush=False, bind=cls.db_engine
+        )
+
+    @classmethod
+    def return_engine(cls):
+        return cls.db_engine
 
 
 class BlockFrameDatabaseInit(DatabaseInterface):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__()
         self.class_model = kwargs.get("class_model")
         if self.class_model is None:
@@ -23,19 +29,19 @@
 
             self.db_model = DefaultChunkModel
         else:
             self.db_model = self.class_model
 
     def create_table(self, db_model):
         with self.db_engine.begin() as conn:
-            DatabaseInterface.sync_session(bind=conn)  # <-- change this line
+            self.sync_session(bind=conn)  # <-- change this line
             db_model.metadata.create_all(conn)
 
     def get_db(self):
         # return an object which can be used to commit data to the database easily
-        return DatabaseInterface.sync_session()
+        return self.sync_session()
 
 
 class BlockFrameModelInstance(DatabaseInterface):
     def __new__(cls):
         instance = super().__new__(cls)
         return instance.Base
```

### Comparing `BlockFrame-0.1.4/BlockFrame.egg-info/SOURCES.txt` & `BlockFrame-1.0.0/BlockFrame.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,13 +5,14 @@
 BlockFrame.egg-info/SOURCES.txt
 BlockFrame.egg-info/dependency_links.txt
 BlockFrame.egg-info/requires.txt
 BlockFrame.egg-info/top_level.txt
 BlockFrame/chunking_service/__init__.py
 BlockFrame/chunking_service/chunking.py
 BlockFrame/chunking_service/config.py
+BlockFrame/chunking_service/fetcher.py
 BlockFrame/database_service/__init__.py
 BlockFrame/database_service/database.py
 BlockFrame/database_service/defaultmodel.py
 BlockFrame/database_service/getters.py
 BlockFrame/database_service/initalisation.py
 BlockFrame/database_service/setters.py
```

