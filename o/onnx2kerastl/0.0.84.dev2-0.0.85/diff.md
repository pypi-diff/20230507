# Comparing `tmp/onnx2kerastl-0.0.84.dev2.tar.gz` & `tmp/onnx2kerastl-0.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2kerastl-0.0.84.dev2.tar", max compression
+gzip compressed data, was "onnx2kerastl-0.0.85.tar", max compression
```

## Comparing `onnx2kerastl-0.0.84.dev2.tar` & `onnx2kerastl-0.0.85.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1067 2022-05-24 12:10:46.678537 onnx2kerastl-0.0.84.dev2/LICENSE
--rw-r--r--   0        0        0       66 2022-05-29 07:44:17.204667 onnx2kerastl-0.0.84.dev2/onnx2kerastl/__init__.py
--rw-r--r--   0        0        0     8121 2023-04-25 09:04:27.467793 onnx2kerastl-0.0.84.dev2/onnx2kerastl/activation_layers.py
--rw-r--r--   0        0        0     1127 2022-08-04 13:51:21.421383 onnx2kerastl-0.0.84.dev2/onnx2kerastl/caffe2_layers.py
--rw-r--r--   0        0        0      780 2022-10-03 15:38:22.085235 onnx2kerastl-0.0.84.dev2/onnx2kerastl/constant_layers.py
--rw-r--r--   0        0        0    13188 2023-04-25 09:04:27.468662 onnx2kerastl-0.0.84.dev2/onnx2kerastl/converter.py
--rw-r--r--   0        0        0    11246 2023-04-25 09:04:27.469775 onnx2kerastl-0.0.84.dev2/onnx2kerastl/convolution_layers.py
--rw-r--r--   0        0        0      499 2022-10-23 09:48:40.399695 onnx2kerastl-0.0.84.dev2/onnx2kerastl/customonnxlayer/__init__.py
--rw-r--r--   0        0        0      236 2022-10-23 09:48:40.399903 onnx2kerastl-0.0.84.dev2/onnx2kerastl/customonnxlayer/onnxabs.py
--rw-r--r--   0        0        0      236 2022-05-30 13:34:03.376696 onnx2kerastl-0.0.84.dev2/onnx2kerastl/customonnxlayer/onnxerf.py
--rw-r--r--   0        0        0      606 2022-05-24 12:10:46.680353 onnx2kerastl-0.0.84.dev2/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
--rw-r--r--   0        0        0      605 2022-09-19 17:39:21.485803 onnx2kerastl-0.0.84.dev2/onnx2kerastl/customonnxlayer/onnxreducemean.py
--rw-r--r--   0        0        0      238 2022-05-30 13:34:03.376950 onnx2kerastl-0.0.84.dev2/onnx2kerastl/customonnxlayer/onnxsqrt.py
--rw-r--r--   0        0        0     9372 2023-04-25 09:04:27.470634 onnx2kerastl-0.0.84.dev2/onnx2kerastl/elementwise_layers.py
--rw-r--r--   0        0        0      179 2022-08-04 13:51:21.427113 onnx2kerastl-0.0.84.dev2/onnx2kerastl/exceptions.py
--rw-r--r--   0        0        0     3867 2023-04-25 09:04:27.471185 onnx2kerastl-0.0.84.dev2/onnx2kerastl/layers.py
--rw-r--r--   0        0        0     2301 2023-01-19 11:41:57.593097 onnx2kerastl-0.0.84.dev2/onnx2kerastl/linear_layers.py
--rw-r--r--   0        0        0     3309 2023-04-25 09:04:27.471485 onnx2kerastl-0.0.84.dev2/onnx2kerastl/ltsm_layers.py
--rw-r--r--   0        0        0      368 2022-05-24 12:10:46.680940 onnx2kerastl-0.0.84.dev2/onnx2kerastl/main.py
--rw-r--r--   0        0        0     5328 2023-01-19 11:41:57.594159 onnx2kerastl-0.0.84.dev2/onnx2kerastl/normalization_layers.py
--rw-r--r--   0        0        0    15619 2023-04-25 09:04:27.472069 onnx2kerastl-0.0.84.dev2/onnx2kerastl/operation_layers.py
--rw-r--r--   0        0        0     3015 2023-04-25 09:04:27.472631 onnx2kerastl-0.0.84.dev2/onnx2kerastl/padding_layers.py
--rw-r--r--   0        0        0     7464 2023-01-19 11:41:57.596399 onnx2kerastl-0.0.84.dev2/onnx2kerastl/pooling_layers.py
--rw-r--r--   0        0        0    16675 2023-04-25 09:04:27.473257 onnx2kerastl-0.0.84.dev2/onnx2kerastl/reshape_layers.py
--rw-r--r--   0        0        0     5354 2023-04-25 09:04:27.473770 onnx2kerastl-0.0.84.dev2/onnx2kerastl/sampling_layers.py
--rw-r--r--   0        0        0     1655 2023-01-19 11:41:57.597650 onnx2kerastl-0.0.84.dev2/onnx2kerastl/upsampling_layers.py
--rw-r--r--   0        0        0     4415 2023-01-19 11:41:57.597962 onnx2kerastl-0.0.84.dev2/onnx2kerastl/utils.py
--rw-r--r--   0        0        0      986 2023-05-07 06:58:52.618336 onnx2kerastl-0.0.84.dev2/pyproject.toml
--rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.84.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-05-24 13:45:54.506384 onnx2kerastl-0.0.85/LICENSE
+-rw-r--r--   0        0        0       66 2022-05-26 14:37:02.229998 onnx2kerastl-0.0.85/onnx2kerastl/__init__.py
+-rw-r--r--   0        0        0     8121 2023-04-30 14:23:13.629683 onnx2kerastl-0.0.85/onnx2kerastl/activation_layers.py
+-rw-r--r--   0        0        0     1127 2022-07-21 11:24:20.166257 onnx2kerastl-0.0.85/onnx2kerastl/caffe2_layers.py
+-rw-r--r--   0        0        0      780 2022-10-13 14:52:08.546058 onnx2kerastl-0.0.85/onnx2kerastl/constant_layers.py
+-rw-r--r--   0        0        0    13188 2023-04-02 11:17:38.559496 onnx2kerastl-0.0.85/onnx2kerastl/converter.py
+-rw-r--r--   0        0        0    13847 2023-04-30 14:23:50.230260 onnx2kerastl-0.0.85/onnx2kerastl/convolution_layers.py
+-rw-r--r--   0        0        0      499 2022-10-19 12:00:07.113116 onnx2kerastl-0.0.85/onnx2kerastl/customonnxlayer/__init__.py
+-rw-r--r--   0        0        0      236 2022-10-19 12:00:07.113921 onnx2kerastl-0.0.85/onnx2kerastl/customonnxlayer/onnxabs.py
+-rw-r--r--   0        0        0      236 2022-05-30 10:49:29.064709 onnx2kerastl-0.0.85/onnx2kerastl/customonnxlayer/onnxerf.py
+-rw-r--r--   0        0        0      606 2022-05-24 13:45:54.510879 onnx2kerastl-0.0.85/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
+-rw-r--r--   0        0        0      605 2022-08-04 16:14:29.703956 onnx2kerastl-0.0.85/onnx2kerastl/customonnxlayer/onnxreducemean.py
+-rw-r--r--   0        0        0      238 2022-05-30 11:45:55.347781 onnx2kerastl-0.0.85/onnx2kerastl/customonnxlayer/onnxsqrt.py
+-rw-r--r--   0        0        0     9372 2023-04-30 14:23:13.630051 onnx2kerastl-0.0.85/onnx2kerastl/elementwise_layers.py
+-rw-r--r--   0        0        0      179 2022-07-21 11:24:20.167508 onnx2kerastl-0.0.85/onnx2kerastl/exceptions.py
+-rw-r--r--   0        0        0     3867 2023-04-30 14:23:13.630361 onnx2kerastl-0.0.85/onnx2kerastl/layers.py
+-rw-r--r--   0        0        0     2301 2023-04-02 11:17:38.561077 onnx2kerastl-0.0.85/onnx2kerastl/linear_layers.py
+-rw-r--r--   0        0        0     3309 2023-04-02 11:17:38.561313 onnx2kerastl-0.0.85/onnx2kerastl/ltsm_layers.py
+-rw-r--r--   0        0        0      368 2022-05-24 13:45:54.512524 onnx2kerastl-0.0.85/onnx2kerastl/main.py
+-rw-r--r--   0        0        0     5551 2023-05-01 11:07:12.428128 onnx2kerastl-0.0.85/onnx2kerastl/normalization_layers.py
+-rw-r--r--   0        0        0    15619 2023-04-30 14:23:13.630719 onnx2kerastl-0.0.85/onnx2kerastl/operation_layers.py
+-rw-r--r--   0        0        0     3015 2023-04-30 14:23:13.631034 onnx2kerastl-0.0.85/onnx2kerastl/padding_layers.py
+-rw-r--r--   0        0        0     7464 2023-04-02 11:17:38.563036 onnx2kerastl-0.0.85/onnx2kerastl/pooling_layers.py
+-rw-r--r--   0        0        0    16675 2023-04-30 14:23:13.631400 onnx2kerastl-0.0.85/onnx2kerastl/reshape_layers.py
+-rw-r--r--   0        0        0     5354 2023-04-30 14:23:13.631673 onnx2kerastl-0.0.85/onnx2kerastl/sampling_layers.py
+-rw-r--r--   0        0        0     1655 2023-04-02 11:17:38.563943 onnx2kerastl-0.0.85/onnx2kerastl/upsampling_layers.py
+-rw-r--r--   0        0        0     4415 2023-04-02 11:17:38.564336 onnx2kerastl-0.0.85/onnx2kerastl/utils.py
+-rw-r--r--   0        0        0     1030 2023-05-01 11:27:13.237750 onnx2kerastl-0.0.85/pyproject.toml
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.85/PKG-INFO
```

### Comparing `onnx2kerastl-0.0.84.dev2/LICENSE` & `onnx2kerastl-0.0.85/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/activation_layers.py` & `onnx2kerastl-0.0.85/onnx2kerastl/activation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/caffe2_layers.py` & `onnx2kerastl-0.0.85/onnx2kerastl/caffe2_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/constant_layers.py` & `onnx2kerastl-0.0.85/onnx2kerastl/constant_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/converter.py` & `onnx2kerastl-0.0.85/onnx2kerastl/converter.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/convolution_layers.py` & `onnx2kerastl-0.0.85/onnx2kerastl/convolution_layers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,32 @@
 import logging
