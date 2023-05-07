# Comparing `tmp/synapgrad-0.3.1-py3-none-any.whl.zip` & `tmp/synapgrad-0.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 29772 bytes, number of entries: 21
+Zip file size: 29809 bytes, number of entries: 21
 -rw-rw-rw-  2.0 fat       72 b- defN 23-Apr-08 18:28 synapgrad/__init__.py
--rw-rw-rw-  2.0 fat    32179 b- defN 23-May-03 18:05 synapgrad/engine.py
+-rw-rw-rw-  2.0 fat    32179 b- defN 23-May-05 17:20 synapgrad/engine.py
 -rw-rw-rw-  2.0 fat      442 b- defN 23-May-01 13:33 synapgrad/nn/__init__.py
 -rw-rw-rw-  2.0 fat     3538 b- defN 23-Apr-20 01:42 synapgrad/nn/activations.py
--rw-rw-rw-  2.0 fat     7831 b- defN 23-Apr-19 17:14 synapgrad/nn/functional.py
+-rw-rw-rw-  2.0 fat     7831 b- defN 23-May-05 17:20 synapgrad/nn/functional.py
 -rw-rw-rw-  2.0 fat     2879 b- defN 23-Apr-20 12:52 synapgrad/nn/initializations.py
--rw-rw-rw-  2.0 fat    18237 b- defN 23-May-03 18:16 synapgrad/nn/layers.py
+-rw-rw-rw-  2.0 fat    18007 b- defN 23-May-06 19:50 synapgrad/nn/layers.py
 -rw-rw-rw-  2.0 fat     6809 b- defN 23-Apr-20 01:41 synapgrad/nn/losses.py
--rw-rw-rw-  2.0 fat     2654 b- defN 23-Apr-19 20:19 synapgrad/nn/modules.py
+-rw-rw-rw-  2.0 fat     2654 b- defN 23-May-05 16:13 synapgrad/nn/modules.py
 -rw-rw-rw-  2.0 fat      989 b- defN 23-May-01 11:50 synapgrad/nn/neurons.py
 -rw-rw-rw-  2.0 fat       46 b- defN 23-Apr-08 14:30 synapgrad/optim/__init__.py
--rw-rw-rw-  2.0 fat     5293 b- defN 23-Apr-20 01:43 synapgrad/optim/optimizers.py
+-rw-rw-rw-  2.0 fat     5398 b- defN 23-May-05 17:24 synapgrad/optim/optimizers.py
 -rw-rw-rw-  2.0 fat      154 b- defN 23-Apr-11 17:18 synapgrad/utils/__init__.py
 -rw-rw-rw-  2.0 fat     3403 b- defN 23-Apr-11 18:19 synapgrad/utils/data.py
 -rw-rw-rw-  2.0 fat     1345 b- defN 23-Apr-21 08:50 synapgrad/utils/graph.py
 -rw-rw-rw-  2.0 fat    10586 b- defN 23-Apr-12 12:20 synapgrad/utils/train.py
--rw-rw-rw-  2.0 fat     1088 b- defN 23-May-03 19:09 synapgrad-0.3.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4756 b- defN 23-May-03 19:09 synapgrad-0.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-03 19:09 synapgrad-0.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-May-03 19:09 synapgrad-0.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1696 b- defN 23-May-03 19:09 synapgrad-0.3.1.dist-info/RECORD
-21 files, 104099 bytes uncompressed, 27032 bytes compressed:  74.0%
+-rw-rw-rw-  2.0 fat     1088 b- defN 23-May-07 01:43 synapgrad-0.3.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4960 b- defN 23-May-07 01:43 synapgrad-0.3.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-07 01:43 synapgrad-0.3.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-07 01:43 synapgrad-0.3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1696 b- defN 23-May-07 01:43 synapgrad-0.3.2.dist-info/RECORD
+21 files, 104178 bytes uncompressed, 27069 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: synapgrad/utils/graph.py
 Comment: 
 
 Filename: synapgrad/utils/train.py
 Comment: 
 
-Filename: synapgrad-0.3.1.dist-info/LICENSE
+Filename: synapgrad-0.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: synapgrad-0.3.1.dist-info/METADATA
+Filename: synapgrad-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: synapgrad-0.3.1.dist-info/WHEEL
+Filename: synapgrad-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: synapgrad-0.3.1.dist-info/top_level.txt
+Filename: synapgrad-0.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: synapgrad-0.3.1.dist-info/RECORD
+Filename: synapgrad-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## synapgrad/nn/layers.py

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from .. import nn, Tensor
+from .. import nn, Tensor, engine
 from .neurons import init_weights
 from .functional import unfold, fold
 from .initializations import init_weights
 
 
 class Linear(nn.Module):
     
