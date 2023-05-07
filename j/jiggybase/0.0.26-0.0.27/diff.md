# Comparing `tmp/jiggybase-0.0.26.tar.gz` & `tmp/jiggybase-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.0.26.tar", last modified: Sun May  7 03:07:59 2023, max compression
+gzip compressed data, was "jiggybase-0.0.27.tar", last modified: Sun May  7 04:38:19 2023, max compression
```

## Comparing `jiggybase-0.0.26.tar` & `jiggybase-0.0.27.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 03:07:59.301152 jiggybase-0.0.26/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.26/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     6715 2023-05-07 03:07:59.300901 jiggybase-0.0.26/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     6181 2023-05-05 04:06:19.000000 jiggybase-0.0.26/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 03:07:59.294922 jiggybase-0.0.26/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.26/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     2044 2023-05-01 01:40:42.000000 jiggybase-0.0.26/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)     9513 2023-05-07 03:05:39.000000 jiggybase-0.0.26/jiggybase/collection.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 03:07:59.296968 jiggybase-0.0.26/jiggybase/examples/
--rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.0.26/jiggybase/examples/jiggybase_upload.py
--rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.26/jiggybase/examples/upload_email_example.py
--rw-r--r--   0 wsk        (501) staff       (20)     4531 2023-04-29 04:12:14.000000 jiggybase-0.0.26/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.26/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 03:07:59.300365 jiggybase-0.0.26/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.26/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.26/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.26/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.26/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.26/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.26/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.26/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.26/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.26/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     3706 2023-05-07 02:56:23.000000 jiggybase-0.0.26/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.26/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.26/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.26/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.26/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.26/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 03:07:59.296473 jiggybase-0.0.26/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     6715 2023-05-07 03:07:59.000000 jiggybase-0.0.26/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      852 2023-05-07 03:07:59.000000 jiggybase-0.0.26/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-07 03:07:59.000000 jiggybase-0.0.26/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-07 03:07:59.000000 jiggybase-0.0.26/jiggybase.egg-info/entry_points.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-07 03:07:59.000000 jiggybase-0.0.26/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-07 03:07:59.000000 jiggybase-0.0.26/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-07 02:54:47.000000 jiggybase-0.0.26/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-07 03:07:59.301224 jiggybase-0.0.26/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 03:07:59.300606 jiggybase-0.0.26/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.26/test/test.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 04:38:19.866749 jiggybase-0.0.27/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.27/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     6715 2023-05-07 04:38:19.866240 jiggybase-0.0.27/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     6181 2023-05-05 04:06:19.000000 jiggybase-0.0.27/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 04:38:19.856720 jiggybase-0.0.27/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.27/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2044 2023-05-01 01:40:42.000000 jiggybase-0.0.27/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)     9498 2023-05-07 04:35:02.000000 jiggybase-0.0.27/jiggybase/collection.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 04:38:19.859101 jiggybase-0.0.27/jiggybase/examples/
+-rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.0.27/jiggybase/examples/jiggybase_upload.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.27/jiggybase/examples/upload_email_example.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4531 2023-04-29 04:12:14.000000 jiggybase-0.0.27/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.27/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 04:38:19.865017 jiggybase-0.0.27/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.27/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.27/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.27/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.27/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.27/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.27/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.27/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.27/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.27/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3166 2023-05-07 04:31:10.000000 jiggybase-0.0.27/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.27/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.27/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.27/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.27/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.27/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 04:38:19.858364 jiggybase-0.0.27/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     6715 2023-05-07 04:38:19.000000 jiggybase-0.0.27/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      852 2023-05-07 04:38:19.000000 jiggybase-0.0.27/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-07 04:38:19.000000 jiggybase-0.0.27/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-07 04:38:19.000000 jiggybase-0.0.27/jiggybase.egg-info/entry_points.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-07 04:38:19.000000 jiggybase-0.0.27/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-07 04:38:19.000000 jiggybase-0.0.27/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-07 04:37:31.000000 jiggybase-0.0.27/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-07 04:38:19.866877 jiggybase-0.0.27/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 04:38:19.865643 jiggybase-0.0.27/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.27/test/test.py
```

### Comparing `jiggybase-0.0.26/LICENSE` & `jiggybase-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/PKG-INFO` & `jiggybase-0.0.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.26
+Version: 0.0.27
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.26/README.md` & `jiggybase-0.0.27/README.md`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/jiggybase/client.py` & `jiggybase-0.0.27/jiggybase/client.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/jiggybase/collection.py` & `jiggybase-0.0.27/jiggybase/collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional, Tuple, List
 from pydantic import BaseModel, Field, BaseConfig, HttpUrl
 from enum import Enum
 from .models import collection, CollectionChatConfig, PatchCollectionChatConfig
 from .jiggybase_session import JiggyBaseSession
-from .models import UpsertResponse,  Query, QueryRequest, QueryResponse, UpsertRequest, Document, DocumentChunk, DeleteRequest, DeleteResponse, DocumentMetadataFilter, DocChunksRequest, DocChunksResponse
+from .models import UpsertResponse,  Query, QueryRequest, QueryResponse, UpsertRequest, Document, DocumentChunk, DeleteRequest, DeleteResponse, DocumentMetadataFilter, DocChunksResponse
 import os
 import mimetypes
 
 from typing import Union, List
 class PluginAuthType(Enum):
     bearer :str = "bearer"
     none   :str = "none"
@@ -173,16 +173,16 @@
         """
         low level interface for iterating through the chunks in a collection
         index - index of the first result to return, should be -1 to start at the end
         limit - Number of results to return starting from the offset
         reverse - Reverse the order of the items returned; True to return newest first
         max_chunks_per_doc - maximum number of chunks to return for each document
         """
-        dcr = DocChunksRequest(index=index, limit=limit, reverse=reverse, max_chunks_per_doc=max_chunks_per_doc)
-        rsp = self.plugin_session.get("/doc_chunks", model=dcr)
+        params = {"index": index, "limit": limit, "reverse": reverse, "max_chunks_per_doc": max_chunks_per_doc}
+        rsp = self.plugin_session.get("/doc_chunks", params=params)
         dcr_rsp = DocChunksResponse.parse_obj(rsp.json())
         return dcr_rsp.docs, dcr_rsp.next_index
 
 
     def delete_docs(self, 
                     ids                      : Optional[List[str]] = None, 
                     document_metadata_filter : Optional[DocumentMetadataFilter] = None,
```

