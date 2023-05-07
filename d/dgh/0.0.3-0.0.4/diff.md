# Comparing `tmp/dgh-0.0.3.tar.gz` & `tmp/dgh-0.0.4.tar.gz`

## Comparing `dgh-0.0.3.tar` & `dgh-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dgh-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 dgh-0.0.3/src/auxiliary.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 dgh-0.0.3/src/constants.py
--rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 dgh-0.0.3/src/dgh.py
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 dgh-0.0.3/src/fw.py
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 dgh-0.0.3/src/mappings.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 dgh-0.0.3/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 dgh-0.0.3/LICENSE
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 dgh-0.0.3/README.md
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 dgh-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 dgh-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 dgh-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dgh-0.0.4/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dgh-0.0.4/src/__init__.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 dgh-0.0.4/src/auxiliary.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 dgh-0.0.4/src/constants.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 dgh-0.0.4/src/dgh.py
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 dgh-0.0.4/src/fw.py
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 dgh-0.0.4/src/mappings.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 dgh-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 dgh-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 dgh-0.0.4/README.md
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 dgh-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 dgh-0.0.4/PKG-INFO
```

### Comparing `dgh-0.0.3/src/auxiliary.py` & `dgh-0.0.4/src/auxiliary.py`

 * *Files identical despite different names*

### Comparing `dgh-0.0.3/src/dgh.py` & `dgh-0.0.4/src/dgh.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,32 +55,33 @@
 
     dis_S = np.abs(X__Y - S @ Y__X @ S.T + S_Y_X - S_Y_X.T).max()
 
     return dis_S
 
 
 def ub(X, Y, phi_first=.1, c_first=None, iter_budget=100, center_start=False,
-       tol=1e-8, return_fg=False, verbose=False, rnd=None):
+       tol=1e-8, return_fg=False, verbose=0, rnd=None):
     """
     Find upper bound of dGH(X, Y) by minimizing smoothed dis(R) = dis(f, g) over
     the bi-mapping polytope 𝓢 using Frank-Wolfe.
 
     :param X: distance matrix of X (2d-array)
     :param Y: distance matrix of Y (2d-array)
     :param phi_first: upper bound of the non-convexity degree ∈ (0, ½) in the
         first minimization problem (float)
     :param c_first: exponentiation base ∈ (1, ∞) for smoothing the distortion
         in the first minimization problem (float)
     :param iter_budget: total number of Frank-Wolfe iterations (int)
     :param center_start: whether to try the center of 𝓢 as a starting point first (bool)
-    :param verbose: whether to print out restarts (bool)
+    :param verbose: 0=no output, 1=print restart results, 2=print iterations
     :return: dGH(X, Y), f [optional], g [optional]
     """
     n, m = len(X), len(Y)
     rnd = rnd or np.random.RandomState(DEFAULT_SEED)
+    assert (X == X.T).all() and (Y == Y.T).all(), 'distance matrices are not symmetric'
 
     # Find c for the first minimization if needed.
     if c_first is not None:
         assert c_first > 1, f'starting exponentiation base must be > 1 (c_first={c_first} )'
     else:
         assert phi_first is not None, f'either phi_first or c_start must be given'
         assert 0 < phi_first < .5, f'starting non-convexity UB must be < 0.5 ' \
@@ -127,15 +128,15 @@
         dis_R = dis(R, X, Y)
 
         # Update the best distortion achieved from all restarts.
         if dis_R < min_dis_R:
             best_f, best_g = S_to_fg(S, n, m)
             min_dis_R = dis_R
 
-        if verbose:
+        if verbose >= 1:
             print(f'finished restart {restart_idx}: ½dis(R)={dis_R/2:.4f}, '
                   f'min ½dis(R)={min_dis_R/2:.4f}')
 
         restart_idx += 1
 
     res = (min_dis_R/2, best_f, best_g) if return_fg else min_dis_R/2
```

### Comparing `dgh-0.0.3/src/fw.py` & `dgh-0.0.4/src/fw.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 from functools import partial
 
 from mappings import fg_to_R
 from auxiliary import arrange_distances
 
 
 def solve_frank_wolfe(obj, grad, find_descent_direction, minimize_obj_wrt_gamma, S0,
-                      tol=1e-8, max_iter=10, verbose=False):
+                      tol=1e-8, max_iter=10, verbose=0):
     """
     Minimize smoothed distortion over the bi-mapping polytope 𝓢.
 
     :param obj: smoothed distortion
     :param grad: ∇obj:𝓢🠒𝓢 (function)
     :param find_descent_direction: R:ℝ^(n+m)×(n+m)🠒𝓢 (function)
     :param minimize_obj_wrt_gamma: γ*:𝓢×𝓢🠒ℝ (function)
     :param S0: starting point in 𝓢 (2d-array)
     :param tol: tolerance for measuring rate of descent (float)
     :param max_iter: maximum number of iterations (int)
-    :param verbose: whether to print out iterations (bool)
+    :param verbose: :param verbose: {0,1}=no output, 2=print iterations
     :return: solution, number of iterations performed
     """
     S = S0.copy()
     iter = 0
     while iter < max_iter:
         # Find the Frank-Wolfe direction.
         grad_at_S = grad(S)
@@ -31,15 +31,15 @@
         # Find γ ∈ [0, 1] defining how much to go in the decided direction.
         global_gamma = minimize_obj_wrt_gamma(S, D)
         critical_gammas = {0, 1}
         if 0 < global_gamma < 1:
             critical_gammas.add(global_gamma)
         gamma = min(critical_gammas, key=lambda x: obj(S + x*D))
 
-        if verbose:
+        if verbose >= 2:
             print(f'  iter {iter}: obj(S)={obj(S):.4f}, γ={gamma:.5f}')
 
         # Stop if the rate of descent is too small or if the line search stalls.
         if np.sum(-grad_at_S * D) < tol or np.isclose(gamma, 0):
             break
 
         # Move S by γ towards R, i.e. to (1-γ)S + γR.
```

### Comparing `dgh-0.0.3/src/mappings.py` & `dgh-0.0.4/src/mappings.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     n, m = len(f), len(g)
     nxn_zeros, mxm_zeros = (np.zeros((size, size), dtype=int) for size in [n, m])
 
     # Construct matrix representations of the mappings.
     F = np.identity(m)[f]
     G = np.identity(n)[g]
 
-    R = np.block([[F, mxm_zeros], [nxn_zeros, G]])
+    R = np.block([[F, nxn_zeros], [mxm_zeros, G]])
 
     return R
 
 
 def S_to_fg(S, n, m):
     """
     Projects a soft mapping pair onto the space of mapping pairs.
```

### Comparing `dgh-0.0.3/LICENSE` & `dgh-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dgh-0.0.3/pyproject.toml` & `dgh-0.0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dgh"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   {name="Vladyslav Oles", email="vlad.oles@proton.me"},
 ]
 description = "Computing the Gromov–Hausdorff distance"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.5"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

