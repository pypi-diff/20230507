# Comparing `tmp/struct_gpt-0.1.0.tar.gz` & `tmp/struct_gpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct_gpt-0.1.0.tar", last modified: Sun May  7 08:09:25 2023, max compression
+gzip compressed data, was "struct_gpt-0.1.1.tar", last modified: Sun May  7 08:15:34 2023, max compression
```

## Comparing `struct_gpt-0.1.0.tar` & `struct_gpt-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1247 2023-05-07 08:07:27.506234 struct_gpt-0.1.0/README.md
--rw-r--r--   0        0        0      440 2023-05-07 08:09:25.334002 struct_gpt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-07 07:47:49.753180 struct_gpt-0.1.0/struct_gpt/__init__.py
--rw-r--r--   0        0        0     4539 2023-05-07 07:41:39.445343 struct_gpt-0.1.0/struct_gpt/models.py
--rw-r--r--   0        0        0     1570 1970-01-01 00:00:00.000000 struct_gpt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1247 2023-05-07 08:07:27.506234 struct_gpt-0.1.1/README.md
+-rw-r--r--   0        0        0      512 2023-05-07 08:15:34.856585 struct_gpt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-07 07:47:49.753180 struct_gpt-0.1.1/struct_gpt/__init__.py
+-rw-r--r--   0        0        0     4539 2023-05-07 07:41:39.445343 struct_gpt-0.1.1/struct_gpt/models.py
+-rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 struct_gpt-0.1.1/PKG-INFO
```

### Comparing `struct_gpt-0.1.0/README.md` & `struct_gpt-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `struct_gpt-0.1.0/struct_gpt/models.py` & `struct_gpt-0.1.1/struct_gpt/models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-0.1.0/PKG-INFO` & `struct_gpt-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: struct-gpt
-Version: 0.1.0
+Version: 0.1.1
 Summary: structured llm outputs
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: MIT
+Project-URL: Source, https://github.com/knowsuchagency/struct-gpt
 Requires-Python: >=3.10
 Requires-Dist: openai>=0.27.6
 Requires-Dist: pydantic>=1.10.7
 Requires-Dist: ruamel-yaml>=0.17.24
 Description-Content-Type: text/markdown
 
 # struct-gpt
```

