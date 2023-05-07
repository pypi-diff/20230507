# Comparing `tmp/keyrock-math-2023.3.18.2024.tar.gz` & `tmp/keyrock-math-2023.5.7.1147.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyrock-math-2023.3.18.2024.tar", last modified: Sat Mar 18 20:24:48 2023, max compression
+gzip compressed data, was "keyrock-math-2023.5.7.1147.tar", last modified: Sun May  7 11:47:31 2023, max compression
```

## Comparing `keyrock-math-2023.3.18.2024.tar` & `keyrock-math-2023.5.7.1147.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 20:24:48.873523 keyrock-math-2023.3.18.2024/
--rw-r--r--   0 root         (0) root         (0)       65 2023-03-18 20:24:48.873523 keyrock-math-2023.3.18.2024/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 20:24:48.862522 keyrock-math-2023.3.18.2024/keyrock_math/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 20:24:48.868523 keyrock-math-2023.3.18.2024/keyrock_math/distribution/
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution/analytic.py
--rw-rw-rw-   0 root         (0) root         (0)      521 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution/beta.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution/constant.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution/distribution.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution/gamma.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution/log_normal.py
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution/logistic.py
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution/normal.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution/skew_normal.py
--rw-rw-rw-   0 root         (0) root         (0)     3658 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution/test_distribution.py
--rw-rw-rw-   0 root         (0) root         (0)      528 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution/uniform.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution/weibull.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 20:24:48.873523 keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/
--rw-rw-rw-   0 root         (0) root         (0)      520 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1603 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/analytic.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/beta.py
--rw-rw-rw-   0 root         (0) root         (0)      650 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/constant.py
--rw-rw-rw-   0 root         (0) root         (0)      920 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/distribution.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/gamma.py
--rw-rw-rw-   0 root         (0) root         (0)     2232 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/log_normal.py
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/logistic.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/normal.py
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/skew_normal.py
--rw-rw-rw-   0 root         (0) root         (0)     2696 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/test_distribution.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/uniform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 20:24:48.864522 keyrock-math-2023.3.18.2024/keyrock_math.egg-info/
--rw-r--r--   0 root         (0) root         (0)       65 2023-03-18 20:24:48.000000 keyrock-math-2023.3.18.2024/keyrock_math.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1241 2023-03-18 20:24:48.000000 keyrock-math-2023.3.18.2024/keyrock_math.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-18 20:24:48.000000 keyrock-math-2023.3.18.2024/keyrock_math.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-03-18 20:24:48.000000 keyrock-math-2023.3.18.2024/keyrock_math.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-18 20:24:48.000000 keyrock-math-2023.3.18.2024/keyrock_math.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-03-18 20:24:32.000000 keyrock-math-2023.3.18.2024/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-03-18 20:24:48.874523 keyrock-math-2023.3.18.2024/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 11:47:31.814106 keyrock-math-2023.5.7.1147/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-05-07 11:47:31.814106 keyrock-math-2023.5.7.1147/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 11:47:31.802105 keyrock-math-2023.5.7.1147/keyrock_math/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 11:47:31.809106 keyrock-math-2023.5.7.1147/keyrock_math/distribution/
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/analytic.py
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/beta.py
+-rw-rw-rw-   0 root         (0) root         (0)      600 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/constant.py
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/gamma.py
+-rw-rw-rw-   0 root         (0) root         (0)     1601 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/log_normal.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/logistic.py
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/normal.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/skew_normal.py
+-rw-rw-rw-   0 root         (0) root         (0)     3658 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/test_distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/uniform.py
+-rw-rw-rw-   0 root         (0) root         (0)      764 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/weibull.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 11:47:31.814106 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/
+-rw-rw-rw-   0 root         (0) root         (0)      520 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1603 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/analytic.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/beta.py
+-rw-rw-rw-   0 root         (0) root         (0)      650 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/constant.py
+-rw-rw-rw-   0 root         (0) root         (0)      920 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/gamma.py
+-rw-rw-rw-   0 root         (0) root         (0)     2232 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/log_normal.py
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/logistic.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/normal.py
+-rw-rw-rw-   0 root         (0) root         (0)      539 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/skew_normal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2696 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/test_distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/uniform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 11:47:31.804105 keyrock-math-2023.5.7.1147/keyrock_math.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-05-07 11:47:31.000000 keyrock-math-2023.5.7.1147/keyrock_math.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-05-07 11:47:31.000000 keyrock-math-2023.5.7.1147/keyrock_math.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 11:47:31.000000 keyrock-math-2023.5.7.1147/keyrock_math.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-07 11:47:31.000000 keyrock-math-2023.5.7.1147/keyrock_math.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-07 11:47:31.000000 keyrock-math-2023.5.7.1147/keyrock_math.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-05-07 11:47:31.814106 keyrock-math-2023.5.7.1147/setup.cfg
```

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution/__init__.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution/analytic.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution/analytic.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 from abc import abstractmethod
 
 from .distribution import Distribution
 
 logger = logging.getLogger(__name__)
 
+cache_size = 100
+
 class Analytic(Distribution):
     _rv: None = None
     _rv_cache: None = None
     _rv_index: int = 0
 
     def pdf(self, x:float) -> float:
         return self._rv.pdf(x)
@@ -21,12 +23,16 @@
     def cdf(self, x:float) -> float:
         return self._rv.cdf(x)
 
     def quantile(self, p:float) -> float:
         return self._rv.ppf(p)
 
     def get_random_value(self, size=1) -> float:
-        if self._rv_cache is None:
-            self._rv_cache = self.rv.rvs(10001)
+        # Build a new cache when limit is reached
+        if self._rv_cache is None or self._rv_index >= cache_size:
+            self._rv_index = 0
+            self._rv_cache = self._rv.rvs(cache_size, random_state=self._rng)
 
-        val = self._rv_cache[self.rv_index % 10001]
+        val = self._rv_cache[self._rv_index]
         self._rv_index += 1
+
+        return val
```

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution/constant.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution/constant.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from .analytic import Distribution
 
 logger = logging.getLogger(__name__)
 
 class Constant(Distribution):
     t: Literal['constant'] = 'constant'
