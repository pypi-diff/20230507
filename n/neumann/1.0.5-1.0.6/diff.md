# Comparing `tmp/neumann-1.0.5.tar.gz` & `tmp/neumann-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neumann-1.0.5.tar", last modified: Fri Apr 14 22:48:24 2023, max compression
+gzip compressed data, was "neumann-1.0.6.tar", last modified: Sun May  7 16:54:48 2023, max compression
```

## Comparing `neumann-1.0.5.tar` & `neumann-1.0.6.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.336143 neumann-1.0.5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-04-14 22:48:17.000000 neumann-1.0.5/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-04-14 22:48:17.000000 neumann-1.0.5/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5753 2023-04-14 22:48:24.336143 neumann-1.0.5/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4789 2023-04-14 22:48:17.000000 neumann-1.0.5/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-04-14 22:48:17.000000 neumann-1.0.5/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2023-04-14 22:48:17.000000 neumann-1.0.5/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-14 22:48:24.336143 neumann-1.0.5/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-04-14 22:48:17.000000 neumann-1.0.5/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.324144 neumann-1.0.5/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.328143 neumann-1.0.5/src/neumann/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.328143 neumann-1.0.5/src/neumann/approx/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/approx/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3697 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/approx/func.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7210 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/approx/lagrange.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9853 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/approx/mls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5607 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/arraysetops.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/decorate.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.332143 neumann-1.0.5/src/neumann/function/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/function/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2530 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/function/constraint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9141 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/function/function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2656 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/function/functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3851 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/function/metafunction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2875 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/function/relation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/function/testfunction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/hist.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.332143 neumann-1.0.5/src/neumann/linalg/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5029 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/abstract.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      443 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26648 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/frame.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.332143 neumann-1.0.5/src/neumann/linalg/frontal/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/frontal/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8015 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/frontal/frontal.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2131 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/frontal/frutils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7447 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/frontal/path.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1103 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/frontal/postproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10580 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/frontal/proc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1605 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/frontal/topo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12864 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/meta.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7996 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/solve.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.336143 neumann-1.0.5/src/neumann/linalg/sparse/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/sparse/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10045 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/sparse/csr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10297 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/sparse/jaggedarray.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1224 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/sparse/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12663 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/tensor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3137 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/top.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24706 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6769 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/linalg/vector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4333 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/logical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3811 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/numint.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.336143 neumann-1.0.5/src/neumann/optimize/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/optimize/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/optimize/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14973 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/optimize/ga.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31396 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/optimize/lp.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.336143 neumann-1.0.5/src/neumann/topology/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/topology/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5492 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/topology/graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13118 2023-04-14 22:48:17.000000 neumann-1.0.5/src/neumann/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.328143 neumann-1.0.5/src/neumann.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5753 2023-04-14 22:48:24.000000 neumann-1.0.5/src/neumann.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1856 2023-04-14 22:48:24.000000 neumann-1.0.5/src/neumann.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-14 22:48:24.000000 neumann-1.0.5/src/neumann.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-14 22:48:24.000000 neumann-1.0.5/src/neumann.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2023-04-14 22:48:24.000000 neumann-1.0.5/src/neumann.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-04-14 22:48:24.000000 neumann-1.0.5/src/neumann.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-14 22:48:24.336143 neumann-1.0.5/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1185 2023-04-14 22:48:17.000000 neumann-1.0.5/tests/test_approx.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4268 2023-04-14 22:48:17.000000 neumann-1.0.5/tests/test_function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2220 2023-04-14 22:48:17.000000 neumann-1.0.5/tests/test_ga.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      579 2023-04-14 22:48:17.000000 neumann-1.0.5/tests/test_graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33836 2023-04-14 22:48:17.000000 neumann-1.0.5/tests/test_linalg.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3776 2023-04-14 22:48:17.000000 neumann-1.0.5/tests/test_logical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7684 2023-04-14 22:48:17.000000 neumann-1.0.5/tests/test_lpp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      682 2023-04-14 22:48:17.000000 neumann-1.0.5/tests/test_numint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3932 2023-04-14 22:48:17.000000 neumann-1.0.5/tests/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.153205 neumann-1.0.6/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-05-07 16:54:42.000000 neumann-1.0.6/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-05-07 16:54:42.000000 neumann-1.0.6/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5753 2023-05-07 16:54:48.153205 neumann-1.0.6/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4789 2023-05-07 16:54:42.000000 neumann-1.0.6/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-05-07 16:54:42.000000 neumann-1.0.6/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2023-05-07 16:54:42.000000 neumann-1.0.6/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-07 16:54:48.153205 neumann-1.0.6/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-05-07 16:54:42.000000 neumann-1.0.6/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.145205 neumann-1.0.6/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.145205 neumann-1.0.6/src/neumann/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.149205 neumann-1.0.6/src/neumann/approx/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/approx/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3697 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/approx/func.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7210 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/approx/lagrange.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9840 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/approx/mls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5607 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/arraysetops.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/decorate.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.149205 neumann-1.0.6/src/neumann/function/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/function/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2530 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/function/constraint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9141 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/function/function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2656 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/function/functions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3851 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/function/metafunction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2875 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/function/relation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/function/testfunction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/hist.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.149205 neumann-1.0.6/src/neumann/linalg/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5029 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/abstract.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      443 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24717 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/frame.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.153205 neumann-1.0.6/src/neumann/linalg/frontal/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/frontal/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8015 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/frontal/frontal.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2131 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/frontal/frutils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7447 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/frontal/path.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1103 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/frontal/postproc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10580 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/frontal/proc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1605 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/frontal/topo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12875 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/meta.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7996 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/solve.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.153205 neumann-1.0.6/src/neumann/linalg/sparse/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/sparse/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10045 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/sparse/csr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10297 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/sparse/jaggedarray.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1224 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/sparse/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12663 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/tensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3137 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/top.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29691 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6763 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/vector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4333 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/logical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3811 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/numint.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.153205 neumann-1.0.6/src/neumann/optimize/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/optimize/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/optimize/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14973 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/optimize/ga.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31396 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/optimize/lp.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.153205 neumann-1.0.6/src/neumann/topology/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/topology/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5492 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/topology/graph.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13118 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.149205 neumann-1.0.6/src/neumann.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5753 2023-05-07 16:54:48.000000 neumann-1.0.6/src/neumann.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1856 2023-05-07 16:54:48.000000 neumann-1.0.6/src/neumann.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-07 16:54:48.000000 neumann-1.0.6/src/neumann.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-07 16:54:48.000000 neumann-1.0.6/src/neumann.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2023-05-07 16:54:48.000000 neumann-1.0.6/src/neumann.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-05-07 16:54:48.000000 neumann-1.0.6/src/neumann.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.153205 neumann-1.0.6/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1185 2023-05-07 16:54:42.000000 neumann-1.0.6/tests/test_approx.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4268 2023-05-07 16:54:42.000000 neumann-1.0.6/tests/test_function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2220 2023-05-07 16:54:42.000000 neumann-1.0.6/tests/test_ga.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      579 2023-05-07 16:54:42.000000 neumann-1.0.6/tests/test_graph.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33834 2023-05-07 16:54:42.000000 neumann-1.0.6/tests/test_linalg.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3776 2023-05-07 16:54:42.000000 neumann-1.0.6/tests/test_logical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7684 2023-05-07 16:54:42.000000 neumann-1.0.6/tests/test_lpp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      682 2023-05-07 16:54:42.000000 neumann-1.0.6/tests/test_numint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3932 2023-05-07 16:54:42.000000 neumann-1.0.6/tests/test_utils.py
```

### Comparing `neumann-1.0.5/LICENSE` & `neumann-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/PKG-INFO` & `neumann-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: neumann
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python Library for Applied Mathematics in Physical Sciences.
 Home-page: https://github.com/dewloosh/Neumann
