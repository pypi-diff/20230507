# Comparing `tmp/phylo-treetime-0.9.5.tar.gz` & `tmp/phylo-treetime-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phylo-treetime-0.9.5.tar", last modified: Wed Feb 15 19:54:53 2023, max compression
+gzip compressed data, was "phylo-treetime-0.9.6.tar", last modified: Sun Apr 16 13:17:06 2023, max compression
```

## Comparing `phylo-treetime-0.9.5.tar` & `phylo-treetime-0.9.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-02-15 19:54:53.317253 phylo-treetime-0.9.5/
--rw-rw-r--   0 richard   (1001) richard   (1001)     1100 2021-04-05 13:42:08.000000 phylo-treetime-0.9.5/LICENSE
--rw-rw-r--   0 richard   (1001) richard   (1001)    14936 2023-02-15 19:54:53.317253 phylo-treetime-0.9.5/PKG-INFO
--rw-rw-r--   0 richard   (1001) richard   (1001)    12519 2022-09-07 08:44:06.000000 phylo-treetime-0.9.5/README.md
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-02-15 19:54:53.317253 phylo-treetime-0.9.5/phylo_treetime.egg-info/
--rw-rw-r--   0 richard   (1001) richard   (1001)    14936 2023-02-15 19:54:53.000000 phylo-treetime-0.9.5/phylo_treetime.egg-info/PKG-INFO
--rw-rw-r--   0 richard   (1001) richard   (1001)      838 2023-02-15 19:54:53.000000 phylo-treetime-0.9.5/phylo_treetime.egg-info/SOURCES.txt
--rw-rw-r--   0 richard   (1001) richard   (1001)        1 2023-02-15 19:54:53.000000 phylo-treetime-0.9.5/phylo_treetime.egg-info/dependency_links.txt
--rw-rw-r--   0 richard   (1001) richard   (1001)       53 2023-02-15 19:54:53.000000 phylo-treetime-0.9.5/phylo_treetime.egg-info/entry_points.txt
--rw-rw-r--   0 richard   (1001) richard   (1001)      166 2023-02-15 19:54:53.000000 phylo-treetime-0.9.5/phylo_treetime.egg-info/requires.txt
--rw-rw-r--   0 richard   (1001) richard   (1001)        9 2023-02-15 19:54:53.000000 phylo-treetime-0.9.5/phylo_treetime.egg-info/top_level.txt
--rw-rw-r--   0 richard   (1001) richard   (1001)       38 2023-02-15 19:54:53.317253 phylo-treetime-0.9.5/setup.cfg
--rw-rw-r--   0 richard   (1001) richard   (1001)     1857 2022-08-04 09:25:04.000000 phylo-treetime-0.9.5/setup.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-02-15 19:54:53.317253 phylo-treetime-0.9.5/test/
--rw-rw-r--   0 richard   (1001) richard   (1001)     4808 2022-03-31 09:14:02.000000 phylo-treetime-0.9.5/test/test_calc_nbranches.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    12852 2023-01-09 17:00:14.000000 phylo-treetime-0.9.5/test/test_treetime.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-02-15 19:54:53.317253 phylo-treetime-0.9.5/treetime/
--rw-rw-r--   0 richard   (1001) richard   (1001)     1737 2023-02-15 19:54:22.000000 phylo-treetime-0.9.5/treetime/__init__.py
--rw-rw-r--   0 richard   (1001) richard   (1001)      724 2022-08-04 09:25:04.000000 phylo-treetime-0.9.5/treetime/__main__.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     4591 2022-02-10 12:32:27.000000 phylo-treetime-0.9.5/treetime/aa_models.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     5674 2022-09-07 08:44:02.000000 phylo-treetime-0.9.5/treetime/arg.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    20617 2023-01-09 17:00:14.000000 phylo-treetime-0.9.5/treetime/argument_parser.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     6196 2022-06-21 10:27:24.000000 phylo-treetime-0.9.5/treetime/branch_len_interpolator.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    55142 2023-01-09 17:00:09.000000 phylo-treetime-0.9.5/treetime/clock_tree.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     1035 2022-03-31 09:14:02.000000 phylo-treetime-0.9.5/treetime/config.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    16279 2022-09-21 12:02:41.000000 phylo-treetime-0.9.5/treetime/distribution.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    39199 2023-01-09 17:00:14.000000 phylo-treetime-0.9.5/treetime/gtr.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    15995 2022-03-06 14:08:22.000000 phylo-treetime-0.9.5/treetime/gtr_site_specific.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    18540 2023-01-09 17:00:09.000000 phylo-treetime-0.9.5/treetime/merger_models.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    14693 2023-01-06 17:07:02.000000 phylo-treetime-0.9.5/treetime/node_interpolator.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     7263 2022-04-06 18:01:25.000000 phylo-treetime-0.9.5/treetime/nuc_models.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    14020 2022-02-10 12:32:27.000000 phylo-treetime-0.9.5/treetime/seq_utils.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     3178 2022-05-19 08:52:34.000000 phylo-treetime-0.9.5/treetime/seqgen.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    22576 2022-08-04 12:40:41.000000 phylo-treetime-0.9.5/treetime/sequence_data.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    73219 2023-01-09 17:00:09.000000 phylo-treetime-0.9.5/treetime/treeanc.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    22803 2023-01-09 17:00:09.000000 phylo-treetime-0.9.5/treetime/treeregression.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    46935 2023-01-09 17:00:09.000000 phylo-treetime-0.9.5/treetime/treetime.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    17909 2022-09-07 08:44:06.000000 phylo-treetime-0.9.5/treetime/utils.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    24609 2023-01-06 17:07:02.000000 phylo-treetime-0.9.5/treetime/vcf_utils.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    49123 2023-02-15 19:27:03.000000 phylo-treetime-0.9.5/treetime/wrappers.py
+drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-04-16 13:17:06.817122 phylo-treetime-0.9.6/
+-rw-rw-r--   0 richard   (1001) richard   (1001)     1100 2021-04-05 13:42:08.000000 phylo-treetime-0.9.6/LICENSE
+-rw-rw-r--   0 richard   (1001) richard   (1001)    14936 2023-04-16 13:17:06.817122 phylo-treetime-0.9.6/PKG-INFO
+-rw-rw-r--   0 richard   (1001) richard   (1001)    12519 2022-09-07 08:44:06.000000 phylo-treetime-0.9.6/README.md
+drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-04-16 13:17:06.813122 phylo-treetime-0.9.6/phylo_treetime.egg-info/
+-rw-rw-r--   0 richard   (1001) richard   (1001)    14936 2023-04-16 13:17:06.000000 phylo-treetime-0.9.6/phylo_treetime.egg-info/PKG-INFO
+-rw-rw-r--   0 richard   (1001) richard   (1001)      838 2023-04-16 13:17:06.000000 phylo-treetime-0.9.6/phylo_treetime.egg-info/SOURCES.txt
+-rw-rw-r--   0 richard   (1001) richard   (1001)        1 2023-04-16 13:17:06.000000 phylo-treetime-0.9.6/phylo_treetime.egg-info/dependency_links.txt
+-rw-rw-r--   0 richard   (1001) richard   (1001)       53 2023-04-16 13:17:06.000000 phylo-treetime-0.9.6/phylo_treetime.egg-info/entry_points.txt
+-rw-rw-r--   0 richard   (1001) richard   (1001)      166 2023-04-16 13:17:06.000000 phylo-treetime-0.9.6/phylo_treetime.egg-info/requires.txt
+-rw-rw-r--   0 richard   (1001) richard   (1001)        9 2023-04-16 13:17:06.000000 phylo-treetime-0.9.6/phylo_treetime.egg-info/top_level.txt
+-rw-rw-r--   0 richard   (1001) richard   (1001)       38 2023-04-16 13:17:06.817122 phylo-treetime-0.9.6/setup.cfg
+-rw-rw-r--   0 richard   (1001) richard   (1001)     1847 2023-04-16 11:00:18.000000 phylo-treetime-0.9.6/setup.py
+drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-04-16 13:17:06.813122 phylo-treetime-0.9.6/test/
+-rw-rw-r--   0 richard   (1001) richard   (1001)     4808 2022-03-31 09:14:02.000000 phylo-treetime-0.9.6/test/test_calc_nbranches.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)    12852 2023-01-09 17:00:14.000000 phylo-treetime-0.9.6/test/test_treetime.py
+drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2023-04-16 13:17:06.817122 phylo-treetime-0.9.6/treetime/
+-rw-rw-r--   0 richard   (1001) richard   (1001)     1950 2023-04-16 11:00:18.000000 phylo-treetime-0.9.6/treetime/__init__.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)      724 2022-08-04 09:25:04.000000 phylo-treetime-0.9.6/treetime/__main__.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)     4591 2022-02-10 12:32:27.000000 phylo-treetime-0.9.6/treetime/aa_models.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)     5674 2022-09-07 08:44:02.000000 phylo-treetime-0.9.6/treetime/arg.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)    20784 2023-04-16 12:07:12.000000 phylo-treetime-0.9.6/treetime/argument_parser.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)     6196 2022-06-21 10:27:24.000000 phylo-treetime-0.9.6/treetime/branch_len_interpolator.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)    55393 2023-04-16 11:00:18.000000 phylo-treetime-0.9.6/treetime/clock_tree.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)     1035 2022-03-31 09:14:02.000000 phylo-treetime-0.9.6/treetime/config.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)    16021 2023-04-16 11:00:18.000000 phylo-treetime-0.9.6/treetime/distribution.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)    39199 2023-01-09 17:00:14.000000 phylo-treetime-0.9.6/treetime/gtr.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)    15995 2022-03-06 14:08:22.000000 phylo-treetime-0.9.6/treetime/gtr_site_specific.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)    18545 2023-04-16 12:07:12.000000 phylo-treetime-0.9.6/treetime/merger_models.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)    15037 2023-04-16 11:00:18.000000 phylo-treetime-0.9.6/treetime/node_interpolator.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)     7263 2022-04-06 18:01:25.000000 phylo-treetime-0.9.6/treetime/nuc_models.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)    14020 2022-02-10 12:32:27.000000 phylo-treetime-0.9.6/treetime/seq_utils.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)     3178 2022-05-19 08:52:34.000000 phylo-treetime-0.9.6/treetime/seqgen.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)    22576 2022-08-04 12:40:41.000000 phylo-treetime-0.9.6/treetime/sequence_data.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)    73195 2023-04-16 11:00:18.000000 phylo-treetime-0.9.6/treetime/treeanc.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)    22803 2023-01-09 17:00:09.000000 phylo-treetime-0.9.6/treetime/treeregression.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)    53820 2023-04-16 12:07:12.000000 phylo-treetime-0.9.6/treetime/treetime.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)    17909 2022-09-07 08:44:06.000000 phylo-treetime-0.9.6/treetime/utils.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)    24609 2023-01-06 17:07:02.000000 phylo-treetime-0.9.6/treetime/vcf_utils.py
+-rw-rw-r--   0 richard   (1001) richard   (1001)    49317 2023-04-16 12:07:12.000000 phylo-treetime-0.9.6/treetime/wrappers.py
```

### Comparing `phylo-treetime-0.9.5/LICENSE` & `phylo-treetime-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/PKG-INFO` & `phylo-treetime-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phylo-treetime
-Version: 0.9.5
+Version: 0.9.6
 Summary: Maximum-likelihood phylodynamic inference
 Home-page: https://github.com/neherlab/treetime
 Author: Pavel Sagulenko, Emma Hodcroft, and Richard Neher
 Author-email: richard.neher@unibas.ch
 License: MIT
 Description: [![CI](https://github.com/neherlab/treetime/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/neherlab/treetime/actions/workflows/ci.yml)
         [![anaconda](https://anaconda.org/bioconda/treetime/badges/installer/conda.svg)](https://anaconda.org/bioconda/treetime)
```

### Comparing `phylo-treetime-0.9.5/README.md` & `phylo-treetime-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/phylo_treetime.egg-info/PKG-INFO` & `phylo-treetime-0.9.6/phylo_treetime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phylo-treetime
-Version: 0.9.5
+Version: 0.9.6
 Summary: Maximum-likelihood phylodynamic inference
 Home-page: https://github.com/neherlab/treetime
 Author: Pavel Sagulenko, Emma Hodcroft, and Richard Neher
 Author-email: richard.neher@unibas.ch
 License: MIT
 Description: [![CI](https://github.com/neherlab/treetime/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/neherlab/treetime/actions/workflows/ci.yml)
         [![anaconda](https://anaconda.org/bioconda/treetime/badges/installer/conda.svg)](https://anaconda.org/bioconda/treetime)
```

### Comparing `phylo-treetime-0.9.5/phylo_treetime.egg-info/SOURCES.txt` & `phylo-treetime-0.9.6/phylo_treetime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/setup.py` & `phylo-treetime-0.9.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 from setuptools import setup
 
 def get_version():
     v = "0.0.0"
     with open('treetime/__init__.py') as ifile:
         for line in ifile:
             if line[:7]=='version':
```

### Comparing `phylo-treetime-0.9.5/test/test_calc_nbranches.py` & `phylo-treetime-0.9.6/test/test_calc_nbranches.py`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/test/test_treetime.py` & `phylo-treetime-0.9.6/test/test_treetime.py`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/treetime/__main__.py` & `phylo-treetime-0.9.6/treetime/__main__.py`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/treetime/aa_models.py` & `phylo-treetime-0.9.6/treetime/aa_models.py`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/treetime/arg.py` & `phylo-treetime-0.9.6/treetime/arg.py`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/treetime/argument_parser.py` & `phylo-treetime-0.9.6/treetime/argument_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,14 +176,16 @@
     parser.add_argument('--time-marginal', default='false', choices = ['false', 'true', 'assign', 'always', 'only-final', 'never'],
                         help="For 'false' or 'never', TreeTime uses the jointly most likely values for the divergence times. "
                              "For 'true' and 'always', it uses the marginal inference mode at every round of optimization, for 'only-final' "
                              "(or 'assign' for compatibility with previous versions) only uses the marginal "
                              "distribution in the final round.")
     parser.add_argument('--keep-polytomies', default=False, action='store_true',
                         help="Don't resolve polytomies using temporal information.")
+    parser.add_argument('--stochastic-resolve', default=False, action='store_true',
+                        help="Resolve polytomies using a random coalescent tree.")
     # parser.add_argument('--keep-node-order', default=False, action='store_true',
     #                     help="Don't ladderize the tree.")
     parser.add_argument('--relax',nargs=2, type=float,
                         help='use an autocorrelated molecular clock. Strength of the gaussian priors on'
                              ' branch specific rate deviation and the coupling of parent and offspring'
                              ' rates can be specified e.g. as --relax 1.0 0.5. Values around 1.0 correspond'
                              ' to weak priors, larger values constrain rate deviations more strongly.'
```

### Comparing `phylo-treetime-0.9.5/treetime/branch_len_interpolator.py` & `phylo-treetime-0.9.6/treetime/branch_len_interpolator.py`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/treetime/clock_tree.py` & `phylo-treetime-0.9.6/treetime/clock_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -699,14 +699,17 @@
                         complementary_msgs = [Distribution.divide(parent.product_of_child_messages, node.marginal_pos_Lx)]
                     # if parent itself got smth from the root node, include it
                     if parent.msg_from_parent is not None:
                         complementary_msgs.append(parent.msg_from_parent)
 
                     if hasattr(self, 'merger_model') and self.merger_model:
                         time_points = parent.marginal_pos_LH.x
+                        if len(time_points)<5:
+                            time_points = np.linspace(np.min([x.xmin for x in complementary_msgs]),
+                                                      np.max([x.xmax for x in complementary_msgs]), 10)
                         # As Lx do not include the node contribution this must be added on
                         complementary_msgs.append(self.merger_model.node_contribution(parent, time_points))
 
                         # Removed merger rate must be added back if no msgs from parent (equivalent to root node case)
                         if parent.msg_from_parent is None:
                             complementary_msgs.append(Distribution(time_points, self.merger_model.integral_merger_rate(time_points), is_log=True))
```

### Comparing `phylo-treetime-0.9.5/treetime/config.py` & `phylo-treetime-0.9.6/treetime/config.py`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/treetime/distribution.py` & `phylo-treetime-0.9.6/treetime/distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import numpy as np
+from . import TreeTimeUnknownError
 from scipy.interpolate import interp1d
 try:
     from collections.abc import Iterable
 except ImportError:
     from collections import Iterable
-from copy import deepcopy as make_copy
-from scipy.ndimage import binary_dilation
-from .config import BIG_NUMBER, MIN_LOG, MIN_INTEGRATION_PEAK, TINY_NUMBER, SUPERTINY_NUMBER
+from .config import BIG_NUMBER, MIN_INTEGRATION_PEAK, TINY_NUMBER
 from .utils import clip
 
 class Distribution(object):
     """
     Class to implement the probability distribution. This class wraps the scipy
     linear interpolation object, and implements some additional operations,
     needed to manipulate distributions for tree nodes positions, branch lengths,
@@ -110,30 +109,26 @@
                 x_vals = np.concatenate((x_vals[:lower_cut_off],
                                          x_vals[lower_cut_off:upper_cut_off].reshape((-1,n_dists)).mean(axis=1),
                                          x_vals[upper_cut_off:]))
             y_vals = np.sum([k.__call__(x_vals) for k in dists], axis=0)
             try:
                 peak = y_vals.min()
             except:
-                print("WARNING: Unexpected behavior detected in multiply function,"
-                        "if you see this error \n please let us know by filling an issue at: https://github.com/neherlab/treetime/issues")
-                x_vals = [0,1]
-                y_vals = [BIG_NUMBER,BIG_NUMBER]
-                res = Distribution(x_vals, y_vals, is_log=True,
-                                    min_width=min_width, kind='linear')
-                return res
+                TreeTimeUnknownError("Error: Unexpected behavior detected in multiply function"
+                        " when determining peak of function with y-values '"+ str(y_vals) + "'.\n\n"
+                        "If you see this error please let us know by filling an issue at: \n"
+                        "https://github.com/neherlab/treetime/issues")
+
             ind = (y_vals-peak)<BIG_NUMBER/1000
             n_points = ind.sum()
             if n_points == 0:
-                print("WARNING: Unexpected behavior detected in multipy function,"
-                        "if you see this error \n please let us know by filling an issue at: https://github.com/neherlab/treetime/issues")
-                x_vals = [0,1]
-                y_vals = [BIG_NUMBER,BIG_NUMBER]
-                res = Distribution(x_vals, y_vals, is_log=True,
-                                   min_width=min_width, kind='linear')
+                TreeTimeUnknownError("Error: Unexpected behavior detected in multiply function. "
+                                     "No valid points left after reducing to plausible region.\n\n"
+                        "If you see this error please let us know by filling an issue at:\n"
+                        "https://github.com/neherlab/treetime/issues")
             elif n_points == 1:
                 res = Distribution.delta_function(x_vals[0])
             else:
                 res = Distribution(x_vals[ind], y_vals[ind], is_log=True,
                                    min_width=min_width, kind='linear', assume_sorted=True)
 
         return res
@@ -155,15 +150,15 @@
         x_vals = x_vals[(x_vals> new_xmin-TINY_NUMBER)&(x_vals< new_xmax+TINY_NUMBER)]
         y_vals = numerator.__call__(x_vals) - denominator.__call__(x_vals)
 
         peak = y_vals.min()
         ind = (y_vals-peak)<BIG_NUMBER/1000
         n_points = ind.sum()
         if n_points == 0:
-            print("WARNING: Unexpected behavior detected in multipy function,"
+            print("WARNING: Unexpected behavior detected in multiply function,"
                     "if you see this error \n please let us know by filling an issue at: https://github.com/neherlab/treetime/issues")
             x_vals = [0,1]
             y_vals = [BIG_NUMBER,BIG_NUMBER]
             res = Distribution(x_vals, y_vals, is_log=True,
                                 min_width=min_width, kind='linear')
         elif n_points == 1:
             res = Distribution.delta_function(x_vals[0])
@@ -267,15 +262,15 @@
             return [self._peak_pos]
         else:
             return self._func.x
 
     @property
     def y(self):
         if self.is_delta:
-            print("THIS SHOULDN'T BE CALLED ON A DELTA FUNCTION")
+            print("Warning: evaluating log probability of a delta distribution.")
             return [self.weight]
         else:
             return self._peak_val + self._func.y
 
     @property
     def xmin(self):
         return self._xmin
@@ -309,15 +304,14 @@
         return Distribution.multiply((self, other))
 
     def calc_effective_support(self, cutoff=1e-15):
         """
         Assess the interval on which the value of self is higher than cutoff
         relative to its peak
         """
-        from scipy.optimize import brentq
         log_cutoff = -np.log(cutoff)
         vals = log_cutoff - self.__call__(self.x) + self.peak_val
         above = vals > 0
         above_idx = np.where(above)[0]
         if len(above_idx)==0:
             return (self.xmin, self.xmax)
 
@@ -430,14 +424,15 @@
                     + np.sum((dx[:-1]+dx[1:])*y[2:-1:2]) + dx[-1]*y[-1]))
 
         return np.sum(res)
 
 
     def fft(self, T, n=None, inverse_time=True):
         if self.is_delta:
+            raise
             import ipdb; ipdb.set_trace()
         from numpy.fft import rfft
         if n is None:
             n=len(T)
         if inverse_time:
             return rfft(self.prob_relative(T), n=n)
         else:
```

### Comparing `phylo-treetime-0.9.5/treetime/gtr.py` & `phylo-treetime-0.9.6/treetime/gtr.py`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/treetime/gtr_site_specific.py` & `phylo-treetime-0.9.6/treetime/gtr_site_specific.py`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/treetime/merger_models.py` & `phylo-treetime-0.9.6/treetime/merger_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,7 +384,12 @@
 
         skyline = interp1d(self.date2dist.to_numdate(self.Tc.x[1:-1]), gen/self.date2dist.clock_rate*self.Tc.y[1:-1])
         if confidence and hasattr(self, 'confidence'):
             conf = [skyline.y*np.exp(-confidence*self.confidence), skyline.y*np.exp(confidence*self.confidence)]
             return skyline, conf
         else:
             return skyline, None
+
+
+
+
+
```

### Comparing `phylo-treetime-0.9.5/treetime/node_interpolator.py` & `phylo-treetime-0.9.6/treetime/node_interpolator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 from . import config as ttconf
+from . import TreeTimeUnknownError
 from .distribution import Distribution
 from .utils import clip
 from .config import FFT_FWHM_GRID_SIZE
 
 def _convolution_integrand(t_val, f, g,
                            inverse_time=None, return_log=False):
     '''
@@ -162,18 +163,18 @@
     def convolve_fft(cls, node_interp, branch_interp, fft_grid_size=FFT_FWHM_GRID_SIZE, inverse_time=True):
 
         dt = max(branch_interp.one_mutation*0.005, min(node_interp.fwhm, branch_interp.fwhm)/fft_grid_size)
         ratio = node_interp.fwhm/branch_interp.fwhm
         if ratio < 1/fft_grid_size and 4*dt > node_interp.fwhm:
             ## node distribution is much narrower than the branch distribution, proceed as if node distribution is
             ## a delta distribution
-            log_scale_node_interp = node_interp.integrate(return_log=True, a=node_interp.xmin,b=node_interp.xmax,n=max(100, len(node_interp.x))) #probability of node distribution 
+            log_scale_node_interp = node_interp.integrate(return_log=True, a=node_interp.xmin,b=node_interp.xmax,n=max(100, len(node_interp.x))) #probability of node distribution
             if inverse_time:
                 x = branch_interp.x + node_interp._peak_pos
-                dist = Distribution(x, branch_interp(x - node_interp._peak_pos) - log_scale_node_interp, min_width=max(node_interp.min_width, branch_interp.min_width), is_log=True)  
+                dist = Distribution(x, branch_interp(x - node_interp._peak_pos) - log_scale_node_interp, min_width=max(node_interp.min_width, branch_interp.min_width), is_log=True)
             else:
                 x = - branch_interp.x + node_interp._peak_pos
                 dist = Distribution(x, branch_interp(branch_interp.x) - log_scale_node_interp, min_width=max(node_interp.min_width, branch_interp.min_width), is_log=True)
             return dist
         elif ratio > fft_grid_size and 4*dt > branch_interp.fwhm:
             raise ValueError("ERROR: Unexpected behavior: branch distribution is much narrower than the node distribution.")
         else:
@@ -205,20 +206,24 @@
                 fft_res = fft_res[raw_len:]
                 Tres = Tn - Tb[0]
 
             # determine region in which we can trust the FFT convolution and avoid
             # inaccuracies due to machine precision. 1e-13 seems robust
             ind = fft_res>fft_res.max()*1e-13
             res = -np.log(fft_res[ind]) + branch_interp.peak_val + node_interp.peak_val - np.log(dt)
+
             Tres_cropped = Tres[ind]
 
             # extrapolate the tails exponentially: use margin last data points
             margin = np.minimum(3, Tres_cropped.shape[0]//3)
             if margin<1 or len(res)==0:
-                import ipdb; ipdb.set_trace()
+                TreeTimeUnknownError("Error: Unexpected behavior detected in FFT function. "
+                                     "No valid points left after reducing to plausible region.\n\n"
+                        "If you see this error please let us know by filling an issue at:\n"
+                        "https://github.com/neherlab/treetime/issues")
             else:
                 left_slope = (res[margin]-res[0])/(Tres_cropped[margin]-Tres_cropped[0])
                 right_slope = (res[-1]-res[-margin-1])/(Tres_cropped[-1]-Tres_cropped[-margin-1])
 
             # only extrapolate on the left when the slope is negative and we are not on the boundary
             if Tmin<Tres_cropped[0] and left_slope<0:
                 Tleft = np.linspace(Tmin, Tres_cropped[0],10)[:-1]
```

### Comparing `phylo-treetime-0.9.5/treetime/nuc_models.py` & `phylo-treetime-0.9.6/treetime/nuc_models.py`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/treetime/seq_utils.py` & `phylo-treetime-0.9.6/treetime/seq_utils.py`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/treetime/seqgen.py` & `phylo-treetime-0.9.6/treetime/seqgen.py`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/treetime/sequence_data.py` & `phylo-treetime-0.9.6/treetime/sequence_data.py`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/treetime/treeanc.py` & `phylo-treetime-0.9.6/treetime/treeanc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import time, sys
 import gc
 import numpy as np
 from Bio import Phylo
 from Bio.Phylo.BaseTree import Clade
-from Bio import AlignIO
 from . import config as ttconf
 from . import MissingDataError,UnknownMethodError
 from .seq_utils import seq2prof, prof2seq, normalize_profile, extend_profile
 from .gtr import GTR
 from .gtr_site_specific import GTR_site_specific
 from .sequence_data import SequenceData
```

### Comparing `phylo-treetime-0.9.5/treetime/treeregression.py` & `phylo-treetime-0.9.6/treetime/treeregression.py`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/treetime/treetime.py` & `phylo-treetime-0.9.6/treetime/treetime.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,20 +73,21 @@
                 sys.exit(2)
 
 
     def _run(self, root=None, infer_gtr=True, relaxed_clock=None, n_iqd = None,
             resolve_polytomies=True, max_iter=0, Tc=None, fixed_clock_rate=None,
             time_marginal='never', sequence_marginal=False, branch_length_mode='auto',
             vary_rate=False, use_covariation=False, tracelog_file=None,
-            method_anc = 'probabilistic', assign_gamma=None, **kwargs):
+            method_anc = 'probabilistic', assign_gamma=None, stochastic_resolve=False,
+            **kwargs):
 
         """
         Run TreeTime reconstruction. Based on the input parameters, it divides
         the analysis into semi-independent jobs and conquers them one-by-one,
-        gradually optimizing the tree given the temporal constarints and leaf
+        gradually optimizing the tree given the temporal constraints and leaf
         node sequences.
 
         Parameters
         ----------
         root : str
            Try to find better root position on a given tree. If string is passed,
            the root will be searched according to the specified method. If none,
@@ -107,14 +108,17 @@
            :code:`n_iqd` interquantile intervals from the molecular clock
            regression will be marked as 'BAD' and not used in the TreeTime
            analysis
 
         resolve_polytomies : bool
            If True, attempt to resolve multiple mergers
 
+        stochastic_resolve : bool (default False)
+           Resolve multiple mergers via a random coalescent tree (True) or via greedy optimization
+
         max_iter : int
            Maximum number of iterations to optimize the tree
 
         Tc : float, str
            If not None, use coalescent model to correct the branch lengths by
            introducing merger costs.
 
@@ -145,15 +149,15 @@
         vary_rate : bool or float, optional
             redo the time tree estimation for rates +/- one standard deviation.
             if a float is passed, it is interpreted as standard deviation,
             otherwise this standard deviation is estimated from the root-to-tip regression
 
         use_covariation : bool, optional
             default False, if False, rate estimates will be performed using simple
-            regression ignoring phylogenetic covaration between nodes. If vary_rate is True,
+            regression ignoring phylogenetic covariation between nodes. If vary_rate is True,
             use_covariation is true by default
 
         method_anc: str, optional
             Which method should be used to reconstruct ancestral sequences.
             Supported values are "parsimony", "fitch", "probabilistic" and "ml".
             Default is "probabilistic"
 
@@ -163,15 +167,15 @@
 
         **kwargs
            Keyword arguments needed by the downstream functions
 
 
         Returns
         -------
-        TreeTime error/succces code : str
+        TreeTime error/success code : str
             return value depending on success or error
 
 
         """
         # register the specified covaration mode
         self.use_covariation = use_covariation or (vary_rate and (not type(vary_rate)==float))
 
@@ -275,15 +279,15 @@
             if relaxed_clock:
                 self.relaxed_clock(**relaxed_clock)
                 need_new_time_tree = True
 
             n_resolved=0
             if resolve_polytomies:
                 # if polytomies are found, rerun the entire procedure
-                n_resolved = self.resolve_polytomies()
+                n_resolved = self.resolve_polytomies(stochastic_resolve=stochastic_resolve)
                 if n_resolved:
                     seq_kwargs['prune_short']=False
                     self.prepare_tree()
                     if self.branch_length_mode!='input': # otherwise reoptimize branch length while preserving branches without mutations
                         self.optimize_tree(max_iter=0, method_anc = method_anc,**seq_kwargs)
                     need_new_time_tree = True
             if assign_gamma and callable(assign_gamma):
@@ -563,44 +567,53 @@
         self.prepare_tree()
 
         self.get_clock_model(covariation=self.use_covariation, slope=slope)
 
         return new_root
 
 
-    def resolve_polytomies(self, merge_compressed=False, resolution_threshold=0.05):
+    def resolve_polytomies(self, merge_compressed=False, resolution_threshold=0.05, stochastic_resolve=False):
         """
         Resolve the polytomies on the tree.
 
         The function scans the tree, resolves polytomies if present,
         and re-optimizes the tree with new topology. Note that polytomies are only
         resolved if that would result in higher likelihood. Sometimes, stretching
         two or more branches that carry several mutations is less costly than
         an additional branch with zero mutations (long branches are not stiff,
         short branches are).
 
         Parameters
         ----------
          merge_compressed : bool
-            If True, keep compressed branches as polytomies. If False,
-            return a strictly binary tree.
+            If True, keep compressed branches as polytomies. Applies to greedy resolve
+         resolution_threshold : float
+            minimal delta LH to consider for polytomy resolution. Otherwise, keep parent as polytomy
+         stochastic_resolve : bool
+            generate a stochastic binary coalescent tree with mutation from the children of
+            a polytomy. Doesn't necessarily resolve the node fully. This step is stochastic
+            and different runs will result in different outcomes.
 
         Returns
         --------
          poly_found : int
             The number of polytomies found
 
         """
         self.logger("TreeTime.resolve_polytomies: resolving multiple mergers...",1)
         poly_found=0
 
         for n in self.tree.find_clades():
             if len(n.clades) > 2:
                 prior_n_clades = len(n.clades)
-                self._poly(n, merge_compressed, resolution_threshold=resolution_threshold)
+                if stochastic_resolve:
+                    self.generate_subtree(n)
+                else:
+                    self._poly(n, merge_compressed, resolution_threshold=resolution_threshold)
+
                 poly_found+=prior_n_clades - len(n.clades)
 
         obsolete_nodes = [n for n in self.tree.find_clades() if len(n.clades)==1 and n.up is not None]
         for node in obsolete_nodes:
             self.logger('TreeTime.resolve_polytomies: remove obsolete node '+node.name,4)
             if node.up is not None:
                 self.tree.collapse(node)
@@ -612,15 +625,15 @@
         return poly_found
 
 
     def _poly(self, clade, merge_compressed, resolution_threshold):
 
         """
         Function to resolve polytomies for a given parent node. If the
-        number of the direct decendants is less than three (not a polytomy), does
+        number of the direct descendants is less than three (not a polytomy), does
         nothing. Otherwise, for each pair of nodes, assess the possible LH increase
         which could be gained by merging the two nodes. The increase in the LH is
         basically the tradeoff between the gain of the LH due to the changing the
         branch lengths towards the optimal values and the decrease due to the
         introduction of the new branch with zero optimal length.
         """
 
@@ -628,30 +641,37 @@
 
         zero_branch_slope = self.gtr.mu*self.data.full_length
 
         def _c_gain(t, n1, n2, parent):
             """
             cost gain if nodes n1, n2 are joined and their parent is placed at time t
             cost gain = (LH loss now) - (LH loss when placed at time t)
+            NOTE: this cost function ignores the coalescent likelihood. Given the greedy
+            and approximate nature of this calculation, this seems justified. But this
+            entire procedure is not well suited for large polytomies.
             """
-            cg2 = n2.branch_length_interpolator._func(parent.time_before_present - n2.time_before_present) - n2.branch_length_interpolator._func(t - n2.time_before_present)
+            # old - new contributions of child branches
             cg1 = n1.branch_length_interpolator._func(parent.time_before_present - n1.time_before_present) - n1.branch_length_interpolator._func(t - n1.time_before_present)
+            cg2 = n2.branch_length_interpolator._func(parent.time_before_present - n2.time_before_present) - n2.branch_length_interpolator._func(t - n2.time_before_present)
+            # old - new contribution of additional branch (no old contribution)
             cg_new = - zero_branch_slope * (parent.time_before_present - t) # loss in LH due to the new branch
-            return -(cg2+cg1+cg_new)
+
+            return -(cg2 + cg1 + cg_new)
 
         def cost_gain(n1, n2, parent):
             """
             cost gained if the two nodes would have been connected.
             """
             try:
                 cg = sciopt.minimize_scalar(_c_gain,
                     bounds=[max(n1.time_before_present,n2.time_before_present), parent.time_before_present],
                     method='bounded',args=(n1,n2, parent), options={'xatol':1e-4*self.one_mutation})
                 return cg['x'], - cg['fun']
             except:
+                import ipdb; ipdb.set_trace()
                 self.logger("TreeTime._poly.cost_gain: optimization of gain failed", 3, warn=True)
                 return parent.time_before_present, 0.0
 
 
         def merge_nodes(source_arr, isall=False):
             mergers = np.array([[cost_gain(n1,n2, clade) if i1<i2 else (0.0,-1.0)
                                     for i1,n1 in enumerate(source_arr)]
@@ -749,14 +769,118 @@
         LH = merge_nodes(stretched, isall=len(stretched)==len(clade.clades))
         if merge_compressed and len(compressed)>1:
             LH += merge_nodes(compressed, isall=len(compressed)==len(clade.clades))
 
         return LH
 
 
+    def generate_subtree(self, parent):
+        from numpy.random import exponential as exp_dis
+        L = self.data.full_length
+        mutation_rate = self.gtr.mu*L
+
+        tmax = parent.time_before_present
+        branches_by_time = sorted(parent.clades, key=lambda x:x.time_before_present)
+        # calculate the mutations on branches leading to nodes from the mutation length
+        # this excludes state chances to ambiguous states
+        mutations_per_branch = {b.name:round(b.mutation_length*L) for b in branches_by_time}
+
+        branches_alive=branches_by_time[:1]
+        branches_to_come = branches_by_time[1:]
+        t = branches_alive[-1].time_before_present
+        if t>=tmax:
+            # no time left -- keep everything as individual children.
+            return
+
+        # if there is no coalescent model, assume a rate that would typically coalesce all tips
+        # in the time window between the latest and the parent node.
+        dummy_coalescent_rate = 2.0/(tmax-t)
+        self.logger(f"TreeTime.generate_subtree: node {parent.name} has {len(branches_by_time)} children."
+                    +f" {len([b for b,k in mutations_per_branch.items() if k>0])} have mutations."
+                    +f" The time window for coalescence is {tmax-t:1.4e}",3)
+
+        # loop until time collides with the parent node or all but two branches have been dealt with
+        # the remaining two would be the children of the parent
+        while len(branches_alive)+len(branches_to_come)>2 and t<tmax:
+            total_mutations = np.sum([mutations_per_branch.get(b.name,0) for b in branches_alive])
+            total_mut_rate = mutation_rate * total_mutations
+
+            # branches without mutations are ready to coalesce -- others have to mutate first
+            ready_to_coalesce = [b for b in branches_alive if mutations_per_branch.get(b.name,0)==0]
+            if self.merger_model is None:
+                total_coalescent_rate = max(0,(len(ready_to_coalesce)-1))*(dummy_coalescent_rate + mutation_rate)
+            else:
+                total_coalescent_rate = max(0,(len(ready_to_coalesce)-1))*(self.merger_model.branch_merger_rate(t) + mutation_rate)
+
+            # just a single branch and no mutations --> advance to next branch
+            if (total_mut_rate + total_coalescent_rate)==0 and len(branches_to_come):
+                branches_alive.append(branches_to_come.pop(0))
+                t = branches_alive[-1].time_before_present
+                continue
+
+            # determine the next time step
+            total_rate_inv = 1.0/(total_mut_rate + total_coalescent_rate)
+            dt = exp_dis(total_rate_inv)
+            t+=dt
+            # if the time advanced past the next branch in the branches_to_come list
+            # add this branch to branches alive and re-renter the loop
+            if len(branches_to_come) and t>branches_to_come[0].time_before_present:
+                while len(branches_to_come) and t>branches_to_come[0].time_before_present:
+                    branches_alive.append(branches_to_come.pop(0))
+            # else mutate or coalesce
+            else:
+                # determine whether to mutate or coalesce
+                p = np.random.random()
+                mut_or_coal = p<total_mut_rate*total_rate_inv
+                if mut_or_coal:
+                    # transform p to be on a scale of 0 to total mutation
+                    p /= total_mut_rate*total_rate_inv
+                    p *= total_mutations
+                    # discount one mutation at a time until p<0, break and remove that mutation
+                    for b in branches_alive:
+                        p -= mutations_per_branch.get(b.name,0)
+                        if p<0: break
+                    mutations_per_branch[b.name] -= 1
+                else:
+                    # pick a pair to coalesce, make a new node.
+                    picks = np.random.choice(len(ready_to_coalesce), size=2, replace=False)
+                    new_node = Phylo.BaseTree.Clade()
+                    new_node.time_before_present = t
+                    n1, n2 = ready_to_coalesce[picks[0]], ready_to_coalesce[picks[1]]
+                    new_node.clades = [n1, n2]
+                    new_node.mutation_length = 0.0
+                    n1.branch_length = t - n1.time_before_present
+                    n2.branch_length = t - n2.time_before_present
+                    n1.up = new_node
+                    n2.up = new_node
+                    if n1.mask is None or n2.mask is None:
+                        new_node.mask = None
+                        new_node.mcc = None
+                    else:
+                        new_node.mask = n1.mask * n2.mask
+                        new_node.mcc = n1.mcc if n1.mcc==n2.mcc else None
+                        self.logger('TreeTime._poly.merge_nodes: assigning mcc to new node ' + new_node.mcc, 4)
+                    new_node.up = parent
+                    new_node.tt = self
+                    if hasattr(parent, "_cseq"):
+                        new_node._cseq = parent._cseq
+                        self.add_branch_state(new_node)
+                    branches_alive = [b for b in branches_alive if b not in [n1,n2]] + [new_node]
+
+        remaining_branches = []
+        for b in branches_alive + branches_to_come:
+            b.branch_length = tmax - b.time_before_present
+            b.up = parent
+            remaining_branches.append(b)
+
+        self.logger(f"TreeTime.generate_subtree: node {parent.name} was resolved from {len(branches_by_time)} to {len(remaining_branches)} children.",3)
+        # assign the remaining branches as new clades to the parent.
+        parent.clades = remaining_branches
+
+
     def print_lh(self, joint=True):
         """
         Print the total likelihood of the tree given the constrained leaves
 
         Parameters
         ----------
```

### Comparing `phylo-treetime-0.9.5/treetime/utils.py` & `phylo-treetime-0.9.6/treetime/utils.py`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/treetime/vcf_utils.py` & `phylo-treetime-0.9.6/treetime/vcf_utils.py`

 * *Files identical despite different names*

### Comparing `phylo-treetime-0.9.5/treetime/wrappers.py` & `phylo-treetime-0.9.6/treetime/wrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -581,14 +581,17 @@
             coalescent = params.coalescent
         else:
             print("unknown coalescent model specification, has to be either "
                   "a float, 'opt', 'const' or 'skyline' -- exiting")
             return 1
     n_branches_posterior = params.n_branches_posterior
 
+    if hasattr(params, 'stochastic_resolve'):
+        stochastic_resolve = params.stochastic_resolve
+    else: stochastic_resolve = False
 
     # determine whether confidence intervals are to be computed and how the
     # uncertainty in the rate estimate should be treated
     calc_confidence = params.confidence
     if params.clock_std_dev:
         vary_rate = params.clock_std_dev if calc_confidence else False
     elif params.confidence and params.covariation:
@@ -611,14 +614,15 @@
 
     time_marginal = reduce_time_marginal_argument(params.time_marginal)
     # RUN
     root = None if params.keep_root else params.reroot
     try:
         success = myTree.run(root=root, relaxed_clock=relaxed_clock_params,
                resolve_polytomies=(not params.keep_polytomies),
+               stochastic_resolve = stochastic_resolve,
                Tc=coalescent, max_iter=params.max_iter,
                fixed_clock_rate=params.clock_rate,
                n_iqd=params.clock_filter,
                time_marginal="confidence-only" if (calc_confidence and time_marginal=='never') else time_marginal,
                vary_rate = vary_rate,
                branch_length_mode = branch_length_mode,
                reconstruct_tip_states=params.reconstruct_tip_states,
```

