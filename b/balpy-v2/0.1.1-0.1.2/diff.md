# Comparing `tmp/balpy_v2-0.1.1.tar.gz` & `tmp/balpy_v2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balpy_v2-0.1.1.tar", max compression
+gzip compressed data, was "balpy_v2-0.1.2.tar", max compression
```

## Comparing `balpy_v2-0.1.1.tar` & `balpy_v2-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0       16 2023-05-06 20:47:21.807633 balpy_v2-0.1.1/README.md
--rw-r--r--   0        0        0      225 2023-05-06 15:41:22.278244 balpy_v2-0.1.1/balpy_v2/lib/__init__.py
--rw-r--r--   0        0        0      610 2023-05-06 15:41:47.816221 balpy_v2-0.1.1/balpy_v2/lib/flatten_json.py
--rw-r--r--   0        0        0      426 2023-05-06 16:35:00.167842 balpy_v2-0.1.1/balpy_v2/lib/gql.py
--rw-r--r--   0        0        0      516 2023-05-06 16:34:56.094613 balpy_v2-0.1.1/balpy_v2/lib/llama/__init__.py
--rw-r--r--   0        0        0      749 2023-05-06 15:41:45.241651 balpy_v2-0.1.1/balpy_v2/lib/time.py
--rw-r--r--   0        0        0     4404 2023-05-06 20:44:55.244682 balpy_v2-0.1.1/balpy_v2/pools/fees_report.py
--rw-r--r--   0        0        0        0 2023-05-06 16:58:15.767914 balpy_v2-0.1.1/balpy_v2/subgraphs/__init__.py
--rw-r--r--   0        0        0      829 2023-05-06 17:39:23.615885 balpy_v2-0.1.1/balpy_v2/subgraphs/balancer/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-06 17:39:49.889781 balpy_v2-0.1.1/balpy_v2/subgraphs/balancer/balancers.py
--rw-r--r--   0        0        0      741 2023-05-06 17:39:45.039892 balpy_v2-0.1.1/balpy_v2/subgraphs/balancer/pools.py
--rw-r--r--   0        0        0      800 2023-05-06 17:39:45.039906 balpy_v2-0.1.1/balpy_v2/subgraphs/balancer/tokens.py
--rw-r--r--   0        0        0     1798 2023-05-06 17:40:27.969674 balpy_v2-0.1.1/balpy_v2/subgraphs/blocks.py
--rw-r--r--   0        0        0      741 2023-05-06 17:38:41.361723 balpy_v2-0.1.1/balpy_v2/subgraphs/client.py
--rw-r--r--   0        0        0      585 2023-05-06 17:39:30.842087 balpy_v2-0.1.1/balpy_v2/subgraphs/query.py
--rw-r--r--   0        0        0      441 2023-05-06 23:28:19.209981 balpy_v2-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 balpy_v2-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      159 2023-05-07 01:57:55.534625 balpy_v2-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-06 23:56:37.544174 balpy_v2-0.1.2/balpy_v2/__init__.py
+-rw-r--r--   0        0        0      690 2023-05-07 01:58:07.689847 balpy_v2-0.1.2/balpy_v2/contracts/__init__.py
+-rw-r--r--   0        0        0     5749 2023-05-07 02:23:37.232611 balpy_v2-0.1.2/balpy_v2/contracts/utils/base_contract.py
+-rw-r--r--   0        0        0     3853 2023-05-07 02:25:57.026772 balpy_v2-0.1.2/balpy_v2/contracts/utils/contract_loader.py
+-rw-r--r--   0        0        0        0 2023-05-07 01:21:26.954072 balpy_v2-0.1.2/balpy_v2/deployments/.keep
+-rw-r--r--   0        0        0     2699 2023-05-07 01:51:00.580867 balpy_v2-0.1.2/balpy_v2/lib/__init__.py
+-rw-r--r--   0        0        0      408 2023-05-07 01:32:50.493011 balpy_v2-0.1.2/balpy_v2/lib/gql.py
+-rw-r--r--   0        0        0      516 2023-05-06 16:34:56.094613 balpy_v2-0.1.2/balpy_v2/lib/llama/__init__.py
+-rw-r--r--   0        0        0      749 2023-05-06 15:41:45.241651 balpy_v2-0.1.2/balpy_v2/lib/time.py
+-rw-r--r--   0        0        0     1098 2023-05-07 02:27:24.198362 balpy_v2-0.1.2/balpy_v2/lib/web3_provider.py
+-rw-r--r--   0        0        0        0 2023-05-06 16:58:15.767914 balpy_v2-0.1.2/balpy_v2/subgraphs/__init__.py
+-rw-r--r--   0        0        0      819 2023-05-07 02:28:30.907534 balpy_v2-0.1.2/balpy_v2/subgraphs/balancer.py
+-rw-r--r--   0        0        0     1798 2023-05-07 01:36:25.582564 balpy_v2-0.1.2/balpy_v2/subgraphs/blocks.py
+-rw-r--r--   0        0        0      658 2023-05-07 02:34:16.249461 balpy_v2-0.1.2/balpy_v2/subgraphs/client.py
+-rw-r--r--   0        0        0      789 2023-05-07 02:29:04.279522 balpy_v2-0.1.2/balpy_v2/subgraphs/gauges.py
+-rw-r--r--   0        0        0      593 2023-05-06 23:50:15.607238 balpy_v2-0.1.2/balpy_v2/subgraphs/query.py
+-rw-r--r--   0        0        0     1292 2023-05-07 02:35:05.473269 balpy_v2-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      643 1970-01-01 00:00:00.000000 balpy_v2-0.1.2/PKG-INFO
```

### Comparing `balpy_v2-0.1.1/balpy_v2/lib/llama/__init__.py` & `balpy_v2-0.1.2/balpy_v2/lib/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `balpy_v2-0.1.1/balpy_v2/lib/time.py` & `balpy_v2-0.1.2/balpy_v2/lib/time.py`

 * *Files identical despite different names*

