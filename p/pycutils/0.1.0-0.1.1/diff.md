# Comparing `tmp/pycutils-0.1.0.tar.gz` & `tmp/pycutils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycutils-0.1.0.tar", last modified: Fri Apr 21 15:45:33 2023, max compression
+gzip compressed data, was "pycutils-0.1.1.tar", last modified: Sun May  7 20:42:34 2023, max compression
```

## Comparing `pycutils-0.1.0.tar` & `pycutils-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-21 15:45:33.437397 pycutils-0.1.0/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1023 2023-04-21 15:45:33.437681 pycutils-0.1.0/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)      552 2023-04-19 15:24:24.000000 pycutils-0.1.0/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      238 2023-04-19 15:24:24.000000 pycutils-0.1.0/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      660 2023-04-21 15:45:33.438733 pycutils-0.1.0/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-21 15:45:33.429602 pycutils-0.1.0/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-21 15:45:33.433644 pycutils-0.1.0/src/cutils/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       27 2023-04-19 15:24:25.000000 pycutils-0.1.0/src/cutils/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     8373 2023-04-21 15:41:26.000000 pycutils-0.1.0/src/cutils/cutils.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2022-04-12 16:00:10.000000 pycutils-0.1.0/src/cutils/py.typed
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-21 15:45:33.435997 pycutils-0.1.0/src/pycutils.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1023 2023-04-21 15:45:33.000000 pycutils-0.1.0/src/pycutils.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)      263 2023-04-21 15:45:33.000000 pycutils-0.1.0/src/pycutils.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-21 15:45:33.000000 pycutils-0.1.0/src/pycutils.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        7 2023-04-21 15:45:33.000000 pycutils-0.1.0/src/pycutils.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-21 15:45:33.436689 pycutils-0.1.0/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1754 2023-04-21 15:44:37.000000 pycutils-0.1.0/tests/test_cutils.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 20:42:34.519502 pycutils-0.1.1/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1078 2023-05-06 22:36:10.000000 pycutils-0.1.1/LICENSE
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1817 2023-05-07 20:42:34.519713 pycutils-0.1.1/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1324 2023-05-06 22:44:57.000000 pycutils-0.1.1/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      261 2023-05-06 22:41:03.000000 pycutils-0.1.1/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      660 2023-05-07 20:42:34.520452 pycutils-0.1.1/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 20:42:34.511362 pycutils-0.1.1/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 20:42:34.515359 pycutils-0.1.1/src/cutils/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       27 2023-05-05 02:42:28.000000 pycutils-0.1.1/src/cutils/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     8651 2023-05-05 02:42:28.000000 pycutils-0.1.1/src/cutils/cutils.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2022-04-12 16:00:10.000000 pycutils-0.1.1/src/cutils/py.typed
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 20:42:34.518277 pycutils-0.1.1/src/pycutils.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1817 2023-05-07 20:42:34.000000 pycutils-0.1.1/src/pycutils.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      271 2023-05-07 20:42:34.000000 pycutils-0.1.1/src/pycutils.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-05-07 20:42:34.000000 pycutils-0.1.1/src/pycutils.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        7 2023-05-07 20:42:34.000000 pycutils-0.1.1/src/pycutils.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-07 20:42:34.518909 pycutils-0.1.1/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1936 2023-05-07 20:36:34.000000 pycutils-0.1.1/tests/test_cutils.py
```

### Comparing `pycutils-0.1.0/setup.cfg` & `pycutils-0.1.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pycutils
-version = 0.1.0
+version = 0.1.1
 author = Cangyuan Li
 author_email = everest229@gmail.com
 description = A list of python utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CangyuanLi/cutils
 project_urls =
```

### Comparing `pycutils-0.1.0/src/cutils/cutils.py` & `pycutils-0.1.1/src/cutils/cutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # Imports
 
 import abc
+import concurrent.futures
 from collections.abc import Callable, Generator, Iterable, MutableMapping, Sequence
 from dataclasses import dataclass
 import functools
 import math
 import random
 import re
 import statistics
 import time
 import threading
-from typing import Any, Protocol, TypeVar, Union
+from typing import Any, Literal, Protocol, Union
 
 # Types
 
 Real = Union[int, float]
 
+ParallelOption = Literal["process", "thread"]
+
 
 class Comparable(Protocol):
     @abc.abstractmethod
     def __lt__(self, other) -> bool:
         pass
 
 
@@ -44,17 +47,18 @@
     Args:
         source (Iterable): arg 1
         query (Iterable): arg 2
 
     Returns:
         bool: True if arg 1 contains an element of arg 2
     """
-    # Note that this method seems to be, on average, faster than using any(). any() can be faster
-    # in the case that no elements of the query are in the source, but the difference is negligeble.
-    # However, in the case that elements of the query are in the source, this method is much faster.
+    # Note that this method seems to be, on average, faster than using any().
+    # any() can be faster in the case that no elements of the query are in the source,
+    # but the difference is negligeble. However, in the case that elements of the query
+    # are in the source, this method is much faster.
     for i in query:
         if i in source:
             return True
 
     return False
 
 
@@ -257,15 +261,16 @@
     should be run, ex:
         cutils.time_func(lambda: time.sleep(1), 100)
     will run time.sleep(1) 100 times.
 
     Args:
         func (Callable): Any function
         iterations (int, optional): Number of times to run func. Defaults to 1.
-        warmups (int, optional): Number of times to run func before timing. Defaults to 0.
+        warmups (int, optional): Number of times to run func before timing.
+            Defaults to 0.
         quiet (bool, optional): Whether to print stats. Defaults to False.
 
     Returns:
         TimeFuncRes: (average, min, max, sd, total, list of raw times)
     """
     for _ in range(warmups):
         func()
@@ -331,7 +336,12 @@
             finally:
                 last_time_called = time.perf_counter()
                 lock.release()
 
         return rate_limited_function
 
     return decorate
+
+
+def run_parallel(func: Callable, iterable: Iterable, *args, **kwargs):
+    with concurrent.futures.ProcessPoolExecutor(*args, **kwargs) as pool:
+        return pool.map(func, iterable)
```

### Comparing `pycutils-0.1.0/tests/test_cutils.py` & `pycutils-0.1.1/tests/test_cutils.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,18 +44,28 @@
         cutils.find_last_index(test_list, 3)
 
 
 def test_flatten():
     test_list = [[1], [2], "ab", 3]
     assert cutils.flatten(test_list) == [1, 2, "ab", 3]
 
+    test_list = [[[[[[[1]]]]]]]
+    assert cutils.flatten(test_list) == [1]
+
+
+def test_flatten_dict():
+    pass
+
 
 def test_get_factors():
     assert cutils.get_factors(10) == {2, 5, 1, 10}
 
+    with pytest.raises(ValueError):
+        cutils.get_factors(1.1)
+
 
 def test_ordered_unique():
     assert cutils.ordered_unique("abbcb") == ["a", "b", "c"]
 
 
 def test_strip_blanks():
     assert cutils.strip_blanks("a   bc\u2009") == "abc"
```

