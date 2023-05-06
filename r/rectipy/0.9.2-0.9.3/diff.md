# Comparing `tmp/rectipy-0.9.2.tar.gz` & `tmp/rectipy-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rectipy-0.9.2.tar", last modified: Sat Jan 14 22:52:43 2023, max compression
+gzip compressed data, was "rectipy-0.9.3.tar", last modified: Sat Feb 11 23:01:22 2023, max compression
```

## Comparing `rectipy-0.9.2.tar` & `rectipy-0.9.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 22:52:43.058618 rectipy-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-14 22:52:35.000000 rectipy-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-14 22:52:35.000000 rectipy-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-01-14 22:52:43.058618 rectipy-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-01-14 22:52:35.000000 rectipy-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 22:52:43.058618 rectipy-0.9.2/neuron_model_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-01-14 22:52:35.000000 rectipy-0.9.2/neuron_model_templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 22:52:43.058618 rectipy-0.9.2/neuron_model_templates/rate_neurons/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-01-14 22:52:35.000000 rectipy-0.9.2/neuron_model_templates/rate_neurons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-01-14 22:52:35.000000 rectipy-0.9.2/neuron_model_templates/rate_neurons/leaky_integrator.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 22:52:43.058618 rectipy-0.9.2/neuron_model_templates/spiking_neurons/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-01-14 22:52:35.000000 rectipy-0.9.2/neuron_model_templates/spiking_neurons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-01-14 22:52:35.000000 rectipy-0.9.2/neuron_model_templates/spiking_neurons/ik.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-01-14 22:52:35.000000 rectipy-0.9.2/neuron_model_templates/spiking_neurons/lif.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-01-14 22:52:35.000000 rectipy-0.9.2/neuron_model_templates/spiking_neurons/qif.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 22:52:43.058618 rectipy-0.9.2/rectipy/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-01-14 22:52:35.000000 rectipy-0.9.2/rectipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-01-14 22:52:35.000000 rectipy-0.9.2/rectipy/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28827 2023-01-14 22:52:35.000000 rectipy-0.9.2/rectipy/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-01-14 22:52:35.000000 rectipy-0.9.2/rectipy/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-01-14 22:52:35.000000 rectipy-0.9.2/rectipy/output_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-01-14 22:52:35.000000 rectipy-0.9.2/rectipy/rnn_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-01-14 22:52:35.000000 rectipy-0.9.2/rectipy/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 22:52:43.058618 rectipy-0.9.2/rectipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-01-14 22:52:43.000000 rectipy-0.9.2/rectipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-01-14 22:52:43.000000 rectipy-0.9.2/rectipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-14 22:52:43.000000 rectipy-0.9.2/rectipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-14 22:52:43.000000 rectipy-0.9.2/rectipy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-14 22:52:43.000000 rectipy-0.9.2/rectipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-01-14 22:52:43.000000 rectipy-0.9.2/rectipy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 22:52:43.058618 rectipy-0.9.2/rectipy_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-01-14 22:52:35.000000 rectipy-0.9.2/rectipy_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-01-14 22:52:35.000000 rectipy-0.9.2/rectipy_tests/test_input_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-01-14 22:52:35.000000 rectipy-0.9.2/rectipy_tests/test_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-01-14 22:52:35.000000 rectipy-0.9.2/rectipy_tests/test_output_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-01-14 22:52:35.000000 rectipy-0.9.2/rectipy_tests/test_rnn_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-14 22:52:43.058618 rectipy-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-01-14 22:52:35.000000 rectipy-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 23:01:22.627254 rectipy-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-11 23:01:12.000000 rectipy-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-11 23:01:12.000000 rectipy-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-02-11 23:01:22.627254 rectipy-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-02-11 23:01:12.000000 rectipy-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 23:01:22.623254 rectipy-0.9.3/neuron_model_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-02-11 23:01:12.000000 rectipy-0.9.3/neuron_model_templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 23:01:22.623254 rectipy-0.9.3/neuron_model_templates/rate_neurons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-02-11 23:01:12.000000 rectipy-0.9.3/neuron_model_templates/rate_neurons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-02-11 23:01:12.000000 rectipy-0.9.3/neuron_model_templates/rate_neurons/leaky_integrator.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 23:01:22.623254 rectipy-0.9.3/neuron_model_templates/spiking_neurons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-02-11 23:01:12.000000 rectipy-0.9.3/neuron_model_templates/spiking_neurons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-02-11 23:01:12.000000 rectipy-0.9.3/neuron_model_templates/spiking_neurons/ik.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-11 23:01:12.000000 rectipy-0.9.3/neuron_model_templates/spiking_neurons/lif.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-02-11 23:01:12.000000 rectipy-0.9.3/neuron_model_templates/spiking_neurons/qif.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 23:01:22.623254 rectipy-0.9.3/rectipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-02-11 23:01:12.000000 rectipy-0.9.3/rectipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-02-11 23:01:12.000000 rectipy-0.9.3/rectipy/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28827 2023-02-11 23:01:12.000000 rectipy-0.9.3/rectipy/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-02-11 23:01:12.000000 rectipy-0.9.3/rectipy/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-02-11 23:01:12.000000 rectipy-0.9.3/rectipy/output_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-02-11 23:01:12.000000 rectipy-0.9.3/rectipy/rnn_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-02-11 23:01:12.000000 rectipy-0.9.3/rectipy/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 23:01:22.627254 rectipy-0.9.3/rectipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-02-11 23:01:22.000000 rectipy-0.9.3/rectipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-02-11 23:01:22.000000 rectipy-0.9.3/rectipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 23:01:22.000000 rectipy-0.9.3/rectipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 23:01:22.000000 rectipy-0.9.3/rectipy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-02-11 23:01:22.000000 rectipy-0.9.3/rectipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-11 23:01:22.000000 rectipy-0.9.3/rectipy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 23:01:22.627254 rectipy-0.9.3/rectipy_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-02-11 23:01:12.000000 rectipy-0.9.3/rectipy_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-02-11 23:01:12.000000 rectipy-0.9.3/rectipy_tests/test_input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-02-11 23:01:12.000000 rectipy-0.9.3/rectipy_tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-02-11 23:01:12.000000 rectipy-0.9.3/rectipy_tests/test_output_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-02-11 23:01:12.000000 rectipy-0.9.3/rectipy_tests/test_rnn_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-11 23:01:22.627254 rectipy-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-02-11 23:01:12.000000 rectipy-0.9.3/setup.py
```

### Comparing `rectipy-0.9.2/LICENSE` & `rectipy-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rectipy-0.9.2/PKG-INFO` & `rectipy-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rectipy
-Version: 0.9.2
+Version: 0.9.3
 Summary: Recurrent neural network training in Python
 Home-page: UNKNOWN
 Author: Richard Gast
 Author-email: richard.gast@northwestern.edu
 License: GPL v3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rectipy-0.9.2/README.md` & `rectipy-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `rectipy-0.9.2/neuron_model_templates/__init__.py` & `rectipy-0.9.3/neuron_model_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `rectipy-0.9.2/neuron_model_templates/rate_neurons/__init__.py` & `rectipy-0.9.3/neuron_model_templates/rate_neurons/__init__.py`

 * *Files identical despite different names*

### Comparing `rectipy-0.9.2/neuron_model_templates/rate_neurons/leaky_integrator.yaml` & `rectipy-0.9.3/neuron_model_templates/rate_neurons/leaky_integrator.yaml`

 * *Files identical despite different names*

### Comparing `rectipy-0.9.2/neuron_model_templates/spiking_neurons/__init__.py` & `rectipy-0.9.3/neuron_model_templates/spiking_neurons/__init__.py`

 * *Files identical despite different names*

### Comparing `rectipy-0.9.2/neuron_model_templates/spiking_neurons/qif.yaml` & `rectipy-0.9.3/neuron_model_templates/spiking_neurons/qif.yaml`

 * *Files identical despite different names*

### Comparing `rectipy-0.9.2/rectipy/__init__.py` & `rectipy-0.9.3/rectipy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,12 +25,12 @@
 # Richard Gast et al. (in preparation)
 """User interface for the initialization, training, and testing of networks with 3 layers:
 Input, recurrent network, and output layer.
 """
 
 __author__ = "Richard Gast"
 __status__ = "Development"
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 from .network import Network, Observer
 from .utility import random_connectivity, circular_connectivity, input_connections, normalize
 from .utility import wta_score, readout
