# Comparing `tmp/jiggybase-0.0.25.tar.gz` & `tmp/jiggybase-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.0.25.tar", last modified: Fri May  5 02:03:04 2023, max compression
+gzip compressed data, was "jiggybase-0.0.26.tar", last modified: Sun May  7 03:07:59 2023, max compression
```

## Comparing `jiggybase-0.0.25.tar` & `jiggybase-0.0.26.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 02:03:04.494290 jiggybase-0.0.25/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.25/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     5826 2023-05-05 02:03:04.493904 jiggybase-0.0.25/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     5292 2023-05-01 15:45:10.000000 jiggybase-0.0.25/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 02:03:04.484206 jiggybase-0.0.25/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.25/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     2044 2023-05-01 01:40:42.000000 jiggybase-0.0.25/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)     8508 2023-04-30 00:50:55.000000 jiggybase-0.0.25/jiggybase/collection.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 02:03:04.487116 jiggybase-0.0.25/jiggybase/examples/
--rwxr-xr-x   0 wsk        (501) staff       (20)     3383 2023-05-05 01:59:33.000000 jiggybase-0.0.25/jiggybase/examples/jiggybase_upload.py
--rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.25/jiggybase/examples/upload_email_example.py
--rw-r--r--   0 wsk        (501) staff       (20)     4531 2023-04-29 04:12:14.000000 jiggybase-0.0.25/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.25/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 02:03:04.492954 jiggybase-0.0.25/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.25/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.25/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.25/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.25/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.25/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.25/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.25/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.25/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.25/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     2777 2023-04-29 00:07:44.000000 jiggybase-0.0.25/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.25/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.25/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.25/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.25/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.25/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 02:03:04.486263 jiggybase-0.0.25/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     5826 2023-05-05 02:03:04.000000 jiggybase-0.0.25/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      852 2023-05-05 02:03:04.000000 jiggybase-0.0.25/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-05 02:03:04.000000 jiggybase-0.0.25/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-05 02:03:04.000000 jiggybase-0.0.25/jiggybase.egg-info/entry_points.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-05 02:03:04.000000 jiggybase-0.0.25/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-05 02:03:04.000000 jiggybase-0.0.25/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-05 01:22:51.000000 jiggybase-0.0.25/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-05 02:03:04.494400 jiggybase-0.0.25/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 02:03:04.493383 jiggybase-0.0.25/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.25/test/test.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 03:07:59.301152 jiggybase-0.0.26/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.26/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     6715 2023-05-07 03:07:59.300901 jiggybase-0.0.26/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     6181 2023-05-05 04:06:19.000000 jiggybase-0.0.26/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 03:07:59.294922 jiggybase-0.0.26/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.26/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2044 2023-05-01 01:40:42.000000 jiggybase-0.0.26/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)     9513 2023-05-07 03:05:39.000000 jiggybase-0.0.26/jiggybase/collection.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 03:07:59.296968 jiggybase-0.0.26/jiggybase/examples/
+-rwxr-xr-x   0 wsk        (501) staff       (20)     3381 2023-05-05 04:06:34.000000 jiggybase-0.0.26/jiggybase/examples/jiggybase_upload.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.26/jiggybase/examples/upload_email_example.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4531 2023-04-29 04:12:14.000000 jiggybase-0.0.26/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.26/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 03:07:59.300365 jiggybase-0.0.26/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.26/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.26/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.26/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.26/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.26/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.26/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.26/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.26/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.26/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3706 2023-05-07 02:56:23.000000 jiggybase-0.0.26/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.26/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.26/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.26/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.26/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.26/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 03:07:59.296473 jiggybase-0.0.26/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     6715 2023-05-07 03:07:59.000000 jiggybase-0.0.26/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      852 2023-05-07 03:07:59.000000 jiggybase-0.0.26/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-07 03:07:59.000000 jiggybase-0.0.26/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-07 03:07:59.000000 jiggybase-0.0.26/jiggybase.egg-info/entry_points.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-07 03:07:59.000000 jiggybase-0.0.26/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-07 03:07:59.000000 jiggybase-0.0.26/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-07 02:54:47.000000 jiggybase-0.0.26/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-07 03:07:59.301224 jiggybase-0.0.26/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-07 03:07:59.300606 jiggybase-0.0.26/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.26/test/test.py
```

### Comparing `jiggybase-0.0.25/LICENSE` & `jiggybase-0.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.25/PKG-INFO` & `jiggybase-0.0.26/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.25
+Version: 0.0.26
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -105,7 +105,25 @@
 JiggyBase supports user-customized prompts for the JiggyBase ChatCompletion API.   The following methods are provided to manage the customized prompts.
 
 - `prompt_tasks([name=None, version=None])` - Returns a list of `PromptTask` objects, optionally filtering by name and version.
 - `create_prompt_task(name: str, version: int, prompts: List[PromptMessage][, type: Optional[PromptTaskType] = None, description: Optional[str] = None])` - Creates a new `PromptTask` object with the specified parameters.
 - `update_prompt_task(name: str, prompts: List[PromptMessage])` - Updates the specified prompt task's prompts.
 - `get_prompt_task(prompt_task_id: int)` - Retrieves a `PromptTask` object using the given prompt_task_id.
 - `delete_prompt_task(prompt_task_id: int)` - Deletes a `PromptTask` object using the given prompt_task_id.
