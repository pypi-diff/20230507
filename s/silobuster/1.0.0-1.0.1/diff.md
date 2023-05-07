# Comparing `tmp/silobuster-1.0.0.tar.gz` & `tmp/silobuster-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silobuster-1.0.0.tar", last modified: Sun May  7 06:11:26 2023, max compression
+gzip compressed data, was "silobuster-1.0.1.tar", last modified: Sun May  7 06:25:20 2023, max compression
```

## Comparing `silobuster-1.0.0.tar` & `silobuster-1.0.1.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.709621 silobuster-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-07 06:11:16.000000 silobuster-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 06:11:26.709621 silobuster-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-07 06:11:16.000000 silobuster-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 06:11:26.709621 silobuster-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-07 06:11:18.000000 silobuster-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/ARCHIVED/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/.ipynb_checkpoints/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/.ipynb_checkpoints/test_conn-checkpoint.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/abstract_connector.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/abstract_connector.cpython-36.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/abstract_connector.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/postgres_connector.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/postgres_connector.cpython-36.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/postgres_connector.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/abstract_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/postgres_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/test_conn.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    55032 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/deduplication_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/__pycache__/abstract_feed.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/__pycache__/abstract_feed.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/__pycache__/postgres_feed.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/__pycache__/postgres_feed.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/abstract_feed.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/postgres_feed.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/__pycache__/uuid.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/base_classes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/base_classes/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/base_classes/__pycache__/base_iterator.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/base_classes/__pycache__/singleton.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/base_classes/base_iterator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1298 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/base_classes/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster/libs/connector/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/connector/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/base_connector.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/base_converter.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/base_convertor.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/base_source.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/dataframe_connector.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/generic_connector.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/log_formatter.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/postgres.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/postgres_connector.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/postgres_converter.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/__pycache__/postgres_convertor.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/base_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/dataframe_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/generic_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/connector/postgres_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/dataframes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/dataframes/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/dataframes/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/dataframes/__pycache__/encoders.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/dataframes/__pycache__/process_dedupe.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/dataframes/__pycache__/to_types.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/dataframes/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/dataframes/map_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/dataframes/process_dedupe.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/dataframes/to_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/globals/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/globals/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/globals/__pycache__/queries.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/globals/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/handler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/handler/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/__pycache__/base_db_source.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/__pycache__/base_handler.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/__pycache__/base_source.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/__pycache__/dataframe_handler.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/__pycache__/excel_handler.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/__pycache__/json_handler.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/__pycache__/postgres_handler.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/__pycache__/postgres_source.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/base_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/dataframe_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/excel_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/handler/postgres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/log_handler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/log_handler/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/log_handler/__pycache__/log_formatter.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/log_handler/__pycache__/log_handler.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/log_handler/log_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/nodes/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/nodes/nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.693620 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.697620 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/__pycache__/connection_exceptions.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/__pycache__/log_exceptions.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/__pycache__/query_exceptions.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/__pycache__/type_exceptions.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/connection_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/log_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/nodes_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/query_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/silobuster_exceptions/type_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.697620 silobuster-1.0.0/silobuster/libs/workers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.697620 silobuster-1.0.0/silobuster/libs/workers/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/__pycache__/helpers.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.697620 silobuster-1.0.0/silobuster/libs/workers/algo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.697620 silobuster-1.0.0/silobuster/libs/workers/algo/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/algo/__pycache__/exact_address.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/algo/__pycache__/exact_identifier.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/algo/__pycache__/exact_lat_long.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/algo/__pycache__/exact_name_url.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/algo/exact_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/algo/exact_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/algo/exact_lat_long.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/algo/exact_name_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.697620 silobuster-1.0.0/silobuster/libs/workers/ml/
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/OLD-deduper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.697620 silobuster-1.0.0/silobuster/libs/workers/ml/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/__pycache__/names_orgs.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.697620 silobuster-1.0.0/silobuster/libs/workers/ml/addresses/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.697620 silobuster-1.0.0/silobuster/libs/workers/ml/addresses/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/addresses/__pycache__/addresses.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/addresses/addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/addresses/dedupe_io_addresses_only_learned_settings
--rw-r--r--   0 runner    (1001) docker     (123)  1623481 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/addresses/dedupe_io_addresses_only_training.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.701620 silobuster-1.0.0/silobuster/libs/workers/ml/name_street/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.701620 silobuster-1.0.0/silobuster/libs/workers/ml/name_street/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/name_street/__pycache__/addresses.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/name_street/__pycache__/name_street.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/name_street/dedupe_io_name_street_learned_settings
--rw-r--r--   0 runner    (1001) docker     (123)  2978387 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/name_street/dedupe_io_name_street_training.json
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/name_street/name_street.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.705621 silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.705621 silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/__pycache__/dedupe_io_addresses.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/__pycache__/names_addresses.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/dedupe_io_addresses_learned_settings
--rw-r--r--   0 runner    (1001) docker     (123)  2759344 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/dedupe_io_addresses_training.json
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/names_addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.705621 silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.705621 silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/__pycache__/names_orgs.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/__pycache__/names_urls_addresses.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/names_orgs_learned_settings
--rw-r--r--   0 runner    (1001) docker     (123)   261631 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/names_orgs_training.json
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/names_urls_addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.705621 silobuster-1.0.0/silobuster/manglers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.705621 silobuster-1.0.0/silobuster/manglers/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/__pycache__/mangle_org_name.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/__pycache__/mangle_url.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/__pycache__/mangle_url.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/__pycache__/tld_swap_prob_dict.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/mangle_org_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/mangle_url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.705621 silobuster-1.0.0/silobuster/manglers/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.705621 silobuster-1.0.0/silobuster/manglers/tests/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/tests/__pycache__/test_mangle_org.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    11819 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/tests/__pycache__/test_mangle_url.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/tests/test_mangle_org.py
--rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/tests/test_mangle_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/tests/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/manglers/tld_swap_prob_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.709621 silobuster-1.0.0/silobuster/reports/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/reports/.~lock.report_1.ods#
--rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/reports/report_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    39465 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/reports/report_1.ods
--rw-r--r--   0 runner    (1001) docker     (123)    17905 2023-05-07 06:11:18.000000 silobuster-1.0.0/silobuster/reports/report_1.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:11:26.689619 silobuster-1.0.0/silobuster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 06:11:26.000000 silobuster-1.0.0/silobuster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-05-07 06:11:26.000000 silobuster-1.0.0/silobuster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 06:11:26.000000 silobuster-1.0.0/silobuster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-07 06:11:26.000000 silobuster-1.0.0/silobuster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 06:11:26.000000 silobuster-1.0.0/silobuster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.534376 silobuster-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-07 06:25:10.000000 silobuster-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 06:25:20.534376 silobuster-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-07 06:25:10.000000 silobuster-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 06:25:20.534376 silobuster-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-07 06:25:12.000000 silobuster-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.510376 silobuster-1.0.1/silobuster/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.510376 silobuster-1.0.1/silobuster/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.510376 silobuster-1.0.1/silobuster/libs/ARCHIVED/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.510376 silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.510376 silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/.ipynb_checkpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/.ipynb_checkpoints/test_conn-checkpoint.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.514376 silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/__pycache__/abstract_connector.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/__pycache__/abstract_connector.cpython-36.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/__pycache__/abstract_connector.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/__pycache__/postgres_connector.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/__pycache__/postgres_connector.cpython-36.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/__pycache__/postgres_connector.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/abstract_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/postgres_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/test_conn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    55032 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/ARCHIVED/deduplication_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.514376 silobuster-1.0.1/silobuster/libs/ARCHIVED/feeds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.514376 silobuster-1.0.1/silobuster/libs/ARCHIVED/feeds/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/ARCHIVED/feeds/__pycache__/abstract_feed.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/ARCHIVED/feeds/__pycache__/abstract_feed.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/ARCHIVED/feeds/__pycache__/postgres_feed.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/ARCHIVED/feeds/__pycache__/postgres_feed.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/ARCHIVED/feeds/abstract_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/ARCHIVED/feeds/postgres_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/ARCHIVED/feeds/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.514376 silobuster-1.0.1/silobuster/libs/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/__pycache__/uuid.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.514376 silobuster-1.0.1/silobuster/libs/base_classes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.514376 silobuster-1.0.1/silobuster/libs/base_classes/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/base_classes/__pycache__/base_iterator.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/base_classes/__pycache__/singleton.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/base_classes/base_iterator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1298 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/base_classes/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.514376 silobuster-1.0.1/silobuster/libs/connector/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.514376 silobuster-1.0.1/silobuster/libs/connector/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/connector/__pycache__/base_connector.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/connector/__pycache__/base_converter.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/connector/__pycache__/base_convertor.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/connector/__pycache__/base_source.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/connector/__pycache__/dataframe_connector.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/connector/__pycache__/generic_connector.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/connector/__pycache__/log_formatter.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/connector/__pycache__/postgres.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/connector/__pycache__/postgres_connector.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/connector/__pycache__/postgres_converter.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/connector/__pycache__/postgres_convertor.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/connector/base_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/connector/dataframe_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/connector/generic_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/connector/postgres_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.518376 silobuster-1.0.1/silobuster/libs/dataframes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.518376 silobuster-1.0.1/silobuster/libs/dataframes/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/dataframes/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/dataframes/__pycache__/encoders.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/dataframes/__pycache__/process_dedupe.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/dataframes/__pycache__/to_types.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/dataframes/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/dataframes/map_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/dataframes/process_dedupe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/dataframes/to_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.518376 silobuster-1.0.1/silobuster/libs/globals/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.518376 silobuster-1.0.1/silobuster/libs/globals/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/globals/__pycache__/queries.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/globals/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.518376 silobuster-1.0.1/silobuster/libs/handler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.518376 silobuster-1.0.1/silobuster/libs/handler/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/handler/__pycache__/base_db_source.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/handler/__pycache__/base_handler.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/handler/__pycache__/base_source.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/handler/__pycache__/dataframe_handler.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/handler/__pycache__/excel_handler.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/handler/__pycache__/json_handler.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/handler/__pycache__/postgres_handler.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/handler/__pycache__/postgres_source.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/handler/base_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/handler/dataframe_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/handler/excel_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/handler/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/handler/postgres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.518376 silobuster-1.0.1/silobuster/libs/log_handler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.518376 silobuster-1.0.1/silobuster/libs/log_handler/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/log_handler/__pycache__/log_formatter.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/log_handler/__pycache__/log_handler.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/log_handler/log_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.518376 silobuster-1.0.1/silobuster/libs/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/nodes/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/nodes/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.518376 silobuster-1.0.1/silobuster/libs/silobuster_exceptions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.518376 silobuster-1.0.1/silobuster/libs/silobuster_exceptions/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/silobuster_exceptions/__pycache__/connection_exceptions.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/silobuster_exceptions/__pycache__/log_exceptions.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/silobuster_exceptions/__pycache__/query_exceptions.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/silobuster_exceptions/__pycache__/type_exceptions.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/silobuster_exceptions/connection_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/silobuster_exceptions/log_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/silobuster_exceptions/nodes_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/silobuster_exceptions/query_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/silobuster_exceptions/type_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.518376 silobuster-1.0.1/silobuster/libs/workers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.518376 silobuster-1.0.1/silobuster/libs/workers/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/__pycache__/helpers.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.522376 silobuster-1.0.1/silobuster/libs/workers/algo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.522376 silobuster-1.0.1/silobuster/libs/workers/algo/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/algo/__pycache__/exact_address.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/algo/__pycache__/exact_identifier.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/algo/__pycache__/exact_lat_long.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/algo/__pycache__/exact_name_url.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    17073 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/algo/exact_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/algo/exact_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/algo/exact_lat_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/algo/exact_name_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.522376 silobuster-1.0.1/silobuster/libs/workers/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/OLD-deduper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.522376 silobuster-1.0.1/silobuster/libs/workers/ml/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/__pycache__/names_orgs.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.522376 silobuster-1.0.1/silobuster/libs/workers/ml/addresses/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.522376 silobuster-1.0.1/silobuster/libs/workers/ml/addresses/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/addresses/__pycache__/addresses.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/addresses/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/addresses/dedupe_io_addresses_only_learned_settings
+-rw-r--r--   0 runner    (1001) docker     (123)  1623481 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/addresses/dedupe_io_addresses_only_training.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.526376 silobuster-1.0.1/silobuster/libs/workers/ml/name_street/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.526376 silobuster-1.0.1/silobuster/libs/workers/ml/name_street/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/name_street/__pycache__/addresses.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/name_street/__pycache__/name_street.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/name_street/dedupe_io_name_street_learned_settings
+-rw-r--r--   0 runner    (1001) docker     (123)  2978387 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/name_street/dedupe_io_name_street_training.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/name_street/name_street.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.530376 silobuster-1.0.1/silobuster/libs/workers/ml/names_addresses/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.530376 silobuster-1.0.1/silobuster/libs/workers/ml/names_addresses/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/names_addresses/__pycache__/dedupe_io_addresses.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/names_addresses/__pycache__/names_addresses.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/names_addresses/dedupe_io_addresses_learned_settings
+-rw-r--r--   0 runner    (1001) docker     (123)  2759344 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/names_addresses/dedupe_io_addresses_training.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/names_addresses/names_addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.530376 silobuster-1.0.1/silobuster/libs/workers/ml/names_urls_addresses/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.530376 silobuster-1.0.1/silobuster/libs/workers/ml/names_urls_addresses/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/names_urls_addresses/__pycache__/names_orgs.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/names_urls_addresses/__pycache__/names_urls_addresses.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/names_urls_addresses/names_orgs_learned_settings
+-rw-r--r--   0 runner    (1001) docker     (123)   261631 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/names_urls_addresses/names_orgs_training.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/libs/workers/ml/names_urls_addresses/names_urls_addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.530376 silobuster-1.0.1/silobuster/manglers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.534376 silobuster-1.0.1/silobuster/manglers/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/manglers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/manglers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/manglers/__pycache__/mangle_org_name.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/manglers/__pycache__/mangle_url.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/manglers/__pycache__/mangle_url.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/manglers/__pycache__/tld_swap_prob_dict.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/manglers/mangle_org_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/manglers/mangle_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.534376 silobuster-1.0.1/silobuster/manglers/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.534376 silobuster-1.0.1/silobuster/manglers/tests/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/manglers/tests/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     7357 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/manglers/tests/__pycache__/test_mangle_org.cpython-39-pytest-7.1.2.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    11819 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/manglers/tests/__pycache__/test_mangle_url.cpython-39-pytest-7.1.2.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/manglers/tests/test_mangle_org.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/manglers/tests/test_mangle_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/manglers/tests/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/manglers/tld_swap_prob_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.534376 silobuster-1.0.1/silobuster/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/reports/.~lock.report_1.ods#
+-rw-r--r--   0 runner    (1001) docker     (123)    18483 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/reports/report_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    39465 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/reports/report_1.ods
+-rw-r--r--   0 runner    (1001) docker     (123)    17905 2023-05-07 06:25:12.000000 silobuster-1.0.1/silobuster/reports/report_1.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:25:20.510376 silobuster-1.0.1/silobuster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 06:25:20.000000 silobuster-1.0.1/silobuster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-05-07 06:25:20.000000 silobuster-1.0.1/silobuster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 06:25:20.000000 silobuster-1.0.1/silobuster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-07 06:25:20.000000 silobuster-1.0.1/silobuster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 06:25:20.000000 silobuster-1.0.1/silobuster.egg-info/top_level.txt
```

### Comparing `silobuster-1.0.0/README.md` & `silobuster-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/.ipynb_checkpoints/test_conn-checkpoint.ipynb` & `silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/.ipynb_checkpoints/test_conn-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/abstract_connector.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/__pycache__/abstract_connector.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/abstract_connector.cpython-36.pyc` & `silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/__pycache__/abstract_connector.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/abstract_connector.cpython-39.pyc` & `silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/__pycache__/abstract_connector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/postgres_connector.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/__pycache__/postgres_connector.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/postgres_connector.cpython-36.pyc` & `silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/__pycache__/postgres_connector.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/__pycache__/postgres_connector.cpython-39.pyc` & `silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/__pycache__/postgres_connector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/abstract_connector.py` & `silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/abstract_connector.py`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/postgres_connector.py` & `silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/postgres_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     abs_dir += '/'
 sys.path.append(abs_dir)
 sys.path.append(f'{abs_dir}connectors/')
 sys.path.append(f'{abs_dir}feeds/')
 
 
 
-from libs.connectors.abstract_connector import AbstractConnector
+from silobuster.libs.connectors.abstract_connector import AbstractConnector
 
 import psycopg2
 
 class PostgresConnector(AbstractConnector):
     
     def __init__(self, db: str, username: str, password: str, host: str, port: int):
         self.__db = db
```

