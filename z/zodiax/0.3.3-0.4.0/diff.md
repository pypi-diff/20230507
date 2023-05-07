# Comparing `tmp/zodiax-0.3.3.tar.gz` & `tmp/zodiax-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodiax-0.3.3.tar", last modified: Tue Apr 11 08:49:33 2023, max compression
+gzip compressed data, was "zodiax-0.4.0.tar", last modified: Sun May  7 07:19:14 2023, max compression
```

## Comparing `zodiax-0.3.3.tar` & `zodiax-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:49:33.563444 zodiax-0.3.3/
--rw-r--r--   0 louis      (501) staff       (20)       70 2022-11-14 06:22:13.000000 zodiax-0.3.3/.gitignore
--rw-r--r--   0 louis      (501) staff       (20)     1523 2022-11-14 06:12:01.000000 zodiax-0.3.3/LICENSE
--rw-r--r--   0 louis      (501) staff       (20)       49 2022-11-14 11:44:43.000000 zodiax-0.3.3/MANIFEST.ini
--rw-r--r--   0 louis      (501) staff       (20)      488 2023-04-11 08:49:33.563284 zodiax-0.3.3/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)     4291 2023-04-11 08:47:45.000000 zodiax-0.3.3/README.md
--rw-r--r--   0 louis      (501) staff       (20)     2992 2023-03-20 01:49:16.000000 zodiax-0.3.3/mkdocs.yml
--rw-r--r--   0 louis      (501) staff       (20)       55 2023-03-09 09:55:10.000000 zodiax-0.3.3/requirements.txt
--rw-r--r--   0 louis      (501) staff       (20)       38 2023-04-11 08:49:33.563488 zodiax-0.3.3/setup.cfg
--rw-r--r--   0 louis      (501) staff       (20)     1508 2023-04-11 07:58:40.000000 zodiax-0.3.3/setup.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:49:33.560862 zodiax-0.3.3/tests/
--rw-r--r--   0 louis      (501) staff       (20)     6936 2023-03-22 06:53:45.000000 zodiax-0.3.3/tests/test_base.py
--rw-r--r--   0 louis      (501) staff       (20)      824 2023-03-20 01:40:07.000000 zodiax-0.3.3/tests/test_equinox.py
--rw-r--r--   0 louis      (501) staff       (20)      700 2023-03-20 01:40:07.000000 zodiax-0.3.3/tests/test_optimisation.py
--rw-r--r--   0 louis      (501) staff       (20)      668 2023-03-20 01:40:07.000000 zodiax-0.3.3/tests/test_serialisation.py
--rw-r--r--   0 louis      (501) staff       (20)      366 2023-03-20 01:40:07.000000 zodiax-0.3.3/tests/test_tree.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:49:33.561758 zodiax-0.3.3/zodiax/
--rw-r--r--   0 louis      (501) staff       (20)      428 2023-04-11 08:47:45.000000 zodiax-0.3.3/zodiax/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)    21745 2023-04-11 08:47:45.000000 zodiax-0.3.3/zodiax/base.py
--rw-r--r--   0 louis      (501) staff       (20)     5112 2023-03-20 01:40:07.000000 zodiax-0.3.3/zodiax/equinox.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:49:33.563060 zodiax-0.3.3/zodiax/experimental/
--rw-r--r--   0 louis      (501) staff       (20)      238 2023-03-22 01:43:50.000000 zodiax-0.3.3/zodiax/experimental/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)     1296 2023-04-11 08:47:45.000000 zodiax-0.3.3/zodiax/experimental/jit.py
--rw-r--r--   0 louis      (501) staff       (20)    17318 2023-04-11 08:47:45.000000 zodiax-0.3.3/zodiax/experimental/serialisation.py
--rw-r--r--   0 louis      (501) staff       (20)     2101 2023-03-23 00:20:31.000000 zodiax-0.3.3/zodiax/optimisation.py
--rw-r--r--   0 louis      (501) staff       (20)     2104 2023-03-20 01:40:07.000000 zodiax-0.3.3/zodiax/tree.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:49:33.562423 zodiax-0.3.3/zodiax.egg-info/
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-04-11 08:49:33.562689 zodiax-0.3.3/zodiax.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 louis      (501) staff       (20)      391 2022-11-14 11:49:15.000000 zodiax-0.3.3/zodiax.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 louis      (501) staff       (20)       33 2022-11-14 11:49:15.000000 zodiax-0.3.3/zodiax.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-r--r--   0 louis      (501) staff       (20)      488 2023-04-11 08:49:33.000000 zodiax-0.3.3/zodiax.egg-info/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)      645 2023-04-11 08:49:33.000000 zodiax-0.3.3/zodiax.egg-info/SOURCES.txt
--rw-r--r--   0 louis      (501) staff       (20)        1 2023-04-11 08:49:33.000000 zodiax-0.3.3/zodiax.egg-info/dependency_links.txt
--rw-r--r--   0 louis      (501) staff       (20)       49 2023-04-11 08:49:33.000000 zodiax-0.3.3/zodiax.egg-info/requires.txt
--rw-r--r--   0 louis      (501) staff       (20)       27 2023-04-11 08:49:33.000000 zodiax-0.3.3/zodiax.egg-info/top_level.txt
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-07 07:19:14.322545 zodiax-0.4.0/
+-rw-r--r--   0 louis      (501) staff       (20)       70 2022-11-14 06:22:13.000000 zodiax-0.4.0/.gitignore
+-rw-r--r--   0 louis      (501) staff       (20)     1523 2022-11-14 06:12:01.000000 zodiax-0.4.0/LICENSE
+-rw-r--r--   0 louis      (501) staff       (20)       49 2022-11-14 11:44:43.000000 zodiax-0.4.0/MANIFEST.ini
+-rw-r--r--   0 louis      (501) staff       (20)      488 2023-05-07 07:19:14.322402 zodiax-0.4.0/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)     4291 2023-04-11 08:47:45.000000 zodiax-0.4.0/README.md
+-rw-r--r--   0 louis      (501) staff       (20)     3030 2023-05-07 07:18:07.000000 zodiax-0.4.0/mkdocs.yml
+-rw-r--r--   0 louis      (501) staff       (20)       55 2023-03-09 09:55:10.000000 zodiax-0.4.0/requirements.txt
+-rw-r--r--   0 louis      (501) staff       (20)       38 2023-05-07 07:19:14.322586 zodiax-0.4.0/setup.cfg
+-rw-r--r--   0 louis      (501) staff       (20)     1508 2023-04-11 07:58:40.000000 zodiax-0.4.0/setup.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-07 07:19:14.319600 zodiax-0.4.0/tests/
+-rw-r--r--   0 louis      (501) staff       (20)     3956 2023-05-07 07:18:07.000000 zodiax-0.4.0/tests/test_base.py
+-rw-r--r--   0 louis      (501) staff       (20)     1667 2023-05-07 07:18:07.000000 zodiax-0.4.0/tests/test_bayes.py
+-rw-r--r--   0 louis      (501) staff       (20)      655 2023-05-07 07:18:07.000000 zodiax-0.4.0/tests/test_eqx.py
+-rw-r--r--   0 louis      (501) staff       (20)      332 2023-05-07 07:18:07.000000 zodiax-0.4.0/tests/test_jit.py
+-rw-r--r--   0 louis      (501) staff       (20)      630 2023-05-07 07:18:07.000000 zodiax-0.4.0/tests/test_optimisation.py
+-rw-r--r--   0 louis      (501) staff       (20)      666 2023-05-07 07:18:07.000000 zodiax-0.4.0/tests/test_serialisation.py
+-rw-r--r--   0 louis      (501) staff       (20)      453 2023-05-07 07:18:07.000000 zodiax-0.4.0/tests/test_tree.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-07 07:19:14.320354 zodiax-0.4.0/zodiax/
+-rw-r--r--   0 louis      (501) staff       (20)      472 2023-05-07 07:18:07.000000 zodiax-0.4.0/zodiax/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)    17880 2023-05-07 07:18:07.000000 zodiax-0.4.0/zodiax/base.py
+-rw-r--r--   0 louis      (501) staff       (20)    12793 2023-05-07 07:18:07.000000 zodiax-0.4.0/zodiax/bayes.py
+-rw-r--r--   0 louis      (501) staff       (20)     5711 2023-05-07 07:18:07.000000 zodiax-0.4.0/zodiax/eqx.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-07 07:19:14.322187 zodiax-0.4.0/zodiax/experimental/
+-rw-r--r--   0 louis      (501) staff       (20)      238 2023-05-04 01:45:02.000000 zodiax-0.4.0/zodiax/experimental/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)     1927 2023-05-07 07:18:07.000000 zodiax-0.4.0/zodiax/experimental/jit.py
+-rw-r--r--   0 louis      (501) staff       (20)    17318 2023-04-11 08:47:45.000000 zodiax-0.4.0/zodiax/experimental/serialisation.py
+-rw-r--r--   0 louis      (501) staff       (20)     2323 2023-05-07 07:18:07.000000 zodiax-0.4.0/zodiax/optimisation.py
+-rw-r--r--   0 louis      (501) staff       (20)     2461 2023-05-07 07:18:07.000000 zodiax-0.4.0/zodiax/tree.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-07 07:19:14.321484 zodiax-0.4.0/zodiax.egg-info/
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-07 07:19:14.321782 zodiax-0.4.0/zodiax.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 louis      (501) staff       (20)      391 2022-11-14 11:49:15.000000 zodiax-0.4.0/zodiax.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 louis      (501) staff       (20)       33 2022-11-14 11:49:15.000000 zodiax-0.4.0/zodiax.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 louis      (501) staff       (20)      488 2023-05-07 07:19:14.000000 zodiax-0.4.0/zodiax.egg-info/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)      691 2023-05-07 07:19:14.000000 zodiax-0.4.0/zodiax.egg-info/SOURCES.txt
+-rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-07 07:19:14.000000 zodiax-0.4.0/zodiax.egg-info/dependency_links.txt
+-rw-r--r--   0 louis      (501) staff       (20)       49 2023-05-07 07:19:14.000000 zodiax-0.4.0/zodiax.egg-info/requires.txt
+-rw-r--r--   0 louis      (501) staff       (20)       27 2023-05-07 07:19:14.000000 zodiax-0.4.0/zodiax.egg-info/top_level.txt
```

### Comparing `zodiax-0.3.3/LICENSE` & `zodiax-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.3/README.md` & `zodiax-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.3/mkdocs.yml` & `zodiax-0.4.0/mkdocs.yml`

 * *Files 9% similar despite different names*

```diff
@@ -90,17 +90,18 @@
 
 # ===== Navigation =====
 nav:
 - Overview: README.md
 - Using Zodiax: docs/usage.md
 
 - API: 
