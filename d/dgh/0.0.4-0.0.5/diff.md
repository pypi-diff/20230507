# Comparing `tmp/dgh-0.0.4.tar.gz` & `tmp/dgh-0.0.5.tar.gz`

## Comparing `dgh-0.0.4.tar` & `dgh-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 dgh-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dgh-0.0.4/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dgh-0.0.4/src/__init__.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 dgh-0.0.4/src/auxiliary.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 dgh-0.0.4/src/constants.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 dgh-0.0.4/src/dgh.py
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 dgh-0.0.4/src/fw.py
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 dgh-0.0.4/src/mappings.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dgh-0.0.4/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 dgh-0.0.4/LICENSE
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 dgh-0.0.4/README.md
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 dgh-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 dgh-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 dgh-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dgh-0.0.5/dgh/__init__.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 dgh-0.0.5/dgh/auxiliary.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 dgh-0.0.5/dgh/constants.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 dgh-0.0.5/dgh/dgh.py
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 dgh-0.0.5/dgh/fw.py
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 dgh-0.0.5/dgh/mappings.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dgh-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 dgh-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 dgh-0.0.5/README.md
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 dgh-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 dgh-0.0.5/PKG-INFO
```

### Comparing `dgh-0.0.4/src/auxiliary.py` & `dgh-0.0.5/dgh/auxiliary.py`

 * *Files identical despite different names*

### Comparing `dgh-0.0.4/src/dgh.py` & `dgh-0.0.5/dgh/dgh.py`

 * *Files identical despite different names*

### Comparing `dgh-0.0.4/src/fw.py` & `dgh-0.0.5/dgh/fw.py`

 * *Files identical despite different names*

### Comparing `dgh-0.0.4/src/mappings.py` & `dgh-0.0.5/dgh/mappings.py`

 * *Files identical despite different names*

### Comparing `dgh-0.0.4/LICENSE` & `dgh-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dgh-0.0.4/README.md` & `dgh-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dgh-0.0.4/pyproject.toml` & `dgh-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dgh"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   {name="Vladyslav Oles", email="vlad.oles@proton.me"},
 ]
 description = "Computing the Gromov–Hausdorff distance"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

### Comparing `dgh-0.0.4/PKG-INFO` & `dgh-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dgh
-Version: 0.0.4
+Version: 0.0.5
 Summary: Computing the Gromov–Hausdorff distance
 Project-URL: Homepage, https://github.com/pypa/dgh
 Project-URL: Bug Tracker, https://github.com/pypa/dgh/issues
 Author-email: Vladyslav Oles <vlad.oles@proton.me>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

