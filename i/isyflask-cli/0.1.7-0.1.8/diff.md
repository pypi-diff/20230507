# Comparing `tmp/isyflask_cli-0.1.7.tar.gz` & `tmp/isyflask_cli-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isyflask_cli-0.1.7.tar", max compression
+gzip compressed data, was "isyflask_cli-0.1.8.tar", max compression
```

## Comparing `isyflask_cli-0.1.7.tar` & `isyflask_cli-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1476 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/__init__.py
--rw-r--r--   0        0        0       51 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/__main__.py
--rw-r--r--   0        0        0      477 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/cli.py
--rw-r--r--   0        0        0     4980 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/globals.py
--rw-r--r--   0        0        0        0 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/src/model/__init__.py
--rw-r--r--   0        0        0     2503 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/src/model/model.py
--rw-r--r--   0        0        0        0 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/src/project/__init__.py
--rw-r--r--   0        0        0     2261 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/src/project/project.py
--rw-r--r--   0        0        0     1690 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/src/utils/folders.py
--rw-r--r--   0        0        0      712 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/src/utils/strings.py
--rw-r--r--   0        0        0     2263 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/isyflask_cli/src/utils/template_gen.py
--rw-r--r--   0        0        0      738 2023-04-12 06:30:52.118863 isyflask_cli-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2283 1970-01-01 00:00:00.000000 isyflask_cli-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     9000 2023-05-07 04:52:01.067242 isyflask_cli-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 04:52:01.067242 isyflask_cli-0.1.8/isyflask_cli/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-07 04:52:01.067242 isyflask_cli-0.1.8/isyflask_cli/__main__.py
+-rw-r--r--   0        0        0      477 2023-05-07 04:52:01.067242 isyflask_cli-0.1.8/isyflask_cli/cli.py
+-rw-r--r--   0        0        0     4980 2023-05-07 04:52:01.067242 isyflask_cli-0.1.8/isyflask_cli/globals.py
+-rw-r--r--   0        0        0        0 2023-05-07 04:52:01.067242 isyflask_cli-0.1.8/isyflask_cli/src/model/__init__.py
+-rw-r--r--   0        0        0     2503 2023-05-07 04:52:01.067242 isyflask_cli-0.1.8/isyflask_cli/src/model/model.py
+-rw-r--r--   0        0        0        0 2023-05-07 04:52:01.067242 isyflask_cli-0.1.8/isyflask_cli/src/project/__init__.py
+-rw-r--r--   0        0        0     2261 2023-05-07 04:52:01.067242 isyflask_cli-0.1.8/isyflask_cli/src/project/project.py
+-rw-r--r--   0        0        0     1690 2023-05-07 04:52:01.067242 isyflask_cli-0.1.8/isyflask_cli/src/utils/folders.py
+-rw-r--r--   0        0        0      712 2023-05-07 04:52:01.067242 isyflask_cli-0.1.8/isyflask_cli/src/utils/strings.py
+-rw-r--r--   0        0        0     2263 2023-05-07 04:52:01.067242 isyflask_cli-0.1.8/isyflask_cli/src/utils/template_gen.py
+-rw-r--r--   0        0        0      738 2023-05-07 04:52:01.067242 isyflask_cli-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     9807 1970-01-01 00:00:00.000000 isyflask_cli-0.1.8/PKG-INFO
```

### Comparing `isyflask_cli-0.1.7/isyflask_cli/globals.py` & `isyflask_cli-0.1.8/isyflask_cli/globals.py`

 * *Files identical despite different names*

### Comparing `isyflask_cli-0.1.7/isyflask_cli/src/model/model.py` & `isyflask_cli-0.1.8/isyflask_cli/src/model/model.py`

 * *Files identical despite different names*

### Comparing `isyflask_cli-0.1.7/isyflask_cli/src/project/project.py` & `isyflask_cli-0.1.8/isyflask_cli/src/project/project.py`

 * *Files identical despite different names*

### Comparing `isyflask_cli-0.1.7/isyflask_cli/src/utils/folders.py` & `isyflask_cli-0.1.8/isyflask_cli/src/utils/folders.py`

 * *Files identical despite different names*

### Comparing `isyflask_cli-0.1.7/isyflask_cli/src/utils/strings.py` & `isyflask_cli-0.1.8/isyflask_cli/src/utils/strings.py`

 * *Files identical despite different names*

### Comparing `isyflask_cli-0.1.7/isyflask_cli/src/utils/template_gen.py` & `isyflask_cli-0.1.8/isyflask_cli/src/utils/template_gen.py`

 * *Files identical despite different names*

### Comparing `isyflask_cli-0.1.7/pyproject.toml` & `isyflask_cli-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "isyflask-cli"
-version = "0.1.7"
+version = "0.1.8"
 description = "Un cli para manejar proyectos de API con flask"
 authors = ["David Cuy <david.cuy.sanchez@gmail.com>"]
 readme = "README.md"
 packages = [{include = "isyflask_cli"}]
 homepage = "https://github.com/DavidCuy/easyflask-cli"
 repository = "https://github.com/DavidCuy/easyflask-cli"
 documentation = "https://github.com/DavidCuy/easyflask-cli"
```

