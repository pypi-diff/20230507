# Comparing `tmp/cliconfig-0.1.3.tar.gz` & `tmp/cliconfig-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-0.1.3.tar", last modified: Sun May  7 00:52:02 2023, max compression
+gzip compressed data, was "cliconfig-0.1.4.tar", last modified: Sun May  7 01:17:04 2023, max compression
```

## Comparing `cliconfig-0.1.3.tar` & `cliconfig-0.1.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.564725 cliconfig-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.556725 cliconfig-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.556725 cliconfig-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-07 00:51:41.000000 cliconfig-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 00:51:41.000000 cliconfig-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-07 00:52:02.560726 cliconfig-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-07 00:51:41.000000 cliconfig-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.560726 cliconfig-0.1.3/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-07 00:51:41.000000 cliconfig-0.1.3/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 00:52:02.000000 cliconfig-0.1.3/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-07 00:51:41.000000 cliconfig-0.1.3/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-05-07 00:51:41.000000 cliconfig-0.1.3/cliconfig/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-07 00:51:41.000000 cliconfig-0.1.3/cliconfig/show.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.560726 cliconfig-0.1.3/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-07 00:52:02.000000 cliconfig-0.1.3/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-07 00:52:02.000000 cliconfig-0.1.3/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 00:52:02.000000 cliconfig-0.1.3/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 00:52:02.000000 cliconfig-0.1.3/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 00:52:02.000000 cliconfig-0.1.3/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.560726 cliconfig-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/manipulate_configs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.560726 cliconfig-0.1.3/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 00:51:41.000000 cliconfig-0.1.3/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-07 00:51:41.000000 cliconfig-0.1.3/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-07 00:51:41.000000 cliconfig-0.1.3/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-07 00:51:41.000000 cliconfig-0.1.3/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-07 00:51:41.000000 cliconfig-0.1.3/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.560726 cliconfig-0.1.3/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-07 00:51:41.000000 cliconfig-0.1.3/licenses_tier/FLATTEN_DICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-07 00:51:41.000000 cliconfig-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-07 00:51:41.000000 cliconfig-0.1.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 00:51:41.000000 cliconfig-0.1.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.560726 cliconfig-0.1.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-07 00:51:41.000000 cliconfig-0.1.3/scripts/integration-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-07 00:51:41.000000 cliconfig-0.1.3/scripts/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 00:52:02.564725 cliconfig-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 00:51:41.000000 cliconfig-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.560726 cliconfig-0.1.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.560726 cliconfig-0.1.3/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 00:51:41.000000 cliconfig-0.1.3/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 00:51:41.000000 cliconfig-0.1.3/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 00:51:41.000000 cliconfig-0.1.3/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 00:51:41.000000 cliconfig-0.1.3/tests/configs/default2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.560726 cliconfig-0.1.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-07 00:51:41.000000 cliconfig-0.1.3/tests/integration/integration_show.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-07 00:51:41.000000 cliconfig-0.1.3/tests/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-07 00:51:41.000000 cliconfig-0.1.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-07 00:51:41.000000 cliconfig-0.1.3/tests/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.250839 cliconfig-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.242839 cliconfig-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.242839 cliconfig-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-07 01:16:42.000000 cliconfig-0.1.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-07 01:16:42.000000 cliconfig-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 01:16:42.000000 cliconfig-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-07 01:17:04.250839 cliconfig-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-07 01:16:42.000000 cliconfig-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.246839 cliconfig-0.1.4/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-07 01:16:42.000000 cliconfig-0.1.4/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 01:17:04.000000 cliconfig-0.1.4/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-07 01:16:42.000000 cliconfig-0.1.4/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-05-07 01:16:42.000000 cliconfig-0.1.4/cliconfig/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-07 01:16:42.000000 cliconfig-0.1.4/cliconfig/show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.246839 cliconfig-0.1.4/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-07 01:17:04.000000 cliconfig-0.1.4/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-07 01:17:04.000000 cliconfig-0.1.4/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 01:17:04.000000 cliconfig-0.1.4/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 01:17:04.000000 cliconfig-0.1.4/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 01:17:04.000000 cliconfig-0.1.4/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.246839 cliconfig-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/manipulate_configs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-07 01:16:42.000000 cliconfig-0.1.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.246839 cliconfig-0.1.4/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 01:16:42.000000 cliconfig-0.1.4/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-07 01:16:42.000000 cliconfig-0.1.4/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-07 01:16:42.000000 cliconfig-0.1.4/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-07 01:16:42.000000 cliconfig-0.1.4/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-07 01:16:42.000000 cliconfig-0.1.4/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.246839 cliconfig-0.1.4/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-07 01:16:42.000000 cliconfig-0.1.4/licenses_tier/FLATTEN_DICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-07 01:16:42.000000 cliconfig-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-07 01:16:42.000000 cliconfig-0.1.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 01:16:42.000000 cliconfig-0.1.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.246839 cliconfig-0.1.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-07 01:16:42.000000 cliconfig-0.1.4/scripts/integration-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-07 01:16:42.000000 cliconfig-0.1.4/scripts/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 01:17:04.250839 cliconfig-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 01:16:42.000000 cliconfig-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.250839 cliconfig-0.1.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.250839 cliconfig-0.1.4/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 01:16:42.000000 cliconfig-0.1.4/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 01:16:42.000000 cliconfig-0.1.4/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 01:16:42.000000 cliconfig-0.1.4/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 01:16:42.000000 cliconfig-0.1.4/tests/configs/default2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:17:04.250839 cliconfig-0.1.4/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-07 01:16:42.000000 cliconfig-0.1.4/tests/integration/integration_show.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-07 01:16:42.000000 cliconfig-0.1.4/tests/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-07 01:16:42.000000 cliconfig-0.1.4/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-07 01:16:42.000000 cliconfig-0.1.4/tests/test_show.py
```

### Comparing `cliconfig-0.1.3/.github/workflows/pipy_deployment.yaml` & `cliconfig-0.1.4/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/.github/workflows/pydocstyle.yaml` & `cliconfig-0.1.4/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/.github/workflows/pylint.yaml` & `cliconfig-0.1.4/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/.github/workflows/tests.yaml` & `cliconfig-0.1.4/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/.pylintrc` & `cliconfig-0.1.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/CONTRIBUTING.md` & `cliconfig-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/LICENSE` & `cliconfig-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/PKG-INFO` & `cliconfig-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.1.3
+Version: 0.1.4
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -114,15 +114,15 @@
         letter3: C
 ```
 
 Note that the configurations are native python dicts.
 
 ## Manipulate configs
 
-To merge configs, you can use `cliconfig.merge` function.
+To merge configs, you can use `cliconfig.merge_config` function.
 It supports unflatten (or nested) dicts like `{'a': {'b': 1, 'c': 2}}`,
 flatten dicts like `{'a.b': 1, 'a.c': 2}`, and a mix of both. The dicts will be flatten
 before merging. Sometimes you can have conflicts in flatten operation for instance with
 `{'a.b': 1, 'a': {'b': 2}}` that have two different values for `a.b`. That's why you
 can use a `priority` parameter to choose which value to keep before merging.
 
 You can also save, load and display configs with `cliconfig.save_config`,
@@ -141,15 +141,15 @@
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ### Todo
 
 To do:
 
 - [ ] add json and ini support
-- [ ] avoid changing keys order in merge
+- [ ] avoid changing keys order in merge_config
 
 ## License
 
 Copyright (C) 2023  Valentin Goldité
 
 This program is free software: you can redistribute it and/or modify it under the
 terms of the [MIT License](LICENSE). This program is distributed in the hope that
```