```

### Comparing `rectipy-0.9.2/rectipy/input_layer.py` & `rectipy-0.9.3/rectipy/input_layer.py`

 * *Files identical despite different names*

### Comparing `rectipy-0.9.2/rectipy/network.py` & `rectipy-0.9.3/rectipy/network.py`

 * *Files identical despite different names*

### Comparing `rectipy-0.9.2/rectipy/observer.py` & `rectipy-0.9.3/rectipy/observer.py`

 * *Files identical despite different names*

### Comparing `rectipy-0.9.2/rectipy/output_layer.py` & `rectipy-0.9.3/rectipy/output_layer.py`

 * *Files identical despite different names*

### Comparing `rectipy-0.9.2/rectipy/rnn_layer.py` & `rectipy-0.9.3/rectipy/rnn_layer.py`

 * *Files identical despite different names*

### Comparing `rectipy-0.9.2/rectipy/utility.py` & `rectipy-0.9.3/rectipy/utility.py`

 * *Files 6% similar despite different names*

```diff
@@ -226,103 +226,113 @@
     """
     z = np.zeros((x.shape[0],))
     for idx in range(x.shape[0]):
         z[idx] = 1.0 if np.argmax(x[idx, :]) == np.argmax(y[idx, :]) else 0.0
     return float(np.mean(z))
 
 
-def readout(X: np.ndarray, y: np.ndarray, k: int = 1, train_split: int = None, verbose: bool = True, **kwargs
-            ) -> dict:
+def readout(X: np.ndarray, y: np.ndarray, k: int = 1, test_size: float = 0.2, verbose: bool = True,
+            normalize: str = None, **kwargs) -> dict:
     """Uses Ridge regression to find a set of coefficients `a` that minimizes `y - aX`.
 
     Parameters
     ----------
     X
         2D array of data (rows = samples, columns = features).
     y
