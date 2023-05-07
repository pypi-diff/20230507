# Comparing `tmp/parse_stages-0.1.2.tar.gz` & `tmp/parse_stages-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parse_stages-0.1.2.tar", last modified: Sat Mar 11 19:50:45 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `parse_stages-0.1.2.tar` & `parse_stages-0.1.3.tar`

### file list

```diff
@@ -1,49 +1,30 @@
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-11 19:50:45.480252 parse_stages-0.1.2/
--rw-r--r--   0 roam      (1000) roam      (1000)      622 2023-03-11 17:41:05.000000 parse_stages-0.1.2/.editorconfig
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-11 19:50:45.476252 parse_stages-0.1.2/LICENSES/
--rw-r--r--   0 roam      (1000) roam      (1000)     1267 2023-03-11 16:43:11.000000 parse_stages-0.1.2/LICENSES/BSD-2-Clause.txt
--rw-r--r--   0 roam      (1000) roam      (1000)      355 2023-03-11 17:46:39.000000 parse_stages-0.1.2/MANIFEST.in
--rw-r--r--   0 roam      (1000) roam      (1000)     4809 2023-03-11 19:50:45.480252 parse_stages-0.1.2/PKG-INFO
--rw-r--r--   0 roam      (1000) roam      (1000)     4290 2023-03-11 18:22:51.000000 parse_stages-0.1.2/README.md
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-11 19:50:45.476252 parse_stages-0.1.2/config/
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-11 19:50:45.476252 parse_stages-0.1.2/config/ruff-all/
--rw-r--r--   0 roam      (1000) roam      (1000)      169 2023-03-11 16:43:11.000000 parse_stages-0.1.2/config/ruff-all/pyproject.toml
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-11 19:50:45.476252 parse_stages-0.1.2/config/ruff-base/
--rw-r--r--   0 roam      (1000) roam      (1000)      661 2023-03-11 16:43:11.000000 parse_stages-0.1.2/config/ruff-base/pyproject.toml
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-11 19:50:45.476252 parse_stages-0.1.2/config/ruff-most/
--rw-r--r--   0 roam      (1000) roam      (1000)      602 2023-03-11 16:43:11.000000 parse_stages-0.1.2/config/ruff-most/pyproject.toml
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-11 19:50:45.476252 parse_stages-0.1.2/docs/
--rw-r--r--   0 roam      (1000) roam      (1000)      728 2023-03-11 19:12:12.000000 parse_stages-0.1.2/docs/api.md
--rw-r--r--   0 roam      (1000) roam      (1000)     3042 2023-03-11 19:45:14.000000 parse_stages-0.1.2/docs/changes.md
--rw-r--r--   0 roam      (1000) roam      (1000)     4198 2023-03-11 19:45:14.000000 parse_stages-0.1.2/docs/index.md
--rw-r--r--   0 roam      (1000) roam      (1000)      860 2023-03-11 17:41:05.000000 parse_stages-0.1.2/docs/language.md
--rw-r--r--   0 roam      (1000) roam      (1000)     1223 2023-03-11 19:25:58.000000 parse_stages-0.1.2/mkdocs.yml
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-11 19:50:45.480252 parse_stages-0.1.2/nix/
--rw-r--r--   0 roam      (1000) roam      (1000)      517 2023-03-11 19:38:09.000000 parse_stages-0.1.2/nix/mkdocs.nix
--rw-r--r--   0 roam      (1000) roam      (1000)      470 2023-03-11 16:43:11.000000 parse_stages-0.1.2/nix/python-pytest.nix
--rwxr-xr-x   0 roam      (1000) roam      (1000)      266 2023-03-11 16:43:11.000000 parse_stages-0.1.2/nix/reformat.sh
--rwxr-xr-x   0 roam      (1000) roam      (1000)      735 2023-03-11 16:43:11.000000 parse_stages-0.1.2/nix/run-pytest.sh
--rw-r--r--   0 roam      (1000) roam      (1000)     2430 2023-03-11 18:31:59.000000 parse_stages-0.1.2/pyproject.toml
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-11 19:50:45.480252 parse_stages-0.1.2/requirements/
--rw-r--r--   0 roam      (1000) roam      (1000)      121 2023-03-11 16:43:11.000000 parse_stages-0.1.2/requirements/install.txt
--rw-r--r--   0 roam      (1000) roam      (1000)      118 2023-03-11 16:43:11.000000 parse_stages-0.1.2/requirements/test.txt
--rw-r--r--   0 roam      (1000) roam      (1000)      153 2023-03-11 19:50:45.480252 parse_stages-0.1.2/setup.cfg
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-11 19:50:45.476252 parse_stages-0.1.2/src/
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-11 19:50:45.480252 parse_stages-0.1.2/src/parse_stages/
--rw-r--r--   0 roam      (1000) roam      (1000)     4238 2023-03-11 17:36:28.000000 parse_stages-0.1.2/src/parse_stages/__init__.py
--rw-r--r--   0 roam      (1000) roam      (1000)     1340 2023-03-11 19:26:40.000000 parse_stages-0.1.2/src/parse_stages/defs.py
--rw-r--r--   0 roam      (1000) roam      (1000)     2677 2023-03-11 19:14:02.000000 parse_stages-0.1.2/src/parse_stages/expr.py
--rw-r--r--   0 roam      (1000) roam      (1000)     4552 2023-03-11 19:34:01.000000 parse_stages-0.1.2/src/parse_stages/p_pyp.py
--rw-r--r--   0 roam      (1000) roam      (1000)        0 2022-11-14 18:08:51.000000 parse_stages-0.1.2/src/parse_stages/py.typed
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-11 19:50:45.480252 parse_stages-0.1.2/src/parse_stages.egg-info/
--rw-r--r--   0 roam      (1000) roam      (1000)     4809 2023-03-11 19:50:45.000000 parse_stages-0.1.2/src/parse_stages.egg-info/PKG-INFO
--rw-r--r--   0 roam      (1000) roam      (1000)      814 2023-03-11 19:50:45.000000 parse_stages-0.1.2/src/parse_stages.egg-info/SOURCES.txt
--rw-r--r--   0 roam      (1000) roam      (1000)        1 2023-03-11 19:50:45.000000 parse_stages-0.1.2/src/parse_stages.egg-info/dependency_links.txt
--rw-r--r--   0 roam      (1000) roam      (1000)       16 2023-03-11 19:50:45.000000 parse_stages-0.1.2/src/parse_stages.egg-info/requires.txt
--rw-r--r--   0 roam      (1000) roam      (1000)       13 2023-03-11 19:50:45.000000 parse_stages-0.1.2/src/parse_stages.egg-info/top_level.txt
--rw-r--r--   0 roam      (1000) roam      (1000)        1 2023-03-11 19:50:45.000000 parse_stages-0.1.2/src/parse_stages.egg-info/zip-safe
--rw-r--r--   0 roam      (1000) roam      (1000)     2918 2023-03-11 18:46:57.000000 parse_stages-0.1.2/tox.ini
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-03-11 19:50:45.480252 parse_stages-0.1.2/unit_tests/
--rw-r--r--   0 roam      (1000) roam      (1000)      152 2023-03-11 16:43:11.000000 parse_stages-0.1.2/unit_tests/__init__.py
--rw-r--r--   0 roam      (1000) roam      (1000)     1876 2023-03-11 16:43:11.000000 parse_stages-0.1.2/unit_tests/test_eval.py
--rw-r--r--   0 roam      (1000) roam      (1000)     2381 2023-03-11 16:43:11.000000 parse_stages-0.1.2/unit_tests/test_parse.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 parse_stages-0.1.3/.editorconfig
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 parse_stages-0.1.3/mkdocs.yml
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 parse_stages-0.1.3/setup.cfg
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 parse_stages-0.1.3/tox.ini
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 parse_stages-0.1.3/LICENSES/BSD-2-Clause.txt
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 parse_stages-0.1.3/config/ruff-all/pyproject.toml
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 parse_stages-0.1.3/config/ruff-base/pyproject.toml
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 parse_stages-0.1.3/config/ruff-most/pyproject.toml
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 parse_stages-0.1.3/docs/api.md
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 parse_stages-0.1.3/docs/changes.md
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 parse_stages-0.1.3/docs/index.md
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 parse_stages-0.1.3/docs/language.md
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 parse_stages-0.1.3/nix/mkdocs.nix
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 parse_stages-0.1.3/nix/python-pytest.nix
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 parse_stages-0.1.3/nix/reformat.sh
+-rwxr-xr-x   0        0        0      735 2020-02-02 00:00:00.000000 parse_stages-0.1.3/nix/run-pytest.sh
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 parse_stages-0.1.3/requirements/install.txt
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 parse_stages-0.1.3/requirements/test.txt
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 parse_stages-0.1.3/src/parse_stages/__init__.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 parse_stages-0.1.3/src/parse_stages/defs.py
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 parse_stages-0.1.3/src/parse_stages/expr.py
+-rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 parse_stages-0.1.3/src/parse_stages/p_pyp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parse_stages-0.1.3/src/parse_stages/py.typed
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 parse_stages-0.1.3/unit_tests/__init__.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 parse_stages-0.1.3/unit_tests/test_eval.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 parse_stages-0.1.3/unit_tests/test_parse.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 parse_stages-0.1.3/.gitignore
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 parse_stages-0.1.3/README.md
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 parse_stages-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 parse_stages-0.1.3/PKG-INFO
```