### Comparing `cliconfig-0.1.3/README.md` & `cliconfig-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         letter3: C
 ```
 
 Note that the configurations are native python dicts.
 
 ## Manipulate configs
 
-To merge configs, you can use `cliconfig.merge` function.
+To merge configs, you can use `cliconfig.merge_config` function.
 It supports unflatten (or nested) dicts like `{'a': {'b': 1, 'c': 2}}`,
 flatten dicts like `{'a.b': 1, 'a.c': 2}`, and a mix of both. The dicts will be flatten
 before merging. Sometimes you can have conflicts in flatten operation for instance with
 `{'a.b': 1, 'a': {'b': 2}}` that have two different values for `a.b`. That's why you
 can use a `priority` parameter to choose which value to keep before merging.
 
 You can also save, load and display configs with `cliconfig.save_config`,
@@ -129,15 +129,15 @@
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ### Todo
 
 To do:
 
 - [ ] add json and ini support
-- [ ] avoid changing keys order in merge
+- [ ] avoid changing keys order in merge_config
 
 ## License
 
 Copyright (C) 2023  Valentin Goldité
 
 This program is free software: you can redistribute it and/or modify it under the
 terms of the [MIT License](LICENSE). This program is distributed in the hope that
```

### Comparing `cliconfig-0.1.3/cliconfig/__init__.py` & `cliconfig-0.1.4/cliconfig/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,19 +9,19 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
     This project is free to use for COMMERCIAL USE, MODIFICATION,
     DISTRIBUTION and PRIVATE USE as long as the original license is
     include as well as this copy right notice.
 """
 # pylint: disable=wrong-import-position
 from cliconfig._version import __version__, __version_tuple__
-from cliconfig.config import load_config, make_config, merge, save_config
+from cliconfig.config import load_config, make_config, merge_config, save_config
 from cliconfig.show import show_config
 
 __all__ = [
     "__version__",
     "__version_tuple__",
     "load_config",
     "make_config",
-    "merge",
+    "merge_config",
     "save_config",
     "show_config",
 ]
```

### Comparing `cliconfig-0.1.3/cliconfig/cli_parser.py` & `cliconfig-0.1.4/cliconfig/cli_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,13 +43,7 @@
                 i += 2
             key = key[2:]
             value = yaml.safe_load(value_str)
             config_cli_params[key] = value
         else:
             i += 1
     return config_paths, config_cli_params
-
-
-if __name__ == "__main__":
-    import sys
-
-    print(sys.argv)
```

### Comparing `cliconfig-0.1.3/cliconfig/config.py` & `cliconfig-0.1.4/cliconfig/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,25 +38,25 @@
         f"[CONFIG] Merge {len(default_configs)} default configs, "
         f"{len(config_paths)} additional configs and "
         f"{len(config_cli_params)} CLI parameter(s)."
     )
     for default_config_path in default_configs:
         with open(default_config_path, "r", encoding="utf-8") as cfg_file:
             default_config = yaml.safe_load(cfg_file)
-        config = merge(config, default_config, allow_new_keys=True)
+        config = merge_config(config, default_config, allow_new_keys=True)
 
     for config_path in config_paths:
         with open(config_path, "r", encoding="utf-8") as cfg_file:
             additional_config = yaml.safe_load(cfg_file)
-        config = merge(config, additional_config, allow_new_keys=allow_new_keys)
-    config = merge(config, config_cli_params, allow_new_keys=allow_new_keys)
+        config = merge_config(config, additional_config, allow_new_keys=allow_new_keys)
+    config = merge_config(config, config_cli_params, allow_new_keys=allow_new_keys)
     return config
 
 
-def merge(
+def merge_config(
     config1: Dict[str, Any],
     config2: Dict[str, Any],
     *,
     allow_new_keys: bool = True,
     priority: str = "flat",
 ) -> Dict[str, Any]:
     """Merge config2 into config1.
