# Comparing `tmp/balpy_v2-0.1.0.tar.gz` & `tmp/balpy_v2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balpy_v2-0.1.0.tar", max compression
+gzip compressed data, was "balpy_v2-0.1.1.tar", max compression
```

## Comparing `balpy_v2-0.1.0.tar` & `balpy_v2-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,17 @@
--rw-r--r--   0        0        0       16 2023-05-06 20:47:21.807633 balpy_v2-0.1.0/README.md
--rw-r--r--   0        0        0     4404 2023-05-06 20:44:55.244682 balpy_v2-0.1.0/balpy_v2/pools/fees_report.py
--rw-r--r--   0        0        0        0 2023-05-06 16:58:15.767914 balpy_v2-0.1.0/balpy_v2/subgraphs/__init__.py
--rw-r--r--   0        0        0      829 2023-05-06 17:39:23.615885 balpy_v2-0.1.0/balpy_v2/subgraphs/balancer/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-06 17:39:49.889781 balpy_v2-0.1.0/balpy_v2/subgraphs/balancer/balancers.py
--rw-r--r--   0        0        0      741 2023-05-06 17:39:45.039892 balpy_v2-0.1.0/balpy_v2/subgraphs/balancer/pools.py
--rw-r--r--   0        0        0      800 2023-05-06 17:39:45.039906 balpy_v2-0.1.0/balpy_v2/subgraphs/balancer/tokens.py
--rw-r--r--   0        0        0     1798 2023-05-06 17:40:27.969674 balpy_v2-0.1.0/balpy_v2/subgraphs/blocks.py
--rw-r--r--   0        0        0      741 2023-05-06 17:38:41.361723 balpy_v2-0.1.0/balpy_v2/subgraphs/client.py
--rw-r--r--   0        0        0      585 2023-05-06 17:39:30.842087 balpy_v2-0.1.0/balpy_v2/subgraphs/query.py
--rw-r--r--   0        0        0      441 2023-05-06 20:47:12.952105 balpy_v2-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 balpy_v2-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-05-06 20:47:21.807633 balpy_v2-0.1.1/README.md
+-rw-r--r--   0        0        0      225 2023-05-06 15:41:22.278244 balpy_v2-0.1.1/balpy_v2/lib/__init__.py
+-rw-r--r--   0        0        0      610 2023-05-06 15:41:47.816221 balpy_v2-0.1.1/balpy_v2/lib/flatten_json.py
+-rw-r--r--   0        0        0      426 2023-05-06 16:35:00.167842 balpy_v2-0.1.1/balpy_v2/lib/gql.py
+-rw-r--r--   0        0        0      516 2023-05-06 16:34:56.094613 balpy_v2-0.1.1/balpy_v2/lib/llama/__init__.py
+-rw-r--r--   0        0        0      749 2023-05-06 15:41:45.241651 balpy_v2-0.1.1/balpy_v2/lib/time.py
+-rw-r--r--   0        0        0     4404 2023-05-06 20:44:55.244682 balpy_v2-0.1.1/balpy_v2/pools/fees_report.py
+-rw-r--r--   0        0        0        0 2023-05-06 16:58:15.767914 balpy_v2-0.1.1/balpy_v2/subgraphs/__init__.py
+-rw-r--r--   0        0        0      829 2023-05-06 17:39:23.615885 balpy_v2-0.1.1/balpy_v2/subgraphs/balancer/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-06 17:39:49.889781 balpy_v2-0.1.1/balpy_v2/subgraphs/balancer/balancers.py
+-rw-r--r--   0        0        0      741 2023-05-06 17:39:45.039892 balpy_v2-0.1.1/balpy_v2/subgraphs/balancer/pools.py
+-rw-r--r--   0        0        0      800 2023-05-06 17:39:45.039906 balpy_v2-0.1.1/balpy_v2/subgraphs/balancer/tokens.py
+-rw-r--r--   0        0        0     1798 2023-05-06 17:40:27.969674 balpy_v2-0.1.1/balpy_v2/subgraphs/blocks.py
+-rw-r--r--   0        0        0      741 2023-05-06 17:38:41.361723 balpy_v2-0.1.1/balpy_v2/subgraphs/client.py
+-rw-r--r--   0        0        0      585 2023-05-06 17:39:30.842087 balpy_v2-0.1.1/balpy_v2/subgraphs/query.py
+-rw-r--r--   0        0        0      441 2023-05-06 23:28:19.209981 balpy_v2-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 balpy_v2-0.1.1/PKG-INFO
```

### Comparing `balpy_v2-0.1.0/balpy_v2/pools/fees_report.py` & `balpy_v2-0.1.1/balpy_v2/pools/fees_report.py`

 * *Files identical despite different names*

### Comparing `balpy_v2-0.1.0/balpy_v2/subgraphs/balancer/__init__.py` & `balpy_v2-0.1.1/balpy_v2/subgraphs/balancer/__init__.py`

 * *Files identical despite different names*

### Comparing `balpy_v2-0.1.0/balpy_v2/subgraphs/balancer/balancers.py` & `balpy_v2-0.1.1/balpy_v2/subgraphs/balancer/balancers.py`

 * *Files identical despite different names*

### Comparing `balpy_v2-0.1.0/balpy_v2/subgraphs/balancer/pools.py` & `balpy_v2-0.1.1/balpy_v2/subgraphs/balancer/pools.py`

 * *Files identical despite different names*

### Comparing `balpy_v2-0.1.0/balpy_v2/subgraphs/balancer/tokens.py` & `balpy_v2-0.1.1/balpy_v2/subgraphs/balancer/tokens.py`

 * *Files identical despite different names*

### Comparing `balpy_v2-0.1.0/balpy_v2/subgraphs/blocks.py` & `balpy_v2-0.1.1/balpy_v2/subgraphs/blocks.py`

 * *Files identical despite different names*

### Comparing `balpy_v2-0.1.0/balpy_v2/subgraphs/client.py` & `balpy_v2-0.1.1/balpy_v2/subgraphs/client.py`

 * *Files identical despite different names*

### Comparing `balpy_v2-0.1.0/balpy_v2/subgraphs/query.py` & `balpy_v2-0.1.1/balpy_v2/subgraphs/query.py`

 * *Files identical despite different names*

