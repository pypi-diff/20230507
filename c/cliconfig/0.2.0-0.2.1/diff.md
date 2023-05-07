# Comparing `tmp/cliconfig-0.2.0.tar.gz` & `tmp/cliconfig-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-0.2.0.tar", last modified: Sun May  7 16:17:25 2023, max compression
+gzip compressed data, was "cliconfig-0.2.1.tar", last modified: Sun May  7 17:08:43 2023, max compression
```

## Comparing `cliconfig-0.2.0.tar` & `cliconfig-0.2.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.830807 cliconfig-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.818807 cliconfig-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.822807 cliconfig-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-07 16:17:07.000000 cliconfig-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 16:17:07.000000 cliconfig-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-07 16:17:25.830807 cliconfig-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-07 16:17:07.000000 cliconfig-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.822807 cliconfig-0.2.0/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-07 16:17:07.000000 cliconfig-0.2.0/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 16:17:25.000000 cliconfig-0.2.0/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-07 16:17:07.000000 cliconfig-0.2.0/cliconfig/build_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-07 16:17:07.000000 cliconfig-0.2.0/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-07 16:17:07.000000 cliconfig-0.2.0/cliconfig/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-07 16:17:07.000000 cliconfig-0.2.0/cliconfig/save_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-07 16:17:07.000000 cliconfig-0.2.0/cliconfig/show.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.826807 cliconfig-0.2.0/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-07 16:17:25.000000 cliconfig-0.2.0/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-07 16:17:25.000000 cliconfig-0.2.0/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 16:17:25.000000 cliconfig-0.2.0/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 16:17:25.000000 cliconfig-0.2.0/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 16:17:25.000000 cliconfig-0.2.0/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.826807 cliconfig-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/edge_cases.md
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/manipulate.md
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.826807 cliconfig-0.2.0/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 16:17:07.000000 cliconfig-0.2.0/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-07 16:17:07.000000 cliconfig-0.2.0/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-07 16:17:07.000000 cliconfig-0.2.0/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-07 16:17:07.000000 cliconfig-0.2.0/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-07 16:17:07.000000 cliconfig-0.2.0/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.826807 cliconfig-0.2.0/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-07 16:17:07.000000 cliconfig-0.2.0/licenses_tier/FLATTEN_DICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-07 16:17:07.000000 cliconfig-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-07 16:17:07.000000 cliconfig-0.2.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 16:17:07.000000 cliconfig-0.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.826807 cliconfig-0.2.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-07 16:17:07.000000 cliconfig-0.2.0/scripts/integration-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-07 16:17:07.000000 cliconfig-0.2.0/scripts/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 16:17:25.830807 cliconfig-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 16:17:07.000000 cliconfig-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.830807 cliconfig-0.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.830807 cliconfig-0.2.0/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/configs/default2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.830807 cliconfig-0.2.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/integration/integration_show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/test_build_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/test_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/test_save_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:08:43.255046 cliconfig-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 17:08:22.000000 cliconfig-0.2.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:08:43.243046 cliconfig-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:08:43.247046 cliconfig-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-07 17:08:22.000000 cliconfig-0.2.1/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-07 17:08:22.000000 cliconfig-0.2.1/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-07 17:08:22.000000 cliconfig-0.2.1/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 17:08:22.000000 cliconfig-0.2.1/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-07 17:08:22.000000 cliconfig-0.2.1/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-07 17:08:22.000000 cliconfig-0.2.1/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 17:08:22.000000 cliconfig-0.2.1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-07 17:08:22.000000 cliconfig-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-07 17:08:22.000000 cliconfig-0.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-07 17:08:22.000000 cliconfig-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 17:08:22.000000 cliconfig-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-07 17:08:43.255046 cliconfig-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-05-07 17:08:22.000000 cliconfig-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:08:43.247046 cliconfig-0.2.1/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-07 17:08:22.000000 cliconfig-0.2.1/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 17:08:43.000000 cliconfig-0.2.1/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-07 17:08:22.000000 cliconfig-0.2.1/cliconfig/build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-07 17:08:22.000000 cliconfig-0.2.1/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-05-07 17:08:22.000000 cliconfig-0.2.1/cliconfig/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-07 17:08:22.000000 cliconfig-0.2.1/cliconfig/save_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-07 17:08:22.000000 cliconfig-0.2.1/cliconfig/show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:08:43.251046 cliconfig-0.2.1/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-05-07 17:08:43.000000 cliconfig-0.2.1/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-07 17:08:43.000000 cliconfig-0.2.1/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 17:08:43.000000 cliconfig-0.2.1/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 17:08:43.000000 cliconfig-0.2.1/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 17:08:43.000000 cliconfig-0.2.1/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:08:43.251046 cliconfig-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-07 17:08:22.000000 cliconfig-0.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-07 17:08:22.000000 cliconfig-0.2.1/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-07 17:08:22.000000 cliconfig-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-07 17:08:22.000000 cliconfig-0.2.1/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-07 17:08:22.000000 cliconfig-0.2.1/docs/edge_cases.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-07 17:08:22.000000 cliconfig-0.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-07 17:08:22.000000 cliconfig-0.2.1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-07 17:08:22.000000 cliconfig-0.2.1/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-07 17:08:22.000000 cliconfig-0.2.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-07 17:08:22.000000 cliconfig-0.2.1/docs/manipulate.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-07 17:08:22.000000 cliconfig-0.2.1/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-07 17:08:22.000000 cliconfig-0.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:08:43.251046 cliconfig-0.2.1/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 17:08:22.000000 cliconfig-0.2.1/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-07 17:08:22.000000 cliconfig-0.2.1/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-07 17:08:22.000000 cliconfig-0.2.1/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-07 17:08:22.000000 cliconfig-0.2.1/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-07 17:08:22.000000 cliconfig-0.2.1/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:08:43.251046 cliconfig-0.2.1/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-07 17:08:22.000000 cliconfig-0.2.1/licenses_tier/FLATTEN_DICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-07 17:08:22.000000 cliconfig-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-07 17:08:22.000000 cliconfig-0.2.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 17:08:22.000000 cliconfig-0.2.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:08:43.251046 cliconfig-0.2.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-07 17:08:22.000000 cliconfig-0.2.1/scripts/integration-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-07 17:08:22.000000 cliconfig-0.2.1/scripts/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 17:08:43.255046 cliconfig-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 17:08:22.000000 cliconfig-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:08:43.251046 cliconfig-0.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:08:43.251046 cliconfig-0.2.1/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 17:08:22.000000 cliconfig-0.2.1/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 17:08:22.000000 cliconfig-0.2.1/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 17:08:22.000000 cliconfig-0.2.1/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 17:08:22.000000 cliconfig-0.2.1/tests/configs/default2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 17:08:43.255046 cliconfig-0.2.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-07 17:08:22.000000 cliconfig-0.2.1/tests/integration/integration_show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-07 17:08:22.000000 cliconfig-0.2.1/tests/test_build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-07 17:08:22.000000 cliconfig-0.2.1/tests/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-07 17:08:22.000000 cliconfig-0.2.1/tests/test_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-07 17:08:22.000000 cliconfig-0.2.1/tests/test_save_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-07 17:08:22.000000 cliconfig-0.2.1/tests/test_show.py
```

### Comparing `cliconfig-0.2.0/.github/workflows/pipy_deployment.yaml` & `cliconfig-0.2.1/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/.github/workflows/pydocstyle.yaml` & `cliconfig-0.2.1/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/.github/workflows/pylint.yaml` & `cliconfig-0.2.1/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/.github/workflows/tests.yaml` & `cliconfig-0.2.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/.pylintrc` & `cliconfig-0.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/CONTRIBUTING.md` & `cliconfig-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/LICENSE` & `cliconfig-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/PKG-INFO` & `cliconfig-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.2.0
+Version: 0.2.1
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 Lightweight library that provides routines to merge your configs (optionally nested)
 and set parameters from command line. It also prevents you from adding new parameters
 if not desired. Finally, it provides helper routines to manage flatten dicts, unflatten
 (= nested) dicts or a mix of both, save config, load, display, etc.
 
 ## Documentation :memo: [here](https://cliconfig.readthedocs.io/en/stable)
 