### Comparing `silobuster-1.0.0/silobuster/libs/ARCHIVED/connectors/test_conn.ipynb` & `silobuster-1.0.1/silobuster/libs/ARCHIVED/connectors/test_conn.ipynb`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/ARCHIVED/deduplication_results.csv` & `silobuster-1.0.1/silobuster/libs/ARCHIVED/deduplication_results.csv`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/__pycache__/abstract_feed.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/ARCHIVED/feeds/__pycache__/abstract_feed.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/__pycache__/abstract_feed.cpython-39.pyc` & `silobuster-1.0.1/silobuster/libs/ARCHIVED/feeds/__pycache__/abstract_feed.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/__pycache__/postgres_feed.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/ARCHIVED/feeds/__pycache__/postgres_feed.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/__pycache__/postgres_feed.cpython-39.pyc` & `silobuster-1.0.1/silobuster/libs/ARCHIVED/feeds/__pycache__/postgres_feed.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/ARCHIVED/feeds/postgres_feed.py` & `silobuster-1.0.1/silobuster/libs/ARCHIVED/feeds/postgres_feed.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,16 +77,16 @@
 if abs_dir[-1] != '/':
     abs_dir += '/'
 sys.path.append(abs_dir)
 sys.path.append(f'{abs_dir}connectors/')
 sys.path.append(f'{abs_dir}feeds/')
 
 
