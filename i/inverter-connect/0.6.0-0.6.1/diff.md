# Comparing `tmp/inverter-connect-0.6.0.tar.gz` & `tmp/inverter-connect-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inverter-connect-0.6.0.tar", last modified: Sat May  6 11:20:24 2023, max compression
+gzip compressed data, was "inverter-connect-0.6.1.tar", last modified: Sun May  7 10:42:43 2023, max compression
```

## Comparing `inverter-connect-0.6.0.tar` & `inverter-connect-0.6.1.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.6.0/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.6.0/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-03 17:50:50.000000 inverter-connect-0.6.0/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.6.0/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)    16300 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)    15886 2023-05-06 10:27:49.000000 inverter-connect-0.6.0/README.md
--rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:23:42.000000 inverter-connect-0.6.0/cli.py
--rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:24:01.000000 inverter-connect-0.6.0/dev-cli.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/
--rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.6.0/inverter/.editorconfig
--rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.6.0/inverter/.flake8
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/.github/
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/.github/workflows/
--rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.6.0/inverter/.github/workflows/tests.yml
--rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.6.0/inverter/.gitignore
--rw-rw-r--   0 jens      (1000) users      (100)      148 2023-05-06 10:44:15.000000 inverter-connect-0.6.0/inverter/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.6.0/inverter/__main__.py
--rw-rw-r--   0 jens      (1000) users      (100)     4788 2023-05-06 10:38:46.000000 inverter-connect-0.6.0/inverter/api.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/cli/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.6.0/inverter/cli/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)    13773 2023-05-06 10:27:47.000000 inverter-connect-0.6.0/inverter/cli/cli_app.py
--rw-rw-r--   0 jens      (1000) users      (100)     7864 2023-05-03 17:42:33.000000 inverter-connect-0.6.0/inverter/cli/dev.py
--rw-rw-r--   0 jens      (1000) users      (100)    10044 2023-05-06 10:26:14.000000 inverter-connect-0.6.0/inverter/connection.py
--rw-rw-r--   0 jens      (1000) users      (100)      312 2023-05-06 10:27:41.000000 inverter-connect-0.6.0/inverter/constants.py
--rw-rw-r--   0 jens      (1000) users      (100)     1768 2023-05-06 10:26:14.000000 inverter-connect-0.6.0/inverter/daily_reset.py
--rw-rw-r--   0 jens      (1000) users      (100)     3686 2023-05-06 11:17:52.000000 inverter-connect-0.6.0/inverter/data_types.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/definitions/
--rw-rw-r--   0 jens      (1000) users      (100)     2918 2023-04-23 17:07:32.000000 inverter-connect-0.6.0/inverter/definitions/deye_2mppt.yaml
--rw-rw-r--   0 jens      (1000) users      (100)      213 2023-05-06 09:30:48.000000 inverter-connect-0.6.0/inverter/definitions/deye_2mppt_validations.yaml
--rw-rw-r--   0 jens      (1000) users      (100)     2260 2023-05-06 10:26:15.000000 inverter-connect-0.6.0/inverter/definitions.py
--rw-rw-r--   0 jens      (1000) users      (100)      538 2023-05-06 10:11:26.000000 inverter-connect-0.6.0/inverter/exceptions.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/mqtt4homeassistant/
--rw-rw-r--   0 jens      (1000) users      (100)       22 2023-04-24 06:39:33.000000 inverter-connect-0.6.0/inverter/mqtt4homeassistant/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     1892 2023-04-27 06:35:47.000000 inverter-connect-0.6.0/inverter/mqtt4homeassistant/converter.py
--rw-rw-r--   0 jens      (1000) users      (100)     1209 2023-04-24 07:07:57.000000 inverter-connect-0.6.0/inverter/mqtt4homeassistant/data_classes.py
--rw-rw-r--   0 jens      (1000) users      (100)     3803 2023-04-24 07:36:06.000000 inverter-connect-0.6.0/inverter/mqtt4homeassistant/mqtt.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/mqtt4homeassistant/tests/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.6.0/inverter/mqtt4homeassistant/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2136 2023-04-27 06:35:47.000000 inverter-connect-0.6.0/inverter/mqtt4homeassistant/tests/test_converter.py
--rw-rw-r--   0 jens      (1000) users      (100)      245 2023-04-24 06:13:14.000000 inverter-connect-0.6.0/inverter/mqtt4homeassistant/tests/test_doctests.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/mqtt4homeassistant/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.6.0/inverter/mqtt4homeassistant/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)      315 2023-04-23 16:57:27.000000 inverter-connect-0.6.0/inverter/mqtt4homeassistant/utilities/string_utils.py
--rw-rw-r--   0 jens      (1000) users      (100)     3047 2023-05-06 10:27:47.000000 inverter-connect-0.6.0/inverter/publish_loop.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/tests/
--rw-rw-r--   0 jens      (1000) users      (100)      269 2023-04-23 16:25:11.000000 inverter-connect-0.6.0/inverter/tests/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     3293 2023-05-06 10:24:09.000000 inverter-connect-0.6.0/inverter/tests/test_api.py
--rw-rw-r--   0 jens      (1000) users      (100)      826 2023-05-06 10:26:14.000000 inverter-connect-0.6.0/inverter/tests/test_connect.py
--rw-rw-r--   0 jens      (1000) users      (100)     5880 2023-05-06 10:42:16.000000 inverter-connect-0.6.0/inverter/tests/test_daily_reset.py
--rw-rw-r--   0 jens      (1000) users      (100)     1589 2023-05-06 10:41:55.000000 inverter-connect-0.6.0/inverter/tests/test_definitions.py
--rw-rw-r--   0 jens      (1000) users      (100)      211 2023-04-17 13:29:40.000000 inverter-connect-0.6.0/inverter/tests/test_doctests.py
--rw-rw-r--   0 jens      (1000) users      (100)     2641 2023-05-03 17:38:17.000000 inverter-connect-0.6.0/inverter/tests/test_project_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     3422 2023-05-05 19:51:25.000000 inverter-connect-0.6.0/inverter/tests/test_readme.py
--rw-rw-r--   0 jens      (1000) users      (100)     2114 2023-05-06 11:19:29.000000 inverter-connect-0.6.0/inverter/tests/test_validators.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter/utilities/
--rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.6.0/inverter/utilities/__init__.py
--rw-rw-r--   0 jens      (1000) users      (100)     2179 2023-05-06 10:25:25.000000 inverter-connect-0.6.0/inverter/utilities/cli.py
--rw-rw-r--   0 jens      (1000) users      (100)      925 2023-04-24 15:15:46.000000 inverter-connect-0.6.0/inverter/utilities/credentials.py
--rw-rw-r--   0 jens      (1000) users      (100)      175 2023-04-24 15:15:46.000000 inverter-connect-0.6.0/inverter/utilities/log_setup.py
--rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-24 08:58:03.000000 inverter-connect-0.6.0/inverter/utilities/modbus_converter.py
--rw-rw-r--   0 jens      (1000) users      (100)     1562 2023-05-06 10:34:37.000000 inverter-connect-0.6.0/inverter/validators.py
-drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/inverter_connect.egg-info/
--rw-rw-r--   0 jens      (1000) users      (100)    16300 2023-05-06 11:20:24.000000 inverter-connect-0.6.0/inverter_connect.egg-info/PKG-INFO
--rw-rw-r--   0 jens      (1000) users      (100)     1744 2023-05-06 11:20:24.000000 inverter-connect-0.6.0/inverter_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-06 11:20:24.000000 inverter-connect-0.6.0/inverter_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 jens      (1000) users      (100)       93 2023-05-06 11:20:24.000000 inverter-connect-0.6.0/inverter_connect.egg-info/entry_points.txt
--rw-rw-r--   0 jens      (1000) users      (100)      277 2023-05-06 11:20:24.000000 inverter-connect-0.6.0/inverter_connect.egg-info/requires.txt
--rw-rw-r--   0 jens      (1000) users      (100)        9 2023-05-06 11:20:24.000000 inverter-connect-0.6.0/inverter_connect.egg-info/top_level.txt
--rw-rw-r--   0 jens      (1000) users      (100)     4882 2023-05-06 09:28:26.000000 inverter-connect-0.6.0/pyproject.toml
--rw-rw-r--   0 jens      (1000) users      (100)    53370 2023-05-06 09:28:51.000000 inverter-connect-0.6.0/requirements.dev.txt
--rw-rw-r--   0 jens      (1000) users      (100)     7830 2023-05-06 09:28:32.000000 inverter-connect-0.6.0/requirements.txt
--rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-06 11:20:24.527930 inverter-connect-0.6.0/setup.cfg
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-13 15:18:51.000000 inverter-connect-0.6.1/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-13 15:18:51.000000 inverter-connect-0.6.1/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1476 2023-05-03 17:50:50.000000 inverter-connect-0.6.1/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-13 15:18:51.000000 inverter-connect-0.6.1/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)    16300 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)    15886 2023-05-06 10:27:49.000000 inverter-connect-0.6.1/README.md
+-rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:23:42.000000 inverter-connect-0.6.1/cli.py
+-rwxrwxr-x   0 jens      (1000) users      (100)     3051 2023-05-03 17:24:01.000000 inverter-connect-0.6.1/dev-cli.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/
+-rw-rw-r--   0 jens      (1000) users      (100)      301 2023-04-17 13:29:40.000000 inverter-connect-0.6.1/inverter/.editorconfig
+-rw-rw-r--   0 jens      (1000) users      (100)      153 2023-04-17 13:29:40.000000 inverter-connect-0.6.1/inverter/.flake8
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/.github/
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/.github/workflows/
+-rw-rw-r--   0 jens      (1000) users      (100)     1460 2023-04-17 13:29:40.000000 inverter-connect-0.6.1/inverter/.github/workflows/tests.yml
+-rw-rw-r--   0 jens      (1000) users      (100)      118 2023-04-17 13:29:40.000000 inverter-connect-0.6.1/inverter/.gitignore
+-rw-rw-r--   0 jens      (1000) users      (100)      148 2023-05-07 09:25:42.000000 inverter-connect-0.6.1/inverter/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      186 2023-04-20 19:23:05.000000 inverter-connect-0.6.1/inverter/__main__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     4852 2023-05-07 09:15:43.000000 inverter-connect-0.6.1/inverter/api.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/cli/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 13:29:40.000000 inverter-connect-0.6.1/inverter/cli/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)    13874 2023-05-07 09:17:33.000000 inverter-connect-0.6.1/inverter/cli/cli_app.py
+-rw-rw-r--   0 jens      (1000) users      (100)     7864 2023-05-03 17:42:33.000000 inverter-connect-0.6.1/inverter/cli/dev.py
+-rw-rw-r--   0 jens      (1000) users      (100)    10423 2023-05-07 09:11:34.000000 inverter-connect-0.6.1/inverter/connection.py
+-rw-rw-r--   0 jens      (1000) users      (100)      312 2023-05-06 10:27:41.000000 inverter-connect-0.6.1/inverter/constants.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1768 2023-05-06 10:26:14.000000 inverter-connect-0.6.1/inverter/daily_reset.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3700 2023-05-07 09:03:56.000000 inverter-connect-0.6.1/inverter/data_types.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/definitions/
+-rw-rw-r--   0 jens      (1000) users      (100)     2918 2023-04-23 17:07:32.000000 inverter-connect-0.6.1/inverter/definitions/deye_2mppt.yaml
+-rw-rw-r--   0 jens      (1000) users      (100)      213 2023-05-06 09:30:48.000000 inverter-connect-0.6.1/inverter/definitions/deye_2mppt_validations.yaml
+-rw-rw-r--   0 jens      (1000) users      (100)     2260 2023-05-06 10:26:15.000000 inverter-connect-0.6.1/inverter/definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      538 2023-05-06 10:11:26.000000 inverter-connect-0.6.1/inverter/exceptions.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/mqtt4homeassistant/
+-rw-rw-r--   0 jens      (1000) users      (100)       22 2023-04-24 06:39:33.000000 inverter-connect-0.6.1/inverter/mqtt4homeassistant/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1892 2023-04-27 06:35:47.000000 inverter-connect-0.6.1/inverter/mqtt4homeassistant/converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1209 2023-04-24 07:07:57.000000 inverter-connect-0.6.1/inverter/mqtt4homeassistant/data_classes.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3803 2023-04-24 07:36:06.000000 inverter-connect-0.6.1/inverter/mqtt4homeassistant/mqtt.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/mqtt4homeassistant/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.6.1/inverter/mqtt4homeassistant/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2136 2023-04-27 06:35:47.000000 inverter-connect-0.6.1/inverter/mqtt4homeassistant/tests/test_converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)      245 2023-04-24 06:13:14.000000 inverter-connect-0.6.1/inverter/mqtt4homeassistant/tests/test_doctests.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/mqtt4homeassistant/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-24 06:00:10.000000 inverter-connect-0.6.1/inverter/mqtt4homeassistant/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)      315 2023-04-23 16:57:27.000000 inverter-connect-0.6.1/inverter/mqtt4homeassistant/utilities/string_utils.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3138 2023-05-07 09:16:41.000000 inverter-connect-0.6.1/inverter/publish_loop.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/tests/
+-rw-rw-r--   0 jens      (1000) users      (100)      269 2023-04-23 16:25:11.000000 inverter-connect-0.6.1/inverter/tests/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3293 2023-05-06 10:24:09.000000 inverter-connect-0.6.1/inverter/tests/test_api.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1230 2023-05-07 09:25:28.000000 inverter-connect-0.6.1/inverter/tests/test_cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)      826 2023-05-06 10:26:14.000000 inverter-connect-0.6.1/inverter/tests/test_connect.py
+-rw-rw-r--   0 jens      (1000) users      (100)     5880 2023-05-06 10:42:16.000000 inverter-connect-0.6.1/inverter/tests/test_daily_reset.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1589 2023-05-06 10:41:55.000000 inverter-connect-0.6.1/inverter/tests/test_definitions.py
+-rw-rw-r--   0 jens      (1000) users      (100)      211 2023-04-17 13:29:40.000000 inverter-connect-0.6.1/inverter/tests/test_doctests.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2641 2023-05-03 17:38:17.000000 inverter-connect-0.6.1/inverter/tests/test_project_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     3422 2023-05-05 19:51:25.000000 inverter-connect-0.6.1/inverter/tests/test_readme.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2114 2023-05-06 11:19:29.000000 inverter-connect-0.6.1/inverter/tests/test_validators.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter/utilities/
+-rw-rw-r--   0 jens      (1000) users      (100)        0 2023-04-17 17:34:28.000000 inverter-connect-0.6.1/inverter/utilities/__init__.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2179 2023-05-06 10:25:25.000000 inverter-connect-0.6.1/inverter/utilities/cli.py
+-rw-rw-r--   0 jens      (1000) users      (100)      925 2023-04-24 15:15:46.000000 inverter-connect-0.6.1/inverter/utilities/credentials.py
+-rw-rw-r--   0 jens      (1000) users      (100)      175 2023-04-24 15:15:46.000000 inverter-connect-0.6.1/inverter/utilities/log_setup.py
+-rw-rw-r--   0 jens      (1000) users      (100)     2187 2023-04-24 08:58:03.000000 inverter-connect-0.6.1/inverter/utilities/modbus_converter.py
+-rw-rw-r--   0 jens      (1000) users      (100)     1562 2023-05-06 10:34:37.000000 inverter-connect-0.6.1/inverter/validators.py
+drwxrwxr-x   0 jens      (1000) users      (100)        0 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/inverter_connect.egg-info/
+-rw-rw-r--   0 jens      (1000) users      (100)    16300 2023-05-07 10:42:43.000000 inverter-connect-0.6.1/inverter_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 jens      (1000) users      (100)     1771 2023-05-07 10:42:43.000000 inverter-connect-0.6.1/inverter_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        1 2023-05-07 10:42:43.000000 inverter-connect-0.6.1/inverter_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       93 2023-05-07 10:42:43.000000 inverter-connect-0.6.1/inverter_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 jens      (1000) users      (100)      277 2023-05-07 10:42:43.000000 inverter-connect-0.6.1/inverter_connect.egg-info/requires.txt
+-rw-rw-r--   0 jens      (1000) users      (100)        9 2023-05-07 10:42:43.000000 inverter-connect-0.6.1/inverter_connect.egg-info/top_level.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     4882 2023-05-06 09:28:26.000000 inverter-connect-0.6.1/pyproject.toml
+-rw-rw-r--   0 jens      (1000) users      (100)    53370 2023-05-06 09:28:51.000000 inverter-connect-0.6.1/requirements.dev.txt
+-rw-rw-r--   0 jens      (1000) users      (100)     7830 2023-05-06 09:28:32.000000 inverter-connect-0.6.1/requirements.txt
+-rw-rw-r--   0 jens      (1000) users      (100)       38 2023-05-07 10:42:43.236178 inverter-connect-0.6.1/setup.cfg
```

### Comparing `inverter-connect-0.6.0/.github/workflows/tests.yml` & `inverter-connect-0.6.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/PKG-INFO` & `inverter-connect-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inverter-connect
-Version: 0.6.0
+Version: 0.6.1
 Summary: Get information from Deye Microinverter
 Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/inverter-connect
 Project-URL: Source, https://github.com/jedie/inverter-connect
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
```

### Comparing `inverter-connect-0.6.0/README.md` & `inverter-connect-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/cli.py` & `inverter-connect-0.6.1/cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/dev-cli.py` & `inverter-connect-0.6.1/dev-cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/.github/workflows/tests.yml` & `inverter-connect-0.6.1/inverter/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/api.py` & `inverter-connect-0.6.1/inverter/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,17 @@
         self.value_validator = InverterValueValidator(config=config)
         self.inv_sock = InverterSock(config)
 
     def __enter__(self):
         self.inv_sock.__enter__()
         return self
 