-Download-URL: https://github.com/dewloosh/Neumann/archive/refs/tags/1.0.5.zip
+Download-URL: https://github.com/dewloosh/Neumann/archive/refs/tags/1.0.6.zip
 Author: Bence Balogh
 Author-email: dewloosh@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `neumann-1.0.5/README.md` & `neumann-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/setup.py` & `neumann-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/approx/func.py` & `neumann-1.0.6/src/neumann/approx/func.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/approx/lagrange.py` & `neumann-1.0.6/src/neumann/approx/lagrange.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/approx/mls.py` & `neumann-1.0.6/src/neumann/approx/mls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from numba import njit
 import numpy as np
 from scipy.special import factorial as fact
 from numpy import outer
 from collections.abc import Iterable
 from numba import njit
 
 
@@ -66,15 +65,15 @@
 
     assert isinstance(points, np.ndarray)
     assert isinstance(values, np.ndarray)
     assert points.shape[0] == values.shape[0]
     dim = points.shape[1]
     try:
         rec = values.shape[1]
-    except:
+    except Exception:
         rec = 1
 
     if isMLSWeightFunction(w):
         assert dim == w.dimension
     else:
         w = ConstantWeightFunction(dim)
```

### Comparing `neumann-1.0.5/src/neumann/arraysetops.py` & `neumann-1.0.6/src/neumann/arraysetops.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/decorate.py` & `neumann-1.0.6/src/neumann/decorate.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/function/constraint.py` & `neumann-1.0.6/src/neumann/function/constraint.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/function/function.py` & `neumann-1.0.6/src/neumann/function/function.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/function/functions.py` & `neumann-1.0.6/src/neumann/function/functions.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/function/metafunction.py` & `neumann-1.0.6/src/neumann/function/metafunction.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/function/relation.py` & `neumann-1.0.6/src/neumann/function/relation.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/function/testfunction.py` & `neumann-1.0.6/src/neumann/function/testfunction.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/hist.py` & `neumann-1.0.6/src/neumann/hist.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/linalg/abstract.py` & `neumann-1.0.6/src/neumann/linalg/abstract.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/linalg/frame.py` & `neumann-1.0.6/src/neumann/linalg/frame.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Iterable, Callable
 from copy import deepcopy as dcopy
 
 import numpy as np
 from numpy import ndarray
-from sympy.physics.vector import ReferenceFrame as SymPyFrame
 
 from dewloosh.core.typing import issequence
 
 from .utils import (
-    _transpose_multi,
     is_rectangular_frame,
     is_orthonormal_frame,
     is_normal_frame,
     normalize_frame,
     Gram,
     dual_frame,
     transpose_axes,
+    show_frame,
+    rotation_matrix
 )
 from ..utils import repeat
 from .meta import FrameLike, TensorLike, ArrayWrapper
 
 
 __all__ = ["ReferenceFrame", "RectangularFrame", "CartesianFrame"]
 
 
-def inplace_binary(obj: FrameLike, other, bop: Callable, rtype: FrameLike = None):
+def inplace_binary(obj: FrameLike, other, bop: Callable, rtype: FrameLike = None) -> FrameLike:
     """
     Performs a binary operation inplace. Components of registered tensorial entities
     are transformed accordingly and registered to the output frame.
     """
     axes = np.copy(obj.show())
     bop(axes, other, out=(axes,))
     if rtype:
@@ -51,20 +51,20 @@
     An important feature of the class is that it maintains the property of objectivity
     of the tensorial quantities that use instances of this class in their representation.
     Upon transformation of a frame, the components of the associated tensorial quantities
     transform correspondingly.
 
     Parameters
     ----------