-from libs.feeds.abstract_feed import AbstractFeed
-from libs.connectors.postgres_connector import PostgresConnector
+from silobuster.libs.feeds.abstract_feed import AbstractFeed
+from silobuster.libs.connectors.postgres_connector import PostgresConnector
 
 
 class PostgresFeed(AbstractFeed):
     
     main_key = 'organization_id'
     report_key = 'job_id'
     main_qry = '''
```

### Comparing `silobuster-1.0.0/silobuster/libs/__pycache__/uuid.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/__pycache__/uuid.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/base_classes/__pycache__/base_iterator.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/base_classes/__pycache__/base_iterator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/base_classes/__pycache__/singleton.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/base_classes/__pycache__/singleton.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/base_classes/base_iterator.py` & `silobuster-1.0.1/silobuster/libs/base_classes/base_iterator.py`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/base_classes/singleton.py` & `silobuster-1.0.1/silobuster/libs/base_classes/singleton.py`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/connector/__pycache__/base_connector.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/connector/__pycache__/base_connector.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/connector/__pycache__/base_converter.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/connector/__pycache__/base_converter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/connector/__pycache__/base_convertor.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/connector/__pycache__/base_convertor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/connector/__pycache__/base_source.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/connector/__pycache__/base_source.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/connector/__pycache__/dataframe_connector.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/connector/__pycache__/dataframe_connector.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/connector/__pycache__/generic_connector.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/connector/__pycache__/generic_connector.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/connector/__pycache__/log_formatter.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/connector/__pycache__/log_formatter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/connector/__pycache__/postgres.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/connector/__pycache__/postgres.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/connector/__pycache__/postgres_connector.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/connector/__pycache__/postgres_connector.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/connector/__pycache__/postgres_converter.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/connector/__pycache__/postgres_converter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/connector/__pycache__/postgres_convertor.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/connector/__pycache__/postgres_convertor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/connector/base_connector.py` & `silobuster-1.0.1/silobuster/libs/connector/base_connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 in a single job. Jobs are then logged and a trace of operations can be retrieved.
 
 By inheriting this class, polymorphism is ensured amongst all connectors so that code bases can expect the same interface.
 '''
 
 from abc import ABC, abstractmethod
 