### Comparing `balpy_v2-0.1.1/balpy_v2/subgraphs/balancer/__init__.py` & `balpy_v2-0.1.2/balpy_v2/subgraphs/balancer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from balpy_v2.lib import Chain
-from balpy_v2.subgraphs.client import SubgraphBaseClient
+from balpy_v2.subgraphs.client import GraphQLClient
 from balpy_v2.subgraphs.query import GraphQLQuery
 
 BASE_URL = "https://api.thegraph.com/subgraphs/name/balancer-labs"
 
 BALANCER_MAINNET_SUBGRAPH_URL_MAP = {
     Chain.mainnet: BASE_URL + "/balancer-v2",
     Chain.polygon: BASE_URL + "/balancer-polygon-v2",
@@ -11,15 +11,15 @@
     Chain.gnosis: BASE_URL + "/balancer-gnosis-chain-v2",
     # TODO: missing subgraph link in https://docs.balancer.fi/reference/subgraph/
     # optimism="",
     # avalanche="",
 }
 
 
-class BalancerSubgraph(SubgraphBaseClient):
+class BalancerSubgraph(GraphQLClient):
     def get_url(self, chain):
         return BALANCER_MAINNET_SUBGRAPH_URL_MAP[chain]
 
 
 class BalancerSubgraphQuery(GraphQLQuery):
     def get_client(self):
         return BalancerSubgraph(self.chain)
```

### Comparing `balpy_v2-0.1.1/balpy_v2/subgraphs/blocks.py` & `balpy_v2-0.1.2/balpy_v2/subgraphs/blocks.py`

 * *Files identical despite different names*

### Comparing `balpy_v2-0.1.1/balpy_v2/subgraphs/query.py` & `balpy_v2-0.1.2/balpy_v2/subgraphs/query.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
 
 from balpy_v2.lib import Chain
 from balpy_v2.subgraphs.client import GraphQLClient
 
 
 class GraphQLQuery(ABC):
-    def __init__(self, chain=Chain.mainnet, variables=dict()):
+    def __init__(self, chain=Chain.mainnet, variables=dict()) -> None:
         self.chain = chain
         self.variables = variables
 
     @abstractmethod
     def get_query(self):
         pass
```

