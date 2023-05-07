# Comparing `tmp/KDEpy-1.1.1-cp39-cp39-win_amd64.whl.zip` & `tmp/KDEpy-1.1.2-cp39-cp39-macosx_10_9_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,19 @@
-Zip file size: 95489 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat   151552 b- defN 23-Mar-18 07:45 cutils.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     8950 b- defN 23-Mar-18 07:40 KDEpy/BaseKDE.py
--rw-rw-rw-  2.0 fat     8471 b- defN 23-Mar-18 07:40 KDEpy/FFTKDE.py
--rw-rw-rw-  2.0 fat     5179 b- defN 23-Mar-18 07:40 KDEpy/NaiveKDE.py
--rw-rw-rw-  2.0 fat     7067 b- defN 23-Mar-18 07:40 KDEpy/TreeKDE.py
--rw-rw-rw-  2.0 fat      254 b- defN 23-Mar-18 07:40 KDEpy/__init__.py
--rw-rw-rw-  2.0 fat    16573 b- defN 23-Mar-18 07:40 KDEpy/binning.py
--rw-rw-rw-  2.0 fat    10346 b- defN 23-Mar-18 07:40 KDEpy/bw_selection.py
--rw-rw-rw-  2.0 fat    10177 b- defN 23-Mar-18 07:40 KDEpy/kernel_funcs.py
--rw-rw-rw-  2.0 fat     3948 b- defN 23-Mar-18 07:40 KDEpy/utils.py
--rw-rw-rw-  2.0 fat     1527 b- defN 23-Mar-18 07:45 KDEpy-1.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     5441 b- defN 23-Mar-18 07:45 KDEpy-1.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Mar-18 07:45 KDEpy-1.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Mar-18 07:45 KDEpy-1.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1129 b- defN 23-Mar-18 07:45 KDEpy-1.1.1.dist-info/RECORD
-15 files, 230727 bytes uncompressed, 93673 bytes compressed:  59.4%
+Zip file size: 222257 bytes, number of entries: 17
+-rwxr-xr-x  2.0 unx   207272 b- defN 23-May-07 13:20 cutils.cpython-39-darwin.so
+-rw-r--r--  2.0 unx    16130 b- defN 23-May-07 13:14 KDEpy/binning.py
+-rw-r--r--  2.0 unx     9817 b- defN 23-May-07 13:14 KDEpy/kernel_funcs.py
+-rw-r--r--  2.0 unx      298 b- defN 23-May-07 13:14 KDEpy/__init__.py
+-rw-r--r--  2.0 unx   894529 b- defN 23-May-07 13:15 KDEpy/cutils.c
+-rw-r--r--  2.0 unx     8259 b- defN 23-May-07 13:14 KDEpy/FFTKDE.py
+-rw-r--r--  2.0 unx     6884 b- defN 23-May-07 13:14 KDEpy/TreeKDE.py
+-rw-r--r--  2.0 unx     5036 b- defN 23-May-07 13:14 KDEpy/NaiveKDE.py
+-rw-r--r--  2.0 unx     8718 b- defN 23-May-07 13:14 KDEpy/BaseKDE.py
+-rw-r--r--  2.0 unx    10045 b- defN 23-May-07 13:14 KDEpy/bw_selection.py
+-rw-r--r--  2.0 unx     3809 b- defN 23-May-07 13:14 KDEpy/utils.py
+-rw-r--r--  2.0 unx    14713 b- defN 23-May-07 13:14 KDEpy/cutils.pyx
+-rw-rw-r--  2.0 unx     1294 b- defN 23-May-07 13:21 KDEpy-1.1.2.dist-info/RECORD
+-rw-r--r--  2.0 unx     1499 b- defN 23-May-07 13:20 KDEpy-1.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      109 b- defN 23-May-07 13:20 KDEpy-1.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-May-07 13:20 KDEpy-1.1.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     5243 b- defN 23-May-07 13:20 KDEpy-1.1.2.dist-info/METADATA
+17 files, 1193668 bytes uncompressed, 220225 bytes compressed:  81.6%
```

## zipnote {}

```diff
@@ -1,46 +1,52 @@
-Filename: cutils.cp39-win_amd64.pyd
+Filename: cutils.cpython-39-darwin.so
 Comment: 
 
-Filename: KDEpy/BaseKDE.py
+Filename: KDEpy/binning.py
 Comment: 
 
-Filename: KDEpy/FFTKDE.py
+Filename: KDEpy/kernel_funcs.py
 Comment: 
 
-Filename: KDEpy/NaiveKDE.py
+Filename: KDEpy/__init__.py
+Comment: 
+
+Filename: KDEpy/cutils.c
+Comment: 
+
+Filename: KDEpy/FFTKDE.py
 Comment: 
 
 Filename: KDEpy/TreeKDE.py
 Comment: 
 
-Filename: KDEpy/__init__.py
+Filename: KDEpy/NaiveKDE.py
 Comment: 
 
-Filename: KDEpy/binning.py
+Filename: KDEpy/BaseKDE.py
 Comment: 
 
 Filename: KDEpy/bw_selection.py
 Comment: 
 
-Filename: KDEpy/kernel_funcs.py
+Filename: KDEpy/utils.py
 Comment: 
 
-Filename: KDEpy/utils.py
+Filename: KDEpy/cutils.pyx
 Comment: 
 
-Filename: KDEpy-1.1.1.dist-info/LICENSE
+Filename: KDEpy-1.1.2.dist-info/RECORD
 Comment: 
 
-Filename: KDEpy-1.1.1.dist-info/METADATA
+Filename: KDEpy-1.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: KDEpy-1.1.1.dist-info/WHEEL
+Filename: KDEpy-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: KDEpy-1.1.1.dist-info/top_level.txt
+Filename: KDEpy-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: KDEpy-1.1.1.dist-info/RECORD
+Filename: KDEpy-1.1.2.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## KDEpy/BaseKDE.py

 * *Ordering differences only*

```diff
@@ -1,232 +1,232 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Module for the BaseKDE class.
-"""
-import numbers
-from abc import ABC, abstractmethod
-from collections.abc import Sequence
-
-import numpy as np
-
-from KDEpy.bw_selection import _bw_methods
-from KDEpy.kernel_funcs import _kernel_functions
-from KDEpy.utils import autogrid
-
-
-class BaseKDE(ABC):
-    """
-    Abstract Base Class for every Kernel Density Estimator.
-
-    This class is never instantiated, it merely defines some common methods
-    which every subclass must implement. In summary, it facilitates:
-
-        - The `_available_kernels` and `_bw_methods` parameter
-        - Correct handling of `kernel` and `bw` in __init__
-        - Forces subclasses to implement `fit(data)`, converts `data` to
-          correct shape (obs, dims) and converts `weights` to correct shape
-          (obs,)
-        - Forces subclasses to implement `evaluate(grid_points)`, with handling
-    """
-
-    _available_kernels = _kernel_functions
-    _bw_methods = _bw_methods
-
-    @abstractmethod
-    def __init__(self, kernel: str, bw: float):
-        """Initialize the kernel density estimator.
-
-        The return type must be duplicated in the docstring to comply
-        with the NumPy docstring style.
-
-        Parameters
-        ----------
-        kernel
-            Kernel function, or string matching available options.
-        bw
-            The bandwidth, either a number, a string or an array-like.
-        """
-
-        # Verify that the choice of kernel is valid, and set the function
-        akernels = sorted(list(self._available_kernels.keys()))
-        msg = "Kernel must be a string or callable. Opts: {}".format(akernels)
-        if isinstance(kernel, str):
-            kernel = kernel.strip().lower()
-            if kernel not in akernels:
-                raise ValueError(msg)
-            else:
-                self.kernel = self._available_kernels[kernel]
-        elif callable(kernel):
-            self.kernel = kernel
-        else:
-            raise ValueError(msg)
-
-        # The `bw` paramter may either be a positive number, a string, or
-        # array-like such that each point in the data has a uniue bw
-        if isinstance(bw, numbers.Number) and bw > 0:
-            self.bw_method = bw
-        elif isinstance(bw, str):
-            amethods = sorted(list(self._bw_methods.keys()))
-            if bw.lower() not in set(m.lower() for m in amethods):
-                msg = "bw not recognized. Options are: {}".format(amethods)
-                raise ValueError(msg)
-            self.bw_method = self._bw_methods[bw]
-        elif isinstance(bw, (np.ndarray, Sequence)):
-            self.bw_method = bw
-        else:
-            raise ValueError("Bandwidth must be > 0, array-like or a string.")
-
-        # Test quickly that the method has done what is was supposed to do
-        assert callable(self.kernel)
-        assert isinstance(self.bw_method, (np.ndarray, Sequence, numbers.Number)) or callable(self.bw_method)
-
-    @abstractmethod
-    def fit(self, data, weights=None):
-        """
-        Fit the kernel density estimator to the data.
-        This method converts the data to shape (obs, dims) and the weights
-        to (obs,).
-
-        Parameters
-        ----------
-        data : array-like or Sequence
-            May be array-like of shape (obs,), shape (obs, dims) or a
-            Python Sequence, e.g. a list or tuple.
-        weights : array-like, Sequence or None
-            May be array-like of shape (obs,), shape (obs, dims), a
-            Python Sequence, e.g. a list or tuple, or None.
-        """
-
-        # -------------- Set up the data depending on input -------------------
-        # In the end, the data should be an ndarray of shape (obs, dims)
-        data = self._process_sequence(data)
-
-        obs, dims = data.shape
-
-        if not obs > 0:
-            raise ValueError("Data must contain at least one data point.")
-        assert dims > 0
-        self.data = data
-
-        # -------------- Set up the weights depending on input ----------------
-        if weights is not None:
-            self.weights = self._process_sequence(weights).ravel()
-            self.weights = self.weights / np.sum(self.weights)
-            if not obs == len(self.weights):
-                raise ValueError("Number of data obs must match weights")
-        else:
-            self.weights = weights
-
-        # TODO: Move bandwidth selection from evaluate to fit
-
-        # Test quickly that the method has done what is was supposed to do
-        assert len(self.data.shape) == 2
-        if self.weights is not None:
-            assert len(self.weights.shape) == 1
-            assert self.data.shape[0] == len(self.weights)
-
-        if isinstance(self.bw_method, (np.ndarray, Sequence)):
-            self.bw = self.bw_method
-        elif callable(self.bw_method):
-            self.bw = self.bw_method(self.data, self.weights)
-        else:
-            self.bw = self.bw_method
-
-    @abstractmethod
-    def evaluate(self, grid_points=None, bw_to_scalar=True):
-        """
-        Evaluate the kernel density estimator on the grid points.
-
-        Parameters
-        ----------
-        grid_points : integer, tuple or array-like
-            If an integer, the number of equidistant grid point in every
-            dimension. If a tuple, the number of grid points in each
-            dimension. If array-like, grid points of shape (obs, dims).
-        """
-        if not hasattr(self, "data"):
-            raise ValueError("Must call fit before evaluating.")
-
-        # -------------- Set up the bandwidth depending on inputs -------------
-        if bw_to_scalar:
-            bw = np.max(self.bw)
-        else:
-            bw = self.bw
-
-        # -------------- Set up the grid depending on input -------------------
-        # If the grid None or an integer, use that in the autogrid method
-        types_for_autogrid = (numbers.Integral, tuple)
-        if grid_points is None or isinstance(grid_points, types_for_autogrid):
-            self._user_supplied_grid = False
-            bw_grid = self.kernel.practical_support(bw)
-            grid_points = autogrid(self.data, bw_grid, grid_points)
-            # Set it here, so as not to call kernel.practical_support(bw) again
-            self._kernel_practical_support = bw_grid
-        else:
-            self._user_supplied_grid = True
-            grid_points = self._process_sequence(grid_points)
-
-        obs, dims = grid_points.shape
-        if not obs > 0:
-            raise ValueError("Grid must contain at least one data point.")
-        self.grid_points = grid_points
-
-        # Test quickly that the method has done what is was supposed to do
-        if bw_to_scalar:
-            assert isinstance(bw, numbers.Number)
-            assert bw > 0
-        assert len(self.grid_points.shape) == 2
-
-    @staticmethod
-    def _process_sequence(sequence_array_like):
-        """
-        Process a sequence of data input to ndarray of shape (obs, dims).
-
-        Parameters
-        ----------
-        sequence_array_like : Sequence or array-like
-            The input data.
-
-        Examples
-        --------
-        >>> res = BaseKDE._process_sequence([1, 2, 3])
-        >>> (res == np.array([[1], [2], [3]])).all()
-        True
-        """
-        # Must convert to float to avoid possible interger overflow
-        if isinstance(sequence_array_like, Sequence):
-            out = np.asfarray(sequence_array_like).reshape(-1, 1)
-        elif isinstance(sequence_array_like, np.ndarray):
-            if len(sequence_array_like.shape) == 1:
-                out = sequence_array_like.reshape(-1, 1)
-            elif len(sequence_array_like.shape) == 2:
-                out = sequence_array_like
-            else:
-                raise ValueError("Must be of shape (obs, dims)")
-        else:
-            raise TypeError("Must be of shape (obs, dims)")
-        return np.asarray_chkfinite(out, dtype=float)
-
-    def _evalate_return_logic(self, evaluated, grid_points):
-        """
-        Return either evaluation points y, or tuple (x, y) based on inputs.
-        """
-        # Adding epsilon to output helps contour plotting functions
-        evaluated = evaluated.ravel() + np.finfo(float).eps
-        obs, dims = grid_points.shape
-        if self._user_supplied_grid:
-            return evaluated
-        else:
-            if dims == 1:
-                return grid_points.ravel(), evaluated
-            return grid_points, evaluated
-
-    def __call__(self, *args, **kwargs):
-        return self.evaluate(*args, **kwargs)
-
-
-if __name__ == "__main__":
-    import pytest
-
-    # --durations=10  <- May be used to show potentially slow tests
-    pytest.main(args=[".", "--doctest-modules", "-v", "-x"])
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Module for the BaseKDE class.
+"""
+import numbers
+from abc import ABC, abstractmethod
+from collections.abc import Sequence
+
+import numpy as np
+
+from KDEpy.bw_selection import _bw_methods
+from KDEpy.kernel_funcs import _kernel_functions
+from KDEpy.utils import autogrid
+
+
+class BaseKDE(ABC):
+    """
+    Abstract Base Class for every Kernel Density Estimator.
+
+    This class is never instantiated, it merely defines some common methods
+    which every subclass must implement. In summary, it facilitates:
+
+        - The `_available_kernels` and `_bw_methods` parameter
+        - Correct handling of `kernel` and `bw` in __init__
+        - Forces subclasses to implement `fit(data)`, converts `data` to
+          correct shape (obs, dims) and converts `weights` to correct shape
+          (obs,)
+        - Forces subclasses to implement `evaluate(grid_points)`, with handling
+    """
+
+    _available_kernels = _kernel_functions
+    _bw_methods = _bw_methods
+
+    @abstractmethod
+    def __init__(self, kernel: str, bw: float):
+        """Initialize the kernel density estimator.
+
+        The return type must be duplicated in the docstring to comply
+        with the NumPy docstring style.
+
+        Parameters
+        ----------
+        kernel
+            Kernel function, or string matching available options.
+        bw
+            The bandwidth, either a number, a string or an array-like.
+        """
+
+        # Verify that the choice of kernel is valid, and set the function
+        akernels = sorted(list(self._available_kernels.keys()))
+        msg = "Kernel must be a string or callable. Opts: {}".format(akernels)
+        if isinstance(kernel, str):
+            kernel = kernel.strip().lower()
+            if kernel not in akernels:
+                raise ValueError(msg)
+            else:
+                self.kernel = self._available_kernels[kernel]
+        elif callable(kernel):
+            self.kernel = kernel
+        else:
+            raise ValueError(msg)
+
+        # The `bw` paramter may either be a positive number, a string, or
+        # array-like such that each point in the data has a uniue bw
+        if isinstance(bw, numbers.Number) and bw > 0:
+            self.bw_method = bw
+        elif isinstance(bw, str):
+            amethods = sorted(list(self._bw_methods.keys()))
+            if bw.lower() not in set(m.lower() for m in amethods):
+                msg = "bw not recognized. Options are: {}".format(amethods)
+                raise ValueError(msg)
+            self.bw_method = self._bw_methods[bw]
+        elif isinstance(bw, (np.ndarray, Sequence)):
+            self.bw_method = bw
+        else:
+            raise ValueError("Bandwidth must be > 0, array-like or a string.")
+
+        # Test quickly that the method has done what is was supposed to do
+        assert callable(self.kernel)
+        assert isinstance(self.bw_method, (np.ndarray, Sequence, numbers.Number)) or callable(self.bw_method)
+
+    @abstractmethod
+    def fit(self, data, weights=None):
+        """
+        Fit the kernel density estimator to the data.
+        This method converts the data to shape (obs, dims) and the weights
+        to (obs,).
+
+        Parameters
+        ----------
+        data : array-like or Sequence
+            May be array-like of shape (obs,), shape (obs, dims) or a
+            Python Sequence, e.g. a list or tuple.
+        weights : array-like, Sequence or None
+            May be array-like of shape (obs,), shape (obs, dims), a
+            Python Sequence, e.g. a list or tuple, or None.
+        """
+
+        # -------------- Set up the data depending on input -------------------
+        # In the end, the data should be an ndarray of shape (obs, dims)
+        data = self._process_sequence(data)
+
+        obs, dims = data.shape
+
+        if not obs > 0:
+            raise ValueError("Data must contain at least one data point.")
+        assert dims > 0
+        self.data = data
+
+        # -------------- Set up the weights depending on input ----------------
+        if weights is not None:
+            self.weights = self._process_sequence(weights).ravel()
+            self.weights = self.weights / np.sum(self.weights)
+            if not obs == len(self.weights):
+                raise ValueError("Number of data obs must match weights")
+        else:
+            self.weights = weights
+
+        # TODO: Move bandwidth selection from evaluate to fit
+
+        # Test quickly that the method has done what is was supposed to do
+        assert len(self.data.shape) == 2
+        if self.weights is not None:
+            assert len(self.weights.shape) == 1
+            assert self.data.shape[0] == len(self.weights)
+
+        if isinstance(self.bw_method, (np.ndarray, Sequence)):
+            self.bw = self.bw_method
+        elif callable(self.bw_method):
+            self.bw = self.bw_method(self.data, self.weights)
+        else:
+            self.bw = self.bw_method
+
+    @abstractmethod
+    def evaluate(self, grid_points=None, bw_to_scalar=True):
+        """
+        Evaluate the kernel density estimator on the grid points.
+
+        Parameters
+        ----------
+        grid_points : integer, tuple or array-like
+            If an integer, the number of equidistant grid point in every
+            dimension. If a tuple, the number of grid points in each
+            dimension. If array-like, grid points of shape (obs, dims).
+        """
+        if not hasattr(self, "data"):
+            raise ValueError("Must call fit before evaluating.")
+
+        # -------------- Set up the bandwidth depending on inputs -------------
+        if bw_to_scalar:
+            bw = np.max(self.bw)
+        else:
+            bw = self.bw
+
+        # -------------- Set up the grid depending on input -------------------
+        # If the grid None or an integer, use that in the autogrid method
+        types_for_autogrid = (numbers.Integral, tuple)
+        if grid_points is None or isinstance(grid_points, types_for_autogrid):
+            self._user_supplied_grid = False
+            bw_grid = self.kernel.practical_support(bw)
+            grid_points = autogrid(self.data, bw_grid, grid_points)
+            # Set it here, so as not to call kernel.practical_support(bw) again
+            self._kernel_practical_support = bw_grid
+        else:
+            self._user_supplied_grid = True
+            grid_points = self._process_sequence(grid_points)
+
+        obs, dims = grid_points.shape
+        if not obs > 0:
+            raise ValueError("Grid must contain at least one data point.")
+        self.grid_points = grid_points
+
+        # Test quickly that the method has done what is was supposed to do
+        if bw_to_scalar:
+            assert isinstance(bw, numbers.Number)
+            assert bw > 0
+        assert len(self.grid_points.shape) == 2
+
+    @staticmethod
+    def _process_sequence(sequence_array_like):
+        """
+        Process a sequence of data input to ndarray of shape (obs, dims).
+
+        Parameters
+        ----------
+        sequence_array_like : Sequence or array-like
+            The input data.
+
+        Examples
+        --------
+        >>> res = BaseKDE._process_sequence([1, 2, 3])
+        >>> (res == np.array([[1], [2], [3]])).all()
+        True
+        """
+        # Must convert to float to avoid possible interger overflow
+        if isinstance(sequence_array_like, Sequence):
+            out = np.asfarray(sequence_array_like).reshape(-1, 1)
+        elif isinstance(sequence_array_like, np.ndarray):
+            if len(sequence_array_like.shape) == 1:
+                out = sequence_array_like.reshape(-1, 1)
+            elif len(sequence_array_like.shape) == 2:
+                out = sequence_array_like
+            else:
+                raise ValueError("Must be of shape (obs, dims)")
+        else:
+            raise TypeError("Must be of shape (obs, dims)")
+        return np.asarray_chkfinite(out, dtype=float)
+
+    def _evalate_return_logic(self, evaluated, grid_points):
+        """
+        Return either evaluation points y, or tuple (x, y) based on inputs.
+        """
+        # Adding epsilon to output helps contour plotting functions
+        evaluated = evaluated.ravel() + np.finfo(float).eps
+        obs, dims = grid_points.shape
+        if self._user_supplied_grid:
+            return evaluated
+        else:
+            if dims == 1:
+                return grid_points.ravel(), evaluated
+            return grid_points, evaluated
+
+    def __call__(self, *args, **kwargs):
+        return self.evaluate(*args, **kwargs)
+
+
+if __name__ == "__main__":
+    import pytest
+
+    # --durations=10  <- May be used to show potentially slow tests
+    pytest.main(args=[".", "--doctest-modules", "-v", "-x"])
```

