# Comparing `tmp/bw_graph_tools-0.1.1.tar.gz` & `tmp/bw_graph_tools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_graph_tools-0.1.1.tar", last modified: Thu Apr 27 05:18:01 2023, max compression
+gzip compressed data, was "bw_graph_tools-0.2.1.tar", last modified: Sun May  7 12:50:40 2023, max compression
```

## Comparing `bw_graph_tools-0.1.1.tar` & `bw_graph_tools-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,35 @@
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 05:18:01.713289 bw_graph_tools-0.1.1/
--rw-r--r--   0 chrismutel   (501) staff       (20)     1456 2023-04-13 06:05:08.000000 bw_graph_tools-0.1.1/LICENSE
--rw-r--r--   0 chrismutel   (501) staff       (20)       31 2023-04-13 06:05:08.000000 bw_graph_tools-0.1.1/MANIFEST.in
--rw-r--r--   0 chrismutel   (501) staff       (20)     3160 2023-04-27 05:18:01.713366 bw_graph_tools-0.1.1/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)     2192 2023-04-26 11:41:49.000000 bw_graph_tools-0.1.1/README.md
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 05:18:01.710960 bw_graph_tools-0.1.1/bw_graph_tools/
--rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-04-27 05:17:33.000000 bw_graph_tools-0.1.1/bw_graph_tools/VERSION
--rw-r--r--   0 chrismutel   (501) staff       (20)      534 2023-04-23 08:47:29.000000 bw_graph_tools-0.1.1/bw_graph_tools/__init__.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      119 2023-04-13 06:07:17.000000 bw_graph_tools-0.1.1/bw_graph_tools/errors.py
--rw-r--r--   0 chrismutel   (501) staff       (20)    25928 2023-04-23 19:13:20.000000 bw_graph_tools-0.1.1/bw_graph_tools/graph_traversal.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2092 2023-04-13 07:48:33.000000 bw_graph_tools-0.1.1/bw_graph_tools/graph_traversal_utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     7702 2023-04-26 14:27:25.000000 bw_graph_tools-0.1.1/bw_graph_tools/matrix_utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)      349 2023-04-13 07:48:33.000000 bw_graph_tools-0.1.1/bw_graph_tools/utils.py
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 05:18:01.711786 bw_graph_tools-0.1.1/bw_graph_tools.egg-info/
--rw-r--r--   0 chrismutel   (501) staff       (20)     3160 2023-04-27 05:18:01.000000 bw_graph_tools-0.1.1/bw_graph_tools.egg-info/PKG-INFO
--rw-r--r--   0 chrismutel   (501) staff       (20)      664 2023-04-27 05:18:01.000000 bw_graph_tools-0.1.1/bw_graph_tools.egg-info/SOURCES.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-27 05:18:01.000000 bw_graph_tools-0.1.1/bw_graph_tools.egg-info/dependency_links.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-13 07:24:55.000000 bw_graph_tools-0.1.1/bw_graph_tools.egg-info/not-zip-safe
--rw-r--r--   0 chrismutel   (501) staff       (20)      124 2023-04-27 05:18:01.000000 bw_graph_tools-0.1.1/bw_graph_tools.egg-info/requires.txt
--rw-r--r--   0 chrismutel   (501) staff       (20)       29 2023-04-27 05:18:01.000000 bw_graph_tools-0.1.1/bw_graph_tools.egg-info/top_level.txt
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 05:18:01.710719 bw_graph_tools-0.1.1/docs/
--rw-r--r--   0 chrismutel   (501) staff       (20)     2261 2023-04-26 11:41:49.000000 bw_graph_tools-0.1.1/docs/conf.py
--rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-04-13 06:05:08.000000 bw_graph_tools-0.1.1/pyproject.toml
--rw-r--r--   0 chrismutel   (501) staff       (20)     1607 2023-04-27 05:18:01.713747 bw_graph_tools-0.1.1/setup.cfg
-drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-04-27 05:18:01.713092 bw_graph_tools-0.1.1/tests/
--rw-r--r--   0 chrismutel   (501) staff       (20)     2494 2023-04-13 06:10:06.000000 bw_graph_tools-0.1.1/tests/test_get_path_from_matrix.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2683 2023-04-25 19:07:42.000000 bw_graph_tools-0.1.1/tests/test_matrix_utils.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     4782 2023-04-13 07:48:29.000000 bw_graph_tools-0.1.1/tests/test_second_heuristic.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     3670 2023-04-13 07:48:29.000000 bw_graph_tools-0.1.1/tests/test_third_heuristic.py
--rw-r--r--   0 chrismutel   (501) staff       (20)     2057 2023-04-25 19:08:11.000000 bw_graph_tools-0.1.1/tests/test_traversal_basic.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-07 12:50:40.624508 bw_graph_tools-0.2.1/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1456 2023-04-13 06:05:08.000000 bw_graph_tools-0.2.1/LICENSE
+-rw-r--r--   0 chrismutel   (501) staff       (20)       31 2023-04-13 06:05:08.000000 bw_graph_tools-0.2.1/MANIFEST.in
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3257 2023-05-07 12:50:40.624717 bw_graph_tools-0.2.1/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2290 2023-05-07 12:27:17.000000 bw_graph_tools-0.2.1/README.md
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-07 12:50:40.617305 bw_graph_tools-0.2.1/bw_graph_tools/
+-rw-r--r--   0 chrismutel   (501) staff       (20)        6 2023-05-07 12:43:47.000000 bw_graph_tools-0.2.1/bw_graph_tools/VERSION
+-rw-r--r--   0 chrismutel   (501) staff       (20)      652 2023-05-07 12:32:09.000000 bw_graph_tools-0.2.1/bw_graph_tools/__init__.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      123 2023-05-07 12:43:29.000000 bw_graph_tools-0.2.1/bw_graph_tools/errors.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)    25891 2023-05-07 12:32:18.000000 bw_graph_tools-0.2.1/bw_graph_tools/graph_traversal.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2074 2023-05-07 12:32:31.000000 bw_graph_tools-0.2.1/bw_graph_tools/graph_traversal_utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8742 2023-05-07 11:32:56.000000 bw_graph_tools-0.2.1/bw_graph_tools/matrix_tools.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)      349 2023-04-13 07:48:33.000000 bw_graph_tools-0.2.1/bw_graph_tools/utils.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-07 12:50:40.620126 bw_graph_tools-0.2.1/bw_graph_tools.egg-info/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3257 2023-05-07 12:50:40.000000 bw_graph_tools-0.2.1/bw_graph_tools.egg-info/PKG-INFO
+-rw-r--r--   0 chrismutel   (501) staff       (20)      860 2023-05-07 12:50:40.000000 bw_graph_tools-0.2.1/bw_graph_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-05-07 12:50:40.000000 bw_graph_tools-0.2.1/bw_graph_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)        1 2023-04-13 07:24:55.000000 bw_graph_tools-0.2.1/bw_graph_tools.egg-info/not-zip-safe
+-rw-r--r--   0 chrismutel   (501) staff       (20)      175 2023-05-07 12:50:40.000000 bw_graph_tools-0.2.1/bw_graph_tools.egg-info/requires.txt
+-rw-r--r--   0 chrismutel   (501) staff       (20)       35 2023-05-07 12:50:40.000000 bw_graph_tools-0.2.1/bw_graph_tools.egg-info/top_level.txt
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-07 12:50:40.612950 bw_graph_tools-0.2.1/docs/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2261 2023-04-26 11:41:49.000000 bw_graph_tools-0.2.1/docs/conf.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)       87 2023-04-13 06:05:08.000000 bw_graph_tools-0.2.1/pyproject.toml
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1702 2023-05-07 12:50:40.625491 bw_graph_tools-0.2.1/setup.cfg
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-07 12:50:40.623438 bw_graph_tools-0.2.1/tests/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5819 2023-05-07 12:32:46.000000 bw_graph_tools-0.2.1/tests/test_first_heuristic.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     2494 2023-04-13 06:10:06.000000 bw_graph_tools-0.2.1/tests/test_get_path_from_matrix.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     1176 2023-05-07 12:33:16.000000 bw_graph_tools-0.2.1/tests/test_matrix_utils.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     4782 2023-05-07 12:33:27.000000 bw_graph_tools-0.2.1/tests/test_second_heuristic.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     3670 2023-05-07 12:33:33.000000 bw_graph_tools-0.2.1/tests/test_third_heuristic.py
+drwxr-xr-x   0 chrismutel   (501) staff       (20)        0 2023-05-07 12:50:40.616499 bw_graph_tools-0.2.1/tests/traversal/
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8160 2023-05-07 10:49:15.000000 bw_graph_tools-0.2.1/tests/traversal/test_negative_production.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8152 2023-05-07 10:49:15.000000 bw_graph_tools-0.2.1/tests/traversal/test_nonunitary_production_with_recursion.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     5607 2023-05-07 10:49:15.000000 bw_graph_tools-0.2.1/tests/traversal/test_only_one_layer.py
+-rw-r--r--   0 chrismutel   (501) staff       (20)     8339 2023-05-07 11:35:36.000000 bw_graph_tools-0.2.1/tests/traversal/test_separate_production.py
```

### Comparing `bw_graph_tools-0.1.1/LICENSE` & `bw_graph_tools-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.1.1/PKG-INFO` & `bw_graph_tools-0.2.1/bw_graph_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bw_graph_tools
-Version: 0.1.1
+Name: bw-graph-tools
+Version: 0.2.1
 Summary: Graph traversal class and utilities
 Home-page: https://github.com/brightway-lca/bw_graph_tools
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
@@ -50,14 +50,16 @@
 
 You can install _bw_graph_tools_ via [pip] from [PyPI]:
 
 ```console
 $ pip install bw_graph_tools
 ```
 
