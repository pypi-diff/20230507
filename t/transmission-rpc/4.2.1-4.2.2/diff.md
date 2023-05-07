# Comparing `tmp/transmission_rpc-4.2.1.tar.gz` & `tmp/transmission_rpc-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transmission_rpc-4.2.1.tar", max compression
+gzip compressed data, was "transmission_rpc-4.2.2.tar", max compression
```

## Comparing `transmission_rpc-4.2.1.tar` & `transmission_rpc-4.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1127 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/LICENSE
--rw-r--r--   0        0        0     1630 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/README.md
--rw-r--r--   0        0        0     3262 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/pyproject.toml
--rw-r--r--   0        0        0     2087 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/transmission_rpc/__init__.py
--rw-r--r--   0        0        0    47198 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/transmission_rpc/client.py
--rw-r--r--   0        0        0    11533 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/transmission_rpc/constants.py
--rw-r--r--   0        0        0     1639 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/transmission_rpc/error.py
--rw-r--r--   0        0        0    12990 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/transmission_rpc/session.py
--rw-r--r--   0        0        0    23663 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/transmission_rpc/torrent.py
--rw-r--r--   0        0        0     1498 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/transmission_rpc/types.py
--rw-r--r--   0        0        0     2669 2023-05-01 04:37:29.821111 transmission_rpc-4.2.1/transmission_rpc/utils.py
--rw-r--r--   0        0        0     3016 1970-01-01 00:00:00.000000 transmission_rpc-4.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1127 2023-05-07 20:19:35.684022 transmission_rpc-4.2.2/LICENSE
+-rw-r--r--   0        0        0     1630 2023-05-07 20:19:35.684022 transmission_rpc-4.2.2/README.md
+-rw-r--r--   0        0        0     3262 2023-05-07 20:19:35.688022 transmission_rpc-4.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2087 2023-05-07 20:19:35.688022 transmission_rpc-4.2.2/transmission_rpc/__init__.py
+-rw-r--r--   0        0        0    47234 2023-05-07 20:19:35.688022 transmission_rpc-4.2.2/transmission_rpc/client.py
+-rw-r--r--   0        0        0    11533 2023-05-07 20:19:35.688022 transmission_rpc-4.2.2/transmission_rpc/constants.py
+-rw-r--r--   0        0        0     1639 2023-05-07 20:19:35.688022 transmission_rpc-4.2.2/transmission_rpc/error.py
+-rw-r--r--   0        0        0    12990 2023-05-07 20:19:35.688022 transmission_rpc-4.2.2/transmission_rpc/session.py
+-rw-r--r--   0        0        0    23734 2023-05-07 20:19:35.688022 transmission_rpc-4.2.2/transmission_rpc/torrent.py
+-rw-r--r--   0        0        0     1498 2023-05-07 20:19:35.688022 transmission_rpc-4.2.2/transmission_rpc/types.py
+-rw-r--r--   0        0        0     2669 2023-05-07 20:19:35.688022 transmission_rpc-4.2.2/transmission_rpc/utils.py
+-rw-r--r--   0        0        0     3016 1970-01-01 00:00:00.000000 transmission_rpc-4.2.2/PKG-INFO
```

### Comparing `transmission_rpc-4.2.1/LICENSE` & `transmission_rpc-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.1/README.md` & `transmission_rpc-4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.1/pyproject.toml` & `transmission_rpc-4.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "transmission-rpc"
-version = "4.2.1"
+version = "4.2.2"
 description = "Python module that implements the Transmission bittorent client JSON-RPC protocol"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'README.md'
 repository = 'https://github.com/Trim21/transmission-rpc'
 license = 'MIT'
 packages = [{ include = 'transmission_rpc' }]
 keywords = ['transmission', 'rpc']
```

### Comparing `transmission_rpc-4.2.1/transmission_rpc/__init__.py` & `transmission_rpc-4.2.2/transmission_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.1/transmission_rpc/client.py` & `transmission_rpc-4.2.2/transmission_rpc/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -496,20 +496,20 @@
         and this lib can't handle table response, So it's unsupported.
 
         Returns a Torrent object with the requested fields.
 
 
         Note
         ----
-        It's recommended that you use torrent's info_hash as torrent id. torrent's info_hash will never change.
+        It's recommended that you use torrent's ``info_hash`` as torrent id. The torrent's ``info_hash`` will never change.
 
         Parameters
         ----------
         torrent_id:
-            torrent id can be an int or a torrent info_hash (hash_string of torrent object).
+            torrent id can be an int or a torrent ``info_hash`` (``hashString`` property of the ``Torrent`` object).
 
         arguments:
             fetched torrent arguments, in most cases you don't need to set this,
             transmission-rpc will fetch all torrent fields it supported.
 
         timeout:
             requests timeout
```

### Comparing `transmission_rpc-4.2.1/transmission_rpc/constants.py` & `transmission_rpc-4.2.2/transmission_rpc/constants.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.1/transmission_rpc/error.py` & `transmission_rpc-4.2.2/transmission_rpc/error.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.1/transmission_rpc/session.py` & `transmission_rpc-4.2.2/transmission_rpc/session.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.1/transmission_rpc/torrent.py` & `transmission_rpc-4.2.2/transmission_rpc/torrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,14 +209,15 @@
 
     @property
     def name(self) -> str:
         return self.fields["name"]
 
     @property
     def hashString(self) -> str:
+        """Torrent info hash string, can also be used as Torrent ID"""
         return self.fields["hashString"]
 
     @property
     def available(self) -> float:
         """Availability in percent"""
         bytes_all = self.total_size
         bytes_done = sum(x["bytesCompleted"] for x in self.fields["fileStats"])
```

### Comparing `transmission_rpc-4.2.1/transmission_rpc/types.py` & `transmission_rpc-4.2.2/transmission_rpc/types.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.1/transmission_rpc/utils.py` & `transmission_rpc-4.2.2/transmission_rpc/utils.py`

 * *Files identical despite different names*

### Comparing `transmission_rpc-4.2.1/PKG-INFO` & `transmission_rpc-4.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transmission-rpc
-Version: 4.2.1
+Version: 4.2.2
 Summary: Python module that implements the Transmission bittorent client JSON-RPC protocol
 Home-page: https://github.com/Trim21/transmission-rpc
 License: MIT
 Keywords: transmission,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.7,<4.0
```

