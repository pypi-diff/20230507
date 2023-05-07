# Comparing `tmp/deadnews_template_python-1.0.2a5.tar.gz` & `tmp/deadnews_template_python-1.0.2a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deadnews_template_python-1.0.2a5.tar", max compression
+gzip compressed data, was "deadnews_template_python-1.0.2a6.tar", max compression
```

## Comparing `deadnews_template_python-1.0.2a5.tar` & `deadnews_template_python-1.0.2a6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2023-05-04 01:29:42.068787 deadnews_template_python-1.0.2a5/LICENSE
--rw-r--r--   0        0        0      845 2023-05-04 01:29:42.068787 deadnews_template_python-1.0.2a5/README.md
--rw-r--r--   0        0        0     2363 2023-05-04 01:30:04.224918 deadnews_template_python-1.0.2a5/pyproject.toml
--rw-r--r--   0        0        0      160 2023-05-04 01:29:42.068787 deadnews_template_python-1.0.2a5/src/deadnews_template_python/__init__.py
--rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 deadnews_template_python-1.0.2a5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-04 01:39:34.631887 deadnews_template_python-1.0.2a6/LICENSE
+-rw-r--r--   0        0        0      845 2023-05-04 01:39:34.631887 deadnews_template_python-1.0.2a6/README.md
+-rw-r--r--   0        0        0     2363 2023-05-04 01:39:51.584123 deadnews_template_python-1.0.2a6/pyproject.toml
+-rw-r--r--   0        0        0      160 2023-05-04 01:39:34.631887 deadnews_template_python-1.0.2a6/src/deadnews_template_python/__init__.py
+-rw-r--r--   0        0        0     1508 1970-01-01 00:00:00.000000 deadnews_template_python-1.0.2a6/PKG-INFO
```

### Comparing `deadnews_template_python-1.0.2a5/LICENSE` & `deadnews_template_python-1.0.2a6/LICENSE`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-1.0.2a5/README.md` & `deadnews_template_python-1.0.2a6/README.md`

 * *Files identical despite different names*

### Comparing `deadnews_template_python-1.0.2a5/pyproject.toml` & `deadnews_template_python-1.0.2a6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "deadnews-template-python"
-version = "1.0.2-alpha.5"
+version = "1.0.2-alpha.6"
 description = "Python Project Template"
 authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/deadnews-template-python"
 repository = "https://github.com/DeadNews/deadnews-template-python"
 keywords = ["python", "template", "layout"]
```

### Comparing `deadnews_template_python-1.0.2a5/PKG-INFO` & `deadnews_template_python-1.0.2a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deadnews-template-python
-Version: 1.0.2a5
+Version: 1.0.2a6
 Summary: Python Project Template
 Home-page: https://github.com/DeadNews/deadnews-template-python
 License: MIT
 Keywords: python,template,layout
 Author: DeadNews
 Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.10,<4.0
```

