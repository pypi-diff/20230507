# Comparing `tmp/flxtrd-0.0.1.tar.gz` & `tmp/flxtrd-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flxtrd-0.0.1.tar", max compression
+gzip compressed data, was "flxtrd-0.0.2.tar", max compression
```

## Comparing `flxtrd-0.0.1.tar` & `flxtrd-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1057 2023-04-24 19:07:04.384041 flxtrd-0.0.1/LICENSE
--rw-r--r--   0        0        0     2590 2023-04-25 18:27:36.870078 flxtrd-0.0.1/README.md
--rw-r--r--   0        0        0     1895 2023-04-25 19:07:48.573369 flxtrd-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 19:08:02.289370 flxtrd-0.0.1/src/empty/__init__.py
--rw-r--r--   0        0        0     3311 1970-01-01 00:00:00.000000 flxtrd-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     9135 2023-05-05 08:04:47.294863 flxtrd-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2547 2023-05-07 17:50:02.220036 flxtrd-0.0.2/README.md
+-rw-r--r--   0        0        0     1883 2023-05-07 17:55:20.495107 flxtrd-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-07 17:55:35.934823 flxtrd-0.0.2/src/__init__.py
+-rw-r--r--   0        0        0     3267 1970-01-01 00:00:00.000000 flxtrd-0.0.2/PKG-INFO
```

### Comparing `flxtrd-0.0.1/README.md` & `flxtrd-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# flextrade
+# flxtrd
 
