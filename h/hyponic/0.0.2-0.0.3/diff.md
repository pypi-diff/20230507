# Comparing `tmp/hyponic-0.0.2.tar.gz` & `tmp/hyponic-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyponic-0.0.2.tar", last modified: Sun May  7 17:10:43 2023, max compression
+gzip compressed data, was "hyponic-0.0.3.tar", last modified: Sun May  7 20:23:52 2023, max compression
```

## Comparing `hyponic-0.0.2.tar` & `hyponic-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 17:10:43.251694 hyponic-0.0.2/
--rw-rw-rw-   0        0        0     1095 2023-05-07 07:36:12.000000 hyponic-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     5539 2023-05-07 17:10:43.250687 hyponic-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4915 2023-05-07 17:06:45.000000 hyponic-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 17:10:43.208546 hyponic-0.0.2/hyponic/
--rw-rw-rw-   0        0        0      756 2023-05-07 16:51:34.000000 hyponic-0.0.2/hyponic/__init__.py
--rw-rw-rw-   0        0        0     4669 2023-05-07 16:51:34.000000 hyponic-0.0.2/hyponic/hyponic.py
-drwxrwxrwx   0        0        0        0 2023-05-07 17:10:43.239055 hyponic-0.0.2/hyponic/metrics/
--rw-rw-rw-   0        0        0        0 2023-05-07 17:07:29.000000 hyponic-0.0.2/hyponic/metrics/__init__.py
--rw-rw-rw-   0        0        0     2065 2023-05-07 16:51:34.000000 hyponic-0.0.2/hyponic/metrics/classification.py
--rw-rw-rw-   0        0        0     3023 2023-05-07 16:51:34.000000 hyponic-0.0.2/hyponic/metrics/decorators.py
--rw-rw-rw-   0        0        0     1950 2023-05-07 16:51:34.000000 hyponic-0.0.2/hyponic/metrics/regression.py
-drwxrwxrwx   0        0        0        0 2023-05-07 17:10:43.241062 hyponic-0.0.2/hyponic/optimizers/
--rw-rw-rw-   0        0        0        0 2023-05-07 08:03:05.000000 hyponic-0.0.2/hyponic/optimizers/__init__.py
--rw-rw-rw-   0        0        0     2532 2023-05-07 16:51:34.000000 hyponic-0.0.2/hyponic/optimizers/base_optimizer.py
-drwxrwxrwx   0        0        0        0 2023-05-07 17:10:43.243411 hyponic-0.0.2/hyponic/optimizers/genetic_based/
--rw-rw-rw-   0        0        0     3086 2023-05-07 16:51:34.000000 hyponic-0.0.2/hyponic/optimizers/genetic_based/GA.py
--rw-rw-rw-   0        0        0        0 2023-05-07 17:04:31.000000 hyponic-0.0.2/hyponic/optimizers/genetic_based/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 17:10:43.245669 hyponic-0.0.2/hyponic/optimizers/physics_based/
--rw-rw-rw-   0        0        0     1689 2023-05-07 16:51:34.000000 hyponic-0.0.2/hyponic/optimizers/physics_based/SA.py
--rw-rw-rw-   0        0        0        0 2023-05-07 17:00:07.000000 hyponic-0.0.2/hyponic/optimizers/physics_based/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 17:10:43.249676 hyponic-0.0.2/hyponic/optimizers/swarm_based/
--rw-rw-rw-   0        0        0     3317 2023-05-07 16:51:34.000000 hyponic-0.0.2/hyponic/optimizers/swarm_based/ABC.py
--rw-rw-rw-   0        0        0     2899 2023-05-07 16:51:34.000000 hyponic-0.0.2/hyponic/optimizers/swarm_based/ACO.py
--rw-rw-rw-   0        0        0     3025 2023-05-07 16:51:34.000000 hyponic-0.0.2/hyponic/optimizers/swarm_based/PSO.py
--rw-rw-rw-   0        0        0        0 2023-05-07 16:59:57.000000 hyponic-0.0.2/hyponic/optimizers/swarm_based/__init__.py
--rw-rw-rw-   0        0        0     3963 2023-05-07 16:51:34.000000 hyponic-0.0.2/hyponic/space.py
--rw-rw-rw-   0        0        0     1546 2023-04-23 15:51:05.000000 hyponic-0.0.2/hyponic/symtable.py
-drwxrwxrwx   0        0        0        0 2023-05-07 17:10:43.234626 hyponic-0.0.2/hyponic.egg-info/
--rw-rw-rw-   0        0        0     5539 2023-05-07 17:10:43.000000 hyponic-0.0.2/hyponic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      771 2023-05-07 17:10:43.000000 hyponic-0.0.2/hyponic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 17:10:43.000000 hyponic-0.0.2/hyponic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-07 17:10:43.000000 hyponic-0.0.2/hyponic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-07 17:10:43.000000 hyponic-0.0.2/hyponic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 17:10:43.251694 hyponic-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      865 2023-05-07 17:09:06.000000 hyponic-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:52.021546 hyponic-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 20:23:33.000000 hyponic-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-05-07 20:23:52.021546 hyponic-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-05-07 20:23:33.000000 hyponic-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:52.021546 hyponic-0.0.3/hyponic/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/hyponic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:52.021546 hyponic-0.0.3/hyponic/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/metrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/metrics/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/metrics/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:52.021546 hyponic-0.0.3/hyponic/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/base_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:52.021546 hyponic-0.0.3/hyponic/optimizers/genetic_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/genetic_based/GA.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/genetic_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:52.021546 hyponic-0.0.3/hyponic/optimizers/physics_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/physics_based/SA.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/physics_based/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:52.021546 hyponic-0.0.3/hyponic/optimizers/swarm_based/
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/swarm_based/ABC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/swarm_based/ACO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/swarm_based/PSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/optimizers/swarm_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-07 20:23:33.000000 hyponic-0.0.3/hyponic/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:23:52.021546 hyponic-0.0.3/hyponic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-05-07 20:23:52.000000 hyponic-0.0.3/hyponic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-07 20:23:52.000000 hyponic-0.0.3/hyponic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:23:52.000000 hyponic-0.0.3/hyponic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-07 20:23:52.000000 hyponic-0.0.3/hyponic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-07 20:23:52.000000 hyponic-0.0.3/hyponic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 20:23:52.021546 hyponic-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-07 20:23:33.000000 hyponic-0.0.3/setup.py
```

### Comparing `hyponic-0.0.2/hyponic/__init__.py` & `hyponic-0.0.3/hyponic/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-__version__ = '0.0.1'
-
-from .hyponic import HypONIC
-
-from .metrics.decorators import add_metric_info, add_metric_to_dict, minimize_metric, maximize_metric
-from .metrics.classification import accuracy, precision, recall, f1_score,\
-    fbeta, confusion_matrix, binary_crossentropy, categorical_crossentropy, log_loss
-from .metrics.regression import mae, mse, rmse, rmsle, r2, adjusted_r2, huber_loss
-
-from .optimizers.genetic_based.GA import GA
-from .optimizers.physics_based.SA import SA
-from .optimizers.swarm_based.ABC import ABC
-from .optimizers.swarm_based.ACO import ACO
-from .optimizers.swarm_based.PSO import PSO, IWPSO
-from .optimizers.base_optimizer import BaseOptimizer
-
-from .space import Space, Dimension, Continuous, Discrete
+__version__ = '0.0.1-alpha-0'
+
+from .hyponic import HypONIC
+
+from .metrics.decorators import add_metric_to_dict, add_metric_info,\
+    add_metric_aliases, minimize_metric, maximize_metric
+
+from .metrics.classification import accuracy, precision, recall, f1_score,\
+    fbeta, confusion_matrix, binary_crossentropy, categorical_crossentropy, log_loss
+
+from .metrics.regression import mae, mse, rmse, rmsle, r2, adjusted_r2, huber_loss
+
+from .optimizers.genetic_based.GA import GA
+from .optimizers.physics_based.SA import SA
+from .optimizers.swarm_based.ABC import ABC
+from .optimizers.swarm_based.ACO import ACO
+from .optimizers.swarm_based.PSO import PSO, IWPSO
+from .optimizers.base_optimizer import BaseOptimizer
+
+from .space import Space, Dimension, Continuous, Discrete
```

### Comparing `hyponic-0.0.2/hyponic/hyponic.py` & `hyponic-0.0.3/hyponic/hyponic.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-from warnings import warn
-
-from hyponic.optimizers.swarm_based.PSO import IWPSO
-from hyponic.metrics.decorators import METRICS_DICT
-
-from typing import Callable
-
-from hyponic.space import Space
-from functools import partial
-
-
-class HypONIC:
-    """
-    HypONIC (Hyperparameter Optimization using Nature-Inspired Computing)
-
-    Main class for hyperparameter optimization.
-    """
-    def __init__(self, model, X, y, metric: Callable | str, optimizer=None, **kwargs):
-        self.model = model
-        self.X = X
-        self.y = y
-
-        if isinstance(metric, str):
-            # Try to get metric from the METRICS_DICT
-            self.metric = METRICS_DICT.get(metric, None)
-
-            if self.metric is None:
-                raise Exception(f"Metric {metric} is not found.")
-        elif isinstance(metric, Callable):
-            self.metric = metric
-
-        try:
-            self.minmax = self.metric.__getattribute__("minmax")
-        except AttributeError:
-            # If a metric does not have minmax attribute,
-            # then it is assumed to be a custom metric and will be minimized by default
-            warn(f"Metric {metric.__name__} does not have minmax attribute. Minimize by default.")
-            self.minmax = "min"
-
-        if kwargs is None:  # Default values for optimizer
-            kwargs = {"epoch": 10, "pop_size": 10}
-
-        if optimizer is None:
-            self.optimizer = IWPSO(**kwargs)
-        else:
-            self.optimizer = optimizer(**kwargs)
-
-        self.hyperparams_optimized = None
-        self.metric_optimized = None
-
-    @staticmethod
-    def warn_not_optimized(func):
-        """
-        Decorator that warns if a method is called before optimization.
-        """
-
-        def wrapper(*args, **kwargs):
-            if args[0].hyperparams_optimized is None:
-                raise Exception("Model is not optimized yet. Please call optimize method first")
-            return func(*args, **kwargs)
-
-        return wrapper
-
-    def _fitness_wrapper(self, dimensions_names: list, mapping_funcs: dict, values: list) -> float:
-        # Map back to original space
-        hyperparams = {
-            dim: mapping_funcs[dim](val) for dim, val in zip(dimensions_names, values)
-        }
-
-        self.model.set_params(**hyperparams)
-        self.model.fit(self.X, self.y)
-
-        y_pred = self.model.predict(self.X)
-        return self.metric(self.y, y_pred)  # TODO: maybe cross-validation could be used instead
-
-    def optimize(self, hyperparams: dict, verbose=False) -> (dict, float):
-        # Create a space for hyperparameters
-        hyperspace = Space(hyperparams)
-        if verbose:
-            print("Successfully created a space for hyperparameters optimization")
-            print(f"Using {self.optimizer.__class__.__name__} optimizer")
-            print(f"Metric {self.metric.__name__} is subject to {self.minmax}imization")
-            print(hyperspace)
-
-        # Map hyperparameters to continuous space
-        mappings_with_bounds = hyperspace.get_continuous_mappings(origins=0)  # Make that all dimensions start from 0
-
-        # Split mappings and bounds
-        mapping_funcs = {}
-
-        low_bounds = []
-        highs_bounds = []
-
-        for name in hyperspace.dimensions_names:
-            mapping, (low, high) = mappings_with_bounds[name]
-
-            mapping_funcs[name] = mapping
-            low_bounds.append(low)
-            highs_bounds.append(high)
-
-        paramspace = {
-            "fit_func": partial(self._fitness_wrapper, hyperspace.dimensions_names, mapping_funcs),
-            "lb": low_bounds,
-            "ub": highs_bounds,
-            "minmax": self.minmax
-        }
-
-        hyperparams_optimized, metric_optimized = self.optimizer.solve(paramspace, verbose=verbose)
-
-        # Map back to the original space
-        hyperparams_optimized = {
-            dim: mapping_funcs[dim](val) for dim, val in zip(hyperspace.dimensions_names, hyperparams_optimized)
-        }
-
-        self.hyperparams_optimized = hyperparams_optimized
-        self.metric_optimized = metric_optimized
-
-        return hyperparams_optimized, metric_optimized
-
-    @warn_not_optimized
-    def get_optimized_model(self):
-        self.model.set_params(**self.hyperparams_optimized)
-        self.model.fit(self.X, self.y)
-        return self.model
-
-    @warn_not_optimized
-    def get_optimized_parameters(self) -> dict:
-        return self.hyperparams_optimized
-
-    @warn_not_optimized
-    def get_optimized_metric(self) -> float:
-        return self.metric_optimized
+from warnings import warn
+
+from hyponic.optimizers.swarm_based.PSO import IWPSO
+from hyponic.metrics.decorators import METRICS_DICT
+
+from typing import Callable
+
+from hyponic.space import Space
+from functools import partial
+
+
+class HypONIC:
+    """
+    HypONIC (Hyperparameter Optimization using Nature-Inspired Computing)
+
+    Main class for hyperparameter optimization.
+    """
+    def __init__(self, model, X, y, metric: Callable | str, optimizer=None, **kwargs):
+        self.model = model
+        self.X = X
+        self.y = y
+
+        if isinstance(metric, str):
+            # Try to get metric from the METRICS_DICT
+            self.metric = METRICS_DICT.get(metric, None)
+
+            if self.metric is None:
+                raise Exception(f"Metric {metric} is not found.")
+        elif isinstance(metric, Callable):
+            self.metric = metric
+
+        try:
+            self.minmax = self.metric.__getattribute__("minmax")
+        except AttributeError:
+            # If a metric does not have minmax attribute,
+            # then it is assumed to be a custom metric and will be minimized by default
+            warn(f"Metric {metric.__name__} does not have minmax attribute. Minimize by default.")
+            self.minmax = "min"
+
+        if kwargs is None:  # Default values for optimizer
+            kwargs = {"epoch": 10, "pop_size": 10}
+
+        if optimizer is None:
+            self.optimizer = IWPSO(**kwargs)
+        else:
+            self.optimizer = optimizer(**kwargs)
+
+        self.hyperparams_optimized = None
+        self.metric_optimized = None
+
+    @staticmethod
+    def warn_not_optimized(func):
+        """
+        Decorator that warns if a method is called before optimization.
+        """
+
+        def wrapper(*args, **kwargs):
+            if args[0].hyperparams_optimized is None:
+                raise Exception("Model is not optimized yet. Please call optimize method first")
+            return func(*args, **kwargs)
+
+        return wrapper
+
+    def _fitness_wrapper(self, dimensions_names: list, mapping_funcs: dict, values: list) -> float:
+        # Map back to original space
+        hyperparams = {
+            dim: mapping_funcs[dim](val) for dim, val in zip(dimensions_names, values)
+        }
+
+        self.model.set_params(**hyperparams)
+        self.model.fit(self.X, self.y)
+
+        y_pred = self.model.predict(self.X)
+        return self.metric(self.y, y_pred)  # TODO: maybe cross-validation could be used instead
+
+    def optimize(self, hyperparams: dict, verbose=False) -> (dict, float):
+        # Create a space for hyperparameters
+        hyperspace = Space(hyperparams)
+        if verbose:
+            print("Successfully created a space for hyperparameters optimization")
+            print(f"Using {self.optimizer.__class__.__name__} optimizer")
+            print(f"Metric {self.metric.__name__} is subject to {self.minmax}imization")
+            print(hyperspace)
+
+        # Map hyperparameters to continuous space
+        mappings_with_bounds = hyperspace.get_continuous_mappings(origins=0)  # Make that all dimensions start from 0
+
+        # Split mappings and bounds
+        mapping_funcs = {}
+
+        low_bounds = []
+        highs_bounds = []
+
+        for name in hyperspace.dimensions_names:
+            mapping, (low, high) = mappings_with_bounds[name]
+
+            mapping_funcs[name] = mapping
+            low_bounds.append(low)
+            highs_bounds.append(high)
+
+        paramspace = {
+            "fit_func": partial(self._fitness_wrapper, hyperspace.dimensions_names, mapping_funcs),
+            "lb": low_bounds,
+            "ub": highs_bounds,
+            "minmax": self.minmax
+        }
+
+        hyperparams_optimized, metric_optimized = self.optimizer.solve(paramspace, verbose=verbose)
+
+        # Map back to the original space
+        hyperparams_optimized = {
+            dim: mapping_funcs[dim](val) for dim, val in zip(hyperspace.dimensions_names, hyperparams_optimized)
+        }
+
+        self.hyperparams_optimized = hyperparams_optimized
+        self.metric_optimized = metric_optimized
+
+        return hyperparams_optimized, metric_optimized
+
+    @warn_not_optimized
+    def get_optimized_model(self):
+        self.model.set_params(**self.hyperparams_optimized)
+        self.model.fit(self.X, self.y)
+        return self.model
+
+    @warn_not_optimized
+    def get_optimized_parameters(self) -> dict:
+        return self.hyperparams_optimized
+
+    @warn_not_optimized
+    def get_optimized_metric(self) -> float:
+        return self.metric_optimized
```

### Comparing `hyponic-0.0.2/hyponic/metrics/classification.py` & `hyponic-0.0.3/hyponic/metrics/regression.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,51 @@
-"""
-This module contains metrics for evaluating classification models.
-"""
-from hyponic.metrics.decorators import add_metric_info, maximize_metric, minimize_metric
-
-import numpy as np
-
-
-@maximize_metric
-def accuracy(y_true: np.array, y_pred: np.array) -> np.ndarray:
-    return np.mean(np.equal(y_true, y_pred))
-
-
-@maximize_metric
-def precision(y_true: np.array, y_pred: np.array) -> np.ndarray:
-    tp = np.sum(np.logical_and(y_true == 1, y_pred == 1))
-    fp = np.sum(np.logical_and(y_true == 0, y_pred == 1))
-    return tp / (tp + fp)
-
-
-@maximize_metric
-def recall(y_true: np.array, y_pred: np.array) -> np.ndarray:
-    tp = np.sum(np.logical_and(y_true == 1, y_pred == 1))
-    fn = np.sum(np.logical_and(y_true == 1, y_pred == 0))
-    return tp / (tp + fn)
-
-
-@maximize_metric
-def f1_score(y_true: np.array, y_pred: np.array) -> np.ndarray:
-    p = precision(y_true, y_pred)
-    r = recall(y_true, y_pred)
-    return 2 * p * r / (p + r)
-
-
-@maximize_metric
-def fbeta(y_true: np.array, y_pred: np.array, beta: float = 1.0) -> np.ndarray:
-    p = precision(y_true, y_pred)
-    r = recall(y_true, y_pred)
-    return (1 + beta ** 2) * p * r / (beta ** 2 * p + r)
-
-
-@maximize_metric
-def confusion_matrix(y_true: np.array, y_pred: np.array) -> np.ndarray:
-    tp = np.sum(np.logical_and(y_true == 1, y_pred == 1))
-    fp = np.sum(np.logical_and(y_true == 0, y_pred == 1))
-    fn = np.sum(np.logical_and(y_true == 1, y_pred == 0))
-    tn = np.sum(np.logical_and(y_true == 0, y_pred == 0))
-    return np.array([[tp, fp], [fn, tn]])
-
-
-@minimize_metric
-def log_loss(y_true: np.array, y_pred: np.array) -> np.ndarray:
-    return np.mean(np.log(1 + np.exp(-y_true * y_pred)))
-
-
-@minimize_metric
-def binary_crossentropy(y_true: np.array, y_pred: np.array) -> np.ndarray:
-    return -np.mean(y_true * np.log(y_pred) + (1 - y_true) * np.log(1 - y_pred))
-
-
-@minimize_metric
-def categorical_crossentropy(y_true: np.array, y_pred: np.array) -> np.ndarray:
-    return -np.mean(np.sum(y_true * np.log(y_pred), axis=-1))
+"""
+This module contains metrics for evaluating regression models.
+"""
+from hyponic.metrics.decorators import add_metric_aliases, add_metric_info, maximize_metric, minimize_metric
+
+import numpy as np
+
+
+@add_metric_aliases("mean_absolute_error")
+@add_metric_info("Mean Absolute Error (MAE) is the average of the absolute errors.")
+@minimize_metric
+def mae(y_true: np.array, y_pred: np.array) -> np.ndarray:
+    return np.mean(np.abs(y_true - y_pred))
+
+
+@add_metric_aliases("mean_squared_error")
+@add_metric_info("Mean Squared Error (MSE) is the average of the squares of the errors.")
+@minimize_metric
+def mse(y_true: np.array, y_pred: np.array) -> np.ndarray:
+    return np.mean(np.square(y_true - y_pred))
+
+
+@add_metric_aliases("root_mean_squared_error")
+@add_metric_info("Root Mean Squared Error (RMSE) is the square root of the average of the squared errors.")
+@minimize_metric
+def rmse(y_true: np.array, y_pred: np.array) -> np.ndarray:
+    return np.sqrt(mse(y_true, y_pred))
+
+
+@add_metric_aliases("root_mean_squared_log_error")
+@add_metric_info("Root Mean Squared Log Error (RMSLE) is the log of the square root of"
+                 "the average of the squared errors.")
+@minimize_metric
+def rmsle(y_true: np.array, y_pred: np.array) -> np.ndarray:
+    return np.log(rmse(y_true, y_pred))
+
+
+@maximize_metric
+def r2(y_true: np.array, y_pred: np.array) -> np.ndarray:
+    return 1 - np.sum(np.square(y_true - y_pred)) / np.sum(np.square(y_true - np.mean(y_true)))
+
+
+@maximize_metric
+def adjusted_r2(y_true: np.array, y_pred: np.array) -> np.ndarray:
+    return 1 - (1 - r2(y_true, y_pred)) * (len(y_true) - 1) / (len(y_true) - len(y_true[0]) - 1)
+
+
+@minimize_metric
+def huber_loss(y_true: np.array, y_pred: np.array, delta: float = 1.0) -> np.ndarray:
+    error = y_true - y_pred
+    return np.where(np.abs(error) <= delta, 0.5 * np.square(error), delta * (np.abs(error) - 0.5 * delta))
```

### Comparing `hyponic-0.0.2/hyponic/optimizers/base_optimizer.py` & `hyponic-0.0.3/hyponic/optimizers/base_optimizer.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-from abc import ABC, abstractmethod
-import numpy as np
-
-
-class BaseOptimizer(ABC):
-    """
-    Base class for all optimizers. All optimizers should inherit from this class
-    """
-
-    def __init__(self, **kwargs):
-        self.epoch = kwargs.get("epoch", 10)
-        self.population_size = kwargs.get("population_size", 10)
-
-        self.function = None
-        self.lb = None
-        self.ub = None
-        self.minmax = kwargs.get('minmax', None)
-
-        self.intervals = None
-        self.dimensions = None
-
-    @abstractmethod
-    def initialize(self, problem_dict):
-        """
-        Initialize the optimizer with the problem dictionary
-        :param problem_dict: dictionary containing the problem definition
-        :return: None
-        """
-        # Unpack the problem dictionary
-        self.function = problem_dict["fit_func"]
-        self.lb = np.array(problem_dict["lb"])
-        self.ub = np.array(problem_dict["ub"])
-        self.minmax = problem_dict['minmax'] if self.minmax is None else self.minmax
-
-        self.intervals = self.ub - self.lb
-        self.dimensions = len(self.lb)
-
-    @abstractmethod
-    def evolve(self, current_epoch):
-        """
-        Evolve the population for one epoch
-        :param current_epoch: current epoch number
-        :return: None
-        """
-        pass
-
-    @abstractmethod
-    def get_best_score(self):
-        """
-        Get the best score of the current population
-        :return: best score
-        """
-        pass
-
-    @abstractmethod
-    def get_best_solution(self):
-        """
-        Get the best solution of the current population
-        :return: best solution
-        """
-        pass
-
-    def _minmax(self):
-        if self.minmax == 'min':
-            return np.min
-        return np.max
-
-    def _argminmax(self):
-        if self.minmax == 'min':
-            return np.argmin
-        return np.argmax
-
-    def solve(self, problem_dict, verbose=False):
-        """
-        Solve the problem
-        :param problem_dict: dictionary containing the problem definition
-        :param verbose: if True, prints the best score at each epoch
-        :return: None
-        """
-        self.initialize(problem_dict)
-        for current_epoch in range(self.epoch):
-            self.evolve(current_epoch)
-            if verbose:
-                print(f'Epoch: {current_epoch}, Best Score: {self.get_best_score()}')
-        return self.get_best_solution(), self.get_best_score()
+from abc import ABC, abstractmethod
+import numpy as np
+
+
+class BaseOptimizer(ABC):
+    """
+    Base class for all optimizers. All optimizers should inherit from this class
+    """
+
+    def __init__(self, **kwargs):
+        self.epoch = kwargs.get("epoch", 10)
+        self.population_size = kwargs.get("population_size", 10)
+
+        self.function = None
+        self.lb = None
+        self.ub = None
+        self.minmax = kwargs.get('minmax', None)
+
+        self.intervals = None
+        self.dimensions = None
+
+    @abstractmethod
+    def initialize(self, problem_dict):
+        """
+        Initialize the optimizer with the problem dictionary
+        :param problem_dict: dictionary containing the problem definition
+        :return: None
+        """
+        # Unpack the problem dictionary
+        self.function = problem_dict["fit_func"]
+        self.lb = np.array(problem_dict["lb"])
+        self.ub = np.array(problem_dict["ub"])
+        self.minmax = problem_dict['minmax'] if self.minmax is None else self.minmax
+
+        self.intervals = self.ub - self.lb
+        self.dimensions = len(self.lb)
+
+    @abstractmethod
+    def evolve(self, current_epoch):
+        """
+        Evolve the population for one epoch
+        :param current_epoch: current epoch number
+        :return: None
+        """
+        pass
+
+    @abstractmethod
+    def get_best_score(self):
+        """
+        Get the best score of the current population
+        :return: best score
+        """
+        pass
+
+    @abstractmethod
+    def get_best_solution(self):
+        """
+        Get the best solution of the current population
+        :return: best solution
+        """
+        pass
+
+    def _minmax(self):
+        if self.minmax == 'min':
+            return np.min
+        return np.max
+
+    def _argminmax(self):
+        if self.minmax == 'min':
+            return np.argmin
+        return np.argmax
+
+    def solve(self, problem_dict, verbose=False):
+        """
+        Solve the problem
+        :param problem_dict: dictionary containing the problem definition
+        :param verbose: if True, prints the best score at each epoch
+        :return: None
+        """
+        self.initialize(problem_dict)
+        for current_epoch in range(self.epoch):
+            self.evolve(current_epoch)
+            if verbose:
+                print(f'Epoch: {current_epoch}, Best Score: {self.get_best_score()}')
+        return self.get_best_solution(), self.get_best_score()
```

### Comparing `hyponic-0.0.2/hyponic/optimizers/genetic_based/GA.py` & `hyponic-0.0.3/hyponic/optimizers/genetic_based/GA.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-from hyponic.optimizers.base_optimizer import BaseOptimizer
-
-import numpy as np
-
-
-class GA(BaseOptimizer):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.population = None
-        self.scores = None
-        self.best_score = None
-        self.best_solution = None
-
-    def initialize(self, problem_dict):
-        super().initialize(problem_dict)
-
-        self.population = np.random.uniform(low=self.lb, high=self.ub, size=(self.population_size, self.dimensions))
-        self.scores = [self.function(x) for x in self.population]
-
-        best_idx = self._argminmax()(self.scores)
-        self.best_score = self.scores[best_idx]
-        self.best_solution = self.population[best_idx]
-
-    def evolve(self, epoch):
-        next_population = np.zeros_like(self.population)
-        next_scores = np.zeros(self.population_size)
-
-        # Elitism: keep the best solution from the previous generation
-        best_idx = self._argminmax()(self.scores)
-        next_population[0] = self.population[best_idx]
-        next_scores[0] = self.scores[best_idx]
-
-        # Roulette Wheel Selection
-        fitness = self.scores - np.min(self.scores) if self.minmax == 'min' else np.max(self.scores) - self.scores
-        total_fitness = np.sum(fitness)
-        if total_fitness == 0:
-            probs = np.ones(self.population_size) / self.population_size
-        else:
-            probs = fitness / total_fitness
-        cum_probs = np.cumsum(probs)
-
-        # Crossover and mutation
-        for i in range(1, self.population_size):
-            # Select two parents using roulette wheel selection
-            parent1_idx = np.searchsorted(cum_probs, np.random.rand())
-            parent2_idx = np.searchsorted(cum_probs, np.random.rand())
-
-            # Single point crossover
-            crossover_point = np.random.randint(1, self.dimensions)
-
-            next_population[i, :crossover_point] = self.population[parent1_idx, :crossover_point]
-            next_population[i, crossover_point:] = self.population[parent2_idx, crossover_point:]
-
-            # Mutation
-            mutation_strength = 0.5 * (self.ub - self.lb)
-
-            next_population[i] += np.random.normal(0, mutation_strength, size=self.dimensions)
-            next_population[i] = np.clip(next_population[i], self.lb, self.ub)
-
-        # evaluate the new population
-        for i in range(self.population_size):
-            next_scores[i] = self.function(next_population[i])
-
-        # update the best solution and score
-        best_idx = self._argminmax()(next_scores)
-        if self._minmax()(next_scores) < self._minmax()(self.scores):
-            self.best_solution = next_population[best_idx]
-            self.best_score = next_scores[best_idx]
-
-        # replace the old population with the new one
-        self.population = next_population
-        self.scores = next_scores
-
-    def get_best_score(self):
-        return self.best_score
-
-    def get_best_solution(self):
-        return self.best_solution
+from hyponic.optimizers.base_optimizer import BaseOptimizer
+
+import numpy as np
+
+
+class GA(BaseOptimizer):
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.population = None
+        self.scores = None
+        self.best_score = None
+        self.best_solution = None
+
+    def initialize(self, problem_dict):
+        super().initialize(problem_dict)
+
+        self.population = np.random.uniform(low=self.lb, high=self.ub, size=(self.population_size, self.dimensions))
+        self.scores = [self.function(x) for x in self.population]
+
+        best_idx = self._argminmax()(self.scores)
+        self.best_score = self.scores[best_idx]
+        self.best_solution = self.population[best_idx]
+
+    def evolve(self, epoch):
+        next_population = np.zeros_like(self.population)
+        next_scores = np.zeros(self.population_size)
+
+        # Elitism: keep the best solution from the previous generation
+        best_idx = self._argminmax()(self.scores)
+        next_population[0] = self.population[best_idx]
+        next_scores[0] = self.scores[best_idx]
+
+        # Roulette Wheel Selection
+        fitness = self.scores - np.min(self.scores) if self.minmax == 'min' else np.max(self.scores) - self.scores
+        total_fitness = np.sum(fitness)
+        if total_fitness == 0:
+            probs = np.ones(self.population_size) / self.population_size
+        else:
+            probs = fitness / total_fitness
+        cum_probs = np.cumsum(probs)
+
+        # Crossover and mutation
+        for i in range(1, self.population_size):
+            # Select two parents using roulette wheel selection
+            parent1_idx = np.searchsorted(cum_probs, np.random.rand())
+            parent2_idx = np.searchsorted(cum_probs, np.random.rand())
+
+            # Single point crossover
+            crossover_point = np.random.randint(1, self.dimensions)
+
+            next_population[i, :crossover_point] = self.population[parent1_idx, :crossover_point]
+            next_population[i, crossover_point:] = self.population[parent2_idx, crossover_point:]
+
+            # Mutation
+            mutation_strength = 0.5 * (self.ub - self.lb)
+
+            next_population[i] += np.random.normal(0, mutation_strength, size=self.dimensions)
+            next_population[i] = np.clip(next_population[i], self.lb, self.ub)
+
+        # evaluate the new population
+        for i in range(self.population_size):
+            next_scores[i] = self.function(next_population[i])
+
+        # update the best solution and score
+        best_idx = self._argminmax()(next_scores)
+        if self._minmax()(next_scores) < self._minmax()(self.scores):
+            self.best_solution = next_population[best_idx]
+            self.best_score = next_scores[best_idx]
+
+        # replace the old population with the new one
+        self.population = next_population
+        self.scores = next_scores
+
+    def get_best_score(self):
+        return self.best_score
+
+    def get_best_solution(self):
+        return self.best_solution
```

### Comparing `hyponic-0.0.2/hyponic/optimizers/swarm_based/ABC.py` & `hyponic-0.0.3/hyponic/optimizers/swarm_based/ABC.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-from hyponic.optimizers.base_optimizer import BaseOptimizer
-
-import numpy as np
-from copy import deepcopy
-
-class ABC(BaseOptimizer):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-        self.limits = kwargs.get('limits', 25)  # The number of trials before abandoning a food source
-        self.coords = None
-        self.fitness = None
-        self.g_best = None
-        self.g_best_coords = None
-        self.trials = None
-
-    def initialize(self, problem_dict):
-        super().initialize(problem_dict)
-        self.g_best = np.inf if self._minmax() == min else -np.inf
-
-        self.coords = np.random.uniform(self.lb, self.ub, (self.population_size, self.dimensions))
-        self.fitness = np.array([self.function(self.coords[i]) for i in range(self.population_size)])
-
-        self.trials = np.zeros(self.population_size)
-
-    def _employed_bees_phase(self):
-        for i in range(self.population_size):
-            k = np.random.choice([j for j in range(self.population_size) if j != i])
-            phi = np.random.uniform(-1, 1, self.dimensions)
-            new_coords = self.coords[i] + phi * (self.coords[i] - self.coords[k])
-
-            # TODO: if lb or ub is provided, clip the coordinates
-            new_coords = np.clip(new_coords, self.lb, self.ub)
-            new_fitness = self.function(new_coords)
-            if self._minmax()(np.array([self.fitness[i], new_fitness])) != self.fitness[i]:
-                self.coords[i] = new_coords
-                self.fitness[i] = new_fitness
-                self.trials[i] = 0
-            else:
-                self.trials[i] += 1
-
-    def _onlooker_bees_phase(self):
-        probabilities = self.fitness / np.sum(self.fitness)
-        if np.isnan(probabilities).any():
-            probabilities = np.ones(self.population_size) / self.population_size
-        for i in range(self.population_size):
-            k = np.random.choice([j for j in range(self.population_size)], p=probabilities)
-            phi = np.random.uniform(-1, 1, self.dimensions)
-            new_coords = self.coords[i] + phi * (self.coords[i] - self.coords[k])
-            new_coords = np.clip(new_coords, self.lb, self.ub)
-            new_fitness = self.function(new_coords)
-            if self._minmax()(np.array([self.fitness[i], new_fitness])) != self.fitness[i]:
-                self.coords[i] = new_coords
-                self.fitness[i] = new_fitness
-                self.trials[i] = 0
-            else:
-                self.trials[i] += 1
-
-    def _scout_bees_phase(self):
-        for i in range(self.population_size):
-            if self.trials[i] > self.limits:
-                self.coords[i] = np.random.uniform(self.lb, self.ub, self.dimensions)
-                self.fitness[i] = self.function(self.coords[i])
-                self.trials[i] = 0
-
-    def evolve(self, epoch):
-        self._employed_bees_phase()
-        self._onlooker_bees_phase()
-        self._scout_bees_phase()
-
-        best_index = self._argminmax()(self.fitness)
-        self.g_best = self.fitness[best_index]
-        self.g_best_coords = deepcopy(self.coords[best_index])
-
-    def get_best_score(self):
-        return self.g_best
-
-    def get_best_solution(self):
-        return self.g_best_coords
+from hyponic.optimizers.base_optimizer import BaseOptimizer
+
+import numpy as np
+from copy import deepcopy
+
+class ABC(BaseOptimizer):
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+        self.limits = kwargs.get('limits', 25)  # The number of trials before abandoning a food source
+        self.coords = None
+        self.fitness = None
+        self.g_best = None
+        self.g_best_coords = None
+        self.trials = None
+
+    def initialize(self, problem_dict):
+        super().initialize(problem_dict)
+        self.g_best = np.inf if self._minmax() == min else -np.inf
+
+        self.coords = np.random.uniform(self.lb, self.ub, (self.population_size, self.dimensions))
+        self.fitness = np.array([self.function(self.coords[i]) for i in range(self.population_size)])
+
+        self.trials = np.zeros(self.population_size)
+
+    def _employed_bees_phase(self):
+        for i in range(self.population_size):
+            k = np.random.choice([j for j in range(self.population_size) if j != i])
+            phi = np.random.uniform(-1, 1, self.dimensions)
+            new_coords = self.coords[i] + phi * (self.coords[i] - self.coords[k])
+
+            # TODO: if lb or ub is provided, clip the coordinates
+            new_coords = np.clip(new_coords, self.lb, self.ub)
+            new_fitness = self.function(new_coords)
+            if self._minmax()(np.array([self.fitness[i], new_fitness])) != self.fitness[i]:
+                self.coords[i] = new_coords
+                self.fitness[i] = new_fitness
+                self.trials[i] = 0
+            else:
+                self.trials[i] += 1
+
+    def _onlooker_bees_phase(self):
+        probabilities = self.fitness / np.sum(self.fitness)
+        if np.isnan(probabilities).any():
+            probabilities = np.ones(self.population_size) / self.population_size
+        for i in range(self.population_size):
+            k = np.random.choice([j for j in range(self.population_size)], p=probabilities)
+            phi = np.random.uniform(-1, 1, self.dimensions)
+            new_coords = self.coords[i] + phi * (self.coords[i] - self.coords[k])
+            new_coords = np.clip(new_coords, self.lb, self.ub)
+            new_fitness = self.function(new_coords)
+            if self._minmax()(np.array([self.fitness[i], new_fitness])) != self.fitness[i]:
+                self.coords[i] = new_coords
+                self.fitness[i] = new_fitness
+                self.trials[i] = 0
+            else:
+                self.trials[i] += 1
+
+    def _scout_bees_phase(self):
+        for i in range(self.population_size):
+            if self.trials[i] > self.limits:
+                self.coords[i] = np.random.uniform(self.lb, self.ub, self.dimensions)
+                self.fitness[i] = self.function(self.coords[i])
+                self.trials[i] = 0
+
+    def evolve(self, epoch):
+        self._employed_bees_phase()
+        self._onlooker_bees_phase()
+        self._scout_bees_phase()
+
+        best_index = self._argminmax()(self.fitness)
+        self.g_best = self.fitness[best_index]
+        self.g_best_coords = deepcopy(self.coords[best_index])
+
+    def get_best_score(self):
+        return self.g_best
+
+    def get_best_solution(self):
+        return self.g_best_coords
```

### Comparing `hyponic-0.0.2/hyponic/optimizers/swarm_based/ACO.py` & `hyponic-0.0.3/hyponic/optimizers/swarm_based/ACO.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-from hyponic.optimizers.base_optimizer import BaseOptimizer
-
-import numpy as np
-
-
-class ACO(BaseOptimizer):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.alpha = kwargs.get('alpha', 1)
-        self.beta = kwargs.get('beta', 1)
-        self.rho = kwargs.get('rho', 0.5)
-        self.q = kwargs.get('q', 1)
-
-        self.pheromone = None
-        self.population = None
-        self.scores = None
-        self.best_score = None
-        self.best_solution = None
-
-    def initialize(self, problem_dict):
-        super().initialize(problem_dict)
-
-        self.pheromone = np.ones((self.population_size, self.dimensions))
-        self.best_score = np.inf if self.minmax == 'min' else -np.inf
-
-        self.population = np.random.uniform(low=self.lb, high=self.ub, size=(self.population_size, self.dimensions))
-        self.scores = np.zeros(self.population_size)
-        for i in range(self.population_size):
-            self.scores[i] = self.function(self.population[i])
-            if self._minmax()(self.scores[i]) < self._minmax()(self.best_score):
-                self.best_score = self.scores[i]
-                self.best_solution = self.population[i]
-
-    def evolve(self, epoch):
-        new_population = np.zeros((self.population_size, self.dimensions))
-        new_scores = np.zeros(self.population_size)
-
-        for i in range(self.population_size):
-            ant_position = np.random.uniform(low=self.lb, high=self.ub, size=self.dimensions)
-
-            for j in range(self.dimensions):
-                pheromone_weights = self.pheromone[:, j] ** self.alpha
-                heuristic_weights = 1 / (np.abs(ant_position[j] - self.population[:, j]) + 1e-6) ** self.beta
-                probs = pheromone_weights * heuristic_weights
-                probs /= np.sum(probs)
-                ant_position[j] = np.random.choice(self.population[:, j], p=probs)
-
-            ant_score = self.function(ant_position)
-            self._update_pheromone(ant_score)
-
-            if self._minmax()(ant_score) < self._minmax()(self.best_score):
-                self.best_solution = ant_position
-                self.best_score = ant_score
-
-            new_population[i] = ant_position
-            new_scores[i] = ant_score
-
-        self.population = new_population
-        self.scores = new_scores
-
-    def get_best_score(self):
-        return self.best_score
-
-    def get_best_solution(self):
-        return self.best_solution
-
-    def _initialize_pheromone(self):
-        self.pheromone = np.ones((self.population_size, self.dimensions))
-
-    def _update_pheromone(self, ant_score):
-        delta_pheromone = np.zeros((self.population_size, self.dimensions))
-        delta_pheromone[:, :] = self.q / ant_score
-        self.pheromone = (1 - self.rho) * self.pheromone + self.rho * delta_pheromone
+from hyponic.optimizers.base_optimizer import BaseOptimizer
+
+import numpy as np
+
+
+class ACO(BaseOptimizer):
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.alpha = kwargs.get('alpha', 1)
+        self.beta = kwargs.get('beta', 1)
+        self.rho = kwargs.get('rho', 0.5)
+        self.q = kwargs.get('q', 1)
+
+        self.pheromone = None
+        self.population = None
+        self.scores = None
+        self.best_score = None
+        self.best_solution = None
+
+    def initialize(self, problem_dict):
+        super().initialize(problem_dict)
+
+        self.pheromone = np.ones((self.population_size, self.dimensions))
+        self.best_score = np.inf if self.minmax == 'min' else -np.inf
+
+        self.population = np.random.uniform(low=self.lb, high=self.ub, size=(self.population_size, self.dimensions))
+        self.scores = np.zeros(self.population_size)
+        for i in range(self.population_size):
+            self.scores[i] = self.function(self.population[i])
+            if self._minmax()(self.scores[i]) < self._minmax()(self.best_score):
+                self.best_score = self.scores[i]
+                self.best_solution = self.population[i]
+
+    def evolve(self, epoch):
+        new_population = np.zeros((self.population_size, self.dimensions))
+        new_scores = np.zeros(self.population_size)
+
+        for i in range(self.population_size):
+            ant_position = np.random.uniform(low=self.lb, high=self.ub, size=self.dimensions)
+
+            for j in range(self.dimensions):
+                pheromone_weights = self.pheromone[:, j] ** self.alpha
+                heuristic_weights = 1 / (np.abs(ant_position[j] - self.population[:, j]) + 1e-6) ** self.beta
+                probs = pheromone_weights * heuristic_weights
+                probs /= np.sum(probs)
+                ant_position[j] = np.random.choice(self.population[:, j], p=probs)
+
+            ant_score = self.function(ant_position)
+            self._update_pheromone(ant_score)
+
+            if self._minmax()(ant_score) < self._minmax()(self.best_score):
+                self.best_solution = ant_position
+                self.best_score = ant_score
+
+            new_population[i] = ant_position
+            new_scores[i] = ant_score
+
+        self.population = new_population
+        self.scores = new_scores
+
+    def get_best_score(self):
+        return self.best_score
+
+    def get_best_solution(self):
+        return self.best_solution
+
+    def _initialize_pheromone(self):
+        self.pheromone = np.ones((self.population_size, self.dimensions))
+
+    def _update_pheromone(self, ant_score):
+        delta_pheromone = np.zeros((self.population_size, self.dimensions))
+        delta_pheromone[:, :] = self.q / ant_score
+        self.pheromone = (1 - self.rho) * self.pheromone + self.rho * delta_pheromone
```

### Comparing `hyponic-0.0.2/hyponic/space.py` & `hyponic-0.0.3/hyponic/space.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,125 +1,154 @@
-from typing import Callable, Any
-
-from numpy import clip
-
-
-class Space:
-    def __init__(self, in_dict: dict[str, Any]):
-        self.__dict = dict
-        self.dimensions = {}
-        self.dimensions_names = []
-
-        for key, value in in_dict.items():
-            # Converting range to list
-            if isinstance(value, range):
-                value = list(value)
-
-            if isinstance(value, tuple):
-                if len(value) != 2:
-                    raise ValueError(f'Value for key {key} is not valid')
-                self.dimensions[key] = Continuous(*value, name=key)
-            elif isinstance(value, list):
-                self.dimensions[key] = Discrete(value, name=key)
-            else:
-                raise ValueError(f'Value for key {key} is not valid')
-
-            self.dimensions_names.append(key)
-
-    def get_continuous_mappings(
-            self, scales: dict | int | float = None, origins: dict | int | float = None
-    ) -> dict[str, (Callable, (float, float))]:
-
-        """
-        Returns a function that maps a discrete value to a continuous value.
-        """
-        if scales is None:
-            scales = {}
-        elif isinstance(scales, (int, float)):
-            scales = {key: scales for key in self.dimensions}
-
-        if origins is None:
-            origins = {}
-        elif isinstance(origins, (int, float)):
-            origins = {key: origins for key in self.dimensions}
-
-        mappings = {}
-        for key in self.dimensions:
-            mappings[key] = self.dimensions[key].get_continuous_mapping(
-                scales.get(key, 1),
-                origins.get(key, None)
-            )
-
-        return mappings
-
-    def map_to_original_space(self, values: list[float]) -> dict[str, Any]:
-        """
-        Maps a list of values from the continuous space to the original space.
-        """
-        mappings = self.get_continuous_mappings()
-        return {
-            name: mappings[name][0](value) for name, value in zip(self.dimensions_names, values)
-        }
-
-    def __str__(self):
-        out = f"Space with {len(self.dimensions)} dimensions"
-        for key in self.dimensions:
-            # TODO: pretty print
-            out += f"\n\t{key}:\t{self.dimensions[key]}"
-        return out
-
-
-class Dimension:
-    def __init__(self, lbound, ubound, name=None):
-        self.name = name
-
-        self._lbound = lbound
-        self._ubound = ubound
-
-    def get_continuous_mapping(self, scale=1, origin=None) -> (Callable, (float, float)):
-        """
-        Returns a function that maps set of values to a continuous value
-        """
-        assert scale != 0, "Scale cannot be 0."
-
-        if origin is None:
-            origin = self._lbound
-
-        low = origin
-        high = origin + (self._ubound - self._lbound) * scale
-
-        def mapping_func(x):
-            x = clip(x, low, high)
-            x = self._lbound + (x - origin) / scale
-            return self.get_value(x)
-
-        return mapping_func, (low, high)
-
-    def get_value(self, x):
-        raise NotImplementedError
-
-    def __str__(self):
-        return f"{self.__class__.__name__}({self._lbound}, {self._ubound})"
-
-    def __repr__(self):
-        return self.__str__()
-
-
-class Continuous(Dimension):
-    def __init__(self, low, high, name=None):
-        super().__init__(low, high, name)
-
-    def get_value(self, x):
-        # Note that x is already in the correct range. No need to clip.
-        # > maybe add transformation here? E.g. log, exp, etc.
-        # TODO: non-linear mapping
-        return x
-
-
-class Discrete(Dimension):
-    def __init__(self, values, name=None):
-        super().__init__(0, len(values) - 1, name)
-        self.values = values
-
-    def get_value(self, x):
-        # Note that x is already in the correct range. No need to clip.
-        return self.values[int(x)]
+"""
+This module contains the Space class, which is used to define the search space.
+"""
+import numpy as np
+
+from typing import Callable, Any
+
+
+class Space:
+    """
+    A class that represents the search space of a hyperparameter optimization problem.
+    """
+    def __init__(self, in_dict: dict[str, Any]):
+        self.__dict = dict
+        self.dimensions = {}
+        self.dimensions_names = []
+
+        for k, v in in_dict.items():
+            # Converting range to list
+            if isinstance(v, range):
+                v = list(v)
+
+            if isinstance(v, Discrete):
+                self.dimensions[k] = v
+            elif isinstance(v, Continuous):
+                self.dimensions[k] = v
+            elif isinstance(v, tuple):
+                if len(v) != 2:
+                    raise ValueError(f"Value for key {k} is not valid")
+
+                self.dimensions[k] = Continuous(*v, name=k)
+            elif isinstance(v, list):
+                self.dimensions[k] = Discrete(v, name=k)
+            else:
+                raise ValueError(f"Value for key {k} is not valid")
+
+            self.dimensions_names.append(k)
+
+    def get_continuous_mappings(
+            self, scales: dict | int | float = None, origins: dict | int | float = None
+    ) -> dict[str, (Callable, (float, float))]:
+        """
+        Returns a function that maps a discrete value to a continuous value.
+        """
+
+        if scales is None:
+            scales = {}
+        elif isinstance(scales, (int, float)):
+            scales = {key: scales for key in self.dimensions}
+
+        if origins is None:
+            origins = {}
+        elif isinstance(origins, (int, float)):
+            origins = {key: origins for key in self.dimensions}
+
+        mappings = {}
+        for key in self.dimensions:
+            mappings[key] = self.dimensions[key].get_continuous_mapping(
+                scales.get(key, 1),
+                origins.get(key, None)
+            )
+
+        return mappings
+
+    def map_to_original_space(self, values: list[float]) -> dict[str, Any]:
+        """
+        Maps a list of values from the continuous space to the original space.
+        """
+        mappings = self.get_continuous_mappings()
+        return {
+            name: mappings[name][0](value) for name, value in zip(self.dimensions_names, values)
+        }
+
+    def __str__(self):
+        if len(self.dimensions) == 0:
+            return "Hyperparameter Search Space is empty."
+
+        # Pretty table of dimensions
+        dim_names = list(self.dimensions.keys())
+        offset = max([len(k) for k in dim_names])
+
+        out_strs = [f"Hyperparameter Search Space with {len(dim_names)} dimensions:"]
+        out_strs += [
+            f"\t{k}: {'-'*(offset - len(k))} {self.dimensions[k]}" for k in dim_names
+        ]
+
+        return "\n".join(out_strs)
+
+
+class Dimension:
+    def __init__(self, lbound, ubound, name=None):
+        self.name = name
+
+        self._lbound = lbound
+        self._ubound = ubound
+
+    def get_continuous_mapping(self, scale=1, origin=None) -> (Callable, (float, float)):
+        """
+        Returns a function that maps set of values to a continuous value
+        """
+        assert scale != 0, "Scale cannot be 0."
+
+        if origin is None:
+            origin = self._lbound
+
+        low = origin
+        high = origin + (self._ubound - self._lbound) * scale
+
+        def mapping_func(x):
+            x = np.clip(x, low, high)
+            x = self._lbound + (x - origin) / scale
+            return self.get_value(x)
+
+        return mapping_func, (low, high)
+
+    def get_value(self, x):
+        raise NotImplementedError
+
+    def __str__(self):
+        return self.__class__.__name__
+
+    def __repr__(self):
+        return self.__str__()
+
+
+class Continuous(Dimension):
+    def __init__(self, low, high, name=None):
+        super().__init__(low, high, name)
+
+    def get_value(self, x):
+        # Note that x is already in the correct range. No need to clip.
+        return x
+
+    def __str__(self):
+        return super().__str__() + f"({self._lbound}, {self._ubound})"
+
+    def __repr__(self):
+        return self.__str__()
+
+
+class Discrete(Dimension):
+    def __init__(self, values, name=None):
+        super().__init__(0, len(values), name)
+        self.values = np.array(values)
+
+    def get_value(self, x):
+        x = np.clip(x, 0, len(self.values) - 1)
+        return self.values[int(x)]
+
+    def __str__(self):
+        return super().__str__() + f"{self.values}"
+
+    def __repr__(self):
+        return self.__str__()
```

### Comparing `hyponic-0.0.2/hyponic.egg-info/SOURCES.txt` & `hyponic-0.0.3/hyponic.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 README.md
 setup.py
 hyponic/__init__.py
 hyponic/hyponic.py
 hyponic/space.py
-hyponic/symtable.py
 hyponic.egg-info/PKG-INFO
 hyponic.egg-info/SOURCES.txt
 hyponic.egg-info/dependency_links.txt
 hyponic.egg-info/requires.txt
 hyponic.egg-info/top_level.txt
 hyponic/metrics/__init__.py
 hyponic/metrics/classification.py
```