## KDEpy/FFTKDE.py

 * *Ordering differences only*

```diff
@@ -1,212 +1,212 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Module for the FFTKDE.
-"""
-import numbers
-import warnings
-
-import numpy as np
-from scipy.signal import convolve
-
-from KDEpy.BaseKDE import BaseKDE
-from KDEpy.binning import grid_is_sorted, linear_binning
-from KDEpy.utils import cartesian
-
-
-class FFTKDE(BaseKDE):
-    r"""
-    This class implements a convolution (FFT) based computation of a KDE.
-    While this implementation is very fast, there are some limitations: (1) the
-    bandwidth must be constant, (2) the KDE must be evaluated on an
-    equidistant grid and (3) the grid must encompass every data point.
-    The finer the grid, the smaller the error.
-
-    The evaluation step is split into two phases. First the :math:`N` data
-    points are binned using a linear binning routine on an equidistant grid `x`
-    with :math:`n` grid points. This runs in :math:`O(N 2^d)` time.
-    Then the kernel is evaluated once on :math:`\leq n` points and the result
-    of the kernel evaluation and the binned data is convolved. Using the
-    convolution theorem, this step runs in :math:`O(n \log n)` time.
-    While :math:`N` may be millions, :math:`n` is typically 2**10. The total
-    running time of the algorithm is :math:`O(N 2^d + n \log n)`.
-    See references for more information.
-
-    The implementation is reminiscent of the one found in statsmodels. However,
-    unlike the statsmodels implementation every kernel is available for FFT
-    computation, weighted data is available for FFT computation, and no large
-    temporary arrays are created.
-
-    Parameters
-    ----------
-    kernel : str
-        The kernel function. See cls._available_kernels.keys() for choices.
-    bw : float or str
-        Bandwidth or bandwidth selection method. If a float is passed, it
-        is the standard deviation of the kernel. If a string it passed, it
-        is the bandwidth selection method, see cls._bw_methods.keys() for
-        choices.
-
-    Examples
-    --------
-    >>> data = np.random.randn(2**10)
-    >>> # (1) Automatic bw selection using Improved Sheather Jones (ISJ)
-    >>> x, y = FFTKDE(bw='ISJ').fit(data).evaluate()
-    >>> # (2) Explicit choice of kernel and bw (standard deviation of kernel)
-    >>> x, y = FFTKDE(kernel='triweight', bw=0.5).fit(data).evaluate()
-    >>> weights = data + 10
-    >>> # (3) Using a grid and weights for the data
-    >>> y = FFTKDE(kernel='epa', bw=0.5).fit(data, weights).evaluate(x)
-    >>> # (4) If you supply your own grid, it must be equidistant
-    >>> y = FFTKDE().fit(data)(np.linspace(-10, 10, num=2**12))
-
-    References
-    ----------
-    - Wand, M. P., and M. C. Jones. Kernel Smoothing.
-      London ; New York: Chapman and Hall/CRC, 1995. Pages 182-192.
-    - Statsmodels implementation, at
-      ``statsmodels.nonparametric.kde.KDEUnivariate``.
-
-    """
-
-    def __init__(self, kernel="gaussian", bw=1, norm=2):
-        self.norm = norm
-        super().__init__(kernel, bw)
-        assert isinstance(self.norm, numbers.Number) and self.norm > 0
-
-    def fit(self, data, weights=None):
-        """
-        Fit the KDE to the data. This validates the data and stores it.
-        Computations are performed upon evaluation on a specific grid.
-
-        Parameters
-        ----------
-        data: array-like
-            The data points.
-        weights: array-like
-            One weight per data point. Must have same shape as the data.
-
-        Returns
-        -------
-        self
-            Returns the instance.
-
-        Examples
-        --------
-        >>> data = [1, 3, 4, 7]
-        >>> weights = [3, 4, 2, 1]
-        >>> kde = FFTKDE().fit(data, weights=None)
-        >>> kde = FFTKDE().fit(data, weights=weights)
-        >>> x, y = kde.evaluate()
-        """
-
-        # Sets self.data
-        super().fit(data, weights)
-        return self
-
-    def evaluate(self, grid_points=None):
-        """
-        Evaluate on equidistant grid points.
-
-        Parameters
-        ----------
-        grid_points: array-like, int, tuple or None
-            A grid (mesh) to evaluate on. High dimensional grids must have
-            shape (obs, dims). If an integer is passed, it's the number of grid
-            points on an equidistant grid. If a tuple is passed, it's the
-            number of grid points in each dimension. If None, a grid will be
-            automatically created.
-
-        Returns
-        -------
-        y: array-like
-            If a grid is supplied, `y` is returned. If no grid is supplied,
-            a tuple (`x`, `y`) is returned.
-
-        Examples
-        --------
-        >>> kde = FFTKDE().fit([1, 3, 4, 7])
-        >>> # Three ways to evaluate a fitted KDE object:
-        >>> x, y = kde.evaluate()  # (1) Auto grid
-        >>> x, y = kde.evaluate(256)  # (2) Auto grid with 256 points
-        >>> # (3) Use a custom grid (make sure it's wider than the data)
-        >>> x_grid = np.linspace(-10, 25, num=2**10)  # <- Must be equidistant
-        >>> y = kde.evaluate(x_grid)  # Notice that only y is returned
-        """
-
-        # This method sets self.grid_points and verifies it
-        super().evaluate(grid_points)
-
-        # Extra verification for FFTKDE (checking the sorting property)
-        if not grid_is_sorted(self.grid_points):
-            raise ValueError("The grid must be sorted.")
-
-        if isinstance(self.bw, numbers.Number) and self.bw > 0:
-            bw = self.bw
-        else:
-            raise ValueError("The bw must be a number.")
-        self.bw = bw
-
-        # Step 0 - Make sure data points are inside of the grid
-        min_grid = np.min(self.grid_points, axis=0)
-        max_grid = np.max(self.grid_points, axis=0)
-
-        min_data = np.min(self.data, axis=0)
-        max_data = np.max(self.data, axis=0)
-        if not ((min_grid < min_data).all() and (max_grid > max_data).all()):
-            raise ValueError("Every data point must be inside of the grid.")
-
-        # Step 1 - Obtaining the grid counts
-        # TODO: Consider moving this to the fitting phase instead
-        data = linear_binning(self.data, grid_points=self.grid_points, weights=self.weights)
-
-        # Step 2 - Computing kernel weights
-        g_shape = self.grid_points.shape[1]
-        num_grid_points = np.array(list(len(np.unique(self.grid_points[:, i])) for i in range(g_shape)))
-
-        num_intervals = num_grid_points - 1
-        dx = (max_grid - min_grid) / num_intervals
-
-        # Find the real bandwidth, the support times the desired bw factor
-        if self.kernel.finite_support:
-            real_bw = self.kernel.support * self.bw
-        else:
-            # The parent class should compute this already. If not, compute
-            # it again. This optimization only dominates a little bit with
-            # few data points
-            try:
-                real_bw = self._kernel_practical_support
-            except AttributeError:
-                real_bw = self.kernel.practical_support(self.bw)
-
-        # Compute L, the number of dx'es to move out from 0 in kernel
-        L = np.minimum(np.floor(real_bw / dx), num_intervals + 1)
-        assert (dx * L <= real_bw).all()
-
-        # Evaluate the kernel once
-        grids = [np.linspace(-dx * L, dx * L, int(L * 2 + 1)) for (dx, L) in zip(dx, L)]
-        kernel_grid = cartesian(grids)
-        kernel_weights = self.kernel(kernel_grid, bw=self.bw, norm=self.norm)
-
-        # Reshape in preparation to
-        kernel_weights = kernel_weights.reshape(*[int(k * 2 + 1) for k in L])
-        data = data.reshape(*tuple(num_grid_points))
-
-        # Step 3 - Performing the convolution
-
-        # The following code block surpressed the warning:
-        #        anaconda3/lib/python3.6/site-packages/mkl_fft/_numpy_fft.py:
-        #            FutureWarning: Using a non-tuple sequence for multidimensional ...
-        #        output = mkl_fft.rfftn_numpy(a, s, axes)
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
-            ans = convolve(data, kernel_weights, mode="same").reshape(-1, 1)
-
-        return self._evalate_return_logic(ans, self.grid_points)
-
-
-if __name__ == "__main__":
-    import pytest
-
-    # --durations=10  <- May be used to show potentially slow tests
-    pytest.main(args=[".", "--doctest-modules", "-v", "--capture=sys"])
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Module for the FFTKDE.
+"""
+import numbers
+import warnings
+
+import numpy as np
+from scipy.signal import convolve
+
+from KDEpy.BaseKDE import BaseKDE
+from KDEpy.binning import grid_is_sorted, linear_binning
+from KDEpy.utils import cartesian
+
+
+class FFTKDE(BaseKDE):
+    r"""
+    This class implements a convolution (FFT) based computation of a KDE.
+    While this implementation is very fast, there are some limitations: (1) the
+    bandwidth must be constant, (2) the KDE must be evaluated on an
+    equidistant grid and (3) the grid must encompass every data point.
+    The finer the grid, the smaller the error.
+
+    The evaluation step is split into two phases. First the :math:`N` data
+    points are binned using a linear binning routine on an equidistant grid `x`
+    with :math:`n` grid points. This runs in :math:`O(N 2^d)` time.
+    Then the kernel is evaluated once on :math:`\leq n` points and the result
+    of the kernel evaluation and the binned data is convolved. Using the
+    convolution theorem, this step runs in :math:`O(n \log n)` time.
+    While :math:`N` may be millions, :math:`n` is typically 2**10. The total
+    running time of the algorithm is :math:`O(N 2^d + n \log n)`.
+    See references for more information.
+
+    The implementation is reminiscent of the one found in statsmodels. However,
+    unlike the statsmodels implementation every kernel is available for FFT
+    computation, weighted data is available for FFT computation, and no large
+    temporary arrays are created.
+
+    Parameters
+    ----------
+    kernel : str
+        The kernel function. See cls._available_kernels.keys() for choices.
+    bw : float or str
+        Bandwidth or bandwidth selection method. If a float is passed, it
+        is the standard deviation of the kernel. If a string it passed, it
+        is the bandwidth selection method, see cls._bw_methods.keys() for
+        choices.
+
+    Examples
+    --------
+    >>> data = np.random.randn(2**10)
+    >>> # (1) Automatic bw selection using Improved Sheather Jones (ISJ)
+    >>> x, y = FFTKDE(bw='ISJ').fit(data).evaluate()
+    >>> # (2) Explicit choice of kernel and bw (standard deviation of kernel)
+    >>> x, y = FFTKDE(kernel='triweight', bw=0.5).fit(data).evaluate()
+    >>> weights = data + 10
+    >>> # (3) Using a grid and weights for the data
+    >>> y = FFTKDE(kernel='epa', bw=0.5).fit(data, weights).evaluate(x)
+    >>> # (4) If you supply your own grid, it must be equidistant
+    >>> y = FFTKDE().fit(data)(np.linspace(-10, 10, num=2**12))
+
+    References
+    ----------
+    - Wand, M. P., and M. C. Jones. Kernel Smoothing.
+      London ; New York: Chapman and Hall/CRC, 1995. Pages 182-192.
+    - Statsmodels implementation, at
+      ``statsmodels.nonparametric.kde.KDEUnivariate``.
+
+    """
+
+    def __init__(self, kernel="gaussian", bw=1, norm=2):
+        self.norm = norm
+        super().__init__(kernel, bw)
+        assert isinstance(self.norm, numbers.Number) and self.norm > 0
+
+    def fit(self, data, weights=None):
+        """
+        Fit the KDE to the data. This validates the data and stores it.
+        Computations are performed upon evaluation on a specific grid.
+
+        Parameters
+        ----------
+        data: array-like
+            The data points.
+        weights: array-like
+            One weight per data point. Must have same shape as the data.
+
+        Returns
+        -------
+        self
+            Returns the instance.
+
+        Examples
+        --------
+        >>> data = [1, 3, 4, 7]
+        >>> weights = [3, 4, 2, 1]
+        >>> kde = FFTKDE().fit(data, weights=None)
+        >>> kde = FFTKDE().fit(data, weights=weights)
+        >>> x, y = kde.evaluate()
+        """
+
+        # Sets self.data
+        super().fit(data, weights)
+        return self
+
+    def evaluate(self, grid_points=None):
+        """
+        Evaluate on equidistant grid points.
+
+        Parameters
+        ----------
+        grid_points: array-like, int, tuple or None
+            A grid (mesh) to evaluate on. High dimensional grids must have
+            shape (obs, dims). If an integer is passed, it's the number of grid
+            points on an equidistant grid. If a tuple is passed, it's the
+            number of grid points in each dimension. If None, a grid will be
+            automatically created.
+
+        Returns
+        -------
+        y: array-like
+            If a grid is supplied, `y` is returned. If no grid is supplied,
+            a tuple (`x`, `y`) is returned.
+
+        Examples
+        --------
+        >>> kde = FFTKDE().fit([1, 3, 4, 7])
+        >>> # Three ways to evaluate a fitted KDE object:
+        >>> x, y = kde.evaluate()  # (1) Auto grid
+        >>> x, y = kde.evaluate(256)  # (2) Auto grid with 256 points
+        >>> # (3) Use a custom grid (make sure it's wider than the data)
+        >>> x_grid = np.linspace(-10, 25, num=2**10)  # <- Must be equidistant
+        >>> y = kde.evaluate(x_grid)  # Notice that only y is returned
+        """
+
+        # This method sets self.grid_points and verifies it
+        super().evaluate(grid_points)
+
+        # Extra verification for FFTKDE (checking the sorting property)
+        if not grid_is_sorted(self.grid_points):
+            raise ValueError("The grid must be sorted.")
+
+        if isinstance(self.bw, numbers.Number) and self.bw > 0:
+            bw = self.bw
+        else:
+            raise ValueError("The bw must be a number.")
+        self.bw = bw
+
+        # Step 0 - Make sure data points are inside of the grid
+        min_grid = np.min(self.grid_points, axis=0)
+        max_grid = np.max(self.grid_points, axis=0)
+
+        min_data = np.min(self.data, axis=0)
+        max_data = np.max(self.data, axis=0)
+        if not ((min_grid < min_data).all() and (max_grid > max_data).all()):
+            raise ValueError("Every data point must be inside of the grid.")
+
+        # Step 1 - Obtaining the grid counts
+        # TODO: Consider moving this to the fitting phase instead
+        data = linear_binning(self.data, grid_points=self.grid_points, weights=self.weights)
+
+        # Step 2 - Computing kernel weights
+        g_shape = self.grid_points.shape[1]
+        num_grid_points = np.array(list(len(np.unique(self.grid_points[:, i])) for i in range(g_shape)))
+
+        num_intervals = num_grid_points - 1
+        dx = (max_grid - min_grid) / num_intervals
+
+        # Find the real bandwidth, the support times the desired bw factor
+        if self.kernel.finite_support:
+            real_bw = self.kernel.support * self.bw
+        else:
+            # The parent class should compute this already. If not, compute
+            # it again. This optimization only dominates a little bit with
+            # few data points
+            try:
+                real_bw = self._kernel_practical_support
+            except AttributeError:
+                real_bw = self.kernel.practical_support(self.bw)
+
+        # Compute L, the number of dx'es to move out from 0 in kernel
+        L = np.minimum(np.floor(real_bw / dx), num_intervals + 1)
+        assert (dx * L <= real_bw).all()
+
+        # Evaluate the kernel once
+        grids = [np.linspace(-dx * L, dx * L, int(L * 2 + 1)) for (dx, L) in zip(dx, L)]
+        kernel_grid = cartesian(grids)
+        kernel_weights = self.kernel(kernel_grid, bw=self.bw, norm=self.norm)
+
+        # Reshape in preparation to
+        kernel_weights = kernel_weights.reshape(*[int(k * 2 + 1) for k in L])
+        data = data.reshape(*tuple(num_grid_points))
+
+        # Step 3 - Performing the convolution
+
+        # The following code block surpressed the warning:
+        #        anaconda3/lib/python3.6/site-packages/mkl_fft/_numpy_fft.py:
+        #            FutureWarning: Using a non-tuple sequence for multidimensional ...
+        #        output = mkl_fft.rfftn_numpy(a, s, axes)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            ans = convolve(data, kernel_weights, mode="same").reshape(-1, 1)
+
+        return self._evalate_return_logic(ans, self.grid_points)
+
+
+if __name__ == "__main__":
+    import pytest
+
+    # --durations=10  <- May be used to show potentially slow tests
+    pytest.main(args=[".", "--doctest-modules", "-v", "--capture=sys"])
```

## KDEpy/NaiveKDE.py

 * *Ordering differences only*

