# Comparing `tmp/cliconfig-0.1.4.tar.gz` & `tmp/cliconfig-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-0.1.4.tar", last modified: Sun May  7 01:17:04 2023, max compression
+gzip compressed data, was "cliconfig-0.2.0.tar", last modified: Sun May  7 16:17:25 2023, max compression
```

## Comparing `cliconfig-0.1.4.tar` & `cliconfig-0.2.0.tar`

### file list

```diff
@@ -1,68 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.250839 cliconfig-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.242839 cliconfig-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.242839 cliconfig-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-07 01:16:42.000000 cliconfig-0.1.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 01:16:42.000000 cliconfig-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-07 01:17:04.250839 cliconfig-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-07 01:16:42.000000 cliconfig-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.246839 cliconfig-0.1.4/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-07 01:16:42.000000 cliconfig-0.1.4/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 01:17:04.000000 cliconfig-0.1.4/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-07 01:16:42.000000 cliconfig-0.1.4/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-05-07 01:16:42.000000 cliconfig-0.1.4/cliconfig/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-07 01:16:42.000000 cliconfig-0.1.4/cliconfig/show.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.246839 cliconfig-0.1.4/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-07 01:17:04.000000 cliconfig-0.1.4/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-07 01:17:04.000000 cliconfig-0.1.4/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 01:17:04.000000 cliconfig-0.1.4/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 01:17:04.000000 cliconfig-0.1.4/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 01:17:04.000000 cliconfig-0.1.4/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.246839 cliconfig-0.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/manipulate_configs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.246839 cliconfig-0.1.4/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 01:16:42.000000 cliconfig-0.1.4/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-07 01:16:42.000000 cliconfig-0.1.4/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-07 01:16:42.000000 cliconfig-0.1.4/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-07 01:16:42.000000 cliconfig-0.1.4/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-07 01:16:42.000000 cliconfig-0.1.4/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.246839 cliconfig-0.1.4/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-07 01:16:42.000000 cliconfig-0.1.4/licenses_tier/FLATTEN_DICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-07 01:16:42.000000 cliconfig-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-07 01:16:42.000000 cliconfig-0.1.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 01:16:42.000000 cliconfig-0.1.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.246839 cliconfig-0.1.4/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-07 01:16:42.000000 cliconfig-0.1.4/scripts/integration-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-07 01:16:42.000000 cliconfig-0.1.4/scripts/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 01:17:04.250839 cliconfig-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 01:16:42.000000 cliconfig-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.250839 cliconfig-0.1.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.250839 cliconfig-0.1.4/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 01:16:42.000000 cliconfig-0.1.4/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 01:16:42.000000 cliconfig-0.1.4/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 01:16:42.000000 cliconfig-0.1.4/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 01:16:42.000000 cliconfig-0.1.4/tests/configs/default2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.250839 cliconfig-0.1.4/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-07 01:16:42.000000 cliconfig-0.1.4/tests/integration/integration_show.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-07 01:16:42.000000 cliconfig-0.1.4/tests/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-07 01:16:42.000000 cliconfig-0.1.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-07 01:16:42.000000 cliconfig-0.1.4/tests/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.830807 cliconfig-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.818807 cliconfig-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.822807 cliconfig-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-07 16:17:07.000000 cliconfig-0.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-07 16:17:07.000000 cliconfig-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 16:17:07.000000 cliconfig-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-07 16:17:25.830807 cliconfig-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-07 16:17:07.000000 cliconfig-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.822807 cliconfig-0.2.0/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-07 16:17:07.000000 cliconfig-0.2.0/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 16:17:25.000000 cliconfig-0.2.0/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-07 16:17:07.000000 cliconfig-0.2.0/cliconfig/build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-07 16:17:07.000000 cliconfig-0.2.0/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-07 16:17:07.000000 cliconfig-0.2.0/cliconfig/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-07 16:17:07.000000 cliconfig-0.2.0/cliconfig/save_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-07 16:17:07.000000 cliconfig-0.2.0/cliconfig/show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.826807 cliconfig-0.2.0/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-07 16:17:25.000000 cliconfig-0.2.0/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-07 16:17:25.000000 cliconfig-0.2.0/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 16:17:25.000000 cliconfig-0.2.0/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 16:17:25.000000 cliconfig-0.2.0/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 16:17:25.000000 cliconfig-0.2.0/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.826807 cliconfig-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/edge_cases.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/manipulate.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-07 16:17:07.000000 cliconfig-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.826807 cliconfig-0.2.0/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 16:17:07.000000 cliconfig-0.2.0/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-07 16:17:07.000000 cliconfig-0.2.0/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-07 16:17:07.000000 cliconfig-0.2.0/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-07 16:17:07.000000 cliconfig-0.2.0/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-07 16:17:07.000000 cliconfig-0.2.0/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.826807 cliconfig-0.2.0/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-07 16:17:07.000000 cliconfig-0.2.0/licenses_tier/FLATTEN_DICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-07 16:17:07.000000 cliconfig-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-07 16:17:07.000000 cliconfig-0.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 16:17:07.000000 cliconfig-0.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.826807 cliconfig-0.2.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-07 16:17:07.000000 cliconfig-0.2.0/scripts/integration-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-07 16:17:07.000000 cliconfig-0.2.0/scripts/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 16:17:25.830807 cliconfig-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 16:17:07.000000 cliconfig-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.830807 cliconfig-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.830807 cliconfig-0.2.0/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/configs/default2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:17:25.830807 cliconfig-0.2.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/integration/integration_show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/test_build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/test_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/test_save_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-07 16:17:07.000000 cliconfig-0.2.0/tests/test_show.py
```

### Comparing `cliconfig-0.1.4/.github/workflows/pipy_deployment.yaml` & `cliconfig-0.2.0/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/.github/workflows/pydocstyle.yaml` & `cliconfig-0.2.0/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/.github/workflows/pylint.yaml` & `cliconfig-0.2.0/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/.github/workflows/tests.yaml` & `cliconfig-0.2.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/.pylintrc` & `cliconfig-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/CONTRIBUTING.md` & `cliconfig-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/LICENSE` & `cliconfig-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/PKG-INFO` & `cliconfig-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,13 @@
-Metadata-Version: 2.1
-Name: cliconfig
-Version: 0.1.4
-Summary: Merge your config files and set parameters from the command line in a simple way.
-Author-email: Valentin Goldite <valentin.goldite@gmail.com>
-Project-URL: Source, https://github.com/valentingol/cliconfig
-Keywords: logging,machine,learning
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CLI Config
 
