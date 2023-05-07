# Comparing `tmp/omoment-0.1.3.tar.gz` & `tmp/omoment-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omoment-0.1.3.tar", last modified: Sat Jan 21 10:10:39 2023, max compression
+gzip compressed data, was "omoment-0.1.4.tar", last modified: Sun May  7 18:16:01 2023, max compression
```

## Comparing `omoment-0.1.3.tar` & `omoment-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,25 @@
--rw-r--r--   0        0        0      726 2022-10-29 21:19:55.803580 omoment-0.1.3/.github/workflows/builddoc.yaml
--rw-r--r--   0        0        0     1050 2022-10-29 20:55:31.453855 omoment-0.1.3/.github/workflows/pytest.yaml
--rw-r--r--   0        0        0     1889 2022-10-29 20:12:44.215687 omoment-0.1.3/.gitignore
--rw-r--r--   0        0        0     1074 2022-10-28 11:01:20.166050 omoment-0.1.3/LICENSE
--rw-r--r--   0        0        0     4273 2022-11-28 18:50:37.231885 omoment-0.1.3/README.rst
--rw-r--r--   0        0        0      515 2023-01-21 09:49:21.871075 omoment-0.1.3/changelog.rst
--rw-r--r--   0        0        0       74 2022-10-29 12:10:17.934348 omoment-0.1.3/doc/api/obase.rst
--rw-r--r--   0        0        0       96 2022-10-29 11:38:32.206847 omoment-0.1.3/doc/api/omean.rst
--rw-r--r--   0        0        0      105 2022-10-29 11:40:59.911415 omoment-0.1.3/doc/api/omeanvar.rst
--rw-r--r--   0        0        0     1730 2022-10-29 20:09:04.562822 omoment-0.1.3/doc/conf.py
--rw-r--r--   0        0        0      487 2022-10-29 11:45:13.624391 omoment-0.1.3/doc/index.rst
--rw-r--r--   0        0        0     4029 2022-11-28 21:51:27.079044 omoment-0.1.3/omoment/__init__.py
--rw-r--r--   0        0        0     4818 2022-11-28 20:16:37.926867 omoment-0.1.3/omoment/obase.py
--rw-r--r--   0        0        0     9963 2023-01-21 09:48:26.322943 omoment-0.1.3/omoment/omean.py
--rw-r--r--   0        0        0    11513 2023-01-21 09:34:12.344936 omoment-0.1.3/omoment/omeanvar.py
--rw-r--r--   0        0        0       17 2023-01-21 09:49:54.387152 omoment-0.1.3/omoment/version.py
--rw-r--r--   0        0        0     1205 2022-11-28 18:35:53.908523 omoment-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       13 2022-10-28 11:24:51.428266 omoment-0.1.3/requirements.txt
--rw-r--r--   0        0        0        7 2022-10-28 12:41:15.741275 omoment-0.1.3/test_requirements.txt
--rw-r--r--   0        0        0     5539 2023-01-21 09:48:09.410903 omoment-0.1.3/tests/test_omean.py
--rw-r--r--   0        0        0     7566 2023-01-21 09:46:18.206640 omoment-0.1.3/tests/test_omeanvar.py
--rw-r--r--   0        0        0     5339 1970-01-01 00:00:00.000000 omoment-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      726 2022-10-29 21:19:55.803580 omoment-0.1.4/.github/workflows/builddoc.yaml
+-rw-r--r--   0        0        0     1050 2022-10-29 20:55:31.453855 omoment-0.1.4/.github/workflows/pytest.yaml
+-rw-r--r--   0        0        0     1889 2022-10-29 20:12:44.215687 omoment-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1074 2022-10-28 11:01:20.166050 omoment-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4468 2023-05-07 18:13:50.450480 omoment-0.1.4/README.rst
+-rw-r--r--   0        0        0      775 2023-05-07 16:09:56.817015 omoment-0.1.4/changelog.rst
+-rw-r--r--   0        0        0       74 2022-10-29 12:10:17.934348 omoment-0.1.4/doc/api/obase.rst
+-rw-r--r--   0        0        0       96 2022-10-29 11:38:32.206847 omoment-0.1.4/doc/api/omean.rst
+-rw-r--r--   0        0        0      105 2022-10-29 11:40:59.911415 omoment-0.1.4/doc/api/omeanvar.rst
+-rw-r--r--   0        0        0       93 2023-05-07 17:57:42.608666 omoment-0.1.4/doc/api/oreg.rst
+-rw-r--r--   0        0        0     1730 2022-10-29 20:09:04.562822 omoment-0.1.4/doc/conf.py
+-rw-r--r--   0        0        0      487 2022-10-29 11:45:13.624391 omoment-0.1.4/doc/index.rst
+-rw-r--r--   0        0        0     4252 2023-05-07 18:06:45.621680 omoment-0.1.4/omoment/__init__.py
+-rw-r--r--   0        0        0     4818 2022-11-28 20:16:37.926867 omoment-0.1.4/omoment/obase.py
+-rw-r--r--   0        0        0    10368 2023-05-07 16:03:54.284352 omoment-0.1.4/omoment/omean.py
+-rw-r--r--   0        0        0    11924 2023-05-07 17:12:45.887940 omoment-0.1.4/omoment/omeanvar.py
+-rw-r--r--   0        0        0    11339 2023-05-07 16:59:00.962464 omoment-0.1.4/omoment/oreg.py
+-rw-r--r--   0        0        0       17 2023-05-07 15:54:42.967358 omoment-0.1.4/omoment/version.py
+-rw-r--r--   0        0        0     1205 2022-11-28 18:35:53.908523 omoment-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       13 2022-10-28 11:24:51.428266 omoment-0.1.4/requirements.txt
+-rw-r--r--   0        0        0       19 2023-05-07 17:50:35.679906 omoment-0.1.4/test_requirements.txt
+-rw-r--r--   0        0        0     5539 2023-01-21 09:48:09.410903 omoment-0.1.4/tests/test_omean.py
+-rw-r--r--   0        0        0     7566 2023-01-21 09:46:18.206640 omoment-0.1.4/tests/test_omeanvar.py
+-rw-r--r--   0        0        0    11003 2023-05-07 17:56:42.696559 omoment-0.1.4/tests/test_oreg.py
+-rw-r--r--   0        0        0     5522 1970-01-01 00:00:00.000000 omoment-0.1.4/PKG-INFO
```

### Comparing `omoment-0.1.3/.github/workflows/builddoc.yaml` & `omoment-0.1.4/.github/workflows/builddoc.yaml`

 * *Files identical despite different names*

### Comparing `omoment-0.1.3/.github/workflows/pytest.yaml` & `omoment-0.1.4/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `omoment-0.1.3/.gitignore` & `omoment-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `omoment-0.1.3/LICENSE` & `omoment-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `omoment-0.1.3/README.rst` & `omoment-0.1.4/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 ..  |doc-badge| image:: https://github.com/protivinsky/omoment/actions/workflows/builddoc.yaml/badge.svg
     :alt: doc
     :target: https://protivinsky.github.io/omoment/index.html
 
 OMoment: Efficient online calculation of statistical moments
 ============================================================
 
-OMoment package calculates moments of statistical distributions (mean and variance) in online or distributed settings.
+OMoment package calculates moments of statistical distributions (means, variances, covariance) in online or
+distributed settings for univariate and bivariate distributions.
 
 - Suitable for large data – works well with numpy and Pandas and in distributed setting.
 - Moments calculated from different parts of data can be easily combined or updated for new data (supports addition
   of results).
 - Objects are lightweight, calculation is done in numpy if possible.
 - Weights for data can be provided.
 - Invalid values (NaNs, infinities are omitted by default).
 
-Typical application is calculation of means and variances of many chunks of data (corresponding to different groups
-or to different parts of the distributed data), the results can be analyzed on level of the groups or easily
-combined to get exact moments for the full dataset.
+Typical application is calculation of means and variances (or even correlation of two variables) of many chunks of data
+(corresponding to different groups or to different parts of the distributed data), the results can be analyzed on level
+of the groups or easily combined to get exact moments for the full dataset.
 
 Basic example
 -------------
 
 .. code:: python
 
     from omoment import OMeanVar
@@ -34,28 +35,29 @@
 
     rng = np.random.default_rng(12354)
     g = rng.integers(low=0, high=10, size=1000)
     x = g + rng.normal(loc=0, scale=10, size=1000)
     w = rng.exponential(scale=1, size=1000)
 
     # calculate overall moments
-    OMeanVar(x, weight=w)
+    OMeanVar.compute(x, w)
     # should give: OMeanVar(mean=4.6, var=108, weight=1.08e+03)
 
     # or calculate moments for every group
     df = pd.DataFrame({'g': g, 'x': x, 'w': w})
     omvs = df.groupby('g').apply(OMeanVar.of_frame, x='x', w='w')
 
     # and combine group moments to obtain the same overall results
     OMeanVar.combine(omvs)
 
     # addition is also supported
     omvs.loc[0] + omvs.loc[1]
 
-At the moment, only univariate distributions are supported. Bivariate or even multivariate distributions can be
+At the moment, univariate and bivariate distributions are supported. Bivariate distributions allow for fast linear
+regression with two variables (and constant) calculation. Even multivariate distributions can be
 efficiently processed in a similar fashion, so the support for them might be added in the future. Moments of
 multivariate distributions would also allow for linear regression estimation and other statistical methods
 (such as PCA or regularized regression) to be calculated in a single pass through large distributed datasets.
 
 Similar packages
 ----------------
 
@@ -98,13 +100,13 @@
 ...
 
 `OpenAI Gym
 <https://github.com/openai/gym>`_ (or newly `Gymnasium
 <https://github.com/Farama-Foundation/Gymnasium>`_)
 provides similar functionality as a part of its normalization of observations and rewards
 (in gym.wrappers.normalize.RunningMeanStd). The functionality is fairly limited as it was developed for a particular
