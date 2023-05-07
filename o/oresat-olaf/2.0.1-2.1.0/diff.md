# Comparing `tmp/oresat-olaf-2.0.1.tar.gz` & `tmp/oresat-olaf-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat-olaf-2.0.1.tar", last modified: Thu May  4 23:18:36 2023, max compression
+gzip compressed data, was "oresat-olaf-2.1.0.tar", last modified: Sun May  7 20:22:13 2023, max compression
```

## Comparing `oresat-olaf-2.0.1.tar` & `oresat-olaf-2.1.0.tar`

### file list

```diff
@@ -1,87 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.917580 oresat-olaf-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-04 23:18:36.917580 oresat-olaf-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.897580 oresat-olaf-2.0.1/olaf/
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.901580 oresat-olaf-2.0.1/olaf/_internals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.901580 oresat-olaf-2.0.1/olaf/_internals/data/
--rw-r--r--   0 runner    (1001) docker     (123)    82085 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/data/oresat_app.eds
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/master_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.905580 oresat-olaf-2.0.1/olaf/_internals/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/ecss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/file_caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/fread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/fwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/os_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/power_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/store_eds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/system_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.905580 oresat-olaf-2.0.1/olaf/_internals/rest_api/
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.905580 oresat-olaf-2.0.1/olaf/_internals/rest_api/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.909580 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/fread.html
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/fwrite.html
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/logs.html
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/od.html
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/os_command.html
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/power_control.html
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/root.html
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/system_info.html
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/updater.html
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.909580 oresat-olaf-2.0.1/olaf/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/common/cpufreq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/common/ecss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/common/gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/common/oresat_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/common/oresat_file_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/common/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/common/timer_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.913580 oresat-olaf-2.0.1/olaf/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2482 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/scripts/file_transfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1832 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/scripts/new_eds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1212 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/scripts/os_command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5444 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/scripts/sdo_transfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/scripts/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3541 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/scripts/system_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.913580 oresat-olaf-2.0.1/oresat_olaf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-04 23:18:36.000000 oresat-olaf-2.0.1/oresat_olaf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-04 23:18:36.000000 oresat-olaf-2.0.1/oresat_olaf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 23:18:36.000000 oresat-olaf-2.0.1/oresat_olaf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-04 23:18:36.000000 oresat-olaf-2.0.1/oresat_olaf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 23:18:36.000000 oresat-olaf-2.0.1/oresat_olaf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 23:18:36.000000 oresat-olaf-2.0.1/oresat_olaf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-04 23:18:36.917580 oresat-olaf-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.913580 oresat-olaf-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.917580 oresat-olaf-2.0.1/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/common/test_ecss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/common/test_oresat_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/common/test_oresat_file_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.917580 oresat-olaf-2.0.1/tests/internals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.917580 oresat-olaf-2.0.1/tests/internals/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/resources/test_ecss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/resources/test_file_caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/resources/test_fread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/resources/test_fwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/resources/test_os_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/resources/test_system_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.917580 oresat-olaf-2.0.1/tests/internals/updater/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/updater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/updater/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.811718 oresat-olaf-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-07 20:22:13.811718 oresat-olaf-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.791717 oresat-olaf-2.1.0/olaf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.791717 oresat-olaf-2.1.0/olaf/_internals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.791717 oresat-olaf-2.1.0/olaf/_internals/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    82085 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/data/oresat_app.eds
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/master_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16950 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.795717 oresat-olaf-2.1.0/olaf/_internals/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/file_caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/fread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/fwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/os_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/power_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/store_eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/system_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/resources/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.795717 oresat-olaf-2.1.0/olaf/_internals/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.799717 oresat-olaf-2.1.0/olaf/_internals/rest_api/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.799717 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/fread.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/fwrite.html
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/od.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/os_command.html
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/power_control.html
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/root.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/system_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/updater.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/_internals/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.803717 oresat-olaf-2.1.0/olaf/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/common/cpufreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/common/ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/common/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/common/oresat_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/common/oresat_file_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/common/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/common/timer_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.807718 oresat-olaf-2.1.0/olaf/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2478 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/scripts/file_transfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1832 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/scripts/new_eds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1208 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/scripts/os_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5444 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/scripts/sdo_transfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/scripts/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3537 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/olaf/scripts/system_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.807718 oresat-olaf-2.1.0/oresat_olaf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-07 20:22:13.000000 oresat-olaf-2.1.0/oresat_olaf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-07 20:22:13.000000 oresat-olaf-2.1.0/oresat_olaf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:22:13.000000 oresat-olaf-2.1.0/oresat_olaf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-07 20:22:13.000000 oresat-olaf-2.1.0/oresat_olaf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-07 20:22:13.000000 oresat-olaf-2.1.0/oresat_olaf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 20:22:13.000000 oresat-olaf-2.1.0/oresat_olaf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-07 20:22:13.815718 oresat-olaf-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.807718 oresat-olaf-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.807718 oresat-olaf-2.1.0/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/common/test_ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/common/test_oresat_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/common/test_oresat_file_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/common/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.811718 oresat-olaf-2.1.0/tests/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.811718 oresat-olaf-2.1.0/tests/internals/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/resources/test_ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/resources/test_file_caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/resources/test_fread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/resources/test_fwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/resources/test_os_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/resources/test_system_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/test_rest_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:13.811718 oresat-olaf-2.1.0/tests/internals/updater/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/updater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-05-07 20:22:03.000000 oresat-olaf-2.1.0/tests/internals/updater/test_updater.py
```

### Comparing `oresat-olaf-2.0.1/LICENSE` & `oresat-olaf-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/PKG-INFO` & `oresat-olaf-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-olaf
-Version: 2.0.1
+Version: 2.1.0
 Summary: Application framework for all OreSat Linux boards
 Home-page: https://github.com/oresat/oresat-olaf
 Author: PSAS
 Author-email: oresat@pdx.edu
 Maintainer: PSAS
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
```

### Comparing `oresat-olaf-2.0.1/README.rst` & `oresat-olaf-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/__init__.py` & `oresat-olaf-2.1.0/olaf/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .common.resource import Resource
 from .common.ecss import scet_int_from_time, scet_int_to_time, utc_int_from_time, utc_int_to_time
 from .common.oresat_file import OreSatFile, new_oresat_file
 from .common.oresat_file_cache import OreSatFileCache
 from .common.timer_loop import TimerLoop
 from .common.gpio import GPIO
 