-
+from typing import List
+import tensorflow as tf
 import keras
+from .utils import ensure_tf_type, ensure_numpy_type, is_numpy
+from functools import partial
+from tensorflow.python.framework.ops import EagerTensor
+
+
+def calculate_permute_values(n_dims: int, to_channel_first: bool) -> List[int]:
+    if to_channel_first:
+        return [n_dims - 1] + list(range(1, n_dims - 1))
+    else:
+        return list(range(2, n_dims)) + [1]
+
 
-from .utils import ensure_tf_type, ensure_numpy_type
+def permute_wrap_conv_if_constant(partial_func, conv_input, is_constant):
+    if is_constant:
+        input_shape = tf.shape(conv_input)
+        permuted = keras.layers.Permute(calculate_permute_values(len(input_shape), to_channel_first=False))(conv_input)
+        conv_res = partial_func(data_format="channels_last")(permuted)
+        result = keras.layers.Permute(calculate_permute_values(len(input_shape), to_channel_first=True))(conv_res)
+    else:
+        result = partial_func()(conv_input)
+    return result
 
 
 def convert_conv(node, params, layers, lambda_func, node_name, keras_name):
     """
     Convert convolution layer
     :param node: current operation node
     :param params: operation attributes
@@ -31,14 +51,15 @@
         W = ensure_numpy_type(layers[node.input[1]])
         bias = None
 
     else:
         raise NotImplementedError('Not implemented')
 
     input_0 = ensure_tf_type(layers[node.input[0]], name="%s_const" % keras_name)
+    is_constant = is_numpy(input_0) or isinstance(input_0, EagerTensor)
     n_groups = params['group'] if 'group' in params else 1
     dilation = params['dilations'][0] if 'dilations' in params else 1
     pads = params['pads'] if 'pads' in params else [0, 0, 0]
     strides = params['strides'] if 'strides' in params else [1, 1, 1]
 
     if len(W.shape) == 5:  # 3D conv
         logger.debug('3D convolution')
@@ -53,27 +74,39 @@
         out_channels, channels_per_group, dimension, height, width = W.shape
         W = W.transpose(2, 3, 4, 1, 0)
 
         if has_bias:
             weights = [W, bias]
         else:
             weights = [W]
-        conv = keras.layers.Conv3D(
-            filters=out_channels,
-            kernel_size=(dimension, height, width),
-            strides=(strides[0], strides[1], strides[2]),
-            padding='valid',
-            weights=weights,
-            use_bias=has_bias,
-            activation=None,
-            dilation_rate=dilation,
-            name=keras_name,
-            groups=n_groups
-        )
-        layers[node_name] = conv(input_0)
+        conv_args = { "filters": out_channels,
+        "kernel_size": (dimension, height, width),
+        "strides": (strides[0], strides[1], strides[2]),
+        "padding": 'valid',
+        "weights": weights,
+        "use_bias": has_bias,
+        "activation": None,
+        "dilation_rate": dilation,
+        "name": keras_name,
+        "groups": n_groups}
+        partial_conv = partial(keras.layers.Conv3D, **conv_args)
+        layers[node_name] = permute_wrap_conv_if_constant(partial_conv, input_0, is_constant)
+        # conv = keras.layers.Conv3D(
+        #     filters=out_channels,
+        #     kernel_size=(dimension, height, width),
+        #     strides=(strides[0], strides[1], strides[2]),
+        #     padding='valid',
+        #     weights=weights,
+        #     use_bias=has_bias,
+        #     activation=None,
+        #     dilation_rate=dilation,
+        #     name=keras_name,
+        #     groups=n_groups
+        # )
+        # layers[node_name] = conv(input_0)
 
     elif len(W.shape) == 4:  # 2D conv
         logger.debug('2D convolution')
 
         padding = None
         if len(pads) == 2 and (pads[0] > 0 or pads[1] > 0):
             padding = (pads[0], pads[1])
@@ -93,72 +126,95 @@
         W = W.transpose(2, 3, 1, 0)
         height, width, channels_per_group, out_channels = W.shape
 
         if has_bias:
             weights = [W, bias]
         else:
             weights = [W]
-
-        conv = keras.layers.Conv2D(
-            filters=out_channels,
-            kernel_size=(height, width),
-            strides=(strides[0], strides[1]),
-            padding='valid',
-            weights=weights,
-            use_bias=has_bias,
-            activation=None,
-            dilation_rate=dilation,
-            groups=n_groups,
-            name=keras_name
-        )
-
-        layers[node_name] = conv(input_0)
+        conv_args = {"filters": out_channels,
+        "kernel_size": (height, width),
+        "strides": (strides[0], strides[1]),
+        "padding": 'valid',
+        "weights": weights,
+        "use_bias": has_bias,
+        "activation": None,
+        "dilation_rate": dilation,
+        "name": keras_name,
+        "groups": n_groups}
+        partial_conv = partial(keras.layers.Conv2D, **conv_args)
+        layers[node_name] = permute_wrap_conv_if_constant(partial_conv, input_0, is_constant)
+        # conv = keras.layers.Conv2D(
+        #     filters=out_channels,
+        #     kernel_size=(height, width),
+        #     strides=(strides[0], strides[1]),
+        #     padding='valid',
+        #     weights=weights,
+        #     use_bias=has_bias,
+        #     activation=None,
+        #     dilation_rate=dilation,
+        #     groups=n_groups,
+        #     name=keras_name
+        # )
+        #
+        # layers[node_name] = conv(input_0)
     else:
         # 1D conv
         W = W.transpose(2, 1, 0)
         width, channels, n_filters = W.shape
         print(width, channels, n_filters, has_bias)
 
         if has_bias:
             weights = [W, bias]
         else:
             weights = [W]
 
         padding = None
         if len(pads) == 2 and (pads[0] > 0 or pads[1] > 0):
             padding = (pads[0], pads[1])
-
+        conv_args = {"filters": n_filters,
+        "kernel_size": (width),
+        "strides": (strides[0]),
+        "weights": weights,
+        "use_bias": has_bias,
+        "activation": None,
+        "dilation_rate": dilation,
+        "name": keras_name,
+        "groups": n_groups}
         if padding:
-            conv = keras.layers.Conv1D(
-                filters=n_filters,
-                kernel_size=width,
-                strides=strides[0],
-                padding='same',
-                weights=weights,
-                use_bias=has_bias,
-                activation=None,
-                dilation_rate=dilation,
-                groups=n_groups,
-                name=keras_name,
-                data_format='channels_first')
+            conv_args['padding'] = 'same'
+            # conv = keras.layers.Conv1D(
+            #     filters=n_filters,
+            #     kernel_size=width,
+            #     strides=strides[0],
+            #     padding='same',
+            #     weights=weights,
+            #     use_bias=has_bias,
+            #     activation=None,
+            #     dilation_rate=dilation,
+            #     groups=n_groups,
+            #     name=keras_name,
+            #     data_format='channels_first')
         else:
-            conv = keras.layers.Conv1D(
-                filters=n_filters,
-                kernel_size=width,
-                strides=strides[0],
-                padding='valid',
-                weights=weights,
-                use_bias=has_bias,
-                activation=None,
-                dilation_rate=dilation,
-                groups=n_groups,
-                name=keras_name,
-                data_format='channels_first')
+            conv_args['padding'] = 'valid'
 
-        layers[node_name] = conv(input_0)
+            # conv = keras.layers.Conv1D(
+            #     filters=n_filters,
+            #     kernel_size=width,
+            #     strides=strides[0],
+            #     padding='valid',
+            #     weights=weights,
+            #     use_bias=has_bias,
+            #     activation=None,
+            #     dilation_rate=dilation,
+            #     groups=n_groups,
+            #     name=keras_name,
+            #     data_format='channels_first')
+        partial_conv = partial(keras.layers.Conv1D, **conv_args)
+        layers[node_name] = permute_wrap_conv_if_constant(partial_conv, input_0, is_constant)
+        # layers[node_name] = conv(input_0)
 
         # padding_name = keras_name + '_pad'
         # padding_layer = keras.layers.ZeroPadding1D(
         #     padding=(pads[0]),
         #     name=padding_name
         # )
         # print(input_0)
```

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py` & `onnx2kerastl-0.0.85/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/customonnxlayer/onnxreducemean.py` & `onnx2kerastl-0.0.85/onnx2kerastl/customonnxlayer/onnxreducemean.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/elementwise_layers.py` & `onnx2kerastl-0.0.85/onnx2kerastl/elementwise_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/layers.py` & `onnx2kerastl-0.0.85/onnx2kerastl/layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/linear_layers.py` & `onnx2kerastl-0.0.85/onnx2kerastl/linear_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/ltsm_layers.py` & `onnx2kerastl-0.0.85/onnx2kerastl/ltsm_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/normalization_layers.py` & `onnx2kerastl-0.0.85/onnx2kerastl/normalization_layers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import logging
+
 import keras
+import numpy as np
 import tensorflow as tf
-import tensorflow_addons as tfa
-import logging
+
 from .utils import ensure_tf_type, ensure_numpy_type
 
 
 def convert_batchnorm(node, params, layers, lambda_func, node_name, keras_name):
     """
     Convert BatchNorm2d layer
     :param node: current operation node
