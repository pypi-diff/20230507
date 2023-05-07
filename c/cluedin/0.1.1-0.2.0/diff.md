# Comparing `tmp/cluedin-0.1.1.tar.gz` & `tmp/cluedin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cluedin-0.1.1.tar", max compression
+gzip compressed data, was "cluedin-0.2.0.tar", max compression
```

## Comparing `cluedin-0.1.1.tar` & `cluedin-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0        0 2023-05-02 20:10:19.990177 cluedin-0.1.1/README.md
--rw-r--r--   0        0        0       41 2023-05-05 20:11:46.996331 cluedin-0.1.1/cluedin/__init__.py
--rw-r--r--   0        0        0      684 2023-05-05 20:46:12.499526 cluedin-0.1.1/cluedin/auth.py
--rw-r--r--   0        0        0      292 2023-05-05 18:02:53.064080 cluedin-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 cluedin-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-02 20:10:19.990177 cluedin-0.2.0/README.md
+-rw-r--r--   0        0        0      119 2023-05-07 15:56:18.443909 cluedin-0.2.0/cluedin/__init__.py
+-rw-r--r--   0        0        0      664 2023-05-06 19:21:43.490227 cluedin-0.2.0/cluedin/auth.py
+-rw-r--r--   0        0        0     1120 2023-05-07 16:45:36.605300 cluedin-0.2.0/cluedin/gql.py
+-rw-r--r--   0        0        0      681 2023-05-07 15:56:40.250091 cluedin-0.2.0/cluedin/urls.py
+-rw-r--r--   0        0        0      264 2023-05-06 19:41:45.000595 cluedin-0.2.0/cluedin/utils.py
+-rw-r--r--   0        0        0      292 2023-05-07 16:51:57.219769 cluedin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 cluedin-0.2.0/PKG-INFO
```

### Comparing `cluedin-0.1.1/cluedin/auth.py` & `cluedin-0.2.0/cluedin/auth.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import requests
+from .urls import get_auth_url
 
 
 def get_token_response(context):
     headers = {
         'Content-Type': 'application/x-www-form-urlencoded'
     }
     data = {
         'username': context['user'],
         'password': context['password'],
         'client_id': context['organization'],
         'grant_type': 'password'
     }
     response = requests.post(
-        url=f'{context["protocol"]}://{context["organization"]}.{context["domain"]}/auth/connect/token',
+        url=f'{get_auth_url(context)}/connect/token',
         headers=headers,
         data=data)
     return response.json()
 
 
 def load_token_into_context(context):
     token_response = get_token_response(context)
```

### Comparing `cluedin-0.1.1/PKG-INFO` & `cluedin-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluedin
-Version: 0.1.1
+Version: 0.2.0
 Summary: 
 Author: Roman Klimenko
 Author-email: romaklimenko@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

