# Comparing `tmp/pytest-static-0.0.0.tar.gz` & `tmp/pytest-static-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-static-0.0.0.tar", max compression
+gzip compressed data, was "pytest-static-0.1.0.tar", max compression
```

## Comparing `pytest-static-0.0.0.tar` & `pytest-static-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2023-05-06 21:48:10.974452 pytest-static-0.0.0/LICENSE
--rw-r--r--   0        0        0     1818 2023-05-06 21:48:10.940420 pytest-static-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     2468 2023-05-06 21:48:10.952420 pytest-static-0.0.0/README.md
--rw-r--r--   0        0        0       21 2023-05-06 21:48:11.094429 pytest-static-0.0.0/src/pytest_static/__init__.py
--rw-r--r--   0        0        0      216 2023-05-06 21:48:11.102420 pytest-static-0.0.0/src/pytest_static/__main__.py
--rw-r--r--   0        0        0        0 2023-05-06 21:48:11.087450 pytest-static-0.0.0/src/pytest_static/py.typed
--rw-r--r--   0        0        0     3360 2023-05-06 22:06:02.599097 pytest-static-0.0.0/setup.py
--rw-r--r--   0        0        0     3320 2023-05-06 22:06:02.600098 pytest-static-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-06 21:48:10.974452 pytest-static-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1818 2023-05-07 00:27:07.258413 pytest-static-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2468 2023-05-06 21:48:10.952420 pytest-static-0.1.0/README.md
+-rw-r--r--   0        0        0       21 2023-05-06 21:48:11.094429 pytest-static-0.1.0/src/pytest_static/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-06 21:48:11.102420 pytest-static-0.1.0/src/pytest_static/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-06 21:48:11.087450 pytest-static-0.1.0/src/pytest_static/py.typed
+-rw-r--r--   0        0        0     3360 2023-05-07 01:22:04.762640 pytest-static-0.1.0/setup.py
+-rw-r--r--   0        0        0     3320 2023-05-07 01:22:04.762640 pytest-static-0.1.0/PKG-INFO
```

### Comparing `pytest-static-0.0.0/LICENSE` & `pytest-static-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-static-0.0.0/pyproject.toml` & `pytest-static-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-static"
-version = "0.0.0"
+version = "0.1.0"
 description = "pytest-static"
 authors = ["Kyle Oliver <56kyleoliver@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/56kyle/pytest-static"
 repository = "https://github.com/56kyle/pytest-static"
 documentation = "https://pytest-static.readthedocs.io"
```

### Comparing `pytest-static-0.0.0/README.md` & `pytest-static-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest-static-0.0.0/setup.py` & `pytest-static-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['click>=8.0.1']
 
 entry_points = \
 {'console_scripts': ['pytest-static = pytest_static.__main__:main']}
 
 setup_kwargs = {
     'name': 'pytest-static',
-    'version': '0.0.0',
+    'version': '0.1.0',
     'description': 'pytest-static',
     'long_description': "# pytest-static\n\n[![PyPI](https://img.shields.io/pypi/v/pytest-static.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/pytest-static.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/pytest-static)][python version]\n[![License](https://img.shields.io/pypi/l/pytest-static)][license]\n\n[![Read the documentation at https://pytest-static.readthedocs.io/](https://img.shields.io/readthedocs/pytest-static/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/56kyle/pytest-static/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/56kyle/pytest-static/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/pytest-static/\n[status]: https://pypi.org/project/pytest-static/\n[python version]: https://pypi.org/project/pytest-static\n[read the docs]: https://pytest-static.readthedocs.io/\n[tests]: https://github.com/56kyle/pytest-static/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/56kyle/pytest-static\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n- TODO\n\n## Requirements\n\n- TODO\n\n## Installation\n\nYou can install _pytest-static_ via [pip] from [PyPI]:\n\n```console\n$ pip install pytest-static\n```\n\n## Usage\n\nPlease see the [Command-line Reference] for details.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_pytest-static_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/56kyle/pytest-static/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/56kyle/pytest-static/blob/main/LICENSE\n[contributor guide]: https://github.com/56kyle/pytest-static/blob/main/CONTRIBUTING.md\n[command-line reference]: https://pytest-static.readthedocs.io/en/latest/usage.html\n",
     'author': 'Kyle Oliver',
     'author_email': '56kyleoliver@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/56kyle/pytest-static',
```

### Comparing `pytest-static-0.0.0/PKG-INFO` & `pytest-static-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-static
-Version: 0.0.0
+Version: 0.1.0
 Summary: pytest-static
 Home-page: https://github.com/56kyle/pytest-static
 License: MIT
 Author: Kyle Oliver
 Author-email: 56kyleoliver@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 1 - Planning
```

