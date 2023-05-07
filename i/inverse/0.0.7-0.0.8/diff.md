# Comparing `tmp/inverse-0.0.7-py3-none-any.whl.zip` & `tmp/inverse-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,95 +1,106 @@
-Zip file size: 280149 bytes, number of entries: 93
+Zip file size: 286904 bytes, number of entries: 104
 -rw-r--r--  2.0 unx      330 b- defN 80-Jan-01 00:00 inverse/__init__.py
 -rw-r--r--  2.0 unx        9 b- defN 80-Jan-01 00:00 inverse/__version__.py
 -rw-r--r--  2.0 unx     1281 b- defN 80-Jan-01 00:00 inverse/c_ext/vector_ops.c
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/__init__.py
 -rw-r--r--  2.0 unx     1380 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/cdeneme.py
 -rw-r--r--  2.0 unx    16728 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/clib
 -rw-r--r--  2.0 unx      216 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/clib.c
 -rw-r--r--  2.0 unx    16232 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/clibSHARED.so
 -rw-r--r--  2.0 unx   222942 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/clibrary.so
 -rw-r--r--  2.0 unx     5342 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/ctypes_class.py
 -rw-r--r--  2.0 unx     2311 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/ctypes_class_float.py
 -rw-r--r--  2.0 unx      468 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/deneme_sum.py
 -rw-r--r--  2.0 unx      621 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/deneme_vector.py
--rw-r--r--  2.0 unx     1238 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/get_c_loc.py
+-rw-r--r--  2.0 unx     1134 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/get_c_loc.py
 -rw-r--r--  2.0 unx     1687 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/lu_comp.c
 -rw-r--r--  2.0 unx     5683 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/restats
 -rw-r--r--  2.0 unx      445 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/sum.c
 -rw-r--r--  2.0 unx    16912 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/vector_ops
 -rw-r--r--  2.0 unx     2332 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/vector_ops.c
 -rw-r--r--  2.0 unx    91050 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/vector_ops.so
 -rw-r--r--  2.0 unx   224109 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/vector_ops2.so
 -rwxr-xr-x  2.0 unx    33818 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/vector_opsMAC
 -rw-r--r--  2.0 unx    16528 b- defN 80-Jan-01 00:00 inverse/ctypes_loc/vector_opsSHARED.so
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/src/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/src/benchmarks/__init__.py
--rw-r--r--  2.0 unx     1973 b- defN 80-Jan-01 00:00 inverse/src/benchmarks/alternatives.py
+-rw-r--r--  2.0 unx     2018 b- defN 80-Jan-01 00:00 inverse/src/benchmarks/alternatives.py
 -rw-r--r--  2.0 unx      599 b- defN 80-Jan-01 00:00 inverse/src/benchmarks/vector_nonvector.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 inverse/src/benchmarks/vector_ops_timeit.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/src/classes/__init__.py
--rw-r--r--  2.0 unx      789 b- defN 80-Jan-01 00:00 inverse/src/classes/_logger.py
 -rw-r--r--  2.0 unx     2364 b- defN 80-Jan-01 00:00 inverse/src/classes/abstract_data.py
--rw-r--r--  2.0 unx     1965 b- defN 80-Jan-01 00:00 inverse/src/classes/abstract_data2.py
--rw-r--r--  2.0 unx     5706 b- defN 80-Jan-01 00:00 inverse/src/classes/buffer_ops.py
+-rw-r--r--  2.0 unx     1902 b- defN 80-Jan-01 00:00 inverse/src/classes/abstract_data2.py
+-rw-r--r--  2.0 unx     6279 b- defN 80-Jan-01 00:00 inverse/src/classes/buffer_ops.py
 -rw-r--r--  2.0 unx     4021 b- defN 80-Jan-01 00:00 inverse/src/classes/buffer_ops_old_yedek.py
 -rw-r--r--  2.0 unx     4177 b- defN 80-Jan-01 00:00 inverse/src/classes/db_ops.py
 -rw-r--r--  2.0 unx     2584 b- defN 80-Jan-01 00:00 inverse/src/classes/randomMatrix.py
--rw-r--r--  2.0 unx     1184 b- defN 80-Jan-01 00:00 inverse/src/classes/random_sparse.py
+-rw-r--r--  2.0 unx     1247 b- defN 80-Jan-01 00:00 inverse/src/classes/random_sparse.py
 -rw-r--r--  2.0 unx      753 b- defN 80-Jan-01 00:00 inverse/src/classes/sp_matrix.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/src/engine/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/src/engine/algos/__init__.py
 -rw-r--r--  2.0 unx     2028 b- defN 80-Jan-01 00:00 inverse/src/engine/algos/_mappings.py
--rw-r--r--  2.0 unx     2220 b- defN 80-Jan-01 00:00 inverse/src/engine/algos/_progress.py
--rw-r--r--  2.0 unx     2032 b- defN 80-Jan-01 00:00 inverse/src/engine/algos/_spsparse.py
--rw-r--r--  2.0 unx     5264 b- defN 80-Jan-01 00:00 inverse/src/engine/algos/base_algo.py
--rw-r--r--  2.0 unx      707 b- defN 80-Jan-01 00:00 inverse/src/engine/algos_save/_save_base.py
--rw-r--r--  2.0 unx     3973 b- defN 80-Jan-01 00:00 inverse/src/engine/algos_save/_save_sparse.py
+-rw-r--r--  2.0 unx     2237 b- defN 80-Jan-01 00:00 inverse/src/engine/algos/_progress.py
+-rw-r--r--  2.0 unx     2329 b- defN 80-Jan-01 00:00 inverse/src/engine/algos/_progress_blast.py
+-rw-r--r--  2.0 unx     2490 b- defN 80-Jan-01 00:00 inverse/src/engine/algos/_spsparse.py
+-rw-r--r--  2.0 unx     1882 b- defN 80-Jan-01 00:00 inverse/src/engine/algos/_spsparse_blast.py
+-rw-r--r--  2.0 unx       78 b- defN 80-Jan-01 00:00 inverse/src/engine/algos/_vector_ops.py
+-rw-r--r--  2.0 unx     5283 b- defN 80-Jan-01 00:00 inverse/src/engine/algos/base_algo.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/src/engine/algos/benchmarks/__init__.py
+-rw-r--r--  2.0 unx      790 b- defN 80-Jan-01 00:00 inverse/src/engine/algos/benchmarks/vector_ops_bench.py
+-rw-r--r--  2.0 unx     1315 b- defN 80-Jan-01 00:00 inverse/src/engine/algos_save/_save_base.py
+-rw-r--r--  2.0 unx     4534 b- defN 80-Jan-01 00:00 inverse/src/engine/algos_save/_save_sparse.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/src/engine/base_classes/__init__.py
 -rw-r--r--  2.0 unx      367 b- defN 80-Jan-01 00:00 inverse/src/engine/base_classes/big_matrix_base.py
 -rw-r--r--  2.0 unx     1884 b- defN 80-Jan-01 00:00 inverse/src/engine/main.py
--rw-r--r--  2.0 unx     2678 b- defN 80-Jan-01 00:00 inverse/src/engine/main_funcs_to_load.py
--rw-r--r--  2.0 unx     5833 b- defN 80-Jan-01 00:00 inverse/src/engine/matrix_converters.py
--rw-r--r--  2.0 unx     2705 b- defN 80-Jan-01 00:00 inverse/src/engine/nontest_test.py
+-rw-r--r--  2.0 unx     2677 b- defN 80-Jan-01 00:00 inverse/src/engine/main_funcs_to_load.py
+-rw-r--r--  2.0 unx     4380 b- defN 80-Jan-01 00:00 inverse/src/engine/matrix_converters.py
+-rw-r--r--  2.0 unx     2763 b- defN 80-Jan-01 00:00 inverse/src/engine/nontest_test.py
 -rw-r--r--  2.0 unx     3357 b- defN 80-Jan-01 00:00 inverse/src/engine/sp_matrix_ops.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/src/large_data/__init__.py
 -rw-r--r--  2.0 unx      467 b- defN 80-Jan-01 00:00 inverse/src/large_data/data_converters.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/src/loggers/__init__.py
+-rw-r--r--  2.0 unx      790 b- defN 80-Jan-01 00:00 inverse/src/loggers/_logger.py
+-rw-r--r--  2.0 unx     2087 b- defN 80-Jan-01 00:00 inverse/src/loggers/_logger3.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/src/optimizations/__init__.py
 -rw-r--r--  2.0 unx     2912 b- defN 80-Jan-01 00:00 inverse/src/optimizations/optimizations_when.py
 -rw-r--r--  2.0 unx      958 b- defN 80-Jan-01 00:00 inverse/src/optimizations/quick_funcs.py
