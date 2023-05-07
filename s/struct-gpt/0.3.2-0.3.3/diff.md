# Comparing `tmp/struct_gpt-0.3.2.tar.gz` & `tmp/struct_gpt-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct_gpt-0.3.2.tar", last modified: Sun May  7 09:53:30 2023, max compression
+gzip compressed data, was "struct_gpt-0.3.3.tar", last modified: Sun May  7 09:56:23 2023, max compression
```

## Comparing `struct_gpt-0.3.2.tar` & `struct_gpt-0.3.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3486 2023-05-07 09:52:50.510832 struct_gpt-0.3.2/README.md
--rw-r--r--   0        0        0      560 2023-05-07 09:53:30.390968 struct_gpt-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-07 09:52:50.514832 struct_gpt-0.3.2/struct_gpt/__init__.py
--rw-r--r--   0        0        0     3697 2023-05-07 09:52:50.514832 struct_gpt-0.3.2/struct_gpt/models.py
--rw-r--r--   0        0        0     1985 2023-05-07 09:52:50.514832 struct_gpt-0.3.2/tests/test_models.py
--rw-r--r--   0        0        0     3875 1970-01-01 00:00:00.000000 struct_gpt-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     3517 2023-05-07 09:55:40.142096 struct_gpt-0.3.3/README.md
+-rw-r--r--   0        0        0      560 2023-05-07 09:56:23.866079 struct_gpt-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-07 09:55:40.142096 struct_gpt-0.3.3/struct_gpt/__init__.py
+-rw-r--r--   0        0        0     3697 2023-05-07 09:55:40.142096 struct_gpt-0.3.3/struct_gpt/models.py
+-rw-r--r--   0        0        0     1985 2023-05-07 09:55:40.142096 struct_gpt-0.3.3/tests/test_models.py
+-rw-r--r--   0        0        0     3906 1970-01-01 00:00:00.000000 struct_gpt-0.3.3/PKG-INFO
```

### Comparing `struct_gpt-0.3.2/README.md` & `struct_gpt-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 * Easy creation of custom models using the OpenAI API
 * Integration with Pydantic for model validation and serialization
 * Flexible configuration with retries and temperature settings
 
 ## Usage
 
+`pip install struct-gpt`
+
+---
+
 Template variables in the class' docstring are replaced with the keyword arguments passed to `create`.
 
 ```python
 from struct_gpt import OpenAiBase
 from pydantic import Field
 
 class SentimentSchema(OpenAiBase):
```

### Comparing `struct_gpt-0.3.2/pyproject.toml` & `struct_gpt-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.3.1",
 ]
 
 [project]
 name = "struct-gpt"
-version = "0.3.2"
+version = "0.3.3"
 description = "structured llm outputs"
 authors = [
     { name = "Stephan Fitzpatrick", email = "knowsuchagency@gmail.com" },
 ]
 dependencies = [
     "openai>=0.27.6",
     "pydantic>=1.10.7",
```

### Comparing `struct_gpt-0.3.2/struct_gpt/models.py` & `struct_gpt-0.3.3/struct_gpt/models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-0.3.2/tests/test_models.py` & `struct_gpt-0.3.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-0.3.2/PKG-INFO` & `struct_gpt-0.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-gpt
-Version: 0.3.2
+Version: 0.3.3
 Summary: structured llm outputs
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/knowsuchagency/struct-gpt
 Requires-Python: >=3.10
 Requires-Dist: openai>=0.27.6
 Requires-Dist: pydantic>=1.10.7
@@ -17,14 +17,18 @@
 
 * Easy creation of custom models using the OpenAI API
 * Integration with Pydantic for model validation and serialization
 * Flexible configuration with retries and temperature settings
 
 ## Usage
 
+`pip install struct-gpt`
+
+---
+
 Template variables in the class' docstring are replaced with the keyword arguments passed to `create`.
 
 ```python
 from struct_gpt import OpenAiBase
 from pydantic import Field
 
 class SentimentSchema(OpenAiBase):
```