-  - Overview:     docs/API/api.md
-  - Base:         docs/API/base.md
-  - Equinox:      docs/API/equinox.md
-  - Optimisation: docs/API/optimisation.md
-  - Tree:         docs/API/tree.md
+  - Overview:      docs/API/api.md
+  - Base:          docs/API/base.md
+  - Tree:          docs/API/tree.md
+  - Bayes:         docs/API/bayes.md
+  - Equinox (eqx): docs/API/eqx.md
+  - Optimisation:  docs/API/optimisation.md
   - Serialisation: docs/API/serialisation.md
 
 - FAQ & Troubleshooting: docs/faq.md
 - Change Log: CHANGELOG.md
 - Contributing: CONTRIBUTING.md
```

### Comparing `zodiax-0.3.3/setup.py` & `zodiax-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.3/tests/test_serialisation.py` & `zodiax-0.4.0/tests/test_serialisation.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from jax import config
 import zodiax
 from equinox import tree_equal
 import os
 config.update("jax_debug_nans", True)
 
 
-def test_serialise_deserialise(Base_instance):
-    pytree = Base_instance
+def test_serialise_deserialise(create_base):
+    pytree = create_base()
     try:
         zodiax.experimental.serialisation.serialise('test_serialisation.zdx', pytree)
         # pytree_2 = zodiax.experimental.serialisation.deserialise('test_serialisation.zdx')
         
         os.remove('test_serialisation.zdx')
         # assert tree_equal(pytree, pytree_2)
     except Exception as e:
```

### Comparing `zodiax-0.3.3/zodiax/equinox.py` & `zodiax-0.4.0/zodiax/eqx.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,36 @@
 import zodiax
 import equinox
 from functools import wraps
 from jaxtyping import PyTree
-from typing import Union, Callable
-from equinox import partition, combine
+from typing import Union, Callable, List
+# from equinox import partition, combine
+import equinox as eqx
 from types import ModuleType
 
 
-def _convert_to_filter(pytree : PyTree, 
-                       params : Union[PyTree, list, str]) -> PyTree:
-    """
-    Converts the input params to a filter spec if not already.
+Params = Union[str, List[str]]
+Base = lambda: zodiax.base.Base
 
-    Parameters
-    ----------
-    pytree : PyTree
-        The pytree to filter.
-    params : Union[PyTree, list, str]
-        The params to filter, or an existing filter.
-    
-    Returns
-    -------
-     : PyTree
-        The filter spec.
-    """
-    if isinstance(params, zodiax.base.Base):
-        return params
-    else:
-        return zodiax.tree.get_args(pytree, params)
 
-
-def filter_grad(params : Union[PyTree, list, str], 
-                *filter_args, **filter_kwargs) -> Callable:
+def filter_grad(
+    parameters : Params, 
+    *filter_args,
+    **filter_kwargs
+    ) -> Callable:
     """
-    Applies the equinox filter_grad function to the input params. The 
+    Applies the equinox filter_grad function to the input parameters. The 
     corresponding equinox docs are found [here](https://docs.kidger.site/
     equinox/api/filtering/transformations/)
 
-
     Parameters
     ----------
-    params : Union[PyTree, list, str]
-        The params to filter. Can either be a single string path, a list of 
-        paths, or a pytree with binary leaves denoting which argument to take
-        gradients with respect to.
+    parameters : Union[str, List[str]]
+        The parameters to filter. Can either be a single string path or a list
+        of paths.
     *filter_args : Any
         The args to pass to the equinox filter_grad function.
     **filter_kwargs : Any
         The kwargs to pass to the equinox filter_grad function.
     
     Returns
     -------
@@ -55,41 +38,43 @@
         The wrapped function.
     """
     def wrapper(func : Callable):
         
         @wraps(func)
         def inner_wrapper(pytree : PyTree, *args, **kwargs):
 
