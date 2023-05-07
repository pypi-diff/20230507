# Comparing `tmp/struct_gpt-2.0.1.tar.gz` & `tmp/struct_gpt-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct_gpt-2.0.1.tar", last modified: Sun May  7 21:10:47 2023, max compression
+gzip compressed data, was "struct_gpt-2.0.2.tar", last modified: Sun May  7 21:26:48 2023, max compression
```

## Comparing `struct_gpt-2.0.1.tar` & `struct_gpt-2.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1076 2023-05-07 21:10:01.345253 struct_gpt-2.0.1/LICENSE
--rw-r--r--   0        0        0     3744 2023-05-07 21:10:01.345253 struct_gpt-2.0.1/README.md
--rw-r--r--   0        0        0      587 2023-05-07 21:10:47.929813 struct_gpt-2.0.1/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-07 21:10:01.345253 struct_gpt-2.0.1/struct_gpt/__init__.py
--rw-r--r--   0        0        0     3844 2023-05-07 21:10:01.345253 struct_gpt-2.0.1/struct_gpt/models.py
--rw-r--r--   0        0        0     4222 2023-05-07 21:10:01.345253 struct_gpt-2.0.1/tests/test_models.py
--rw-r--r--   0        0        0     5365 1970-01-01 00:00:00.000000 struct_gpt-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-07 21:26:06.746005 struct_gpt-2.0.2/LICENSE
+-rw-r--r--   0        0        0     3749 2023-05-07 21:26:06.746005 struct_gpt-2.0.2/README.md
+-rw-r--r--   0        0        0      587 2023-05-07 21:26:48.290264 struct_gpt-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-07 21:26:06.750005 struct_gpt-2.0.2/struct_gpt/__init__.py
+-rw-r--r--   0        0        0     3844 2023-05-07 21:26:06.750005 struct_gpt-2.0.2/struct_gpt/models.py
+-rw-r--r--   0        0        0     4222 2023-05-07 21:26:06.750005 struct_gpt-2.0.2/tests/test_models.py
+-rw-r--r--   0        0        0     5370 1970-01-01 00:00:00.000000 struct_gpt-2.0.2/PKG-INFO
```

### Comparing `struct_gpt-2.0.1/LICENSE` & `struct_gpt-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.0.1/README.md` & `struct_gpt-2.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 ## Usage
 
 `pip install struct-gpt`
 
 ---
 
-Template variables in the class' docstring are replaced with the keyword arguments passed to `create`.
+Template variables in the class' docstring are replaced with the keyword arguments passed to `from_openai`.
 
 ```python
 from struct_gpt import OpenAiBase
 from pydantic import Field
 
 
 class SentimentSchema(OpenAiBase):
```

### Comparing `struct_gpt-2.0.1/pyproject.toml` & `struct_gpt-2.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 dev = [
     "pytest>=7.3.1",
     "coverage>=7.2.5",
 ]
 
 [project]
 name = "struct-gpt"
-version = "2.0.1"
+version = "2.0.2"
 description = "structured llm outputs"
 authors = [
     { name = "Stephan Fitzpatrick", email = "knowsuchagency@gmail.com" },
 ]
 dependencies = [
     "openai>=0.27.6",
     "pydantic>=1.10.7",
```

### Comparing `struct_gpt-2.0.1/struct_gpt/models.py` & `struct_gpt-2.0.2/struct_gpt/models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.0.1/tests/test_models.py` & `struct_gpt-2.0.2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.0.1/PKG-INFO` & `struct_gpt-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-gpt
-Version: 2.0.1
+Version: 2.0.2
 Summary: structured llm outputs
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Stephan Fitzpatrick
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -45,15 +45,15 @@
 
 ## Usage
 
 `pip install struct-gpt`
 
 ---
 
-Template variables in the class' docstring are replaced with the keyword arguments passed to `create`.
+Template variables in the class' docstring are replaced with the keyword arguments passed to `from_openai`.
 
 ```python
 from struct_gpt import OpenAiBase
 from pydantic import Field
 
 
 class SentimentSchema(OpenAiBase):
```