-use case, but the calculation is fast and it is possible to compose the results. It does not support weights though.
+use case, but the calculation is fast, and it is possible to compose the results. It does not support weights though.
 
 Documentation
 -------------
 
 - https://protivinsky.github.io/omoment/index.html
```

### Comparing `omoment-0.1.3/doc/conf.py` & `omoment-0.1.4/doc/conf.py`

 * *Files identical despite different names*

### Comparing `omoment-0.1.3/omoment/__init__.py` & `omoment-0.1.4/omoment/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """
-OMoment package calculates moments of statistical distributions (means and variance) in online or distributed settings.
+OMoment package calculates moments of statistical distributions (means, variances, covariance) in online or
+distributed settings for univariate and bivariate distributions.
 
 - Suitable for large data – works well with numpy and Pandas and in distributed setting.
 - Moments calculated from different parts of data can be easily combined or updated for new data (supports addition
   of results).
 - Objects are lightweight, calculation is done in numpy if possible.
 - Weights for data can be provided.
 - Invalid values (NaNs, infinities are omitted by default).
 
-Typical application is calculation of means and variances of many chunks of data (corresponding to different groups
-or to different parts of the distributed data), the results can be analyzed on level of the groups or easily
-combined to get exact moments for the full dataset.
+Typical application is calculation of means and variances (or even correlation of two variables) of many chunks of data
+(corresponding to different groups or to different parts of the distributed data), the results can be analyzed on level
+of the groups or easily combined to get exact moments for the full dataset.
 
 Basic example
 -------------
 
 .. code:: python
 
     from omoment import OMeanVar
@@ -38,15 +39,16 @@
 
     # and combine group moments to obtain the same overall results
     OMeanVar.combine(omvs)
 
     # addition is also supported
     omvs.loc[0] + omvs.loc[1]
 
-At the moment, only univariate distributions are supported. Bivariate or even multivariate distributions can be
+At the moment, univariate and bivariate distributions are supported. Bivariate distributions allow for fast linear
+regression with two variables (and constant) calculation. Even multivariate distributions can be
 efficiently processed in a similar fashion, so the support for them might be added in the future. Moments of
 multivariate distributions would also allow for linear regression estimation and other statistical methods
 (such as PCA or regularized regression) to be calculated in a single pass through large distributed datasets.
 
 Similar packages
 ----------------
 
@@ -96,10 +98,11 @@
 use case, but the calculation is fast, and it is possible to compose the results. It does not support weights though.
 """
 
 from .version import VERSION as __version__
 from .obase import OBase, HandlingInvalid
 from .omean import OMean
 from .omeanvar import OMeanVar