-from libs.handler.base_handler import BaseHandler
-from libs.log_handler.log_handler import LogHandler
+from silobuster.libs.handler.base_handler import BaseHandler
+from silobuster.libs.log_handler.log_handler import LogHandler
 
 import pandas as pd
 
 
 class BaseConnector(ABC):
 
     @property
```

### Comparing `silobuster-1.0.0/silobuster/libs/connector/generic_connector.py` & `silobuster-1.0.1/silobuster/libs/connector/generic_connector.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 All Connectors maintain an attribute "df", or DataFrame. Functions that mutate this dataframe are passed in the "transform" method. Once a transformation is complete, the "write" method then
 handles the results by executing the output handler's execute action.
 '''
 
 import pandas as pd
 import json
 
-from libs.connector.base_connector import BaseConnector
-from libs.handler.base_handler import BaseHandler
-from libs.log_handler.log_handler import LogHandler
+from silobuster.libs.connector.base_connector import BaseConnector
+from silobuster.libs.handler.base_handler import BaseHandler
+from silobuster.libs.log_handler.log_handler import LogHandler
 
 
-from libs.uuid import random_uuid
-from libs.dataframes.to_types import to_list_of_dicts
+from silobuster.libs.uuid import random_uuid
+from silobuster.libs.dataframes.to_types import to_list_of_dicts
 
 
 HANDLER_METHODS = {
     1: 'original',
     2: 'enrich',
     3: 'join',
     10: 'transform',
```

### Comparing `silobuster-1.0.0/silobuster/libs/connector/postgres_connector.py` & `silobuster-1.0.1/silobuster/libs/connector/postgres_connector.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 '''
 Postgres connectors are used to either connect to a Postgres database or write to a Postgres database.
 '''
 
 import pandas as pd
 import json
 
-from libs.connector.generic_connector import GenericConnecter
+from silobuster.libs.connector.generic_connector import GenericConnecter
 
-from libs.log_handler.log_handler import LogHandler
-from libs.handler.postgres_handler import PostgresHandler
-from libs.handler.json_handler import JsonHandler
-from libs.handler.excel_handler import ExcelHandler
+from silobuster.libs.log_handler.log_handler import LogHandler
+from silobuster.libs.handler.postgres_handler import PostgresHandler
+from silobuster.libs.handler.json_handler import JsonHandler
+from silobuster.libs.handler.excel_handler import ExcelHandler
 
 
-from libs.uuid import random_uuid
+from silobuster.libs.uuid import random_uuid
 
-from libs.dataframes.to_types import to_list_of_dicts
+from silobuster.libs.dataframes.to_types import to_list_of_dicts
 
 class BasePostgresConnector(GenericConnecter):
     def __init__(
             self, 
             input_handler: PostgresHandler, 
             output_handler: PostgresHandler, 
             log_handler: LogHandler,
```

### Comparing `silobuster-1.0.0/silobuster/libs/dataframes/__pycache__/encoders.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/dataframes/__pycache__/encoders.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/dataframes/__pycache__/process_dedupe.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/dataframes/__pycache__/process_dedupe.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/dataframes/__pycache__/to_types.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/dataframes/__pycache__/to_types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/dataframes/encoders.py` & `silobuster-1.0.1/silobuster/libs/dataframes/encoders.py`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/dataframes/process_dedupe.py` & `silobuster-1.0.1/silobuster/libs/dataframes/process_dedupe.py`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/handler/__pycache__/base_db_source.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/handler/__pycache__/base_db_source.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/handler/__pycache__/base_handler.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/handler/__pycache__/base_handler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/handler/__pycache__/base_source.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/handler/__pycache__/base_source.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/handler/__pycache__/dataframe_handler.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/handler/__pycache__/dataframe_handler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/handler/__pycache__/excel_handler.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/handler/__pycache__/excel_handler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/handler/__pycache__/json_handler.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/handler/__pycache__/json_handler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/handler/__pycache__/postgres_handler.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/handler/__pycache__/postgres_handler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/handler/__pycache__/postgres_source.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/handler/__pycache__/postgres_source.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/handler/base_handler.py` & `silobuster-1.0.1/silobuster/libs/handler/base_handler.py`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/handler/dataframe_handler.py` & `silobuster-1.0.1/silobuster/libs/handler/dataframe_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
 Dataframe handlers return the dataframe of the connector
 '''
 
 import pandas as pd
 
