# Comparing `tmp/nographs-3.0.3.tar.gz` & `tmp/nographs-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nographs-3.0.3.tar", last modified: Thu Feb  9 20:28:33 2023, max compression
+gzip compressed data, was "nographs-3.1.0.tar", last modified: Sun May  7 17:44:16 2023, max compression
```

## Comparing `nographs-3.0.3.tar` & `nographs-3.1.0.tar`

### file list

```diff
@@ -1,26 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-02-09 20:28:33.405051 nographs-3.0.3/
--rw-rw-rw-   0        0        0     8758 2023-02-09 20:28:33.403052 nographs-3.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7447 2023-01-31 08:24:53.000000 nographs-3.0.3/README.rst
--rw-rw-rw-   0        0        0      162 2022-11-27 13:28:03.000000 nographs-3.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-09 20:28:33.405051 nographs-3.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1900 2023-02-09 20:25:02.000000 nographs-3.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-09 20:28:33.190175 nographs-3.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-02-09 20:28:33.317101 nographs-3.0.3/src/nographs/
--rw-rw-rw-   0        0        0     6492 2023-02-09 20:09:01.000000 nographs-3.0.3/src/nographs/__init__.py
--rw-rw-rw-   0        0        0     8123 2022-11-27 13:28:03.000000 nographs-3.0.3/src/nographs/edge_gadgets.py
--rw-rw-rw-   0        0        0    42018 2023-02-02 18:45:09.000000 nographs-3.0.3/src/nographs/gear_collections.py
--rw-rw-rw-   0        0        0    35182 2023-02-02 18:45:09.000000 nographs-3.0.3/src/nographs/gears.py
--rw-rw-rw-   0        0        0    13537 2023-01-22 19:07:55.000000 nographs-3.0.3/src/nographs/matrix_gadgets.py
--rw-rw-rw-   0        0        0    19400 2023-02-09 20:09:01.000000 nographs-3.0.3/src/nographs/paths.py
--rw-rw-rw-   0        0        0        0 2022-11-27 13:28:03.000000 nographs-3.0.3/src/nographs/py.typed
--rw-rw-rw-   0        0        0   155461 2023-02-09 20:09:01.000000 nographs-3.0.3/src/nographs/strategies.py
--rw-rw-rw-   0        0        0     3779 2023-02-09 20:25:02.000000 nographs-3.0.3/src/nographs/types.py
-drwxrwxrwx   0        0        0        0 2023-02-09 20:28:33.381065 nographs-3.0.3/src/nographs.egg-info/
--rw-rw-rw-   0        0        0     8758 2023-02-09 20:28:33.000000 nographs-3.0.3/src/nographs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      478 2023-02-09 20:28:33.000000 nographs-3.0.3/src/nographs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-09 20:28:33.000000 nographs-3.0.3/src/nographs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-02-09 20:28:33.000000 nographs-3.0.3/src/nographs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-09 20:28:33.397056 nographs-3.0.3/tests/
--rw-rw-rw-   0        0        0   133826 2023-02-09 20:09:01.000000 nographs-3.0.3/tests/test_code.py
--rw-rw-rw-   0        0        0     2068 2023-02-09 20:09:01.000000 nographs-3.0.3/tests/test_nographs.py
--rw-rw-rw-   0        0        0     2906 2022-11-27 13:28:03.000000 nographs-3.0.3/tests/test_unit_typed.py
+drwxrwxrwx   0        0        0        0 2023-05-07 17:44:16.787736 nographs-3.1.0/
+-rw-rw-rw-   0        0        0     9118 2023-05-07 17:44:16.786736 nographs-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7807 2023-05-07 17:05:23.000000 nographs-3.1.0/README.rst
+-rw-rw-rw-   0        0        0      162 2022-11-27 13:28:03.000000 nographs-3.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 17:44:16.787736 nographs-3.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1876 2023-05-07 17:05:23.000000 nographs-3.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 17:44:16.729657 nographs-3.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 17:44:16.759736 nographs-3.1.0/src/nographs/
+-rw-rw-rw-   0        0        0     7644 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/__init__.py
+-rw-rw-rw-   0        0        0    41849 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_bidir_search.py
+-rw-rw-rw-   0        0        0      761 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_compatibility.py
+-rw-rw-rw-   0        0        0     8188 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_edge_gadgets.py
+-rw-rw-rw-   0        0        0    42642 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_gear_collections.py
+-rw-rw-rw-   0        0        0    35184 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_gears.py
+-rw-rw-rw-   0        0        0    13918 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_matrix_gadgets.py
+-rw-rw-rw-   0        0        0     9679 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_path.py
+-rw-rw-rw-   0        0        0    19478 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_paths.py
+-rw-rw-rw-   0        0        0    13949 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_strategies.py
+-rw-rw-rw-   0        0        0   147991 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_traversals.py
+-rw-rw-rw-   0        0        0     3232 2023-05-07 17:05:23.000000 nographs-3.1.0/src/nographs/_types.py
+-rw-rw-rw-   0        0        0        0 2022-11-27 13:28:03.000000 nographs-3.1.0/src/nographs/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-07 17:44:16.765735 nographs-3.1.0/src/nographs.egg-info/
+-rw-rw-rw-   0        0        0     9118 2023-05-07 17:44:16.000000 nographs-3.1.0/src/nographs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      834 2023-05-07 17:44:16.000000 nographs-3.1.0/src/nographs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 17:44:16.000000 nographs-3.1.0/src/nographs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-07 17:44:16.000000 nographs-3.1.0/src/nographs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 17:44:16.784735 nographs-3.1.0/tests/
+-rw-rw-rw-   0        0        0     5033 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_docs_examples.py
+-rw-rw-rw-   0        0        0     5963 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_edge_gadgets.py
+-rw-rw-rw-   0        0        0    11625 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_gear_collections.py
+-rw-rw-rw-   0        0        0     2065 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_gears.py
+-rw-rw-rw-   0        0        0     1923 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_matrix_gadgets.py
+-rw-rw-rw-   0        0        0     2138 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_nographs.py
+-rw-rw-rw-   0        0        0      510 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_path.py
+-rw-rw-rw-   0        0        0     5828 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_paths.py
+-rw-rw-rw-   0        0        0     2783 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_strategies.py
+-rw-rw-rw-   0        0        0   155814 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_traversals_and_searches.py
+-rw-rw-rw-   0        0        0     1419 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_types.py
+-rw-rw-rw-   0        0        0     3389 2023-05-07 17:05:23.000000 nographs-3.1.0/tests/test_unit_typed.py
```

### Comparing `nographs-3.0.3/PKG-INFO` & `nographs-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nographs
-Version: 3.0.3
+Version: 3.1.0
 Summary: Graph analysis – the lazy (evaluation) way: Analysis on the fly, for graphs, that are computed and/or adapted on the fly.
 Home-page: https://github.com/HeWeMel/nographs
 Author: Dr. Helmut Melcher
 Author-email: HeWeMel@web.de
 Project-URL: Documentation, https://nographs.readthedocs.io/
 Project-URL: Source, https://github.com/hewemel/nographs/
 Project-URL: Bug Reports, https://github.com/hewemel/nographs/issues
@@ -71,45 +71,57 @@
 **the analysis and the reporting of results by the library happen on the fly**
 (when, and as far as, results can already be derived).
 
 Think of it as *graph analysis - the lazy (evaluation) way*.
 
 **Feature overview**
 
-- Algorithms: DFS, BFS, topological search,
+- Unidirectional traversal algorithms: DFS, BFS, topological search,
   Dijkstra, A\* and MST.
-- Flexible graph notion: Infinite directed multigraphs with loops and
-  attributes (this includes
-  multiple adjacency, cycles, self-loops,
-  directed edges,
-  weighted edges and edges with application specific attributes).
-  Your vertices can be nearly anything.
-  Wide range of data types for edge weights and path length
-  supported (float, int, Decimal, mpmath.mpf and others), e.g.,
-  for high precision computations.
-  Infinite graphs are supported, but need to be
-  locally finite (i.e., a vertex has only finitely many outgoing edges).
+- Bidirectional search algorithms: BFS and Dijkstra.
+- Flexible graph notion:
+
+  - Infinite directed multigraphs with loops and
+    attributes (this includes
+    multiple adjacency, cycles, self-loops,
+    directed edges,
+    weighted edges and edges with application specific attributes).
+  - Infinite graphs are supported, but need to be
+    locally finite (i.e., a vertex has only finitely many outgoing edges).
+
+- Generic API. The application can define the following:
+
+  - Vertices: Can be anything except for None. Hashable vertices can be
+    used directly, unhashable vertices can be used together with
+    hashable identifiers.
+  - Edge weights and distances: Wide range of data types
+    supported (float, int, Decimal, mpmath.mpf and others), e.g.,
+    for high precision computations.
+  - Edge attributes: Any object, e.g, a container
+    with further data.
+  - Identity and equivalence of vertices.
+  - Bookkeeping: Several sets of bookkeeping data structures
+    are predefined, optimized for different situations (data types used by the
+    application, hashing vs. indexing, collections for *Python* objects or *C* native
+    data types,...); Adaptable and extendable, e.g., specialized
+    collections of 3rd party libraries can be integrated easily and runtime
+    efficiently
+
 - Results: Reachability, depth, distance, paths and trees.
   Paths can be
   calculated with vertices or edges or attributed edges
   and can be iterated in both directions.
 - Flexible API: The concept of implicit graphs that NoGraphs is based on
-  allows for an API that eases operations like
-  graph pruning, graph product and graph abstraction ike
+  allows for an API that eases
+  operations like
   graph pruning, graph abstraction, the typical binary
   graph operations (union, intersection, several types of products), the
   computation of search-aware graphs, and
   traversals of vertex equivalence classes on the fly.
-- Flexible bookkeeping:
-  Several sets of bookkeeping data structures,
-  optimized for different situations (data types used by the application,
-  hashing vs. indexing, collections for Python objects or *C* native data types,
-  ...); Adaptable and extendable, e.g., specialized collections of
-  3rd party libraries can be integrated easily and runtime efficiently. Internal
-  bookkeeping data can be
+  Bookkeeping data can be
   pre-initialized and accessed during computations.
 - Typing: The API can be used fully typed (optionally).
 - Implementation: Pure Python (>=3.9). It introduces no further dependencies.
 - Runtime and memory performance: Have been goals. In its domain, it
   often even outperforms Rust- and C-based libraries.
 
 **Documentation**
```

### Comparing `nographs-3.0.3/README.rst` & `nographs-3.1.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -44,45 +44,57 @@
 **the analysis and the reporting of results by the library happen on the fly**
 (when, and as far as, results can already be derived).
 
 Think of it as *graph analysis - the lazy (evaluation) way*.
 
 **Feature overview**
 
-- Algorithms: DFS, BFS, topological search,
+- Unidirectional traversal algorithms: DFS, BFS, topological search,
   Dijkstra, A\* and MST.
-- Flexible graph notion: Infinite directed multigraphs with loops and
-  attributes (this includes
-  multiple adjacency, cycles, self-loops,
-  directed edges,
-  weighted edges and edges with application specific attributes).
-  Your vertices can be nearly anything.
-  Wide range of data types for edge weights and path length
-  supported (float, int, Decimal, mpmath.mpf and others), e.g.,
-  for high precision computations.
-  Infinite graphs are supported, but need to be
-  locally finite (i.e., a vertex has only finitely many outgoing edges).
+- Bidirectional search algorithms: BFS and Dijkstra.
+- Flexible graph notion:
+
+  - Infinite directed multigraphs with loops and
+    attributes (this includes
+    multiple adjacency, cycles, self-loops,
+    directed edges,
+    weighted edges and edges with application specific attributes).
+  - Infinite graphs are supported, but need to be
+    locally finite (i.e., a vertex has only finitely many outgoing edges).
+
+- Generic API. The application can define the following:
+
+  - Vertices: Can be anything except for None. Hashable vertices can be
+    used directly, unhashable vertices can be used together with
+    hashable identifiers.
+  - Edge weights and distances: Wide range of data types
+    supported (float, int, Decimal, mpmath.mpf and others), e.g.,
+    for high precision computations.
+  - Edge attributes: Any object, e.g, a container
+    with further data.
+  - Identity and equivalence of vertices.
+  - Bookkeeping: Several sets of bookkeeping data structures
+    are predefined, optimized for different situations (data types used by the
+    application, hashing vs. indexing, collections for *Python* objects or *C* native
+    data types,...); Adaptable and extendable, e.g., specialized
+    collections of 3rd party libraries can be integrated easily and runtime
+    efficiently
+
 - Results: Reachability, depth, distance, paths and trees.
   Paths can be
   calculated with vertices or edges or attributed edges
   and can be iterated in both directions.
 - Flexible API: The concept of implicit graphs that NoGraphs is based on
-  allows for an API that eases operations like
-  graph pruning, graph product and graph abstraction ike
+  allows for an API that eases
+  operations like
   graph pruning, graph abstraction, the typical binary
   graph operations (union, intersection, several types of products), the
   computation of search-aware graphs, and
   traversals of vertex equivalence classes on the fly.
-- Flexible bookkeeping:
-  Several sets of bookkeeping data structures,
-  optimized for different situations (data types used by the application,
-  hashing vs. indexing, collections for Python objects or *C* native data types,
-  ...); Adaptable and extendable, e.g., specialized collections of
-  3rd party libraries can be integrated easily and runtime efficiently. Internal
-  bookkeeping data can be
+  Bookkeeping data can be
   pre-initialized and accessed during computations.
 - Typing: The API can be used fully typed (optionally).
 - Implementation: Pure Python (>=3.9). It introduces no further dependencies.
 - Runtime and memory performance: Have been goals. In its domain, it
   often even outperforms Rust- and C-based libraries.
 
 **Documentation**
```

### Comparing `nographs-3.0.3/setup.py` & `nographs-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.rst').read_text(encoding='utf-8')
 
 setup(
     name="nographs",
-    version="3.0.3",  # prev dev: 3.0.0.dev2
+    version="3.1.0",
     description=("Graph analysis – the lazy (evaluation) way: Analysis on the fly, "
                  + "for graphs, that are computed and/or adapted on the fly."),
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/HeWeMel/nographs",
     author="Dr. Helmut Melcher",
     author_email='HeWeMel@web.de',
```

### Comparing `nographs-3.0.3/src/nographs/edge_gadgets.py` & `nographs-3.1.0/src/nographs/_edge_gadgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
 import collections
 import itertools
 from collections.abc import Sequence, Mapping, Callable, Iterable
 from typing import Union, Any, Literal, overload
-from nographs import (  # types
+
+from ._types import (
     T_vertex,
     T_weight,
     T_labels,
     OutEdge,
     WeightedOrLabeledFullEdge,
+    AnyFullEdge,
 )
 
 
 # ---------- functions for handling test data given as some kind of edges -------------
 
 
 @overload
@@ -132,28 +134,28 @@
                         for e_to in edges_to
                     ),
                     add_inverted=add_inverted,
                     attributes=False,
                 )
         raise ValueError("graph must be Mapping or Sequence")
 
-    def get(vertex, _):
+    def get(vertex: Any, _: Any) -> Union[Any, Sequence[Any]]:
         try:
             return index[vertex]
         except KeyError:
             return ()
         except IndexError:
             return ()
 
     return get
 
 
 @overload
 def adapt_edge_iterable(
-    edges: Iterable[tuple[T_vertex, T_vertex]],
+    edges: Iterable[AnyFullEdge[T_vertex, T_weight, T_labels]],
     *,
     add_inverted: bool,
     attributes: Literal[False],
 ) -> Callable[[T_vertex, Any], Iterable[T_vertex]]:
     ...
```

### Comparing `nographs-3.0.3/src/nographs/gear_collections.py` & `nographs-3.1.0/src/nographs/_gear_collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,18 +310,18 @@
     and statements *assert not None* in a cases where the type
     checker cannot fully correctly track all execution paths. The AssertionError,
     that were being raised by the assert statements in case of implementation
     errors are now raised when a method of _GettableSettableForGearAssertNoCall
     is really called by mistake.
     """
 
-    def __getitem__(self, item):
+    def __getitem__(self, item: T_hashable_key_contra) -> T_value_co:
         raise AssertionError(called_by_mistake)
 
-    def __setitem__(self, item, value):
+    def __setitem__(self, item: T_hashable_key_contra, value: T_value_contra) -> None:
         raise AssertionError(called_by_mistake)
 
 
 class _VertexSequenceWrapperAssertNoCall(
     VertexSequenceWrapperForSetProto[T_hashable_key, T_value_contra, T_value_co],
     VertexSequenceWrapperForMappingProto[T_hashable_key, T_value_contra, T_value_co],
 ):
@@ -332,43 +332,53 @@
     together with statements *assert not None* in a cases where the type
     checker cannot fully correctly track all execution paths. The AssertionError,
     that were being raised by the assert statements in case of implementation
     errors are now raised when a method of _VertexSequenceWrapperAssertNoCall
     is really called by mistake.
     """
 
-    def sequence(self):
+    def sequence(
+        self,
+    ) -> GettableSettableForGearProto[T_hashable_key, T_value_contra, T_value_co]:
         raise AssertionError(called_by_mistake)
 
-    def default(self):
+    def default(self) -> T_value_co:
         raise AssertionError(called_by_mistake)
 
-    def extend_and_set(self, key, value):
+    def extend_and_set(self, key: T_hashable_key_contra, value: T_value_contra) -> None:
         raise AssertionError(called_by_mistake)
 
-    def update_from_keys(self, elements):
+    def update_from_keys(self, elements: Iterable[T_hashable_key]) -> None:
         raise AssertionError(called_by_mistake)
 
-    def index_and_bit_method(self):
+    def index_and_bit_method(
+        self,
+    ) -> Optional[Callable[[T_hashable_key, int], tuple[T_hashable_key, int]]]:
         raise AssertionError(called_by_mistake)
 
-    def update_from_keys_values(self, elements):
+    def update_from_keys_values(
+        self, elements: Iterable[tuple[T_hashable_key_contra, T_value_contra]]
+    ) -> None:
         raise AssertionError(called_by_mistake)
 
-    def update_default(self, elements):
+    def update_default(
+        self, elements: Iterable[tuple[T_hashable_key_contra, T_value_contra]]
+    ) -> None:
         raise AssertionError(called_by_mistake)
 
-    def _from_iterable(self, elements):
+    def _from_iterable(
+        self, elements: Iterable[T_hashable_key]
+    ) -> "_VertexSequenceWrapperAssertNoCall":
         raise AssertionError(called_by_mistake)
 
 
 # - Set
 
 
-class VertexSetByWrapper(
+class _VertexSetByWrapper(
     VertexSequenceWrapperForSetProto[T_hashable_key, int, int],
     VertexSet[T_hashable_key],
     ABC,
 ):
     """
     A VertexSet that is implemented based on a sequence-like internal container
     needs to subclass this class in order to allow NoGraphs' traversal algorithms to
@@ -378,22 +388,22 @@
 
     pass
 
 
 def get_wrapper_from_vertex_set(
     vertex_set: VertexSet[T_hashable_key],
 ) -> Optional[VertexSequenceWrapperForSetProto[T_hashable_key, int, int]]:
-    """If *vertex_set* is implemented by a VertexSetByWrapper,
+    """If *vertex_set* is implemented by a _VertexSetByWrapper,
     return its wrapper, otherwise return None. The class encapsulates the
     down cast and the argumentation for its correctness.
     """
-    if isinstance(vertex_set, VertexSetByWrapper):
+    if isinstance(vertex_set, _VertexSetByWrapper):
         # VertexSet is invariant in T_hashable_key. So,
         # having a VertexSet[T_hashable_key] also means having a
-        # VertexSetByWrapper[T_hashable_key], and thus a
+        # _VertexSetByWrapper[T_hashable_key], and thus a
         # VertexSequenceWrapperForSetProto[T_hashable_key, int, int].
         return cast(
             VertexSequenceWrapperForSetProto[T_hashable_key, int, int], vertex_set
         )
     return None
 
 
@@ -403,15 +413,15 @@
     bool,
     GettableSettableForGearProto[T_hashable_key, int, int],
     VertexSequenceWrapperForSetProto[T_hashable_key, int, int],
     bool,
     Callable[[T_hashable_key, int], tuple[T_hashable_key, int]],
 ]:
     """
-    If *vertex_set* is implemented by a VertexSetByWrapper,
+    If *vertex_set* is implemented by a _VertexSetByWrapper,
     return True, the wrapper, the wrapped sequence,
     and either True and the index_and_bit_method of the wrapper, if available,
     or False and a dummy function. It the returned sequence raises an IndexError
     on access, the wrapper can be used to extend the sequence in order to solve
     the problem.
 
     Otherwise, return False ("no wrapper, no underlying sequence") and dummy
@@ -440,15 +450,15 @@
         else:
             return (True, wrapper.sequence(), wrapper, True, index_and_bit_method)
 
 
 # - Mapping (without None)
 
 
-class VertexMappingByWrapper(
+class _VertexMappingByWrapper(
     VertexSequenceWrapperForMappingProto[T_hashable_key, T_value, T_value],
     VertexMapping[T_hashable_key, T_value],
     ABC,
 ):
     """
     A VertexMapping that is implemented based on a sequence-like internal container
     needs to subclass this class in order to allow NoGraphs' traversal algorithms to
