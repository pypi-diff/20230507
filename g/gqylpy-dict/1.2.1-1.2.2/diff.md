# Comparing `tmp/gqylpy_dict-1.2.1.tar.gz` & `tmp/gqylpy_dict-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gqylpy_dict-1.2.1.tar", last modified: Sat Apr 29 02:25:21 2023, max compression
+gzip compressed data, was "gqylpy_dict-1.2.2.tar", last modified: Sun May  7 08:22:57 2023, max compression
```

## Comparing `gqylpy_dict-1.2.1.tar` & `gqylpy_dict-1.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:25:21.751060 gqylpy_dict-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    12343 2023-04-29 02:25:08.000000 gqylpy_dict-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-29 02:25:08.000000 gqylpy_dict-1.2.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-29 02:25:21.747060 gqylpy_dict-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-29 02:25:08.000000 gqylpy_dict-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:25:21.747060 gqylpy_dict-1.2.1/gqylpy_dict/
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-04-29 02:25:08.000000 gqylpy_dict-1.2.1/gqylpy_dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-04-29 02:25:08.000000 gqylpy_dict-1.2.1/gqylpy_dict/g dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 02:25:21.747060 gqylpy_dict-1.2.1/gqylpy_dict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-29 02:25:21.000000 gqylpy_dict-1.2.1/gqylpy_dict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-29 02:25:21.000000 gqylpy_dict-1.2.1/gqylpy_dict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 02:25:21.000000 gqylpy_dict-1.2.1/gqylpy_dict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-29 02:25:21.000000 gqylpy_dict-1.2.1/gqylpy_dict.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 02:25:21.751060 gqylpy_dict-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-29 02:25:09.000000 gqylpy_dict-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:22:57.212764 gqylpy_dict-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12343 2023-05-07 08:22:46.000000 gqylpy_dict-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-07 08:22:46.000000 gqylpy_dict-1.2.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-07 08:22:57.212764 gqylpy_dict-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-07 08:22:46.000000 gqylpy_dict-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:22:57.208764 gqylpy_dict-1.2.2/gqylpy_dict/
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-05-07 08:22:46.000000 gqylpy_dict-1.2.2/gqylpy_dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-05-07 08:22:46.000000 gqylpy_dict-1.2.2/gqylpy_dict/g dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:22:57.208764 gqylpy_dict-1.2.2/gqylpy_dict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-07 08:22:57.000000 gqylpy_dict-1.2.2/gqylpy_dict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-07 08:22:57.000000 gqylpy_dict-1.2.2/gqylpy_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 08:22:57.000000 gqylpy_dict-1.2.2/gqylpy_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 08:22:57.000000 gqylpy_dict-1.2.2/gqylpy_dict.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 08:22:57.212764 gqylpy_dict-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-07 08:22:46.000000 gqylpy_dict-1.2.2/setup.py
```

### Comparing `gqylpy_dict-1.2.1/LICENSE` & `gqylpy_dict-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gqylpy_dict-1.2.1/NOTICE` & `gqylpy_dict-1.2.2/NOTICE`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 gqylpy-dict is released under the dual license WTFPL and Apache-2.0.
 
 ────────────────────────────────────────────────────────────────────────────────
 
-Lines 51-95 in the "gqylpy_dict/g dict.py" file are licensed under Apache-2.0:
+Lines 51-96 in the "gqylpy_dict/g dict.py" file are licensed under Apache-2.0:
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `gqylpy_dict-1.2.1/PKG-INFO` & `gqylpy_dict-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gqylpy_dict
-Version: 1.2.1
+Version: 1.2.2
 Summary: 基于内置 dict，它是对内置 dict 的增强。内置 dict 能做的它都能做，内置 dict 不能做的它更能做。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: WTFPL,Apache-2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-dict
 Classifier: Environment :: Web Environment