-    axes : numpy.ndarray, Optional
+    axes: numpy.ndarray, Optional
         2d numpy array of floats specifying cartesian reference frames.
         Default is None.
-    dim : int, Optional
+    dim: int, Optional
         Dimension of the mesh. Default is 3.
-    name : str, Optional
+    name: str, Optional
         The name of the frame. Default is None.
 
     Notes
     -----
     1) The object is able to handle any reference frame, not just cartesian ones.
     The only restriction is that the base vectors should be linearly independent.
     2) All NumPy universal functions return ReferenceFrame instances. If for a NumPy
@@ -75,15 +75,15 @@
 
     Examples
     --------
     Define a frame and rotate it around axis 'Z' with an amount of 180 degrees:
 
     >>> from neumann.linalg import ReferenceFrame
     >>> A = ReferenceFrame(dim=3)
-    >>> B = A.orient_new('Body', [0, 0, np.pi], 'XYZ')
+    >>> B = A.orient_new('Space', [0, 0, np.pi], 'XYZ')
 
     If we define a tensorial quantity with components in a frame, the
     components of the quantity change if the frame changes:
 
     >>> from neumann.linalg import Vector
     >>> v = Vector([1., 0, 0], frame=A)
     >>> A *= 2.0
@@ -137,24 +137,23 @@
     >>> v
     Array([0.5, 0. , 0. ])
 
     To get the matrix that transforms quantities from frame A to frame B,
     use the `dcm` method:
 
     >>> source = ReferenceFrame(dim=3)
-    >>> target = source.orient_new('Body', [0, 0, 90*np.pi/180],  'XYZ')
+    >>> target = source.orient_new('Space', [0, 0, 90*np.pi/180],  'XYZ')
     >>> DCM = source.dcm(target=target)
 
     or equivalenty
 
     >>> DCM = target.dcm(source=source)
 
     See Also
     --------
-    :class:`sympy.physics.ReferenceFrame`
     :class:`~neumann.linalg.RectangularFrame`
     :class:`~neumann.linalg.CartesianFrame`
     """
 
     def __init__(self, axes: ndarray = None, *args, name: str = None, dim: int = None):
         try:
             if not isinstance(axes, ndarray):
@@ -266,37 +265,38 @@
         Sets the array of the frame.
         """
         if isinstance(value, np.ndarray):
             buf = value
         else:
             if not issequence(value):
                 raise TypeError("'value' must be some kind of iterable")
-            buf = np.array(value)
+            buf = np.array(value).astype(float)
         value = self._array_cls_(shape=buf.shape, buffer=buf, dtype=buf.dtype)
         if value.shape == self._array.shape:
             if self._weakrefs and len(self._weakrefs) > 0:
                 target = ReferenceFrame(value)
                 dcm = self.dcm(target=target)
                 for v in self._weakrefs.values():
                     arr = v.show(dcm=dcm)
                     v.array = arr
             self._array = value
         else:
-            raise RuntimeError("Mismatch in data dimensinons!")
+            raise ValueError("Mismatch in data dimensinons!")
 
     def show(self, target: "ReferenceFrame" = None) -> ndarray:
         """
         Returns the components of the current frame in a target frame.
         If the target is None, the componants are returned in the ambient frame.
 
         Returns
         -------
         numpy.ndarray
         """
-        return self.dcm(target=target)
+        return self.dcm(source=target)
+        #return show_frame(self.dcm(target=target), eye_like(self.axes))
 
     def dcm(
         self, *, target: "ReferenceFrame" = None, source: "ReferenceFrame" = None
     ) -> ndarray:
         """
         Returns the direction cosine matrix (DCM) of a transformation
         from a source (S) to a target (T) frame. The current frame can be
@@ -307,152 +307,112 @@
 
         If `source` is not `None`, then T=self.
 
         If `target` is not `None`, then S=self.
 
         Parameters
         ----------
-        source : 'ReferenceFrame', Optional
+        source: 'ReferenceFrame', Optional
             Source frame. Default is None.
-        target : 'ReferenceFrame', Optional
+        target: 'ReferenceFrame', Optional
             Target frame. Default is None.
 
         Returns
         -------
         numpy.ndarray
             DCM matrix from S to T.
 
         Example
         -------
         >>> from neumann.linalg import ReferenceFrame
         >>> import numpy as np
         >>> source = ReferenceFrame(dim=3)
-        >>> target = source.orient_new('Body', [0, 0, 90*np.pi/180],  'XYZ')
+        >>> target = source.orient_new('Space', [0, 0, 90*np.pi/180],  'XYZ')
         >>> DCM = source.dcm(target=target)
         >>> arr_source = np.array([3 ** 0.5 / 2, 0.5, 0])
         >>> arr_target = DCM @ arr_source
         """
         if source is not None:
             S, T = source.dcm(), self.dual().dcm()
             return T @ transpose_axes(S)
         elif target is not None:
             S, T = self.dcm(), target.dual().dcm()
             if len(S.shape) == 3:
