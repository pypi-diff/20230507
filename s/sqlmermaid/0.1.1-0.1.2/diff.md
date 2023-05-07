# Comparing `tmp/sqlmermaid-0.1.1.tar.gz` & `tmp/sqlmermaid-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmermaid-0.1.1.tar", last modified: Sat May 14 20:36:53 2022, max compression
+gzip compressed data, was "sqlmermaid-0.1.2.tar", last modified: Sun May  7 13:01:45 2023, max compression
```

## Comparing `sqlmermaid-0.1.1.tar` & `sqlmermaid-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0      583 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      565 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/.github/workflows/twine_release.yml
--rw-r--r--   0        0        0     1770 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/.gitignore
--rw-r--r--   0        0        0      248 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/.readthedocs.yml
--rw-r--r--   0        0        0     1056 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/LICENSE
--rw-r--r--   0        0        0     2059 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/README.md
--rw-r--r--   0        0        0       98 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/docs/api/sqlmermaid.format_col_type.rst
--rw-r--r--   0        0        0       86 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/docs/api/sqlmermaid.get_mermaid.rst
--rw-r--r--   0        0        0       98 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/docs/api/sqlmermaid.open_in_browser.rst
--rw-r--r--   0        0        0       74 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/docs/api/sqlmermaid.to_file.rst
--rw-r--r--   0        0        0       98 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/docs/api/sqlmermaid.to_mermaid_node.rst
--rw-r--r--   0        0        0       39 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/docs/autosumm.rst
--rw-r--r--   0        0        0     2430 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/docs/conf.py
--rw-r--r--   0        0        0      263 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/docs/index.rst
--rw-r--r--   0        0        0      137 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/docs/notebooks/doc-000-intro.rst
--rw-r--r--   0        0        0     1832 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/docs/notebooks/doc-001-quickstart.rst
--rw-r--r--   0        0        0     1153 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/docs/notebooks/doc-002-multi-fk.rst
--rw-r--r--   0        0        0      102 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/docs/release_notes/main.rst
--rw-r--r--   0        0        0       33 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/docs/release_notes/v0.0.0.rst
--rw-r--r--   0        0        0       38 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/docs/release_notes/v0.1.0.rst
--rw-r--r--   0        0        0       29 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/docs/release_notes/v0.1.1.rst
--rw-r--r--   0        0        0      827 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/notebooks/doc-000-intro.ipynb
--rw-r--r--   0        0        0     3606 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/notebooks/doc-001-quickstart.ipynb
--rw-r--r--   0        0        0     2672 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/notebooks/doc-002-multi-fk.ipynb
--rw-r--r--   0        0        0      560 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3037 2022-05-14 20:36:46.612103 sqlmermaid-0.1.1/sqlmermaid.py
--rw-r--r--   0        0        0     2555 1970-01-01 00:00:00.000000 sqlmermaid-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      565 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/.github/workflows/twine_release.yml
+-rw-r--r--   0        0        0     1770 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/.gitignore
+-rw-r--r--   0        0        0      248 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/.readthedocs.yml
+-rw-r--r--   0        0        0     1056 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2059 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/README.md
+-rw-r--r--   0        0        0       98 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/docs/api/sqlmermaid.format_col_type.rst
+-rw-r--r--   0        0        0       86 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/docs/api/sqlmermaid.get_mermaid.rst
+-rw-r--r--   0        0        0       98 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/docs/api/sqlmermaid.open_in_browser.rst
+-rw-r--r--   0        0        0       74 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/docs/api/sqlmermaid.to_file.rst
+-rw-r--r--   0        0        0       98 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/docs/api/sqlmermaid.to_mermaid_node.rst
+-rw-r--r--   0        0        0       39 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/docs/autosumm.rst
+-rw-r--r--   0        0        0     2430 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/docs/conf.py
+-rw-r--r--   0        0        0      263 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/docs/index.rst
+-rw-r--r--   0        0        0      137 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/docs/notebooks/doc-000-intro.rst
+-rw-r--r--   0        0        0     1832 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/docs/notebooks/doc-001-quickstart.rst
+-rw-r--r--   0        0        0     1153 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/docs/notebooks/doc-002-multi-fk.rst
+-rw-r--r--   0        0        0      102 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/docs/release_notes/main.rst
+-rw-r--r--   0        0        0       33 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/docs/release_notes/v0.0.0.rst
+-rw-r--r--   0        0        0       38 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/docs/release_notes/v0.1.0.rst
+-rw-r--r--   0        0        0       29 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/docs/release_notes/v0.1.1.rst
+-rw-r--r--   0        0        0       50 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/docs/release_notes/v0.1.2.rst
+-rw-r--r--   0        0        0      827 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/notebooks/doc-000-intro.ipynb
+-rw-r--r--   0        0        0     3606 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/notebooks/doc-001-quickstart.ipynb
+-rw-r--r--   0        0        0     2672 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/notebooks/doc-002-multi-fk.ipynb
+-rw-r--r--   0        0        0      567 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3026 2023-05-07 13:01:38.434085 sqlmermaid-0.1.2/sqlmermaid.py
+-rw-r--r--   0        0        0     2562 1970-01-01 00:00:00.000000 sqlmermaid-0.1.2/PKG-INFO
```

### Comparing `sqlmermaid-0.1.1/.github/workflows/test.yml` & `sqlmermaid-0.1.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `sqlmermaid-0.1.1/.github/workflows/twine_release.yml` & `sqlmermaid-0.1.2/.github/workflows/twine_release.yml`

 * *Files identical despite different names*

