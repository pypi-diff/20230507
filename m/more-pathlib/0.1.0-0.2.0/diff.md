# Comparing `tmp/more_pathlib-0.1.0.tar.gz` & `tmp/more_pathlib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "more_pathlib-0.1.0.tar", max compression
+gzip compressed data, was "more_pathlib-0.2.0.tar", max compression
```

## Comparing `more_pathlib-0.1.0.tar` & `more_pathlib-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11357 2022-11-21 05:52:47.000493 more_pathlib-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2022-11-21 05:52:47.000493 more_pathlib-0.1.0/more_pathlib/__init__.py
--rw-r--r--   0        0        0      312 2022-11-21 05:52:47.000493 more_pathlib-0.1.0/more_pathlib/common.py
--rw-r--r--   0        0        0      861 2022-11-21 05:52:47.000493 more_pathlib-0.1.0/more_pathlib/json.py
--rw-r--r--   0        0        0      796 2022-11-21 05:52:47.000493 more_pathlib-0.1.0/more_pathlib/pickle.py
--rw-r--r--   0        0        0        0 2022-11-21 05:52:47.000493 more_pathlib-0.1.0/more_pathlib/py.typed
--rw-r--r--   0        0        0      577 2022-11-21 05:52:47.000493 more_pathlib-0.1.0/more_pathlib/rm.py
--rw-r--r--   0        0        0     1189 2022-11-21 05:52:47.000493 more_pathlib-0.1.0/more_pathlib/validation.py
--rw-r--r--   0        0        0      894 2022-11-21 05:52:47.000493 more_pathlib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      507 2022-11-21 05:52:57.943766 more_pathlib-0.1.0/setup.py
--rw-r--r--   0        0        0      351 2022-11-21 05:52:57.944066 more_pathlib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-07 16:05:50.317062 more_pathlib-0.2.0/LICENSE
+-rw-r--r--   0        0        0      467 2023-05-07 16:05:50.321062 more_pathlib-0.2.0/more_pathlib/__init__.py
+-rw-r--r--   0        0        0      338 2023-05-07 16:05:50.321062 more_pathlib-0.2.0/more_pathlib/common.py
+-rw-r--r--   0        0        0      810 2023-05-07 16:05:50.321062 more_pathlib-0.2.0/more_pathlib/copy.py
+-rw-r--r--   0        0        0      900 2023-05-07 16:05:50.321062 more_pathlib-0.2.0/more_pathlib/json.py
+-rw-r--r--   0        0        0      843 2023-05-07 16:05:50.321062 more_pathlib-0.2.0/more_pathlib/pickle.py
+-rw-r--r--   0        0        0        0 2023-05-07 16:05:50.321062 more_pathlib-0.2.0/more_pathlib/py.typed
+-rw-r--r--   0        0        0      440 2023-05-07 16:05:50.321062 more_pathlib-0.2.0/more_pathlib/rm.py
+-rw-r--r--   0        0        0     1189 2023-05-07 16:05:50.321062 more_pathlib-0.2.0/more_pathlib/validation.py
+-rw-r--r--   0        0        0      946 2023-05-07 16:05:50.321062 more_pathlib-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      559 2023-05-07 16:06:08.025456 more_pathlib-0.2.0/setup.py
+-rw-r--r--   0        0        0      403 2023-05-07 16:06:08.025735 more_pathlib-0.2.0/PKG-INFO
```

### Comparing `more_pathlib-0.1.0/LICENSE` & `more_pathlib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `more_pathlib-0.1.0/more_pathlib/json.py` & `more_pathlib-0.2.0/more_pathlib/json.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 _JSON_EXTENSIONS = frozenset(('.json',))
 
 
 def dump_json(
     obj: Any,  # noqa: WPS110
     path: Path,
     *,
-    strict: bool = False,
+    validate_parent_dir: bool = False,
     encoding: str = 'utf-8',
     **kwargs: Any,
 ) -> None:
     before_dump_hook(
         path,
-        strict=strict,
+        validate_parent_dir=validate_parent_dir,
     )
 
     with open(path, 'w', encoding=encoding) as out:
         json.dump(
             obj,
             out,
             **kwargs,
```

### Comparing `more_pathlib-0.1.0/more_pathlib/validation.py` & `more_pathlib-0.2.0/more_pathlib/validation.py`

 * *Files identical despite different names*

### Comparing `more_pathlib-0.1.0/pyproject.toml` & `more_pathlib-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "more_pathlib"
-version = "0.1.0"
-description = ""
-authors = ["Timur Kasimov <t.kasimov@aventica.ru>"]
+version = "0.2.0"
+description = "Extending Python's pathlib with more useful functions."
+authors = ["Timur Kasimov <tkasimov@icloud.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
 wemake-python-styleguide = "^0.17.0"
 flake8-colors = "^0.1.9"
```

