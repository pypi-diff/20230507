# Comparing `tmp/cliconfig-0.1.2.tar.gz` & `tmp/cliconfig-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-0.1.2.tar", last modified: Sun May  7 00:33:53 2023, max compression
+gzip compressed data, was "cliconfig-0.1.3.tar", last modified: Sun May  7 00:52:02 2023, max compression
```

## Comparing `cliconfig-0.1.2.tar` & `cliconfig-0.1.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.653164 cliconfig-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.645164 cliconfig-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.649164 cliconfig-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-07 00:33:36.000000 cliconfig-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 00:33:36.000000 cliconfig-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-07 00:33:53.653164 cliconfig-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-07 00:33:36.000000 cliconfig-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.649164 cliconfig-0.1.2/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-07 00:33:36.000000 cliconfig-0.1.2/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 00:33:53.000000 cliconfig-0.1.2/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-07 00:33:36.000000 cliconfig-0.1.2/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-05-07 00:33:36.000000 cliconfig-0.1.2/cliconfig/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-07 00:33:36.000000 cliconfig-0.1.2/cliconfig/show.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.649164 cliconfig-0.1.2/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-07 00:33:53.000000 cliconfig-0.1.2/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-07 00:33:53.000000 cliconfig-0.1.2/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 00:33:53.000000 cliconfig-0.1.2/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 00:33:53.000000 cliconfig-0.1.2/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 00:33:53.000000 cliconfig-0.1.2/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.649164 cliconfig-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/manipulate_configs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.649164 cliconfig-0.1.2/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 00:33:36.000000 cliconfig-0.1.2/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-07 00:33:36.000000 cliconfig-0.1.2/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-07 00:33:36.000000 cliconfig-0.1.2/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-07 00:33:36.000000 cliconfig-0.1.2/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-07 00:33:36.000000 cliconfig-0.1.2/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.649164 cliconfig-0.1.2/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-07 00:33:36.000000 cliconfig-0.1.2/licenses_tier/FLATDICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-07 00:33:36.000000 cliconfig-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-07 00:33:36.000000 cliconfig-0.1.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 00:33:36.000000 cliconfig-0.1.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.649164 cliconfig-0.1.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-07 00:33:36.000000 cliconfig-0.1.2/scripts/integration-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-07 00:33:36.000000 cliconfig-0.1.2/scripts/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 00:33:53.653164 cliconfig-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 00:33:36.000000 cliconfig-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.653164 cliconfig-0.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.653164 cliconfig-0.1.2/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 00:33:36.000000 cliconfig-0.1.2/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 00:33:36.000000 cliconfig-0.1.2/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 00:33:36.000000 cliconfig-0.1.2/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 00:33:36.000000 cliconfig-0.1.2/tests/configs/default2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.653164 cliconfig-0.1.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-07 00:33:36.000000 cliconfig-0.1.2/tests/integration/integration_show.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-07 00:33:36.000000 cliconfig-0.1.2/tests/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-07 00:33:36.000000 cliconfig-0.1.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-07 00:33:36.000000 cliconfig-0.1.2/tests/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.564725 cliconfig-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.556725 cliconfig-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.556725 cliconfig-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-07 00:51:41.000000 cliconfig-0.1.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-07 00:51:41.000000 cliconfig-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 00:51:41.000000 cliconfig-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-07 00:52:02.560726 cliconfig-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-07 00:51:41.000000 cliconfig-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.560726 cliconfig-0.1.3/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-07 00:51:41.000000 cliconfig-0.1.3/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 00:52:02.000000 cliconfig-0.1.3/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-07 00:51:41.000000 cliconfig-0.1.3/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-05-07 00:51:41.000000 cliconfig-0.1.3/cliconfig/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-07 00:51:41.000000 cliconfig-0.1.3/cliconfig/show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.560726 cliconfig-0.1.3/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-07 00:52:02.000000 cliconfig-0.1.3/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-07 00:52:02.000000 cliconfig-0.1.3/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 00:52:02.000000 cliconfig-0.1.3/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 00:52:02.000000 cliconfig-0.1.3/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 00:52:02.000000 cliconfig-0.1.3/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.560726 cliconfig-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/manipulate_configs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-07 00:51:41.000000 cliconfig-0.1.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.560726 cliconfig-0.1.3/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 00:51:41.000000 cliconfig-0.1.3/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-07 00:51:41.000000 cliconfig-0.1.3/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-07 00:51:41.000000 cliconfig-0.1.3/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-07 00:51:41.000000 cliconfig-0.1.3/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-07 00:51:41.000000 cliconfig-0.1.3/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.560726 cliconfig-0.1.3/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-07 00:51:41.000000 cliconfig-0.1.3/licenses_tier/FLATTEN_DICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-07 00:51:41.000000 cliconfig-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-07 00:51:41.000000 cliconfig-0.1.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 00:51:41.000000 cliconfig-0.1.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.560726 cliconfig-0.1.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-07 00:51:41.000000 cliconfig-0.1.3/scripts/integration-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-07 00:51:41.000000 cliconfig-0.1.3/scripts/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 00:52:02.564725 cliconfig-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 00:51:41.000000 cliconfig-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.560726 cliconfig-0.1.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.560726 cliconfig-0.1.3/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 00:51:41.000000 cliconfig-0.1.3/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 00:51:41.000000 cliconfig-0.1.3/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 00:51:41.000000 cliconfig-0.1.3/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 00:51:41.000000 cliconfig-0.1.3/tests/configs/default2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:52:02.560726 cliconfig-0.1.3/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-07 00:51:41.000000 cliconfig-0.1.3/tests/integration/integration_show.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-07 00:51:41.000000 cliconfig-0.1.3/tests/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-07 00:51:41.000000 cliconfig-0.1.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-07 00:51:41.000000 cliconfig-0.1.3/tests/test_show.py
```

### Comparing `cliconfig-0.1.2/.github/workflows/pipy_deployment.yaml` & `cliconfig-0.1.3/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/.github/workflows/pydocstyle.yaml` & `cliconfig-0.1.3/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/.github/workflows/pylint.yaml` & `cliconfig-0.1.3/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/.github/workflows/tests.yaml` & `cliconfig-0.1.3/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/.pylintrc` & `cliconfig-0.1.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/CONTRIBUTING.md` & `cliconfig-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/LICENSE` & `cliconfig-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/PKG-INFO` & `cliconfig-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.1.2
+Version: 0.1.3
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CLI Config
 
 Lightweight library to merge your configs (optionally nested) and set parameters
 from command line.
 