-__version__ = '2.0.1'
+__version__ = '2.1.0'
 
 
 def olaf_setup(eds_path: str = None, master_node: bool = False) -> Namespace:
     '''
     Parse runtime args and setup the app and REST API.
 
     Parameters
@@ -49,29 +49,27 @@
                         help='rest api address, defaults to localhost')
     parser.add_argument('-p', '--port', type=int, default=8000,
                         help='rest api port number, defaults to 8000')
     args = parser.parse_args()
 
     if args.verbose:
         level = 'DEBUG'
-        backtrace = True
     else:
         level = 'INFO'
-        backtrace = False
 
     logger.remove()  # remove default logger
     if args.log:
-        logger.add(SysLogHandler(address='/dev/log'), level=level, backtrace=backtrace)
+        logger.add(SysLogHandler(address='/dev/log'), level=level, backtrace=True)
     else:
-        logger.add(sys.stdout, level=level, backtrace=backtrace)
+        logger.add(sys.stdout, level=level, backtrace=True)
 
     olaf_boot_logs = '/tmp/olaf.log'
     if os.path.isfile(olaf_boot_logs):
         os.remove(olaf_boot_logs)
-    logger.add(olaf_boot_logs, level=level, backtrace=backtrace)
+    logger.add(olaf_boot_logs, level=level, backtrace=True)
 
     if eds_path is None:
         eds_path = args.eds
 
     app.setup(eds_path, args.bus, args.node_id, master_node=master_node)
     rest_api.setup(address=args.address, port=args.port)
```

### Comparing `oresat-olaf-2.0.1/olaf/_internals/app.py` & `oresat-olaf-2.1.0/olaf/_internals/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,19 +30,18 @@
     '''
 
     _BACKUP_EDS = abspath(dirname(__file__)) + '/data/oresat_app.eds'
     '''Internal eds file incase app's is misformatted or missing.'''
 
     def __init__(self):
 
+        self._od = None
         self._bus = None
         self._resources = []
-        self._network = None
         self._node = None
-        self._app_node = None
         self._updater = None
         self._factory_reset_cb = None
 
         # setup event
         for sig in ['SIGTERM', 'SIGHUP', 'SIGINT']:
             signal.signal(getattr(signal, sig), self._quit)
 
@@ -52,26 +51,29 @@
 
     def _quit(self, signo, _frame):
         '''Called when signals are caught'''
 
         logger.debug(f'signal {signal.Signals(signo).name} was caught')
         self.stop()
 
-    def _load_node(self, node_id: int, eds: str):
+    def _load_od(self, node_id: int, eds: str):
 
-        dcf_node_id = canopen.import_od(eds).node_id
+        self._od = canopen.objectdictionary.eds.import_eds(eds, node_id)
+
+        dcf_node_id = self._od.node_id
         if node_id != 0:
             self._node_id = node_id
         elif dcf_node_id:
             self._node_id = dcf_node_id
         else:
             self._node_id = 0x7C
-        self._node = canopen.LocalNode(self._node_id, eds)
-        self._node.object_dictionary.node_id = self._node_id
-        self._node.object_dictionary.bitrate = 1_000_000  # oresat node will always have 1 Mbps
+
+        # make sure these are set
+        self._od.node_id = self._node_id
+        self._od.bitrate = 1_000_000  # oresat node will always have 1 Mbps
 
     def setup(self, eds: str, bus: str, node_id: [int, str] = 0, master_node: bool = False):
         '''
         Setup the app. Will be called by ``olaf_setup`` automatically.
 
         Parameters
         ----------
@@ -97,35 +99,35 @@
             else:
                 node_id = int(node_id)
         elif not isinstance(node_id, int):
             raise ValueError('node_id is not a int/hex str or a int')
 
         if eds is not None:
             try:
-                self._load_node(node_id, eds)
+                self._load_od(node_id, eds)
             except Exception as e:
-                logger.error(f'{e.__class__.__name__}: {e}')
+                logger.exception(f'{e.__class__.__name__}: {e}')
                 logger.warning(f'failed to read in {eds}, using OLAF\'s internal eds as backup')
                 eds = self._BACKUP_EDS
-                self._load_node(node_id, eds)
+                self._load_od(node_id, eds)
         else:
             logger.warning('No eds or dcf was supplied, using OLAF\'s internal eds')
             eds = self._BACKUP_EDS
-            self._load_node(node_id, eds)
+            self._load_od(node_id, eds)
 
-        self._name = self._node.object_dictionary.device_information.product_name
+        self._name = self._od.device_information.product_name
 
         if master_node:
-            self._app_node = MasterNode(self._node, bus)
+            self._node = MasterNode(self._od, bus)
         else:
-            self._app_node = Node(self._node, bus)
+            self._node = Node(self._od, bus)
 
         # setup updater
-        self._updater = Updater(f'{self._app_node.work_base_dir}/updater',
-                                f'{self._app_node.cache_base_dir}/updates')
+        self._updater = Updater(f'{self._node.work_base_dir}/updater',
+                                f'{self._node.cache_base_dir}/updates')
 
         # default resources
         self.add_resource(OSCommandResource())
         self.add_resource(ECSSResource())
         self.add_resource(SystemInfoResource())
         self.add_resource(FileCachesResource())
         self.add_resource(FreadResource())
@@ -144,52 +146,52 @@
         resource: Resource
             The resource to add.
         '''
 
         self._resources.append(resource)
 
     def run(self):
-        logger.info(f'{self._app_node.name} app is starting')
+        logger.info(f'{self._node.name} app is starting')
 
         for resource in self._resources:
-            resource.start(self._app_node)
+            resource.start(self._node)
 
-        if self._app_node:
+        if self._node:
             try:
-                reset = self._app_node.run()
+                reset = self._node.run()
             except Exception as e:
-                logger.critical(f'unexpected error was raised by app node: {e}')
+                logger.exception(f'unexpected error was raised by app node: {e}')
                 reset = NodeStop.SOFT_RESET
 
         for resource in self._resources:
             resource.end()
 
-        logger.info(f'{self._app_node.name} app has ended')
+        logger.info(f'{self._node.name} app has ended')
 
         if reset == NodeStop.HARD_RESET:
             logger.info('hard reseting the system')
 
             if os.geteuid() == 0:  # running as root
                 subprocess.run('reboot', shell=True)
             else:
                 logger.error('not running as root, cannot reboot the system')
         elif reset == NodeStop.FACTORY_RESET:
             logger.info('factory reseting the system')
 
             # clear caches