### Comparing `sqlmermaid-0.1.1/.gitignore` & `sqlmermaid-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlmermaid-0.1.1/LICENSE` & `sqlmermaid-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmermaid-0.1.1/README.md` & `sqlmermaid-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sqlmermaid-0.1.1/docs/conf.py` & `sqlmermaid-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sqlmermaid-0.1.1/docs/notebooks/doc-001-quickstart.rst` & `sqlmermaid-0.1.2/docs/notebooks/doc-001-quickstart.rst`

 * *Files identical despite different names*

### Comparing `sqlmermaid-0.1.1/docs/notebooks/doc-002-multi-fk.rst` & `sqlmermaid-0.1.2/docs/notebooks/doc-002-multi-fk.rst`

 * *Files identical despite different names*

### Comparing `sqlmermaid-0.1.1/notebooks/doc-000-intro.ipynb` & `sqlmermaid-0.1.2/notebooks/doc-000-intro.ipynb`

 * *Files identical despite different names*

### Comparing `sqlmermaid-0.1.1/notebooks/doc-001-quickstart.ipynb` & `sqlmermaid-0.1.2/notebooks/doc-001-quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `sqlmermaid-0.1.1/notebooks/doc-002-multi-fk.ipynb` & `sqlmermaid-0.1.2/notebooks/doc-002-multi-fk.ipynb`

 * *Files identical despite different names*

### Comparing `sqlmermaid-0.1.1/pyproject.toml` & `sqlmermaid-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "sqlmermaid"
 dynamic = ["version", "description"]
 authors = [{name = "Endre Márk Borza", email = "endremborza@gmail.com"}]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.8"
-dependencies = ["sqlalchemy"]
+dependencies = ["sqlalchemy>=2.0.0"]
 
 [project.optional-dependencies]
 test = ["branthebuilder"]
 doc = [
     "branthebuilder[doc]",
     "sphinxcontrib-mermaid"
 ]
```

### Comparing `sqlmermaid-0.1.1/sqlmermaid.py` & `sqlmermaid-0.1.2/sqlmermaid.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 import urllib
 import webbrowser
 from collections import defaultdict
 from pathlib import Path
 
 import sqlalchemy as sa
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 
 def get_mermaid(constr):
     engine = sa.create_engine(constr)
-    meta = sa.MetaData(bind=engine)
-    sa.MetaData.reflect(meta)
+    meta = sa.MetaData()
+    meta.reflect(bind=engine)
     nodes = [to_mermaid_node(table) for table in meta.tables.values()]
 
     edge_fstr = '%s ||--|{ %s : "%s"'
     edges = []
     for table_id, table in meta.tables.items():
         edge_dic = defaultdict(list)
         for fk in table.foreign_keys:
```

### Comparing `sqlmermaid-0.1.1/PKG-INFO` & `sqlmermaid-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: sqlmermaid
-Version: 0.1.1
+Version: 0.1.2
 Summary: Visualizing SQL databases
 Author-email: Endre Márk Borza <endremborza@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: sqlalchemy
+Requires-Dist: sqlalchemy>=2.0.0
 Requires-Dist: branthebuilder[doc] ; extra == "doc"
 Requires-Dist: sphinxcontrib-mermaid ; extra == "doc"
 Requires-Dist: branthebuilder ; extra == "test"
 Project-URL: Homepage, https://github.com/endremborza/sqlmermaid
 Provides-Extra: doc
 Provides-Extra: test
```