-                return T @ _transpose_multi(S)
+                return T @ transpose_axes(S)
             elif len(S.shape) == 2:
                 return T @ transpose_axes(S)
             else:  # pragma: no cover
                 msg = (
                     "There is no transformation rule implemented for"
                     " source shape {} and target shape {}"
                 )
                 raise NotImplementedError(msg.format(S.shape, T.shape))
         # We only get here if the function is called without arguments.
         # The DCM from the ambient frame to the current frame is returned.
         return self.axes
 
     def orient(self, *args, **kwargs) -> "ReferenceFrame":
         """
-        Orients the current frame inplace.
-        See :func:`orient_new` for the possible arguments.
-
-        Parameters
-        ----------
-        args : tuple, Optional
-            A tuple of arguments to pass to the `orientnew`
-            function in `sympy`.
-        kwargs : dict, Optional
-            A dictionary of keyword arguments to pass to the
-            `orientnew` function in `sympy`.
+        Orients the current frame inplace. All arguments are forwarded
+        to :func:`~neumann.linalg.utils.rotation_matrix`, see there for the 
+        details.
 
         Returns
         -------
         ReferenceFrame
 
         Example
         -------
         Define a standard Cartesian frame and rotate it around axis 'Z'
         with 180 degrees:
 
         >>> A = ReferenceFrame(dim=3)
-        >>> A.orient('Body', [0, 0, np.pi], 'XYZ')
-        Array([[-1.0000000e+00,  1.2246468e-16,  0.0000000e+00],
+        >>> A.orient('Space', [0, 0, np.pi], 'XYZ')
+        array([[-1.0000000e+00,  1.2246468e-16,  0.0000000e+00],
                [-1.2246468e-16, -1.0000000e+00,  0.0000000e+00],
                [ 0.0000000e+00,  0.0000000e+00,  1.0000000e+00]])
 
         See Also
         --------
         :func:`orient_new`
+        :func:`~neumann.linalg.utils.rotation_matrix`
         """
-        source = SymPyFrame("S")
-        target = source.orientnew("T", *args, **kwargs)
-        dcm = np.array(target.dcm(source).evalf()).astype(float)
-        self._array = dcm @ self.axes
+        dcm = rotation_matrix(*args, **kwargs)
+        self._array = show_frame(dcm.T, self.axes)
         return self
 
     def orient_new(self, *args, name="", **kwargs) -> "ReferenceFrame":
         """
         Returns a new frame, oriented relative to the called object.
-        The orientation can be provided by all ways supported in
-        `sympy.physics.vector.ReferenceFrame.orientnew`.
+        All extra positional and keyword arguments are forwarded to 
+        :func:`~neumann.linalg.utils.rotation_matrix`, see there for the 
+        details.
 
         Parameters
         ----------
-        name : str
+        name: str
             Name for the new reference frame.
-        rot_type : str
-            The method used to generate the direction cosine matrix. Supported
-            methods are:
-
-            - ``'Axis'``: simple rotations about a single common axis
-            - ``'DCM'``: for setting the direction cosine matrix directly
-            - ``'Body'``: three successive rotations about new intermediate
-              axes, also called "Euler and Tait-Bryan angles"
-            - ``'Space'``: three successive rotations about the parent
-              frames' unit vectors
-            - ``'Quaternion'``: rotations defined by four parameters which
-              result in a singularity free direction cosine matrix
-        amounts : str
-            Expressions defining the rotation angles or direction cosine
-            matrix. These must match the ``rot_type``. See examples below for
-            details. The input types are:
-
-            - ``'Axis'``: 2-tuple (expr/sym/func, Vector)
-            - ``'DCM'``: Matrix, shape(3, 3)
-            - ``'Body'``: 3-tuple of expressions, symbols, or functions
-            - ``'Space'``: 3-tuple of expressions, symbols, or functions
-            - ``'Quaternion'``: 4-tuple of expressions, symbols, or
-              functions
-        rot_order : str or int, Optional
-            If applicable, the order of the successive of rotations. The string
-            ``'123'`` and integer ``123`` are equivalent, for example. Required
-            for ``'Body'`` and ``'Space'``.
-        *args : tuple, Optional
-            Extra positional arguments forwarded to `sympy.orientnew`.
-            Default is None.
-        **kwargs : dict, Optional
-            Extra keyword arguments forwarded to `sympy.orientnew`.
-            Default is None.
-
+        
         Returns
         -------
         ReferenceFrame
             A new ReferenceFrame object.
 
         See Also
         --------
-        :func:`sympy.physics.vector.ReferenceFrame.orientnew`
+        :func:`orient`
+        :func:`~neumann.linalg.utils.rotation_matrix`
 
         Example
         -------
         Define a standard Cartesian frame and rotate it around axis 'Z'
         with 180 degrees:
 
         >>> A = ReferenceFrame(dim=3)
-        >>> B = A.orient_new('Body', [0, 0, np.pi], 'XYZ')
+        >>> B = A.orient_new('Space', [0, 0, np.pi], 'XYZ')
         """
         result = self.deepcopy(name=name)
         if (len(args) + len(kwargs)) == 0:
             return result
         else:
             result.orient(*args, **kwargs)
             return result
