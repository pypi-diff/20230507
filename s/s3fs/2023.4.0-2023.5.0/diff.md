# Comparing `tmp/s3fs-2023.4.0.tar.gz` & `tmp/s3fs-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3fs-2023.4.0.tar", last modified: Sat Apr  8 18:01:05 2023, max compression
+gzip compressed data, was "s3fs-2023.5.0.tar", last modified: Sun May  7 19:14:19 2023, max compression
```

## Comparing `s3fs-2023.4.0.tar` & `s3fs-2023.5.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 18:01:05.942296 s3fs-2023.4.0/
--rw-r--r--   0 mdurant    (502) staff       (20)     1505 2022-09-18 01:28:11.000000 s3fs-2023.4.0/LICENSE.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      225 2022-09-18 01:28:11.000000 s3fs-2023.4.0/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)     1341 2023-04-08 18:01:05.942373 s3fs-2023.4.0/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)      620 2022-09-18 01:28:11.000000 s3fs-2023.4.0/README.rst
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 18:01:05.935002 s3fs-2023.4.0/docs/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 18:01:05.938276 s3fs-2023.4.0/docs/source/
--rw-r--r--   0 mdurant    (502) staff       (20)      906 2023-02-23 19:42:13.000000 s3fs-2023.4.0/docs/source/api.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     4029 2023-04-08 17:52:10.000000 s3fs-2023.4.0/docs/source/changelog.rst
--rw-r--r--   0 mdurant    (502) staff       (20)      151 2022-09-18 01:28:11.000000 s3fs-2023.4.0/docs/source/development.rst
--rw-r--r--   0 mdurant    (502) staff       (20)    11489 2023-04-08 17:17:48.000000 s3fs-2023.4.0/docs/source/index.rst
--rw-r--r--   0 mdurant    (502) staff       (20)      530 2022-09-18 01:28:11.000000 s3fs-2023.4.0/docs/source/install.rst
--rw-r--r--   0 mdurant    (502) staff       (20)       64 2023-04-08 17:51:12.000000 s3fs-2023.4.0/requirements.txt
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 18:01:05.942981 s3fs-2023.4.0/s3fs/
--rw-r--r--   0 mdurant    (502) staff       (20)      160 2022-09-18 01:28:11.000000 s3fs-2023.4.0/s3fs/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      500 2023-04-08 18:01:05.943035 s3fs-2023.4.0/s3fs/_version.py
--rw-r--r--   0 mdurant    (502) staff       (20)    83227 2023-04-08 17:48:33.000000 s3fs-2023.4.0/s3fs/core.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7779 2022-09-18 01:28:11.000000 s3fs-2023.4.0/s3fs/errors.py
--rw-r--r--   0 mdurant    (502) staff       (20)      237 2022-09-18 01:28:11.000000 s3fs-2023.4.0/s3fs/mapping.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 18:01:05.942162 s3fs-2023.4.0/s3fs/tests/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:11.000000 s3fs-2023.4.0/s3fs/tests/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2859 2022-09-18 01:28:11.000000 s3fs-2023.4.0/s3fs/tests/test_mapping.py
--rw-r--r--   0 mdurant    (502) staff       (20)    78932 2023-04-08 17:48:28.000000 s3fs-2023.4.0/s3fs/tests/test_s3fs.py
--rw-r--r--   0 mdurant    (502) staff       (20)      370 2022-09-18 01:28:11.000000 s3fs-2023.4.0/s3fs/tests/test_utils.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5246 2023-01-02 15:39:19.000000 s3fs-2023.4.0/s3fs/utils.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 18:01:05.941203 s3fs-2023.4.0/s3fs.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     1341 2023-04-08 18:01:05.000000 s3fs-2023.4.0/s3fs.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)      561 2023-04-08 18:01:05.000000 s3fs-2023.4.0/s3fs.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-04-08 18:01:05.000000 s3fs-2023.4.0/s3fs.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-10-19 15:15:30.000000 s3fs-2023.4.0/s3fs.egg-info/not-zip-safe
--rw-r--r--   0 mdurant    (502) staff       (20)      135 2023-04-08 18:01:05.000000 s3fs-2023.4.0/s3fs.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        5 2023-04-08 18:01:05.000000 s3fs-2023.4.0/s3fs.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      438 2023-04-08 18:01:05.942749 s3fs-2023.4.0/setup.cfg
--rwxr-xr-x   0 mdurant    (502) staff       (20)     1365 2023-02-23 19:42:13.000000 s3fs-2023.4.0/setup.py
--rw-r--r--   0 mdurant    (502) staff       (20)    78281 2022-09-18 01:28:11.000000 s3fs-2023.4.0/versioneer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:14:19.290045 s3fs-2023.5.0/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1505 2022-09-18 01:28:11.000000 s3fs-2023.5.0/LICENSE.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      225 2022-09-18 01:28:11.000000 s3fs-2023.5.0/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     1341 2023-05-07 19:14:19.290121 s3fs-2023.5.0/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      620 2022-09-18 01:28:11.000000 s3fs-2023.5.0/README.rst
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:14:19.282518 s3fs-2023.5.0/docs/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:14:19.285810 s3fs-2023.5.0/docs/source/
+-rw-r--r--   0 mdurant    (502) staff       (20)      906 2023-02-23 19:42:13.000000 s3fs-2023.5.0/docs/source/api.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     4290 2023-05-07 19:13:40.000000 s3fs-2023.5.0/docs/source/changelog.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)      151 2022-09-18 01:28:11.000000 s3fs-2023.5.0/docs/source/development.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)    11489 2023-04-25 15:48:31.000000 s3fs-2023.5.0/docs/source/index.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)      530 2022-09-18 01:28:11.000000 s3fs-2023.5.0/docs/source/install.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)       64 2023-05-07 19:13:40.000000 s3fs-2023.5.0/requirements.txt
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:14:19.290876 s3fs-2023.5.0/s3fs/
+-rw-r--r--   0 mdurant    (502) staff       (20)      160 2022-09-18 01:28:11.000000 s3fs-2023.5.0/s3fs/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      500 2023-05-07 19:14:19.290935 s3fs-2023.5.0/s3fs/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    82930 2023-05-05 14:01:13.000000 s3fs-2023.5.0/s3fs/core.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7779 2022-09-18 01:28:11.000000 s3fs-2023.5.0/s3fs/errors.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      237 2022-09-18 01:28:11.000000 s3fs-2023.5.0/s3fs/mapping.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:14:19.289887 s3fs-2023.5.0/s3fs/tests/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:11.000000 s3fs-2023.5.0/s3fs/tests/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2859 2022-09-18 01:28:11.000000 s3fs-2023.5.0/s3fs/tests/test_mapping.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    79706 2023-05-05 14:56:21.000000 s3fs-2023.5.0/s3fs/tests/test_s3fs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      370 2022-09-18 01:28:11.000000 s3fs-2023.5.0/s3fs/tests/test_utils.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5246 2023-01-02 15:39:19.000000 s3fs-2023.5.0/s3fs/utils.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:14:19.288810 s3fs-2023.5.0/s3fs.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1341 2023-05-07 19:14:19.000000 s3fs-2023.5.0/s3fs.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      561 2023-05-07 19:14:19.000000 s3fs-2023.5.0/s3fs.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-05-07 19:14:19.000000 s3fs-2023.5.0/s3fs.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-10-19 15:15:30.000000 s3fs-2023.5.0/s3fs.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)      135 2023-05-07 19:14:19.000000 s3fs-2023.5.0/s3fs.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        5 2023-05-07 19:14:19.000000 s3fs-2023.5.0/s3fs.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      438 2023-05-07 19:14:19.290481 s3fs-2023.5.0/setup.cfg
+-rwxr-xr-x   0 mdurant    (502) staff       (20)     1365 2023-02-23 19:42:13.000000 s3fs-2023.5.0/setup.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    78281 2022-09-18 01:28:11.000000 s3fs-2023.5.0/versioneer.py
```

### Comparing `s3fs-2023.4.0/LICENSE.txt` & `s3fs-2023.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `s3fs-2023.4.0/PKG-INFO` & `s3fs-2023.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3fs
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: Convenient Filesystem interface over S3
 Home-page: http://github.com/fsspec/s3fs/
 Maintainer: Martin Durant
 Maintainer-email: mdurant@continuum.io
 License: BSD
 Keywords: s3,boto
 Classifier: Development Status :: 4 - Beta
```