@@ -458,22 +468,22 @@
 
     pass
 
 
 def get_wrapper_from_vertex_mapping(
     vertex_mapping: VertexMapping[T_hashable_key, T_value]
 ) -> Optional[VertexSequenceWrapperForMappingProto[T_hashable_key, T_value, T_value]]:
-    """If *vertex_mapping* is implemented by a VertexMappingByWrapper,
+    """If *vertex_mapping* is implemented by a _VertexMappingByWrapper,
     return its wrapper, otherwise return None. The class encapsulates the
     down cast and the argumentation for its correctness.
     """
-    if isinstance(vertex_mapping, VertexMappingByWrapper):
+    if isinstance(vertex_mapping, _VertexMappingByWrapper):
         # VertexMapping is invariant in T_hashable_key and T_value. So,
         # having a VertexMapping[T_hashable_key, T_value] also means having a
-        # VertexMappingByWrapper[T_hashable_key, T_value, T_value] , and thus a
+        # _VertexMappingByWrapper[T_hashable_key, T_value, T_value] , and thus a
         # VertexSequenceWrapperForMappingProto[T_hashable_key, T_value, T_value].
         return cast(
             VertexSequenceWrapperForMappingProto[T_hashable_key, T_value, T_value],
             vertex_mapping,
         )
     return None
 
@@ -482,15 +492,15 @@
     vertex_mapping: VertexMapping[T_hashable_key, T_value]
 ) -> tuple[
     bool,
     GettableSettableForGearProto[T_hashable_key, T_value, T_value],
     VertexSequenceWrapperForMappingProto[T_hashable_key, T_value, T_value],
 ]:
     """
-    If *vertex_mapping* is implemented by a VertexMappingByWrapper,
+    If *vertex_mapping* is implemented by a _VertexMappingByWrapper,
     return True, the wrapped sequence for direct access,
     and the wrapper to extend to sequence if necessary.
     Otherwise, return False, the vertex_mapping itself, and a
     dummy implementation or a wrapper.
 
     Note: If the returned GettableSettableForGearProto raises an IndexError
     on access, it is guaranteed that the third returned value had been a
@@ -498,15 +508,15 @@
     sequence in order solve the problem.
     """
 
     wrapper = get_wrapper_from_vertex_mapping(vertex_mapping)
     if wrapper is None:
         # The vertex_mapping returned here never raises an IndexError,
         # because it is a VertexMapping (see there) but is no
-        # VertexMappingByWrapper.
+        # _VertexMappingByWrapper.
         return (
             False,
             vertex_mapping,
             _VertexSequenceWrapperAssertNoCall[T_hashable_key, T_value, T_value](),
         )
 
     # The sequence returned here may raise an IndexError, but then a wrapper
@@ -517,15 +527,15 @@
         wrapper,
     )
 
 
 # - Mapping with None
 
 
-class VertexMappingByWrapperWithNone(
+class _VertexMappingByWrapperWithNone(
     VertexSequenceWrapperForMappingProto[T_hashable_key, T_value, Optional[T_value]],
     VertexMapping[T_hashable_key, T_value],
     ABC,
 ):
     """
     A VertexMapping that is implemented based on a sequence-like internal container
     needs to subclass this class in order to allow NoGraphs' traversal algorithms to
@@ -537,22 +547,22 @@
 
 
 def get_wrapper_from_vertex_mapping_with_none(
     vertex_mapping: VertexMapping[T_hashable_key, T_value]
 ) -> Optional[
     VertexSequenceWrapperForMappingProto[T_hashable_key, T_value, Optional[T_value]]
 ]:
-    """If *vertex_mapping* is implemented by a VertexMappingByWrapper,
+    """If *vertex_mapping* is implemented by a _VertexMappingByWrapper,
     return its wrapper, otherwise return None. The class encapsulates the
     down cast and the argumentation for its correctness.
     """
-    if isinstance(vertex_mapping, VertexMappingByWrapperWithNone):
+    if isinstance(vertex_mapping, _VertexMappingByWrapperWithNone):
         # VertexMapping is invariant in T_hashable_key and T_value. So,
         # having a VertexMapping[T_hashable_key, T_value] also means having a
-        # VertexMappingByWrapperWithNone[T_hashable_key, T_value], and thus a
+        # _VertexMappingByWrapperWithNone[T_hashable_key, T_value], and thus a
         # VertexSequenceWrapperForMappingProto[T_hashable_key, T_value, T_value].
         return cast(
             VertexSequenceWrapperForMappingProto[
                 T_hashable_key, T_value, Optional[T_value]
             ],
             vertex_mapping,
         )
@@ -563,16 +573,16 @@
     vertex_mapping: VertexMapping[T_hashable_key, T_value]
 ) -> tuple[
     bool,
     GettableSettableForGearProto[T_hashable_key, T_value, Optional[T_value]],
     VertexSequenceWrapperForMappingProto[T_hashable_key, T_value, Optional[T_value]],
 ]:
     """
-    If *vertex_mapping* is implemented by a VertexMappingByWrapper or a
-    VertexMappingByWrapperWithNone,
+    If *vertex_mapping* is implemented by a _VertexMappingByWrapper or a
+    _VertexMappingByWrapperWithNone,
     return True, the wrapped sequence for direct access, and the wrapper to
     extend to sequence if necessary.
     Otherwise, return False, the vertex_mapping itself, and a
     dummy implementation or a wrapper.
 
     If the returned container ever raises an IndexError on access, it
     is guaranteed that the second returned value had been a
@@ -699,15 +709,15 @@
 # --- VertexMapping (...ByWrapperWithNone or ...ByWrapperWithoutNone)
 # --- based on a VertexSequenceWrapper
 
 # --  VertexSet
 
 
 class VertexSetWrappingSequence(
-    VertexSequenceWrapper[int, int], VertexSetByWrapper[NonNegativeDenseInt], ABC
+    VertexSequenceWrapper[int, int], _VertexSetByWrapper[NonNegativeDenseInt], ABC
 ):
     """A VertexSequenceWrapper that emulates a VertexSet for
     non-negative dense integer keys based on an underlying SequenceForGearProto.
 
     It must be initialized with a factory function for the SequenceForGearProto
     to be wrapped, the number of elements the sequence should be extended when
     more space is needed, and an iterable of keys with initial content.
@@ -1028,21 +1038,21 @@
             except IndexError:
                 # Key outside length of collection -> no value stored so far -> store
                 self.extend_and_set(key, value)
 
 
 class VertexMappingWrappingSequenceWithNone(
     VertexMappingWrappingSequence[T_value, None],
-    VertexMappingByWrapperWithNone[NonNegativeDenseInt, T_value],
+    _VertexMappingByWrapperWithNone[NonNegativeDenseInt, T_value],
 ):
     """Special case: sequence can/will store None as values"""
 
     pass
 
 
 class VertexMappingWrappingSequenceWithoutNone(
     VertexMappingWrappingSequence[T_value, T_value],
-    VertexMappingByWrapper[NonNegativeDenseInt, T_value],
+    _VertexMappingByWrapper[NonNegativeDenseInt, T_value],
 ):
     """Special case: sequence can/will not store None as values"""
 
     pass
```

### Comparing `nographs-3.0.3/src/nographs/gears.py` & `nographs-3.1.0/src/nographs/_gears.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,21 @@
     Tuple,
 )
 from abc import abstractmethod
 from array import array
 from itertools import repeat
 from decimal import Decimal
 
-from nographs import (
-    # from types
+from ._types import (
     T_vertex,
     T_vertex_id,
     T_weight,
     T_labels,
 )
-from nographs import (
-    # from gear_collections
+from ._gear_collections import (
     SequenceForGearProto,
     VertexSet,
     VertexMapping,
     VertexSetWrappingSequenceNoBitPacking,
     VertexSetWrappingSequenceBitPacking,
     VertexMappingWrappingSequenceWithoutNone,
     VertexMappingWrappingSequenceWithNone,
@@ -52,20 +50,20 @@
 # In the API documentation, they are replaced by their respective definition.
 
 """
 ABC for a collection that is intended to be used by NoGraphs for storing sets
 of vertices represented by your chosen type of hashable vertex ids.
 
 If a VertexIdSet is implemented by a
-VertexSetByWrapper
+_VertexSetByWrapper
 class based on a wrapped sequence, NoGraphs directly accesses the sequence for
 better performance.
-If method index_and_bit_method of the VertexSetByWrapper returns a function
+If method index_and_bit_method of the _VertexSetByWrapper returns a function
 (not None), the set elements will be stored as bits in the sequence, see
-VertexSetByWrapper.
+_VertexSetByWrapper.
 """
 VertexIdSet = VertexSet[T_vertex_id]
 
 """
 ABC for a collection that is intended to be used by NoGraphs for
 storing mappings from your chosen type of hashable vertex ids to vertices
 of your chosen data type.
@@ -184,16 +182,16 @@
     vertex_ids, and edge data (like a GearWithoutDistances), and additionally,
     edge weights / distances. It also provides suitable distance values for
     zero and positive infinity.
 
     In case you use a gear that allows for manually choosing a zero and/or infinity
     value, or when you define your own gear, please note:
 
-    The zero value must be a neutral element of the addition in T_weight, i.e., for
-    any value v in T_weight, v + zero == v needs to hold.
+    The zero value must be a neutral element of addition and subtraction in T_weight,
+    i.e., for any value v in T_weight, v + zero == v and v - zero == v need to hold.
 
     The infinity value must be larger (w.r.t. to the comparison operators of weights)
     than all T_weight values that can occur as edge weight or as distance of
     vertices (sum of a set of edge weights) in the use cases of the gear.
 
     Note: The infinity value does not need to be a special, build-in infinity value
     of the type used for weights and distances, with the usual guarantees made for
@@ -232,15 +230,15 @@
         If the returned mapping does not contain a value for some key,
         its method __getitem__ needs to return the positive infinity value.
 
         :param initial_content: The collection is created with this initial content.
         """
         raise NotImplementedError
 
-    def raise_distance_infinity_overflow_error(self, value: T_weight):
+    def raise_distance_infinity_overflow_error(self, value: T_weight) -> None:
         """Report that the computed value is equal or larger than the chosen
         infinity value of the gear and cannot be further handled.
 
         The method is intended to be only called by NoGraphs itself.
         """
         raise OverflowError(
             f"Distance {value} is equal or larger than the "
```

### Comparing `nographs-3.0.3/src/nographs/matrix_gadgets.py` & `nographs-3.1.0/src/nographs/_matrix_gadgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 
 import itertools
 import operator
 from collections.abc import (
     Container,
     Sequence,
+    MutableSequence,
     Mapping,
     Callable,
     Iterable,
     Iterator,
     Hashable,
 )
-from numbers import Real
-from typing import Optional, Any, SupportsIndex
+from typing import Optional, Any, SupportsIndex, cast
+
+from ._types import T_weight
 
 
 Vector = Sequence[int]  # api.rst: documented manually
 Vectors = Sequence[Vector]
 Limits = Sequence[tuple[int, int]]  # api.rst: documented manually
 
 
@@ -148,15 +150,15 @@
                 yield neighbor_position.wrap_to_cuboid(limits)
             else:
                 if neighbor_position.is_in_cuboid(limits):
                     yield neighbor_position
 
 
 class Array:
-    def __init__(self, nested_sequences, dimensions: int = 2):
+    def __init__(self, nested_sequences: Sequence, dimensions: int = 2) -> None:
         """An n-dimensional array.
 
         Based on *nested sequences* that, up to a given number of
         *dimensions*, define its content. Data in nestings deeper than
         that is interpreted as part of the content of an array cell.
 
         Coordinates of a position in the array are meant in the order from "outer"
@@ -186,59 +188,61 @@
         *from* is always zero and *to* equals the size of the array
         in this dimension."""
         return [(0, upper) for upper in self.size()]
 
     def mutable_copy(self) -> Array:
         """Create a mutable copy of the array."""
 
-        def _writable(area, dimensions):
+        def _writable(area: Sequence, dimensions: int) -> list:
             if dimensions > 1:
                 return [_writable(sub_area, dimensions - 1) for sub_area in area]
             else:
                 return list(area)
 
         return Array(_writable(self.content, self.dimensions), self.dimensions)
 
-    def __getitem__(self, position: Vector):
+    def __getitem__(self, position: Vector) -> Any:
         """Get the content at the given position. This allows for using
         the expression syntax *array[...]*.
 
         :param position: The content at this position `Vector` is returned.
         """
         i = self.content
         for coordinate in position:
             i = i[coordinate]
         return i
 
-    def __setitem__(self, position: Vector, content: Any):
+    def __setitem__(self, position: Vector, content: Any) -> None:
         # noinspection PyShadowingNames
         """Set the content at the given position. Assumption: The nested
         sequence the array is build upon is mutable in its last dimension
         (i.e., a list). Allows for using the assignment syntax
         *array[...] = ...* .
 
         :param position: The content at this position `Vector` is replaced.
         :param content: This content is stored at the position.
         """
         # inspection PyShadowingNames
         field = self.content
         for coordinate in position[:-1]:
             field = field[coordinate]
-        field[position[-1]] = content
+        cast(MutableSequence, field)[position[-1]] = content
 
     def items(self) -> Iterator[tuple[Position, Any]]:
         """Iterate positions and content.
 
         :rtype: Iterator[tuple[Position, Any]]
         """
         # Above, the rtype is documented manually because Sphinx autodocs with
         # option autodoc_typehints = 'description' cannot correctly
         # evaluate the type parameters of tuple (whilst typing.Tuple works).
 
-        def _items_in_dimension(area, dimensions):
+        def _items_in_dimension(
+            area: Sequence, dimensions: int
+        ) -> Iterator[tuple[tuple[int, ...], Any]]:
             if dimensions == 1:
                 for coordinate, sub_area in enumerate(area):
                     yield (coordinate,), sub_area
             else:
                 for coordinate, sub_area in enumerate(area):
                     for sub_vector, content in _items_in_dimension(
                         sub_area, dimensions - 1
@@ -258,15 +262,17 @@
         :param content: Content to be searched.
         :rtype: tuple[Position, ...]
         """
         # For reason for manually documented rtype see method items above.
 
         content_set = set(content)
 
-        def find_in_dimension(p_matrix, p_dimensions) -> Iterator[tuple[int, ...]]:
+        def find_in_dimension(
+            p_matrix: Sequence, p_dimensions: int
+        ) -> Iterator[tuple[int, ...]]:
             if p_dimensions == 1:
                 for coordinate, cell_content in enumerate(p_matrix):
                     if cell_content in content_set:
                         yield (coordinate,)
             else:
                 for coordinate, sub_area in enumerate(p_matrix):
                     for found in find_in_dimension(sub_area, p_dimensions - 1):
@@ -294,27 +300,27 @@
         :param diagonals: Diagonal moves are allowed.
         """
         # inspection PyShadowingNames
         forbidden_content = set(forbidden)
         limits = self.limits()
         moves = Position.moves(dimensions=self.dimensions, diagonals=diagonals)
 
-        def next_vertices(position, _):
+        def next_vertices(position: Position, _: Any) -> Iterator[Position]:
             for neighbor in position.neighbors(moves=moves, limits=limits, wrap=wrap):
                 if self[neighbor] not in forbidden_content:
                     yield neighbor
 
         return next_vertices
 
     def next_edges_from_cell_weights(
         self,
-        content_to_weight: Mapping[Any, Real],
+        content_to_weight: Mapping[Any, T_weight],
         wrap: bool = False,
         diagonals: bool = False,
-    ) -> Callable:
+    ) -> Callable[[Position, Any], Iterable[tuple[Position, T_weight]]]:
         # noinspection PyShadowingNames
         """Return a `NextEdges` function for traversal strategies, based on
         given choice of when positions qualify as neighbors (goals of a
         move) of a given position (options *wrap* and *diagonals*) and what
         weight such a move has w.r.t. the content of the matrix at this
         position (parameter *content_to_weight*, and no assigned weight means
         the move is impossible).
@@ -323,14 +329,14 @@
         :param wrap: Positions are wrapped at the array limits.
         :param diagonals: Diagonal moves are allowed.
         """
         # inspection PyShadowingNames
         limits = self.limits()
         moves = Position.moves(dimensions=self.dimensions, diagonals=diagonals)
 
-        def next_edges(vector, _):
+        def next_edges(vector: Position, _: Any) -> Iterator[tuple[Position, T_weight]]:
             for neighbor in vector.neighbors(moves=moves, limits=limits, wrap=wrap):
                 weight = content_to_weight.get(self[neighbor], None)
                 if weight is not None:
                     yield neighbor, weight
 
         return next_edges
```

### Comparing `nographs-3.0.3/src/nographs/paths.py` & `nographs-3.1.0/src/nographs/_paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from __future__ import annotations
 
 from collections.abc import Sequence, Iterator, MutableMapping
 from typing import Optional, Any, Generic, cast, Union
 from abc import ABC, abstractmethod
 
-import nographs
-from nographs import (
+from ._types import (
+    T,
     T_vertex,
     T_vertex_id,
     T_labels,
     VertexToID,
     vertex_as_id,
     LabeledOutEdge,
     UnweightedUnlabeledFullEdge,
     UnweightedLabeledFullEdge,
-    VertexIdToVertexMapping,
-    VertexIdToPathEdgeDataMapping,
+)
+from ._gear_collections import (
     GettableSettableForGearProto,
     VertexSequenceWrapperForMappingProto,
     access_to_vertex_mapping_expect_none,
 )
+from ._gears import (
+    VertexIdToVertexMapping,
+    VertexIdToPathEdgeDataMapping,
+)
 
 
 class Paths(ABC, Generic[T_vertex, T_vertex_id, T_labels]):
     """
     Bases: ABC, Generic[`T_vertex`, `T_vertex_id`, `T_labels`]
 
     A Paths object is a container that stores the paths ("ways" through a graph)
@@ -225,16 +229,15 @@
     ]:
         """Return the path that ends at *vertex* as a sequence. The orientation
         of the path is from first to last vertex / edge. In case of a labeled
         path, the edges are returned, for an unlabeled path the vertices.
 
         The method allows for expressions like *paths[vertex]*.
 
-        In fully typed code, you can use an equivalent and fully typed alternative
-        for paths without resp. with labels:
+        In fully typed code, you can use the following alternative:
 
         .. code-block:: python
 
            # If the paths are not labeled, the following is equivalent to paths[vertex]:
            tuple(paths.iter_vertices_from_start(vertex))
 
            # If the paths are labeled, the following is equivalent to paths[vertex]:
@@ -243,42 +246,46 @@
         Internally, the path from the given vertex back to the first vertex
         in the path is computed, and then reversed and stored as sequence.
 
         :param vertex: The path ending at this vertex will be returned.
         """
 
 
-class _PathsDummy(Paths[T_vertex, T_vertex_id, Any]):
-    """Empty and non-functional default Paths container. Raises RuntimeError
-    for all methods returning or iterating a Path, and __contains__ returns False.
-    """
+class DummyPredecessorOrAttributesMapping(MutableMapping[T_vertex_id, T]):
+    def __getitem__(self, key: T_vertex_id) -> T:
+        raise KeyError
 
-    class MappingOfNothing(MutableMapping[T_vertex_id, T_vertex]):
-        def __getitem__(self, key: T_vertex_id) -> T_vertex:
-            raise KeyError
+    def __delitem__(self, key: T_vertex_id) -> None:
+        raise KeyError
 
-        def __delitem__(self, key: T_vertex_id) -> None:
-            raise KeyError
+    def __iter__(self) -> Iterator[T_vertex_id]:
+        return iter(())
 