@@ -68,24 +68,38 @@
     config2 : Dict[str, Any]
         The second configuration to merge into config1.
     allow_new_keys : bool, optional
         If True, new keys (that are not in config1) are allowed in config2.
         By default True.
     priority : str, optional
         One of 'flat' or 'unflat'.
-        If 'flat', keys with dots at the root like `a.b: ...` (flat keys) have
-        priority over unflat keys like `'a(): {'b': ...}` when there are conflicts.
+        If 'flat', keys with dots at the root like `{'a.b': ...}` (flat keys) have
+        priority over unflat keys like `{'a': {'b': ...}}` when there are conflicts.
         If 'unflat', unflat keys have priority over flat keys when there are conflicts.
 
     Raises
     ------
     ValueError
         If priority is not one of 'flat', 'unflat' or 'order'.
     ValueError
         If allow_new_keys is False and config2 has new keys that are not in config1.
+
+    Examples
+    --------
+    ::
+
+        >>> merge_config({'a.b': 1, 'a': {'b': 2}}, {'c': 3}, allow_new_keys=True,
+                         priority='flat')
+        {'a.b': 1, 'c': 3}
+        >>> merge_config({'a.b': 1, 'a': {'b': 2}}, {'c': 3}, allow_new_keys=True,
+                         priority='unflat')
+        {'a.b': 2, 'c': 3}
+        >>> merge_config({'a.b': 1, 'a': {'b': 2}}, {'c': 3}, allow_new_keys=False,
+                         priority='unflat')
+        ValueError: New parameter found 'c' that is not in the original config.
     """
     if priority in ("flat", "unflat"):
         # Split flat and unflat keys
         config1_flat = dict(filter(lambda x: "." in x[0], config1.items()))
         config1_unflat = dict(filter(lambda x: "." not in x[0], config1.items()))
         config2_flat = dict(filter(lambda x: "." in x[0], config2.items()))
         config2_unflat = dict(filter(lambda x: "." not in x[0], config2.items()))
@@ -106,15 +120,15 @@
             "'flat', 'unflat' or 'order'."
         )
     if not allow_new_keys:
         # Check that there are no new keys in config2
         for key in config2_flat:
             if key not in config1_flat.keys():
                 raise ValueError(
-                    f"New parameter '{key}' found that is not in the original config."
+                    f"New parameter found '{key}' that is not in the original config."
                 )
     # Merge flat configs
     flat_config = {**config1_flat, **config2_flat}
     # Unflats config
     config = unflatten(flat_config, splitter="dot")
     return config
 
@@ -167,12 +181,12 @@
         The config merged from default configs and the loaded config.
     """
     config: Dict[str, Any] = {}
     if default_configs:
         for config_path in default_configs:
             with open(config_path, "r", encoding="utf-8") as cfg_file:
                 default_config = yaml.safe_load(cfg_file)