-            self._app_node.fread_cache.clear()
-            self._app_node.fwrite_cache.clear()
+            self._node.fread_cache.clear()
+            self._node.fwrite_cache.clear()
             self._updater.clear_cache()
 
             # run custom factory reset function
             try:
                 if self._factory_reset_cb:
                     self._factory_reset_cb()
             except Exception as e:
-                logger.error(f'custom factory reset function raised: {e}')
+                logger.exception(f'custom factory reset function raised: {e}')
 
             if os.geteuid() == 0:  # running as root
                 subprocess.run('reboot', shell=True)
             else:
                 logger.error('not running as root, cannot reboot the system')
         elif reset == NodeStop.POWER_OFF:
             logger.info('powering off the system')
@@ -198,20 +200,20 @@
                 subprocess.run('poweroff', shell=True)
             else:
                 logger.error('not running as root, cannot power off the system')
 
     def stop(self):
         '''End the run loop'''
 
-        if self._app_node:
-            self._app_node.stop()
+        if self._node:
+            self._node.stop()
 
     @property
-    def node(self) -> Node:
-        return self._app_node
+    def node(self) -> Node or MasterNode:
+        return self._node
 
     def set_factory_reset_callback(self, cb_func):
         '''Set a custom factory reset callback function.'''
 
         self._factory_reset_cb = cb_func
```

### Comparing `oresat-olaf-2.0.1/olaf/_internals/data/oresat_app.eds` & `oresat-olaf-2.1.0/olaf/_internals/data/oresat_app.eds`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/_internals/master_node.py` & `oresat-olaf-2.1.0/olaf/_internals/master_node.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,42 @@
+from time import time
+
 import canopen
 from loguru import logger
 
 from .node import Node, NetworkError
 
 
 class MasterNode(Node):
     '''OreSat CANopen Master Node'''
 
-    def __init__(self, node: canopen.LocalNode, bus: str):
+    def __init__(self, od: canopen.ObjectDictionary, bus: str):
         '''
         Parameters
         ----------
-        node: canopen.LocalNode
-            The canopen node obj this class wraps around.
+        od: canopen.ObjectDictionary
+            The CANopen ObjectDictionary
         bus: str
             Which CAN bus to use.
         '''
 
-        super().__init__(node, bus)
+        super().__init__(od, bus)
 
         self.node_status = {}
         for i in range(0x01, 0x80):
-            if i == self._node.object_dictionary.node_id:
+            if i == self._od.node_id:
                 continue  # skip itself
-            self.node_status[i] = 0xFF  # a flag, not a CANopen standard
+            self.node_status[i] = (0xFF, time())  # 0xFF is a flag, not a CANopen standard
 
     def _restart_network(self):
         '''Restart the CANopen network'''
         super()._restart_network()
 
         for i in range(0x01, 0x80):
-            if i == self._node.object_dictionary.node_id:
+            if i == self._od.node_id:
                 continue  # skip itself
             self._network.subscribe(0x80 + i, self._on_emergency)
             self._network.subscribe(0x700 + i, self._on_heartbeat)
 
     def _on_heartbeat(self, cob_id: int, data: bytes, timestamp: float):
         '''Callback on node hearbeat messages.'''
```

### Comparing `oresat-olaf-2.0.1/olaf/_internals/node.py` & `oresat-olaf-2.1.0/olaf/_internals/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,32 +28,34 @@
 class NetworkError(Exception):
     '''Error with the CANopen network / bus'''
 
 
 class Node:
     '''OreSat CANopen Node'''
 
-    def __init__(self, node: canopen.LocalNode, bus: str):
+    def __init__(self, od: canopen.ObjectDictionary, bus: str):
         '''
         Parameters
         ----------
-        node: canopen.LocalNode
-            The canopen node obj this class wraps around.
+        od: canopen.ObjectDictionary
+            The CANopen ObjectDictionary
         bus: str
             Which CAN bus to use.
         '''
 
-        self._node = node
+        self._od = od
         self._bus = bus
+        self._node = None
         self._network = None
         self._event = Event()
         self._read_cbs = {}
         self._write_cbs = {}
         self._syncs = 0
         self._reset = NodeStop.SOFT_RESET
+        self._tpdo_timers = []
 
         if geteuid() == 0:  # running as root
             self.work_base_dir = '/var/lib/oresat'
             self.cache_base_dir = '/var/cache/oresat'
         else:
             self.work_base_dir = str(Path.home()) + '/.oresat'
             self.cache_base_dir = str(Path.home()) + '/.cache/oresat'
@@ -80,59 +82,21 @@
             elif self.od[i].data_type == canopen.objectdictionary.BOOLEAN:
                 # fix bools to be bools
                 self.od[i].default = bool(self.od[i].default)
                 self.od[i].value = bool(self.od[i].default)
             else:
                 self.od[i].value = self.od[i].default
 
-        if self._node.object_dictionary.node_id is None:
-            self._node.object_dictionary.node_id = 0x7C
-
-        node_id = self._node.object_dictionary.node_id
-
-        default_rpdos = [
-            0x200 + node_id,
-            0x300 + node_id,
-            0x400 + node_id,
-            0x500 + node_id
-        ]
-        default_tpdos = [
-            0x180 + node_id,
-            0x280 + node_id,
-            0x380 + node_id,
-            0x480 + node_id
-        ]
-
-        # fix COB-IDs for invaild PDOs
-        #
-        # all oresat node RPDO COB-ID follow values of 0x[2345]00 + $NODEID
-        # all oresat node TPDO COB-ID follow values of 0x[1234]80 + $NODEID
-        # this fixes the values for all 16 RPDOs/TPDOs
-        for i in range(len(self._node.rpdo)):
-            cob_id = self.od[0x1400 + i][1].default & 0xFFF
-            if cob_id in default_rpdos:
-                cob_id = 0x200 + 0x100 * (i % 4) + node_id + i // 4
-            else:
-                cob_id = self.od[0x1400 + i][1].default
-            self.od[0x1400 + i][1].value = cob_id
-        for i in range(len(self._node.tpdo)):
-            cob_id = self.od[0x1800 + i][1].default & 0xFFF
-            if cob_id in default_tpdos:
-                cob_id = 0x180 + 0x100 * (i % 4) + node_id + i // 4
-            else:
-                cob_id = self.od[0x1800 + i][1].default
-            self.od[0x1800 + i][1].value = cob_id
-
-        self._node.add_read_callback(self._on_sdo_read)
-        self._node.add_write_callback(self._on_sdo_write)
-
     def __del__(self):
 