-        2D array of data (rows = samples, columns = output dimensions).
+        2D array of data (rows = samples, columns = output dimensions) or 1D array of samples.
     k
         If larger 1, `k` splits into training and testing data will be performed, and for each of these splits a ridge
         regression will be calculated.
-    train_split
-        An integer that splits `X` and `y` into a training and a test data set. Must be smaller than the size of the
-        first dimension of `X` and `y`.
+    test_size
+        Fraction of the input data that is used for independent testing after the training is done.
     verbose
         If true, updates about the regression procedure will be displayed.
+    method
+        Regression method/model to be used. Can be one of 'Ridge', 'RidgeClassifier', 'LogisticRegression',
+        'ElasticNet', or 'Lasso'.
+    normalize
+        Choose from "minmax" or "standard" to scale the input data.
     kwargs
-        Additional keyword arguments passed to `sklearn.linear_model.Ridge`
+        Additional keyword arguments passed to `sklearn.linear_model.SGDClassifier`
 
     Returns
     -------
     dict
         Contains entries with the following keys:
          - 'train_score': R2 score training data
          - 'test_score': R2 score on test data
          - 'readout_weights': Regression coefficients
          - 'readout_bias': Regression bias term
          - 'prediction': Prediction of the fitted classifier for the testing data
          - 'target': Prediction target, i.e. the testing data
     """
 
     # imports
-    from sklearn.linear_model import Ridge
-    from sklearn.model_selection import StratifiedKFold
+    from sklearn.linear_model import SGDClassifier
+    from sklearn.model_selection import StratifiedKFold, train_test_split
+    from sklearn.preprocessing import scale, minmax_scale
+
+    # initialize classifier
+    classifier = SGDClassifier(**kwargs)
+
+    # normalize input data
+    if normalize == "minmax":
+        X = minmax_scale(X)
+    elif normalize == "standard":
+        X = scale(X)
 
     # split into training and test data set
-    if train_split:
-        X, X_t = X[:train_split], X[train_split:]
-        y, y_t = y[:train_split], y[train_split:]
+    if test_size > 0.0:
+        X, X_t, y, y_t = train_test_split(X, y, test_size=test_size, shuffle=False)
 
     # perform ridge regression
     if k > 1:
         splitter = StratifiedKFold(n_splits=k)
         scores, coefs, intercepts = [], [], []
         for i, (train_idx, test_idx) in enumerate(splitter.split(X=X, y=y)):
-            classifier = Ridge(**kwargs)
             classifier.fit(X[train_idx], y[train_idx])
             scores.append(classifier.score(X=X[test_idx], y=y[test_idx]))
             coefs.append(classifier.coef_)
             intercepts.append(classifier.intercept_)
     else:
-        classifier = Ridge(**kwargs)
         classifier.fit(X, y)
         scores = [classifier.score(X=X, y=y)]
         coefs = [classifier.coef_]
         intercepts = [classifier.intercept_]
 
     # store readout weights
     w_out = np.mean(coefs, axis=0)
     intercept = np.mean(intercepts, axis=0)
     train_score = np.mean(scores)
 
     if verbose:
         print(f'Finished readout training.')
         if k > 1:
-            print(fr'Average, cross-validated $R^2$ score across {k} test folds: {train_score}')
+            print(fr'Average, cross-validated score across {k} test folds: {train_score}')
         else:
-            print(fr'$R^2$ score on training data: {train_score}')
+            print(fr'Score on training data: {train_score}')
 
     # store temporary results
     res = {"train_score": train_score, "readout_weights": w_out, "readout_bias": intercept, "test_score": None,
            "prediction": None, "target": None}
 
     # perform testing
-    if train_split:
+    if test_size > 0.0:
 
-        classifier = Ridge(**kwargs)
         classifier.coef_ = w_out
         classifier.intercept_ = intercept
 
         res["test_score"] = classifier.score(X=X_t, y=y_t)
         res["prediction"] = classifier.predict(X_t)
         res["target"] = y_t
 
         if verbose:
             print(f'Finished readout training.')
-            print(fr"$R^2$ score on testing data: {res['test_score']}")
+            print(fr"Score on testing data: {res['test_score']}")
 
     else:
 
         res["prediction"] = classifier.predict(X)
         res["target"] = y
 
     return res
```

### Comparing `rectipy-0.9.2/rectipy.egg-info/PKG-INFO` & `rectipy-0.9.3/rectipy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rectipy
-Version: 0.9.2
+Version: 0.9.3
 Summary: Recurrent neural network training in Python
 Home-page: UNKNOWN
 Author: Richard Gast
 Author-email: richard.gast@northwestern.edu
 License: GPL v3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rectipy-0.9.2/rectipy.egg-info/SOURCES.txt` & `rectipy-0.9.3/rectipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rectipy-0.9.2/rectipy_tests/__init__.py` & `rectipy-0.9.3/rectipy_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rectipy-0.9.2/rectipy_tests/test_input_layer.py` & `rectipy-0.9.3/rectipy_tests/test_input_layer.py`

 * *Files identical despite different names*

### Comparing `rectipy-0.9.2/rectipy_tests/test_network.py` & `rectipy-0.9.3/rectipy_tests/test_network.py`

 * *Files identical despite different names*

### Comparing `rectipy-0.9.2/rectipy_tests/test_output_layer.py` & `rectipy-0.9.3/rectipy_tests/test_output_layer.py`

 * *Files identical despite different names*

### Comparing `rectipy-0.9.2/rectipy_tests/test_rnn_layer.py` & `rectipy-0.9.3/rectipy_tests/test_rnn_layer.py`

 * *Files identical despite different names*

### Comparing `rectipy-0.9.2/setup.py` & `rectipy-0.9.3/setup.py`

 * *Files identical despite different names*

