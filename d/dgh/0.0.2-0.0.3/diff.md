# Comparing `tmp/dgh-0.0.2.tar.gz` & `tmp/dgh-0.0.3.tar.gz`

## Comparing `dgh-0.0.2.tar` & `dgh-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 dgh-0.0.2/auxiliary.py
--rw-r--r--   0        0        0     5250 2020-02-02 00:00:00.000000 dgh-0.0.2/dgh.py
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 dgh-0.0.2/fw.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 dgh-0.0.2/mappings.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 dgh-0.0.2/LICENSE
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 dgh-0.0.2/README.md
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 dgh-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 dgh-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dgh-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 dgh-0.0.3/src/auxiliary.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 dgh-0.0.3/src/constants.py
+-rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 dgh-0.0.3/src/dgh.py
+-rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 dgh-0.0.3/src/fw.py
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 dgh-0.0.3/src/mappings.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 dgh-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 dgh-0.0.3/LICENSE
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 dgh-0.0.3/README.md
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 dgh-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 dgh-0.0.3/PKG-INFO
```

### Comparing `dgh-0.0.2/auxiliary.py` & `dgh-0.0.3/src/auxiliary.py`

 * *Files identical despite different names*

### Comparing `dgh-0.0.2/dgh.py` & `dgh-0.0.3/src/dgh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 import scipy.optimize as opt
 
-from mappings import rnd_S, center, S_to_fg, S_to_R, DEFAULT_SEED
+from mappings import rnd_S, center, S_to_fg, S_to_R
 from fw import make_frank_wolfe_solver
 from auxiliary import arrange_distances
+from constants import DEFAULT_SEED, MAX_C
 
 
 def find_c(phi, X, Y):
     """
     Find c > 1 s.t. the Hessian is at most φ away from the set of positive
     semidefinite matrices (w.r.t. normalized nuclear norm-induced distance).
 
@@ -53,87 +54,89 @@
     S_Y_X = S @ _Y_X
 
     dis_S = np.abs(X__Y - S @ Y__X @ S.T + S_Y_X - S_Y_X.T).max()
 
     return dis_S
 
 
-def ub(X, Y, phi_first=.1, c_first=None, n_restarts=1, center_start=False, max_iter=10,
+def ub(X, Y, phi_first=.1, c_first=None, iter_budget=100, center_start=False,
        tol=1e-8, return_fg=False, verbose=False, rnd=None):
     """
     Find upper bound of dGH(X, Y) by minimizing smoothed dis(R) = dis(f, g) over
     the bi-mapping polytope 𝓢 using Frank-Wolfe.
 
     :param X: distance matrix of X (2d-array)
     :param Y: distance matrix of Y (2d-array)
     :param phi_first: upper bound of the non-convexity degree ∈ (0, ½) in the
         first minimization problem (float)
     :param c_first: exponentiation base ∈ (1, ∞) for smoothing the distortion
         in the first minimization problem (float)
+    :param iter_budget: total number of Frank-Wolfe iterations (int)
     :param center_start: whether to try the center of 𝓢 as a starting point first (bool)
-    :param n_restarts: number of restarts for the minimization sequence (int)
-    :param max_iter: maximum number of Frank-Wolfe iterations (int)
     :param verbose: whether to print out restarts (bool)
     :return: dGH(X, Y), f [optional], g [optional]
     """
     n, m = len(X), len(Y)
+    rnd = rnd or np.random.RandomState(DEFAULT_SEED)
 
     # Find c for the first minimization if needed.
     if c_first is not None:
         assert c_first > 1, f'starting exponentiation base must be > 1 (c_first={c_first} )'
     else:
         assert phi_first is not None, f'either phi_first or c_start must be given'
         assert 0 < phi_first < .5, f'starting non-convexity UB must be < 0.5 ' \
                                    f'(phi_first={phi_first})'
         c_first = find_c(phi_first, X, Y)
 
-    # Initialize the starting points.
-    rnd = rnd or np.random.RandomState(DEFAULT_SEED)
-    S0s = [rnd_S(n, m, rnd) for _ in range(n_restarts)]
-    if center_start:
-        S0s[0] = center(n, m)
-
-    # Find a solution for each of the starting points.
+    # Find minima from new restarts until run out of iteration budget.
     min_dis_R = np.inf
     fw_seq = []
-    for restart, S in enumerate(S0s):
+    restart_idx = 0
+    while iter_budget > 0:
+        # Initialize new restart.
+        S = center(n, m) if restart_idx == 0 and center_start else rnd_S(n, m, rnd)
         fw_idx = 0
         c = c_first
-        remaining_iter = max_iter
+
         # Run a sequence of FW solvers using solutions as subsequent warm starts.
-        while remaining_iter > 0:
+        stopping = False
+        while not stopping:
             # Set up next FW solver in the sequence if needed.
             try:
                 fw = fw_seq[fw_idx]
             except IndexError:
-                fw = make_frank_wolfe_solver(X, Y, c, max_iter=max_iter, tol=tol, verbose=verbose)
+                fw = make_frank_wolfe_solver(
+                    X, Y, c, tol=tol, verbose=verbose)
                 fw_seq.append(fw)
 
             # Solve the minimization problem.
-            S, used_iter = fw(S0=S, max_iter=remaining_iter)
+            S, used_iter = fw(S0=S, max_iter=iter_budget)
 
-            # Terminate if no iterations were made.
-            if used_iter == 0:
-                break
+            # Terminate if no iterations were made, run out of iteration budget,
+            # or next c will exceed floating point arithmetic limits.
+            stopping = iter_budget == used_iter or used_iter == 0 or c > MAX_C
 
             # Move to the next minimization obtained by squaring c.
-            remaining_iter -= used_iter
+            iter_budget -= used_iter
             fw_idx += 1
-            c **= 2
+            with np.errstate(over='ignore'):
+                c **= 2
 
         # Project the solution to the set of correspondences and find the
         # resulting distortion.
         R = S_to_R(S, n, m)
         dis_R = dis(R, X, Y)
 
-        # Update the best distortion achieved across all restarts.
+        # Update the best distortion achieved from all restarts.
         if dis_R < min_dis_R:
             best_f, best_g = S_to_fg(S, n, m)
             min_dis_R = dis_R
 
         if verbose:
-            print(f'finished restart {restart}: ½dis(R)={dis_R/2:.4f}, '
+            print(f'finished restart {restart_idx}: ½dis(R)={dis_R/2:.4f}, '
                   f'min ½dis(R)={min_dis_R/2:.4f}')
 
+        restart_idx += 1
+
     res = (min_dis_R/2, best_f, best_g) if return_fg else min_dis_R/2
 
     return res
```

### Comparing `dgh-0.0.2/fw.py` & `dgh-0.0.3/src/fw.py`

 * *Files identical despite different names*

### Comparing `dgh-0.0.2/mappings.py` & `dgh-0.0.3/src/mappings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
+from constants import DEFAULT_SEED
 
-DEFAULT_SEED = 666
 
 def rnd_S(n, m, rnd=None):
     """
     Generates random soft mapping in X🠖Y as a point in the bi-mapping polytope 𝓢.
 
     :param n: cardinality of X (int)
     :param m: cardinality of Y (int)