-            # Convert params to filter spec if not already
-            filter_spec = _convert_to_filter(pytree, params)
+            # Convert parameters
+            boolean_filter = zodiax.tree.boolean_filter(pytree, parameters)
 
             # Wrap original function
             @equinox.filter_grad(*filter_args, **filter_kwargs)
-            def recombine(diff : PyTree, non_diff : PyTree):
-                return func(combine(diff, non_diff), *args, **kwargs)
+            def recombine(traced : PyTree, static : PyTree):
+                return func(eqx.combine(traced, static), *args, **kwargs)
             
             # Return wrapped function
-            return recombine(*partition(pytree, filter_spec))
+            return recombine(*eqx.partition(pytree, boolean_filter))
         return inner_wrapper
     return wrapper
 
 
-def filter_value_and_grad(params : Union[PyTree, list, str], 
-                *filter_args, **filter_kwargs) -> Callable:
+def filter_value_and_grad(
+    parameters : Params, 
+    *filter_args, 
+    **filter_kwargs
+    ) -> Callable:
     """
-    Applies the equinox filter_value_and_grad function to the input params. The 
-    corresponding equinox docs are found [here](https://docs.kidger.site/
+    Applies the equinox filter_value_and_grad function to the input parameters.
+    The corresponding equinox docs are found [here](https://docs.kidger.site/
     equinox/api/filtering/transformations/)
 
     Parameters
     ----------
-    params : Union[PyTree, list, str]
-        The params to filter. Can either be a single string path, a list of 
-        paths, or a pytree with binary leaves denoting which argument to take
-        gradients with respect to.
+    parameters : Union[str, List[str]]
+        The parameters to filter. Can either be a single string path or a list
+        of paths.
     *filter_args : Any
         The args to pass to the equinox filter_value_and_grad function.
     **filter_kwargs : Any
         The kwargs to pass to the equinox filter_value_and_grad function.
     
     Returns
     -------
@@ -97,43 +82,81 @@
         The wrapped function.
     """
     def wrapper(func : Callable):
 
         @wraps(func)
         def inner_wrapper(pytree : PyTree, *args, **kwargs):
 