-        self.stop()
+        # stop the monitor thread if it is running
+        if not self._event.is_set():
+            self.stop()
 
+        # stop the CANopen network
         if self._network:
             try:
                 self._network.disconnect()
             except Exception:
                 pass
 
     def _on_sync(self, cob_id: int, data: bytes, timestamp: float):
@@ -193,44 +157,27 @@
                 value_bytes = self.od[index][subindex].encode_raw(value)
 
             # pack pdo with bytes
             data += value_bytes
 
         try:
             i = self._network.send_message(cob_id, data)
-        except Exception as exc:
-            logger.error(f'TPDO{tpdo} failed with: {exc}')
+        except Exception as e:
+            logger.exception(f'TPDO{tpdo} failed with: {e}')
 
     def _tpdo_timer_loop(self, tpdo: int) -> bool:
         '''Send TPDO for TPDO loop. Can handle network errors.'''
 
         try:
             self.send_tpdo(tpdo)
         except NetworkError:
             pass
 
         return True
 
-    def _start_tpdo_timer_loops(self) -> list:
-        '''Start TPDO timer loops'''
-
-        tpdo_timers = []
-
-        for i in range(len(self._node.tpdo)):
-            transmission_type = self.od[0x1800 + i][2].default
-            event_time = self.od[0x1800 + i][5].default
-            if transmission_type in [0xFE, 0xFF] and event_time > 0:
-                t = TimerLoop(name=f'TPDO{i + 1}', loop_func=self._tpdo_timer_loop,
-                              delay=self.od[0x1800 + i][5], start_delay=self.od[0x1800 + i][3],
-                              args=(i,))
-                tpdo_timers.append(t)
-                t.start()
-
-        return tpdo_timers
-
     def _on_rpdo_update_od(self, map: canopen.pdo.base.Map):
         '''Handle parsering an RPDO'''
 
         for i in map.map_array:
             if i == 0:
                 continue
 
@@ -240,44 +187,100 @@
 
             index, subindex, size = struct.unpack('>HBB', value.to_bytes(4, 'big'))
             if isinstance(self.od[index], canopen.objectdictionary.Variable):
                 self._node.sdo[index].raw = map.map[i - 1].get_data()
             else:
                 self._node.sdo[index][subindex].raw = map.map[i - 1].get_data()
 
+    def _setup_node(self):
+        '''Create the CANopen and TPDO timer loops'''
+
+        if self._od.node_id is None:
+            self._od.node_id = 0x7C
+
+        self._node = canopen.LocalNode(self._od.node_id, self._od)
+
+        node_id = self._od.node_id
+        default_rpdos = [0x200 + node_id, 0x300 + node_id, 0x400 + node_id, 0x500 + node_id]
+        default_tpdos = [0x180 + node_id, 0x280 + node_id, 0x380 + node_id, 0x480 + node_id]
+
+        # fix COB-IDs for invaild PDOs
+        #
+        # all oresat node RPDO COB-ID follow values of 0x[2345]00 + $NODEID
+        # all oresat node TPDO COB-ID follow values of 0x[1234]80 + $NODEID
+        # this fixes the values for all 16 RPDOs/TPDOs
+        for i in range(len(self._node.rpdo)):
+            cob_id = self.od[0x1400 + i][1].default & 0xFFF
+            if cob_id in default_rpdos:
+                cob_id = 0x200 + 0x100 * (i % 4) + node_id + i // 4
+            else:
+                cob_id = self.od[0x1400 + i][1].default
+            self.od[0x1400 + i][1].value = cob_id
+        for i in range(len(self._node.tpdo)):
+            cob_id = self.od[0x1800 + i][1].default & 0xFFF
+            if cob_id in default_tpdos:
+                cob_id = 0x180 + 0x100 * (i % 4) + node_id + i // 4
+            else:
+                cob_id = self.od[0x1800 + i][1].default
+            self.od[0x1800 + i][1].value = cob_id
+
+        self._node.add_read_callback(self._on_sdo_read)
+        self._node.add_write_callback(self._on_sdo_write)
+
+        for i in range(len(self._node.tpdo)):
+            transmission_type = self.od[0x1800 + i][2].default
+            event_time = self.od[0x1800 + i][5].default
+            if transmission_type in [0xFE, 0xFF] and event_time > 0:
+                t = TimerLoop(name=f'TPDO{i + 1}', loop_func=self._tpdo_timer_loop,
+                              delay=self.od[0x1800 + i][5], start_delay=self.od[0x1800 + i][3],
+                              args=(i,))
+                self._tpdo_timers.append(t)
+                t.start()
+
+    def _destroy_node(self):
+        '''Destroy the CANopen and TPDO timer loops'''
+
+        for t in self._tpdo_timers:
+            t.stop()
+
+        self._tpdo_timers = []  # remove all
+
+        self._node = None
+
     def _restart_bus(self):
         '''Try to restart the CAN bus'''
 
         if self.first_bus_reset:
             logger.error(f'{self._bus} is down')
-            self.first_bus_reset = False
 
         if geteuid() == 0:  # running as root
             if self.first_bus_reset:
                 logger.info(f'trying to restart CAN bus {self._bus}')
-
-            out = subprocess.run(f'ip link set {self._bus} up', shell=True)
+            cmd = f'ip link set {self._bus} down;ip link set {self._bus} up'
+            out = subprocess.run(cmd, shell=True)
             if out.returncode != 0:
                 logger.error(out)
 
+        self.first_bus_reset = False
+
     def _restart_network(self):
         '''Restart the CANopen network'''
 
         logger.info('(re)starting CANopen network')
 
         self._network = canopen.Network()
         self._network.connect(bustype='socketcan', channel=self._bus)
+        self._setup_node()
         self._network.add_node(self._node)
 
         try:
-            self._node.nmt.state = 'PRE-OPERATIONAL'
             self._node.nmt.start_heartbeat(self.od[0x1017].default)
             self._node.nmt.state = 'OPERATIONAL'
-        except Exception as exc:
-            logger.error(f'failed to (re)start CANopen network with {exc}')
+        except Exception as e:
+            logger.exception(f'failed to (re)start CANopen network with {e}')
 
         self._network.subscribe(0x80, self._on_sync)
 
         # setup RPDOs callbacks
         self._node.rpdo.read()
         for i in self._node.rpdo:
             if self._node.rpdo[i].enabled:
@@ -285,16 +288,18 @@
 
     def _disable_network(self):
         '''Disable the CANopen network'''
 
         try:
             if self._network:
                 self._network.disconnect()
+            self._destroy_node()
         except Exception:
             self._network = None  # make sure the canopen network is down
+            self._node = None
 
     def _monitor_can(self):
         '''Monitor the CAN bus and CAN network'''
 
         first_bus_down = True  # flag to only log error message on first error
         self.first_bus_reset = True  # flag to only log error message on first error
         logger.info(f'{self.name} app is running')
@@ -324,37 +329,35 @@
         everything in a loop.
 
         Returns
         -------
         NodeStop
             Reset / power off condition.
         '''
-        tpdo_timers = []
 
         logger.info(f'{self.name} app is starting')
         if geteuid() != 0:  # running as root
             logger.warning('not running as root, cannot restart CAN bus if it goes down')
 
-        tpdo_timers = self._start_tpdo_timer_loops()
-
         try:
             self._monitor_can()
         except Exception as e:
-            logger.critical(e)
+            logger.exception(e)
 
-        for t in tpdo_timers:
-            t.stop()
+        # stop the node and TPDO timers
+        self._destroy_node()
 
         logger.info(f'{self.name} app has ended')
         return self._reset
 
-    def stop(self, reset: NodeStop = NodeStop.SOFT_RESET):
+    def stop(self, reset: NodeStop = None):
         '''End the run loop'''
 
-        self._reset = reset
+        if reset is not None:
+            self._reset = reset
         self._event.set()
 
     def add_sdo_read_callback(self, index: int, sdo_cb):
         '''
         Add an SDO read callback
 
         Parameters
@@ -438,15 +441,15 @@
         ret = None
 
         if index in self._read_cbs:
             for cb_func in self._read_cbs[index]:
                 try:
                     ret = cb_func(index, subindex)
                 except Exception as e:
-                    logger.error(f'sdo read cb for 0x{index:04X} 0x{subindex:02X} raised: {e}')
+                    logger.exception(f'sdo read cb for 0x{index:04X} 0x{subindex:02X} raised: {e}')
 
         return ret
 
     def _on_sdo_write(self, index: int, subindex: int, od: canopen.objectdictionary.Variable,
                       data: bytes):
         '''SDO write callback function. Gives access to the data being received on a SDO write.
 
@@ -466,28 +469,29 @@
 
         if index in self._write_cbs:
             value = od.decode_raw(data)
             for cb_func in self._write_cbs[index]:
                 try:
                     cb_func(index, subindex, value)
                 except Exception as e:
-                    logger.error(f'sdo write cb for 0x{index:04X} 0x{subindex:02X} raised: {e}')
+                    logger.exception(f'sdo write cb for 0x{index:04X} 0x{subindex:02X} raised: '
+                                     f'{e}')
 
     @property
     def name(self) -> str:
         '''str: The nodes name.'''
 
         if self._node:
             return self._node.object_dictionary.device_information.product_name
 
     @property
     def od(self) -> canopen.ObjectDictionary:
         '''canopen.ObjectDictionary: Access to the object dictionary.'''
 
-        return self._node.object_dictionary
+        return self._od
 
     @property
     def fread_cache(self) -> OreSatFileCache:
         '''OreSatFile: Cache the CANopen master node can read to.'''
 
         return self._fread_cache
```

### Comparing `oresat-olaf-2.0.1/olaf/_internals/resources/ecss.py` & `oresat-olaf-2.1.0/olaf/_internals/resources/ecss.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/_internals/resources/file_caches.py` & `oresat-olaf-2.1.0/olaf/_internals/resources/file_caches.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     def on_start(self):
 
         self.file_caches = [self.node.fread_cache, self.node.fwrite_cache]
         self.node.add_sdo_read_callback(self.index, self.on_read)
         self.node.add_sdo_write_callback(self.index, self.on_write)
 
-    def on_read(self, index, subindex):
+    def on_read(self, index: int, subindex: int):
 
         ret = None
 
         if index != self.index:
             return ret
 
         try:
@@ -58,20 +58,20 @@
             elif subindex == Subindex.FILE_NAME:
                 ret = self.file_caches[self.selector].files(self.filter)[self.iter].name
             elif subindex == Subindex.FILE_SIZE:
                 dir_name = self.file_caches[self.selector].dir
                 file_name = self.file_caches[self.selector].files(self.filter)[self.iter].name
                 file_path = f'{dir_name}/{file_name}'
                 ret = getsize(file_path)
-        except Exception as exc:
-            logger.error(exc)
+        except Exception as e:
+            logger.error(e)
 
         return ret
 
-    def on_write(self, index, subindex, value):
+    def on_write(self, index: int, subindex: int, value):
 
         if index != self.index:
             return
 
         try:
             if subindex == Subindex.CACHE_SELECTOR:
                 if value in [0, 1]:  # check for invalid input
@@ -85,9 +85,9 @@
                     logger.debug(f'file cache filter now "{self.filter}"')
             elif subindex == Subindex.ITER:
                 self.iter = value
             elif subindex == Subindex.DELETE_FILE:
                 file_name = self.file_caches[self.selector].files(self.filter)[self.iter].name
                 self.file_caches[self.selector].remove(file_name)
                 logger.info(f'deleted {file_name}')
-        except Exception as exc:
-            logger.error(exc)
+        except Exception as e:
+            logger.exception(e)
```

### Comparing `oresat-olaf-2.0.1/olaf/_internals/resources/fread.py` & `oresat-olaf-2.1.0/olaf/_internals/resources/fread.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,43 +32,43 @@
             remove(f'{self.tmp_dir}/{i}')
 
     def on_start(self):
 
         self.node.add_sdo_read_callback(self.index, self.on_read)
         self.node.add_sdo_write_callback(self.index, self.on_write)
 
-    def on_read(self, index, subindex):
+    def on_read(self, index: int, subindex: int):
 
         ret = None
 
         if index != self.index:
             return ret
 
         if subindex == Subindex.FILE_NAME:
             ret = basename(self.file_path)
         elif subindex == Subindex.CRC32:
             try:
                 with open(self.file_path, 'rb') as f:
                     ret = zlib.crc32(f.read())
-            except FileNotFoundError as exc:
-                logger.error(exc)
+            except FileNotFoundError as e:
+                logger.exception(e)
         elif subindex == Subindex.FILE_DATA:
             if not self.file_path:
                 logger.error('fread file path was not set before trying to read file data')
                 return b''
 
             try:
                 with open(self.file_path, 'rb') as f:
                     ret = f.read()
-            except FileNotFoundError as exc:
-                logger.error(exc)
+            except FileNotFoundError as e:
+                logger.exception(e)
 
         return ret
 
-    def on_write(self, index, subindex, value):
+    def on_write(self, index: int, subindex: int, value):
 
         if index != self.index:
             return
 
         if subindex == Subindex.FILE_NAME:
             try:
                 self.file_path = self.node.fread_cache.get(value, self.tmp_dir, True)
```

### Comparing `oresat-olaf-2.0.1/olaf/_internals/resources/fwrite.py` & `oresat-olaf-2.1.0/olaf/_internals/resources/fwrite.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,24 +30,24 @@
             remove(f'{self.tmp_dir}/{i}')
 
     def on_start(self):
 
         self.node.add_sdo_read_callback(self.index, self.on_read)
         self.node.add_sdo_write_callback(self.index, self.on_write)
 
-    def on_read(self, index, subindex, value):
+    def on_read(self, index: int, subindex: int):
 
         ret = None
 
         if index == self.index and subindex == Subindex.FILE_NAME:
             ret = basename(self.file_path)
 
         return ret
 
-    def on_write(self, index, subindex, value):
+    def on_write(self, index: int, subindex: int, value):
 
         if index != self.index:
             return
 
         if subindex == Subindex.FILE_NAME:
             try:
                 OreSatFile(value)  # valiate file name format
@@ -62,14 +62,14 @@
                 return
 
             try:
                 with open(self.file_path, 'wb') as f:
                     f.write(value)
                 logger.info(f'receive new file: {basename(self.file_path)}')
                 self.node.fwrite_cache.add(self.file_path, consume=True)
-            except Exception as exc:
-                logger.error(exc)
+            except Exception as e:
+                logger.exception(e)
 
             self.file_path = ''
 
             # clear buffers to not waste memory
             self.node.od[index][subindex].value = ''
```

### Comparing `oresat-olaf-2.0.1/olaf/_internals/resources/logs.py` & `oresat-olaf-2.1.0/olaf/_internals/resources/logs.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/_internals/resources/os_command.py` & `oresat-olaf-2.1.0/olaf/_internals/resources/os_command.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,30 +70,31 @@
 
     def _loop_error(self, exc: Exception):
 
         self.failed = True
         self.command = ''
         self.state = OSCommandState.ERROR_NO_REPLY
         self.reply = ''
+        logger.exception(exc)
 
-    def on_read(self, index, subindex):
+    def on_read(self, index: int, subindex: int):
 
         ret = None
 
         if index == self.index and not self.failed:
             if subindex == self.sub_command:
                 ret = self.command.encode()
             elif subindex == self.sub_state:
                 ret = self.state.value
             elif subindex == self.sub_reply:
                 ret = self.reply.encode()
 
         return ret
 
-    def on_write(self, index, subindex, value):
+    def on_write(self, index: int, subindex: int, value):
 
         if index == self.index and subindex == self.sub_command:
             if self.state == OSCommandState.EXECUTING or self.failed:
                 logger.eror('cannot start another os command when one is running')
                 return
 
             self.reply = ''
```

### Comparing `oresat-olaf-2.0.1/olaf/_internals/resources/power_control.py` & `oresat-olaf-2.1.0/olaf/_internals/resources/power_control.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/_internals/resources/store_eds.py` & `oresat-olaf-2.1.0/olaf/_internals/resources/store_eds.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/_internals/resources/system_info.py` & `oresat-olaf-2.1.0/olaf/_internals/resources/system_info.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/_internals/resources/updater.py` & `oresat-olaf-2.1.0/olaf/_internals/resources/updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,16 @@
         for i in self.node.fwrite_cache.files('update'):
             self._updater.add_update(self.node.fwrite_cache.dir + '/' + i)
 
         # check for flag to start a update
         if self.update_obj.value:
             try:
                 self._updater.update()
-            except UpdaterError as exc:
-                logger.critical(exc)
+            except UpdaterError as e:
+                logger.exception(e)
             self.update_obj.value = False
 
         # check for flag to make a status archive
         if self.make_status_obj.value:
             status_archive_file_path = self._updater.make_status_archive()
             self.node.fread_cache.add(status_archive_file_path, consume=True)
             self.make_status_obj.value = False
```

### Comparing `oresat-olaf-2.0.1/olaf/_internals/rest_api/__init__.py` & `oresat-olaf-2.1.0/olaf/_internals/rest_api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import base64
 import shutil
+import logging
 from enum import IntEnum
 from pathlib import Path
 from threading import Thread
 
 import canopen
 from flask import Flask, render_template, jsonify, request, send_from_directory
 from loguru import logger
@@ -53,16 +54,16 @@
     An optional Flask app for reading and writing values into the OD.
 
     Use the global ``olaf.rest_api`` object.
     '''
 
     def __init__(self):
 
-        self.app = Flask(_TITLE, template_folder=_TEMPLATE_DIR,
-                         static_folder=f'{_PATH}/static')
+        self.app = Flask(_TITLE, template_folder=_TEMPLATE_DIR, static_folder=f'{_PATH}/static')
+        logging.getLogger('werkzeug').setLevel(logging.ERROR)
         self._thread = Thread(target=self._run)
         self._server = None
         self._ctx = None
         Path(_TEMPLATE_DIR).mkdir(parents=True, exist_ok=True)
 
         # add all core templates
         for i in os.listdir(f'{_PATH}/templates'):
@@ -145,15 +146,18 @@
     path = os.path.dirname(os.path.abspath(__file__))
     return send_from_directory(f'{path}/static', 'favicon.ico')
 
 
 @rest_api.app.route('/od/<index>/', methods=['GET', 'PUT'])
 def od_index(index: str):
 
-    index = int(index, 16) if index.startswith('0x') else int(index)
+    try:
+        index = int(index, 16) if index.startswith('0x') else int(index)
+    except ValueError:
+        return jsonify({'error': f'invalid index {index}'})
 
     try:
         obj = app.node.od[index]
     except Exception:
         msg = f'no object at index {index:02X}'
         logger.error(f'RestApiError: {msg}')
         return jsonify({'error': msg})