+-rw-r--r--  2.0 unx     1884 b- defN 80-Jan-01 00:00 inverse/src/sp_utils/_logger3.py.lib
+-rw-r--r--  2.0 unx     1503 b- defN 80-Jan-01 00:00 inverse/src/sp_utils/pickle_works.py.lib
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/src/testing_utils/__init__.py
 -rw-r--r--  2.0 unx      412 b- defN 80-Jan-01 00:00 inverse/src/testing_utils/timeit_sp.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/src/utils/__init__.py
 -rw-r--r--  2.0 unx       87 b- defN 80-Jan-01 00:00 inverse/src/utils/check_result.py
 -rw-r--r--  2.0 unx       39 b- defN 80-Jan-01 00:00 inverse/src/utils/initial_checks_matrix.py
 -rw-r--r--  2.0 unx      292 b- defN 80-Jan-01 00:00 inverse/src/utils/inverse_typings.py
 -rw-r--r--  2.0 unx       83 b- defN 80-Jan-01 00:00 inverse/src/utils/measure_calls.py
 -rw-r--r--  2.0 unx      283 b- defN 80-Jan-01 00:00 inverse/src/utils/opening_logo.py
 -rw-r--r--  2.0 unx      547 b- defN 80-Jan-01 00:00 inverse/src/utils/partition.py
 -rw-r--r--  2.0 unx      474 b- defN 80-Jan-01 00:00 inverse/src/utils/pickle_file.py
--rw-r--r--  2.0 unx      823 b- defN 80-Jan-01 00:00 inverse/src/utils/pickle_works.py
+-rw-r--r--  2.0 unx     1503 b- defN 80-Jan-01 00:00 inverse/src/utils/pickle_works.py
 -rw-r--r--  2.0 unx      174 b- defN 80-Jan-01 00:00 inverse/src/utils/sp_general_utils.py
 -rw-r--r--  2.0 unx     3501 b- defN 80-Jan-01 00:00 inverse/src/utils/sp_utils_inverse.py
 -rw-r--r--  2.0 unx      285 b- defN 80-Jan-01 00:00 inverse/src/utils/sure.py
--rw-r--r--  2.0 unx     1283 b- defN 80-Jan-01 00:00 inverse/src/utils/tuple_for_buffer.py
+-rw-r--r--  2.0 unx     1244 b- defN 80-Jan-01 00:00 inverse/src/utils/tuple_for_buffer.py
 -rw-r--r--  2.0 unx     1342 b- defN 80-Jan-01 00:00 inverse/src/utils/tuple_for_buffer.pyx
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/src/vector_ops/__init__.py
 -rw-r--r--  2.0 unx     1063 b- defN 80-Jan-01 00:00 inverse/src/vector_ops/d1.py
 -rw-r--r--  2.0 unx       46 b- defN 80-Jan-01 00:00 inverse/tests/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/tests/c_tests2/__init__.py
 -rw-r--r--  2.0 unx     1139 b- defN 80-Jan-01 00:00 inverse/tests/c_tests2/c_tests.py
 -rw-r--r--  2.0 unx      660 b- defN 80-Jan-01 00:00 inverse/tests/main_test.py
--rw-r--r--  2.0 unx     3631 b- defN 80-Jan-01 00:00 inverse/tests/mini_tests.py
 -rw-r--r--  2.0 unx      173 b- defN 80-Jan-01 00:00 inverse/tests/tdisplay.py
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 inverse/tests/test_alternatives.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/tests/test_classes/__init__.py
 -rw-r--r--  2.0 unx      206 b- defN 80-Jan-01 00:00 inverse/tests/test_classes/test_buffer.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 inverse/tests/test_inverse_matrices/__init__.py
 -rw-r--r--  2.0 unx     1300 b- defN 80-Jan-01 00:00 inverse/tests/test_inverse_matrices/test_some.py
+-rw-r--r--  2.0 unx      715 b- defN 80-Jan-01 00:00 inverse/tests/test_inverse_matrices/test_sparse_inverse.py
+-rw-r--r--  2.0 unx      421 b- defN 80-Jan-01 00:00 inverse/tests/test_main.py
 -rw-r--r--  2.0 unx     1443 b- defN 80-Jan-01 00:00 inverse/tests/test_matrix_op_main.py
+-rw-r--r--  2.0 unx     3630 b- defN 80-Jan-01 00:00 inverse/tests/test_mini_tests.py
 -rw-r--r--  2.0 unx     1548 b- defN 80-Jan-01 00:00 inverse/tests/tests.py
--rw-r--r--  2.0 unx      435 b- defN 80-Jan-01 00:00 inverse/tests/tests_main.py
--rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 inverse-0.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     2327 b- defN 80-Jan-01 00:00 inverse-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 inverse-0.0.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx     8307 b- defN 16-Jan-01 00:00 inverse-0.0.7.dist-info/RECORD
-93 files, 758675 bytes uncompressed, 266797 bytes compressed:  64.8%
+-rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 inverse-0.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2327 b- defN 80-Jan-01 00:00 inverse-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 inverse-0.0.8.dist-info/WHEEL
+?rw-r--r--  2.0 unx     9388 b- defN 16-Jan-01 00:00 inverse-0.0.8.dist-info/RECORD
+104 files, 772432 bytes uncompressed, 271786 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -81,17 +81,14 @@
 
 Filename: inverse/src/benchmarks/vector_ops_timeit.py
 Comment: 
 
 Filename: inverse/src/classes/__init__.py
 Comment: 
 
-Filename: inverse/src/classes/_logger.py
-Comment: 
-
 Filename: inverse/src/classes/abstract_data.py
 Comment: 
 
 Filename: inverse/src/classes/abstract_data2.py
 Comment: 
 
 Filename: inverse/src/classes/buffer_ops.py
@@ -120,20 +117,35 @@
 
 Filename: inverse/src/engine/algos/_mappings.py
 Comment: 
 
 Filename: inverse/src/engine/algos/_progress.py
 Comment: 
 
+Filename: inverse/src/engine/algos/_progress_blast.py
+Comment: 
+
 Filename: inverse/src/engine/algos/_spsparse.py
 Comment: 
 
+Filename: inverse/src/engine/algos/_spsparse_blast.py
+Comment: 
+
+Filename: inverse/src/engine/algos/_vector_ops.py
+Comment: 
+
 Filename: inverse/src/engine/algos/base_algo.py
 Comment: 
 
+Filename: inverse/src/engine/algos/benchmarks/__init__.py
+Comment: 
+
+Filename: inverse/src/engine/algos/benchmarks/vector_ops_bench.py
+Comment: 
+
 Filename: inverse/src/engine/algos_save/_save_base.py
 Comment: 
 
 Filename: inverse/src/engine/algos_save/_save_sparse.py
 Comment: 
 
 Filename: inverse/src/engine/base_classes/__init__.py
@@ -159,23 +171,38 @@
 
 Filename: inverse/src/large_data/__init__.py
 Comment: 
 
 Filename: inverse/src/large_data/data_converters.py
 Comment: 
 
+Filename: inverse/src/loggers/__init__.py
+Comment: 
+
+Filename: inverse/src/loggers/_logger.py
+Comment: 
+
+Filename: inverse/src/loggers/_logger3.py
+Comment: 
+
 Filename: inverse/src/optimizations/__init__.py
 Comment: 
 
 Filename: inverse/src/optimizations/optimizations_when.py
 Comment: 
 
 Filename: inverse/src/optimizations/quick_funcs.py
 Comment: 
 
+Filename: inverse/src/sp_utils/_logger3.py.lib
+Comment: 
+
+Filename: inverse/src/sp_utils/pickle_works.py.lib
+Comment: 
+
 Filename: inverse/src/testing_utils/__init__.py
 Comment: 
 
 Filename: inverse/src/testing_utils/timeit_sp.py
 Comment: 
 
 Filename: inverse/src/utils/__init__.py
@@ -234,47 +261,53 @@
 
 Filename: inverse/tests/c_tests2/c_tests.py
 Comment: 
 
 Filename: inverse/tests/main_test.py
 Comment: 
 
-Filename: inverse/tests/mini_tests.py
-Comment: 
-
 Filename: inverse/tests/tdisplay.py
 Comment: 
 
 Filename: inverse/tests/test_alternatives.py
 Comment: 
 
+Filename: inverse/tests/test_classes/__init__.py
+Comment: 
+
 Filename: inverse/tests/test_classes/test_buffer.py
 Comment: 
 
 Filename: inverse/tests/test_inverse_matrices/__init__.py
 Comment: 
 
 Filename: inverse/tests/test_inverse_matrices/test_some.py
 Comment: 
 
+Filename: inverse/tests/test_inverse_matrices/test_sparse_inverse.py
+Comment: 
+
+Filename: inverse/tests/test_main.py
+Comment: 
+
 Filename: inverse/tests/test_matrix_op_main.py
 Comment: 
 
-Filename: inverse/tests/tests.py
+Filename: inverse/tests/test_mini_tests.py
 Comment: 
 
-Filename: inverse/tests/tests_main.py
+Filename: inverse/tests/tests.py
 Comment: 
 
-Filename: inverse-0.0.7.dist-info/LICENSE
+Filename: inverse-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: inverse-0.0.7.dist-info/METADATA
+Filename: inverse-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: inverse-0.0.7.dist-info/WHEEL
+Filename: inverse-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: inverse-0.0.7.dist-info/RECORD
+Filename: inverse-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## inverse/ctypes_loc/get_c_loc.py