@@ -65,34 +67,34 @@
     :param params: operation attributes
     :param layers: available keras layers
     :param lambda_func: function for keras Lambda layer
     :param node_name: internal converter name
     :param keras_name: resulting layer name
     :return: None
     """
+    # based on https://github.com/onnx/onnx/blob/main/docs/Operators.md#InstanceNormalization
     logger = logging.getLogger('onnx2keras.instancenorm2d')
 
     input_0 = ensure_tf_type(layers[node.input[0]], name="%s_const" % keras_name)
 
     if len(node.input) == 3:
-        gamma = ensure_numpy_type(layers[node.input[1]])
-        beta = ensure_numpy_type(layers[node.input[2]])
+        scale = ensure_numpy_type(layers[node.input[1]])
+        bias = ensure_numpy_type(layers[node.input[2]])
     else:
         raise AttributeError('Unknown arguments for instance norm')
 
     epsilon = params['epsilon']
-
-    instance_norm = tfa.layers.InstanceNormalization(
-        axis=1,
-        epsilon=epsilon,
-        beta_initializer=tf.constant_initializer(beta),
-        gamma_initializer=tf.constant_initializer(gamma),
-        trainable=False
-        )
-    layers[node_name] = instance_norm(input_0)
+    dims_x = len(input_0.shape)
+    axis = list(range(2, dims_x))
+    var = tf.math.reduce_variance(input_0, axis=axis, keepdims=True, name=None)
+    mean = tf.math.reduce_mean(input_0, axis=axis, keepdims=True, name=None)
+    dim_ones = (1,) * (dims_x - 2)
+    scale = np.reshape(scale, (-1, *dim_ones))
+    bias = np.reshape(bias, (-1, *dim_ones))
+    layers[node_name] = (input_0 - mean) * scale / tf.sqrt(var + epsilon) + bias
 
 
 def convert_dropout(node, params, layers, lambda_func, node_name, keras_name):
     """
     Convert Dropout layer
     :param node: current operation node
     :param params: operation attributes