+Packages are also on conda at the [channel cmutel](https://anaconda.org/cmutel/bw_graph_tools).
+
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

### Comparing `bw_graph_tools-0.1.1/README.md` & `bw_graph_tools-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
 You can install _bw_graph_tools_ via [pip] from [PyPI]:
 
 ```console
 $ pip install bw_graph_tools
 ```
 
+Packages are also on conda at the [channel cmutel](https://anaconda.org/cmutel/bw_graph_tools).
+
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
 
@@ -51,8 +53,8 @@
 sphinx-autobuild docs _build/html -a -j auto --open-browser
 ```
 
 <!-- github-only -->
 
 [command-line reference]: https://bw_graph_tools.readthedocs.io/en/latest/usage.html
 [license]: https://github.com/brightway-lca/bw_graph_tools/blob/main/LICENSE
-[contributor guide]: https://github.com/brightway-lca/bw_graph_tools/blob/main/CONTRIBUTING.md
+[contributor guide]: https://github.com/brightway-lca/bw_graph_tools/blob/main/CONTRIBUTING.md
```

### Comparing `bw_graph_tools-0.1.1/bw_graph_tools/__init__.py` & `bw_graph_tools-0.2.1/bw_graph_tools/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 __all__ = (
     "__version__",
     "AssumedDiagonalGraphTraversal",
     "Edge",
     "Flow",
     "get_path_from_matrix",
-    "GraphTraversal",
+    "guess_production_exchanges",
+    "NewNodeEachVisitGraphTraversal",
     "Node",
     "path_as_brightway_objects",
     "to_normalized_adjacency_matrix",
 )
 
 from .graph_traversal_utils import get_path_from_matrix, path_as_brightway_objects
-from .matrix_utils import to_normalized_adjacency_matrix
+from .matrix_tools import guess_production_exchanges, to_normalized_adjacency_matrix
 from .utils import get_version_tuple
-from .graph_traversal import GraphTraversal, Node, Edge, Flow, AssumedDiagonalGraphTraversal
-
+from .graph_traversal import (
+    AssumedDiagonalGraphTraversal,
+    Edge,
+    Flow,
+    NewNodeEachVisitGraphTraversal,
+    Node,
+)
 
 __version__ = get_version_tuple()
```

### Comparing `bw_graph_tools-0.1.1/bw_graph_tools/graph_traversal.py` & `bw_graph_tools-0.2.1/bw_graph_tools/graph_traversal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,24 @@
+import warnings
 from dataclasses import dataclass
-from heapq import heappush, heappop
+from functools import lru_cache
+from heapq import heappop, heappush
+
+from bw2calc import LCA
 from scipy.sparse import spmatrix
-import numpy as np
-import warnings
 import matrix_utils as mu
-from functools import lru_cache
+import numpy as np
 
 try:
     from bw2data import databases
 except ImportError:
     databases = {}
-try:
-    from bw2calc import LCA
-except ImportError:
 
-    class LCA:
-        pass
 
-
-from .matrix_utils import guess_production_exchanges
+from .matrix_tools import guess_production_exchanges
 
 
 class CachingSolver:
     """Class which caches expensive linear algebra solution vectors."""
 
     def __init__(self, lca: LCA):
         self.lca = lca
@@ -68,15 +64,15 @@
     reference_product_datapackage_id : int
         The id that identifies the reference product of this activity in the datapackage
     reference_product_index : int
         The technosphere matrix row index of this activity's reference product
     reference_product_production_amount : float
         The *net* production amount of this activity's reference product
     supply_amount : float
-        The amount of the *activity* needed to supply the demand from the requesting supply chain edge. *Not scaled to the reference product production amount*.
+        The amount of the *activity* (not reference product!) needed to supply the demand from the requesting supply chain edge.
     cumulative_score : float
         Total LCIA score attributed to `supply_amount` of this activity. Includes direct emissions unless explicitly removed.
     direct_emissions_score : float
         Total LCIA score attributed only to the direct characterized biosphere flows of `supply_amount` of this activity.
 
     """
 
@@ -100,30 +96,30 @@
     """
     An edge between two *activities*. The `amount` is the amount of the product demanded by the `consumer`.
 
     Parameters
     ----------
     consumer_index : int
         The matrix column index of the consuming activity
-    consumer_id : int
-        The id that identifies the consuming activity in the datapackage
+    consumer_unique_id : int
+        The traversal-specific unique id of the consuming activity
     producer_index : int
         The matrix column index of the producing activity
-    producer_id : int
-        The id that identifies the producing activity in the datapackage
+    producer_unique_id : int
+        The traversal-specific unique id of the producing activity
     product_index : int
         The matrix row index of the consumed product
     amount : float
         The amount of the product demanded by the consumer. Not scaled to producer production amount.
     """
 
     consumer_index: int
-    consumer_id: int
+    consumer_unique_id: int
     producer_index: int
-    producer_id: int
+    producer_unique_id: int
     product_index: int
     amount: float
 
 
 @dataclass
 class Flow:
     """
@@ -156,15 +152,15 @@
     score: float
 
     def __lt__(self, other):
         # Needed for sorting
         return self.score < other.score
 
 
-class GraphTraversal:
+class NewNodeEachVisitGraphTraversal:
     """
     Traverse a supply chain, following paths of greatest impact.
 
     This implementation uses a queue of datasets to assess. As the supply chain is traversed, activities are added to a list sorted by LCA score. Each activity in the sorted list is assessed, and added to the supply chain graph, as long as its impact is above a certain threshold, and the maximum number of calculations has not been exceeded.
 
     Because the next dataset assessed is chosen by its impact, not its position in the graph, this is neither a breadth-first nor a depth-first search, but rather "importance-first".
 
@@ -204,15 +200,15 @@
 
         * `technosphere_matrix`
         * `technosphere_mm`
         * `solve_linear_system()`
         * `demand`
         * `demand_array`
 
-        You can subclass `GraphTraversal` and redefine `get_characterized_biosphere` if your LCA class does not have a traditional `characterization_matrix` and `biosphere_matrix`.
+        You can subclass `NewNodeEachVisitGraphTraversal` and redefine `get_characterized_biosphere` if your LCA class does not have a traditional `characterization_matrix` and `biosphere_matrix`.
 
         The return object is a dictionary with four values. The `nodes` is a dictionary of visited **activities**; the keys in this dictionary are unique increasing integer ids (not related to any other ids or indices), and values are instances of the `Node` dataclass. Each `Node` has a `unique_id`, as every time we arrive at an activity (even if we have seen it before via another branch of the supply chain), we create a new `Node` object with a unique id. See the `Node` documentation for its other attributes.
 
         edges
 
         flows
 
@@ -281,15 +277,15 @@
                 cumulative_score=lca_object.score,
                 direct_emissions_score=0.0,
             )
         }
 
         cls.traverse_edges(
             consumer_index=functional_unit_unique_id,
-            consumer_id=functional_unit_unique_id,
+            consumer_unique_id=functional_unit_unique_id,
             product_indices=[
                 lca_object.dicts.product[key] for key in lca_object.demand
             ],
             product_amounts=lca_object.demand.values(),
             lca=lca_object,
             calculation_count=calculation_count,
             characterized_biosphere=characterized_biosphere,
@@ -412,15 +408,15 @@
                 node=node,
                 skip_coproducts=skip_coproducts,
                 matrix=technosphere_matrix,
             )
 
             cls.traverse_edges(
                 consumer_index=node.activity_index,
-                consumer_id=node.unique_id,
+                consumer_unique_id=node.unique_id,
                 product_indices=product_indices,
                 product_amounts=product_amounts,
                 lca=lca,
                 calculation_count=calculation_count,
                 characterized_biosphere=characterized_biosphere,
                 matrix=technosphere_matrix,
                 edges=edges,
@@ -435,15 +431,15 @@
                 biosphere_cutoff_score=biosphere_cutoff_score,
             )
 
     @classmethod
     def traverse_edges(
         cls,
         consumer_index: int,
-        consumer_id: int,
+        consumer_unique_id: int,
         product_indices: list[int],
         product_amounts: list[float],
         lca: LCA,
         calculation_count: Counter,
         characterized_biosphere: spmatrix,
         matrix: spmatrix,
         edges: list[Edge],
@@ -459,57 +455,54 @@
     ) -> None:
         for product_index, product_amount in zip(product_indices, product_amounts):
             producer_index = production_exchange_mapping[product_index]
 
             if producer_index in static_activity_indices:
                 return
 
-            next(calculation_count)
             supply = caching_solver(product_index, product_amount)
-            activity_supply_amount = supply[producer_index]
             cumulative_score = float((characterized_biosphere * supply).sum())
+            reference_product_net_production_amount = matrix[
+                product_index, producer_index
+            ]
+            scale = product_amount / reference_product_net_production_amount
 
             if abs(cumulative_score) < cutoff_score:
                 return
 
             producing_node = Node(
                 unique_id=next(calculation_count),
                 activity_datapackage_id=lca.dicts.activity.reversed[producer_index],
                 activity_index=producer_index,
                 reference_product_datapackage_id=lca.dicts.product.reversed[
                     product_index
                 ],
                 reference_product_index=product_index,
-                reference_product_production_amount=matrix[
-                    product_index, producer_index
-                ],
-                supply_amount=activity_supply_amount,
+                reference_product_production_amount=reference_product_net_production_amount,
+                supply_amount=scale,
                 cumulative_score=cumulative_score,
                 direct_emissions_score=(
-                    activity_supply_amount * characterized_biosphere[:, producer_index]
+                    scale * characterized_biosphere[:, producer_index]
                 ).sum(),
             )
             edges.append(
                 Edge(
                     consumer_index=consumer_index,
-                    consumer_id=consumer_id,
+                    consumer_unique_id=consumer_unique_id,
                     producer_index=producer_index,
-                    producer_id=producing_node.unique_id,
+                    producer_unique_id=producing_node.unique_id,
                     product_index=product_index,
                     amount=product_amount,
                 )
             )
 
             if separate_biosphere_flows:
                 cls.add_biosphere_flows(
                     flows=flows,
-                    matrix=(
-                        activity_supply_amount
-                        * characterized_biosphere[:, producer_index]
-                    ).tocoo(),
+                    matrix=(scale * characterized_biosphere[:, producer_index]).tocoo(),
                     lca=lca,
                     node=producing_node,
                     biosphere_cutoff_score=biosphere_cutoff_score,
                 )
 
             heappush(heap, (abs(1 / cumulative_score), producing_node))
             nodes[producing_node.unique_id] = producing_node
@@ -649,15 +642,15 @@
             elif y < 0 and skip_coproducts:
                 continue
             rows.append(x)
             vals.append(y)
         return rows, vals
 
 
-class AssumedDiagonalGraphTraversal(GraphTraversal):
+class AssumedDiagonalGraphTraversal(NewNodeEachVisitGraphTraversal):
     @classmethod
     def get_production_exchanges(
         cls, mapped_matrix: mu.MappedMatrix
     ) -> (np.ndarray, np.ndarray):
         """
         Assume production exchanges are always on the diagonal instead of
         examining matrix structure and input data.
```

### Comparing `bw_graph_tools-0.1.1/bw_graph_tools/graph_traversal_utils.py` & `bw_graph_tools-0.2.1/bw_graph_tools/graph_traversal_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import List, Optional
 
-import sknetwork as skn
+from bw2calc import LCA
 from scipy import sparse
+import sknetwork as skn
 
-from .matrix_utils import to_normalized_adjacency_matrix
+from .matrix_tools import to_normalized_adjacency_matrix
 
 try:
     import bw2data as bd
-    from bw2calc import LCA
     from bw2data import Edge, Node
 
     brightway_available = True
 except ImportError:
 
     class Dummy:
         def get_node(self):
             pass
 
-    bd, LCA, Node, Edge = Dummy(), Dummy(), Dummy(), Dummy()
+    bd, Node, Edge = Dummy(), Dummy(), Dummy()
     brightway_available = False
 
 
 def get_path_from_matrix(
     matrix: sparse.spmatrix, source: int, target: int, algorithm: str = "BF"
 ) -> List:
     """Get the path with the most mass or energetic flow from ``source`` (the function unit) to ``target`` (something deep in the supply chain). Both ``source`` and ``target`` are integer matrix indices.
```

### Comparing `bw_graph_tools-0.1.1/bw_graph_tools/matrix_utils.py` & `bw_graph_tools-0.2.1/bw_graph_tools/matrix_tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,24 +54,50 @@
     is definitely a production exchange location. We don't care if there are duplicates (e.g.
     production and some loss), we will return unique pairs.
 
     If activities have different ids than products, this won't find anything.
 
     Returns a tuple of numpy integer matrix indices, rows by columns.
     """
-    found = []
 
-    first_heuristic = np.hstack(
-        [group.row_masked[group.row_masked == group.col_masked] for group in mm.groups]
-    )
-    if first_heuristic.size:
-        found.append((first_heuristic, first_heuristic))
+    def get_used_mapped_indices_for_group(
+        group: mu.ResourceGroup,
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        indices = group.get_indices_data()
+
+        # Need to check the original input values, not after mapping when they are
+        # normalized to [0, X] range.
+        ident_mask = indices["row"] == indices["col"]
+        row_mapped = group.row_mapper.map_array(indices["row"][ident_mask])
+        col_mapped = group.col_mapper.map_array(indices["col"][ident_mask])
+
+        if (row_mapped == -1).sum() or (col_mapped == -1).sum():
+            ERROR = """
+Found unmapped values in technosphere matrix generator, but that should be impossible.
+
+{} unmapped values in the row indices: {}
+{} unmapped values in the column indices: {}
+
+Please report this as an issue, something went very wrong!
+            """
+            raise ValueError(
+                ERROR.format(
+                    (row_mapped == -1).sum(),
+                    indices["row"][row_mapped == -1],
+                    (col_mapped == -1).sum(),
+                    indices["col"][col_mapped == -1],
+                )
+            )
 
-    row_indices = np.hstack([array for array, _ in found])
-    col_indices = np.hstack([array for _, array in found])
+        return row_mapped, col_mapped
+
+    first_heuristic = [get_used_mapped_indices_for_group(group) for group in mm.groups]
+
+    row_indices = np.hstack([array for array, _ in first_heuristic])
+    col_indices = np.hstack([array for _, array in first_heuristic])
 
     return row_indices, col_indices
 
 
 def gpe_second_heuristic(
     mm: mu.MappedMatrix, row_existing: np.ndarray, col_existing: np.ndarray
 ) -> Tuple[np.ndarray, np.ndarray]:
```

### Comparing `bw_graph_tools-0.1.1/bw_graph_tools.egg-info/PKG-INFO` & `bw_graph_tools-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bw-graph-tools
-Version: 0.1.1
+Name: bw_graph_tools
+Version: 0.2.1
 Summary: Graph traversal class and utilities
 Home-page: https://github.com/brightway-lca/bw_graph_tools
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
@@ -50,14 +50,16 @@
 
 You can install _bw_graph_tools_ via [pip] from [PyPI]:
 
 ```console
 $ pip install bw_graph_tools
 ```
 
+Packages are also on conda at the [channel cmutel](https://anaconda.org/cmutel/bw_graph_tools).
+
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

### Comparing `bw_graph_tools-0.1.1/docs/conf.py` & `bw_graph_tools-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.1.1/setup.cfg` & `bw_graph_tools-0.2.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -28,28 +28,31 @@
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=.
 python_requires = >=3.8
 install_requires = 
+	bw2calc >=2.0.dev13
+	matrix_utils
+	numpy
 	scikit-network
 	scipy
-	numpy
 
 [options.packages.find]
 where = .
 exclude = 
 	tests
 
 [options.extras_require]
 testing = 
 	setuptools
 	pytest
 	pytest-cov
+	bw2data >=4.0.dev18
 dev = 
 	pre-commit
 	pylint
 docs = 
 	sphinx
 	myst_parser
 	furo
@@ -60,15 +63,17 @@
 addopts = 
 	--cov bw_graph_tools --cov-report term-missing
 	--verbose
 norecursedirs = 
 	dist
 	build
 	.tox
-testpaths = tests
+testpaths = 
+	tests/test_*.py
+	tests/traversal/test_*.py
 
 [devpi:upload]
 no_vcs = 1
 formats = bdist_wheel
 
 [flake8]
 max_line_length = 88
```

### Comparing `bw_graph_tools-0.1.1/tests/test_get_path_from_matrix.py` & `bw_graph_tools-0.2.1/tests/test_get_path_from_matrix.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.1.1/tests/test_matrix_utils.py` & `bw_graph_tools-0.2.1/tests/test_matrix_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,28 @@
 import bw_processing as bwp
 import matrix_utils as mu
 import numpy as np
 import pytest
 
 from bw_graph_tools.errors import UnclearProductionExchange
-from bw_graph_tools.matrix_utils import guess_production_exchanges
+from bw_graph_tools.matrix_tools import guess_production_exchanges
 
 
 @pytest.mark.skip(reason="MappedMatrix won't allow empty matrix construction")
 def test_gpe_empty_matrix():
     dp1 = bwp.create_datapackage()
     mm = mu.MappedMatrix(
         packages=[dp1],
         matrix="test",
     )
     with pytest.raises(ValueError):
         guess_production_exchanges(mm)
 
 
-def test_gpe_first_heuristic_single_dp():
-    dp1 = bwp.create_datapackage()
-    data = np.array([1, 2, 3, 4])
-    indices = np.array(
-        [
-            (1, 1),
-            (0, 1),
-            (0, 0),
-            (1, 0),
-        ],
-        dtype=bwp.INDICES_DTYPE,
-    )
-    dp1.add_persistent_vector(
-        matrix="test",
-        indices_array=indices,
-        name="foo",
-        data_array=data,
-    )
-    mm = mu.MappedMatrix(
-        packages=[dp1],
-        matrix="test",
-    )
-    row, col = guess_production_exchanges(mm)
-    assert np.array_equal(np.array([1, 0]), row)
-    assert np.array_equal(np.array([1, 0]), col)
-
-
-def test_gpe_multiple_datapackages():
-    pass
-
-
-def test_gpe_first_heuristic_one_dp_empty():
-    dp1 = bwp.create_datapackage()
-    data = np.array([1, 2, 3, 4])
-    indices = np.array(
-        [
-            (1, 1),
-            (0, 1),
-            (0, 0),
-            (1, 0),
-        ],
-        dtype=bwp.INDICES_DTYPE,
-    )
-    dp1.add_persistent_vector(
-        matrix="test",
-        indices_array=indices,
-        name="foo",
-        data_array=data,
-    )
-    dp2 = bwp.create_datapackage()
-    dp2.add_persistent_vector(
-        matrix="other",
-        indices_array=indices,
-        name="foo",
-        data_array=data,
-    )
-    mm = mu.MappedMatrix(
-        packages=[dp1, dp2],
-        matrix="test",
-    )
-    row, col = guess_production_exchanges(mm)
-    assert np.array_equal(np.array([1, 0]), row)
-    assert np.array_equal(np.array([1, 0]), col)
-
-
-# Don't remember the intended functionality or test case
+# Don't remember the intended functionality for test case
 @pytest.mark.skip("Don't remember the point of this test")
 def test_gpe_raise_error():
     dp1 = bwp.create_datapackage()
     data = np.array([1, 2, 4])
     indices = np.array(
         [
             (1, 1),
@@ -103,8 +38,8 @@
         data_array=data,
     )
     mm = mu.MappedMatrix(
         packages=[dp1],
         matrix="test",
     )
     with pytest.raises(UnclearProductionExchange):
-        print(guess_production_exchanges(mm))
+        guess_production_exchanges(mm)
```

### Comparing `bw_graph_tools-0.1.1/tests/test_second_heuristic.py` & `bw_graph_tools-0.2.1/tests/test_second_heuristic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import bw_processing as bwp
 import matrix_utils as mu
 import numpy as np
 
-from bw_graph_tools.matrix_utils import gpe_second_heuristic
+from bw_graph_tools.matrix_tools import gpe_second_heuristic
 
 
 def test_second_heuristic_empty_existing():
     dp1 = bwp.create_datapackage()
     data = np.array([1, 2, 3, 4])
     indices = np.array(
         [
```

### Comparing `bw_graph_tools-0.1.1/tests/test_third_heuristic.py` & `bw_graph_tools-0.2.1/tests/test_third_heuristic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import bw_processing as bwp
 import matrix_utils as mu
 import numpy as np
 
-from bw_graph_tools.matrix_utils import gpe_third_heuristic
+from bw_graph_tools.matrix_tools import gpe_third_heuristic
 
 
 def test_third_heuristic_empty_existing():
     dp1 = bwp.create_datapackage()
     data = np.array([1, -2, -3, -4])
     indices = np.array(
         [
```