-from libs.handler.base_handler import BaseHandler
+from silobuster.libs.handler.base_handler import BaseHandler
 
 
 class DataFrameHandler(BaseHandler):
     def __init__(self, df: pd.DataFrame=pd.DataFrame()):
         self.__df = df.copy(deep=True)
```

### Comparing `silobuster-1.0.0/silobuster/libs/handler/excel_handler.py` & `silobuster-1.0.1/silobuster/libs/handler/excel_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Json handlers return/serialize the connectors dataframe.
 '''
 
 import io
 
 import pandas as pd
 
-from libs.handler.base_handler import BaseHandler
+from silobuster.libs.handler.base_handler import BaseHandler
 
 
 class ExcelHandler(BaseHandler):
     def __init__(self):
         pass
```

### Comparing `silobuster-1.0.0/silobuster/libs/handler/postgres_handler.py` & `silobuster-1.0.1/silobuster/libs/handler/postgres_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 import os
 import psycopg2
 from psycopg2._psycopg import connection
 from psycopg2 import extras
 
 
-from libs.handler.base_handler import BaseDBHandler
-from libs.silobuster_exceptions.connection_exceptions import PostgresConnectionFailed
+from silobuster.libs.handler.base_handler import BaseDBHandler
+from silobuster.libs.silobuster_exceptions.connection_exceptions import PostgresConnectionFailed
 
-from libs.silobuster_exceptions.query_exceptions import PostgresQueryError
+from silobuster.libs.silobuster_exceptions.query_exceptions import PostgresQueryError
 
-from libs.globals.queries import ALLOWED_QUERIES
+from silobuster.libs.globals.queries import ALLOWED_QUERIES
 
 
 
 class PostgresHandler(BaseDBHandler):
     
     @classmethod
     def load_param(cls, param: str, env_name: str) -> str:
```

### Comparing `silobuster-1.0.0/silobuster/libs/log_handler/__pycache__/log_formatter.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/log_handler/__pycache__/log_formatter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/log_handler/__pycache__/log_handler.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/log_handler/__pycache__/log_handler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/log_handler/log_handler.py` & `silobuster-1.0.1/silobuster/libs/log_handler/log_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 Retrieving logs: The log handler retrieves the logs in various formats (i.e. dataframe, json)
 '''
 
 import pandas as pd 
 import json
 import xlsxwriter
 