### Comparing `parse_stages-0.1.2/.editorconfig` & `parse_stages-0.1.3/.editorconfig`

 * *Files identical despite different names*

### Comparing `parse_stages-0.1.2/LICENSES/BSD-2-Clause.txt` & `parse_stages-0.1.3/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `parse_stages-0.1.2/PKG-INFO` & `parse_stages-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: parse_stages
-Version: 0.1.2
+Version: 0.1.3
 Summary: Parse an expression for selecting stages and tags
-Author-email: Peter Pentchev <roam@ringlet.net>
 Project-URL: Homepage, https://devel.ringlet.net/devel/parse-stages/
 Project-URL: Changes, https://devel.ringlet.net/devel/parse-stages/changes/
 Project-URL: Issue Tracker, https://gitlab.com/ppentchev/parse-stages/-/issues
 Project-URL: Source Code, https://gitlab.com/ppentchev/parse-stages
+Author-email: Peter Pentchev <roam@ringlet.net>
 Requires-Python: >=3.8
+Requires-Dist: pyparsing<4,>=3
 Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
 SPDX-License-Identifier: BSD-2-Clause
 -->
 
 # Parse a mini-language for selecting objects by tag or name
 
+\[[Home][ringlet-parse-stages] | [GitLab][gitlab] | [PyPI][pypi]\]
+
 This library is mostly useful for command-line parsing by other tools like
 `tox-stages` and `nox-stages`. It may be used to parse e.g. a command-line
 specification like `@check and not pylint` or `@tests or ruff` and then
 match it against a list of objects that have names and lists of tags.
 
 ## Parse stage specifications
 