```diff
@@ -33,23 +33,20 @@
     cfiles = {
         'clib.c': c1,
         'vector_ops.c': c2
     }
     return cfiles[name_of_file][platform_name]
 
 
+
+
 @lru_cache(maxsize=128, typed=False)
 def get_c_lib(name_of_file='clib.c'):
-    obj = {'Windows': ctypes.CDLL,
-           'Linux': cdll.LoadLibrary,
-           'Mac':  cdll.LoadLibrary}
-    fnc = obj[get_platform()]
-    file_name = get_c_file_for_platform(name_of_file)
-    path = Path(os.path.dirname(__file__))
-    file_name_full = os.path.join(path, file_name)
 
-    return fnc(file_name_full)
+    return {'Windows': ctypes.CDLL,
+           'Linux': cdll.LoadLibrary,
+           'Mac':  cdll.LoadLibrary}[get_platform()](os.path.join(Path(os.path.dirname(__file__)), get_c_file_for_platform(name_of_file)))
 
 
 __all__ = [
     'get_c_lib'
 ]
```

## inverse/src/benchmarks/alternatives.py

```diff
@@ -1,43 +1,43 @@
 from abc import ABC
 
 import scipy.sparse.linalg as splu
 from scipy.sparse import eye
 from scipy.sparse.linalg import (inv, spsolve)
 
-from inverse.src.classes._logger import set_logger
 from inverse.src.classes.random_sparse import get_random_sparse
+from inverse.src.loggers._logger3 import get_my_logger, free_logger
 
 
 # N = Bs.shape[0]
 # iBs = inv(Bs)
 # iBs = spsolve(Bs, eye(N))
 
-
 class AlternativesInverse(ABC):
     """AlternativesInverse"""
 
     def __init__(self):
         # self.logger = logging.getLogger(self.__class__.__name__)
         name = self.__class__.__name__
         # print(name, " started  ...")
-        self.logger = set_logger(name, "AlternativesInverse.log")
+        self.logger = free_logger #  get_my_logger(name)  # set_logger(name, "AlternativesInverse.log")
+
         self.log(f"{name} started...")
         # self.warn(f"{name} started...")
         # self.log(f"{name} started...")
 
     # def warn(self, msg):
     #     self.logger.warning(msg)
     #     self.logger.info(msg)
 
     def log(self, msg):
-        self.logger.info(msg)
+        self.logger(msg)
 
     def log2(self, msg):
-        self.logger.info(msg)
+        self.logger(msg)
 
 
 class SPLUInverse(AlternativesInverse):
     """SPLUInverse"""
 
     def inv(self, matrix):
         return splu.inv(matrix)
```

## inverse/src/classes/abstract_data2.py

```diff
@@ -1,58 +1,57 @@
+import functools
+
 from inverse.src.classes.abstract_data import DataAbstract
 from inverse.src.classes.db_ops import DB_class_Opt
+from inverse.src.engine.algos_save._save_sparse import algo_save_sparse_on_begin
+from inverse.src.loggers._logger3 import get_my_logger
 from inverse.src.utils.inverse_typings import *
 from inverse.src.utils.partition import table_name_format
 
+logging_ = get_my_logger('DBDataOpt')
+
 
 class DBDataOpt(DataAbstract):
     buffer: dict = {}
 
     def __init__(self, threshold: int, name="test"):
         self.threshold = threshold
         self.name = name
         self.db_option = DB_class_Opt
 
     def key_format(self, r: int, name=False) -> str:
         if not name:
             name = self.name
         return f"{name}_{r}"
 
+    @logging_
     def transpose_list(self, big_list: list_tuple, say: int) -> pddf:
-        print("I will transopoze this ", big_list)
-
         def get_name(index):
             return f"column_{self.threshold * (say) + index}"
 
         column_names = list(map(get_name, range(0, self.threshold)))
-        print(column_names, "column_names")
-        df = pd.DataFrame(big_list)
-        print("df ...", df)
-        df_t = pd.DataFrame(big_list).transpose()
 
+        df_t = pd.DataFrame(big_list).transpose()
         if len(df_t.columns) < self.threshold:
             column_names = column_names[0:  len(df_t.columns)]
         df_t.columns = column_names
-
-        print("df_t ...")
-        print(df_t)
         return df_t
 
+    @logging_
     def save_part(self, say: int, big_list: list_tuple) -> None:
-
         self.db_option.write_db(table_name_format(self.name, say)
                                 , self.transpose_list(big_list, say))
 
+    @logging_
     def save_on_begin_rand(self, matrix: npar) -> None:
         from inverse.src.engine.algos_save._save_base import base_save_on_begin_rand
-        base_save_on_begin_rand(self, matrix)
+        return base_save_on_begin_rand(self, matrix)
 
+    @logging_
     def save_sparse_on_begin(self, sparce_matrix, id_ekle_option=True) -> None:
-        from inverse.src.engine.algos_save._save_sparse import algo_save_sparse_on_begin
-        matrix = sparce_matrix
-
         return algo_save_sparse_on_begin(self, sparce_matrix)
 
 
+@logging_
 def get_test_row(i):
     matrix = [[9, 17, 12], [2, 19, 12], [26, 8, 12]]
     return matrix[i]
```

## inverse/src/classes/buffer_ops.py

```diff
@@ -1,13 +1,17 @@
 from functools import lru_cache
 
-from .db_ops import DB_class_Opt
-from inverse.src.utils.measure_calls import CallStack
-from inverse.src.utils.partition import get_table_name_treshold, table_name_format, column_name_format, table_name_format_reverse
 from inverse.src.utils.inverse_typings import *
+from inverse.src.utils.measure_calls import CallStack
+from inverse.src.utils.partition import get_table_name_treshold, table_name_format, column_name_format, \
+    table_name_format_reverse
+from .db_ops import DB_class_Opt
+from ..loggers._logger3 import get_my_logger, free_logger
+
+logging_ = get_my_logger('Buffer')
 
 
 @lru_cache(maxsize=128, typed=False)
 def get_table_names_from_tuple(liste: list_tuple, threshold: int) -> list_tuple:
     new_set = []
     for i in liste:
         num = get_table_name_treshold(i, threshold)
@@ -57,14 +61,15 @@
 
         return tuple(map(table_name_format_reverse, tuple(self.buffer_data.keys())))
 
     @lru_cache(maxsize=128, typed=False)
     def buffer_key_format(self, say: int) -> str:
         return table_name_format(self.name, say)
 
+    @logging_
     def load_buffer(self, diff_set: list_tuple) -> None:
         """burada desteleri yükleyecek"""
 
         for set_say in diff_set:
 
             # print("loading ... ", set_say)
             table_name = table_name_format(self.name, set_say)
@@ -86,77 +91,101 @@
 
         for table_name in diff_set:
             try:
                 DB_class_Opt.write_db(table_name, self.buffer_data[table_name])
             except:
                 print("bunu bulamadım save_buffer ", table_name)
 
+    @logging_
     def empty_buffer(self, tuple_set=()) -> None:
         if tuple_set:
             for item in tuple_set:
-                self.buffer_data.pop(item)
+                try:
+                    self.buffer_data.pop(item)
+                except:
+                    print('no key found buffer ops 104', item)
         else:
             self.buffer_data = {}
 
+    @logging_
     def refresh_buffer(self, new_set: list_tuple, onload=False) -> None:
 
         old_set = self.buffer_get_current_key_nums()
 
         diff_set_garbage = tuple(x for x in old_set if x not in new_set)
         diff_set_load = tuple(x for x in new_set if x not in old_set)
-        if onload:
-            diff_set_load = new_set
+
+
+        if onload or not old_set:
+            return self.load_buffer(new_set)
+
         if self.threshold < len(tuple(self.buffer_data.keys())):
             ...
-            self.save_buffer(diff_set_garbage)
-            self.empty_buffer(diff_set_garbage)
+            # self.save_buffer(diff_set_garbage)
+            # self.empty_buffer(diff_set_garbage)
         if diff_set_load:
             self.load_buffer(diff_set_load)
 
+    @logging_
     def load_column_names_with_set_onload(self, column_tuple: list_tuple) -> None:
         CallStack["load_column_names_with_set_onload"] += 1
 
         new_set = get_table_names_from_tuple(tuple(set(column_tuple)), self.threshold)
 
-        self.refresh_buffer(new_set , onload=True )
+        self.refresh_buffer(new_set, onload=True)
+
+    @logging_
     def load_column_names_with_set(self, column_tuple: list_tuple) -> None:
         CallStack["load_column_names_with_set"] += 1
 
-        # column_tuple = tuple(set(column_tuple))
+        column_tuple = tuple(set(column_tuple))
 
-        # print("load_column_names_with_set column_tuple", column_tuple)
         # (0,)
         new_set = get_table_names_from_tuple(column_tuple, self.threshold)
         # print("load_column_names_with_set new_set", new_set)
+
+        # print("load_column_names_with_set new_set", new_set)
         # exit()
         self.refresh_buffer(new_set)
 
+    @logging_
     def setItem(self, num: int, i: int, data: list_tuple) -> None:
         buffer_key = self.buffer_key_format(num)
         df = self.buffer_data[buffer_key]
         keyname = column_name_format(i)
         df[keyname] = data
         self.buffer_data[buffer_key] = df
 
+    @logging_
     def get_column(self, i: int) -> pddf:
         column = column_name_format(i)
         keyName = self.columns_tables_dict[column]
         return self.buffer_data[keyName]
 
     def get_cell(self, j: int, i: int) -> int_float:
         column = column_name_format(j)
         df = self.get_column(j)
         return tuple(df[column])[i]
 
+    @logging_
     def get_row(self, i: int) -> tuple:
         column = column_name_format(i)
-        keyName = self.columns_tables_dict[column]
+
+        # free_logger(f'{self.columns_tables_dict.keys()} ')
+        try:
+            keyName = self.columns_tables_dict[column]
+        except:
+            print(column, i, 'ERROR', tuple(self.columns_tables_dict.keys()))
+            raise Exception
+
         return tuple(self.buffer_data[keyName][column])
 
+    @logging_
     def set_row(self, i: int, data: list_tuple) -> None:
         num = get_table_name_treshold(i, self.threshold)
         self.setItem(num, i, data)
 
+    @logging_
     def final_save(self) -> None:
         # print("final save operation")
         self.save_buffer()
         # self.buffer_data = {}
```