-## Documentation :memo: [here](cliconfig.readthedocs.io)
+## Documentation :memo: [here](https://cliconfig.readthedocs.io/en/stable)
 
 [![PyPI version](https://badge.fury.io/py/cliconfig.svg)](https://badge.fury.io/py/cliconfig)
 ![PythonVersion](https://img.shields.io/badge/python-3.7%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/cliconfig?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `cliconfig-0.1.2/README.md` & `cliconfig-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # CLI Config
 
 Lightweight library to merge your configs (optionally nested) and set parameters
 from command line.
 
-## Documentation :memo: [here](cliconfig.readthedocs.io)
+## Documentation :memo: [here](https://cliconfig.readthedocs.io/en/stable)
 
 [![PyPI version](https://badge.fury.io/py/cliconfig.svg)](https://badge.fury.io/py/cliconfig)
 ![PythonVersion](https://img.shields.io/badge/python-3.7%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/cliconfig?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `cliconfig-0.1.2/cliconfig/__init__.py` & `cliconfig-0.1.3/cliconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/cliconfig/cli_parser.py` & `cliconfig-0.1.3/cliconfig/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/cliconfig/config.py` & `cliconfig-0.1.3/cliconfig/config.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/cliconfig/show.py` & `cliconfig-0.1.3/cliconfig/show.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/cliconfig.egg-info/PKG-INFO` & `cliconfig-0.1.3/cliconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.1.2
+Version: 0.1.3
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CLI Config
 
 Lightweight library to merge your configs (optionally nested) and set parameters
 from command line.
 
-## Documentation :memo: [here](cliconfig.readthedocs.io)
+## Documentation :memo: [here](https://cliconfig.readthedocs.io/en/stable)
 
 [![PyPI version](https://badge.fury.io/py/cliconfig.svg)](https://badge.fury.io/py/cliconfig)
 ![PythonVersion](https://img.shields.io/badge/python-3.7%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/cliconfig?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `cliconfig-0.1.2/cliconfig.egg-info/SOURCES.txt` & `cliconfig-0.1.3/cliconfig.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 docs/quickstart.md
 docs/requirements.txt
 github_actions_utils/__init__.py
 github_actions_utils/color.py
 github_actions_utils/pydocstyle_manager.py
 github_actions_utils/pylint_manager.py
 github_actions_utils/pytest_manager.py
-licenses_tier/FLATDICT_LICENSE
+licenses_tier/FLATTEN_DICT_LICENSE
 scripts/integration-tests.sh
 scripts/pre-commit-checks.sh
 tests/test_cli_parser.py
 tests/test_config.py
 tests/test_show.py
 tests/configs/config1.yaml
 tests/configs/config2.yaml
```

### Comparing `cliconfig-0.1.2/docs/Makefile` & `cliconfig-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/docs/conf.py` & `cliconfig-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/docs/index.rst` & `cliconfig-0.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/docs/license.md` & `cliconfig-0.1.3/docs/license.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/docs/make.bat` & `cliconfig-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/docs/manipulate_configs.md` & `cliconfig-0.1.3/docs/manipulate_configs.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/docs/quickstart.md` & `cliconfig-0.1.3/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/github_actions_utils/pydocstyle_manager.py` & `cliconfig-0.1.3/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/github_actions_utils/pylint_manager.py` & `cliconfig-0.1.3/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/github_actions_utils/pytest_manager.py` & `cliconfig-0.1.3/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/pyproject.toml` & `cliconfig-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/scripts/pre-commit-checks.sh` & `cliconfig-0.1.3/scripts/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/tests/integration/integration_show.py` & `cliconfig-0.1.3/tests/integration/integration_show.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/tests/test_cli_parser.py` & `cliconfig-0.1.3/tests/test_cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/tests/test_config.py` & `cliconfig-0.1.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.2/tests/test_show.py` & `cliconfig-0.1.3/tests/test_show.py`

 * *Files identical despite different names*