+from .oreg import OReg
 
-__all__ = ['OBase', 'OMean', 'OMeanVar', 'HandlingInvalid']
+__all__ = ['OBase', 'OMean', 'OMeanVar', 'OReg', 'HandlingInvalid']
 __author__ = 'Tomas Protivinsky'
```

### Comparing `omoment-0.1.3/omoment/obase.py` & `omoment-0.1.4/omoment/obase.py`

 * *Files identical despite different names*

### Comparing `omoment-0.1.3/omoment/omean.py` & `omoment-0.1.4/omoment/omean.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         OMean is zero if it has zero weight: it behaves as zero element under the addition.
         """
         return self.weight.__nonzero__()
 
     @classmethod
     def of_frame(cls, data: pd.DataFrame, x: str, w: Optional[str] = None,
                  handling_invalid: HandlingInvalid = HandlingInvalid.Drop) -> OMean:
-        """Convenient function for calculation OMean of pandas DataFrame.
+        """Convenience function for calculation OMean of pandas DataFrame.
 
         Args:
             data: input DataFrame
             x: name of column with values to calculated mean of
             w: name of column with weights (optional)
             handling_invalid: How to handle invalid values in calculation ['drop', 'keep', 'raise'], default value
              'drop'. Provided either as enum or its string representation.
@@ -220,7 +220,17 @@
         """Convenience function to be used as a lambda."""
         return om.mean
 
     @staticmethod
     def get_weight(om: OMean):
         """Convenience function to be used as a lambda."""
         return om.weight
+
+    # Explicit override to allow for intellisense
+    @classmethod
+    def compute(cls,
+                x: Union[Number, np.ndarray, pd.Series],
+                w: Optional[Union[Number, np.ndarray, pd.Series]] = None,
+                handling_invalid: HandlingInvalid = HandlingInvalid.Drop) -> OMean:
+        om = cls()
+        om.update(x=x, w=w, handling_invalid=handling_invalid)
+        return om
```

### Comparing `omoment-0.1.3/omoment/omeanvar.py` & `omoment-0.1.4/omoment/omeanvar.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,7 +249,18 @@
         """Convenience function to be used as a lambda."""
         return om.unbiased_var
 
     @staticmethod
     def get_unbiased_std_dev(om: OMeanVar):
         """Convenience function to be used as a lambda."""
         return om.unbiased_std_dev
+
+    # Explicit override to allow for intellisense
+    @classmethod
+    def compute(cls,
+                x: Union[Number, np.ndarray, pd.Series],
+                w: Optional[Union[Number, np.ndarray, pd.Series]] = None,
+                handling_invalid: HandlingInvalid = HandlingInvalid.Drop) -> OMeanVar:
+        omv = cls()
+        omv.update(x=x, w=w, handling_invalid=handling_invalid)
+        return omv
+
```

### Comparing `omoment-0.1.3/pyproject.toml` & `omoment-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `omoment-0.1.3/tests/test_omean.py` & `omoment-0.1.4/tests/test_omean.py`

 * *Files identical despite different names*

### Comparing `omoment-0.1.3/tests/test_omeanvar.py` & `omoment-0.1.4/tests/test_omeanvar.py`

 * *Files identical despite different names*

### Comparing `omoment-0.1.3/PKG-INFO` & `omoment-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: omoment
-Version: 0.1.3
-Summary: OMoment package calculates moments of statistical distributions (means and variance) in online or distributed settings.
+Version: 0.1.4
+Summary: OMoment package calculates moments of statistical distributions (means, variances, covariance) in online or
 Keywords: statistics,mean,variance,distributed,estimation,efficient,additive
 Author-email: Tomas Protivinsky <tomas.protivinsky@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -30,26 +30,27 @@
 ..  |doc-badge| image:: https://github.com/protivinsky/omoment/actions/workflows/builddoc.yaml/badge.svg
     :alt: doc
     :target: https://protivinsky.github.io/omoment/index.html
 
 OMoment: Efficient online calculation of statistical moments
 ============================================================
 
-OMoment package calculates moments of statistical distributions (mean and variance) in online or distributed settings.
+OMoment package calculates moments of statistical distributions (means, variances, covariance) in online or
+distributed settings for univariate and bivariate distributions.
 
 - Suitable for large data – works well with numpy and Pandas and in distributed setting.
 - Moments calculated from different parts of data can be easily combined or updated for new data (supports addition
   of results).
 - Objects are lightweight, calculation is done in numpy if possible.
 - Weights for data can be provided.
 - Invalid values (NaNs, infinities are omitted by default).
 
-Typical application is calculation of means and variances of many chunks of data (corresponding to different groups
-or to different parts of the distributed data), the results can be analyzed on level of the groups or easily
-combined to get exact moments for the full dataset.
+Typical application is calculation of means and variances (or even correlation of two variables) of many chunks of data
+(corresponding to different groups or to different parts of the distributed data), the results can be analyzed on level
+of the groups or easily combined to get exact moments for the full dataset.
 
 Basic example
 -------------
 
 .. code:: python
 
     from omoment import OMeanVar
@@ -58,28 +59,29 @@
 
     rng = np.random.default_rng(12354)
     g = rng.integers(low=0, high=10, size=1000)
     x = g + rng.normal(loc=0, scale=10, size=1000)
     w = rng.exponential(scale=1, size=1000)
 
     # calculate overall moments
-    OMeanVar(x, weight=w)
+    OMeanVar.compute(x, w)
     # should give: OMeanVar(mean=4.6, var=108, weight=1.08e+03)
 
     # or calculate moments for every group
     df = pd.DataFrame({'g': g, 'x': x, 'w': w})
     omvs = df.groupby('g').apply(OMeanVar.of_frame, x='x', w='w')
 
     # and combine group moments to obtain the same overall results
     OMeanVar.combine(omvs)
 
     # addition is also supported
     omvs.loc[0] + omvs.loc[1]
 
-At the moment, only univariate distributions are supported. Bivariate or even multivariate distributions can be
+At the moment, univariate and bivariate distributions are supported. Bivariate distributions allow for fast linear
+regression with two variables (and constant) calculation. Even multivariate distributions can be
 efficiently processed in a similar fashion, so the support for them might be added in the future. Moments of
 multivariate distributions would also allow for linear regression estimation and other statistical methods
 (such as PCA or regularized regression) to be calculated in a single pass through large distributed datasets.
 
 Similar packages
 ----------------
 
@@ -122,14 +124,14 @@
 ...
 
 `OpenAI Gym
 <https://github.com/openai/gym>`_ (or newly `Gymnasium
 <https://github.com/Farama-Foundation/Gymnasium>`_)
 provides similar functionality as a part of its normalization of observations and rewards
 (in gym.wrappers.normalize.RunningMeanStd). The functionality is fairly limited as it was developed for a particular
-use case, but the calculation is fast and it is possible to compose the results. It does not support weights though.
+use case, but the calculation is fast, and it is possible to compose the results. It does not support weights though.
 
 Documentation
 -------------
 
 - https://protivinsky.github.io/omoment/index.html
```