```diff
@@ -1,143 +1,143 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Module for the NaiveKDE.
-"""
-import itertools
-import numbers
-
-import numpy as np
-
-from KDEpy.BaseKDE import BaseKDE
-
-
-class NaiveKDE(BaseKDE):
-    """
-    This class implements a naive computation of a kernel density estimate. The
-    advantages are that choices of bandwidth, norms, weights and grids are
-    straightforward -- the user can do almost anything. The disadvantage is
-    that computations are slow on more than a couple of thousand data points.
-
-    Parameters
-    ----------
-    kernel : str
-        The kernel function. See cls._available_kernels.keys() for choices.
-    bw : float, str or array-like
-        Bandwidth or bandwidth selection method. If a float is passed, it
-        is the standard deviation of the kernel. If a string it passed, it
-        is the bandwidth selection method, see cls._bw_methods.keys() for
-        choices. If an array-like it passed, it is the bandwidth of each
-        point.
-    norm : float
-        The p-norm used to compute the distances in higher dimensions.
-
-    Examples
-    --------
-    >>> data = np.random.randn(2**10)
-    >>> # (1) Automatic bw selection using Improved Sheather Jones
-    >>> x, y = NaiveKDE(bw='ISJ').fit(data).evaluate()
-    >>> # (2) Explicit choice of kernel and bw (standard deviation of kernel)
-    >>> x, y = NaiveKDE(kernel='triweight', bw=0.5).fit(data).evaluate()
-    >>> weights = data + 10
-    >>> # (3) Using a grid and weights for the data
-    >>> y = NaiveKDE(kernel='epa', bw=0.5).fit(data, weights).evaluate(x)
-
-    References
-    ----------
-    - Silverman, B. W. Density Estimation for Statistics and Data Analysis.
-      Boca Raton: Chapman and Hall, 1986.
-    - Wand, M. P., and M. C. Jones. Kernel Smoothing.
-      London ; New York: Chapman and Hall/CRC, 1995.
-    - Scipy implementation, at ``scipy.stats.gaussian_kde``.
-    """
-
-    def __init__(self, kernel="gaussian", bw=1, norm=2):
-        super().__init__(kernel, bw)
-        self.norm = norm
-
-    def fit(self, data, weights=None):
-        """
-        Fit the KDE to the data. This validates the data and stores it.
-        Computations are performed when the KDE is evaluated on a grid.
-
-        Parameters
-        ----------
-        data: array-like
-            The data points. High dimensional data must have shape (obs, dims).
-        weights: array-like
-            One weight per data point. Must have shape (obs,). If None is
-            passed, uniform weights are used.
-
-        Returns
-        -------
-        self
-            Returns the instance.
-
-        Examples
-        --------
-        >>> data = [1, 3, 4, 7]
-        >>> weights = [3, 4, 2, 1]
-        >>> kde = NaiveKDE().fit(data, weights=None)
-        >>> kde = NaiveKDE().fit(data, weights=weights)
-        >>> x, y = kde()
-        """
-        # Sets self.data
-        super().fit(data, weights)
-        return self
-
-    def evaluate(self, grid_points=None):
-        """
-        Evaluate on grid points.
-
-        Parameters
-        ----------
-        grid_points: array-like, int, tuple or None
-            A grid (mesh) to evaluate on. High dimensional grids must have
-            shape (obs, dims). If an integer is passed, it's the number of grid
-            points on an equidistant grid. If a tuple is passed, it's the
-            number of grid points in each dimension. If None, a grid will be
-            automatically created.
-
-        Returns
-        -------
-        y: array-like
-            If a grid is supplied, `y` is returned. If no grid is supplied,
-            a tuple (`x`, `y`) is returned.
-
-        Examples
-        --------
-        >>> kde = NaiveKDE().fit([1, 3, 4, 7])
-        >>> # Two ways to evaluate, either with a grid or without
-        >>> x, y = kde.evaluate()
-        >>> x, y = kde.evaluate(256)
-        >>> y = kde.evaluate(x)
-        """
-        # This method sets self.grid points and verifies it
-        # NaiveKDE does not convert the bw to a scalar, since a vector is
-        # allowed too.
-        super().evaluate(grid_points, bw_to_scalar=False)
-
-        # Create zeros on the grid points
-        evaluated = np.zeros(self.grid_points.shape[0])
-
-        # For every data point, compute the kernel and add to the grid
-        bw = self.bw
-        if isinstance(bw, numbers.Number):
-            bw = np.asfarray(np.ones(self.data.shape[0]) * bw)
-
-        # TODO: Implementation w.r.t grid points for faster evaluation
-        # See the SciPy evaluation for how this can be done
-        weights = itertools.repeat(1 / self.data.shape[0]) if self.weights is None else self.weights
-
-        for weight, data_point, bw in zip(weights, self.data, bw):
-            x = self.grid_points - data_point
-            evaluated += weight * self.kernel(x, bw=bw, norm=self.norm)
-
-        return self._evalate_return_logic(evaluated, self.grid_points)
-
-
-if __name__ == "__main__":
-    import pytest
-
-    # --durations=10  <- May be used to show potentially slow tests
-    pytest.main(args=[".", "--doctest-modules", "-v"])
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Module for the NaiveKDE.
+"""
+import itertools
+import numbers
+
+import numpy as np
+
+from KDEpy.BaseKDE import BaseKDE
+
+
+class NaiveKDE(BaseKDE):
+    """
+    This class implements a naive computation of a kernel density estimate. The
+    advantages are that choices of bandwidth, norms, weights and grids are
+    straightforward -- the user can do almost anything. The disadvantage is
+    that computations are slow on more than a couple of thousand data points.
+
+    Parameters
+    ----------
+    kernel : str
+        The kernel function. See cls._available_kernels.keys() for choices.
+    bw : float, str or array-like
+        Bandwidth or bandwidth selection method. If a float is passed, it
+        is the standard deviation of the kernel. If a string it passed, it
+        is the bandwidth selection method, see cls._bw_methods.keys() for
+        choices. If an array-like it passed, it is the bandwidth of each
+        point.
+    norm : float
+        The p-norm used to compute the distances in higher dimensions.
+
+    Examples
+    --------
+    >>> data = np.random.randn(2**10)
+    >>> # (1) Automatic bw selection using Improved Sheather Jones
+    >>> x, y = NaiveKDE(bw='ISJ').fit(data).evaluate()
+    >>> # (2) Explicit choice of kernel and bw (standard deviation of kernel)
+    >>> x, y = NaiveKDE(kernel='triweight', bw=0.5).fit(data).evaluate()
+    >>> weights = data + 10
+    >>> # (3) Using a grid and weights for the data
+    >>> y = NaiveKDE(kernel='epa', bw=0.5).fit(data, weights).evaluate(x)
+
+    References
+    ----------
+    - Silverman, B. W. Density Estimation for Statistics and Data Analysis.
+      Boca Raton: Chapman and Hall, 1986.
+    - Wand, M. P., and M. C. Jones. Kernel Smoothing.
+      London ; New York: Chapman and Hall/CRC, 1995.
+    - Scipy implementation, at ``scipy.stats.gaussian_kde``.
+    """
+
+    def __init__(self, kernel="gaussian", bw=1, norm=2):
+        super().__init__(kernel, bw)
+        self.norm = norm
+
+    def fit(self, data, weights=None):
+        """
+        Fit the KDE to the data. This validates the data and stores it.
+        Computations are performed when the KDE is evaluated on a grid.
+
+        Parameters
+        ----------
+        data: array-like
+            The data points. High dimensional data must have shape (obs, dims).
+        weights: array-like
+            One weight per data point. Must have shape (obs,). If None is
+            passed, uniform weights are used.
+
+        Returns
+        -------
+        self
+            Returns the instance.
+
+        Examples
+        --------
+        >>> data = [1, 3, 4, 7]
+        >>> weights = [3, 4, 2, 1]
+        >>> kde = NaiveKDE().fit(data, weights=None)
+        >>> kde = NaiveKDE().fit(data, weights=weights)
+        >>> x, y = kde()
+        """
+        # Sets self.data
+        super().fit(data, weights)
+        return self
+
+    def evaluate(self, grid_points=None):
+        """
+        Evaluate on grid points.
+
+        Parameters
+        ----------
+        grid_points: array-like, int, tuple or None
+            A grid (mesh) to evaluate on. High dimensional grids must have
+            shape (obs, dims). If an integer is passed, it's the number of grid
+            points on an equidistant grid. If a tuple is passed, it's the
+            number of grid points in each dimension. If None, a grid will be
+            automatically created.
+
+        Returns
+        -------
+        y: array-like
+            If a grid is supplied, `y` is returned. If no grid is supplied,
+            a tuple (`x`, `y`) is returned.
+
+        Examples
+        --------
+        >>> kde = NaiveKDE().fit([1, 3, 4, 7])
+        >>> # Two ways to evaluate, either with a grid or without
+        >>> x, y = kde.evaluate()
+        >>> x, y = kde.evaluate(256)
+        >>> y = kde.evaluate(x)
+        """
+        # This method sets self.grid points and verifies it
+        # NaiveKDE does not convert the bw to a scalar, since a vector is
+        # allowed too.
+        super().evaluate(grid_points, bw_to_scalar=False)
+
+        # Create zeros on the grid points
+        evaluated = np.zeros(self.grid_points.shape[0])
+
+        # For every data point, compute the kernel and add to the grid
+        bw = self.bw
+        if isinstance(bw, numbers.Number):
+            bw = np.asfarray(np.ones(self.data.shape[0]) * bw)
+
+        # TODO: Implementation w.r.t grid points for faster evaluation
+        # See the SciPy evaluation for how this can be done
+        weights = itertools.repeat(1 / self.data.shape[0]) if self.weights is None else self.weights
+
+        for weight, data_point, bw in zip(weights, self.data, bw):
+            x = self.grid_points - data_point
+            evaluated += weight * self.kernel(x, bw=bw, norm=self.norm)
+
+        return self._evalate_return_logic(evaluated, self.grid_points)
+
+
+if __name__ == "__main__":
+    import pytest
+
+    # --durations=10  <- May be used to show potentially slow tests
+    pytest.main(args=[".", "--doctest-modules", "-v"])
```

## KDEpy/TreeKDE.py

 * *Ordering differences only*

```diff
@@ -1,183 +1,183 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Module for the TreeKDE.
-"""
-import numbers
-
-import numpy as np
-from scipy.spatial import cKDTree
-
-from KDEpy.BaseKDE import BaseKDE
-
-
-class TreeKDE(BaseKDE):
-    """
-    This class implements a tree-based computation of a kernel density
-    estimate. It works by segmenting the space recursively into smaller parts.
-
-    This makes computing a kernel density estimate at a location easier, since
-    we are able to query the tree structure for nearby points instead of having
-    to evaluate the kernel function on all data points. For kernels without
-    finite support, their support is approximated. The ``scipy`` k-d tree is
-    used as the underlying algorithm.
-
-    Parameters
-    ----------
-    kernel : str
-        The kernel function. See cls._available_kernels.keys() for choices.
-    bw : float, str or array-like
-        Bandwidth or bandwidth selection method. If a float is passed, it
-        is the standard deviation of the kernel. If a string it passed, it
-        is the bandwidth selection method, see cls._bw_methods.keys() for
-        choices. If an array-like it passed, it is the bandwidth of each
-        point.
-    norm : float
-        The p-norm used to compute the distances in higher dimensions.
-
-    Examples
-    --------
-    >>> data = np.random.randn(2**10)
-    >>> # (1) Automatic bw selection using Improved Sheather Jones
-    >>> x, y = TreeKDE(bw='ISJ').fit(data).evaluate()
-    >>> # (2) Explicit choice of kernel and bw (standard deviation of kernel)
-    >>> x, y = TreeKDE(kernel='triweight', bw=0.5).fit(data).evaluate()
-    >>> weights = data + 10
-    >>> # (3) Using a grid and weights for the data
-    >>> y = TreeKDE(kernel='epa', bw=0.5).fit(data, weights).evaluate(x)
-
-    References
-    ----------
-    - Friedman, Jerome H., Jon Louis Bentley, and Raphael Ari Finkel.
-      An Algorithm for Finding Best Matches in Logarithmic Expected Time.
-      ACM Trans. Math. Softw. 3, no. 3 (September 1977): 209–226.
-      https://doi.org/10.1145/355744.355745.
-    - Maneewongvatana, Songrit, and David M. Mount.
-      It’s Okay to Be Skinny, If Your Friends Are Fat.
-      In Center for Geometric Computing 4th Annual Workshop on Computational
-      Geometry, 2:1–8, 1999.
-    - Silverman, B. W. Density Estimation for Statistics and Data Analysis.
-      Boca Raton: Chapman and Hall, 1986. Page 99 for reference to kd-tree.
-    - Scipy implementation, at ``scipy.spatial.KDTree``.
-    """
-
-    def __init__(self, kernel="gaussian", bw=1, norm=2.0):
-        super().__init__(kernel, bw)
-        self.norm = norm
-
-    def fit(self, data, weights=None):
-        """
-        Fit the KDE to the data. This validates the data and stores it.
-        Computations are performed upon evaluation on a grid.
-
-        Parameters
-        ----------
-        data: array-like
-            The data points.
-        weights: array-like
-            One weight per data point. Numbers of observations must match
-            the data points.
-
-        Returns
-        -------
-        self
-            Returns the instance.
-
-        Examples
-        --------
-        >>> data = [1, 3, 4, 7]
-        >>> weights = [3, 4, 2, 1]
-        >>> kde = TreeKDE().fit(data, weights=None)
-        >>> kde = TreeKDE().fit(data, weights=weights)
-        >>> x, y = kde()
-        """
-        # Sets self.data
-        super().fit(data, weights)
-        return self
-
-    def evaluate(self, grid_points=None, eps=10e-4):
-        """
-        Evaluate on grid points.
-
-        Parameters
-        ----------
-        grid_points: array-like, int, tuple or None
-            A grid (mesh) to evaluate on. High dimensional grids must have
-            shape (obs, dims). If an integer is passed, it's the number of grid
-            points on an equidistant grid. If a tuple is passed, it's the
-            number of grid points in each dimension. If None, a grid will be
-            automatically created.
-        eps: float
-            The maximal total error in absolute terms when estimating the
-            effective support of a kernel which has infinite support. Setting
-            this too high will produced a jagged estimate.
-
-        Returns
-        -------
-        y: array-like
-            If a grid is supplied, `y` is returned. If no grid is supplied,
-            a tuple (`x`, `y`) is returned.
-
-        Examples
-        --------
-        >>> kde = TreeKDE().fit([1, 3, 4, 7])
-        >>> # Two ways to evaluate, either with a grid or without
-        >>> x, y = kde.evaluate()
-        >>> x, y = kde.evaluate(256)
-        >>> y = kde.evaluate(x)
-        """
-
-        # This method sets self.grid points and verifies it
-        super().evaluate(grid_points)
-
-        evaluated = np.zeros(self.grid_points.shape[0])
-
-        # For every data point, compute the kernel and add to the grid
-        obs, dims = self.data.shape
-        bw = self.bw
-        if isinstance(bw, numbers.Number):
-            bw = np.asfarray(np.ones(obs) * bw)
-        else:
-            bw = np.asarray_chkfinite(bw, dtype=float)
-
-        # Initialize the tree structure for fast lookups of neighbors
-        tree = cKDTree(self.data)
-
-        # Compute the kernel radius
-        maximal_bw = np.max(bw)
-        if not eps > 0:
-            raise ValueError("eps must be > 0.")
-        kernel_radius = self.kernel.practical_support(maximal_bw, eps)
-
-        # Since we iterate through grid points, we need the maximum bw to
-        # ensure that we get data points that are close enough
-        for i, grid_point in enumerate(self.grid_points):
-            # Query for data points that are close to this grid point
-            # TODO: Is this epsilon value sensible?
-            # Scipy 1.3.0 introduced error: ValueError: ndarray is not C-contiguous
-            grid_point = np.ascontiguousarray(grid_point)
-            indices = tree.query_ball_point(x=grid_point, r=kernel_radius, p=self.norm, eps=eps * obs**0.5)
-
-            # Use broadcasting to find x-values (distances)
-            x = grid_point - self.data[indices]
-            kernel_estimates = self.kernel(x, bw=bw[indices], norm=self.norm)
-
-            if self.weights is not None:
-                weights_subset = self.weights[indices]
-                assert kernel_estimates.shape == weights_subset.shape
-            assert kernel_estimates.shape == bw[indices].shape
-
-            # Unpack the (n, 1) arrays to (n,) and compute the doc product
-            if self.weights is not None:
-                evaluated[i] += np.dot(kernel_estimates, weights_subset)
-            else:
-                evaluated[i] += np.sum(kernel_estimates) / obs
-
-        return self._evalate_return_logic(evaluated, self.grid_points)
-
-
-if __name__ == "__main__":
-    import pytest
-
-    # --durations=10  <- May be used to show potentially slow tests
-    pytest.main(args=[".", "--doctest-modules", "-v"])
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Module for the TreeKDE.
+"""
+import numbers
+
+import numpy as np
+from scipy.spatial import cKDTree
+
+from KDEpy.BaseKDE import BaseKDE
+
+
+class TreeKDE(BaseKDE):
+    """
+    This class implements a tree-based computation of a kernel density
+    estimate. It works by segmenting the space recursively into smaller parts.
+
+    This makes computing a kernel density estimate at a location easier, since
+    we are able to query the tree structure for nearby points instead of having
+    to evaluate the kernel function on all data points. For kernels without
+    finite support, their support is approximated. The ``scipy`` k-d tree is
+    used as the underlying algorithm.
+
+    Parameters
+    ----------
+    kernel : str
+        The kernel function. See cls._available_kernels.keys() for choices.
+    bw : float, str or array-like
+        Bandwidth or bandwidth selection method. If a float is passed, it
+        is the standard deviation of the kernel. If a string it passed, it
+        is the bandwidth selection method, see cls._bw_methods.keys() for
+        choices. If an array-like it passed, it is the bandwidth of each
+        point.
+    norm : float
+        The p-norm used to compute the distances in higher dimensions.
+
+    Examples
+    --------
+    >>> data = np.random.randn(2**10)
+    >>> # (1) Automatic bw selection using Improved Sheather Jones
+    >>> x, y = TreeKDE(bw='ISJ').fit(data).evaluate()
+    >>> # (2) Explicit choice of kernel and bw (standard deviation of kernel)
+    >>> x, y = TreeKDE(kernel='triweight', bw=0.5).fit(data).evaluate()
+    >>> weights = data + 10
+    >>> # (3) Using a grid and weights for the data
+    >>> y = TreeKDE(kernel='epa', bw=0.5).fit(data, weights).evaluate(x)
+
+    References
+    ----------
+    - Friedman, Jerome H., Jon Louis Bentley, and Raphael Ari Finkel.
+      An Algorithm for Finding Best Matches in Logarithmic Expected Time.
+      ACM Trans. Math. Softw. 3, no. 3 (September 1977): 209–226.
+      https://doi.org/10.1145/355744.355745.
+    - Maneewongvatana, Songrit, and David M. Mount.
+      It’s Okay to Be Skinny, If Your Friends Are Fat.
+      In Center for Geometric Computing 4th Annual Workshop on Computational
+      Geometry, 2:1–8, 1999.
+    - Silverman, B. W. Density Estimation for Statistics and Data Analysis.
+      Boca Raton: Chapman and Hall, 1986. Page 99 for reference to kd-tree.
+    - Scipy implementation, at ``scipy.spatial.KDTree``.
+    """
+
+    def __init__(self, kernel="gaussian", bw=1, norm=2.0):
+        super().__init__(kernel, bw)
+        self.norm = norm
+
+    def fit(self, data, weights=None):
+        """
+        Fit the KDE to the data. This validates the data and stores it.
+        Computations are performed upon evaluation on a grid.
+
+        Parameters
+        ----------
+        data: array-like
+            The data points.
+        weights: array-like
+            One weight per data point. Numbers of observations must match
+            the data points.
+
+        Returns
+        -------
+        self
+            Returns the instance.
+
+        Examples
+        --------
+        >>> data = [1, 3, 4, 7]
+        >>> weights = [3, 4, 2, 1]
+        >>> kde = TreeKDE().fit(data, weights=None)
+        >>> kde = TreeKDE().fit(data, weights=weights)
+        >>> x, y = kde()
+        """
+        # Sets self.data
+        super().fit(data, weights)
+        return self
+
+    def evaluate(self, grid_points=None, eps=10e-4):
+        """
+        Evaluate on grid points.
+
+        Parameters
+        ----------
+        grid_points: array-like, int, tuple or None
+            A grid (mesh) to evaluate on. High dimensional grids must have
+            shape (obs, dims). If an integer is passed, it's the number of grid
+            points on an equidistant grid. If a tuple is passed, it's the
+            number of grid points in each dimension. If None, a grid will be
+            automatically created.
+        eps: float
+            The maximal total error in absolute terms when estimating the
+            effective support of a kernel which has infinite support. Setting
+            this too high will produced a jagged estimate.
+
+        Returns
+        -------
+        y: array-like
+            If a grid is supplied, `y` is returned. If no grid is supplied,
+            a tuple (`x`, `y`) is returned.
+
+        Examples
+        --------
+        >>> kde = TreeKDE().fit([1, 3, 4, 7])
+        >>> # Two ways to evaluate, either with a grid or without
+        >>> x, y = kde.evaluate()
+        >>> x, y = kde.evaluate(256)
+        >>> y = kde.evaluate(x)
+        """
+
+        # This method sets self.grid points and verifies it
+        super().evaluate(grid_points)
+
+        evaluated = np.zeros(self.grid_points.shape[0])
+
+        # For every data point, compute the kernel and add to the grid
+        obs, dims = self.data.shape
+        bw = self.bw
+        if isinstance(bw, numbers.Number):
+            bw = np.asfarray(np.ones(obs) * bw)
+        else:
+            bw = np.asarray_chkfinite(bw, dtype=float)
+
+        # Initialize the tree structure for fast lookups of neighbors
+        tree = cKDTree(self.data)
+
+        # Compute the kernel radius
+        maximal_bw = np.max(bw)
+        if not eps > 0:
+            raise ValueError("eps must be > 0.")
+        kernel_radius = self.kernel.practical_support(maximal_bw, eps)
+
+        # Since we iterate through grid points, we need the maximum bw to
+        # ensure that we get data points that are close enough
+        for i, grid_point in enumerate(self.grid_points):
+            # Query for data points that are close to this grid point
+            # TODO: Is this epsilon value sensible?
+            # Scipy 1.3.0 introduced error: ValueError: ndarray is not C-contiguous
+            grid_point = np.ascontiguousarray(grid_point)
+            indices = tree.query_ball_point(x=grid_point, r=kernel_radius, p=self.norm, eps=eps * obs**0.5)
+
+            # Use broadcasting to find x-values (distances)
+            x = grid_point - self.data[indices]
+            kernel_estimates = self.kernel(x, bw=bw[indices], norm=self.norm)
+
+            if self.weights is not None:
+                weights_subset = self.weights[indices]
+                assert kernel_estimates.shape == weights_subset.shape
+            assert kernel_estimates.shape == bw[indices].shape
+
+            # Unpack the (n, 1) arrays to (n,) and compute the doc product
+            if self.weights is not None:
+                evaluated[i] += np.dot(kernel_estimates, weights_subset)
+            else:
+                evaluated[i] += np.sum(kernel_estimates) / obs
+
+        return self._evalate_return_logic(evaluated, self.grid_points)
+
+
+if __name__ == "__main__":
+    import pytest
+
+    # --durations=10  <- May be used to show potentially slow tests
+    pytest.main(args=[".", "--doctest-modules", "-v"])
```