+
+## jiggybase_upload
+
+This utility is installed via pip and allows you to upload files or directories to your JiggyBase collection using command-line arguments. It's included in the `jiggybase/examples` directory.
+
+#### Usage
+
+```bash
+jiggybase_upload [--org <organization>] [--collection <collection>] [--dir <directory>] [--file <file>]
+```
+
+- `--org`: The name of your JiggyBase organization. Alternatively, set `JIGGYBASE_ORG` environment variable, or be a member of a single organization.
+- `--collection`: The name of your JiggyBase collection. Alternatively, set the `JIGGYBASE_COLLECTION` environment variable, or have a single collection in your organization.
+- `--dir`: The directory you want to upload.
+- `--file`: The file you want to upload.
+
+If neither `--file` nor `--dir` options are provided, the script will automatically process other arguments as a file or directory.
+
```

### Comparing `jiggybase-0.0.25/README.md` & `jiggybase-0.0.26/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -91,7 +91,25 @@
 JiggyBase supports user-customized prompts for the JiggyBase ChatCompletion API.   The following methods are provided to manage the customized prompts.
 
 - `prompt_tasks([name=None, version=None])` - Returns a list of `PromptTask` objects, optionally filtering by name and version.
 - `create_prompt_task(name: str, version: int, prompts: List[PromptMessage][, type: Optional[PromptTaskType] = None, description: Optional[str] = None])` - Creates a new `PromptTask` object with the specified parameters.
 - `update_prompt_task(name: str, prompts: List[PromptMessage])` - Updates the specified prompt task's prompts.
 - `get_prompt_task(prompt_task_id: int)` - Retrieves a `PromptTask` object using the given prompt_task_id.
 - `delete_prompt_task(prompt_task_id: int)` - Deletes a `PromptTask` object using the given prompt_task_id.
+
+## jiggybase_upload
+
+This utility is installed via pip and allows you to upload files or directories to your JiggyBase collection using command-line arguments. It's included in the `jiggybase/examples` directory.
+
+#### Usage
+
+```bash
+jiggybase_upload [--org <organization>] [--collection <collection>] [--dir <directory>] [--file <file>]
+```
+
+- `--org`: The name of your JiggyBase organization. Alternatively, set `JIGGYBASE_ORG` environment variable, or be a member of a single organization.
+- `--collection`: The name of your JiggyBase collection. Alternatively, set the `JIGGYBASE_COLLECTION` environment variable, or have a single collection in your organization.
+- `--dir`: The directory you want to upload.
+- `--file`: The file you want to upload.
+
+If neither `--file` nor `--dir` options are provided, the script will automatically process other arguments as a file or directory.
+
```

### Comparing `jiggybase-0.0.25/jiggybase/client.py` & `jiggybase-0.0.26/jiggybase/client.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.25/jiggybase/collection.py` & `jiggybase-0.0.26/jiggybase/collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Optional
+from typing import Optional, Tuple, List
 from pydantic import BaseModel, Field, BaseConfig, HttpUrl
 from enum import Enum
 from .models import collection, CollectionChatConfig, PatchCollectionChatConfig
 from .jiggybase_session import JiggyBaseSession
-from .models import UpsertResponse,  Query, QueryRequest, QueryResponse, UpsertRequest, Document, DocumentChunk, DeleteRequest, DeleteResponse, DocumentMetadataFilter
+from .models import UpsertResponse,  Query, QueryRequest, QueryResponse, UpsertRequest, Document, DocumentChunk, DeleteRequest, DeleteResponse, DocumentMetadataFilter, DocChunksRequest, DocChunksResponse
 import os
 import mimetypes
 
 from typing import Union, List
 class PluginAuthType(Enum):
     bearer :str = "bearer"
     none   :str = "none"
@@ -161,14 +161,31 @@
         limit - Number of results to return starting from the offset
         reverse - Reverse the order of the items returned
         """
         params = {"start": start, "limit": limit, "reverse": reverse}
         rsp = self.plugin_session.get("/chunks", params=params)
         return [DocumentChunk.parse_obj(chunk) for chunk in rsp.json()]
 
+    def get_doc_chunks(self, 
+                       index: int = -1, 
+                       limit: int = 10, 
+                       reverse: bool = True,
+                       max_chunks_per_doc = 1) -> Tuple[List[List[DocumentChunk]], int]:
+        """
+        low level interface for iterating through the chunks in a collection
+        index - index of the first result to return, should be -1 to start at the end
+        limit - Number of results to return starting from the offset
+        reverse - Reverse the order of the items returned; True to return newest first
+        max_chunks_per_doc - maximum number of chunks to return for each document
+        """
+        dcr = DocChunksRequest(index=index, limit=limit, reverse=reverse, max_chunks_per_doc=max_chunks_per_doc)
+        rsp = self.plugin_session.get("/doc_chunks", model=dcr)
+        dcr_rsp = DocChunksResponse.parse_obj(rsp.json())
+        return dcr_rsp.docs, dcr_rsp.next_index
+
 
     def delete_docs(self, 
                     ids                      : Optional[List[str]] = None, 
                     document_metadata_filter : Optional[DocumentMetadataFilter] = None, 
                     delete_all               : Optional[bool] = False) -> DeleteResponse:
         """
         Delete items in the collection by document id's or document metadata filter.