## inverse/src/classes/random_sparse.py

```diff
@@ -1,13 +1,15 @@
 import numpy as np
 from numpy.random import default_rng
 from scipy import stats
 from scipy.sparse import random
 from scipy.stats import rv_continuous
 
+from inverse.src.utils.pickle_works import sp_cache
+
 
 class CustomDistribution(rv_continuous):
     def _rvs(self, size=None, random_state=None):
         return random_state.standard_normal(size)
 
 
 rng = default_rng()
@@ -15,14 +17,15 @@
 
 def get_random_sparse2():
     X = CustomDistribution(seed=rng)
     print(X)
     return X
 
 
+@sp_cache
 def get_random_sparse(m=30, n=None, density=0.25):
     if not n:
         n = m
 
     rng = default_rng()
     rvs = stats.poisson(25, loc=10).rvs
     S = random(m, n, density=density, random_state=rng, data_rvs=rvs)
```

## inverse/src/engine/algos/_progress.py

```diff
@@ -2,20 +2,21 @@
 from rich.progress import Progress
 
 from inverse.src.engine.base_classes.big_matrix_base import BigMatrixAbstract
 from inverse.src.engine.sp_matrix_ops import divide_pivot, combine_row_op
 from inverse.src.utils.measure_calls import CallStack
 from inverse.src.utils.tuple_for_buffer import get_tuple_for_buffer
 
+
 def basic_algo_progress(bg_matrix: BigMatrixAbstract):
     self = bg_matrix
 
     with Progress() as progress:
         bucket = get_tuple_for_buffer(self.n, self.threshold)
-        task1 = progress.add_task("[red]Calculating...", total=len(bucket))
+        task1 = progress.add_task("[red]Calculating inverse matrix ...", total=len(bucket))
         for sira in bucket:
             CallStack["dıs_dongu"] += 1
             progress.update(task1, advance=1)
             # sira = tuple(x for x in sira if x < self.n)
             sira = tuple(int(x) for x in sira if x < self.n and x > -1)
             x, *y = sira
             y = tuple(set(y))
```

## inverse/src/engine/algos/_spsparse.py

```diff
@@ -1,64 +1,70 @@
 # from inverse import tic, toc
+from rich.progress import Progress
+
 from inverse.ctypes_loc.ctypes_class import py_operate_inside_double, c_divide
 from inverse.src.engine.base_classes.big_matrix_base import BigMatrixAbstract
 from inverse.src.utils.tuple_for_buffer import get_tuple_for_buffer
 from ...classes.sp_matrix import SPMatrix
 
 
 def basic_algo_spsparse(bg_matrix: BigMatrixAbstract, sp_matrix: SPMatrix):
-    self = bg_matrix
-    """TODO"""
-    global CallStack
-    from inverse import tic, toc
-
-    tic()
-    bucket = get_tuple_for_buffer(self.n, self.threshold)
-
-    for index, sira in enumerate(bucket):
-        # print(sira)
-        # exit()
-        CallStack["dis_dongu"] += 1
-        sira = tuple(int(x) for x in sira if x < self.n and x > -1)
-        i, *y = sira
-        y = tuple(set(y))
-        sira_set = tuple(set(sira))
-        self.buffer.load_column_names_with_set(sira_set)
-
-        row = tuple(self.buffer.get_row(i))
-        # pivot = row[i]
-
-        # SET Calculation
-        self.buffer.set_row(i, c_divide(row, row[i]))
-        mat_indexes, mat_vals = sp_matrix.get_line(i)
-        for j in (a for a in y if a != i):
-
-            if j not in mat_indexes:
-                # row2 = tuple(0 for _ in range(self.n))
-                # print(row2)
-
-                # self.buffer.set_row(j, tuple(0 for _ in range(self.n * 2)))
-                # exit()
-                continue
-
-            CallStack["ic_dongu"] += 1
-            row_J = tuple(self.buffer.get_row(j))  # 3 array
-            row_i = tuple(self.buffer.get_row(i))  # 4 array
-
-            number_j = row_J[i]
-            number_i = row_i[i]
-
-            nrow = py_operate_inside_double(
-                number_j, number_i, row_J, row_i, len(row_J))
-            # nrow = py_operate_inside_double_opt(i, row_J, row_i, len(row_J))
-
-            # SET Calculation
-
-            self.buffer.set_row(j, nrow)
-
-    self.buffer.final_save()
-    toc()
-    inv_matrix = self.buffer.get_current_matrix()
-    self.id_and_inv = inv_matrix
-    # print(inv_matrix)
-
-    return inv_matrix[:, self.n:]
+    raise NotImplementedError
+    #
+    # from inverse.src.utils.measure_calls import CallStack
+    # assert isinstance(bg_matrix, BigMatrixAbstract)
+    # assert isinstance(sp_matrix, SPMatrix)
+    #
+    # self = bg_matrix
+    # """TODO"""
+    # global CallStack
+    # from inverse import tic, toc
+    # msg = f"[red]Calculating inverse matrix {self.n} x {self.n} ..."
+    # # msg = "[red]Calculating inverse matrix   ..."
+    # tic()
+    # with Progress() as progress:
+    #     bucket = get_tuple_for_buffer(self.n, bg_matrix.threshold)
+    #     task1 = progress.add_task(msg, total=len(bucket))
+    #
+    #     # exit()
+    #     for index, sira in enumerate(bucket):
+    #
+    #         CallStack["dis_dongu"] += 1
+    #         progress.update(task1, advance=1)
+    #
+    #         sira = tuple(int(x) for x in sira if x < self.n and x > -1)
+    #         i, *y = sira
+    #
+    #         sira_set = tuple(set(sira))
+    #         self.buffer.load_column_names_with_set(sira_set)
+    #         row = tuple(self.buffer.get_row(i))
+    #         # pivot = row[i]
+    #
+    #         # SET Calculation
+    #         self.buffer.set_row(i, c_divide(row, row[i]))
+    #         mat_indexes, mat_vals = sp_matrix.get_line(i)
+    #         for j in (a for a in tuple(set(y)) if a != i):
+    #
+    #             if j not in mat_indexes:
+    #                 continue
+    #
+    #             CallStack["ic_dongu"] += 1
+    #             row_J = tuple(self.buffer.get_row(j))  # 3 array
+    #             row_i = tuple(self.buffer.get_row(i))  # 4 array
+    #
+    #             number_j = row_J[i]
+    #             number_i = row_i[i]
+    #
+    #             nrow = py_operate_inside_double(
+    #                 number_j, number_i, row_J, row_i, len(row_J))
+    #
+    #             # SET Calculation
+    #
+    #             self.buffer.set_row(j, nrow)
+    #
+    #     self.buffer.final_save()
+    #     toc()
+    #     inv_matrix = self.buffer.get_current_matrix()
+    #     self.id_and_inv = inv_matrix
+    #     # print(inv_matrix)
+    #
+    # return inv_matrix[:, self.n:]
```

## inverse/src/engine/algos/base_algo.py

```diff
@@ -8,15 +8,14 @@
 
 
 def basic_algo(bg_matrix: BigMatrixAbstract):
     from inverse.src.utils.measure_calls import CallStack
     global CallStack
     tic()
     bucket = get_tuple_for_buffer(bg_matrix.n, bg_matrix.threshold)
-    print(bucket)
     # exit()
     with Progress() as progress:
         task1 = progress.add_task("[red]Calculating...", total=len(bucket))
         for index, sira in enumerate(bucket):
             progress.update(task1, advance=1)
             CallStack["dis_dongu"] += 1
             sira = tuple(int(x) for x in \
@@ -39,14 +38,15 @@
                 # SET Calculation
                 bg_matrix.buffer.set_row(j, nrow)
 
     bg_matrix.buffer.final_save()
     toc()
     inv_matrix = bg_matrix.buffer.get_current_matrix()
     bg_matrix.id_and_inv = inv_matrix
+    print(CallStack)
 
     return inv_matrix[:, bg_matrix.n:]
 
 
 def basic_algo_sparse(bg_matrix: BigMatrixAbstract):
     from inverse.src.utils.measure_calls import CallStack
     global CallStack
@@ -55,15 +55,15 @@
 
     if bg_matrix.test:
         print("Since bg_matrix.test was True, bucket was reduced to 5 element.")
         bucket = bucket[:5]
     # print(bucket)
     # exit()
     with Progress() as progress:
-        task1 = progress.add_task("[red]Calculating...", total=len(bucket))
+        task1 = progress.add_task("[red]Calculating inverse matrix ...", total=len(bucket))
         for index, sira in enumerate(bucket):
             progress.update(task1, advance=1)
             CallStack["dis_dongu"] += 1
             sira = tuple(int(x) for x in \
                          sira if x < bg_matrix.n and x > -1)
             i, *y = sira
             sira_set = tuple(set(sira))
```