## KDEpy/__init__.py

```diff
@@ -1,12 +1,15 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-
-from KDEpy.FFTKDE import FFTKDE
-from KDEpy.NaiveKDE import NaiveKDE
-from KDEpy.TreeKDE import TreeKDE
-
-__version__ = "1.1.1"
-__author__ = "tommyod"
-
-__all__ = ["TreeKDE", "NaiveKDE", "FFTKDE"]
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+import importlib.metadata
+
+
+from KDEpy.FFTKDE import FFTKDE
+from KDEpy.NaiveKDE import NaiveKDE
+from KDEpy.TreeKDE import TreeKDE
+
+
+__version__ = importlib.metadata.version("KDEpy")
+__author__ = "tommyod"
+
+__all__ = ["TreeKDE", "NaiveKDE", "FFTKDE"]
```

## KDEpy/binning.py

 * *Ordering differences only*

```diff
@@ -1,443 +1,443 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Module for functions related to linear binning. These functions perform
-linear binning on weighted data. This is typically a preprocessing step
-before convolving with a kernel in the FFTKDE, but may also be used to
-reduce the effective number of data points in any algorithm.
-
-The idea behind linear binning is the following: (1) go through every
-data point and (2) assign a weight to the 2^dims nearest grid points.
-In `dims` dimensions, there are 2 points on the grid to consider in
-each dimension, so a total of 2^dims grid points must be assigned weights to
-for every data point. The weights are determined by the proportion of
-the volume of this hypercube that is enclosed by the data point.
-
-A ------------------------------ B
-|                    |           |
-|                    |           |
-|                    X-----------|
-|                                |
-|                                |
-|                                |
-C ------------------------------ C
-
-References
-----------
-- Fan, Jianqing, and James S. Marron.
-  “Fast Implementations of Nonparametric Curve Estimators.”
-  Journal of Computational and Graphical Statistics 3, no. 1 (March 1, 1994).
-  https://doi.org/10.1080/10618600.1994.10474629.
-"""
-import functools
-import itertools
-import operator
-
-import numpy as np
-
-import cutils
-from KDEpy.utils import cartesian
-
-grid_is_sorted = cutils.grid_is_sorted
-
-# This parameter was in use when a NumPy implementation and a Cython
-# implementation were both used. Now only Cython is used.
-_use_Cython = True
-
-
-def linbin_cython(data, grid_points, weights=None):
-    """
-    1D Linear binning using Cython. Assigns weights to grid points from data.
-
-    Runs in approx 10 ms on 1 million data points.
-
-    Parameters
-    ----------
-    data : array-like
-        The data to bin. Must be of shape (obs,).
-    grid_points : array-like
-        Equidistant grid points to assign weights to.
-        Must be of shape (points,).
-    weights : array-like
-        The weights of the data points.
-        Must be of shape (obs,).
-
-    Examples
-    --------
-    >>> data = np.array([2, 2.5, 3, 4])
-    >>> ans = linbin_cython(data, np.arange(6), weights=None)
-    >>> np.allclose(ans, np.array([0, 0, 0.375, 0.375, 0.25, 0]))
-    True
-    >>> ans = linbin_cython(data, np.arange(6), weights=np.arange(1, 5))
-    >>> np.allclose(ans, np.array([0, 0, 0.2, 0.4, 0.4, 0]))
-    True
-    >>> data = np.array([2, 2.5, 3, 4])
-    >>> ans = linbin_cython(data, np.arange(1, 7), weights=None)
-    >>> np.allclose(ans, np.array([0, 0.375, 0.375, 0.25, 0, 0]))
-    True
-    """
-    # Convert the data and grid points
-    data = np.asarray_chkfinite(data, dtype=float)
-    grid_points = np.asarray_chkfinite(grid_points, dtype=float)
-
-    assert len(data.shape) == 1
-    assert len(grid_points.shape) == 1
-
-    # Verify that the grid is equidistant
-    diffs = np.diff(grid_points)
-    assert np.allclose(np.ones_like(diffs) * diffs[0], diffs)
-
-    if weights is not None:
-        assert len(weights.shape) == 1
-        weights = np.asarray_chkfinite(weights, dtype=float)
-        weights = weights / np.sum(weights)
-
-    if (weights is not None) and (len(data) != len(weights)):
-        raise ValueError("Length of data must match length of weights.")
-
-    # Transform the data
-    min_grid = np.min(grid_points)
-    max_grid = np.max(grid_points)
-    num_intervals = len(grid_points) - 1  # Number of intervals
-    dx = (max_grid - min_grid) / num_intervals
-    transformed_data = (data - min_grid) / dx
-
-    result = np.asfarray(np.zeros(num_intervals + 2))
-
-    # Two Cython functions are implemented, one for weighted data and one
-    # for unweighted data, since creating equal weights is costly w.r.t time
-    if weights is None:
-        result = cutils.iterate_data_1D(transformed_data, result)
-        return np.asfarray(result[:-1]) / transformed_data.shape[0]
-    else:
-        res = cutils.iterate_data_1D_weighted(transformed_data, weights, result)
-        return np.asfarray(res[:-1])  # Remove last, outside of grid
-
-
-def linbin_numpy(data, grid_points, weights=None):
-    """
-    1D Linear binning using NumPy. Assigns weights to grid points from data.
-
-    This function is fast for data sets upto approximately 1-10 million,
-    it uses vectorized NumPy functions to perform linear binning. Takes around
-    100 ms on 1 million data points, so not nearly as fast as the Cython
-    implementation (10 ms).
-
-    Parameters
-    ----------
-    data : array-like
-        Must be of shape (obs,).
-    grid_points : array-like
-        Must be of shape (points,).
-    weights : array-like
-        Must be of shape (obs,).
-
-    Examples
-    --------
-    >>> data = np.array([2, 2.5, 3, 4])
-    >>> ans = linbin_numpy(data, np.arange(6), weights=None)
-    >>> np.allclose(ans, np.array([0, 0, 0.375, 0.375, 0.25, 0]))
-    True
-    >>> ans = linbin_numpy(data, np.arange(6), weights=np.arange(1, 5))
-    >>> np.allclose(ans, np.array([0, 0, 0.2, 0.4, 0.4, 0]))
-    True
-    >>> data = np.array([2, 2.5, 3, 4])
-    >>> ans = linbin_numpy(data, np.arange(1, 7), weights=None)
-    >>> np.allclose(ans, np.array([0, 0.375, 0.375, 0.25, 0, 0]))
-    True
-    """
-    # Convert the data and grid points
-    data = np.asarray_chkfinite(data, dtype=float)
-    grid_points = np.asarray_chkfinite(grid_points, dtype=float)
-    assert len(data.shape) == 1
-    assert len(grid_points.shape) == 1
-
-    # Verify that the grid is equidistant
-    diffs = np.diff(grid_points)
-    assert np.allclose(np.ones_like(diffs) * diffs[0], diffs)
-
-    if weights is None:
-        weights = np.ones_like(data)
-
-    weights = np.asarray_chkfinite(weights, dtype=float)
-    weights = weights / np.sum(weights)
-
-    if not len(data) == len(weights):
-        raise ValueError("Length of data must match length of weights.")
-
-    # Transform the data
-    min_grid = np.min(grid_points)
-    max_grid = np.max(grid_points)
-    num_intervals = len(grid_points) - 1
-    dx = (max_grid - min_grid) / num_intervals
-    transformed_data = (data - min_grid) / dx
-
-    # Compute the integral and fractional part of the data
-    # The integral part is used for lookups, the fractional part is used
-    # to weight the data
-    fractional, integral = np.modf(transformed_data)
-    integral = integral.astype(int)
-
-    # Sort the integral values, and the fractional data and weights by
-    # the same key. This lets us use binary search, which is faster
-    # than using a mask in the the loop below
-    indices_sorted = np.argsort(integral)
-    integral = integral[indices_sorted]
-    fractional = fractional[indices_sorted]
-    weights = weights[indices_sorted]
-
-    # Pre-compute these products, as they are used in the loop many times
-    frac_weights = fractional * weights
-    neg_frac_weights = weights - frac_weights
-
-    # If the data is not a subset of the grid, the integral values will be
-    # outside of the grid. To solve the problem, we filter these values away
-    unique_integrals = np.unique(integral)
-    unique_integrals = unique_integrals[(unique_integrals >= 0) & (unique_integrals <= len(grid_points))]
-
-    result = np.asfarray(np.zeros(len(grid_points) + 1))
-    for grid_point in unique_integrals:
-        # Use binary search to find indices for the grid point
-        # Then sum the data assigned to that grid point
-        low_index = np.searchsorted(integral, grid_point, side="left")
-        high_index = np.searchsorted(integral, grid_point, side="right")
-        result[grid_point] += neg_frac_weights[low_index:high_index].sum()
-        result[grid_point + 1] += frac_weights[low_index:high_index].sum()
-
-    return result[:-1]
-
-
-def linbin_Ndim_python(data, grid_points, weights=None):
-    """
-    d-dimensional linear binning. This is a slow, pure-Python function.
-    Mainly used for testing purposes.
-
-    With :math:`N` data points, and :math:`n` grid points in each dimension
-    :math:`d`, the running time is :math:`O(N2^d)`. For each point the
-    algorithm finds the nearest points, of which there are two in each
-    dimension.
-
-    Parameters
-    ----------
-    data : array-like
-        The data must be of shape (obs, dims).
-    grid_points : array-like
-        Grid, where cartesian product is already performed.
-    weights : array-like
-        Must have shape (obs,).
-
-    Examples
-    --------
-    >>> from KDEpy.utils import autogrid
-    >>> grid_points = autogrid(np.array([[0, 0, 0]]), num_points=(3, 3, 3))
-    >>> d = linbin_Ndim_python(np.array([[1.0, 0, 0]]), grid_points, None)
-    """
-    # Convert the data and grid points
-    data = np.asarray_chkfinite(data, dtype=float)
-    grid_points = np.asarray_chkfinite(grid_points, dtype=float)
-    if weights is not None:
-        weights = np.asarray_chkfinite(weights, dtype=float)
-    else:
-        # This is not efficient, but this function should just be correct
-        # The faster algorithm is implemented in Cython
-        weights = np.ones(data.shape[0])
-    weights = weights / np.sum(weights)
-
-    if (weights is not None) and (data.shape[0] != len(weights)):
-        raise ValueError("Length of data must match length of weights.")
-
-    obs_tot, dims = grid_points.shape
-
-    # Compute the number of grid points for each dimension in the grid
-    grid_num = (grid_points[:, i] for i in range(dims))
-    grid_num = np.array(list(len(np.unique(g)) for g in grid_num))
-
-    # Scale the data to the grid
-    min_grid = np.min(grid_points, axis=0)
-    max_grid = np.max(grid_points, axis=0)
-    num_intervals = grid_num - 1  # Number of intervals
-    dx = (max_grid - min_grid) / num_intervals
-    data = (data - min_grid) / dx
-
-    # Create results
-    result = np.zeros(grid_points.shape[0], dtype=float)
-
-    # Go through every data point
-    for observation, weight in zip(data, weights):
-        # Compute integer part and fractional part for every x_i
-        # Compute relation to previous grid point, and next grid point
-        int_frac = (
-            (
-                (int(coordinate), 1 - (coordinate % 1)),
-                (int(coordinate) + 1, (coordinate % 1)),
-            )
-            for coordinate in observation
-        )
-
-        # Go through every cartesian product, i.e. every corner in the
-        # hypercube grid points surrounding the observation
-        for cart_prod in itertools.product(*int_frac):
-            fractions = (frac for (integral, frac) in cart_prod)
-            integrals = list(integral for (integral, frac) in cart_prod)
-            # Find the index in the resulting array, compured by
-            # x_1 * (g_2 * g_3 * g_4) + x_2 * (g_3 * g_4) + x_3 * (g_4) + x_4
-
-            index = integrals[0]
-            for j in range(1, dims):
-                index = grid_num[j] * index + integrals[j]
-
-            value = functools.reduce(operator.mul, fractions)
-            result[index % obs_tot] += value * weight
-
-    assert np.allclose(np.sum(result), 1)
-    return result
-
-
-def linbin_Ndim(data, grid_points, weights=None):
-    """
-    d-dimensional linear binning, when d >= 2.
-
-    With :math:`N` data points, and :math:`n` grid points in each dimension
-    :math:`d`, the running time is :math:`O(N2^d)`. For each point the
-    algorithm finds the nearest points, of which there are two in each
-    dimension. Approximately 200 times faster than pure Python implementation.
-
-    Parameters
-    ----------
-    data : array-like
-        The data must be of shape (obs, dims).
-    grid_points : array-like
-        Grid, where cartesian product is already performed.
-    weights : array-like
-        Must have shape (obs,).
-
-    Examples
-    --------
-    >>> from KDEpy.utils import autogrid
-    >>> grid_points = autogrid(np.array([[0, 0, 0]]), num_points=(3, 3, 3))
-    >>> d = linbin_Ndim(np.array([[1.0, 0, 0]]), grid_points, None)
-    """
-    data_obs, data_dims = data.shape
-    assert len(grid_points.shape) == 2
-    assert data_dims >= 2
-
-    # Convert the data and grid points
-    data = np.asarray_chkfinite(data, dtype=float)
-    grid_points = np.asarray_chkfinite(grid_points, dtype=float)
-    if weights is not None:
-        weights = np.asarray_chkfinite(weights, dtype=float)
-        weights = weights / np.sum(weights)
-
-    if (weights is not None) and (data.shape[0] != len(weights)):
-        raise ValueError("Length of data must match length of weights.")
-
-    obs_tot, dims = grid_points.shape
-
-    # Compute the number of grid points for each dimension in the grid
-    grid_num = (grid_points[:, i] for i in range(dims))
-    grid_num = np.array(list(len(np.unique(g)) for g in grid_num))
-
-    # Scale the data to the grid
-    min_grid = np.min(grid_points, axis=0)
-    max_grid = np.max(grid_points, axis=0)
-    num_intervals = grid_num - 1
-    dx = (max_grid - min_grid) / num_intervals
-    data = (data - min_grid) / dx
-
-    # Create results
-    result = np.zeros(grid_points.shape[0], dtype=float)
-
-    # Call the Cython implementation. Loops are unrolled if d=1 or d=2,
-    # and if d >= 3 a more general routine is called. It's a bit slower since
-    # the loops are not unrolled.
-
-    # Weighted data has two specific routines
-    if weights is not None:
-        if data_dims >= 3:
-            binary_flgs = cartesian(([0, 1],) * dims)
-            result = cutils.iterate_data_ND_weighted(data, weights, result, grid_num, obs_tot, binary_flgs)
-        else:
-            result = cutils.iterate_data_2D_weighted(data, weights, result, grid_num, obs_tot)
-        result = np.asarray_chkfinite(result, dtype=float)
-
-    # Unweighted data has two specific routines too. This is because creating
-    # uniform weights takes relatively long time. It's faster to have a
-    # specialize routine for this case.
-    else:
-        if data_dims >= 3:
-            binary_flgs = cartesian(([0, 1],) * dims)
-            result = cutils.iterate_data_ND(data, result, grid_num, obs_tot, binary_flgs)
-        else:
-            result = cutils.iterate_data_2D(data, result, grid_num, obs_tot)
-        result = np.asarray_chkfinite(result, dtype=float)
-        result = result / data_obs
-
-    assert np.allclose(np.sum(result), 1)
-    return result
-
-
-def linear_binning(data, grid_points, weights=None):
-    """
-    This wrapper function computes d-dimensional binning, very quickly.
-
-    Computes binning by setting a linear grid and weighting points linearily
-    by their distance to the grid points. In addition, weight asssociated with
-    data points may be passed. Depending on whether or not weights are passed
-    and the dimensionality of the data, specific sub-routines are called for
-    fast evaluation.
-
-    Parameters
-    ----------
-    data
-        The data points.
-    grid_points
-        The number of points in the grid.
-    weights
-        The weights.
-
-    Returns
-    -------
-    (grid, data)
-        Data weighted at each grid point.
-
-    Examples
-    --------
-    >>> data = [1, 1.5, 1.5, 2, 2.8, 3]
-    >>> grid_points = [1, 2, 3]
-    >>> data = linear_binning(data, grid_points)
-    >>> np.allclose(data, np.array([0.33333, 0.36667, 0.3]))
-    True
-    """
-    data = np.asarray_chkfinite(data, dtype=float)
-    grid_points = np.asarray_chkfinite(grid_points, dtype=float)
-    if weights is not None:
-        weights = np.asarray_chkfinite(weights, dtype=float)
-
-    # Make sure the dimensionality makes sense
-    try:
-        data_obs, data_dims = data.shape
-    except ValueError:
-        data_dims = 1
-
-    try:
-        grid_obs, grid_dims = grid_points.shape
-    except ValueError:
-        grid_dims = 1
-
-    if not data_dims == grid_dims:
-        raise ValueError("Shape of data and grid points must be the same.")
-
-    if data_dims == 1:
-        if _use_Cython:
-            return linbin_cython(data.ravel(), grid_points.ravel(), weights=weights)
-        else:
-            return linbin_numpy(data.ravel(), grid_points.ravel(), weights=weights)
-    else:
-        return linbin_Ndim(data, grid_points, weights=weights)
-
-
-if __name__ == "__main__":
-    import pytest
-
-    # --durations=10  <- May be used to show potentially slow tests
-    pytest.main(args=[".", "--doctest-modules", "-v", "--capture=sys"])
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Module for functions related to linear binning. These functions perform
+linear binning on weighted data. This is typically a preprocessing step
+before convolving with a kernel in the FFTKDE, but may also be used to
+reduce the effective number of data points in any algorithm.
+
+The idea behind linear binning is the following: (1) go through every
+data point and (2) assign a weight to the 2^dims nearest grid points.
+In `dims` dimensions, there are 2 points on the grid to consider in
+each dimension, so a total of 2^dims grid points must be assigned weights to
+for every data point. The weights are determined by the proportion of
+the volume of this hypercube that is enclosed by the data point.
+
+A ------------------------------ B
+|                    |           |
+|                    |           |
+|                    X-----------|
+|                                |
+|                                |
+|                                |
+C ------------------------------ C
+
+References
+----------
+- Fan, Jianqing, and James S. Marron.
+  “Fast Implementations of Nonparametric Curve Estimators.”
+  Journal of Computational and Graphical Statistics 3, no. 1 (March 1, 1994).
+  https://doi.org/10.1080/10618600.1994.10474629.
+"""
+import functools
+import itertools
+import operator
+
+import numpy as np
+
+import cutils
+from KDEpy.utils import cartesian
+
+grid_is_sorted = cutils.grid_is_sorted
+
+# This parameter was in use when a NumPy implementation and a Cython
+# implementation were both used. Now only Cython is used.
+_use_Cython = True
+
+
+def linbin_cython(data, grid_points, weights=None):
+    """
+    1D Linear binning using Cython. Assigns weights to grid points from data.
+
+    Runs in approx 10 ms on 1 million data points.
+
+    Parameters
+    ----------
+    data : array-like
+        The data to bin. Must be of shape (obs,).
+    grid_points : array-like
+        Equidistant grid points to assign weights to.
+        Must be of shape (points,).
+    weights : array-like
+        The weights of the data points.
+        Must be of shape (obs,).
+
+    Examples
+    --------
+    >>> data = np.array([2, 2.5, 3, 4])
+    >>> ans = linbin_cython(data, np.arange(6), weights=None)
+    >>> np.allclose(ans, np.array([0, 0, 0.375, 0.375, 0.25, 0]))
+    True
+    >>> ans = linbin_cython(data, np.arange(6), weights=np.arange(1, 5))
+    >>> np.allclose(ans, np.array([0, 0, 0.2, 0.4, 0.4, 0]))
+    True
+    >>> data = np.array([2, 2.5, 3, 4])
+    >>> ans = linbin_cython(data, np.arange(1, 7), weights=None)
+    >>> np.allclose(ans, np.array([0, 0.375, 0.375, 0.25, 0, 0]))
+    True
+    """
+    # Convert the data and grid points
+    data = np.asarray_chkfinite(data, dtype=float)
+    grid_points = np.asarray_chkfinite(grid_points, dtype=float)
+
+    assert len(data.shape) == 1
+    assert len(grid_points.shape) == 1
+
+    # Verify that the grid is equidistant
+    diffs = np.diff(grid_points)
+    assert np.allclose(np.ones_like(diffs) * diffs[0], diffs)
+
+    if weights is not None:
+        assert len(weights.shape) == 1
+        weights = np.asarray_chkfinite(weights, dtype=float)
+        weights = weights / np.sum(weights)
+
+    if (weights is not None) and (len(data) != len(weights)):
+        raise ValueError("Length of data must match length of weights.")
+
+    # Transform the data
+    min_grid = np.min(grid_points)
+    max_grid = np.max(grid_points)
+    num_intervals = len(grid_points) - 1  # Number of intervals
+    dx = (max_grid - min_grid) / num_intervals
+    transformed_data = (data - min_grid) / dx
+
+    result = np.asfarray(np.zeros(num_intervals + 2))
+
+    # Two Cython functions are implemented, one for weighted data and one
+    # for unweighted data, since creating equal weights is costly w.r.t time
+    if weights is None:
+        result = cutils.iterate_data_1D(transformed_data, result)
+        return np.asfarray(result[:-1]) / transformed_data.shape[0]
+    else:
+        res = cutils.iterate_data_1D_weighted(transformed_data, weights, result)
+        return np.asfarray(res[:-1])  # Remove last, outside of grid
+
+
+def linbin_numpy(data, grid_points, weights=None):
+    """
+    1D Linear binning using NumPy. Assigns weights to grid points from data.
+
+    This function is fast for data sets upto approximately 1-10 million,
+    it uses vectorized NumPy functions to perform linear binning. Takes around
+    100 ms on 1 million data points, so not nearly as fast as the Cython
+    implementation (10 ms).
+
+    Parameters
+    ----------
+    data : array-like
+        Must be of shape (obs,).
+    grid_points : array-like
+        Must be of shape (points,).
+    weights : array-like
+        Must be of shape (obs,).
+
+    Examples
+    --------
+    >>> data = np.array([2, 2.5, 3, 4])
+    >>> ans = linbin_numpy(data, np.arange(6), weights=None)
+    >>> np.allclose(ans, np.array([0, 0, 0.375, 0.375, 0.25, 0]))
+    True
+    >>> ans = linbin_numpy(data, np.arange(6), weights=np.arange(1, 5))
+    >>> np.allclose(ans, np.array([0, 0, 0.2, 0.4, 0.4, 0]))
+    True
+    >>> data = np.array([2, 2.5, 3, 4])
+    >>> ans = linbin_numpy(data, np.arange(1, 7), weights=None)
+    >>> np.allclose(ans, np.array([0, 0.375, 0.375, 0.25, 0, 0]))
+    True
+    """
+    # Convert the data and grid points
+    data = np.asarray_chkfinite(data, dtype=float)
+    grid_points = np.asarray_chkfinite(grid_points, dtype=float)
+    assert len(data.shape) == 1
+    assert len(grid_points.shape) == 1
+
+    # Verify that the grid is equidistant
+    diffs = np.diff(grid_points)
+    assert np.allclose(np.ones_like(diffs) * diffs[0], diffs)
+
+    if weights is None:
+        weights = np.ones_like(data)
+
+    weights = np.asarray_chkfinite(weights, dtype=float)
+    weights = weights / np.sum(weights)
+
+    if not len(data) == len(weights):
+        raise ValueError("Length of data must match length of weights.")
+
+    # Transform the data
+    min_grid = np.min(grid_points)
+    max_grid = np.max(grid_points)
+    num_intervals = len(grid_points) - 1
+    dx = (max_grid - min_grid) / num_intervals
+    transformed_data = (data - min_grid) / dx
+
+    # Compute the integral and fractional part of the data
+    # The integral part is used for lookups, the fractional part is used
+    # to weight the data
+    fractional, integral = np.modf(transformed_data)
+    integral = integral.astype(int)
+
+    # Sort the integral values, and the fractional data and weights by
+    # the same key. This lets us use binary search, which is faster
+    # than using a mask in the the loop below
+    indices_sorted = np.argsort(integral)
+    integral = integral[indices_sorted]
+    fractional = fractional[indices_sorted]
+    weights = weights[indices_sorted]
+
+    # Pre-compute these products, as they are used in the loop many times
+    frac_weights = fractional * weights
+    neg_frac_weights = weights - frac_weights
+
+    # If the data is not a subset of the grid, the integral values will be
+    # outside of the grid. To solve the problem, we filter these values away
+    unique_integrals = np.unique(integral)
+    unique_integrals = unique_integrals[(unique_integrals >= 0) & (unique_integrals <= len(grid_points))]
+
+    result = np.asfarray(np.zeros(len(grid_points) + 1))
+    for grid_point in unique_integrals:
+        # Use binary search to find indices for the grid point
+        # Then sum the data assigned to that grid point
+        low_index = np.searchsorted(integral, grid_point, side="left")
+        high_index = np.searchsorted(integral, grid_point, side="right")
+        result[grid_point] += neg_frac_weights[low_index:high_index].sum()
+        result[grid_point + 1] += frac_weights[low_index:high_index].sum()
+
+    return result[:-1]
+
+
+def linbin_Ndim_python(data, grid_points, weights=None):
+    """
+    d-dimensional linear binning. This is a slow, pure-Python function.
+    Mainly used for testing purposes.
+
+    With :math:`N` data points, and :math:`n` grid points in each dimension
+    :math:`d`, the running time is :math:`O(N2^d)`. For each point the
+    algorithm finds the nearest points, of which there are two in each
+    dimension.
+
+    Parameters
+    ----------
+    data : array-like
+        The data must be of shape (obs, dims).
+    grid_points : array-like
+        Grid, where cartesian product is already performed.
+    weights : array-like
+        Must have shape (obs,).
+
+    Examples
+    --------
+    >>> from KDEpy.utils import autogrid
+    >>> grid_points = autogrid(np.array([[0, 0, 0]]), num_points=(3, 3, 3))
+    >>> d = linbin_Ndim_python(np.array([[1.0, 0, 0]]), grid_points, None)
+    """
+    # Convert the data and grid points
+    data = np.asarray_chkfinite(data, dtype=float)
+    grid_points = np.asarray_chkfinite(grid_points, dtype=float)
+    if weights is not None:
+        weights = np.asarray_chkfinite(weights, dtype=float)
+    else:
+        # This is not efficient, but this function should just be correct
+        # The faster algorithm is implemented in Cython
+        weights = np.ones(data.shape[0])
+    weights = weights / np.sum(weights)
+
+    if (weights is not None) and (data.shape[0] != len(weights)):
+        raise ValueError("Length of data must match length of weights.")
+
+    obs_tot, dims = grid_points.shape
+
+    # Compute the number of grid points for each dimension in the grid
+    grid_num = (grid_points[:, i] for i in range(dims))
+    grid_num = np.array(list(len(np.unique(g)) for g in grid_num))
+
+    # Scale the data to the grid
+    min_grid = np.min(grid_points, axis=0)
+    max_grid = np.max(grid_points, axis=0)
+    num_intervals = grid_num - 1  # Number of intervals
+    dx = (max_grid - min_grid) / num_intervals
+    data = (data - min_grid) / dx
+
+    # Create results
+    result = np.zeros(grid_points.shape[0], dtype=float)
+
+    # Go through every data point
+    for observation, weight in zip(data, weights):
+        # Compute integer part and fractional part for every x_i
+        # Compute relation to previous grid point, and next grid point
+        int_frac = (
+            (
+                (int(coordinate), 1 - (coordinate % 1)),
+                (int(coordinate) + 1, (coordinate % 1)),
+            )
+            for coordinate in observation
+        )
+
+        # Go through every cartesian product, i.e. every corner in the
+        # hypercube grid points surrounding the observation
+        for cart_prod in itertools.product(*int_frac):
+            fractions = (frac for (integral, frac) in cart_prod)
+            integrals = list(integral for (integral, frac) in cart_prod)
+            # Find the index in the resulting array, compured by
+            # x_1 * (g_2 * g_3 * g_4) + x_2 * (g_3 * g_4) + x_3 * (g_4) + x_4
+
+            index = integrals[0]
+            for j in range(1, dims):
+                index = grid_num[j] * index + integrals[j]
+
+            value = functools.reduce(operator.mul, fractions)
+            result[index % obs_tot] += value * weight
+
+    assert np.allclose(np.sum(result), 1)
+    return result
+
+
+def linbin_Ndim(data, grid_points, weights=None):
+    """
+    d-dimensional linear binning, when d >= 2.
+
+    With :math:`N` data points, and :math:`n` grid points in each dimension
+    :math:`d`, the running time is :math:`O(N2^d)`. For each point the
+    algorithm finds the nearest points, of which there are two in each
+    dimension. Approximately 200 times faster than pure Python implementation.
+
+    Parameters
+    ----------
+    data : array-like
+        The data must be of shape (obs, dims).
+    grid_points : array-like
+        Grid, where cartesian product is already performed.
+    weights : array-like
+        Must have shape (obs,).
+
+    Examples
+    --------
+    >>> from KDEpy.utils import autogrid
+    >>> grid_points = autogrid(np.array([[0, 0, 0]]), num_points=(3, 3, 3))
+    >>> d = linbin_Ndim(np.array([[1.0, 0, 0]]), grid_points, None)
+    """
+    data_obs, data_dims = data.shape
+    assert len(grid_points.shape) == 2
+    assert data_dims >= 2
+
+    # Convert the data and grid points
+    data = np.asarray_chkfinite(data, dtype=float)
+    grid_points = np.asarray_chkfinite(grid_points, dtype=float)
+    if weights is not None:
+        weights = np.asarray_chkfinite(weights, dtype=float)
+        weights = weights / np.sum(weights)
+
+    if (weights is not None) and (data.shape[0] != len(weights)):
+        raise ValueError("Length of data must match length of weights.")
+
+    obs_tot, dims = grid_points.shape
+
+    # Compute the number of grid points for each dimension in the grid
+    grid_num = (grid_points[:, i] for i in range(dims))
+    grid_num = np.array(list(len(np.unique(g)) for g in grid_num))
+
+    # Scale the data to the grid
+    min_grid = np.min(grid_points, axis=0)
+    max_grid = np.max(grid_points, axis=0)
+    num_intervals = grid_num - 1
+    dx = (max_grid - min_grid) / num_intervals
+    data = (data - min_grid) / dx
+
+    # Create results
+    result = np.zeros(grid_points.shape[0], dtype=float)
+
+    # Call the Cython implementation. Loops are unrolled if d=1 or d=2,
+    # and if d >= 3 a more general routine is called. It's a bit slower since
+    # the loops are not unrolled.
+
+    # Weighted data has two specific routines
+    if weights is not None:
+        if data_dims >= 3:
+            binary_flgs = cartesian(([0, 1],) * dims)
+            result = cutils.iterate_data_ND_weighted(data, weights, result, grid_num, obs_tot, binary_flgs)
+        else:
+            result = cutils.iterate_data_2D_weighted(data, weights, result, grid_num, obs_tot)
+        result = np.asarray_chkfinite(result, dtype=float)
+
+    # Unweighted data has two specific routines too. This is because creating
+    # uniform weights takes relatively long time. It's faster to have a
+    # specialize routine for this case.
+    else:
+        if data_dims >= 3:
+            binary_flgs = cartesian(([0, 1],) * dims)
+            result = cutils.iterate_data_ND(data, result, grid_num, obs_tot, binary_flgs)
+        else:
+            result = cutils.iterate_data_2D(data, result, grid_num, obs_tot)
+        result = np.asarray_chkfinite(result, dtype=float)
+        result = result / data_obs
+
+    assert np.allclose(np.sum(result), 1)
+    return result
+
+
+def linear_binning(data, grid_points, weights=None):
+    """
+    This wrapper function computes d-dimensional binning, very quickly.
+
+    Computes binning by setting a linear grid and weighting points linearily
+    by their distance to the grid points. In addition, weight asssociated with
+    data points may be passed. Depending on whether or not weights are passed
+    and the dimensionality of the data, specific sub-routines are called for
+    fast evaluation.
+
+    Parameters
+    ----------
+    data
+        The data points.
+    grid_points
+        The number of points in the grid.
+    weights
+        The weights.
+
+    Returns
+    -------
+    (grid, data)
+        Data weighted at each grid point.
+
+    Examples
+    --------
+    >>> data = [1, 1.5, 1.5, 2, 2.8, 3]
+    >>> grid_points = [1, 2, 3]
+    >>> data = linear_binning(data, grid_points)
+    >>> np.allclose(data, np.array([0.33333, 0.36667, 0.3]))
+    True
+    """
+    data = np.asarray_chkfinite(data, dtype=float)
+    grid_points = np.asarray_chkfinite(grid_points, dtype=float)
+    if weights is not None:
+        weights = np.asarray_chkfinite(weights, dtype=float)
+
+    # Make sure the dimensionality makes sense
+    try:
+        data_obs, data_dims = data.shape
+    except ValueError:
+        data_dims = 1
+
+    try:
+        grid_obs, grid_dims = grid_points.shape
+    except ValueError:
+        grid_dims = 1
+
+    if not data_dims == grid_dims:
+        raise ValueError("Shape of data and grid points must be the same.")
+
+    if data_dims == 1:
+        if _use_Cython:
+            return linbin_cython(data.ravel(), grid_points.ravel(), weights=weights)
+        else:
+            return linbin_numpy(data.ravel(), grid_points.ravel(), weights=weights)
+    else:
+        return linbin_Ndim(data, grid_points, weights=weights)
+
+
+if __name__ == "__main__":
+    import pytest
+
+    # --durations=10  <- May be used to show potentially slow tests
+    pytest.main(args=[".", "--doctest-modules", "-v", "--capture=sys"])
```