-            config = merge(config, default_config, allow_new_keys=True)
+            config = merge_config(config, default_config, allow_new_keys=True)
     with open(path, "r", encoding="utf-8") as cfg_file:
         loaded_config = yaml.safe_load(cfg_file)
-    config = merge(config, loaded_config, allow_new_keys=allow_new_keys)
+    config = merge_config(config, loaded_config, allow_new_keys=allow_new_keys)
     return config
```

### Comparing `cliconfig-0.1.3/cliconfig/show.py` & `cliconfig-0.1.4/cliconfig/show.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/cliconfig.egg-info/PKG-INFO` & `cliconfig-0.1.4/cliconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.1.3
+Version: 0.1.4
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -114,15 +114,15 @@
         letter3: C
 ```
 
 Note that the configurations are native python dicts.
 
 ## Manipulate configs
 
-To merge configs, you can use `cliconfig.merge` function.
+To merge configs, you can use `cliconfig.merge_config` function.
 It supports unflatten (or nested) dicts like `{'a': {'b': 1, 'c': 2}}`,
 flatten dicts like `{'a.b': 1, 'a.c': 2}`, and a mix of both. The dicts will be flatten
 before merging. Sometimes you can have conflicts in flatten operation for instance with
 `{'a.b': 1, 'a': {'b': 2}}` that have two different values for `a.b`. That's why you
 can use a `priority` parameter to choose which value to keep before merging.
 
 You can also save, load and display configs with `cliconfig.save_config`,
@@ -141,15 +141,15 @@
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ### Todo
 
 To do:
 
 - [ ] add json and ini support
-- [ ] avoid changing keys order in merge
+- [ ] avoid changing keys order in merge_config
 
 ## License
 
 Copyright (C) 2023  Valentin Goldité
 
 This program is free software: you can redistribute it and/or modify it under the
 terms of the [MIT License](LICENSE). This program is distributed in the hope that
```

### Comparing `cliconfig-0.1.3/cliconfig.egg-info/SOURCES.txt` & `cliconfig-0.1.4/cliconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/docs/Makefile` & `cliconfig-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/docs/conf.py` & `cliconfig-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/docs/index.rst` & `cliconfig-0.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/docs/license.md` & `cliconfig-0.1.4/docs/license.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/docs/make.bat` & `cliconfig-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/docs/manipulate_configs.md` & `cliconfig-0.1.4/docs/manipulate_configs.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Manipulate configs
 
