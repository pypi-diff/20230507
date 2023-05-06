# Comparing `tmp/optimal_loc-0.0.1.tar.gz` & `tmp/optimal_loc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimal_loc-0.0.1.tar", max compression
+gzip compressed data, was "optimal_loc-0.0.2.tar", max compression
```

## Comparing `optimal_loc-0.0.1.tar` & `optimal_loc-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-01 00:26:25.432650 optimal_loc-0.0.1/README.md
--rw-r--r--   0        0        0       27 2023-04-30 23:48:01.553355 optimal_loc-0.0.1/optimal_loc/__init__.py
--rw-r--r--   0        0        0      354 2023-04-30 23:49:23.324892 optimal_loc-0.0.1/optimal_loc/optimal_loc.py
--rw-r--r--   0        0        0      719 2023-05-01 00:25:16.938155 optimal_loc-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      938 1970-01-01 00:00:00.000000 optimal_loc-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.0.2/LICENSE
+-rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.0.2/README.md
+-rw-r--r--   0        0        0       27 2023-04-30 23:48:01.553355 optimal_loc-0.0.2/optimal_loc/__init__.py
+-rw-r--r--   0        0        0     8647 2023-05-06 22:13:25.474844 optimal_loc-0.0.2/optimal_loc/optimal_loc.py
+-rw-r--r--   0        0        0      803 2023-05-06 23:00:37.866930 optimal_loc-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 optimal_loc-0.0.2/PKG-INFO
```

### Comparing `optimal_loc-0.0.1/pyproject.toml` & `optimal_loc-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 [tool.poetry]
 name = "optimal-loc"
-version = "0.0.1"
+version = "0.0.2"
 description = "A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs."
 
 authors = ["Sinan Demirhan <sdemirhan1320@gmail.com>"]
 readme = "README.md"
 packages = [{include = "optimal_loc"}]
 license = "MIT"
 homepage = "https://github.com/sinan-demirhan/optimal-loc"
 repository = "https://github.com/sinan-demirhan/optimal-loc"
 keywords = ["optimal_loc", "optimal-loc", "optimal", "optimal location", "optimal location finder"]
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
+numpy = "^1.20.2"
+pandas = "^1.2.4"
+pymongo = "^3.11.0"
+h3 = "^3.7.6"
+pulp = "^2.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `optimal_loc-0.0.1/PKG-INFO` & `optimal_loc-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,55 @@
 Metadata-Version: 2.1
 Name: optimal-loc
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs.
 Home-page: https://github.com/sinan-demirhan/optimal-loc
 License: MIT
 Keywords: optimal_loc,optimal-loc,optimal,optimal location,optimal location finder
 Author: Sinan Demirhan
 Author-email: sdemirhan1320@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: h3 (>=3.7.6,<4.0.0)
+Requires-Dist: numpy (>=1.20.2,<2.0.0)
+Requires-Dist: pandas (>=1.2.4,<2.0.0)
+Requires-Dist: pulp (>=2.4,<3.0)
+Requires-Dist: pymongo (>=3.11.0,<4.0.0)
 Project-URL: Repository, https://github.com/sinan-demirhan/optimal-loc
 Description-Content-Type: text/markdown
 
+# optimal-loc
+A python project which finds the optimal N locations in a given area according to the given location inputs.
 
+### Purpose of the Package
++ dsd
++ dsds
+
+### Features
+
+
+### Getting Started
++ Package can be found on pypi hence you can install it using pip.
+
+### Installation
+```bash
+pip install optimal_loc
+```
+
+### Usage
+```bash
+from optimal_loc import return_message
+output = return_message(my_input=5) # 50
+```
+
+### Contribution
+Contributions are welcome.
+Notice a bug let us know.
+
+### Author
++ Main Maintainer: Sinan Demirhan (SDemirhan)
```

