# Comparing `tmp/hyperfast_python_template-0.4.8.tar.gz` & `tmp/hyperfast_python_template-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfast_python_template-0.4.8.tar", max compression
+gzip compressed data, was "hyperfast_python_template-0.4.9.tar", max compression
```

## Comparing `hyperfast_python_template-0.4.8.tar` & `hyperfast_python_template-0.4.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-05-01 11:44:46.529304 hyperfast_python_template-0.4.8/LICENSE
--rw-r--r--   0        0        0     2573 2023-05-01 11:44:46.529304 hyperfast_python_template-0.4.8/README.md
--rw-r--r--   0        0        0     2991 2023-05-01 11:45:01.665567 hyperfast_python_template-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      323 2023-05-01 11:44:46.529304 hyperfast_python_template-0.4.8/src/hyperfastpy/__cli__.py
--rw-r--r--   0        0        0      135 2023-05-01 11:44:46.529304 hyperfast_python_template-0.4.8/src/hyperfastpy/__init__.py
--rw-r--r--   0        0        0       22 2023-05-01 11:45:01.613566 hyperfast_python_template-0.4.8/src/hyperfastpy/_version.py
--rw-r--r--   0        0        0      272 2023-05-01 11:45:01.613566 hyperfast_python_template-0.4.8/src/hyperfastpy/conf/about/__init__.yaml
--rw-r--r--   0        0        0      243 2023-05-01 11:44:46.529304 hyperfast_python_template-0.4.8/src/hyperfastpy/project.toml
--rw-r--r--   0        0        0        0 2023-05-01 11:44:46.529304 hyperfast_python_template-0.4.8/src/hyperfastpy/py.typed
--rw-r--r--   0        0        0      242 2023-05-01 11:44:46.529304 hyperfast_python_template-0.4.8/src/hyperfastpy/pyproject.toml
--rw-r--r--   0        0        0     3239 1970-01-01 00:00:00.000000 hyperfast_python_template-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-05 01:02:42.633668 hyperfast_python_template-0.4.9/LICENSE
+-rw-r--r--   0        0        0     2573 2023-05-05 01:02:42.633668 hyperfast_python_template-0.4.9/README.md
+-rw-r--r--   0        0        0     2991 2023-05-05 01:02:59.541535 hyperfast_python_template-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0      323 2023-05-05 01:02:42.637668 hyperfast_python_template-0.4.9/src/hyperfastpy/__cli__.py
+-rw-r--r--   0        0        0      135 2023-05-05 01:02:42.637668 hyperfast_python_template-0.4.9/src/hyperfastpy/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-05 01:02:59.493535 hyperfast_python_template-0.4.9/src/hyperfastpy/_version.py
+-rw-r--r--   0        0        0      272 2023-05-05 01:02:59.493535 hyperfast_python_template-0.4.9/src/hyperfastpy/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      243 2023-05-05 01:02:42.637668 hyperfast_python_template-0.4.9/src/hyperfastpy/project.toml
+-rw-r--r--   0        0        0        0 2023-05-05 01:02:42.637668 hyperfast_python_template-0.4.9/src/hyperfastpy/py.typed
+-rw-r--r--   0        0        0      242 2023-05-05 01:02:42.637668 hyperfast_python_template-0.4.9/src/hyperfastpy/pyproject.toml
+-rw-r--r--   0        0        0     3239 1970-01-01 00:00:00.000000 hyperfast_python_template-0.4.9/PKG-INFO
```

### Comparing `hyperfast_python_template-0.4.8/LICENSE` & `hyperfast_python_template-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.4.8/README.md` & `hyperfast_python_template-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.4.8/pyproject.toml` & `hyperfast_python_template-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperfast-python-template"
-version = "0.4.8"
+version = "0.4.9"
 description = "A python template that helps you jump start your project"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyperfast-python.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyperfast-python-template"
 readme = "README.md"
 packages = [{ include = "hyperfastpy", from = "src" }]
```

### Comparing `hyperfast_python_template-0.4.8/PKG-INFO` & `hyperfast_python_template-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperfast-python-template
-Version: 0.4.8
+Version: 0.4.9
 Summary: A python template that helps you jump start your project
 Home-page: https://hyperfast-python.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