-To merge configs, you can use `cliconfig.merge` function.
+To merge configs, you can use `cliconfig.merge_config` function.
 It supports unflatten (or nested) dicts like `{'a': {'b': 1, 'c': 2}}`,
 flatten dicts like `{'a.b': 1, 'a.c': 2}`, and a mix of both. The dicts will be flatten
 before merging. Sometimes you can have conflicts in flatten operation for instance with
 `{'a.b': 1, 'a': {'b': 2}}` that have two different values for `a.b`. That's why you
 can use a `priority` parameter to choose which value to keep before merging.
 
 You can also save, load and display configs with `cliconfig.save_config`,
```

### Comparing `cliconfig-0.1.3/docs/quickstart.md` & `cliconfig-0.1.4/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/github_actions_utils/pydocstyle_manager.py` & `cliconfig-0.1.4/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/github_actions_utils/pylint_manager.py` & `cliconfig-0.1.4/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/github_actions_utils/pytest_manager.py` & `cliconfig-0.1.4/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/licenses_tier/FLATTEN_DICT_LICENSE` & `cliconfig-0.1.4/licenses_tier/FLATTEN_DICT_LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/pyproject.toml` & `cliconfig-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/scripts/pre-commit-checks.sh` & `cliconfig-0.1.4/scripts/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/tests/integration/integration_show.py` & `cliconfig-0.1.4/tests/integration/integration_show.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/tests/test_cli_parser.py` & `cliconfig-0.1.4/tests/test_cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.3/tests/test_config.py` & `cliconfig-0.1.4/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 import os
 import shutil
 import sys
 
 import pytest
 import pytest_check as check
 
-from cliconfig import load_config, make_config, merge, save_config
+from cliconfig import load_config, make_config, merge_config, save_config
 
 
-def test_merge() -> None:
-    """Test merge."""
+def test_merge_config() -> None:
+    """Test merge_config."""
     config1 = {"a.b": 1, "a": {"b": 2, "c": 3}}
     config2 = {"a": {"c": 1}, "a.d": 6}
-    config = merge(config1, config2, allow_new_keys=True, priority="flat")
+    config = merge_config(config1, config2, allow_new_keys=True, priority="flat")
     check.equal(config, {"a": {"b": 1, "c": 1, "d": 6}})
-    config = merge(config1, config2, allow_new_keys=True, priority="unflat")
+    config = merge_config(config1, config2, allow_new_keys=True, priority="unflat")
     check.equal(config, {"a": {"b": 2, "c": 1, "d": 6}})
-    with pytest.raises(ValueError, match="New parameter 'a.d' found.*"):
-        merge(config1, config2, allow_new_keys=False)
+    with pytest.raises(ValueError, match="New parameter found 'a.d'.*"):
+        merge_config(config1, config2, allow_new_keys=False)
     with pytest.raises(ValueError, match="Unknown dot_prior 'UNKONWN'.*"):
-        merge(config1, config2, allow_new_keys=True, priority="UNKONWN")
+        merge_config(config1, config2, allow_new_keys=True, priority="UNKONWN")
 
 
 def test_make_config(capsys: pytest.CaptureFixture) -> None:
     """Test make_config."""
     sys_argv = sys.argv.copy()
     sys.argv = [
         "tests/test_make_config.py.py",
@@ -115,15 +115,15 @@
             "letter4": "d",
         },
     }
     check.equal(config, expected_config)
     # Additional keys when allow_new_keys=False
     config = {"param4": 0}
     save_config(config, "tests/tmp/config3.yaml")
-    with pytest.raises(ValueError, match="New parameter 'param4' found.*"):
+    with pytest.raises(ValueError, match="New parameter found 'param4'.*"):
         load_config(
             "tests/tmp/config3.yaml",
             default_configs=[
                 "tests/configs/default1.yaml",
                 "tests/configs/default2.yaml",
             ],
             allow_new_keys=False,
```

### Comparing `cliconfig-0.1.3/tests/test_show.py` & `cliconfig-0.1.4/tests/test_show.py`

 * *Files identical despite different names*