@@ -279,14 +279,15 @@
                  track_running_stats:bool=True, dtype=None) -> None:
         super().__init__()
         self.num_features = num_features
         self.eps = eps
         self.momentum = momentum
         self.affine = affine
         self.track_running_stats = track_running_stats
+        self.num_batches_tracked = 0
         
         valid_modes = ['1d', '2d']
         
         if mode not in valid_modes:
             raise ValueError(f"'{mode}' is not a valid mode, expected one of {valid_modes}")
         self.mode = mode
         
@@ -324,55 +325,46 @@
                 N, C = x.shape
                 n = N # num_samples
                 dims = (0,)
                 view_shape = (1,C)
             else: raise RuntimeError(f"Expected 2D or 3D tensor, but got {len(x.shape)}D")
         assert C == self.num_features, f"Expected {self.num_features} channels, got {C}."
         
-        if self.training or not self.track_running_stats:
-            # Compute the mean of each channel
-            mu = x.mean(dim=dims)
-            # Compute the variance of each channel
-            var_sum = ((x-mu.reshape(view_shape))**2).sum(dim=dims)
+        exponential_average_factor = 0.0
+
+        if self.training and self.track_running_stats:
+            if self.num_batches_tracked is not None:
+                self.num_batches_tracked += 1
+                if self.momentum is None:  # use cumulative moving average
+                    exponential_average_factor = 1.0 / float(self.num_batches_tracked)
+                else:  # use exponential moving average
+                    exponential_average_factor = self.momentum
+
+        # calculate running estimates
+        if self.training:
+            mean = x.mean(dim=dims)
+            # use biased var in train
+            var_sum = ((x - mean.reshape(view_shape))**2).sum(dim=dims)
             var = var_sum / n
             
-            x_norm = self.__normalize(x, mu, var)
-
-            # Update the running average of mean and variance
-            if self.training and self.track_running_stats:
-                r_mu = (self.momentum * mu.data + (1 - self.momentum) * self.running_mean.data)
-                self.running_mean = Tensor(r_mu)
-                
-                unbiased_var = var_sum.data / (n - 1)
-                r_var = (self.momentum * unbiased_var + (1 - self.momentum) * self.running_var.data)
-                self.running_var = Tensor(r_var)
+            r_mu = (exponential_average_factor * mean.data + (1 - exponential_average_factor) * self.running_mean.data)
+            self.running_mean = Tensor(r_mu, dtype=x.dtype)
+            
+            unbiased_var = var_sum.data / (n - 1)
+            r_var = (exponential_average_factor * unbiased_var + (1 - exponential_average_factor) * self.running_var.data)
+            self.running_var = Tensor(r_var, dtype=x.dtype)
         else:
-            x_norm = self.__normalize(x, self.running_mean, self.running_var)
+            mean = self.running_mean
+            var = self.running_var
 
-        # Scale and shift the normalization
+        out = (x - mean.reshape(view_shape)) / (var.reshape(view_shape) + self.eps).sqrt()
         if self.affine:
-            out = (x_norm * self.weight.reshape(view_shape)) + self.bias.reshape(view_shape)
-        else:
-            out = x_norm
-        
-        return out
-    
-    def __normalize(self, x:Tensor, mean:Tensor, var:Tensor, channel_dim=1) -> Tensor:
-        """Normalize a Tensor with mean and variance over the channel dimension
+            out = out * self.weight.reshape(view_shape) + self.bias.reshape(view_shape)
 
-            Args:
-                x (Tensor): Input
-                mean (Tensor): Computed batch mean
-                var (Tensor): Computed batch var
-            
-            Returns:
-                Tensor: Normalized tensor
-        """
-        shape = [1,]*len(x.shape); shape[channel_dim] = x.shape[channel_dim]
-        return (x - mean.reshape(shape)) / ((var + self.eps).reshape(shape).sqrt())
+        return out
         
     def parameters(self) -> list[Tensor]:
         return [self.weight, self.bias] if self.affine else []
 
 
 class BatchNorm1d(BatchNorm):
     """
```

## synapgrad/optim/optimizers.py

```diff
@@ -5,14 +5,16 @@
 import numpy as np
 
 
 class Optimizer(ABC):
     
     def __init__(self, parameters:list[Tensor], lr=0.001) -> None:
         super().__init__()
+        if len(parameters) == 0:
+            raise ValueError("optimizer got an empty parameter list")
         self.parameters = parameters
         self.lr = lr
         self.t = 0
         
     def zero_grad(self):
         for p in self.parameters:
             p.zero_()
```

## Comparing `synapgrad-0.3.1.dist-info/LICENSE` & `synapgrad-0.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `synapgrad-0.3.1.dist-info/METADATA` & `synapgrad-0.3.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapgrad
-Version: 0.3.1
+Version: 0.3.2
 Summary: An autograd Tensor-based engine with a deep learning library built on top of it made from scratch
 Home-page: https://github.com/pgmesa/synapgrad
 Author: Pablo García Mesa
 Author-email: pgmesa.sm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -15,18 +15,25 @@
 License-File: LICENSE
 Requires-Dist: numpy (>=1.21.0)
 
 #  SynapGrad
 
 An autograd Tensor-based engine with a deep learning library built on top of it made from scratch
 
+[![Downloads](https://static.pepy.tech/personalized-badge/synapgrad?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads)](https://pepy.tech/project/synapgrad)
+
+## Installation
+```bash
+pip install synapgrad
+```
+
 ## Technical Description
 This project implements a completely functional engine for tracking operations between Tensors, by dynamically building a Directed Acyclic Graph (DAG), and an automatic backpropagation algorithm (reverse-mode autodiff) over this DAG.
 
-Built on top of the engine, the deep learning library implements the most common functions, layers, losses and optimizers in order to create MLPs and CNNs able to solve AI problems
+Built on top of the engine, the deep learning library implements the most common functions, layers, losses and optimizers in order to create AI models able to solve real problems.
 
 This library tries to mimic Pytorch in a simplified way, but with similar functions and behaviour. 
 
 ## Aim of the project
 The aim of this project is to create a deep learning library from scratch, without using any existing framework (such as keras, pytorch, tensorflow, sklearn, etc) in order to fully understand the core aspects of how they work. Specifically, this time I have focused on pytorch.
 
 However, some of these external frameworks have been used for the following reasons:
@@ -35,19 +42,14 @@
 - (keras) to download handwritten digits MNIST dataset
 - (sklearn) to create 'make_moons' dataset
 
 This project stems from the amazing educational project `micrograd` by `karpathy` (https://github.com/karpathy/micrograd)
 
 Note: Supporting GPU execution is out of the scope of this project
 
-## Installation
-```bash
-pip install synapgrad
-```
-
 ## Autograd Example
 Below is a random example of some of the operations that can be tracked with synapgrad.Tensor
 ```python
 from synapgrad import Tensor
 
 l1 = [[-4.0, 0, 5.0], [6.3, 3.2, 1.3]]
 l2 = [[2.0, 2,  3.0], [2.4, 1.7, 0.5]]
@@ -74,15 +76,15 @@
 
 - [x] 1. Basic MLP for binary classification (sklearn 'make_moons' toy dataset)
 - [x] 2. MLP for handwritten digits classification (MNIST dataset) 
 - [x] 3. CNN for handwritten digits classification (MNIST dataset)
 
 Example 1 (synapgrad MLP solution)     |  Example 2 and 3
 :-------------------------:|:-------------------------:
-![Image 1](/assets/example_moons.png) | ![Image 2](/assets/example_mnist.png) 
+![Image 1](/.github/example_moons.png) | ![Image 2](/.github/example_mnist.png) 
 
 ## Comparisons with other frameworks
 In order to see the efficiency of synapgrad, it is compared with other existing engines (in this case torch and micrograd). All trainings have been runned on a laptop with an Intel Core i7 10th generation processor.
 
 | Training Example | synapgrad | torch | micrograd |
 |     :---:        |  :---:  |  :---:  |   :---:   |  
 | 1 | 1.7 s | 1.5 s | 1 min 43 s |
@@ -107,15 +109,15 @@
     y2 = (x2 / x)
     z = y * y2 * x2
     z = z.sum()
     z.backward()
 utils.graph.draw(z)
 ```
 
-![Graph Image](/assets/graph_example.svg)
+![Graph Image](/.github/graph_example.svg)
 
 ## Running tests
 To run the unit tests you will have to install PyTorch. In these tests, gradients calculation as well as losses, layers, etc, are assessed with pytorch to check everything is working fine. To run the tests:
 ```bash
 python -m pytest
 ```
```

## Comparing `synapgrad-0.3.1.dist-info/RECORD` & `synapgrad-0.3.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 synapgrad/__init__.py,sha256=rzU1koPmJ4_LyMdxWzho4Qd-qWUqh16aKSgmF5HBOEw,72
 synapgrad/engine.py,sha256=nMvbz8hdQ49SzrJe5qX98p-YYa2SnE1jj5Jj3Nr7ELg,32179
 synapgrad/nn/__init__.py,sha256=kJVBFgfaX-9Rsg0QDV3lKjPaRNuWVn2RgCkb-mAvXhM,442
 synapgrad/nn/activations.py,sha256=TEUzX6IvnYlnWkmCyLQMxTDENH-cukG8R0R26ikV5QA,3538
 synapgrad/nn/functional.py,sha256=jICas3UKdjRsxh4xZBTl4nNMfswrrEmqRoOKzu4Qgjw,7831
 synapgrad/nn/initializations.py,sha256=WjgU7KfSQh_aMXBXrj5KOyaz6C3y-tPbmsodFiu6uRc,2879
-synapgrad/nn/layers.py,sha256=MI9erbQ1UQB2D-SlXd3ceiMoIaD7bLFPm8woahUq5SU,18237
+synapgrad/nn/layers.py,sha256=9YXz2OJdsUtOUgXKBu6iddpyhTUNl0Wm83qLQA5aB4E,18007
 synapgrad/nn/losses.py,sha256=N7uLz_ILdv_LQ_MGLH3xCfyC9FPyEWz7zVO51Di0XJY,6809
 synapgrad/nn/modules.py,sha256=y_F6iUE5t0rlXGwvOtsSVttqgJ3OPMkdx5MbDxceVYc,2654
 synapgrad/nn/neurons.py,sha256=oQNtsfpAE-CYymK45Wz-ORsuiOzk6CAg5ZcCLYnjl6A,989
 synapgrad/optim/__init__.py,sha256=8X56jD7Dcyw-Hdux1K7_YK9_oc3BuNPk9YwC7gSNWaE,46
-synapgrad/optim/optimizers.py,sha256=Y5ryseve_Virrpsl2ynSt2npq2O0-kyIj_Tj0jfKko0,5293
+synapgrad/optim/optimizers.py,sha256=xewScCOI04dzXC0WGabmm-A8OOJ83xC4KfsJi509PZo,5398
 synapgrad/utils/__init__.py,sha256=eCwZrBr9yWO92hufOIWwAFhwrA_JuMCsmHeDL7PSAtE,154
 synapgrad/utils/data.py,sha256=cwSsVZwEbB6BU9tWrf5aIeZo9u5KNgar7rVYa6WV328,3403
 synapgrad/utils/graph.py,sha256=FOkPCSYcmOaoPRhdoXweUQRvoxH0n3x4nASGLr7HQjw,1345
 synapgrad/utils/train.py,sha256=V3j4iqSW9sjSfIz9bski95Ni25KuYzIAkjqD4o3-Tjg,10586
-synapgrad-0.3.1.dist-info/LICENSE,sha256=tILw81bLBHb_8uhiXZAlAo5QrlyMSCJH33lb7GYpz6E,1088
-synapgrad-0.3.1.dist-info/METADATA,sha256=3bXzYfFAagKRkV_Hk_dEAwjDqg0k3Z7A5uan4NvI5M0,4756
-synapgrad-0.3.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-synapgrad-0.3.1.dist-info/top_level.txt,sha256=D7_rcC0S5ytl1AFRAo5c73mZggZB-Z_zm_GNIGe0QgM,10
-synapgrad-0.3.1.dist-info/RECORD,,
+synapgrad-0.3.2.dist-info/LICENSE,sha256=tILw81bLBHb_8uhiXZAlAo5QrlyMSCJH33lb7GYpz6E,1088
+synapgrad-0.3.2.dist-info/METADATA,sha256=Owf5vmRgs4AufREgbqIL-VBkoJ2NGfYYWbx9TMx2WZ8,4960
+synapgrad-0.3.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+synapgrad-0.3.2.dist-info/top_level.txt,sha256=D7_rcC0S5ytl1AFRAo5c73mZggZB-Z_zm_GNIGe0QgM,10
+synapgrad-0.3.2.dist-info/RECORD,,
```