## inverse/src/engine/algos_save/_save_base.py

```diff
@@ -4,24 +4,40 @@
 
 # from inverse.src.classes.db_ops import DB_class_Opt
 
 
 def base_save_on_begin_rand(self: DataAbstract, matrix: npar) -> None:
     say = -1
     big_list = []
+    part_say = -1
+    for i in range(len(matrix)):
+        numbers = list(matrix[i])  # list(random.randint(0, 100) for _ in range(n))
+        numbers += id_ekle(i, len(matrix))
+        if len(big_list) == self.threshold:
+            say = 0
+            part_say += 1
+            self.save_part(part_say, big_list)
+            big_list = [numbers]
+        else:
+            say += 1
+            big_list.append(numbers)
+    if big_list:
+        part_say += 1
+        self.save_part(part_say, big_list)
+
 
+def base_save_on_begin_rand_yedek(self: DataAbstract, matrix: npar) -> None:
+    say = -1
+    big_list = []
 
     for i in range(len(matrix)):
         numbers = list(matrix[i])  # list(random.randint(0, 100) for _ in range(n))
         numbers += id_ekle(i, len(matrix))
         if len(big_list) == self.threshold:
             say += 1
             self.save_part(say, big_list)
             big_list = [numbers]
         else:
             big_list.append(numbers)
     if big_list:
         say += 1
         self.save_part(say, big_list)
-
-
-
```

## inverse/src/engine/algos_save/_save_sparse.py

```diff
@@ -1,60 +1,97 @@
 import numpy as np
+from rich.progress import Progress
 from scipy.sparse import csc_matrix
 
-from inverse import BigMatrixConverter, close_identity
 from inverse.src.classes.abstract_data import id_ekle, DataAbstract
 from inverse.src.classes.random_sparse import get_random_sparse
 from inverse.src.classes.sp_matrix import SPMatrix
-from inverse.src.utils.check_result import inverse_check
-from inverse.src.utils.measure_calls import CallStack
-
+from inverse.src.loggers._logger3 import get_my_logger
 
 # from inverse.src.classes.db_ops import DB_class_Opt
 
+save_sparse_logging = get_my_logger('save_sparse_logging')
+
 
 def get_zeros_and_values(coords, values, n):
     values_ = []
     # [ 0 , 5 , 12 ] [ 1 , 2 , 3 ]
     for i in range(n):
         if i not in coords:
             values_.append(0)
-
         else:
             values_.append(values.pop())
     return values_
 
 
+@save_sparse_logging
 def algo_save_sparse_on_begin(self: DataAbstract, sparce_matrix: csc_matrix) -> None:
+    """This Will get the sparse matrix and save it in the database"""
+    print('here ', sparce_matrix)
+    # exit()
     say = -1
+    part_say = -1
     big_list = []
+
     n = sparce_matrix.shape[0]
 
     sp_matrix = SPMatrix(sparce_matrix)
 
-    for i in range(n):
-        coords, values = sp_matrix.get_line(i)
-        # print(coords, values, "coords, values")
+    print('DB save started...')
+    # exit()
+    with Progress() as progress:
+        # bucket = get_tuple_for_buffer(self.n, self.threshold)
+        task1 = progress.add_task("[red]Writing to database...", total=n)
 
-        numbers = get_zeros_and_values(coords, values, n)
-        numbers += tuple(id_ekle(i, n))
+        for i in range(n):
 
-        # self.threshold = 500
-        if len(big_list) == self.threshold:
-            say += 1
-            self.save_part(say, big_list)
-            big_list = []
-        else:
-            big_list.append(numbers)
-    if big_list:
-        say += 1
-        self.save_part(say, big_list)
+            # print(i)
+            progress.update(task1, advance=1)
+            coords, values = sp_matrix.get_line(i)
+
+            numbers = get_zeros_and_values(coords, values, n)
+            numbers += tuple(id_ekle(i, n))
+            if len(big_list) == self.threshold:
+                say = 0
+                part_say += 1
+                self.save_part(part_say, big_list)
+                big_list = [numbers]
+
+            else:
+                say += 1
+                big_list.append(numbers)
+
+        if big_list:
+            part_say += 1
+            # print('SAVING THIS ONE TOO', say, big_list)
+
+            assert not (len(big_list) > self.threshold)
 
+            self.save_part(part_say, big_list)
 
-def t_save_sparse_on_begin(n=30, threshold=500, Test=False):
+
+def t_save_sparse_on_begin(n, threshold, test=False):
+    from inverse.src.engine.sp_matrix_ops import display_matrix_ozet
+    from inverse import BigMatrixConverter
+    matrix = get_random_sparse(m=n, n=n, density=0.25)
+    sparce_matrix = csc_matrix(matrix)
+    sp_mat = SPMatrix(sparce_matrix)
+
+    big_matrix = BigMatrixConverter(
+        "sparce_matrix_test").convert_sparse_to_bigmatrix(sparce_matrix, threshold)
+    big_matrix.test = test
+    inverse_mat = big_matrix.sp_inverse_with_spsparse(sp_mat)
+    if isinstance(inverse_mat, np.ndarray or np.matrix):
+        display_matrix_ozet(inverse_mat, "inverse_mat")
+
+
+# ---------------------------------------------------------------
+
+'''
+def t_save_sparse_on_begin222(n=30, threshold=500, Test=False):
     # threshold = 500
     # matrix = np.array([[19, 2, 3, 8],
     #                    [8, 3, 6, 9],
     #                    [7, 8, 15, 11],
     #                    [4, 7, 8, 5]])
 
     matrix = get_random_sparse(m=n, n=n, density=0.25)
@@ -64,15 +101,15 @@
     # print(matrix.shape, "matrix.shape")
     sparce_matrix = csc_matrix(matrix)
 
     # exit()
 
     big_matrix = BigMatrixConverter(
         "sparce_matrix_test").convert_sparse_to_bigmatrix(sparce_matrix, threshold)
-    big_matrix.test = False 
+    big_matrix.test = Test
     inverse_mat = big_matrix.sp_sparse_inverse()
     # inverse_mat = big_matrix.sp_inverse_progress()
     print(inverse_mat)
     return
 
     matrix_check = inverse_check(matrix)
 
@@ -88,38 +125,15 @@
     eps = 0.0001
     kontrol = close_identity(matrix=sonuc1, eps=eps)
     # kontrol2 = close_identity(matrix=sonuc2, eps=eps)
     kontrol2 = close_identity(matrix=sonuc3, eps=eps)
     print(CallStack)
 
 
-def t_save_sparse_on_begin(n=30, threshold=500, Test=False):
-    # threshold = 500
-    # matrix = np.array([[19, 2, 3, 8],
-    #                    [8, 3, 6, 9],
-    #                    [7, 8, 15, 11],
-    #                    [4, 7, 8, 5]])
-
-    matrix = get_random_sparse(m=n, n=n, density=0.25)
-
-    # eye = np.eye(3, dtype=np.int64)
-    # matrix = matrix + eye
-    # print(matrix.shape, "matrix.shape")
-    sparce_matrix = csc_matrix(matrix)
-
-    # exit()
-
-    big_matrix = BigMatrixConverter(
-        "sparce_matrix_test").convert_sparse_to_bigmatrix(sparce_matrix, threshold)
-    big_matrix.test = Test
-    inverse_mat = big_matrix.sp_sparse_inverse()
-    # inverse_mat = big_matrix.sp_inverse_progress()
-    print(inverse_mat)
-    return
-
+def _aaa():
     matrix_check = inverse_check(matrix)
 
     print(matrix, "matrix")
     print(inverse_mat, "inverse_mat")
     # print(inverse_mat2, "inverse_mat2")
     print(matrix_check, "matrix_check")
 
@@ -128,7 +142,11 @@
     sonuc3 = np.matmul(matrix, matrix_check)
 
     eps = 0.0001
     kontrol = close_identity(matrix=sonuc1, eps=eps)
     # kontrol2 = close_identity(matrix=sonuc2, eps=eps)
     kontrol2 = close_identity(matrix=sonuc3, eps=eps)
     print(CallStack)
+    
+
+
+'''
```

## inverse/src/engine/main_funcs_to_load.py

```diff
@@ -66,10 +66,10 @@
 
 
 #import pytest
 
 
 def test_all():
     import pytest
-    # pytest inverse/tests/tests_main.py -W ignore::DeprecationWarning -v
+    # pytest inverse/tests/test_main.py -W ignore::DeprecationWarning -v
     retcode = pytest.main()
     print("retcode = ", retcode)
```