-        def __iter__(self) -> Iterator[T_vertex_id]:
-            return iter(())
+    def __len__(self) -> int:
+        return 0
 
-        def __len__(self) -> int:
-            return 0
+    def __contains__(self, key: object) -> bool:
+        return False
 
-        def __contains__(self, key: object) -> bool:
-            return False
+    def __setitem__(self, key: T_vertex_id, value: T) -> None:
+        raise RuntimeError(
+            "Cannot add a path, " + "traversal not started or no paths requested."
+        )
 
-        def __setitem__(self, key: T_vertex_id, value: T_vertex):
-            raise RuntimeError(
-                "Cannot add a path, " + "traversal not started or no paths requested."
-            )
 
-    def __init__(self):
-        super().__init__(_PathsDummy.MappingOfNothing(), nographs.vertex_as_id)
+class PathsDummy(Paths[T_vertex, T_vertex_id, T_labels]):
+    """Empty and non-functional default Paths container. Raises RuntimeError
+    for all methods returning or iterating a Path, and __contains__ returns False.
+    """
+
+    def __init__(self, vertex_to_id: VertexToID[T_vertex, T_vertex_id]) -> None:
+        super().__init__(
+            DummyPredecessorOrAttributesMapping[T_vertex_id, T_vertex](),
+            vertex_to_id,
+        )
 
     def _check_vertex(self, vertex: T_vertex) -> T_vertex_id:
         """Raise RuntimeError with helpful explanation. This method
         is called by each method of Paths that returns a path as first step.
         So, they all raise the exception."""
         raise RuntimeError(
             "No paths available: " + "Traversal not started or no paths requested."
@@ -293,15 +300,15 @@
         raise RuntimeError(
             "No paths available: " + "Traversal not started or no paths requested."
         )
 
 
 class PathsOfUnlabeledEdges(Paths[T_vertex, T_vertex_id, Any]):
     """
-    Path of edges that are not labeled, i.e., for some starting vertex, an
+    Paths of edges that are not labeled, i.e., for some starting vertex, an
     edge leading to a specific end vertex is represented only by this end
     vertex.
 
     This class is not part of the public interface of the library. Its
     signature, methods and implementation can be subject to breaking
     changes even in minor releases. It is not intended to be used by
     application code.
@@ -317,15 +324,15 @@
         predecessor: VertexIdToVertexMapping[T_vertex_id, T_vertex],
         vertex_to_id: VertexToID[T_vertex, T_vertex_id],
     ):
         super().__init__(predecessor, vertex_to_id)
 
     def append_edge(
         self, from_vertex: T_vertex, to_vertex_id: T_vertex_id, to_edge: Any
-    ):
+    ) -> None:
         """Create a new path that starts with the existing path to
         from_vertex and ends with the given vertex (resp. id).
 
         :param from_vertex: The resulting path will start with the path to this vertex.
         :param to_vertex_id: The resulting path will end with an edge to this
            vertex (resp. vertex id).
         :param to_edge: The current class ignores this parameter.
@@ -346,15 +353,15 @@
         :param vertex: The path ending at this vertex will be returned.
         """
         return tuple(self.iter_vertices_from_start(vertex))
 
 
 class PathsOfLabeledEdges(Paths[T_vertex, T_vertex_id, T_labels]):
     """
-    Path of edges that are labeled, i.e., for some starting vertex, an
+    Paths of edges that are labeled, i.e., for some starting vertex, an
     edge leading to a specific end vertex is represented by a tuple that
     starts with the end vertex and, optionally, contains additional data.
 
     This class is not part of the public interface of the library. Its
     signature, methods and implementation can be subject to breaking
     changes even in minor releases. It is not intended to be used by
     application code.
@@ -388,15 +395,15 @@
             _,
             self._attributes_collection,
             self._attributes_wrapper,
         ) = access_to_vertex_mapping_expect_none(attributes)
 
     def append_edge(
         self, from_vertex: T_vertex, to_vertex_id: T_vertex_id, to_edge: LabeledOutEdge
-    ):
+    ) -> None:
         """Create a new path that starts with the existing path to
         from_vertex and ends with the given vertex (resp. id). The additional
         edge data provided in to_edge after to_vertex is stored in the path,
         too.
 
         :param from_vertex: The resulting path will start with the path to this vertex.
         :param to_vertex_id: The resulting path will end with an edge to this
```

### Comparing `nographs-3.0.3/src/nographs/strategies.py` & `nographs-3.1.0/src/nographs/_traversals.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,263 +1,93 @@
 from __future__ import annotations
 
 import array
-import itertools
 import copy
+import itertools
 from abc import ABC, abstractmethod
 from collections.abc import (
     Callable,
     Iterator,
     Iterable,
 )
 from heapq import heapify, heappop, heappush
 from numbers import Real
-from typing import TypeVar, Optional, Any, Union, cast, overload, Generic, Literal
+from typing import Optional, Any, Union, cast, overload, Generic, Literal
 
-from nographs import (  # types
-    T_vertex,
-    T_vertex_id,
-    T_weight,
-    T_labels,
-    VertexToID,
-    vertex_as_id,
-    UnweightedLabeledOutEdge,
-    WeightedUnlabeledOutEdge,
-    WeightedLabeledOutEdge,
-    WeightedOutEdge,
-    LabeledOutEdge,
-    OutEdge,
-    WeightedFullEdge,
-)
-from nographs import (  # gear_collections
-    get_wrapper_from_vertex_set,
+from ._gear_collections import (
     access_to_vertex_set,
-    get_wrapper_from_vertex_mapping,
     access_to_vertex_mapping,
     access_to_vertex_mapping_expect_none,
 )
-from nographs import (  # gears
+from ._gears import (
     GearWithoutDistances,
     Gear,
     GearDefault,
     VertexIdSet,
     VertexIdToVertexMapping,
     VertexIdToDistanceMapping,
     VertexIdToPathEdgeDataMapping,
     MutableSequenceOfVertices,
 )
-
-from nographs import (  # paths
+from ._paths import (
     Paths,
-    _PathsDummy,
-    PathsOfUnlabeledEdges,
-    PathsOfLabeledEdges,
+    DummyPredecessorOrAttributesMapping,
+    PathsDummy,
+)
+from ._strategies import (
+    Strategy,
+    T_strategy,
+    NextVertices,
+    NextEdges,
+    NextLabeledEdges,
+    NextWeightedEdges,
+    NextWeightedLabeledEdges,
+    NextEdgesOrVertices,
+    NextWeightedMaybeLabeledEdges,
+    iter_start_ids,
+    iter_start_vertices_and_ids,
+    define_visited,
+    define_distances,
+    create_paths,
+    NoIterator,
+    NoVisitedSet,
+    NoDistancesMapping,
+)
+from ._types import (
+    T_vertex,
+    T_vertex_id,
+    T_weight,
+    T_labels,
+    VertexToID,
+    vertex_as_id,
+    WeightedOutEdge,
+    WeightedFullEdge,
 )
-
-
-# --------------- exported types -------------
-
-# todo: Warning: The following types are manually documented in api.rst
-
-# next vertices and next edges functions for traversals
-# that work with and without weights
-T_traversal = TypeVar("T_traversal")
-
-NextVertices = Callable[[T_vertex, T_traversal], Iterable[T_vertex]]
-
-NextEdges = Callable[[T_vertex, T_traversal], Iterable[OutEdge[T_vertex, Any, Any]]]
-
-NextLabeledEdges = Callable[
-    [T_vertex, T_traversal], Iterable[LabeledOutEdge[T_vertex, Any, T_labels]]
-]
-
-# next edges functions for traversal that work with weights
-NextWeightedEdges = Callable[
-    [T_vertex, T_traversal],
-    Iterable[
-        Union[
-            WeightedUnlabeledOutEdge[T_vertex, T_weight],
-            WeightedLabeledOutEdge[T_vertex, T_weight, Any],
-        ]
-    ],
-]
-
-NextWeightedLabeledEdges = Callable[
-    [T_vertex, T_traversal],
-    Iterable[WeightedLabeledOutEdge[T_vertex, T_weight, T_labels]],
-]
-
-
-# --------------- internal types -------------
-
-NextEdgesOrVertices = Callable[
-    [T_vertex, T_traversal],
-    Iterable[
-        Union[
-            T_vertex,
-            WeightedUnlabeledOutEdge[T_vertex, Any],
-            UnweightedLabeledOutEdge[T_vertex, T_labels],
-            WeightedLabeledOutEdge[T_vertex, Any, T_labels],
-        ]
-    ],
-]
-
-NextWeightedMaybeLabeledEdges = Callable[
-    [T_vertex, T_traversal],
-    Iterable[
-        Union[
-            WeightedUnlabeledOutEdge[T_vertex, T_weight],
-            WeightedLabeledOutEdge[T_vertex, T_weight, T_labels],
-        ]
-    ],
-]
 
 
 # --------------- internal support functions -------------
 
 
-def _start_from_needs_traversal_object(obj: Any):
+def _start_from_needs_traversal_object(obj: Any) -> None:
     if not isinstance(obj, Traversal):
         raise RuntimeError(
             "Method start_from can only be called on a Traversal object."
         )
 
 
-def _iter_start_ids(
-    start_vertices: Iterable[T_vertex], vertex_to_id: VertexToID[T_vertex, T_vertex_id]
-) -> Iterable[T_vertex_id]:
-    """Compute vertex ids for given start vertices and allow for iterating
-    them"""
-    if vertex_to_id == vertex_as_id:
-        # If the identity function (in a mathematical sense)
-        # vertex_as_id is used with correct typing, this means that
-        # T_vertex is a subtype of T_vertex_id (typically: identical).
-        # So, instead of applying the function, we could just cast the vertices
-        # to vertex ids. For improved performance, we cast the whole iterator.
-        return cast(Iterable[T_vertex_id], start_vertices)
-
-    return (vertex_to_id(vertex) for vertex in start_vertices)
-
-
-def _iter_start_vertices_and_ids(
-    start_vertices: Iterable[T_vertex], vertex_to_id: VertexToID[T_vertex, T_vertex_id]
-) -> Iterable[tuple[T_vertex, T_vertex_id]]:
-    """Compute vertex ids for given start vertices and allow for iterating
-    pairs of vertex and vertex id."""
-    if vertex_to_id == vertex_as_id:
-        # If the identity function (in a mathematical sense)
-        # vertex_as_id is used with correct typing, this means that
-        # T_vertex is a subtype of T_vertex_id (typically: identical).
-        # So, instead of applying the function, we could just cast the vertices
-        # to vertex ids. For improved performance, we cast the whole iterator.
-        vertices_and_vertices = ((vertex, vertex) for vertex in start_vertices)
-        vertices_and_ids = cast(
-            Iterator[tuple[T_vertex, T_vertex_id]], vertices_and_vertices
-        )
-        return vertices_and_ids
-
-    return ((vertex, vertex_to_id(vertex)) for vertex in start_vertices)
-
-
-def _define_visited(
-    gear: GearWithoutDistances[T_vertex, T_vertex_id, T_labels],
-    already_visited: Optional[VertexIdSet[T_vertex_id]],
-    iter_start_ids: Iterable[T_vertex_id],
-    is_tree: bool,
-) -> VertexIdSet[T_vertex_id]:
-    """Use and return already_visited, if provided, for storing visited vertices,
-    and otherwise a new VertexIdSet. Mark start vertices as visited."""
-    if already_visited is None:
-        return gear.vertex_id_set(() if is_tree else iter_start_ids)
-
-    if not is_tree:
-        if (wrapper := get_wrapper_from_vertex_set(already_visited)) is None:
-            method_add = already_visited.add
-            for v_id in iter_start_ids:
-                method_add(v_id)
-        else:
-            wrapper.update_from_keys(iter_start_ids)
-    return already_visited
-
-
-def _define_distances(
-    gear: Gear[T_vertex, T_vertex_id, T_weight, T_labels],
-    known_distances: Optional[VertexIdToDistanceMapping[T_vertex_id, T_weight]],
-    iter_start_ids_and_distances: Iterable[tuple[T_vertex_id, T_weight]],
-    is_tree: bool,
-) -> VertexIdToDistanceMapping[T_vertex_id, T_weight]:
-    """Use and return known_distances, if provided, for storing vertex distances, and
-    otherwise new VertexIdToDistanceMapping. Store the distances given for the
-    start vertices."""
-    if known_distances is None:
-        return gear.vertex_id_to_distance_mapping(iter_start_ids_and_distances)
-
-    if not is_tree:
-        if (wrapper := get_wrapper_from_vertex_mapping(known_distances)) is None:
-            method_setdefault = known_distances.setdefault
-            for v_id, distance in iter_start_ids_and_distances:
-                method_setdefault(v_id, distance)
-        else:
-            wrapper.update_default(iter_start_ids_and_distances)
-
-    return known_distances
-
-
-def _create_no_paths():
-    """Create setting of paths, predecessors and attributes collections
-    (here: None) for case that no paths should be built."""
-    return None, None, None
-
-
-def _create_paths(
-    gear: GearWithoutDistances[T_vertex, T_vertex_id, T_labels],
-    labeled_edges: bool,
-    vertex_to_id: VertexToID[T_vertex, T_vertex_id],
-    start_vertices: Iterable[T_vertex],
-) -> tuple[
-    Paths[T_vertex, T_vertex_id, T_labels],
-    VertexIdToVertexMapping[T_vertex_id, T_vertex],
-    Optional[VertexIdToPathEdgeDataMapping[T_vertex_id, T_labels]],
-]:
-    """Translate from configuration of path generation to setting of
-    paths, predecessors and attributes collection. Store empty paths for start
-    vertices."""
-
-    # Create container for predecessors.
-    # From each start vertex, store an empty paths to itself.
-    predecessor = gear.vertex_id_to_vertex_mapping(
-        (
-            (vertex_id, vertex)
-            for vertex, vertex_id in _iter_start_vertices_and_ids(
-                start_vertices, vertex_to_id
-            )
-        )
-    )
-    paths: Paths[T_vertex, T_vertex_id, T_labels]
-    attributes: Optional[VertexIdToPathEdgeDataMapping[T_vertex_id, T_labels]]
-    if labeled_edges:
-        attributes = gear.vertex_id_to_path_attributes_mapping(())
-        paths = PathsOfLabeledEdges[T_vertex, T_vertex_id, T_labels](
-            predecessor, attributes, vertex_to_id
-        )
-    else:
-        paths = PathsOfUnlabeledEdges[T_vertex, T_vertex_id](predecessor, vertex_to_id)
-        attributes = None
-    return paths, predecessor, attributes
-
-
 def _create_unified_next(
-    next_vertices: Optional[NextVertices[T_vertex, T_traversal]],
-    next_edges: Optional[NextEdges[T_vertex, T_traversal]],
-    next_labeled_edges: Optional[NextLabeledEdges[T_vertex, T_traversal, T_labels]],
-) -> tuple[NextEdgesOrVertices[T_vertex, T_traversal, T_labels], bool, bool]:
+    next_vertices: Optional[NextVertices[T_vertex, T_strategy]],
+    next_edges: Optional[NextEdges[T_vertex, T_strategy]],
+    next_labeled_edges: Optional[NextLabeledEdges[T_vertex, T_strategy, T_labels]],
+) -> tuple[NextEdgesOrVertices[T_vertex, T_strategy, T_labels], bool, bool]:
     """Check configuration of given next_vertices, next_edges, and next_labeled_edges
-    and calculate unified NextEdgesOrVertices[] and whether we have edges with data
-    (weights and/or labels) and/or labeled_edges."""
-    next_edges_or_vertices: NextEdgesOrVertices[T_vertex, T_traversal, T_labels]
+    and calculate unified NextEdgesOrVertices
+    and whether we have edges with data (weights and/or labels) and/or labeled_edges.
+    """
+    next_edges_or_vertices: NextEdgesOrVertices[T_vertex, T_strategy, T_labels]
     if next_vertices is not None:
         if next_edges is not None:
             raise RuntimeError("Both next_vertices and next_edges provided.")
         if next_labeled_edges is not None:
             raise RuntimeError("Both next_vertices and next_labeled_edges provided.")
         next_edges_or_vertices = next_vertices
         edges_with_data = False
@@ -277,61 +107,43 @@
         next_edges_or_vertices = next_labeled_edges
         edges_with_data = True
         labeled_edges = True
     return next_edges_or_vertices, edges_with_data, labeled_edges
 
 
 def _create_unified_next_weighted(
-    next_edges: Optional[NextWeightedEdges[T_vertex, T_traversal, T_weight]],
+    next_edges: Optional[NextWeightedEdges[T_vertex, T_strategy, T_weight]],
     next_labeled_edges: Optional[
-        NextWeightedLabeledEdges[T_vertex, T_traversal, T_weight, T_labels]
+        NextWeightedLabeledEdges[T_vertex, T_strategy, T_weight, T_labels]
     ],
 ) -> tuple[
-    NextWeightedMaybeLabeledEdges[T_vertex, T_traversal, T_weight, T_labels], bool
+    NextWeightedMaybeLabeledEdges[T_vertex, T_strategy, T_weight, T_labels], bool
 ]:
-    """Check configuration of given next_vertices and next_edges and calculate
-    unified NextEdgesOrVertices[] and whether we have labeled_edges."""
+    """Check configuration of given next_edges and next_labeled_edges and calculate
+    unified _NextWeightedMaybeLabeledEdges[] and whether we have labeled_edges."""
     next_maybe_labeled_edges: NextWeightedMaybeLabeledEdges[
-        T_vertex, T_traversal, T_weight, T_labels
+        T_vertex, T_strategy, T_weight, T_labels
     ]
     if next_edges is not None:
         if next_labeled_edges is not None:
             raise RuntimeError("Both next_edges and next_labeled_edges provided.")
         next_maybe_labeled_edges = next_edges
         labeled_edges = False
     else:
         if next_labeled_edges is None:
             raise RuntimeError("Neither next_edges and next_labeled_edges provided.")
         next_maybe_labeled_edges = next_labeled_edges
         labeled_edges = True
     return next_maybe_labeled_edges, labeled_edges
 
 
-class NoIterator(Generic[T_vertex]):
-    def __next__(self) -> T_vertex:
-        """
-        >>> next(NoIterator())
-        Traceback (most recent call last):
-        RuntimeError: Traversal not started, iteration not possible
-        """
-        raise RuntimeError("Traversal not started, iteration not possible")
-
-    def __iter__(self):
-        """
-        >>> iter(NoIterator())
-        Traceback (most recent call last):
-        RuntimeError: Traversal not started, iteration not possible
-        """
-        raise RuntimeError("Traversal not started, iteration not possible")
-
-
 # -- traversal strategies for unweighted graphs with or without edge labels --
 
 