-from libs.handler.base_handler import BaseHandler, BaseDBHandler
-from libs.handler.postgres_handler import PostgresHandler
-from libs.silobuster_exceptions.type_exceptions import HandlerError
-from libs.silobuster_exceptions.log_exceptions import LogTypeNotImplemented
-
-from libs.dataframes.to_types import to_list_of_dicts
-from libs.dataframes.encoders import NpEncoder
-from libs.uuid import random_uuid
+from silobuster.libs.handler.base_handler import BaseHandler, BaseDBHandler
+from silobuster.libs.handler.postgres_handler import PostgresHandler
+from silobuster.libs.silobuster_exceptions.type_exceptions import HandlerError
+from silobuster.libs.silobuster_exceptions.log_exceptions import LogTypeNotImplemented
+
+from silobuster.libs.dataframes.to_types import to_list_of_dicts
+from silobuster.libs.dataframes.encoders import NpEncoder
+from silobuster.libs.uuid import random_uuid
 
-from libs.base_classes.singleton import SingletonMeta
+from silobuster.libs.base_classes.singleton import SingletonMeta
 
-from libs.silobuster_exceptions.log_exceptions import InvalidQueryParams, LogDoesNotExist
+from silobuster.libs.silobuster_exceptions.log_exceptions import InvalidQueryParams, LogDoesNotExist
 
 
 class LOG_DESTINATION:
     DB = 1
     JSON = 2
```

### Comparing `silobuster-1.0.0/silobuster/libs/nodes/node.py` & `silobuster-1.0.1/silobuster/libs/nodes/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 
-from libs.silobuster_exceptions.nodes_exceptions import NodeException, RelationDoesNotExist
+from silobuster.libs.silobuster_exceptions.nodes_exceptions import NodeException, RelationDoesNotExist
 
 
 class Node:
     '''
     Nodes are a representation of an object that relational databases typically model as a table. Attributes are considered concrete data that are absolute or are derived by a consensus of contributor
     data sources.
```

### Comparing `silobuster-1.0.0/silobuster/libs/silobuster_exceptions/__pycache__/connection_exceptions.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/silobuster_exceptions/__pycache__/connection_exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/silobuster_exceptions/__pycache__/log_exceptions.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/silobuster_exceptions/__pycache__/log_exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/silobuster_exceptions/__pycache__/query_exceptions.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/silobuster_exceptions/__pycache__/query_exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/silobuster_exceptions/__pycache__/type_exceptions.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/silobuster_exceptions/__pycache__/type_exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/uuid.py` & `silobuster-1.0.1/silobuster/libs/uuid.py`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/__pycache__/helpers.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/workers/__pycache__/helpers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/algo/__pycache__/exact_address.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/workers/algo/__pycache__/exact_address.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/algo/__pycache__/exact_identifier.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/workers/algo/__pycache__/exact_identifier.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/algo/__pycache__/exact_lat_long.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/workers/algo/__pycache__/exact_lat_long.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/algo/__pycache__/exact_name_url.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/workers/algo/__pycache__/exact_name_url.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/algo/exact_address.py` & `silobuster-1.0.1/silobuster/libs/workers/algo/exact_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Deduplicates HSDS3 formatted addresses using exact matching on name, address_1, address_2, city, state_province, and postal_code
 '''
 
 import pandas as pd
 import numpy as np
 import pandas_dedupe
 
-from libs.uuid import random_uuid
+from silobuster.libs.uuid import random_uuid
 
