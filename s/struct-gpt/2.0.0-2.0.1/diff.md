# Comparing `tmp/struct_gpt-2.0.0.tar.gz` & `tmp/struct_gpt-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct_gpt-2.0.0.tar", last modified: Sun May  7 20:28:41 2023, max compression
+gzip compressed data, was "struct_gpt-2.0.1.tar", last modified: Sun May  7 21:10:47 2023, max compression
```

## Comparing `struct_gpt-2.0.0.tar` & `struct_gpt-2.0.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     3647 2023-05-07 20:27:58.323813 struct_gpt-2.0.0/README.md
--rw-r--r--   0        0        0      583 2023-05-07 20:28:41.456481 struct_gpt-2.0.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-07 20:27:58.323813 struct_gpt-2.0.0/struct_gpt/__init__.py
--rw-r--r--   0        0        0     3844 2023-05-07 20:27:58.323813 struct_gpt-2.0.0/struct_gpt/models.py
--rw-r--r--   0        0        0     4222 2023-05-07 20:27:58.323813 struct_gpt-2.0.0/tests/test_models.py
--rw-r--r--   0        0        0     4036 1970-01-01 00:00:00.000000 struct_gpt-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-07 21:10:01.345253 struct_gpt-2.0.1/LICENSE
+-rw-r--r--   0        0        0     3744 2023-05-07 21:10:01.345253 struct_gpt-2.0.1/README.md
+-rw-r--r--   0        0        0      587 2023-05-07 21:10:47.929813 struct_gpt-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-07 21:10:01.345253 struct_gpt-2.0.1/struct_gpt/__init__.py
+-rw-r--r--   0        0        0     3844 2023-05-07 21:10:01.345253 struct_gpt-2.0.1/struct_gpt/models.py
+-rw-r--r--   0        0        0     4222 2023-05-07 21:10:01.345253 struct_gpt-2.0.1/tests/test_models.py
+-rw-r--r--   0        0        0     5365 1970-01-01 00:00:00.000000 struct_gpt-2.0.1/PKG-INFO
```

### Comparing `struct_gpt-2.0.0/README.md` & `struct_gpt-2.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # struct-gpt
 
 
 [![codecov](https://codecov.io/gh/knowsuchagency/struct-gpt/branch/main/graph/badge.svg?token=TMUQNTCTDI)](https://codecov.io/gh/knowsuchagency/struct-gpt)
+[![PyPI version](https://badge.fury.io/py/struct-gpt.svg)](https://pypi.org/project/struct-gpt/)
 
 ## Features
 
 * Easy creation of custom models using the OpenAI API
 * Integration with Pydantic for model validation and serialization
 * Flexible configuration with retries and temperature settings
```

### Comparing `struct_gpt-2.0.0/pyproject.toml` & `struct_gpt-2.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 dev = [
     "pytest>=7.3.1",
     "coverage>=7.2.5",
 ]
 
 [project]
 name = "struct-gpt"
-version = "2.0.0"
+version = "2.0.1"
 description = "structured llm outputs"
 authors = [
     { name = "Stephan Fitzpatrick", email = "knowsuchagency@gmail.com" },
 ]
 dependencies = [
     "openai>=0.27.6",
     "pydantic>=1.10.7",
     "ruamel-yaml>=0.17.24",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
-text = "MIT"
+file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/knowsuchagency/struct-gpt"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `struct_gpt-2.0.0/struct_gpt/models.py` & `struct_gpt-2.0.1/struct_gpt/models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-2.0.0/tests/test_models.py` & `struct_gpt-2.0.1/tests/test_models.py`

 * *Files identical despite different names*

