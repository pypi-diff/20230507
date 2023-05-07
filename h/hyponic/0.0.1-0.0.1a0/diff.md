# Comparing `tmp/hyponic-0.0.1.tar.gz` & `tmp/hyponic-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyponic-0.0.1.tar", last modified: Sun May  7 08:05:47 2023, max compression
+gzip compressed data, was "hyponic-0.0.1a0.tar", last modified: Sun May  7 10:19:05 2023, max compression
```

## Comparing `hyponic-0.0.1.tar` & `hyponic-0.0.1a0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 08:05:47.273505 hyponic-0.0.1/
--rw-rw-rw-   0        0        0     1095 2023-05-07 07:36:12.000000 hyponic-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     4890 2023-05-07 08:05:47.271995 hyponic-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4266 2023-05-07 07:24:04.000000 hyponic-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 08:05:47.249928 hyponic-0.0.1/hyponic/
--rw-rw-rw-   0        0        0      568 2023-05-07 08:05:21.000000 hyponic-0.0.1/hyponic/__init__.py
--rw-rw-rw-   0        0        0     3816 2023-05-07 07:23:55.000000 hyponic-0.0.1/hyponic/metrics.py
--rw-rw-rw-   0        0        0     4487 2023-05-04 11:45:00.000000 hyponic-0.0.1/hyponic/optimizer.py
-drwxrwxrwx   0        0        0        0 2023-05-07 08:05:47.270995 hyponic-0.0.1/hyponic/optimizers/
--rw-rw-rw-   0        0        0     3317 2023-05-07 07:36:12.000000 hyponic-0.0.1/hyponic/optimizers/ABC.py
--rw-rw-rw-   0        0        0     2897 2023-05-07 07:36:12.000000 hyponic-0.0.1/hyponic/optimizers/ACO.py
--rw-rw-rw-   0        0        0     3086 2023-05-07 07:36:12.000000 hyponic-0.0.1/hyponic/optimizers/GA.py
--rw-rw-rw-   0        0        0     3001 2023-05-07 07:36:12.000000 hyponic-0.0.1/hyponic/optimizers/PSO.py
--rw-rw-rw-   0        0        0     1689 2023-05-04 13:23:32.000000 hyponic-0.0.1/hyponic/optimizers/SA.py
--rw-rw-rw-   0        0        0        0 2023-05-07 08:03:05.000000 hyponic-0.0.1/hyponic/optimizers/__init__.py
--rw-rw-rw-   0        0        0     2535 2023-05-04 13:23:19.000000 hyponic-0.0.1/hyponic/optimizers/base_optimizer.py
--rw-rw-rw-   0        0        0     4001 2023-04-25 06:50:09.000000 hyponic-0.0.1/hyponic/space.py
--rw-rw-rw-   0        0        0     1546 2023-04-23 15:51:05.000000 hyponic-0.0.1/hyponic/symtable.py
-drwxrwxrwx   0        0        0        0 2023-05-07 08:05:47.262463 hyponic-0.0.1/hyponic.egg-info/
--rw-rw-rw-   0        0        0     4890 2023-05-07 08:05:47.000000 hyponic-0.0.1/hyponic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-05-07 08:05:47.000000 hyponic-0.0.1/hyponic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 08:05:47.000000 hyponic-0.0.1/hyponic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-07 08:05:47.000000 hyponic-0.0.1/hyponic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-07 08:05:47.000000 hyponic-0.0.1/hyponic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 08:05:47.273505 hyponic-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      865 2023-05-07 08:05:21.000000 hyponic-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:19:05.920322 hyponic-0.0.1a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 10:18:51.000000 hyponic-0.0.1a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-07 10:19:05.920322 hyponic-0.0.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-07 10:18:51.000000 hyponic-0.0.1a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:19:05.920322 hyponic-0.0.1a0/hyponic/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-07 10:18:51.000000 hyponic-0.0.1a0/hyponic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-07 10:18:51.000000 hyponic-0.0.1a0/hyponic/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-07 10:18:51.000000 hyponic-0.0.1a0/hyponic/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:19:05.920322 hyponic-0.0.1a0/hyponic/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-07 10:18:51.000000 hyponic-0.0.1a0/hyponic/optimizers/ABC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-07 10:18:51.000000 hyponic-0.0.1a0/hyponic/optimizers/ACO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-07 10:18:51.000000 hyponic-0.0.1a0/hyponic/optimizers/GA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-07 10:18:51.000000 hyponic-0.0.1a0/hyponic/optimizers/PSO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-07 10:18:51.000000 hyponic-0.0.1a0/hyponic/optimizers/SA.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 10:18:51.000000 hyponic-0.0.1a0/hyponic/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-07 10:18:51.000000 hyponic-0.0.1a0/hyponic/optimizers/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-07 10:18:51.000000 hyponic-0.0.1a0/hyponic/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-07 10:18:51.000000 hyponic-0.0.1a0/hyponic/symtable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 10:19:05.920322 hyponic-0.0.1a0/hyponic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-07 10:19:05.000000 hyponic-0.0.1a0/hyponic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-07 10:19:05.000000 hyponic-0.0.1a0/hyponic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 10:19:05.000000 hyponic-0.0.1a0/hyponic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-07 10:19:05.000000 hyponic-0.0.1a0/hyponic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-07 10:19:05.000000 hyponic-0.0.1a0/hyponic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 10:19:05.920322 hyponic-0.0.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-07 10:18:51.000000 hyponic-0.0.1a0/setup.py
```

### Comparing `hyponic-0.0.1/PKG-INFO` & `hyponic-0.0.1a0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,138 +1,134 @@
-Metadata-Version: 2.1
-Name: hyponic
-Version: 0.0.1
-Summary: Hyperparameter Optimization with Nature-Inspired Computing
-Home-page: https://github.com/slewie/HypONIC
-Author: Vladislav Kulikov, Daniel Satarov, Ivan Chernakov
-Author-email: v.kulikov@innopolis.university, d.satarov@innopolis.university, i.chernakov@innopolis.university
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# HypONIC -- Hyperparameter Optimization with Nature Inspired Computing
-
-*HypONIC* is a hyperparameter optimization library that uses various nature inspired computing algorithms to optimize
-the hyperparameters of machine learning models. The library provides a simple interface for sklearn and keras models.
-
-## Implementation details
-*HypONIC* library follows a common high-level approach by providing a unified interface for applying an optimization algorithm
-of choice to the parameters of a machine learning model (based on the `BaseEstimator` from the `sklearn`). Evalution of the
-optimization process is done by a metric of choice.
-
-### Metrics
-*HypONIC* provides a list of classical evalution metrics:
-
-- Mean Squared Error
-- Mean Absolute Error
-- Root Mean Square Error
-- Huber Loss
-- Log Loss
-- Binary Crossentropy
-- Precision Score
-- Accuracy Score
-- Recall Score
-- F1 Score
-- R2 Score
-- ...and many others.
-
-*HypONIC* library provides decorators for annotating custom metrics: `@minimize_metric` and `@maximize_metric`. These decorators
-allows using names of the metric functions as string literals instead of passing the function itself, i.e.
-
-```python
-from hyponic.optimizer import HypONIC
-...
-hyponic = HypONIC(model, X, y, "mse", **optimizer_kwargs)
-...
-```
-
-instead of
-
-```python
-from hyponic.optimizer import HypONIC
-from hyponic.metrics import mse
-...
-hyponic = HypONIC(model, X, y, mse, **optimizer_kwargs)
-...
-```
-
-### Hyperparameter Space
-*HypONIC* library supports mixed space of hyperparameters, meaning that one optimization space can have both
-dimensions of discrete and continuous parameters. The notation for each space is the following:
-
-```python
-hyperparams = {
-    "min_impurity_decrease": (0.0, 0.9),              # Continious space -- (lower bound, upper bound)
-    "min_samples_split": [2, 3, 4, 5, 6],             # Discrete space   -- a list of values of any type
-    "criterion": ["absolute_error", "squared_error"]  # Discrete space   -- a list of values of any type
-}
-```
-
-For the discrete space an automatic uniform mapping* to the continious space is provided if needed. Discrete space of
-non numerical values is encoded first and then uniformly mapped to the continious space.
-
-*is subject to change
-
-## Features
-*HypONIC* supports different nature inspired computing algorithms.
-Please note that the library is currently under development and may contain a significant number of bugs and errors.
-All algorithms are subject to further improvement.
-
-The following algorithms are currently implemented or are planned to be implemented:
-
-**Swarm-based:**
-- - [x] Particle Swarm Optimization (PSO)
-- - [x] Inertia Weight PSO (IWPSO)
-- - [x] Ant Colony Optimization (ACO)
-- - [x] Artificial Bee Colony (ABC)
-- - [ ] Grey Wolf Optimizer (GWO)
-- - [ ] Cuckoo Search (CS)
-- - [ ] Firefly Algorithm (FA)
-
-**Physics-based:**
-- - [x] Simulated Annealing (SA)
-
-**Genetic-based:**
-- - [x] Genetic Algorithm
-
-## Minimal Example
-
-This is a minimal example for tuning hyperparameters of the `RandomForestRegressor` from `sklearn`. The default optimizator is *Inertia Weight Particle Swarm Optimization* (IWPSO), as it has high applicability and has shown fast convergence.
-
-```python
-from sklearn.datasets import load_diabetes
-from sklearn.ensemble import RandomForestRegressor
-
-from hyponic.metrics import mse
-from hyponic.optimizer import HypONIC
-
-X, y = load_diabetes(return_X_y=True)
-model = RandomForestRegressor()
-
-hyperparams = {
-    "min_samples_split": (0.01, 0.9),  # Continious space
-    "min_samples_leaf": (0.01, 0.9),  # Continious space
-    "min_weight_fraction_leaf": (0.0, 0.5),  # Continious space
-    "min_impurity_decrease": (0.0, 0.9),  # Continious space
-    "criterion": ["absolute_error", "squared_error"]  # Discrete space
-}
-
-optimizer_kwargs = {
-    "epoch": 50,
-    "pop_size": 50,
-}
-
-# The default optimizator is the Inertia Weight Particle Swarm Optimization (IWPSO)
-hyponic = HypONIC(model, X, y, mse, **optimizer_kwargs)
-hyponic.optimize(hyperparams, verbose=True)
-
-print(hyponic.get_optimized_parameters())
-print(hyponic.get_optimized_metric())
-print(hyponic.get_optimized_model())
-```
-
-
+Metadata-Version: 2.1
+Name: hyponic
+Version: 0.0.1a0
+Summary: Hyperparameter Optimization with Nature-Inspired Computing
+Home-page: https://github.com/slewie/HypONIC
+Author: Vladislav Kulikov, Daniel Satarov, Ivan Chernakov
+Author-email: v.kulikov@innopolis.university, d.satarov@innopolis.university, i.chernakov@innopolis.university
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# HypONIC -- Hyperparameter Optimization with Nature Inspired Computing
+
+*HypONIC* is a hyperparameter optimization library that uses various nature inspired computing algorithms to optimize
+the hyperparameters of machine learning models. The library provides a simple interface for sklearn and keras models.
+
+## Implementation details
+*HypONIC* library follows a common high-level approach by providing a unified interface for applying an optimization algorithm
+of choice to the parameters of a machine learning model (based on the `BaseEstimator` from the `sklearn`). Evalution of the
+optimization process is done by a metric of choice.
+
+### Metrics
+*HypONIC* provides a list of classical evalution metrics:
+
+- Mean Squared Error
+- Mean Absolute Error
+- Root Mean Square Error
+- Huber Loss
+- Log Loss
+- Binary Crossentropy
+- Precision Score
+- Accuracy Score
+- Recall Score
+- F1 Score
+- R2 Score
+- ...and many others.
+
+*HypONIC* library provides decorators for annotating custom metrics: `@minimize_metric` and `@maximize_metric`. These decorators
+allows using names of the metric functions as string literals instead of passing the function itself, i.e.
+
+```python
+from hyponic.optimizer import HypONIC
+...
+hyponic = HypONIC(model, X, y, "mse", **optimizer_kwargs)
+...
+```
+
+instead of
+
+```python
+from hyponic.optimizer import HypONIC
+from hyponic.metrics import mse
+...
+hyponic = HypONIC(model, X, y, mse, **optimizer_kwargs)
+...
+```
+
+### Hyperparameter Space
+*HypONIC* library supports mixed space of hyperparameters, meaning that one optimization space can have both
+dimensions of discrete and continuous parameters. The notation for each space is the following:
+
+```python
+hyperparams = {
+    "min_impurity_decrease": (0.0, 0.9),              # Continious space -- (lower bound, upper bound)
+    "min_samples_split": [2, 3, 4, 5, 6],             # Discrete space   -- a list of values of any type
+    "criterion": ["absolute_error", "squared_error"]  # Discrete space   -- a list of values of any type
+}
+```
+
+For the discrete space an automatic uniform mapping* to the continious space is provided if needed. Discrete space of
+non numerical values is encoded first and then uniformly mapped to the continious space.
+
+*is subject to change
+
+## Features
+*HypONIC* supports different nature inspired computing algorithms.
+Please note that the library is currently under development and may contain a significant number of bugs and errors.
+All algorithms are subject to further improvement.
+
+The following algorithms are currently implemented or are planned to be implemented:
+
+**Swarm-based:**
+- - [x] Particle Swarm Optimization (PSO)
+- - [x] Inertia Weight PSO (IWPSO)
+- - [x] Ant Colony Optimization (ACO)
+- - [x] Artificial Bee Colony (ABC)
+- - [ ] Grey Wolf Optimizer (GWO)
+- - [ ] Cuckoo Search (CS)
+- - [ ] Firefly Algorithm (FA)
+
+**Physics-based:**
+- - [x] Simulated Annealing (SA)
+
+**Genetic-based:**
+- - [x] Genetic Algorithm
+
+## Minimal Example
+
+This is a minimal example for tuning hyperparameters of the `RandomForestRegressor` from `sklearn`. The default optimizator is *Inertia Weight Particle Swarm Optimization* (IWPSO), as it has high applicability and has shown fast convergence.
+
+```python
+from sklearn.datasets import load_diabetes
+from sklearn.ensemble import RandomForestRegressor
+
+from hyponic.metrics import mse
+from hyponic.optimizer import HypONIC
+
+X, y = load_diabetes(return_X_y=True)
+model = RandomForestRegressor()
+
+hyperparams = {
+    "min_samples_split": (0.01, 0.9),  # Continious space
+    "min_samples_leaf": (0.01, 0.9),  # Continious space
+    "min_weight_fraction_leaf": (0.0, 0.5),  # Continious space
+    "min_impurity_decrease": (0.0, 0.9),  # Continious space
+    "criterion": ["absolute_error", "squared_error"]  # Discrete space
+}
+
+optimizer_kwargs = {
+    "epoch": 50,
+    "pop_size": 50,
+}
+
+# The default optimizator is the Inertia Weight Particle Swarm Optimization (IWPSO)
+hyponic = HypONIC(model, X, y, mse, **optimizer_kwargs)
+hyponic.optimize(hyperparams, verbose=True)
+
+print(hyponic.get_optimized_parameters())
+print(hyponic.get_optimized_metric())
+print(hyponic.get_optimized_model())
+```
```

### Comparing `hyponic-0.0.1/README.md` & `hyponic-0.0.1a0/README.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-# HypONIC -- Hyperparameter Optimization with Nature Inspired Computing
-
-*HypONIC* is a hyperparameter optimization library that uses various nature inspired computing algorithms to optimize
-the hyperparameters of machine learning models. The library provides a simple interface for sklearn and keras models.
-
-## Implementation details
-*HypONIC* library follows a common high-level approach by providing a unified interface for applying an optimization algorithm
-of choice to the parameters of a machine learning model (based on the `BaseEstimator` from the `sklearn`). Evalution of the
-optimization process is done by a metric of choice.
-
-### Metrics
-*HypONIC* provides a list of classical evalution metrics:
-
-- Mean Squared Error
-- Mean Absolute Error
-- Root Mean Square Error
-- Huber Loss
-- Log Loss
-- Binary Crossentropy
-- Precision Score
-- Accuracy Score
-- Recall Score
-- F1 Score
-- R2 Score
-- ...and many others.
-
-*HypONIC* library provides decorators for annotating custom metrics: `@minimize_metric` and `@maximize_metric`. These decorators
-allows using names of the metric functions as string literals instead of passing the function itself, i.e.
-
-```python
-from hyponic.optimizer import HypONIC
-...
-hyponic = HypONIC(model, X, y, "mse", **optimizer_kwargs)
-...
-```
-
-instead of
-
-```python
-from hyponic.optimizer import HypONIC
-from hyponic.metrics import mse
-...
-hyponic = HypONIC(model, X, y, mse, **optimizer_kwargs)
-...
-```
-
-### Hyperparameter Space
-*HypONIC* library supports mixed space of hyperparameters, meaning that one optimization space can have both
-dimensions of discrete and continuous parameters. The notation for each space is the following:
-
-```python
-hyperparams = {
-    "min_impurity_decrease": (0.0, 0.9),              # Continious space -- (lower bound, upper bound)
-    "min_samples_split": [2, 3, 4, 5, 6],             # Discrete space   -- a list of values of any type
-    "criterion": ["absolute_error", "squared_error"]  # Discrete space   -- a list of values of any type
-}
-```
-
-For the discrete space an automatic uniform mapping* to the continious space is provided if needed. Discrete space of
-non numerical values is encoded first and then uniformly mapped to the continious space.
-
-*is subject to change
-
-## Features
-*HypONIC* supports different nature inspired computing algorithms.
-Please note that the library is currently under development and may contain a significant number of bugs and errors.
-All algorithms are subject to further improvement.
-
-The following algorithms are currently implemented or are planned to be implemented:
-
-**Swarm-based:**
-- - [x] Particle Swarm Optimization (PSO)
-- - [x] Inertia Weight PSO (IWPSO)
-- - [x] Ant Colony Optimization (ACO)
-- - [x] Artificial Bee Colony (ABC)
-- - [ ] Grey Wolf Optimizer (GWO)
-- - [ ] Cuckoo Search (CS)
-- - [ ] Firefly Algorithm (FA)
-
-**Physics-based:**
-- - [x] Simulated Annealing (SA)
-
-**Genetic-based:**
-- - [x] Genetic Algorithm
-
-## Minimal Example
-
-This is a minimal example for tuning hyperparameters of the `RandomForestRegressor` from `sklearn`. The default optimizator is *Inertia Weight Particle Swarm Optimization* (IWPSO), as it has high applicability and has shown fast convergence.
-
-```python
-from sklearn.datasets import load_diabetes
-from sklearn.ensemble import RandomForestRegressor
-
-from hyponic.metrics import mse
-from hyponic.optimizer import HypONIC
-
-X, y = load_diabetes(return_X_y=True)
-model = RandomForestRegressor()
-
-hyperparams = {
-    "min_samples_split": (0.01, 0.9),  # Continious space
-    "min_samples_leaf": (0.01, 0.9),  # Continious space
-    "min_weight_fraction_leaf": (0.0, 0.5),  # Continious space
-    "min_impurity_decrease": (0.0, 0.9),  # Continious space
-    "criterion": ["absolute_error", "squared_error"]  # Discrete space
-}
-
-optimizer_kwargs = {
-    "epoch": 50,
-    "pop_size": 50,
-}
-
-# The default optimizator is the Inertia Weight Particle Swarm Optimization (IWPSO)
-hyponic = HypONIC(model, X, y, mse, **optimizer_kwargs)
-hyponic.optimize(hyperparams, verbose=True)
-
-print(hyponic.get_optimized_parameters())
-print(hyponic.get_optimized_metric())
-print(hyponic.get_optimized_model())
-```
+# HypONIC -- Hyperparameter Optimization with Nature Inspired Computing
+
+*HypONIC* is a hyperparameter optimization library that uses various nature inspired computing algorithms to optimize
+the hyperparameters of machine learning models. The library provides a simple interface for sklearn and keras models.
+
+## Implementation details
+*HypONIC* library follows a common high-level approach by providing a unified interface for applying an optimization algorithm
+of choice to the parameters of a machine learning model (based on the `BaseEstimator` from the `sklearn`). Evalution of the
+optimization process is done by a metric of choice.
+
+### Metrics
+*HypONIC* provides a list of classical evalution metrics:
+
+- Mean Squared Error
+- Mean Absolute Error
+- Root Mean Square Error
+- Huber Loss
+- Log Loss
+- Binary Crossentropy
+- Precision Score
+- Accuracy Score
+- Recall Score
+- F1 Score
+- R2 Score
+- ...and many others.
+
+*HypONIC* library provides decorators for annotating custom metrics: `@minimize_metric` and `@maximize_metric`. These decorators
+allows using names of the metric functions as string literals instead of passing the function itself, i.e.
+
+```python
+from hyponic.optimizer import HypONIC
+...
+hyponic = HypONIC(model, X, y, "mse", **optimizer_kwargs)
+...
+```
+
+instead of
+
+```python
+from hyponic.optimizer import HypONIC
+from hyponic.metrics import mse
+...
+hyponic = HypONIC(model, X, y, mse, **optimizer_kwargs)
+...
+```
+
+### Hyperparameter Space
+*HypONIC* library supports mixed space of hyperparameters, meaning that one optimization space can have both
+dimensions of discrete and continuous parameters. The notation for each space is the following:
+
+```python
+hyperparams = {
+    "min_impurity_decrease": (0.0, 0.9),              # Continious space -- (lower bound, upper bound)
+    "min_samples_split": [2, 3, 4, 5, 6],             # Discrete space   -- a list of values of any type
+    "criterion": ["absolute_error", "squared_error"]  # Discrete space   -- a list of values of any type
+}
+```
+
+For the discrete space an automatic uniform mapping* to the continious space is provided if needed. Discrete space of
+non numerical values is encoded first and then uniformly mapped to the continious space.
+
+*is subject to change
+
+## Features
+*HypONIC* supports different nature inspired computing algorithms.
+Please note that the library is currently under development and may contain a significant number of bugs and errors.
+All algorithms are subject to further improvement.
+
+The following algorithms are currently implemented or are planned to be implemented:
+
+**Swarm-based:**
+- - [x] Particle Swarm Optimization (PSO)
+- - [x] Inertia Weight PSO (IWPSO)
+- - [x] Ant Colony Optimization (ACO)
+- - [x] Artificial Bee Colony (ABC)
+- - [ ] Grey Wolf Optimizer (GWO)
+- - [ ] Cuckoo Search (CS)
+- - [ ] Firefly Algorithm (FA)
+
+**Physics-based:**
+- - [x] Simulated Annealing (SA)
+
+**Genetic-based:**
+- - [x] Genetic Algorithm
+
+## Minimal Example
+
+This is a minimal example for tuning hyperparameters of the `RandomForestRegressor` from `sklearn`. The default optimizator is *Inertia Weight Particle Swarm Optimization* (IWPSO), as it has high applicability and has shown fast convergence.
+
+```python
+from sklearn.datasets import load_diabetes
+from sklearn.ensemble import RandomForestRegressor
+
+from hyponic.metrics import mse
+from hyponic.optimizer import HypONIC
+
+X, y = load_diabetes(return_X_y=True)
+model = RandomForestRegressor()
+
+hyperparams = {
+    "min_samples_split": (0.01, 0.9),  # Continious space
+    "min_samples_leaf": (0.01, 0.9),  # Continious space
+    "min_weight_fraction_leaf": (0.0, 0.5),  # Continious space
+    "min_impurity_decrease": (0.0, 0.9),  # Continious space
+    "criterion": ["absolute_error", "squared_error"]  # Discrete space
+}
+
+optimizer_kwargs = {
+    "epoch": 50,
+    "pop_size": 50,
+}
+
+# The default optimizator is the Inertia Weight Particle Swarm Optimization (IWPSO)
+hyponic = HypONIC(model, X, y, mse, **optimizer_kwargs)
+hyponic.optimize(hyperparams, verbose=True)
+
+print(hyponic.get_optimized_parameters())
+print(hyponic.get_optimized_metric())
+print(hyponic.get_optimized_model())
+```
```

### Comparing `hyponic-0.0.1/hyponic/__init__.py` & `hyponic-0.0.1a0/hyponic/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-__version__ = '0.0.1'
-
-from .optimizer import HypONIC
-from .optimizers.PSO import PSO, IWPSO
-from .optimizers.ABC import ABC
-from .optimizers.SA import SA
-from .optimizers.base_optimizer import BaseOptimizer
-from .optimizers.GA import GA
-from .optimizers.ACO import ACO
-from .metrics import MetricInfo, METRICS_DICT, accuracy, precision, recall, fbeta, f1, mse, rmse, mae, r2, adjusted_r2, \
-    huber_loss, log_loss, binary_crossentropy, categorical_crossentropy, minimize_metric, maximize_metric
-from .space import Space, Dimension, Continuous, Discrete
+__version__ = '0.0.1-alpha-0'
+
+from .optimizer import HypONIC
+from .optimizers.PSO import PSO, IWPSO
+from .optimizers.ABC import ABC
+from .optimizers.SA import SA
+from .optimizers.base_optimizer import BaseOptimizer
+from .optimizers.GA import GA
+from .optimizers.ACO import ACO
+from .metrics import MetricInfo, METRICS_DICT, accuracy, precision, recall, fbeta, f1, mse, rmse, mae, r2, adjusted_r2, \
+    huber_loss, log_loss, binary_crossentropy, categorical_crossentropy, minimize_metric, maximize_metric
+from .space import Space, Dimension, Continuous, Discrete
```

### Comparing `hyponic-0.0.1/hyponic/metrics.py` & `hyponic-0.0.1a0/hyponic/metrics.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-from collections import defaultdict
-
-import numpy as np
-
-METRICS_DICT = defaultdict()
-
-
-def minimize_metric(metric):
-    metric.minmax = "min"
-    METRICS_DICT[metric.__name__] = metric
-    return metric
-
-
-def maximize_metric(metric):
-    metric.minmax = "max"
-    METRICS_DICT[metric.__name__] = metric
-    return metric
-
-
-class MetricInfo:
-    def __init__(self, info):
-        self.__info = info
-
-    def __str__(self):
-        if self.__info is None:
-            return self.__name__ + " provides no information."
-
-        return self.__info
-
-    def __call__(self, *args, **kwargs):
-        print(self.__info)
-        return self.__info
-
-
-def add_metric_info(info):
-    def decorator(metric):
-        metric.info = MetricInfo(info)
-        return metric
-
-    return decorator
-
-
-@add_metric_info("Mean Squared Error (MSE) is the average of the squared error that is used as the loss function.")
-@minimize_metric
-def mse(y_true: np.array, y_pred: np.array) -> np.ndarray:
-    return np.mean(np.square(y_true - y_pred))
-
-
-@minimize_metric
-def mae(y_true: np.array, y_pred: np.array) -> np.ndarray:
-    return np.mean(np.abs(y_true - y_pred))
-
-
-@minimize_metric
-def rmse(y_true: np.array, y_pred: np.array) -> np.ndarray:
-    return np.sqrt(np.mean(np.square(y_true - y_pred)))
-
-
-@maximize_metric
-def r2(y_true: np.array, y_pred: np.array) -> np.ndarray:
-    return 1 - np.sum(np.square(y_true - y_pred)) / np.sum(np.square(y_true - np.mean(y_true)))
-
-
-@maximize_metric
-def adjusted_r2(y_true: np.array, y_pred: np.array) -> np.ndarray:
-    return 1 - (1 - r2(y_true, y_pred)) * (len(y_true) - 1) / (len(y_true) - len(y_true[0]) - 1)
-
-
-@minimize_metric
-def huber_loss(y_true: np.array, y_pred: np.array, delta: float = 1.0) -> np.ndarray:
-    error = y_true - y_pred
-    return np.where(np.abs(error) <= delta, 0.5 * np.square(error), delta * (np.abs(error) - 0.5 * delta))
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
-def f1(y_true: np.array, y_pred: np.array) -> np.ndarray:
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
+from collections import defaultdict
+
+import numpy as np
+
+METRICS_DICT = defaultdict()
+
+
+def minimize_metric(metric):
+    metric.minmax = "min"
+    METRICS_DICT[metric.__name__] = metric
+    return metric
+
+
+def maximize_metric(metric):
+    metric.minmax = "max"
+    METRICS_DICT[metric.__name__] = metric
+    return metric
+
+
+class MetricInfo:
+    def __init__(self, info):
+        self.__info = info
+
+    def __str__(self):
+        if self.__info is None:
+            return self.__name__ + " provides no information."
+
+        return self.__info
+
+    def __call__(self, *args, **kwargs):
+        print(self.__info)
+        return self.__info
+
+
+def add_metric_info(info):
+    def decorator(metric):
+        metric.info = MetricInfo(info)
+        return metric
+
+    return decorator
+
+
+@add_metric_info("Mean Squared Error (MSE) is the average of the squared error that is used as the loss function.")
+@minimize_metric
+def mse(y_true: np.array, y_pred: np.array) -> np.ndarray:
+    return np.mean(np.square(y_true - y_pred))
+
+
+@minimize_metric
+def mae(y_true: np.array, y_pred: np.array) -> np.ndarray:
+    return np.mean(np.abs(y_true - y_pred))
+
+
+@minimize_metric
+def rmse(y_true: np.array, y_pred: np.array) -> np.ndarray:
+    return np.sqrt(np.mean(np.square(y_true - y_pred)))
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
+
+
+@minimize_metric
+def log_loss(y_true: np.array, y_pred: np.array) -> np.ndarray:
+    return np.mean(np.log(1 + np.exp(-y_true * y_pred)))
+
+
+@minimize_metric
+def binary_crossentropy(y_true: np.array, y_pred: np.array) -> np.ndarray:
+    return -np.mean(y_true * np.log(y_pred) + (1 - y_true) * np.log(1 - y_pred))
+
+
+@minimize_metric
+def categorical_crossentropy(y_true: np.array, y_pred: np.array) -> np.ndarray:
+    return -np.mean(np.sum(y_true * np.log(y_pred), axis=-1))
+
+
+@maximize_metric
+def accuracy(y_true: np.array, y_pred: np.array) -> np.ndarray:
+    return np.mean(np.equal(y_true, y_pred))
+
+
+@maximize_metric
+def precision(y_true: np.array, y_pred: np.array) -> np.ndarray:
+    tp = np.sum(np.logical_and(y_true == 1, y_pred == 1))
+    fp = np.sum(np.logical_and(y_true == 0, y_pred == 1))
+    return tp / (tp + fp)
+
+
+@maximize_metric
+def recall(y_true: np.array, y_pred: np.array) -> np.ndarray:
+    tp = np.sum(np.logical_and(y_true == 1, y_pred == 1))
+    fn = np.sum(np.logical_and(y_true == 1, y_pred == 0))
+    return tp / (tp + fn)
+
+
+@maximize_metric
+def f1(y_true: np.array, y_pred: np.array) -> np.ndarray:
+    p = precision(y_true, y_pred)
+    r = recall(y_true, y_pred)
+    return 2 * p * r / (p + r)
+
+
+@maximize_metric
+def fbeta(y_true: np.array, y_pred: np.array, beta: float = 1.0) -> np.ndarray:
+    p = precision(y_true, y_pred)
+    r = recall(y_true, y_pred)
+    return (1 + beta ** 2) * p * r / (beta ** 2 * p + r)
+
+
+@maximize_metric
+def confusion_matrix(y_true: np.array, y_pred: np.array) -> np.ndarray:
+    tp = np.sum(np.logical_and(y_true == 1, y_pred == 1))
+    fp = np.sum(np.logical_and(y_true == 0, y_pred == 1))
+    fn = np.sum(np.logical_and(y_true == 1, y_pred == 0))
+    tn = np.sum(np.logical_and(y_true == 0, y_pred == 0))
+    return np.array([[tp, fp], [fn, tn]])
```

### Comparing `hyponic-0.0.1/hyponic/optimizer.py` & `hyponic-0.0.1a0/hyponic/optimizer.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-from warnings import warn
-
-from hyponic.optimizers.PSO import IWPSO
-from hyponic.metrics import METRICS_DICT
-
-from typing import Callable
-
-from hyponic.space import Space
-from functools import partial
-
-
-class HypONIC:
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
-    def not_optimized_error(func):
-        """
-        Decorator for checking if model is optimized
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
-    @not_optimized_error
-    def get_optimized_model(self):
-        self.model.set_params(**self.hyperparams_optimized)
-        self.model.fit(self.X, self.y)
-        return self.model
-
-    @not_optimized_error
-    def get_optimized_parameters(self) -> dict:
-        return self.hyperparams_optimized
-
-    @not_optimized_error
-    def get_optimized_metric(self) -> float:
-        return self.metric_optimized
+from warnings import warn
+
+from hyponic.optimizers.PSO import IWPSO
+from hyponic.metrics import METRICS_DICT
+
+from typing import Callable
+
+from hyponic.space import Space
+from functools import partial
+
+
+class HypONIC:
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
+    def not_optimized_error(func):
+        """
+        Decorator for checking if model is optimized
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
+    @not_optimized_error
+    def get_optimized_model(self):
+        self.model.set_params(**self.hyperparams_optimized)
+        self.model.fit(self.X, self.y)
+        return self.model
+
+    @not_optimized_error
+    def get_optimized_parameters(self) -> dict:
+        return self.hyperparams_optimized
+
+    @not_optimized_error
+    def get_optimized_metric(self) -> float:
+        return self.metric_optimized
```

### Comparing `hyponic-0.0.1/hyponic/optimizers/ABC.py` & `hyponic-0.0.1a0/hyponic/optimizers/ABC.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-from hyponic.optimizers.base_optimizer import BaseOptimizer
-import numpy as np
-from copy import deepcopy
-
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
+import numpy as np
+from copy import deepcopy
+
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