-from libs.workers.helpers import split_addresses, add_unique_key
+from silobuster.libs.workers.helpers import split_addresses, add_unique_key
 
 
 addr2_types = [
     'rm',
     'bldg',
     'apt',
     'unit'
```

### Comparing `silobuster-1.0.0/silobuster/libs/workers/algo/exact_identifier.py` & `silobuster-1.0.1/silobuster/libs/workers/algo/exact_identifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
 Deduplicates HSDS3 formatted organization identifiers using exact match on the identifiers
 '''
 
 
 import pandas as pd
-from libs.uuid import random_uuid
+from silobuster.libs.uuid import random_uuid
 
 
 def exact_identifier(df: pd.DataFrame):
     
     df.fillna("",inplace=True)
     duplicates = pd.DataFrame(columns=[*df.columns, "original_organization_id", "original_source_organization_id", "original_name", "original_identifier"])
     uniques = pd.DataFrame(columns=[*df.columns, "cluster_id"])
```

### Comparing `silobuster-1.0.0/silobuster/libs/workers/algo/exact_lat_long.py` & `silobuster-1.0.1/silobuster/libs/workers/algo/exact_lat_long.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Deduplicates HSDS3 formatted latitude and longitude using exact matches.
 '''
 
-from libs.uuid import random_uuid
+from silobuster.libs.uuid import random_uuid
 import pandas as pd
 
 
 def exact_lat_long(df: pd.DataFrame):
 
     df.fillna("", inplace=True)
     df['key'] = df.apply(lambda row: str(row['name']).replace(' ', '').lower().strip() + str(row['latitude']) + str(row['longitude']), axis = 1)
```

### Comparing `silobuster-1.0.0/silobuster/libs/workers/algo/exact_name_url.py` & `silobuster-1.0.1/silobuster/libs/workers/algo/exact_name_url.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Deduplicates HSDS3 formatted name and urls using exact matching urls and names.
 '''
 import pandas as pd
 
-from libs.uuid import random_uuid
+from silobuster.libs.uuid import random_uuid
 
 
 def extract_url(base_url: str):
     if not base_url:
         return ''
     
     if '//' in base_url.lower():
```

### Comparing `silobuster-1.0.0/silobuster/libs/workers/helpers.py` & `silobuster-1.0.1/silobuster/libs/workers/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import secrets
 import hashlib
 import pandas as pd
 import numpy as np
 
 
-from libs.uuid import random_uuid
+from silobuster.libs.uuid import random_uuid
 
 
 
 def split_addresses(addr1: str, addr2: str=""):
     addr1 = addr1.lower().strip()
     addr2 = addr2.lower().strip()
```

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/OLD-deduper.py` & `silobuster-1.0.1/silobuster/libs/workers/ml/OLD-deduper.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     sys.path.append('..')
 
 import pandas as pd
 import pandas_dedupe
 import csv
 import json
 
-from libs.feeds.postgres_feed import PostgresFeed
-from libs.uuid import random_uuid
+from silobuster.libs.feeds.postgres_feed import PostgresFeed
+from silobuster.libs.uuid import random_uuid
 
 
 pg_feed = PostgresFeed.from_main()
 pg_write = PostgresFeed.from_write_log()
 
 def dedupe_it():
     print ("Starting deduplication...")
```

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/__pycache__/names_orgs.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/workers/ml/__pycache__/names_orgs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/addresses/__pycache__/addresses.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/workers/ml/addresses/__pycache__/addresses.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/addresses/addresses.py` & `silobuster-1.0.1/silobuster/libs/workers/ml/addresses/addresses.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Deduplicates addresses using the dedupe.io (Pandas version) using name, address_1, address_2, city, state_province, and postal_code
 '''
 import pandas as pd
 import pandas_dedupe
 
 from inspect import getsourcefile
 from os.path import abspath
-from libs.uuid import random_uuid
+from silobuster.libs.uuid import random_uuid
 import datetime
 
-from libs.workers.helpers import split_addresses, replace_cluster_id_with_uuid
+from silobuster.libs.workers.helpers import split_addresses, replace_cluster_id_with_uuid
 
 # Make sure we are getting the absolute path to the training file!
 path_arr = abspath(getsourcefile(lambda:0)).split('/')
 path_arr.pop()
 curpath = '/'.join(path_arr)
```

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/addresses/dedupe_io_addresses_only_learned_settings` & `silobuster-1.0.1/silobuster/libs/workers/ml/addresses/dedupe_io_addresses_only_learned_settings`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/addresses/dedupe_io_addresses_only_training.json` & `silobuster-1.0.1/silobuster/libs/workers/ml/addresses/dedupe_io_addresses_only_training.json`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/name_street/__pycache__/addresses.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/workers/ml/name_street/__pycache__/addresses.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/name_street/__pycache__/name_street.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/workers/ml/name_street/__pycache__/name_street.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/name_street/dedupe_io_name_street_learned_settings` & `silobuster-1.0.1/silobuster/libs/workers/ml/name_street/dedupe_io_name_street_learned_settings`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/name_street/dedupe_io_name_street_training.json` & `silobuster-1.0.1/silobuster/libs/workers/ml/name_street/dedupe_io_name_street_training.json`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/name_street/name_street.py` & `silobuster-1.0.1/silobuster/libs/workers/ml/name_street/name_street.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 '''
 import pandas as pd
 import pandas_dedupe
 import numpy as np
 
 from inspect import getsourcefile
 from os.path import abspath
-from libs.uuid import random_uuid
+from silobuster.libs.uuid import random_uuid
 import datetime
 
-from libs.workers.helpers import split_addresses, replace_cluster_id_with_uuid
+from silobuster.libs.workers.helpers import split_addresses, replace_cluster_id_with_uuid
 
 # Make sure we are getting the absolute path to the training file!
 path_arr = abspath(getsourcefile(lambda:0)).split('/')
 path_arr.pop()
 curpath = '/'.join(path_arr)
```

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/__pycache__/dedupe_io_addresses.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/workers/ml/names_addresses/__pycache__/dedupe_io_addresses.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/__pycache__/names_addresses.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/workers/ml/names_addresses/__pycache__/names_addresses.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/dedupe_io_addresses_learned_settings` & `silobuster-1.0.1/silobuster/libs/workers/ml/names_addresses/dedupe_io_addresses_learned_settings`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/dedupe_io_addresses_training.json` & `silobuster-1.0.1/silobuster/libs/workers/ml/names_addresses/dedupe_io_addresses_training.json`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/names_addresses/names_addresses.py` & `silobuster-1.0.1/silobuster/libs/workers/ml/names_addresses/names_addresses.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 Deduplicates addresses using the dedupe.io (Pandas version) using name, address_1, address_2, city, state_province, and postal_code
 '''
 import pandas as pd
 import pandas_dedupe
 
 from inspect import getsourcefile
 from os.path import abspath
-from libs.uuid import random_uuid
+from silobuster.libs.uuid import random_uuid
 import datetime
 
-from libs.workers.helpers import split_addresses, replace_cluster_id_with_uuid
+from silobuster.libs.workers.helpers import split_addresses, replace_cluster_id_with_uuid
 
 # Make sure we are getting the absolute path to the training file!
 path_arr = abspath(getsourcefile(lambda:0)).split('/')
 path_arr.pop()
 curpath = '/'.join(path_arr)
```

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/__pycache__/names_orgs.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/workers/ml/names_urls_addresses/__pycache__/names_orgs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/__pycache__/names_urls_addresses.cpython-310.pyc` & `silobuster-1.0.1/silobuster/libs/workers/ml/names_urls_addresses/__pycache__/names_urls_addresses.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/names_orgs_learned_settings` & `silobuster-1.0.1/silobuster/libs/workers/ml/names_urls_addresses/names_orgs_learned_settings`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/names_orgs_training.json` & `silobuster-1.0.1/silobuster/libs/workers/ml/names_urls_addresses/names_orgs_training.json`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/libs/workers/ml/names_urls_addresses/names_urls_addresses.py` & `silobuster-1.0.1/silobuster/libs/workers/ml/names_urls_addresses/names_urls_addresses.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 '''
 
 import pandas as pd 
 import pandas_dedupe
 
 from inspect import getsourcefile
 from os.path import abspath
-from libs.dataframes.process_dedupe import deduplicate
-from libs.workers.helpers import replace_cluster_id_with_uuid
+from silobuster.libs.dataframes.process_dedupe import deduplicate
+from silobuster.libs.workers.helpers import replace_cluster_id_with_uuid
 
 # Make sure we are getting the absolute path to the training file!
 path_arr = abspath(getsourcefile(lambda:0)).split('/')
 path_arr.pop()
 curpath = '/'.join(path_arr)
```

### Comparing `silobuster-1.0.0/silobuster/manglers/__pycache__/mangle_org_name.cpython-39.pyc` & `silobuster-1.0.1/silobuster/manglers/__pycache__/mangle_org_name.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/manglers/__pycache__/mangle_url.cpython-310.pyc` & `silobuster-1.0.1/silobuster/manglers/__pycache__/mangle_url.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/manglers/__pycache__/mangle_url.cpython-39.pyc` & `silobuster-1.0.1/silobuster/manglers/__pycache__/mangle_url.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/manglers/mangle_org_name.py` & `silobuster-1.0.1/silobuster/manglers/mangle_org_name.py`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/manglers/mangle_url.py` & `silobuster-1.0.1/silobuster/manglers/mangle_url.py`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/manglers/tests/__pycache__/test_mangle_org.cpython-39-pytest-7.1.2.pyc` & `silobuster-1.0.1/silobuster/manglers/tests/__pycache__/test_mangle_org.cpython-39-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/manglers/tests/__pycache__/test_mangle_url.cpython-39-pytest-7.1.2.pyc` & `silobuster-1.0.1/silobuster/manglers/tests/__pycache__/test_mangle_url.cpython-39-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/manglers/tests/test_mangle_org.py` & `silobuster-1.0.1/silobuster/manglers/tests/test_mangle_org.py`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/manglers/tests/test_mangle_url.py` & `silobuster-1.0.1/silobuster/manglers/tests/test_mangle_url.py`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/manglers/tests/testing.py` & `silobuster-1.0.1/silobuster/manglers/tests/testing.py`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/manglers/tld_swap_prob_dict.py` & `silobuster-1.0.1/silobuster/manglers/tld_swap_prob_dict.py`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/reports/report_1.csv` & `silobuster-1.0.1/silobuster/reports/report_1.csv`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/reports/report_1.ods` & `silobuster-1.0.1/silobuster/reports/report_1.ods`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster/reports/report_1.xlsx` & `silobuster-1.0.1/silobuster/reports/report_1.xlsx`

 * *Files identical despite different names*

### Comparing `silobuster-1.0.0/silobuster.egg-info/SOURCES.txt` & `silobuster-1.0.1/silobuster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