@@ -461,31 +421,31 @@
         """
         Alias for `orient` and `orient_new`, all extra arguments are forwarded.
 
         .. versionadded:: 0.0.4
 
         Parameters
         ----------
-        inplace : bool, Optional
+        inplace: bool, Optional
             If True, transformation is carried out on the instance the function call
             is made upon, otherwise a new frame is returned. Default is True.
 
         Returns
         -------
         ReferenceFrame
-            An exisitng (if inplace is True) or a new ReferenceFrame object.
+            An exisitng (if inplace is `True`) or a new ReferenceFrame object.
 
         Example
         -------
         Define a standard Cartesian frame and rotate it around axis 'Z'
         with 180 degrees:
 
         >>> A = ReferenceFrame(dim=3)
-        >>> A.rotate('Body', [0, 0, np.pi], 'XYZ')
-        Array([[-1.0000000e+00,  1.2246468e-16,  0.0000000e+00],
+        >>> A.rotate('Space', [0, 0, np.pi], 'XYZ')
+        array([[-1.0000000e+00,  1.2246468e-16,  0.0000000e+00],
                [-1.2246468e-16, -1.0000000e+00,  0.0000000e+00],
                [ 0.0000000e+00,  0.0000000e+00,  1.0000000e+00]])
 
         See Also
         --------
         :func:`orient`
         :func:`orient_new`
@@ -710,16 +670,16 @@
     >>> A += 2
     >>> type(A)
     <class 'neumann.linalg.frame.ReferenceFrame'>
 
     The only operation that results in a CartesianFrame object is a rotation:
 
     >>> A = CartesianFrame(dim=3)
-    >>> A.orient('Body', [0, 0, np.pi], 'XYZ')
-    Array([[-1.0000000e+00,  1.2246468e-16,  0.0000000e+00],
+    >>> A.orient('Space', [0, 0, np.pi], 'XYZ')
+    array([[-1.0000000e+00,  1.2246468e-16,  0.0000000e+00],
            [-1.2246468e-16, -1.0000000e+00,  0.0000000e+00],
            [ 0.0000000e+00,  0.0000000e+00,  1.0000000e+00]])
 
     >>> type(A)
     <class 'neumann.linalg.frame.CartesianFrame'>
 
     See also
```

### Comparing `neumann-1.0.5/src/neumann/linalg/frontal/frontal.py` & `neumann-1.0.6/src/neumann/linalg/frontal/frontal.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/linalg/frontal/frutils.py` & `neumann-1.0.6/src/neumann/linalg/frontal/frutils.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/linalg/frontal/path.py` & `neumann-1.0.6/src/neumann/linalg/frontal/path.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/linalg/frontal/postproc.py` & `neumann-1.0.6/src/neumann/linalg/frontal/postproc.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/linalg/frontal/proc.py` & `neumann-1.0.6/src/neumann/linalg/frontal/proc.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/linalg/frontal/topo.py` & `neumann-1.0.6/src/neumann/linalg/frontal/topo.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/linalg/meta.py` & `neumann-1.0.6/src/neumann/linalg/meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
 
 class TensorLike(ArrayWrapper):
     """
     Abstract base class for numerical data classes that walk and talk like
     a tensor does.
     """
 
-    _frame_cls_ = None
+    _frame_cls_: FrameLike = None
     _rank_: int = None
 
     def __init__(
         self,
         *args,
         frame: FrameLike = None,
         bulk: bool = None,
```

### Comparing `neumann-1.0.5/src/neumann/linalg/solve.py` & `neumann-1.0.6/src/neumann/linalg/solve.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/linalg/sparse/csr.py` & `neumann-1.0.6/src/neumann/linalg/sparse/csr.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/linalg/sparse/jaggedarray.py` & `neumann-1.0.6/src/neumann/linalg/sparse/jaggedarray.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/linalg/sparse/utils.py` & `neumann-1.0.6/src/neumann/linalg/sparse/utils.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/linalg/tensor.py` & `neumann-1.0.6/src/neumann/linalg/tensor.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/linalg/top.py` & `neumann-1.0.6/src/neumann/linalg/top.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/linalg/utils.py` & `neumann-1.0.6/src/neumann/linalg/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from typing import Union
+from typing import Union, Iterable
 import numbers
 import itertools
 
 import numpy as np
 from numpy import ndarray
 from numba import njit, prange, guvectorize as guv
 import sympy as sy
 from sympy import symbols, Matrix
+from sympy.physics.vector import ReferenceFrame as SymPyFrame
 
 from dewloosh.core.tools.alphabet import latinrange
 
 from .meta import TensorLike, ArrayWrapper, FrameLike
 from .exceptions import LinalgOperationInputError, LinalgMissingInputError
 
 __cache = True
@@ -46,18 +47,84 @@
     "normalize",
     "normalize2d",
     "norm",
     "norm2d",
     "linspace",
     "linspace1d",
     "inv",
-    "show_vector"
+    "show_vector",
+    "show_frame",
+    "rotation_matrix"
 ]
 
 
+def rotation_matrix(
+    rot_type: str,
+    amounts: Iterable,
+    rot_order: Union[str, int] = ''
+) -> ndarray:
+    """
+    Returns a rotation matrix using the mechanism provided by
+    `sympy.physics.vector.ReferenceFrame.orientnew`.
+
+    Parameters
+    ----------
+    rot_type: str
+        The method used to generate the direction cosine matrix. Supported
+        methods are:
+
+        - ``'Axis'``: simple rotations about a single common axis
+        - ``'DCM'``: for setting the direction cosine matrix directly
+        - ``'Body'``: three successive rotations about new intermediate
+            axes, also called "Euler and Tait-Bryan angles"
+        - ``'Space'``: three successive rotations about the parent
+            frames' unit vectors
+        - ``'Quaternion'``: rotations defined by four parameters which
+            result in a singularity free direction cosine matrix
+            
+    amounts: Iterable
+        Expressions defining the rotation angles or direction cosine
+        matrix. These must match the ``rot_type``. See examples below for
+        details. The input types are:
+
+        - ``'Axis'``: 2-tuple (expr/sym/func, Vector)
+        - ``'DCM'``: Matrix, shape(3, 3)
+        - ``'Body'``: 3-tuple of expressions, symbols, or functions
+        - ``'Space'``: 3-tuple of expressions, symbols, or functions
+        - ``'Quaternion'``: 4-tuple of expressions, symbols, or
+            functions
+            
+    rot_order: str or int, Optional
+        If applicable, the order of the successive of rotations. The string
+        ``'123'`` and integer ``123`` are equivalent, for example. Required
+        for ``'Body'`` and ``'Space'``.
+
+    Returns
+    -------
+    ReferenceFrame
+        A new ReferenceFrame object.
+
+    See Also
+    --------
+    :func:`sympy.physics.vector.ReferenceFrame.orientnew`
+
+    Example
+    -------
+    Define a standard Cartesian frame and rotate it around axis 'Z'
+    with 180 degrees:
+
+    >>> from neumann.linalg.utils import rotation_matrix
+    >>> R = rotation_matrix('Space', [0, 0, np.pi], 'XYZ')
+    """
+    source = SymPyFrame("S")
+    target = source.orientnew("T", rot_type, amounts, rot_order)
+    dcm = np.array(target.dcm(source).evalf()).astype(float)
+    return dcm
+
+
 def permutation_tensor(dim: int = 3) -> ndarray:
     """
     Returns the Levi-Civita pseudotensor for N dimensions.
 
     Parameters
     ----------
     N : int, Optional
