# Comparing `tmp/pyportfolioopt-1.5.4.tar.gz` & `tmp/pyportfolioopt-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyportfolioopt-1.5.4.tar", max compression
+gzip compressed data, was "pyportfolioopt-1.5.5.tar", max compression
```

## Comparing `pyportfolioopt-1.5.4.tar` & `pyportfolioopt-1.5.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1077 2021-12-15 21:55:19.433215 pyportfolioopt-1.5.4/LICENSE.txt
--rwxr-xr-x   0        0        0    20940 2022-11-26 16:37:09.526412 pyportfolioopt-1.5.4/README.md
--rwxr-xr-x   0        0        0      767 2022-11-26 16:37:09.532103 pyportfolioopt-1.5.4/pypfopt/__init__.py
--rw-r--r--   0        0        0    24419 2022-11-26 16:37:09.532466 pyportfolioopt-1.5.4/pypfopt/base_optimizer.py
--rw-r--r--   0        0        0    19446 2022-11-26 16:37:09.532847 pyportfolioopt-1.5.4/pypfopt/black_litterman.py
--rw-r--r--   0        0        0    17052 2022-11-26 16:37:09.533107 pyportfolioopt-1.5.4/pypfopt/cla.py
--rw-r--r--   0        0        0    13639 2022-11-26 15:15:33.742282 pyportfolioopt-1.5.4/pypfopt/discrete_allocation.py
--rw-r--r--   0        0        0      494 2021-12-15 21:55:19.459459 pyportfolioopt-1.5.4/pypfopt/efficient_frontier/__init__.py
--rw-r--r--   0        0        0     9590 2022-11-26 16:37:09.533414 pyportfolioopt-1.5.4/pypfopt/efficient_frontier/efficient_cdar.py
--rw-r--r--   0        0        0     9770 2022-11-26 16:37:09.533651 pyportfolioopt-1.5.4/pypfopt/efficient_frontier/efficient_cvar.py
--rw-r--r--   0        0        0    19514 2022-11-26 16:37:09.534102 pyportfolioopt-1.5.4/pypfopt/efficient_frontier/efficient_frontier.py
--rw-r--r--   0        0        0    12911 2022-11-26 16:37:09.534438 pyportfolioopt-1.5.4/pypfopt/efficient_frontier/efficient_semivariance.py
--rw-r--r--   0        0        0      675 2021-12-15 21:55:19.459883 pyportfolioopt-1.5.4/pypfopt/exceptions.py
--rw-r--r--   0        0        0    10639 2022-11-26 16:37:09.534720 pyportfolioopt-1.5.4/pypfopt/expected_returns.py
--rw-r--r--   0        0        0     7764 2021-12-15 21:55:19.460029 pyportfolioopt-1.5.4/pypfopt/hierarchical_portfolio.py
--rw-r--r--   0        0        0     8584 2021-12-15 21:55:19.460111 pyportfolioopt-1.5.4/pypfopt/objective_functions.py
--rw-r--r--   0        0        0     9731 2022-11-26 16:37:09.535107 pyportfolioopt-1.5.4/pypfopt/plotting.py
--rw-r--r--   0        0        0    21228 2021-12-15 21:55:19.460306 pyportfolioopt-1.5.4/pypfopt/risk_models.py
--rw-r--r--   0        0        0     1791 2022-11-26 16:37:09.535411 pyportfolioopt-1.5.4/pyproject.toml
--rw-r--r--   0        0        0    22400 2022-11-26 16:37:22.872474 pyportfolioopt-1.5.4/setup.py
--rw-r--r--   0        0        0    22615 2022-11-26 16:37:22.873291 pyportfolioopt-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2021-12-15 21:55:19.433215 pyportfolioopt-1.5.5/LICENSE.txt
+-rwxr-xr-x   0        0        0    21366 2023-05-07 14:09:52.162598 pyportfolioopt-1.5.5/README.md
+-rwxr-xr-x   0        0        0      766 2023-05-07 14:09:47.536466 pyportfolioopt-1.5.5/pypfopt/__init__.py
+-rw-r--r--   0        0        0    24375 2023-05-07 13:59:56.655694 pyportfolioopt-1.5.5/pypfopt/base_optimizer.py
+-rw-r--r--   0        0        0    19448 2023-05-07 13:59:56.655857 pyportfolioopt-1.5.5/pypfopt/black_litterman.py
+-rw-r--r--   0        0        0    17051 2023-05-07 13:59:56.656002 pyportfolioopt-1.5.5/pypfopt/cla.py
+-rw-r--r--   0        0        0    13493 2023-05-07 13:59:56.656127 pyportfolioopt-1.5.5/pypfopt/discrete_allocation.py
+-rw-r--r--   0        0        0      493 2023-05-07 13:59:56.656222 pyportfolioopt-1.5.5/pypfopt/efficient_frontier/__init__.py
+-rw-r--r--   0        0        0     9591 2023-05-07 13:59:56.656329 pyportfolioopt-1.5.5/pypfopt/efficient_frontier/efficient_cdar.py
+-rw-r--r--   0        0        0     9771 2023-05-07 13:59:56.656432 pyportfolioopt-1.5.5/pypfopt/efficient_frontier/efficient_cvar.py
+-rw-r--r--   0        0        0    19452 2023-05-07 13:59:56.656596 pyportfolioopt-1.5.5/pypfopt/efficient_frontier/efficient_frontier.py
+-rw-r--r--   0        0        0    12906 2023-05-07 13:59:56.656747 pyportfolioopt-1.5.5/pypfopt/efficient_frontier/efficient_semivariance.py
+-rw-r--r--   0        0        0      675 2021-12-15 21:55:19.459883 pyportfolioopt-1.5.5/pypfopt/exceptions.py
+-rw-r--r--   0        0        0    10616 2023-05-07 13:59:56.656887 pyportfolioopt-1.5.5/pypfopt/expected_returns.py
+-rw-r--r--   0        0        0     7765 2023-05-07 13:59:56.657023 pyportfolioopt-1.5.5/pypfopt/hierarchical_portfolio.py
+-rw-r--r--   0        0        0     8584 2023-05-07 13:59:56.657141 pyportfolioopt-1.5.5/pypfopt/objective_functions.py
+-rw-r--r--   0        0        0     9708 2023-05-07 13:59:56.657258 pyportfolioopt-1.5.5/pypfopt/plotting.py
+-rw-r--r--   0        0        0    21212 2023-05-07 13:59:56.657430 pyportfolioopt-1.5.5/pypfopt/risk_models.py
+-rw-r--r--   0        0        0     1955 2023-05-07 14:15:37.680654 pyportfolioopt-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0    22835 2023-05-07 14:21:51.430265 pyportfolioopt-1.5.5/setup.py
+-rw-r--r--   0        0        0    23094 2023-05-07 14:21:51.431086 pyportfolioopt-1.5.5/PKG-INFO
```

### Comparing `pyportfolioopt-1.5.4/LICENSE.txt` & `pyportfolioopt-1.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyportfolioopt-1.5.4/README.md` & `pyportfolioopt-1.5.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 <p align="center">
     <img width=60% src="https://github.com/robertmartin8/PyPortfolioOpt/blob/master/media/logo_v1.png?raw=true">
 </p>
 
 <!-- buttons -->
 <p align="center">
-    <a href="https://www.python.org/">
-        <img src="https://img.shields.io/badge/python-v3-brightgreen.svg"
+    <a href="https://www.python.org">
+        <img src="https://img.shields.io/pypi/pyversions/PyPortfolioOpt.svg"
             alt="python"></a> &nbsp;
+    <a href="https://www.python.org">
+        <img src="https://img.shields.io/badge/Platforms-linux--64,win--64,osx--64-orange.svg?style=flat-square"
+            alt="platforms"></a> &nbsp;
     <a href="https://pypi.org/project/PyPortfolioOpt/">
-        <img src="https://img.shields.io/badge/pypi-v1.5.4-brightgreen.svg"
+        <img src="https://img.shields.io/badge/pypi-v1.5.5-brightgreen.svg"
             alt="pypi"></a> &nbsp;
     <a href="https://opensource.org/licenses/MIT">
         <img src="https://img.shields.io/badge/license-MIT-brightgreen.svg"
             alt="MIT license"></a> &nbsp;
     <a href="https://github.com/robertmartin8/PyPortfolioOpt/actions">
-        <img src="https://github.com/robertmartin8/PyPortfolioOpt/workflows/pytest/badge.svg?event=push"
+        <img src="https://github.com/robertmartin8/PyPortfolioOpt/workflows/pytest/badge.svg?branch=master"
             alt="build"></a> &nbsp;
+    <a href="https://app.codecov.io/gh/robertmartin8/PyPortfolioOpt">
+        <img src="https://codecov.io/github/robertmartin8/PyPortfolioOpt/coverage.svg?branch=main"
+            alt="codecov"></a> &nbsp;
     <a href="https://pepy.tech/project/pyportfolioopt">
         <img src="https://pepy.tech/badge/pyportfolioopt"
             alt="downloads"></a> &nbsp;
     <a href="https://mybinder.org/v2/gh/robertmartin8/pyportfolioopt/master/?filepath=cookbook">
       <img src="https://mybinder.org/badge_logo.svg"
             alt="binder"></a> &nbsp;
 </p>
 
 <!-- content -->