@@ -169,16 +173,19 @@
 
     return jsonify(object_to_json(index))
 
 
 @rest_api.app.route('/od/<index>/<subindex>/', methods=['GET', 'PUT'])
 def od_subindex(index: str, subindex: str):
 
-    index = int(index, 16) if index.startswith('0x') else int(index)
-    subindex = int(subindex, 16) if subindex.startswith('0x') else int(subindex)
+    try:
+        index = int(index, 16) if index.startswith('0x') else int(index)
+        subindex = int(subindex, 16) if subindex.startswith('0x') else int(subindex)
+    except ValueError:
+        return jsonify({'error': f'invalid index {index} or subindex {subindex}'})
 
     try:
         obj = app.node.od[index][subindex]
     except Exception:
         msg = f'no object at index {index:04X} subindex {subindex:02X}'
         logger.error(f'RestApiError: {msg}')
         return jsonify({'error': msg})
```

### Comparing `oresat-olaf-2.0.1/olaf/_internals/rest_api/static/favicon.ico` & `oresat-olaf-2.1.0/olaf/_internals/rest_api/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/base.html` & `oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/base.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/fread.html` & `oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/fread.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/fwrite.html` & `oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/fwrite.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/logs.html` & `oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/logs.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/od.html` & `oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/od.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/os_command.html` & `oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/os_command.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/power_control.html` & `oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/power_control.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/system_info.html` & `oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/system_info.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/updater.html` & `oresat-olaf-2.1.0/olaf/_internals/rest_api/templates/updater.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/_internals/updater.py` & `oresat-olaf-2.1.0/olaf/_internals/updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,37 +189,37 @@
             logger.info('no update to resume or in cache')
             self._state = UpdaterState.UPDATE_SUCCESSFUL
             return
 
         logger.info('extracting files from update')
         try:
             self._extract_update_archive(update_archive_file_path)
-        except Exception as exc:
-            logger.error(exc)
+        except Exception as e:
+            logger.exception(e)
             self._clear_work_dir()
             self._state = UpdaterState.PRE_UPDATE_FAILED
             return
 
         logger.info('reading instructions file')
         try:
             commands = self._read_instructions()
-        except Exception as exc:
-            logger.error(exc)
+        except Exception as e:
+            logger.exception(e)
             self._clear_work_dir()
             self._state = UpdaterState.PRE_UPDATE_FAILED
             return
 
         logger.info('running instructions')
         try:
             # No turn back point, the update is starting!!!
             # If anything fails/errors the board's software could break.
             # All errors are log at critical level.
             self._run_instructions(commands)
-        except Exception as exc:
-            logger.critical(exc)
+        except Exception as e:
+            logger.exception(e)
             self._clear_work_dir()
             self._cache.clear()
             self._state = UpdaterState.UPDATE_FAILED
             return
 
         logger.info(f'update {self._update_archive} was successful')
         self._clear_work_dir()