-    loc: float = 0
+    loc: float = 0.0
 
     @property
     def x_min(self):
         return self.loc
 
     @property
     def x_max(self):
```

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution/distribution.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution/distribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from keyrock_model.model import KrBaseModel
 
 logger = logging.getLogger(__name__)
 
 class Distribution(KrBaseModel):
     t: Literal['base'] = 'base'
     _x_space: None = None
+    _rng: None = None
 
     @property
     def x_min(self):
         return -math.inf
 
     @property
     def x_max(self):
@@ -32,14 +33,17 @@
     @abstractmethod
     def quantile(self, p: float) -> float:
         raise NotImplementedError()
 
     def get_random_value(self, size=1) -> float:
         raise NotImplementedError()
 
+    def set_rng(self, rng):
+        self._rng = rng
+
     ### Helpers ###
 
     def get_percentile(self, p):
         return self.quantile(p)
 
     def get_x_space(self):
         if self._x_space is None:
```

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution/gamma.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution/gamma.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 from .analytic import Analytic
 
 logger = logging.getLogger(__name__)
 
 class Gamma(Analytic):
     t: Literal['gamma'] = 'gamma'
-    a: float = 1
-    rate: float = 1
-    loc: float = 0
+    a: float = 1.0
+    rate: float = 1.0
+    loc: float = 0.0
 
     def __post_init__(self):
         scale = 1.0 / self.rate
         self._rv = sps.gamma(
             a=self.a,
             loc=self.loc,
             scale=scale)
```

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution/log_normal.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution/log_normal.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 SQRT2 = math.sqrt(2)
 SQRT2PI = math.sqrt(2 * math.pi)
 MIN_X = 0.000000001
 
 class LogNormal(Distribution):
     t: Literal['log_normal'] = 'log_normal'
-    loc: float = 0
-    scale: float = 1
+    loc: float = 0.0
+    scale: float = 1.0
 
     def __post_init__(self):
         self.mu = self.loc
         self.sigma = self.scale
 
     @property
     def x_min(self):
@@ -52,8 +52,11 @@
         Q = math.sqrt(2.0 * self.sigma * self.sigma)
         Q *= erfinv(2.0 * p - 1.0)
         Q += self.mu
         Q = math.exp(Q)
         return Q
 
     def get_random_value(self, size=1) -> float:
-        return np.random.lognormal(self.mu, self.sigma)
+        if self._rng:
+            return self._rng.lognormal(self.mu, self.sigma)
+        else:
+            return np.random.lognormal(self.mu, self.sigma)
```

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution/test_distribution.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution/test_distribution.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution/uniform.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution/uniform.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from .analytic import Analytic
 
 logger = logging.getLogger(__name__)
 
 class Uniform(Analytic):
     t: Literal['uniform'] = 'uniform'
-    a: float = 0
-    b: float = 1
+    a: float = 0.0
+    b: float = 1.0
 
     def __post_init__(self):
         scale = self.b - self.a
         self._rv = sps.uniform(
                 loc=self.a,
                 scale=scale
             )
```

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution/weibull.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution/weibull.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # Special shape values are 1 and 2
 #   where Weibull distribution reduces to the expon and rayleigh distributions respectively
 
 # The value of the scale parameter equals the 63.2 percentile in the distribution
 
 class Weibull(Analytic):
     t: Literal['weibull'] = 'weibull'
-    threshold: float = 0
-    shape: float = 2 # beta or k
-    scale: float = 1 # lambda
+    threshold: float = 0.0
+    shape: float = 2.0 # beta or k
+    scale: float = 1.0 # lambda
 
     def __post_init__(self):
         self._rv = sps.weibull_min(
                 c=self.shape,
                 loc=self.threshold,
                 scale=self.scale
             )
```

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/__init__.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/__init__.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/analytic.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/analytic.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/beta.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/beta.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/constant.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/constant.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/distribution.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/distribution.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/gamma.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/gamma.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/log_normal.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/log_normal.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/normal.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/normal.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/skew_normal.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/skew_normal.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/test_distribution.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/test_distribution.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math/distribution_old/uniform.py` & `keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/uniform.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.3.18.2024/keyrock_math.egg-info/SOURCES.txt` & `keyrock-math-2023.5.7.1147/keyrock_math.egg-info/SOURCES.txt`

 * *Files identical despite different names*