+    def connect(self) -> None:
+        self.inv_sock.connect()
+
     def __iter__(self) -> Iterable[InverterValue]:
         values = {}
         for parameter in self.parameters:
             name = parameter.name
 
             result = None  # noqa
             for try_count in range(3):
```

### Comparing `inverter-connect-0.6.0/inverter/cli/cli_app.py` & `inverter-connect-0.6.1/inverter/cli/cli_app.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 from rich_click import RichGroup
 
 import inverter
 from inverter import constants
 from inverter.api import Inverter, set_current_time
 from inverter.connection import InverterSock
 from inverter.constants import ERROR_STR_NO_DATA
-from inverter.data_types import Config, InverterInfo, Parameter, ValueType
+from inverter.data_types import Config, Parameter, ValueType
+from inverter.exceptions import ReadInverterError
 from inverter.mqtt4homeassistant.data_classes import MqttSettings
 from inverter.mqtt4homeassistant.mqtt import get_connected_client
 from inverter.publish_loop import publish_forever
 from inverter.utilities.cli import convert_address_option, print_register
 from inverter.utilities.credentials import get_mqtt_settings, store_mqtt_settings
 from inverter.utilities.log_setup import basic_log_setup
 
@@ -98,18 +99,21 @@
     Print all known register values from Inverter, e.g.:
 
     .../inverter-connect$ ./cli.py print-values 192.168.123.456
     """
     basic_log_setup(debug=debug)
 
     config = Config(inverter_name=inverter, host=ip, port=port, verbose=verbose, debug=debug)
+
     with Inverter(config=config) as inverter:
-        inverter_info: InverterInfo = inverter.inv_sock.inverter_info
-        print(inverter_info)
-        print()
+        try:
+            inverter.connect()
+        except ReadInverterError as err:
+            print(f'[red]{err}')
+            sys.exit(1)
 
         for value in inverter:
             print(f'\t* [yellow]{value.name:<31}[/yellow]:', end=' ')
             if value.value == ERROR_STR_NO_DATA:
                 color = 'red'
                 msg = ERROR_STR_NO_DATA
             else:
@@ -208,21 +212,21 @@
             'NTPEN',  # Enable/Disable NTP Server
             'WSDNS',  # Set/Get the DNS Server address
             'DEVICENUM',  # Set/Get Device Link Num
             'DEVSELCTL',  # Set/Get Web Device List Info
         )
 
     config = Config(inverter_name=None, host=ip, port=port, verbose=verbose, debug=debug)
-    if debug:
-        print(config)
 
     with InverterSock(config) as inv_sock:
-        inverter_info: InverterInfo = inv_sock.inverter_info
-        print(inverter_info)
-        print()
+        try:
+            inv_sock.connect()
+        except ReadInverterError as err:
+            print(f'[red]{err}')
+            sys.exit(1)
 
         for command in commands:
             print(f'\t* [grey]AT+[/grey][bold][yellow]{command:<10}[/yellow]:', end=' ')
             result: str = inv_sock.cleaned_at_command(command)
             print(f'[green]{result}')
 
 
@@ -245,21 +249,21 @@
         0x16 - year + month
         0x17 - day + hour
         0x18 - minute + second
     """
     address = convert_address_option(raw_address=register, debug=debug)
 
     config = Config(inverter_name=None, host=ip, port=port, verbose=verbose, debug=debug)