-            # Convert params to filter spec if not already
-            filter_spec = _convert_to_filter(pytree, params)
+            # Convert parameters
+            boolean_filter = zodiax.tree.boolean_filter(pytree, parameters)
 
             # Wrap original function
             @equinox.filter_value_and_grad(*filter_args, **filter_kwargs)
-            def recombine(diff : PyTree, non_diff : PyTree):
-                return func(combine(diff, non_diff), *args, **kwargs)
+            def recombine(traced : PyTree, static : PyTree):
+                return func(eqx.combine(traced, static), *args, **kwargs)
             
             # Return wrapped function
-            return recombine(*partition(pytree, filter_spec))
+            return recombine(*eqx.partition(pytree, boolean_filter))
         return inner_wrapper
     return wrapper
 
 
+def partition(
+    pytree : Base(), 
+    parameters : Params, 
+    *partition_args, 
+    **partition_kwargs) -> tuple:
+    """
+    Wraps the equinox partition function to take in a list of parameters to
+    partition. The corresponding equinox docs are found [here](https://docs.
+    kidger.site/equinox/api/filtering/transformations/)
+
+    Parameters
+    ----------
+    pytree : Base()
+        The pytree to partition.
+    parameters : Union[str, List[str]]
+        The parameters to partition. Can either be a single string path or a
+        list of paths.
+    *partition_args : Any
+        The args to pass to the equinox partition function.
+    **partition_kwargs : Any
+        The kwargs to pass to the equinox partition function.
+    
+    Returns
+    -------
+    pytree1 : Base()
+        A matching pytree with Nones at all leaves not specified by the
+        parameters.
+    pytree2 : Base()
+        A matching pytree with Nones at all leaves specified by the parameters.
+    """
+    if isinstance(parameters, str):
+        parameters = [parameters]
+    boolean_filter = zodiax.tree.boolean_filter(pytree, parameters)
+    return equinox.partition(pytree, boolean_filter, *partition_args,
+        **partition_kwargs)
+
+
 # Dictionary of replaced functions
 replaced_dict = {
-    'filter_grad': filter_grad,
-    'filter_value_and_grad': filter_value_and_grad
+    'filter_grad'           : filter_grad,
+    'filter_value_and_grad' : filter_value_and_grad,
+    'partition'             : partition,
 }
 
 
 # Use the __all__ attribute of the external package to get a list of all 
 # public functions
 external_functions = [func_name for func_name in dir(equinox) 
     if not func_name.startswith("_")]
 
 
 # Define what function we want to overwrite
-replace = ['filter_grad', 'filter_value_and_grad']
+replace = list(replaced_dict.keys())
 
 
 # Create a dictionary of wrapper functions that simply call the corresponding 
 # function from the external package
 wrapper_functions = {}
 replaced_functions = []
 for func_name in external_functions:
```

### Comparing `zodiax-0.3.3/zodiax/experimental/serialisation.py` & `zodiax-0.4.0/zodiax/experimental/serialisation.py`

 * *Files identical despite different names*

### Comparing `zodiax-0.3.3/zodiax/optimisation.py` & `zodiax-0.4.0/zodiax/optimisation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 import zodiax
 from jax.tree_util import tree_map
 from equinox import is_array, filter as eqx_filter
 from optax import adam, multi_transform, GradientTransformation
