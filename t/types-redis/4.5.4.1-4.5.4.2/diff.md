# Comparing `tmp/types-redis-4.5.4.1.tar.gz` & `tmp/types-redis-4.5.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-redis-4.5.4.1.tar", last modified: Thu Mar 30 01:18:44 2023, max compression
+gzip compressed data, was "types-redis-4.5.4.2.tar", last modified: Sun May  7 01:19:43 2023, max compression
```

## Comparing `types-redis-4.5.4.1.tar` & `types-redis-4.5.4.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 01:18:44.013852 types-redis-4.5.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    12359 2023-03-30 01:18:43.000000 types-redis-4.5.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-30 01:18:43.000000 types-redis-4.5.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-03-30 01:18:44.013852 types-redis-4.5.4.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 01:18:44.009852 types-redis-4.5.4.1/redis-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-30 01:18:43.000000 types-redis-4.5.4.1/redis-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 01:18:44.009852 types-redis-4.5.4.1/redis-stubs/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/asyncio/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    47443 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/asyncio/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/asyncio/cluster.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/asyncio/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/asyncio/lock.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/asyncio/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/asyncio/retry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/asyncio/sentinel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/asyncio/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/backoff.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    41553 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10838 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/cluster.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 01:18:44.013852 types-redis-4.5.4.1/redis-stubs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 01:18:44.013852 types-redis-4.5.4.1/redis-stubs/commands/bf/
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/bf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/bf/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/bf/info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/cluster.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    72157 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/core.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 01:18:44.013852 types-redis-4.5.4.1/redis-stubs/commands/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/graph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/graph/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/graph/edge.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/graph/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/graph/node.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/graph/path.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/graph/query_result.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/helpers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 01:18:44.013852 types-redis-4.5.4.1/redis-stubs/commands/json/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/json/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/json/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/json/decoders.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/json/path.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/redismodules.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 01:18:44.013852 types-redis-4.5.4.1/redis-stubs/commands/search/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/search/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/search/aggregation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/search/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/search/query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/search/result.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/sentinel.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 01:18:44.013852 types-redis-4.5.4.1/redis-stubs/commands/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/timeseries/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/timeseries/commands.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/timeseries/info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/commands/timeseries/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/crc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/credentials.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/lock.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/ocsp.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/retry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/sentinel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/typing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-03-30 01:18:26.000000 types-redis-4.5.4.1/redis-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 01:18:44.013852 types-redis-4.5.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-03-30 01:18:43.000000 types-redis-4.5.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 01:18:44.013852 types-redis-4.5.4.1/types_redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-03-30 01:18:43.000000 types-redis-4.5.4.1/types_redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-03-30 01:18:43.000000 types-redis-4.5.4.1/types_redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 01:18:43.000000 types-redis-4.5.4.1/types_redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-30 01:18:43.000000 types-redis-4.5.4.1/types_redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-30 01:18:43.000000 types-redis-4.5.4.1/types_redis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:19:43.260056 types-redis-4.5.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-05-07 01:19:42.000000 types-redis-4.5.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 01:19:42.000000 types-redis-4.5.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-07 01:19:43.260056 types-redis-4.5.4.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:19:43.252056 types-redis-4.5.4.2/redis-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-07 01:19:42.000000 types-redis-4.5.4.2/redis-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:19:43.252056 types-redis-4.5.4.2/redis-stubs/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/asyncio/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    47443 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/asyncio/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/asyncio/cluster.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/asyncio/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/asyncio/lock.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/asyncio/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/asyncio/retry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/asyncio/sentinel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/asyncio/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/backoff.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    41553 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10838 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/cluster.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:19:43.256056 types-redis-4.5.4.2/redis-stubs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:19:43.256056 types-redis-4.5.4.2/redis-stubs/commands/bf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/bf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/bf/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/bf/info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/cluster.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    72157 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/core.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:19:43.256056 types-redis-4.5.4.2/redis-stubs/commands/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/graph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/graph/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/graph/edge.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/graph/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/graph/node.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/graph/path.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/graph/query_result.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/helpers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:19:43.256056 types-redis-4.5.4.2/redis-stubs/commands/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/json/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/json/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/json/decoders.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/json/path.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/redismodules.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:19:43.256056 types-redis-4.5.4.2/redis-stubs/commands/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/search/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/search/aggregation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/search/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/search/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/search/result.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/sentinel.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:19:43.260056 types-redis-4.5.4.2/redis-stubs/commands/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/timeseries/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/timeseries/commands.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/timeseries/info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/commands/timeseries/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/crc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/credentials.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/lock.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/ocsp.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/retry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/sentinel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/typing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-07 01:19:27.000000 types-redis-4.5.4.2/redis-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 01:19:43.260056 types-redis-4.5.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-07 01:19:42.000000 types-redis-4.5.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:19:43.260056 types-redis-4.5.4.2/types_redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-07 01:19:43.000000 types-redis-4.5.4.2/types_redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-07 01:19:43.000000 types-redis-4.5.4.2/types_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 01:19:43.000000 types-redis-4.5.4.2/types_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-07 01:19:43.000000 types-redis-4.5.4.2/types_redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 01:19:43.000000 types-redis-4.5.4.2/types_redis.egg-info/top_level.txt
```

### Comparing `types-redis-4.5.4.1/CHANGELOG.md` & `types-redis-4.5.4.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 4.5.4.2 (2023-05-07)
+
+Redis: Add missing exported names (#10151)
+
 ## 4.5.4.1 (2023-03-30)
 
 [redis] Add CredentialProvider types to __init__.pyi (#9982)
 
 ## 4.5.4.0 (2023-03-29)
 
 [redis] Fix type of connection_class in ConnectionPool (#9981)
```

### Comparing `types-redis-4.5.4.1/PKG-INFO` & `types-redis-4.5.4.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-redis
-Version: 4.5.4.1
+Version: 4.5.4.2
 Summary: Typing stubs for redis
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/redis.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `redis`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/redis. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `ff3b558fb3c74d49c957a2a400d32d7319ba9dca`.
+This package was generated from typeshed commit `03e39550379b7edc78094298ea890350e386a260`.
```

### Comparing `types-redis-4.5.4.1/redis-stubs/__init__.pyi` & `types-redis-4.5.4.2/redis-stubs/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from . import client, connection, credentials, exceptions, sentinel, utils
+from . import backoff, client, connection, credentials, exceptions, sentinel, utils
 from .cluster import RedisCluster as RedisCluster
 
 __all__ = [
     "AuthenticationError",
     "AuthenticationWrongNumberOfArgsError",
     "BlockingConnectionPool",
     "BusyLoadingError",
     "ChildDeadlockedError",
     "Connection",
     "ConnectionError",
     "ConnectionPool",
     "CredentialProvider",
     "DataError",
     "from_url",
+    "default_backoff",
     "InvalidResponse",
     "PubSubError",
     "ReadOnlyError",
     "Redis",
     "RedisCluster",
     "RedisError",
     "ResponseError",
@@ -28,14 +29,16 @@
     "UsernamePasswordCredentialProvider",
     "StrictRedis",
     "TimeoutError",
     "UnixDomainSocketConnection",
     "WatchError",
 ]
 
+default_backoff = backoff.default_backoff
+
 Redis = client.Redis
 
 BlockingConnectionPool = connection.BlockingConnectionPool
 Connection = connection.Connection
 ConnectionPool = connection.ConnectionPool
 SSLConnection = connection.SSLConnection
 StrictRedis = client.StrictRedis
```

### Comparing `types-redis-4.5.4.1/redis-stubs/asyncio/__init__.pyi` & `types-redis-4.5.4.2/redis-stubs/asyncio/__init__.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from redis.asyncio.client import Redis as Redis, StrictRedis as StrictRedis
+from redis.asyncio.cluster import RedisCluster as RedisCluster
 from redis.asyncio.connection import (
     BlockingConnectionPool as BlockingConnectionPool,
     Connection as Connection,
     ConnectionPool as ConnectionPool,
     SSLConnection as SSLConnection,
     UnixDomainSocketConnection as UnixDomainSocketConnection,
 )
+from redis.asyncio.parser import CommandsParser as CommandsParser
 from redis.asyncio.sentinel import (
     Sentinel as Sentinel,
     SentinelConnectionPool as SentinelConnectionPool,
     SentinelManagedConnection as SentinelManagedConnection,
     SentinelManagedSSLConnection as SentinelManagedSSLConnection,
 )
 from redis.asyncio.utils import from_url as from_url
+from redis.backoff import default_backoff as default_backoff
 from redis.exceptions import (
     AuthenticationError as AuthenticationError,
     AuthenticationWrongNumberOfArgsError as AuthenticationWrongNumberOfArgsError,
     BusyLoadingError as BusyLoadingError,
     ChildDeadlockedError as ChildDeadlockedError,
     ConnectionError as ConnectionError,
     DataError as DataError,
@@ -31,23 +34,26 @@
 
 __all__ = [
     "AuthenticationError",
     "AuthenticationWrongNumberOfArgsError",
     "BlockingConnectionPool",
     "BusyLoadingError",
     "ChildDeadlockedError",
+    "CommandsParser",
     "Connection",
     "ConnectionError",
     "ConnectionPool",
     "DataError",
     "from_url",
+    "default_backoff",
     "InvalidResponse",
     "PubSubError",
     "ReadOnlyError",
     "Redis",
+    "RedisCluster",
     "RedisError",
     "ResponseError",
     "Sentinel",
     "SentinelConnectionPool",
     "SentinelManagedConnection",
     "SentinelManagedSSLConnection",
     "SSLConnection",
```

### Comparing `types-redis-4.5.4.1/redis-stubs/asyncio/client.pyi` & `types-redis-4.5.4.2/redis-stubs/asyncio/client.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/asyncio/cluster.pyi` & `types-redis-4.5.4.2/redis-stubs/asyncio/cluster.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/asyncio/connection.pyi` & `types-redis-4.5.4.2/redis-stubs/asyncio/connection.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/asyncio/lock.pyi` & `types-redis-4.5.4.2/redis-stubs/asyncio/lock.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/asyncio/retry.pyi` & `types-redis-4.5.4.2/redis-stubs/asyncio/retry.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/asyncio/sentinel.pyi` & `types-redis-4.5.4.2/redis-stubs/asyncio/sentinel.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/asyncio/utils.pyi` & `types-redis-4.5.4.2/redis-stubs/asyncio/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/backoff.pyi` & `types-redis-4.5.4.2/redis-stubs/backoff.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -23,7 +23,9 @@
 class EqualJitterBackoff(AbstractBackoff):
     def __init__(self, cap: float = 0.512, base: float = 0.008) -> None: ...
     def compute(self, failures: int) -> float: ...
 
 class DecorrelatedJitterBackoff(AbstractBackoff):
     def __init__(self, cap: float = 0.512, base: float = 0.008) -> None: ...
     def compute(self, failures: int) -> float: ...
+
+def default_backoff() -> EqualJitterBackoff: ...
```

### Comparing `types-redis-4.5.4.1/redis-stubs/client.pyi` & `types-redis-4.5.4.2/redis-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/cluster.pyi` & `types-redis-4.5.4.2/redis-stubs/cluster.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/__init__.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/bf/__init__.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/bf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/bf/commands.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/bf/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/bf/info.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/bf/info.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/cluster.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/cluster.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/core.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/core.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/graph/__init__.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/graph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/graph/commands.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/graph/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/graph/query_result.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/graph/query_result.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/json/__init__.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/json/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/json/commands.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/json/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/search/__init__.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/search/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/search/aggregation.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/search/aggregation.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/search/commands.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/search/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/search/query.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/search/query.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/sentinel.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/sentinel.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/timeseries/__init__.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/timeseries/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/timeseries/commands.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/timeseries/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/commands/timeseries/info.pyi` & `types-redis-4.5.4.2/redis-stubs/commands/timeseries/info.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/connection.pyi` & `types-redis-4.5.4.2/redis-stubs/connection.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/exceptions.pyi` & `types-redis-4.5.4.2/redis-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/lock.pyi` & `types-redis-4.5.4.2/redis-stubs/lock.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/ocsp.pyi` & `types-redis-4.5.4.2/redis-stubs/ocsp.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/sentinel.pyi` & `types-redis-4.5.4.2/redis-stubs/sentinel.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/typing.pyi` & `types-redis-4.5.4.2/redis-stubs/typing.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/redis-stubs/utils.pyi` & `types-redis-4.5.4.2/redis-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-redis-4.5.4.1/setup.py` & `types-redis-4.5.4.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `redis`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/redis. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `ff3b558fb3c74d49c957a2a400d32d7319ba9dca`.
+This package was generated from typeshed commit `03e39550379b7edc78094298ea890350e386a260`.
 '''.lstrip()
 
 setup(name=name,
-      version="4.5.4.1",
+      version="4.5.4.2",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/redis.md",
```

### Comparing `types-redis-4.5.4.1/types_redis.egg-info/PKG-INFO` & `types-redis-4.5.4.2/types_redis.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-redis
-Version: 4.5.4.1
+Version: 4.5.4.2
 Summary: Typing stubs for redis
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/redis.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `redis`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/redis. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `ff3b558fb3c74d49c957a2a400d32d7319ba9dca`.
+This package was generated from typeshed commit `03e39550379b7edc78094298ea890350e386a260`.
```

### Comparing `types-redis-4.5.4.1/types_redis.egg-info/SOURCES.txt` & `types-redis-4.5.4.2/types_redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