```

### Comparing `gqylpy_dict-1.2.1/README.md` & `gqylpy_dict-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `gqylpy_dict-1.2.1/gqylpy_dict/__init__.py` & `gqylpy_dict-1.2.2/gqylpy_dict/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     >>> x = gdict(x)
     >>> x.a[0].b
     'B'
 
     >>> x.deepget('a[0].b')
     'B'
 
-    @version: 1.2.1
+    @version: 1.2.2
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/gqylpy-dict
 
 ────────────────────────────────────────────────────────────────────────────────
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 This file is licensed under the WTFPL:
@@ -47,27 +47,27 @@
 
 class gdict(dict):
 
     def __new__(cls, __data__={}, /, **data):
         if isinstance(__data__, dict):
             return dict.__new__(cls)
 
-        if isinstance(__data__, (list, tuple, set, frozenset)):
+        if isinstance(__data__, (list, tuple)):
             return __data__.__class__(cls(v) for v in __data__)
 
         return __data__
 
     def __init__(self, __data__=None, /, **data):
         if __data__ is None:
             __data__ = data
         else:
             __data__.update(data)
 
         for key, value in __data__.items():
-            dict.__setitem__(self, key, gdict(value))
+            self[key] = value
 
     def __getattr__(self, key: str, /) -> Any:
         return self[key]
 
     def __setattr__(self, key: str, value: Any, /) -> None:
         self[key] = value
 
@@ -93,18 +93,17 @@
     def copy(self) -> 'gdict':
         """Get a replica instance."""
 
     def deepcopy(self) -> 'gdict':
         """
         Incomplete deep copy, NOTE not the same as `copy.deepcopy`!
 
-        Copy only the instances of container types (only instances of `dict`,
-        `gdict`, `list`, `tuple`, `set`, and `frozenset`). Just pass `self`
-        directly to `gdict`, you can view the code blocks for `gdict.__new__`
-        and `gdict.__init__`.
+        Copy only the instances of container types (only instances of `gdict`,
+        `dict`, `list` and `tuple`). Just pass `self` directly to `gdict`, you
+        can view the code blocks for `gdict.__new__` and `gdict.__init__`.
 
         Backstory https://github.com/gqylpy/gqylpy-dict/issues/9
         """
         return gdict(self)
 
     def deepget(
             self,
```

### Comparing `gqylpy_dict-1.2.1/gqylpy_dict/g dict.py` & `gqylpy_dict-1.2.2/gqylpy_dict/g dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 ────────────────────────────────────────────────────────────────────────────────
 
-Lines 51 through 95 is licensed under the Apache-2.0:
+Lines 51 through 96 is licensed under the Apache-2.0:
 
     Licensed under the Apache License, Version 2.0 (the "License");
     you may not use this file except in compliance with the License.
     You may obtain a copy of the License at
 
         https://www.apache.org/licenses/LICENSE-2.0
 
@@ -66,16 +66,17 @@
         if not isinstance(__masquerade_class__, type):
             raise TypeError('"__masquerade_class__" is not a class.')
 
         cls = type.__new__(
             mcs, __masquerade_class__.__name__, __bases__, __dict__
         )
 
-        mcs.__name__ = type.__name__
-        cls.__module__ = __masquerade_class__.__module__
+        mcs.__name__     = type.__name__
+        mcs.__qualname__ = type.__qualname__
+        cls.__module__   = __masquerade_class__.__module__
 
         # cls.__qualname__ = __masquerade_class__.__qualname__
         # Warning: Modify this attribute will cannot create the portable
         # serialized representation.
 
         if getattr(builtins, __masquerade_class__.__name__, None) is \
                 __masquerade_class__:
@@ -93,30 +94,35 @@
 
 
 builtins.MasqueradeClass = MasqueradeClass
 
 
 class GqylpyDict(dict, metaclass=MasqueradeClass):
     __masquerade_class__ = dict
-    __slots__ = ()
+
+    # __slots__ = ()
+    # ChatGPT-3.5 argues that the use of `__slots__` here is not very necessary
+    # and may cause some small performance loss. After preliminary analysis, we
+    # think what ChatGPT said may be correct. We will comment it out first and
+    # follow up later.
 
     def __init__(self, __data__=None, /, **data):
         if __data__ is None:
             __data__ = data
         else:
             __data__.update(data)
 
         for name, value in __data__.items():
-            dict.__setitem__(self, name, GqylpyDict(value))
+            self[name] = value
 
     def __new__(cls, __data__={}, /, **data):
         if isinstance(__data__, dict):
             return dict.__new__(cls)
 
-        if isinstance(__data__, (list, tuple, set, frozenset)):
+        if isinstance(__data__, (list, tuple)):
             return __data__.__class__(cls(v) for v in __data__)
 
         return __data__
 
     def __getattr__(self, name: str, /) -> Any:
         return self[name]
```

### Comparing `gqylpy_dict-1.2.1/gqylpy_dict.egg-info/PKG-INFO` & `gqylpy_dict-1.2.2/gqylpy_dict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gqylpy-dict
-Version: 1.2.1
+Version: 1.2.2
 Summary: 基于内置 dict，它是对内置 dict 的增强。内置 dict 能做的它都能做，内置 dict 不能做的它更能做。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: WTFPL,Apache-2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-dict
 Classifier: Environment :: Web Environment
```

### Comparing `gqylpy_dict-1.2.1/setup.py` & `gqylpy_dict-1.2.2/setup.py`

 * *Files identical despite different names*