@@ -85,27 +152,27 @@
     coincides with NumPy when all inputs are arrays and generalizes when they are not,
     but all inputs must be either all arrays or all tensors of some kind. The operation for
     tensors of order 1 and 2 have dedicated implementations, for higher order tensors
     it generalizes to tensor contraction along specified axes.
 
     Parameters
     ----------
-    a : TensorLike or ArrayLike
-        A tensor or an array.
-    b : TensorLike or ArrayLike
-        A tensor or an array.
-    out : ArrayLike, Optional
+    a: TensorLike or ArrayLike
+       A tensor or an array.
+    b: TensorLike or ArrayLike
+       A tensor or an array.
+    out: ArrayLike, Optional
         Output argument. This must have the exact kind that would be returned if it was
         not used. See `numpy.dot` for the details. Only if all inputs are ArrayLike.
         Default is None.
-    frame : FrameLike, Optinal
+    frame: FrameLike, Optinal
         The target frame of the output. Only if all inputs are TensorLike. If not specified,
         the returned tensor migh be returned in an arbitrary frame, depending on the inputs.
         Default is None.
-    axes : tuple or list, Optional
+    axes: tuple or list, Optional
         The indices along which contraction happens if any of the input tensors have a rank
         higher than 2. Default is None.
 
     Returns
     -------
     TensorLike or numpy.ndarray or scalar
         An array or a tensor, depending on the inputs.
@@ -197,23 +264,23 @@
     tensor. The behaviour coincides with NumPy when all inputs are arrays and generalizes
     when they are not, but all inputs must be either all arrays or all tensors of some kind.
 
     Parameters
     ----------
     *args : Tuple, Optional
         Positional arguments forwarded to NumPy, if all input objects are arrays.
-    a : TensorLike or ArrayLike
+    a: TensorLike or ArrayLike
         A tensor or an array.
-    b : TensorLike or ArrayLike
+    b: TensorLike or ArrayLike
         A tensor or an array.
-    frame : FrameLike, Optional
+    frame: FrameLike, Optional
         The target frame of the output. Only if all inputs are TensorLike. If not specified,
         the returned tensor migh be returned in an arbitrary frame, depending on the inputs.
         Default is None.
-    **kwargs : dict, Optional
+    **kwargs: dict, Optional
         Keyword arguments forwarded to `numpy.cross`. As of NumPy version '1.22.4', there
         are no keyword arguments for `numpy.cross`, this is to assure compliance with
         all future versions of numpy.
 
     Returns
     -------
     numpy.ndarray or TensorLike
@@ -276,26 +343,26 @@
     return np.cross(*inputs, *args, **kwargs)
 
 
 def show_vector(dcm: ndarray, arr: ndarray) -> ndarray:
     """
     Returns the coordinates of a single or multiple vectors in a frame specified
     by one or several DCM matrices. The function can handle the following scenarios:
-    
+
         - a single (1d) vector and a single (2d) dcm matrix (trivial case)
         - a stack of vectors (2d) and a single (2d) dcm matrix
         - a stack of fectors (2d) and dcm matrices for each vector in the stack (3d)
-        
+
     .. versionadded:: 1.0.5
 
     Parameters
     ----------
-    dcm : numpy.ndarray
+    dcm: numpy.ndarray
         The dcm matrix of the transformation as a 2d or 3d float array.
-    arr : numpy.ndarray
+    arr: numpy.ndarray
         1d or 2d float array of coordinates of a single vector. If it is 2d, then
         it is assumed that the coordinates of the i-th vector are accessible as
         `arr[i]`.
 
     Returns
     -------
     numpy.ndarray
@@ -312,25 +379,41 @@
             "Mismatch in shapes!"
             f"Input one has shape {dcm.shape} and input two has shape {arr.shape}."
             "See the docs for the correct input shapes."
         )
         raise LinalgOperationInputError(msg)
 
 
+def show_frame(dcm: ndarray, arr: ndarray) -> ndarray:
+    if len(arr.shape) == 2 and len(dcm.shape) == 2:
+        return _show_frame(dcm, arr)  # dcm @ arr
+    elif len(arr.shape) == 3 and len(dcm.shape) == 2:
+        return _show_frames(dcm, arr)  # dcm @ arr
+    elif len(arr.shape) == 3 and len(dcm.shape) == 3:
+        return _show_frames_multi(dcm, arr)  # dcm @ arr
+    else:
+        msg = (
+            "Mismatch in shapes!"
+            f"Input one has shape {dcm.shape} and input two has shape {arr.shape}."
+            "See the docs for the correct input shapes."
+        )
+        raise LinalgOperationInputError(msg)
+
+
 @njit(nogil=True, cache=__cache)
 def _show_vector(dcm: ndarray, arr: ndarray) -> ndarray:
     """
     Returns the coordinates of a single vector in a frame specified
     by a DCM matrix.
 
     Parameters
     ----------
-    dcm : numpy.ndarray
+    dcm: numpy.ndarray
         The dcm matrix of the transformation as a 2d float array.
-    arr : numpy.ndarray
+    arr: numpy.ndarray
         1d float array of coordinates of a single vector.
 
     Returns
     -------
     numpy.ndarray
         The new coordinates of the vector with the same shape as `arr`.
     """
@@ -341,17 +424,17 @@
 def _show_vectors(dcm: ndarray, arr: ndarray) -> ndarray:
     """
     Returns the coordinates of multiple vectors in a frame specified
     by a DCM matrix.
 
     Parameters
     ----------