### Comparing `hyponic-0.0.1/hyponic/optimizers/ACO.py` & `hyponic-0.0.1a0/hyponic/optimizers/ACO.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-import numpy as np
-from hyponic.optimizers.base_optimizer import BaseOptimizer
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
+import numpy as np
+from hyponic.optimizers.base_optimizer import BaseOptimizer
+
+
+class AntColonyOptimization(BaseOptimizer):
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

### Comparing `hyponic-0.0.1/hyponic/optimizers/PSO.py` & `hyponic-0.0.1a0/hyponic/optimizers/PSO.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,76 @@
-from .base_optimizer import BaseOptimizer
-import numpy as np
-from copy import deepcopy
-
-
-class PSO(BaseOptimizer):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.a1 = kwargs.get('a1', 0.5)
-        self.a2 = kwargs.get('a2', 0.5)
-        self.coords = None
-        self.velocities = None
-        self.p_best = None
-        self.p_best_coords = None
-        self.g_best = None
-        self.g_best_coords = None
-
-    def initialize(self, problem_dict):
-        # TODO: add multithreading and multiprocessing
-        # TODO: check if the problem_dict is valid
-        # TODO: if lb and ub are not provided, use the default values
-        super().initialize(problem_dict)
-        self.g_best = np.inf if self.minmax == "min" else -np.inf
-
-        self.coords = np.random.uniform(self.lb, self.ub, (self.population_size, self.dimensions))
-        max_velocity = self.ub - self.lb
-
-        self.velocities = np.random.uniform(-max_velocity, max_velocity, size=(self.population_size, self.dimensions))
-        self.p_best_coords = deepcopy(self.coords)
-        self.p_best = np.array([self.function(self.coords[i]) for i in range(self.population_size)])
-        self._update_global_best()
-
-    def evolve(self, epoch):
-        self.velocities = self._update_velocity()
-        self.coords = self.coords + self.velocities
-
-        # TODO: if lb or ub is provided, clip the coordinates
-        self.coords = np.clip(self.coords, self.lb, self.ub)
-        fitness = np.array([self.function(self.coords[i]) for i in range(self.population_size)])
-        condition = all(self._minmax()(np.concatenate([self.p_best, fitness])) != self.p_best)
-        self.p_best_coords = np.where(condition, self.coords, self.p_best_coords)
-        self.p_best = np.where(condition, fitness, self.p_best)
-        self._update_global_best()
-
-    def _update_velocity(self):
-        r1 = np.random.random()
-        r2 = np.random.random()
-        return self.velocities + self.a1 * r1 * (self.p_best_coords - self.coords) + self.a2 * r2 * (self.g_best_coords - self.coords)
-
-    def _update_global_best(self):
-        if self._minmax()(np.concatenate([self.p_best, [self.g_best]])) != self.g_best:
-            self.g_best = self._minmax()(self.p_best)
-            self.g_best_coords = deepcopy(self.p_best_coords[self._argminmax()(self.p_best)])
-
-    def get_best_score(self):
-        return self.g_best
-
-    def get_best_solution(self):
-        return self.g_best_coords
-
-
-class IWPSO(PSO):
-    """
-    Inertia Weight Particle Swarm Optimization
-    """
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.w = kwargs.get('w', 0.8)
-
-    def _update_velocity(self):
-        r1 = np.random.random()
-        r2 = np.random.random()
-        return self.w * self.velocities + self.a1 * r1 * (self.p_best_coords - self.coords) + self.a2 * r2 * (
-                    self.g_best_coords - self.coords)
+from .base_optimizer import BaseOptimizer
+import numpy as np
+from copy import deepcopy
+
+
+class PSO(BaseOptimizer):
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.a1 = kwargs.get('a1', 0.5)
+        self.a2 = kwargs.get('a2', 0.5)
+        self.coords = None
+        self.velocities = None
+        self.p_best = None
+        self.p_best_coords = None
+        self.g_best = None
+        self.g_best_coords = None
+
+    def initialize(self, problem_dict):
+        # TODO: add multithreading and multiprocessing
+        # TODO: check if the problem_dict is valid
+        # TODO: if lb and ub are not provided, use the default values
+        super().initialize(problem_dict)
+        self.g_best = np.inf if self.minmax == "min" else -np.inf
+
+        self.coords = np.random.uniform(self.lb, self.ub, (self.population_size, self.dimensions))
+        max_velocity = self.ub - self.lb
+
+        self.velocities = np.random.uniform(-max_velocity, max_velocity, size=(self.population_size, self.dimensions))
+        self.p_best_coords = deepcopy(self.coords)
+        self.p_best = np.array([self.function(self.coords[i]) for i in range(self.population_size)])
+        self._update_global_best()
+
+    def evolve(self, epoch):
+        self.velocities = self._update_velocity()
+        self.coords = self.coords + self.velocities
+
+        # TODO: if lb or ub is provided, clip the coordinates
+        self.coords = np.clip(self.coords, self.lb, self.ub)
+        fitness = np.array([self.function(self.coords[i]) for i in range(self.population_size)])
+        condition = all(self._minmax()(np.concatenate([self.p_best, fitness])) != self.p_best)
+
+        self.p_best_coords = np.where(condition, self.coords, self.p_best_coords)
+
+        self.p_best = np.where(condition, fitness, self.p_best)
+        self._update_global_best()
+
+    def _update_velocity(self):
+        r1 = np.random.random()
+        r2 = np.random.random()
+        return self.velocities + self.a1 * r1 * (self.p_best_coords - self.coords) + self.a2 * r2 * (self.g_best_coords - self.coords)
+
+    def _update_global_best(self):
+        if self._minmax()(np.concatenate([self.p_best, [self.g_best]])) != self.g_best:
+            self.g_best = self._minmax()(self.p_best)
+            self.g_best_coords = deepcopy(self.p_best_coords[self._argminmax()(self.p_best)])
+
+    def get_best_score(self):
+        return self.g_best
+
+    def get_best_solution(self):
+        return self.g_best_coords
+
+
+class IWPSO(PSO):
+    """
+    Inertia Weight Particle Swarm Optimization
+    """
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.w = kwargs.get('w', 0.8)
+
+    def _update_velocity(self):
+        r1 = np.random.random()
+        r2 = np.random.random()
+        return self.w * self.velocities + self.a1 * r1 * (self.p_best_coords - self.coords) + self.a2 * r2 * (
+                    self.g_best_coords - self.coords)
```

### Comparing `hyponic-0.0.1/hyponic/optimizers/SA.py` & `hyponic-0.0.1a0/hyponic/optimizers/SA.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-import numpy as np
-
-from hyponic.optimizers.base_optimizer import BaseOptimizer
-
-
-class SA(BaseOptimizer):
-    """
-    Simulated Annealing
-    """
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-        self.currents = None
-        self.best = None
-        self.best_score = None
-
-    def initialize(self, problem_dict):
-        super().initialize(problem_dict)
-
-        self.currents = np.random.uniform(self.lb, self.ub, (self.population_size, self.dimensions))
-
-        self.best = self.currents[0]
-        self.best_score = self.function(self.best)
-
-    def evolve(self, current_epoch):
-        progress = current_epoch / self.epoch
-        t = max(0.01, min(1, 1 - progress))
-
-        amplitudes = (np.max(self.intervals) - np.min(self.intervals)) * progress * 0.1
-        deltas = np.random.uniform(-amplitudes / 2, amplitudes / 2, (self.population_size, self.dimensions))
-
-        candidates = self.currents + deltas
-
-        for idx, candidate in enumerate(candidates):
-            candidate = np.clip(candidate, self.lb, self.ub)
-            candidate_score = self.function(candidate)
-
-            if candidate_score < self.best_score:
-                self.best = candidate
-                self.best_score = candidate_score
-                self.currents[idx] = candidate
-            else:
-                score_abs_diff = abs(candidate_score - self.best_score)
-
-                if np.random.uniform() < np.exp(-score_abs_diff / t):
-                    self.currents[idx] = candidate
-
-    def get_best_score(self):
-        return self.best_score
-
-    def get_best_solution(self):
-        return self.best
+import numpy as np
+
+from hyponic.optimizers.base_optimizer import BaseOptimizer
+
+
+class SA(BaseOptimizer):
+    """
+    Simulated Annealing
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+        self.currents = None
+        self.best = None
+        self.best_score = None
+
+    def initialize(self, problem_dict):
+        super().initialize(problem_dict)
+
+        self.currents = np.random.uniform(self.lb, self.ub, (self.population_size, self.dimensions))
+
+        self.best = self.currents[0]
+        self.best_score = self.function(self.best)
+
+    def evolve(self, current_epoch):
+        progress = current_epoch / self.epoch
+        t = max(0.01, min(1, 1 - progress))
+
+        amplitudes = (np.max(self.intervals) - np.min(self.intervals)) * progress * 0.1
+        deltas = np.random.uniform(-amplitudes / 2, amplitudes / 2, (self.population_size, self.dimensions))
+
+        candidates = self.currents + deltas
+
+        for idx, candidate in enumerate(candidates):
+            candidate = np.clip(candidate, self.lb, self.ub)
+            candidate_score = self.function(candidate)
+
+            if candidate_score < self.best_score:
+                self.best = candidate
+                self.best_score = candidate_score
+                self.currents[idx] = candidate
+            else:
+                score_abs_diff = abs(candidate_score - self.best_score)
+
+                if np.random.uniform() < np.exp(-score_abs_diff / t):
+                    self.currents[idx] = candidate
+
+    def get_best_score(self):
+        return self.best_score
+
+    def get_best_solution(self):
+        return self.best
```

### Comparing `hyponic-0.0.1/hyponic/optimizers/base_optimizer.py` & `hyponic-0.0.1a0/hyponic/optimizers/base_optimizer.py`

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
-        self.interval_len = None
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
+        self.interval_len = None
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

### Comparing `hyponic-0.0.1/hyponic/space.py` & `hyponic-0.0.1a0/hyponic/space.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-from typing import Callable, Any
-
-
-def clip(x, low, high):
-    return max(low, min(x, high))
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
+from typing import Callable, Any
+
+
+def clip(x, low, high):
+    return max(low, min(x, high))
+
+
+class Space:
+    def __init__(self, in_dict: dict[str, Any]):
+        self.__dict = dict
+        self.dimensions = {}
+        self.dimensions_names = []
+
+        for key, value in in_dict.items():
+            # Converting range to list
+            if isinstance(value, range):
+                value = list(value)
+
+            if isinstance(value, tuple):
+                if len(value) != 2:
+                    raise ValueError(f'Value for key {key} is not valid')
+                self.dimensions[key] = Continuous(*value, name=key)
+            elif isinstance(value, list):
+                self.dimensions[key] = Discrete(value, name=key)
+            else:
+                raise ValueError(f'Value for key {key} is not valid')
+
+            self.dimensions_names.append(key)
+
+    def get_continuous_mappings(
+            self, scales: dict | int | float = None, origins: dict | int | float = None
+    ) -> dict[str, (Callable, (float, float))]:
+
+        """
+        Returns a function that maps a discrete value to a continuous value.
+        """
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
+        out = f"Space with {len(self.dimensions)} dimensions"
+        for key in self.dimensions:
+            # TODO: pretty print
+            out += f"\n\t{key}:\t{self.dimensions[key]}"
+        return out
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
+            x = clip(x, low, high)
+            x = self._lbound + (x - origin) / scale
+            return self.get_value(x)
+
+        return mapping_func, (low, high)
+
+    def get_value(self, x):
+        raise NotImplementedError
+
+    def __str__(self):
+        return f"{self.__class__.__name__}({self._lbound}, {self._ubound})"
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
+        # > maybe add transformation here? E.g. log, exp, etc.
+        # TODO: non-linear mapping
+        return x
+
+
+class Discrete(Dimension):
+    def __init__(self, values, name=None):
+        super().__init__(0, len(values) - 1, name)
+        self.values = values
+
+    def get_value(self, x):
+        # Note that x is already in the correct range. No need to clip.
+        return self.values[int(x)]
```

### Comparing `hyponic-0.0.1/hyponic/symtable.py` & `hyponic-0.0.1a0/hyponic/symtable.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-class Symbol:
-    def __init__(self, symtable, name, *args, **kwargs):
-        self._symtable = symtable
-        self._name = name
-        self._args = args
-        self._kwargs = kwargs  # TODO: Implement kwargs
-
-    def __call__(self, *args):
-        return Symbol(self._symtable, self._name, *args)
-
-    def __repr__(self):
-        return f"{self._name}({', '.join(repr(arg) for arg in self._args)})"
-
-    def eval(self):
-        args = [arg.eval() if isinstance(arg, Symbol) else arg for arg in self._args]
-
-        # If all arguments are literals, evaluate the function
-        # Otherwise, evaluate partially
-        if all(not isinstance(arg, Symbol) for arg in args):
-            if self._name in self._symtable.get_symbol_list():
-                return self._symtable.get_symbol(self._name)(*args)
-            else:
-                return self
-        else:
-            # Partially evaluate
-            self._args = args
-            return self
-
-
-class SymbolTable:
-    def __init__(self):
-        self._symbols = {
-            "int": int,
-            "float": float,
-            "add": lambda x, y: x + y,
-        }
-
-    def get_symbol(self, name):
-        return self._symbols[name]
-
-    def get_symbol_list(self):
-        return self._symbols.keys()
-
-    def add_symbol(self, name, func):
-        self._symbols[name] = func
-
-    def __getattr__(self, name):
-        return Symbol(self, name)
-
-
-# scope = SymbolTable()
-# expr = scope.add(scope.int(1), scope.int(2.5))
-# expr.eval()
+class Symbol:
+    def __init__(self, symtable, name, *args, **kwargs):
+        self._symtable = symtable
+        self._name = name
+        self._args = args
+        self._kwargs = kwargs  # TODO: Implement kwargs
+
+    def __call__(self, *args):
+        return Symbol(self._symtable, self._name, *args)
+
+    def __repr__(self):
+        return f"{self._name}({', '.join(repr(arg) for arg in self._args)})"
+
+    def eval(self):
+        args = [arg.eval() if isinstance(arg, Symbol) else arg for arg in self._args]
+
+        # If all arguments are literals, evaluate the function
+        # Otherwise, evaluate partially
+        if all(not isinstance(arg, Symbol) for arg in args):
+            if self._name in self._symtable.get_symbol_list():
+                return self._symtable.get_symbol(self._name)(*args)
+            else:
+                return self
+        else:
+            # Partially evaluate
+            self._args = args
+            return self
+
+
+class SymbolTable:
+    def __init__(self):
+        self._symbols = {
+            "int": int,
+            "float": float,
+            "add": lambda x, y: x + y,
+        }
+
+    def get_symbol(self, name):
+        return self._symbols[name]
+
+    def get_symbol_list(self):
+        return self._symbols.keys()
+
+    def add_symbol(self, name, func):
+        self._symbols[name] = func
+
+    def __getattr__(self, name):
+        return Symbol(self, name)
+
+
+# scope = SymbolTable()
+# expr = scope.add(scope.int(1), scope.int(2.5))
+# expr.eval()
```

### Comparing `hyponic-0.0.1/hyponic.egg-info/PKG-INFO` & `hyponic-0.0.1a0/hyponic.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,138 +1,134 @@
-Metadata-Version: 2.1
-Name: hyponic
-Version: 0.0.1
-Summary: Hyperparameter Optimization with Nature-Inspired Computing
-Home-page: https://github.com/slewie/HypONIC
-Author: Vladislav Kulikov, Daniel Satarov, Ivan Chernakov
-Author-email: v.kulikov@innopolis.university, d.satarov@innopolis.university, i.chernakov@innopolis.university
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# HypONIC -- Hyperparameter Optimization with Nature Inspired Computing
-
-*HypONIC* is a hyperparameter optimization library that uses various nature inspired computing algorithms to optimize
-the hyperparameters of machine learning models. The library provides a simple interface for sklearn and keras models.
-
-## Implementation details
-*HypONIC* library follows a common high-level approach by providing a unified interface for applying an optimization algorithm
-of choice to the parameters of a machine learning model (based on the `BaseEstimator` from the `sklearn`). Evalution of the
-optimization process is done by a metric of choice.
-
-### Metrics
-*HypONIC* provides a list of classical evalution metrics:
-
-- Mean Squared Error
-- Mean Absolute Error
-- Root Mean Square Error
-- Huber Loss
-- Log Loss
-- Binary Crossentropy
-- Precision Score
-- Accuracy Score
-- Recall Score
-- F1 Score
-- R2 Score
-- ...and many others.
-
-*HypONIC* library provides decorators for annotating custom metrics: `@minimize_metric` and `@maximize_metric`. These decorators
-allows using names of the metric functions as string literals instead of passing the function itself, i.e.
-
-```python
-from hyponic.optimizer import HypONIC
-...
-hyponic = HypONIC(model, X, y, "mse", **optimizer_kwargs)
-...
-```
-
-instead of
-
-```python
-from hyponic.optimizer import HypONIC
-from hyponic.metrics import mse
-...
-hyponic = HypONIC(model, X, y, mse, **optimizer_kwargs)
-...
-```
-
-### Hyperparameter Space
-*HypONIC* library supports mixed space of hyperparameters, meaning that one optimization space can have both
-dimensions of discrete and continuous parameters. The notation for each space is the following:
-
-```python
-hyperparams = {
-    "min_impurity_decrease": (0.0, 0.9),              # Continious space -- (lower bound, upper bound)
-    "min_samples_split": [2, 3, 4, 5, 6],             # Discrete space   -- a list of values of any type
-    "criterion": ["absolute_error", "squared_error"]  # Discrete space   -- a list of values of any type
-}
-```
-
-For the discrete space an automatic uniform mapping* to the continious space is provided if needed. Discrete space of
-non numerical values is encoded first and then uniformly mapped to the continious space.
-
-*is subject to change
-
-## Features
-*HypONIC* supports different nature inspired computing algorithms.
-Please note that the library is currently under development and may contain a significant number of bugs and errors.
-All algorithms are subject to further improvement.
-
-The following algorithms are currently implemented or are planned to be implemented:
-
-**Swarm-based:**
-- - [x] Particle Swarm Optimization (PSO)
-- - [x] Inertia Weight PSO (IWPSO)
-- - [x] Ant Colony Optimization (ACO)
-- - [x] Artificial Bee Colony (ABC)
-- - [ ] Grey Wolf Optimizer (GWO)
-- - [ ] Cuckoo Search (CS)
-- - [ ] Firefly Algorithm (FA)
-
-**Physics-based:**
-- - [x] Simulated Annealing (SA)
-
-**Genetic-based:**
-- - [x] Genetic Algorithm
-
-## Minimal Example
-
-This is a minimal example for tuning hyperparameters of the `RandomForestRegressor` from `sklearn`. The default optimizator is *Inertia Weight Particle Swarm Optimization* (IWPSO), as it has high applicability and has shown fast convergence.
-
-```python
-from sklearn.datasets import load_diabetes
-from sklearn.ensemble import RandomForestRegressor
-
-from hyponic.metrics import mse
-from hyponic.optimizer import HypONIC
-
-X, y = load_diabetes(return_X_y=True)
-model = RandomForestRegressor()
-
-hyperparams = {
-    "min_samples_split": (0.01, 0.9),  # Continious space
-    "min_samples_leaf": (0.01, 0.9),  # Continious space
-    "min_weight_fraction_leaf": (0.0, 0.5),  # Continious space
-    "min_impurity_decrease": (0.0, 0.9),  # Continious space
-    "criterion": ["absolute_error", "squared_error"]  # Discrete space
-}
-
-optimizer_kwargs = {
-    "epoch": 50,
-    "pop_size": 50,
-}
-
-# The default optimizator is the Inertia Weight Particle Swarm Optimization (IWPSO)
-hyponic = HypONIC(model, X, y, mse, **optimizer_kwargs)
-hyponic.optimize(hyperparams, verbose=True)
-
-print(hyponic.get_optimized_parameters())
-print(hyponic.get_optimized_metric())
-print(hyponic.get_optimized_model())
-```
-
-
+Metadata-Version: 2.1
+Name: hyponic
+Version: 0.0.1a0
+Summary: Hyperparameter Optimization with Nature-Inspired Computing
+Home-page: https://github.com/slewie/HypONIC
+Author: Vladislav Kulikov, Daniel Satarov, Ivan Chernakov
+Author-email: v.kulikov@innopolis.university, d.satarov@innopolis.university, i.chernakov@innopolis.university
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# HypONIC -- Hyperparameter Optimization with Nature Inspired Computing
+
+*HypONIC* is a hyperparameter optimization library that uses various nature inspired computing algorithms to optimize
+the hyperparameters of machine learning models. The library provides a simple interface for sklearn and keras models.
+
+## Implementation details
+*HypONIC* library follows a common high-level approach by providing a unified interface for applying an optimization algorithm
+of choice to the parameters of a machine learning model (based on the `BaseEstimator` from the `sklearn`). Evalution of the
+optimization process is done by a metric of choice.
+
+### Metrics
+*HypONIC* provides a list of classical evalution metrics:
+
+- Mean Squared Error
+- Mean Absolute Error
+- Root Mean Square Error
+- Huber Loss
+- Log Loss
+- Binary Crossentropy
+- Precision Score
+- Accuracy Score
+- Recall Score
+- F1 Score
+- R2 Score
+- ...and many others.
+
+*HypONIC* library provides decorators for annotating custom metrics: `@minimize_metric` and `@maximize_metric`. These decorators
+allows using names of the metric functions as string literals instead of passing the function itself, i.e.
+
+```python
+from hyponic.optimizer import HypONIC
+...
+hyponic = HypONIC(model, X, y, "mse", **optimizer_kwargs)
+...
+```
+
+instead of
+
+```python
+from hyponic.optimizer import HypONIC
+from hyponic.metrics import mse
+...
+hyponic = HypONIC(model, X, y, mse, **optimizer_kwargs)
+...
+```
+
+### Hyperparameter Space
+*HypONIC* library supports mixed space of hyperparameters, meaning that one optimization space can have both
+dimensions of discrete and continuous parameters. The notation for each space is the following:
+
+```python
+hyperparams = {
+    "min_impurity_decrease": (0.0, 0.9),              # Continious space -- (lower bound, upper bound)
+    "min_samples_split": [2, 3, 4, 5, 6],             # Discrete space   -- a list of values of any type
+    "criterion": ["absolute_error", "squared_error"]  # Discrete space   -- a list of values of any type
+}
+```
+
+For the discrete space an automatic uniform mapping* to the continious space is provided if needed. Discrete space of
+non numerical values is encoded first and then uniformly mapped to the continious space.
+
+*is subject to change
+
+## Features
+*HypONIC* supports different nature inspired computing algorithms.
+Please note that the library is currently under development and may contain a significant number of bugs and errors.
+All algorithms are subject to further improvement.
+
+The following algorithms are currently implemented or are planned to be implemented:
+
+**Swarm-based:**
+- - [x] Particle Swarm Optimization (PSO)
+- - [x] Inertia Weight PSO (IWPSO)
+- - [x] Ant Colony Optimization (ACO)
+- - [x] Artificial Bee Colony (ABC)
+- - [ ] Grey Wolf Optimizer (GWO)
+- - [ ] Cuckoo Search (CS)
+- - [ ] Firefly Algorithm (FA)
+
+**Physics-based:**
+- - [x] Simulated Annealing (SA)
+
+**Genetic-based:**
+- - [x] Genetic Algorithm
+
+## Minimal Example
+
+This is a minimal example for tuning hyperparameters of the `RandomForestRegressor` from `sklearn`. The default optimizator is *Inertia Weight Particle Swarm Optimization* (IWPSO), as it has high applicability and has shown fast convergence.
+
+```python
+from sklearn.datasets import load_diabetes
+from sklearn.ensemble import RandomForestRegressor
+
+from hyponic.metrics import mse
+from hyponic.optimizer import HypONIC
+
+X, y = load_diabetes(return_X_y=True)
+model = RandomForestRegressor()
+
+hyperparams = {
+    "min_samples_split": (0.01, 0.9),  # Continious space
+    "min_samples_leaf": (0.01, 0.9),  # Continious space
+    "min_weight_fraction_leaf": (0.0, 0.5),  # Continious space
+    "min_impurity_decrease": (0.0, 0.9),  # Continious space
+    "criterion": ["absolute_error", "squared_error"]  # Discrete space
+}
+
+optimizer_kwargs = {
+    "epoch": 50,
+    "pop_size": 50,
+}
+
+# The default optimizator is the Inertia Weight Particle Swarm Optimization (IWPSO)
+hyponic = HypONIC(model, X, y, mse, **optimizer_kwargs)
+hyponic.optimize(hyperparams, verbose=True)
+
+print(hyponic.get_optimized_parameters())
+print(hyponic.get_optimized_metric())
+print(hyponic.get_optimized_model())
+```
```

