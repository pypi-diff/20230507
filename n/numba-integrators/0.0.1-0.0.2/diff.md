# Comparing `tmp/numba-integrators-0.0.1.tar.gz` & `tmp/numba-integrators-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numba-integrators-0.0.1.tar", last modified: Sat May  6 20:50:39 2023, max compression
+gzip compressed data, was "numba-integrators-0.0.2.tar", last modified: Sun May  7 20:40:24 2023, max compression
```

## Comparing `numba-integrators-0.0.1.tar` & `numba-integrators-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 20:50:39.772031 numba-integrators-0.0.1/
--rw-rw-rw-   0        0        0     1085 2023-05-06 18:14:27.000000 numba-integrators-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1372 2023-05-06 20:50:39.772031 numba-integrators-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-05-06 20:50:34.000000 numba-integrators-0.0.1/README.md
--rw-rw-rw-   0        0        0       33 2023-05-06 20:13:25.000000 numba-integrators-0.0.1/dependencies.txt
--rw-rw-rw-   0        0        0      311 2023-05-06 20:26:37.000000 numba-integrators-0.0.1/dependencies_dev.txt
--rw-rw-rw-   0        0        0     1262 2023-05-06 20:50:34.000000 numba-integrators-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 20:50:39.773029 numba-integrators-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-06 20:50:39.753031 numba-integrators-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 20:50:39.763028 numba-integrators-0.0.1/src/numba_integrators/
--rw-rw-rw-   0        0        0       40 2023-05-06 20:13:29.000000 numba-integrators-0.0.1/src/numba_integrators/_API.py
--rw-rw-rw-   0        0        0       66 2023-05-06 20:19:46.000000 numba-integrators-0.0.1/src/numba_integrators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 20:50:39.770032 numba-integrators-0.0.1/src/numba_integrators.egg-info/
--rw-rw-rw-   0        0        0     1372 2023-05-06 20:50:39.000000 numba-integrators-0.0.1/src/numba_integrators.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-05-06 20:50:39.000000 numba-integrators-0.0.1/src/numba_integrators.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 20:50:39.000000 numba-integrators-0.0.1/src/numba_integrators.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      296 2023-05-06 20:50:39.000000 numba-integrators-0.0.1/src/numba_integrators.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-06 20:50:39.000000 numba-integrators-0.0.1/src/numba_integrators.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:40:24.652508 numba-integrators-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-07 20:39:49.000000 numba-integrators-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-07 20:40:24.652508 numba-integrators-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-07 20:40:21.000000 numba-integrators-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 20:39:49.000000 numba-integrators-0.0.2/dependencies.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-07 20:39:49.000000 numba-integrators-0.0.2/dependencies_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-07 20:40:21.000000 numba-integrators-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 20:40:24.652508 numba-integrators-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:40:24.648508 numba-integrators-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:40:24.652508 numba-integrators-0.0.2/src/numba_integrators/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-07 20:39:49.000000 numba-integrators-0.0.2/src/numba_integrators/_API.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-07 20:39:49.000000 numba-integrators-0.0.2/src/numba_integrators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:40:24.652508 numba-integrators-0.0.2/src/numba_integrators.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-07 20:40:24.000000 numba-integrators-0.0.2/src/numba_integrators.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-07 20:40:24.000000 numba-integrators-0.0.2/src/numba_integrators.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:40:24.000000 numba-integrators-0.0.2/src/numba_integrators.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-07 20:40:24.000000 numba-integrators-0.0.2/src/numba_integrators.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 20:40:24.000000 numba-integrators-0.0.2/src/numba_integrators.egg-info/top_level.txt
```

### Comparing `numba-integrators-0.0.1/LICENSE` & `numba-integrators-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Limespy
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Limespy
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `numba-integrators-0.0.1/PKG-INFO` & `numba-integrators-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,40 @@
-Metadata-Version: 2.1
-Name: numba-integrators
-Version: 0.0.1
-Summary: Numerical integrators using Numba
-Author: Limespy
-License: MIT License
-Project-URL: Homepage, https://github.com/Limespy/numba-integrators
-Project-URL: Changelog, https://github.com/Limespy/numba-integrators/blob/main/README.md#Changelog
-Project-URL: Issue Tracker, https://github.com/Limespy/numba-integrators/issues
-Classifier: Development Status :: 1 - Planning
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# Numba Integrators
-
-[![PyPI Package latest release](https://img.shields.io/pypi/v/numba-integrators.svg)][1]
-[![PyPI Wheel](https://img.shields.io/pypi/wheel/numba-integrators.svg)][1]
-[![Supported versions](https://img.shields.io/pypi/pyversions/numba-integrators.svg)][1]
-[![Supported implementations](https://img.shields.io/pypi/implementation/numba-integrators.svg)][1]
-
-Numerical integrators using Numba
-
-[1]: <https://pypi.org/project/numba-integrators> ""
+Metadata-Version: 2.1
+Name: numba-integrators
+Version: 0.0.2
+Summary: Numerical integrators using Numba
+Author: Limespy
+Project-URL: Homepage, https://github.com/Limespy/numba-integrators
+Project-URL: Changelog, https://github.com/Limespy/numba-integrators/blob/main/README.md#Changelog
+Project-URL: Issue Tracker, https://github.com/Limespy/numba-integrators/issues
+Classifier: Development Status :: 1 - Planning
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Unix
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# Overview of Numba integrators
+
+[https://pypi.org/project/numba-integrators][1]
+[https://pypi.org/project/numba-integrators][2]
+[https://pypi.org/project/numba-integrators][3]
+[https://pypi.org/project/numba-integrators][4]
+
+Numerical integrators using Numba
+
+# Changelog <!-- omit in toc -->
+
+## 0.0.2 2023-05-07 <!-- omit in toc -->
+
+- Setup
+
+[1]: <![PyPI Package latest release](https://img.shields.io/pypi/v/numba-integrators.svg)> ""
+[2]: <![PyPI Wheel](https://img.shields.io/pypi/wheel/numba-integrators.svg)> ""
+[3]: <![Supported versions](https://img.shields.io/pypi/pyversions/numba-integrators.svg)> ""
+[4]: <![Supported implementations](https://img.shields.io/pypi/implementation/numba-integrators.svg)> ""
```

