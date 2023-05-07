# Comparing `tmp/gradient-accumulator-0.4.2.tar.gz` & `tmp/gradient-accumulator-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gradient-accumulator-0.4.2.tar", last modified: Wed May  3 08:47:11 2023, max compression
+gzip compressed data, was "dist/gradient-accumulator-0.5.0.tar", last modified: Sun May  7 20:35:18 2023, max compression
```

## Comparing `gradient-accumulator-0.4.2.tar` & `gradient-accumulator-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 08:47:11.000000 gradient-accumulator-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (122)     8266 2023-05-03 08:47:11.000000 gradient-accumulator-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6390 2023-05-03 08:46:30.000000 gradient-accumulator-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 08:47:11.000000 gradient-accumulator-0.4.2/gradient_accumulator/
--rw-r--r--   0 runner    (1001) docker     (122)      166 2023-05-03 08:46:30.000000 gradient-accumulator-0.4.2/gradient_accumulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14885 2023-05-03 08:46:30.000000 gradient-accumulator-0.4.2/gradient_accumulator/accumulators.py
--rw-r--r--   0 runner    (1001) docker     (122)     2538 2023-05-03 08:46:30.000000 gradient-accumulator-0.4.2/gradient_accumulator/agc.py
--rw-r--r--   0 runner    (1001) docker     (122)     9004 2023-05-03 08:46:30.000000 gradient-accumulator-0.4.2/gradient_accumulator/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 08:47:11.000000 gradient-accumulator-0.4.2/gradient_accumulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8266 2023-05-03 08:47:11.000000 gradient-accumulator-0.4.2/gradient_accumulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-05-03 08:47:11.000000 gradient-accumulator-0.4.2/gradient_accumulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 08:47:11.000000 gradient-accumulator-0.4.2/gradient_accumulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-03 08:47:11.000000 gradient-accumulator-0.4.2/gradient_accumulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-03 08:47:11.000000 gradient-accumulator-0.4.2/gradient_accumulator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-03 08:47:11.000000 gradient-accumulator-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-05-03 08:46:30.000000 gradient-accumulator-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 20:35:18.000000 gradient-accumulator-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     8743 2023-05-07 20:35:18.000000 gradient-accumulator-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6815 2023-05-07 20:34:30.000000 gradient-accumulator-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 20:35:18.000000 gradient-accumulator-0.5.0/gradient_accumulator/
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-07 20:34:30.000000 gradient-accumulator-0.5.0/gradient_accumulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20181 2023-05-07 20:34:30.000000 gradient-accumulator-0.5.0/gradient_accumulator/accumulators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2609 2023-05-07 20:34:30.000000 gradient-accumulator-0.5.0/gradient_accumulator/agc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9030 2023-05-07 20:34:30.000000 gradient-accumulator-0.5.0/gradient_accumulator/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 20:35:18.000000 gradient-accumulator-0.5.0/gradient_accumulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8743 2023-05-07 20:35:17.000000 gradient-accumulator-0.5.0/gradient_accumulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-05-07 20:35:18.000000 gradient-accumulator-0.5.0/gradient_accumulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-07 20:35:17.000000 gradient-accumulator-0.5.0/gradient_accumulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-07 20:35:17.000000 gradient-accumulator-0.5.0/gradient_accumulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-05-07 20:35:17.000000 gradient-accumulator-0.5.0/gradient_accumulator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-05-07 20:35:18.000000 gradient-accumulator-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-05-07 20:34:30.000000 gradient-accumulator-0.5.0/setup.py
```

### Comparing `gradient-accumulator-0.4.2/PKG-INFO` & `gradient-accumulator-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: gradient-accumulator
-Version: 0.4.2
+Version: 0.5.0
 Summary: Package for gradient accumulation in TensorFlow
 Home-page: https://github.com/andreped/GradientAccumulator