```

### Comparing `dgh-0.0.2/LICENSE` & `dgh-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dgh-0.0.2/README.md` & `dgh-0.0.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,3 +1,5 @@
 # dGH
 
-Computes the Gromov–Hausdorff distance $d_\text{GH}(X, Y)$ by solving (a parametric family of) quadratic minimizations with affine constraints, whose solutions are guaranteed to deliver $d_\text{GH}(X, Y)$ for sufficiently large value of the parameter $c$. The minimizations are solved using the Frank-Wolfe algorithm in $O(n^3)$ time per its iteration, where $n = |X| + |Y|$ is the total number of points. Even when the algorithm fails to find a global minimum, the resulting solution provides an upper bound for $d_\text{GH}(X, Y)$.
+Computes the Gromov–Hausdorff distance $d_\text{GH}(X, Y)$ by solving (a parametric family of) quadratic minimizations with affine constraints, whose solutions are guaranteed to deliver $d_\text{GH}(X, Y)$ for sufficiently large value of the parameter $c$. The minimizations are solved using the Frank-Wolfe algorithm in $O(n^3)$ time per its iteration, where $n = |X| + |Y|$ is the total number of points. Even when the algorithm fails to find a global minimum, the resulting solution provides an upper bound for $d_\text{GH}(X, Y)$.
+
+A manuscript describing the underlying theory is currently in preparation.
```

### Comparing `dgh-0.0.2/pyproject.toml` & `dgh-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dgh"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   {name="Vladyslav Oles", email="vlad.oles@proton.me"},
 ]
 description = "Computing the Gromov–Hausdorff distance"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dgh-0.0.2/PKG-INFO` & `dgh-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: dgh
-Version: 0.0.2
+Version: 0.0.3
 Summary: Computing the Gromov–Hausdorff distance
 Project-URL: Homepage, https://github.com/pypa/dgh
 Project-URL: Bug Tracker, https://github.com/pypa/dgh/issues
 Author-email: Vladyslav Oles <vlad.oles@proton.me>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # dGH
 
-Computes the Gromov–Hausdorff distance $d_\text{GH}(X, Y)$ by solving (a parametric family of) quadratic minimizations with affine constraints, whose solutions are guaranteed to deliver $d_\text{GH}(X, Y)$ for sufficiently large value of the parameter $c$. The minimizations are solved using the Frank-Wolfe algorithm in $O(n^3)$ time per its iteration, where $n = |X| + |Y|$ is the total number of points. Even when the algorithm fails to find a global minimum, the resulting solution provides an upper bound for $d_\text{GH}(X, Y)$.
+Computes the Gromov–Hausdorff distance $d_\text{GH}(X, Y)$ by solving (a parametric family of) quadratic minimizations with affine constraints, whose solutions are guaranteed to deliver $d_\text{GH}(X, Y)$ for sufficiently large value of the parameter $c$. The minimizations are solved using the Frank-Wolfe algorithm in $O(n^3)$ time per its iteration, where $n = |X| + |Y|$ is the total number of points. Even when the algorithm fails to find a global minimum, the resulting solution provides an upper bound for $d_\text{GH}(X, Y)$.
+
+A manuscript describing the underlying theory is currently in preparation.
```