```

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/operation_layers.py` & `onnx2kerastl-0.0.85/onnx2kerastl/operation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/padding_layers.py` & `onnx2kerastl-0.0.85/onnx2kerastl/padding_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/pooling_layers.py` & `onnx2kerastl-0.0.85/onnx2kerastl/pooling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/reshape_layers.py` & `onnx2kerastl-0.0.85/onnx2kerastl/reshape_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/sampling_layers.py` & `onnx2kerastl-0.0.85/onnx2kerastl/sampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/upsampling_layers.py` & `onnx2kerastl-0.0.85/onnx2kerastl/upsampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.84.dev2/onnx2kerastl/utils.py` & `onnx2kerastl-0.0.85/onnx2kerastl/utils.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.84.dev2/pyproject.toml` & `onnx2kerastl-0.0.85/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "onnx2kerastl"
-version = "0.0.84.dev2"
+version = "0.0.85"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
-tensorflow = "2.12.0"
-tensorflow-macos = {version = "^2.11.0", markers = "platform_machine  == 'arm64'"}
+tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
+tensorflow-macos = {version = "2.11.0", markers = "platform_machine  == 'arm64'"}
 onnx = "1.10.1"
-protobuf = "^4.21.0"
-keras-data-format-converter = "0.1.15.dev2"
+protobuf = "^3.19.6"
+keras-data-format-converter = "0.1.14"
 tensorflow-addons = {version = "^0.19.0", markers = "platform_machine  == 'x86_64'"}
 numpy = "1.23.5"
 fvcore = "^0.1.5.post20221221"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 torch = {version = "1.12.1", markers = "platform_machine  == 'x86_64'"}
```

### Comparing `onnx2kerastl-0.0.84.dev2/PKG-INFO` & `onnx2kerastl-0.0.85/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: onnx2kerastl
-Version: 0.0.84.dev2
+Version: 0.0.85
 Summary: 
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: fvcore (>=0.1.5.post20221221,<0.2.0)
-Requires-Dist: keras-data-format-converter (==0.1.15.dev2)
+Requires-Dist: keras-data-format-converter (==0.1.14)
 Requires-Dist: numpy (==1.23.5)
 Requires-Dist: onnx (==1.10.1)
-Requires-Dist: protobuf (>=4.21.0,<5.0.0)
-Requires-Dist: tensorflow (==2.12.0)
+Requires-Dist: protobuf (>=3.19.6,<4.0.0)
+Requires-Dist: tensorflow (==2.11.0) ; platform_machine == "x86_64"
 Requires-Dist: tensorflow-addons (>=0.19.0,<0.20.0) ; platform_machine == "x86_64"
-Requires-Dist: tensorflow-macos (>=2.11.0,<3.0.0) ; platform_machine == "arm64"
+Requires-Dist: tensorflow-macos (==2.11.0) ; platform_machine == "arm64"
```