-[![Release](https://img.shields.io/github/v/release/glocalflex/flextrade)](https://img.shields.io/github/v/release/glocalflex/flextrade)
-[![Build status](https://img.shields.io/github/actions/workflow/status/glocalflex/flextrade/main.yml?branch=main)](https://github.com/glocalflex/flextrade/actions/workflows/main.yml?query=branch%3Amain)
-[![codecov](https://codecov.io/gh/glocalflex/flextrade/branch/main/graph/badge.svg)](https://codecov.io/gh/glocalflex/flextrade)
-[![Commit activity](https://img.shields.io/github/commit-activity/m/glocalflex/flextrade)](https://img.shields.io/github/commit-activity/m/glocalflex/flextrade)
-[![License](https://img.shields.io/github/license/glocalflex/flextrade)](https://img.shields.io/github/license/glocalflex/flextrade)
+[![Release](https://img.shields.io/github/v/release/glocalflex/flxtrd)](https://img.shields.io/github/v/release/glocalflex/flxtrd)
+[![Build status](https://img.shields.io/github/actions/workflow/status/glocalflex/flxtrd/main.yml?branch=main)](https://github.com/glocalflex/flxtrd/actions/workflows/main.yml?query=branch%3Amain)
+[![codecov](https://codecov.io/gh/glocalflex/flxtrd/branch/main/graph/badge.svg)](https://codecov.io/gh/glocalflex/flxtrd)
+[![Commit activity](https://img.shields.io/github/commit-activity/m/glocalflex/flxtrd)](https://img.shields.io/github/commit-activity/m/glocalflex/flxtrd)
+[![License](https://img.shields.io/github/license/glocalflex/flxtrd)](https://img.shields.io/github/license/glocalflex/flxtrd)
 
-trading API for the flexible energy trading platform GLocalFlex
+Public client API for the flexible energy trading market GLocalFlex.
 
-- **Github repository**: <https://github.com/glocalflex/flextrade/>
-- **Documentation** <https://glocalflex.github.io/flextrade/>
+- **Github repository**: <https://github.com/glocalflex/flxtrd/>
+- **Documentation** <https://glocalflex.github.io/flxtrd/>
 
 ## Getting started with your project
 
 First, create a repository on GitHub with the same name as this project, and then run the following commands:
 
 ``` bash
 git init -b main
 git add .
 git commit -m "init commit"
-git remote add origin git@github.com:glocalflex/flextrade.git
+git remote add origin git@github.com:glocalflex/flxtrd.git
 git push -u origin main
 ```
 
 Finally, install the environment and the pre-commit hooks with 
 
 ```bash
 make install
@@ -39,16 +39,16 @@
 [here](https://fpgmaas.github.io/cookiecutter-poetry/features/mkdocs/#enabling-the-documentation-on-github).
 To enable the code coverage reports, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/codecov/).
 
 ## Releasing a new version
 
 - Create an API Token on [Pypi](https://pypi.org/).
 - Add the API Token to your projects secrets with the name `PYPI_TOKEN` by visiting 
-[this page](https://github.com/glocalflex/flextrade/settings/secrets/actions/new).
-- Create a [new release](https://github.com/glocalflex/flextrade/releases/new) on Github. 
+[this page](https://github.com/glocalflex/flxtrd/settings/secrets/actions/new).
+- Create a [new release](https://github.com/glocalflex/flxtrd/releases/new) on Github. 
 Create a new tag in the form ``*.*.*``.
 
 For more details, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/cicd/#how-to-trigger-a-release).
 
 ---
 
 Repository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).
```

### Comparing `flxtrd-0.0.1/pyproject.toml` & `flxtrd-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "flxtrd"
-version = "0.0.1"
-description = "Trading client for the flexible energy trading platform GLocalFlex"
+version = "0.0.2"
+description = "Public client API for the flexible energy trading market GLocalFlex."
 authors = ["glocalflex"]
-repository = "https://github.com/glocalflex/flextrade"
-documentation = "https://glocalflex.github.io/flextrade/"
+repository = "https://github.com/glocalflex/flxtrade"
+documentation = "https://glocalflex.github.io/flxtrade/"
 readme = "README.md"
 packages = [
-  {include = "src/empty"}
+  {include = "src"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 pika = "^1.3.1"
 requests = ">=2.28.0"
 
@@ -36,15 +36,15 @@
 
 [tool.black]
 line-length = 120
 target-version = ['py37']
 preview = true
 
 [tool.mypy]
-files = ["flextrade"]
+files = ["flxtrd"]
 disallow_untyped_defs = "True"
 disallow_any_unimported = "True"
 no_implicit_optional = "True"
 check_untyped_defs = "True"
 warn_return_any = "True"
 warn_unused_ignores = "True"
 show_error_codes = "True"
@@ -96,10 +96,10 @@
 "tests/*" = ["S101"]
 
 [tool.coverage.report]
 skip_empty = true
 
 [tool.coverage.run]
 branch = true
-source = ["flextrade"]
+source = ["flxtrd"]
```

### Comparing `flxtrd-0.0.1/PKG-INFO` & `flxtrd-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 Metadata-Version: 2.1
 Name: flxtrd
-Version: 0.0.1
-Summary: Trading client for the flexible energy trading platform GLocalFlex
-Home-page: https://github.com/glocalflex/flextrade
+Version: 0.0.2
+Summary: Public client API for the flexible energy trading market GLocalFlex.
+Home-page: https://github.com/glocalflex/flxtrade
 Author: glocalflex
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pika (>=1.3.1,<2.0.0)
 Requires-Dist: requests (>=2.28.0)
-Project-URL: Documentation, https://glocalflex.github.io/flextrade/
-Project-URL: Repository, https://github.com/glocalflex/flextrade
+Project-URL: Documentation, https://glocalflex.github.io/flxtrade/
+Project-URL: Repository, https://github.com/glocalflex/flxtrade
 Description-Content-Type: text/markdown
 
-# flextrade
+# flxtrd
 
-[![Release](https://img.shields.io/github/v/release/glocalflex/flextrade)](https://img.shields.io/github/v/release/glocalflex/flextrade)
-[![Build status](https://img.shields.io/github/actions/workflow/status/glocalflex/flextrade/main.yml?branch=main)](https://github.com/glocalflex/flextrade/actions/workflows/main.yml?query=branch%3Amain)
-[![codecov](https://codecov.io/gh/glocalflex/flextrade/branch/main/graph/badge.svg)](https://codecov.io/gh/glocalflex/flextrade)
-[![Commit activity](https://img.shields.io/github/commit-activity/m/glocalflex/flextrade)](https://img.shields.io/github/commit-activity/m/glocalflex/flextrade)
-[![License](https://img.shields.io/github/license/glocalflex/flextrade)](https://img.shields.io/github/license/glocalflex/flextrade)
+[![Release](https://img.shields.io/github/v/release/glocalflex/flxtrd)](https://img.shields.io/github/v/release/glocalflex/flxtrd)
+[![Build status](https://img.shields.io/github/actions/workflow/status/glocalflex/flxtrd/main.yml?branch=main)](https://github.com/glocalflex/flxtrd/actions/workflows/main.yml?query=branch%3Amain)
+[![codecov](https://codecov.io/gh/glocalflex/flxtrd/branch/main/graph/badge.svg)](https://codecov.io/gh/glocalflex/flxtrd)
+[![Commit activity](https://img.shields.io/github/commit-activity/m/glocalflex/flxtrd)](https://img.shields.io/github/commit-activity/m/glocalflex/flxtrd)
+[![License](https://img.shields.io/github/license/glocalflex/flxtrd)](https://img.shields.io/github/license/glocalflex/flxtrd)
 
-trading API for the flexible energy trading platform GLocalFlex
+Public client API for the flexible energy trading market GLocalFlex.
 
-- **Github repository**: <https://github.com/glocalflex/flextrade/>
-- **Documentation** <https://glocalflex.github.io/flextrade/>
+- **Github repository**: <https://github.com/glocalflex/flxtrd/>
+- **Documentation** <https://glocalflex.github.io/flxtrd/>
 
 ## Getting started with your project
 
 First, create a repository on GitHub with the same name as this project, and then run the following commands:
 
 ``` bash
 git init -b main
 git add .
 git commit -m "init commit"
-git remote add origin git@github.com:glocalflex/flextrade.git
+git remote add origin git@github.com:glocalflex/flxtrd.git
 git push -u origin main
 ```
 
 Finally, install the environment and the pre-commit hooks with 
 
 ```bash
 make install
@@ -57,16 +57,16 @@
 [here](https://fpgmaas.github.io/cookiecutter-poetry/features/mkdocs/#enabling-the-documentation-on-github).
 To enable the code coverage reports, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/codecov/).
 
 ## Releasing a new version
 
 - Create an API Token on [Pypi](https://pypi.org/).
 - Add the API Token to your projects secrets with the name `PYPI_TOKEN` by visiting 
-[this page](https://github.com/glocalflex/flextrade/settings/secrets/actions/new).
-- Create a [new release](https://github.com/glocalflex/flextrade/releases/new) on Github. 
+[this page](https://github.com/glocalflex/flxtrd/settings/secrets/actions/new).
+- Create a [new release](https://github.com/glocalflex/flxtrd/releases/new) on Github. 
 Create a new tag in the form ``*.*.*``.
 
 For more details, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/cicd/#how-to-trigger-a-release).
 
 ---
 
 Repository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).
```

