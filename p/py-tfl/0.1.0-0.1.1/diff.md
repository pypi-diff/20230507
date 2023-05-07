# Comparing `tmp/py_tfl-0.1.0.tar.gz` & `tmp/py_tfl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_tfl-0.1.0.tar", max compression
+gzip compressed data, was "py_tfl-0.1.1.tar", max compression
```

## Comparing `py_tfl-0.1.0.tar` & `py_tfl-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1068 2023-05-07 13:05:34.905241 py_tfl-0.1.0/LICENSE
--rw-r--r--   0        0        0     3536 2023-05-07 13:05:34.905241 py_tfl-0.1.0/README.md
--rw-r--r--   0        0        0     2291 2023-05-07 13:05:34.905241 py_tfl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      121 2023-05-07 13:05:34.905241 py_tfl-0.1.0/tfl/__init__.py
--rw-r--r--   0        0        0       68 2023-05-07 13:05:34.905241 py_tfl-0.1.0/tfl/cli/__init__.py
--rw-r--r--   0        0        0     1345 2023-05-07 13:05:34.905241 py_tfl-0.1.0/tfl/cli/_async_typer.py
--rw-r--r--   0        0        0     1105 2023-05-07 13:05:34.905241 py_tfl-0.1.0/tfl/cli/main.py
--rw-r--r--   0        0        0        0 2023-05-07 13:05:34.905241 py_tfl-0.1.0/tfl/cli/py.typed
--rw-r--r--   0        0        0      231 2023-05-07 13:05:34.905241 py_tfl-0.1.0/tfl/clients/__init__.py
--rw-r--r--   0        0        0     1696 2023-05-07 13:05:34.905241 py_tfl-0.1.0/tfl/clients/_auth.py
--rw-r--r--   0        0        0     5000 2023-05-07 13:05:34.905241 py_tfl-0.1.0/tfl/clients/_client.py
--rw-r--r--   0        0        0     4463 2023-05-07 13:05:34.905241 py_tfl-0.1.0/tfl/clients/_lift_disruptions_client.py
--rw-r--r--   0        0        0        0 2023-05-07 13:05:34.905241 py_tfl-0.1.0/tfl/clients/py.typed
--rw-r--r--   0        0        0        0 2023-05-07 13:05:34.905241 py_tfl-0.1.0/tfl/py.typed
--rw-r--r--   0        0        0     4710 1970-01-01 00:00:00.000000 py_tfl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-07 14:39:49.887967 py_tfl-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4118 2023-05-07 14:39:49.887967 py_tfl-0.1.1/README.md
+-rw-r--r--   0        0        0     2291 2023-05-07 14:39:49.891967 py_tfl-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      121 2023-05-07 14:39:49.891967 py_tfl-0.1.1/tfl/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-07 14:39:49.891967 py_tfl-0.1.1/tfl/cli/__init__.py
+-rw-r--r--   0        0        0     1345 2023-05-07 14:39:49.891967 py_tfl-0.1.1/tfl/cli/_async_typer.py
+-rw-r--r--   0        0        0     1105 2023-05-07 14:39:49.891967 py_tfl-0.1.1/tfl/cli/main.py
+-rw-r--r--   0        0        0        0 2023-05-07 14:39:49.891967 py_tfl-0.1.1/tfl/cli/py.typed
+-rw-r--r--   0        0        0      231 2023-05-07 14:39:49.891967 py_tfl-0.1.1/tfl/clients/__init__.py
+-rw-r--r--   0        0        0     1696 2023-05-07 14:39:49.891967 py_tfl-0.1.1/tfl/clients/_auth.py
+-rw-r--r--   0        0        0     5000 2023-05-07 14:39:49.891967 py_tfl-0.1.1/tfl/clients/_client.py
+-rw-r--r--   0        0        0     4463 2023-05-07 14:39:49.891967 py_tfl-0.1.1/tfl/clients/_lift_disruptions_client.py
+-rw-r--r--   0        0        0        0 2023-05-07 14:39:49.891967 py_tfl-0.1.1/tfl/clients/py.typed
+-rw-r--r--   0        0        0        0 2023-05-07 14:39:49.891967 py_tfl-0.1.1/tfl/py.typed
+-rw-r--r--   0        0        0     5292 1970-01-01 00:00:00.000000 py_tfl-0.1.1/PKG-INFO
```

### Comparing `py_tfl-0.1.0/LICENSE` & `py_tfl-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_tfl-0.1.0/README.md` & `py_tfl-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-# tfl
+![TFL-Image.jpg](https://github.com/Ce11an/tfl/raw/main/assets/TFL-Image.jpg)
 
-![TFL-Image.jpg](https://github.com/Ce11an/tfl/blob/main/assets/TFL-Image.jpg)
-
-[![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/downloads/)
+[![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/py-tfl/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/Ce11an/tfl/blob/main/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/Ce11an/tfl/releases)
 ![Code Stability](https://github.com/Ce11an/tfl/actions/workflows/stability.yml/badge.svg)
 ![Unit Tests](https://github.com/Ce11an/tfl/actions/workflows/unit-tests.yml/badge.svg)
@@ -23,15 +21,21 @@
 Currently, this package only supports the
 [Lift Disruptions API](https://api-portal.tfl.gov.uk/api-details#api=Disruptions-Lifts-v2&operation=get). However,
 the plan is to add support for all the TFL APIs. Contributions are welcome!
 
 ## Installation
 
 ```bash
-poetry install
+pip install py-tfl
+```
+
+or install with [Poetry](https://python-poetry.org/):
+
+```bash
+poetry add py-tfl
 ```
 
 ## ⚡️Quickstart
 
 ### ⌨️ CLI
 The TFL CLI provides a command line interface to the TFL API. It is built on top of
 [Typer](https://typer.tiangolo.com/), which provides easy way to build command line interfaces.
@@ -44,25 +48,38 @@
 The TFL client provides a Python interface to the TFL API. It provides a Pythonic interface to the API, and handles
 authentication and rate limiting for you. The client is built on top of [HTTPX](https://www.python-httpx.org/), which
 provides a fast, async HTTP client.
 
 ```python
 from tfl import clients
 
+
 async with clients.LiftDisruptionsV2Client() as client:
     response = await client.get_lift_disruptions()
 
 print(response.json())
 ```
 
+## 📈 Releases
+
+You can see the list of available releases on the [GitHub Releases](https://github.com/Ce11an/tfl/releases)
+page.
+
+We follow [Semantic Versions](https://semver.org/) specification.
+
+We use [`Release Drafter`](https://github.com/marketplace/actions/release-drafter). As pull requests are merged, a draft
+release is kept up-to-date listing the changes, ready to publish when you’re ready. With the categories option, you can
+categorize pull requests in release notes using labels.
+
 ## 🛡 License
 
 [![License](https://img.shields.io/github/license/Ce11an/tfl)](https://github.com/Ce11an/tfl/blob/main/LICENSE)
 
-This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/Ce11an/tfl/blob/main/LICENSE) for more details.
+This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/Ce11an/tfl/blob/main/LICENSE)
+for more details.
 
 ## 🚀 Credits
 
 A special thanks to HTTPX, Typer, and the TFL API team for making this project possible.
 
 This project was built using [IntelliJ IDEA](https://www.jetbrains.com/community/opensource/?utm_campaign=opensource&utm_content=approved&utm_medium=email&utm_source=newsletter&utm_term=jblogo#support).
```

### Comparing `py_tfl-0.1.0/pyproject.toml` & `py_tfl-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "py-tfl"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python package for the Transport for London (TFL) API."
 authors = ["Cellan Hall <hallcellan@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "tfl"},
 ]
 homepage = "https://ce11an.github.io/tfl/"
```

### Comparing `py_tfl-0.1.0/tfl/cli/_async_typer.py` & `py_tfl-0.1.1/tfl/cli/_async_typer.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.1.0/tfl/cli/main.py` & `py_tfl-0.1.1/tfl/cli/main.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.1.0/tfl/clients/_auth.py` & `py_tfl-0.1.1/tfl/clients/_auth.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.1.0/tfl/clients/_client.py` & `py_tfl-0.1.1/tfl/clients/_client.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.1.0/tfl/clients/_lift_disruptions_client.py` & `py_tfl-0.1.1/tfl/clients/_lift_disruptions_client.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.1.0/PKG-INFO` & `py_tfl-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-tfl
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for the Transport for London (TFL) API.
 Home-page: https://ce11an.github.io/tfl/
 Author: Cellan Hall
 Author-email: hallcellan@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -22,19 +22,17 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/Ce11an/tfl
 Description-Content-Type: text/markdown
 
-# tfl
+![TFL-Image.jpg](https://github.com/Ce11an/tfl/raw/main/assets/TFL-Image.jpg)
 
-![TFL-Image.jpg](https://github.com/Ce11an/tfl/blob/main/assets/TFL-Image.jpg)
-
-[![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/downloads/)
+[![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/py-tfl/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/Ce11an/tfl/blob/main/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/Ce11an/tfl/releases)
 ![Code Stability](https://github.com/Ce11an/tfl/actions/workflows/stability.yml/badge.svg)
 ![Unit Tests](https://github.com/Ce11an/tfl/actions/workflows/unit-tests.yml/badge.svg)
@@ -51,15 +49,21 @@
 Currently, this package only supports the
 [Lift Disruptions API](https://api-portal.tfl.gov.uk/api-details#api=Disruptions-Lifts-v2&operation=get). However,
 the plan is to add support for all the TFL APIs. Contributions are welcome!
 
 ## Installation
 
 ```bash
-poetry install
+pip install py-tfl
+```
+
+or install with [Poetry](https://python-poetry.org/):
+
+```bash
+poetry add py-tfl
 ```
 
 ## ⚡️Quickstart
 
 ### ⌨️ CLI
 The TFL CLI provides a command line interface to the TFL API. It is built on top of
 [Typer](https://typer.tiangolo.com/), which provides easy way to build command line interfaces.
@@ -72,25 +76,38 @@
 The TFL client provides a Python interface to the TFL API. It provides a Pythonic interface to the API, and handles
 authentication and rate limiting for you. The client is built on top of [HTTPX](https://www.python-httpx.org/), which
 provides a fast, async HTTP client.
 
 ```python
 from tfl import clients
 
+
 async with clients.LiftDisruptionsV2Client() as client:
     response = await client.get_lift_disruptions()
 
 print(response.json())
 ```
 
+## 📈 Releases
+
+You can see the list of available releases on the [GitHub Releases](https://github.com/Ce11an/tfl/releases)
+page.
+
+We follow [Semantic Versions](https://semver.org/) specification.
+
+We use [`Release Drafter`](https://github.com/marketplace/actions/release-drafter). As pull requests are merged, a draft
+release is kept up-to-date listing the changes, ready to publish when you’re ready. With the categories option, you can
+categorize pull requests in release notes using labels.
+
 ## 🛡 License
 
 [![License](https://img.shields.io/github/license/Ce11an/tfl)](https://github.com/Ce11an/tfl/blob/main/LICENSE)
 
-This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/Ce11an/tfl/blob/main/LICENSE) for more details.
+This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/Ce11an/tfl/blob/main/LICENSE)
+for more details.
 
 ## 🚀 Credits
 
 A special thanks to HTTPX, Typer, and the TFL API team for making this project possible.
 
 This project was built using [IntelliJ IDEA](https://www.jetbrains.com/community/opensource/?utm_campaign=opensource&utm_content=approved&utm_medium=email&utm_source=newsletter&utm_term=jblogo#support).
```