## KDEpy/bw_selection.py

 * *Ordering differences only*

```diff
@@ -1,301 +1,301 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Functions for bandwidth selection.
-"""
-import warnings
-
-import numpy as np
-import scipy
-from scipy import fftpack
-from scipy.optimize import brentq
-
-from KDEpy.binning import linear_binning
-from KDEpy.utils import autogrid
-
-# Choose the largest available float on the system
-try:
-    FLOAT = scipy.float128
-except AttributeError:
-    FLOAT = np.float64
-
-
-def _fixed_point(t, N, I_sq, a2):
-    r"""
-    Compute the fixed point as described in the paper by Botev et al.
-
-    .. math:
-
-        t = \xi \gamma^{5}(t)
-
-    Parameters
-    ----------
-    t : float
-        Initial guess.
-    N : int
-        Number of data points.
-    I_sq : array-like
-        The numbers [1, 2, 9, 16, ...]
-    a2 : array-like
-        The DCT of the original data, divided by 2 and squared.
-
-    Examples
-    --------
-    >>> # From the matlab code
-    >>> ans = _fixed_point(0.01, 50, np.arange(1, 51), np.arange(1, 51))
-    >>> assert np.allclose(ans, 0.0099076220293967618515)
-    >>> # another
-    >>> ans = _fixed_point(0.07, 25, np.arange(1, 11), np.arange(1, 11))
-    >>> assert np.allclose(ans, 0.068342291525717486795)
-
-    References
-    ----------
-     - Implementation by Daniel B. Smith, PhD, found at
-       https://github.com/Daniel-B-Smith/KDE-for-SciPy/blob/master/kde.py
-    """
-
-    # This is important, as the powers might overflow if not done
-    I_sq = np.asfarray(I_sq, dtype=FLOAT)
-    a2 = np.asfarray(a2, dtype=FLOAT)
-
-    # ell = 7 corresponds to the 5 steps recommended in the paper
-    ell = 7
-
-    # Fast evaluation of |f^l|^2 using the DCT, see Plancherel theorem
-    f = (0.5) * np.pi ** (2 * ell) * np.sum(np.power(I_sq, ell) * a2 * np.exp(-I_sq * np.pi**2 * t))
-
-    # Norm of a function, should never be negative
-    if f <= 0:
-        return -1
-    for s in reversed(range(2, ell)):
-        # This could also be formulated using the double factorial n!!,
-        # but this is faster so and requires an import less
-
-        # Step one: estimate t_s from |f^(s+1)|^2
-        odd_numbers_prod = np.product(np.arange(1, 2 * s + 1, 2, dtype=FLOAT))
-        K0 = odd_numbers_prod / np.sqrt(2 * np.pi)
-        const = (1 + (1 / 2) ** (s + 1 / 2)) / 3
-        time = np.power((2 * const * K0 / (N * f)), (2.0 / (3.0 + 2.0 * s)))
-
-        # Step two: estimate |f^s| from t_s
-        f = (0.5) * np.pi ** (2 * s) * np.sum(np.power(I_sq, s) * a2 * np.exp(-I_sq * np.pi**2 * time))
-
-    # This is the minimizer of the AMISE
-    t_opt = np.power(2 * N * np.sqrt(np.pi) * f, -2.0 / 5)
-
-    # Return the difference between the original t and the optimal value
-    return t - t_opt
-
-
-def _root(function, N, args):
-    """
-    Root finding algorithm. Based on MATLAB implementation by Botev et al.
-
-    >>> # From the matlab code
-    >>> ints = np.arange(1, 51)
-    >>> ans = _root(_fixed_point, N=50, args=(50, ints, ints))
-    >>> np.allclose(ans, 9.237610787616029e-05)
-    True
-    """
-    # From the implementation by Botev, the original paper author
-    # Rule of thumb of obtaining a feasible solution
-    N = max(min(1050, N), 50)
-    tol = 10e-12 + 0.01 * (N - 50) / 1000
-    # While a solution is not found, increase the tolerance and try again
-    found = 0
-    while found == 0:
-        try:
-            # Other viable solvers include: [brentq, brenth, ridder, bisect]
-            x, res = brentq(function, 0, tol, args=args, full_output=True, disp=False)
-            found = 1 if res.converged else 0
-        except ValueError:
-            x = 0
-            tol *= 2.0
-            found = 0
-        if x <= 0:
-            found = 0
-
-        # If the tolerance grows too large, minimize the function
-        if tol >= 1:
-            raise ValueError("Root finding did not converge. Need more data.")
-
-    if not x > 0:
-        raise ValueError("Root finding failed to find positive solution.")
-    return x
-
-
-def improved_sheather_jones(data, weights=None):
-    """
-    The Improved Sheater Jones (ISJ) algorithm from the paper by Botev et al.
-    This algorithm computes the optimal bandwidth for a gaussian kernel,
-    and works very well for bimodal data (unlike other rules). The
-    disadvantage of this algorithm is longer computation time, and the fact
-    that this implementation does not always converge if very few data
-    points are supplied.
-
-    Understanding this algorithm is difficult, see:
-    https://books.google.no/books?id=Trj9HQ7G8TUC&pg=PA328&lpg=PA328&dq=
-    sheather+jones+why+use+dct&source=bl&ots=1ETdKd_6EF&sig=jZk4R515GB1xsn-
-    VZVnjr-JfjSI&hl=en&sa=X&ved=2ahUKEwi1_czNncTcAhVGhqYKHaPiBtcQ6AEwA3oEC
-    AcQAQ#v=onepage&q=sheather%20jones%20why%20use%20dct&f=false
-
-    Parameters
-    ----------
-    data: array-like
-        The data points. Data must have shape (obs, 1).
-    weights: array-like, optional
-        One weight per data point. Must have shape (obs,). If None is
-        passed, uniform weights are used.
-    """
-    obs, dims = data.shape
-    if not dims == 1:
-        raise ValueError("ISJ is only available for 1D data.")
-
-    n = 2**10
-
-    # weights <= 0 still affect calculations unless we remove them
-    if weights is not None:
-        data = data[weights > 0]
-        weights = weights[weights > 0]
-
-    # Setting `percentile` higher decreases the chance of overflow
-    xmesh = autogrid(data, boundary_abs=6, num_points=n, boundary_rel=0.5)
-    data = data.ravel()
-    xmesh = xmesh.ravel()
-
-    # Create an equidistant grid
-    R = np.max(data) - np.min(data)
-    # dx = R / (n - 1)
-    data = data.ravel()
-    N = len(np.unique(data))
-
-    # Use linear binning to bin the data on an equidistant grid, this is a
-    # prerequisite for using the FFT (evenly spaced samples)
-    initial_data = linear_binning(data.reshape(-1, 1), xmesh, weights)
-    assert np.allclose(initial_data.sum(), 1)
-
-    # Compute the type 2 Discrete Cosine Transform (DCT) of the data
-    a = fftpack.dct(initial_data)
-
-    # Compute the bandwidth
-    # The definition of a2 used here and in `_fixed_point` correspond to
-    # the one cited in this issue:
-    # https://github.com/tommyod/KDEpy/issues/95
-    I_sq = np.power(np.arange(1, n, dtype=FLOAT), 2)
-    a2 = a[1:] ** 2
-
-    # Solve for the optimal (in the AMISE sense) t
-    t_star = _root(_fixed_point, N, args=(N, I_sq, a2))
-
-    # The remainder of the algorithm computes the actual density
-    # estimate, but this function is only used to compute the
-    # bandwidth, since the bandwidth may be used for other kernels
-    # apart from the Gaussian kernel
-
-    # Smooth the initial data using the computed optimal t
-    # Multiplication in frequency domain is convolution
-    # integers = np.arange(n, dtype=float)
-    # a_t = a * np.exp(-integers**2 * np.pi ** 2 * t_star / 2)
-
-    # Diving by 2 done because of the implementation of fftpack.idct
-    # density = fftpack.idct(a_t) / (2 * R)
-
-    # Due to overflow, some values might be smaller than zero, correct it
-    # density[density < 0] = 0.
-    bandwidth = np.sqrt(t_star) * R
-    return bandwidth
-
-
-def scotts_rule(data, weights=None):
-    """
-    Scotts rule.
-
-    Scott (1992, page 152)
-    Scott, D.W. (1992) Multivariate Density Estimation. Theory, Practice and
-    Visualization. New York: Wiley.
-
-    Examples
-    --------
-    >>> data = np.arange(9).reshape(-1, 1)
-    >>> ans = scotts_rule(data)
-    >>> assert np.allclose(ans, 1.76474568962182)
-    """
-    if not len(data.shape) == 2:
-        raise ValueError("Data must be of shape (obs, dims).")
-
-    if weights is not None:
-        warnings.warn("Scott's rule currently ignores all weights")
-
-    obs, dims = data.shape
-    if not dims == 1:
-        raise ValueError("Scotts rule is only available for 1D data.")
-    sigma = np.std(data, ddof=1)
-    # scipy.norm.ppf(.75) - scipy.norm.ppf(.25) -> 1.3489795003921634
-    IQR = (np.percentile(data, q=75) - np.percentile(data, q=25)) / 1.3489795003921634
-
-    sigma = min(sigma, IQR)
-    return sigma * np.power(obs, -1.0 / (dims + 4))
-
-
-def silvermans_rule(data, weights=None):
-    """
-    Returns optimal smoothing (standard deviation) if the data is close to
-    normal.
-
-    TODO: Extend to multidimensional:
-        https://docs.scipy.org/doc/scipy-0.13.0/reference/generated/scipy.
-        stats.gaussian_kde.html#r216
-
-    Examples
-    --------
-    >>> data = np.arange(9).reshape(-1, 1)
-    >>> ans = silvermans_rule(data)
-    >>> assert np.allclose(ans, 1.8692607078355594)
-    """
-    if not len(data.shape) == 2:
-        raise ValueError("Data must be of shape (obs, dims).")
-    obs, dims = data.shape
-    if not dims == 1:
-        raise ValueError("Silverman's rule is only available for 1D data.")
-
-    if weights is not None:
-        warnings.warn("Silverman's rule currently ignores all weights")
-
-    if obs == 1:
-        return 1
-    if obs < 1:
-        raise ValueError("Data must be of length > 0.")
-
-    sigma = np.std(data, ddof=1)
-    # scipy.stats.norm.ppf(.75) - scipy.stats.norm.ppf(.25) -> 1.3489795003921634
-    IQR = (np.percentile(data, q=75) - np.percentile(data, q=25)) / 1.3489795003921634
-
-    sigma = min(sigma, IQR)
-
-    # The logic below is not related to silverman's rule, but if the data is constant
-    # it's nice to return a value instead of getting an error. A warning will be raised.
-    if sigma > 0:
-        return sigma * (obs * 3 / 4.0) ** (-1 / 5)
-    else:
-        # stats.norm.ppf(.99) - stats.norm.ppf(.01) = 4.6526957480816815
-        IQR = (np.percentile(data, q=99) - np.percentile(data, q=1)) / 4.6526957480816815
-        if IQR > 0:
-            bw = IQR * (obs * 3 / 4.0) ** (-1 / 5)
-            warnings.warn(
-                "Silverman's rule failed. Too many idential values. \
-Setting bw = {}".format(
-                    bw
-                )
-            )
-            return bw
-
-        # Here, all values are basically constant
-        warnings.warn("Silverman's rule failed. Too many idential values. Setting bw = 1.0")
-        return 1.0
-
-
-_bw_methods = {
-    "silverman": silvermans_rule,
-    "scott": scotts_rule,
-    "ISJ": improved_sheather_jones,
-}
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Functions for bandwidth selection.
+"""
+import warnings
+
+import numpy as np
+import scipy
+from scipy import fftpack
+from scipy.optimize import brentq
+
+from KDEpy.binning import linear_binning
+from KDEpy.utils import autogrid
+
+# Choose the largest available float on the system
+try:
+    FLOAT = scipy.float128
+except AttributeError:
+    FLOAT = np.float64
+
+
+def _fixed_point(t, N, I_sq, a2):
+    r"""
+    Compute the fixed point as described in the paper by Botev et al.
+
+    .. math:
+
+        t = \xi \gamma^{5}(t)
+
+    Parameters
+    ----------
+    t : float
+        Initial guess.
+    N : int
+        Number of data points.
+    I_sq : array-like
+        The numbers [1, 2, 9, 16, ...]
+    a2 : array-like
+        The DCT of the original data, divided by 2 and squared.
+
+    Examples
+    --------
+    >>> # From the matlab code
+    >>> ans = _fixed_point(0.01, 50, np.arange(1, 51), np.arange(1, 51))
+    >>> assert np.allclose(ans, 0.0099076220293967618515)
+    >>> # another
+    >>> ans = _fixed_point(0.07, 25, np.arange(1, 11), np.arange(1, 11))
+    >>> assert np.allclose(ans, 0.068342291525717486795)
+
+    References
+    ----------
+     - Implementation by Daniel B. Smith, PhD, found at
+       https://github.com/Daniel-B-Smith/KDE-for-SciPy/blob/master/kde.py
+    """
+
+    # This is important, as the powers might overflow if not done
+    I_sq = np.asfarray(I_sq, dtype=FLOAT)
+    a2 = np.asfarray(a2, dtype=FLOAT)
+
+    # ell = 7 corresponds to the 5 steps recommended in the paper
+    ell = 7
+
+    # Fast evaluation of |f^l|^2 using the DCT, see Plancherel theorem
+    f = (0.5) * np.pi ** (2 * ell) * np.sum(np.power(I_sq, ell) * a2 * np.exp(-I_sq * np.pi**2 * t))
+
+    # Norm of a function, should never be negative
+    if f <= 0:
+        return -1
+    for s in reversed(range(2, ell)):
+        # This could also be formulated using the double factorial n!!,
+        # but this is faster so and requires an import less
+
+        # Step one: estimate t_s from |f^(s+1)|^2
+        odd_numbers_prod = np.product(np.arange(1, 2 * s + 1, 2, dtype=FLOAT))
+        K0 = odd_numbers_prod / np.sqrt(2 * np.pi)
+        const = (1 + (1 / 2) ** (s + 1 / 2)) / 3
+        time = np.power((2 * const * K0 / (N * f)), (2.0 / (3.0 + 2.0 * s)))
+
+        # Step two: estimate |f^s| from t_s
+        f = (0.5) * np.pi ** (2 * s) * np.sum(np.power(I_sq, s) * a2 * np.exp(-I_sq * np.pi**2 * time))
+
+    # This is the minimizer of the AMISE
+    t_opt = np.power(2 * N * np.sqrt(np.pi) * f, -2.0 / 5)
+
+    # Return the difference between the original t and the optimal value
+    return t - t_opt
+
+
+def _root(function, N, args):
+    """
+    Root finding algorithm. Based on MATLAB implementation by Botev et al.
+
+    >>> # From the matlab code
+    >>> ints = np.arange(1, 51)
+    >>> ans = _root(_fixed_point, N=50, args=(50, ints, ints))
+    >>> np.allclose(ans, 9.237610787616029e-05)
+    True
+    """
+    # From the implementation by Botev, the original paper author
+    # Rule of thumb of obtaining a feasible solution
+    N = max(min(1050, N), 50)
+    tol = 10e-12 + 0.01 * (N - 50) / 1000
+    # While a solution is not found, increase the tolerance and try again
+    found = 0
+    while found == 0:
+        try:
+            # Other viable solvers include: [brentq, brenth, ridder, bisect]
+            x, res = brentq(function, 0, tol, args=args, full_output=True, disp=False)
+            found = 1 if res.converged else 0
+        except ValueError:
+            x = 0
+            tol *= 2.0
+            found = 0
+        if x <= 0:
+            found = 0
+
+        # If the tolerance grows too large, minimize the function
+        if tol >= 1:
+            raise ValueError("Root finding did not converge. Need more data.")
+
+    if not x > 0:
+        raise ValueError("Root finding failed to find positive solution.")
+    return x
+
+
+def improved_sheather_jones(data, weights=None):
+    """
+    The Improved Sheater Jones (ISJ) algorithm from the paper by Botev et al.
+    This algorithm computes the optimal bandwidth for a gaussian kernel,
+    and works very well for bimodal data (unlike other rules). The
+    disadvantage of this algorithm is longer computation time, and the fact
+    that this implementation does not always converge if very few data
+    points are supplied.
+
+    Understanding this algorithm is difficult, see:
+    https://books.google.no/books?id=Trj9HQ7G8TUC&pg=PA328&lpg=PA328&dq=
+    sheather+jones+why+use+dct&source=bl&ots=1ETdKd_6EF&sig=jZk4R515GB1xsn-
+    VZVnjr-JfjSI&hl=en&sa=X&ved=2ahUKEwi1_czNncTcAhVGhqYKHaPiBtcQ6AEwA3oEC
+    AcQAQ#v=onepage&q=sheather%20jones%20why%20use%20dct&f=false
+
+    Parameters
+    ----------
+    data: array-like
+        The data points. Data must have shape (obs, 1).
+    weights: array-like, optional
+        One weight per data point. Must have shape (obs,). If None is
+        passed, uniform weights are used.
+    """
+    obs, dims = data.shape
+    if not dims == 1:
+        raise ValueError("ISJ is only available for 1D data.")
+
+    n = 2**10
+
+    # weights <= 0 still affect calculations unless we remove them
+    if weights is not None:
+        data = data[weights > 0]
+        weights = weights[weights > 0]
+
+    # Setting `percentile` higher decreases the chance of overflow
+    xmesh = autogrid(data, boundary_abs=6, num_points=n, boundary_rel=0.5)
+    data = data.ravel()
+    xmesh = xmesh.ravel()
+
+    # Create an equidistant grid
+    R = np.max(data) - np.min(data)
+    # dx = R / (n - 1)
+    data = data.ravel()
+    N = len(np.unique(data))
+
+    # Use linear binning to bin the data on an equidistant grid, this is a
+    # prerequisite for using the FFT (evenly spaced samples)
+    initial_data = linear_binning(data.reshape(-1, 1), xmesh, weights)
+    assert np.allclose(initial_data.sum(), 1)
+
+    # Compute the type 2 Discrete Cosine Transform (DCT) of the data
+    a = fftpack.dct(initial_data)
+
+    # Compute the bandwidth
+    # The definition of a2 used here and in `_fixed_point` correspond to
+    # the one cited in this issue:
+    # https://github.com/tommyod/KDEpy/issues/95
+    I_sq = np.power(np.arange(1, n, dtype=FLOAT), 2)
+    a2 = a[1:] ** 2
+
+    # Solve for the optimal (in the AMISE sense) t
+    t_star = _root(_fixed_point, N, args=(N, I_sq, a2))
+
+    # The remainder of the algorithm computes the actual density
+    # estimate, but this function is only used to compute the
+    # bandwidth, since the bandwidth may be used for other kernels
+    # apart from the Gaussian kernel
+
+    # Smooth the initial data using the computed optimal t
+    # Multiplication in frequency domain is convolution
+    # integers = np.arange(n, dtype=float)
+    # a_t = a * np.exp(-integers**2 * np.pi ** 2 * t_star / 2)
+
+    # Diving by 2 done because of the implementation of fftpack.idct
+    # density = fftpack.idct(a_t) / (2 * R)
+
+    # Due to overflow, some values might be smaller than zero, correct it
+    # density[density < 0] = 0.
+    bandwidth = np.sqrt(t_star) * R
+    return bandwidth
+
+
+def scotts_rule(data, weights=None):
+    """
+    Scotts rule.
+
+    Scott (1992, page 152)
+    Scott, D.W. (1992) Multivariate Density Estimation. Theory, Practice and
+    Visualization. New York: Wiley.
+
+    Examples
+    --------
+    >>> data = np.arange(9).reshape(-1, 1)
+    >>> ans = scotts_rule(data)
+    >>> assert np.allclose(ans, 1.76474568962182)
+    """
+    if not len(data.shape) == 2:
+        raise ValueError("Data must be of shape (obs, dims).")
+
+    if weights is not None:
+        warnings.warn("Scott's rule currently ignores all weights")
+
+    obs, dims = data.shape
+    if not dims == 1:
+        raise ValueError("Scotts rule is only available for 1D data.")
+    sigma = np.std(data, ddof=1)
+    # scipy.norm.ppf(.75) - scipy.norm.ppf(.25) -> 1.3489795003921634
+    IQR = (np.percentile(data, q=75) - np.percentile(data, q=25)) / 1.3489795003921634
+
+    sigma = min(sigma, IQR)
+    return sigma * np.power(obs, -1.0 / (dims + 4))
+
+
+def silvermans_rule(data, weights=None):
+    """
+    Returns optimal smoothing (standard deviation) if the data is close to
+    normal.
+
+    TODO: Extend to multidimensional:
+        https://docs.scipy.org/doc/scipy-0.13.0/reference/generated/scipy.
+        stats.gaussian_kde.html#r216
+
+    Examples
+    --------
+    >>> data = np.arange(9).reshape(-1, 1)
+    >>> ans = silvermans_rule(data)
+    >>> assert np.allclose(ans, 1.8692607078355594)
+    """
+    if not len(data.shape) == 2:
+        raise ValueError("Data must be of shape (obs, dims).")
+    obs, dims = data.shape
+    if not dims == 1:
+        raise ValueError("Silverman's rule is only available for 1D data.")
+
+    if weights is not None:
+        warnings.warn("Silverman's rule currently ignores all weights")
+
+    if obs == 1:
+        return 1
+    if obs < 1:
+        raise ValueError("Data must be of length > 0.")
+
+    sigma = np.std(data, ddof=1)
+    # scipy.stats.norm.ppf(.75) - scipy.stats.norm.ppf(.25) -> 1.3489795003921634
+    IQR = (np.percentile(data, q=75) - np.percentile(data, q=25)) / 1.3489795003921634
+
+    sigma = min(sigma, IQR)
+
+    # The logic below is not related to silverman's rule, but if the data is constant
+    # it's nice to return a value instead of getting an error. A warning will be raised.
+    if sigma > 0:
+        return sigma * (obs * 3 / 4.0) ** (-1 / 5)
+    else:
+        # stats.norm.ppf(.99) - stats.norm.ppf(.01) = 4.6526957480816815
+        IQR = (np.percentile(data, q=99) - np.percentile(data, q=1)) / 4.6526957480816815
+        if IQR > 0:
+            bw = IQR * (obs * 3 / 4.0) ** (-1 / 5)
+            warnings.warn(
+                "Silverman's rule failed. Too many idential values. \
+Setting bw = {}".format(
+                    bw
+                )
+            )
+            return bw
+
+        # Here, all values are basically constant
+        warnings.warn("Silverman's rule failed. Too many idential values. Setting bw = 1.0")
+        return 1.0
+
+
+_bw_methods = {
+    "silverman": silvermans_rule,
+    "scott": scotts_rule,
+    "ISJ": improved_sheather_jones,
+}
```

