# Comparing `tmp/relib-0.2.4-py3-none-any.whl.zip` & `tmp/relib-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7898 bytes, number of entries: 10
--rw-r--r--  2.0 unx      309 b- defN 23-Mar-08 16:24 relib/__init__.py
+Zip file size: 8200 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      409 b- defN 23-May-07 12:15 relib/__init__.py
 -rw-r--r--  2.0 unx     8943 b- defN 23-Jan-21 17:58 relib/hashing.py
 -rw-r--r--  2.0 unx      555 b- defN 23-Jan-21 18:12 relib/measure_duration.py
 -rw-r--r--  2.0 unx     1905 b- defN 23-Jan-21 17:58 relib/raypipe.py
--rw-r--r--  2.0 unx     3002 b- defN 23-Mar-08 16:38 relib/utils.py
--rw-r--r--  2.0 unx     1054 b- defN 23-Mar-08 16:38 relib-0.2.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      260 b- defN 23-Mar-08 16:38 relib-0.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-08 16:38 relib-0.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-08 16:38 relib-0.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      749 b- defN 23-Mar-08 16:38 relib-0.2.4.dist-info/RECORD
-10 files, 16875 bytes uncompressed, 6634 bytes compressed:  60.7%
+-rw-r--r--  2.0 unx     3963 b- defN 23-May-07 12:20 relib/utils.py
+-rw-r--r--  2.0 unx     1054 b- defN 23-May-07 12:20 relib-1.0.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      304 b- defN 23-May-07 12:20 relib-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-07 12:20 relib-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-07 12:20 relib-1.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      749 b- defN 23-May-07 12:20 relib-1.0.0.dist-info/RECORD
+10 files, 17980 bytes uncompressed, 6936 bytes compressed:  61.4%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: relib/raypipe.py
 Comment: 
 
 Filename: relib/utils.py
 Comment: 
 
-Filename: relib-0.2.4.dist-info/LICENSE.txt
+Filename: relib-1.0.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: relib-0.2.4.dist-info/METADATA
+Filename: relib-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: relib-0.2.4.dist-info/WHEEL
+Filename: relib-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: relib-0.2.4.dist-info/top_level.txt
+Filename: relib-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: relib-0.2.4.dist-info/RECORD
+Filename: relib-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## relib/__init__.py

```diff
@@ -1,5 +1,25 @@
-from .utils import list_split, drop_none, distinct, find, transpose_dict, make_combinations_by_dict, \
-  merge_dicts, intersect, ensure_tuple, omit, dict_by, tuple_by, flatten, transpose, deepen_dict, group
+from .utils import (
+  list_split,
+  drop_none,
+  distinct,
+  find,
+  transpose_dict,
+  make_combinations_by_dict,
+  merge_dicts,
+  intersect,
+  ensure_tuple,
+  omit,
+  dict_by,
+  tuple_by,
+  flatten,
+  transpose,
+  deepen_dict,
+  group,
+  sized_partitions,
+  num_partitions,
+  StrFilter,
+  str_filterer,
+)
 from .raypipe import raypipe
 from .hashing import hash
 from .measure_duration import measure_duration
```

## relib/utils.py

```diff
@@ -1,21 +1,21 @@
-from typing import TypeVar, Union, Iterable, Any
+from typing import TypeVar, Union, Iterable, Callable
+import re
 
 T = TypeVar('T')
 U = TypeVar('U')
 
 def list_split(l: list[T], sep: T) -> list[list[T]]:
   l = [sep, *l, sep]
   split_at = [i for i, x in enumerate(l) if x is sep]
   ranges = list(zip(split_at[0:-1], split_at[1:]))
-  result: Any = [
+  return [
     l[start + 1:end]
     for start, end in ranges
   ]
-  return result
 
 def drop_none(l: Iterable[Union[T, None]]) -> list[T]:
   return [x for x in l if x is not None]
 
 def distinct(items: Iterable[T]) -> list[T]:
   return list(set(items))
 
@@ -109,7 +109,34 @@
 def get_at(d, keys, default):
   try:
     for key in keys:
       d = d[key]
   except KeyError:
     return default
   return d
+
+def sized_partitions(values: Iterable[T], part_size: int) -> list[list[T]]:
+  if not isinstance(values, list):
+    values = list(values)
+  num_parts = (len(values) / part_size).__ceil__()
+  return [values[i * part_size : (i + 1) * part_size] for i in range(num_parts)]
+
+def num_partitions(values: Iterable[T], num_parts: int) -> list[list[T]]:
+  if not isinstance(values, list):
+    values = list(values)
+  part_size = (len(values) / num_parts).__ceil__()
+  return [values[i * part_size : (i + 1) * part_size] for i in range(num_parts)]
+
+StrFilter = Callable[[str], bool]
+
+def str_filterer(
+  include_patterns: list[re.Pattern[str]] = [],
+  exclude_patterns: list[re.Pattern[str]] = [],
+) -> StrFilter:
+  def str_filter(string: str) -> bool:
+    if any(pattern.search(string) for pattern in exclude_patterns):
+      return False
+    if not include_patterns:
+      return True
+    return any(pattern.search(string) for pattern in include_patterns)
+
+  return str_filter
```

## Comparing `relib-0.2.4.dist-info/LICENSE.txt` & `relib-1.0.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