-[![PyPI version](https://badge.fury.io/py/cliconfig.svg)](https://badge.fury.io/py/cliconfig)
+[![Release](https://img.shields.io/github/v/release/valentingol/cliconfig?include_prereleases)](https://pypi.org/project/cliconfig/)
 ![PythonVersion](https://img.shields.io/badge/python-3.7%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/cliconfig?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![Ruff](https://github.com/valentingol/cliconfig/actions/workflows/ruff.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/ruff.yaml)
```

### Comparing `cliconfig-0.2.0/README.md` & `cliconfig-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Lightweight library that provides routines to merge your configs (optionally nested)
 and set parameters from command line. It also prevents you from adding new parameters
 if not desired. Finally, it provides helper routines to manage flatten dicts, unflatten
 (= nested) dicts or a mix of both, save config, load, display, etc.
 
 ## Documentation :memo: [here](https://cliconfig.readthedocs.io/en/stable)
 
-[![PyPI version](https://badge.fury.io/py/cliconfig.svg)](https://badge.fury.io/py/cliconfig)
+[![Release](https://img.shields.io/github/v/release/valentingol/cliconfig?include_prereleases)](https://pypi.org/project/cliconfig/)
 ![PythonVersion](https://img.shields.io/badge/python-3.7%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/cliconfig?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![Ruff](https://github.com/valentingol/cliconfig/actions/workflows/ruff.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/ruff.yaml)
```

### Comparing `cliconfig-0.2.0/cliconfig/__init__.py` & `cliconfig-0.2.1/cliconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/cliconfig/build_config.py` & `cliconfig-0.2.1/cliconfig/build_config.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/cliconfig/cli_parser.py` & `cliconfig-0.2.1/cliconfig/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/cliconfig/routines.py` & `cliconfig-0.2.1/cliconfig/routines.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,16 +142,16 @@
         If config has some conflicting keys (like `{'a.b': ..., 'a': {'b': ...}}`).
 
     Returns
     -------
     config : Dict[str, Any]
         The flattened config.
 
-    Notes
-    -----
+    Note
+    ----
         Nested empty dict are ignored even if they are conflicting (see last example).
 
     Examples
     --------
     ::
 
         >>> flat_config({'a.b': 1, 'a': {'c': 2}, 'd': 3})
```

### Comparing `cliconfig-0.2.0/cliconfig/save_load.py` & `cliconfig-0.2.1/cliconfig/save_load.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/cliconfig/show.py` & `cliconfig-0.2.1/cliconfig/show.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/cliconfig.egg-info/PKG-INFO` & `cliconfig-0.2.1/cliconfig.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.2.0
+Version: 0.2.1
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 Lightweight library that provides routines to merge your configs (optionally nested)
 and set parameters from command line. It also prevents you from adding new parameters
 if not desired. Finally, it provides helper routines to manage flatten dicts, unflatten
 (= nested) dicts or a mix of both, save config, load, display, etc.
 
 ## Documentation :memo: [here](https://cliconfig.readthedocs.io/en/stable)
 
-[![PyPI version](https://badge.fury.io/py/cliconfig.svg)](https://badge.fury.io/py/cliconfig)
+[![Release](https://img.shields.io/github/v/release/valentingol/cliconfig?include_prereleases)](https://pypi.org/project/cliconfig/)
 ![PythonVersion](https://img.shields.io/badge/python-3.7%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/cliconfig?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 [![Ruff](https://github.com/valentingol/cliconfig/actions/workflows/ruff.yaml/badge.svg)](https://github.com/valentingol/cliconfig/actions/workflows/ruff.yaml)
```

### Comparing `cliconfig-0.2.0/cliconfig.egg-info/SOURCES.txt` & `cliconfig-0.2.1/cliconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/docs/Makefile` & `cliconfig-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/docs/cliconfig_api.rst` & `cliconfig-0.2.1/docs/cliconfig_api.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/docs/conf.py` & `cliconfig-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/docs/edge_cases.md` & `cliconfig-0.2.1/docs/edge_cases.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/docs/index.rst` & `cliconfig-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/docs/license.md` & `cliconfig-0.2.1/docs/license.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/docs/make.bat` & `cliconfig-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/docs/manipulate.md` & `cliconfig-0.2.1/docs/manipulate.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/docs/quickstart.md` & `cliconfig-0.2.1/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/github_actions_utils/pydocstyle_manager.py` & `cliconfig-0.2.1/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/github_actions_utils/pylint_manager.py` & `cliconfig-0.2.1/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/github_actions_utils/pytest_manager.py` & `cliconfig-0.2.1/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/licenses_tier/FLATTEN_DICT_LICENSE` & `cliconfig-0.2.1/licenses_tier/FLATTEN_DICT_LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/pyproject.toml` & `cliconfig-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/scripts/pre-commit-checks.sh` & `cliconfig-0.2.1/scripts/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/tests/integration/integration_show.py` & `cliconfig-0.2.1/tests/integration/integration_show.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/tests/test_build_config.py` & `cliconfig-0.2.1/tests/test_build_config.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/tests/test_cli_parser.py` & `cliconfig-0.2.1/tests/test_cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/tests/test_routines.py` & `cliconfig-0.2.1/tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/tests/test_save_load.py` & `cliconfig-0.2.1/tests/test_save_load.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.2.0/tests/test_show.py` & `cliconfig-0.2.1/tests/test_show.py`

 * *Files identical despite different names*