```

### Comparing `jiggybase-0.0.25/jiggybase/examples/jiggybase_upload.py` & `jiggybase-0.0.26/jiggybase/examples/jiggybase_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 def upload_directory(collection : jiggybase.models.Collection, dirname : str):
     for fn in os.listdir(dirname):
         fn = os.path.join(dirname, fn)
         upload_file(collection, fn)
 
 
-epilog = "If neither '--file' nor '--dir' options are provided, the script will automatically process the last argument as a file or directory"
+epilog = "If neither '--file' nor '--dir' options are provided, the script will automatically process other arguments as a file or directory"
 
 
 def main():
     parser = argparse.ArgumentParser(description="Upload a file or directory to a JiggyBase collection",  epilog=epilog )    
     parser.add_argument("--org", type=str, help="The name of your JiggyBase organization.  Alternatively, set JIGGYBASE_ORG environment variable or be a member of a single Org.")
     parser.add_argument("--collection", type=str, help="The name of your JiggyBase collection. Alternatively, set JIGGYBASE_COLLECTION environment variable or have a single collection in your org.")
     parser.add_argument("--dir", type=str, help="The directory you want to upload.")
```

### Comparing `jiggybase-0.0.25/jiggybase/examples/upload_email_example.py` & `jiggybase-0.0.26/jiggybase/examples/upload_email_example.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.25/jiggybase/jiggybase_session.py` & `jiggybase-0.0.26/jiggybase/jiggybase_session.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.25/jiggybase/login.py` & `jiggybase-0.0.26/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.25/jiggybase/models/auth.py` & `jiggybase-0.0.26/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.25/jiggybase/models/chat.py` & `jiggybase-0.0.26/jiggybase/models/chat.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.25/jiggybase/models/chunk.py` & `jiggybase-0.0.26/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.25/jiggybase/models/collection.py` & `jiggybase-0.0.26/jiggybase/models/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.25/jiggybase/models/metadata.py` & `jiggybase-0.0.26/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.25/jiggybase/models/org.py` & `jiggybase-0.0.26/jiggybase/models/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.25/jiggybase/models/plugin_config.py` & `jiggybase-0.0.26/jiggybase/models/plugin_config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.25/jiggybase/models/prompt.py` & `jiggybase-0.0.26/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.25/jiggybase/models/providers.py` & `jiggybase-0.0.26/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.25/jiggybase/models/user.py` & `jiggybase-0.0.26/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.25/jiggybase/org.py` & `jiggybase-0.0.26/jiggybase/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.25/jiggybase.egg-info/PKG-INFO` & `jiggybase-0.0.26/jiggybase.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.25
+Version: 0.0.26
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -105,7 +105,25 @@
 JiggyBase supports user-customized prompts for the JiggyBase ChatCompletion API.   The following methods are provided to manage the customized prompts.
 
 - `prompt_tasks([name=None, version=None])` - Returns a list of `PromptTask` objects, optionally filtering by name and version.
 - `create_prompt_task(name: str, version: int, prompts: List[PromptMessage][, type: Optional[PromptTaskType] = None, description: Optional[str] = None])` - Creates a new `PromptTask` object with the specified parameters.
 - `update_prompt_task(name: str, prompts: List[PromptMessage])` - Updates the specified prompt task's prompts.
 - `get_prompt_task(prompt_task_id: int)` - Retrieves a `PromptTask` object using the given prompt_task_id.
 - `delete_prompt_task(prompt_task_id: int)` - Deletes a `PromptTask` object using the given prompt_task_id.
+
+## jiggybase_upload
+
+This utility is installed via pip and allows you to upload files or directories to your JiggyBase collection using command-line arguments. It's included in the `jiggybase/examples` directory.
+
+#### Usage
+
+```bash
+jiggybase_upload [--org <organization>] [--collection <collection>] [--dir <directory>] [--file <file>]
+```
+
+- `--org`: The name of your JiggyBase organization. Alternatively, set `JIGGYBASE_ORG` environment variable, or be a member of a single organization.
+- `--collection`: The name of your JiggyBase collection. Alternatively, set the `JIGGYBASE_COLLECTION` environment variable, or have a single collection in your organization.
+- `--dir`: The directory you want to upload.
+- `--file`: The file you want to upload.
+
+If neither `--file` nor `--dir` options are provided, the script will automatically process other arguments as a file or directory.
+
```

### Comparing `jiggybase-0.0.25/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.0.26/jiggybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.25/pyproject.toml` & `jiggybase-0.0.26/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.0.25"
+version = "0.0.26"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pydantic[email]', 'requests']
 description = "Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `jiggybase-0.0.25/test/test.py` & `jiggybase-0.0.26/test/test.py`

 * *Files identical despite different names*

