# Comparing `tmp/silobuster-0.1.8.tar.gz` & `tmp/silobuster-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silobuster-0.1.8.tar", last modified: Sun May  7 05:27:57 2023, max compression
+gzip compressed data, was "silobuster-1.0.0.tar", last modified: Sun May  7 06:11:26 2023, max compression
```

## Comparing `silobuster-0.1.8.tar` & `silobuster-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:27:57.038255 silobuster-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 05:27:57.038255 silobuster-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-07 05:27:50.000000 silobuster-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 05:27:57.038255 silobuster-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-07 05:27:52.000000 silobuster-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:27:57.034255 silobuster-0.1.8/silobuster/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 05:27:52.000000 silobuster-0.1.8/silobuster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:27:57.038255 silobuster-0.1.8/silobuster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 05:27:57.000000 silobuster-0.1.8/silobuster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-07 05:27:57.000000 silobuster-0.1.8/silobuster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 05:27:57.000000 silobuster-0.1.8/silobuster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-07 05:27:57.000000 silobuster-0.1.8/silobuster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 05:27:57.000000 silobuster-0.1.8/silobuster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.709621 silobuster-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-07 06:11:16.000000 silobuster-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 06:11:26.709621 silobuster-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-07 06:11:16.000000 silobuster-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 06:11:26.709621 silobuster-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-07 06:11:18.000000 silobuster-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/ARCHIVED/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/.ipynb_checkpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/.ipynb_checkpoints/test_conn-checkpoint.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/abstract_connector.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/abstract_connector.cpython-36.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/abstract_connector.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/postgres_connector.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/postgres_connector.cpython-36.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/postgres_connector.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/abstract_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/postgres_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/test_conn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    55032 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/deduplication_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/__pycache__/abstract_feed.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/__pycache__/abstract_feed.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/__pycache__/postgres_feed.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/__pycache__/postgres_feed.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/abstract_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/postgres_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/__pycache__/uuid.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/base_classes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/base_classes/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/base_classes/__pycache__/base_iterator.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/base_classes/__pycache__/singleton.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/base_classes/base_iterator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1298 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/base_classes/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/connector/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/connector/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/base_connector.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/base_converter.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/base_convertor.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/base_source.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/dataframe_connector.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/generic_connector.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/log_formatter.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/postgres.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/postgres_connector.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/postgres_converter.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/postgres_convertor.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/base_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/dataframe_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/generic_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/postgres_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/dataframes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/dataframes/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/dataframes/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/dataframes/__pycache__/encoders.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/dataframes/__pycache__/process_dedupe.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/dataframes/__pycache__/to_types.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/dataframes/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/dataframes/map_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/dataframes/process_dedupe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/dataframes/to_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/globals/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/globals/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/globals/__pycache__/queries.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/globals/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/handler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/handler/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/__pycache__/base_db_source.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/__pycache__/base_handler.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/__pycache__/base_source.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/__pycache__/dataframe_handler.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/__pycache__/excel_handler.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/__pycache__/json_handler.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/__pycache__/postgres_handler.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/__pycache__/postgres_source.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/dataframe_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/excel_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/postgres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/log_handler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/log_handler/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/log_handler/__pycache__/log_formatter.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/log_handler/__pycache__/log_handler.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/log_handler/log_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/nodes/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/nodes/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.697620 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/__pycache__/connection_exceptions.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/__pycache__/log_exceptions.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/__pycache__/query_exceptions.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/__pycache__/type_exceptions.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/connection_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/log_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/nodes_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/query_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/type_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.697620 silobuster-1.0.0/silobuster/libs/workers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.697620 silobuster-1.0.0/silobuster/libs/workers/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/__pycache__/helpers.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.697620 silobuster-1.0.0/silobuster/libs/workers/algo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.697620 silobuster-1.0.0/silobuster/libs/workers/algo/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/algo/__pycache__/exact_address.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/algo/__pycache__/exact_identifier.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/algo/__pycache__/exact_lat_long.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/algo/__pycache__/exact_name_url.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/algo/exact_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/algo/exact_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/algo/exact_lat_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/algo/exact_name_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.697620 silobuster-1.0.0/silobuster/libs/workers/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/OLD-deduper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.697620 silobuster-1.0.0/silobuster/libs/workers/ml/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/__pycache__/names_orgs.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.697620 silobuster-1.0.0/silobuster/libs/workers/ml/addresses/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.697620 silobuster-1.0.0/silobuster/libs/workers/ml/addresses/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/addresses/__pycache__/addresses.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/addresses/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/addresses/dedupe_io_addresses_only_learned_settings
+-rw-r--r--   0 runner    (1001) docker     (123)  1623481 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/addresses/dedupe_io_addresses_only_training.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.701620 silobuster-1.0.0/silobuster/libs/workers/ml/name_street/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.701620 silobuster-1.0.0/silobuster/libs/workers/ml/name_street/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/name_street/__pycache__/addresses.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/name_street/__pycache__/name_street.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/name_street/dedupe_io_name_street_learned_settings
+-rw-r--r--   0 runner    (1001) docker     (123)  2978387 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/name_street/dedupe_io_name_street_training.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/name_street/name_street.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.705621 silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.705621 silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/__pycache__/dedupe_io_addresses.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/__pycache__/names_addresses.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/dedupe_io_addresses_learned_settings
+-rw-r--r--   0 runner    (1001) docker     (123)  2759344 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/dedupe_io_addresses_training.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/names_addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.705621 silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.705621 silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/__pycache__/names_orgs.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/__pycache__/names_urls_addresses.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/names_orgs_learned_settings
+-rw-r--r--   0 runner    (1001) docker     (123)   261631 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/names_orgs_training.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/names_urls_addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.705621 silobuster-1.0.0/silobuster/manglers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.705621 silobuster-1.0.0/silobuster/manglers/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/__pycache__/mangle_org_name.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/__pycache__/mangle_url.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/__pycache__/mangle_url.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/__pycache__/tld_swap_prob_dict.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/mangle_org_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/mangle_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.705621 silobuster-1.0.0/silobuster/manglers/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.705621 silobuster-1.0.0/silobuster/manglers/tests/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/tests/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/tests/__pycache__/test_mangle_org.cpython-39-pytest-7.1.2.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    11819 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/tests/__pycache__/test_mangle_url.cpython-39-pytest-7.1.2.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/tests/test_mangle_org.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/tests/test_mangle_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/tests/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/tld_swap_prob_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.709621 silobuster-1.0.0/silobuster/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/reports/.~lock.report_1.ods#
+-rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/reports/report_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    39465 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/reports/report_1.ods
+-rw-r--r--   0 runner    (1001) docker     (123)    17905 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/reports/report_1.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 06:11:26.000000 silobuster-1.0.0/silobuster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-05-07 06:11:26.000000 silobuster-1.0.0/silobuster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 06:11:26.000000 silobuster-1.0.0/silobuster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-07 06:11:26.000000 silobuster-1.0.0/silobuster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 06:11:26.000000 silobuster-1.0.0/silobuster.egg-info/top_level.txt
```

### Comparing `silobuster-0.1.8/README.md` & `silobuster-1.0.0/README.md`

 * *Files identical despite different names*