-Author: André Pedersen and David Bouget and Javier Pérez de Frutos
+Author: André Pedersen and David Bouget and Javier Pérez de Frutos and Tor-Arne Schmidt Nordmo
 Author-email: andrped94@gmail.com
 License: UNKNOWN
 Description: <div align="center">
         <img src="assets/accum_grad_v5_reduced.png" width="35%" alt='gradient-accumulator'>
         <h1 align="center">GradientAccumulator</h1>
         <h3 align="center">Seemless gradient accumulation for TensorFlow 2</h3>
         
         [![Pip Downloads](https://img.shields.io/pypi/dm/gradient-accumulator?label=pip%20downloads&logo=python)](https://pypi.org/project/gradient-accumulator/)
         [![PyPI version](https://badge.fury.io/py/gradient-accumulator.svg)](https://badge.fury.io/py/gradient-accumulator)
         [![License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7890319.svg)](https://doi.org/10.5281/zenodo.7890319)
+        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6615018.svg)](https://doi.org/10.5281/zenodo.6615018)
         
         **GradientAccumulator** was developed by SINTEF Health due to the lack of an easy-to-use method for gradient accumulation in TensorFlow 2.
         
-        The package is available on PyPI and is compatible with and have been tested against `TensorFlow 2.2-2.12` and `Python 3.6-3.12`, and works cross-platform (Ubuntu, Windows, macOS).
+        The package is available on PyPI and is compatible with and have been tested against `TensorFlow 2.2-2.10` and `Python 3.6-3.11`, and works cross-platform (Ubuntu, Windows, macOS).
         </div>
         
         ## [Continuous integration](https://github.com/andreped/GradientAccumulator#continuous-integration)
         
         | Build Type | Status |
         | - | - |
         | **Code coverage** | [![codecov](https://codecov.io/gh/andreped/GradientAccumulator/branch/main/graph/badge.svg?token=MWLK71V750)](https://codecov.io/gh/andreped/GradientAccumulator) |
@@ -57,66 +57,69 @@
         
         In practice, using gradient accumulation with a custom pipeline might require some extra overhead and tricks to get working.
         
         For more information, see documentations which are hosted at [gradientaccumulator.readthedocs.io](https://gradientaccumulator.readthedocs.io/en/latest/)
         
         
         ## [What?](https://github.com/andreped/GradientAccumulator#what)
-        Gradient accumulation (GA) enables reduced GPU memory consumption through dividing a batch into smaller reduced batches, and performing gradient computation either in a distributing setting across multiple GPUs or sequentially on the same GPU. When the full batch is processed, the gradients are the _accumulated_ to produce the full batch gradient.
+        Gradient accumulation (GA) enables reduced GPU memory consumption through dividing a batch into smaller reduced batches, and performing gradient computation either in a distributing setting across multiple GPUs or sequentially on the same GPU. When the full batch is processed, the gradients are then _accumulated_ to produce the full batch gradient.
         
         <p align="center">
         <img src="assets/grad_accum.png" width="70%">
         </p>
         
+        Note that the very natural how we perform gradient accumulation is slightly different to avoid us needing to have the entire batch in CPU memory. More information on what goes under the hood can be seen in the [documentations](https://gradientaccumulator.readthedocs.io/en/latest/background/gradient_accumulation.html).
+        
         
         ## [Why?](https://github.com/andreped/GradientAccumulator#why)
         In TensorFlow 2, there did not exist a plug-and-play method to use gradient accumulation with any custom pipeline. Hence, we have implemented two generic TF2-compatible approaches:
         
         | Method | Usage |
         | - | - |
         | `GradientAccumulateModel` | `model = GradientAccumulateModel(accum_steps=4, inputs=model.input, outputs=model.output)` |
         | `GradientAccumulateOptimizer` | `opt = GradientAccumulateOptimizer(accum_steps=4, optimizer=tf.keras.optimizers.SGD(1e-2))` |
         
-        Both approaches control how frequently the weigths are updated, but in their own way. Approach (1) is for single-GPU only, whereas (2) supports both single-GPU and distributed training (multi-GPU). However, note that (2) is not yet working as intended. Hence, use (1) for most applications.
+        Both approaches control how frequently the weigths are updated but in their own way. Approach (1) overrides the `train_step` method of a given Model, whereas approach (2) wraps the optimizer. (1) is only compatible with single-GPU usage, whereas (2) also supports distributed training (multi-GPU).
         
         Our implementations enable theoretically **infinitely large batch size**, with **identical memory consumption** as for a regular mini batch. If a single GPU is used, this comes at the cost of increased training runtime. Multiple GPUs could be used to improve runtime performance.
         
         | Technique | Usage |
         | - | - |
         | `Batch Normalization` | `layer = AccumBatchNormalization(accum_steps=4)` |
         | `Adaptive Gradient Clipping` | `model = GradientAccumulateModel(accum_steps=4, agc=True, inputs=model.input, outputs=model.output)` |
         | `Mixed precision` | `model = GradientAccumulateModel(accum_steps=4, mixed_precision=True, inputs=model.input, outputs=model.output)` |
         
         * As batch normalization (BN) is not natively compatible with GA, we have implemented a custom BN layer which can be used as a drop-in replacement.
         * Support for adaptive gradient clipping has been added as an alternative to BN.
         * Mixed precision can also be utilized on both GPUs and TPUs.
+        * Multi-GPU distributed training using generic optimizer wrapper.
         
         For more information on usage, supported techniques, and examples, refer to [the documentations](https://gradientaccumulator.readthedocs.io/en/latest/).
         
         
         ## [Acknowledgements](https://github.com/andreped/GradientAccumulator#acknowledgements)
         The gradient accumulator model wrapper is based on the implementation presented in [this thread](https://stackoverflow.com/a/66524901) on stack overflow. The adaptive gradient clipping method is based on [the implementation by @sayakpaul](https://github.com/sayakpaul/Adaptive-Gradient-Clipping).
         The optimizer wrapper is derived from [the implementation by @fsx950223 and @stefan-falk](https://github.com/tensorflow/addons/pull/2525).
         
-        The documentations hosted [here](https://gradientaccumulator.readthedocs.io/en/latest/index.html) was made possible by the incredible [ReadTheDocs team](https://readthedocs.org/) which offer free documentation hosting!
+        The documentations hosted [here](https://gradientaccumulator.readthedocs.io/en/latest/index.html) was made possible by the incredible [Read The Docs team](https://readthedocs.org/) which offer free documentation hosting!
         
           
         ## [How to cite?](https://github.com/andreped/GradientAccumulator#how-to-cite)
         If you used this package or found the project relevant in your research, please, include the following citation:
         
         ```
-        @software{andre_pedersen_2023_7890319,
-          author       = {André Pedersen and Javier Pérez de Frutos and David Bouget},
-          title        = {andreped/GradientAccumulator: v0.4.2},
+        @software{andre_pedersen_2023_7905351,
+          author       = {André Pedersen and Tor-Arne Schmidt Nordmo and Javier Pérez de Frutos and David Bouget},
+          title        = {andreped/GradientAccumulator: v0.5.0},
           month        = may,
           year         = 2023,
           publisher    = {Zenodo},
-          version      = {v0.4.2},
-          doi          = {10.5281/zenodo.7890319},
-          url          = {https://doi.org/10.5281/zenodo.7890319}
+          version      = {v0.5.0},
+          doi          = {10.5281/zenodo.7905351},
+          url          = {https://doi.org/10.5281/zenodo.7905351}
         }
         ```
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `gradient-accumulator-0.4.2/README.md` & `gradient-accumulator-0.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 <img src="assets/accum_grad_v5_reduced.png" width="35%" alt='gradient-accumulator'>
 <h1 align="center">GradientAccumulator</h1>
 <h3 align="center">Seemless gradient accumulation for TensorFlow 2</h3>
 
 [![Pip Downloads](https://img.shields.io/pypi/dm/gradient-accumulator?label=pip%20downloads&logo=python)](https://pypi.org/project/gradient-accumulator/)
 [![PyPI version](https://badge.fury.io/py/gradient-accumulator.svg)](https://badge.fury.io/py/gradient-accumulator)
 [![License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7890319.svg)](https://doi.org/10.5281/zenodo.7890319)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6615018.svg)](https://doi.org/10.5281/zenodo.6615018)
 
 **GradientAccumulator** was developed by SINTEF Health due to the lack of an easy-to-use method for gradient accumulation in TensorFlow 2.
 
-The package is available on PyPI and is compatible with and have been tested against `TensorFlow 2.2-2.12` and `Python 3.6-3.12`, and works cross-platform (Ubuntu, Windows, macOS).
+The package is available on PyPI and is compatible with and have been tested against `TensorFlow 2.2-2.10` and `Python 3.6-3.11`, and works cross-platform (Ubuntu, Windows, macOS).
 </div>
 
 ## [Continuous integration](https://github.com/andreped/GradientAccumulator#continuous-integration)
 
 | Build Type | Status |
 | - | - |
 | **Code coverage** | [![codecov](https://codecov.io/gh/andreped/GradientAccumulator/branch/main/graph/badge.svg?token=MWLK71V750)](https://codecov.io/gh/andreped/GradientAccumulator) |
@@ -49,61 +49,64 @@
 
 In practice, using gradient accumulation with a custom pipeline might require some extra overhead and tricks to get working.
 
 For more information, see documentations which are hosted at [gradientaccumulator.readthedocs.io](https://gradientaccumulator.readthedocs.io/en/latest/)
 
 
 ## [What?](https://github.com/andreped/GradientAccumulator#what)
-Gradient accumulation (GA) enables reduced GPU memory consumption through dividing a batch into smaller reduced batches, and performing gradient computation either in a distributing setting across multiple GPUs or sequentially on the same GPU. When the full batch is processed, the gradients are the _accumulated_ to produce the full batch gradient.
+Gradient accumulation (GA) enables reduced GPU memory consumption through dividing a batch into smaller reduced batches, and performing gradient computation either in a distributing setting across multiple GPUs or sequentially on the same GPU. When the full batch is processed, the gradients are then _accumulated_ to produce the full batch gradient.
 
 <p align="center">
 <img src="assets/grad_accum.png" width="70%">
 </p>
 
+Note that the very natural how we perform gradient accumulation is slightly different to avoid us needing to have the entire batch in CPU memory. More information on what goes under the hood can be seen in the [documentations](https://gradientaccumulator.readthedocs.io/en/latest/background/gradient_accumulation.html).
+
 
 ## [Why?](https://github.com/andreped/GradientAccumulator#why)
 In TensorFlow 2, there did not exist a plug-and-play method to use gradient accumulation with any custom pipeline. Hence, we have implemented two generic TF2-compatible approaches:
 
 | Method | Usage |
 | - | - |
 | `GradientAccumulateModel` | `model = GradientAccumulateModel(accum_steps=4, inputs=model.input, outputs=model.output)` |
 | `GradientAccumulateOptimizer` | `opt = GradientAccumulateOptimizer(accum_steps=4, optimizer=tf.keras.optimizers.SGD(1e-2))` |
 
-Both approaches control how frequently the weigths are updated, but in their own way. Approach (1) is for single-GPU only, whereas (2) supports both single-GPU and distributed training (multi-GPU). However, note that (2) is not yet working as intended. Hence, use (1) for most applications.
+Both approaches control how frequently the weigths are updated but in their own way. Approach (1) overrides the `train_step` method of a given Model, whereas approach (2) wraps the optimizer. (1) is only compatible with single-GPU usage, whereas (2) also supports distributed training (multi-GPU).
 
 Our implementations enable theoretically **infinitely large batch size**, with **identical memory consumption** as for a regular mini batch. If a single GPU is used, this comes at the cost of increased training runtime. Multiple GPUs could be used to improve runtime performance.
 
 | Technique | Usage |
 | - | - |
 | `Batch Normalization` | `layer = AccumBatchNormalization(accum_steps=4)` |
 | `Adaptive Gradient Clipping` | `model = GradientAccumulateModel(accum_steps=4, agc=True, inputs=model.input, outputs=model.output)` |
 | `Mixed precision` | `model = GradientAccumulateModel(accum_steps=4, mixed_precision=True, inputs=model.input, outputs=model.output)` |
 
 * As batch normalization (BN) is not natively compatible with GA, we have implemented a custom BN layer which can be used as a drop-in replacement.
 * Support for adaptive gradient clipping has been added as an alternative to BN.
 * Mixed precision can also be utilized on both GPUs and TPUs.
+* Multi-GPU distributed training using generic optimizer wrapper.
 
 For more information on usage, supported techniques, and examples, refer to [the documentations](https://gradientaccumulator.readthedocs.io/en/latest/).
 
 
 ## [Acknowledgements](https://github.com/andreped/GradientAccumulator#acknowledgements)
 The gradient accumulator model wrapper is based on the implementation presented in [this thread](https://stackoverflow.com/a/66524901) on stack overflow. The adaptive gradient clipping method is based on [the implementation by @sayakpaul](https://github.com/sayakpaul/Adaptive-Gradient-Clipping).
 The optimizer wrapper is derived from [the implementation by @fsx950223 and @stefan-falk](https://github.com/tensorflow/addons/pull/2525).
 
-The documentations hosted [here](https://gradientaccumulator.readthedocs.io/en/latest/index.html) was made possible by the incredible [ReadTheDocs team](https://readthedocs.org/) which offer free documentation hosting!
+The documentations hosted [here](https://gradientaccumulator.readthedocs.io/en/latest/index.html) was made possible by the incredible [Read The Docs team](https://readthedocs.org/) which offer free documentation hosting!
 
   
 ## [How to cite?](https://github.com/andreped/GradientAccumulator#how-to-cite)
 If you used this package or found the project relevant in your research, please, include the following citation:
 
 ```
-@software{andre_pedersen_2023_7890319,
-  author       = {André Pedersen and Javier Pérez de Frutos and David Bouget},
-  title        = {andreped/GradientAccumulator: v0.4.2},
+@software{andre_pedersen_2023_7905351,
+  author       = {André Pedersen and Tor-Arne Schmidt Nordmo and Javier Pérez de Frutos and David Bouget},
+  title        = {andreped/GradientAccumulator: v0.5.0},
   month        = may,
   year         = 2023,
   publisher    = {Zenodo},
-  version      = {v0.4.2},
-  doi          = {10.5281/zenodo.7890319},
-  url          = {https://doi.org/10.5281/zenodo.7890319}
+  version      = {v0.5.0},
+  doi          = {10.5281/zenodo.7905351},
+  url          = {https://doi.org/10.5281/zenodo.7905351}
 }
 ```
```

### Comparing `gradient-accumulator-0.4.2/gradient_accumulator/agc.py` & `gradient-accumulator-0.5.0/gradient_accumulator/agc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import tensorflow as tf
 
 
-# implementation from: https://github.com/sayakpaul/Adaptive-Gradient-Clipping/blob/main/agc.py
+# implementation from: https://github.com/sayakpaul/Adaptive-Gradient-Clipping/blob/main/agc.py  # noqa
 def compute_norm(x, axis, keepdims):
     """
     Computes the euclidean norm of a tensor :math:`x`.
 
     Args:
         x: input tensor.
         axis: which axis to compute norm across.
         keepdims: whether to keep dimension after applying along axis.
-    
+
     Returns:
         Euclidean norm.
     """
-    return tf.math.reduce_sum(x ** 2, axis=axis, keepdims=keepdims) ** 0.5
+    return tf.math.reduce_sum(x**2, axis=axis, keepdims=keepdims) ** 0.5
 
 
 def unitwise_norm(x):
     """
     Wrapper class which dynamically sets `axis` and `keepdims` given an
     input `x` for calculating euclidean norm.
 
@@ -27,41 +27,50 @@
 
     Returns:
         Euclidean norm.
     """
     if len(x.get_shape()) <= 1:  # Scalars and vectors
         axis = None
         keepdims = False
-    elif len(x.get_shape()) in [2, 3]:  # Linear layers of shape IO or multihead linear
+    elif len(x.get_shape()) in [
+        2,
+        3,
+    ]:  # Linear layers of shape IO or multihead linear
         axis = 0
         keepdims = True
     elif len(x.get_shape()) == 4:  # Conv kernels of shape HWIO
         axis = [0, 1, 2]
         keepdims = True
     elif len(x.get_shape()) == 5:  # Conv kernels of shape HWDIO
         axis = [0, 1, 2, 3]
         keepdims = True
     else:
         raise ValueError(f"Got a parameter with shape not in [1, 2, 4, 5]! {x}")
     return compute_norm(x, axis, keepdims)
 
 
-def adaptive_clip_grad(parameters, gradients, clip_factor: float = 0.01, eps: float = 1e-3):
-    """
-    Performs adaptive gradient clipping on a given set of parameters and gradients.
-
-    * Official JAX implementation (paper authors): https://github.com/deepmind/deepmind-research/tree/master/nfnets
-    * Ross Wightman's implementation https://github.com/rwightman/pytorch-image-models/blob/master/timm/utils/agc.py
+def adaptive_clip_grad(
+    parameters, gradients, clip_factor: float = 0.01, eps: float = 1e-3
+):
+    """
+    Performs adaptive gradient clipping on a given set of parameters and
+    gradients.
+
+    * Official JAX implementation (paper authors):
+      https://github.com/deepmind/deepmind-research/tree/master/nfnets  # noqa
+    * Ross Wightman's implementation
+      https://github.com/rwightman/pytorch-image-models/blob/master/timm/utils/agc.py  # noqa
 
     Args:
         parameters: Which parameters to apply method on.
         gradients: Which gradients to apply clipping on.
         clip_factor: Sets upper limit for gradient clipping.
-        eps: Epsilon - small number in :math:`max()` to avoid zero norm and preserve numerical stability.
-    
+        eps: Epsilon - small number in :math:`max()` to avoid zero norm and
+            preserve numerical stability.
+
     Returns:
         Updated gradients after gradient clipping.
     """
     new_grads = []
     for (params, grads) in zip(parameters, gradients):
         p_norm = unitwise_norm(params)
         max_norm = tf.math.maximum(p_norm, eps) * clip_factor
```

### Comparing `gradient-accumulator-0.4.2/gradient_accumulator/layers.py` & `gradient-accumulator-0.5.0/gradient_accumulator/layers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,56 @@
-from tensorflow.keras.layers import Layer
-from tensorflow.keras import initializers
 import tensorflow as tf
+from tensorflow.keras.layers import Layer
 
 
-# https://stackoverflow.com/questions/65195956/keras-custom-batch-normalization-layer-with-an-extra-variable-that-can-be-change
+# https://stackoverflow.com/questions/65195956/keras-custom-batch-normalization-layer-with-an-extra-variable-that-can-be-change  # noqa
 # https://github.com/dksakkos/BatchNorm/blob/main/BatchNorm.py
 @tf.keras.utils.register_keras_serializable()
 class AccumBatchNormalization(Layer):
     """Custom Batch Normaliztion layer with gradient accumulation support."""
-    def __init__(self, accum_steps: int = 1, momentum: float = 0.99, epsilon:float = 1e-3, trainable:bool = True, **kwargs):
+
+    def __init__(
+        self,
+        accum_steps: int = 1,
+        momentum: float = 0.99,
+        epsilon: float = 1e-3,
+        trainable: bool = True,
+        **kwargs
+    ):
         """Construct the AccumBatchNormalization layer.
 
         Args:
             accum_steps: int > 0. Update gradient in every accumulation steps.
             momentum: float [0, 1]. Momentum used in variable update.
             epsilon: float > 0: Small value to aid numerical stability.
-            trainable: bool: Whether layer should be updated during training. Different from training/inference mode.
-            **kwargs: keyword arguments. Supports various arguments from the Keras' Layer class.
+            trainable: bool: Whether layer should be updated during training.
+                Different from training/inference mode.
+            **kwargs: keyword arguments. Supports various arguments from the
+                Keras' Layer class.
         """
         self.accum_steps = accum_steps
-        self.accum_steps_tf = tf.constant(accum_steps, dtype=tf.int32, name="accum_steps")
+        self.accum_steps_tf = tf.constant(
+            accum_steps, dtype=tf.int32, name="accum_steps"
+        )
         self.momentum = momentum
         self.epsilon = epsilon
         self.trainable = trainable
         self.accum_step_counter = tf.Variable(
-            0, dtype=tf.int32, trainable=False, name="accum_counter",
+            0,
+            dtype=tf.int32,
+            trainable=False,
+            name="accum_counter",
             synchronization=tf.VariableSynchronization.ON_READ,
             aggregation=tf.VariableAggregation.ONLY_FIRST_REPLICA,
         )
         super().__init__(**kwargs)
 
     def build(self, input_shape):
         """Builds layer and variables.
-        
+
         Args:
             input_shape: input feature map size.
         """
         self.param_shape = input_shape[-1]
 
         self.beta = self.add_weight(
             shape=(self.param_shape),
@@ -88,157 +102,165 @@
             aggregation=tf.VariableAggregation.MEAN,
             experimental_autocast=False,
         )
 
         self.accum_variance = self.add_weight(
             shape=(self.param_shape),
             dtype=self.dtype,
-            initializer="zeros",  # this should be "zeros" as we use it for accumulation
+            initializer="zeros",
             trainable=False,
             name="accum_variance",
             synchronization=tf.VariableSynchronization.ON_READ,
             aggregation=tf.VariableAggregation.MEAN,
             experimental_autocast=False,
         )
 
     def get_moving_average(self, statistic, new_value):
         """Returns the moving average given a statistic and current estimate.
-        
+
         Args:
-            statistic: summary statistic e.g. average across for single feature over multiple samples
+            statistic: summary statistic e.g. average across for single
+                feature over multiple samples
             new_value: statistic of single feature for single forward step.
         Returns:
             Updated statistic.
         """
         decay = tf.convert_to_tensor(1.0 - self.momentum, name="decay")
         if decay.dtype != statistic.dtype.base_dtype:
             decay = tf.cast(decay, statistic.dtype.base_dtype)
         delta = (statistic - tf.cast(new_value, statistic.dtype)) * decay
         return statistic.assign_sub(delta)
-    
+
     def update_variables(self, mean, var):
         """Updates the batch normalization variables.
-        
+
         Args:
             mean: average for single feature
             var: variance for single feature
         """
         self.moving_mean.assign(self.get_moving_average(self.moving_mean, mean))
-        self.moving_variance.assign(self.get_moving_average(self.moving_variance, var))
+        self.moving_variance.assign(
+            self.get_moving_average(self.moving_variance, var)
+        )
 
         self.reset_accum()
-    
+
     def reset_accum(self):
         """Resets accumulator slots."""
         self.accum_mean.assign(tf.zeros_like(self.accum_mean))
         self.accum_variance.assign(tf.zeros_like(self.accum_variance))
 
         self.accum_step_counter.assign(0)
 
     def call(self, inputs, training=None, mask=None):
         """Performs the batch normalization step.
-        
+
         Args:
             inputs: input feature map to apply batch normalization across.
             training: whether layer should be in training mode or not.
-            mask: whether to calculate statistics within masked region of feature map.
+            mask: whether to calculate statistics within masked region of
+                feature map.
         Returns:
             Normalized feature map.
         """
         self.inputs_dtype = inputs.dtype.base_dtype
         if self.inputs_dtype in (tf.float16, tf.bfloat16):
             # Do all math in float32 if given 16-bit inputs for numeric
-            # stability.  In particular, it's very easy for variance to overflow
-            # in float16 and for safety we also choose to cast bfloat16 to
-            # float32.
+            # stability. In particular, it's very easy for variance to
+            # overflow in float16 and for safety we also choose to cast
+            # bfloat16 to float32.
             inputs = tf.cast(inputs, self.dtype)
 
         if training:
             assert len(inputs.shape) in (2, 4, 5)
             if len(inputs.shape) > 2:
                 axes = list(range(len(inputs.shape)))[:-1]
             else:
                 axes = [0]
-            
+
             # step accum count
             self.accum_step_counter.assign_add(1)
-            
+
             # get batch norm statistics
             mean, var = tf.nn.moments(inputs, axes=axes, keepdims=False)
 
             # scale mean and variance to produce mean later
             mean_scaled = mean / tf.cast(self.accum_steps_tf, mean.dtype)
             var_scaled = var / tf.cast(self.accum_steps_tf, var.dtype)
-            
+
             # accumulate statistics
             self.accum_mean.assign_add(mean_scaled)
             self.accum_variance.assign_add(var_scaled)
 
             # only update variables after n accumulation steps
             tf.cond(
                 tf.equal(self.accum_step_counter, self.accum_steps_tf),
-                true_fn=lambda: self.update_variables(self.accum_mean, self.accum_variance),
-                false_fn=lambda: None
+                true_fn=lambda: self.update_variables(
+                    self.accum_mean, self.accum_variance
+                ),
+                false_fn=lambda: None,
             )
         else:
             mean, var = self.moving_mean, self.moving_variance
 
         scale = self.gamma
         offset = self.beta
-        
+
         inv = tf.math.rsqrt(var + self.epsilon)
         if scale is not None:
             inv *= scale
-        
-        outputs =  inputs * tf.cast(inv, inputs.dtype) + \
-            tf.cast(offset - mean * inv if offset is not None else -mean * inv, inputs.dtype)
-        
+
+        outputs = inputs * tf.cast(inv, inputs.dtype) + tf.cast(
+            offset - mean * inv if offset is not None else -mean * inv,
+            inputs.dtype,
+        )
+
         # need to convert back to float16 after applying batch norm
         if self.inputs_dtype in (tf.float16, tf.bfloat16):
             outputs = tf.cast(outputs, self.dtype)
 
         return outputs
-    
+
     @property
     def trainable(self):
         """Returns whether layer is trainable.
-        
+
         Returns:
             trainable boolean state.
         """
         return self._trainable
 
     @trainable.setter
-    def trainable(self, value:bool):
+    def trainable(self, value: bool):
         """Sets trainable variable.
-        
+
         Args:
             value: which boolean state to change variable to.
         """
         self._trainable = value
-    
+
     @property
     def _param_dtype(self):
         """Raise parameters of fp16 batch norm to fp32
-        
+
         Returns:
             dtype of params.
         """
         if self.dtype == tf.float16 or self.dtype == tf.bfloat16:
             return tf.float32
         else:
             return self.dtype or tf.float32
-    
+
     def get_config(self):
         """Returns configurations as dict.
-        
+
         Returns:
             Configuration file.
         """
         config = {
-            'accum_steps': self.accum_steps,
-            'momentum': self.momentum,
-            'epsilon': self.epsilon,
-            'trainable': self.trainable,
+            "accum_steps": self.accum_steps,
+            "momentum": self.momentum,
+            "epsilon": self.epsilon,
+            "trainable": self.trainable,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
```

### Comparing `gradient-accumulator-0.4.2/gradient_accumulator.egg-info/PKG-INFO` & `gradient-accumulator-0.5.0/gradient_accumulator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: gradient-accumulator
-Version: 0.4.2
+Version: 0.5.0
 Summary: Package for gradient accumulation in TensorFlow
 Home-page: https://github.com/andreped/GradientAccumulator
-Author: André Pedersen and David Bouget and Javier Pérez de Frutos
+Author: André Pedersen and David Bouget and Javier Pérez de Frutos and Tor-Arne Schmidt Nordmo
 Author-email: andrped94@gmail.com
 License: UNKNOWN
 Description: <div align="center">
         <img src="assets/accum_grad_v5_reduced.png" width="35%" alt='gradient-accumulator'>
         <h1 align="center">GradientAccumulator</h1>
         <h3 align="center">Seemless gradient accumulation for TensorFlow 2</h3>
         
         [![Pip Downloads](https://img.shields.io/pypi/dm/gradient-accumulator?label=pip%20downloads&logo=python)](https://pypi.org/project/gradient-accumulator/)
         [![PyPI version](https://badge.fury.io/py/gradient-accumulator.svg)](https://badge.fury.io/py/gradient-accumulator)
         [![License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7890319.svg)](https://doi.org/10.5281/zenodo.7890319)
+        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6615018.svg)](https://doi.org/10.5281/zenodo.6615018)
         
         **GradientAccumulator** was developed by SINTEF Health due to the lack of an easy-to-use method for gradient accumulation in TensorFlow 2.
         
-        The package is available on PyPI and is compatible with and have been tested against `TensorFlow 2.2-2.12` and `Python 3.6-3.12`, and works cross-platform (Ubuntu, Windows, macOS).
+        The package is available on PyPI and is compatible with and have been tested against `TensorFlow 2.2-2.10` and `Python 3.6-3.11`, and works cross-platform (Ubuntu, Windows, macOS).
         </div>
         
         ## [Continuous integration](https://github.com/andreped/GradientAccumulator#continuous-integration)
         
         | Build Type | Status |
         | - | - |
         | **Code coverage** | [![codecov](https://codecov.io/gh/andreped/GradientAccumulator/branch/main/graph/badge.svg?token=MWLK71V750)](https://codecov.io/gh/andreped/GradientAccumulator) |
@@ -57,66 +57,69 @@
         
         In practice, using gradient accumulation with a custom pipeline might require some extra overhead and tricks to get working.
         
         For more information, see documentations which are hosted at [gradientaccumulator.readthedocs.io](https://gradientaccumulator.readthedocs.io/en/latest/)
         
         
         ## [What?](https://github.com/andreped/GradientAccumulator#what)
-        Gradient accumulation (GA) enables reduced GPU memory consumption through dividing a batch into smaller reduced batches, and performing gradient computation either in a distributing setting across multiple GPUs or sequentially on the same GPU. When the full batch is processed, the gradients are the _accumulated_ to produce the full batch gradient.
+        Gradient accumulation (GA) enables reduced GPU memory consumption through dividing a batch into smaller reduced batches, and performing gradient computation either in a distributing setting across multiple GPUs or sequentially on the same GPU. When the full batch is processed, the gradients are then _accumulated_ to produce the full batch gradient.
         
         <p align="center">
         <img src="assets/grad_accum.png" width="70%">
         </p>
         
+        Note that the very natural how we perform gradient accumulation is slightly different to avoid us needing to have the entire batch in CPU memory. More information on what goes under the hood can be seen in the [documentations](https://gradientaccumulator.readthedocs.io/en/latest/background/gradient_accumulation.html).
+        
         
         ## [Why?](https://github.com/andreped/GradientAccumulator#why)
         In TensorFlow 2, there did not exist a plug-and-play method to use gradient accumulation with any custom pipeline. Hence, we have implemented two generic TF2-compatible approaches:
         
         | Method | Usage |
         | - | - |
         | `GradientAccumulateModel` | `model = GradientAccumulateModel(accum_steps=4, inputs=model.input, outputs=model.output)` |
         | `GradientAccumulateOptimizer` | `opt = GradientAccumulateOptimizer(accum_steps=4, optimizer=tf.keras.optimizers.SGD(1e-2))` |
         
-        Both approaches control how frequently the weigths are updated, but in their own way. Approach (1) is for single-GPU only, whereas (2) supports both single-GPU and distributed training (multi-GPU). However, note that (2) is not yet working as intended. Hence, use (1) for most applications.
+        Both approaches control how frequently the weigths are updated but in their own way. Approach (1) overrides the `train_step` method of a given Model, whereas approach (2) wraps the optimizer. (1) is only compatible with single-GPU usage, whereas (2) also supports distributed training (multi-GPU).
         
         Our implementations enable theoretically **infinitely large batch size**, with **identical memory consumption** as for a regular mini batch. If a single GPU is used, this comes at the cost of increased training runtime. Multiple GPUs could be used to improve runtime performance.
         
         | Technique | Usage |
         | - | - |
         | `Batch Normalization` | `layer = AccumBatchNormalization(accum_steps=4)` |
         | `Adaptive Gradient Clipping` | `model = GradientAccumulateModel(accum_steps=4, agc=True, inputs=model.input, outputs=model.output)` |
         | `Mixed precision` | `model = GradientAccumulateModel(accum_steps=4, mixed_precision=True, inputs=model.input, outputs=model.output)` |
         
         * As batch normalization (BN) is not natively compatible with GA, we have implemented a custom BN layer which can be used as a drop-in replacement.
         * Support for adaptive gradient clipping has been added as an alternative to BN.
         * Mixed precision can also be utilized on both GPUs and TPUs.
+        * Multi-GPU distributed training using generic optimizer wrapper.
         
         For more information on usage, supported techniques, and examples, refer to [the documentations](https://gradientaccumulator.readthedocs.io/en/latest/).
         
         
         ## [Acknowledgements](https://github.com/andreped/GradientAccumulator#acknowledgements)
         The gradient accumulator model wrapper is based on the implementation presented in [this thread](https://stackoverflow.com/a/66524901) on stack overflow. The adaptive gradient clipping method is based on [the implementation by @sayakpaul](https://github.com/sayakpaul/Adaptive-Gradient-Clipping).
         The optimizer wrapper is derived from [the implementation by @fsx950223 and @stefan-falk](https://github.com/tensorflow/addons/pull/2525).
         
-        The documentations hosted [here](https://gradientaccumulator.readthedocs.io/en/latest/index.html) was made possible by the incredible [ReadTheDocs team](https://readthedocs.org/) which offer free documentation hosting!
+        The documentations hosted [here](https://gradientaccumulator.readthedocs.io/en/latest/index.html) was made possible by the incredible [Read The Docs team](https://readthedocs.org/) which offer free documentation hosting!
         
           
         ## [How to cite?](https://github.com/andreped/GradientAccumulator#how-to-cite)
         If you used this package or found the project relevant in your research, please, include the following citation:
         
         ```
-        @software{andre_pedersen_2023_7890319,
-          author       = {André Pedersen and Javier Pérez de Frutos and David Bouget},
-          title        = {andreped/GradientAccumulator: v0.4.2},
+        @software{andre_pedersen_2023_7905351,
+          author       = {André Pedersen and Tor-Arne Schmidt Nordmo and Javier Pérez de Frutos and David Bouget},
+          title        = {andreped/GradientAccumulator: v0.5.0},
           month        = may,
           year         = 2023,
           publisher    = {Zenodo},
-          version      = {v0.4.2},
-          doi          = {10.5281/zenodo.7890319},
-          url          = {https://doi.org/10.5281/zenodo.7890319}
+          version      = {v0.5.0},
+          doi          = {10.5281/zenodo.7905351},
+          url          = {https://doi.org/10.5281/zenodo.7905351}
         }
         ```
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `gradient-accumulator-0.4.2/setup.py` & `gradient-accumulator-0.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gradient-accumulator",
-    version="0.4.2",
-    author="André Pedersen and David Bouget and Javier Pérez de Frutos",
+    version="0.5.0",
+    author="André Pedersen and David Bouget and Javier Pérez de Frutos and Tor-Arne Schmidt Nordmo",
     author_email="andrped94@gmail.com",
     description="Package for gradient accumulation in TensorFlow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andreped/GradientAccumulator",
-    packages=setuptools.find_packages(exclude=('tests', 'notebooks', 'assets', 'docs')),
+    packages=setuptools.find_packages(exclude=('tests', 'notebooks', 'assets', 'docs', 'shell')),
     install_requires=[
         "tensorflow",
+        "numpy<=1.23.2",
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

