# Comparing `tmp/cliconfig-0.1.1.tar.gz` & `tmp/cliconfig-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-0.1.1.tar", last modified: Sun May  7 00:18:41 2023, max compression
+gzip compressed data, was "cliconfig-0.1.2.tar", last modified: Sun May  7 00:33:53 2023, max compression
```

## Comparing `cliconfig-0.1.1.tar` & `cliconfig-0.1.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:18:41.019494 cliconfig-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 00:18:17.000000 cliconfig-0.1.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:18:41.011494 cliconfig-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:18:41.015494 cliconfig-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-07 00:18:17.000000 cliconfig-0.1.1/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-07 00:18:17.000000 cliconfig-0.1.1/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-07 00:18:17.000000 cliconfig-0.1.1/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 00:18:17.000000 cliconfig-0.1.1/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-07 00:18:17.000000 cliconfig-0.1.1/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-07 00:18:17.000000 cliconfig-0.1.1/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 00:18:17.000000 cliconfig-0.1.1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-07 00:18:17.000000 cliconfig-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-07 00:18:17.000000 cliconfig-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-07 00:18:17.000000 cliconfig-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 00:18:17.000000 cliconfig-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-05-07 00:18:41.019494 cliconfig-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-05-07 00:18:17.000000 cliconfig-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:18:41.015494 cliconfig-0.1.1/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-07 00:18:17.000000 cliconfig-0.1.1/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 00:18:40.000000 cliconfig-0.1.1/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-07 00:18:17.000000 cliconfig-0.1.1/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-07 00:18:17.000000 cliconfig-0.1.1/cliconfig/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-07 00:18:17.000000 cliconfig-0.1.1/cliconfig/show.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:18:41.015494 cliconfig-0.1.1/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-05-07 00:18:40.000000 cliconfig-0.1.1/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-07 00:18:41.000000 cliconfig-0.1.1/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 00:18:40.000000 cliconfig-0.1.1/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-07 00:18:40.000000 cliconfig-0.1.1/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 00:18:40.000000 cliconfig-0.1.1/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:18:41.015494 cliconfig-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-07 00:18:17.000000 cliconfig-0.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-07 00:18:17.000000 cliconfig-0.1.1/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-07 00:18:17.000000 cliconfig-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-07 00:18:17.000000 cliconfig-0.1.1/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-07 00:18:17.000000 cliconfig-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-07 00:18:17.000000 cliconfig-0.1.1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-07 00:18:17.000000 cliconfig-0.1.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-07 00:18:17.000000 cliconfig-0.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-07 00:18:17.000000 cliconfig-0.1.1/docs/manipulate_configs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-07 00:18:17.000000 cliconfig-0.1.1/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-07 00:18:17.000000 cliconfig-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:18:41.015494 cliconfig-0.1.1/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 00:18:17.000000 cliconfig-0.1.1/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-07 00:18:17.000000 cliconfig-0.1.1/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-07 00:18:17.000000 cliconfig-0.1.1/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-07 00:18:17.000000 cliconfig-0.1.1/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-07 00:18:17.000000 cliconfig-0.1.1/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:18:41.015494 cliconfig-0.1.1/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-07 00:18:17.000000 cliconfig-0.1.1/licenses_tier/FLATDICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-07 00:18:17.000000 cliconfig-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-07 00:18:17.000000 cliconfig-0.1.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-07 00:18:17.000000 cliconfig-0.1.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:18:41.019494 cliconfig-0.1.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-07 00:18:17.000000 cliconfig-0.1.1/scripts/integration-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-07 00:18:17.000000 cliconfig-0.1.1/scripts/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 00:18:41.019494 cliconfig-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 00:18:17.000000 cliconfig-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:18:41.019494 cliconfig-0.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:18:41.019494 cliconfig-0.1.1/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 00:18:17.000000 cliconfig-0.1.1/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 00:18:17.000000 cliconfig-0.1.1/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 00:18:17.000000 cliconfig-0.1.1/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 00:18:17.000000 cliconfig-0.1.1/tests/configs/default2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:18:41.019494 cliconfig-0.1.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-07 00:18:17.000000 cliconfig-0.1.1/tests/integration/integration_show.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-07 00:18:17.000000 cliconfig-0.1.1/tests/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-07 00:18:17.000000 cliconfig-0.1.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-07 00:18:17.000000 cliconfig-0.1.1/tests/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.653164 cliconfig-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.645164 cliconfig-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.649164 cliconfig-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-07 00:33:36.000000 cliconfig-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-07 00:33:36.000000 cliconfig-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 00:33:36.000000 cliconfig-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-07 00:33:53.653164 cliconfig-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-07 00:33:36.000000 cliconfig-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.649164 cliconfig-0.1.2/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-07 00:33:36.000000 cliconfig-0.1.2/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 00:33:53.000000 cliconfig-0.1.2/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-07 00:33:36.000000 cliconfig-0.1.2/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-05-07 00:33:36.000000 cliconfig-0.1.2/cliconfig/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-07 00:33:36.000000 cliconfig-0.1.2/cliconfig/show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.649164 cliconfig-0.1.2/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-07 00:33:53.000000 cliconfig-0.1.2/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-07 00:33:53.000000 cliconfig-0.1.2/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 00:33:53.000000 cliconfig-0.1.2/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 00:33:53.000000 cliconfig-0.1.2/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 00:33:53.000000 cliconfig-0.1.2/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.649164 cliconfig-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/manipulate_configs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-07 00:33:36.000000 cliconfig-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.649164 cliconfig-0.1.2/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 00:33:36.000000 cliconfig-0.1.2/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-07 00:33:36.000000 cliconfig-0.1.2/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-07 00:33:36.000000 cliconfig-0.1.2/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-07 00:33:36.000000 cliconfig-0.1.2/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-07 00:33:36.000000 cliconfig-0.1.2/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.649164 cliconfig-0.1.2/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-07 00:33:36.000000 cliconfig-0.1.2/licenses_tier/FLATDICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-07 00:33:36.000000 cliconfig-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-07 00:33:36.000000 cliconfig-0.1.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 00:33:36.000000 cliconfig-0.1.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.649164 cliconfig-0.1.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-07 00:33:36.000000 cliconfig-0.1.2/scripts/integration-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-07 00:33:36.000000 cliconfig-0.1.2/scripts/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 00:33:53.653164 cliconfig-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 00:33:36.000000 cliconfig-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.653164 cliconfig-0.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.653164 cliconfig-0.1.2/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 00:33:36.000000 cliconfig-0.1.2/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 00:33:36.000000 cliconfig-0.1.2/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 00:33:36.000000 cliconfig-0.1.2/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 00:33:36.000000 cliconfig-0.1.2/tests/configs/default2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:33:53.653164 cliconfig-0.1.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-07 00:33:36.000000 cliconfig-0.1.2/tests/integration/integration_show.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-07 00:33:36.000000 cliconfig-0.1.2/tests/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-07 00:33:36.000000 cliconfig-0.1.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-07 00:33:36.000000 cliconfig-0.1.2/tests/test_show.py
```

### Comparing `cliconfig-0.1.1/.github/workflows/pipy_deployment.yaml` & `cliconfig-0.1.2/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/.github/workflows/pydocstyle.yaml` & `cliconfig-0.1.2/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/.github/workflows/pylint.yaml` & `cliconfig-0.1.2/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/.github/workflows/tests.yaml` & `cliconfig-0.1.2/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/.pylintrc` & `cliconfig-0.1.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/CONTRIBUTING.md` & `cliconfig-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/LICENSE` & `cliconfig-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/PKG-INFO` & `cliconfig-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.1.1
+Version: 0.1.2
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
 