## KDEpy/kernel_funcs.py

 * *Ordering differences only*

```diff
@@ -1,360 +1,360 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Module for kernel functions. A kernel function is a radial basis function which
-is everywhere non-negative and whose integral evalutes to unity. Every kernel
-function takes an `x` of shape (obs, dims) and returns a y of shape (obs, 1).
-"""
-
-import collections.abc
-import functools
-import numbers
-
-import numpy as np
-from scipy.optimize import brentq
-from scipy.special import factorial2, gamma
-from scipy.stats import norm
-
-# In R, the following are implemented:
-# "gaussian", "rectangular", "triangular", "epanechnikov",
-# "biweight", "cosine" or "optcosine"
-
-# Wikipedia
-# uniform, trinagular, epanechnikov, quartic,triweight, tricube,
-# gaussian, cosine, logistic, sigmoid, silverman
-
-# All kernel functions take x of shape (obs, dims) and returns (obs, 1)
-# All kernel functions integrate to unity
-
-
-def gauss_integral(n):
-    r"""
-    Solve the integral
-    \int_0^1 exp(-0.5 * x * x) x^n dx
-
-    See
-    https://en.wikipedia.org/wiki/List_of_integrals_of_Gaussian_functions
-
-    Examples
-    --------
-    >>> ans = gauss_integral(3)
-    >>> np.allclose(ans, 2)
-    True
-    >>> ans = gauss_integral(4)
-    >>> np.allclose(ans, 3.75994)
-    True
-    """
-    factor = np.sqrt(np.pi * 2)
-    if n % 2 == 0:
-        return factor * factorial2(n - 1) / 2
-    elif n % 2 == 1:
-        return factor * norm.pdf(0) * factorial2(n - 1)
-    else:
-        raise ValueError("n must be odd or even.")
-
-
-def trig_integral(k):
-    """
-    Returns the solutions to
-    Is(k) = int_0^1 sin(pi * x / 2) x^k dx
-    Ic(k) = int_0^1 cos(pi * x / 2) x^k dx
-    using a recursive formula. Returns a tuple (Is, Ic).
-
-    Examples
-    --------
-    >>> import numpy as np
-    >>> Is, Ic = trig_integral(2) # Verify with solution from WolframAlpha
-    >>> np.allclose([Is, Ic], [0.29454, 0.12060], rtol=10e-5)
-    True
-    """
-
-    Ic = 2 / np.pi
-    Is = 2 / np.pi
-
-    if k <= 0:
-        return Is, Ic
-
-    for i in range(1, k + 1):
-        Ic, Is = (2 / np.pi) * (1 - i * Is), (2 / np.pi) * i * Ic
-
-    return Is, Ic
-
-
-def p_norm(x, p):
-    """
-    The p-norm of an array of shape (obs, dims)
-
-    Examples
-    --------
-    >>> x = np.arange(9).reshape((3, 3))
-    >>> p = 2
-    >>> np.allclose(p_norm(x, p), euclidean_norm(x))
-    True
-    """
-    if np.isinf(p):
-        return infinity_norm(x)
-    elif p == 2:
-        return euclidean_norm(x)
-    elif p == 1:
-        return taxicab_norm(x)
-    return np.power(np.power(np.abs(x), p).sum(axis=1), 1 / p)
-
-
-def euclidean_norm(x):
-    """
-    The 2 norm of an array of shape (obs, dims)
-    """
-    return np.sqrt((x * x).sum(axis=1))
-
-
-def euclidean_norm_sq(x):
-    """
-    The squared 2 norm of an array of shape (obs, dims)
-    """
-    return (x * x).sum(axis=1)
-
-
-def infinity_norm(x):
-    """
-    The infinity norm of an array of shape (obs, dims)
-    """
-    return np.abs(x).max(axis=1)
-
-
-def taxicab_norm(x):
-    """
-    The taxicab norm of an array of shape (obs, dims)
-    """
-    return np.abs(x).sum(axis=1)
-
-
-def volume_unit_ball(d, p=2):
-    """
-    Volume of d-dimensional unit ball under the p-norm. When p=1 this is called
-    a cross-polytype, when p=2 it's called a hypersphere, and when p=infty it's
-    called a hypercube.
-
-    Notes
-    -----
-    See the following paper for a very general result related to this:
-
-    - Wang, Xianfu. “Volumes of Generalized Unit Balls.”
-      Mathematics Magazine 78, no. 5 (2005): 390–95.
-      https://doi.org/10.2307/30044198.
-    """
-    return 2.0**d * gamma(1 + 1 / p) ** d / gamma(1 + d / p)
-
-
-def epanechnikov(x, dims=1):
-    normalization = 2 / (dims + 2)
-    dist_sq = x**2
-    out = np.zeros_like(dist_sq)
-    mask = dist_sq < 1
-    out[mask] = (1 - dist_sq)[mask] / normalization
-    return out
-
-
-def gaussian(x, dims=1):
-    normalization = dims * gauss_integral(dims - 1)
-    dist_sq = x**2
-    return np.exp(-dist_sq / 2) / normalization
-
-
-def box(x, dims=1):
-    normalization = 1
-    out = np.zeros_like(x)
-    mask = x < 1
-    out[mask] = 1 / normalization
-    return out
-
-
-def exponential(x, dims=1):
-    normalization = gamma(dims) * dims
-    return np.exp(-x) / normalization
-
-
-def tri(x, dims=1):
-    normalization = 1 / (dims + 1)
-    out = np.zeros_like(x)
-    mask = x < 1
-    out[mask] = np.maximum(0, 1 - x)[mask] / normalization
-    return out
-
-
-def biweight(x, dims=1):
-    normalization = 8 / ((dims + 2) * (dims + 4))
-    dist_sq = x**2
-    out = np.zeros_like(dist_sq)
-    mask = dist_sq < 1
-    out[mask] = np.maximum(0, (1 - dist_sq) ** 2)[mask] / normalization
-    return out
-
-
-def triweight(x, dims=1):
-    normalization = 48 / ((dims + 2) * (dims + 4) * (dims + 6))
-    dist_sq = x**2
-    out = np.zeros_like(dist_sq)
-    mask = dist_sq < 1
-    out[mask] = np.maximum(0, (1 - dist_sq) ** 3)[mask] / normalization
-    return out
-
-
-def tricube(x, dims=1):
-    normalization = 162 / ((dims + 3) * (dims + 6) * (dims + 9))
-    out = np.zeros_like(x)
-    mask = x < 1
-    out[mask] = np.maximum(0, (1 - x**3) ** 3)[mask] / normalization
-    return out
-
-
-def cosine(x, dims=1):
-    Is, Ic = trig_integral(dims - 1)
-    normalization = Ic
-    out = np.zeros_like(x)
-    mask = x < 1
-    out[mask] = np.cos((np.pi * x) / 2)[mask] / (normalization * dims)
-    return out
-
-
-def logistic(x, dims=1):
-    return 1 / (2 + 2 * np.cosh(x))
-
-
-def sigmoid(x, dims=1):
-    return 1 / (np.pi * np.cosh(x))
-
-
-class Kernel(collections.abc.Callable):
-    def __init__(self, function, var=1, support=3):
-        """
-        Initialize a new kernel function.
-
-        function: callable, numpy.arr -> numpy.arr, should integrate to 1
-        expected_value : peak, typically 0
-        support: support of the function.
-
-        Example
-        -------
-        >>> from scipy.special import gamma
-        >>> # Normalized function of x
-        >>> def exp(x, dims=1):
-        ...     normalization = gamma(dims) * dims
-        ...     return np.exp(-x) / normalization
-        >>> kernel = Kernel(exp, var=4, support=np.inf)
-        >>> # The function is scaled so that the standard deviation (bw) = 1
-        >>> kernel(0, bw=1, norm=2)[0] > kernel(1, bw=1, norm=2)[0]
-        True
-        >>> np.allclose(kernel(np.array([0, 1, 2])), kernel([0, 1, 2]))
-        True
-        >>> np.allclose(kernel(0), kernel([0]))
-        True
-        >>> np.allclose(kernel(0), kernel.evaluate(0))
-        True
-        """
-        self.function = function
-        self.var = var
-        self.finite_support = np.isfinite(support)
-
-        # If the function has finite support, scale the support so that it
-        # corresponds to the support of the function when it is scaled to have
-        # unit variance.
-        self.support = support / np.sqrt(self.var)
-
-    def practical_support(self, bw, atol=10e-5):
-        """
-        Return the support for practical purposes. Used to find a support value
-        for computations for kernel functions without finite (bounded) support.
-        """
-        # If the kernel has finite support, return the support accounting for
-        # the bw
-        if self.finite_support:
-            return self.support * bw
-
-        # If the function does not have finite support, find a practical value
-        else:
-
-            def f(x):
-                return self.evaluate(x, bw=bw) - atol
-
-            try:
-                xtol = 1e-3
-                ans = brentq(f, a=0, b=8 * bw, xtol=xtol, full_output=False)
-                return ans + xtol
-            except ValueError:
-                msg = (
-                    "Unable to solve for support numerically. Use a "
-                    + "kernel with finite support or scale data to smaller bw."
-                )
-                raise ValueError(msg)
-
-    def evaluate(self, x, bw=1, norm=2):
-        """
-        Evaluate the kernel.
-
-        Parameters
-        ----------
-        x : array-like
-            Should have shape (obs, dims).
-        bw : array-like
-            Must have shape (obs, ), or float.
-        """
-
-        # If x is a number, convert it to a length-1 NumPy vector
-        if isinstance(x, numbers.Number):
-            x = np.asarray_chkfinite([x])
-        else:
-            x = np.asarray_chkfinite(x)
-
-        if len(x.shape) == 1:
-            x = x.reshape(-1, 1)
-
-        # Scale the function, such that bw=1 corresponds to the function having
-        # a standard deviation (or variance) equal to 1
-        real_bw = bw / np.sqrt(self.var)
-        obs, dims = x.shape
-
-        # Set the volume function
-        volume_func = functools.partial(volume_unit_ball, p=norm)
-
-        if dims > 1:
-            distances = p_norm(x, norm).ravel()
-        else:
-            distances = np.abs(x).ravel()
-
-        return self.function(distances / real_bw, dims) / ((real_bw**dims) * volume_func(dims))
-
-    __call__ = evaluate
-
-
-gaussian = Kernel(gaussian, var=1, support=np.inf)
-exp = Kernel(exponential, var=2, support=np.inf)
-box = Kernel(box, var=1 / 3, support=1)
-tri = Kernel(tri, var=1 / 6, support=1)
-epa = Kernel(epanechnikov, var=1 / 5, support=1)
-biweight = Kernel(biweight, var=1 / 7, support=1)
-triweight = Kernel(triweight, var=1 / 9, support=1)
-tricube = Kernel(tricube, var=35 / 243, support=1)
-cosine = Kernel(cosine, var=(1 - (8 / np.pi**2)), support=1)
-logistic = Kernel(logistic, var=(np.pi**2 / 3), support=np.inf)
-sigmoid = Kernel(sigmoid, var=(np.pi**2 / 4), support=np.inf)
-
-_kernel_functions = {
-    "gaussian": gaussian,
-    "exponential": exp,
-    "box": box,
-    "tri": tri,
-    "epa": epa,
-    "biweight": biweight,
-    "triweight": triweight,
-    "tricube": tricube,
-    "cosine": cosine,
-    # 'logistic': logistic,
-    # 'sigmoid': sigmoid
-}
-
-
-if __name__ == "__main__" and False:
-    import pytest
-
-    # --durations=10  <- May be used to show potentially slow tests
-    pytest.main(args=[".", "--doctest-modules", "-v"])
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Module for kernel functions. A kernel function is a radial basis function which
+is everywhere non-negative and whose integral evalutes to unity. Every kernel
+function takes an `x` of shape (obs, dims) and returns a y of shape (obs, 1).
+"""
+
+import collections.abc
+import functools
+import numbers
+
+import numpy as np
+from scipy.optimize import brentq
+from scipy.special import factorial2, gamma
+from scipy.stats import norm
+
+# In R, the following are implemented:
+# "gaussian", "rectangular", "triangular", "epanechnikov",
+# "biweight", "cosine" or "optcosine"
+
+# Wikipedia
+# uniform, trinagular, epanechnikov, quartic,triweight, tricube,
+# gaussian, cosine, logistic, sigmoid, silverman
+
+# All kernel functions take x of shape (obs, dims) and returns (obs, 1)
+# All kernel functions integrate to unity
+
+
+def gauss_integral(n):
+    r"""
+    Solve the integral
+    \int_0^1 exp(-0.5 * x * x) x^n dx
+
+    See
+    https://en.wikipedia.org/wiki/List_of_integrals_of_Gaussian_functions
+
+    Examples
+    --------
+    >>> ans = gauss_integral(3)
+    >>> np.allclose(ans, 2)
+    True
+    >>> ans = gauss_integral(4)
+    >>> np.allclose(ans, 3.75994)
+    True
+    """
+    factor = np.sqrt(np.pi * 2)
+    if n % 2 == 0:
+        return factor * factorial2(n - 1) / 2
+    elif n % 2 == 1:
+        return factor * norm.pdf(0) * factorial2(n - 1)
+    else:
+        raise ValueError("n must be odd or even.")
+
+
+def trig_integral(k):
+    """
+    Returns the solutions to
+    Is(k) = int_0^1 sin(pi * x / 2) x^k dx
+    Ic(k) = int_0^1 cos(pi * x / 2) x^k dx
+    using a recursive formula. Returns a tuple (Is, Ic).
+
+    Examples
+    --------
+    >>> import numpy as np
+    >>> Is, Ic = trig_integral(2) # Verify with solution from WolframAlpha
+    >>> np.allclose([Is, Ic], [0.29454, 0.12060], rtol=10e-5)
+    True
+    """
+
+    Ic = 2 / np.pi
+    Is = 2 / np.pi
+
+    if k <= 0:
+        return Is, Ic
+
+    for i in range(1, k + 1):
+        Ic, Is = (2 / np.pi) * (1 - i * Is), (2 / np.pi) * i * Ic
+
+    return Is, Ic
+
+
+def p_norm(x, p):
+    """
+    The p-norm of an array of shape (obs, dims)
+
+    Examples
+    --------
+    >>> x = np.arange(9).reshape((3, 3))
+    >>> p = 2
+    >>> np.allclose(p_norm(x, p), euclidean_norm(x))
+    True
+    """
+    if np.isinf(p):
+        return infinity_norm(x)
+    elif p == 2:
+        return euclidean_norm(x)
+    elif p == 1:
+        return taxicab_norm(x)
+    return np.power(np.power(np.abs(x), p).sum(axis=1), 1 / p)
+
+
+def euclidean_norm(x):
+    """
+    The 2 norm of an array of shape (obs, dims)
+    """
+    return np.sqrt((x * x).sum(axis=1))
+
+
+def euclidean_norm_sq(x):
+    """
+    The squared 2 norm of an array of shape (obs, dims)
+    """
+    return (x * x).sum(axis=1)
+
+
+def infinity_norm(x):
+    """
+    The infinity norm of an array of shape (obs, dims)
+    """
+    return np.abs(x).max(axis=1)
+
+
+def taxicab_norm(x):
+    """
+    The taxicab norm of an array of shape (obs, dims)
+    """
+    return np.abs(x).sum(axis=1)
+
+
+def volume_unit_ball(d, p=2):
+    """
+    Volume of d-dimensional unit ball under the p-norm. When p=1 this is called
+    a cross-polytype, when p=2 it's called a hypersphere, and when p=infty it's
+    called a hypercube.
+
+    Notes
+    -----
+    See the following paper for a very general result related to this:
+
+    - Wang, Xianfu. “Volumes of Generalized Unit Balls.”
+      Mathematics Magazine 78, no. 5 (2005): 390–95.
+      https://doi.org/10.2307/30044198.
+    """
+    return 2.0**d * gamma(1 + 1 / p) ** d / gamma(1 + d / p)
+
+
+def epanechnikov(x, dims=1):
+    normalization = 2 / (dims + 2)
+    dist_sq = x**2
+    out = np.zeros_like(dist_sq)
+    mask = dist_sq < 1
+    out[mask] = (1 - dist_sq)[mask] / normalization
+    return out
+
+
+def gaussian(x, dims=1):
+    normalization = dims * gauss_integral(dims - 1)
+    dist_sq = x**2
+    return np.exp(-dist_sq / 2) / normalization
+
+
+def box(x, dims=1):
+    normalization = 1
+    out = np.zeros_like(x)
+    mask = x < 1
+    out[mask] = 1 / normalization
+    return out
+
+
+def exponential(x, dims=1):
+    normalization = gamma(dims) * dims
+    return np.exp(-x) / normalization
+
+
+def tri(x, dims=1):
+    normalization = 1 / (dims + 1)
+    out = np.zeros_like(x)
+    mask = x < 1
+    out[mask] = np.maximum(0, 1 - x)[mask] / normalization
+    return out
+
+
+def biweight(x, dims=1):
+    normalization = 8 / ((dims + 2) * (dims + 4))
+    dist_sq = x**2
+    out = np.zeros_like(dist_sq)
+    mask = dist_sq < 1
+    out[mask] = np.maximum(0, (1 - dist_sq) ** 2)[mask] / normalization
+    return out
+
+
+def triweight(x, dims=1):
+    normalization = 48 / ((dims + 2) * (dims + 4) * (dims + 6))
+    dist_sq = x**2
+    out = np.zeros_like(dist_sq)
+    mask = dist_sq < 1
+    out[mask] = np.maximum(0, (1 - dist_sq) ** 3)[mask] / normalization
+    return out
+
+
+def tricube(x, dims=1):
+    normalization = 162 / ((dims + 3) * (dims + 6) * (dims + 9))
+    out = np.zeros_like(x)
+    mask = x < 1
+    out[mask] = np.maximum(0, (1 - x**3) ** 3)[mask] / normalization
+    return out
+
+
+def cosine(x, dims=1):
+    Is, Ic = trig_integral(dims - 1)
+    normalization = Ic
+    out = np.zeros_like(x)
+    mask = x < 1
+    out[mask] = np.cos((np.pi * x) / 2)[mask] / (normalization * dims)
+    return out
+
+
+def logistic(x, dims=1):
+    return 1 / (2 + 2 * np.cosh(x))
+
+
+def sigmoid(x, dims=1):
+    return 1 / (np.pi * np.cosh(x))
+
+
+class Kernel(collections.abc.Callable):
+    def __init__(self, function, var=1, support=3):
+        """
+        Initialize a new kernel function.
+
+        function: callable, numpy.arr -> numpy.arr, should integrate to 1
+        expected_value : peak, typically 0
+        support: support of the function.
+
+        Example
+        -------
+        >>> from scipy.special import gamma
+        >>> # Normalized function of x
+        >>> def exp(x, dims=1):
+        ...     normalization = gamma(dims) * dims
+        ...     return np.exp(-x) / normalization
+        >>> kernel = Kernel(exp, var=4, support=np.inf)
+        >>> # The function is scaled so that the standard deviation (bw) = 1
+        >>> kernel(0, bw=1, norm=2)[0] > kernel(1, bw=1, norm=2)[0]
+        True
+        >>> np.allclose(kernel(np.array([0, 1, 2])), kernel([0, 1, 2]))
+        True
+        >>> np.allclose(kernel(0), kernel([0]))
+        True
+        >>> np.allclose(kernel(0), kernel.evaluate(0))
+        True
+        """
+        self.function = function
+        self.var = var
+        self.finite_support = np.isfinite(support)
+
+        # If the function has finite support, scale the support so that it
+        # corresponds to the support of the function when it is scaled to have
+        # unit variance.
+        self.support = support / np.sqrt(self.var)
+
+    def practical_support(self, bw, atol=10e-5):
+        """
+        Return the support for practical purposes. Used to find a support value
+        for computations for kernel functions without finite (bounded) support.
+        """
+        # If the kernel has finite support, return the support accounting for
+        # the bw
+        if self.finite_support:
+            return self.support * bw
+
+        # If the function does not have finite support, find a practical value
+        else:
+
+            def f(x):
+                return self.evaluate(x, bw=bw) - atol
+
+            try:
+                xtol = 1e-3
+                ans = brentq(f, a=0, b=8 * bw, xtol=xtol, full_output=False)
+                return ans + xtol
+            except ValueError:
+                msg = (
+                    "Unable to solve for support numerically. Use a "
+                    + "kernel with finite support or scale data to smaller bw."
+                )
+                raise ValueError(msg)
+
+    def evaluate(self, x, bw=1, norm=2):
+        """
+        Evaluate the kernel.
+
+        Parameters
+        ----------
+        x : array-like
+            Should have shape (obs, dims).
+        bw : array-like
+            Must have shape (obs, ), or float.
+        """
+
+        # If x is a number, convert it to a length-1 NumPy vector
+        if isinstance(x, numbers.Number):
+            x = np.asarray_chkfinite([x])
+        else:
+            x = np.asarray_chkfinite(x)
+
+        if len(x.shape) == 1:
+            x = x.reshape(-1, 1)
+
+        # Scale the function, such that bw=1 corresponds to the function having
+        # a standard deviation (or variance) equal to 1
+        real_bw = bw / np.sqrt(self.var)
+        obs, dims = x.shape
+
+        # Set the volume function
+        volume_func = functools.partial(volume_unit_ball, p=norm)
+
+        if dims > 1:
+            distances = p_norm(x, norm).ravel()
+        else:
+            distances = np.abs(x).ravel()
+
+        return self.function(distances / real_bw, dims) / ((real_bw**dims) * volume_func(dims))
+
+    __call__ = evaluate
+
+
+gaussian = Kernel(gaussian, var=1, support=np.inf)
+exp = Kernel(exponential, var=2, support=np.inf)
+box = Kernel(box, var=1 / 3, support=1)
+tri = Kernel(tri, var=1 / 6, support=1)
+epa = Kernel(epanechnikov, var=1 / 5, support=1)
+biweight = Kernel(biweight, var=1 / 7, support=1)
+triweight = Kernel(triweight, var=1 / 9, support=1)
+tricube = Kernel(tricube, var=35 / 243, support=1)
+cosine = Kernel(cosine, var=(1 - (8 / np.pi**2)), support=1)
+logistic = Kernel(logistic, var=(np.pi**2 / 3), support=np.inf)
+sigmoid = Kernel(sigmoid, var=(np.pi**2 / 4), support=np.inf)
+
+_kernel_functions = {
+    "gaussian": gaussian,
+    "exponential": exp,
+    "box": box,
+    "tri": tri,
+    "epa": epa,
+    "biweight": biweight,
+    "triweight": triweight,
+    "tricube": tricube,
+    "cosine": cosine,
+    # 'logistic': logistic,
+    # 'sigmoid': sigmoid
+}
+
+
+if __name__ == "__main__" and False:
+    import pytest
+
+    # --durations=10  <- May be used to show potentially slow tests
+    pytest.main(args=[".", "--doctest-modules", "-v"])
```