-Lightweight library to merge your configs (optionally nested) and set parameters
-from command line.
+Lightweight library that provides routines to merge your configs (optionally nested)
+and set parameters from command line. It also prevents you from adding new parameters
+if not desired. Finally, it provides helper routines to manage flatten dicts, unflatten
+(= nested) dicts or a mix of both, save config, load, display, etc.
 
 ## Documentation :memo: [here](https://cliconfig.readthedocs.io/en/stable)
 
 [![PyPI version](https://badge.fury.io/py/cliconfig.svg)](https://badge.fury.io/py/cliconfig)
 ![PythonVersion](https://img.shields.io/badge/python-3.7%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/cliconfig?color=999)](https://stringfixer.com/fr/MIT_license)
 
@@ -41,27 +31,26 @@
 ```bash
 pip install cliconfig
 ```
 
 ## Quick start
 
 First create a default config that can be split in multiple files that will be merged
-(from left to right in `make_config` function):
+(from left to right in `make_config` function). There is no limit of depth for the
+configurations parameters.
 
 ```yaml
-# default1.yaml
+---  # default1.yaml
 param1: 1
 param2: 0
 letters:
   letter1: a
   letter2: b
-```
 
-```yaml
-# default2.yaml
+---  # default2.yaml
 param1: 1
 param2: 2  # will override param2 from default1.yaml
 letters.letter3: c  # add a new parameter
 ```
 
 Now you can set up your program to use the config:
 
@@ -70,38 +59,38 @@
 from cliconfig import make_config, show_config
 
 config = make_config('default1.yaml', 'default2.yaml')
 show_config(config)
 ```
 
 Then add one or multiple additional config files that will override the default values.
-**Be careful, the additional config files cannot bring new parameters by default**.
-If you want to add new parameters (not advised for retro-compatibility, readability
-and security), you can add `allow_new_keys=True` in `make_config` function.
+**By default the additional config files cannot bring new parameters**.
+It is intended to prevent typos in the config files that would not be detected.
+It also improves the readability of the config files and the retro-compatibility.
+By the way, you can change this behavior with `allow_new_keys=True` in `make_config`
+(be careful).
 
 ```yaml
-# exp1.yaml
+---  # first.yaml
 letters:
   letter3: C
-```
 
-```yaml
-# exp2.yaml
+---  # second.yaml
 param1: -1
 letters.letter1: A
 ```
 
 Now you can launch the program with additional configurations and parameters.
 The additional configurations are indicated with `--config` (separate with comma,
 without space) and the parameters with `--<param_name>`. The default configuration
 will be merged with the additional configurations (from left to right), then the
 parameters will be set.
 
 ```bash
-python main.py --config exp1.yaml,exp2.yaml --param2=-2 --letters.letter2='B'
+python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
 ```
 
 Will show:
 
 ```text
 [CONFIG] Merge 2 default configs, 2 additional configs and 2 CLI parameter(s).
 
@@ -112,25 +101,55 @@
         letter1: A
         letter2: B
         letter3: C
 ```
 
 Note that the configurations are native python dicts.
 
+## Edge cases
+
+**Be careful, tuples and sets are not supported by YAML and cannot be used in configs.**
+Use lists instead if possible
+
+`None` is not recognized as a None object by YAML but as a string, you may use `null`
+or `Null` instead if you want to
+set a None object.
+
+Dicts are considered as sub-configs and so you may not be able to change the keys if
+`allow_new_keys=False` (default). If you want to modify a dict keys, you should
+enclose it in a list.
+
+For instance:
+
+```yaml
+--- default.yaml
+logging:
+  metrics: ['train loss', 'val loss']
+  styles: [{'train loss': 'red', 'val loss': 'blue'}]
+--- experiment.yaml
+logging:
+  metrics: ['train loss', 'val loss', 'val acc']
+  styles: [{'train loss': 'red', 'val loss': 'blue', 'val acc': 'cyan'}]
+```
+
 ## Manipulate configs
 
-To merge configs, you can use `cliconfig.merge_config` function.
-It supports unflatten (or nested) dicts like `{'a': {'b': 1, 'c': 2}}`,
-flatten dicts like `{'a.b': 1, 'a.c': 2}`, and a mix of both. The dicts will be flatten
-before merging. Sometimes you can have conflicts in flatten operation for instance with
-`{'a.b': 1, 'a': {'b': 2}}` that have two different values for `a.b`. That's why you
-can use a `priority` parameter to choose which value to keep before merging.
+You are encouraged to use the routines provided by `cliconfig` to manipulate configs
+and even create your own config builder to replace `make_config`. You can use:
 
-You can also save, load and display configs with `cliconfig.save_config`,
-`cliconfig.load_config` and `cliconfig.show_config` functions.
+- `merge_config` and `merge_config_file` to merge your configs
+- `parse_cli` to parse CLI arguments on config files and additional parameters
+- `flat_config` and `unflat_config` to flatten and unflatten your configs
+- `clean_pre_flat` to clean conflicting keys before flattening
+
+You can also save, load and display configs with `save_config`,
+`load_config` and `show_config` functions.
+
+Note that theses functions are aimed to be use with configs but can be used with
+any python dict.
 
 ## How to contribute
 
 For **development**, install the package dynamically and dev requirements with:
 
 ```bash
 pip install -e .
@@ -140,16 +159,23 @@
 Everyone can contribute to CLI Config, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ### Todo
 
 To do:
 
-- [ ] add json and ini support
-- [ ] avoid changing keys order in merge_config
+- [ ] log warning when `None` is used in CLI (considered as string a by PyYAML)
+
+Done:
+
+- [x] add `merge_config_file` to merge from path (= `merge_config` that includes
+  config loading)
+- [x] add `clean_pre_flat` to solve conflicting flatten and unflatten parameters
+  before flattening the config
+- [x] avoid changing keys order in merge_config
 
 ## License
 
 Copyright (C) 2023  Valentin Goldité
 
 This program is free software: you can redistribute it and/or modify it under the
 terms of the [MIT License](LICENSE). This program is distributed in the hope that
```

### Comparing `cliconfig-0.1.4/cliconfig/__init__.py` & `cliconfig-0.2.0/cliconfig/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,19 +9,33 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
     This project is free to use for COMMERCIAL USE, MODIFICATION,
     DISTRIBUTION and PRIVATE USE as long as the original license is
     include as well as this copy right notice.
 """
 # pylint: disable=wrong-import-position
 from cliconfig._version import __version__, __version_tuple__
-from cliconfig.config import load_config, make_config, merge_config, save_config
+from cliconfig.build_config import make_config
+from cliconfig.cli_parser import parse_cli
+from cliconfig.routines import (
+    clean_pre_flat,
+    flat_config,
+    merge_config,
+    merge_config_file,
+    unflat_config,
+)
+from cliconfig.save_load import load_config, save_config
 from cliconfig.show import show_config
 
 __all__ = [
     "__version__",
     "__version_tuple__",
+    "clean_pre_flat",
+    "flat_config",
     "load_config",
     "make_config",
     "merge_config",
+    "merge_config_file",
+    "parse_cli",
     "save_config",
     "show_config",
+    "unflat_config",
 ]
```

### Comparing `cliconfig-0.1.4/cliconfig/cli_parser.py` & `cliconfig-0.2.0/cliconfig/cli_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Parser for CLI commands."""
 from typing import Any, Dict, List, Tuple
 
 import yaml
 
 
-def parse(sys_argv: List[str]) -> Tuple[List[str], Dict[str, Any]]:
+def parse_cli(sys_argv: List[str]) -> Tuple[List[str], Dict[str, Any]]:
     """Parser for CLI commands.
 
     Parameters
     ----------
     sys_argv : List[str]
         List of arguments from sys.argv.
```

### Comparing `cliconfig-0.1.4/cliconfig/show.py` & `cliconfig-0.2.0/cliconfig/show.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/cliconfig.egg-info/SOURCES.txt` & `cliconfig-0.2.0/cliconfig.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,42 +13,47 @@
 .github/workflows/pipy_deployment.yaml
 .github/workflows/pydocstyle.yaml
 .github/workflows/pylint.yaml
 .github/workflows/ruff.yaml
 .github/workflows/tests.yaml
 cliconfig/__init__.py
 cliconfig/_version.py
+cliconfig/build_config.py
 cliconfig/cli_parser.py
-cliconfig/config.py
+cliconfig/routines.py
+cliconfig/save_load.py
 cliconfig/show.py
 cliconfig.egg-info/PKG-INFO
 cliconfig.egg-info/SOURCES.txt
 cliconfig.egg-info/dependency_links.txt
 cliconfig.egg-info/requires.txt
 cliconfig.egg-info/top_level.txt
 docs/Makefile
 docs/cliconfig_api.rst
 docs/conf.py
 docs/contribute.md
+docs/edge_cases.md
 docs/index.rst
 docs/installation.md
 docs/license.md
 docs/make.bat
-docs/manipulate_configs.md
+docs/manipulate.md
 docs/quickstart.md
 docs/requirements.txt
 github_actions_utils/__init__.py
 github_actions_utils/color.py
 github_actions_utils/pydocstyle_manager.py
 github_actions_utils/pylint_manager.py
 github_actions_utils/pytest_manager.py
 licenses_tier/FLATTEN_DICT_LICENSE
 scripts/integration-tests.sh
 scripts/pre-commit-checks.sh
+tests/test_build_config.py
 tests/test_cli_parser.py
-tests/test_config.py
+tests/test_routines.py
+tests/test_save_load.py
 tests/test_show.py
 tests/configs/config1.yaml
 tests/configs/config2.yaml
 tests/configs/default1.yaml
 tests/configs/default2.yaml
 tests/integration/integration_show.py
```

### Comparing `cliconfig-0.1.4/docs/Makefile` & `cliconfig-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/docs/conf.py` & `cliconfig-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/docs/index.rst` & `cliconfig-0.2.0/docs/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 CLI Config
 ==========
 
-Merge your configs (optionally nested with dots) and set parameters from command
-line.
+Lightweight library that provides routines to merge your configs (optionally nested)
+and set parameters from command line. It also prevents you from adding new parameters
+if not desired. Finally, it provides helper routines to manage flatten dicts,
+unflatten (= nested) dicts or a mix of both, save config, load, display, etc.
 
 |PyPI version| |PythonVersion| |License|
 
 |Ruff_logo| |Black_logo|
 
 |Ruff| |Flake8| |Pydocstyle| |MyPy| |PyLint|
 
 |Tests| |Coverage| |Documentation Status|
 
-Access to a default config file in your project (configs are merged from left to right):
+Make a default config file in your project (configs are merged from left to right):
 
 .. code:: python
 
    # main.py
    from cliconfig import make_config, show_config
 
    config = make_config('default1.yaml', 'default2.yaml')  # it's a dict
 
-Then launch your script with additional config(s) file(s) and parameters:
+Then launch your script with additional config(s) file(s) and parameters.
+By default, these additional configs cannot add new parameters to the default config
+(for security and retro-compatibility reasons).
 
 .. code:: bash
 
-   python main.py --config exp1.yaml,exp2.yaml --param1 1 --subconfig.param2 'foo'
+   python main.py --config first.yaml,second.yaml --param1 1 --subconfig.param2 'foo'
 
 .. |PyPI version| image:: https://badge.fury.io/py/cliconfig.svg
    :target: https://badge.fury.io/py/cliconfig
 .. |PythonVersion| image:: https://img.shields.io/badge/python-3.7%20%7E%203.11-informational
 .. |License| image:: https://img.shields.io/github/license/valentingol/cliconfig?color=999
    :target: https://stringfixer.com/fr/MIT_license
 .. |Ruff_logo| image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
@@ -55,11 +59,12 @@
 
 .. toctree::
    :maxdepth: 4
    :caption: Contents:
 
    installation
    quickstart
-   manipulate_configs
+   edge_cases
+   manipulate
    cliconfig_api
    contribute
    license
```

### Comparing `cliconfig-0.1.4/docs/license.md` & `cliconfig-0.2.0/docs/license.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/docs/make.bat` & `cliconfig-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/docs/quickstart.md` & `cliconfig-0.2.0/docs/quickstart.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # Quick start
 
 First create a default config that can be split in multiple files that will be merged
-(from left to right in `make_config` function):
+(from left to right in `make_config` function). There is no limit of depth for the
+configurations parameters.
 
 ```yaml
-# default1.yaml
+---  # default1.yaml
 param1: 1
 param2: 0
 letters:
   letter1: a
   letter2: b
-```
 
-```yaml
-# default2.yaml
+---  # default2.yaml
 param1: 1
 param2: 2  # will override param2 from default1.yaml
 letters.letter3: c  # add a new parameter
 ```
 
 Now you can set up your program to use the config:
 
@@ -26,38 +25,38 @@
 from cliconfig import make_config, show_config
 
 config = make_config('default1.yaml', 'default2.yaml')
 show_config(config)
 ```
 
 Then add one or multiple additional config files that will override the default values.
-**Be careful, the additional config files cannot bring new parameters by default**.
-If you want to add new parameters (not advised for retro-compatibility, readability
-and security), you can add `allow_new_keys=True` in `make_config` function.
+**By default the additional config files cannot bring new parameters**.
+It is intended to prevent typos in the config files that would not be detected.
+It also improves the readability of the config files and the retro-compatibility.
+By the way, you can change this behavior with `allow_new_keys=True` in `make_config`
+(be careful).
 
 ```yaml
-# exp1.yaml
+---  # first.yaml
 letters:
   letter3: C
-```
 
-```yaml
-# exp2.yaml
+---  # second.yaml
 param1: -1
 letters.letter1: A
 ```
 
 Now you can launch the program with additional configurations and parameters.
 The additional configurations are indicated with `--config` (separate with comma,
 without space) and the parameters with `--<param_name>`. The default configuration
 will be merged with the additional configurations (from left to right), then the
 parameters will be set.
 
 ```bash
-python main.py --config exp1.yaml,exp2.yaml --param2=-2 --letters.letter2='B'
+python main.py --config first.yaml,second.yaml --param2=-2 --letters.letter2='B'
 ```
 
 Will show:
 
 ```text
 [CONFIG] Merge 2 default configs, 2 additional configs and 2 CLI parameter(s).
```

### Comparing `cliconfig-0.1.4/github_actions_utils/pydocstyle_manager.py` & `cliconfig-0.2.0/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/github_actions_utils/pylint_manager.py` & `cliconfig-0.2.0/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/github_actions_utils/pytest_manager.py` & `cliconfig-0.2.0/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/licenses_tier/FLATTEN_DICT_LICENSE` & `cliconfig-0.2.0/licenses_tier/FLATTEN_DICT_LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/pyproject.toml` & `cliconfig-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/scripts/pre-commit-checks.sh` & `cliconfig-0.2.0/scripts/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/tests/integration/integration_show.py` & `cliconfig-0.2.0/tests/integration/integration_show.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.4/tests/test_cli_parser.py` & `cliconfig-0.2.0/tests/test_cli_parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Test for cli_parser.py."""
 import pytest
 import pytest_check as check
 
-from cliconfig.cli_parser import parse
+from cliconfig.cli_parser import parse_cli
 
 
-def test_parse() -> None:
-    """Test for parse."""
-    config_paths, config_cli_params = parse(
+def test_parse_cli() -> None:
+    """Test for parse_cli."""
+    config_paths, config_cli_params = parse_cli(
         ["main.py", "--config", "config1.yaml,config2.yaml", "--a", "1", "--b=2"]
     )
     check.equal(config_paths, ["config1.yaml", "config2.yaml"])
     check.equal(config_cli_params, {"a": 1, "b": 2})
     b_str = "{'2': {'3': 4, '5': [6.3], '7': True, '8': Null, '9': [2, {'a': 1}]}}"
-    config_paths, config_cli_params = parse(["main.py", "--a='b=c'", f"--b={b_str}"])
+    config_paths, config_cli_params = parse_cli(
+        ["main.py", "--a='b=c'", f"--b={b_str}"]
+    )
     val = {
         "a": "b=c",
         "b": {"2": {"3": 4, "5": [6.3], "7": True, "8": None, "9": [2, {"a": 1}]}},
     }
     check.equal(config_paths, [])
     check.equal(config_cli_params, val)
     with pytest.raises(ValueError, match="Only one '--config ' argument is allowed.*"):
-        parse(["main.py", "--config", "config1.yaml", "--config", "config2.yaml"])
+        parse_cli(["main.py", "--config", "config1.yaml", "--config", "config2.yaml"])
```

### Comparing `cliconfig-0.1.4/tests/test_show.py` & `cliconfig-0.2.0/tests/test_show.py`

 * *Files identical despite different names*

