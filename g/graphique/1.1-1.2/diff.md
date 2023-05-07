# Comparing `tmp/graphique-1.1.tar.gz` & `tmp/graphique-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphique-1.1.tar", last modified: Sun Jan 29 20:17:09 2023, max compression
+gzip compressed data, was "graphique-1.2.tar", last modified: Sun May  7 18:32:34 2023, max compression
```

## Comparing `graphique-1.1.tar` & `graphique-1.2.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 20:17:09.760099 graphique-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-01-29 20:16:42.000000 graphique-1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-01-29 20:17:09.760099 graphique-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-01-29 20:16:42.000000 graphique-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 20:17:09.760099 graphique-1.1/graphique/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-29 20:16:42.000000 graphique-1.1/graphique/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23539 2023-01-29 20:16:42.000000 graphique-1.1/graphique/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    29839 2023-01-29 20:16:42.000000 graphique-1.1/graphique/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23387 2023-01-29 20:16:42.000000 graphique-1.1/graphique/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-01-29 20:16:42.000000 graphique-1.1/graphique/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-01-29 20:16:42.000000 graphique-1.1/graphique/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-29 20:16:42.000000 graphique-1.1/graphique/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-01-29 20:16:42.000000 graphique-1.1/graphique/scalars.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-01-29 20:16:42.000000 graphique-1.1/graphique/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-01-29 20:16:42.000000 graphique-1.1/graphique/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 20:17:09.760099 graphique-1.1/graphique.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-01-29 20:17:09.000000 graphique-1.1/graphique.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-01-29 20:17:09.000000 graphique-1.1/graphique.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 20:17:09.000000 graphique-1.1/graphique.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-01-29 20:17:09.000000 graphique-1.1/graphique.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-29 20:17:09.000000 graphique-1.1/graphique.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-01-29 20:16:42.000000 graphique-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-29 20:17:09.760099 graphique-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:32:34.269271 graphique-1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-07 18:32:05.000000 graphique-1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-05-07 18:32:34.265270 graphique-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-05-07 18:32:05.000000 graphique-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:32:34.265270 graphique-1.2/graphique/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-07 18:32:05.000000 graphique-1.2/graphique/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24189 2023-05-07 18:32:05.000000 graphique-1.2/graphique/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30184 2023-05-07 18:32:05.000000 graphique-1.2/graphique/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24570 2023-05-07 18:32:05.000000 graphique-1.2/graphique/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-07 18:32:05.000000 graphique-1.2/graphique/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-05-07 18:32:05.000000 graphique-1.2/graphique/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 18:32:05.000000 graphique-1.2/graphique/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-07 18:32:05.000000 graphique-1.2/graphique/scalars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-07 18:32:05.000000 graphique-1.2/graphique/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:32:34.265270 graphique-1.2/graphique.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-05-07 18:32:34.000000 graphique-1.2/graphique.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-07 18:32:34.000000 graphique-1.2/graphique.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 18:32:34.000000 graphique-1.2/graphique.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-07 18:32:34.000000 graphique-1.2/graphique.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 18:32:34.000000 graphique-1.2/graphique.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-07 18:32:05.000000 graphique-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 18:32:34.269271 graphique-1.2/setup.cfg
```

### Comparing `graphique-1.1/LICENSE.txt` & `graphique-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `graphique-1.1/PKG-INFO` & `graphique-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphique
-Version: 1.1
+Version: 1.2
 Summary: GraphQL service for arrow tables and parquet data sets.
 Author-email: Aric Coady <aric.coady@gmail.com>
 License: Copyright 2022 Aric Coady
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
@@ -84,15 +84,15 @@
 app = GraphQL(ds.dataset(...))  # Table is root query type
 app = GraphQL.federated({<name>: ds.dataset(...), ...}, keys={...})  # Tables on federated fields
 ```
 
 Start like any ASGI app.
 
 ```console
-uvicorn <package>:app
+uvicorn <module>:app
 ```
 
 Configuration options exist to provide a convenient no-code solution, but are subject to change in the future. Using a custom app is recommended for production usage.
 
 ### API
 #### types
 * `Dataset`: interface for an arrow dataset, scanner, or table.
@@ -134,32 +134,39 @@
 
 ## Installation
 ```console
 % pip install graphique[server]
 ```
 
 ## Dependencies