```

### Comparing `oresat-olaf-2.0.1/olaf/common/cpufreq.py` & `oresat-olaf-2.1.0/olaf/common/cpufreq.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/common/ecss.py` & `oresat-olaf-2.1.0/olaf/common/ecss.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/common/gpio.py` & `oresat-olaf-2.1.0/olaf/common/gpio.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/common/oresat_file.py` & `oresat-olaf-2.1.0/olaf/common/oresat_file.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/common/oresat_file_cache.py` & `oresat-olaf-2.1.0/olaf/common/oresat_file_cache.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/common/resource.py` & `oresat-olaf-2.1.0/olaf/common/resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,30 +21,30 @@
         '''
 
         logger.debug(f'starting resource {self.__class__.__name__}')
         self.node = node
 
         try:
             self.on_start()
-        except Exception as exc:
-            logger.critical(f'{self.__class__.__name__}\'s on_start raised an uncaught exception:'
-                            f'{exc}')
+        except Exception as e:
+            logger.exception(f'{self.__class__.__name__}\'s on_start raised an uncaught exception:'
+                             f'{e}')
 
     def end(self):
         '''
         App will call this to stop the resource. This will call `self.on_end()`.
         '''
 
         logger.debug(f'stopping resource {self.__class__.__name__}')
 
         try:
             self.on_end()
-        except Exception as exc:
-            logger.critical(f'{self.__class__.__name__}\'s on_end raised an uncaught exception:'
-                            f' {exc}')
+        except Exception as e:
+            logger.exception(f'{self.__class__.__name__}\'s on_end raised an uncaught exception:'
+                             f'{e}')
 
     def on_start(self) -> None:
         '''
         Start the resource.
         '''
 
         pass
```

### Comparing `oresat-olaf-2.0.1/olaf/common/timer_loop.py` & `oresat-olaf-2.1.0/olaf/common/timer_loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,22 +66,22 @@
         elif not isinstance(self._start_delay, Variable) and self._start_delay > 0:
             self._event.wait(self._start_delay / 1000)
 
         ret = True
         while ret is True and not self._event.is_set():
             try:
                 ret = self._loop_func(*self._args)
-            except Exception as exc:
+            except Exception as e:
                 self._event.set()
-                logger.error(f'{self._name} timer loop loop_func raise: {exc}')
+                logger.exception(f'{self._name} timer loop loop_func raise: {e}')
                 if self._exc_func:
                     try:
-                        self._exc_func(exc)
-                    except Exception:
-                        logger.error(f'{self._name} timer loop exc_func raise: {exc}')
+                        self._exc_func(e)
+                    except Exception as e:
+                        logger.exception(f'{self._name} timer loop exc_func raise: {e}')
 
             if isinstance(self._delay, Variable):
                 self._event.wait(self._delay.value / 1000)
             else:
                 self._event.wait(self._delay / 1000)
 
     def stop(self):
```

### Comparing `oresat-olaf-2.0.1/olaf/scripts/file_transfer.py` & `oresat-olaf-2.1.0/olaf/scripts/file_transfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         elif args.read_file is not None:
             read_file(node, args.read_file)
         elif args.write_file is not None:
             write_file(node, args.write_file)
         else:
             print('invalid mode')
             sys.exit(1)
-    except Exception as exc:
-        print(exc)
+    except Exception as e:
+        print(e)
 
     network.disconnect()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `oresat-olaf-2.0.1/olaf/scripts/new_eds.py` & `oresat-olaf-2.1.0/olaf/scripts/new_eds.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/scripts/os_command.py` & `oresat-olaf-2.1.0/olaf/scripts/os_command.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     network = canopen.Network()
     node = canopen.RemoteNode(int(args.node, 16), EDS_FILE)
     network.add_node(node)
     network.connect(bustype='socketcan', channel=args.bus)
 
     try:
         node.sdo[OS_COMMAND_INDEX][1].raw = args.command.encode('utf-8')
-    except Exception as exc:
-        print(exc)
+    except Exception as e:
+        print(e)
         return
 
     while node.sdo[OS_COMMAND_INDEX][2].phys == 0xFF:
         sleep(0.1)
 
     print('status: ' + hex(node.sdo[OS_COMMAND_INDEX][2].phys))
     print('reply:\n\n' + node.sdo[OS_COMMAND_INDEX][3].raw.decode('utf-8'))
```

### Comparing `oresat-olaf-2.0.1/olaf/scripts/sdo_transfer.py` & `oresat-olaf-2.1.0/olaf/scripts/sdo_transfer.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/olaf/scripts/system_info.py` & `oresat-olaf-2.1.0/olaf/scripts/system_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     network = canopen.Network()
     node = canopen.RemoteNode(int(args.node, 16), EDS_FILE)
     network.add_node(node)
     network.connect(bustype='socketcan', channel=args.bus)
 
     try:
         system_info_record = node.sdo[SYSTEM_INFO_INDEX]
-    except Exception as exc:
-        print(exc)
+    except Exception as e:
+        print(e)
         return
 
     print('')
 
     os_name = system_info_record[1].phys
     os_distro = system_info_record[2].phys
     kernel_ver = system_info_record[3].phys
```

### Comparing `oresat-olaf-2.0.1/oresat_olaf.egg-info/PKG-INFO` & `oresat-olaf-2.1.0/oresat_olaf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-olaf
-Version: 2.0.1
+Version: 2.1.0
 Summary: Application framework for all OreSat Linux boards
 Home-page: https://github.com/oresat/oresat-olaf
 Author: PSAS
 Author-email: oresat@pdx.edu
 Maintainer: PSAS
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
```

### Comparing `oresat-olaf-2.0.1/oresat_olaf.egg-info/SOURCES.txt` & `oresat-olaf-2.1.0/oresat_olaf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,17 @@
 oresat_olaf.egg-info/requires.txt
 oresat_olaf.egg-info/top_level.txt
 tests/__init__.py
 tests/common/__init__.py
 tests/common/test_ecss.py
 tests/common/test_oresat_file.py
 tests/common/test_oresat_file_cache.py
+tests/common/test_resources.py
 tests/internals/__init__.py
+tests/internals/test_rest_api.py
 tests/internals/resources/__init__.py
 tests/internals/resources/test_ecss.py
 tests/internals/resources/test_file_caches.py
 tests/internals/resources/test_fread.py
 tests/internals/resources/test_fwrite.py
 tests/internals/resources/test_os_command.py
 tests/internals/resources/test_system_info.py
```

### Comparing `oresat-olaf-2.0.1/setup.cfg` & `oresat-olaf-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/tests/common/test_ecss.py` & `oresat-olaf-2.1.0/tests/common/test_ecss.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/tests/common/test_oresat_file.py` & `oresat-olaf-2.1.0/tests/common/test_oresat_file.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/tests/common/test_oresat_file_cache.py` & `oresat-olaf-2.1.0/tests/common/test_oresat_file_cache.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/tests/internals/resources/__init__.py` & `oresat-olaf-2.1.0/tests/internals/resources/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,42 +6,46 @@
 
 logger.disable('olaf')
 
 
 class MockNode(Node):
 
     def __init__(self):
-        self.node = canopen.LocalNode(0x10, 'olaf/_internals/data/oresat_app.eds')
-        super().__init__(self.node, None)
+        eds_path = 'olaf/_internals/data/oresat_app.eds'
+        od = canopen.objectdictionary.eds.import_eds(eds_path, 0x10)
+        super().__init__(od, None)
 
         self._fread_cache = OreSatFileCache('/tmp/fread')
         self._fread_cache.clear()
         self._fwrite_cache = OreSatFileCache('/tmp/fwrite')
         self._fwrite_cache.clear()
 
+        self._setup_node()
+
     def send_tpdo(self, tpdo: int) -> bool:
 
         return True  # override to do nothing
 
 
 class MockApp:
 
     def __init__(self):
         super().__init__()
+
         self.node = MockNode()
 
     def add_resource(self, resource: Resource):
         '''Add the resource for testing'''
 
         self.resource = resource
 
     def sdo_read(self, index: [int, str], subindex: [None, int, str]):
         '''Call a internal SDO read for testing'''
 
-        co_node = self.node.node
+        co_node = self.node._node
         domain = canopen.objectdictionary.DOMAIN
 
         if subindex is None:
             if co_node.object_dictionary[index].data_type == domain:
                 return co_node.sdo[index].raw
             else:
                 return co_node.sdo[index].phys
@@ -50,15 +54,15 @@
                 return co_node.sdo[index][subindex].raw
             else:
                 return co_node.sdo[index][subindex].phys
 
     def sdo_write(self, index: [int, str], subindex: [None, int, str], value):
         '''Call a internal SDO write for testing'''
 
-        co_node = self.node.node
+        co_node = self.node._node
         domain = canopen.objectdictionary.DOMAIN
 
         if subindex is None:
             if co_node.object_dictionary[index].data_type == domain:
                 co_node.sdo[index].raw = value
             else:
                 co_node.sdo[index].phys = value
@@ -71,7 +75,9 @@
     def start(self):
 
         self.resource.start(self.node)
 
     def stop(self):
 
         self.resource.end()
+        self.node._destroy_node()
+        self.node.stop()
```

### Comparing `oresat-olaf-2.0.1/tests/internals/resources/test_file_caches.py` & `oresat-olaf-2.1.0/tests/internals/resources/test_file_caches.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/tests/internals/resources/test_fread.py` & `oresat-olaf-2.1.0/tests/internals/resources/test_fread.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/tests/internals/resources/test_fwrite.py` & `oresat-olaf-2.1.0/tests/internals/resources/test_fwrite.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/tests/internals/resources/test_os_command.py` & `oresat-olaf-2.1.0/tests/internals/resources/test_os_command.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/tests/internals/resources/test_system_info.py` & `oresat-olaf-2.1.0/tests/internals/resources/test_system_info.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.1/tests/internals/updater/test_updater.py` & `oresat-olaf-2.1.0/tests/internals/updater/test_updater.py`

 * *Files identical despite different names*