@@ -117,8 +120,9 @@
 
 The `parse-stages` library was written by [Peter Pentchev][roam].
 It is developed in [a GitLab repository][gitlab]. This documentation is
 hosted at [Ringlet][ringlet-parse-stages].
 
 [roam]: mailto:roam@ringlet.net "Peter Pentchev"
 [gitlab]: https://gitlab.com/ppentchev/parse-stages "The parse-stages GitLab repository"
+[pypi]: https://pypi.org/project/parse-stages/ "The parse-stages Python Package Index page"
 [ringlet-parse-stages]: https://devel.ringlet.net/devel/parse-stages/ "The Ringlet parse-stages homepage"
```

### Comparing `parse_stages-0.1.2/README.md` & `parse_stages-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 <!--
 SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
 SPDX-License-Identifier: BSD-2-Clause
 -->
 
 # Parse a mini-language for selecting objects by tag or name
 
+\[[Home][ringlet-parse-stages] | [GitLab][gitlab] | [PyPI][pypi]\]
+
 This library is mostly useful for command-line parsing by other tools like
 `tox-stages` and `nox-stages`. It may be used to parse e.g. a command-line
 specification like `@check and not pylint` or `@tests or ruff` and then
 match it against a list of objects that have names and lists of tags.
 
 ## Parse stage specifications
 