-    dcm : numpy.ndarray
+    dcm: numpy.ndarray
         The dcm matrix of the transformation as a 2d float array.
-    arr : numpy.ndarray
+    arr: numpy.ndarray
         2d float array of coordinates of multiple vectors.
 
     Returns
     -------
     numpy.ndarray
         The new coordinates of the vectors with the same shape as `arr`.
     """
@@ -364,31 +447,104 @@
 @njit(nogil=True, parallel=True, cache=__cache)
 def _show_vectors_multi(dcm: ndarray, arr: ndarray) -> ndarray:
     """
     Returns the coordinates of multiple vectors and multiple DCM matrices.
 
     Parameters
     ----------
-    dcm : numpy.ndarray
+    dcm: numpy.ndarray
         The dcm matrix of the transformation as a 3d float array.
-    arr : numpy.ndarray
+    arr: numpy.ndarray
         2d float array of coordinates of multiple vectors.
 
     Returns
     -------
     numpy.ndarray
         The new coordinates of the vectors with the same shape as `arr`.
     """
     res = np.zeros_like(arr)
     for i in prange(arr.shape[0]):
         res[i] = dcm[i] @ arr[i, :]
     return res
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
+def _show_frame(dcm: ndarray, arr: ndarray) -> ndarray:
+    """
+    Returns the coordinates of a single frame in a target frame specified
+    by a DCM matrix.
+
+    Parameters
+    ----------
+    dcm: numpy.ndarray
+        The dcm matrix of the transformation as a 2d float array.
+    arr: numpy.ndarray
+        2d float array of coordinates of a single frame.
+
+    Returns
+    -------
+    numpy.ndarray
+        The new coordinates of the frame with the same shape as `arr`.
+    """
+    res = np.zeros_like(arr)
+    for i in prange(arr.shape[-1]): 
+        res[i, :] = dcm @ arr[i, :] 
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def _show_frames(dcm: ndarray, arr: ndarray) -> ndarray:
+    """
+    Returns the coordinates of multiple frames in a target frame specified
+    by a DCM matrix.
+
+    Parameters
+    ----------
+    dcm: numpy.ndarray
+        The dcm matrix of the transformation as a 2d float array.
+    arr: numpy.ndarray
+        3d float array of coordinates of multiple frames.
+
+    Returns
+    -------
+    numpy.ndarray
+        The new coordinates of the frames with the same shape as `arr`.
+    """
+    res = np.zeros_like(arr)
+    for i in prange(arr.shape[0]):
+        for j in prange(arr.shape[-1]): 
+            res[i, j, :] = dcm @ arr[i, j, :]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def _show_frames_multi(dcm: ndarray, arr: ndarray) -> ndarray:
+    """
+    Returns the coordinates of multiple frames and multiple DCM matrices.
+
+    Parameters
+    ----------
+    dcm: numpy.ndarray
+        The dcm matrix of the transformation as a 3d float array.
+    arr: numpy.ndarray
+        3d float array of coordinates of multiple frames.
+
+    Returns
+    -------
+    numpy.ndarray
+        The new coordinates of the frames with the same shape as `arr`.
+    """
+    res = np.zeros_like(arr)
+    for i in prange(arr.shape[0]):
+        for j in prange(arr.shape[-1]): 
+            res[i, j, :] = dcm[i] @ arr[i, j, :]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
 def _transpose_multi(dcm: ndarray) -> ndarray:
     N = dcm.shape[0]
     res = np.zeros_like(dcm)
     for i in prange(N):
         res[i] = dcm[i].T
     return res
 
@@ -404,15 +560,15 @@
 
 def is_rectangular_frame(axes: ndarray) -> bool:
     """
     Returns True if a frame is Cartesian.
 
     Parameters
     ----------
-    axes : numpy.ndarray
+    axes: numpy.ndarray
         A matrix where the i-th row is the i-th basis vector.
     """
     assert len(axes.shape) == 2, "Input is not a matrix!"
     assert axes.shape[0] == axes.shape[1], "Input is not a square matrix!"
     agram = np.abs(axes @ axes.T)
     return np.isclose(np.trace(agram), np.sum(agram))
 
@@ -420,39 +576,39 @@
 def is_normal_frame(axes: ndarray) -> bool:
     """
     Returns True if a frame is normal, meaning, that it's base vectors
     are all of unit length.
 
     Parameters
     ----------
-    axes : numpy.ndarray
+    axes: numpy.ndarray
         A matrix where the i-th row is the i-th basis vector.
     """
     return np.allclose(np.linalg.norm(axes, axis=1), 1.0)
 
 
 def is_orthonormal_frame(axes: ndarray) -> bool:
     """
     Returns True if a frame is orthonormal.
 
     Parameters
     ----------
-    axes : numpy.ndarray
+    axes: numpy.ndarray
         A matrix where the i-th row is the i-th basis vector.
     """
     return is_rectangular_frame(axes) and is_normal_frame(axes)
 
 
 def is_independent_frame(axes: ndarray, tol: float = 0) -> bool:
     """
     Returns True if a the base vectors of a frame are linearly independent.
 
     Parameters
     ----------
-    axes : numpy.ndarray
+    axes: numpy.ndarray
         A matrix where the i-th row is the i-th basis vector.
     """
     return np.linalg.det(Gram(axes)) > tol
 
 
 def is_hermitian(arr: ndarray) -> bool:
     """