## KDEpy/utils.py

 * *Ordering differences only*

```diff
@@ -1,139 +1,139 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Module for utility functions.
-"""
-import numbers
-
-import numpy as np
-
-
-def cartesian(arrays):
-    """
-    Generate a cartesian product of input arrays.
-    Adapted from:
-        https://github.com/scikit-learn/scikit-learn/blob/
-        master/sklearn/utils/extmath.py#L489
-
-    Parameters
-    ----------
-    arrays : list of array-like
-        1-D arrays to form the cartesian product of.
-    out : ndarray
-        Array to place the cartesian product in.
-
-    Returns
-    -------
-    out : ndarray
-        2-D array of shape (M, len(arrays)) containing cartesian products
-        formed of input arrays.
-
-    Examples
-    --------
-    >>> cartesian(([1, 2, 3], [4, 5], [6, 7]))
-    array([[1, 4, 6],
-           [1, 4, 7],
-           [1, 5, 6],
-           [1, 5, 7],
-           [2, 4, 6],
-           [2, 4, 7],
-           [2, 5, 6],
-           [2, 5, 7],
-           [3, 4, 6],
-           [3, 4, 7],
-           [3, 5, 6],
-           [3, 5, 7]])
-    """
-    arrays = [np.asarray(x) for x in arrays]
-    shape = (len(x) for x in arrays)
-    dtype = arrays[0].dtype
-
-    ix = np.indices(shape)
-    ix = ix.reshape(len(arrays), -1).T
-
-    out = np.empty_like(ix, dtype=dtype)
-
-    for n, _ in enumerate(arrays):
-        out[:, n] = arrays[n][ix[:, n]]
-
-    return out
-
-
-def autogrid(data, boundary_abs=3, num_points=None, boundary_rel=0.05):
-    """
-    Automatically select a grid if the user did not supply one.
-    Input is (obs, dims), and so is ouput.
-
-    number of grid : should be a power of two
-    percentile : is how far out we go out
-
-    Parameters
-    ----------
-    data : array-like
-        Data with shape (obs, dims).
-    boundary_abs: float
-        How far out from boundary observations the grid goes in each dimension.
-    num_points: int
-        The number of points in the resulting grid (after cartesian product).
-        Should be a number such that k**dims = `num_points`.
-    boundary_rel: float
-        How far out to go, relatively to max - min.
-
-    Returns
-    -------
-    grid : array-like
-        A grid of shape (obs, dims).
-
-    Examples
-    --------
-    >>> autogrid(np.array([[0, 0]]), boundary_abs=1, num_points=3)
-    array([[-1., -1.],
-           [-1.,  0.],
-           [-1.,  1.],
-           [ 0., -1.],
-           [ 0.,  0.],
-           [ 0.,  1.],
-           [ 1., -1.],
-           [ 1.,  0.],
-           [ 1.,  1.]])
-    >>> autogrid(np.array([[0, 0]]), boundary_abs=0.5, num_points=(2, 3))
-    array([[-0.5, -0.5],
-           [-0.5,  0. ],
-           [-0.5,  0.5],
-           [ 0.5, -0.5],
-           [ 0.5,  0. ],
-           [ 0.5,  0.5]])
-    """
-    _, dims = data.shape
-    minimums, maximums = data.min(axis=0), data.max(axis=0)
-    ranges = maximums - minimums
-
-    if num_points is None:
-        num_points = [int(np.power(1024, 1 / dims))] * dims
-    elif isinstance(num_points, (numbers.Number,)):
-        num_points = [num_points] * dims
-    elif isinstance(num_points, (list, tuple)):
-        pass
-    else:
-        msg = "`num_points` must be None, a number, or list/tuple for dims"
-        raise TypeError(msg)
-
-    if not len(num_points) == dims:
-        raise ValueError("Number of points must be sequence matching dims.")
-
-    list_of_grids = []
-
-    generator = enumerate(zip(minimums, maximums, ranges, num_points))
-    for _, (minimum, maximum, rang, points) in generator:
-        assert points >= 2
-        outside_borders = max(boundary_rel * rang, boundary_abs)
-        list_of_grids.append(np.linspace(minimum - outside_borders, maximum + outside_borders, num=points))
-
-    return cartesian(list_of_grids)
-
-
-if __name__ == "__main__":
-    import pytest
-
-    # --durations=10  <- May be used to show potentially slow tests
-    pytest.main(args=[".", "--doctest-modules", "-v", "--capture=sys"])
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Module for utility functions.
+"""
+import numbers
+
+import numpy as np
+
+
+def cartesian(arrays):
+    """
+    Generate a cartesian product of input arrays.
+    Adapted from:
+        https://github.com/scikit-learn/scikit-learn/blob/
+        master/sklearn/utils/extmath.py#L489
+
+    Parameters
+    ----------
+    arrays : list of array-like
+        1-D arrays to form the cartesian product of.
+    out : ndarray
+        Array to place the cartesian product in.
+
+    Returns
+    -------
+    out : ndarray
+        2-D array of shape (M, len(arrays)) containing cartesian products
+        formed of input arrays.
+
+    Examples
+    --------
+    >>> cartesian(([1, 2, 3], [4, 5], [6, 7]))
+    array([[1, 4, 6],
+           [1, 4, 7],
+           [1, 5, 6],
+           [1, 5, 7],
+           [2, 4, 6],
+           [2, 4, 7],
+           [2, 5, 6],
+           [2, 5, 7],
+           [3, 4, 6],
+           [3, 4, 7],
+           [3, 5, 6],
+           [3, 5, 7]])
+    """
+    arrays = [np.asarray(x) for x in arrays]
+    shape = (len(x) for x in arrays)
+    dtype = arrays[0].dtype
+
+    ix = np.indices(shape)
+    ix = ix.reshape(len(arrays), -1).T
+
+    out = np.empty_like(ix, dtype=dtype)
+
+    for n, _ in enumerate(arrays):
+        out[:, n] = arrays[n][ix[:, n]]
+
+    return out
+
+
+def autogrid(data, boundary_abs=3, num_points=None, boundary_rel=0.05):
+    """
+    Automatically select a grid if the user did not supply one.
+    Input is (obs, dims), and so is ouput.
+
+    number of grid : should be a power of two
+    percentile : is how far out we go out
+
+    Parameters
+    ----------
+    data : array-like
+        Data with shape (obs, dims).
+    boundary_abs: float
+        How far out from boundary observations the grid goes in each dimension.
+    num_points: int
+        The number of points in the resulting grid (after cartesian product).
+        Should be a number such that k**dims = `num_points`.
+    boundary_rel: float
+        How far out to go, relatively to max - min.
+
+    Returns
+    -------
+    grid : array-like
+        A grid of shape (obs, dims).
+
+    Examples
+    --------
+    >>> autogrid(np.array([[0, 0]]), boundary_abs=1, num_points=3)
+    array([[-1., -1.],
+           [-1.,  0.],
+           [-1.,  1.],
+           [ 0., -1.],
+           [ 0.,  0.],
+           [ 0.,  1.],
+           [ 1., -1.],
+           [ 1.,  0.],
+           [ 1.,  1.]])
+    >>> autogrid(np.array([[0, 0]]), boundary_abs=0.5, num_points=(2, 3))
+    array([[-0.5, -0.5],
+           [-0.5,  0. ],
+           [-0.5,  0.5],
+           [ 0.5, -0.5],
+           [ 0.5,  0. ],
+           [ 0.5,  0.5]])
+    """
+    _, dims = data.shape
+    minimums, maximums = data.min(axis=0), data.max(axis=0)
+    ranges = maximums - minimums
+
+    if num_points is None:
+        num_points = [int(np.power(1024, 1 / dims))] * dims
+    elif isinstance(num_points, (numbers.Number,)):
+        num_points = [num_points] * dims
+    elif isinstance(num_points, (list, tuple)):
+        pass
+    else:
+        msg = "`num_points` must be None, a number, or list/tuple for dims"
+        raise TypeError(msg)
+
+    if not len(num_points) == dims:
+        raise ValueError("Number of points must be sequence matching dims.")
+
+    list_of_grids = []
+
+    generator = enumerate(zip(minimums, maximums, ranges, num_points))
+    for _, (minimum, maximum, rang, points) in generator:
+        assert points >= 2
+        outside_borders = max(boundary_rel * rang, boundary_abs)
+        list_of_grids.append(np.linspace(minimum - outside_borders, maximum + outside_borders, num=points))
+
+    return cartesian(list_of_grids)
+
+
+if __name__ == "__main__":
+    import pytest
+
+    # --durations=10  <- May be used to show potentially slow tests
+    pytest.main(args=[".", "--doctest-modules", "-v", "--capture=sys"])
```

