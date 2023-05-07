# Comparing `tmp/struct_gpt-1.0.0.tar.gz` & `tmp/struct_gpt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct_gpt-1.0.0.tar", last modified: Sun May  7 19:43:53 2023, max compression
+gzip compressed data, was "struct_gpt-1.0.1.tar", last modified: Sun May  7 19:58:03 2023, max compression
```

## Comparing `struct_gpt-1.0.0.tar` & `struct_gpt-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3468 2023-05-07 19:43:16.804088 struct_gpt-1.0.0/README.md
--rw-r--r--   0        0        0      583 2023-05-07 19:43:53.404899 struct_gpt-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-07 19:43:16.804088 struct_gpt-1.0.0/struct_gpt/__init__.py
--rw-r--r--   0        0        0     3839 2023-05-07 19:43:16.804088 struct_gpt-1.0.0/struct_gpt/models.py
--rw-r--r--   0        0        0     4177 2023-05-07 19:43:16.804088 struct_gpt-1.0.0/tests/test_models.py
--rw-r--r--   0        0        0     3857 1970-01-01 00:00:00.000000 struct_gpt-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3625 2023-05-07 19:57:24.756725 struct_gpt-1.0.1/README.md
+-rw-r--r--   0        0        0      583 2023-05-07 19:58:03.008738 struct_gpt-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-07 19:57:24.756725 struct_gpt-1.0.1/struct_gpt/__init__.py
+-rw-r--r--   0        0        0     3839 2023-05-07 19:57:24.756725 struct_gpt-1.0.1/struct_gpt/models.py
+-rw-r--r--   0        0        0     4177 2023-05-07 19:57:24.756725 struct_gpt-1.0.1/tests/test_models.py
+-rw-r--r--   0        0        0     4014 1970-01-01 00:00:00.000000 struct_gpt-1.0.1/PKG-INFO
```

### Comparing `struct_gpt-1.0.0/README.md` & `struct_gpt-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # struct-gpt
 
+[![codecov](https://codecov.io/gh/knowsuchagency/struct-gpt/branch/main/graph/badge.svg?token=TMUQNTCTDI)](https://codecov.io/gh/knowsuchagency/struct-gpt)
+
 ## Features
 
 * Easy creation of custom models using the OpenAI API
 * Integration with Pydantic for model validation and serialization
 * Flexible configuration with retries and temperature settings
 
 ## Usage
```

### Comparing `struct_gpt-1.0.0/pyproject.toml` & `struct_gpt-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 dev = [
     "pytest>=7.3.1",
     "coverage>=7.2.5",
 ]
 
 [project]
 name = "struct-gpt"
-version = "1.0.0"
+version = "1.0.1"
 description = "structured llm outputs"
 authors = [
     { name = "Stephan Fitzpatrick", email = "knowsuchagency@gmail.com" },
 ]
 dependencies = [
     "openai>=0.27.6",
     "pydantic>=1.10.7",
```

### Comparing `struct_gpt-1.0.0/struct_gpt/models.py` & `struct_gpt-1.0.1/struct_gpt/models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-1.0.0/tests/test_models.py` & `struct_gpt-1.0.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-1.0.0/PKG-INFO` & `struct_gpt-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: struct-gpt
-Version: 1.0.0
+Version: 1.0.1
 Summary: structured llm outputs
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/knowsuchagency/struct-gpt
 Requires-Python: >=3.10
 Requires-Dist: openai>=0.27.6
 Requires-Dist: pydantic>=1.10.7
 Requires-Dist: ruamel-yaml>=0.17.24
 Description-Content-Type: text/markdown
 
 # struct-gpt
 
+[![codecov](https://codecov.io/gh/knowsuchagency/struct-gpt/branch/main/graph/badge.svg?token=TMUQNTCTDI)](https://codecov.io/gh/knowsuchagency/struct-gpt)
+
 ## Features
 
 * Easy creation of custom models using the OpenAI API
 * Integration with Pydantic for model validation and serialization
 * Flexible configuration with retries and temperature settings
 
 ## Usage
```