-class Traversal(ABC, Generic[T_vertex, T_vertex_id, T_labels]):
+class Traversal(Strategy[T_vertex, T_vertex_id, T_labels]):
     """
     Abstract Class. Its subclasses provide methods to iterate through vertices
     and edges using some specific traversal strategies.
     """
 
     @abstractmethod
     def __init__(
@@ -343,32 +155,32 @@
         # -- attributes of graph adaptation
         self._labeled_edges = labeled_edges
         self._is_tree = is_tree
         self._vertex_to_id = vertex_to_id
 
         # -- general attributes set and needed by all traversal strategies
         self._generator: Iterator[T_vertex] = NoIterator[T_vertex]()
-        self._start_vertices: tuple[T_vertex, ...] = tuple[T_vertex]()
+        self._start_vertices: Iterable[T_vertex] = tuple[T_vertex]()
         self._build_paths: bool = False
         self._calculation_limit: Optional[int] = None
 
         # -- attributes for path data, needed by all traversal strategies
-        self.paths: Paths[T_vertex, T_vertex_id, T_labels] = _PathsDummy[
-            T_vertex, T_vertex_id
-        ]()
-        """ If path creation has been demanded, the container *paths* provides the
-        found paths for all vertices visited so far. If labeled edges were provided,
-        the paths contain them instead of just vertices, if demanded.
-        """
-        self._predecessors: Optional[
-            VertexIdToVertexMapping[T_vertex_id, T_vertex]
-        ] = None
-        self._attributes: Optional[
-            VertexIdToPathEdgeDataMapping[T_vertex_id, T_labels]
-        ] = None
+        self.paths: Paths[T_vertex, T_vertex_id, T_labels] = PathsDummy[
+            T_vertex, T_vertex_id, T_labels
+        ](vertex_to_id)
+        """ The container *paths* holds the created paths, if path creation has been
+        demanded. If labeled edges were provided (parameter *next_labeled_edges*), the
+        paths contain them instead of just vertices.
+        """
+        self._predecessors: VertexIdToVertexMapping[
+            T_vertex_id, T_vertex
+        ] = DummyPredecessorOrAttributesMapping[T_vertex_id, T_vertex]()
+        self._attributes: VertexIdToPathEdgeDataMapping[
+            T_vertex_id, T_labels
+        ] = DummyPredecessorOrAttributesMapping[T_vertex_id, T_labels]()
 
     def __iter__(
         self,
     ) -> Iterator[T_vertex]:  # Type alias needed do to a sphinx limitation
         """
         Return the iterator of a started traversal. This allows for using a
         `Traversal` in *for* loops or as parameter to a call of function
@@ -395,18 +207,21 @@
 
     def go_for_vertices_in(
         self, vertices: Iterable[T_vertex], fail_silently: bool = False
     ) -> Iterator[T_vertex]:
         """
         For a started traversal, return an iterator that fetches vertices
         from the traversal, reports a vertex if it is in *vertices*, and stops when
-        all the *vertices* have been found and reported. If the iterator has no
-        more vertices to report (graph is exhausted) without having found all the
-        *vertices*, KeyError is raised, or the traversal just terminates, if a silent
-        fail is demanded.
+        all the *vertices* have been found and reported.
+
+        If the iterator has no more vertices to report (graph is exhausted) without
+        having found all the *vertices*, KeyError is raised, or the traversal just
+        terminates, if a silent fail is demanded.
+
+        If *vertices* does not provide any vertices, an empty iterator is returned.
 
         If a `VertexToID` function is used, the method searches for vertices
         that have the same id as one of the *vertices*.
 
         Whenever a vertex is reported, specific attributes of the traversal object
         contain additional data about the state of the traversal (see the API
         documentation of the respective subclass of `Traversal`).
@@ -423,39 +238,36 @@
         # In order to make the above check work, the following generator functionality
         # needs to be encapsulated in a local function
 
         def my_generator() -> Iterator[T_vertex]:
             vertex_to_id = self._vertex_to_id
             if vertex_to_id == vertex_as_id:
                 vertex_set = set(cast(Iterable[T_vertex_id], vertices))
-
                 v_count = len(vertex_set)
-                for v in self._generator:
-                    if v not in vertex_set:
-                        continue
-                    yield v
-                    v_count -= 1
-                    if v_count == 0:
-                        break
-                else:
-                    if not fail_silently:
-                        raise KeyError("Not all of the given vertices have been found")
+                if v_count:
+                    for v in self._generator:
+                        if v not in vertex_set:
+                            continue
+                        yield v
+                        v_count -= 1
+                        if v_count == 0:
+                            break
             else:
                 vertex_set = set(vertex_to_id(vertex) for vertex in vertices)
                 v_count = len(vertex_set)
-                for v in self._generator:
-                    if vertex_to_id(v) not in vertex_set:
-                        continue
-                    yield v
-                    v_count -= 1
-                    if v_count == 0:
-                        break
-                else:
-                    if not fail_silently:
-                        raise KeyError("Not all of the given vertices have been found")
+                if v_count:
+                    for v in self._generator:
+                        if vertex_to_id(v) not in vertex_set:
+                            continue
+                        yield v
+                        v_count -= 1
+                        if v_count == 0:
+                            break
+            if v_count > 0 and not fail_silently:
+                raise KeyError("Not all of the given vertices have been found")
 
         return my_generator()
 
     @overload
     def go_to(
         self, vertex: T_vertex, fail_silently: Literal[False] = False
     ) -> T_vertex:
@@ -517,90 +329,97 @@
     def _start_from(
         self,
         start_vertex: Optional[T_vertex],
         start_vertices: Optional[Iterable[T_vertex]],
         build_paths: bool,
         calculation_limit: Optional[int],
         gear: GearWithoutDistances[T_vertex, T_vertex_id, T_labels],
-    ):
+    ) -> None:
+        # Check start vertices options. Compute multi-vertices form from single vertex.
         if start_vertex is not None:
             if start_vertices is not None:
                 raise RuntimeError("Both start_vertex and start_vertices provided.")
             self._start_vertices = (start_vertex,)
         else:
             if start_vertices is None:
                 raise RuntimeError("Neither start_vertex nor start_vertices provided.")
-            self._start_vertices = tuple(start_vertices)  # copy from iterable
+            self._start_vertices = start_vertices
 
-        # Note: Detection of wrong option combinations for paths is implemented in
-        # _create_paths and _create_no_paths.
-        self.paths, self._predecessors, self._attributes = (
-            _create_paths(
-                gear,
-                self._labeled_edges,
-                self._vertex_to_id,
-                self._start_vertices,
-            )
-            if build_paths
-            else _create_no_paths()
+        # Create and store path container and path setting
+        self._build_paths = build_paths
+        self.paths, self._predecessors, self._attributes = create_paths(
+            build_paths,
+            gear,
+            self._labeled_edges,
+            self._vertex_to_id,
+            self._start_vertices,
         )
+
+        # store calculation limit
         self._calculation_limit = calculation_limit
 
     def _start(self) -> None:
         self._generator = self._traverse()
 
     @abstractmethod
     def _traverse(self) -> Iterator[T_vertex]:
         """Has to be implemented in subclass"""
 
+    def state_to_str(self, vertices: Optional[Iterable[T_vertex]] = None) -> str:
+        more = dict()
+        if vertices is not None and self._build_paths:
+            for vertex in vertices:
+                more[f"paths[{vertex}]"] = self.paths[vertex]
+        return self._state_and_more_to_str(less=["paths"], more=more)
+
 
 # -------------- Traversal strategies for unweighted edges -----------------
 
 
 class _TraversalWithoutWeights(Traversal[T_vertex, T_vertex_id, T_labels], ABC):
+    """Internal: A traversal without weight type and distances collection, but
+    with attribute visited."""
+
     def __init__(
         self,
         edges_with_data: bool,
         labeled_edges: bool,
         is_tree: bool,
         vertex_to_id: VertexToID[T_vertex, T_vertex_id],
         gear: GearWithoutDistances[T_vertex, T_vertex_id, T_labels],
     ) -> None:
         super().__init__(labeled_edges, is_tree, vertex_to_id)
         self._edges_with_data = edges_with_data
         self._gear = gear
-        self.visited: Optional[VertexIdSet[T_vertex_id]] = None
-        """ A collection that contains the vertices (resp. their hashable ids
-        from vertex_to_id) that have been visited so far, and the start
-        vertices. After an exhaustive search, it contains
+        self.visited: VertexIdSet[T_vertex_id] = NoVisitedSet[T_vertex_id]()
+        """ A collection that contains the visited vertices (resp. their hashable ids
+        from vertex_to_id). After an exhaustive search, it contains
         the vertices (resp. vertex ids) reachable from the start vertices.
         """
 
     def _start_with_or_without_labels_from(
         self,
         start_vertex: Optional[T_vertex],
         start_vertices: Optional[Iterable[T_vertex]],
         build_paths: bool,
         calculation_limit: Optional[int],
         already_visited: Optional[VertexIdSet[T_vertex_id]],
-    ):
+    ) -> None:
         _start_from_needs_traversal_object(self)
-
         self._start_from(
             start_vertex,
             start_vertices,
             build_paths,
             calculation_limit,
             self._gear,
         )
-
-        self.visited = _define_visited(
+        self.visited = define_visited(
             self._gear,
             already_visited,
-            _iter_start_ids(self._start_vertices, self._vertex_to_id),
+            iter_start_ids(self._start_vertices, self._vertex_to_id),
             self._is_tree,
         )
         super()._start()
 
 
 class _TraversalWithoutWeightsBasic(
     _TraversalWithoutWeights[T_vertex, T_vertex_id, T_labels], ABC
@@ -617,19 +436,19 @@
     ) -> Traversal[T_vertex, T_vertex_id, T_labels]:
         """
         Start the traversal at a vertex or a set of vertices and set parameters.
 
         :param start_vertex: The vertex the search should start at. If None, provide
             start_vertices.
 
-        :param start_vertices: The vertices (iterator) the search should start at. Only
+        :param start_vertices: The vertices the search should start at. Only
             allowed if start_vertex equals None.
 
         :param build_paths: If true, build paths from some start vertex to each visited
-            vertex.
+            vertex. Paths of start vertices are empty paths.
 
         :param calculation_limit: If provided, maximal number of vertices to process
             (read in) from your graph. If it is exceeded, a RuntimeError will be raised.
 
         :param already_visited: If provided, this set is used instead of an internal
             one to keep vertices (resp. their hashable ids from vertex_to_id),
             that have already been visited. This parameter can be used to get online
@@ -658,15 +477,15 @@
     ) -> Traversal[T_vertex, T_vertex_id, T_labels]:
         """
         Start the traversal at a vertex or a set of vertices and set parameters.
 
         :param start_vertex: The vertex the search should start at. If None, provide
             start_vertices.
 
-        :param start_vertices: The vertices (iterator) the search should start at. Only
+        :param start_vertices: The vertices the search should start at. Only
             allowed if start_vertex equals None.
 
         :param build_paths: If true, build paths from some start vertex to each visited
             vertex.
 
         :param compute_depth: For each reported vertex, provide the search depth is has
             been found at (Note: Often, this information is not helpful, and the
@@ -698,32 +517,34 @@
 
     :param gear: See `gears API <gears_api>` and class `GearWithoutDistances`.
 
     :param next_vertices: See `NextVertices` function. If None, provide next_edges
      or next_labeled_edges.
 
     :param next_edges: See `NextEdges` function. Only allowed if next_vertices equals
-     None. If both are None, provide next_labeled_edges.
+      None. If both are None, provide next_labeled_edges.
 
-    :param next_labeled_edges: See `NextEdges` function. Only allowed if next_vertices
-     and next_edges equal None. If given, paths will record the given labels.
+    :param next_labeled_edges: See `NextLabeledEdges` function. Only allowed if
+      next_vertices and next_edges equal None. If given, paths will record the given
+      labels.
 
     :param is_tree: bool: If it is certain, that during each traversal run,
      each vertex can be reached only once, is_tree can be set to True. This
      improves performance, but attribute *visited* of the traversal will not be
      updated during and after the traversal.
 
     **Algorithm:** Breadth First Search, non-recursive, based on FIFO queue,
     vertices are reported when they are first "seen".
 
-    **Properties:** Visits and reports vertices in breadth first order, i.e.,
+    **Properties:** Reports and expands vertices in breadth first order, i.e.,
     with ascending depth (edge count of the path with the fewest edges from a start
-    vertex). If paths are demanded, all computed paths are *shortest paths*,
-    i.e., paths with minimal number of edges from a start vertex to their end vertex.
-    Vertices are regarded as visited when they have been seen.
+    vertex). All computed paths are *shortest paths* , i.e., paths with minimal number
+    of edges from a start vertex to their end vertex.
+    A vertex is regarded as visited when it has been reported or if it is a start
+    vertex.
 
     **Input:** Directed graph. Unlabeled or labeled edges. One or more start
     vertices. Optional calculation limit.
 
     **Search state:** When a vertex is
     *expanded* (traversal calls next_vertices, next_edges or next_labeled_edges)
     or *reported* (an iterator of the traversal returns it),
@@ -752,117 +573,107 @@
                 TraversalBreadthFirstFlex[T_vertex, T_vertex_id, T_labels],
                 T_labels,
             ]
         ] = None,
         is_tree: bool = False,
     ) -> None:
         (
-            self.next_edge_or_vertex,
-            self.edges_with_data,
-            self.labeled_edges,
+            self._next_edge_or_vertex,
+            edges_with_data,
+            labeled_edges,
         ) = _create_unified_next(next_vertices, next_edges, next_labeled_edges)
-        super().__init__(
-            self.edges_with_data, self.labeled_edges, is_tree, vertex_to_id, gear
-        )
+        super().__init__(edges_with_data, labeled_edges, is_tree, vertex_to_id, gear)
         self.depth: int = -1  # value not used, initialized during traversal
         """ At this *search depth*, the reported (resp. the expanded) vertex has been
         found. It equals the length (number of edges) of the created path to the
         vertex, if path creation is demanded.
         For the special case of TraversalBreadthFirst, it equals the
         *depth of the vertex* (minimal number of edges needed to come to it
         from a start vertex).
+        When a traversal has been started, but no vertex has been reported or expanded
+        so far, the depth is 0 (depth of the start vertices).
         """
+        self._report_depth_increase = False
 
     def start_from(
         self,
         start_vertex: Optional[T_vertex] = None,
         *,
         start_vertices: Optional[Iterable[T_vertex]] = None,
         build_paths: bool = False,
         calculation_limit: Optional[int] = None,
         already_visited: Optional[VertexIdSet[T_vertex_id]] = None,
+        _report_depth_increase: bool = False,  # hidden parameter for internal use
     ) -> TraversalBreadthFirstFlex[T_vertex, T_vertex_id, T_labels]:
         _start_from_needs_traversal_object(self)
         self._start_with_or_without_labels_from(
             start_vertex,
             start_vertices,
             build_paths,
             calculation_limit,
             already_visited,
         )
+        self._report_depth_increase = _report_depth_increase
+        self.depth = 0
         return self
 
     def _traverse(self) -> Iterator[T_vertex]:
         # ----- Prepare efficient environment for inner loop -----
         # Copy Traversal attributes into method scope (faster access)
         labeled_edges = self._labeled_edges
         is_tree = self._is_tree
         maybe_vertex_to_id = (
             None if self._vertex_to_id == vertex_as_id else self._vertex_to_id
         )  # Case vertex_as_id: not apply; T_vertex_id > T_vertex
+        build_paths = self._build_paths
         calculation_limit = self._calculation_limit
-        paths = self.paths
+        report_depth_increase = self._report_depth_increase
         predecessors = self._predecessors
         attributes = self._attributes
 
         # Prepare limit check done by zero check
         if calculation_limit is not None:
             calculation_limit += 1
 
         # Copy _TraversalWithoutWeights attributes into method scope
         edges_with_data = self._edges_with_data
-        next_edge_or_vertex = self.next_edge_or_vertex
+        next_edge_or_vertex = self._next_edge_or_vertex
         visited = self.visited
-        assert visited is not None
-
-        # Create booleans (avoid checks with "is")
-        attributes_exists = attributes is not None
 
         # Get references of used gear objects and methods (avoid attribute resolution)
         visited_add = visited.add
         (
             visited_uses_sequence,
             visited_sequence,
             visited_wrapper,
             visited_uses_bits,
             index_and_bit_method,
         ) = access_to_vertex_set(visited)
-
-        if paths:  # has no __len__, so this checks for non-None
-            assert predecessors is not None
-            (
-                _,
-                predecessors_sequence,
-                predecessors_wrapper,
-            ) = access_to_vertex_mapping_expect_none(predecessors)
-
-        if attributes_exists:
-            assert labeled_edges
-            assert attributes is not None
-            (
-                _,
-                attributes_sequence,
-                attributes_wrapper,
-            ) = access_to_vertex_mapping_expect_none(attributes)
+        (
+            _,
+            predecessors_sequence,
+            predecessors_wrapper,
+        ) = access_to_vertex_mapping_expect_none(predecessors)
+        (
+            _,
+            attributes_sequence,
+            attributes_wrapper,
+        ) = access_to_vertex_mapping_expect_none(attributes)
 
         # ----- Initialize method specific bookkeeping -----
 
         # Two lists used as FIFO queue with just two buckets
         # (using a queue and counting down the size of current depth horizon is slower,
         # and creating a new list instead of clear() is also slower)
 
-        # to_expand = list(self._start_vertices)
-        # next_to_expand = list[T_vertex]()
-
         to_expand = self._gear.sequence_of_vertices(self._start_vertices)
         next_to_expand = self._gear.sequence_of_vertices(())
 
         prev_traversal = copy.copy(self)  # copy of self, for keeping previous depth
-        self.depth = 1
-        prev_traversal.depth = 0
+        self.depth = 1  # used for reporting (prev_traversal starts at 0)
 
         # Get method references of specific bookkeeping (avoid attribute resolution)
         to_expand_append = to_expand.append
         next_to_expand_append = next_to_expand.append
 
         # ----- Typing preparation of inner loop -----
 
@@ -888,15 +699,15 @@
                     calculation_limit := calculation_limit - 1
                 ):
                     raise RuntimeError("Number of visited vertices reached limit")
 
                 for edge_or_vertex in next_edge_or_vertex(vertex, prev_traversal):
                     neighbor = edge_or_vertex[0] if edges_with_data else edge_or_vertex
 
-                    if not is_tree or paths:
+                    if not is_tree or build_paths:
                         n_id: T_vertex_id = (
                             maybe_vertex_to_id(neighbor)  # type: ignore[assignment]
                             if maybe_vertex_to_id
                             else neighbor
                         )
 
                         # If not is_tree: Ignore neighbor if already seen, and
@@ -926,37 +737,40 @@
                                 try:
                                     if visited_sequence[n_id]:
                                         continue
                                     visited_sequence[n_id] = True
                                 except IndexError:
                                     visited_wrapper.extend_and_set(n_id, True)
 
-                        if paths:
+                        if build_paths:
                             # Store the predecessor (vertex) of the neighbor
                             try:
-                                # noinspection PyUnboundLocalVariable
                                 predecessors_sequence[n_id] = vertex
                             except IndexError:
-                                # noinspection PyUnboundLocalVariable
                                 predecessors_wrapper.extend_and_set(n_id, vertex)
                             # Store the labels of the edge to the neighbor
-                            if attributes_exists:
+                            if labeled_edges:
                                 edge_data = edge_or_vertex[-1]
                                 try:
-                                    # noinspection PyUnboundLocalVariable
                                     attributes_sequence[n_id] = edge_data
                                 except IndexError:
-                                    # noinspection PyUnboundLocalVariable
                                     attributes_wrapper.extend_and_set(n_id, edge_data)
 
                     # Vertex has been seen, report it now
                     yield neighbor
                     # Needs to be expanded in the next round
                     next_to_expand_append(neighbor)
 
+            if report_depth_increase and next_to_expand:
+                # We are not finished yet, because we found new vertices to expand,
+                # and we are about to increase the depth now, and it is demanded
+                # to report this situation by reporting the last vertex reported so far
+                # again. So we report it again.
+                yield next_to_expand[-1]
+
             # Update external views (reporting/expanding) on depth
             self.depth += 1
             prev_traversal.depth += 1
             # Prepare state for next depth level of vertices
             to_expand, next_to_expand, to_expand_append, next_to_expand_append = (
                 next_to_expand,
                 to_expand,
@@ -983,15 +797,15 @@
             raise RuntimeError(
                 "Method go_for_depth_range can only be called "
                 + "on a Traversal object."
             )
 
         # In order to make the above check work, the following generator functionality
         # needs to be encapsulated in a local function
-        def my_generator():
+        def my_generator() -> Iterator[T_vertex]:
             for v in self._generator:
                 if self.depth >= start:
                     if self.depth < stop:
                         yield v
                     break
             for v in self._generator:
                 if self.depth >= stop:
@@ -1058,30 +872,32 @@
 
     :param next_vertices: See `NextVertices` function. If None, provide next_edges
      or next_labeled_edges.
 
     :param next_edges: See `NextEdges` function. Only allowed if next_vertices equals
      None. If both are None, provide next_labeled_edges.
 
-    :param next_labeled_edges: See `NextEdges` function. Only allowed if next_vertices
-     and next_edges equal None. If given, paths will record the given labels.
+    :param next_labeled_edges: See `NextLabeledEdges` function. Only allowed if
+      next_vertices and next_edges equal None. If given, paths will record the given
+      labels.
 
     :param is_tree: bool: If it is certain, that during each traversal run, each vertex
         can be reached only once, is_tree can be set to True. This improves
         performance, but attribute *visited* of the traversal will not be updated
         during and after the traversal.
 
     **Algorithm:** Depth First Search ("BFS"), non-recursive, based on stack,
     vertices are reported when they are about to be expanded (neighbors read from the
     graph).
 
-    **Properties:** Follows edges to new vertices as long as possible, and goes back
-    a step and follows further edges that start at some visited vertex only if
-    necessary to come to new vertices.
-    A vertex is regarded as visited when the traversal started reporting it.
+    **Properties:** Follows edges to new vertices (and reports and expands them) as
+    long as possible, and goes back a step and follows further edges that start at some
+    visited vertex only if necessary to come to new vertices.
+    A vertex is regarded as visited when it has been reported or if it is a start
+    vertex.
 
     **Input:** Directed graph. One or more start vertices. Vertices must be
     hashable, or hashable id can be provided. Unlabeled or labeled edges. Optional
     calculation limit.
 
     **Search state:** When a vertex is
     *expanded* (traversal calls next_vertices, next_edges or next_labeled_edges)
@@ -1111,28 +927,28 @@
                 TraversalDepthFirstFlex[T_vertex, T_vertex_id, T_labels],
                 T_labels,
             ]
         ] = None,
         is_tree: bool = False,
     ) -> None:
         (
-            self.next_edge_or_vertex,
-            self.edges_with_data,
-            self.labeled_edges,
+            self._next_edge_or_vertex,
+            edges_with_data,
+            labeled_edges,
         ) = _create_unified_next(next_vertices, next_edges, next_labeled_edges)
-        super().__init__(
-            self.edges_with_data, self.labeled_edges, is_tree, vertex_to_id, gear
-        )
+        super().__init__(edges_with_data, labeled_edges, is_tree, vertex_to_id, gear)
         self.depth: int = -1  # value not used
         """ If depth computation has been demanded:
         At this *search depth*, the reported (resp. the expanded) vertex has been
         found. It equals the length (number of edges) of the created path to the
         vertex, if path creation is demanded.
         Note: The search depth does not need to be the depth of the vertex
         (see `TraversalBreadthFirstFlex`).