@@ -105,8 +107,9 @@
 
 The `parse-stages` library was written by [Peter Pentchev][roam].
 It is developed in [a GitLab repository][gitlab]. This documentation is
 hosted at [Ringlet][ringlet-parse-stages].
 
 [roam]: mailto:roam@ringlet.net "Peter Pentchev"
 [gitlab]: https://gitlab.com/ppentchev/parse-stages "The parse-stages GitLab repository"
+[pypi]: https://pypi.org/project/parse-stages/ "The parse-stages Python Package Index page"
 [ringlet-parse-stages]: https://devel.ringlet.net/devel/parse-stages/ "The Ringlet parse-stages homepage"
```

### Comparing `parse_stages-0.1.2/config/ruff-base/pyproject.toml` & `parse_stages-0.1.3/config/ruff-base/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -11,22 +11,16 @@
 
   # No blank lines before the class docstring, TYVM
   "D203",
 
   # The multi-line docstring summary starts on the same line
   "D213",
 
-  # Our exceptions are simple enough
-  "EM",
-
-  # ruff does not seem to like the empty line before "from typing import ..."
-  "I",
-
   # The Tagged and TaggedFrozen classes need to be typedload-compatible
   "TCH",
-
-  # We are fine with relative imports
-  "TID",
-
-  # Much too restrictive
-  "TRY",
 ]
+
+[tool.ruff.isort]
+force-single-line = true
+known-first-party = ["parse_stages"]
+lines-after-imports = 2
+single-line-exclusions = ["typing"]
```

### Comparing `parse_stages-0.1.2/config/ruff-most/pyproject.toml` & `parse_stages-0.1.3/config/ruff-most/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
 # SPDX-License-Identifier: BSD-2-Clause
 
 [tool.ruff]
 extend = "../ruff-base/pyproject.toml"
-# These are all the Ruff 0.0.254 linters.
+# These are all the Ruff 0.0.265 linters.
 select = [
   "A",
   "ANN",
   "ARG",
   "B",
   "BLE",
   "C4",
   "C90",
   "COM",
   "D",
   "DJ",
   "DTZ",
   "E",
-  # "EM",
+  "EM",
   "ERA",
   "EXE",
   "F",
   "FBT",
   "G",
-  # "I",
+  "I",
   "ICN",
   "INP",
+  "INT",
   "ISC",
   "N",
   "NPY",
   "PD",
   "PGH",
   "PIE",
   "PL",
@@ -41,14 +42,14 @@
   "RSE",
   "RUF",
   "S",
   "SIM",
   "SLF",
   "T10",
   "T20",
-  # "TCH",
-  # "TID",
-  # "TRY",
+  "TCH",
+  "TID",
+  "TRY",
   "UP",
   "W",
   "YTT",
 ]
