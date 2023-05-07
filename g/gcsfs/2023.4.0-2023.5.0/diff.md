# Comparing `tmp/gcsfs-2023.4.0.tar.gz` & `tmp/gcsfs-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcsfs-2023.4.0.tar", last modified: Tue Apr 11 13:58:16 2023, max compression
+gzip compressed data, was "gcsfs-2023.5.0.tar", last modified: Sun May  7 19:22:00 2023, max compression
```

## Comparing `gcsfs-2023.4.0.tar` & `gcsfs-2023.5.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-11 13:58:16.889359 gcsfs-2023.4.0/
--rw-r--r--   0 mdurant    (502) staff       (20)     1536 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/LICENSE.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      227 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)     1280 2023-04-11 13:58:16.889424 gcsfs-2023.4.0/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)      526 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/README.rst
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-11 13:58:16.881876 gcsfs-2023.4.0/docs/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-11 13:58:16.884503 gcsfs-2023.4.0/docs/source/
--rw-r--r--   0 mdurant    (502) staff       (20)      800 2023-02-24 20:42:20.000000 gcsfs-2023.4.0/docs/source/api.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     4125 2023-04-11 13:57:22.000000 gcsfs-2023.4.0/docs/source/changelog.rst
--rw-r--r--   0 mdurant    (502) staff       (20)      906 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/docs/source/developer.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     1776 2023-02-24 20:42:20.000000 gcsfs-2023.4.0/docs/source/fuse.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     6393 2023-02-24 20:42:20.000000 gcsfs-2023.4.0/docs/source/index.rst
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-11 13:58:16.890161 gcsfs-2023.4.0/gcsfs/
--rw-r--r--   0 mdurant    (502) staff       (20)      192 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/gcsfs/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      500 2023-04-11 13:58:16.890202 gcsfs-2023.4.0/gcsfs/_version.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3618 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/checkers.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-11 13:58:16.887541 gcsfs-2023.4.0/gcsfs/cli/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/gcsfs/cli/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1942 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/cli/gcsfuse.py
--rw-r--r--   0 mdurant    (502) staff       (20)    60406 2023-03-02 18:45:14.000000 gcsfs-2023.4.0/gcsfs/core.py
--rw-r--r--   0 mdurant    (502) staff       (20)     8947 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/credentials.py
--rw-r--r--   0 mdurant    (502) staff       (20)       68 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/gcsfs/dask_link.py
--rw-r--r--   0 mdurant    (502) staff       (20)      227 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/gcsfs/mapping.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4691 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/retry.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-11 13:58:16.889231 gcsfs-2023.4.0/gcsfs/tests/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/gcsfs/tests/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3885 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/tests/conftest.py
--rw-r--r--   0 mdurant    (502) staff       (20)      178 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/tests/settings.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4029 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/tests/test_checkers.py
--rw-r--r--   0 mdurant    (502) staff       (20)    41351 2023-02-24 20:42:20.000000 gcsfs-2023.4.0/gcsfs/tests/test_core.py
--rw-r--r--   0 mdurant    (502) staff       (20)      222 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/gcsfs/tests/test_credentials.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1822 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/tests/test_fuse.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1040 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/tests/test_manyopens.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3064 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/tests/test_mapping.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3429 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/tests/test_retry.py
--rw-r--r--   0 mdurant    (502) staff       (20)      911 2023-01-02 14:01:40.000000 gcsfs-2023.4.0/gcsfs/tests/utils.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-11 13:58:16.887318 gcsfs-2023.4.0/gcsfs.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     1280 2023-04-11 13:58:16.000000 gcsfs-2023.4.0/gcsfs.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)      842 2023-04-11 13:58:16.000000 gcsfs-2023.4.0/gcsfs.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-04-11 13:58:16.000000 gcsfs-2023.4.0/gcsfs.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-27 12:31:48.000000 gcsfs-2023.4.0/gcsfs.egg-info/not-zip-safe
--rw-r--r--   0 mdurant    (502) staff       (20)      160 2023-04-11 13:58:16.000000 gcsfs-2023.4.0/gcsfs.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        6 2023-04-11 13:58:16.000000 gcsfs-2023.4.0/gcsfs.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      129 2023-04-11 13:57:22.000000 gcsfs-2023.4.0/requirements.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      445 2023-04-11 13:58:16.889693 gcsfs-2023.4.0/setup.cfg
--rwxr-xr-x   0 mdurant    (502) staff       (20)     1184 2023-02-24 20:42:20.000000 gcsfs-2023.4.0/setup.py
--rw-r--r--   0 mdurant    (502) staff       (20)    68739 2022-09-18 01:28:26.000000 gcsfs-2023.4.0/versioneer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:22:00.342964 gcsfs-2023.5.0/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1536 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/LICENSE.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      227 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     1280 2023-05-07 19:22:00.343070 gcsfs-2023.5.0/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      526 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/README.rst
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:22:00.332376 gcsfs-2023.5.0/docs/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:22:00.335776 gcsfs-2023.5.0/docs/source/
+-rw-r--r--   0 mdurant    (502) staff       (20)      800 2023-02-24 20:42:20.000000 gcsfs-2023.5.0/docs/source/api.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     4254 2023-05-07 19:21:12.000000 gcsfs-2023.5.0/docs/source/changelog.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)      906 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/docs/source/developer.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     1776 2023-02-24 20:42:20.000000 gcsfs-2023.5.0/docs/source/fuse.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     6393 2023-02-24 20:42:20.000000 gcsfs-2023.5.0/docs/source/index.rst
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:22:00.343814 gcsfs-2023.5.0/gcsfs/
+-rw-r--r--   0 mdurant    (502) staff       (20)      192 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/gcsfs/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      500 2023-05-07 19:22:00.343870 gcsfs-2023.5.0/gcsfs/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3618 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/checkers.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:22:00.340256 gcsfs-2023.5.0/gcsfs/cli/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/gcsfs/cli/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1942 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/cli/gcsfuse.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    60829 2023-05-07 19:16:48.000000 gcsfs-2023.5.0/gcsfs/core.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     8947 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/credentials.py
+-rw-r--r--   0 mdurant    (502) staff       (20)       68 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/gcsfs/dask_link.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      227 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/gcsfs/mapping.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4691 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/retry.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:22:00.342782 gcsfs-2023.5.0/gcsfs/tests/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/gcsfs/tests/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3885 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/tests/conftest.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      178 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/tests/settings.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4029 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/tests/test_checkers.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    41351 2023-02-24 20:42:20.000000 gcsfs-2023.5.0/gcsfs/tests/test_core.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      222 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/gcsfs/tests/test_credentials.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1822 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/tests/test_fuse.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1040 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/tests/test_manyopens.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3064 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/tests/test_mapping.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3429 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/tests/test_retry.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      911 2023-01-02 14:01:40.000000 gcsfs-2023.5.0/gcsfs/tests/utils.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:22:00.339760 gcsfs-2023.5.0/gcsfs.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1280 2023-05-07 19:22:00.000000 gcsfs-2023.5.0/gcsfs.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      842 2023-05-07 19:22:00.000000 gcsfs-2023.5.0/gcsfs.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-05-07 19:22:00.000000 gcsfs-2023.5.0/gcsfs.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-27 12:31:48.000000 gcsfs-2023.5.0/gcsfs.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)      160 2023-05-07 19:22:00.000000 gcsfs-2023.5.0/gcsfs.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        6 2023-05-07 19:22:00.000000 gcsfs-2023.5.0/gcsfs.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      129 2023-05-07 19:21:12.000000 gcsfs-2023.5.0/requirements.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      445 2023-05-07 19:22:00.343480 gcsfs-2023.5.0/setup.cfg
+-rwxr-xr-x   0 mdurant    (502) staff       (20)     1184 2023-02-24 20:42:20.000000 gcsfs-2023.5.0/setup.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    68739 2022-09-18 01:28:26.000000 gcsfs-2023.5.0/versioneer.py
```

### Comparing `gcsfs-2023.4.0/LICENSE.txt` & `gcsfs-2023.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/PKG-INFO` & `gcsfs-2023.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcsfs
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: Convenient Filesystem interface over GCS
 Home-page: https://github.com/fsspec/gcsfs
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
 Keywords: google-cloud-storage,gcloud,file-system
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gcsfs-2023.4.0/README.rst` & `gcsfs-2023.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/docs/source/api.rst` & `gcsfs-2023.5.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/docs/source/changelog.rst` & `gcsfs-2023.5.0/docs/source/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+2023.5.0
+--------
+
+* Allow emulator host without protocol (#548)
+* Prevent upload retry from closing the file being sent (#540)
+
 2023.4.0
 --------
 
 No changes
 
 2023.3.0
 --------
```

### Comparing `gcsfs-2023.4.0/docs/source/developer.rst` & `gcsfs-2023.5.0/docs/source/developer.rst`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/docs/source/fuse.rst` & `gcsfs-2023.5.0/docs/source/fuse.rst`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/docs/source/index.rst` & `gcsfs-2023.5.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/gcsfs/checkers.py` & `gcsfs-2023.5.0/gcsfs/checkers.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/gcsfs/cli/gcsfuse.py` & `gcsfs-2023.5.0/gcsfs/cli/gcsfuse.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/gcsfs/core.py` & `gcsfs-2023.5.0/gcsfs/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,28 +92,40 @@
 
 
 async def _req_to_text(r):
     async with r:
         return (await r.read()).decode()
 
 
+class UnclosableBytesIO(io.BytesIO):
+    """Prevent closing BytesIO to avoid errors during retries."""
+
+    def close(self):
+        """Reset stream position for next retry."""
+        self.seek(0)
+
+
 def _location():
     """
     Resolves GCS HTTP location as http[s]://host
 
     Enables storage emulation for integration tests.
 
     Returns
     -------
     valid http location
     """
     _emulator_location = os.getenv("STORAGE_EMULATOR_HOST", None)
-    return (
-        _emulator_location if _emulator_location else "https://storage.googleapis.com"
-    )
+    if _emulator_location:
+        if not any(
+            _emulator_location.startswith(scheme) for scheme in ("http://", "https://")
+        ):
+            _emulator_location = f"http://{_emulator_location}"
+        return _emulator_location
+    return "https://storage.googleapis.com"
 
 
 def _chunks(lst, n):
     """
     Yield evenly-sized chunks from a list.
 
     Implementation based on https://stackoverflow.com/a/312464.
@@ -398,15 +410,14 @@
             url=self._format_path(path, args),
             params=self._get_params(kwargs),
             json=json,
             headers=self._get_headers(headers),
             data=data,
             timeout=self.requests_timeout,
         ) as r:
-
             status = r.status
             headers = r.headers
             info = r.request_info  # for debug only
             contents = await r.read()
 
             validate_response(status, contents, path, args)
             return status, headers, info, contents
@@ -1560,28 +1571,28 @@
                 "POST", self.location, headers=head, data=chunk
             )
             if "Range" in headers:
                 end = int(headers["Range"].split("-")[1])
                 shortfall = (self.offset + l - 1) - end
                 if shortfall > 0:
                     self.checker.update(data[:-shortfall])
-                    self.buffer = io.BytesIO(data[-shortfall:])
+                    self.buffer = UnclosableBytesIO(data[-shortfall:])
                     self.buffer.seek(shortfall)
                     self.offset += l - shortfall
                     continue
                 else:
                     self.checker.update(data)
             else:
                 assert final, "Response looks like upload is over"
                 if l:
                     j = json.loads(contents)
                     self.checker.update(data)
                     self.checker.validate_json_response(j)
             # Clear buffer and update offset when all is received
-            self.buffer = io.BytesIO()
+            self.buffer = UnclosableBytesIO()
             self.offset += l
             break
         return True
 
     def commit(self):
         """If not auto-committing, finalize file"""
         self.autocommit = True
@@ -1678,15 +1689,17 @@
 
 async def upload_chunk(fs, location, data, offset, size, content_type):
     head = {}
     l = len(data)
     range = "bytes %i-%i/%i" % (offset, offset + l - 1, size)
     head["Content-Range"] = range
     head.update({"Content-Type": content_type, "Content-Length": str(l)})
-    headers, txt = await fs._call("POST", location, headers=head, data=io.BytesIO(data))
+    headers, txt = await fs._call(
+        "POST", location, headers=head, data=UnclosableBytesIO(data)
+    )
     if "Range" in headers:
         end = int(headers["Range"].split("-")[1])
         shortfall = (offset + l - 1) - end
         if shortfall:
             return await upload_chunk(
                 fs, location, data[-shortfall:], end, size, content_type
             )
@@ -1744,12 +1757,12 @@
 
     data = template.encode() + datain + b"\n--==0==--"
     j = await fs._call(
         "POST",
         path,
         uploadType="multipart",
         headers={"Content-Type": 'multipart/related; boundary="==0=="'},
-        data=io.BytesIO(data),
+        data=UnclosableBytesIO(data),
         json_out=True,
     )
     checker.update(datain)
     checker.validate_json_response(j)
```

### Comparing `gcsfs-2023.4.0/gcsfs/credentials.py` & `gcsfs-2023.5.0/gcsfs/credentials.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/gcsfs/retry.py` & `gcsfs-2023.5.0/gcsfs/retry.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/gcsfs/tests/conftest.py` & `gcsfs-2023.5.0/gcsfs/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/gcsfs/tests/test_checkers.py` & `gcsfs-2023.5.0/gcsfs/tests/test_checkers.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/gcsfs/tests/test_core.py` & `gcsfs-2023.5.0/gcsfs/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/gcsfs/tests/test_fuse.py` & `gcsfs-2023.5.0/gcsfs/tests/test_fuse.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/gcsfs/tests/test_manyopens.py` & `gcsfs-2023.5.0/gcsfs/tests/test_manyopens.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/gcsfs/tests/test_mapping.py` & `gcsfs-2023.5.0/gcsfs/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/gcsfs/tests/test_retry.py` & `gcsfs-2023.5.0/gcsfs/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/gcsfs/tests/utils.py` & `gcsfs-2023.5.0/gcsfs/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/gcsfs.egg-info/PKG-INFO` & `gcsfs-2023.5.0/gcsfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcsfs
-Version: 2023.4.0
+Version: 2023.5.0
 Summary: Convenient Filesystem interface over GCS
 Home-page: https://github.com/fsspec/gcsfs
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
 Keywords: google-cloud-storage,gcloud,file-system
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gcsfs-2023.4.0/gcsfs.egg-info/SOURCES.txt` & `gcsfs-2023.5.0/gcsfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/setup.py` & `gcsfs-2023.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `gcsfs-2023.4.0/versioneer.py` & `gcsfs-2023.5.0/versioneer.py`

 * *Files identical despite different names*