## inverse/src/engine/matrix_converters.py

```diff
@@ -47,64 +47,18 @@
 
         self.db_rep.save_on_begin_rand(matrix)
 
     def save_on_begin_bigmatrix_lines(self, lines):
 
         self.db_rep.save_on_begin_bigmatrix_lines(lines)
 
-    def sp_inverse_hatali(self) -> np.array:
-        """TODO"""
-        global CallStack
-        from inverse import tic, toc
-
-        tic()
-        bucket = get_tuple_for_buffer(self.n, self.threshold)
-
-        for index, sira in enumerate(bucket):
-
-            sira = tuple(int(x) for x in sira if x < self.n and x > -1)
-            i, *y = sira
-            y = tuple(set(y))
-            sira_set = tuple(set(sira))
-            self.buffer.load_column_names_with_set(sira_set)
-
-            row = tuple(self.buffer.get_row(i))
-            # pivot = row[i]
-
-            # SET Calculation
-            self.buffer.set_row(i, c_divide(row, row[i]))
-
-            for j in (a for a in y if a != i):
-                # CallStack["ic_dongu"] += 1
-                # number_j = self.buffer.get_cell(j, i)  # 1 number
-                # number_i = self.buffer.get_cell(i, i)  # 2 number
-
-                # factor = number_j / number_i if number_i != 0 else 0
-                row_J = tuple(self.buffer.get_row(j))  # 3 array
-                row_i = tuple(self.buffer.get_row(i))  # 4 array
-                # nrow = row_J - c_multiply(row_i, factor)
-
-                nrow = py_operate_inside_double_opt(
-                    i, row_J, row_i, len(row_J))
-                # nrow = py_equivalent_operate_inside_double(i  , row_J, row_i, len(row_J))
-
-                # SET Calculation
-
-                self.buffer.set_row(j, nrow)
-
-        self.buffer.final_save()
-        toc()
-        inv_matrix = self.buffer.get_current_matrix()
-        self.id_and_inv = inv_matrix
-        # print(inv_matrix)
-
-        return inv_matrix[:, self.n:]
-
     def sp_inverse_with_spsparse(self, sp_matrix: SPMatrix) -> np.array:
-        return basic_algo_spsparse(self, sp_matrix)
+        return basic_algo(self)
+        # exit()
+        # return basic_algo_spsparse(self, sp_matrix)
 
     def sp_inverse_with_mappings(self, mappings) -> np.array:
         return basic_algo_mappings(self, mappings)
 
     def sp_inverse(self) -> np.array:
         return basic_algo(self)
 
@@ -126,20 +80,23 @@
         big_matrix.db_rep.save_on_begin_rand(matrix)
         return big_matrix
 
     def convert_sparse_to_bigmatrix(self,
                                     sparce_matrix: csc_matrix,
                                     threshold: int) -> BigMatrix:
         n = sparce_matrix.shape[0]
-
         big_matrix = BigMatrix(self.name, n, threshold)
+        # print('here...')
+        # exit()
         big_matrix.db_rep.save_sparse_on_begin(sparce_matrix)
         return big_matrix
 
-    def create_bigmatrix_from_lines(self, lines, name="test", threshold: int = 5) -> BigMatrix:
+    def create_bigmatrix_from_lines(self,
+                                    lines, name="test",
+                                    threshold: int = 5) -> BigMatrix:
         ...
         big_matrix = BigMatrix(self.name, len(lines), threshold)
         big_matrix.db_rep.save_on_begin_rand(lines)
         return big_matrix
 
 
 def convert_small_to_big(matrix, name='test', threshold=50):
```

## inverse/src/engine/nontest_test.py

```diff
@@ -33,30 +33,30 @@
 
         display_matrix_ozet(self.inv_matrix, "{0}   {1}  ".format(self.name, 'inv_matrix'))
         display_matrix_ozet(self.np_inv_matrix, "{0}   {1}  ".format(self.name, 'np_inv_matrix'))
         return ""
         # return f"matrix: {self.matrix} \n inv_matrix: {self.inv_matrix} \n np_inv_matrix: {self.np_inv_matrix} \n"
 
 
-def sp_inverse_t1(n, silent=False):
+def sp_inverse_t1(n,   threshold = 50 ,  silent=False):
     matrix = get_test_some_zero_matrix(n, prime=191)
 
-    bg = convert_small_to_big(matrix, 't2')
+    bg = convert_small_to_big(matrix, 't2' , threshold=threshold)
 
     bg_inv_kontrol = bg.sp_inverse()
     if not silent:
         display_matrix_ozet(matrix, 'bg_inv_kontrol')
         display_matrix_ozet(bg_inv_kontrol, 'bg_inv_kontrol')
 
     return MatrixOps("sp_inverse_t1", matrix, bg_inv_kontrol)
 
 
 def sp_inverse_mappings_t1(n, silent=False):
     matrix = get_test_some_zero_matrix(n, prime=191)
-    bg = convert_small_to_big(matrix, 't2')
+    bg = convert_small_to_big(matrix, 't3' , threshold=50 )
     mapping = create_mapping(matrix)
     # print(mapping)
     bg_inv = bg.sp_inverse_with_mappings(mapping)
     if not silent:
         display_matrix_ozet(matrix, 'matrix')
         display_matrix_ozet(bg_inv, 'bg_inv_kontrol')
```

## inverse/src/utils/pickle_works.py

```diff
@@ -1,9 +1,11 @@
+import functools
 import os
 import pickle
+from typing import Any
 
 from inverse.src.utils.inverse_typings import *
 
 pickle_folder = "./pickles2"
 pickle_folder_path = Path(pickle_folder)
 if not pickle_folder_path.is_dir():
     os.makedirs(pickle_folder_path)
@@ -25,7 +27,35 @@
             new_data = pickle.load(f)
         return new_data
 
     @staticmethod
     def save_pickle(key: str, data: list_tuple) -> None:
         with open(Pickles.name_format(key), 'wb') as f:
             pickle.dump(data, f)
+
+
+def sterialize(string):
+    import re
+    return re.sub('\W+', '', string)
+
+
+def sp_cache(
+        func: Callable[..., Any]
+
+) -> Callable[..., Any]:
+    @functools.wraps(func)
+    def wrapper(*args: Any, **kwargs: Any) -> Any:
+        key = f"{func.__name__}{args}{kwargs}"
+        key = sterialize(key)
+        print('=' * 20)
+        print('CHECKING', key)
+        print('=' * 20)
+        if Pickles.check_pickle(key):
+            return Pickles.read_pickle(key)
+
+        value = func(*args, **kwargs)
+        Pickles.save_pickle(key, value)
+
+        # logger.info(f"Finished {func.__name__}")
+        return value
+
+    return wrapper
```

## inverse/src/utils/tuple_for_buffer.py

```diff
@@ -1,9 +1,7 @@
-from functools import lru_cache
-
 from inverse.src.utils.inverse_typings import *
 
 bulk_ = []
 big_bulk = []
 
 
 def number_gen(n) -> Iterable:
@@ -13,18 +11,19 @@
 
 def number_gen_x(n) -> Iterable:
     x = 0
     while x < n:
         yield x
         x += 1
 
+
 def get_tuple_for_buffer(n: int, threshold: int) -> tuple:
     big_list = []
     liste = []
-    for x in number_gen_x(n + 1):
+    for x in number_gen_x(n):
         if liste:
             big_list.append(liste)
         liste = [x]
         for y in number_gen(n):
             _, *new_items = liste
             if not new_items or max(new_items) < y:
                 liste.append(y)
@@ -34,15 +33,15 @@
     return tuple(big_list)
 
 
 # @lru_cache(maxsize=128, typed=False)
 def get_tuple_for_buffer_eski(n: int, threshold: int) -> tuple:
     big_list = []
     liste = []
-    for x in number_gen_x(n + 1):
+    for x in number_gen_x(n ):
         if liste:
             big_list.append(liste)
         liste = [x]
         for y in number_gen(n):
             _, *new_items = liste
             if not new_items or max(new_items) < y:
                 liste.append(y)
```

## Comparing `inverse/src/classes/_logger.py` & `inverse/src/loggers/_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,7 +20,8 @@
     # stream_handler = logging.StreamHandler(sys.stderr)
     # stream_handler.setFormatter(logging.Formatter(fmt=logformat, datefmt=datefmt))
 
     logger = logging.getLogger(name)
     # logger.addHandler(stream_handler)
 
     return logger
+
```

## Comparing `inverse/tests/mini_tests.py` & `inverse/tests/test_mini_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from inverse.src.classes.buffer_ops import get_table_names_from_tuple
 from inverse.src.utils.partition import get_table_name_treshold
 from inverse.src.utils.sp_utils_inverse import close_two_matrices, close_identity
 from inverse.src.utils.tuple_for_buffer import get_tuple_for_buffer
 from inverse.tests.tdisplay import tdisplay
 
 
-# pytest ./tests/tests_main.py -W ignore::DeprecationWarning -v
+# pytest ./tests/test_main.py -W ignore::DeprecationWarning -v
 
 # pytest -W ignore::DeprecationWarning
 
 # def test_inverse_random_matrix(capsys):
 #    with capsys.disabled():
 #        inverse_random_matrix(5, 50)
 #       inverse_random_matrix(4, 12)
