# Comparing `tmp/butterflymx-0.1.0.tar.gz` & `tmp/butterflymx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butterflymx-0.1.0.tar", max compression
+gzip compressed data, was "butterflymx-0.1.1.tar", max compression
```

## Comparing `butterflymx-0.1.0.tar` & `butterflymx-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-05-01 12:35:35.508797 butterflymx-0.1.0/LICENSE
--rw-r--r--   0        0        0       63 2023-05-01 12:35:35.508862 butterflymx-0.1.0/README.md
--rw-r--r--   0        0        0       93 2023-05-06 01:46:26.714043 butterflymx-0.1.0/butterflymx/__init__.py
--rw-r--r--   0        0        0     5230 2023-05-06 15:03:11.286697 butterflymx-0.1.0/butterflymx/butterflymx.py
--rw-r--r--   0        0        0       49 2023-05-06 01:36:17.661480 butterflymx-0.1.0/butterflymx/graphql/__init__.py
--rw-r--r--   0        0        0     3013 2023-05-06 02:15:53.991406 butterflymx-0.1.0/butterflymx/graphql/query_builder.py
--rw-r--r--   0        0        0      150 2023-05-06 01:45:36.640453 butterflymx-0.1.0/butterflymx/models/__init__.py
--rw-r--r--   0        0        0      424 2023-05-06 01:45:06.261959 butterflymx-0.1.0/butterflymx/models/butterflymx.py
--rw-r--r--   0        0        0      519 2023-05-06 01:45:10.029747 butterflymx-0.1.0/butterflymx/models/login.py
--rw-r--r--   0        0        0        0 2023-05-07 16:02:09.666488 butterflymx-0.1.0/butterflymx/py.typed
--rw-r--r--   0        0        0     6854 2023-05-07 16:05:53.102547 butterflymx-0.1.0/butterflymx/request_client.py
--rw-r--r--   0        0        0      203 2023-05-06 00:16:46.612362 butterflymx-0.1.0/butterflymx/utils.py
--rw-r--r--   0        0        0      675 2023-05-07 16:06:49.893362 butterflymx-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      818 1970-01-01 00:00:00.000000 butterflymx-0.1.0/setup.py
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 butterflymx-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-01 12:35:35.508797 butterflymx-0.1.1/LICENSE
+-rw-r--r--   0        0        0       63 2023-05-01 12:35:35.508862 butterflymx-0.1.1/README.md
+-rw-r--r--   0        0        0       93 2023-05-06 01:46:26.714043 butterflymx-0.1.1/butterflymx/__init__.py
+-rw-r--r--   0        0        0     5230 2023-05-06 15:03:11.286697 butterflymx-0.1.1/butterflymx/butterflymx.py
+-rw-r--r--   0        0        0       49 2023-05-06 01:36:17.661480 butterflymx-0.1.1/butterflymx/graphql/__init__.py
+-rw-r--r--   0        0        0     3013 2023-05-06 02:15:53.991406 butterflymx-0.1.1/butterflymx/graphql/query_builder.py
+-rw-r--r--   0        0        0      150 2023-05-06 01:45:36.640453 butterflymx-0.1.1/butterflymx/models/__init__.py
+-rw-r--r--   0        0        0      424 2023-05-06 01:45:06.261959 butterflymx-0.1.1/butterflymx/models/butterflymx.py
+-rw-r--r--   0        0        0      519 2023-05-06 01:45:10.029747 butterflymx-0.1.1/butterflymx/models/login.py
+-rw-r--r--   0        0        0        0 2023-05-07 16:02:09.666488 butterflymx-0.1.1/butterflymx/py.typed
+-rw-r--r--   0        0        0     6854 2023-05-07 16:05:53.102547 butterflymx-0.1.1/butterflymx/request_client.py
+-rw-r--r--   0        0        0      203 2023-05-06 00:16:46.612362 butterflymx-0.1.1/butterflymx/utils.py
+-rw-r--r--   0        0        0      800 2023-05-07 16:09:59.765637 butterflymx-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 butterflymx-0.1.1/setup.py
+-rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 butterflymx-0.1.1/PKG-INFO
```

### Comparing `butterflymx-0.1.0/LICENSE` & `butterflymx-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `butterflymx-0.1.0/butterflymx/butterflymx.py` & `butterflymx-0.1.1/butterflymx/butterflymx.py`

 * *Files identical despite different names*

### Comparing `butterflymx-0.1.0/butterflymx/graphql/query_builder.py` & `butterflymx-0.1.1/butterflymx/graphql/query_builder.py`

 * *Files identical despite different names*

### Comparing `butterflymx-0.1.0/butterflymx/models/login.py` & `butterflymx-0.1.1/butterflymx/models/login.py`

 * *Files identical despite different names*

### Comparing `butterflymx-0.1.0/butterflymx/request_client.py` & `butterflymx-0.1.1/butterflymx/request_client.py`

 * *Files identical despite different names*

### Comparing `butterflymx-0.1.0/pyproject.toml` & `butterflymx-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 [tool.poetry]
 name = "butterflymx"
-version = "0.1.0"
+version = "0.1.1"
 description = "A reverse-engineered ButterflyMX app API wrapper"
 authors = ["Milo Weinberg <iapetus011@gmail.com>"]
 readme = "README.md"
+repository = "https://github.com/Iapetus-11/ButterflyMX"
+keywords = ["butterflymx", "butterflymx-api", "butterflymx-graphql"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "^3.8.4"
 beautifulsoup4 = "^4.12.2"
 ruff = "^0.0.265"
 
@@ -25,8 +27,7 @@
 python_version = "3.10"
 warn_unused_configs = true
 namespace_packages = true
 explicit_package_bases = true
 
 [tool.ruff]
 line-length = 100
-
```

### Comparing `butterflymx-0.1.0/setup.py` & `butterflymx-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 install_requires = \
 ['aiohttp>=3.8.4,<4.0.0',
  'beautifulsoup4>=4.12.2,<5.0.0',
  'ruff>=0.0.265,<0.0.266']
 
 setup_kwargs = {
     'name': 'butterflymx',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A reverse-engineered ButterflyMX app API wrapper',
     'long_description': '# ButterflyMX\nA reverse-engineered ButterflyMX app API wrapper\n',
     'author': 'Milo Weinberg',
     'author_email': 'iapetus011@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'None',
+    'url': 'https://github.com/Iapetus-11/ButterflyMX',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.10,<4.0',
 }
```

### Comparing `butterflymx-0.1.0/PKG-INFO` & `butterflymx-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: butterflymx
-Version: 0.1.0
+Version: 0.1.1
 Summary: A reverse-engineered ButterflyMX app API wrapper
+Home-page: https://github.com/Iapetus-11/ButterflyMX
+Keywords: butterflymx,butterflymx-api,butterflymx-graphql
 Author: Milo Weinberg
 Author-email: iapetus011@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: ruff (>=0.0.265,<0.0.266)
+Project-URL: Repository, https://github.com/Iapetus-11/ButterflyMX
 Description-Content-Type: text/markdown
 
 # ButterflyMX
 A reverse-engineered ButterflyMX app API wrapper
```