-* pyarrow >=11
-* strawberry-graphql[asgi,cli] >=0.149.2
+* pyarrow >=12
+* strawberry-graphql[asgi,cli]
 * uvicorn (or other [ASGI server](https://asgi.readthedocs.io/en/latest/implementations.html))
 
 ## Tests
 100% branch coverage.
 
 ```console
 % pytest [--cov]
 ```
 
 ## Changes
+1.2
+
+* Pyarrow >=12 required
+* Grouping fragments optimized
+* Group by empty columns
+* Batch sorting and grouping into lists
+
 1.1
 
 * Pyarrow >=11 required
 * Python >=3.8 required
 * Scannable functions added
-* List aggregations deprecaated
+* List aggregations deprecated
 * Group by fragments
 * Month day nano interval array
 * `min` and `max` fields memory optimized
 
 1.0
 
 * Pyarrow >=10 required
@@ -222,13 +229,13 @@
 
 * Pyarrow >=3 required
 * `any` and `all` fields
 * String column `split` field
 
 0.2
 
+* Pyarrow >= 2 required
 * `ListColumn` and `StructColumn` types
 * `Groups` type with `aggregate` field
 * `group` and `unique` optimized
-* pyarrow >= 2 required
 * Statistical fields: `mode`, `stddev`, `variance`
 * `is_in`, `min`, and `max` optimized
```

### Comparing `graphique-1.1/README.md` & `graphique-1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 app = GraphQL(ds.dataset(...))  # Table is root query type
 app = GraphQL.federated({<name>: ds.dataset(...), ...}, keys={...})  # Tables on federated fields
 ```
 
 Start like any ASGI app.
 
 ```console
-uvicorn <package>:app
+uvicorn <module>:app
 ```
 
 Configuration options exist to provide a convenient no-code solution, but are subject to change in the future. Using a custom app is recommended for production usage.
 
 ### API
 #### types
 * `Dataset`: interface for an arrow dataset, scanner, or table.
@@ -92,32 +92,39 @@
 
 ## Installation
 ```console
 % pip install graphique[server]
 ```
 
 ## Dependencies
-* pyarrow >=11
-* strawberry-graphql[asgi,cli] >=0.149.2
+* pyarrow >=12
+* strawberry-graphql[asgi,cli]
 * uvicorn (or other [ASGI server](https://asgi.readthedocs.io/en/latest/implementations.html))
 
 ## Tests
 100% branch coverage.
 
 ```console
 % pytest [--cov]
 ```
 
 ## Changes
+1.2
+
+* Pyarrow >=12 required
+* Grouping fragments optimized
+* Group by empty columns
+* Batch sorting and grouping into lists
+
 1.1
 
 * Pyarrow >=11 required
 * Python >=3.8 required
 * Scannable functions added
-* List aggregations deprecaated
+* List aggregations deprecated
 * Group by fragments
 * Month day nano interval array
 * `min` and `max` fields memory optimized
 
 1.0
 
 * Pyarrow >=10 required
@@ -180,13 +187,13 @@
 
 * Pyarrow >=3 required
 * `any` and `all` fields
 * String column `split` field
 
 0.2
 
+* Pyarrow >= 2 required
 * `ListColumn` and `StructColumn` types
 * `Groups` type with `aggregate` field
 * `group` and `unique` optimized
-* pyarrow >= 2 required
 * Statistical fields: `mode`, `stddev`, `variance`
 * `is_in`, `min`, and `max` optimized
```

### Comparing `graphique-1.1/graphique/core.py` & `graphique-1.2/graphique/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 Their methods are called as functions.
 """
 import bisect
 import contextlib
 import functools
 import inspect
 import itertools
+import operator
 import json
-from concurrent import futures
 from dataclasses import dataclass
 from typing import Callable, Iterable, Iterator, Optional, Sequence, Union, get_type_hints
 import numpy as np  # type: ignore
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.dataset as ds
 
-threader = futures.ThreadPoolExecutor(pa.cpu_count())
+Array = Union[pa.Array, pa.ChunkedArray]
 
 
 class Agg:
     """Aggregation options."""
 
     option_map = {
         'all': pc.ScalarAggregateOptions,
@@ -48,19 +48,22 @@
 
     def __init__(self, name: str, alias: str = '', **options):
         self.name = name
         self.alias = alias or name
         self.options = options
 
     def astuple(self, func: str) -> tuple:
-        return f'hash_{func}', self.option_map[func](**self.options)
+        options = self.option_map[func](**self.options)
+        return self.name, func, options
 
     @classmethod
     def getfunc(cls, name: str) -> Callable:
         """Return callable with named parameters for keyword arguments."""
+        if name in ('first', 'last', 'one'):
+            return operator.itemgetter(-1 if name == 'last' else 0)
         if name == 'element':
             return lambda array, index: array[index]
         if name == 'slice':
             return lambda array, start, stop, step: array[start:stop:step]
         return getattr(pc, name)
 
 
@@ -140,37 +143,47 @@
         return (scalar.values or empty for scalar in self)
 
     def map_list(self, func: Callable, **kwargs) -> pa.lib.BaseListArray:
         """Return list array by mapping function across scalars, with null handling."""
         values = [func(value, **kwargs) for value in ListChunk.scalars(self)]
         return ListChunk.from_scalars(values)
 
-    def aggregate(self, **funcs: Optional[pc.FunctionOptions]) -> pa.StructArray:
+    def inner_flatten(self) -> pa.lib.BaseListArray:
+        """Return flattened inner lists from a nested list array."""
+        offsets = self.values.offsets.take(self.offsets)
+        return type(self).from_arrays(offsets, self.values.values)
+
+    def aggregate(self, **funcs: Optional[pc.FunctionOptions]) -> pa.RecordBatch:
         """Return aggregated scalars by grouping each hash function on the parent indices.
 
         If there are empty or null scalars, then the result must be padded with null defaults and
         reordered. If the function is a `count`, then the default is 0.
         """
-        items = {f'hash_{name}': funcs[name] for name in funcs}.items()
-        indices = pc.list_parent_indices(self)
-        groups = pc._group_by([pc.list_flatten(self)] * len(funcs), [indices], items)
-        if len(groups) == len(self):  # no empty or null scalars
-            return groups
+        columns = {'key': pc.list_parent_indices(self), '': pc.list_flatten(self)}
+        items = [('', name, funcs[name]) for name in funcs]
+        table = pa.table(columns).group_by(['key']).aggregate(items)
+        indices, table = table['key'], table.remove_column(table.schema.get_field_index('key'))
+        (batch,) = table.to_batches()
+        if len(batch) == len(self):  # no empty or null scalars
+            return batch
         mask = pc.equal(pc.list_value_length(self), 0)
         empties = pc.indices_nonzero(Column.fill_null(mask, True))
-        indices = pa.concat_arrays([groups.field(-1).cast('uint64'), empties])
-        counters = [field.name for field in groups.type if 'count' in field.name]
-        empties = pa.repeat(pa.scalar(dict.fromkeys(counters, 0), groups.type), len(empties))
-        return pa.concat_arrays([groups, empties]).take(pc.sort_indices(indices))
+        indices = pa.chunked_array(indices.chunks + [empties.cast(indices.type)])
+        columns = {}
+        for field in batch.schema:
+            scalar = pa.scalar(0 if 'count' in field.name else None, field.type)
+            columns[field.name] = pa.repeat(scalar, len(empties))
+        table = pa.concat_tables([table, pa.table(columns)]).combine_chunks()
+        return table.to_batches()[0].take(pc.sort_indices(indices))
 
     def min_max(self, **options) -> pa.Array:
         if pa.types.is_dictionary(self.type.value_type):
-            self = ListChunk.aggregate(self, distinct=None).field(0)
+            (self,) = ListChunk.aggregate(self, distinct=None)
             self = type(self).from_arrays(self.offsets, self.values.dictionary_decode())
-        return ListChunk.aggregate(self, min_max=pc.ScalarAggregateOptions(**options)).field(0)
+        return ListChunk.aggregate(self, min_max=pc.ScalarAggregateOptions(**options))[0]
 
     def min(self, **options) -> pa.Array:
         """min value of each list scalar"""
         return ListChunk.min_max(self, **options).field('min')
 
     def max(self, **options) -> pa.Array:
         """max value of each list scalar"""
@@ -188,20 +201,20 @@
         """index for first occurrence of each list scalar"""
         values = [pc.index(value, **options) for value in ListChunk.scalars(self)]
         return Column.from_scalars(values)
 
     @register
     def list_all(ctx, self: pa.list_(pa.bool_())) -> pa.bool_():  # type: ignore
         """Test whether all elements in a boolean array evaluate to true."""
-        return ListChunk.aggregate(self, all=None).field(0)
+        return ListChunk.aggregate(self, all=None)[0]
 
     @register
     def list_any(ctx, self: pa.list_(pa.bool_())) -> pa.bool_():  # type: ignore
         """Test whether any element in a boolean array evaluates to true."""
-        return ListChunk.aggregate(self, any=None).field(0)
+        return ListChunk.aggregate(self, any=None)[0]
 
 
 class Column(pa.ChunkedArray):
     """Chunked array interface as a namespace of functions."""
 
     def from_scalars(values: Sequence) -> pa.Array:
         """Return array from arrow scalars."""
@@ -210,55 +223,37 @@
     def scalar_type(self):
         return self.type.value_type if pa.types.is_dictionary(self.type) else self.type
 
     def is_list_type(self):
         funcs = pa.types.is_list, pa.types.is_large_list, pa.types.is_fixed_size_list
         return any(func(self.type) for func in funcs)
 
-    def combine_dictionaries(self) -> tuple:
+    def call_indices(self, func: Callable) -> Array:
         if not pa.types.is_dictionary(self.type):
-            return self, None
-        if not self or len(self) <= max(len(chunk.dictionary) for chunk in self.iterchunks()):
-            return self.cast(self.type.value_type), None
-        self = self.unify_dictionaries()
-        indices = pa.chunked_array(chunk.indices for chunk in self.iterchunks())
-        return self.chunk(0).dictionary, indices
-
-    def indices(self) -> Union[pa.Array, pa.ChunkedArray]:
-        """Return chunked indices suitable for aggregation."""
-        if isinstance(self, pa.Array):
-            return pa.array(np.arange(len(self)))
-        offsets = list(itertools.accumulate(map(len, self.iterchunks())))
-        return pa.chunked_array(map(np.arange, [0] + offsets, offsets))
-
-    def call_indices(self, func: Callable) -> pa.ChunkedArray:
-        dictionary, indices = Column.combine_dictionaries(self)
-        if indices is None:
-            return func(dictionary)
-        return pa.chunked_array(
-            pa.DictionaryArray.from_arrays(chunk, dictionary) for chunk in func(indices).chunks
-        )
+            return func(self)
+        array = self.combine_chunks()
+        return pa.DictionaryArray.from_arrays(func(array.indices), array.dictionary)
 
-    def fill_null_backward(self) -> pa.ChunkedArray:
+    def fill_null_backward(self) -> Array:
         """`fill_null_backward` with dictionary support."""
         return Column.call_indices(self, pc.fill_null_backward)
 
-    def fill_null_forward(self) -> pa.ChunkedArray:
+    def fill_null_forward(self) -> Array:
         """`fill_null_forward` with dictionary support."""
         return Column.call_indices(self, pc.fill_null_forward)
 
     def fill_null(self, value) -> pa.ChunkedArray:
         """Optimized `fill_null` to check `null_count`."""
         return self.fill_null(value) if self.null_count else self
 
-    def sort_values(self) -> pa.Array:
-        dictionary, indices = Column.combine_dictionaries(self)
-        if indices is None:
-            return dictionary
-        return pc.sort_indices(pc.sort_indices(dictionary)).take(indices)
+    def sort_values(self) -> Array:
+        if not pa.types.is_dictionary(self.type):
+            return self
+        array = self if isinstance(self, pa.Array) else self.combine_chunks()
+        return pc.sort_indices(pc.sort_indices(array.dictionary)).take(array.indices)
 
     def diff(self, func: Callable = pc.subtract) -> pa.ChunkedArray:
         """Return discrete differences between adjacent values."""
         return func(self[1:], self[:-1])
 
     def partition_offsets(self, predicate: Callable = pc.not_equal, *args) -> pa.IntegerArray:
         """Return list array offsets by partitioning on discrete differences.
@@ -314,18 +309,18 @@
             stop = bisect.bisect_right(self, value, start)
             yield slice(start, stop)
 
 
 class Table(pa.Table):
     """Table interface as a namespace of functions."""
 
-    def map_batch(self, func: Callable, *rargs, **kwargs) -> pa.Table:
-        return pa.Table.from_batches(
-            threader.map(lambda batch: func(batch, *rargs, **kwargs), self.to_batches())
-        )
+    def map_batch(scanner: ds.Scanner, func: Callable, *rargs, **kwargs) -> pa.Table:
+        # TODO(apache/arrow#31612): replace with user defined function for multiple kernels
+        batches = [func(batch, *rargs, **kwargs) for batch in scanner.to_batches() if batch]
+        return pa.Table.from_batches(batches, None if batches else scanner.projected_schema)
 
     def union(*tables: pa.Table) -> pa.Table:
         """Return table with union of columns."""
         columns: dict = {}
         for table in tables:
             columns.update(zip(table.column_names, table))
         return pa.table(columns)
@@ -347,15 +342,15 @@
 
     def not_equal(self, name: str, value) -> pa.Table:
         """Return rows which don't match the value.
 
         Assumes the table is sorted by the column name, i.e., indexed.
         """
         (slc,) = Column.find(self[name], value)
-        return pa.concat_tables([self[: slc.start], self[slc.stop :]])  # noqa: E203
+        return pa.concat_tables([self[: slc.start], self[slc.stop :]])
 
     def from_offsets(self, offsets: pa.IntegerArray) -> pa.Table:
         """Return table with columns converted into list columns."""
         cls = pa.LargeListArray if offsets.type == 'int64' else pa.ListArray
         arrays = [col.combine_chunks() if col else pa.array([], col.type) for col in self]
         return pa.table([cls.from_arrays(offsets, array) for array in arrays], self.column_names)
 
@@ -395,134 +390,157 @@
         Args:
             *names: columns to group by
             counts: alias for optional row counts
             first: columns to take first value
             last: columns to take last value
             **funcs: aggregate funcs with columns options
         """
-        column = self[names[0]]
-        args = [(column, 'hash_count', pc.CountOptions(mode='all'))] if counts else []
+        if isinstance(self, pa.Table):
+            self = self.unify_dictionaries()
+        columns = {name: self[name] for name in self.schema.names}
+        aliases, args = {}, []  # type: ignore
+        if counts:
+            aliases['count_all'] = counts
+            args.append(([], 'count_all'))
         if first or last:
-            args.append((Column.indices(column), 'hash_min_max', None))
+            columns[''] = np.arange(len(self))
+            args.append(('', 'min_max'))
         lists: Sequence[Agg] = []
         list_cols = [self[agg.name] for agg in funcs.get('list', [])]
         if any(pa.types.is_dictionary(col.type) or Column.is_list_type(col) for col in list_cols):
-            args.append((Column.indices(column), 'hash_list', None))
+            columns[''] = np.arange(len(self))
+            args.append(('', 'list'))
             lists = funcs.pop('list')
-        for func in funcs:
-            args += [(self[agg.name], *agg.astuple(func)) for agg in funcs[func]]  # type: ignore
-        values, hashes, options = zip(*args) if args else [()] * 3
-        keys = map(self.column, names)
-        if isinstance(self, pa.Table):
-            keys = (key.unify_dictionaries() for key in keys)  # type: ignore
-            values = (
-                value.unify_dictionaries() if 'distinct' in func else value
-                for value, func in zip(values, hashes)
-            )
-        arrays = iter(pc._group_by(values, keys, zip(hashes, options)).flatten())
-        columns = {counts: next(arrays)} if counts else {}
+        for func, aggs in funcs.items():
+            aliases.update({f'{agg.name}_{func}': agg.alias for agg in aggs})
+            args += (agg.astuple(func) for agg in aggs)  # type: ignore
+        table = pa.table(columns).group_by(list(names)).aggregate(args)
+        columns = {name: table[name].combine_chunks() for name in table.schema.names}
         if first or last:
-            for aggs, indices in zip([first, last], next(arrays).flatten()):
+            for aggs, indices in zip([first, last], columns.pop('_min_max').flatten()):
                 columns.update({agg.alias: self[agg.name].take(indices) for agg in aggs})
         if lists:
-            indices = next(arrays)
+            indices = columns.pop('_list')
             table = self.select({agg.name for agg in lists}).take(indices.values)
             table = Table.from_offsets(table, indices.offsets)
-            columns.update({agg.alias: table[agg.name] for agg in lists})
-        for aggs in funcs.values():
-            columns.update(zip([agg.alias for agg in aggs], arrays))
-        columns.update(zip(names, map(decode, arrays)))
+            columns.update({agg.alias: table[agg.name].combine_chunks() for agg in lists})
+        columns.update({name: decode(columns[name]) for name in names})
+        columns = {aliases.get(name, name): columns[name] for name in columns}
         return type(self).from_pydict(columns)
 
     def aggregate(self, counts: str = '', **funcs: Sequence[Agg]) -> dict:
         """Return aggregated scalars as a row of data."""
         row = {name: self[name] for name in self.column_names}
         if counts:
             row[counts] = len(self)
+        aliases, args = {}, []  # type: ignore
         for key in funcs:
-            func = Agg.getfunc(key)
-            row.update({agg.alias: func(self[agg.name], **agg.options) for agg in funcs[key]})
+            if key in Agg.option_map:
+                aliases.update({f'{agg.name}_{key}': agg.alias for agg in funcs[key]})
+                args += (agg.astuple(key) for agg in funcs[key])
+            else:
+                func = Agg.getfunc(key)
+                row.update({agg.alias: func(self[agg.name], **agg.options) for agg in funcs[key]})
+        if args:
+            table = self.group_by([]).aggregate(args)
+            row.update({aliases[name]: table[name][0] for name in table.column_names})
         for name, value in row.items():
             if isinstance(value, pa.ChunkedArray):
                 row[name] = value.combine_chunks()
         return row
 
+    def list_fields(self) -> set:
+        return {field.name for field in self.schema if Column.is_list_type(field)}
+
     def list_value_length(self) -> pa.Array:
-        lists = {name for name in self.column_names if Column.is_list_type(self[name])}
+        lists = Table.list_fields(self)
         if not lists:
-            raise ValueError(f"no list columns available: {self.column_names}")
+            raise ValueError(f"no list columns available: {self.schema.names}")
         counts, *others = (pc.list_value_length(self[name]) for name in lists)
         if any(counts != other for other in others):
             raise ValueError(f"list columns have different value lengths: {lists}")
-        return counts.chunk(0)
+        return counts if isinstance(counts, pa.Array) else counts.chunk(0)
 
-    def sort_list(self, *names: str, length: Optional[int] = None) -> pa.Table:
+    def sort_list(
+        self, *names: str, length: Optional[int] = None, null_placement: str = 'at_end'
+    ) -> pa.Table:
         """Return table with list columns sorted within scalars."""
         keys = dict(map(sort_key, names))  # type: ignore
         columns = {name: Column.sort_values(pc.list_flatten(self[name])) for name in keys}
         columns[''] = pc.list_parent_indices(self[next(iter(keys))])
         keys = dict({'': 'ascending'}, **keys)
-        indices = pc.sort_indices(pa.table(columns), sort_keys=keys.items())
+        indices = pc.sort_indices(
+            pa.table(columns), sort_keys=keys.items(), null_placement=null_placement
+        )
         counts = Table.list_value_length(self)
         if length is not None:
             indices = pa.concat_arrays(
                 scalar.values[:length] for scalar in ListChunk.from_counts(counts, indices)
             )
             counts = pc.min_element_wise(counts, length)
         table = Table.select_list(self, pc.list_flatten).take(indices)
         return Table.union(self, Table.from_counts(table, counts))
 
     def select_list(self, apply: Callable = lambda c: c) -> pa.Table:
         """Return table with only the list columns."""
-        names = [name for name in self.column_names if Column.is_list_type(self[name])]
+        names = list(Table.list_fields(self))
         return pa.table(list(map(apply, self.select(names))), names)
 
-    def sort_indices(self, *names: str, length: Optional[int] = None) -> pa.Table:
+    def sort_indices(
+        self, *names: str, length: Optional[int] = None, null_placement: str = 'at_end'
+    ) -> pa.Array:
         """Return indices which would sort the table by columns, optimized for fixed length."""
-        func = pc.sort_indices
+        func = functools.partial(pc.sort_indices, null_placement=null_placement)
         if length is not None:
             func = functools.partial(pc.select_k_unstable, k=length)
         keys = dict(map(sort_key, names))  # type: ignore
         table = pa.table({name: Column.sort_values(self[name]) for name in keys})
         return func(table, sort_keys=keys.items())
 
-    def sort(self, *names: str, length: Optional[int] = None, indices: str = '') -> pa.Table:
+    def sort(
+        self,
+        *names: str,
+        length: Optional[int] = None,
+        indices: str = '',
+        null_placement: str = 'at_end',
+    ) -> pa.Table:
         """Return table sorted by columns, optimized for fixed length.
 
         Args:
             *names: columns to sort by
             length: maximum number of rows to return
             indices: include original indices in the table
         """
-        indices_ = Table.sort_indices(self, *names, length=length)
+        indices_ = Table.sort_indices(self, *names, length=length, null_placement=null_placement)
         table = self.take(indices_)
         if indices:
             table = table.append_column(indices, indices_)
         func = lambda name: not name.startswith('-') and not self[name].null_count  # noqa: E731
         metadata = {'index_columns': list(itertools.takewhile(func, names))}
         return table.replace_schema_metadata({'pandas': json.dumps(metadata)})
 
-    def filter_list(self, expr: ds.Expression) -> 'Table':
+    def filter_list(self, expr: ds.Expression) -> pa.Table:
         """Return table with list columns filtered within scalars."""
         table = Table.select_list(self)
         counts = Table.list_value_length(table)
         first = table[0].combine_chunks()
         indices = pc.list_parent_indices(first)
         columns = [
             pc.list_flatten(column) if Column.is_list_type(column) else column.take(indices)
             for column in self
         ]
         flattened = pa.table(columns, self.column_names)
         mask = ds.dataset(flattened).to_table(columns={'mask': expr})['mask'].combine_chunks()
         masks = type(first).from_arrays(first.offsets, mask)
-        counts = Column.fill_null(ListChunk.aggregate(masks, sum=None).field(0), 0)
+        counts = Column.fill_null(ListChunk.aggregate(masks, sum=None)[0], 0)
         flattened = flattened.select(table.column_names).filter(mask)
         return Table.union(self, Table.from_counts(flattened, counts))
 
-    def matched(self, func: Callable, *names: str) -> pa.Table:
-        for name in names:
+    def min_max(self, *names: str) -> pa.Table:
+        for name, order in map(sort_key, names):
+            func = Column.min if order == 'ascending' else Column.max
             if Column.is_list_type(self[name]):
                 self = self.append_column('', getattr(ListChunk, func.__name__)(self[name]))
                 self = Table.filter_list(self, pc.field(name) == pc.field('')).drop([''])
             else:
                 self = self.filter(pc.field(name) == func(self[name]))
         return self
```

### Comparing `graphique-1.1/graphique/inputs.py` & `graphique-1.2/graphique/inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from strawberry import UNSET
 from strawberry.annotation import StrawberryAnnotation
 from strawberry.arguments import StrawberryArgument
 from strawberry.schema_directive import Location
 from strawberry.field import StrawberryField
 from strawberry.scalars import JSON
 from strawberry.types.fields.resolver import StrawberryResolver
+from typing_extensions import Self
 from .core import Agg, ListChunk
 from .scalars import Long
 
 T = TypeVar('T')
 
 
 class links:
@@ -158,25 +159,34 @@
     q: List[float] = (0.5,)  # type: ignore
     interpolation: str = 'linear'
     skip_nulls: bool = True
     min_count: int = 1
 
 
 @strawberry.input
+class Rank(Field):
+    sort_keys: str = 'ascending'
+    null_placement: str = 'at_end'
+    tiebreaker: str = 'first'
+
+
+@strawberry.input
 class Sort:
     by: List[str]
     length: Long
 
 
 @strawberry.input(description=f"[functions]({links.compute}#structural-transforms) for lists")
 class ListFunction(Input):
+    deprecation = "List scalar functions will be moved to `scan(...: {list: ...})`"
+
     filter: 'Expression' = default_field({}, description="filter within list scalars")
-    index: Optional[Index] = default_field(func=pc.index)
-    mode: Optional[Mode] = default_field(func=pc.mode)
-    quantile: Optional[Quantile] = default_field(func=pc.quantile)
+    index: Optional[Index] = default_field(func=pc.index, deprecation_reason=deprecation)
+    mode: Optional[Mode] = default_field(func=pc.mode, deprecation_reason=deprecation)
+    quantile: Optional[Quantile] = default_field(func=pc.quantile, deprecation_reason=deprecation)
 
 
 @strawberry.input(description=f"options for count [aggregation]({links.compute}#aggregations)")
 class CountAggregate(Field):
     mode: str = 'only_valid'
 
 
@@ -395,15 +405,15 @@
             name += '_checked'
         if name.endswith('_'):  # `and_` and `or_` functions differ from operators
             return getattr(operator, name)
         return getattr(pc if hasattr(pc, name) else operator, name)
 
     @classmethod
     @no_type_check
-    def from_query(cls, **queries: Filter) -> 'Expression':
+    def from_query(cls, **queries: Filter) -> Self:
         """Transform query syntax into an Expression input."""
         exprs = []
         for name, query in queries.items():
             field = cls(name=[name])
             exprs += (cls(**{op: [field, cls(value=value)]}) for op, value in dict(query).items())
         return cls(and_=exprs)
```

### Comparing `graphique-1.1/graphique/interface.py` & `graphique-1.2/graphique/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,21 +13,20 @@
 import pyarrow.compute as pc
 import pyarrow.dataset as ds
 import strawberry.asgi
 from strawberry.types import Info
 from typing_extensions import Annotated, Self
 from .core import Column as C, ListChunk, Table as T, sort_key
 from .inputs import CountAggregate, Cumulative, Diff, Expression, Field, Filter
-from .inputs import HashAggregates, ListFunction, Projection, ScalarAggregate, Sort
+from .inputs import HashAggregates, ListFunction, Projection, Rank, ScalarAggregate, Sort
 from .inputs import TDigestAggregate, VarianceAggregate, VectorAggregates, links
 from .models import Column, doc_field, selections
 from .scalars import Long
 
 Root = Union[ds.Dataset, ds.Scanner, pa.Table]
-list_deprecation = "List functions will be moved to `scan(...: {list: ...})`"
 
 
 def references(field) -> Iterator:
     """Generate every possible column reference from strawberry `SelectedField`."""
     if isinstance(field, str):
         yield field.lstrip('-')
     elif isinstance(field, Iterable):
@@ -159,15 +158,18 @@
     @doc_field
     def length(self) -> Long:
         """number of rows"""
         return len(self.table) if hasattr(self.table, '__len__') else self.table.count_rows()
 
     @doc_field
     def any(self, info: Info, length: Long = 1) -> bool:
-        """Provisional: return whether there are at least `length` rows."""
+        """Return whether there are at least `length` rows.
+
+        May be significantly faster than `length` for out-of-core data.
+        """
         table = self.select(info, length)
         return len(table) >= length
 
     @doc_field(
         name="column name(s); multiple names access nested struct fields",
         cast=f"cast array to {links.type}",
         safe="check for conversion errors on cast",
@@ -196,33 +198,42 @@
 
     @doc_field(
         by="column names",
         counts="optionally include counts in an aliased column",
         aggregate="grouped aggregation functions",
     )
     def group(
-        self, info: Info, by: List[str], counts: str = '', aggregate: HashAggregates = {}  # type: ignore
+        self, info: Info, by: List[str] = [], counts: str = '', aggregate: HashAggregates = {}  # type: ignore
     ) -> Self:
         """Return table grouped by columns, with stable ordering.
 
         Columns which are not aggregated are transformed into list columns.
         See `column`, `aggregate`, and `tables` for further usage of list columns.
         """
         scalars, aggs = set(by), dict(aggregate)
         for values in aggs.values():
             scalars.update(agg.alias for agg in values)
         lists = self.references(info, level=1) - scalars - {counts}
-        if isinstance(self.table, pa.Table) or lists or not set(aggs) <= Field.associatives:
+        flat = isinstance(self.table, pa.Table) or not set(aggs) <= Field.associatives
+        aggs['list'] = list(map(Field, lists))
+        if flat:
             table = self.select(info)
-        else:  # scan in parallel when possible
-            table = T.map_batch(self.scanner(info), T.group, *by, counts=counts, **aggs)
+        else:  # scan fragments or batches when possible
+            if set(by) <= set(self.schema().partitioning) > set():
+                table = self.fragments(info, Expression(), counts, aggregate, Expression()).table
+            else:
+                table = T.map_batch(self.scanner(info), T.group, *by, counts=counts, **aggs)
             if counts:
                 aggs.setdefault('sum', []).append(Field(counts))
                 counts = ''
-        return type(self)(T.group(table, *by, counts=counts, list=list(map(Field, lists)), **aggs))
+        table = T.group(table, *by, counts=counts, **aggs)
+        columns = dict(zip(table.column_names, table))
+        if not flat:
+            columns.update({name: ListChunk.inner_flatten(*columns[name].chunks) for name in lists})
+        return type(self)(pa.table(columns))
 
     @doc_field(
         keys="selected fragments",
         counts="optionally include counts in an aliased column",
         aggregate="scalar aggregation functions",
         filter="selected rows (within fragment)",
         columns="projected columns",
@@ -249,16 +260,15 @@
         if sort:
             projection.update({name: ds.field(name) for name in dict(map(sort_key, sort.by))})
         projection.update(self.project(info, columns))
         for name in schema.names:
             projection.pop(name, None)
         columns = collections.defaultdict(list)
         for fragment in self.table.get_fragments(filter=keys.to_arrow()):
-            # TODO(apache/arrow#33825): `get_partition_keys` will be public
-            row = ds._get_partition_keys(fragment.partition_expression)
+            row = ds.get_partition_keys(fragment.partition_expression)
             if projection:
                 table = fragment.to_table(filter=filter, columns=projection)
                 row.update(T.aggregate(table, counts=counts, **aggs))
             elif counts:
                 row[counts] = fragment.count_rows(filter=filter)
             arrays = {name: value for name, value in row.items() if isinstance(value, pa.Array)}
             if sort:
@@ -267,16 +277,15 @@
             for name in row:
                 columns[name].append(row[name])
         for name, values in columns.items():
             if isinstance(values[0], pa.Scalar):
                 columns[name] = C.from_scalars(values)
             elif isinstance(values[0], pa.Array):
                 columns[name] = ListChunk.from_scalars(values)
-        for name, tp in zip(schema.names, schema.types):
-            columns[name] = pa.array(columns[name], tp)
+        columns.update({field.name: pa.array(columns[field.name], field.type) for field in schema})
         return type(self)(pa.table(columns))
 
     @doc_field(
         by="column names",
         diffs="optional inequality predicates; scalars are compared to the adjacent difference",
         counts="optionally include counts in an aliased column",
     )
@@ -290,120 +299,137 @@
         Other columns can be accessed by the `column` field as a `ListColumn`.
         Typically used in conjunction with `aggregate` or `tables`.
         """
         table = self.select(info)
         funcs = {diff.pop('name'): diff for diff in map(dict, diffs)}
         names = list(itertools.takewhile(lambda name: name not in funcs, by))
         predicates = {}
-        for name in by[len(names) :]:  # noqa: E203
+        for name in by[len(names) :]:
             ((func, value),) = funcs.pop(name, {'not_equal': None}).items()
             predicates[name] = (getattr(pc, func),)
             if value is not None:
                 if pa.types.is_timestamp(C.scalar_type(table[name])):
                     value = timedelta(seconds=value)
                 predicates[name] += (value,)
         table, counts_ = T.partition(table, *names, **predicates)
         return type(self)(table.append_column(counts, counts_) if counts else table)
 
     @doc_field(
         by="column names; prefix with `-` for descending order",
         length="maximum number of rows to return; may be significantly faster but is unstable",
+        null_placement="where nulls in input should be sorted; incompatible with `length`",
     )
-    def sort(self, info: Info, by: List[str], length: Optional[Long] = None) -> Self:
+    def sort(
+        self,
+        info: Info,
+        by: List[str],
+        length: Optional[Long] = None,
+        null_placement: str = 'at_end',
+    ) -> Self:
         """Return table slice sorted by specified columns.
 
-        Sorting on list columns will sort within scalars, all of which must have the same lengths.
+        Optimized for length == 1; matches min or max values.
+        Pending deprecation: sorting on list columns will sort within scalars, all of which must have the same lengths.
         """
-        table = self.select(info)
+        if length == 1:
+            self = self.min_max(info, by).slice(info, length=length)
+        table = self.table
+        schema = table.projected_schema if isinstance(table, ds.Scanner) else table.schema
         scalars, lists = [], []  # type: ignore
         for key in by:
-            (lists if C.is_list_type(table[key.lstrip('-')]) else scalars).append(key)
+            (lists if C.is_list_type(schema.field(key.lstrip('-'))) else scalars).append(key)
+        if not scalars or isinstance(table, pa.Table) or length is None:
+            table = self.select(info)
+        else:
+            kwargs = dict(length=length, null_placement=null_placement)
+            table = T.map_batch(
+                self.scanner(info), lambda b: b.take(T.sort_indices(b, *scalars, **kwargs))
+            )
         if scalars:
-            table = T.sort(table, *scalars, length=length)
+            table = T.sort(table, *scalars, length=length, null_placement=null_placement)
         if lists:
-            table = T.sort_list(table, *lists, length=length)
+            table = T.sort_list(table, *lists, length=length, null_placement=null_placement)
         return type(self)(table)
 
-    def min_max(self, info: Info, by: List[str], func: Callable) -> Self:
-        table, name = self.table, by[0]
+    def min_max(self, info: Info, by: List[str]) -> Self:
+        table, (name, order) = self.table, sort_key(by[0])
+        func = C.min if order == 'ascending' else C.max
         schema = table.projected_schema if isinstance(table, ds.Scanner) else table.schema
         if isinstance(table, pa.Table) or C.is_list_type(schema.field(name)):
             table = self.select(info)
-        elif getattr(table, 'partitioning', None) and name in table.partitioning.schema.names:
+        elif name in self.schema().partitioning:
             values = pa.array(
-                ds._get_partition_keys(fragment.partition_expression)[name]
+                ds.get_partition_keys(fragment.partition_expression)[name]
                 for fragment in table.get_fragments()
             )
             scanner = self.scanner(info, filter=ds.field(name) == func(values))
             if len(by) == 1:
                 return type(self)(scanner)
             table, by = scanner.to_table(), by[1:]
         else:
-            # TODO(ARROW-16212): replace with user defined function for multiple kernels
-            batches = self.scanner(info).to_batches()
-            table = pa.Table.from_batches(
-                batch.filter(pc.equal(batch[name], func(batch[name]))) for batch in batches
-            )
-        return type(self)(T.matched(table, func, *by))
+            scanner = self.scanner(info)
+            table = T.map_batch(scanner, lambda b: b.filter(pc.equal(b[name], func(b[name]))))
+        return type(self)(T.min_max(table, *by))
 
     @doc_field(by="column names")
     def min(self, info: Info, by: List[str]) -> Self:
-        """Return table with minimum values per column."""
-        return self.min_max(info, by, C.min)
+        """Pending deprecation: return table with minimum values per column."""
+        return self.min_max(info, by)
 
     @doc_field(by="column names")
     def max(self, info: Info, by: List[str]) -> Self:
-        """Return table with maximum values per column."""
-        return self.min_max(info, by, C.max)
+        """Pending deprecation: return table with maximum values per column."""
+        return self.min_max(info, ['-' + name for name in by])
 
     @doc_field
     @no_type_check
     def apply(
         self,
         info: Info,
         cumulative_sum: doc_argument(List[Cumulative], func=pc.cumulative_sum) = [],
         fill_null_backward: doc_argument(List[Field], func=pc.fill_null_backward) = [],
         fill_null_forward: doc_argument(List[Field], func=pc.fill_null_forward) = [],
+        rank: doc_argument(List[Rank], func=pc.rank) = [],
         list: Annotated[
-            List[ListFunction], strawberry.argument(deprecation_reason=list_deprecation)
+            List[ListFunction], strawberry.argument(description="Functions for list arrays.")
         ] = [],
     ) -> Self:
         """Return view of table with vector functions applied across columns.
 
-        Applied function load arrays into memory as needed. See `scan` for scalar functions,
+        Applied functions load arrays into memory as needed. See `scan` for scalar functions,
         which do not require loading.
         """
         table = self.select(info)
         columns = {}
         for value in map(dict, list):
             expr = value.pop('filter').to_arrow()
             if expr is not None:
                 table = T.filter_list(table, expr)
             for func, field in value.items():
                 columns[field.alias] = getattr(ListChunk, func)(table[field.name], **field.options)
-        args = cumulative_sum, fill_null_backward, fill_null_forward
-        funcs = pc.cumulative_sum, C.fill_null_backward, C.fill_null_forward
+        args = cumulative_sum, fill_null_backward, fill_null_forward, rank
+        funcs = pc.cumulative_sum, C.fill_null_backward, C.fill_null_forward, pc.rank
         for fields, func in zip(args, funcs):
             for field in fields:
                 columns[field.alias] = func(table[field.name], **field.options)
         return type(self)(T.union(table, pa.table(columns)))
 
     @doc_field
     def tables(self, info: Info) -> List[Self]:  # type: ignore
         """Return a list of tables by splitting list columns.
 
         At least one list column must be referenced, and all list columns must have the same lengths.
         """
-        table = self.select(info)
-        lists = {name for name in table.column_names if C.is_list_type(table[name])}
-        scalars = set(table.column_names) - lists
-        for index, count in enumerate(T.list_value_length(table).to_pylist()):
-            row = {name: pa.repeat(table[name][index], count) for name in scalars}
-            row.update({name: table[name][index].values for name in lists})
-            yield type(self)(pa.table(row))
+        for batch in self.scanner(info).to_batches():
+            lists = T.list_fields(batch)
+            scalars = set(batch.schema.names) - lists
+            for index, count in enumerate(T.list_value_length(batch).to_pylist()):
+                row = {name: pa.repeat(batch[name][index], count) for name in scalars}
+                row.update({name: batch[name][index].values for name in lists})
+                yield type(self)(pa.table(row))
 
     @doc_field
     def aggregate(
         self,
         info: Info,
         approximate_median: doc_argument(List[ScalarAggregate], func=pc.approximate_median) = [],
         count: doc_argument(List[CountAggregate], func=pc.count) = [],
@@ -433,20 +459,20 @@
             func = getattr(ListChunk, key, None)
             for agg in locals()[key]:
                 if func is None or key == 'sum':  # `sum` is a method on `Array``
                     agg_fields[agg.name][key] = agg
                 else:
                     columns[agg.alias] = func(table[agg.name], **agg.options)
         for name, aggs in agg_fields.items():
-            funcs = {key: agg.astuple(key)[1] for key, agg in aggs.items()}
-            arrays = ListChunk.aggregate(table[name], **funcs).flatten()
-            columns.update(zip([agg.alias for agg in aggs.values()], arrays))
+            funcs = {key: agg.astuple(key)[-1] for key, agg in aggs.items()}
+            batch = ListChunk.aggregate(table[name], **funcs)
+            columns.update(zip([agg.alias for agg in aggs.values()], batch))
         return type(self)(pa.table(columns))
 
-    aggregate.deprecation_reason = list_deprecation
+    aggregate.deprecation_reason = ListFunction.deprecation
 
     def project(self, info: Info, columns: List[Projection]) -> dict:
         """Return projected columns, including all references from below fields."""
         projection = {name: pc.field(name) for name in self.references(info, level=1)}
         projection.update({col.alias or '.'.join(col.name): col.to_arrow() for col in columns})
         if '' in projection:
             raise ValueError(f"projected columns need a name or alias: {projection['']}")
@@ -454,22 +480,24 @@
 
     @doc_field(filter="selected rows", columns="projected columns")
     def scan(
         self, info: Info, filter: Expression = {}, columns: List[Projection] = []  # type: ignore
     ) -> Self:
         """Select rows and project columns without memory usage."""
         scanner = self.scanner(info, filter=filter.to_arrow(), columns=self.project(info, columns))
-        oneshot = len(selections(*info.selected_fields)) > 1 and isinstance(self.table, ds.Scanner)
+        selected = selections(*info.selected_fields)
+        selected['type'] = selected['schema'] = 0
+        oneshot = sum(selected.values()) > 1 and isinstance(self.table, ds.Scanner)
         return type(self)(scanner.to_table() if oneshot else scanner)
 
     @doc_field(
         right="name of right table; must be on root Query type",
         keys="column names used as keys on the left side",
         right_keys="column names used as keys on the right side; defaults to left side.",
-        join_type="""the kind of join: “left semi”, “right semi”, “left anti”, “right anti”, “inner”, “left outer”, “right outer”, “full outer”""",
+        join_type="the kind of join: 'left semi', 'right semi', 'left anti', 'right anti', 'inner', 'left outer', 'right outer', 'full outer'",
         left_suffix="add suffix to left column names; for preventing collisions",
         right_suffix="add suffix to right column names; for preventing collisions.",
         coalesce_keys="omit duplicate keys",
     )
     def join(
         self,
         info: Info,
@@ -495,9 +523,9 @@
             right_suffix=right_suffix,
             coalesce_keys=coalesce_keys,
         )
         return type(self)(table)
 
     @doc_field
     def take(self, info: Info, indices: List[Long]) -> Self:
-        """Provisional: select rows from indices."""
+        """Select rows from indices."""
         return type(self)(self.scanner(info).take(indices))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `graphique-1.1/graphique/middleware.py` & `graphique-1.2/graphique/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 """
 ASGI GraphQL utilities.
 """
 from datetime import datetime
-from typing import Iterable, Mapping, Optional, Union
-import pyarrow as pa
+from typing import Iterable, Mapping, Optional
 import pyarrow.dataset as ds
 import strawberry.asgi
 from strawberry import UNSET
 from strawberry.utils.str_converters import to_camel_case
 from strawberry.types import Info
 from .core import Column as C
 from .inputs import Filter
-from .interface import Dataset
+from .interface import Dataset, Root
 from .models import Column, doc_field
 from .scalars import Long, scalar_map, type_map
 
-Root = Union[ds.Dataset, ds.Scanner, pa.Table]
 
-
-class TimingExtension(strawberry.extensions.Extension):
-    def on_request_start(self):
-        self.start = datetime.now()
-
-    def on_request_end(self):
+class TimingExtension(strawberry.extensions.SchemaExtension):
+    def on_operation(self):
+        start = datetime.now()
+        yield
         end = datetime.now()
-        print(f"[{end.replace(microsecond=0)}]: {end - self.start}")
+        print(f"[{end.replace(microsecond=0)}]: {end - start}")
 
 
 class GraphQL(strawberry.asgi.GraphQL):
     """ASGI GraphQL app with root value(s).
 
     Args:
         root: root dataset to attach as the Query type
         debug: enable timing extension
+        extensions: schema extensions
         **kwargs: additional `asgi.GraphQL` options
     """
 
     options = dict(types=Column.registry.values(), scalar_overrides=scalar_map)
 
-    def __init__(self, root: Root, debug: bool = False, **kwargs):
-        options = dict(self.options, extensions=[TimingExtension] * bool(debug))
+    def __init__(self, root: Root, debug: bool = False, extensions: list = [], **kwargs):
+        options = dict(self.options, extensions=extensions + [TimingExtension][: bool(debug)])
         if type(root).__name__ == 'Query':
             self.root_value = root
             options['enable_federation_2'] = True  # type: ignore
             schema = strawberry.federation.Schema(type(self.root_value), **options)
         else:
             self.root_value = implemented(root)
             schema = strawberry.Schema(type(self.root_value), **options)
```

### Comparing `graphique-1.1/graphique/models.py` & `graphique-1.2/graphique/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 GraphQL output types and resolvers.
 """
+import collections
 import functools
 import inspect
 import itertools
 import operator
 from datetime import date, datetime, time, timedelta
 from decimal import Decimal
 from typing import Callable, Generic, List, Optional, TypeVar, TYPE_CHECKING
@@ -29,17 +30,17 @@
     for selection in field.selections:
         if hasattr(selection, 'name'):
             yield selection.name
         else:
             yield from _selections(selection)
 
 
-def selections(*fields) -> set:
-    """Return set of field name selections from strawberry `SelectedField`."""
-    return set(itertools.chain(*map(_selections, fields)))
+def selections(*fields) -> dict:
+    """Return counts of field name selections from strawberry `SelectedField`."""
+    return collections.Counter(itertools.chain(*map(_selections, fields)))
 
 
 def doc_field(func: Optional[Callable] = None, **kwargs: str) -> StrawberryField:
     """Return strawberry field with argument and docstring descriptions."""
     if func is None:
         return functools.partial(doc_field, **kwargs)
     for name in kwargs:
@@ -241,15 +242,15 @@
 @operator.methodcaller('register', Long, description="column of longs")
 @strawberry.type(name='Column')
 class IntColumn(RatioColumn[T]):
     @doc_field
     def take_from(
         self, info: Info, field: str
     ) -> Annotated['Dataset', strawberry.lazy('.interface')]:
-        """Provisional: select indices from a table on the root Query type."""
+        """Select indices from a table on the root Query type."""
         root = getattr(info.root_value, field)
         return type(root)(root.scanner(info).take(self.array.combine_chunks()))
 
 
 @strawberry.type(description="column of lists")
 class ListColumn(Column):
     @doc_field
```

### Comparing `graphique-1.1/graphique/scalars.py` & `graphique-1.2/graphique/scalars.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     if isinstance(value, int):
         return value
     raise TypeError(f"Long cannot represent value: {value}")
 
 
 @strawberry.type(description="month day nano interval")
 class Interval:
-    months: int = 0
-    days: int = 0
-    nanoseconds: 'Long' = 0  # type: ignore
+    months: int
+    days: int
+    nanoseconds: 'Long'  # type: ignore
 
 
 Long = strawberry.scalar(int, name='Long', description="64-bit int", parse_value=parse_long)
 Duration = strawberry.scalar(  # pragma: no branch
     timedelta,
     name='Duration',
     description="duration float (in seconds)",
```

### Comparing `graphique-1.1/graphique.egg-info/PKG-INFO` & `graphique-1.2/graphique.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphique
-Version: 1.1
+Version: 1.2
 Summary: GraphQL service for arrow tables and parquet data sets.
 Author-email: Aric Coady <aric.coady@gmail.com>
 License: Copyright 2022 Aric Coady
         
            Licensed under the Apache License, Version 2.0 (the "License");
            you may not use this file except in compliance with the License.
            You may obtain a copy of the License at
@@ -84,15 +84,15 @@
 app = GraphQL(ds.dataset(...))  # Table is root query type
 app = GraphQL.federated({<name>: ds.dataset(...), ...}, keys={...})  # Tables on federated fields
 ```
 
 Start like any ASGI app.
 
 ```console
-uvicorn <package>:app
+uvicorn <module>:app
 ```
 
 Configuration options exist to provide a convenient no-code solution, but are subject to change in the future. Using a custom app is recommended for production usage.
 
 ### API
 #### types
 * `Dataset`: interface for an arrow dataset, scanner, or table.
@@ -134,32 +134,39 @@
 
 ## Installation
 ```console
 % pip install graphique[server]
 ```
 
 ## Dependencies
-* pyarrow >=11
-* strawberry-graphql[asgi,cli] >=0.149.2
+* pyarrow >=12
+* strawberry-graphql[asgi,cli]
 * uvicorn (or other [ASGI server](https://asgi.readthedocs.io/en/latest/implementations.html))
 
 ## Tests
 100% branch coverage.
 
 ```console
 % pytest [--cov]
 ```
 
 ## Changes
+1.2
+
+* Pyarrow >=12 required
+* Grouping fragments optimized
+* Group by empty columns
+* Batch sorting and grouping into lists
+
 1.1
 
 * Pyarrow >=11 required
 * Python >=3.8 required
 * Scannable functions added
-* List aggregations deprecaated
+* List aggregations deprecated
 * Group by fragments
 * Month day nano interval array
 * `min` and `max` fields memory optimized
 
 1.0
 
 * Pyarrow >=10 required
@@ -222,13 +229,13 @@
 
 * Pyarrow >=3 required
 * `any` and `all` fields
 * String column `split` field
 
 0.2
 
+* Pyarrow >= 2 required
 * `ListColumn` and `StructColumn` types
 * `Groups` type with `aggregate` field
 * `group` and `unique` optimized
-* pyarrow >= 2 required
 * Statistical fields: `mode`, `stddev`, `variance`
 * `is_in`, `min`, and `max` optimized
```

### Comparing `graphique-1.1/pyproject.toml` & `graphique-1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Database :: Database Engines/Servers",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
-dependencies = ["pyarrow>=11", "strawberry-graphql[asgi,cli]>=0.149.2"]
+dependencies = ["pyarrow>=12", "strawberry-graphql[asgi,cli]>=0.160"]
 
 [project.urls]
 Homepage = "https://github.com/coady/graphique"
 Documentation = "https://coady.github.io/graphique"
 
 [project.optional-dependencies]
 server = ["uvicorn[standard]"]
@@ -46,14 +46,17 @@
 [tool.setuptools.package-data]
 graphique = ["py.typed"]
 
 [tool.black]
 line-length = 100
 skip-string-normalization = true
 
+[tool.ruff]
+ignore = ["E501"]
+
 [[tool.mypy.overrides]]
 module = ["pyarrow.*", "strawberry.*", "starlette.*"]
 ignore_missing_imports = true
 
 [tool.coverage.run]
 source = ["graphique"]
 branch = true
```