+        When a traversal has been started, but no vertex has been reported or expanded
+        so far, the depth is 0 (depth of the start vertices).
         """
         self._compute_depth = False  # value not used
         self._allow_reordering = False  # value not used
 
     def start_from(
         self,
         start_vertex: Optional[T_vertex] = None,
@@ -1148,42 +964,42 @@
             start_vertex,
             start_vertices,
             build_paths,
             calculation_limit,
             already_visited,
         )
         self._compute_depth = compute_depth
+        self.depth = 0
         return self
 
     def _traverse(self) -> Iterator[T_vertex]:
         # ----- Prepare efficient environment for inner loop -----
         # Copy Traversal attributes into method scope (faster access)
         labeled_edges = self._labeled_edges
         compute_depth = self._compute_depth
         is_tree = self._is_tree
         maybe_vertex_to_id = (
             None if self._vertex_to_id == vertex_as_id else self._vertex_to_id
         )  # Case vertex_as_id: not apply; T_vertex_id > T_vertex
+        build_paths = self._build_paths
         calculation_limit = self._calculation_limit
         paths = self.paths
         predecessors = self._predecessors
         attributes = self._attributes
 
         # Prepare limit check done by zero check
         if calculation_limit is not None:
             calculation_limit += 1  # Allows for limit check by zero check
 
         # Copy _TraversalWithoutWeights attributes into method scope
         edges_with_data = self._edges_with_data
-        next_edge_or_vertex = self.next_edge_or_vertex
+        next_edge_or_vertex = self._next_edge_or_vertex
         visited = self.visited
-        assert visited is not None
 
         # Create booleans (avoid checks with "is", make decisions clear)
-        attributes_exists = attributes is not None
         check_and_set_visited_on_expand = not is_tree
         check_visited_when_seen = paths and not is_tree
         # An alternative is, to choose here: not is_tree.
         # This always checks and avoids taking already visited vertices
         # on top of the stack. It saves space, but costs runtime.
         # For an average of n children per node, it reduces the
         # space needed by the stack by factor 1/(n/2), e.g. for 6
@@ -1198,77 +1014,76 @@
         (
             visited_uses_sequence,
             visited_sequence,
             visited_wrapper,
             visited_uses_bits,
             index_and_bit_method,
         ) = access_to_vertex_set(visited)
-        if paths:  # has no __len__, so this checks for non-None
-            assert predecessors is not None
-            (
-                _,
-                predecessors_sequence,
-                predecessors_wrapper,
-            ) = access_to_vertex_mapping_expect_none(predecessors)
-        if attributes is not None:
-            assert labeled_edges
-            (
-                _,
-                attributes_sequence,
-                attributes_wrapper,
-            ) = access_to_vertex_mapping_expect_none(attributes)
+        (
+            _,
+            predecessors_sequence,
+            predecessors_wrapper,
+        ) = access_to_vertex_mapping_expect_none(predecessors)
+        (
+            _,
+            attributes_sequence,
+            attributes_wrapper,
+        ) = access_to_vertex_mapping_expect_none(attributes)
 
         # ----- Initialize method specific bookkeeping -----
 
-        depth = -1
+        depth = -1  # The inner loop starts with incrementing, so, we pre-decrement
         if not compute_depth:
-            self.depth = depth
-
-        if len(self._start_vertices) == 0:
-            return
+            self.depth = depth  # In this case, we leave the -1 the whole time
 
         # vertices to enter or leave
         to_visit = self._gear.sequence_of_vertices(self._start_vertices)
         to_visit_append = to_visit.append
         to_visit_pop = to_visit.pop
 
         if compute_depth:
             # Sequence of flag bytes (store in a Q array) marking the vertices to leave
             # by 1 and the vertices to enter by 0.
             # Initially, store a zero flag for each start vertex.
-            to_leave_markers = array.array(
-                "B", itertools.repeat(False, len(self._start_vertices))
-            )
+            to_leave_markers = array.array("B", itertools.repeat(False, len(to_visit)))
             to_leave_markers_pop = to_leave_markers.pop
             to_leave_markers_append = to_leave_markers.append
         else:
             # the following is needed to replace the real depth with at least
-            # to information whether it is 0 oder higher.
+            # the information whether it is 0 oder higher.
+            # This does not work if we have no start vertices, but in this case,
+            # we can just stop working because we will not report results anyway
+            if len(to_visit) == 0:
+                return
             top_start_vertex: Optional[T_vertex] = to_visit[-1]
 
         # ----- Typing preparation of inner loop (for details see BFS) -----
 
         edge_or_vertex: Any  # "Hole" in typing, but types "around" make it safe
         neighbor: T_vertex  # Re-establish type "after" the "hole"
         data_of_edge: T_labels  # Re-establish type "after" the "hole"
 
         # ----- Inner loop -----
 
         while to_visit:
             vertex = to_visit_pop()  # Enter first added vertex first
             if compute_depth:
                 depth += 1
+                # (noinspection necessary due to bug PY-9479, also below...)
+                # noinspection PyUnboundLocalVariable
                 while to_leave_markers_pop():
                     depth -= 1  # Got marker "leave a vertex", update depth
                 # Update external view on depth
                 self.depth = depth
                 # Store marker True: when reached, we are leaving a vertex
+                # noinspection PyUnboundLocalVariable
                 to_leave_markers_append(True)
             else:
                 # if vertex is top_start_vertex:
+                # noinspection PyUnboundLocalVariable
                 if vertex is top_start_vertex:  # "is" is used on purpose
                     depth = 0  # is start vertex
                     if to_visit:
                         top_start_vertex = to_visit[-1]  # new top start vertex
                     else:
                         top_start_vertex = None
                 else:
@@ -1317,15 +1132,15 @@
 
             if calculation_limit and not (calculation_limit := calculation_limit - 1):
                 raise RuntimeError("Number of visited vertices reached limit")
 
             for edge_or_vertex in next_edge_or_vertex(vertex, self):
                 neighbor = edge_or_vertex[0] if edges_with_data else edge_or_vertex
 
-                if check_visited_when_seen or paths:
+                if check_visited_when_seen or build_paths:
                     n_id: T_vertex_id = (
                         maybe_vertex_to_id(neighbor)  # type: ignore[assignment]
                         if maybe_vertex_to_id
                         else neighbor
                     )
                     # Ignore neighbor if already visited/expanded, i.e., not put it
                     # onto the stack to_visit.
@@ -1358,32 +1173,26 @@
                     elif check_visited_when_seen:
                         # Same as above, but with booleans in byte sequence
                         try:
                             if visited_sequence[n_id]:
                                 continue
                         except IndexError:
                             pass
-                    if paths:
+                    if build_paths:
                         # Store the predecessor (vertex) of the neighbor
                         try:
-                            # noinspection PyUnboundLocalVariable
                             predecessors_sequence[n_id] = vertex
                         except IndexError:
-                            # noinspection PyUnboundLocalVariable
-                            assert predecessors_wrapper is not None  # safe
-                            # noinspection PyUnboundLocalVariable
                             predecessors_wrapper.extend_and_set(n_id, vertex)
                         # Store the labels of the edge to the neighbor
-                        if attributes_exists:
+                        if labeled_edges:
                             data_of_edge = edge_or_vertex[-1]
                             try:
-                                # noinspection PyUnboundLocalVariable
                                 attributes_sequence[n_id] = data_of_edge
                             except IndexError:
-                                # noinspection PyUnboundLocalVariable
                                 attributes_wrapper.extend_and_set(n_id, data_of_edge)
 
                 # Needs to be visited, in stack order
                 to_visit_append(neighbor)
 
                 if compute_depth:
                     # Store marker False: when reached, we are entering a vertex
@@ -1447,28 +1256,30 @@
 
     :param next_vertices: See `NextVertices` function. If None, provide next_edges
      or next_labeled_edges.
 
     :param next_edges: See `NextEdges` function. Only allowed if next_vertices equals
      None. If both are None, provide next_labeled_edges.
 
-    :param next_labeled_edges: See `NextEdges` function. Only allowed if next_vertices
-     and next_edges equal None. If given, paths will record the given labels.
+    :param next_labeled_edges: See `NextLabeledEdges` function. Only allowed if
+      next_vertices and next_edges equal None. If given, paths will record the given
+      labels.
 
     :param is_tree: bool: If it is certain, that during each traversal run, each vertex
         can be reached only once, is_tree can be set to True. This improves
         performance, but attribute *visited* of the traversal will not be updated
         during and after the traversal.
 
     **Algorithm:** Variant of Depth First Search ("DFS"), non-recursive, based on stack,
     vertices are reported when they are seen (neighbors read from the graph).
 
-    **Properties:** Like Depth First Search, but first reports all neighbors of
-    the current vertex and then goes deeper.
-    Vertices are regarded as visited when they have been seen.
+    **Properties:** Like `nographs.TraversalDepthFirst`, but first reports all
+    neighbors of the current vertex and then goes deeper.
+    A vertex is regarded as visited when it has been reported or if it is a start
+    vertex.
 
     **Input:** Directed graph. One or more start vertices. Vertices must be
     hashable, or hashable id can be provided. Unlabeled or labeled edges. Optional
     calculation limit.
 
     **Search state:** When a vertex is
     *expanded* (traversal calls next_vertices, next_edges or next_labeled_edges)
@@ -1500,28 +1311,28 @@
                 TraversalNeighborsThenDepthFlex[T_vertex, T_vertex_id, T_labels],
                 T_labels,
             ]
         ] = None,
         is_tree: bool = False,
     ) -> None:
         (
-            self.next_edge_or_vertex,
-            self.edges_with_data,
-            self.labeled_edges,
+            self._next_edge_or_vertex,
+            edges_with_data,
+            labeled_edges,
         ) = _create_unified_next(next_vertices, next_edges, next_labeled_edges)
-        super().__init__(
-            self.edges_with_data, self.labeled_edges, is_tree, vertex_to_id, gear
-        )
+        super().__init__(edges_with_data, labeled_edges, is_tree, vertex_to_id, gear)
         self.depth: int = -1  # value not used
         """ If depth computation has been demanded:
         At this *search depth*, the reported (resp. the expanded) vertex has been
         found. It equals the length (number of edges) of the created path to the
         vertex, if path creation is demanded.
         Note: The search depth does not need to be the depth of the vertex
         (see `TraversalBreadthFirstFlex`).
+        When a traversal has been started, but no vertex has been reported or expanded
+        so far, the depth is 0 (depth of the start vertices).
         """
         self._compute_depth = False  # value not used
 
     def start_from(
         self,
         start_vertex: Optional[T_vertex] = None,
         *,
@@ -1535,88 +1346,78 @@
         self._start_with_or_without_labels_from(
             start_vertex,
             start_vertices,
             build_paths,
             calculation_limit,
             already_visited,
         )
+        self.depth = 0
         self._compute_depth = compute_depth
         return self
 
     def _traverse(self) -> Iterator[T_vertex]:
         # ----- Prepare efficient environment for inner loop -----
         # Copy Traversal attributes into method scope (faster access)
         labeled_edges = self._labeled_edges
         compute_depth = self._compute_depth
         is_tree = self._is_tree
         maybe_vertex_to_id = (
             None if self._vertex_to_id == vertex_as_id else self._vertex_to_id
         )  # Case vertex_as_id: not apply; T_vertex_id > T_vertex
+        build_paths = self._build_paths
         calculation_limit = self._calculation_limit
-        paths = self.paths
         predecessors = self._predecessors
         attributes = self._attributes
 
         # Prepare limit check done by zero check
         if calculation_limit is not None:
             calculation_limit += 1  # Allows for limit check by zero check
 
         # Copy TraversalWithoutWeights attributes into method scope
         edges_with_data = self._edges_with_data
-        next_edge_or_vertex = self.next_edge_or_vertex
+        next_edge_or_vertex = self._next_edge_or_vertex
         visited = self.visited
-        assert visited is not None
-
-        # Create booleans (avoid checks with "is", make decisions clear)
-        attributes_exists = attributes is not None
 
         # Get references of used gear objects and methods (avoid attribute resolution)
         visited_add = visited.add
         (
             visited_uses_sequence,
             visited_sequence,
             visited_wrapper,
             visited_uses_bits,
             visited_index_and_bit_method,
         ) = access_to_vertex_set(visited)
-        if paths:  # has no __len__, so this checks for non-None
-            assert predecessors is not None
-            (
-                _,
-                predecessors_sequence,
-                predecessors_wrapper,
-            ) = access_to_vertex_mapping_expect_none(predecessors)
-        if attributes is not None:
-            assert labeled_edges
-            (
-                _,
-                attributes_sequence,
-                attributes_wrapper,
-            ) = access_to_vertex_mapping_expect_none(attributes)
+        (
+            _,
+            predecessors_sequence,
+            predecessors_wrapper,
+        ) = access_to_vertex_mapping_expect_none(predecessors)
+        (
+            _,
+            attributes_sequence,
+            attributes_wrapper,
+        ) = access_to_vertex_mapping_expect_none(attributes)
 
         # ----- Initialize method specific bookkeeping -----
 
+        depth = -1  # The inner loop starts with incrementing, so, we pre-decrement
+        if not compute_depth:
+            self.depth = depth  # In this case, we leave the -1 the whole time
         prev_traversal = copy.copy(self)  # copy of self, for keeping previous depth
-        depth = -1
-
-        if len(self._start_vertices) == 0:
-            return
 
         # vertices to expand
         to_expand = self._gear.sequence_of_vertices(self._start_vertices)
         to_expand_append = to_expand.append
         to_expand_pop = to_expand.pop
 
         if compute_depth:
             # Sequence of flag bytes (store in a Q array) marking the vertices to leave
             # by 1 and the vertices to enter (these are in to_expand) by 0.
             # Initially, store a zero flag for each start vertex.
-            to_leave_marker = array.array(
-                "B", itertools.repeat(False, len(self._start_vertices))
-            )
+            to_leave_marker = array.array("B", itertools.repeat(False, len(to_expand)))
             to_leave_marker_pop = to_leave_marker.pop
             to_leave_marker_append = to_leave_marker.append
 
         # ----- Typing preparation of inner loop (for details see BFS) -----
 
         edge_or_vertex: Any  # "Hole" in typing, but types "around" make it safe
         neighbor: T_vertex  # Re-establish type "after" the "hole"
@@ -1624,29 +1425,31 @@
 
         # ----- Inner loop -----
 
         while to_expand:
             vertex = to_expand_pop()  # Enter first added vertex first
             if compute_depth:
                 depth += 1
+                # noinspection PyUnboundLocalVariable
                 while to_leave_marker_pop():
                     depth -= 1  # Got marker "leave a vertex", update depth
                 # Update external view on depth
                 prev_traversal.depth = depth
                 self.depth = depth + 1
                 # Store marker True: when reached, we are leaving a vertex
+                # noinspection PyUnboundLocalVariable
                 to_leave_marker_append(True)
 
             if calculation_limit and not (calculation_limit := calculation_limit - 1):
                 raise RuntimeError("Number of visited vertices reached limit")
 
             for edge_or_vertex in next_edge_or_vertex(vertex, prev_traversal):
                 neighbor = edge_or_vertex[0] if edges_with_data else edge_or_vertex
 
-                if not is_tree or paths:
+                if not is_tree or build_paths:
                     n_id: T_vertex_id = (
                         maybe_vertex_to_id(neighbor)  # type: ignore[assignment]
                         if maybe_vertex_to_id
                         else neighbor
                     )
                     # Ignore neighbor if already visited/expanded, i.e., not put it
                     # onto the stack to_expand.
@@ -1671,32 +1474,26 @@
                         # Same as above, but with booleans in byte sequence
                         try:
                             if visited_sequence[n_id]:
                                 continue
                             visited_sequence[n_id] = True
                         except IndexError:
                             visited_wrapper.extend_and_set(n_id, True)
-                    if paths:
+                    if build_paths:
                         # Store the predecessor (vertex) of the neighbor
                         try:
-                            # noinspection PyUnboundLocalVariable
                             predecessors_sequence[n_id] = vertex
                         except IndexError:
-                            # noinspection PyUnboundLocalVariable
-                            assert predecessors_wrapper is not None  # safe
-                            # noinspection PyUnboundLocalVariable
                             predecessors_wrapper.extend_and_set(n_id, vertex)
                         # Store the labels of the edge to the neighbor
-                        if attributes_exists:
+                        if labeled_edges:
                             data_of_edge = edge_or_vertex[-1]
                             try:
-                                # noinspection PyUnboundLocalVariable
                                 attributes_sequence[n_id] = data_of_edge
                             except IndexError:
-                                # noinspection PyUnboundLocalVariable
                                 attributes_wrapper.extend_and_set(n_id, data_of_edge)
 
                 yield neighbor
 
                 # Needs to be expanded, in stack order
                 to_expand_append(neighbor)
 
@@ -1765,31 +1562,37 @@
 
     :param next_vertices: See `NextVertices` function. If None, provide next_edges
      or next_labeled_edges.
 
     :param next_edges: See `NextEdges` function. Only allowed if next_vertex equals
        None. If both are None, provide next_labeled_edges.
 
-    :param next_labeled_edges: See `NextEdges` function. Only allowed if next_vertices
-     and next_edges equal None. If given, paths will record the given labels.
+    :param next_labeled_edges: See `NextLabeledEdges` function. Only allowed if
+      next_vertices and next_edges equal None. If given, paths will record the given
+      labels.
 
     :param is_tree: bool: If it is certain, that during each traversal run, each vertex
        can be reached only once, is_tree can be set to True. This improves performance,
        but attribute *visited* of the traversal will not be updated during and after
        the traversal.
 
     **Algorithm:** Topological Search, non-recursive, based on stack, vertices are
     reported when they "are left" for backtracking.
 
     **Properties:** Vertices are reported in topological ordering, i.e. a linear
     ordering of the vertices such that for every directed edge *uv* from vertex *u* to
     vertex *v* ("*u* depends on *v*"), *v* comes before *u* in the ordering. If the
     graph contains a cycle that can be reached within the sorting process, a
     RuntimeError exception is raised and a cyclic path from a start vertex is provided.
-    A vertex is regarded as visited when the traversal started expanding it.
+
+    Vertices are expanded following the strategy `nographs.TraversalDepthFirst`.
+
+    For topological search, a vertex is regarded as visited when it has been expanded
+    (see search state) or if it is a start vertex. Note this difference in comparison
+    to other traversals that mark a vertex as visited when it is reported.
 
     **Input:** Directed graph. One or more start vertices. Vertices must be
     hashable, or hashable id can be provided. Unlabeled or labeled edges. Optional
     calculation limit.
 
     **Search state:** When a vertex is
     *expanded* (traversal calls next_vertices, next_edges or next_labeled_edges)
@@ -1819,28 +1622,28 @@
                 TraversalTopologicalSortFlex[T_vertex, T_vertex_id, T_labels],
                 T_labels,
             ]
         ] = None,
         is_tree: bool = False,
     ) -> None:
         (
-            self.next_edge_or_vertex,
-            self.edges_with_data,
-            self.labeled_edges,
+            self._next_edge_or_vertex,
+            edges_with_data,
+            labeled_edges,
         ) = _create_unified_next(next_vertices, next_edges, next_labeled_edges)
-        super().__init__(
-            self.edges_with_data, self.labeled_edges, is_tree, vertex_to_id, gear
-        )
+        super().__init__(edges_with_data, labeled_edges, is_tree, vertex_to_id, gear)
         # the following values are not used, and initialized during traversal
         self.depth: int = -1
         """  At this *search depth*, the reported (resp. the expanded) vertex has been
         found. It equals the length (number of edges) of the created path to the
         vertex, if path creation is demanded.
         Note: The search depth does not need to be the depth of the vertex
         (see `TraversalBreadthFirstFlex`).