-    if debug:
-        print(config)
 
     with InverterSock(config) as inv_sock:
-        inverter_info: InverterInfo = inv_sock.inverter_info
-        print(inverter_info)
-        print()
+        try:
+            inv_sock.connect()
+        except ReadInverterError as err:
+            print(f'[red]{err}')
+            sys.exit(1)
 
         set_current_time(inv_sock=inv_sock, address=address, verbose=True)
 
         print('\nRead register...')
         time.sleep(1)
         print_register(inv_sock, start_register=address, length=3)
 
@@ -297,17 +301,20 @@
     """
     print(f'Read {length} register(s) from {register=!r} ({ip}:{port})')
     address = convert_address_option(raw_address=register, debug=debug)
 
     config = Config(inverter_name=None, host=ip, port=port, verbose=verbose, debug=debug)
 
     with InverterSock(config) as inv_sock:
-        inverter_info: InverterInfo = inv_sock.inverter_info
-        print(inverter_info)
-        print()
+        try:
+            inv_sock.connect()
+        except ReadInverterError as err:
+            print(f'[red]{err}')
+            sys.exit(1)
+
         print_register(inv_sock, start_register=address, length=length)
 
 
 cli.add_command(read_register)
 
 
 ######################################################################################################
```

### Comparing `inverter-connect-0.6.0/inverter/cli/dev.py` & `inverter-connect-0.6.1/inverter/cli/dev.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/connection.py` & `inverter-connect-0.6.1/inverter/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,22 @@
 import socket
 import time
 
 from rich import print  # noqa
 
 from inverter.constants import AT_READ_FUNC_NUMBER, AT_WRITE_FUNC_NUMBER, ERROR_STR_NO_DATA
 from inverter.data_types import Config, InverterInfo, ModbusReadResult, ModbusResponse, Parameter, RawModBusResponse
-from inverter.exceptions import CrcError, ModbusNoData, ModbusNoHexData, ParseModbusValueError, ReadTimeout
+from inverter.exceptions import (
+    CrcError,
+    ModbusNoData,
+    ModbusNoHexData,
+    ParseModbusValueError,
+    ReadInverterError,
+    ReadTimeout,
+)
 
 
 logger = logging.getLogger(__name__)
 
 
 def make_modbus_result(*, response: ModbusResponse, parameter: Parameter) -> ModbusReadResult:
     parser_func = parameter.parser
@@ -163,46 +170,63 @@
     return result
 
 
 class InverterSock:
     def __init__(self, config: Config):
         self.config = config
 
+        self.sock = None
         self.dock = None
         self.inverter_info = None
 
-    def __enter__(self):
+    def __enter__(self) -> InverterSock:
+        return self
+
+    def init_inventer(self) -> None:
+        data = self.recv_command(command=self.config.init_cmd)
+        self.send(command=b'+ok')
+        data = data.decode()
+        data = data.split(',')
+        self.inverter_info = InverterInfo(ip=data[0], mac=data[1], serial=int(data[2]))
+
+        print(self.inverter_info)
+        print()
+
+    def connect(self) -> None:
+        assert self.sock is None
         logger.info(f'Connect to {self.config.host}:{self.config.port}...')
         self.sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
         self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self.sock.settimeout(self.config.timeout)
 
-        self.inverter_info = self.init_inventer()
-
-        return self
+        self.init_inventer()
 
     def send(self, *, command: bytes):
         if self.config.debug:
             print(f'send: {command}', end='...', flush=True)
-        self.sock.sendto(command, (self.config.host, self.config.port))
+
+        try:
+            self.sock.sendto(command, (self.config.host, self.config.port))
+        except socket.gaierror as err:
+            raise ReadInverterError(f'{err} (Hint: Check {self.config.host}:{self.config.port})')
 
         if self.config.debug:
             print('OK', flush=True)
 
         time.sleep(self.config.pause)
 
     def recv_command(self, *, command: bytes, buffer_size=1024):
         self.send(command=command)
 
         if self.config.debug:
             print('recv', end='...', flush=True)
 
         try:
             data = self.sock.recv(buffer_size)
-        except TimeoutError as err:
+        except (TimeoutError, socket.timeout) as err:
             raise ReadTimeout(f'Get no response from {self.config.host}: {err}')
         else:
             if self.config.debug:
                 print(f'{data}', flush=True)
 
             return data
 
@@ -231,26 +255,20 @@
         logger.debug(f'{raw_modbus_response=}')
         if data == 'no data':
             raise ModbusNoData
 
         return raw_modbus_response.data
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        print('\nSigning off with "AT+Q"', end='...')
-        self.send(command=b'AT+Q\n')
-        print('Goodbye ;)\n')
         if exc_type:
             return False
 
-    def init_inventer(self):
-        data = self.recv_command(command=self.config.init_cmd)
-        self.send(command=b'+ok')
-        data = data.decode()
-        data = data.split(',')
-        return InverterInfo(ip=data[0], mac=data[1], serial=int(data[2]))
+        print('\nSigning off with "AT+Q"', end='...')
+        self.send(command=b'AT+Q\n')
+        print('Goodbye ;)\n')
 
     def read(self, *, start_register: int, length: int) -> ModbusResponse:
         if self.config.debug:
             print(f'Read {length} value(s) from start register: {hex(start_register)}')
 
         command = parameter2modbus_at_command(
             start_register=start_register,
```

### Comparing `inverter-connect-0.6.0/inverter/daily_reset.py` & `inverter-connect-0.6.1/inverter/daily_reset.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/data_types.py` & `inverter-connect-0.6.1/inverter/data_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
             self.validation_file_path = BASE_PATH / 'definitions' / f'{self.inverter_name}_validations.yaml'
             if not self.validation_file_path.is_file():
                 raise FileNotFoundError(
                     f'Wrong inverter name: {self.inverter_name!r}: File not found: {self.validation_file_path}'
                 )
 
-        if self.verbose:
+        if self.verbose or self.debug:
             print(self)
 
 
 @dataclasses.dataclass
 class ResetState:
     started: datetime
     set_time_count: int = 0
```

### Comparing `inverter-connect-0.6.0/inverter/definitions/deye_2mppt.yaml` & `inverter-connect-0.6.1/inverter/definitions/deye_2mppt.yaml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/definitions.py` & `inverter-connect-0.6.1/inverter/definitions.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/exceptions.py` & `inverter-connect-0.6.1/inverter/exceptions.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/mqtt4homeassistant/converter.py` & `inverter-connect-0.6.1/inverter/mqtt4homeassistant/converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/mqtt4homeassistant/data_classes.py` & `inverter-connect-0.6.1/inverter/mqtt4homeassistant/data_classes.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/mqtt4homeassistant/mqtt.py` & `inverter-connect-0.6.1/inverter/mqtt4homeassistant/mqtt.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/mqtt4homeassistant/tests/test_converter.py` & `inverter-connect-0.6.1/inverter/mqtt4homeassistant/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/publish_loop.py` & `inverter-connect-0.6.1/inverter/publish_loop.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,18 +21,18 @@
     publisher = HaMqttPublisher(settings=mqtt_settings, verbose=verbose, config_count=1)
 
     reset_state = ResetState(started=datetime.now())
 
     while True:
         try:
             with Inverter(config=config) as inverter:
+                inverter.connect()
+                inverter_info: InverterInfo = inverter.inv_sock.inverter_info
+
                 with DailyProductionReset(reset_state, inverter, config) as daily_production_reset:
-                    inverter_info: InverterInfo = inverter.inv_sock.inverter_info
-                    print(inverter_info)
-                    print()
 
                     try:
                         values = []
                         for value in inverter:
                             assert isinstance(value, InverterValue), f'{value!r}'
                             if value.value == ERROR_STR_NO_DATA:
                                 # Don't send a MQTT message if one of the values are missing:
@@ -60,12 +60,15 @@
                             prefix='homeassistant',
                             component='sensor',
                         )
                         ha_mqtt_payload = values2mqtt_payload(values=values, name_prefix='inverter')
                         publisher.publish2homeassistant(ha_mqtt_payload=ha_mqtt_payload)
         except ReadTimeout as err:
             print(f'[red]{err}')
+        except BaseException as err:
+            print(f'[red]{err}')
+            logger.exception('Unexpected error: %s', err)
 
         print('Wait', end='...')
         for i in range(10, 1, -1):
             time.sleep(1)
             print(i, end='...')
```

### Comparing `inverter-connect-0.6.0/inverter/tests/test_api.py` & `inverter-connect-0.6.1/inverter/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/tests/test_connect.py` & `inverter-connect-0.6.1/inverter/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/tests/test_daily_reset.py` & `inverter-connect-0.6.1/inverter/tests/test_daily_reset.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/tests/test_definitions.py` & `inverter-connect-0.6.1/inverter/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/tests/test_project_setup.py` & `inverter-connect-0.6.1/inverter/tests/test_project_setup.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/tests/test_readme.py` & `inverter-connect-0.6.1/inverter/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/tests/test_validators.py` & `inverter-connect-0.6.1/inverter/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/utilities/cli.py` & `inverter-connect-0.6.1/inverter/utilities/cli.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/utilities/credentials.py` & `inverter-connect-0.6.1/inverter/utilities/credentials.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/utilities/modbus_converter.py` & `inverter-connect-0.6.1/inverter/utilities/modbus_converter.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter/validators.py` & `inverter-connect-0.6.1/inverter/validators.py`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/inverter_connect.egg-info/PKG-INFO` & `inverter-connect-0.6.1/inverter_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inverter-connect
-Version: 0.6.0
+Version: 0.6.1
 Summary: Get information from Deye Microinverter
 Author-email: Jens Diemer <inverter-connect@jensdiemer.de>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://github.com/jedie/inverter-connect
 Project-URL: Source, https://github.com/jedie/inverter-connect
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
```

### Comparing `inverter-connect-0.6.0/inverter_connect.egg-info/SOURCES.txt` & `inverter-connect-0.6.1/inverter_connect.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 inverter/mqtt4homeassistant/tests/__init__.py
 inverter/mqtt4homeassistant/tests/test_converter.py
 inverter/mqtt4homeassistant/tests/test_doctests.py
 inverter/mqtt4homeassistant/utilities/__init__.py
 inverter/mqtt4homeassistant/utilities/string_utils.py
 inverter/tests/__init__.py
 inverter/tests/test_api.py
+inverter/tests/test_cli.py
 inverter/tests/test_connect.py
 inverter/tests/test_daily_reset.py
 inverter/tests/test_definitions.py
 inverter/tests/test_doctests.py
 inverter/tests/test_project_setup.py
 inverter/tests/test_readme.py
 inverter/tests/test_validators.py
```

### Comparing `inverter-connect-0.6.0/pyproject.toml` & `inverter-connect-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/requirements.dev.txt` & `inverter-connect-0.6.1/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `inverter-connect-0.6.0/requirements.txt` & `inverter-connect-0.6.1/requirements.txt`

 * *Files identical despite different names*