### Comparing `numba-integrators-0.0.1/pyproject.toml` & `numba-integrators-0.0.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,47 @@
-[build-system]
-requires = [
-    "setuptools>=64.0",
-]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "numba-integrators"
-description = "Numerical integrators using Numba"
-classifiers = [
-    "Development Status :: 1 - Planning",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: Unix",
-    "Operating System :: POSIX",
-    "Operating System :: Microsoft :: Windows",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.10",
-]
-requires-python = ">=3.10"
-readme = "README.md"
-dynamic = [
-    "dependencies",
-    "optional-dependencies",
-    "version",
-]
-authors = [
-    { name = "Limespy" },
-]
-
-[project.license]
-text = "MIT License"
-
-[project.urls]
-Homepage = "https://github.com/Limespy/numba-integrators"
-Changelog = "https://github.com/Limespy/numba-integrators/blob/main/README.md#Changelog"
-"Issue Tracker" = "https://github.com/Limespy/numba-integrators/issues"
-
-[tool.setuptools.dynamic.dependencies]
-file = [
-    "dependencies.txt",
-]
-
-[tool.setuptools.dynamic.optional-dependencies.dev]
-file = "dependencies_dev.txt"
-
-[tool.setuptools.dynamic.version]
-attr = "numba_integrators.__version__"
+[master-info]
+organisation = "https://github.com/Limespy"
+package_name = "numba-integrators"
+description = "Numerical integrators using Numba"
+
+[build-system]
+requires = [
+    "setuptools>=64.0",
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "numba-integrators"
+description = "Numerical integrators using Numba"
+classifiers = [
+    "Development Status :: 1 - Planning",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: Unix",
+    "Operating System :: POSIX",
+    "Operating System :: Microsoft :: Windows",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.10",
+]
+authors = [
+    { name = "Limespy" },
+]
+requires-python = ">=3.10"
+readme = "README.md"
+version = "0.0.2"
+dynamic = [
+    "dependencies",
+    "optional-dependencies",
+]
+
+[project.urls]
+Homepage = "https://github.com/Limespy/numba-integrators"
+Changelog = "https://github.com/Limespy/numba-integrators/blob/main/README.md#Changelog"
+"Issue Tracker" = "https://github.com/Limespy/numba-integrators/issues"
+
+[tool.setuptools.dynamic.dependencies]
+file = [
+    "dependencies.txt",
+]
+
+[tool.setuptools.dynamic.optional-dependencies.dev]
+file = "dependencies_dev.txt"
```

### Comparing `numba-integrators-0.0.1/src/numba_integrators.egg-info/PKG-INFO` & `numba-integrators-0.0.2/src/numba_integrators.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,40 @@
-Metadata-Version: 2.1
-Name: numba-integrators
-Version: 0.0.1
-Summary: Numerical integrators using Numba
-Author: Limespy
-License: MIT License
-Project-URL: Homepage, https://github.com/Limespy/numba-integrators
-Project-URL: Changelog, https://github.com/Limespy/numba-integrators/blob/main/README.md#Changelog
-Project-URL: Issue Tracker, https://github.com/Limespy/numba-integrators/issues
-Classifier: Development Status :: 1 - Planning
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# Numba Integrators
-
-[![PyPI Package latest release](https://img.shields.io/pypi/v/numba-integrators.svg)][1]
-[![PyPI Wheel](https://img.shields.io/pypi/wheel/numba-integrators.svg)][1]
-[![Supported versions](https://img.shields.io/pypi/pyversions/numba-integrators.svg)][1]
-[![Supported implementations](https://img.shields.io/pypi/implementation/numba-integrators.svg)][1]
-
-Numerical integrators using Numba
-
-[1]: <https://pypi.org/project/numba-integrators> ""
+Metadata-Version: 2.1
+Name: numba-integrators
+Version: 0.0.2
+Summary: Numerical integrators using Numba
+Author: Limespy
+Project-URL: Homepage, https://github.com/Limespy/numba-integrators
+Project-URL: Changelog, https://github.com/Limespy/numba-integrators/blob/main/README.md#Changelog
+Project-URL: Issue Tracker, https://github.com/Limespy/numba-integrators/issues
+Classifier: Development Status :: 1 - Planning
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Unix
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# Overview of Numba integrators
+
+[https://pypi.org/project/numba-integrators][1]
+[https://pypi.org/project/numba-integrators][2]
+[https://pypi.org/project/numba-integrators][3]
+[https://pypi.org/project/numba-integrators][4]
+
+Numerical integrators using Numba
+
+# Changelog <!-- omit in toc -->
+
+## 0.0.2 2023-05-07 <!-- omit in toc -->
+
+- Setup
+
+[1]: <![PyPI Package latest release](https://img.shields.io/pypi/v/numba-integrators.svg)> ""
+[2]: <![PyPI Wheel](https://img.shields.io/pypi/wheel/numba-integrators.svg)> ""
+[3]: <![Supported versions](https://img.shields.io/pypi/pyversions/numba-integrators.svg)> ""
+[4]: <![Supported implementations](https://img.shields.io/pypi/implementation/numba-integrators.svg)> ""
```