```

### Comparing `parse_stages-0.1.2/docs/changes.md` & `parse_stages-0.1.3/docs/changes.md`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,58 @@
 All notable changes to the parse-stages project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.3] - 2023-05-07
+
+### Fixes
+
+- Add a blank line to a docstring section (ruff D214).
+- Drop the text in a `NotImplementedError` raised in an abstract method;
+  it should be obvious (ruff EM101)
+
+### Additions
+
+- Add a `.gitignore` file, mostly so that `reuse` can be run at any time
+- Add a "Home, GitLab, PyPI" navigational line to the documentation
+  index page and to the `README.md` file
+
+### Other changes
+
+- Main source:
+    - reformat the import sections using Ruff's `isort` implementation
+- Build system:
+    - switch to `hatch` / `hatchling` for the PEP517 build
+- Documentation:
+    - use the `default_handler` configuration option of `mkdocstrings`
+      instead of specifying `handler: python` for each class!
+    - bump the versions of `mkdocstrings` and `mkdocstrings-python` with
+      no changes
+- Test suite:
+    - specify 4.1 as the Tox minimum version and switch to the Tox 4.x
+      format for the multiline list of files
+    - rename the `black` Tox environment to `format` and
+      the `black-reformat` one to `reformat`, since they also run
+      Ruff's `isort` now
+    - Ruff:
+        - use Ruff 0.0.265, enable the `INT` checks area although
+          we do not use gettext
+        - enable all ruff check areas in `config/ruff-most/`, let
+          the `config/ruff-base/` files take care of the ignored ones
+        - no longer disable the "relative imports" check, it does not
+          complain about our source code
+    - Pylint:
+        - reenable the "empty comment" plugin; we should have no
+          trouble with it since switching to SPDX license tags
+    - Bump the versions of `flake8-implicit-str-concat`, `flake8-simplify`,
+      `pylint`, and `triceratops` with no code changes
+
 ## [0.1.2] - 2023-03-10
 
 ### Semi-incompatible changes
 
 - Drop Python 3.7 support.
 
 ### Fixes
@@ -72,11 +116,12 @@
 
 ## [0.1.0] - 2023-01-25
 
 ### Started
 
 - First public release.
 
-[Unreleased]: https://gitlab.com/ppentchev/parse-stages/-/compare/release%2F0.1.2...main
+[Unreleased]: https://gitlab.com/ppentchev/parse-stages/-/compare/release%2F0.1.3...main
+[0.1.3]: https://gitlab.com/ppentchev/parse-stages/-/compare/release%2F0.1.2...release%2F0.1.3
 [0.1.2]: https://gitlab.com/ppentchev/parse-stages/-/compare/release%2F0.1.1...release%2F0.1.2
 [0.1.1]: https://gitlab.com/ppentchev/parse-stages/-/compare/release%2F0.1.0...release%2F0.1.1
 [0.1.0]: https://gitlab.com/ppentchev/parse-stages/-/tags/release%2F0.1.0
```

### Comparing `parse_stages-0.1.2/docs/index.md` & `parse_stages-0.1.3/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 <!--
 SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
 SPDX-License-Identifier: BSD-2-Clause
 -->
 
 # Parse a mini-language for selecting objects by tag or name
 
+\[[Home][ringlet-parse-stages] | [GitLab][gitlab] | [PyPI][pypi]\]
+
 ## Overview
 
 The `parse-stages` Python library may be used by other tools to group
 objects (e.g. [Tox] or [Nox] test environments) for step-by-step processing
 (e.g. running some tests in parallel, then only running others if the first
 group passes).
 
@@ -20,15 +22,15 @@
 [nox]: https://nox.thea.codes/en/stable/ "The nox flexible automation tool"
 
 ## Installation
 
 A program that uses the `parse-stages` library should specify it in
 its list of requirements, e.g. using [PEP508][pep508] syntax:
 
-    parse-stages >= 0.1.2, < 0.2
+    parse-stages >= 0.1.3, < 0.2
 
 [pep508]: https://peps.python.org/pep-0508/ "PEP 508 – Dependency specification for Python Software Packages"
 
 ## Parsing a stage specification
 
 The `parse_spec()` function parses a string specification into
 a [BoolExpr][parse_stages.BoolExpr] object that may later be used to
@@ -98,8 +100,9 @@
 
 The `parse-stages` library was written by [Peter Pentchev][roam].
 It is developed in [a GitLab repository][gitlab]. This documentation is
 hosted at [Ringlet][ringlet-parse-stages].
 
 [roam]: mailto:roam@ringlet.net "Peter Pentchev"
 [gitlab]: https://gitlab.com/ppentchev/parse-stages "The parse-stages GitLab repository"
