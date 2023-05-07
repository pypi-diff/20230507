# Comparing `tmp/embedbase_qdrant-1.0.0.tar.gz` & `tmp/embedbase_qdrant-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase_qdrant-1.0.0.tar", max compression
+gzip compressed data, was "embedbase_qdrant-1.0.1.tar", max compression
```

## Comparing `embedbase_qdrant-1.0.0.tar` & `embedbase_qdrant-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      130 2023-05-05 16:52:16.598811 embedbase_qdrant-1.0.0/README.md
--rw-r--r--   0        0        0       30 2023-05-05 16:52:16.598811 embedbase_qdrant-1.0.0/embedbase_qdrant/__init__.py
--rw-r--r--   0        0        0     8969 2023-05-05 16:52:16.598811 embedbase_qdrant-1.0.0/embedbase_qdrant/qdrant_db.py
--rw-r--r--   0        0        0     3237 2023-05-05 16:52:16.598811 embedbase_qdrant-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 embedbase_qdrant-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2082 2023-05-07 10:48:31.978185 embedbase_qdrant-1.0.1/README.md
+-rw-r--r--   0        0        0       30 2023-05-07 10:48:31.978185 embedbase_qdrant-1.0.1/embedbase_qdrant/__init__.py
+-rw-r--r--   0        0        0    10831 2023-05-07 10:48:31.978185 embedbase_qdrant-1.0.1/embedbase_qdrant/qdrant_db.py
+-rw-r--r--   0        0        0     3237 2023-05-07 10:48:32.014185 embedbase_qdrant-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3343 1970-01-01 00:00:00.000000 embedbase_qdrant-1.0.1/PKG-INFO
```

### Comparing `embedbase_qdrant-1.0.0/embedbase_qdrant/qdrant_db.py` & `embedbase_qdrant-1.0.1/embedbase_qdrant/qdrant_db.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import asyncio
 from embedbase.database import VectorDatabase
-from typing import Coroutine, List, Optional
+from typing import Union, List, Optional
 from pandas import DataFrame
 from embedbase.utils import BatchGenerator
 from qdrant_client import QdrantClient
 from qdrant_client.http.models import PointStruct
 from qdrant_client.http.models import (
     Filter,
     FieldCondition,
     MatchValue,
-    PointIdsList,
     FilterSelector,
     VectorParams,
     Distance,
     HasIdCondition,
+    Record,
 )
 from qdrant_client.http.exceptions import UnexpectedResponse
-
+import itertools
 from embedbase.database.base import SearchResponse, SelectResponse, Dataset
 from typing import Callable, TypeVar
 
 T = TypeVar("T")
 
 
 class Qdrant(VectorDatabase):
@@ -51,26 +51,65 @@
                 raise exc
             self.client.create_collection(
                 collection_name=dataset_id,
                 vectors_config=VectorParams(
                     size=self._dimensions, distance=Distance.COSINE
                 ),
             )
+            self._collections.add(dataset_id)
             return func(**kwargs)
 
     def __init__(self, host: str = "localhost", port: int = 6333, **kwargs):
         """
 
         :param host: qdrant host
         :param port: qdrant port
         """
 
         super().__init__(**kwargs)
 
         self.client = QdrantClient(host=host, port=port)
+        self._collections = set()
+        cols = self.client.get_collections().collections
+        for col in cols:
+            self._collections.add(col.name)
+        print(f"Qdrant collections: {self._collections}")
+
+    async def _multi_collections_scroll(
+        self,
+        collections: List[str],
+        query_filter: Filter,
+        with_payload: bool = True,
+        with_vectors: bool = True,
+        limit: int = 10_000,
+    ) -> List[Record]:
+        """
+        Scroll through multiple collections
+        :param collections: list of collections
+        :param query_filter: query filter
+        :param with_payload: with payload
+        :param with_vectors: with vectors
+        :param limit: scroll size
+        :return: list of points
+        """
+        # scroll multiple collections in parallel
+
+        async def _scroll(collection_name: str) -> List[Record]:
+            records, _ = self.client.scroll(
+                collection_name=collection_name,
+                query_filter=query_filter,
+                with_payload=with_payload,
+                with_vectors=with_vectors,
+                limit=limit,
+            )
+            return records
+
+        results = await asyncio.gather(*[_scroll(col) for col in collections])
+        results = list(itertools.chain(*results))
+        return results
 
     async def select(
         self,
         ids: List[str] = [],
         hashes: List[str] = [],
         dataset_id: Optional[str] = None,
         user_id: Optional[str] = None,
@@ -96,40 +135,45 @@
         if hashes:
             for h in hashes:
                 should.append(FieldCondition(key="hash", match=MatchValue(value=h)))
         if ids:
             should.append(HasIdCondition(has_id=ids))
 
         try:
-            search_result = self.client.scroll(
-                collection_name=dataset_id,
-                # query_vector=[0.0] * self._dimensions,
+            scroll_results = await self._multi_collections_scroll(
+                collections=[dataset_id] or list(self._collections),
                 query_filter=Filter(
                     should=should,
                     must=must,
                 ),
                 with_payload=True,
                 with_vectors=True,
                 # TODO pagination
                 limit=10_000,
             )
+            if distinct:
+                if ids:
+                    scroll_results = {e.id: e for e in scroll_results}
+                elif hashes:
+                    scroll_results = {e.payload["hash"]: e for e in scroll_results}
+                scroll_results = list(scroll_results.values())
         except UnexpectedResponse as exc:
             # ignore unexisting collections
             if exc.status_code != 404:
                 raise exc
             return []
         responses = []
-        for e in search_result[0]:
+        for record in scroll_results:
             responses.append(
                 SelectResponse(
-                    id=e.id,
-                    data=e.payload.get("data"),
-                    metadata=e.payload.get("metadata"),
-                    hash=e.payload.get("hash"),
-                    embedding=e.vector,
+                    id=record.id,
+                    data=record.payload.get("data"),
+                    metadata=record.payload.get("metadata"),
+                    hash=record.payload.get("hash"),
+                    embedding=record.vector,
                 )
             )
         return responses
 
     async def update(
         self,
         df: DataFrame,
@@ -146,15 +190,15 @@
             points = [
                 PointStruct(
                     id=row.id,
                     vector=row.embedding,
                     payload={
                         "dataset_id": dataset_id,
                         "user_id": user_id,
-                        "metadata": row.metadata,
+                        "metadata": row.metadata or {},
                         "data": row.data,
                         "hash": row.hash,
                     },
                 )
                 for _, row in batch_df.iterrows()
             ]
 
@@ -197,15 +241,18 @@
 
     async def search(
         self,
         vector: List[float],
         top_k: Optional[int],
         dataset_ids: List[str],
         user_id: Optional[str] = None,
+        where: Optional[Union[dict, List[dict]]] = None,
     ):
+        if where:
+            raise NotImplementedError("where is not implemented yet in embedbase-qdrant")
         must = []
         if user_id:
             must.append(
                 FieldCondition(key="user_id", range=MatchValue(value="user_id"))
             )
         try:
             search_result = self.client.search(
```

### Comparing `embedbase_qdrant-1.0.0/pyproject.toml` & `embedbase_qdrant-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [virtualenvs]
 create = true
 in-project = true
 
 [tool.poetry]
 name = "embedbase_qdrant"
-version = "1.0.0"
+version = "1.0.1"
 description = "Embedbase + Qdrant - Advanced and high-performant vector similarity search technology in your AI applications."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase-qdrant"
 homepage = "https://github.com/different-ai/embedbase-qdrant"
 keywords = ["embeddings", "machine learning", "artificial intelligence"]
```