-from typing import Union
+from typing import Union, List
 from jaxtyping import PyTree
 
 
 __all__ = ["get_optimiser"]
 
 
-def get_optimiser(pytree     : PyTree,
-                  paths      : Union[str, list],
-                  optimisers : Union[GradientTransformation, list],
+Base = lambda: zodiax.base.Base
+Params = Union[str, List[str]]
+Optimisers = Union[GradientTransformation, list]
+
+
+def get_optimiser(pytree     : Base(),
+                  parameters : Params,
+                  optimisers : Optimisers,
                   ) -> tuple:
     """
     Returns an Optax.GradientTransformion object, with the optimisers
-    specified by optimisers applied to the leaves specified by paths.
+    specified by optimisers applied to the leaves specified by parameters.
 
     Parameters
     ----------
-    paths : Union[str, list]
-        A path or list of paths or list of nested paths.
+    pytree : Base
+        A zodiax.base.Base object.
+    parameters :  Union[str, List[str]]
+        A path or list of parameters or list of nested parameters.
     optimisers : Union[optax.GradientTransformation, list]
         A optax.GradientTransformation or list of
         optax.GradientTransformation objects to be applied to the leaves
-        specified by paths.
+        specified by parameters.
 
     Returns
     -------
-    (optimiser, state) : tuple
+    optimiser : optax.GradientTransformion
+        TODO Update
         A tuple of (Optax.GradientTransformion, optax.MultiTransformState)
         objects, with the optimisers applied to the leaves specified by
-        paths, and the initialised optimisation state.
+        parameters, and the initialised optimisation state.
+    state : optax.MultiTransformState
     """
     # Pre-wrap single inputs into a list since optimisers have a length of 2
     if not isinstance(optimisers, list):
         optimisers = [optimisers]
     
-    # Paths have to default be wrapped in a list to match optimiser
-    if isinstance(paths, str):
-        paths = [paths]
+    # parameters have to default be wrapped in a list to match optimiser
+    if isinstance(parameters, str):
+        parameters = [parameters]
 
     # Construct groups and get param_spec
     groups = [str(i) for i in range(len(optimisers))]
     param_spec = tree_map(lambda _: "null", pytree)
-    param_spec = param_spec.set(paths, groups)
+    param_spec = param_spec.set(parameters, groups)
 
-    # Generate optimiser dictionary
+    # Generate optimiser dictionary and Assign the null group
     opt_dict = dict([(groups[i], optimisers[i]) \
                         for i in range(len(groups))])
-
-    # Assign the null group
-    # TODO: Can this be set to None?
     opt_dict["null"] = adam(0.0)
 
-    # Get optimiser object
+    # Get optimiser object and filtered optimiser
     optim = multi_transform(opt_dict, param_spec)
-
-    # Get filtered optimiser
     opt_state = optim.init(eqx_filter(pytree, is_array))
 
     # Return
     return (optim, opt_state)
```

### Comparing `zodiax-0.3.3/zodiax.egg-info/SOURCES.txt` & `zodiax-0.4.0/zodiax.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 LICENSE
 MANIFEST.ini
 README.md
 mkdocs.yml
 requirements.txt
 setup.py
 tests/test_base.py
-tests/test_equinox.py
+tests/test_bayes.py
+tests/test_eqx.py
+tests/test_jit.py
 tests/test_optimisation.py
 tests/test_serialisation.py
 tests/test_tree.py
 zodiax/__init__.py
 zodiax/base.py
-zodiax/equinox.py
+zodiax/bayes.py
+zodiax/eqx.py
 zodiax/optimisation.py
 zodiax/tree.py
 zodiax.egg-info/PKG-INFO
 zodiax.egg-info/SOURCES.txt
 zodiax.egg-info/dependency_links.txt
 zodiax.egg-info/requires.txt
 zodiax.egg-info/top_level.txt
```