+[pypi]: https://pypi.org/project/parse-stages/ "The parse-stages Python Package Index page"
 [ringlet-parse-stages]: https://devel.ringlet.net/devel/parse-stages/ "The Ringlet parse-stages homepage"
```

### Comparing `parse_stages-0.1.2/docs/language.md` & `parse_stages-0.1.3/docs/language.md`

 * *Files identical despite different names*

### Comparing `parse_stages-0.1.2/mkdocs.yml` & `parse_stages-0.1.3/mkdocs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -35,14 +35,15 @@
   - toc:
   - pymdownx.highlight:
       anchor_linenums: true
   - pymdownx.inlinehilite:
   - pymdownx.superfences:
 plugins:
   - mkdocstrings:
+      default_handler: python
       handlers:
         python:
           paths: [src]
           options:
             heading_level: 3
             show_root_heading: true
   - search
```

### Comparing `parse_stages-0.1.2/nix/mkdocs.nix` & `parse_stages-0.1.3/nix/mkdocs.nix`

 * *Files identical despite different names*

### Comparing `parse_stages-0.1.2/nix/run-pytest.sh` & `parse_stages-0.1.3/nix/run-pytest.sh`

 * *Files identical despite different names*

### Comparing `parse_stages-0.1.2/pyproject.toml` & `parse_stages-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
 # SPDX-License-Identifier: BSD-2-Clause
 
 [build-system]
-requires = ["setuptools >= 61", "wheel"]
-build-backend = "setuptools.build_meta"
+requires = [
+  "hatchling",
+  "hatch-requirements-txt >= 0.4, < 0.5",
+]
+build-backend = "hatchling.build"
 
 [project]
 name = "parse_stages"
 description = "Parse an expression for selecting stages and tags"
 readme = "README.md"
 requires-python = ">= 3.8"
 dynamic = ["dependencies", "version"]
@@ -18,26 +21,29 @@
 
 [project.urls]
 Homepage = "https://devel.ringlet.net/devel/parse-stages/"
 Changes = "https://devel.ringlet.net/devel/parse-stages/changes/"
 "Issue Tracker" = "https://gitlab.com/ppentchev/parse-stages/-/issues"
 "Source Code" = "https://gitlab.com/ppentchev/parse-stages"
 
+[tool.hatch.build.targets.wheel]
+packages = ["src/parse_stages"]
+
+[tool.hatch.metadata.hooks.requirements_txt]
+files = ["requirements/install.txt"]
+
+[tool.hatch.version]
+path = "src/parse_stages/defs.py"
+
 [tool.setuptools]
 zip-safe = true
-package-dir = {"" = "src"}
-packages = ["parse_stages"]
 
 [tool.setuptools.package-data]
 parse_stages = ["py.typed"]
 
-[tool.setuptools.dynamic]
-dependencies = {file = "requirements/install.txt"}
-version = {attr = "parse_stages.defs.VERSION"}
-
 [tool.black]
 target-version = ["py38", "py39", "py310", "py311"]
 line-length = 100
 
 [tool.mypy]
 strict = true
 python_version = "3.8"
@@ -55,15 +61,15 @@
   "pylint.extensions.confusing_elif",
   "pylint.extensions.consider_refactoring_into_while_condition",
   "pylint.extensions.consider_ternary_expression",
   "pylint.extensions.dict_init_mutate",
   "pylint.extensions.docparams",
   "pylint.extensions.docstyle",
   "pylint.extensions.dunder",
-  # "pylint.extensions.empty_comment",  # the copyright notices trigger that one
+  "pylint.extensions.empty_comment",
   "pylint.extensions.emptystring",
   "pylint.extensions.eq_without_hash",
   "pylint.extensions.for_any_all",
   "pylint.extensions.magic_value",
   "pylint.extensions.mccabe",
   "pylint.extensions.no_self_use",
   "pylint.extensions.overlapping_exceptions",