### Comparing `jiggybase-0.0.26/jiggybase/examples/jiggybase_upload.py` & `jiggybase-0.0.27/jiggybase/examples/jiggybase_upload.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/jiggybase/examples/upload_email_example.py` & `jiggybase-0.0.27/jiggybase/examples/upload_email_example.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/jiggybase/jiggybase_session.py` & `jiggybase-0.0.27/jiggybase/jiggybase_session.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/jiggybase/login.py` & `jiggybase-0.0.27/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/jiggybase/models/auth.py` & `jiggybase-0.0.27/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/jiggybase/models/chat.py` & `jiggybase-0.0.27/jiggybase/models/chat.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/jiggybase/models/chunk.py` & `jiggybase-0.0.27/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/jiggybase/models/collection.py` & `jiggybase-0.0.27/jiggybase/models/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/jiggybase/models/metadata.py` & `jiggybase-0.0.27/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/jiggybase/models/org.py` & `jiggybase-0.0.27/jiggybase/models/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/jiggybase/models/plugin.py` & `jiggybase-0.0.27/jiggybase/models/plugin.py`

 * *Files 19% similar despite different names*

```diff
@@ -115,18 +115,11 @@
 class Accounting(BaseModel):
     chunk_count: int
     doc_count: int
     page_count: int
 
 
 
-
-class DocChunksRequest(BaseModel):
-    index              : int = Field(-1,    description="The index of the first document to return.  Use 0 to start at the beginning.  Use -1 to start at the end.")
-    limit              : int = Field(10,    description="The maximum number of documents to return")
-    max_chunks_per_doc : int = Field(1,     description="The maximum number of chunks to return per document")
-    reverse            : bool = Field(True, description="If true, return documents in reverse order with most recent First.")
-
 class DocChunksResponse(BaseModel):
     docs       : list[list[DocumentChunk]] = Field(..., description="A list of documents, each containing a list of chunks")
     next_index : int                       = Field(..., description="The index of the next document to return.  Use this value as the index parameter in the next request to get the next set of documents")
```

### Comparing `jiggybase-0.0.26/jiggybase/models/plugin_config.py` & `jiggybase-0.0.27/jiggybase/models/plugin_config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/jiggybase/models/prompt.py` & `jiggybase-0.0.27/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/jiggybase/models/providers.py` & `jiggybase-0.0.27/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/jiggybase/models/user.py` & `jiggybase-0.0.27/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/jiggybase/org.py` & `jiggybase-0.0.27/jiggybase/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/jiggybase.egg-info/PKG-INFO` & `jiggybase-0.0.27/jiggybase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.26
+Version: 0.0.27
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.26/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.0.27/jiggybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.26/pyproject.toml` & `jiggybase-0.0.27/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.0.26"
+version = "0.0.27"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pydantic[email]', 'requests']
 description = "Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `jiggybase-0.0.26/test/test.py` & `jiggybase-0.0.27/test/test.py`

 * *Files identical despite different names*