@@ -465,39 +621,39 @@
 
 def normalize_frame(axes: ndarray) -> ndarray:
     """
     Returns the frame with normalized base vectors.
 
     Parameters
     ----------
-    axes : numpy.ndarray
+    axes: numpy.ndarray
         A matrix where the i-th row is the i-th basis vector.
     """
     return np.array([normalize(a) for a in axes], dtype=axes.dtype)
 
 
 def Gram(axes: ndarray) -> ndarray:
     """
     Returns the Gram matrix of a frame.
 
     Parameters
     ----------
-    axes : numpy.ndarray
+    axes: numpy.ndarray
         A matrix where the i-th row is the i-th basis vector.
     """
     return axes @ axes.T
 
 
 def dual_frame(axes: ndarray) -> ndarray:
     """
     Returns the dual frame of the input.
 
     Parameters
     ----------
-    axes : numpy.ndarray
+    axes: numpy.ndarray
         A matrix where the i-th row is the i-th basis vector.
     """
     return transpose_axes(np.linalg.inv(axes))
 
 
 def is_pos_def(arr) -> bool:
     """
@@ -798,8 +954,8 @@
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def _transform_tensors2_multi(arr: ndarray, Q: ndarray):
     nE = arr.shape[0]
     res = np.zeros_like(arr)
     for iE in prange(nE):
         res[iE, :, :] = Q[iE] @ arr[iE] @ Q[iE].T
-    return res
+    return res
```

### Comparing `neumann-1.0.5/src/neumann/linalg/vector.py` & `neumann-1.0.6/src/neumann/linalg/vector.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
     instance.
 
     All parameters are identical to those of ``numpy.ndarray``, except that
     this class allows to specify an embedding frame.
 
     Parameters
     ----------
-    args : tuple, Optional
+    args: tuple, Optional
         Positional arguments forwarded to `numpy.ndarray`.
-    frame : numpy.ndarray, Optional
+    frame: numpy.ndarray, Optional
         The reference frame the vector is represented by its coordinates.
-    kwargs : dict, Optional
+    kwargs: dict, Optional
         Keyword arguments forwarded to `numpy.ndarray`.
 
     Examples
     --------
     Import the necessary classes:
 
     >>> import numpy as np
@@ -113,17 +113,17 @@
         Returns the components in a target frame. If the target is
         `None`, the components are returned in the ambient frame.
 
         The transformation can also be specified with a proper DCM matrix.
 
         Parameters
         ----------
-        target : numpy.ndarray, Optional
+        target: numpy.ndarray, Optional
             Target frame.
-        dcm : numpy.ndarray, Optional
+        dcm: numpy.ndarray, Optional
             The DCM matrix of the transformation.
 
         Returns
         -------
         numpy.ndarray
             The components of the vector in a specified frame, or
             the ambient frame, depending on the arguments.
@@ -137,15 +137,15 @@
     def orient(self, *args, dcm: ndarray = None, **kwargs) -> "Vector":
         """
         Orients the vector inplace. If the transformation is not specified by 'dcm',
         all arguments are forwarded to `orient_new`.
 
         Parameters
         ----------
-        dcm : numpy.ndarray, Optional
+        dcm: numpy.ndarray, Optional
             The DCM matrix of the transformation.
 
         Returns
         -------
         Vector
             The same vector the function is called upon.
```

### Comparing `neumann-1.0.5/src/neumann/logical.py` & `neumann-1.0.6/src/neumann/logical.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/numint.py` & `neumann-1.0.6/src/neumann/numint.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/optimize/ga.py` & `neumann-1.0.6/src/neumann/optimize/ga.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/optimize/lp.py` & `neumann-1.0.6/src/neumann/optimize/lp.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/topology/graph.py` & `neumann-1.0.6/src/neumann/topology/graph.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann/utils.py` & `neumann-1.0.6/src/neumann/utils.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/src/neumann.egg-info/PKG-INFO` & `neumann-1.0.6/src/neumann.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: neumann
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python Library for Applied Mathematics in Physical Sciences.
 Home-page: https://github.com/dewloosh/Neumann
-Download-URL: https://github.com/dewloosh/Neumann/archive/refs/tags/1.0.5.zip
+Download-URL: https://github.com/dewloosh/Neumann/archive/refs/tags/1.0.6.zip
 Author: Bence Balogh
 Author-email: dewloosh@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `neumann-1.0.5/src/neumann.egg-info/SOURCES.txt` & `neumann-1.0.6/src/neumann.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/tests/test_approx.py` & `neumann-1.0.6/tests/test_approx.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/tests/test_function.py` & `neumann-1.0.6/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/tests/test_ga.py` & `neumann-1.0.6/tests/test_ga.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/tests/test_graph.py` & `neumann-1.0.6/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/tests/test_linalg.py` & `neumann-1.0.6/tests/test_linalg.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         self._call_frame_methods(RectangularFrame(dim=3))
         self._call_frame_methods(CartesianFrame(dim=3))
 
         # create a random frame and call everything
         f = ReferenceFrame(dim=3)
         self.assertFailsProperly(TypeError, setattr, f, 'name', 5)
         self.assertFailsProperly(TypeError, setattr, f, 'axes', "a")
-        self.assertFailsProperly(RuntimeError, setattr, f, 'axes', np.eye(5))
+        self.assertFailsProperly(ValueError, setattr, f, 'axes', np.eye(5))
         
         # copy and deepcopy
         f = ReferenceFrame(dim=3) 
         f.copy()
         f.deepcopy() 
         
         # misc
```

### Comparing `neumann-1.0.5/tests/test_logical.py` & `neumann-1.0.6/tests/test_logical.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/tests/test_lpp.py` & `neumann-1.0.6/tests/test_lpp.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/tests/test_numint.py` & `neumann-1.0.6/tests/test_numint.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.5/tests/test_utils.py` & `neumann-1.0.6/tests/test_utils.py`

 * *Files identical despite different names*