+        When a traversal has been started, but no vertex has been reported or expanded
+        so far, the depth is 0 (depth of the start vertices).
         """
         self.cycle_from_start: list[T_vertex] = []
         """ If the graph contains a cycle that can be reached within the sorting
         process, a RuntimeError exception is raised, and the traversal provides
         a cyclic path from a start vertex in attribute cycle_from_start."""
 
     def start_from(
@@ -1854,15 +1657,15 @@
     ) -> TraversalTopologicalSortFlex[T_vertex, T_vertex_id, T_labels]:
         """
         Start the traversal at a vertex or a set of vertices and set parameters.
 
         :param start_vertex: The vertex the search should start at. If None, provide
             start_vertices.
 
-        :param start_vertices: The vertices (iterator) the search should start at. Only
+        :param start_vertices: The vertices the search should start at. Only
             allowed if start_vertex equals None.
 
         :param build_paths: If true, build paths from some start vertex to each visited
             vertex.
 
         :param calculation_limit: If provided, maximal number of vertices to process
             (read in) from your graph. If it is exceeded, a RuntimeError will be raised.
@@ -1889,65 +1692,58 @@
         self._start_with_or_without_labels_from(
             start_vertex,
             start_vertices,
             build_paths,
             calculation_limit,
             already_visited,
         )
+        self.depth = 0
         return self
 
     def _traverse(self) -> Iterator[T_vertex]:
         # ----- Prepare efficient environment for inner loop -----
         # Copy Traversal attributes into method scope (faster access)
         labeled_edges = self._labeled_edges
         is_tree = self._is_tree
         maybe_vertex_to_id = (
             None if self._vertex_to_id == vertex_as_id else self._vertex_to_id
         )  # Case vertex_as_id: not apply; T_vertex_id > T_vertex
+        build_paths = self._build_paths
         calculation_limit = self._calculation_limit
-        paths = self.paths
         predecessors = self._predecessors
         attributes = self._attributes
 
         # Prepare limit check done by zero check
         if calculation_limit is not None:
             calculation_limit += 1  # allows for limit check by zero check
 
         # Copy _TraversalWithoutWeights attributes into method scope
         edges_with_data = self._edges_with_data
-        next_edge_or_vertex = self.next_edge_or_vertex
+        next_edge_or_vertex = self._next_edge_or_vertex
         visited = self.visited
-        assert visited is not None
-
-        # Create booleans (avoid checks with "is")
-        attributes_exists = attributes is not None
 
         # Get references of used gear objects and methods (avoid attribute resolution)
         visited_add = visited.add
         (
             visited_uses_sequence,
             visited_sequence,
             visited_wrapper,
             visited_uses_bits,
             visited_index_and_bit_method,
         ) = access_to_vertex_set(visited)
-        if paths:  # has no __len__, so this checks for non-None
-            assert predecessors is not None
-            (
-                predecessors_uses_sequence,
-                predecessors_sequence,
-                predecessors_wrapper,
-            ) = access_to_vertex_mapping_expect_none(predecessors)
-        if attributes is not None:
-            assert labeled_edges
-            (
-                attributes_uses_sequence,
-                attributes_sequence,
-                attributes_wrapper,
-            ) = access_to_vertex_mapping_expect_none(attributes)
+        (
+            predecessors_uses_sequence,
+            predecessors_sequence,
+            predecessors_wrapper,
+        ) = access_to_vertex_mapping_expect_none(predecessors)
+        (
+            attributes_uses_sequence,
+            attributes_sequence,
+            attributes_wrapper,
+        ) = access_to_vertex_mapping_expect_none(attributes)
 
         # ----- Typing preparation of inner loop (for details see DFS) -----
 
         edge_or_vertex: Any  # "Hole" in typing, but types "around" make it safe
         neighbor: T_vertex  # Re-establish type "after" the "hole"
         data_of_edge: T_labels  # Re-establish type "after" the "hole"
 
@@ -1959,25 +1755,24 @@
             # already seen vertices.
             # We just use a stack for vertices we have to enter or leave, and store
             # None on top of the vertices we need to enter in order to differentiate
             # the two cases.
 
             # ----- Initialize specific bookkeeping -----
 
-            self.depth = 0
             self.cycle_from_start = []
             # Sequence used as stack of vertices that we need to enter & expand (if
             # it is not on the trace, see below) or leave & report (otherwise)
             to_expand_or_leave = self._gear.sequence_of_vertices(self._start_vertices)
 
             # Sequence of flag bytes (store in a Q array) marking the vertices to leave
             # by 1 and the vertices to enter by 0.
             # Initially, store a zero flag for each start vertex.
             to_leave_markers = array.array(
-                "B", itertools.repeat(False, len(self._start_vertices))
+                "B", itertools.repeat(False, len(to_expand_or_leave))
             )
 
             # Get method references of specific bookkeeping (avoid attribute resolution)
             to_expand_or_leave_append = to_expand_or_leave.append
             to_expand_or_leave_pop = to_expand_or_leave.pop
             to_leave_markers_pop = to_leave_markers.pop
             to_leave_markers_append = to_leave_markers.append
@@ -2010,41 +1805,33 @@
 
                     n_id: T_vertex_id = (
                         maybe_vertex_to_id(neighbor)  # type: ignore[assignment]
                         if maybe_vertex_to_id
                         else neighbor
                     )
 
-                    if paths:
+                    if build_paths:
                         # We have to store the predecessor here, because at time of
                         # visit, it is already lost. And we cannot yield here,
                         # because only the first of the neighbors will indeed be
                         # visited next.
-                        # But since the visiting order is defined by a stack we know
-                        # that for each vertex, the predecessor stored last is the
-                        # edge visited first, and after that no other predecessor can
-                        # be stored for that vertex.
+                        # But since we are in a tree, no other predecessor can
+                        # be stored for that vertex later on.
 
                         # Store the predecessor (vertex) of the neighbor
                         try:
-                            # noinspection PyUnboundLocalVariable
                             predecessors_sequence[n_id] = vertex
                         except IndexError:
-                            # noinspection PyUnboundLocalVariable
-                            assert predecessors_wrapper is not None  # safe
-                            # noinspection PyUnboundLocalVariable
                             predecessors_wrapper.extend_and_set(n_id, vertex)
                         # Store the labels of the edge to the neighbor
-                        if attributes_exists:
+                        if labeled_edges:
                             data_of_edge = edge_or_vertex[-1]
                             try:
-                                # noinspection PyUnboundLocalVariable
                                 attributes_sequence[n_id] = data_of_edge
                             except IndexError:
-                                # noinspection PyUnboundLocalVariable
                                 attributes_wrapper.extend_and_set(n_id, data_of_edge)
 
                     # Put vertex on the stack
                     to_expand_or_leave_append(neighbor)
                     # Remember that we have to expand it
                     to_leave_markers_append(False)
 
@@ -2056,15 +1843,14 @@
             # For detecting cycles, we store the vertices, that are on the current
             # path, in a set. We use a stack for storing the vertices we have to
             # enter or leave (when such a vertex is in the path set, we need to leave
             # the vertex).
 
             # ----- Initialize specific bookkeeping -----
 
-            self.depth = 0
             self.cycle_from_start = []
 
             # Sequence used as stack of vertices that we need to enter & expand (if
             # it is not on the trace, see below) or leave & report (otherwise)
             to_enter_or_leave = self._gear.sequence_of_vertices(self._start_vertices)
 
             # Set of vertices along the current path
@@ -2250,15 +2036,15 @@
                                 except IndexError:
                                     # In order to become visited, a vertex needs to
                                     # get into the trace set and then be discarded
                                     # from it. Thus, if a vertex is visited, the
                                     # trace set sequence already has the necessary
                                     # length to store it. So, no IndexError can happen
                                     # here.
-                                    raise RuntimeError(
+                                    raise AssertionError(
                                         "Internal error in TS"
                                     )  # pragma: no cover
                                 continue
                         except IndexError:
                             pass
                     else:
                         # Same as above, but with booleans in byte sequence
@@ -2270,46 +2056,38 @@
                                             neighbor,
                                             to_enter_or_leave,
                                             trace_set,
                                             maybe_vertex_to_id,
                                         )
                                 except IndexError:
                                     # See above case for the reason for the pragma
-                                    raise RuntimeError(
+                                    raise AssertionError(
                                         "Internal error in TS"
                                     )  # pragma: no cover
                                 continue
                         except IndexError:
                             pass
 
-                    if paths:
+                    if build_paths:
                         # We have to store the predecessor here, because at time of
                         # visit, it is already lost. And we cannot yield here,
                         # because TopologicalSorted reports not until leaving vertices.
                         # But since the visiting order is defined by a stack we know
                         # that for each vertex, the predecessor stored last is the
                         # edge visited first, and after that no other predecessor can
                         # be stored for that vertex.
                         try:
-                            # noinspection PyUnboundLocalVariable
                             predecessors_sequence[n_id2] = vertex
                         except IndexError:
-                            # noinspection PyUnboundLocalVariable
-                            assert predecessors_wrapper is not None  # safe
-                            # noinspection PyUnboundLocalVariable
                             predecessors_wrapper.extend_and_set(n_id2, vertex)
-                        if attributes_exists:
+                        if labeled_edges:
                             data_of_edge = edge_or_vertex[-1]
                             try:
-                                # noinspection PyUnboundLocalVariable
                                 attributes_sequence[n_id2] = data_of_edge
                             except IndexError:
-                                # noinspection PyUnboundLocalVariable
-                                assert attributes_wrapper is not None  # safe
-                                # noinspection PyUnboundLocalVariable
                                 attributes_wrapper.extend_and_set(n_id2, data_of_edge)
 
                     # Needs to be visited, in stack order
                     to_visit_append(neighbor)
 
                 # Update depth. The following vertices are one level deeper.
                 self.depth += 1
@@ -2409,29 +2187,29 @@
     | Bases: Generic[`T_vertex`, `T_vertex_id`, `T_weight`, `T_labels`],
     | `Traversal` [`T_vertex`, `T_vertex_id`, `T_labels`]
 
     :param vertex_to_id: See `VertexToID` function.
 
     :param gear: See `gears API <gears_api>` and class `Gear`.
 
-    :param next_edges: See `NextEdges` function. If None, provide next_labeled_edges.
+    :param next_edges: See `NextWeightedEdges` function. If None, provide
+      next_labeled_edges.
 
-    :param next_labeled_edges: See `NextEdges` function. Only allowed if next_edges
-      equals None. If given, paths will record the given labels.
+    :param next_labeled_edges: See `NextWeightedLabeledEdges` function. Only allowed
+      if next_edges equals None. If given, paths will record the given labels.
 
     :param is_tree: bool: If it is certain, that during each traversal run, each vertex
-       can be reached only once, is_tree can be set to True. This improves performance,
-       but attribute *distances* of the traversal will not be updated during and after
-       the traversal.
+      can be reached only once, is_tree can be set to True. This improves performance,
+      but attribute *distances* of the traversal will not be updated during and after
+      the traversal.
 
     **Algorithm:** Shortest paths algorithm of Dijkstra, non-recursive, based on heap.
 
-    **Properties:** Vertices are visited and reported ordered by increasing distance
-    (minimally necessary sum of edge weights) from a start vertex. Each vertex is
-    visited only once.
+    **Properties:** Vertices are reported (and expanded) ordered by increasing distance
+    (minimally necessary sum of edge weights) from a start vertex.
 
     **Input:** Weighted directed graph. One or more start vertices. Vertices must be
     hashable, or hashable id can be provided. Weights need to be non-negative.
     Optional calculation limit.
 
     **Search state:** When a vertex is *expanded* (traversal calls next_edges or
     next_labeled_edges) or *reported* (an iterator of the traversal returns it),
@@ -2457,50 +2235,53 @@
                 TraversalShortestPathsFlex[T_vertex, T_vertex_id, T_weight, T_labels],
                 T_weight,
                 T_labels,
             ]
         ] = None,
         is_tree: bool = False,
     ) -> None:
-        self.next_edges, self.labeled_edges = _create_unified_next_weighted(
+        self._next_edges, labeled_edges = _create_unified_next_weighted(
             next_edges, next_labeled_edges
         )
-        super().__init__(self.labeled_edges, is_tree, vertex_to_id, gear)
+        super().__init__(labeled_edges, is_tree, vertex_to_id, gear)
 
         self._known_distances: Optional[
             VertexIdToDistanceMapping[T_vertex_id, T_weight]
         ] = None
         self._keep_distances = False
 
-        self.distances: Optional[
-            VertexIdToDistanceMapping[T_vertex_id, T_weight]
-        ] = None
-        """ Current candidates of distance values
+        self.distances: VertexIdToDistanceMapping[
+            T_vertex_id, T_weight
+        ] = NoDistancesMapping[T_vertex_id, T_weight]()
+        """ Provisional or final distance values of some vertices
         (distance from a start vertex). Without option *keep_distances*,
         the value for a vertex is removed once the vertex has been reported. With
         option *keep_distances*, values are never removed, and that means: During a
         traversal, the distance values for already reported vertices can be found in
         the collection. After an exhaustive search, the collection contains exactly
         and only the distances of all vertices that are reachable from the start
         vertices and of the start vertices themselves.
         """
 
-        # The following two values are not used by NoGraphs. They are only set
+        # The following three values are not used by NoGraphs. They are only set
         # to have some initialization.
         self.distance: T_weight = self._gear.infinity()
         """ The length of the shortest path (sum of edge weights) from a
         start vertex to the visited vertex
         """
         self.depth: int = -1
         """  At this *search depth*, the reported (resp. the expanded) vertex has been
         found. It equals the length (number of edges) of the created path to the
         vertex, if path creation is demanded.
         Note: The search depth does not need to be the depth of the vertex
         (see `TraversalBreadthFirstFlex`).
+        When a traversal has been started, but no vertex has been reported or expanded
+        so far, the depth is 0 (depth of the start vertices).
         """
+        self._start_vertices_and_ids = tuple[tuple[T_vertex, T_vertex_id]]()
 
     def start_from(
         self,
         start_vertex: Optional[T_vertex] = None,
         *,
         start_vertices: Optional[Iterable[T_vertex]] = None,
         build_paths: bool = False,
@@ -2512,19 +2293,19 @@
     ) -> TraversalShortestPathsFlex[T_vertex, T_vertex_id, T_weight, T_labels]:
         """
         Start the traversal at a vertex or a set of vertices and set parameters.
 
         :param start_vertex: The vertex the search should start at. If None, provide
             start_vertices.
 
-        :param start_vertices: The set of vertices (iterator) the search should start
+        :param start_vertices: The set of vertices the search should start
             at. Only allowed if start_vertex equals None.
 
-        :param build_paths: If true, build paths from start vertices for each visited
-            vertex.
+        :param build_paths: If true, build paths from start vertices for each reported
+            vertex, and an empty path for each start vertex.
 
         :param calculation_limit: If provided, maximal number of vertices to process
             (read in) from your graph. If it is exceeded, a RuntimeError will be raised.
 
         :param keep_distances: If True, the found distances of vertices are
             collected in traversal attribute distances, and not deleted after
             having reported the vertex. See attribute distances.
@@ -2545,112 +2326,107 @@
         """
 
         if not isinstance(type(self), type(Traversal)):
             raise RuntimeError(
                 "Method start_from can only be called on a Traversal object."
             )
 
+        # ----- Initialize method specific public bookkeeping -----
         self._start_from(
             start_vertex,
             start_vertices,
             build_paths,
             calculation_limit,
             self._gear,
         )
         self._keep_distances = keep_distances
         self._known_distances = known_distances
-        super()._start()
+
+        # Explicitly list start vertices and their id. Needed several times.
+        self._start_vertices_and_ids = tuple(
+            iter_start_vertices_and_ids(self._start_vertices, self._vertex_to_id)
+        )
+
+        # At start, most of the distances from a vertex to a start vertex are not
+        # known. If accessed for comparison for possibly better distances, infinity
+        # is used, if no other value is given. Each start vertex has distance 0
+        # from a start vertex (itself), if not defined otherwise.
+        zero = self._gear.zero()
+        self.distances = define_distances(
+            self._gear,
+            self._known_distances,
+            ((vertex_id, zero) for vertex, vertex_id in self._start_vertices_and_ids),
+            self._is_tree,
+        )
 
         # The following two values are not used by NoGraphs. They are only set
-        # to have some defined values before the traversal starts.
+        # to have some defined values before the traversal iterator sets them.
         self.distance = self._gear.infinity()
-        self.depth = -1
+        self.depth = 0
+
+        super()._start()
         return self
 
     def _traverse(self) -> Iterator[T_vertex]:
         # ----- Prepare efficient environment for inner loop -----
         # Copy Gear attributes into method scope (faster access)
         infinity = self._gear.infinity()
 
         # Copy Traversal attributes into method scope (faster access)
+        labeled_edges = self._labeled_edges
         is_tree = self._is_tree
         maybe_vertex_to_id = (
             None if self._vertex_to_id == vertex_as_id else self._vertex_to_id
         )  # Case vertex_as_id: not apply; T_vertex_id > T_vertex
+        build_paths = self._build_paths
         calculation_limit = self._calculation_limit
-        paths = self.paths
         predecessors = self._predecessors
         attributes = self._attributes
 
         # Prepare limit check done by zero check
         if calculation_limit is not None:
             calculation_limit += 1
 
         # Copy traversal specific attributes into method scope
-        next_edges = self.next_edges
+        next_edges = self._next_edges
         keep_distances = self._keep_distances
 
-        # Create booleans (avoid checks with "is"), local check for consistency
-        if attributes is None:
-            attributes_exists = False
-        else:
-            attributes_exists = True
-            assert self.labeled_edges
-
         # Get references of used gear objects and methods (avoid attribute resolution)
-        if paths:  # has no __len__, so this checks for non-None
-            assert predecessors is not None
-            (
-                _,
-                predecessors_sequence,
-                predecessors_wrapper,
-            ) = access_to_vertex_mapping_expect_none(predecessors)
-        if attributes is not None:
-            (
-                _,
-                attributes_sequence,
-                attributes_wrapper,
-            ) = access_to_vertex_mapping_expect_none(attributes)
+        (
+            _,
+            predecessors_sequence,
+            predecessors_wrapper,
+        ) = access_to_vertex_mapping_expect_none(predecessors)
+        (
+            _,
+            attributes_sequence,
+            attributes_wrapper,
+        ) = access_to_vertex_mapping_expect_none(attributes)
+        zero = self._gear.zero()
 
-        # ----- Initialize method specific bookkeeping -----
+        # ----- Initialize method specific private bookkeeping -----
 
         # Unique number, that prevents heapq from sorting by vertices in case of a
         # tie in the sort field, because vertices do not need to be pairwise
         # comparable. The integers from -5 to 256 are used first, because they are
         # internalized (pre-calculated, and thus fastest). We count downwards like we
         # do in A* search. There, it is preferable, because a LIFO behavior makes A*
         # often faster. Here, we do it simply to do it the same way.
         unique_no = itertools.count(256, -1)
 
-        # Explicitly list start vertices and their id. Needed several times.
-        start_vertices_and_ids = tuple(
-            _iter_start_vertices_and_ids(self._start_vertices, self._vertex_to_id)
-        )
-
-        # At start, most of the distances from a vertex to a start vertex are not
-        # known. If accessed for comparison for possibly better distances, infinity
-        # is used, if no other value is given. Each start vertex has distance 0
-        # from a start vertex (itself), if not defined otherwise.
-        zero = self._gear.zero()
-        distances = _define_distances(
-            self._gear,
-            self._known_distances,
-            ((vertex_id, zero) for vertex, vertex_id in start_vertices_and_ids),
-            is_tree,
-        )
-        self.distances = distances
-
         # Get references of used gear objects and methods (avoid attribute resolution)
-        _, distances_sequence, distances_wrapper = access_to_vertex_mapping(distances)
+        _, distances_sequence, distances_wrapper = access_to_vertex_mapping(
+            self.distances
+        )
 
         # So far, the start vertices are to be visited. Each has an edge count of 0.
         # (No index exception possible at the following indexed access)
         to_visit = [  # used as collection.heapq of tuples, the lowest distance first
             (distances_sequence[vertex_id], next(unique_no), vertex, 0)
-            for vertex, vertex_id in start_vertices_and_ids
+            for vertex, vertex_id in self._start_vertices_and_ids
         ]
         heapify(to_visit)
 
         # ----- Inner loop -----
 
         while to_visit:
             # Visit path with the lowest distance first
@@ -2696,15 +2472,15 @@
                 if infinity <= n_path_weight:
                     self._gear.raise_distance_infinity_overflow_error(n_path_weight)
 
                 # If the found path to the neighbor is not shorter than the shortest
                 # such path found so far, we can safely ignore it. Otherwise, it is a
                 # new candidate for a shortest path to the neighbor, and we push it to
                 # the heap.
-                if paths or not is_tree:
+                if build_paths or not is_tree:
                     n_id: T_vertex_id = (
                         maybe_vertex_to_id(neighbor)  # type: ignore[assignment]
                         if maybe_vertex_to_id
                         else neighbor
                     )
 
                     if not is_tree:
@@ -2713,35 +2489,28 @@
                                 continue
                             distances_sequence[n_id] = n_path_weight
                         except IndexError:
                             distances_wrapper.extend_and_set(n_id, n_path_weight)
 
                     # If we are to generate a path, we have to do it here, since the
                     # edge we have to add to the path prefix is not stored on the heap
-                    if paths:
+                    if build_paths:
                         try:
-                            # noinspection PyUnboundLocalVariable
                             predecessors_sequence[n_id] = vertex
                         except IndexError:
-                            # noinspection PyUnboundLocalVariable
-                            assert predecessors_wrapper is not None  # safe
-                            # noinspection PyUnboundLocalVariable
                             predecessors_wrapper.extend_and_set(n_id, vertex)
-                        if attributes_exists:
-                            # attributes_exists -> self.labeled_edges (see assert above)
-                            # -> next_edges (a NextWeightedEdges) is a
-                            # NextWeightedLabeledEdges -> edge[-1] is a T_labels.
+                        if labeled_edges:
+                            # self._labeled_edges -> next_edges (a NextWeightedEdges)
+                            # is a NextWeightedLabeledEdges -> edge[-1] is a T_labels
                             data_of_edge: T_labels = edge[
                                 -1
                             ]  # type: ignore[assignment]
                             try:
-                                # noinspection PyUnboundLocalVariable
                                 attributes_sequence[n_id] = data_of_edge
                             except IndexError:
-                                # noinspection PyUnboundLocalVariable
                                 attributes_wrapper.extend_and_set(n_id, data_of_edge)
 
                 heappush(
                     to_visit,
                     (
                         n_path_weight,
                         next(unique_no),
@@ -2765,27 +2534,45 @@
             raise RuntimeError(
                 "Method go_for_distance_range can only be called "
                 + "on a Traversal object."
             )
 
         # In order to make the above check work, the following generator functionality
         # needs to be encapsulated in a local function
-        def my_generator():
+        def my_generator() -> Iterator[T_vertex]:
             for v in self._generator:
                 if self.distance >= start:
                     if self.distance < stop:
                         yield v
                     break
             for v in self._generator:
                 if self.distance >= stop:
                     break
                 yield v
 
         return my_generator()
 
+    def state_to_str(self, vertices: Optional[Iterable[T_vertex]] = None) -> str:
+        more = dict[str, Any]()
+        if vertices is not None:
+            if self._build_paths:
+                for vertex in vertices:
+                    more[f"paths[{vertex}]"] = self.paths[vertex]
+            if self._vertex_to_id is vertex_as_id:
+                for vertex in vertices:
+                    more[f"distances[{vertex}]"] = self.distances[
+                        self._vertex_to_id(vertex)
+                    ]
+            else:
+                for vertex in vertices:
+                    more[f"distances[vertex_to_id({vertex})]"] = self.distances[
+                        self._vertex_to_id(vertex)
+                    ]
+        return self._state_and_more_to_str(less=["paths", "distances"], more=more)
+
 
 class TraversalShortestPaths(
     Generic[T_vertex, T_weight, T_labels],
     TraversalShortestPathsFlex[T_vertex, T_vertex, Union[T_weight, float], T_labels],
 ):
     """
     Eases the use of `TraversalShortestPathsFlex` for typical cases.
@@ -2844,18 +2631,19 @@
     | Bases: Generic[`T_vertex`, `T_vertex_id`, `T_weight`, `T_labels`],
     | `Traversal` [`T_vertex`, `T_vertex_id`, `T_labels`]
 
     :param vertex_to_id: See `VertexToID` function.
 
     :param gear: See `gears API <gears_api>` and class `Gear`.
 
-    :param next_edges: See `NextEdges` function. If None, provide next_labeled_edges.
+    :param next_edges: See `NextWeightedEdges` function. If None, provide
+      next_labeled_edges.
 
-    :param next_labeled_edges: See `NextEdges` function. Only allowed if next_edges
-      equals None. If given, paths will record the given labels.
+    :param next_labeled_edges: See `NextWeightedLabeledEdges` function. Only allowed
+      if next_edges equals None. If given, paths will record the given labels.
 
     :param is_tree: bool: If it is certain, that during each traversal run, each vertex
        can be reached only once, is_tree can be set to True. This improves performance,
        but if *start_from* has been called with parameter *known_path_length_guesses*
        given, this collection will not be updated during the traversal.
 
     **Algorithm:** The search algorithm A*, non-recursive, based on heap.
@@ -2863,25 +2651,26 @@
     **Input:** Weighted directed graph. One or more start vertices. Vertices must be
     hashable, or hashable id can be provided. Weights need to be non-negative.
     A heuristic function that estimates the cost of the cheapest path from a given
     vertex to the goal (resp. to any of your goal vertices, if you have more than
     one), and never overestimates the actual needed costs ("admissible heuristic
     function"). Optionally, a calculation limit.
 
-    **Properties:** Vertices are visited and reported ordered by increasing path
-    length (sum of edge weights) of the shortest path from a start vertex to the
-    visited vertex that have been found so far (!).
-
-    When the goal is visited, the reported path is a shortest path from start to goal
-    and the reported length is the distance of the goal from start.
+    **Properties:** Vertices are reported and expanded ordered by increasing path
+    length (sum of edge weights) of the shortest paths from a start vertex to the
+    respective vertex that have been found so far.
+
+    When the goal is reported, the path stored for it in *paths* is a shortest
+    path from start to goal and the path_length of the search state is the distance
+    of the goal from start.
 
     In case the used heuristic function is *consistent* (i.e., following an edge from
     one vertex to another never reduces the estimated costs to get to the goal by
     more than the weight of the edge), further guarantees hold: Each vertex is only
-    visited once. And for each visited vertex, the yielded path length and edge count
+    visited once. And for each visited vertex, the respective path_length and depth
     (and optionally, the path) are the data of the shortest existing path from start
     (not only from the shortest path found so far).
 
     **Search state:** When a vertex is *expanded* (traversal calls next_edges or
     next_labeled_edges) or *reported* (an iterator of the traversal returns it),
     the traversal provides updated values for the attributes
     *path_length*, *depth*, *paths*.
@@ -2905,44 +2694,45 @@
                 TraversalAStarFlex[T_vertex, T_vertex_id, T_weight, T_labels],
                 T_weight,
                 T_labels,
             ]
         ] = None,
         is_tree: bool = False,
     ) -> None:
-        self.next_edges, self.labeled_edges = _create_unified_next_weighted(
+        self._next_edges, labeled_edges = _create_unified_next_weighted(
             next_edges, next_labeled_edges
         )
-        super().__init__(self.labeled_edges, is_tree, vertex_to_id, gear)
+        super().__init__(labeled_edges, is_tree, vertex_to_id, gear)
 
-        # The following two values are not used by NoGraphs. They are only set
+        # The following three values are not used by NoGraphs. They are only set
         # to have some initialization.
         self.path_length: T_weight = self._gear.infinity()
         """ Length (sum of edge weights) of the found path to the
         vertex (for the goal vertex: a shortest path)
         """
         self.depth: int = -1
         """  At this *search depth*, the reported (resp. the expanded) vertex has been
         found. It equals the length (number of edges) of the created path to the
         vertex, if path creation is demanded.
         Note: The search depth does not need to be the depth of the vertex
         (see `TraversalBreadthFirstFlex`).
         """
+        self._start_vertices_and_ids = tuple[tuple[T_vertex, T_vertex_id]]()
 
         self._heuristic: Optional[Callable[[T_vertex], Real]] = None
         self._known_distances: Optional[
             VertexIdToDistanceMapping[T_vertex_id, T_weight]
         ] = None
         self._known_path_length_guesses: Optional[
             VertexIdToDistanceMapping[T_vertex_id, T_weight]
         ] = None
 
-        self.distances: Optional[
-            VertexIdToDistanceMapping[T_vertex_id, T_weight]
-        ] = None
+        self.distances: VertexIdToDistanceMapping[
+            T_vertex_id, T_weight
+        ] = NoDistancesMapping[T_vertex_id, T_weight]()
         self._path_length_guesses: Optional[
             VertexIdToDistanceMapping[T_vertex_id, T_weight]
         ] = None
 
     def start_from(
         self,
         heuristic: Callable[[T_vertex], Real],
@@ -2964,19 +2754,19 @@
         :param heuristic: The admissible and consistent heuristic function that
             estimates the cost of the cheapest path from a given vertex to the goal
             (resp. one of the goals).
 
         :param start_vertex: The vertex the search should start at. Provide either
             start_vertex or start_vertices, but not both.
 
-        :param start_vertices: The set of vertices (iterator) the search should start
+        :param start_vertices: The set of vertices the search should start
             at. Provide either start_vertex or start_vertices, but not both.
 
-        :param build_paths: If true, build paths from start vertices for each visited
-            vertex.
+        :param build_paths: If true, build paths from start vertices for each reported
+            vertex, and an empty path for each start vertex.
 
         :param calculation_limit: If provided, maximal number of vertices to process
             (read in) from your graph. If it is exceeded, a RuntimeError will be raised.
 
         :param known_distances: If provided, this mapping is used instead of an internal
             one to keep the distances of vertices that have already been visited
             (resp. their hashable ids from vertex_to_id is used as key) from some
@@ -3005,122 +2795,118 @@
         self._start_from(
             start_vertex,
             start_vertices,
             build_paths,
             calculation_limit,
             self._gear,
         )
-        self.path_length = self._gear.infinity()  # Value never used
-        self.depth = -1  # Value never used
+
         self._heuristic = heuristic
         self._known_distances = known_distances
         self._known_path_length_guesses = known_path_length_guesses
+
+        # Explicitly list start vertices and their id. Needed several times.
+        self._start_vertices_and_ids = tuple(
+            iter_start_vertices_and_ids(self._start_vertices, self._vertex_to_id)
+        )
+
+        # At start, most of the distances from a vertex to a start vertex are not
+        # known. If accessed for comparison for possibly better distances, infinity
+        # is used, if no other value is given.
+        # Each start vertex has distance 0 from a start vertex (itself),
+        # and a path_length_guess of distance + heuristic(vertex), both if not
+        # defined otherwise.
+        zero = self._gear.zero()
+        self.distances = define_distances(
+            self._gear,
+            self._known_distances,
+            ((vertex_id, zero) for vertex, vertex_id in self._start_vertices_and_ids),
+            self._is_tree,
+        )
+
+        # The following two values are not used by NoGraphs. They are only set
+        # to have some defined values before the traversal iterator sets them.
+        self.path_length = self._gear.infinity()
+        self.depth = 0
+
         super()._start()
         return self
 
     def _traverse(self) -> Iterator[T_vertex]:
         # Copy Gear attributes into method scope (faster access)
         infinity = self._gear.infinity()
 
         # Copy Traversal attributes into method scope (faster access)
+        labeled_edges = self._labeled_edges
         is_tree = self._is_tree
         maybe_vertex_to_id = (
             None if self._vertex_to_id == vertex_as_id else self._vertex_to_id
         )  # Case vertex_as_id: not apply; T_vertex_id > T_vertex
+        build_paths = self._build_paths
         calculation_limit = self._calculation_limit
-        paths = self.paths
         predecessors = self._predecessors
         attributes = self._attributes
 
         # Prepare limit check done by zero check
         if calculation_limit is not None:
             calculation_limit += 1  # allows for limit check by zero check
 
         # Copy traversal specific attributes into method scope
-        next_edges = self.next_edges
+        next_edges = self._next_edges
         heuristic = self._heuristic
 
-        # Create booleans (avoid checks with "is"), local check for consistency
-        if attributes is None:
-            attributes_exists = False
-        else:
-            attributes_exists = True
-            assert self.labeled_edges
-
         # Get references of used gear objects and methods (avoid attribute resolution)
-        if paths:  # has no __len__, so this checks for non-None
-            assert predecessors is not None
-            (
-                _,
-                predecessors_sequence,
-                predecessors_wrapper,
-            ) = access_to_vertex_mapping_expect_none(predecessors)
-        if attributes is not None:
-            (
-                _,
-                attributes_sequence,
-                attributes_wrapper,
-            ) = access_to_vertex_mapping_expect_none(attributes)
+        (
+            _,
+            predecessors_sequence,
+            predecessors_wrapper,
+        ) = access_to_vertex_mapping_expect_none(predecessors)
+        (
+            _,
+            attributes_sequence,
+            attributes_wrapper,
+        ) = access_to_vertex_mapping_expect_none(attributes)
 
-        # ----- Initialize method specific bookkeeping -----
+        # ----- Initialize method specific private bookkeeping -----
 
         # Unique number, that prevents heapq from sorting by vertices in case of a
         # tie in the sort field, because vertices do not need to be pairwise
         # comparable. The numbers are generated in decreasing order to make the min
         # heap behave like a LIFO queue in case of ties. The integers from -5 to 256
         # are used first, because they are internalized (pre-calculated, and thus
         # fastest).
         unique_no = itertools.count(256, -1)
 
-        # Explicitly list start vertices and their id. Needed several times.
-        start_vertices_and_ids = tuple(
-            _iter_start_vertices_and_ids(self._start_vertices, self._vertex_to_id)
-        )
-
-        # At start, most of the distances from a vertex to a start vertex are not
-        # known. If accessed for comparison for possibly better distances, infinity
-        # is used, if no other value is given.
-        # Each start vertex has distance 0 from a start vertex (itself),
-        # and a path_length_guess of distance + heuristic(vertex), both if not
-        # defined otherwise.
-        zero = self._gear.zero()
-        distances = _define_distances(
-            self._gear,
-            self._known_distances,
-            ((vertex_id, zero) for vertex, vertex_id in start_vertices_and_ids),
-            is_tree,
-        )
-        self.distances = distances
-
         # Get references of used gear objects and methods (avoid attribute resolution)
-        _, distances_sequence, distances_wrapper = access_to_vertex_mapping(distances)
+        _, distances_sequence, distances_wrapper = access_to_vertex_mapping(
+            self.distances
+        )
 
         assert heuristic is not None  # set by __init__
-        path_length_guesses = _define_distances(
+        path_length_guesses = define_distances(
             self._gear,
             self._known_path_length_guesses,
             (
                 (vertex_id, distances_sequence[vertex_id] + heuristic(vertex))
-                for vertex, vertex_id in start_vertices_and_ids
+                for vertex, vertex_id in self._start_vertices_and_ids
             ),
             is_tree,
         )
-
         # Get references of used gear objects and methods (avoid attribute resolution)
         (
             _,
             path_length_guesses_sequence,
             path_length_guesses_wrapper,
         ) = access_to_vertex_mapping(path_length_guesses)
 
         # So far, the start vertices are to be visited. Each has an edge count of 0,
         # and its path length guess is the one computed above.
         to_visit = [  # used as collection.heapq of tuples, the lowest distance first
             (path_length_guesses_sequence[vertex_id], next(unique_no), vertex, 0)
-            for vertex, vertex_id in start_vertices_and_ids
+            for vertex, vertex_id in self._start_vertices_and_ids
         ]
         heapify(to_visit)
 
         # ----- Inner loop -----
 
         while to_visit:
             # Visit path with the lowest path_length_guess first
@@ -3185,51 +2971,64 @@
                 except IndexError:
                     # n_id not in distances_collection. To be regarded as value
                     # infinity, i.e., n_path_weight is smaller.
                     distances_wrapper.extend_and_set(n_id, n_path_weight)
 
                 # If we are to generate a path, we have to do it here, since the edge
                 # we have to add to the path prefix is not stored on the heap
-                if paths:
+                if build_paths:
                     try:
-                        # noinspection PyUnboundLocalVariable
                         predecessors_sequence[n_id] = vertex
                     except IndexError:
-                        # noinspection PyUnboundLocalVariable
-                        assert predecessors_wrapper is not None  # safe
-                        # noinspection PyUnboundLocalVariable
                         predecessors_wrapper.extend_and_set(n_id, vertex)
-                    if attributes_exists:
+                    if labeled_edges:
                         data_of_edge: T_labels = edge[-1]  # type: ignore[assignment]
                         try:
-                            # noinspection PyUnboundLocalVariable
                             attributes_sequence[n_id] = data_of_edge
                         except IndexError:
-                            # noinspection PyUnboundLocalVariable
                             attributes_wrapper.extend_and_set(n_id, data_of_edge)
 
                 h = heuristic(neighbor)
                 if h == infinity:
                     n_guess = infinity
                 else:
                     n_guess = n_path_weight + h
                     # (Distance values equal to or higher than the chosen infinity
                     # value of the gear are invalid and cannot be handled further.)
                     if infinity <= n_guess:
                         self._gear.raise_distance_infinity_overflow_error(n_guess)
+
+                if not is_tree:
                     try:
                         path_length_guesses_sequence[n_id] = n_guess
                     except IndexError:
-                        # noinspection PyUnboundLocalVariable
                         path_length_guesses_wrapper.extend_and_set(n_id, n_guess)
                 heappush(
                     to_visit,
                     (n_guess, next(unique_no), neighbor, n_path_edge_count),
                 )
 
+    def state_to_str(self, vertices: Optional[Iterable[T_vertex]] = None) -> str:
+        more = dict[str, Any]()
+        if vertices is not None:
+            if self._build_paths:
+                for vertex in vertices:
+                    more[f"paths[{vertex}]"] = self.paths[vertex]
+            if self._vertex_to_id is vertex_as_id:
+                for vertex in vertices:
+                    more[f"distances[{vertex}]"] = self.distances[
+                        self._vertex_to_id(vertex)
+                    ]
+            else:
+                for vertex in vertices:
+                    more[f"distances[vertex_to_id({vertex})]"] = self.distances[
+                        self._vertex_to_id(vertex)
+                    ]
+        return self._state_and_more_to_str(less=["paths", "distances"], more=more)
+
 
 class TraversalAStar(
     Generic[T_vertex, T_weight, T_labels],
     TraversalAStarFlex[T_vertex, T_vertex, Union[T_weight, float], T_labels],
 ):
     """
     Eases the use of `TraversalAStarFlex` for typical cases.
@@ -3288,26 +3087,28 @@
     | Bases: Generic[`T_vertex`, `T_vertex_id`, `T_weight`, `T_labels`],
     | `Traversal` [`T_vertex`, `T_vertex_id`, `T_labels`]
 
     :param vertex_to_id: See `VertexToID` function.
 
     :param gear: See `gears API <gears_api>` and class `Gear`.
 
-    :param next_edges: See `NextEdges` function. If None, provide next_labeled_edges.
+    :param next_edges: See `NextWeightedEdges` function. If None, provide
+      next_labeled_edges.
 
-    :param next_labeled_edges: See `NextEdges` function. Only allowed if next_edges
-      equals None. If given, paths will record the given labels.
+    :param next_labeled_edges: See `NextWeightedLabeledEdges` function. Only allowed
+      if next_edges equals None. If given, paths will record the given labels.
 
     **Algorithm:**  Minimum spanning tree ("MST") algorithm of Jarnik, Prim, Dijkstra.
     Non-recursive, based on heap. A so-called *tie breaker* is implemented, that
     prioritizes edges that have been found more recently about edges that have been
     found earlier. This is a typical choice that often improves search performance.
 
     **Properties:** Only edges of the MST from start vertices are reported. Each
-    vertex is visited only once.
+    vertex is reported (as end vertex of an edge) and expanded only once. Computed
+    paths only use MST edges.
 
     **Input:** Weighted undirected graph, given as directed edges with the same
     weight in both directions. One or more start vertices (e.g. for components in
     unconnected graphs). Optional calculation limit.
 
     **Search state:** When a vertex is *expanded* (traversal calls next_edges or
     next_labeled_edges) or an edge is *reported* (an iterator of the traversal returns
@@ -3336,109 +3137,129 @@
                     T_vertex, T_vertex_id, T_weight, T_labels
                 ],
                 T_weight,
                 T_labels,
             ]
         ] = None,
     ) -> None:
-        self.next_edges, self.labeled_edges = _create_unified_next_weighted(
+        self._next_edges, labeled_edges = _create_unified_next_weighted(
             next_edges, next_labeled_edges
         )
-        super().__init__(self.labeled_edges, False, vertex_to_id, gear)
+        super().__init__(labeled_edges, False, vertex_to_id, gear)
         self.edge: Optional[WeightedFullEdge[T_vertex, T_weight, T_labels]] = None
         """ Tuple of from_vertex, to_vertex, the weight of the edge,
         and additional data you have provided with the edge (if so).
         """
 
+        # The following value is not used by NoGraphs. It is only set
+        # to have some initialization.
+        self._start_vertices_and_ids = tuple[tuple[T_vertex, T_vertex_id]]()
+
     def start_from(
         self,
         start_vertex: Optional[T_vertex] = None,
         *,
         start_vertices: Optional[Iterable[T_vertex]] = None,
         build_paths: bool = False,
         calculation_limit: Optional[int] = None,
     ) -> TraversalMinimumSpanningTreeFlex[T_vertex, T_vertex_id, T_weight, T_labels]:
         """
         Start the traversal at a vertex or a set of vertices and set parameters.
 
         :param start_vertex: The vertex the search should start at. If None, provide
             start_vertices.
 
-        :param start_vertices: The set of vertices (iterator) the search should start
+        :param start_vertices: The set of vertices the search should start
             at. Only allowed if start_vertex equals None. Leads to a result
             consisting of several trees that are only connected if the start vertices
             are connected.
 
-        :param build_paths: If true, build paths from start vertices for each visited
-            vertex.
+        :param build_paths: If true, build paths from start vertices for each reported
+            vertex, and an empty path for each start vertex.
 
         :param calculation_limit: If provided, maximal number of vertices to process
             (read in) from your graph. If it is exceeded, a RuntimeError will be raised.
 
         :return: Traversal, that has been started, e.g., the methods go* can now be
             used.
         """
 
         if not isinstance(type(self), type(Traversal)):
             raise RuntimeError(
                 "Method start_from can only be called on a Traversal object."
             )
 
+        # ----- Initialize method specific public bookkeeping -----
         self._start_from(
             start_vertex,
             start_vertices,
             build_paths,
             calculation_limit,
             self._gear,
         )
+
+        # Explicitly list start vertices and their id. Needed several times.
+        self._start_vertices_and_ids = tuple(
+            iter_start_vertices_and_ids(self._start_vertices, self._vertex_to_id)
+        )
+
+        # The following value is not used by NoGraphs. It is only set
+        # to have some defined value before the traversal iterator sets them.
         self.edge = None
+
         super()._start()
         return self
 
     def _traverse(self) -> Iterator[T_vertex]:
         # ----- Prepare efficient environment for inner loop -----
         # Copy Traversal attributes into method scope (faster access)
+        labeled_edges = self._labeled_edges
         maybe_vertex_to_id = (
             None if self._vertex_to_id == vertex_as_id else self._vertex_to_id
         )  # Case vertex_as_id: not apply; T_vertex_id > T_vertex
+        build_paths = self._build_paths
         calculation_limit = self._calculation_limit
-        paths = self.paths
         predecessors = self._predecessors
         attributes = self._attributes
 
         # Copy traversal specific attributes into method scope
-        next_edges = self.next_edges
+        next_edges = self._next_edges
 
-        # Create booleans (avoid checks with "is")
-        attributes_exists = attributes is not None
-
-        # ----- Initialize method specific bookkeeping -----
+        # Get references of used gear objects and methods (avoid attribute resolution)
+        (
+            _,
+            predecessors_sequence,
+            predecessors_wrapper,
+        ) = access_to_vertex_mapping_expect_none(predecessors)
+        (
+            _,
+            attributes_sequence,
+            attributes_wrapper,
+        ) = access_to_vertex_mapping_expect_none(attributes)
 
-        # Explicitly list start vertices and their id. Needed several times.
-        start_vertices_and_ids = tuple(
-            _iter_start_vertices_and_ids(self._start_vertices, self._vertex_to_id)
-        )
+        # ----- Initialize method specific private bookkeeping -----
 
         # At start, only the start vertices are regarded as visited
         # (The protocol VertexSet abandons checking the element type, see
         #  VertexSet. Flake8 and MyPy accept this, PyCharm does not and need
         #   noinspection.)
         # noinspection PyTypeChecker
         visited: VertexIdSet[T_vertex_id] = self._gear.vertex_id_set(
-            vertex_id for vertex, vertex_id in start_vertices_and_ids
+            vertex_id for vertex, vertex_id in self._start_vertices_and_ids
         )
 
         # Check if we already go over the calculation limit when we evaluate the
         # edges from start vertices ("expanding the start vertices"). This avoids a
         # step by step check that slows down the to_visit loop for large sets of
         # start vertices. Note: A calculation limit below 0 leads nowhere ever to an
         # exception. So, neither here.
         if calculation_limit is not None and calculation_limit >= 0:
             if (
-                calculation_limit := calculation_limit - len(start_vertices_and_ids)
+                calculation_limit := calculation_limit
+                - len(self._start_vertices_and_ids)
             ) < 0:
                 raise RuntimeError("Number of visited vertices reached limit")
 
         # So far, the edges from the start vertices are to be visited as candidates
         # for edges of a MST. (Unique number prevents heapq from sorting by (possibly
         # not comparable) fields)
         unique_no = itertools.count()
@@ -3463,28 +3284,14 @@
             visited_uses_sequence,
             visited_sequence,
             visited_wrapper,
             visited_uses_bits,
             index_and_bit_method,
         ) = access_to_vertex_set(visited)
 
-        if paths:  # has no __len__, so this checks for non-None
-            assert predecessors is not None
-            (
-                _,
-                predecessors_sequence,
-                predecessors_wrapper,
-            ) = access_to_vertex_mapping_expect_none(predecessors)
-        if attributes is not None:
-            (
-                _,
-                attributes_sequence,
-                attributes_wrapper,
-            ) = access_to_vertex_mapping_expect_none(attributes)
-
         # ----- Inner loop -----
 
         while to_visit:
             # Visit edge with the lowest weight first
             _weight, _, vertex, to_edge = heappop(to_visit)
             to_vertex = to_edge[0]
 
@@ -3497,50 +3304,42 @@
                 maybe_vertex_to_id(to_vertex)  # type: ignore[assignment]
                 if maybe_vertex_to_id
                 else to_vertex
             )
 
             if visited_uses_sequence:
                 try:
-                    # noinspection PyUnboundLocalVariable
                     if visited_sequence[to_id]:
                         continue
                     visited_sequence[to_id] = True
                 except IndexError:
-                    # noinspection PyUnboundLocalVariable
                     visited_wrapper.extend_and_set(to_id, True)
             else:
                 if to_id in visited:
                     continue
                 visited_add(to_id)
 
-            if paths:
+            if build_paths:
                 try:
-                    # noinspection PyUnboundLocalVariable
                     predecessors_sequence[to_id] = vertex
                 except IndexError:
-                    # noinspection PyUnboundLocalVariable
-                    assert predecessors_wrapper is not None  # safe
-                    # noinspection PyUnboundLocalVariable
                     predecessors_wrapper.extend_and_set(to_id, vertex)
-                if attributes_exists:
-                    # attributes_exists -> self.labeled_edges (see assert above)
-                    # -> next_edges (a NextWeightedEdges) is a
+                if labeled_edges:
+                    # self._labeled_edges -> next_edges (a NextWeightedEdges) is a
                     # NextWeightedLabeledEdges -> edge[-1] is a T_labels.
                     data_of_edge: T_labels = to_edge[-1]  # type: ignore[assignment]
                     try:
-                        # noinspection PyUnboundLocalVariable
                         attributes_sequence[to_id] = data_of_edge
                     except IndexError:
-                        # noinspection PyUnboundLocalVariable
                         attributes_wrapper.extend_and_set(to_id, data_of_edge)
 
             # Export traversal data to traversal attribute and report vertex
             # (Expression type follows from types of vertex and to_edge and the
-            #  definition of WeightedFullEdge. MyPy cannot derive this.)
+            #  definition of WeightedFullEdge. MyPy + PyCharm cannot derive this.)
+            # noinspection PyTypeChecker
             full_edge: WeightedFullEdge[T_vertex, T_weight, T_labels] = (
                 vertex,
             ) + to_edge  # type: ignore[assignment]
             self.edge = full_edge
             yield to_vertex
 
             if calculation_limit and not (calculation_limit := calculation_limit - 1):
```

### Comparing `nographs-3.0.3/src/nographs/types.py` & `nographs-3.1.0/src/nographs/_types.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,44 +8,30 @@
 """
 Basic types used in NoGraphs.
 """
 
 
 T_vertex = TypeVar("T_vertex")
 T_vertex_id = TypeVar("T_vertex_id", bound=Hashable)
-
-""" T_weight: Type bound for weights.
-Discussion:
-- The real runtime-requirements of NoGraphs for weight values are:
-  - They are **mutual comparable**,
-  - they are **comparable to float('infinity')** or the supremal value
-    provided by the application and
-  - it is possible to **add them up**.
-- Real cannot be specified possible here, since float, int and Decimal are
-  not seen as Real by MyPy. And both PEP 484 and Guide von Rossum himself
-  clearly recommends to specify float instead of Real.
-- And both sources state, that for Python, int is acceptable as float. So,
-  the application can use values of Union(int, Literal[float("infinity"))) or
-  Union[range(max_weight), Literal[max_weight]] for weight values and
-  the needed supremal value. Note, that both expressions are no
-  type specification existing type checkers can process, in practice,
-  float has to be specified.
-"""
-
 T = TypeVar("T")
 
 
 # The following class is manually documented in api.rst, keep docs consistent.
 class Weight(Protocol[T]):
     @abstractmethod
     def __add__(self: T, value: T) -> T:
         """Return self+value."""
         raise NotImplementedError
 
     @abstractmethod
+    def __sub__(self: T, value: T) -> T:
+        """Return self-value."""
+        raise NotImplementedError
+
+    @abstractmethod
     def __lt__(self: T, value: T) -> bool:
         # inherited doc string
         raise NotImplementedError
 
     @abstractmethod
     def __le__(self: T, value: T) -> bool:
         # inherited doc string
@@ -107,7 +93,13 @@
     WeightedLabeledFullEdge[T_vertex, T_weight, T_labels],
 ]
 WeightedOrLabeledFullEdge = Union[
     WeightedUnlabeledFullEdge[T_vertex, T_weight],
     UnweightedLabeledFullEdge[T_vertex, T_labels],
     WeightedLabeledFullEdge[T_vertex, T_weight, T_labels],
 ]
+AnyFullEdge = Union[
+    UnweightedUnlabeledFullEdge[T_vertex],
+    WeightedUnlabeledFullEdge[T_vertex, T_weight],
+    UnweightedLabeledFullEdge[T_vertex, T_labels],
+    WeightedLabeledFullEdge[T_vertex, T_weight, T_labels],
+]
```

### Comparing `nographs-3.0.3/src/nographs.egg-info/PKG-INFO` & `nographs-3.1.0/src/nographs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nographs
-Version: 3.0.3
+Version: 3.1.0
 Summary: Graph analysis – the lazy (evaluation) way: Analysis on the fly, for graphs, that are computed and/or adapted on the fly.
 Home-page: https://github.com/HeWeMel/nographs
 Author: Dr. Helmut Melcher
 Author-email: HeWeMel@web.de
 Project-URL: Documentation, https://nographs.readthedocs.io/
 Project-URL: Source, https://github.com/hewemel/nographs/
 Project-URL: Bug Reports, https://github.com/hewemel/nographs/issues
@@ -71,45 +71,57 @@
 **the analysis and the reporting of results by the library happen on the fly**
 (when, and as far as, results can already be derived).
 
 Think of it as *graph analysis - the lazy (evaluation) way*.
 
 **Feature overview**
 
-- Algorithms: DFS, BFS, topological search,
+- Unidirectional traversal algorithms: DFS, BFS, topological search,
   Dijkstra, A\* and MST.
-- Flexible graph notion: Infinite directed multigraphs with loops and
-  attributes (this includes
-  multiple adjacency, cycles, self-loops,
-  directed edges,
-  weighted edges and edges with application specific attributes).
-  Your vertices can be nearly anything.
-  Wide range of data types for edge weights and path length
-  supported (float, int, Decimal, mpmath.mpf and others), e.g.,
-  for high precision computations.
-  Infinite graphs are supported, but need to be
-  locally finite (i.e., a vertex has only finitely many outgoing edges).
+- Bidirectional search algorithms: BFS and Dijkstra.
+- Flexible graph notion:
+
+  - Infinite directed multigraphs with loops and
+    attributes (this includes
+    multiple adjacency, cycles, self-loops,
+    directed edges,
+    weighted edges and edges with application specific attributes).
+  - Infinite graphs are supported, but need to be
+    locally finite (i.e., a vertex has only finitely many outgoing edges).
+
+- Generic API. The application can define the following:
+
+  - Vertices: Can be anything except for None. Hashable vertices can be
+    used directly, unhashable vertices can be used together with
+    hashable identifiers.
+  - Edge weights and distances: Wide range of data types
+    supported (float, int, Decimal, mpmath.mpf and others), e.g.,
+    for high precision computations.
+  - Edge attributes: Any object, e.g, a container
+    with further data.
+  - Identity and equivalence of vertices.
+  - Bookkeeping: Several sets of bookkeeping data structures
+    are predefined, optimized for different situations (data types used by the
+    application, hashing vs. indexing, collections for *Python* objects or *C* native
+    data types,...); Adaptable and extendable, e.g., specialized
+    collections of 3rd party libraries can be integrated easily and runtime
+    efficiently
+
 - Results: Reachability, depth, distance, paths and trees.
   Paths can be
   calculated with vertices or edges or attributed edges
   and can be iterated in both directions.
 - Flexible API: The concept of implicit graphs that NoGraphs is based on
-  allows for an API that eases operations like
-  graph pruning, graph product and graph abstraction ike
+  allows for an API that eases
+  operations like
   graph pruning, graph abstraction, the typical binary
   graph operations (union, intersection, several types of products), the
   computation of search-aware graphs, and
   traversals of vertex equivalence classes on the fly.
-- Flexible bookkeeping:
-  Several sets of bookkeeping data structures,
-  optimized for different situations (data types used by the application,
-  hashing vs. indexing, collections for Python objects or *C* native data types,
-  ...); Adaptable and extendable, e.g., specialized collections of
-  3rd party libraries can be integrated easily and runtime efficiently. Internal
-  bookkeeping data can be
+  Bookkeeping data can be
   pre-initialized and accessed during computations.
 - Typing: The API can be used fully typed (optionally).
 - Implementation: Pure Python (>=3.9). It introduces no further dependencies.
 - Runtime and memory performance: Have been goals. In its domain, it
   often even outperforms Rust- and C-based libraries.
 
 **Documentation**
```

### Comparing `nographs-3.0.3/tests/test_nographs.py` & `nographs-3.1.0/tests/test_nographs.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,26 +30,28 @@
     cov = coverage.Coverage(source_pkgs=["nographs"])
     cov.start()
 
     # Create empty TestSuite
     test_suite = unittest.TestSuite()
 
     # Unittests from doc tests in module with special test cases
-    for file in ["test_code"]:
-        __import__(file)
-        test_suite.addTests(doctest.DocTestSuite(file))
+
+    for file in pathlib.Path("tests").glob("*.py"):
+        name = file.name.removesuffix(".py")
+        __import__(name)
+        test_suite.addTests(doctest.DocTestSuite(name))
 
     # Unittests from unit test classes in some unit test files in tests folder
     new_suite = unittest.defaultTestLoader.discover("tests", pattern="test_unit*.py")
     test_suite.addTests(new_suite)
 
     # Unittests from doc tests in modules of package
     modules = ("types", "strategies", "matrix_gadgets", "edge_gadgets", "paths")
     for f in modules:
-        temp_module = importlib.import_module("." + f, "nographs")
+        temp_module = importlib.import_module("._" + f, "nographs")
         test_suite.addTests(doctest.DocTestSuite(temp_module))
 
     # Unittests from doc tests in documentation
     p = pathlib.Path("./docs/source")
     for file_path in p.glob("*.rst"):
         test_suite.addTests(doctest.DocFileSuite(str(file_path), module_relative=False))
```

### Comparing `nographs-3.0.3/tests/test_unit_typed.py` & `nographs-3.1.0/tests/test_unit_typed.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,29 @@
-import decimal
-from decimal import Decimal
+import sys
+from decimal import Decimal, getcontext
 from collections.abc import Iterator
-from typing import Any, TypeVar, TYPE_CHECKING
+from typing import Any, TypeVar, Union, TYPE_CHECKING
+
+if sys.version_info >= (3, 11):
+    from typing import assert_type
 import unittest
 
 from mpmath import mp, mpf  # type: ignore
 
 import nographs as nog
 
 
+# --- Types ---
+
 T_any_typical_weight_type = TypeVar("T_any_typical_weight_type", float, Decimal, mpf)
 
 
+# --- Tests ---
+
+
 class Test1(unittest.TestCase):
     def test_variable_edge_weights(self) -> None:
         def test_with_small_weights(
             zero: T_any_typical_weight_type,
             one_half: T_any_typical_weight_type,
             one: T_any_typical_weight_type,
         ) -> int:
@@ -40,35 +48,44 @@
                 previous_distance = distance
             raise RuntimeError("Unexpected end of loop")  # pragma: no cover
 
         with self.assertRaises(RuntimeError) as cm:
             test_with_small_weights(float(0), float("0.5"), float(1))
         self.assertEqual(cm.exception.args, ("Error: Distance stays constant",))
 
-        decimal.getcontext().prec = 75  # precision (number of places)
+        getcontext().prec = 75  # precision (number of places)
         self.assertEquals(
             test_with_small_weights(Decimal(0), Decimal("0.5"), Decimal(1)), 65
         )
 
         mp.prec = 64
         self.assertEquals(test_with_small_weights(mpf(0), mpf("0.5"), mpf(1)), 65)
 
     def test_typing_docs_example(self) -> None:
-        def next_edges(i: int, _) -> Iterator[tuple[int, int]]:
+        def next_edges(i: int, _: Any) -> Iterator[tuple[int, int]]:
             j = (i + i // 6) % 6
             yield i + 1, j * 2 + 1
             if i % 2 == 0:
                 yield i + 6, 7 - j
             elif i % 1200000 > 5:
                 yield i - 6, 1
 
         traversal = nog.TraversalShortestPaths[int, int, Any](next_edges)
         v = traversal.start_from(0, build_paths=True).go_to(5)
         d = traversal.distance
         p = tuple(traversal.paths.iter_vertices_from_start(v))
-        if TYPE_CHECKING:  # pragma: no cover
-            reveal_type(v)  # noqa: F821, reveals: int
-            reveal_type(d)  # noqa: F821, reveals: float
-            reveal_type(p)  # noqa: F821, reveals: tuple[int, ...]
+        if sys.version_info >= (3, 11):
+            if TYPE_CHECKING:
+                # for Python>=3.11, check types
+                assert_type(v, int)
+                assert_type(d, Union[int, float])
+                assert_type(p, tuple[int, ...])
+        else:
+            reveal_type = print  # will never be used; just for IDEs
+            # for Python<3.11, reveal types
+            if TYPE_CHECKING:
+                reveal_type(v)  # reveals: int
+                reveal_type(d)  # reveals: Union[int, float]
+                reveal_type(p)  # reveals: tuple[int, ...]
         self.assertEquals(v, 5)
         self.assertEquals(d, 24)
         self.assertEquals(p, (0, 1, 2, 3, 4, 10, 16, 17, 11, 5))
```