-**PyPortfolioOpt is looking for maintainers! Please reach out to the email address at the bottom of the readme if you're interested**
 
 PyPortfolioOpt is a library that implements portfolio optimization methods, including
 classical mean-variance optimization techniques and Black-Litterman allocation, as well as more
 recent developments in the field like shrinkage and Hierarchical Risk Parity.
 
 It is **extensive** yet easily **extensible**, and can be useful for either a casual investors, or a professional looking for an easy prototyping tool. Whether you are a fundamentals-oriented investor who has identified a
 handful of undervalued picks, or an algorithmic trader who has a basket of
 strategies, PyPortfolioOpt can help you combine your alpha sources
 in a risk-efficient way.
 
 **PyPortfolioOpt has been [published](https://joss.theoj.org/papers/10.21105/joss.03066) in the Journal of Open Source Software 🎉**
 
+PyPortfolioOpt is now being maintained by [Tuan Tran](https://github.com/88d52bdba0366127fffca9dfa93895).
+
 Head over to the **[documentation on ReadTheDocs](https://pyportfolioopt.readthedocs.io/en/latest/)** to get an in-depth look at the project, or check out the [cookbook](https://github.com/robertmartin8/PyPortfolioOpt/tree/master/cookbook) to see some examples showing the full process from downloading data to building a portfolio.
 
 <center>
 <img src="https://github.com/robertmartin8/PyPortfolioOpt/blob/master/media/conceptual_flowchart_v2.png?raw=true" style="width:70%;"/>
 </center>
 
 ## Table of contents
@@ -76,15 +83,15 @@
 
 This project is available on PyPI, meaning that you can just:
 
 ```bash
 pip install PyPortfolioOpt
 ```
 
-(you may need to follow separate installation instructions for [cvxopt](https://cvxopt.org/install/index.html#) and [cvxpy](https://www.cvxpy.org/install/))).
+(you may need to follow separate installation instructions for [cvxopt](https://cvxopt.org/install/index.html#) and [cvxpy](https://www.cvxpy.org/install/)).
 
 However, it is best practice to use a dependency manager within a virtual environment.
 My current recommendation is to get yourself set up with [poetry](https://github.com/sdispater/poetry) then just run
 
 ```bash
 poetry add PyPortfolioOpt
 ```
@@ -414,14 +421,15 @@
 ## Contributing
 
 Contributions are _most welcome_. Have a look at the [Contribution Guide](https://github.com/robertmartin8/PyPortfolioOpt/blob/master/CONTRIBUTING.md) for more.
 
 I'd like to thank all of the people who have contributed to PyPortfolioOpt since its release in 2018.
 Special shout-outs to:
 
+-   Tuan Tran (who is now the primary maintainer!)
 -   Philipp Schiele
 -   Carl Peasnell
 -   Felipe Schneider
 -   Dingyuan Wang
 -   Pat Newell
 -   Aditya Bhutra
 -   Thomas Schmelzer
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
       [https://github.com/robertmartin8/PyPortfolioOpt/blob/master/media/
                              logo_v1.png?raw=true]
-    [python]   [pypi]   [MIT_license]   [build]   [downloads]   [binder]  
- **PyPortfolioOpt is looking for maintainers! Please reach out to the email
-address at the bottom of the readme if you're interested** PyPortfolioOpt is a
-library that implements portfolio optimization methods, including classical
-mean-variance optimization techniques and Black-Litterman allocation, as well
-as more recent developments in the field like shrinkage and Hierarchical Risk
-Parity. It is **extensive** yet easily **extensible**, and can be useful for
-either a casual investors, or a professional looking for an easy prototyping
-tool. Whether you are a fundamentals-oriented investor who has identified a
-handful of undervalued picks, or an algorithmic trader who has a basket of
-strategies, PyPortfolioOpt can help you combine your alpha sources in a risk-
-efficient way. **PyPortfolioOpt has been [published](https://joss.theoj.org/
-papers/10.21105/joss.03066) in the Journal of Open Source Software ð** Head
-over to the **[documentation on ReadTheDocs](https://
-pyportfolioopt.readthedocs.io/en/latest/)** to get an in-depth look at the
-project, or check out the [cookbook](https://github.com/robertmartin8/
-PyPortfolioOpt/tree/master/cookbook) to see some examples showing the full
-process from downloading data to building a portfolio.
+   [python]   [platforms]   [pypi]   [MIT_license]   [build]   [codecov]  
+                           [downloads]   [binder]  
+ PyPortfolioOpt is a library that implements portfolio optimization methods,
+including classical mean-variance optimization techniques and Black-Litterman
+allocation, as well as more recent developments in the field like shrinkage and
+Hierarchical Risk Parity. It is **extensive** yet easily **extensible**, and
+can be useful for either a casual investors, or a professional looking for an
+easy prototyping tool. Whether you are a fundamentals-oriented investor who has
+identified a handful of undervalued picks, or an algorithmic trader who has a
+basket of strategies, PyPortfolioOpt can help you combine your alpha sources in
+a risk-efficient way. **PyPortfolioOpt has been [published](https://
+joss.theoj.org/papers/10.21105/joss.03066) in the Journal of Open Source
+Software ð** PyPortfolioOpt is now being maintained by [Tuan Tran](https://
+github.com/88d52bdba0366127fffca9dfa93895). Head over to the **[documentation
+on ReadTheDocs](https://pyportfolioopt.readthedocs.io/en/latest/)** to get an
+in-depth look at the project, or check out the [cookbook](https://github.com/
+robertmartin8/PyPortfolioOpt/tree/master/cookbook) to see some examples showing
+the full process from downloading data to building a portfolio.
       [https://github.com/robertmartin8/PyPortfolioOpt/blob/master/media/
                      conceptual_flowchart_v2.png?raw=true]
 ## Table of contents - [Table of contents](#table-of-contents) - [Getting
 started](#getting-started) - [For development](#for-development) - [A quick
 example](#a-quick-example) - [An overview of classical portfolio optimization
 methods](#an-overview-of-classical-portfolio-optimization-methods) - [Features]
 (#features) - [Expected returns](#expected-returns) - [Risk models
@@ -42,15 +42,15 @@
 if you are on windows, you first need to installl C++. ([download](https://
 visualstudio.microsoft.com/thank-you-downloading-visual-studio/
 ?sku=BuildTools&rel=16), [install instructions](https://drive.google.com/file/
 d/0B4GsMXCRaSSIOWpYQkstajlYZ0tPVkNQSElmTWh1dXFaYkJr/view))_ This project is
 available on PyPI, meaning that you can just: ```bash pip install
 PyPortfolioOpt ``` (you may need to follow separate installation instructions
 for [cvxopt](https://cvxopt.org/install/index.html#) and [cvxpy](https://
-www.cvxpy.org/install/))). However, it is best practice to use a dependency
+www.cvxpy.org/install/)). However, it is best practice to use a dependency
 manager within a virtual environment. My current recommendation is to get
 yourself set up with [poetry](https://github.com/sdispater/poetry) then just
 run ```bash poetry add PyPortfolioOpt ``` Otherwise, clone/download the project
 and in the project directory run: ```bash python setup.py install ```
 PyPortfolioOpt supports Docker. Build your first container with `docker build -
 f docker/Dockerfile . -t pypfopt`. You can use the image to run tests or even
 launch a Jupyter server. ```bash # iPython interpreter: docker run -it pypfopt
@@ -246,14 +246,14 @@
 doi.org/10.21105/joss.03066}, year = {2021}, publisher = {The Open Journal},
 volume = {6}, number = {61}, pages = {3066}, author = {Robert Andrew Martin},
 title = {PyPortfolioOpt: portfolio optimization in Python}, journal = {Journal
 of Open Source Software} } ``` ## Contributing Contributions are _most
 welcome_. Have a look at the [Contribution Guide](https://github.com/
 robertmartin8/PyPortfolioOpt/blob/master/CONTRIBUTING.md) for more. I'd like to
 thank all of the people who have contributed to PyPortfolioOpt since its
-release in 2018. Special shout-outs to: - Philipp Schiele - Carl Peasnell -
-Felipe Schneider - Dingyuan Wang - Pat Newell - Aditya Bhutra - Thomas
-Schmelzer - Rich Caputo - Nicolas Knudde ## Getting in touch If you are having
-a problem with PyPortfolioOpt, please raise a GitHub issue. For anything else,
-you can reach me at:
+release in 2018. Special shout-outs to: - Tuan Tran (who is now the primary
+maintainer!) - Philipp Schiele - Carl Peasnell - Felipe Schneider - Dingyuan
+Wang - Pat Newell - Aditya Bhutra - Thomas Schmelzer - Rich Caputo - Nicolas
+Knudde ## Getting in touch If you are having a problem with PyPortfolioOpt,
+please raise a GitHub issue. For anything else, you can reach me at:
  [https://github.com/robertmartin8/ReasonableDeviations/blob/gh-pages/assets/
                          images/contact.png?raw=true]
```

### Comparing `pyportfolioopt-1.5.4/pypfopt/base_optimizer.py` & `pyportfolioopt-1.5.5/pypfopt/base_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,20 @@
 import collections
 import copy
 import json
 import warnings
 from collections.abc import Iterable
 from typing import List
 
+import cvxpy as cp
 import numpy as np
 import pandas as pd
-import cvxpy as cp
 import scipy.optimize as sco
 
-from . import objective_functions
-from . import exceptions
+from . import exceptions, objective_functions
 
 
 class BaseOptimizer:
 
     """
     Instance variables:
 
@@ -160,15 +159,15 @@
     ):
         """
         :param weight_bounds: minimum and maximum weight of each asset OR single min/max pair
                               if all identical, defaults to (0, 1). Must be changed to (-1, 1)
                               for portfolios with shorting.
         :type weight_bounds: tuple OR tuple list, optional
         :param solver: name of solver. list available solvers with: ``cvxpy.installed_solvers()``
-        :type solver: str, optional. Defaults to "ECOS"
+        :type solver: str, optional.
         :param verbose: whether performance and debugging info should be printed, defaults to False
         :type verbose: bool, optional
         :param solver_options: parameters for the given solver
         :type solver_options: dict, optional
         """
         super().__init__(n_assets, tickers)
 
@@ -217,16 +216,15 @@
             bounds = np.array(test_bounds, dtype=float)
             self._lower_bounds = np.nan_to_num(bounds[:, 0], nan=-np.inf)
             self._upper_bounds = np.nan_to_num(bounds[:, 1], nan=np.inf)
         else:
             # Otherwise this must be a pair.
             if len(test_bounds) != 2 or not isinstance(test_bounds, (tuple, list)):
                 raise TypeError(
-                    "test_bounds must be a pair (lower bound, upper bound) "
-                    "OR a collection of bounds for each asset"
+                    "test_bounds must be a pair (lower bound, upper bound) OR a collection of bounds for each asset"
                 )
             lower, upper = test_bounds
 
             # Replace None values with the appropriate +/- 1
             if np.isscalar(lower) or lower is None:
                 lower = -1 if lower is None else lower
                 self._lower_bounds = np.array([lower] * self.n_assets)
@@ -394,18 +392,18 @@
         :type sector_upper: {str:float} dict
         """
         if np.any(self._lower_bounds < 0):
             warnings.warn(
                 "Sector constraints may not produce reasonable results if shorts are allowed."
             )
         for sector in sector_upper:
-            is_sector = [sector_mapper[t] == sector for t in self.tickers]
+            is_sector = [sector_mapper.get(t) == sector for t in self.tickers]
             self.add_constraint(lambda w: cp.sum(w[is_sector]) <= sector_upper[sector])
         for sector in sector_lower:
-            is_sector = [sector_mapper[t] == sector for t in self.tickers]
+            is_sector = [sector_mapper.get(t) == sector for t in self.tickers]
             self.add_constraint(lambda w: cp.sum(w[is_sector]) >= sector_lower[sector])
 
     def convex_objective(self, custom_objective, weights_sum_to_one=True, **kwargs):
         """
         Optimize a custom convex objective function. Constraints should be added with
         ``ef.add_constraint()``. Optimizer arguments must be passed as keyword-args. Example::
 
@@ -589,14 +587,14 @@
     """
     if expression.args == []:
         return [expression]
     else:
         return list(_flatten([_get_all_args(arg) for arg in expression.args]))
 
 
-def _flatten(l: Iterable) -> Iterable:
+def _flatten(alist: Iterable) -> Iterable:
     # Helper method to flatten an iterable
-    for el in l:
-        if isinstance(el, Iterable) and not isinstance(el, (str, bytes)):
-            yield from _flatten(el)
+    for v in alist:
+        if isinstance(v, Iterable) and not isinstance(v, (str, bytes)):
+            yield from _flatten(v)
         else:
-            yield el
+            yield v
```

### Comparing `pyportfolioopt-1.5.4/pypfopt/black_litterman.py` & `pyportfolioopt-1.5.5/pypfopt/black_litterman.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 views. In addition, two utility functions are defined, which calculate:
 
 - market-implied prior estimate of returns
 - market-implied risk-aversion parameter
 """
 import sys
 import warnings
+
 import numpy as np
 import pandas as pd
+
 from . import base_optimizer
 
 
 def market_implied_prior_returns(
     market_caps, risk_aversion, cov_matrix, risk_free_rate=0.02
 ):
     r"""
```

### Comparing `pyportfolioopt-1.5.4/pypfopt/cla.py` & `pyportfolioopt-1.5.5/pypfopt/cla.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 The ``cla`` module houses the CLA class, which
 generates optimal portfolios using the Critical Line Algorithm as implemented
 by Marcos Lopez de Prado and David Bailey.
 """
 
 import numpy as np
 import pandas as pd
+
 from . import base_optimizer
 
 
 class CLA(base_optimizer.BaseOptimizer):
 
     """
     Instance variables:
@@ -217,15 +218,15 @@
             if abs(sum(self.w[i]) - 1) > tol:
                 flag = True
             else:
                 for j in range(self.w[i].shape[0]):
                     if (
                         self.w[i][j] - self.lB[j] < -tol
                         or self.w[i][j] - self.uB[j] > tol
-                    ):  #  pragma: no cover
+                    ):  # pragma: no cover
                         flag = True
                         break
             if flag is True:
                 del self.w[i]
                 del self.ls[i]
                 del self.g[i]
                 del self.f[i]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyportfolioopt-1.5.4/pypfopt/discrete_allocation.py` & `pyportfolioopt-1.5.5/pypfopt/discrete_allocation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 The ``discrete_allocation`` module contains the ``DiscreteAllocation`` class, which
 offers multiple methods to generate a discrete portfolio allocation from continuous weights.
 """
 import collections
+
+import cvxpy as cp
 import numpy as np
 import pandas as pd
-import cvxpy as cp
+
 from . import exceptions
 
 
 def get_latest_prices(prices):
     """
     A helper tool which retrieves the most recent asset prices from a dataframe of
     asset prices, required in order to generate a discrete allocation.
@@ -315,17 +317,14 @@
         # Set up linear program
         eta = w * self.total_portfolio_value - cp.multiply(x, p)
         u = cp.Variable(n)
         constraints = [eta <= u, eta >= -u, x >= 0, r >= 0]
         objective = cp.sum(u) + r
 
         opt = cp.Problem(cp.Minimize(objective), constraints)
-
-        if solver is not None and solver not in cp.installed_solvers():
-            raise NameError("Solver {} is not installed. ".format(solver))
         opt.solve(solver=solver)
 
         if opt.status not in {"optimal", "optimal_inaccurate"}:  # pragma: no cover
             raise exceptions.OptimizationError("Please try greedy_portfolio")
 
         vals = np.rint(x.value).astype(int)
         self.allocation = self._remove_zero_positions(
```

### Comparing `pyportfolioopt-1.5.4/pypfopt/efficient_frontier/efficient_cdar.py` & `pyportfolioopt-1.5.5/pypfopt/efficient_frontier/efficient_cdar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 The ``efficient_cdar`` submodule houses the EfficientCDaR class, which
 generates portfolios along the mean-CDaR (conditional drawdown-at-risk) frontier.
 """
 
 import warnings
-import numpy as np
+
 import cvxpy as cp
+import numpy as np
 
 from .. import objective_functions
 from .efficient_frontier import EfficientFrontier
 
 
 class EfficientCDaR(EfficientFrontier):
     """
```

### Comparing `pyportfolioopt-1.5.4/pypfopt/efficient_frontier/efficient_cvar.py` & `pyportfolioopt-1.5.5/pypfopt/efficient_frontier/efficient_cvar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 The ``efficient_cvar`` submodule houses the EfficientCVaR class, which
 generates portfolios along the mean-CVaR frontier.
 """
 
 import warnings
-import numpy as np
+
 import cvxpy as cp
+import numpy as np
 
 from .. import objective_functions
 from .efficient_frontier import EfficientFrontier
 
 
 class EfficientCVaR(EfficientFrontier):
     """
```

### Comparing `pyportfolioopt-1.5.4/pypfopt/efficient_frontier/efficient_frontier.py` & `pyportfolioopt-1.5.5/pypfopt/efficient_frontier/efficient_frontier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 The ``efficient_frontier`` submodule houses the EfficientFrontier class, which generates
 classical mean-variance optimal portfolios for a variety of objectives and constraints
 """
 import warnings
 
+import cvxpy as cp
 import numpy as np
 import pandas as pd
-import cvxpy as cp
 
-from .. import exceptions
-from .. import objective_functions, base_optimizer
+from .. import base_optimizer, exceptions, objective_functions
 
 
 class EfficientFrontier(base_optimizer.BaseConvexOptimizer):
 
     """
     An EfficientFrontier object (inheriting from BaseConvexOptimizer) contains multiple
     optimization methods that can be called (corresponding to different objective
@@ -79,18 +78,16 @@
         :type verbose: bool, optional
         :param solver_options: parameters for the given solver
         :type solver_options: dict, optional
         :raises TypeError: if ``expected_returns`` is not a series, list or array
         :raises TypeError: if ``cov_matrix`` is not a dataframe or array
         """
         # Inputs
-        self.cov_matrix = EfficientFrontier._validate_cov_matrix(cov_matrix)
-        self.expected_returns = EfficientFrontier._validate_expected_returns(
-            expected_returns
-        )
+        self.cov_matrix = self._validate_cov_matrix(cov_matrix)
+        self.expected_returns = self._validate_expected_returns(expected_returns)
         self._max_return_value = None
         self._market_neutral = None
 
         if self.expected_returns is None:
             num_assets = len(cov_matrix)
         else:
             num_assets = len(expected_returns)
```

### Comparing `pyportfolioopt-1.5.4/pypfopt/efficient_frontier/efficient_semivariance.py` & `pyportfolioopt-1.5.5/pypfopt/efficient_frontier/efficient_semivariance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The ``efficient_semivariance`` submodule houses the EfficientSemivariance class, which
 generates portfolios along the mean-semivariance frontier.
 """
 
 
-import numpy as np
 import cvxpy as cp
+import numpy as np
 
 from .. import objective_functions
 from .efficient_frontier import EfficientFrontier
 
 
 class EfficientSemivariance(EfficientFrontier):
     """
@@ -181,28 +181,28 @@
         :return: asset weights for the efficient risk portfolio
         :rtype: OrderedDict
         """
         update_existing_parameter = self.is_parameter_defined("target_semivariance")
         if update_existing_parameter:
             self._validate_market_neutral(market_neutral)
             self.update_parameter_value(
-                "target_semivariance", target_semideviation ** 2
+                "target_semivariance", target_semideviation**2
             )
         else:
             self._objective = objective_functions.portfolio_return(
                 self._w, self.expected_returns
             )
             for obj in self._additional_objectives:
                 self._objective += obj
 
             p = cp.Variable(self._T, nonneg=True)
             n = cp.Variable(self._T, nonneg=True)
 
             target_semivariance = cp.Parameter(
-                value=target_semideviation ** 2, name="target_semivariance", nonneg=True
+                value=target_semideviation**2, name="target_semivariance", nonneg=True
             )
             self.add_constraint(
                 lambda _: self.frequency * cp.sum(cp.square(n)) <= target_semivariance
             )
             B = (self.returns.values - self.benchmark) / np.sqrt(self._T)
             self.add_constraint(lambda w: B @ w - p + n == 0)
             self._make_weight_sum_constraint(market_neutral)
@@ -230,15 +230,14 @@
             )
 
         update_existing_parameter = self.is_parameter_defined("target_return")
         if update_existing_parameter:
             self._validate_market_neutral(market_neutral)
             self.update_parameter_value("target_return", target_return)
         else:
-
             p = cp.Variable(self._T, nonneg=True)
             n = cp.Variable(self._T, nonneg=True)
             self._objective = cp.sum(cp.square(n))
             for obj in self._additional_objectives:
                 self._objective += obj
 
             target_return_par = cp.Parameter(name="target_return", value=target_return)
```

### Comparing `pyportfolioopt-1.5.4/pypfopt/exceptions.py` & `pyportfolioopt-1.5.5/pypfopt/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyportfolioopt-1.5.4/pypfopt/expected_returns.py` & `pyportfolioopt-1.5.5/pypfopt/expected_returns.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,17 @@
     - exponentially weighted mean historical return
     - CAPM estimate of returns
 
 Additionally, we provide utility functions to convert from returns to prices and vice-versa.
 """
 
 import warnings
-import pandas as pd
+
 import numpy as np
+import pandas as pd
 
 
 def _check_returns(returns):
     # Check NaNs excluding leading NaNs
     if np.any(np.isnan(returns.mask(returns.ffill().isnull(), 0))):
         warnings.warn(
             "Some returns are NaN. Please check your price data.", UserWarning
@@ -243,20 +244,20 @@
 
     if returns_data:
         returns = prices.copy()
         if market_prices is not None:
             market_returns = market_prices
     else:
         returns = returns_from_prices(prices, log_returns)
-        
+
         if market_prices is not None:
             if not isinstance(market_prices, pd.DataFrame):
                 warnings.warn("market prices are not in a dataframe", RuntimeWarning)
                 market_prices = pd.DataFrame(market_prices)
-                
+
             market_returns = returns_from_prices(market_prices, log_returns)
     # Use the equally-weighted dataset as a proxy for the market
     if market_returns is None:
         # Append market return to right and compute sample covariance matrix
         returns["mkt"] = returns.mean(axis=1)
     else:
         market_returns.columns = ["mkt"]
```

### Comparing `pyportfolioopt-1.5.4/pypfopt/hierarchical_portfolio.py` & `pyportfolioopt-1.5.5/pypfopt/hierarchical_portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 Currently implemented:
 
 - ``HRPOpt`` implements the Hierarchical Risk Parity (HRP) portfolio. Code reproduced with
   permission from Marcos Lopez de Prado (2016).
 """
 
 import collections
+
 import numpy as np
 import pandas as pd
 import scipy.cluster.hierarchy as sch
 import scipy.spatial.distance as ssd
 
 from . import base_optimizer, risk_models
```

### Comparing `pyportfolioopt-1.5.4/pypfopt/objective_functions.py` & `pyportfolioopt-1.5.5/pypfopt/objective_functions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 - L2 regularisation (minimising this reduces nonzero weights)
 - Quadratic utility
 - Transaction cost model (a simple one)
 - Ex-ante (squared) tracking error
 - Ex-post (squared) tracking error
 """
 
-import numpy as np
 import cvxpy as cp
+import numpy as np
 
 
 def _objective_value(w, obj):
     """
     Helper method to return either the value of the objective function
     or the objective function as a cvxpy object depending on whether
     w is a cvxpy variable or np array.
```

### Comparing `pyportfolioopt-1.5.4/pypfopt/plotting.py` & `pyportfolioopt-1.5.5/pypfopt/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 Currently implemented:
 
   - ``plot_covariance`` - plot a correlation matrix
   - ``plot_dendrogram`` - plot the hierarchical clusters in a portfolio
   - ``plot_efficient_frontier`` – plot the efficient frontier from an EfficientFrontier or CLA object
   - ``plot_weights`` - bar chart of weights
 """
-import copy
+import warnings
+
 import numpy as np
-from . import risk_models, exceptions
-from . import EfficientFrontier, CLA
 import scipy.cluster.hierarchy as sch
-import warnings
+
+from . import CLA, EfficientFrontier, exceptions, risk_models
 
 try:
     import matplotlib.pyplot as plt
 
     plt.style.use("seaborn-deep")
 except (ModuleNotFoundError, ImportError):  # pragma: no cover
     raise ImportError("Please install matplotlib via pip or poetry")
```

### Comparing `pyportfolioopt-1.5.4/pypfopt/risk_models.py` & `pyportfolioopt-1.5.5/pypfopt/risk_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,18 @@
     - Ledoit Wolf shrinkage
     - Oracle Approximating shrinkage
 
 - covariance to correlation matrix
 """
 
 import warnings
+
 import numpy as np
 import pandas as pd
+
 from .expected_returns import returns_from_prices
 
 
 def _is_positive_semidefinite(matrix):
     """
     Helper function to check if a given matrix is positive semidefinite.
     Any method that requires inverting the covariance matrix will struggle
@@ -482,31 +484,31 @@
         varmkt = sample[n, n]
         sample = sample[:n, :n]
         F = np.dot(betas, betas.T) / varmkt
         F[np.eye(n) == 1] = np.diag(sample)
 
         # compute shrinkage parameters
         c = np.linalg.norm(sample - F, "fro") ** 2
-        y = Xm ** 2
-        p = 1 / t * np.sum(np.dot(y.T, y)) - np.sum(sample ** 2)
+        y = Xm**2
+        p = 1 / t * np.sum(np.dot(y.T, y)) - np.sum(sample**2)
 
         # r is divided into diagonal
         # and off-diagonal terms, and the off-diagonal term
         # is itself divided into smaller terms
-        rdiag = 1 / t * np.sum(y ** 2) - sum(np.diag(sample) ** 2)
+        rdiag = 1 / t * np.sum(y**2) - sum(np.diag(sample) ** 2)
         z = Xm * np.tile(xmkt, (n,))
         v1 = 1 / t * np.dot(y.T, z) - np.tile(betas, (n,)) * sample
         roff1 = (
             np.sum(v1 * np.tile(betas, (n,)).T) / varmkt
             - np.sum(np.diag(v1) * betas.T) / varmkt
         )
         v3 = 1 / t * np.dot(z.T, z) - varmkt * sample
         roff3 = (
-            np.sum(v3 * np.dot(betas, betas.T)) / varmkt ** 2
-            - np.sum(np.diag(v3).reshape(-1, 1) * betas ** 2) / varmkt ** 2
+            np.sum(v3 * np.dot(betas, betas.T)) / varmkt**2
+            - np.sum(np.diag(v3).reshape(-1, 1) * betas**2) / varmkt**2
         )
         roff = 2 * roff1 - roff3
         r = rdiag + roff
 
         # compute shrinkage constant
         k = (p - r) / c
         delta = max(0, min(1, k / t))
@@ -536,20 +538,20 @@
         _std = np.tile(std, (n,))
         r_bar = (np.sum(S / (_std * _std.T)) - n) / (n * (n - 1))
         F = r_bar * (_std * _std.T)
         F[np.eye(n) == 1] = var.reshape(-1)
 
         # Estimate pi
         Xm = X - X.mean(axis=0)
-        y = Xm ** 2
-        pi_mat = np.dot(y.T, y) / t - 2 * np.dot(Xm.T, Xm) * S / t + S ** 2
+        y = Xm**2
+        pi_mat = np.dot(y.T, y) / t - 2 * np.dot(Xm.T, Xm) * S / t + S**2
         pi_hat = np.sum(pi_mat)
 
         # Theta matrix, expanded term by term
-        term1 = np.dot((Xm ** 3).T, Xm) / t
+        term1 = np.dot((Xm**3).T, Xm) / t
         help_ = np.dot(Xm.T, Xm) / t
         help_diag = np.diag(help_)
         term2 = np.tile(help_diag, (n, 1)).T * S
         term3 = help_ * _var
         term4 = _var * S
         theta_mat = term1 - term2 - term3 + term4
         theta_mat[np.eye(n) == 1] = np.zeros(n)
```

### Comparing `pyportfolioopt-1.5.4/pyproject.toml` & `pyportfolioopt-1.5.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyportfolioopt"
-version = "1.5.4"
+version = "1.5.5"
 description = "Financial portfolio optimization in python"
 license = "MIT"
 authors = ["Robert Andrew Martin <martin.robertandrew@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/robertmartin8/PyPortfolioOpt"
 documentation = "https://pyportfolioopt.readthedocs.io/en/latest/"
 keywords= ["finance", "portfolio", "optimization", "quant", "investing"]
@@ -12,45 +12,53 @@
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Financial and Insurance Industry",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Office/Business :: Financial",
         "Topic :: Office/Business :: Financial :: Investment",
     ]
 packages = [ {include = "pypfopt"} ]
 
 [tool.poetry.urls]
 "Issues" = "https://github.com/robertmartin8/PyPortfolioOpt/issues"
 "Personal website" = "https://reasonabledeviations.com"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.15"
 scipy = "^1.3"
 pandas = ">=0.19"
-cvxpy = "^1.1.10"
+cvxpy = "^1.1.19"
 numpy = "^1.22.4"
-matplotlib = { version="^3.5.2", optional=true }
-scikit-learn = { version="^1.1.1", optional=true }
+matplotlib = { version="^3.2.0", optional=true }
+scikit-learn = { version="^0.24.1", optional=true }
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 flake8 = "^4.0.1"
 jupyterlab = "^3.4.2"
 black = "^22.3.0"
 ipykernel = "^6.13.0"
 jedi = "^0.18.1"
 pytest-cov = "^3.0.0"
 yfinance = "^0.1.70"
 
 [tool.poetry.extras]
 optionals = ["scikit-learn", "matplotlib", "cvxopt"]
 
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+
+[tool.black]
+line-length = 88
+
+[tool.isort]
+profile = "black"
```

### Comparing `pyportfolioopt-1.5.4/setup.py` & `pyportfolioopt-1.5.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 packages = \
 ['pypfopt', 'pypfopt.efficient_frontier']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['cvxpy>=1.1.10,<2.0.0',
+['cvxpy>=1.1.19,<2.0.0',
  'numpy>=1.22.4,<2.0.0',
  'pandas>=0.19',
  'scipy>=1.3,<2.0']
 
 extras_require = \
-{'optionals': ['matplotlib>=3.5.2,<4.0.0', 'scikit-learn>=1.1.1,<2.0.0']}
+{'optionals': ['matplotlib>=3.2.0,<4.0.0', 'scikit-learn>=0.24.1,<0.25.0']}
 
 setup_kwargs = {
     'name': 'pyportfolioopt',
-    'version': '1.5.4',
+    'version': '1.5.5',
     'description': 'Financial portfolio optimization in python',
-    'long_description': '<p align="center">\n    <img width=60% src="https://github.com/robertmartin8/PyPortfolioOpt/blob/master/media/logo_v1.png?raw=true">\n</p>\n\n<!-- buttons -->\n<p align="center">\n    <a href="https://www.python.org/">\n        <img src="https://img.shields.io/badge/python-v3-brightgreen.svg"\n            alt="python"></a> &nbsp;\n    <a href="https://pypi.org/project/PyPortfolioOpt/">\n        <img src="https://img.shields.io/badge/pypi-v1.5.4-brightgreen.svg"\n            alt="pypi"></a> &nbsp;\n    <a href="https://opensource.org/licenses/MIT">\n        <img src="https://img.shields.io/badge/license-MIT-brightgreen.svg"\n            alt="MIT license"></a> &nbsp;\n    <a href="https://github.com/robertmartin8/PyPortfolioOpt/actions">\n        <img src="https://github.com/robertmartin8/PyPortfolioOpt/workflows/pytest/badge.svg?event=push"\n            alt="build"></a> &nbsp;\n    <a href="https://pepy.tech/project/pyportfolioopt">\n        <img src="https://pepy.tech/badge/pyportfolioopt"\n            alt="downloads"></a> &nbsp;\n    <a href="https://mybinder.org/v2/gh/robertmartin8/pyportfolioopt/master/?filepath=cookbook">\n      <img src="https://mybinder.org/badge_logo.svg"\n            alt="binder"></a> &nbsp;\n</p>\n\n<!-- content -->\n**PyPortfolioOpt is looking for maintainers! Please reach out to the email address at the bottom of the readme if you\'re interested**\n\nPyPortfolioOpt is a library that implements portfolio optimization methods, including\nclassical mean-variance optimization techniques and Black-Litterman allocation, as well as more\nrecent developments in the field like shrinkage and Hierarchical Risk Parity.\n\nIt is **extensive** yet easily **extensible**, and can be useful for either a casual investors, or a professional looking for an easy prototyping tool. Whether you are a fundamentals-oriented investor who has identified a\nhandful of undervalued picks, or an algorithmic trader who has a basket of\nstrategies, PyPortfolioOpt can help you combine your alpha sources\nin a risk-efficient way.\n\n**PyPortfolioOpt has been [published](https://joss.theoj.org/papers/10.21105/joss.03066) in the Journal of Open Source Software 🎉**\n\nHead over to the **[documentation on ReadTheDocs](https://pyportfolioopt.readthedocs.io/en/latest/)** to get an in-depth look at the project, or check out the [cookbook](https://github.com/robertmartin8/PyPortfolioOpt/tree/master/cookbook) to see some examples showing the full process from downloading data to building a portfolio.\n\n<center>\n<img src="https://github.com/robertmartin8/PyPortfolioOpt/blob/master/media/conceptual_flowchart_v2.png?raw=true" style="width:70%;"/>\n</center>\n\n## Table of contents\n\n-   [Table of contents](#table-of-contents)\n-   [Getting started](#getting-started)\n    -   [For development](#for-development)\n-   [A quick example](#a-quick-example)\n-   [An overview of classical portfolio optimization methods](#an-overview-of-classical-portfolio-optimization-methods)\n-   [Features](#features)\n    -   [Expected returns](#expected-returns)\n    -   [Risk models (covariance)](#risk-models-covariance)\n    -   [Objective functions](#objective-functions)\n    -   [Adding constraints or different objectives](#adding-constraints-or-different-objectives)\n    -   [Black-Litterman allocation](#black-litterman-allocation)\n    -   [Other optimizers](#other-optimizers)\n-   [Advantages over existing implementations](#advantages-over-existing-implementations)\n-   [Project principles and design decisions](#project-principles-and-design-decisions)\n-   [Testing](#testing)\n-   [Citing PyPortfolioOpt](#citing-pyportfolioopt)\n-   [Contributing](#contributing)\n-   [Getting in touch](#getting-in-touch)\n\n## Getting started\n\nIf you would like to play with PyPortfolioOpt interactively in your browser, you may launch Binder [here](https://mybinder.org/v2/gh/robertmartin8/pyportfolioopt/master). It takes a\nwhile to set up, but it lets you try out the cookbook recipes without having to deal with all of the requirements.\n\n_Note: macOS users will need to install [Command Line Tools](https://osxdaily.com/2014/02/12/install-command-line-tools-mac-os-x/)._\n\n_Note: if you are on windows, you first need to installl C++. ([download](https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=BuildTools&rel=16), [install instructions](https://drive.google.com/file/d/0B4GsMXCRaSSIOWpYQkstajlYZ0tPVkNQSElmTWh1dXFaYkJr/view))_\n\nThis project is available on PyPI, meaning that you can just:\n\n```bash\npip install PyPortfolioOpt\n```\n\n(you may need to follow separate installation instructions for [cvxopt](https://cvxopt.org/install/index.html#) and [cvxpy](https://www.cvxpy.org/install/))).\n\nHowever, it is best practice to use a dependency manager within a virtual environment.\nMy current recommendation is to get yourself set up with [poetry](https://github.com/sdispater/poetry) then just run\n\n```bash\npoetry add PyPortfolioOpt\n```\n\nOtherwise, clone/download the project and in the project directory run:\n\n```bash\npython setup.py install\n```\n\nPyPortfolioOpt supports Docker. Build your first container with `docker build -f docker/Dockerfile . -t pypfopt`. You can use the image to run tests or even launch a Jupyter server.\n\n```bash\n# iPython interpreter:\ndocker run -it pypfopt poetry run ipython\n\n# Jupyter notebook server:\ndocker run -it -p 8888:8888 pypfopt poetry run jupyter notebook --allow-root --no-browser --ip 0.0.0.0\n# click on http://127.0.0.1:8888/?token=xxx\n\n# Pytest\ndocker run -t pypfopt poetry run pytest\n\n# Bash\ndocker run -it pypfopt bash\n```\n\nFor more information, please read [this guide](https://docker-curriculum.com/#introduction).\n\n### For development\n\nIf you would like to make major changes to integrate this with your proprietary system, it probably makes sense to clone this repository and to just use the source code.\n\n```bash\ngit clone https://github.com/robertmartin8/PyPortfolioOpt\n```\n\nAlternatively, you could try:\n\n```bash\npip install -e git+https://github.com/robertmartin8/PyPortfolioOpt.git\n```\n\n## A quick example\n\nHere is an example on real life stock data, demonstrating how easy it is to find the long-only portfolio that maximises the Sharpe ratio (a measure of risk-adjusted returns).\n\n```python\nimport pandas as pd\nfrom pypfopt import EfficientFrontier\nfrom pypfopt import risk_models\nfrom pypfopt import expected_returns\n\n# Read in price data\ndf = pd.read_csv("tests/resources/stock_prices.csv", parse_dates=True, index_col="date")\n\n# Calculate expected returns and sample covariance\nmu = expected_returns.mean_historical_return(df)\nS = risk_models.sample_cov(df)\n\n# Optimize for maximal Sharpe ratio\nef = EfficientFrontier(mu, S)\nraw_weights = ef.max_sharpe()\ncleaned_weights = ef.clean_weights()\nef.save_weights_to_file("weights.csv")  # saves to file\nprint(cleaned_weights)\nef.portfolio_performance(verbose=True)\n```\n\nThis outputs the following weights:\n\n```txt\n{\'GOOG\': 0.03835,\n \'AAPL\': 0.0689,\n \'FB\': 0.20603,\n \'BABA\': 0.07315,\n \'AMZN\': 0.04033,\n \'GE\': 0.0,\n \'AMD\': 0.0,\n \'WMT\': 0.0,\n \'BAC\': 0.0,\n \'GM\': 0.0,\n \'T\': 0.0,\n \'UAA\': 0.0,\n \'SHLD\': 0.0,\n \'XOM\': 0.0,\n \'RRC\': 0.0,\n \'BBY\': 0.01324,\n \'MA\': 0.35349,\n \'PFE\': 0.1957,\n \'JPM\': 0.0,\n \'SBUX\': 0.01082}\n\nExpected annual return: 30.5%\nAnnual volatility: 22.2%\nSharpe Ratio: 1.28\n```\n\nThis is interesting but not useful in itself. However, PyPortfolioOpt provides a method which allows you to convert the above continuous weights to an actual allocation that you could buy. Just enter the most recent prices, and the desired portfolio size ($10,000 in this example):\n\n```python\nfrom pypfopt.discrete_allocation import DiscreteAllocation, get_latest_prices\n\n\nlatest_prices = get_latest_prices(df)\n\nda = DiscreteAllocation(weights, latest_prices, total_portfolio_value=10000)\nallocation, leftover = da.greedy_portfolio()\nprint("Discrete allocation:", allocation)\nprint("Funds remaining: ${:.2f}".format(leftover))\n```\n\n```txt\n12 out of 20 tickers were removed\nDiscrete allocation: {\'GOOG\': 1, \'AAPL\': 4, \'FB\': 12, \'BABA\': 4, \'BBY\': 2,\n                      \'MA\': 20, \'PFE\': 54, \'SBUX\': 1}\nFunds remaining: $11.89\n```\n\n_Disclaimer: nothing about this project constitues investment advice, and the author bears no responsibiltiy for your subsequent investment decisions. Please refer to the [license](https://github.com/robertmartin8/PyPortfolioOpt/blob/master/LICENSE.txt) for more information._\n\n## An overview of classical portfolio optimization methods\n\nHarry Markowitz\'s 1952 paper is the undeniable classic, which turned portfolio optimization from an art into a science. The key insight is that by combining assets with different expected returns and volatilities, one can decide on a mathematically optimal allocation which minimises the risk for a target return – the set of all such optimal portfolios is referred to as the **efficient frontier**.\n\n<center>\n<img src="https://github.com/robertmartin8/PyPortfolioOpt/blob/master/media/efficient_frontier_white.png?raw=true" style="width:60%;"/>\n</center>\n\nAlthough much development has been made in the subject, more than half a century later, Markowitz\'s core ideas are still fundamentally important and see daily use in many portfolio management firms.\nThe main drawback of mean-variance optimization is that the theoretical treatment requires knowledge of the expected returns and the future risk-characteristics (covariance) of the assets. Obviously, if we knew the expected returns of a stock life would be much easier, but the whole game is that stock returns are notoriously hard to forecast. As a substitute, we can derive estimates of the expected return and covariance based on historical data – though we do lose the theoretical guarantees provided by Markowitz, the closer our estimates are to the real values, the better our portfolio will be.\n\nThus this project provides four major sets of functionality (though of course they are intimately related)\n\n-   Estimates of expected returns\n-   Estimates of risk (i.e covariance of asset returns)\n-   Objective functions to be optimized\n-   Optimizers.\n\nA key design goal of PyPortfolioOpt is **modularity** – the user should be able to swap in their\ncomponents while still making use of the framework that PyPortfolioOpt provides.\n\n## Features\n\nIn this section, we detail some of PyPortfolioOpt\'s available functionality. More examples are offered in the Jupyter notebooks [here](https://github.com/robertmartin8/PyPortfolioOpt/tree/master/cookbook). Another good resource is the [tests](https://github.com/robertmartin8/PyPortfolioOpt/tree/master/tests).\n\nA far more comprehensive version of this can be found on [ReadTheDocs](https://pyportfolioopt.readthedocs.io/en/latest/), as well as possible extensions for more advanced users.\n\n### Expected returns\n\n-   Mean historical returns:\n    -   the simplest and most common approach, which states that the expected return of each asset is equal to the mean of its historical returns.\n    -   easily interpretable and very intuitive\n-   Exponentially weighted mean historical returns:\n    -   similar to mean historical returns, except it gives exponentially more weight to recent prices\n    -   it is likely the case that an asset\'s most recent returns hold more weight than returns from 10 years ago when it comes to estimating future returns.\n-   Capital Asset Pricing Model (CAPM):\n    -   a simple model to predict returns based on the beta to the market\n    -   this is used all over finance!\n\n### Risk models (covariance)\n\nThe covariance matrix encodes not just the volatility of an asset, but also how it correlated to other assets. This is important because in order to reap the benefits of diversification (and thus increase return per unit risk), the assets in the portfolio should be as uncorrelated as possible.\n\n-   Sample covariance matrix:\n    -   an unbiased estimate of the covariance matrix\n    -   relatively easy to compute\n    -   the de facto standard for many years\n    -   however, it has a high estimation error, which is particularly dangerous in mean-variance optimization because the optimizer is likely to give excess weight to these erroneous estimates.\n-   Semicovariance: a measure of risk that focuses on downside variation.\n-   Exponential covariance: an improvement over sample covariance that gives more weight to recent data\n-   Covariance shrinkage: techniques that involve combining the sample covariance matrix with a structured estimator, to reduce the effect of erroneous weights. PyPortfolioOpt provides wrappers around the efficient vectorised implementations provided by `sklearn.covariance`.\n    -   manual shrinkage\n    -   Ledoit Wolf shrinkage, which chooses an optimal shrinkage parameter. We offer three shrinkage targets: `constant_variance`, `single_factor`, and `constant_correlation`.\n    -   Oracle Approximating Shrinkage\n-   Minimum Covariance Determinant:\n    -   a robust estimate of the covariance\n    -   implemented in `sklearn.covariance`\n\n<p align="center">\n    <img width=60% src="https://github.com/robertmartin8/PyPortfolioOpt/blob/master/media/corrplot_white.png?raw=true">\n</p>\n\n(This plot was generated using `plotting.plot_covariance`)\n\n### Objective functions\n\n-   Maximum Sharpe ratio: this results in a _tangency portfolio_ because on a graph of returns vs risk, this portfolio corresponds to the tangent of the efficient frontier that has a y-intercept equal to the risk-free rate. This is the default option because it finds the optimal return per unit risk.\n-   Minimum volatility. This may be useful if you\'re trying to get an idea of how low the volatility _could_ be, but in practice it makes a lot more sense to me to use the portfolio that maximises the Sharpe ratio.\n-   Efficient return, a.k.a. the Markowitz portfolio, which minimises risk for a given target return – this was the main focus of Markowitz 1952\n-   Efficient risk: the Sharpe-maximising portfolio for a given target risk.\n-   Maximum quadratic utility. You can provide your own risk-aversion level and compute the appropriate portfolio.\n\n### Adding constraints or different objectives\n\n-   Long/short: by default all of the mean-variance optimization methods in PyPortfolioOpt are long-only, but they can be initialised to allow for short positions by changing the weight bounds:\n\n```python\nef = EfficientFrontier(mu, S, weight_bounds=(-1, 1))\n```\n\n-   Market neutrality: for the `efficient_risk` and `efficient_return` methods, PyPortfolioOpt provides an option to form a market-neutral portfolio (i.e weights sum to zero). This is not possible for the max Sharpe portfolio and the min volatility portfolio because in those cases because they are not invariant with respect to leverage. Market neutrality requires negative weights:\n\n```python\nef = EfficientFrontier(mu, S, weight_bounds=(-1, 1))\nef.efficient_return(target_return=0.2, market_neutral=True)\n```\n\n-   Minimum/maximum position size: it may be the case that you want no security to form more than 10% of your portfolio. This is easy to encode:\n\n```python\nef = EfficientFrontier(mu, S, weight_bounds=(0, 0.1))\n```\n\nOne issue with mean-variance optimization is that it leads to many zero-weights. While these are\n"optimal" in-sample, there is a large body of research showing that this characteristic leads\nmean-variance portfolios to underperform out-of-sample. To that end, I have introduced an\nobjective function that can reduce the number of negligible weights for any of the objective functions. Essentially, it adds a penalty (parameterised by `gamma`) on small weights, with a term that looks just like L2 regularisation in machine learning. It may be necessary to try several `gamma` values to achieve the desired number of non-negligible weights. For the test portfolio of 20 securities, `gamma ~ 1` is sufficient\n\n```python\nef = EfficientFrontier(mu, S)\nef.add_objective(objective_functions.L2_reg, gamma=1)\nef.max_sharpe()\n```\n\n### Black-Litterman allocation\n\nAs of v0.5.0, we now support Black-Litterman asset allocation, which allows you to combine\na prior estimate of returns (e.g the market-implied returns) with your own views to form a\nposterior estimate. This results in much better estimates of expected returns than just using\nthe mean historical return. Check out the [docs](https://pyportfolioopt.readthedocs.io/en/latest/BlackLitterman.html) for a discussion of the theory, as well as advice\non formatting inputs.\n\n```python\nS = risk_models.sample_cov(df)\nviewdict = {"AAPL": 0.20, "BBY": -0.30, "BAC": 0, "SBUX": -0.2, "T": 0.131321}\nbl = BlackLittermanModel(S, pi="equal", absolute_views=viewdict, omega="default")\nrets = bl.bl_returns()\n\nef = EfficientFrontier(rets, S)\nef.max_sharpe()\n```\n\n### Other optimizers\n\nThe features above mostly pertain to solving mean-variance optimization problems via quadratic programming (though this is taken care of by `cvxpy`). However, we offer different optimizers as well:\n\n-   Mean-semivariance optimization\n-   Mean-CVaR optimization\n-   Hierarchical Risk Parity, using clustering algorithms to choose uncorrelated assets\n-   Markowitz\'s critical line algorithm (CLA)\n\nPlease refer to the [documentation](https://pyportfolioopt.readthedocs.io/en/latest/OtherOptimizers.html) for more.\n\n## Advantages over existing implementations\n\n-   Includes both classical methods (Markowitz 1952 and Black-Litterman), suggested best practices\n    (e.g covariance shrinkage), along with many recent developments and novel\n    features, like L2 regularisation, shrunk covariance, hierarchical risk parity.\n-   Native support for pandas dataframes: easily input your daily prices data.\n-   Extensive practical tests, which use real-life data.\n-   Easy to combine with your proprietary strategies and models.\n-   Robust to missing data, and price-series of different lengths (e.g FB data\n    only goes back to 2012 whereas AAPL data goes back to 1980).\n\n## Project principles and design decisions\n\n-   It should be easy to swap out individual components of the optimization process\n    with the user\'s proprietary improvements.\n-   Usability is everything: it is better to be self-explanatory than consistent.\n-   There is no point in portfolio optimization unless it can be practically\n    applied to real asset prices.\n-   Everything that has been implemented should be tested.\n-   Inline documentation is good: dedicated (separate) documentation is better.\n    The two are not mutually exclusive.\n-   Formatting should never get in the way of coding: because of this,\n    I have deferred **all** formatting decisions to [Black](https://github.com/ambv/black).\n\n## Testing\n\nTests are written in pytest (much more intuitive than `unittest` and the variants in my opinion), and I have tried to ensure close to 100% coverage. Run the tests by navigating to the package directory and simply running `pytest` on the command line.\n\nPyPortfolioOpt provides a test dataset of daily returns for 20 tickers:\n\n```python\n[\'GOOG\', \'AAPL\', \'FB\', \'BABA\', \'AMZN\', \'GE\', \'AMD\', \'WMT\', \'BAC\', \'GM\',\n\'T\', \'UAA\', \'SHLD\', \'XOM\', \'RRC\', \'BBY\', \'MA\', \'PFE\', \'JPM\', \'SBUX\']\n```\n\nThese tickers have been informally selected to meet several criteria:\n\n-   reasonably liquid\n-   different performances and volatilities\n-   different amounts of data to test robustness\n\nCurrently, the tests have not explored all of the edge cases and combinations\nof objective functions and parameters. However, each method and parameter has\nbeen tested to work as intended.\n\n## Citing PyPortfolioOpt\n\nIf you use PyPortfolioOpt for published work, please cite the [JOSS paper](https://joss.theoj.org/papers/10.21105/joss.03066).\n\nCitation string:\n\n```text\nMartin, R. A., (2021). PyPortfolioOpt: portfolio optimization in Python. Journal of Open Source Software, 6(61), 3066, https://doi.org/10.21105/joss.03066\n```\n\nBibTex::\n\n```bibtex\n@article{Martin2021,\n  doi = {10.21105/joss.03066},\n  url = {https://doi.org/10.21105/joss.03066},\n  year = {2021},\n  publisher = {The Open Journal},\n  volume = {6},\n  number = {61},\n  pages = {3066},\n  author = {Robert Andrew Martin},\n  title = {PyPortfolioOpt: portfolio optimization in Python},\n  journal = {Journal of Open Source Software}\n}\n```\n\n## Contributing\n\nContributions are _most welcome_. Have a look at the [Contribution Guide](https://github.com/robertmartin8/PyPortfolioOpt/blob/master/CONTRIBUTING.md) for more.\n\nI\'d like to thank all of the people who have contributed to PyPortfolioOpt since its release in 2018.\nSpecial shout-outs to:\n\n-   Philipp Schiele\n-   Carl Peasnell\n-   Felipe Schneider\n-   Dingyuan Wang\n-   Pat Newell\n-   Aditya Bhutra\n-   Thomas Schmelzer\n-   Rich Caputo\n-   Nicolas Knudde\n\n## Getting in touch\n\nIf you are having a problem with PyPortfolioOpt, please raise a GitHub issue. For anything else, you can reach me at:\n\n<center>\n<img src="https://github.com/robertmartin8/ReasonableDeviations/blob/gh-pages/assets/images/contact.png?raw=true" style="width:60%;"/>\n</center>\n',
+    'long_description': '<p align="center">\n    <img width=60% src="https://github.com/robertmartin8/PyPortfolioOpt/blob/master/media/logo_v1.png?raw=true">\n</p>\n\n<!-- buttons -->\n<p align="center">\n    <a href="https://www.python.org">\n        <img src="https://img.shields.io/pypi/pyversions/PyPortfolioOpt.svg"\n            alt="python"></a> &nbsp;\n    <a href="https://www.python.org">\n        <img src="https://img.shields.io/badge/Platforms-linux--64,win--64,osx--64-orange.svg?style=flat-square"\n            alt="platforms"></a> &nbsp;\n    <a href="https://pypi.org/project/PyPortfolioOpt/">\n        <img src="https://img.shields.io/badge/pypi-v1.5.5-brightgreen.svg"\n            alt="pypi"></a> &nbsp;\n    <a href="https://opensource.org/licenses/MIT">\n        <img src="https://img.shields.io/badge/license-MIT-brightgreen.svg"\n            alt="MIT license"></a> &nbsp;\n    <a href="https://github.com/robertmartin8/PyPortfolioOpt/actions">\n        <img src="https://github.com/robertmartin8/PyPortfolioOpt/workflows/pytest/badge.svg?branch=master"\n            alt="build"></a> &nbsp;\n    <a href="https://app.codecov.io/gh/robertmartin8/PyPortfolioOpt">\n        <img src="https://codecov.io/github/robertmartin8/PyPortfolioOpt/coverage.svg?branch=main"\n            alt="codecov"></a> &nbsp;\n    <a href="https://pepy.tech/project/pyportfolioopt">\n        <img src="https://pepy.tech/badge/pyportfolioopt"\n            alt="downloads"></a> &nbsp;\n    <a href="https://mybinder.org/v2/gh/robertmartin8/pyportfolioopt/master/?filepath=cookbook">\n      <img src="https://mybinder.org/badge_logo.svg"\n            alt="binder"></a> &nbsp;\n</p>\n\n<!-- content -->\n\nPyPortfolioOpt is a library that implements portfolio optimization methods, including\nclassical mean-variance optimization techniques and Black-Litterman allocation, as well as more\nrecent developments in the field like shrinkage and Hierarchical Risk Parity.\n\nIt is **extensive** yet easily **extensible**, and can be useful for either a casual investors, or a professional looking for an easy prototyping tool. Whether you are a fundamentals-oriented investor who has identified a\nhandful of undervalued picks, or an algorithmic trader who has a basket of\nstrategies, PyPortfolioOpt can help you combine your alpha sources\nin a risk-efficient way.\n\n**PyPortfolioOpt has been [published](https://joss.theoj.org/papers/10.21105/joss.03066) in the Journal of Open Source Software 🎉**\n\nPyPortfolioOpt is now being maintained by [Tuan Tran](https://github.com/88d52bdba0366127fffca9dfa93895).\n\nHead over to the **[documentation on ReadTheDocs](https://pyportfolioopt.readthedocs.io/en/latest/)** to get an in-depth look at the project, or check out the [cookbook](https://github.com/robertmartin8/PyPortfolioOpt/tree/master/cookbook) to see some examples showing the full process from downloading data to building a portfolio.\n\n<center>\n<img src="https://github.com/robertmartin8/PyPortfolioOpt/blob/master/media/conceptual_flowchart_v2.png?raw=true" style="width:70%;"/>\n</center>\n\n## Table of contents\n\n-   [Table of contents](#table-of-contents)\n-   [Getting started](#getting-started)\n    -   [For development](#for-development)\n-   [A quick example](#a-quick-example)\n-   [An overview of classical portfolio optimization methods](#an-overview-of-classical-portfolio-optimization-methods)\n-   [Features](#features)\n    -   [Expected returns](#expected-returns)\n    -   [Risk models (covariance)](#risk-models-covariance)\n    -   [Objective functions](#objective-functions)\n    -   [Adding constraints or different objectives](#adding-constraints-or-different-objectives)\n    -   [Black-Litterman allocation](#black-litterman-allocation)\n    -   [Other optimizers](#other-optimizers)\n-   [Advantages over existing implementations](#advantages-over-existing-implementations)\n-   [Project principles and design decisions](#project-principles-and-design-decisions)\n-   [Testing](#testing)\n-   [Citing PyPortfolioOpt](#citing-pyportfolioopt)\n-   [Contributing](#contributing)\n-   [Getting in touch](#getting-in-touch)\n\n## Getting started\n\nIf you would like to play with PyPortfolioOpt interactively in your browser, you may launch Binder [here](https://mybinder.org/v2/gh/robertmartin8/pyportfolioopt/master). It takes a\nwhile to set up, but it lets you try out the cookbook recipes without having to deal with all of the requirements.\n\n_Note: macOS users will need to install [Command Line Tools](https://osxdaily.com/2014/02/12/install-command-line-tools-mac-os-x/)._\n\n_Note: if you are on windows, you first need to installl C++. ([download](https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=BuildTools&rel=16), [install instructions](https://drive.google.com/file/d/0B4GsMXCRaSSIOWpYQkstajlYZ0tPVkNQSElmTWh1dXFaYkJr/view))_\n\nThis project is available on PyPI, meaning that you can just:\n\n```bash\npip install PyPortfolioOpt\n```\n\n(you may need to follow separate installation instructions for [cvxopt](https://cvxopt.org/install/index.html#) and [cvxpy](https://www.cvxpy.org/install/)).\n\nHowever, it is best practice to use a dependency manager within a virtual environment.\nMy current recommendation is to get yourself set up with [poetry](https://github.com/sdispater/poetry) then just run\n\n```bash\npoetry add PyPortfolioOpt\n```\n\nOtherwise, clone/download the project and in the project directory run:\n\n```bash\npython setup.py install\n```\n\nPyPortfolioOpt supports Docker. Build your first container with `docker build -f docker/Dockerfile . -t pypfopt`. You can use the image to run tests or even launch a Jupyter server.\n\n```bash\n# iPython interpreter:\ndocker run -it pypfopt poetry run ipython\n\n# Jupyter notebook server:\ndocker run -it -p 8888:8888 pypfopt poetry run jupyter notebook --allow-root --no-browser --ip 0.0.0.0\n# click on http://127.0.0.1:8888/?token=xxx\n\n# Pytest\ndocker run -t pypfopt poetry run pytest\n\n# Bash\ndocker run -it pypfopt bash\n```\n\nFor more information, please read [this guide](https://docker-curriculum.com/#introduction).\n\n### For development\n\nIf you would like to make major changes to integrate this with your proprietary system, it probably makes sense to clone this repository and to just use the source code.\n\n```bash\ngit clone https://github.com/robertmartin8/PyPortfolioOpt\n```\n\nAlternatively, you could try:\n\n```bash\npip install -e git+https://github.com/robertmartin8/PyPortfolioOpt.git\n```\n\n## A quick example\n\nHere is an example on real life stock data, demonstrating how easy it is to find the long-only portfolio that maximises the Sharpe ratio (a measure of risk-adjusted returns).\n\n```python\nimport pandas as pd\nfrom pypfopt import EfficientFrontier\nfrom pypfopt import risk_models\nfrom pypfopt import expected_returns\n\n# Read in price data\ndf = pd.read_csv("tests/resources/stock_prices.csv", parse_dates=True, index_col="date")\n\n# Calculate expected returns and sample covariance\nmu = expected_returns.mean_historical_return(df)\nS = risk_models.sample_cov(df)\n\n# Optimize for maximal Sharpe ratio\nef = EfficientFrontier(mu, S)\nraw_weights = ef.max_sharpe()\ncleaned_weights = ef.clean_weights()\nef.save_weights_to_file("weights.csv")  # saves to file\nprint(cleaned_weights)\nef.portfolio_performance(verbose=True)\n```\n\nThis outputs the following weights:\n\n```txt\n{\'GOOG\': 0.03835,\n \'AAPL\': 0.0689,\n \'FB\': 0.20603,\n \'BABA\': 0.07315,\n \'AMZN\': 0.04033,\n \'GE\': 0.0,\n \'AMD\': 0.0,\n \'WMT\': 0.0,\n \'BAC\': 0.0,\n \'GM\': 0.0,\n \'T\': 0.0,\n \'UAA\': 0.0,\n \'SHLD\': 0.0,\n \'XOM\': 0.0,\n \'RRC\': 0.0,\n \'BBY\': 0.01324,\n \'MA\': 0.35349,\n \'PFE\': 0.1957,\n \'JPM\': 0.0,\n \'SBUX\': 0.01082}\n\nExpected annual return: 30.5%\nAnnual volatility: 22.2%\nSharpe Ratio: 1.28\n```\n\nThis is interesting but not useful in itself. However, PyPortfolioOpt provides a method which allows you to convert the above continuous weights to an actual allocation that you could buy. Just enter the most recent prices, and the desired portfolio size ($10,000 in this example):\n\n```python\nfrom pypfopt.discrete_allocation import DiscreteAllocation, get_latest_prices\n\n\nlatest_prices = get_latest_prices(df)\n\nda = DiscreteAllocation(weights, latest_prices, total_portfolio_value=10000)\nallocation, leftover = da.greedy_portfolio()\nprint("Discrete allocation:", allocation)\nprint("Funds remaining: ${:.2f}".format(leftover))\n```\n\n```txt\n12 out of 20 tickers were removed\nDiscrete allocation: {\'GOOG\': 1, \'AAPL\': 4, \'FB\': 12, \'BABA\': 4, \'BBY\': 2,\n                      \'MA\': 20, \'PFE\': 54, \'SBUX\': 1}\nFunds remaining: $11.89\n```\n\n_Disclaimer: nothing about this project constitues investment advice, and the author bears no responsibiltiy for your subsequent investment decisions. Please refer to the [license](https://github.com/robertmartin8/PyPortfolioOpt/blob/master/LICENSE.txt) for more information._\n\n## An overview of classical portfolio optimization methods\n\nHarry Markowitz\'s 1952 paper is the undeniable classic, which turned portfolio optimization from an art into a science. The key insight is that by combining assets with different expected returns and volatilities, one can decide on a mathematically optimal allocation which minimises the risk for a target return – the set of all such optimal portfolios is referred to as the **efficient frontier**.\n\n<center>\n<img src="https://github.com/robertmartin8/PyPortfolioOpt/blob/master/media/efficient_frontier_white.png?raw=true" style="width:60%;"/>\n</center>\n\nAlthough much development has been made in the subject, more than half a century later, Markowitz\'s core ideas are still fundamentally important and see daily use in many portfolio management firms.\nThe main drawback of mean-variance optimization is that the theoretical treatment requires knowledge of the expected returns and the future risk-characteristics (covariance) of the assets. Obviously, if we knew the expected returns of a stock life would be much easier, but the whole game is that stock returns are notoriously hard to forecast. As a substitute, we can derive estimates of the expected return and covariance based on historical data – though we do lose the theoretical guarantees provided by Markowitz, the closer our estimates are to the real values, the better our portfolio will be.\n\nThus this project provides four major sets of functionality (though of course they are intimately related)\n\n-   Estimates of expected returns\n-   Estimates of risk (i.e covariance of asset returns)\n-   Objective functions to be optimized\n-   Optimizers.\n\nA key design goal of PyPortfolioOpt is **modularity** – the user should be able to swap in their\ncomponents while still making use of the framework that PyPortfolioOpt provides.\n\n## Features\n\nIn this section, we detail some of PyPortfolioOpt\'s available functionality. More examples are offered in the Jupyter notebooks [here](https://github.com/robertmartin8/PyPortfolioOpt/tree/master/cookbook). Another good resource is the [tests](https://github.com/robertmartin8/PyPortfolioOpt/tree/master/tests).\n\nA far more comprehensive version of this can be found on [ReadTheDocs](https://pyportfolioopt.readthedocs.io/en/latest/), as well as possible extensions for more advanced users.\n\n### Expected returns\n\n-   Mean historical returns:\n    -   the simplest and most common approach, which states that the expected return of each asset is equal to the mean of its historical returns.\n    -   easily interpretable and very intuitive\n-   Exponentially weighted mean historical returns:\n    -   similar to mean historical returns, except it gives exponentially more weight to recent prices\n    -   it is likely the case that an asset\'s most recent returns hold more weight than returns from 10 years ago when it comes to estimating future returns.\n-   Capital Asset Pricing Model (CAPM):\n    -   a simple model to predict returns based on the beta to the market\n    -   this is used all over finance!\n\n### Risk models (covariance)\n\nThe covariance matrix encodes not just the volatility of an asset, but also how it correlated to other assets. This is important because in order to reap the benefits of diversification (and thus increase return per unit risk), the assets in the portfolio should be as uncorrelated as possible.\n\n-   Sample covariance matrix:\n    -   an unbiased estimate of the covariance matrix\n    -   relatively easy to compute\n    -   the de facto standard for many years\n    -   however, it has a high estimation error, which is particularly dangerous in mean-variance optimization because the optimizer is likely to give excess weight to these erroneous estimates.\n-   Semicovariance: a measure of risk that focuses on downside variation.\n-   Exponential covariance: an improvement over sample covariance that gives more weight to recent data\n-   Covariance shrinkage: techniques that involve combining the sample covariance matrix with a structured estimator, to reduce the effect of erroneous weights. PyPortfolioOpt provides wrappers around the efficient vectorised implementations provided by `sklearn.covariance`.\n    -   manual shrinkage\n    -   Ledoit Wolf shrinkage, which chooses an optimal shrinkage parameter. We offer three shrinkage targets: `constant_variance`, `single_factor`, and `constant_correlation`.\n    -   Oracle Approximating Shrinkage\n-   Minimum Covariance Determinant:\n    -   a robust estimate of the covariance\n    -   implemented in `sklearn.covariance`\n\n<p align="center">\n    <img width=60% src="https://github.com/robertmartin8/PyPortfolioOpt/blob/master/media/corrplot_white.png?raw=true">\n</p>\n\n(This plot was generated using `plotting.plot_covariance`)\n\n### Objective functions\n\n-   Maximum Sharpe ratio: this results in a _tangency portfolio_ because on a graph of returns vs risk, this portfolio corresponds to the tangent of the efficient frontier that has a y-intercept equal to the risk-free rate. This is the default option because it finds the optimal return per unit risk.\n-   Minimum volatility. This may be useful if you\'re trying to get an idea of how low the volatility _could_ be, but in practice it makes a lot more sense to me to use the portfolio that maximises the Sharpe ratio.\n-   Efficient return, a.k.a. the Markowitz portfolio, which minimises risk for a given target return – this was the main focus of Markowitz 1952\n-   Efficient risk: the Sharpe-maximising portfolio for a given target risk.\n-   Maximum quadratic utility. You can provide your own risk-aversion level and compute the appropriate portfolio.\n\n### Adding constraints or different objectives\n\n-   Long/short: by default all of the mean-variance optimization methods in PyPortfolioOpt are long-only, but they can be initialised to allow for short positions by changing the weight bounds:\n\n```python\nef = EfficientFrontier(mu, S, weight_bounds=(-1, 1))\n```\n\n-   Market neutrality: for the `efficient_risk` and `efficient_return` methods, PyPortfolioOpt provides an option to form a market-neutral portfolio (i.e weights sum to zero). This is not possible for the max Sharpe portfolio and the min volatility portfolio because in those cases because they are not invariant with respect to leverage. Market neutrality requires negative weights:\n\n```python\nef = EfficientFrontier(mu, S, weight_bounds=(-1, 1))\nef.efficient_return(target_return=0.2, market_neutral=True)\n```\n\n-   Minimum/maximum position size: it may be the case that you want no security to form more than 10% of your portfolio. This is easy to encode:\n\n```python\nef = EfficientFrontier(mu, S, weight_bounds=(0, 0.1))\n```\n\nOne issue with mean-variance optimization is that it leads to many zero-weights. While these are\n"optimal" in-sample, there is a large body of research showing that this characteristic leads\nmean-variance portfolios to underperform out-of-sample. To that end, I have introduced an\nobjective function that can reduce the number of negligible weights for any of the objective functions. Essentially, it adds a penalty (parameterised by `gamma`) on small weights, with a term that looks just like L2 regularisation in machine learning. It may be necessary to try several `gamma` values to achieve the desired number of non-negligible weights. For the test portfolio of 20 securities, `gamma ~ 1` is sufficient\n\n```python\nef = EfficientFrontier(mu, S)\nef.add_objective(objective_functions.L2_reg, gamma=1)\nef.max_sharpe()\n```\n\n### Black-Litterman allocation\n\nAs of v0.5.0, we now support Black-Litterman asset allocation, which allows you to combine\na prior estimate of returns (e.g the market-implied returns) with your own views to form a\nposterior estimate. This results in much better estimates of expected returns than just using\nthe mean historical return. Check out the [docs](https://pyportfolioopt.readthedocs.io/en/latest/BlackLitterman.html) for a discussion of the theory, as well as advice\non formatting inputs.\n\n```python\nS = risk_models.sample_cov(df)\nviewdict = {"AAPL": 0.20, "BBY": -0.30, "BAC": 0, "SBUX": -0.2, "T": 0.131321}\nbl = BlackLittermanModel(S, pi="equal", absolute_views=viewdict, omega="default")\nrets = bl.bl_returns()\n\nef = EfficientFrontier(rets, S)\nef.max_sharpe()\n```\n\n### Other optimizers\n\nThe features above mostly pertain to solving mean-variance optimization problems via quadratic programming (though this is taken care of by `cvxpy`). However, we offer different optimizers as well:\n\n-   Mean-semivariance optimization\n-   Mean-CVaR optimization\n-   Hierarchical Risk Parity, using clustering algorithms to choose uncorrelated assets\n-   Markowitz\'s critical line algorithm (CLA)\n\nPlease refer to the [documentation](https://pyportfolioopt.readthedocs.io/en/latest/OtherOptimizers.html) for more.\n\n## Advantages over existing implementations\n\n-   Includes both classical methods (Markowitz 1952 and Black-Litterman), suggested best practices\n    (e.g covariance shrinkage), along with many recent developments and novel\n    features, like L2 regularisation, shrunk covariance, hierarchical risk parity.\n-   Native support for pandas dataframes: easily input your daily prices data.\n-   Extensive practical tests, which use real-life data.\n-   Easy to combine with your proprietary strategies and models.\n-   Robust to missing data, and price-series of different lengths (e.g FB data\n    only goes back to 2012 whereas AAPL data goes back to 1980).\n\n## Project principles and design decisions\n\n-   It should be easy to swap out individual components of the optimization process\n    with the user\'s proprietary improvements.\n-   Usability is everything: it is better to be self-explanatory than consistent.\n-   There is no point in portfolio optimization unless it can be practically\n    applied to real asset prices.\n-   Everything that has been implemented should be tested.\n-   Inline documentation is good: dedicated (separate) documentation is better.\n    The two are not mutually exclusive.\n-   Formatting should never get in the way of coding: because of this,\n    I have deferred **all** formatting decisions to [Black](https://github.com/ambv/black).\n\n## Testing\n\nTests are written in pytest (much more intuitive than `unittest` and the variants in my opinion), and I have tried to ensure close to 100% coverage. Run the tests by navigating to the package directory and simply running `pytest` on the command line.\n\nPyPortfolioOpt provides a test dataset of daily returns for 20 tickers:\n\n```python\n[\'GOOG\', \'AAPL\', \'FB\', \'BABA\', \'AMZN\', \'GE\', \'AMD\', \'WMT\', \'BAC\', \'GM\',\n\'T\', \'UAA\', \'SHLD\', \'XOM\', \'RRC\', \'BBY\', \'MA\', \'PFE\', \'JPM\', \'SBUX\']\n```\n\nThese tickers have been informally selected to meet several criteria:\n\n-   reasonably liquid\n-   different performances and volatilities\n-   different amounts of data to test robustness\n\nCurrently, the tests have not explored all of the edge cases and combinations\nof objective functions and parameters. However, each method and parameter has\nbeen tested to work as intended.\n\n## Citing PyPortfolioOpt\n\nIf you use PyPortfolioOpt for published work, please cite the [JOSS paper](https://joss.theoj.org/papers/10.21105/joss.03066).\n\nCitation string:\n\n```text\nMartin, R. A., (2021). PyPortfolioOpt: portfolio optimization in Python. Journal of Open Source Software, 6(61), 3066, https://doi.org/10.21105/joss.03066\n```\n\nBibTex::\n\n```bibtex\n@article{Martin2021,\n  doi = {10.21105/joss.03066},\n  url = {https://doi.org/10.21105/joss.03066},\n  year = {2021},\n  publisher = {The Open Journal},\n  volume = {6},\n  number = {61},\n  pages = {3066},\n  author = {Robert Andrew Martin},\n  title = {PyPortfolioOpt: portfolio optimization in Python},\n  journal = {Journal of Open Source Software}\n}\n```\n\n## Contributing\n\nContributions are _most welcome_. Have a look at the [Contribution Guide](https://github.com/robertmartin8/PyPortfolioOpt/blob/master/CONTRIBUTING.md) for more.\n\nI\'d like to thank all of the people who have contributed to PyPortfolioOpt since its release in 2018.\nSpecial shout-outs to:\n\n-   Tuan Tran (who is now the primary maintainer!)\n-   Philipp Schiele\n-   Carl Peasnell\n-   Felipe Schneider\n-   Dingyuan Wang\n-   Pat Newell\n-   Aditya Bhutra\n-   Thomas Schmelzer\n-   Rich Caputo\n-   Nicolas Knudde\n\n## Getting in touch\n\nIf you are having a problem with PyPortfolioOpt, please raise a GitHub issue. For anything else, you can reach me at:\n\n<center>\n<img src="https://github.com/robertmartin8/ReasonableDeviations/blob/gh-pages/assets/images/contact.png?raw=true" style="width:60%;"/>\n</center>\n',
     'author': 'Robert Andrew Martin',
     'author_email': 'martin.robertandrew@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/robertmartin8/PyPortfolioOpt',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.8,<3.11',
+    'python_requires': '>=3.8,<3.15',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,37 +1,38 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['pypfopt',
 'pypfopt.efficient_frontier'] package_data = \ {'': ['*']} install_requires = \
-['cvxpy>=1.1.10,<2.0.0', 'numpy>=1.22.4,<2.0.0', 'pandas>=0.19',
+['cvxpy>=1.1.19,<2.0.0', 'numpy>=1.22.4,<2.0.0', 'pandas>=0.19',
 'scipy>=1.3,<2.0'] extras_require = \ {'optionals':
-['matplotlib>=3.5.2,<4.0.0', 'scikit-learn>=1.1.1,<2.0.0']} setup_kwargs =
-{ 'name': 'pyportfolioopt', 'version': '1.5.4', 'description': 'Financial
+['matplotlib>=3.2.0,<4.0.0', 'scikit-learn>=0.24.1,<0.25.0']} setup_kwargs =
+{ 'name': 'pyportfolioopt', 'version': '1.5.5', 'description': 'Financial
 portfolio optimization in python', 'long_description': '
     \n [https://github.com/robertmartin8/PyPortfolioOpt/blob/master/media/
                             logo_v1.png?raw=true]\n
 \n\n\n
-\n \n_n_alt="python">  \n \n_n_alt="pypi">  \n \n_n_alt="MIT_license">  \n \n_n
-       alt="build">  \n \n_n_alt="downloads">  \n \n_n_alt="binder">  \n
-\n\n\n**PyPortfolioOpt is looking for maintainers! Please reach out to the
-email address at the bottom of the readme if you\'re
-interested**\n\nPyPortfolioOpt is a library that implements portfolio
-optimization methods, including\nclassical mean-variance optimization
-techniques and Black-Litterman allocation, as well as more\nrecent developments
-in the field like shrinkage and Hierarchical Risk Parity.\n\nIt is
-**extensive** yet easily **extensible**, and can be useful for either a casual
-investors, or a professional looking for an easy prototyping tool. Whether you
-are a fundamentals-oriented investor who has identified a\nhandful of
-undervalued picks, or an algorithmic trader who has a basket of\nstrategies,
-PyPortfolioOpt can help you combine your alpha sources\nin a risk-efficient
+ \n \n_n_alt="python">  \n \n_n_alt="platforms">  \n \n_n_alt="pypi">  \n \n_n
+   alt="MIT_license">  \n \n_n_alt="build">  \n \n_n_alt="codecov">  \n \n_n
+                  alt="downloads">  \n \n_n_alt="binder">  \n
+\n\n\n\nPyPortfolioOpt is a library that implements portfolio optimization
+methods, including\nclassical mean-variance optimization techniques and Black-
+Litterman allocation, as well as more\nrecent developments in the field like
+shrinkage and Hierarchical Risk Parity.\n\nIt is **extensive** yet easily
+**extensible**, and can be useful for either a casual investors, or a
+professional looking for an easy prototyping tool. Whether you are a
+fundamentals-oriented investor who has identified a\nhandful of undervalued
+picks, or an algorithmic trader who has a basket of\nstrategies, PyPortfolioOpt
+can help you combine your alpha sources\nin a risk-efficient
 way.\n\n**PyPortfolioOpt has been [published](https://joss.theoj.org/papers/
-10.21105/joss.03066) in the Journal of Open Source Software ð**\n\nHead over
-to the **[documentation on ReadTheDocs](https://pyportfolioopt.readthedocs.io/
-en/latest/)** to get an in-depth look at the project, or check out the
-[cookbook](https://github.com/robertmartin8/PyPortfolioOpt/tree/master/
-cookbook) to see some examples showing the full process from downloading data
-to building a portfolio.\n\n
+10.21105/joss.03066) in the Journal of Open Source Software
+ð**\n\nPyPortfolioOpt is now being maintained by [Tuan Tran](https://
+github.com/88d52bdba0366127fffca9dfa93895).\n\nHead over to the **
+[documentation on ReadTheDocs](https://pyportfolioopt.readthedocs.io/en/latest/
+)** to get an in-depth look at the project, or check out the [cookbook](https:/
+/github.com/robertmartin8/PyPortfolioOpt/tree/master/cookbook) to see some
+examples showing the full process from downloading data to building a
+portfolio.\n\n
      \n[https://github.com/robertmartin8/PyPortfolioOpt/blob/master/media/
                     conceptual_flowchart_v2.png?raw=true]\n
 \n\n## Table of contents\n\n- [Table of contents](#table-of-contents)\n-
 [Getting started](#getting-started)\n - [For development](#for-development)\n-
 [A quick example](#a-quick-example)\n- [An overview of classical portfolio
 optimization methods](#an-overview-of-classical-portfolio-optimization-
 methods)\n- [Features](#features)\n - [Expected returns](#expected-returns)\n -
@@ -53,15 +54,15 @@
 to installl C++. ([download](https://visualstudio.microsoft.com/thank-you-
 downloading-visual-studio/?sku=BuildTools&rel=16), [install instructions]
 (https://drive.google.com/file/d/
 0B4GsMXCRaSSIOWpYQkstajlYZ0tPVkNQSElmTWh1dXFaYkJr/view))_\n\nThis project is
 available on PyPI, meaning that you can just:\n\n```bash\npip install
 PyPortfolioOpt\n```\n\n(you may need to follow separate installation
 instructions for [cvxopt](https://cvxopt.org/install/index.html#) and [cvxpy]
-(https://www.cvxpy.org/install/))).\n\nHowever, it is best practice to use a
+(https://www.cvxpy.org/install/)).\n\nHowever, it is best practice to use a
 dependency manager within a virtual environment.\nMy current recommendation is
 to get yourself set up with [poetry](https://github.com/sdispater/poetry) then
 just run\n\n```bash\npoetry add PyPortfolioOpt\n```\n\nOtherwise, clone/
 download the project and in the project directory run:\n\n```bash\npython
 setup.py install\n```\n\nPyPortfolioOpt supports Docker. Build your first
 container with `docker build -f docker/Dockerfile . -t pypfopt`. You can use
 the image to run tests or even launch a Jupyter server.\n\n```bash\n# iPython
@@ -267,20 +268,20 @@
 Journal},\n volume = {6},\n number = {61},\n pages = {3066},\n author = {Robert
 Andrew Martin},\n title = {PyPortfolioOpt: portfolio optimization in Python},\n
 journal = {Journal of Open Source Software}\n}\n```\n\n##
 Contributing\n\nContributions are _most welcome_. Have a look at the
 [Contribution Guide](https://github.com/robertmartin8/PyPortfolioOpt/blob/
 master/CONTRIBUTING.md) for more.\n\nI\'d like to thank all of the people who
 have contributed to PyPortfolioOpt since its release in 2018.\nSpecial shout-
-outs to:\n\n- Philipp Schiele\n- Carl Peasnell\n- Felipe Schneider\n- Dingyuan
-Wang\n- Pat Newell\n- Aditya Bhutra\n- Thomas Schmelzer\n- Rich Caputo\n-
-Nicolas Knudde\n\n## Getting in touch\n\nIf you are having a problem with
-PyPortfolioOpt, please raise a GitHub issue. For anything else, you can reach
-me at:\n\n
+outs to:\n\n- Tuan Tran (who is now the primary maintainer!)\n- Philipp
+Schiele\n- Carl Peasnell\n- Felipe Schneider\n- Dingyuan Wang\n- Pat Newell\n-
+Aditya Bhutra\n- Thomas Schmelzer\n- Rich Caputo\n- Nicolas Knudde\n\n##
+Getting in touch\n\nIf you are having a problem with PyPortfolioOpt, please
+raise a GitHub issue. For anything else, you can reach me at:\n\n
 \n[https://github.com/robertmartin8/ReasonableDeviations/blob/gh-pages/assets/
                         images/contact.png?raw=true]\n
 \n', 'author': 'Robert Andrew Martin', 'author_email':
 'martin.robertandrew@gmail.com', 'maintainer': None, 'maintainer_email': None,
 'url': 'https://github.com/robertmartin8/PyPortfolioOpt', 'packages': packages,
 'package_data': package_data, 'install_requires': install_requires,
-'extras_require': extras_require, 'python_requires': '>=3.8,<3.11', } setup
+'extras_require': extras_require, 'python_requires': '>=3.8,<3.15', } setup
 (**setup_kwargs)
```

### Comparing `pyportfolioopt-1.5.4/PKG-INFO` & `pyportfolioopt-1.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,84 +1,92 @@
 Metadata-Version: 2.1
 Name: pyportfolioopt
-Version: 1.5.4
+Version: 1.5.5
 Summary: Financial portfolio optimization in python
 Home-page: https://github.com/robertmartin8/PyPortfolioOpt
 License: MIT
 Keywords: finance,portfolio,optimization,quant,investing
 Author: Robert Andrew Martin
 Author-email: martin.robertandrew@gmail.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.15
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Office/Business :: Financial
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Provides-Extra: optionals
-Requires-Dist: cvxpy (>=1.1.10,<2.0.0)
-Requires-Dist: matplotlib (>=3.5.2,<4.0.0); extra == "optionals"
+Requires-Dist: cvxpy (>=1.1.19,<2.0.0)
+Requires-Dist: matplotlib (>=3.2.0,<4.0.0); extra == "optionals"
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: pandas (>=0.19)
-Requires-Dist: scikit-learn (>=1.1.1,<2.0.0); extra == "optionals"
+Requires-Dist: scikit-learn (>=0.24.1,<0.25.0); extra == "optionals"
 Requires-Dist: scipy (>=1.3,<2.0)
 Project-URL: Documentation, https://pyportfolioopt.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/robertmartin8/PyPortfolioOpt/issues
 Project-URL: Personal website, https://reasonabledeviations.com
 Project-URL: Repository, https://github.com/robertmartin8/PyPortfolioOpt
 Description-Content-Type: text/markdown
 
 <p align="center">
     <img width=60% src="https://github.com/robertmartin8/PyPortfolioOpt/blob/master/media/logo_v1.png?raw=true">
 </p>
 
 <!-- buttons -->
 <p align="center">
-    <a href="https://www.python.org/">
-        <img src="https://img.shields.io/badge/python-v3-brightgreen.svg"
+    <a href="https://www.python.org">
+        <img src="https://img.shields.io/pypi/pyversions/PyPortfolioOpt.svg"
             alt="python"></a> &nbsp;
+    <a href="https://www.python.org">
+        <img src="https://img.shields.io/badge/Platforms-linux--64,win--64,osx--64-orange.svg?style=flat-square"
+            alt="platforms"></a> &nbsp;
     <a href="https://pypi.org/project/PyPortfolioOpt/">
-        <img src="https://img.shields.io/badge/pypi-v1.5.4-brightgreen.svg"
+        <img src="https://img.shields.io/badge/pypi-v1.5.5-brightgreen.svg"
             alt="pypi"></a> &nbsp;
     <a href="https://opensource.org/licenses/MIT">
         <img src="https://img.shields.io/badge/license-MIT-brightgreen.svg"
             alt="MIT license"></a> &nbsp;
     <a href="https://github.com/robertmartin8/PyPortfolioOpt/actions">
-        <img src="https://github.com/robertmartin8/PyPortfolioOpt/workflows/pytest/badge.svg?event=push"
+        <img src="https://github.com/robertmartin8/PyPortfolioOpt/workflows/pytest/badge.svg?branch=master"
             alt="build"></a> &nbsp;
+    <a href="https://app.codecov.io/gh/robertmartin8/PyPortfolioOpt">
+        <img src="https://codecov.io/github/robertmartin8/PyPortfolioOpt/coverage.svg?branch=main"
+            alt="codecov"></a> &nbsp;
     <a href="https://pepy.tech/project/pyportfolioopt">
         <img src="https://pepy.tech/badge/pyportfolioopt"
             alt="downloads"></a> &nbsp;
     <a href="https://mybinder.org/v2/gh/robertmartin8/pyportfolioopt/master/?filepath=cookbook">
       <img src="https://mybinder.org/badge_logo.svg"
             alt="binder"></a> &nbsp;
 </p>
 
 <!-- content -->
-**PyPortfolioOpt is looking for maintainers! Please reach out to the email address at the bottom of the readme if you're interested**
 
 PyPortfolioOpt is a library that implements portfolio optimization methods, including
 classical mean-variance optimization techniques and Black-Litterman allocation, as well as more
 recent developments in the field like shrinkage and Hierarchical Risk Parity.
 
 It is **extensive** yet easily **extensible**, and can be useful for either a casual investors, or a professional looking for an easy prototyping tool. Whether you are a fundamentals-oriented investor who has identified a
 handful of undervalued picks, or an algorithmic trader who has a basket of
 strategies, PyPortfolioOpt can help you combine your alpha sources
 in a risk-efficient way.
 
 **PyPortfolioOpt has been [published](https://joss.theoj.org/papers/10.21105/joss.03066) in the Journal of Open Source Software 🎉**
 
+PyPortfolioOpt is now being maintained by [Tuan Tran](https://github.com/88d52bdba0366127fffca9dfa93895).
+
 Head over to the **[documentation on ReadTheDocs](https://pyportfolioopt.readthedocs.io/en/latest/)** to get an in-depth look at the project, or check out the [cookbook](https://github.com/robertmartin8/PyPortfolioOpt/tree/master/cookbook) to see some examples showing the full process from downloading data to building a portfolio.
 
 <center>
 <img src="https://github.com/robertmartin8/PyPortfolioOpt/blob/master/media/conceptual_flowchart_v2.png?raw=true" style="width:70%;"/>
 </center>
 
 ## Table of contents
@@ -113,15 +121,15 @@
 
 This project is available on PyPI, meaning that you can just:
 
 ```bash
 pip install PyPortfolioOpt
 ```
 
-(you may need to follow separate installation instructions for [cvxopt](https://cvxopt.org/install/index.html#) and [cvxpy](https://www.cvxpy.org/install/))).
+(you may need to follow separate installation instructions for [cvxopt](https://cvxopt.org/install/index.html#) and [cvxpy](https://www.cvxpy.org/install/)).
 
 However, it is best practice to use a dependency manager within a virtual environment.
 My current recommendation is to get yourself set up with [poetry](https://github.com/sdispater/poetry) then just run
 
 ```bash
 poetry add PyPortfolioOpt
 ```
@@ -451,14 +459,15 @@
 ## Contributing
 
 Contributions are _most welcome_. Have a look at the [Contribution Guide](https://github.com/robertmartin8/PyPortfolioOpt/blob/master/CONTRIBUTING.md) for more.
 
 I'd like to thank all of the people who have contributed to PyPortfolioOpt since its release in 2018.
 Special shout-outs to:
 
+-   Tuan Tran (who is now the primary maintainer!)
 -   Philipp Schiele
 -   Carl Peasnell
 -   Felipe Schneider
 -   Dingyuan Wang
 -   Pat Newell
 -   Aditya Bhutra
 -   Thomas Schmelzer
```

#### html2text {}

```diff
@@ -1,50 +1,51 @@
-Metadata-Version: 2.1 Name: pyportfolioopt Version: 1.5.4 Summary: Financial
+Metadata-Version: 2.1 Name: pyportfolioopt Version: 1.5.5 Summary: Financial
 portfolio optimization in python Home-page: https://github.com/robertmartin8/
 PyPortfolioOpt License: MIT Keywords:
 finance,portfolio,optimization,quant,investing Author: Robert Andrew Martin
-Author-email: martin.robertandrew@gmail.com Requires-Python: >=3.8,<3.11
+Author-email: martin.robertandrew@gmail.com Requires-Python: >=3.8,<3.15
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
 Classifier: Intended Audience :: Financial and Insurance Industry Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 MIT License Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Office/
-Business :: Financial Classifier: Topic :: Office/Business :: Financial ::
-Investment Provides-Extra: optionals Requires-Dist: cvxpy (>=1.1.10,<2.0.0)
-Requires-Dist: matplotlib (>=3.5.2,<4.0.0); extra == "optionals" Requires-Dist:
-numpy (>=1.22.4,<2.0.0) Requires-Dist: pandas (>=0.19) Requires-Dist: scikit-
-learn (>=1.1.1,<2.0.0); extra == "optionals" Requires-Dist: scipy (>=1.3,<2.0)
-Project-URL: Documentation, https://pyportfolioopt.readthedocs.io/en/latest/
-Project-URL: Issues, https://github.com/robertmartin8/PyPortfolioOpt/issues
-Project-URL: Personal website, https://reasonabledeviations.com Project-URL:
-Repository, https://github.com/robertmartin8/PyPortfolioOpt Description-
-Content-Type: text/markdown
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Topic :: Office/Business :: Financial
+Classifier: Topic :: Office/Business :: Financial :: Investment Provides-Extra:
+optionals Requires-Dist: cvxpy (>=1.1.19,<2.0.0) Requires-Dist: matplotlib
+(>=3.2.0,<4.0.0); extra == "optionals" Requires-Dist: numpy (>=1.22.4,<2.0.0)
+Requires-Dist: pandas (>=0.19) Requires-Dist: scikit-learn (>=0.24.1,<0.25.0);
+extra == "optionals" Requires-Dist: scipy (>=1.3,<2.0) Project-URL:
+Documentation, https://pyportfolioopt.readthedocs.io/en/latest/ Project-URL:
+Issues, https://github.com/robertmartin8/PyPortfolioOpt/issues Project-URL:
+Personal website, https://reasonabledeviations.com Project-URL: Repository,
+https://github.com/robertmartin8/PyPortfolioOpt Description-Content-Type: text/
+markdown
       [https://github.com/robertmartin8/PyPortfolioOpt/blob/master/media/
                              logo_v1.png?raw=true]
-    [python]   [pypi]   [MIT_license]   [build]   [downloads]   [binder]  
- **PyPortfolioOpt is looking for maintainers! Please reach out to the email
-address at the bottom of the readme if you're interested** PyPortfolioOpt is a
-library that implements portfolio optimization methods, including classical
-mean-variance optimization techniques and Black-Litterman allocation, as well
-as more recent developments in the field like shrinkage and Hierarchical Risk
-Parity. It is **extensive** yet easily **extensible**, and can be useful for
-either a casual investors, or a professional looking for an easy prototyping
-tool. Whether you are a fundamentals-oriented investor who has identified a
-handful of undervalued picks, or an algorithmic trader who has a basket of
-strategies, PyPortfolioOpt can help you combine your alpha sources in a risk-
-efficient way. **PyPortfolioOpt has been [published](https://joss.theoj.org/
-papers/10.21105/joss.03066) in the Journal of Open Source Software ð** Head
-over to the **[documentation on ReadTheDocs](https://
-pyportfolioopt.readthedocs.io/en/latest/)** to get an in-depth look at the
-project, or check out the [cookbook](https://github.com/robertmartin8/
-PyPortfolioOpt/tree/master/cookbook) to see some examples showing the full
-process from downloading data to building a portfolio.
+   [python]   [platforms]   [pypi]   [MIT_license]   [build]   [codecov]  
+                           [downloads]   [binder]  
+ PyPortfolioOpt is a library that implements portfolio optimization methods,
+including classical mean-variance optimization techniques and Black-Litterman
+allocation, as well as more recent developments in the field like shrinkage and
+Hierarchical Risk Parity. It is **extensive** yet easily **extensible**, and
+can be useful for either a casual investors, or a professional looking for an
+easy prototyping tool. Whether you are a fundamentals-oriented investor who has
+identified a handful of undervalued picks, or an algorithmic trader who has a
+basket of strategies, PyPortfolioOpt can help you combine your alpha sources in
+a risk-efficient way. **PyPortfolioOpt has been [published](https://
+joss.theoj.org/papers/10.21105/joss.03066) in the Journal of Open Source
+Software ð** PyPortfolioOpt is now being maintained by [Tuan Tran](https://
+github.com/88d52bdba0366127fffca9dfa93895). Head over to the **[documentation
+on ReadTheDocs](https://pyportfolioopt.readthedocs.io/en/latest/)** to get an
+in-depth look at the project, or check out the [cookbook](https://github.com/
+robertmartin8/PyPortfolioOpt/tree/master/cookbook) to see some examples showing
+the full process from downloading data to building a portfolio.
       [https://github.com/robertmartin8/PyPortfolioOpt/blob/master/media/
                      conceptual_flowchart_v2.png?raw=true]
 ## Table of contents - [Table of contents](#table-of-contents) - [Getting
 started](#getting-started) - [For development](#for-development) - [A quick
 example](#a-quick-example) - [An overview of classical portfolio optimization
 methods](#an-overview-of-classical-portfolio-optimization-methods) - [Features]
 (#features) - [Expected returns](#expected-returns) - [Risk models
@@ -65,15 +66,15 @@
 if you are on windows, you first need to installl C++. ([download](https://
 visualstudio.microsoft.com/thank-you-downloading-visual-studio/
 ?sku=BuildTools&rel=16), [install instructions](https://drive.google.com/file/
 d/0B4GsMXCRaSSIOWpYQkstajlYZ0tPVkNQSElmTWh1dXFaYkJr/view))_ This project is
 available on PyPI, meaning that you can just: ```bash pip install
 PyPortfolioOpt ``` (you may need to follow separate installation instructions
 for [cvxopt](https://cvxopt.org/install/index.html#) and [cvxpy](https://
-www.cvxpy.org/install/))). However, it is best practice to use a dependency
+www.cvxpy.org/install/)). However, it is best practice to use a dependency
 manager within a virtual environment. My current recommendation is to get
 yourself set up with [poetry](https://github.com/sdispater/poetry) then just
 run ```bash poetry add PyPortfolioOpt ``` Otherwise, clone/download the project
 and in the project directory run: ```bash python setup.py install ```
 PyPortfolioOpt supports Docker. Build your first container with `docker build -
 f docker/Dockerfile . -t pypfopt`. You can use the image to run tests or even
 launch a Jupyter server. ```bash # iPython interpreter: docker run -it pypfopt
@@ -269,14 +270,14 @@
 doi.org/10.21105/joss.03066}, year = {2021}, publisher = {The Open Journal},
 volume = {6}, number = {61}, pages = {3066}, author = {Robert Andrew Martin},
 title = {PyPortfolioOpt: portfolio optimization in Python}, journal = {Journal
 of Open Source Software} } ``` ## Contributing Contributions are _most
 welcome_. Have a look at the [Contribution Guide](https://github.com/
 robertmartin8/PyPortfolioOpt/blob/master/CONTRIBUTING.md) for more. I'd like to
 thank all of the people who have contributed to PyPortfolioOpt since its
-release in 2018. Special shout-outs to: - Philipp Schiele - Carl Peasnell -
-Felipe Schneider - Dingyuan Wang - Pat Newell - Aditya Bhutra - Thomas
-Schmelzer - Rich Caputo - Nicolas Knudde ## Getting in touch If you are having
-a problem with PyPortfolioOpt, please raise a GitHub issue. For anything else,
-you can reach me at:
+release in 2018. Special shout-outs to: - Tuan Tran (who is now the primary
+maintainer!) - Philipp Schiele - Carl Peasnell - Felipe Schneider - Dingyuan
+Wang - Pat Newell - Aditya Bhutra - Thomas Schmelzer - Rich Caputo - Nicolas
+Knudde ## Getting in touch If you are having a problem with PyPortfolioOpt,
+please raise a GitHub issue. For anything else, you can reach me at:
  [https://github.com/robertmartin8/ReasonableDeviations/blob/gh-pages/assets/
                          images/contact.png?raw=true]
```