```

### Comparing `parse_stages-0.1.2/src/parse_stages/__init__.py` & `parse_stages-0.1.3/src/parse_stages/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,27 +91,28 @@
     all_envs = [TestEnv(name, env["tags"], ...) for name, env in tox_envs.items()]
 
     # Select the ones that match the "@check" expression
     matched = [env for env in all_envs if e_check.evaluate(env)]
 
     # Or if we only care about the names...
     quick_names = [env.name for env in all_envs if e_check_quick.evaluate(env)]
+
 """
 
-from .defs import Tagged, TaggedFrozen, VERSION
-from .expr import BoolExpr, OrExpr, AndExpr, NotExpr, TagExpr, KeywordExpr
-from .p_pyp import parse_spec, parse_stage_ids
+from .defs import VERSION, Tagged, TaggedFrozen  # isort: skip
+from .expr import AndExpr, BoolExpr, KeywordExpr, NotExpr, OrExpr, TagExpr  # isort: skip
+from .p_pyp import parse_spec, parse_stage_ids  # isort: skip
 
 
 __all__ = [
+    "VERSION",
     "Tagged",
     "TaggedFrozen",
-    "BoolExpr",
-    "OrExpr",
     "AndExpr",
+    "BoolExpr",
+    "KeywordExpr",
     "NotExpr",
+    "OrExpr",
     "TagExpr",
-    "KeywordExpr",
     "parse_spec",
     "parse_stage_ids",
-    "VERSION",
 ]
```

### Comparing `parse_stages-0.1.2/src/parse_stages/defs.py` & `parse_stages-0.1.3/src/parse_stages/defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """Common definitions for the parse-stages library."""
 
 # Some of this library's consumers need to be able to use typedload on
 # Python versions < 3.9, so we cannot use the generic types.
 # pylint: disable=deprecated-typing-alias
 
 import dataclasses
-
 from typing import List
 
 
 @dataclasses.dataclass(frozen=True)
 class TaggedFrozen:
     """A base class for representing a constant object that has some tags."""
 
@@ -43,8 +42,8 @@
         """Get the strings to look for keywords in.
 
         Default: the object's `name` attribute.
         """
         return [self.name]
 
 
-VERSION = "0.1.2"
+VERSION = "0.1.3"
```

### Comparing `parse_stages-0.1.2/src/parse_stages/expr.py` & `parse_stages-0.1.3/src/parse_stages/expr.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 @dataclasses.dataclass(frozen=True)
 class BoolExpr(metaclass=abc.ABCMeta):
     """A boolean expression parsed out of a specification string."""
 
     @abc.abstractmethod
     def evaluate(self, obj: defs.TaggedFrozen | defs.Tagged) -> bool:
         """Evaluate the expression for the specified object."""
-        raise NotImplementedError(f"{type(self).__name__}.evaluate() must be overridden")
+        raise NotImplementedError
 
 
 @dataclasses.dataclass(frozen=True)
 class TagExpr(BoolExpr):
     """A tag to be checked against obj.tags."""
 
     tag: str
```

### Comparing `parse_stages-0.1.2/src/parse_stages/p_pyp.py` & `parse_stages-0.1.3/src/parse_stages/p_pyp.py`

 * *Files identical despite different names*

### Comparing `parse_stages-0.1.2/tox.ini` & `parse_stages-0.1.3/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,68 @@
 # SPDX-FileCopyrightText: Peter Pentchev <roam@ringlet.net>
 # SPDX-License-Identifier: BSD-2-Clause
 
 [tox]
+minversion = 4.1
 envlist =
   ruff
   ruff-all
-  black
+  format
   pep8
   mypy
   pylint
   pydocstyle
   pyupgrade
   unit-tests
 isolated_build = True
 
 [defs]
 pyfiles =
-  src/parse_stages
+  src/parse_stages \
   unit_tests
 
 [testenv:ruff]
 skip_install = True
 tags =
   check
 deps =
-  ruff >= 0.0.254, < 0.1
+  ruff >= 0.0.265, < 0.1
 commands =
   ruff check --config config/ruff-most/pyproject.toml -- {[defs]pyfiles}
 
 [testenv:ruff-all]
 skip_install = True
 tags =
   check
 deps =
-  ruff == 0.0.254
+  ruff == 0.0.265
 commands =
   ruff check --config config/ruff-all/pyproject.toml -- {[defs]pyfiles}
 
-[testenv:black]
+[testenv:format]
 skip_install = True
 tags =
   check
 deps =
   black >= 23, < 24
+  ruff >= 0.0.265, < 0.1
 commands =
+  ruff check --config config/ruff-base/pyproject.toml --select=I --diff -- {[defs]pyfiles}
   black --check {[defs]pyfiles}
 
-[testenv:black-reformat]
+[testenv:reformat]
 skip_install = True
 tags =
   format
   manual
 deps =
   black >= 23, < 24
+  ruff >= 0.0.265, < 0.1
 commands =
+  ruff check --config config/ruff-base/pyproject.toml --select=I --fix -- {[defs]pyfiles}
   black {[defs]pyfiles}
 
 # Add flake8-import-conventions if it ever hits PyPI
 [testenv:pep8]
 skip_install = True
 tags =
   check
@@ -69,27 +74,27 @@
   flake8-bugbear >= 23, < 24
   flake8-builtins >= 2, < 3
   flake8-commas >= 2, < 3
   flake8-comprehensions >= 3, < 4
   flake8-datetimez >= 20, < 21
   flake8-debugger >= 4, < 5
   flake8-executable >= 2, < 3
-  flake8-implicit-str-concat >= 0.3, < 0.4
+  flake8-implicit-str-concat >= 0.4, < 0.5
   flake8-no-pep420 >= 2, < 3
   flake8-pie >= 0.16, < 0.17
   flake8-print >= 5, < 6
   flake8-pytest-style >= 1, < 2
   flake8-quotes >= 3, < 4
   flake8-return >= 1, < 2
-  flake8-simplify >= 0.19, < 0.20
+  flake8-simplify >= 0.20, < 0.21
   flake8-use-pathlib >= 0.3, < 0.4
   mccabe >= 0.7, < 0.8
   pep8-naming >= 0.13, < 0.14
   pycodestyle >= 2.10, < 3
-  tryceratops >= 1, < 2
+  tryceratops >= 2, < 3
 commands =
   flake8 {[defs]pyfiles}
   pycodestyle {[defs]pyfiles}
 
 [testenv:mypy]
 skip_install = True
 tags =
@@ -106,15 +111,15 @@
 [testenv:pylint]
 skip_install = True
 tags =
   check
 deps =
   -r requirements/install.txt
   -r requirements/test.txt
-  pylint >= 2.16, < 2.17
+  pylint >= 2.17, < 2.18
 commands =
   pylint {[defs]pyfiles}
 
 [testenv:pydocstyle]
 skip_install = True
 tags =
   check
@@ -148,16 +153,16 @@
 skip_install = True
 tags =
   docs
   manual
 deps =
   mkdocs >= 1.4.2, < 2
   mkdocs-material >= 9.1.2, < 10
-  mkdocstrings >= 0.20, < 0.21
-  mkdocstrings-python >= 0.8.3, < 0.9
+  mkdocstrings >= 0.21.2, < 0.22
+  mkdocstrings-python >= 0.10, < 0.11
 commands =
   mkdocs build
 
 [testenv:reuse]
 skip_install = True
 tags =
   check
```

### Comparing `parse_stages-0.1.2/unit_tests/test_eval.py` & `parse_stages-0.1.3/unit_tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `parse_stages-0.1.2/unit_tests/test_parse.py` & `parse_stages-0.1.3/unit_tests/test_parse.py`

 * *Files identical despite different names*

