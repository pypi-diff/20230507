# Comparing `tmp/prelude_parser-0.1.0.tar.gz` & `tmp/prelude_parser-0.1.1.tar.gz`

## Comparing `prelude_parser-0.1.0.tar` & `prelude_parser-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 prelude_parser-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123      539 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/.github/release-draft-template.yml
--rw-r--r--   0     1001      123     2599 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/.github/workflows/pypi_publish.yml
--rw-r--r--   0     1001      123      309 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/.github/workflows/release-drafter.yml
--rw-r--r--   0     1001      123     1884 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/.github/workflows/testing.yml
--rw-r--r--   0     1001      123      686 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/.gitignore
--rw-r--r--   0     1001      123      640 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     7942 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/CONTRIBUTING.md
--rw-r--r--   0     1001      123     1080 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/LICENSE
--rw-r--r--   0     1001      123     1162 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/README.md
--rw-r--r--   0     1001      123       81 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/prelude_parser/__init__.py
--rw-r--r--   0     1001      123      293 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/prelude_parser/_prelude_parser.pyi
--rw-r--r--   0     1001      123     1966 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/prelude_parser/parser.py
--rw-r--r--   0     1001      123        0 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/prelude_parser/py.typed
--rw-r--r--   0     1001      123     1326 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123       89 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/requirements-dev.txt
--rw-r--r--   0     1001      123     3469 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123        0 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/tests/__init__.py
--rw-r--r--   0     1001      123     1304 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/tests/assets/test1.xml
--rw-r--r--   0     1001      123     1839 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/tests/assets/test2.xml
--rw-r--r--   0     1001      123     2122 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/tests/assets/test3.xml
--rw-r--r--   0     1001      123      312 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/tests/conftest.py
--rw-r--r--   0     1001      123     2474 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/tests/test_parser.py
--rw-r--r--   0     1001      123     8093 2023-05-07 00:33:55.000000 prelude_parser-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1697 1970-01-01 00:00:00.000000 prelude_parser-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 prelude_parser-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      123      539 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/.github/release-draft-template.yml
+-rw-r--r--   0     1001      123     2599 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/.github/workflows/pypi_publish.yml
+-rw-r--r--   0     1001      123      309 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/.github/workflows/release-drafter.yml
+-rw-r--r--   0     1001      123     1884 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/.github/workflows/testing.yml
+-rw-r--r--   0     1001      123      686 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/.gitignore
+-rw-r--r--   0     1001      123      640 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     7942 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     1080 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/LICENSE
+-rw-r--r--   0     1001      123     1162 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/README.md
+-rw-r--r--   0     1001      123       81 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/prelude_parser/__init__.py
+-rw-r--r--   0     1001      123      293 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/prelude_parser/_prelude_parser.pyi
+-rw-r--r--   0     1001      123     1966 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/prelude_parser/parser.py
+-rw-r--r--   0     1001      123        0 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/prelude_parser/py.typed
+-rw-r--r--   0     1001      123     1609 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      123       89 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/requirements-dev.txt
+-rw-r--r--   0     1001      123     3469 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/tests/__init__.py
+-rw-r--r--   0     1001      123     1304 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/tests/assets/test1.xml
+-rw-r--r--   0     1001      123     1839 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/tests/assets/test2.xml
+-rw-r--r--   0     1001      123     2122 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/tests/assets/test3.xml
+-rw-r--r--   0     1001      123      312 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/tests/conftest.py
+-rw-r--r--   0     1001      123     2474 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/tests/test_parser.py
+-rw-r--r--   0     1001      123     8093 2023-05-07 01:14:59.000000 prelude_parser-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     2011 1970-01-01 00:00:00.000000 prelude_parser-0.1.1/PKG-INFO
```

### Comparing `prelude_parser-0.1.0/.github/release-draft-template.yml` & `prelude_parser-0.1.1/.github/release-draft-template.yml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.0/.github/workflows/pypi_publish.yml` & `prelude_parser-0.1.1/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.0/.github/workflows/testing.yml` & `prelude_parser-0.1.1/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.0/.gitignore` & `prelude_parser-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.0/.pre-commit-config.yaml` & `prelude_parser-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.0/CONTRIBUTING.md` & `prelude_parser-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.0/LICENSE` & `prelude_parser-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.0/README.md` & `prelude_parser-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.0/prelude_parser/parser.py` & `prelude_parser-0.1.1/prelude_parser/parser.py`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.0/src/lib.rs` & `prelude_parser-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.0/tests/assets/test1.xml` & `prelude_parser-0.1.1/tests/assets/test1.xml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.0/tests/assets/test2.xml` & `prelude_parser-0.1.1/tests/assets/test2.xml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.0/tests/assets/test3.xml` & `prelude_parser-0.1.1/tests/assets/test3.xml`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.0/tests/test_parser.py` & `prelude_parser-0.1.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `prelude_parser-0.1.0/Cargo.lock` & `prelude_parser-0.1.1/Cargo.lock`

 * *Files identical despite different names*

```diff
@@ -78,15 +78,15 @@
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "prelude-parser"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "pyo3",
  "roxmltree",
 ]
 
 [[package]]
 name = "proc-macro2"
```

### Comparing `prelude_parser-0.1.0/PKG-INFO` & `prelude_parser-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 Metadata-Version: 2.1
 Name: prelude-parser
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Typing :: Typed
 Requires-Dist: camel-converter>=3.0.0
 License-File: LICENSE
+Keywords: prelude-edc,xml,parser
 Home-Page: https://github.com/pbs-data-solutions/prelude-parser
 Author-email: Paul Sanders <paul@pbsdatasolutions.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/pbs-data-solutions/prelude-parser
```