```

## Comparing `inverse-0.0.7.dist-info/LICENSE` & `inverse-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `inverse-0.0.7.dist-info/METADATA` & `inverse-0.0.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inverse
-Version: 0.0.7
+Version: 0.0.8
 Summary: large matrix operations
 Home-page: https://github.com/SermetPekin/inverse-repo
 License: MIT
 Author: Sermet Pekin
 Author-email: sermet.pekin@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `inverse-0.0.7.dist-info/RECORD` & `inverse-0.0.8.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -7,87 +7,98 @@
 inverse/ctypes_loc/clib.c,sha256=ZbXX1ZfeKbOxn_8iZlkvGJHKwM8ezJcvoYHykjBJNis,216
 inverse/ctypes_loc/clibSHARED.so,sha256=ZH5iljosNtAxjUMpBPcuZII-UmrblyzBCX6S0ZAEZy4,16232
 inverse/ctypes_loc/clibrary.so,sha256=Fo6aTkdnq-AC9no5Kvy6XRzTuli-xoIjogSnWN8d3eE,222942
 inverse/ctypes_loc/ctypes_class.py,sha256=qe6zPJE-8SdFH5lUj_fiTAdiYtL6z7QPsTTAUYI8nbs,5342
 inverse/ctypes_loc/ctypes_class_float.py,sha256=g9lEeiuveMYSqU87nv38Gz0c6qLk0RVdE87EjNOrBFc,2311
 inverse/ctypes_loc/deneme_sum.py,sha256=I0iJ6syK67d_nypYRL-NUICH3jnPsPNN2wVI_IRhn2k,468
 inverse/ctypes_loc/deneme_vector.py,sha256=9ZwnNmIAU1sLeh23TEDUfRnyuiAOGKb9awbqJjN15Z8,621
-inverse/ctypes_loc/get_c_loc.py,sha256=gfjXYX7i0Jxsjr2YWFvSM9S3OCdfXnC0hmGUPktctrg,1238
+inverse/ctypes_loc/get_c_loc.py,sha256=6_SVBnQDOygsdfT8zodnHnw63q85gHloDvkFDwSlTpU,1134
 inverse/ctypes_loc/lu_comp.c,sha256=GPHLECe_E5ZaTdBV_SqP-oW3-qNwkIf1Jso5XEGASCo,1687
 inverse/ctypes_loc/restats,sha256=qheIht1WUJS0hO9Il7y09cnznfuQV36XjVfQ3XjH4sk,5683
 inverse/ctypes_loc/sum.c,sha256=aRJhYiGgb3DTjYafO3bH7skERGIUOobHzphU4eEdTag,445
 inverse/ctypes_loc/vector_ops,sha256=_EhO2UKKg21ffcneD6A09o_jht52vll4LpexsZnL9Bg,16912
 inverse/ctypes_loc/vector_ops.c,sha256=eK8TIbw19cmj--bmhwC2SgNMouY7s1BMerwTM_PXpso,2332
 inverse/ctypes_loc/vector_ops.so,sha256=3Cg-A2jsY6fPXf9VzlK5NdIaVuz0AupsPLa6cOlzBss,91050
 inverse/ctypes_loc/vector_ops2.so,sha256=eKwvvSTXSvcWRl8b77s0xlrcGzMh8zs5314JjDJpnIM,224109
 inverse/ctypes_loc/vector_opsMAC,sha256=jsaLg8d3PgrFXZdOkp5uukkJK7877zWjuQABM-DpI_s,33818
 inverse/ctypes_loc/vector_opsSHARED.so,sha256=xSYQCRSvLS-v28S0-l_dQPCunAUo3Ye8vETanx9bVgc,16528
 inverse/src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inverse/src/benchmarks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-inverse/src/benchmarks/alternatives.py,sha256=1f-Vs_ywbPHryH83D-GHKEz2Jni1_uPe-TPyIvkvcVM,1973
+inverse/src/benchmarks/alternatives.py,sha256=xF9fqsBMgP8q7niSu78cEjd8DfzM-Tml-qUrfi-tInQ,2018
 inverse/src/benchmarks/vector_nonvector.py,sha256=T1nEc98RbAk3tw5oafy6LQ1l7johgf01oJdIlx-9BpI,599
 inverse/src/benchmarks/vector_ops_timeit.py,sha256=q1QmvcL2MxAbTZv8W9HB8X4qtKjpZnyS723QEx12O8k,191
 inverse/src/classes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-inverse/src/classes/_logger.py,sha256=fz82-0WQx_7alUMy5aPojXA9aUnWFerNnpNmbeLVRcU,789
 inverse/src/classes/abstract_data.py,sha256=8AWdwL6MUelSSHNMxm1Mnf8TrlgRpsbKyqk_R0oOJk8,2364
-inverse/src/classes/abstract_data2.py,sha256=rfvaVl0BBzdBCxuzZ88qXVUBluKQGr1uKDo_Aj47rlo,1965
-inverse/src/classes/buffer_ops.py,sha256=CDgpo0pAUEaYHJBWo0LJZdWcSYgkWzdz124MKPwiWVk,5706
+inverse/src/classes/abstract_data2.py,sha256=fbe0nS-PYgbAkkyayVmYFGsWVZBPqa9L7wB2_-cu5mk,1902
+inverse/src/classes/buffer_ops.py,sha256=Pl9Hx03lPtQI93LDBm3sYKfmnWlydZWCHCFMVfgqKPU,6279
 inverse/src/classes/buffer_ops_old_yedek.py,sha256=DzI0EfM0FNsRJmj7d0ZUJ4yFB8roDJxie99p1PAufzA,4021
 inverse/src/classes/db_ops.py,sha256=yKuWxvMmACrvV8zqmgQm6PUdDKGQ1DxX4L4rCe2ro9A,4177
 inverse/src/classes/randomMatrix.py,sha256=81Bjrq0VZz0osBGCtlzNevxvY7XrU92myBoWPJ7Of04,2584
-inverse/src/classes/random_sparse.py,sha256=tPewfYtkDgcNc-0HCyJ4IIKm3HKdDKPA0kQgosZt1ao,1184
+inverse/src/classes/random_sparse.py,sha256=L1E37VFpgo9ohMOyPHPiXP0uXldIPwTIDfHPf1oi1oE,1247
 inverse/src/classes/sp_matrix.py,sha256=Ejh55ebxvHESWCeSwy3cLW3DCDLGx3zg36BAX1C_Kk0,753
 inverse/src/engine/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inverse/src/engine/algos/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inverse/src/engine/algos/_mappings.py,sha256=wRO2sx0PnVoEQqHDlpORf4KU8UjbZsLBt7f2kjPbhsM,2028
-inverse/src/engine/algos/_progress.py,sha256=JrrOWAZwAoRogh7gZR3L-nL9zFLmt6-2V91hOsBm2Po,2220
-inverse/src/engine/algos/_spsparse.py,sha256=GF8YstMZ6bSLlXKngvW1h2c7RnhsougjyN1aTdQJws0,2032
-inverse/src/engine/algos/base_algo.py,sha256=2az6MLxoTfmHsvbwSoscMPWu53zmf8-QeH0Nfh6fHcg,5264
-inverse/src/engine/algos_save/_save_base.py,sha256=IYXLWTjGTWtDzBncZ6z8U_upX3-fJo31WArgS5Duu2E,707
-inverse/src/engine/algos_save/_save_sparse.py,sha256=hseAvkxezWYKvZJSXMMWCtm8jkVRHMBnYrBAeuSQF14,3973
+inverse/src/engine/algos/_progress.py,sha256=l-Ts8ubEf5u8Zw5N4ZSTAWDxPwT8OV683nMNGQk9gag,2237
+inverse/src/engine/algos/_progress_blast.py,sha256=_jO4_27LroCK_DyQgZIciuBIS9oGKaHiTbWQh4pT-Rg,2329
+inverse/src/engine/algos/_spsparse.py,sha256=1j-DO4AdXjVciSItMBr1mGnWxVwVQwtj6hC3P4LnjuA,2490
+inverse/src/engine/algos/_spsparse_blast.py,sha256=clrSdtWXqRQuIsENENKTUUN3LDnZvKAr4IKoPMM4YQo,1882
+inverse/src/engine/algos/_vector_ops.py,sha256=VQv-g161HNhNuOK348dRYOpxPUtG-oml3TisKFnOLdk,78
+inverse/src/engine/algos/base_algo.py,sha256=z7kANm5Eqfx1FeZk-y_hsqPqpIahteulPnD2HM6JWD8,5283
+inverse/src/engine/algos/benchmarks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+inverse/src/engine/algos/benchmarks/vector_ops_bench.py,sha256=JzWriBPL-bA10k7U4ITzGef4Kp0-uL3sXSpPzgTl-zE,790
+inverse/src/engine/algos_save/_save_base.py,sha256=lUr48MvFEODhZJ9Oc6-QZI2y_Q_RtBcZLb6qZxfnBN4,1315
+inverse/src/engine/algos_save/_save_sparse.py,sha256=TQRViJD33oWw84BJSCKlq96TURP33_rf9PJQFcbc0Ks,4534
 inverse/src/engine/base_classes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inverse/src/engine/base_classes/big_matrix_base.py,sha256=OKOmkAOAvfJviuQsqa13FP0L2X2gnFieNmqUaEgVdsg,367
 inverse/src/engine/main.py,sha256=sQ4cTO5FCvG3r6kY6UgLhHlRZlGuyFO0nshkpEXn4T8,1884