+## Documentation :memo: [here](cliconfig.readthedocs.io)
+
 [![PyPI version](https://badge.fury.io/py/cliconfig.svg)](https://badge.fury.io/py/cliconfig)
 ![PythonVersion](https://img.shields.io/badge/python-3.7%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/cliconfig?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `cliconfig-0.1.1/README.md` & `cliconfig-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # CLI Config
 
 Lightweight library to merge your configs (optionally nested) and set parameters
 from command line.
 
+## Documentation :memo: [here](cliconfig.readthedocs.io)
+
 [![PyPI version](https://badge.fury.io/py/cliconfig.svg)](https://badge.fury.io/py/cliconfig)
 ![PythonVersion](https://img.shields.io/badge/python-3.7%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/cliconfig?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `cliconfig-0.1.1/cliconfig/__init__.py` & `cliconfig-0.1.2/cliconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/cliconfig/cli_parser.py` & `cliconfig-0.1.2/cliconfig/cli_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,35 +20,36 @@
         Dictionary of parameters from CLI.
     """
     config_cli_params: Dict[str, Any] = {}
     config_paths: List[str] = []
     i = 0
     while i < len(sys_argv):
         elem = sys_argv[i]
-        if elem == '--config':
+        if elem == "--config":
             if config_paths:
                 raise ValueError(
                     "Only one '--config ' argument is allowed in CLI (used for "
                     "config merging). If you have a subconfig called 'config', "
                     "use '--config=<val>' (with an '=')."
                 )
-            config_paths = sys_argv[i + 1].split(',')
+            config_paths = sys_argv[i + 1].split(",")
             i += 2
 
-        elif elem.startswith('--'):
-            if '=' in elem:
-                key, value_str = elem.split('=', maxsplit=1)
+        elif elem.startswith("--"):
+            if "=" in elem:
+                key, value_str = elem.split("=", maxsplit=1)
                 i += 1
             else:
                 key, value_str = elem, sys_argv[i + 1]
                 i += 2
             key = key[2:]
             value = yaml.safe_load(value_str)
             config_cli_params[key] = value
         else:
             i += 1
     return config_paths, config_cli_params
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import sys
+
     print(sys.argv)
```

### Comparing `cliconfig-0.1.1/cliconfig/config.py` & `cliconfig-0.1.2/cliconfig/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 
 import yaml
 from flatten_dict import flatten, unflatten
 
 from cliconfig.cli_parser import parse
 
 
-def make_config(
-    *default_configs: str,
-    allow_new_keys: bool = False
-) -> Dict[str, Any]:
+def make_config(*default_configs: str, allow_new_keys: bool = False) -> Dict[str, Any]:
     """Make a config from default configs and CLI arguments.
 
     Parameters
     ----------
     default_configs : Tuple[str]
         Paths to default configs. They are merged in order and new keys
         are allowed.
@@ -33,36 +30,38 @@
     Returns
     -------
     config : Dict[str, Any]
         The merged config.
     """
     config: Dict[str, Any] = {}
     config_paths, config_cli_params = parse(sys.argv)
-    print(f"[CONFIG] Merge {len(default_configs)} default configs, "
-          f"{len(config_paths)} additional configs and "
-          f"{len(config_cli_params)} CLI parameter(s).")
+    print(
+        f"[CONFIG] Merge {len(default_configs)} default configs, "
+        f"{len(config_paths)} additional configs and "
+        f"{len(config_cli_params)} CLI parameter(s)."
+    )
     for default_config_path in default_configs:
-        with open(default_config_path, 'r', encoding='utf-8') as cfg_file:
+        with open(default_config_path, "r", encoding="utf-8") as cfg_file:
             default_config = yaml.safe_load(cfg_file)
         config = merge(config, default_config, allow_new_keys=True)
 
     for config_path in config_paths:
-        with open(config_path, 'r', encoding='utf-8') as cfg_file:
+        with open(config_path, "r", encoding="utf-8") as cfg_file:
             additional_config = yaml.safe_load(cfg_file)
         config = merge(config, additional_config, allow_new_keys=allow_new_keys)
     config = merge(config, config_cli_params, allow_new_keys=allow_new_keys)
     return config
 
 
 def merge(
     config1: Dict[str, Any],
     config2: Dict[str, Any],
     *,
     allow_new_keys: bool = True,
-    priority: str = 'flat',
+    priority: str = "flat",
 ) -> Dict[str, Any]:
     """Merge config2 into config1.
 
     Parameters
     ----------
     config1 : Dict[str, Any]
         The first configuration.
@@ -80,45 +79,47 @@
     Raises
     ------
     ValueError
         If priority is not one of 'flat', 'unflat' or 'order'.
     ValueError
         If allow_new_keys is False and config2 has new keys that are not in config1.
     """
-    if priority in ('flat', 'unflat'):
+    if priority in ("flat", "unflat"):
         # Split flat and unflat keys
-        config1_flat = dict(filter(lambda x: '.' in x[0], config1.items()))
-        config1_unflat = dict(filter(lambda x: '.' not in x[0], config1.items()))
-        config2_flat = dict(filter(lambda x: '.' in x[0], config2.items()))
-        config2_unflat = dict(filter(lambda x: '.' not in x[0], config2.items()))
+        config1_flat = dict(filter(lambda x: "." in x[0], config1.items()))
+        config1_unflat = dict(filter(lambda x: "." not in x[0], config1.items()))
+        config2_flat = dict(filter(lambda x: "." in x[0], config2.items()))
+        config2_unflat = dict(filter(lambda x: "." not in x[0], config2.items()))
         # Flatten unflat keys
-        config1_unflat_flat = flatten(config1_unflat, reducer='dot')
-        config2_unflat_flat = flatten(config2_unflat, reducer='dot')
-        if priority == 'flat':
+        config1_unflat_flat = flatten(config1_unflat, reducer="dot")
+        config2_unflat_flat = flatten(config2_unflat, reducer="dot")
+        if priority == "flat":
             # Flat keys erase the previous unflat keys with the same name
             config1_flat = {**config1_unflat_flat, **config1_flat}
             config2_flat = {**config2_unflat_flat, **config2_flat}
         else:
             # The previous unflat keys erase the flat keys with the same name
             config1_flat = {**config1_flat, **config1_unflat_flat}
             config2_flat = {**config2_flat, **config2_unflat_flat}
     else:
-        raise ValueError(f"Unknown dot_prior '{priority}'. Should be one of "
-                         "'flat', 'unflat' or 'order'.")
+        raise ValueError(
+            f"Unknown dot_prior '{priority}'. Should be one of "
+            "'flat', 'unflat' or 'order'."
+        )
     if not allow_new_keys:
         # Check that there are no new keys in config2
         for key in config2_flat:
             if key not in config1_flat.keys():
                 raise ValueError(
                     f"New parameter '{key}' found that is not in the original config."
                 )
     # Merge flat configs
     flat_config = {**config1_flat, **config2_flat}
     # Unflats config
-    config = unflatten(flat_config, splitter='dot')
+    config = unflatten(flat_config, splitter="dot")
     return config
 
 
 def save_config(config: Dict[str, Any], path: str) -> None:
     """Save config to a file.
 
     Parameters
@@ -126,15 +127,15 @@
     config : Dict[str, Any]
         The configuration to save.
     path : str
         The path to the file to save the configuration.
     """
     dir_path = os.path.dirname(path)
     os.makedirs(dir_path, exist_ok=True)
-    with open(path, 'w', encoding='utf-8') as cfg_file:
+    with open(path, "w", encoding="utf-8") as cfg_file:
         yaml.dump(config, cfg_file, default_flow_style=False)
 
 
 def load_config(
     path: str,
     default_configs: Optional[List[str]] = None,
     *,
@@ -164,14 +165,14 @@
     -------
     config : Dict[str, Any]
         The config merged from default configs and the loaded config.
     """
     config: Dict[str, Any] = {}
     if default_configs:
         for config_path in default_configs:
-            with open(config_path, 'r', encoding='utf-8') as cfg_file:
+            with open(config_path, "r", encoding="utf-8") as cfg_file:
                 default_config = yaml.safe_load(cfg_file)
             config = merge(config, default_config, allow_new_keys=True)
-    with open(path, 'r', encoding='utf-8') as cfg_file:
+    with open(path, "r", encoding="utf-8") as cfg_file:
         loaded_config = yaml.safe_load(cfg_file)
     config = merge(config, loaded_config, allow_new_keys=allow_new_keys)
     return config
```

### Comparing `cliconfig-0.1.1/cliconfig/show.py` & `cliconfig-0.1.2/cliconfig/show.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,23 @@
     """Show the configurations.
 
     Parameters
     ----------
     config : Dict[str, Any]
         The configuration to show.
     """
+
     def pretty_print(config: Dict[str, Any], indent: int = 1) -> None:
         """Pretty print the configuration recursively."""
         for key, value in config.items():
-            print(f"{'    ' * indent}{key}: ", end='')
+            print(f"{'    ' * indent}{key}: ", end="")
             if isinstance(value, dict):
                 print()
                 pretty_print(value, indent + 1)
             elif isinstance(value, str):
-                print(f"\'{value}\'")
+                print(f"'{value}'")
             else:
                 print(value)
-    print('Config:')
+
+    print("Config:")
     # printer.pprint(config)
     pretty_print(config)
```

### Comparing `cliconfig-0.1.1/cliconfig.egg-info/PKG-INFO` & `cliconfig-0.1.2/cliconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.1.1
+Version: 0.1.2
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
 
+## Documentation :memo: [here](cliconfig.readthedocs.io)
+
 [![PyPI version](https://badge.fury.io/py/cliconfig.svg)](https://badge.fury.io/py/cliconfig)
 ![PythonVersion](https://img.shields.io/badge/python-3.7%20%7E%203.11-informational)
 [![License](https://img.shields.io/github/license/valentingol/cliconfig?color=999)](https://stringfixer.com/fr/MIT_license)
 
 [![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `cliconfig-0.1.1/cliconfig.egg-info/SOURCES.txt` & `cliconfig-0.1.2/cliconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/docs/Makefile` & `cliconfig-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/docs/conf.py` & `cliconfig-0.1.2/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,41 +3,41 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 import os
 import sys
 
 from setuptools_scm import get_version
 
-sys.path.insert(0, os.path.abspath('../'))
+sys.path.insert(0, os.path.abspath("../"))
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
-project = 'CLI Config'
-copyright = '2023, Valentin Goldite'  # noqa A001
-author = 'Valentin Goldite'
+project = "CLI Config"
+copyright = "2023, Valentin Goldite"  # noqa A001
+author = "Valentin Goldite"
 try:
     release = get_version()
 except:  # noqa E722
-    release = get_version(root='..', relative_to=__file__)
+    release = get_version(root="..", relative_to=__file__)
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "myst_parser",
     "sphinx.ext.autodoc",
     "sphinx.ext.inheritance_diagram",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx_autodoc_typehints",
 ]
 
 master_doc = "index"
-autoapi_type = 'python'
+autoapi_type = "python"
 autoapi_dirs = ["cliconfig"]
 
 autodoc_default_options = {
     "member-order": "bysource",
     "undoc-members": True,
 }
 
@@ -46,16 +46,16 @@
 napoleon_use_param = True
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/", None),
     "numpy": ("http://docs.scipy.org/doc/numpy/", None),
 }
 
-templates_path = ['_templates']
-exclude_patterns = ['_build']
+templates_path = ["_templates"]
+exclude_patterns = ["_build"]
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "sphinx_rtd_theme"
 
 html_theme_options = {
```

### Comparing `cliconfig-0.1.1/docs/index.rst` & `cliconfig-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/docs/license.md` & `cliconfig-0.1.2/docs/license.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/docs/make.bat` & `cliconfig-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/docs/manipulate_configs.md` & `cliconfig-0.1.2/docs/manipulate_configs.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/docs/quickstart.md` & `cliconfig-0.1.2/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/github_actions_utils/pydocstyle_manager.py` & `cliconfig-0.1.2/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/github_actions_utils/pylint_manager.py` & `cliconfig-0.1.2/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/github_actions_utils/pytest_manager.py` & `cliconfig-0.1.2/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/licenses_tier/FLATDICT_LICENSE` & `cliconfig-0.1.2/licenses_tier/FLATDICT_LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/pyproject.toml` & `cliconfig-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/scripts/pre-commit-checks.sh` & `cliconfig-0.1.2/scripts/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `cliconfig-0.1.1/tests/integration/integration_show.py` & `cliconfig-0.1.2/tests/test_show.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,37 @@
-"""Integration tests for show.py."""
+"""Test show.py."""
 
 from cliconfig.show import show_config
 
 
-def main() -> None:
-    """Integration for show_config."""
+def test_show_config() -> None:
+    """Test show_config."""
     config = {
-        'model': {
-            's1_ae_config': {
-                'in_dim': 2,
-                'out_dim': 1,
-                'layer_channels': [16, 32, 64],
-                'conv_per_layer': 1,
-                'residual': False,
-                'dropout_rate': 0.0,
+        "model": {
+            "s1_ae_config": {
+                "in_dim": 2,
+                "out_dim": 1,
+                "layer_channels": [16, 32, 64],
+                "conv_per_layer": 1,
+                "residual": False,
+                "dropout_rate": 0.0,
             },
-            'mask_module_dim': [6, 2],
-            'glob_module_dims': [2, 8, 2],
-            'conv_block_dims': [32, 64, 128],
+            "mask_module_dim": [6, 2],
+            "glob_module_dims": [2, 8, 2],
+            "conv_block_dims": [32, 64, 128],
         },
-        'train': {
-            'n_epochs': 100,
-            'optimizer': {
-                'name': 'Adam',
-                'lr': 0.001,
-                'weight_decay': 0.0,
-                'warmup_steps': 0,
+        "train": {
+            "n_epochs": 100,
+            "optimizer": {
+                "name": "Adam",
+                "lr": 0.001,
+                "weight_decay": 0.0,
+                "warmup_steps": 0,
             },
         },
-        'data': {
-            'dataset': 'mnist',
-            'batch_size': 128,
-            'num_workers': 6,
+        "data": {
+            "dataset": "mnist",
+            "batch_size": 128,
+            "num_workers": 6,
         },
     }
     show_config(config)
-
-
-if __name__ == '__main__':
-    main()
```

### Comparing `cliconfig-0.1.1/tests/test_config.py` & `cliconfig-0.1.2/tests/test_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,124 +7,126 @@
 import pytest_check as check
 
 from cliconfig import load_config, make_config, merge, save_config
 
 
 def test_merge() -> None:
     """Test merge."""
-    config1 = {'a.b': 1, 'a': {'b': 2, 'c': 3}}
-    config2 = {'a': {'c': 1}, 'a.d': 6}
-    config = merge(config1, config2, allow_new_keys=True, priority='flat')
-    check.equal(config, {'a': {'b': 1, 'c': 1, 'd': 6}})
-    config = merge(config1, config2, allow_new_keys=True, priority='unflat')
-    check.equal(config, {'a': {'b': 2, 'c': 1, 'd': 6}})
+    config1 = {"a.b": 1, "a": {"b": 2, "c": 3}}
+    config2 = {"a": {"c": 1}, "a.d": 6}
+    config = merge(config1, config2, allow_new_keys=True, priority="flat")
+    check.equal(config, {"a": {"b": 1, "c": 1, "d": 6}})
+    config = merge(config1, config2, allow_new_keys=True, priority="unflat")
+    check.equal(config, {"a": {"b": 2, "c": 1, "d": 6}})
     with pytest.raises(ValueError, match="New parameter 'a.d' found.*"):
         merge(config1, config2, allow_new_keys=False)
     with pytest.raises(ValueError, match="Unknown dot_prior 'UNKONWN'.*"):
-        merge(config1, config2, allow_new_keys=True, priority='UNKONWN')
+        merge(config1, config2, allow_new_keys=True, priority="UNKONWN")
 
 
 def test_make_config(capsys: pytest.CaptureFixture) -> None:
     """Test make_config."""
     sys_argv = sys.argv.copy()
     sys.argv = [
         "tests/test_make_config.py.py",
         "--config",
         "tests/configs/config1.yaml,tests/configs/config2.yaml",
         "--param2",
         "6",
     ]
     capsys.readouterr()  # Clear stdout and stderr
-    config = make_config('tests/configs/default1.yaml',
-                         'tests/configs/default2.yaml')
+    config = make_config("tests/configs/default1.yaml", "tests/configs/default2.yaml")
     captured = capsys.readouterr()
     out = captured.out
     expected_config = {
-        'param1': 4,
-        'param2': 6,
-        'param3': 3,
-        'letters': {
-            'letter1': 'f',
-            'letter2': 'e',
-            'letter3': 'c',
-            'letter4': 'd',
+        "param1": 4,
+        "param2": 6,
+        "param3": 3,
+        "letters": {
+            "letter1": "f",
+            "letter2": "e",
+            "letter3": "c",
+            "letter4": "d",
         },
     }
-    expected_out = ("[CONFIG] Merge 2 default configs, "
-                    "2 additional configs and 1 CLI parameter(s).\n")
+    expected_out = (
+        "[CONFIG] Merge 2 default configs, "
+        "2 additional configs and 1 CLI parameter(s).\n"
+    )
     check.equal(config, expected_config)
     check.equal(out, expected_out)
 
     # No default configs
     config = make_config(allow_new_keys=True)
     expected_config = {
-        'param1': 4,
-        'param2': 6,
-        'letters': {
-            'letter1': 'f',
-            'letter2': 'e',
+        "param1": 4,
+        "param2": 6,
+        "letters": {
+            "letter1": "f",
+            "letter2": "e",
         },
     }
     check.equal(config, expected_config)
 
     # No additional configs
     sys.argv = [
         "tests/test_make_config.py.py",
     ]
-    config = make_config('tests/configs/default1.yaml',
-                         'tests/configs/default2.yaml')
+    config = make_config("tests/configs/default1.yaml", "tests/configs/default2.yaml")
     expected_config = {
-        'param1': 1,
-        'param2': 2,
-        'param3': 3,
-        'letters': {
-            'letter1': 'a',
-            'letter2': 'b',
-            'letter3': 'c',
-            'letter4': 'd',
+        "param1": 1,
+        "param2": 2,
+        "param3": 3,
+        "letters": {
+            "letter1": "a",
+            "letter2": "b",
+            "letter3": "c",
+            "letter4": "d",
         },
     }
     check.equal(config, expected_config)
 
     sys.argv = sys_argv.copy()
 
 
 def test_save_load_config() -> None:
     """Test save_config and load_config."""
-    config1 = {'a': 1, 'b': {'c': 2}, 'd': [2, 3.0], 'e': [{'f': 4}]}
-    save_config(config1, 'tests/tmp/config.yaml')
-    check.is_true(os.path.isfile('tests/tmp/config.yaml'))
-    config2 = load_config('tests/tmp/config.yaml')
+    config1 = {"a": 1, "b": {"c": 2}, "d": [2, 3.0], "e": [{"f": 4}]}
+    save_config(config1, "tests/tmp/config.yaml")
+    check.is_true(os.path.isfile("tests/tmp/config.yaml"))
+    config2 = load_config("tests/tmp/config.yaml")
     check.equal(config1, config2)
 
     # With default configs
-    config = {'param1': 3, 'param2': 4, 'letters': {'letter1': 'e'}}
-    save_config(config, 'tests/tmp/config2.yaml')
+    config = {"param1": 3, "param2": 4, "letters": {"letter1": "e"}}
+    save_config(config, "tests/tmp/config2.yaml")
     config = load_config(
-        'tests/tmp/config2.yaml',
-        default_configs=['tests/configs/default1.yaml', 'tests/configs/default2.yaml'],
+        "tests/tmp/config2.yaml",
+        default_configs=["tests/configs/default1.yaml", "tests/configs/default2.yaml"],
         allow_new_keys=False,
     )
     expected_config = {
-        'param1': 3,
-        'param2': 4,
-        'param3': 3,
-        'letters': {
-            'letter1': 'e',
-            'letter2': 'b',
-            'letter3': 'c',
-            'letter4': 'd',
+        "param1": 3,
+        "param2": 4,
+        "param3": 3,
+        "letters": {
+            "letter1": "e",
+            "letter2": "b",
+            "letter3": "c",
+            "letter4": "d",
         },
     }
     check.equal(config, expected_config)
     # Additional keys when allow_new_keys=False
-    config = {'param4': 0}
-    save_config(config, 'tests/tmp/config3.yaml')
+    config = {"param4": 0}
+    save_config(config, "tests/tmp/config3.yaml")
     with pytest.raises(ValueError, match="New parameter 'param4' found.*"):
         load_config(
-            'tests/tmp/config3.yaml',
-            default_configs=['tests/configs/default1.yaml',
-                             'tests/configs/default2.yaml'],
+            "tests/tmp/config3.yaml",
+            default_configs=[
+                "tests/configs/default1.yaml",
+                "tests/configs/default2.yaml",
+            ],
             allow_new_keys=False,
         )
 
-    shutil.rmtree('tests/tmp')
+    shutil.rmtree("tests/tmp")
```

### Comparing `cliconfig-0.1.1/tests/test_show.py` & `cliconfig-0.1.2/tests/integration/integration_show.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-"""Test show.py."""
+"""Integration tests for show.py."""
 
 from cliconfig.show import show_config
 
 
-def test_show_config() -> None:
-    """Test show_config."""
+def main() -> None:
+    """Integration for show_config."""
     config = {
-        'model': {
-            's1_ae_config': {
-                'in_dim': 2,
-                'out_dim': 1,
-                'layer_channels': [16, 32, 64],
-                'conv_per_layer': 1,
-                'residual': False,
-                'dropout_rate': 0.0,
+        "model": {
+            "s1_ae_config": {
+                "in_dim": 2,
+                "out_dim": 1,
+                "layer_channels": [16, 32, 64],
+                "conv_per_layer": 1,
+                "residual": False,
+                "dropout_rate": 0.0,
             },
-            'mask_module_dim': [6, 2],
-            'glob_module_dims': [2, 8, 2],
-            'conv_block_dims': [32, 64, 128],
+            "mask_module_dim": [6, 2],
+            "glob_module_dims": [2, 8, 2],
+            "conv_block_dims": [32, 64, 128],
         },
-        'train': {
-            'n_epochs': 100,
-            'optimizer': {
-                'name': 'Adam',
-                'lr': 0.001,
-                'weight_decay': 0.0,
-                'warmup_steps': 0,
+        "train": {
+            "n_epochs": 100,
+            "optimizer": {
+                "name": "Adam",
+                "lr": 0.001,
+                "weight_decay": 0.0,
+                "warmup_steps": 0,
             },
         },
-        'data': {
-            'dataset': 'mnist',
-            'batch_size': 128,
-            'num_workers': 6,
+        "data": {
+            "dataset": "mnist",
+            "batch_size": 128,
+            "num_workers": 6,
         },
     }
     show_config(config)
+
+
+if __name__ == "__main__":
+    main()
```

