# Comparing `tmp/savvy_rest-0.0.1.tar.gz` & `tmp/savvy_rest-0.0.1.dev0.tar.gz`

## Comparing `savvy_rest-0.0.1.tar` & `savvy_rest-0.0.1.dev0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/.flake8
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/.gitattributes
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/mypy.ini
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/pylintrc
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/requirements-dev.txt
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/requirements.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/tox.ini
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/src/savvy_rest/__about__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/src/savvy_rest/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/src/savvy_rest/cli/__init__.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/src/savvy_rest/cli/cli.py
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/src/savvy_rest/cli/cli_manager.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/src/savvy_rest/templates/structure.yaml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/README.md
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 savvy_rest-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/.flake8
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/.gitattributes
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/mypy.ini
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/pylintrc
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/requirements-dev.txt
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/requirements.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/tox.ini
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/src/savvy_rest/__about__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/src/savvy_rest/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/src/savvy_rest/cli/__init__.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/src/savvy_rest/cli/cli.py
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/src/savvy_rest/cli/cli_manager.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/src/savvy_rest/templates/structure.yaml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/tests/__init__.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/LICENSE.txt
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/README.md
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/pyproject.toml
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 savvy_rest-0.0.1.dev0/PKG-INFO
```

### Comparing `savvy_rest-0.0.1/.pre-commit-config.yaml` & `savvy_rest-0.0.1.dev0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `savvy_rest-0.0.1/src/savvy_rest/cli/cli.py` & `savvy_rest-0.0.1.dev0/src/savvy_rest/cli/cli.py`

 * *Files identical despite different names*

### Comparing `savvy_rest-0.0.1/src/savvy_rest/cli/cli_manager.py` & `savvy_rest-0.0.1.dev0/src/savvy_rest/cli/cli_manager.py`

 * *Files identical despite different names*

### Comparing `savvy_rest-0.0.1/.gitignore` & `savvy_rest-0.0.1.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `savvy_rest-0.0.1/LICENSE.txt` & `savvy_rest-0.0.1.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `savvy_rest-0.0.1/pyproject.toml` & `savvy_rest-0.0.1.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `savvy_rest-0.0.1/PKG-INFO` & `savvy_rest-0.0.1.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: savvy-rest
-Version: 0.0.1
+Version: 0.0.1.dev0
 Summary: A comprehensive framework for testing RESTful APIs.
 Project-URL: Homepage, https://github.com/qatoolist/savvy-rest
 Project-URL: Documentation, https://github.com/qatoolist/savvy-rest#readme
 Project-URL: Issues, https://github.com/qatoolist/savvy-rest/issues
 Project-URL: Source, https://github.com/qatoolist/savvy-rest
 Project-URL: Repository, https://github.com/qatoolist/savvy-rest
 Project-URL: Changelog, https://github.com/qatoolist/savvy-rest/releases
```