-inverse/src/engine/main_funcs_to_load.py,sha256=Iu74SAE9ihru6DMSdFJGoHqv_0lhykLwKnsviEZv4X8,2678
-inverse/src/engine/matrix_converters.py,sha256=iXEJpGAVqDIqwYI_GN9YNI1JMhDKuXaiYW31LsaWaiM,5833
-inverse/src/engine/nontest_test.py,sha256=5bHMvF7FqD9Hls6dFBlehbG3h5iQ3w5JWAUv7eOhuP4,2705
+inverse/src/engine/main_funcs_to_load.py,sha256=UPL-AP9zxJSiDXfMhF9Kf9lCuW5IWoSw9SRrfIshe_E,2677
+inverse/src/engine/matrix_converters.py,sha256=O5Qa02oS10QstApONSZFS7_9Ezhi8nq6THf5HjvFz3E,4380
+inverse/src/engine/nontest_test.py,sha256=Rpu9W3f9mRMEN31tO4wEuq9R6J3D60kCGk6j29rJroY,2763
 inverse/src/engine/sp_matrix_ops.py,sha256=_8L-OYJTLVfa6u3kiMG3qKOSgsV2niinMTxJY1s0lqw,3357
 inverse/src/large_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inverse/src/large_data/data_converters.py,sha256=yGlEge3y7bzQnIXWEHOz-c0ldOvZYtEWPpiaCMICeDY,467
+inverse/src/loggers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+inverse/src/loggers/_logger.py,sha256=IglHV2MkswZEM5Ok6awmmMpPKOfSRN1SuTL6lsDpP2E,790
+inverse/src/loggers/_logger3.py,sha256=V9QftNCW8v1PldB31iIe39Iihvw5m9tSoHR0UCISvDA,2087
 inverse/src/optimizations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inverse/src/optimizations/optimizations_when.py,sha256=CSctIKluqjlkHwSTYyd0FdONcifNTZowc9LgT2ME9Os,2912
 inverse/src/optimizations/quick_funcs.py,sha256=jlgGbENZa6duHtNTytj1i4zDtXZfjuyCLasJb85K-cI,958
+inverse/src/sp_utils/_logger3.py.lib,sha256=goebjWxFTYkritwz7KvoQ7z8iuoi0kR6aVpi6lJgPdI,1884
+inverse/src/sp_utils/pickle_works.py.lib,sha256=XId7wFEceL0l6ZH7n0VUtzWvzHHwnBFm4fRvM3jxVrA,1503
 inverse/src/testing_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inverse/src/testing_utils/timeit_sp.py,sha256=bEJkoqtSWYAyOaEowPWgCY40ACMz_zLgeWZO78lI3IM,412
 inverse/src/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inverse/src/utils/check_result.py,sha256=rWW7xVX7BvYK4K0ahrpN_TemKCx8Na7bKIPSKNhPEi0,87
 inverse/src/utils/initial_checks_matrix.py,sha256=4XNbGbkl_nsq-8SbNevP8GS7kgKByGtGUIi78Ifp-jM,39
 inverse/src/utils/inverse_typings.py,sha256=5143ePC4-VAa8jD1RykK0BZZ6U0f9KD1cEpwxm9IMMc,292
 inverse/src/utils/measure_calls.py,sha256=GHDJtiTHdNojasGaXtlFj7_qk8L98kKgWKn-7HwsLQ8,83
 inverse/src/utils/opening_logo.py,sha256=CGGyE4F3Mk86fd774e-LWjcYF4x2MWeF-jmL3xwVZis,283
 inverse/src/utils/partition.py,sha256=DDJPdspbCGpQFP41xYW7I7e7OG0bK_tsB6XlKvtvouY,547
 inverse/src/utils/pickle_file.py,sha256=Y-qZcfDSLlK1pp1du9C5tPDUD1YUux6g96EgrmDWIB8,474
-inverse/src/utils/pickle_works.py,sha256=qosB5zp1-ED1guCUY1LqlPVnNfLcJYKOO_lqiqWLR3E,823
+inverse/src/utils/pickle_works.py,sha256=XId7wFEceL0l6ZH7n0VUtzWvzHHwnBFm4fRvM3jxVrA,1503
 inverse/src/utils/sp_general_utils.py,sha256=TnJ4IsqDoBPsBCAWs1iY7ARUvFRjTinnLL_IIlVRVC4,174
 inverse/src/utils/sp_utils_inverse.py,sha256=pc-sXmXbMHOJCdkXtE0fenEFnuqL3Ta5wkeKJyvTCqU,3501
 inverse/src/utils/sure.py,sha256=Kk35oo9l9ApPCixWowyYY8nuarfyG0wEmiabDLXvgsQ,285
-inverse/src/utils/tuple_for_buffer.py,sha256=J1VpWpeHlq8EXLx4iDBF9fs05OoVIYa3rBDACFxdAsU,1283
+inverse/src/utils/tuple_for_buffer.py,sha256=mLMm59vsZXaidUbx64Fuhq0Rs2xN3ktdd0pzo6n9H7U,1244
 inverse/src/utils/tuple_for_buffer.pyx,sha256=r7RKiHoDsOX70P11bGflR5IOkvHnJe7kabPAxwA33Js,1342
 inverse/src/vector_ops/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inverse/src/vector_ops/d1.py,sha256=yN2vy94KSR1S6eWiX8oL2QgHHRWMhMr8s5YRK1SRfpA,1063
 inverse/tests/__init__.py,sha256=xlJkcGJcQJnu_uuFCoRI6IqNL_9Y7F3Up4X0tIo5Z10,46
 inverse/tests/c_tests2/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inverse/tests/c_tests2/c_tests.py,sha256=4NsCr0LOEw0iWMVRWPZJg-XTLBlUrTTJXYzuZAwwQJ8,1139
 inverse/tests/main_test.py,sha256=oY4xUmOGJUo5_j7sZMDUvox2gTsKista2GtkZ4RWzCg,660
-inverse/tests/mini_tests.py,sha256=F4FDPg2b9Eg3mwTj4gNElcF66X-isASuJuDh8NnGfFQ,3631
 inverse/tests/tdisplay.py,sha256=yyHHqa77rOaXL8v066gFbZaLLpdIyFsMUxtU88cects,173
 inverse/tests/test_alternatives.py,sha256=S0TI_VUUWgQJm-O-U20xxBKyb9Ap1KqtT8l-_x5CILI,262
+inverse/tests/test_classes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inverse/tests/test_classes/test_buffer.py,sha256=Gs-ocFzgOtOGMRyaZ7owfqGjGI0DzkDK7tYEE1deYoM,206
 inverse/tests/test_inverse_matrices/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 inverse/tests/test_inverse_matrices/test_some.py,sha256=8rGE5qC9Sapy3nK6B8ikjWC8HL-NRnDsqJtXIdYJWNs,1300
+inverse/tests/test_inverse_matrices/test_sparse_inverse.py,sha256=DkLIE5Zpn2OQU9bVAgpzNYh8QCcI7r231VMdlE6GZzw,715
+inverse/tests/test_main.py,sha256=F3q6UOEIB90I_g5CYhIDlhiXhxnPUspfUaHnzQETTNI,421
 inverse/tests/test_matrix_op_main.py,sha256=ZiR4oAXV27kmZhimNhs4Xfyru4a6zMf633u5uSs9SXg,1443
+inverse/tests/test_mini_tests.py,sha256=FTES-jBIJ2QH5APyMCsKLhAG2DbbwrQjfmmQdhcOcHQ,3630
 inverse/tests/tests.py,sha256=QV1Gv33kfsqCxGlAAIMVucTopTnAu6fj8lQw8wfw9is,1548
-inverse/tests/tests_main.py,sha256=gRM8OVzbrDraZsPCshh74KTZFz_BTccWaoRCAoVVVC4,435
-inverse-0.0.7.dist-info/LICENSE,sha256=HfUG_pNgR_KESlLAy_oG9ttnqf9XDmCmIHrtkXICRlE,1069
-inverse-0.0.7.dist-info/METADATA,sha256=Hu8UwnLBsB3DvBLykxNsIggnHHhdtGZ6DqslfTh-jI8,2327
-inverse-0.0.7.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-inverse-0.0.7.dist-info/RECORD,,
+inverse-0.0.8.dist-info/LICENSE,sha256=HfUG_pNgR_KESlLAy_oG9ttnqf9XDmCmIHrtkXICRlE,1069
+inverse-0.0.8.dist-info/METADATA,sha256=nhgnPo00VVe9vhU8lZ3HXkAHxbphj2wV141T_2PPzHo,2327
+inverse-0.0.8.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+inverse-0.0.8.dist-info/RECORD,,
```

