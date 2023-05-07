# Comparing `tmp/cluedin-0.2.1.tar.gz` & `tmp/cluedin-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cluedin-0.2.1.tar", max compression
+gzip compressed data, was "cluedin-0.2.2.tar", max compression
```

## Comparing `cluedin-0.2.1.tar` & `cluedin-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1927 2023-05-07 18:00:02.022377 cluedin-0.2.1/README.md
--rw-r--r--   0        0        0      119 2023-05-07 15:56:18.443909 cluedin-0.2.1/cluedin/__init__.py
--rw-r--r--   0        0        0      664 2023-05-06 19:21:43.490227 cluedin-0.2.1/cluedin/auth.py
--rw-r--r--   0        0        0     1120 2023-05-07 16:45:36.605300 cluedin-0.2.1/cluedin/gql.py
--rw-r--r--   0        0        0      681 2023-05-07 15:56:40.250091 cluedin-0.2.1/cluedin/urls.py
--rw-r--r--   0        0        0      264 2023-05-06 19:41:45.000595 cluedin-0.2.1/cluedin/utils.py
--rw-r--r--   0        0        0      292 2023-05-07 18:00:27.016967 cluedin-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2372 1970-01-01 00:00:00.000000 cluedin-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1921 2023-05-07 18:04:57.326657 cluedin-0.2.2/README.md
+-rw-r--r--   0        0        0      119 2023-05-07 15:56:18.443909 cluedin-0.2.2/cluedin/__init__.py
+-rw-r--r--   0        0        0      664 2023-05-06 19:21:43.490227 cluedin-0.2.2/cluedin/auth.py
+-rw-r--r--   0        0        0     1120 2023-05-07 16:45:36.605300 cluedin-0.2.2/cluedin/gql.py
+-rw-r--r--   0        0        0      681 2023-05-07 15:56:40.250091 cluedin-0.2.2/cluedin/urls.py
+-rw-r--r--   0        0        0      264 2023-05-06 19:41:45.000595 cluedin-0.2.2/cluedin/utils.py
+-rw-r--r--   0        0        0      562 2023-05-07 19:21:51.712953 cluedin-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 cluedin-0.2.2/PKG-INFO
```

### Comparing `cluedin-0.2.1/README.md` & `cluedin-0.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,19 @@
 [cluedin](https://pypi.org/project/cluedin/) is a Python client for [CluedIn](https://www.cluedin.com/) API. It can help you with the following:
 
 * getting JWT access tokens to CluedIn
 * calling CluedIn REST API
 * calling CluedIn GraphQL API
 
 The use is pretty simple. First, install it from [PyPi](https://pypi.org/project/cluedin/):
-
 ```shell
 pip install cluedin
 ```
 
 Next, you will need to obtain an access token:
-
 ```python
 import cluedin
 
 context = {
     "protocol": "http", # if you skip this parameter, it will fall back to `https`
     "domain": "cluedin.local",
     "organization": "foobar",
@@ -26,16 +24,16 @@
 }
 
 cluedin.load_token_into_context(context)
 
 print(context['access_token'])
 ```
 
-Run a GraphQL query:
 
+Run a GraphQL query:
 ```python
 query = """
     query searchEntities($cursor: PagingCursor, $query: String, $pageSize: Int) {
       search(query: $query, sort: DATE, cursor: $cursor, pageSize: $pageSize) {
         totalResults
         cursor
         entries {
@@ -52,15 +50,14 @@
     "pageSize": 1
 }
 
 response = cluedin.gql.gql(context, query, variables)
 ```
 
 Get paged results:
-
 ```python
 import numpy as np
 import pandas as pd
 
 query = """
     query searchEntities($cursor: PagingCursor, $query: String, $pageSize: Int) {
       search(query: $query, sort: DATE, cursor: $cursor, pageSize: $pageSize) {
```

### Comparing `cluedin-0.2.1/cluedin/auth.py` & `cluedin-0.2.2/cluedin/auth.py`

 * *Files identical despite different names*

### Comparing `cluedin-0.2.1/cluedin/gql.py` & `cluedin-0.2.2/cluedin/gql.py`

 * *Files identical despite different names*

### Comparing `cluedin-0.2.1/cluedin/urls.py` & `cluedin-0.2.2/cluedin/urls.py`

 * *Files identical despite different names*

### Comparing `cluedin-0.2.1/PKG-INFO` & `cluedin-0.2.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 Metadata-Version: 2.1
 Name: cluedin
-Version: 0.2.1
-Summary: 
+Version: 0.2.2
+Summary: A Python client for CluedIn API.
+Home-page: https://github.com/romaklimenko/cluedin
+License: MIT
+Keywords: cluedin,mdm,master data management
 Author: Roman Klimenko
 Author-email: romaklimenko@gmail.com
+Maintainer: Roman Klimenko
+Maintainer-email: romaklimenko@gmail.com
 Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.29.0,<3.0.0)
+Project-URL: Repository, https://github.com/romaklimenko/cluedin
 Description-Content-Type: text/markdown
 
 # CluedIn
 
 [cluedin](https://pypi.org/project/cluedin/) is a Python client for [CluedIn](https://www.cluedin.com/) API. It can help you with the following:
 
 * getting JWT access tokens to CluedIn
 * calling CluedIn REST API
 * calling CluedIn GraphQL API
 
 The use is pretty simple. First, install it from [PyPi](https://pypi.org/project/cluedin/):
-
 ```shell
 pip install cluedin
 ```
 
 Next, you will need to obtain an access token:
-
 ```python
 import cluedin
 
 context = {
     "protocol": "http", # if you skip this parameter, it will fall back to `https`
     "domain": "cluedin.local",
     "organization": "foobar",
@@ -42,16 +47,16 @@
 }
 
 cluedin.load_token_into_context(context)
 
 print(context['access_token'])
 ```
 
-Run a GraphQL query:
 
+Run a GraphQL query:
 ```python
 query = """
     query searchEntities($cursor: PagingCursor, $query: String, $pageSize: Int) {
       search(query: $query, sort: DATE, cursor: $cursor, pageSize: $pageSize) {
         totalResults
         cursor
         entries {
@@ -68,15 +73,14 @@
     "pageSize": 1
 }
 
 response = cluedin.gql.gql(context, query, variables)
 ```
 
 Get paged results:
-
 ```python
 import numpy as np
 import pandas as pd
 
 query = """
     query searchEntities($cursor: PagingCursor, $query: String, $pageSize: Int) {
       search(query: $query, sort: DATE, cursor: $cursor, pageSize: $pageSize) {
```