### Comparing `s3fs-2023.4.0/README.rst` & `s3fs-2023.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `s3fs-2023.4.0/docs/source/api.rst` & `s3fs-2023.5.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `s3fs-2023.4.0/docs/source/changelog.rst` & `s3fs-2023.5.0/docs/source/changelog.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+2023.5.0
+--------
+
+- Fix "_" in xattrs tests (#732)
+- Fix file pointer already at end of file when retrying put (#731)
+- Fix repeated find corrupting cache (#730)
+- Remove duplicate class definition (#727)
+- return list of deleted keys in bulk deleted (#726)
+
+
 2023.4.0
 --------
 
 - Add streaming async read file (#722)
 - Doc fixes (#721)
 - aiobotocore to 2.5.0 (#710)
```

### Comparing `s3fs-2023.4.0/docs/source/index.rst` & `s3fs-2023.5.0/docs/source/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 --------
 
 Simple locate and read a file:
 
 .. code-block:: python
 
    >>> import s3fs
-   >>> fs = s3fs.S3FileSystem(anon=True)
-   >>> fs.ls('my-bucket')
+   >>> s3 = s3fs.S3FileSystem(anon=True)
+   >>> s3.ls('my-bucket')
    ['my-file.txt']
-   >>> with fs.open('my-bucket/my-file.txt', 'rb') as f:
+   >>> with s3.open('my-bucket/my-file.txt', 'rb') as f:
    ...     print(f.read())
    b'Hello, world'
 
 (see also ``walk`` and ``glob``)
 
 Reading with delimited blocks:
```

### Comparing `s3fs-2023.4.0/docs/source/install.rst` & `s3fs-2023.5.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `s3fs-2023.4.0/s3fs/core.py` & `s3fs-2023.5.0/s3fs/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -816,33 +816,32 @@
             except FileNotFoundError:
                 out = []
         dirs = []
         sdirs = set()
         thisdircache = {}
         for o in out:
             par = self._parent(o["name"])
-            if par not in self.dircache:
-                if par not in sdirs:
-                    sdirs.add(par)
-                    d = False
-                    if len(path) <= len(par):
-                        d = {
-                            "Key": self.split_path(par)[1],
-                            "Size": 0,
-                            "name": par,
-                            "StorageClass": "DIRECTORY",
-                            "type": "directory",
-                            "size": 0,
-                        }
-                        dirs.append(d)
-                    thisdircache[par] = []
-                    ppar = self._parent(par)
-                    if ppar in thisdircache:
-                        if d and d not in thisdircache[ppar]:
-                            thisdircache[ppar].append(d)
+            if par not in sdirs:
+                sdirs.add(par)
+                d = False
+                if len(path) <= len(par):
+                    d = {
+                        "Key": self.split_path(par)[1],
+                        "Size": 0,
+                        "name": par,
+                        "StorageClass": "DIRECTORY",
+                        "type": "directory",
+                        "size": 0,
+                    }
+                    dirs.append(d)
+                thisdircache[par] = []
+                ppar = self._parent(par)
+                if ppar in thisdircache:
+                    if d and d not in thisdircache[ppar]:
+                        thisdircache[ppar].append(d)
             if par in sdirs:
                 thisdircache[par].append(o)
         if not prefix:
             for k, v in thisdircache.items():
                 if k not in self.dircache and len(k) >= len(path):
                     self.dircache[k] = v
         if withdirs:
@@ -1104,16 +1103,17 @@
         if "ContentType" not in kwargs:
             content_type, _ = mimetypes.guess_type(lpath)
             if content_type is not None:
                 kwargs["ContentType"] = content_type
 
         with open(lpath, "rb") as f0:
             if size < min(5 * 2**30, 2 * chunksize):
+                chunk = f0.read()
                 await self._call_s3(
-                    "put_object", Bucket=bucket, Key=key, Body=f0, **kwargs
+                    "put_object", Bucket=bucket, Key=key, Body=chunk, **kwargs
                 )
                 callback.relative_update(size)
             else:
 
                 mpu = await self._call_s3(
                     "create_multipart_upload", Bucket=bucket, Key=key, **kwargs
                 )
@@ -1837,15 +1837,20 @@
             raise ValueError("Max number of files to delete in one call is 1000")
         delete_keys = {
             "Objects": [{"Key": self.split_path(path)[1]} for path in pathlist],
             "Quiet": True,
         }
         for path in pathlist:
             self.invalidate_cache(self._parent(path))
-        await self._call_s3("delete_objects", kwargs, Bucket=bucket, Delete=delete_keys)
+        out = await self._call_s3(
+            "delete_objects", kwargs, Bucket=bucket, Delete=delete_keys
+        )
+        # TODO: we report on successes but don't raise on any errors, effectively
+        #  on_error="omit"
+        return [f"{bucket}/{_['Key']}" for _ in out.get("Deleted", [])]
 
     async def _rm_file(self, path, **kwargs):
         bucket, key, _ = self.split_path(path)
 
         try:
             await self._call_s3("delete_object", Bucket=bucket, Key=key)
         except ClientError as e:
@@ -1857,27 +1862,28 @@
             if not key and await self._is_bucket_versioned(bucket):
                 # special path to completely remove versioned bucket
                 await self._rm_versioned_bucket_contents(bucket)
         paths = await self._expand_path(path, recursive=recursive)
         files = [p for p in paths if self.split_path(p)[1]]
         dirs = [p for p in paths if not self.split_path(p)[1]]
         # TODO: fails if more than one bucket in list
-        await _run_coros_in_chunks(
+        out = await _run_coros_in_chunks(
             [
                 self._bulk_delete(files[i : i + 1000])
                 for i in range(0, len(files), 1000)
             ],
             batch_size=3,
             nofiles=True,
         )
         await asyncio.gather(*[self._rmdir(d) for d in dirs])
         [
             (self.invalidate_cache(p), self.invalidate_cache(self._parent(p)))
             for p in paths
         ]
+        return sum(out, [])
 
     async def _is_bucket_versioned(self, bucket):
         return (await self._call_s3("get_bucket_versioning", Bucket=bucket)).get(
             "Status", ""
         ) == "Enabled"
 
     is_bucket_versioned = sync_wrapper(_is_bucket_versioned)
@@ -2284,29 +2290,14 @@
 
 
 class S3AsyncStreamedFile(AbstractAsyncStreamedFile):
     def __init__(self, fs, path, mode):
         self.fs = fs
         self.path = path
         self.mode = mode
-        self.r = None
-
-    async def read(self, length=-1):
-        if self.r is None:
-            bucket, key, gen = self.fs.split_path(self.path)
-            r = await self.fs._call_s3("get_object", Bucket=bucket, Key=key)
-            self.r = r["Body"]
-        return await self.r.read(length)
-
-
-class S3AsyncStreamedFile(AbstractAsyncStreamedFile):
-    def __init__(self, fs, path, mode):
-        self.fs = fs
-        self.path = path
-        self.mode = mode
         self.r = None
 
     async def read(self, length=-1):
         if self.r is None:
             bucket, key, gen = self.fs.split_path(self.path)
             r = await self.fs._call_s3("get_object", Bucket=bucket, Key=key)
             self.r = r["Body"]
```

### Comparing `s3fs-2023.4.0/s3fs/errors.py` & `s3fs-2023.5.0/s3fs/errors.py`

 * *Files identical despite different names*

### Comparing `s3fs-2023.4.0/s3fs/tests/test_mapping.py` & `s3fs-2023.5.0/s3fs/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `s3fs-2023.4.0/s3fs/tests/test_s3fs.py` & `s3fs-2023.5.0/s3fs/tests/test_s3fs.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,30 +370,30 @@
                 {"PartNumber": 2, "ETag": etag2},
             ]
         },
     )
     s3.checksum(path1, refresh=True)
 
 
-test_xattr_sample_metadata = {"test_xattr": "1"}
+test_xattr_sample_metadata = {"testxattr": "1"}
 
 
 def test_xattr(s3):
     bucket, key = (test_bucket_name, "tmp/test/xattr")
     filename = bucket + "/" + key
     body = b"aaaa"
     public_read_acl = {
         "Permission": "READ",
         "Grantee": {
             "URI": "http://acs.amazonaws.com/groups/global/AllUsers",
             "Type": "Group",
         },
     }
 
-    sync(
+    resp = sync(
         s3.loop,
         s3.s3.put_object,
         Bucket=bucket,
         Key=key,
         ACL="public-read",
         Metadata=test_xattr_sample_metadata,
         Body=body,
@@ -402,26 +402,24 @@
     # save etag for later
     etag = s3.info(filename)["ETag"]
     assert (
         public_read_acl
         in sync(s3.loop, s3.s3.get_object_acl, Bucket=bucket, Key=key)["Grants"]
     )
 
-    assert (
-        s3.getxattr(filename, "test_xattr") == test_xattr_sample_metadata["test_xattr"]
-    )
-    assert s3.metadata(filename) == {"test-xattr": "1"}  # note _ became -
+    assert s3.getxattr(filename, "testxattr") == test_xattr_sample_metadata["testxattr"]
+    assert s3.metadata(filename) == {"testxattr": "1"}  # note _ became -
 
     s3file = s3.open(filename)
-    assert s3file.getxattr("test_xattr") == test_xattr_sample_metadata["test_xattr"]
-    assert s3file.metadata() == {"test-xattr": "1"}  # note _ became -
+    assert s3file.getxattr("testxattr") == test_xattr_sample_metadata["testxattr"]
+    assert s3file.metadata() == {"testxattr": "1"}  # note _ became -
 
-    s3file.setxattr(test_xattr="2")
-    assert s3file.getxattr("test_xattr") == "2"
-    s3file.setxattr(**{"test_xattr": None})
+    s3file.setxattr(testxattr="2")
+    assert s3file.getxattr("testxattr") == "2"
+    s3file.setxattr(**{"testxattr": None})
     assert s3file.metadata() == {}
     assert s3.cat(filename) == body
 
     # check that ACL and ETag are preserved after updating metadata
     assert (
         public_read_acl
         in sync(s3.loop, s3.s3.get_object_acl, Bucket=bucket, Key=key)["Grants"]
@@ -572,19 +570,21 @@
     s3.rm(a)
     assert not s3.exists(a)
     # the API is OK with deleting non-files; maybe this is an effect of using bulk
     # with pytest.raises(FileNotFoundError):
     #    s3.rm(test_bucket_name + '/nonexistent')
     with pytest.raises(FileNotFoundError):
         s3.rm("nonexistent")
-    s3.rm(test_bucket_name + "/nested", recursive=True)
+    out = s3.rm(test_bucket_name + "/nested", recursive=True)
+    assert test_bucket_name + "/nested/nested2/file1" in out
     assert not s3.exists(test_bucket_name + "/nested/nested2/file1")
 
     # whole bucket
-    s3.rm(test_bucket_name, recursive=True)
+    out = s3.rm(test_bucket_name, recursive=True)
+    assert test_bucket_name + "/2014-01-01.csv" in out
     assert not s3.exists(test_bucket_name + "/2014-01-01.csv")
     assert not s3.exists(test_bucket_name)
 
 
 def test_rmdir(s3):
     bucket = "test1_bucket"
     s3.mkdir(bucket)
@@ -2141,14 +2141,37 @@
 
     assert s3.ls(test_bucket_name) == s3.find(
         test_bucket_name, maxdepth=1, withdirs=True
     )
     assert s3.ls(test_bucket_name) == s3.glob(test_bucket_name + "/*")
 
 
+def test_multi_find(s3):
+    s3.mkdir("bucket/test")
+    s3.mkdir("bucket/test/sub")
+    s3.write_text("bucket/test/file.txt", "some_text")
+    s3.write_text("bucket/test/sub/file.txt", "some_text")
+
+    out1 = s3.find("bucket", withdirs=True)
+    out2 = s3.find("bucket", withdirs=True)
+    assert (
+        out1
+        == out2
+        == [
+            "bucket/test",
+            "bucket/test/file.txt",
+            "bucket/test/sub",
+            "bucket/test/sub/file.txt",
+        ]
+    )
+    out1 = s3.find("bucket", withdirs=False)
+    out2 = s3.find("bucket", withdirs=False)
+    assert out1 == out2 == ["bucket/test/file.txt", "bucket/test/sub/file.txt"]
+
+
 def test_version_sizes(s3):
     # protect against caching of incorrect version details
     s3 = S3FileSystem(
         anon=False, version_aware=True, client_kwargs={"endpoint_url": endpoint_uri}
     )
     import gzip
```

### Comparing `s3fs-2023.4.0/s3fs/utils.py` & `s3fs-2023.5.0/s3fs/utils.py`

 * *Files identical despite different names*

### Comparing `s3fs-2023.4.0/s3fs.egg-info/PKG-INFO` & `s3fs-2023.5.0/s3fs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3fs
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: Convenient Filesystem interface over S3
 Home-page: http://github.com/fsspec/s3fs/
 Maintainer: Martin Durant
 Maintainer-email: mdurant@continuum.io
 License: BSD
 Keywords: s3,boto
 Classifier: Development Status :: 4 - Beta
```

### Comparing `s3fs-2023.4.0/s3fs.egg-info/SOURCES.txt` & `s3fs-2023.5.0/s3fs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s3fs-2023.4.0/setup.py` & `s3fs-2023.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `s3fs-2023.4.0/versioneer.py` & `s3fs-2023.5.0/versioneer.py`

 * *Files identical despite different names*

