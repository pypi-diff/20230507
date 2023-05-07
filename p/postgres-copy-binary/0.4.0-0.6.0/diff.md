# Comparing `tmp/postgres_copy_binary-0.4.0.tar.gz` & `tmp/postgres_copy_binary-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgres_copy_binary-0.4.0.tar", max compression
+gzip compressed data, was "postgres_copy_binary-0.6.0.tar", max compression
```

## Comparing `postgres_copy_binary-0.4.0.tar` & `postgres_copy_binary-0.6.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      704 2023-04-09 22:26:13.893575 postgres_copy_binary-0.4.0/README.md
--rw-r--r--   0        0        0      635 2023-04-10 11:18:24.175951 postgres_copy_binary-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      723 2023-04-09 22:26:13.893575 postgres_copy_binary-0.4.0/src/postgres_copy_binary/__init__.py
--rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 postgres_copy_binary-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      704 2023-05-07 21:33:30.824916 postgres_copy_binary-0.6.0/README.md
+-rw-r--r--   0        0        0      652 2023-05-07 21:33:30.824916 postgres_copy_binary-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      797 2023-05-07 21:33:30.824916 postgres_copy_binary-0.6.0/src/postgres_copy_binary/__init__.py
+-rw-r--r--   0        0        0     1603 1970-01-01 00:00:00.000000 postgres_copy_binary-0.6.0/PKG-INFO
```

### Comparing `postgres_copy_binary-0.4.0/README.md` & `postgres_copy_binary-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `postgres_copy_binary-0.4.0/pyproject.toml` & `postgres_copy_binary-0.6.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "postgres-copy-binary"
-version = "0.4.0"
+version = "0.6.0"
 description = "Provides a decoder for postgres COPY FROM WITH BINARY format that produces pyarrow / pandas / numpy / polars arrays."
 repository = "https://github.com/grihabor/postgres-copy-binary"
 authors = ["Gregory Borodin <grihabor@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = []
 packages = [
     { include = "postgres_copy_binary", from = "src" },
 ]
 
 [tool.poetry.dependencies]
-postgres-copy-binary-extension-module = { version = "0.4.0", python = ">=3.7" }
+python = ">=3.7"
+postgres-copy-binary-extension-module = { version = "0.6.0", python = ">=3.7" }
```

### Comparing `postgres_copy_binary-0.4.0/src/postgres_copy_binary/__init__.py` & `postgres_copy_binary-0.6.0/src/postgres_copy_binary/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 
 
 def read_table(cursor, table: str) -> list[pyarrow.Array]:
 
     # get column types, we need them to decode postgres binary format
     cursor.execute(
         """
-        select data_type from information_schema.columns
+        select column_name, data_type from information_schema.columns
         where table_name = %s
         order by ordinal_position
     """,
         (table,),
     )
-    types = [row[0] for row in cursor.fetchall()]
+    names, types = zip(*list(cursor.fetchall()))
 
     # copy table into buffer
     buf = io.BytesIO()
     cursor.copy_expert(f"copy {table} to stdin WITH binary", buf)
     buffer = buf.getvalue()
 
     # decode buffer
-    return decode_buffer(buffer, types)
+    columns = decode_buffer(buffer, types)
+    return pyarrow.Table.from_arrays(columns, names=names)
 
 
 __all__ = (
     "read_pyarrow",
     "decode_buffer",
 )
```

### Comparing `postgres_copy_binary-0.4.0/PKG-INFO` & `postgres_copy_binary-0.6.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 2.1
 Name: postgres-copy-binary
-Version: 0.4.0
+Version: 0.6.0
 Summary: Provides a decoder for postgres COPY FROM WITH BINARY format that produces pyarrow / pandas / numpy / polars arrays.
 Home-page: https://github.com/grihabor/postgres-copy-binary
 License: MIT
 Author: Gregory Borodin
 Author-email: grihabor@gmail.com
+Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: postgres-copy-binary-extension-module (==0.4.0) ; python_version >= "3.7"
+Requires-Dist: postgres-copy-binary-extension-module (==0.6.0) ; python_version >= "3.7"
 Project-URL: Repository, https://github.com/grihabor/postgres-copy-binary
 Description-Content-Type: text/markdown
 
 # postgres-copy-binary
 
 Provides a decoder for postgres `COPY FROM WITH BINARY` format that spits out pyarrow / pandas / numpy arrays
```

