# Comparing `tmp/project_lighter-0.0.2a0.tar.gz` & `tmp/project_lighter-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project_lighter-0.0.2a0.tar", max compression
+gzip compressed data, was "project_lighter-0.0.2a1.tar", max compression
```

## Comparing `project_lighter-0.0.2a0.tar` & `project_lighter-0.0.2a1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1080 2023-05-05 21:09:25.315727 project_lighter-0.0.2a0/LICENSE
--rw-r--r--   0        0        0      485 2023-05-05 21:09:25.315727 project_lighter-0.0.2a0/README.md
--rw-r--r--   0        0        0       58 2023-05-05 21:11:47.209691 project_lighter-0.0.2a0/lighter/__init__.py
--rw-r--r--   0        0        0      125 2023-05-05 21:09:25.315727 project_lighter-0.0.2a0/lighter/callbacks/__init__.py
--rw-r--r--   0        0        0    13987 2023-05-05 21:09:25.315727 project_lighter-0.0.2a0/lighter/callbacks/logger.py
--rw-r--r--   0        0        0     5784 2023-05-05 21:09:25.315727 project_lighter-0.0.2a0/lighter/callbacks/utils.py
--rw-r--r--   0        0        0        0 2023-05-05 21:09:25.315727 project_lighter-0.0.2a0/lighter/callbacks/writer/__init__.py
--rw-r--r--   0        0        0     7593 2023-05-05 21:09:25.315727 project_lighter-0.0.2a0/lighter/callbacks/writer/base.py
--rw-r--r--   0        0        0     2662 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/callbacks/writer/file.py
--rw-r--r--   0        0        0     2427 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/callbacks/writer/table.py
--rw-r--r--   0        0        0    21386 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/system.py
--rw-r--r--   0        0        0       36 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/utils/__init__.py
--rw-r--r--   0        0        0     3510 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/utils/cli.py
--rw-r--r--   0        0        0     2352 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/utils/collate.py
--rw-r--r--   0        0        0     1424 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/utils/dynamic_imports.py
--rw-r--r--   0        0        0     3431 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/utils/freezer.py
--rw-r--r--   0        0        0     2618 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/utils/misc.py
--rw-r--r--   0        0        0     5881 2023-05-05 21:09:25.319727 project_lighter-0.0.2a0/lighter/utils/model.py
--rw-r--r--   0        0        0     4400 2023-05-05 21:11:47.153690 project_lighter-0.0.2a0/pyproject.toml
--rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 project_lighter-0.0.2a0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/LICENSE
+-rw-r--r--   0        0        0      485 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/README.md
+-rw-r--r--   0        0        0       67 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/__init__.py
+-rw-r--r--   0        0        0      125 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/callbacks/__init__.py
+-rw-r--r--   0        0        0    13987 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/callbacks/logger.py
+-rw-r--r--   0        0        0     5784 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/callbacks/utils.py
+-rw-r--r--   0        0        0        0 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/callbacks/writer/__init__.py
+-rw-r--r--   0        0        0     7593 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/callbacks/writer/base.py
+-rw-r--r--   0        0        0     2662 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/callbacks/writer/file.py
+-rw-r--r--   0        0        0     2427 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/callbacks/writer/table.py
+-rw-r--r--   0        0        0    21386 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/system.py
+-rw-r--r--   0        0        0       36 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/utils/__init__.py
+-rw-r--r--   0        0        0     3510 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/utils/cli.py
+-rw-r--r--   0        0        0     2352 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/utils/collate.py
+-rw-r--r--   0        0        0     1424 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/utils/dynamic_imports.py
+-rw-r--r--   0        0        0     3431 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/utils/freezer.py
+-rw-r--r--   0        0        0     2618 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/utils/misc.py
+-rw-r--r--   0        0        0     5881 2023-05-07 04:43:13.525977 project_lighter-0.0.2a1/lighter/utils/model.py
+-rw-r--r--   0        0        0       24 2023-05-07 04:43:34.398168 project_lighter-0.0.2a1/lighter/version.py
+-rw-r--r--   0        0        0     4399 2023-05-07 04:43:34.346168 project_lighter-0.0.2a1/pyproject.toml
+-rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 project_lighter-0.0.2a1/PKG-INFO
```

### Comparing `project_lighter-0.0.2a0/LICENSE` & `project_lighter-0.0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a0/lighter/callbacks/logger.py` & `project_lighter-0.0.2a1/lighter/callbacks/logger.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a0/lighter/callbacks/utils.py` & `project_lighter-0.0.2a1/lighter/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a0/lighter/callbacks/writer/base.py` & `project_lighter-0.0.2a1/lighter/callbacks/writer/base.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a0/lighter/callbacks/writer/file.py` & `project_lighter-0.0.2a1/lighter/callbacks/writer/file.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a0/lighter/callbacks/writer/table.py` & `project_lighter-0.0.2a1/lighter/callbacks/writer/table.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a0/lighter/system.py` & `project_lighter-0.0.2a1/lighter/system.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a0/lighter/utils/cli.py` & `project_lighter-0.0.2a1/lighter/utils/cli.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a0/lighter/utils/collate.py` & `project_lighter-0.0.2a1/lighter/utils/collate.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a0/lighter/utils/dynamic_imports.py` & `project_lighter-0.0.2a1/lighter/utils/dynamic_imports.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a0/lighter/utils/freezer.py` & `project_lighter-0.0.2a1/lighter/utils/freezer.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a0/lighter/utils/misc.py` & `project_lighter-0.0.2a1/lighter/utils/misc.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a0/lighter/utils/model.py` & `project_lighter-0.0.2a1/lighter/utils/model.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a0/pyproject.toml` & `project_lighter-0.0.2a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 lighter = "lighter.utils.cli:interface"
 
 [tool.poetry]
 name = "project-lighter"
-version = "0.0.2a0"
+version = "0.0.2a1"
 description = "YAML-based automated rapid prototyping framework for deep learning experiments"
 readme = "README.md"
 authors = ["Ibrahim Hadzic <ibrahimhadzic45@gmail.com>" ,
             "Suraj Pai <b.pai@maastrichtuniversity.nl>", 
             "Keno Bressem <kbressem@bwh.harvard.edu>"]
 license = "MIT"
 repository = "https://github.com/lighter/lighter"
@@ -178,8 +178,8 @@
     no-else-return,
 """
 generated-members = "torch.*"
 
 [tool.pylint.master]
 fail-under=8
 
-[tool.poetry_bumpversion.file."lighter/__init__.py"]
+[tool.poetry_bumpversion.file."lighter/version.py"]
```

### Comparing `project_lighter-0.0.2a0/PKG-INFO` & `project_lighter-0.0.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-lighter
-Version: 0.0.2a0
+Version: 0.0.2a1
 Summary: YAML-based automated rapid prototyping framework for deep learning experiments
 Home-page: https://github.com/lighter/lighter
 License: MIT
 Author: Ibrahim Hadzic
 Author-email: ibrahimhadzic45@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