## Comparing `KDEpy-1.1.1.dist-info/LICENSE` & `KDEpy-1.1.2.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-BSD 3-Clause License
-
-Copyright (c) 2023, Tommy Odland
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2023, Tommy Odland
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

## Comparing `KDEpy-1.1.1.dist-info/METADATA` & `KDEpy-1.1.2.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,98 +1,96 @@
-Metadata-Version: 2.1
-Name: KDEpy
-Version: 1.1.1
-Summary: Kernel Density Estimation in Python.
-Home-page: https://github.com/tommyod/KDEpy
-Author: tommyod
-Author-email: tommy.odland@gmail.com
-License: new BSD
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy (>=1.14.2)
-Requires-Dist: scipy (>=1.0.1)
-Requires-Dist: matplotlib (>=2.2.0)
-
-[![DOI](https://zenodo.org/badge/118142261.svg)](https://zenodo.org/badge/latestdoi/118142261) ![Build Status](https://github.com/tommyod/KDEpy/workflows/Python%20CI/badge.svg?branch=master) [![Documentation Status](https://readthedocs.org/projects/kdepy/badge/?version=latest)](http://kdepy.readthedocs.io/en/latest/?badge=latest) [![PyPI version](https://badge.fury.io/py/KDEpy.svg)](https://badge.fury.io/py/KDEpy) [![Downloads](https://pepy.tech/badge/kdepy)](https://pepy.tech/project/kdepy)
----------
-
-Want to cite KDEpy in your work? See the [bottom right part of this website](https://zenodo.org/record/2392268) for citation information.
-
-# [KDEpy](https://kdepy.readthedocs.io/en/latest/)
-
-## About
-
-This Python 3.7+ package implements various kernel density estimators (KDE).
-Three algorithms are implemented through the same API: [`NaiveKDE`](https://kdepy.readthedocs.io/en/latest/API.html#naivekde), [`TreeKDE`](https://kdepy.readthedocs.io/en/latest/API.html#treekde) and [`FFTKDE`](https://kdepy.readthedocs.io/en/latest/API.html#fftkde).
-The class [`FFTKDE`](https://kdepy.readthedocs.io/en/latest/API.html#fftkde) outperforms other popular implementations, see the [comparison page](https://kdepy.readthedocs.io/en/latest/comparison.html).
-**The code is stable and in widespread by practitioners and in other packages.**
-
-![Plot](https://raw.githubusercontent.com/tommyod/KDEpy/master/docs/source/_static/img/showcase.png)
-
-*The code generating the above graph is found in [examples.py](https://github.com/tommyod/KDEpy/blob/master/docs/source/examples.py).*
-
-## Installation
-
-KDEpy is available through [PyPI](https://pypi.org/project/KDEpy/), and may be installed using `pip`:
-
-```text
-pip install KDEpy
-```
-
-If you have [trouble on Ubuntu](https://github.com/tommyod/KDEpy/issues/11), try running `sudo apt install libpython3.X-dev`, where `3.X` is your Python version. 
-
-## Example code and documentation
-
-Below is an example showing an unweighted and weighted kernel density.
-From the code below, it should be clear how to set the *kernel*, *bandwidth* (variance of the kernel) and *weights*.
-See the [documentation](https://kdepy.readthedocs.io/en/latest/examples.html) for more examples.
-
-```python
-from KDEpy import FFTKDE
-import matplotlib.pyplot as plt
-
-customer_ages = [40, 56, 20, 35, 27, 24, 29, 37, 39, 46]
-
-# Distribution of customers
-x, y = FFTKDE(kernel="gaussian", bw="silverman").fit(customer_ages).evaluate()
-plt.plot(x, y)
-
-# Distribution of customer income (weight each customer by their income)
-customer_income = [152, 64, 24, 140, 88, 64, 103, 148, 150, 132]
-
-# The `bw` parameter can be manually set, e.g. `bw=5`
-x, y = FFTKDE(bw="silverman").fit(customer_ages, weights=customer_income).evaluate()
-plt.plot(x, y)
-```
-![Plot](https://raw.githubusercontent.com/tommyod/KDEpy/master/docs/source/_static/img/README_example.png)
-
-The package consists of three algorithms. Here's a brief explanation:
-- [`NaiveKDE`](https://kdepy.readthedocs.io/en/latest/API.html#naivekde) - A naive computation. Supports d-dimensional data, variable bandwidth, weighted data and many kernel functions. Very slow on large data sets.
-- [`TreeKDE`](https://kdepy.readthedocs.io/en/latest/API.html#treekde) - A tree-based computation. Supports the same features as the naive algorithm, but is faster at the expense of small inaccuracy when using a kernel without finite support. Good for evaluation on non-uniform, arbitrary grids.
-- [`FFTKDE`](https://kdepy.readthedocs.io/en/latest/API.html#fftkde) - A very fast convolution-based computation. Supports weighted d-dimensional data and many kernels, but not variable bandwidth. Must be evaluated on an equidistant grid, the finer the grid the higher the accuracy. Data points may not be outside of the grid.
-
-## Issues and contributing
-
-### Issues
-
-If you are having trouble using the package, please let me know by creating an [Issue on GitHub](https://github.com/tommyod/KDEpy/issues) and I'll get back to you.
-
-### Contributing
-
-Whatever your mathematical and Python background is, you are very welcome to contribute to KDEpy.
-To contribute, fork the project, create a branch and submit and Pull Request.
-Please follow these guidelines:
-
-- Import as few external dependencies as possible.
-- Use test driven development, have tests and docs for every method.
-- Cite literature and implement recent methods.
-- Unless it's a bottleneck computation, readability trumps speed.
-- Employ object orientation, but resist the temptation to implement many methods -- stick to the basics.
-- Follow PEP8.
+Metadata-Version: 2.1
+Name: KDEpy
+Version: 1.1.2
+Summary: Kernel Density Estimation in Python.
+Home-page: https://github.com/tommyod/KDEpy
+Author: tommyod
+Author-email: tommy.odland@gmail.com
+License: new BSD
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy (>=1.14.2)
+Requires-Dist: scipy (>=1.0.1)
+Requires-Dist: matplotlib (>=2.2.0)
+
+[![DOI](https://zenodo.org/badge/118142261.svg)](https://zenodo.org/badge/latestdoi/118142261) ![Build Status](https://github.com/tommyod/KDEpy/workflows/Python%20CI/badge.svg?branch=master) [![Documentation Status](https://readthedocs.org/projects/kdepy/badge/?version=latest)](http://kdepy.readthedocs.io/en/latest/?badge=latest) [![PyPI version](https://badge.fury.io/py/KDEpy.svg)](https://badge.fury.io/py/KDEpy) [![Downloads](https://pepy.tech/badge/kdepy)](https://pepy.tech/project/kdepy)
+---------
+
+Want to cite KDEpy in your work? See the [bottom right part of this website](https://zenodo.org/record/2392268) for citation information.
+
+# [KDEpy](https://kdepy.readthedocs.io/en/latest/)
+
+## About
+
+This Python 3.7+ package implements various kernel density estimators (KDE).
+Three algorithms are implemented through the same API: [`NaiveKDE`](https://kdepy.readthedocs.io/en/latest/API.html#naivekde), [`TreeKDE`](https://kdepy.readthedocs.io/en/latest/API.html#treekde) and [`FFTKDE`](https://kdepy.readthedocs.io/en/latest/API.html#fftkde).
+The class [`FFTKDE`](https://kdepy.readthedocs.io/en/latest/API.html#fftkde) outperforms other popular implementations, see the [comparison page](https://kdepy.readthedocs.io/en/latest/comparison.html).
+**The code is stable and in widespread by practitioners and in other packages.**
+
+![Plot](https://raw.githubusercontent.com/tommyod/KDEpy/master/docs/source/_static/img/showcase.png)
+
+*The code generating the above graph is found in [examples.py](https://github.com/tommyod/KDEpy/blob/master/docs/source/examples.py).*
+
+## Installation
+
+KDEpy is available through [PyPI](https://pypi.org/project/KDEpy/), and may be installed using `pip`:
+
+```text
+pip install KDEpy
+```
+
+If you have [trouble on Ubuntu](https://github.com/tommyod/KDEpy/issues/11), try running `sudo apt install libpython3.X-dev`, where `3.X` is your Python version. 
+
+## Example code and documentation
+
+Below is an example showing an unweighted and weighted kernel density.
+From the code below, it should be clear how to set the *kernel*, *bandwidth* (variance of the kernel) and *weights*.
+See the [documentation](https://kdepy.readthedocs.io/en/latest/examples.html) for more examples.
+
+```python
+from KDEpy import FFTKDE
+import matplotlib.pyplot as plt
+
+customer_ages = [40, 56, 20, 35, 27, 24, 29, 37, 39, 46]
+
+# Distribution of customers
+x, y = FFTKDE(kernel="gaussian", bw="silverman").fit(customer_ages).evaluate()
+plt.plot(x, y)
+
+# Distribution of customer income (weight each customer by their income)
+customer_income = [152, 64, 24, 140, 88, 64, 103, 148, 150, 132]
+
+# The `bw` parameter can be manually set, e.g. `bw=5`
+x, y = FFTKDE(bw="silverman").fit(customer_ages, weights=customer_income).evaluate()
+plt.plot(x, y)
+```
+![Plot](https://raw.githubusercontent.com/tommyod/KDEpy/master/docs/source/_static/img/README_example.png)
+
+The package consists of three algorithms. Here's a brief explanation:
+- [`NaiveKDE`](https://kdepy.readthedocs.io/en/latest/API.html#naivekde) - A naive computation. Supports d-dimensional data, variable bandwidth, weighted data and many kernel functions. Very slow on large data sets.
+- [`TreeKDE`](https://kdepy.readthedocs.io/en/latest/API.html#treekde) - A tree-based computation. Supports the same features as the naive algorithm, but is faster at the expense of small inaccuracy when using a kernel without finite support. Good for evaluation on non-uniform, arbitrary grids.
+- [`FFTKDE`](https://kdepy.readthedocs.io/en/latest/API.html#fftkde) - A very fast convolution-based computation. Supports weighted d-dimensional data and many kernels, but not variable bandwidth. Must be evaluated on an equidistant grid, the finer the grid the higher the accuracy. Data points may not be outside of the grid.
+
+## Issues and contributing
+
+### Issues
+
+If you are having trouble using the package, please let me know by creating an [Issue on GitHub](https://github.com/tommyod/KDEpy/issues) and I'll get back to you.
+
+### Contributing
+
+Whatever your mathematical and Python background is, you are very welcome to contribute to KDEpy.
+To contribute, fork the project, create a branch and submit and Pull Request.
+Please follow these guidelines:
+
+- Import as few external dependencies as possible.
+- Use test driven development, have tests and docs for every method.
+- Cite literature and implement recent methods.
+- Unless it's a bottleneck computation, readability trumps speed.
+- Employ object orientation, but resist the temptation to implement many methods -- stick to the basics.
+- Follow PEP8.
```

