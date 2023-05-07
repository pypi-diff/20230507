# Comparing `tmp/qlat-0.8.tar.gz` & `tmp/qlat-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlat-0.8.tar", last modified: Sun Nov 27 17:51:20 2022, max compression
+gzip compressed data, was "qlat-0.9.tar", last modified: Sat Dec 10 16:32:15 2022, max compression
```

## Comparing `qlat-0.8.tar` & `qlat-0.9.tar`

### file list

```diff
@@ -1,210 +1,215 @@
--rw-rw-r--   0        0        0    35092 1970-01-01 00:00:00.000000 qlat-0.8/LICENSE
--rw-rw-r--   0        0        0       42 1970-01-01 00:00:00.000000 qlat-0.8/README.md
--rwxrwxr-x   0        0        0      293 1970-01-01 00:00:00.000000 qlat-0.8/bin/eigen-system-checksum
--rwxrwxr-x   0        0        0      531 1970-01-01 00:00:00.000000 qlat-0.8/bin/eigen-system-repartition
--rwxrwxr-x   0        0        0      269 1970-01-01 00:00:00.000000 qlat-0.8/bin/fields-checksum
--rwxrwxr-x   0        0        0      322 1970-01-01 00:00:00.000000 qlat-0.8/bin/fields-list
--rwxrwxr-x   0        0        0     2398 1970-01-01 00:00:00.000000 qlat-0.8/bin/gauge-fix-coulomb
--rwxrwxr-x   0        0        0       92 1970-01-01 00:00:00.000000 qlat-0.8/bin/qlat-include
--rwxrwxr-x   0        0        0     1177 1970-01-01 00:00:00.000000 qlat-0.8/bin/topo-measure
--rw-rw-r--   0        0        0       50 1970-01-01 00:00:00.000000 qlat-0.8/include/meson.build
--rw-rw-r--   0        0        0    61945 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/compressed-eigen-io.h
--rw-rw-r--   0        0        0       43 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/config.h
--rw-rw-r--   0        0        0    25309 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/contract-field.h
--rw-rw-r--   0        0        0     1950 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/contract-hvp.h
--rw-rw-r--   0        0        0    23687 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/contract-pion.h
--rw-rw-r--   0        0        0     6729 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/contract-wall-src-prop.h
--rw-rw-r--   0        0        0     3659 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/coordinate-d.h
--rw-r--r--   0        0        0     4018 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/coordinate.h
--rw-rw-r--   0        0        0    36314 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/core.h
--rw-r--r--   0        0        0     3022 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/cps-lanc.h
--rw-r--r--   0        0        0    13273 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/cps-pio.h
--rw-r--r--   0        0        0    21932 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/cps-utils.h
--rw-r--r--   0        0        0    13466 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/cps.h
--rw-rw-r--   0        0        0    58314 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/dslash.h
--rw-r--r--   0        0        0     2322 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/fermion-action.h
--rw-rw-r--   0        0        0    13448 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/field-comm.h
--rw-rw-r--   0        0        0    22077 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/field-dist-io.h
--rw-rw-r--   0        0        0    22303 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/field-expand.h
--rw-rw-r--   0        0        0     6788 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/field-fft.h
--rw-rw-r--   0        0        0    11693 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/field-io.h
--rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/field-rng.h
--rw-rw-r--   0        0        0    21013 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/field-serial-io.h
--rw-rw-r--   0        0        0    57816 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/field-shuffle.h
--rw-rw-r--   0        0        0    25471 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/field-utils.h
--rw-rw-r--   0        0        0     4100 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/field.h
--rw-rw-r--   0        0        0    57183 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/fields-io.h
--rw-r--r--   0        0        0      426 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/gauge-action.h
--rw-rw-r--   0        0        0      683 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/geometry.h
--rw-rw-r--   0        0        0    12987 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/grid.h
--rw-rw-r--   0        0        0    10155 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/hmc-stats.h
--rw-rw-r--   0        0        0     9672 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/hmc.h
--rw-rw-r--   0        0        0    11678 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/matrix-hmc.h
--rw-rw-r--   0        0        0    23068 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/matrix.h
--rw-rw-r--   0        0        0      909 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/meson.build
--rw-rw-r--   0        0        0    30836 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/mpi.h
--rw-rw-r--   0        0        0     2113 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/mvector.h
--rw-rw-r--   0        0        0     7268 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/py_convert.h
--rw-r--r--   0        0        0    11844 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/qcd-gauge-transformation-boundary.h
--rw-rw-r--   0        0        0    12041 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/qcd-gauge-transformation.h
--rw-rw-r--   0        0        0    25191 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/qcd-prop.h
--rw-rw-r--   0        0        0    12372 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/qcd-smear.h
--rw-rw-r--   0        0        0    11596 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/qcd-topology.h
--rw-rw-r--   0        0        0    22242 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/qcd-utils.h
--rw-rw-r--   0        0        0    21363 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/qcd.h
--rw-rw-r--   0        0        0    13496 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/qed.h
--rw-r--r--   0        0        0    22559 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/qlat-analysis.h
--rw-r--r--   0        0        0    17080 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/qlat-setup.h
--rw-rw-r--   0        0        0     1412 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/qlat.h
--rw-r--r--   0        0        0    15925 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/quda.h
--rw-rw-r--   0        0        0    14891 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/scalar-action.h
--rw-rw-r--   0        0        0    27399 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/selected-field-io.h
--rw-rw-r--   0        0        0    26152 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/selected-field.h
--rw-rw-r--   0        0        0    13972 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/selected-points.h
--rw-r--r--   0        0        0      420 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/setup.h
--rw-rw-r--   0        0        0     4051 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/utils-coordinate.h
--rw-rw-r--   0        0        0    11502 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/utils-io.h
--rw-rw-r--   0        0        0     8650 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/check_fun.h
--rw-rw-r--   0        0        0    38808 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/general_funs.h
--rw-rw-r--   0        0        0    14168 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/quda_para.h
--rw-rw-r--   0        0        0     7013 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_COPY_data.h
--rw-rw-r--   0        0        0    31413 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_FFT_GPU.h
--rw-rw-r--   0        0        0    18370 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_Matrix_prod.h
--rw-rw-r--   0        0        0    17016 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_Vec_redistribute.h
--rw-rw-r--   0        0        0      826 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_construction.h
--rw-rw-r--   0        0        0    28150 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_corr_baryon.h
--rw-rw-r--   0        0        0    19921 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_corr_meson.h
--rw-rw-r--   0        0        0    20097 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_corr_prop.h
--rw-rw-r--   0        0        0    34079 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_eigensys.h
--rw-rw-r--   0        0        0    13986 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_fft_desc.h
--rw-rw-r--   0        0        0    10410 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_float_type.h
--rw-rw-r--   0        0        0     8331 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_gammas.h
--rw-rw-r--   0        0        0     1006 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_gaugefield.h
--rw-rw-r--   0        0        0    15587 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_grid_src.h
--rw-rw-r--   0        0        0    75526 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_io_vec.h
--rw-rw-r--   0        0        0    20158 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_lms_funs.h
--rw-rw-r--   0        0        0    34367 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_low_rho.h
--rw-rw-r--   0        0        0    15893 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_momentum.h
--rw-rw-r--   0        0        0    95090 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_quda_inverter.h
--rw-rw-r--   0        0        0    45346 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_read_txt.h
--rw-rw-r--   0        0        0     9137 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_reduce_vec.h
--rw-rw-r--   0        0        0    28978 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_shift_vecs.h
--rw-rw-r--   0        0        0    36685 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_smear_vecs.h
--rw-rw-r--   0        0        0     1606 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_stagger_contractions.h
--rw-rw-r--   0        0        0     1624 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_test_unified.h
--rw-rw-r--   0        0        0    11029 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/vector_utils/utils_vector_GPU.h
--rw-rw-r--   0        0        0     2931 1970-01-01 00:00:00.000000 qlat-0.8/include/qlat/wilson-flow.h
--rw-rw-r--   0        0        0     1945 1970-01-01 00:00:00.000000 qlat-0.8/meson.build
--rw-rw-r--   0        0        0      213 1970-01-01 00:00:00.000000 qlat-0.8/meson_options.txt
--rw-rw-r--   0        0        0       43 1970-01-01 00:00:00.000000 qlat-0.8/pylib/auto_contractor/README.md
--rw-rw-r--   0        0        0      509 1970-01-01 00:00:00.000000 qlat-0.8/pylib/auto_contractor/TODO.md
--rw-rw-r--   0        0        0     8113 1970-01-01 00:00:00.000000 qlat-0.8/pylib/auto_contractor/ama.py
--rw-rw-r--   0        0        0     3994 1970-01-01 00:00:00.000000 qlat-0.8/pylib/auto_contractor/benchmark.py
--rw-rw-r--   0        0        0    40181 1970-01-01 00:00:00.000000 qlat-0.8/pylib/auto_contractor/compile.py
--rw-rw-r--   0        0        0    10715 1970-01-01 00:00:00.000000 qlat-0.8/pylib/auto_contractor/eval.py
--rw-rw-r--   0        0        0     3584 1970-01-01 00:00:00.000000 qlat-0.8/pylib/auto_contractor/eval_sc_qlat.py
--rw-rw-r--   0        0        0     6589 1970-01-01 00:00:00.000000 qlat-0.8/pylib/auto_contractor/expr_arithmetic.py
--rw-rw-r--   0        0        0      183 1970-01-01 00:00:00.000000 qlat-0.8/pylib/auto_contractor/meson.build
--rw-rw-r--   0        0        0    55109 1970-01-01 00:00:00.000000 qlat-0.8/pylib/auto_contractor/operators.py
--rw-rw-r--   0        0        0     1382 1970-01-01 00:00:00.000000 qlat-0.8/pylib/auto_contractor/runtime.py
--rw-rw-r--   0        0        0    46986 1970-01-01 00:00:00.000000 qlat-0.8/pylib/auto_contractor/simulation.py
--rw-rw-r--   0        0        0    23041 1970-01-01 00:00:00.000000 qlat-0.8/pylib/auto_contractor/wick.py
--rw-rw-r--   0        0        0      535 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/contraction-field.cpp
--rw-rw-r--   0        0        0      679 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/contraction-hvp.cpp
--rw-rw-r--   0        0        0      888 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/contraction-pion.cpp
--rw-rw-r--   0        0        0     1661 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/coordinate.cpp
--rw-rw-r--   0        0        0    12850 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/exports.h
--rw-rw-r--   0        0        0     2800 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/fermion-action.cpp
--rw-rw-r--   0        0        0     4445 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/field-double.cpp
--rw-rw-r--   0        0        0     4034 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/field-io.cpp
--rw-rw-r--   0        0        0    11083 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/field-selection.cpp
--rw-rw-r--   0        0        0    22526 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/field-utils.cpp
--rw-rw-r--   0        0        0    12813 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/field.cpp
--rw-rw-r--   0        0        0     9373 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/fields-io.cpp
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/gauge-action.cpp
--rw-rw-r--   0        0        0     6667 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/geometry.cpp
--rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/hmc-stats.cpp
--rw-rw-r--   0        0        0     1915 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/hmc.cpp
--rw-rw-r--   0        0        0     1573 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/init.cpp
--rw-rw-r--   0        0        0     3066 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/inverter.cpp
--rw-rw-r--   0        0        0      482 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/lat-io.cpp
--rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/lib.cpp
--rw-rw-r--   0        0        0     2225 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/lib.h
--rw-rw-r--   0        0        0     7995 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/mat.cpp
--rw-rw-r--   0        0        0      369 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/meson.build
--rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/mpi.cpp
--rw-rw-r--   0        0        0     8646 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/propagator.cpp
--rw-rw-r--   0        0        0     8060 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/qcd.cpp
--rw-rw-r--   0        0        0     6901 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/scalar-action.cpp
--rw-rw-r--   0        0        0    23483 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/selected-field.cpp
--rw-rw-r--   0        0        0    17537 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/selected-points.cpp
--rw-rw-r--   0        0        0     2639 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/smear.cpp
--rw-rw-r--   0        0        0     1775 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/topology.cpp
--rwxr-xr-x   0        0        0      766 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/update.sh
--rw-rw-r--   0        0        0     7440 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/utils-io.cpp
--rw-rw-r--   0        0        0      590 1970-01-01 00:00:00.000000 qlat-0.8/pylib/cqlat/wilson-flow.cpp
--rw-rw-r--   0        0        0      241 1970-01-01 00:00:00.000000 qlat-0.8/pylib/meson.build
--rw-rw-r--   0        0        0      795 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/__init__.py
--rw-rw-r--   0        0        0      175 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/c.py
--rw-rw-r--   0        0        0      247 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/contract_field.py
--rw-rw-r--   0        0        0      219 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/contract_hvp.py
--rw-rw-r--   0        0        0      377 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/contract_pion.py
--rw-rw-r--   0        0        0      687 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/coordinate.py
--rw-rw-r--   0        0        0     1086 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/fermion_action.py
--rw-rw-r--   0        0        0    15422 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/field.py
--rw-rw-r--   0        0        0     1312 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/field_double.py
--rw-rw-r--   0        0        0     6179 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/field_selection.py
--rw-rw-r--   0        0        0     4550 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/field_utils.py
--rw-rw-r--   0        0        0     6344 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/fields_io.py
--rw-rw-r--   0        0        0      491 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/gauge_action.py
--rw-rw-r--   0        0        0     3684 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/geometry.py
--rw-rw-r--   0        0        0      234 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/get_include_dir.py
--rw-rw-r--   0        0        0     1160 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/hmc.py
--rw-rw-r--   0        0        0      671 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/hmc_stats.py
--rw-rw-r--   0        0        0     3378 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/inverter.py
--rw-rw-r--   0        0        0     4955 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/mat.py
--rw-rw-r--   0        0        0      172 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/meson.build
--rw-rw-r--   0        0        0     1540 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/mpi.py
--rw-rw-r--   0        0        0     6732 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/propagator.py
--rw-rw-r--   0        0        0     5215 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/qcd.py
--rw-rw-r--   0        0        0     3348 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/scalar_action.py
--rw-rw-r--   0        0        0    10295 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/selected_field.py
--rw-rw-r--   0        0        0     6050 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/selected_points.py
--rw-rw-r--   0        0        0     1198 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/smear.py
--rw-rw-r--   0        0        0     3444 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/topology.py
--rw-rw-r--   0        0        0      330 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/utils.py
--rw-rw-r--   0        0        0      573 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/utils_io.py
--rw-rw-r--   0        0        0     1593 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat/wilson_flow.py
--rw-rw-r--   0        0        0    21037 1970-01-01 00:00:00.000000 qlat-0.8/pylib/qlat_gpt.py
--rw-rw-r--   0        0        0    14723 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd.py
--rw-rw-r--   0        0        0      919 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/__init__.py
--rw-rw-r--   0        0        0      184 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/meson.build
--rw-rw-r--   0        0        0     2702 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_16IH2.py
--rw-rw-r--   0        0        0     4397 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_24D.py
--rw-rw-r--   0        0        0     4394 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_24DH.py
--rw-rw-r--   0        0        0     1912 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_24IH01.py
--rw-rw-r--   0        0        0     1209 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_24IH02.py
--rw-rw-r--   0        0        0     1213 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_24IH03.py
--rw-rw-r--   0        0        0     1965 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_24IH04.py
--rw-rw-r--   0        0        0     1961 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_24IH05.py
--rw-rw-r--   0        0        0     3542 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_24IH1.py
--rw-rw-r--   0        0        0     3541 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_24IH2.py
--rw-rw-r--   0        0        0     3541 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_24IH3.py
--rw-rw-r--   0        0        0     3541 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_24IH4.py
--rw-rw-r--   0        0        0     1662 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_32D.py
--rw-rw-r--   0        0        0     2717 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_32Dfine.py
--rw-rw-r--   0        0        0     1124 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_32IH01.py
--rw-rw-r--   0        0        0     3540 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_32IH1.py
--rw-rw-r--   0        0        0     3540 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_32IH2.py
--rw-rw-r--   0        0        0     3540 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_32IH3.py
--rw-rw-r--   0        0        0     1919 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_32IcoarseH01.py
--rw-rw-r--   0        0        0     1915 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_32IcoarseH02.py
--rw-rw-r--   0        0        0     3551 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_32IcoarseH1.py
--rw-rw-r--   0        0        0     3551 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_32IfineH.py
--rw-rw-r--   0        0        0     1909 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_48I.py
--rw-rw-r--   0        0        0     1122 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_64I.py
--rw-rw-r--   0        0        0      285 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_96I.py
--rw-rw-r--   0        0        0     3926 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/p_test.py
--rw-rw-r--   0        0        0     1473 1970-01-01 00:00:00.000000 qlat-0.8/pylib/rbc_ukqcd_params/utils.py
--rw-rw-r--   0        0        0      405 1970-01-01 00:00:00.000000 qlat-0.8/pyproject.toml
--rw-r--r--   0        0        0      271 1970-01-01 00:00:00.000000 qlat-0.8/PKG-INFO
+-rw-rw-r--   0        0        0    35092 1970-01-01 00:00:00.000000 qlat-0.9/LICENSE
+-rw-rw-r--   0        0        0       42 1970-01-01 00:00:00.000000 qlat-0.9/README.md
+-rwxrwxr-x   0        0        0      293 1970-01-01 00:00:00.000000 qlat-0.9/bin/eigen-system-checksum
+-rwxrwxr-x   0        0        0      531 1970-01-01 00:00:00.000000 qlat-0.9/bin/eigen-system-repartition
+-rwxrwxr-x   0        0        0      269 1970-01-01 00:00:00.000000 qlat-0.9/bin/fields-checksum
+-rwxrwxr-x   0        0        0      322 1970-01-01 00:00:00.000000 qlat-0.9/bin/fields-list
+-rwxrwxr-x   0        0        0     2398 1970-01-01 00:00:00.000000 qlat-0.9/bin/gauge-fix-coulomb
+-rwxrwxr-x   0        0        0       92 1970-01-01 00:00:00.000000 qlat-0.9/bin/qlat-include
+-rwxrwxr-x   0        0        0     1177 1970-01-01 00:00:00.000000 qlat-0.9/bin/topo-measure
+-rw-rw-r--   0        0        0       50 1970-01-01 00:00:00.000000 qlat-0.9/include/meson.build
+-rw-rw-r--   0        0        0    61945 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/compressed-eigen-io.h
+-rw-rw-r--   0        0        0       43 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/config.h
+-rw-rw-r--   0        0        0    25309 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/contract-field.h
+-rw-rw-r--   0        0        0     1950 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/contract-hvp.h
+-rw-rw-r--   0        0        0    23687 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/contract-pion.h
+-rw-rw-r--   0        0        0     6729 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/contract-wall-src-prop.h
+-rw-rw-r--   0        0        0     3659 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/coordinate-d.h
+-rw-r--r--   0        0        0     4018 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/coordinate.h
+-rw-rw-r--   0        0        0    36314 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/core.h
+-rw-r--r--   0        0        0     3022 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/cps-lanc.h
+-rw-r--r--   0        0        0    13273 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/cps-pio.h
+-rw-r--r--   0        0        0    21932 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/cps-utils.h
+-rw-r--r--   0        0        0    13466 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/cps.h
+-rw-rw-r--   0        0        0    58314 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/dslash.h
+-rw-r--r--   0        0        0     2322 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/fermion-action.h
+-rw-rw-r--   0        0        0    13448 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/field-comm.h
+-rw-rw-r--   0        0        0    22077 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/field-dist-io.h
+-rw-rw-r--   0        0        0    22303 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/field-expand.h
+-rw-rw-r--   0        0        0     6788 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/field-fft.h
+-rw-rw-r--   0        0        0    11693 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/field-io.h
+-rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/field-rng.h
+-rw-rw-r--   0        0        0    21013 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/field-serial-io.h
+-rw-rw-r--   0        0        0    57816 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/field-shuffle.h
+-rw-rw-r--   0        0        0    25471 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/field-utils.h
+-rw-rw-r--   0        0        0     4100 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/field.h
+-rw-rw-r--   0        0        0    57183 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/fields-io.h
+-rw-r--r--   0        0        0      426 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/gauge-action.h
+-rw-rw-r--   0        0        0      683 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/geometry.h
+-rw-rw-r--   0        0        0    12987 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/grid.h
+-rw-rw-r--   0        0        0    10155 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/hmc-stats.h
+-rw-rw-r--   0        0        0     9672 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/hmc.h
+-rw-rw-r--   0        0        0    11678 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/matrix-hmc.h
+-rw-rw-r--   0        0        0    23068 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/matrix.h
+-rw-rw-r--   0        0        0      909 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/meson.build
+-rw-rw-r--   0        0        0    30836 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/mpi.h
+-rw-rw-r--   0        0        0     2113 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/mvector.h
+-rw-rw-r--   0        0        0     7268 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/py_convert.h
+-rw-r--r--   0        0        0    11844 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/qcd-gauge-transformation-boundary.h
+-rw-rw-r--   0        0        0    12041 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/qcd-gauge-transformation.h
+-rw-rw-r--   0        0        0    25191 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/qcd-prop.h
+-rw-rw-r--   0        0        0    12372 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/qcd-smear.h
+-rw-rw-r--   0        0        0    11596 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/qcd-topology.h
+-rw-rw-r--   0        0        0    22242 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/qcd-utils.h
+-rw-rw-r--   0        0        0    21363 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/qcd.h
+-rw-rw-r--   0        0        0    13496 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/qed.h
+-rw-r--r--   0        0        0    22559 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/qlat-analysis.h
+-rw-r--r--   0        0        0    17080 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/qlat-setup.h
+-rw-rw-r--   0        0        0     1412 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/qlat.h
+-rw-r--r--   0        0        0    15925 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/quda.h
+-rw-rw-r--   0        0        0    14891 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/scalar-action.h
+-rw-rw-r--   0        0        0    27399 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/selected-field-io.h
+-rw-rw-r--   0        0        0    26152 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/selected-field.h
+-rw-rw-r--   0        0        0    13972 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/selected-points.h
+-rw-r--r--   0        0        0      420 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/setup.h
+-rw-rw-r--   0        0        0     4051 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/utils-coordinate.h
+-rw-rw-r--   0        0        0    11502 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/utils-io.h
+-rw-rw-r--   0        0        0     9487 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/check_fun.h
+-rw-rw-r--   0        0        0    28221 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/general_funs.h
+-rw-rw-r--   0        0        0    14200 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/quda_para.h
+-rw-rw-r--   0        0        0     7542 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_COPY_data.h
+-rw-rw-r--   0        0        0    31572 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_FFT_GPU.h
+-rw-rw-r--   0        0        0    18370 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_Matrix_prod.h
+-rw-rw-r--   0        0        0    17016 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_Vec_redistribute.h
+-rw-rw-r--   0        0        0      936 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_construction.h
+-rw-rw-r--   0        0        0    34067 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_corr_baryon.h
+-rw-rw-r--   0        0        0    25656 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_corr_meson.h
+-rw-rw-r--   0        0        0    29262 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_corr_prop.h
+-rw-rw-r--   0        0        0    33789 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_eigensys.h
+-rw-rw-r--   0        0        0    14267 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_fft_desc.h
+-rw-rw-r--   0        0        0    10708 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_float_type.h
+-rw-rw-r--   0        0        0     8331 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_gammas.h
+-rw-rw-r--   0        0        0     1049 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_gaugefield.h
+-rw-rw-r--   0        0        0    18319 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_grid_src.h
+-rw-rw-r--   0        0        0    70142 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_io_vec.h
+-rw-rw-r--   0        0        0    16855 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_lms_funs.h
+-rw-rw-r--   0        0        0    34367 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_low_rho.h
+-rw-rw-r--   0        0        0    15893 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_momentum.h
+-rw-rw-r--   0        0        0    12076 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_mpi.h
+-rw-rw-r--   0        0        0    97811 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_quda_inverter.h
+-rw-rw-r--   0        0        0    45272 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_read_txt.h
+-rw-rw-r--   0        0        0     9137 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_reduce_vec.h
+-rw-rw-r--   0        0        0    28978 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_shift_vecs.h
+-rw-rw-r--   0        0        0    36818 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_smear_vecs.h
+-rw-rw-r--   0        0        0     1499 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_stagger_contractions.h
+-rw-rw-r--   0        0        0     1624 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_test_unified.h
+-rw-rw-r--   0        0        0    11029 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/vector_utils/utils_vector_GPU.h
+-rw-rw-r--   0        0        0     2931 1970-01-01 00:00:00.000000 qlat-0.9/include/qlat/wilson-flow.h
+-rw-rw-r--   0        0        0     2001 1970-01-01 00:00:00.000000 qlat-0.9/meson.build
+-rw-rw-r--   0        0        0      213 1970-01-01 00:00:00.000000 qlat-0.9/meson_options.txt
+-rw-rw-r--   0        0        0       43 1970-01-01 00:00:00.000000 qlat-0.9/pylib/auto_contractor/README.md
+-rw-rw-r--   0        0        0      509 1970-01-01 00:00:00.000000 qlat-0.9/pylib/auto_contractor/TODO.md
+-rw-rw-r--   0        0        0     8113 1970-01-01 00:00:00.000000 qlat-0.9/pylib/auto_contractor/ama.py
+-rw-rw-r--   0        0        0     3994 1970-01-01 00:00:00.000000 qlat-0.9/pylib/auto_contractor/benchmark.py
+-rw-rw-r--   0        0        0    40181 1970-01-01 00:00:00.000000 qlat-0.9/pylib/auto_contractor/compile.py
+-rw-rw-r--   0        0        0    10715 1970-01-01 00:00:00.000000 qlat-0.9/pylib/auto_contractor/eval.py
+-rw-rw-r--   0        0        0     3584 1970-01-01 00:00:00.000000 qlat-0.9/pylib/auto_contractor/eval_sc_qlat.py
+-rw-rw-r--   0        0        0     6589 1970-01-01 00:00:00.000000 qlat-0.9/pylib/auto_contractor/expr_arithmetic.py
+-rw-rw-r--   0        0        0      183 1970-01-01 00:00:00.000000 qlat-0.9/pylib/auto_contractor/meson.build
+-rw-rw-r--   0        0        0    55109 1970-01-01 00:00:00.000000 qlat-0.9/pylib/auto_contractor/operators.py
+-rw-rw-r--   0        0        0     1382 1970-01-01 00:00:00.000000 qlat-0.9/pylib/auto_contractor/runtime.py
+-rw-rw-r--   0        0        0    46986 1970-01-01 00:00:00.000000 qlat-0.9/pylib/auto_contractor/simulation.py
+-rw-rw-r--   0        0        0    23041 1970-01-01 00:00:00.000000 qlat-0.9/pylib/auto_contractor/wick.py
+-rw-rw-r--   0        0        0      535 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/contraction-field.cpp
+-rw-rw-r--   0        0        0      679 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/contraction-hvp.cpp
+-rw-rw-r--   0        0        0      888 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/contraction-pion.cpp
+-rw-rw-r--   0        0        0     1661 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/coordinate.cpp
+-rw-rw-r--   0        0        0    12786 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/exports.h
+-rw-rw-r--   0        0        0     2800 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/fermion-action.cpp
+-rw-rw-r--   0        0        0     4445 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/field-double.cpp
+-rw-rw-r--   0        0        0     4034 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/field-io.cpp
+-rw-rw-r--   0        0        0    11083 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/field-selection.cpp
+-rw-rw-r--   0        0        0    22526 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/field-utils.cpp
+-rw-rw-r--   0        0        0    12813 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/field.cpp
+-rw-rw-r--   0        0        0     9373 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/fields-io.cpp
+-rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/gauge-action.cpp
+-rw-rw-r--   0        0        0     6667 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/geometry.cpp
+-rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/hmc-stats.cpp
+-rw-rw-r--   0        0        0     1915 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/hmc.cpp
+-rw-rw-r--   0        0        0     1573 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/init.cpp
+-rw-rw-r--   0        0        0     3066 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/inverter.cpp
+-rw-rw-r--   0        0        0      482 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/lat-io.cpp
+-rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/lib.cpp
+-rw-rw-r--   0        0        0     2225 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/lib.h
+-rw-rw-r--   0        0        0     7995 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/mat.cpp
+-rw-rw-r--   0        0        0      369 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/meson.build
+-rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/mpi.cpp
+-rw-rw-r--   0        0        0     8646 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/propagator.cpp
+-rw-rw-r--   0        0        0     8060 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/qcd.cpp
+-rw-rw-r--   0        0        0     6901 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/scalar-action.cpp
+-rw-rw-r--   0        0        0    23483 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/selected-field.cpp
+-rw-rw-r--   0        0        0    17537 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/selected-points.cpp
+-rw-rw-r--   0        0        0     2639 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/smear.cpp
+-rw-rw-r--   0        0        0     1775 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/topology.cpp
+-rwxr-xr-x   0        0        0      766 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/update.sh
+-rw-rw-r--   0        0        0     6882 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/utils-io.cpp
+-rw-rw-r--   0        0        0      590 1970-01-01 00:00:00.000000 qlat-0.9/pylib/cqlat/wilson-flow.cpp
+-rw-rw-r--   0        0        0      241 1970-01-01 00:00:00.000000 qlat-0.9/pylib/meson.build
+-rw-rw-r--   0        0        0       29 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/__init__.pxd
+-rw-rw-r--   0        0        0      795 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/__init__.py
+-rw-rw-r--   0        0        0      193 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/c.py
+-rw-rw-r--   0        0        0      247 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/contract_field.py
+-rw-rw-r--   0        0        0      219 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/contract_hvp.py
+-rw-rw-r--   0        0        0      377 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/contract_pion.py
+-rw-rw-r--   0        0        0      687 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/coordinate.py
+-rw-rw-r--   0        0        0      211 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/cp.pyx
+-rw-rw-r--   0        0        0     1086 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/fermion_action.py
+-rw-rw-r--   0        0        0    15422 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/field.py
+-rw-rw-r--   0        0        0     1312 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/field_double.py
+-rw-rw-r--   0        0        0     6179 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/field_selection.py
+-rw-rw-r--   0        0        0     4550 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/field_utils.py
+-rw-rw-r--   0        0        0     6344 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/fields_io.py
+-rw-rw-r--   0        0        0      491 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/gauge_action.py
+-rw-rw-r--   0        0        0     3684 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/geometry.py
+-rw-rw-r--   0        0        0      443 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/get_include_dir.py
+-rw-rw-r--   0        0        0     1160 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/hmc.py
+-rw-rw-r--   0        0        0      671 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/hmc_stats.py
+-rw-rw-r--   0        0        0     3378 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/inverter.py
+-rw-rw-r--   0        0        0     4955 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/mat.py
+-rw-rw-r--   0        0        0      573 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/meson.build
+-rw-rw-r--   0        0        0     1540 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/mpi.py
+-rw-rw-r--   0        0        0     6732 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/propagator.py
+-rw-rw-r--   0        0        0     5215 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/qcd.py
+-rw-rw-r--   0        0        0     3348 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/scalar_action.py
+-rw-rw-r--   0        0        0    10295 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/selected_field.py
+-rw-rw-r--   0        0        0     6050 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/selected_points.py
+-rw-rw-r--   0        0        0     1198 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/smear.py
+-rw-rw-r--   0        0        0     3444 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/topology.py
+-rw-rw-r--   0        0        0       79 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/utils-io.cpp
+-rw-rw-r--   0        0        0      330 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/utils.py
+-rw-rw-r--   0        0        0      184 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/utils_io.pxd
+-rw-rw-r--   0        0        0      573 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/utils_io.py
+-rw-rw-r--   0        0        0     1593 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat/wilson_flow.py
+-rw-rw-r--   0        0        0    21037 1970-01-01 00:00:00.000000 qlat-0.9/pylib/qlat_gpt.py
+-rw-rw-r--   0        0        0    14723 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd.py
+-rw-rw-r--   0        0        0      919 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/__init__.py
+-rw-rw-r--   0        0        0      184 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/meson.build
+-rw-rw-r--   0        0        0     2702 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_16IH2.py
+-rw-rw-r--   0        0        0     4397 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_24D.py
+-rw-rw-r--   0        0        0     4394 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_24DH.py
+-rw-rw-r--   0        0        0     1912 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_24IH01.py
+-rw-rw-r--   0        0        0     1209 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_24IH02.py
+-rw-rw-r--   0        0        0     1213 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_24IH03.py
+-rw-rw-r--   0        0        0     1965 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_24IH04.py
+-rw-rw-r--   0        0        0     1961 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_24IH05.py
+-rw-rw-r--   0        0        0     3542 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_24IH1.py
+-rw-rw-r--   0        0        0     3541 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_24IH2.py
+-rw-rw-r--   0        0        0     3541 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_24IH3.py
+-rw-rw-r--   0        0        0     3541 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_24IH4.py
+-rw-rw-r--   0        0        0     1662 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_32D.py
+-rw-rw-r--   0        0        0     2717 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_32Dfine.py
+-rw-rw-r--   0        0        0     1124 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_32IH01.py
+-rw-rw-r--   0        0        0     3540 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_32IH1.py
+-rw-rw-r--   0        0        0     3540 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_32IH2.py
+-rw-rw-r--   0        0        0     3540 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_32IH3.py
+-rw-rw-r--   0        0        0     1919 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_32IcoarseH01.py
+-rw-rw-r--   0        0        0     1915 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_32IcoarseH02.py
+-rw-rw-r--   0        0        0     3551 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_32IcoarseH1.py
+-rw-rw-r--   0        0        0     3551 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_32IfineH.py
+-rw-rw-r--   0        0        0     1909 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_48I.py
+-rw-rw-r--   0        0        0     1122 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_64I.py
+-rw-rw-r--   0        0        0      285 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_96I.py
+-rw-rw-r--   0        0        0     3926 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/p_test.py
+-rw-rw-r--   0        0        0     1473 1970-01-01 00:00:00.000000 qlat-0.9/pylib/rbc_ukqcd_params/utils.py
+-rw-rw-r--   0        0        0      405 1970-01-01 00:00:00.000000 qlat-0.9/pyproject.toml
+-rw-r--r--   0        0        0      271 1970-01-01 00:00:00.000000 qlat-0.9/PKG-INFO
```

### Comparing `qlat-0.8/LICENSE` & `qlat-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qlat-0.8/bin/eigen-system-repartition` & `qlat-0.9/bin/eigen-system-repartition`

 * *Files identical despite different names*

### Comparing `qlat-0.8/bin/gauge-fix-coulomb` & `qlat-0.9/bin/gauge-fix-coulomb`

 * *Files identical despite different names*

### Comparing `qlat-0.8/bin/topo-measure` & `qlat-0.9/bin/topo-measure`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/compressed-eigen-io.h` & `qlat-0.9/include/qlat/compressed-eigen-io.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/contract-field.h` & `qlat-0.9/include/qlat/contract-field.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/contract-hvp.h` & `qlat-0.9/include/qlat/contract-hvp.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/contract-pion.h` & `qlat-0.9/include/qlat/contract-pion.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/contract-wall-src-prop.h` & `qlat-0.9/include/qlat/contract-wall-src-prop.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/coordinate-d.h` & `qlat-0.9/include/qlat/coordinate-d.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/coordinate.h` & `qlat-0.9/include/qlat/coordinate.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/core.h` & `qlat-0.9/include/qlat/core.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/cps-lanc.h` & `qlat-0.9/include/qlat/cps-lanc.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/cps-pio.h` & `qlat-0.9/include/qlat/cps-pio.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/cps-utils.h` & `qlat-0.9/include/qlat/cps-utils.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/cps.h` & `qlat-0.9/include/qlat/cps.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/dslash.h` & `qlat-0.9/include/qlat/dslash.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/fermion-action.h` & `qlat-0.9/include/qlat/fermion-action.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/field-comm.h` & `qlat-0.9/include/qlat/field-comm.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/field-dist-io.h` & `qlat-0.9/include/qlat/field-dist-io.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/field-expand.h` & `qlat-0.9/include/qlat/field-expand.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/field-fft.h` & `qlat-0.9/include/qlat/field-fft.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/field-io.h` & `qlat-0.9/include/qlat/field-io.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/field-rng.h` & `qlat-0.9/include/qlat/field-rng.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/field-serial-io.h` & `qlat-0.9/include/qlat/field-serial-io.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/field-shuffle.h` & `qlat-0.9/include/qlat/field-shuffle.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/field-utils.h` & `qlat-0.9/include/qlat/field-utils.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/field.h` & `qlat-0.9/include/qlat/field.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/fields-io.h` & `qlat-0.9/include/qlat/fields-io.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/geometry.h` & `qlat-0.9/include/qlat/geometry.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/grid.h` & `qlat-0.9/include/qlat/grid.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/hmc-stats.h` & `qlat-0.9/include/qlat/hmc-stats.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/hmc.h` & `qlat-0.9/include/qlat/hmc.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/matrix-hmc.h` & `qlat-0.9/include/qlat/matrix-hmc.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/matrix.h` & `qlat-0.9/include/qlat/matrix.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/meson.build` & `qlat-0.9/include/qlat/meson.build`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/mpi.h` & `qlat-0.9/include/qlat/mpi.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/mvector.h` & `qlat-0.9/include/qlat/mvector.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/py_convert.h` & `qlat-0.9/include/qlat/py_convert.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/qcd-gauge-transformation-boundary.h` & `qlat-0.9/include/qlat/qcd-gauge-transformation-boundary.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/qcd-gauge-transformation.h` & `qlat-0.9/include/qlat/qcd-gauge-transformation.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/qcd-prop.h` & `qlat-0.9/include/qlat/qcd-prop.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/qcd-smear.h` & `qlat-0.9/include/qlat/qcd-smear.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/qcd-topology.h` & `qlat-0.9/include/qlat/qcd-topology.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/qcd-utils.h` & `qlat-0.9/include/qlat/qcd-utils.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/qcd.h` & `qlat-0.9/include/qlat/qcd.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/qed.h` & `qlat-0.9/include/qlat/qed.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/qlat-analysis.h` & `qlat-0.9/include/qlat/qlat-analysis.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/qlat-setup.h` & `qlat-0.9/include/qlat/qlat-setup.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/qlat.h` & `qlat-0.9/include/qlat/qlat.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/quda.h` & `qlat-0.9/include/qlat/quda.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/scalar-action.h` & `qlat-0.9/include/qlat/scalar-action.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/selected-field-io.h` & `qlat-0.9/include/qlat/selected-field-io.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/selected-field.h` & `qlat-0.9/include/qlat/selected-field.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/selected-points.h` & `qlat-0.9/include/qlat/selected-points.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/utils-coordinate.h` & `qlat-0.9/include/qlat/utils-coordinate.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/utils-io.h` & `qlat-0.9/include/qlat/utils-io.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/vector_utils/check_fun.h` & `qlat-0.9/include/qlat/vector_utils/check_fun.h`

 * *Files 6% similar despite different names*

```diff
@@ -46,16 +46,16 @@
     Coordinate xg0 = p0.geo().coordinate_g_from_l(xl0);
 
     qlat::WilsonMatrixT<T>&  s0 =  p0.get_elem_offset(index);
     qlat::WilsonMatrixT<T>&  s1 =  p1.get_elem_offset(index);
     for(int d0=0;d0<12;d0++)
     for(int d1=0;d1<12;d1++)
     {
-      T p0 = s0(d0,d1);
-      T p1 = s1(d0,d1);
+      qlat::ComplexT<T > p0 = s0(d0,d1);
+      qlat::ComplexT<T > p1 = s1(d0,d1);
 
       double diff = 0.0;
       double n0 = qlat::qnorm(p0);
       double n1 = qlat::qnorm(p1);
       bool checknan = false;
       if(std::isnan(p0.real()) or std::isnan(p0.imag())){checknan = true;}
       if(std::isnan(p1.real()) or std::isnan(p1.imag())){checknan = true;}
@@ -255,12 +255,34 @@
   qlat::vector_acc<Ty > sum;sum.resize(1);sum[0] = 0.0;
   Ty* pres = sum.data();
   if(GPU == 1){reduce_vec(a, pres , size, 1);}
   if(GPU == 0){reduce_cpu(a, pres , size, 1);}
   print0("%s, sum %.3e \n", stmp.c_str(), qlat::qnorm(sum[0]) );
 }
 
-
+template <typename Ty>
+double check_sum_prop(qpropT& p0)
+{
+  ////int rank = qlat::get_id_node();
+  const Geometry& geo = p0.geo();
+  double check_sum = 0.0;
+  const Ty* src = (Ty*) qlat::get_data(p0).data();
+  const long Nvol = geo.local_volume();
+  for(long index = 0; index < Nvol; ++index){
+    Coordinate xl = geo.coordinate_from_index(index);
+    Coordinate xg = geo.coordinate_g_from_l(xl);
+    double cor = xg[0]*0.5 + xg[1]*1.7 + xg[2]*xg[2]*2.5 + xg[3]*xg[3]*0.2;
+    for(long dc = 0;dc<12*12;dc++)
+    {
+      Ty fac = Ty(std::cos(cor + dc) , std::sin(cor*5.7  + dc*dc) );
+      check_sum += qlat::qnorm( src[dc*Nvol + index] * fac ) ;
+    }
+  }
+  sum_all_size(&check_sum,1);
+  MPI_Barrier(get_comm());fflush(stdout);
+  /////print0("==prop check_sum %.8e \n", check_sum);
+  return check_sum;
+}
 
 }
 
 #endif
```

### Comparing `qlat-0.8/include/qlat/vector_utils/general_funs.h` & `qlat-0.9/include/qlat/vector_utils/general_funs.h`

 * *Files 24% similar despite different names*

```diff
@@ -15,379 +15,19 @@
 
 #include "utils_float_type.h"
 #include<type_traits>
 
 #include <iterator>
 #include "utils_read_txt.h"
 #include "utils_vector_GPU.h"
+#include "utils_mpi.h"
 
 namespace qlat
 {
 
-template<typename Iy>
-void reduce_MPI_type(Iy num, MPI_Datatype& curr, unsigned int& size)
-{
-  if(num <= 0){curr = MPI_BYTE; size = 1;return;}
-  //if(num%(sizeof(std::complex<double>)) == 0){curr = MPI::DOUBLE_COMPLEX ; size=sizeof( std::complex<double> );return;}
-  //if(num%(sizeof(std::complex<float >)) == 0){curr = MPI::COMPLEX        ; size=sizeof( std::complex<float > );return;}
-
-  if(num%(sizeof(std::int64_t )) == 0){curr = MPI_INT64_T ; size=sizeof(std::int64_t );return;}
-  if(num%(sizeof(std::int32_t )) == 0){curr = MPI_INT32_T ; size=sizeof(std::int32_t );return;}
-  if(num%(sizeof(std::int16_t )) == 0){curr = MPI_INT16_T ; size=sizeof(std::int16_t );return;}
-  if(num%(sizeof(std::int8_t  )) == 0){curr = MPI_INT8_T  ; size=sizeof(std::int8_t  );return;}
-}
-
-template<class M>
-unsigned int get_MPI_type(MPI_Datatype& curr)
-{
-  curr = MPI_BYTE;unsigned int size = 1;
-  DATA_TYPE typenum = get_data_type<M >();
-  if(typenum == INVALID_TYPE){
-    if(get_id_node()== 0){printf("Type not found !!!! \n");}qassert(false); return 0;
-  }
-
-  int dtype = typenum % MAXTYPE;
-  if(dtype <= FLOATIND + 3){
-
-    size = typenum/MAXTYPE;
-
-    if(dtype == 0){curr =  MPI_CHAR                 ; return size ;}
-    if(dtype == 1){curr =  MPI_UNSIGNED_CHAR        ; return size ;}
-    if(dtype == 2){curr =  MPI_SHORT                ; return size ;}
-    if(dtype == 3){curr =  MPI_UNSIGNED_SHORT       ; return size ;}
-    if(dtype == 4){curr =  MPI_INT                  ; return size ;}
-    if(dtype == 5){curr =  MPI_UNSIGNED             ; return size ;}
-    if(dtype == 6){curr =  MPI_LONG                 ; return size ;}
-    if(dtype == 7){curr =  MPI_UNSIGNED_LONG        ; return size ;}
-    if(dtype == 8){curr =  MPI_LONG_LONG            ; return size ;}
-    if(dtype == 9){curr =  MPI_UNSIGNED_LONG_LONG   ; return size ;}
-    if(dtype ==10){curr =  MPI_INT8_T               ; return size ;}
-    if(dtype ==11){curr =  MPI_UINT8_T              ; return size ;}
-    if(dtype ==12){curr =  MPI_INT16_T              ; return size ;}
-    if(dtype ==13){curr =  MPI_UINT16_T             ; return size ;}
-    if(dtype ==14){curr =  MPI_INT32_T              ; return size ;}
-    if(dtype ==15){curr =  MPI_UINT32_T             ; return size ;}
-    if(dtype ==16){curr =  MPI_INT64_T              ; return size ;}
-    if(dtype ==17){curr =  MPI_UINT64_T             ; return size ;}
-    
-    if(dtype ==FLOATIND+0){curr =  MPI_DOUBLE               ; return size ;}
-    if(dtype ==FLOATIND+1){curr =  MPI_FLOAT                ; return size ;}
-    if(dtype ==FLOATIND+2){curr =  MPI_C_DOUBLE_COMPLEX     ; return size ;}
-    if(dtype ==FLOATIND+3){curr =  MPI_C_FLOAT_COMPLEX      ; return size ;}
-  }
-  else{
-    if( get_data_type_is_double<M >()){curr = MPI_C_DOUBLE_COMPLEX; size = Complex_TYPE/MAXTYPE ;return size ;}
-    if(!get_data_type_is_double<M >()){curr = MPI_C_FLOAT_COMPLEX ; size = ComplexF_TYPE/MAXTYPE;return size ;}
-  }
-
-  if(get_id_node()== 0){printf("Type not found !!!! \n");}qassert(false);
-  return 0;
-
-}
-
-template<typename Ty>
-void sum_all_size(Ty *src,Ty *sav,long size, int GPU=0, MPI_Comm* commp=NULL)
-{
-  TIMER("global sum sum_all_size");
-  if(size == 0){return ;}
-  if(qlat::get_num_node() == 1){
-    if(src == sav){return;}
-    if(src != sav){
-      cpy_data_thread(sav, src, size, GPU, true);return;}
-  }
-
-  const int iomp = omp_get_thread_num(); ////each thread will have it's own buf
-  Ty* buf_res;int GPU_set = GPU;
-  #ifndef QLAT_USE_ACC
-  GPU_set = 0;
-  #endif
-  VectorGPUKey gkey(size_t(size)*sizeof(Ty), ssprintf("sum_all_size_buf_%d", iomp), GPU_set); ////read buffers for global sum
-  if(src == sav){
-    const vector_gpu<char >& tmp = get_vector_gpu_plan<char >(gkey);
-    buf_res = (Ty*) tmp.p;
-  }else{buf_res = sav;}////small modify for pointers
-
-  MPI_Datatype curr = MPI_DOUBLE;unsigned int M_size = sizeof(double);
-  M_size = get_MPI_type<Ty >(curr);
-
-  qassert(sizeof(Ty)%M_size == 0);int fac = sizeof(Ty)/M_size;
-
-
-  Ty* tem_src = NULL; Ty* tem_res = NULL;
-  std::vector<Ty > tem_sHIP,tem_rHIP;
-  bool do_copy = false;
-
-  #ifdef __NO_GPU_DIRECT__
-  #ifdef QLAT_USE_ACC
-  if(GPU == 1){do_copy = true;}
-  #endif
-  #endif
-
-  if(do_copy == false){tem_src = src;tem_res = buf_res;}
-  if(do_copy == true ){
-    tem_sHIP.resize(size);tem_rHIP.resize(size);
-
-    cpy_data_thread(&tem_sHIP[0], src, size, 3, true);
-    tem_src = &tem_sHIP[0];tem_res = &tem_rHIP[0];
-  }
-  
-  if(commp == NULL){MPI_Allreduce(tem_src,tem_res, size * fac, curr, MPI_SUM, get_comm());}
-  else{MPI_Allreduce(tem_src,tem_res, size * fac, curr, MPI_SUM, *commp);}
-
-  if(do_copy == true){
-    cpy_data_thread(buf_res, &tem_rHIP[0], size, 2, true);
-  }
-
-
-  if(src == sav)
-  {
-    cpy_data_thread(sav, buf_res, size, GPU, true);
-  }
-  if(src != sav){safe_free_vector_gpu_plan<char>(gkey);}
-}
-
-template<typename Ty>
-void sum_all_size(Ty *src,long size, int GPU=0, MPI_Comm* commp=NULL)
-{
-  sum_all_size(src,src,size, GPU, commp);
-}
-
-template<typename Ty>
-void Bcast_all_Nt(Ty *src,long size,const qlat::Geometry &geo)
-{
-  if(qlat::get_num_node() == 1){return;}
-  int Nt = geo.node_site[3];
-  int Nmpi  = qlat::get_num_node();
-
-  const Coordinate vg = geo.total_site();
-  const int nt = vg[3];
-
-  if(nt/Nt != Nmpi){
-    sum_all_size(src,size);
-    return;
-  }
-
-  int mt = nt/Nt;
-  int rank  = qlat::get_id_node();
-  long size_c = sizeof(Ty)*size/mt;
-
-  unsigned short t0 = 0;
-  {
-    Coordinate xl = geo.coordinate_from_index(0);
-    xl[3] = 0;
-    Coordinate xg = geo.coordinate_g_from_l(xl);
-    t0 = xg[3];
-  }
-
-  std::vector<int > send,recv,spls,rpls;
-  send.resize(Nmpi);
-  recv.resize(Nmpi);
-  spls.resize(Nmpi);
-  rpls.resize(Nmpi);
-
-  std::fill(send.begin(), send.end(), 0);
-  std::fill(recv.begin(), recv.end(), 0);
-  std::fill(spls.begin(), spls.end(), 0);
-  std::fill(rpls.begin(), rpls.end(), 0);
-
-  for(int ti=0;ti<mt;ti++){
-    int tini = ti*Nt;
-    if(t0 == tini){
-      for(int ri=0;ri<Nmpi;ri++)if(ri != rank)
-      {
-        send[ri] = size_c;
-        spls[ri] = size_c*ti;
-      }
-    }
-
-    if(t0 != tini){
-      int ri_recv = ti;
-      recv[ri_recv] = size_c;
-      rpls[ri_recv] = size_c*ti;
-    }
-  }
-
-  MPI_Alltoallv(src,(int*) &send[0],(int*) &spls[0], MPI_CHAR,
-                src,(int*) &recv[0],(int*) &rpls[0], MPI_CHAR, get_comm());
-
-}
-
-////Need add explanations
-template<typename Ty>
-void Redistribute_all_Nt(Ty *src,long size,const qlat::Geometry &geo, int GPU=0)
-{
-  if(qlat::get_num_node() == 1){return;}
-  int Nt = geo.node_site[3];
-  int Nmpi  = qlat::get_num_node();
-
-  const Coordinate vg = geo.total_site();
-  const int nt = vg[3];
-
-  int mt = nt/Nt;
-  if(mt != Nmpi){print0("Not supported !");qassert(false);return;}
-
-  /////int rank  = qlat::get_id_node();
-  long size_c = sizeof(Ty)*size/mt;
-
-  std::vector<int > send,recv,spls,rpls;
-  send.resize(Nmpi);
-  recv.resize(Nmpi);
-  spls.resize(Nmpi);
-  rpls.resize(Nmpi);
-
-  for(int ri=0;ri<Nmpi;ri++)
-  {
-    send[ri] = size_c;
-    spls[ri] = size_c*ri;
-
-    recv[ri] = size_c;
-    rpls[ri] = size_c*ri;
-  }
-
-  //Ty* buf;
-  //if(GPU == 0){buf = (Ty *)aligned_alloc_no_acc(size*sizeof(Ty));}
-  //if(GPU == 1){gpuMalloc(buf, size, Ty);}
-  qlat::vector_gpu<Ty > buf; buf.resize(size, GPU);
-
-  {
-  ////TIMER("MPI call CPU");
-  MPI_Alltoallv(src   ,(int*) &send[0],(int*) &spls[0], MPI_CHAR,
-            buf.data(),(int*) &recv[0],(int*) &rpls[0], MPI_CHAR, get_comm());
-  }
-
-  #ifdef QLAT_USE_ACC
-  if(GPU == 0){
-    #pragma omp parallel for
-    for(long isp=0;isp<size;isp++){src[isp] = buf[isp];}
-    ///delete [] buf;
-    //free(buf);
-  }
-  if(GPU == 1){
-    /////qacc_for(isp, size,{ src[isp] = buf[isp];});
-    cudaMemcpy(src, buf.data(), size*sizeof(Ty), cudaMemcpyDeviceToDevice);
-    ////gpuFree(buf);
-  }
-  #else
-  #pragma omp parallel for
-  for(long isp=0;isp<size;isp++){src[isp] = buf[isp];}
-  //delete [] buf;
-  //free(buf);
-  #endif
-
-}
-
-inline void abort_sum(double flag, std::string stmp=std::string(""))
-{
-  sum_all_size(&flag,1);
-  if(flag > 0)
-  {
-    abort_r(stmp);
-  }
-}
-
-inline void fflush_MPI(){
-  MPI_Barrier(get_comm());
-  fflush(stdout);
-}
-
-//////"INT_MAX"
-//////offset by number of char
-template<typename Iy0, typename Iy1>
-void MPI_Alltoallv_Send_Recv(char* src, Iy0* send, Iy1* spls, char* res, Iy0* recv, Iy1* rpls, MPI_Comm& comm)
-{
-  int num_node;MPI_Comm_size(comm, &num_node);
-  int id_node;MPI_Comm_rank(comm, &id_node);
-  std::vector<MPI_Request> send_reqs(num_node);
-  int mpi_tag = id_node;
-  int c1 = 0;
-
-  /////===get proper M_size
-  MPI_Datatype curr = MPI_BYTE;unsigned int M_size = 1;unsigned int M_tem = 1;
-  for(int n = 0; n < num_node; n++){
-    if(send[n]!= 0){
-      reduce_MPI_type(send[n], curr, M_tem);
-      if(M_size == 1){M_size = M_tem;}
-      else{if(M_tem != M_size){curr = MPI_BYTE;M_size = 1;break;}}
-    }
-  }
-  /////
-
-  for(int n = 0; n < num_node; n++){
-    if(send[n]!=0){MPI_Isend(&src[spls[n]], int(send[n]/M_size), curr, n, mpi_tag + n, comm, &send_reqs[c1]);c1 += 1;}
-  }
-
-  for(int n = 0; n < num_node; n++){
-    if(recv[n]!=0){MPI_Recv( &res[rpls[n]], int(recv[n]/M_size), curr, n, mpi_tag + n, comm, MPI_STATUS_IGNORE);}
-  }
-  if(c1!=0){MPI_Waitall(c1, send_reqs.data(), MPI_STATUS_IGNORE);}
-}
-
-
-
-template<typename Ty>
-void MPI_Alltoallv_mode(Ty* src0, int* send, int* spls, Ty* res0, int* recv, int* rpls, MPI_Comm& comm, int mode=0, int GPU = 0)
-{
-  (void)GPU;
-  Ty* src = NULL;Ty* res = NULL;
-
-  std::vector<Ty > tem_src,tem_res;
-  bool do_copy = false;
-  #ifdef __NO_GPU_DIRECT__
-  #ifdef QLAT_USE_ACC
-  if(GPU == 1){do_copy = true;}
-  #endif
-  #endif
-
-  if(do_copy == false){src = src0; res = res0;}
-
-  ////resize buffers
-  long max_src = 0;
-  long max_res = 0;
-  if(do_copy == true){
-    int num_node;MPI_Comm_size(comm, &num_node);
-    for(int n = 0; n < num_node; n++){
-      long cur_size = spls[n]/sizeof(Ty) + send[n]/sizeof(Ty);
-      if(cur_size > max_src){max_src = cur_size;}
-      cur_size = rpls[n]/sizeof(Ty) + recv[n]/sizeof(Ty);
-      if(cur_size > max_res){max_res = cur_size;}
-    }
-
-    tem_src.resize(max_src);tem_res.resize(max_res);
-    cpy_data_thread(&tem_src[0], src0, max_src, 3);
-    cpy_data_thread(&tem_res[0], res0, max_res, 3);
-    src = &tem_src[0]; res = &tem_res[0];
-  }
-
-  if(mode == 0){
-    MPI_Alltoallv(src, send, spls, MPI_CHAR,
-                  res, recv, rpls, MPI_CHAR, comm);
-  }
-  if(mode == 1){
-    MPI_Alltoallv_Send_Recv((char*) src, send, spls, (char*) res, recv, rpls, comm);
-
-    //int num_node;MPI_Comm_size(comm, &num_node);
-    //int id_node;MPI_Comm_rank(comm, &id_node);
-    //std::vector<MPI_Request> send_reqs(num_node);
-    //int mpi_tag = id_node;
-    //int c1 = 0;
-    //for(int n = 0; n < num_node; n++){
-    //  if(send[n]!=0){MPI_Isend(&src[spls[n]/sizeof(Ty)], send[n], MPI_CHAR, n, mpi_tag + n, comm, &send_reqs[c1]);c1 += 1;}
-    //}
-
-    //for(int n = 0; n < num_node; n++){
-    //  if(recv[n]!=0){MPI_Recv( &res[rpls[n]/sizeof(Ty)], recv[n], MPI_CHAR, n, mpi_tag + n, comm, MPI_STATUS_IGNORE);}
-    //}
-    //if(c1!=0){MPI_Waitall(c1, send_reqs.data(), MPI_STATUS_IGNORE);}
-  }
-
-
-  if(do_copy == true){cpy_data_thread(res0, &tem_res[0], max_res, 2);}
-
-}
-
 ////Only cpu verstion
 ////flag = 1 --> biva * sizeF * civ * size_inner --> biva * civ * sizeF * size_inner
 inline void reorder_civ(char* src,char* res,int biva,int civ,size_t sizeF,int flag,int size_inner)
 {
   //TIMER("reorder_civ vectors char");
   if(biva == 0 or civ == 0 or sizeF == 0 or size_inner == 0){return ;}
 
@@ -899,53 +539,49 @@
   Ty* resP = tmp.data();
   qacc_for(isp,V*civ,{ resP[isp] = srcP[isp];});
   Ty  norm = tmp.norm();
   return norm;
   //print0("norm %.3e %.3e \n", norm.real(), norm.imag());
 }
 
-template <class T>
-void random_prop(Propagator4dT<T >& prop, int seed = -1)
+template <class Td>
+void random_prop(Propagator4dT<Td >& prop, int seed = -1)
 {
   qassert(prop.initialized);
   ////print0("print time %.3f\n", tm.tv_sec);
   int rand_seed = qlat::get_id_node() + 1;
   if(seed == -1){timeval tm;gettimeofday(&tm, NULL);rand_seed += int(tm.tv_sec);}else{rand_seed += seed;}
 
   qlat::RngState rs(rand_seed);
   double ini = qlat::u_rand_gen(rs);
 
   /////int dir_limit = 4;
   const Geometry& geo = prop.geo();
 
   qacc_for(isp,  geo.local_volume(),{
-    qlat::WilsonMatrixT<T >& v0 =  prop.get_elem_offset(isp);
-    //for(int ci=0;ci<12*12;ci++){
-    //  //v0.p[ci] = T(std::cos((ini+isp + ci*2)*0.5 + (isp+ ci%4)/5) , ((5.0+ci)/(isp+1))*ini*0.1 + (isp*2 + ci%3)/5); 
-    //  v0.p[ci] = T(std::cos((ini+isp + ci*2)*0.5 + ci) , ((5.0+ci)/(isp+1))*ini*0.1 + 0.2); 
-    //}
+    qlat::WilsonMatrixT<Td>& v0 =  prop.get_elem_offset(isp);
     for(int ci=0;ci<12*12;ci++){
-      v0.p[ci] = (ci/(12*12.0))*T(std::cos((ini+isp + ci*2)*0.5 + ci) , (ci+(5.0+ci)/(isp+1))*ini*0.1 + 0.2); 
+      v0.p[ci] = (ci/(12*12.0))* qlat::ComplexT<Td>(std::cos((ini+isp + ci*2)*0.5 + ci) , (ci+(5.0+ci)/(isp+1))*ini*0.1 + 0.2); 
     }
   }); 
 }
 
-template <class T>
-void random_link(GaugeFieldT<T> &gf, const int seed = -1)
+template <class Td>
+void random_link(GaugeFieldT<Td> &gf, const int seed = -1)
 {
   if(seed == -1)
   {
     qacc_for(isp, gf.field.size(), { set_unit(gf.get_elem_offset(isp), 1.0);});
   }else{
     const Geometry& geo = gf.geo();
-    T* res = (T*) qlat::get_data(gf).data();
-    random_Ty(res, geo.local_volume()*geo.multiplicity*sizeof(ColorMatrixT<T>)/sizeof(T), 1, seed);
+    qlat::ComplexT<Td>* res = (qlat::ComplexT<Td>*) qlat::get_data(gf).data();
+    random_Ty(res, geo.local_volume()*geo.multiplicity*sizeof(ColorMatrixT<Td>)/(sizeof(Td)*2), 1, seed);
 
     //qacc_for(isp, gf.field.size(), { set_unit(gf.get_elem_offset(isp), 1.0);});
-    ColorMatrixT<T> unit;set_unit(unit, 1.0);
+    ColorMatrixT<Td> unit;set_unit(unit, 1.0);
     /////TODO This function cannot be done on GPU
     /////Eigen normalize/normalized problem
     for(long isp=0;isp<gf.field.size();isp++)
     {
       gf.get_elem_offset(isp) = gf.get_elem_offset(isp) * (1/2.0) + unit;
       unitarize(gf.get_elem_offset(isp));
     }
@@ -1167,14 +803,24 @@
   print0("===nthreads %8d %8d, max %8d \n",qlat::qacc_num_threads(),omp_get_num_threads(),omp_get_max_threads());
 
   fflush_MPI();
   print_mem_info();
 
 }
 
+inline int end_Lat()
+{
+  fflush_MPI();
+  qlat::end();
+  fflush_MPI();
+  qlat::Timer::display();
+  if(qlat::is_MPI_initialized()){MPI_Finalize();}
+  return 0;
+}
+
 inline std::vector<long > job_create(long total, long each)
 {
   if(total < 1 or each < 1){
     print0("Give me valid job types total %ld, each %ld \n", total, each);
     abort_r();}
   /////std::vector<long > a = job_create(total, each);
   std::vector<long > a;a.resize(0);
@@ -1230,21 +876,47 @@
   std::complex<double > tem(lam.real(),lam.imag());
   std::complex<double > v0 = (one_minus_halfD>0)?(1.0-tem/2.0)/(rho*tem+m*(1.0-tem/2.0)):1.0/(rho*tem+m*(1.0-tem/2.0));
   Ty res(v0.real(),v0.imag());
   return res;
 }
 
 template<typename Ty>
-qlat::vector_acc<Ty* > EigenM_to_pointers(std::vector<qlat::vector_gpu<Ty > >& src)
+qlat::vector_acc<Ty* > EigenM_to_pointers(std::vector<qpropT >& src)
 {
   qlat::vector_acc< Ty* >  res;
   res.resize(src.size());
   for(LInt iv=0;iv<src.size();iv++)
   {
-    res[iv] = src[iv].data();
+    res[iv] = (Ty*) qlat::get_data(src[iv]).data();
+  }
+  return res;
+}
+
+template<typename Ty>
+qlat::vector_acc<Ty* > EigenM_to_pointers(std::vector<qlat::vector_gpu<Ty > >& src, long Nvol = -1)
+{
+  qlat::vector_acc< Ty* >  res;
+  const size_t Nvec = src.size();
+  if(Nvec == 0){return res;}
+
+  if(Nvol != -1){
+    qassert(src[0].size() % Nvol == 0);
+  }else{
+    Nvol = src[0].size();
+  }
+
+  const size_t Nt = src[0].size() / Nvol;
+  res.resize(Nvec * Nt);
+  for(size_t iv=0;iv<Nvec;iv++)
+  {
+    qassert(src[iv].size() == Nt * Nvol);
+    for(size_t it=0;it<Nt;it++)
+    {
+      res[iv*Nt + it] = &src[iv].data()[it* Nvol];
+    }
   }
   return res;
 }
 
 template<typename Ty>
 qlat::vector_acc<Ty* > EigenM_to_pointers(std::vector<qlat::vector_acc<Ty > >& src)
 {
@@ -1262,18 +934,18 @@
 Ty sum_local_to_global_vector(Ty src, MPI_Comm* commp=NULL)
 {
   ////int Nt = geo.node_site[3];
   int Nmpi  = qlat::get_num_node();
   int rank  = qlat::get_id_node();
   if(commp != NULL){MPI_Comm_size(*commp, &Nmpi);MPI_Comm_rank(*commp, &rank);}
 
-  qlat::vector<long > size_global;size_global.resize(Nmpi);for(unsigned long i=0;i<(unsigned long)size_global.size();i++){size_global[i]=0;}
+  qlat::vector<long > size_global;size_global.resize(Nmpi);
+  zero_Ty(size_global.data(), size_global.size(), 0);
 
   size_global[rank] = src.size();
-
   sum_all_size(size_global.data(), size_global.size(), 0, commp);
 
   long total = 0;long current = 0;
   for(int i=0;i<Nmpi;i++){total += size_global[i];if(i < rank){current += size_global[i];}}
 
   /////for(unsigned int i=0;i<size_global.size();i++){printf("rank %d, size %ld \n", rank, size_global[i]);}
   /////printf("rank %d, Total %ld, current %ld \n", rank, total, current);
@@ -1322,28 +994,22 @@
     b.push_back(r[u]);
     r.erase(r.begin()+ u);
   }
   return b;
 
 }
 
-///num to be zero for nodes
-template<typename Ty>
-void sum_value_mpi(Ty& num)
-{
-  //int Nmpi  = qlat::get_num_node();
-  //int rank  = qlat::get_id_node();
-  Ty buf = num;
-  long nvalue = 0;
-  if(std::fabs(num) > 1e-30){nvalue = 1;}
-  sum_all_size(&buf, 1);
-  sum_all_size(&nvalue, 1);
-  if(nvalue != 0){buf = buf/nvalue;}
-  num = buf;
-}
-
-
-
+//inline qlat::vector_acc<int > Coordinates_to_list(std::vector<Coordinate >& moms)
+//{
+//  qlat::vector_acc<int > momN;
+//  momN.resize(moms.size() * 4);
+//  for(unsigned int i=0;i<moms.size;i++){
+//    for(int j=0;j<4;j++){
+//      momN[i*4 + j] = moms[i][j];
+//    }
+//  }
+//  return momN;
+//}
 
 }
 
 #endif
```

### Comparing `qlat-0.8/include/qlat/vector_utils/quda_para.h` & `qlat-0.9/include/qlat/vector_utils/quda_para.h`

 * *Files 2% similar despite different names*

```diff
@@ -398,26 +398,26 @@
         gauge[indexo + i] *= sign;
       }
     }
   }
 }
 
 
-template <class Ty, class T1>
-void Ffield4d_to_quda_ff(T1*  quda_ff, qlat::FermionField4dT<Ty>& ff, int dir = 1)
+template <class Td, class T1>
+void Ffield4d_to_quda_ff(T1*  quda_ff, qlat::FermionField4dT<Td>& ff, int dir = 1)
 {
   TIMER("Ffield4d_to_quda_ff(ff, quda_ff)");
   qassert(ff.initialized);
   const Geometry& geo = ff.geo();
   //const WilsonVector* quda_pt =
   //    reinterpret_cast<const WilsonVector*>(qff.data());
   long V = geo.local_volume();
   long Vh = V / 2;
 
-  Ty* src = (Ty*) qlat::get_data(ff).data();
+  qlat::ComplexT<Td>* src = (qlat::ComplexT<Td>*) qlat::get_data(ff).data();
 
   //
   #pragma omp parallel for
   for (long qlat_idx_4d = 0; qlat_idx_4d < V; qlat_idx_4d++) {
     const Coordinate xl = geo.coordinate_from_index(qlat_idx_4d);
     int eo = (xl[0] + xl[1] + xl[2] + xl[3]) % 2;
     for (int dc = 0; dc < 12; dc++)
@@ -426,16 +426,16 @@
       if(dir == 1){quda_ff[quda_idx*12 + dc] = src[qlat_idx_4d*12 + dc];}
       if(dir == 0){src[qlat_idx_4d*12 + dc] = quda_ff[quda_idx*12 + dc];}
     }
   }
 
 }
 
-template <class Ty, class T1>
-void quda_ff_to_Ffield4d(qlat::FermionField4dT<Ty>& ff, T1* quda_ff)
+template <class Td, class T1>
+void quda_ff_to_Ffield4d(qlat::FermionField4dT<Td>& ff, T1* quda_ff)
 {
   Ffield4d_to_quda_ff(quda_ff, ff, 0);
 }
 
 template <class Ty, class T1>
 void qlat_cf_to_quda_cf(T1*  quda_cf, colorFT& qlat_cf, int dir = 1)
 {
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_COPY_data.h` & `qlat-0.9/include/qlat/vector_utils/utils_COPY_data.h`

 * *Files 9% similar despite different names*

```diff
@@ -72,30 +72,30 @@
   T* s0 = (T*) qlat::get_data(src).data();
   long* m1 = (long*) qlat::get_data(map_res).data();
   long* m0 = (long*) qlat::get_data(map_src).data();
   cpy_data_from_index(s1, s0, m1, m0, map_res.size(), bfac, GPU, dummy);
 }
 
 #ifdef QLAT_USE_ACC
-template <typename T0, typename T1, typename TInt, int bfac, int ADD_FAC>
-__global__ void cpy_data_thread_global(T0* Pres, const T1* Psrc,  const TInt Nvol, const double ADD)
+template <typename T0, typename T1, typename TInt, int bfac, int ADD_FAC, typename Tadd>
+__global__ void cpy_data_thread_global(T0* Pres, const T1* Psrc,  const TInt Nvol, const Tadd ADD)
 {
   TInt off = blockIdx.x*blockDim.x*bfac + threadIdx.x;
   for(int i=0;i<bfac;i++)
   {
     if(ADD_FAC== 0)if(off < Nvol){Pres[off]  = Psrc[off];}
     if(ADD_FAC== 1)if(off < Nvol){Pres[off] += ADD*Psrc[off];}
     off += blockDim.x;
   }
 }
 #endif
 
 //////Copy data thread, cannot give to zero with ADD = 0
-template <typename T0, typename T1, typename TInt>
-void CPY_data_thread_basic(T0* Pres, const T1* Psrc, const TInt Nvol, int GPU=1, bool dummy=true, const double ADD = 0)
+template <typename T0, typename T1, typename TInt, typename Tadd>
+void CPY_data_thread_basic(T0* Pres, const T1* Psrc, const TInt Nvol, int GPU, bool dummy, const Tadd ADD)
 {
   (void)dummy;
   if(GPU != 0 and GPU != 1){qassert(false);}
   bool do_copy = true;
   if(qlat::qnorm(ADD) <  1e-13){do_copy = true ;}
   if(qlat::qnorm(ADD) >= 1e-13){do_copy = false;}
 
@@ -104,16 +104,16 @@
   /////qacc_forNB(i, Nvol, {Pres[i]=Psrc[i];});
 
   const int Threads = 64;const int Biva = (4*16+sizeof(T0)-1)/sizeof(T0);
   long Nb = (Nvol + Threads*Biva -1)/(Threads*Biva);
   dim3 dimBlock(    Threads,    1, 1);
   dim3 dimGrid(     Nb,    1, 1);
 
-  if( do_copy)cpy_data_thread_global<T0, T1, TInt , Biva, 0><<< dimGrid, dimBlock >>>(Pres, Psrc, Nvol, ADD);
-  if(!do_copy)cpy_data_thread_global<T0, T1, TInt , Biva, 1><<< dimGrid, dimBlock >>>(Pres, Psrc, Nvol, ADD);
+  if( do_copy)cpy_data_thread_global<T0, T1, TInt , Biva, 0, Tadd><<< dimGrid, dimBlock >>>(Pres, Psrc, Nvol, ADD);
+  if(!do_copy)cpy_data_thread_global<T0, T1, TInt , Biva, 1, Tadd><<< dimGrid, dimBlock >>>(Pres, Psrc, Nvol, ADD);
 
   if(dummy)qacc_barrier(dummy);
   return ;}
   #endif
 
   //////===from device to device, mode 0
   if(do_copy){
@@ -134,16 +134,16 @@
   }
 
 }
 
 //////Copy data thread
 //0--> host to host, 1 device to device
 //2--> ===from host to device, 3 ===from device to host
-template <typename T0, typename T1,  typename TInt>
-void cpy_data_thread(T0* Pres, const T1* Psrc, const TInt Nvol, int GPU=1, bool dummy=true, const double ADD = 0)
+template <typename T0, typename T1,  typename TInt, typename Tadd>
+void cpy_data_threadT(T0* Pres, const T1* Psrc, const TInt Nvol, int GPU, bool dummy, const Tadd ADD)
 {
   if((void*) Pres == (void*) Psrc){return ;}////return if points are the same
   TIMERA("cpy_data_thread");
   ////if(Pres == Psrc){return ;}
   ////0--> host to host, 1 device to device
   if(GPU == 0 or GPU == 1){CPY_data_thread_basic(Pres, Psrc, Nvol, GPU, dummy, ADD);return ;}
   /////if(GPU == 2 or GPU == 3){if(ADD != 0){qassert(false);}}
@@ -154,39 +154,50 @@
   /////qassert(sizeof(T0) == sizeof(T1));
   if(sizeof(T0) == sizeof(T1) and qlat::qnorm(ADD) <  1e-13){
     gpuErrchk(cudaMemcpyAsync(Pres, Psrc , Nvol*sizeof(T0), cudaMemcpyHostToDevice));
     if(dummy)qacc_barrier(dummy);
   }else{
     qlat::vector_acc< T0 > buf;buf.resize(Nvol);T0* s0 = (T0*) qlat::get_data(buf).data();
     /////host to host
-    CPY_data_thread_basic(s0, Psrc, Nvol, 0, false);
+    CPY_data_thread_basic(s0, Psrc, Nvol, 0, false, 0.0);
     /////devic to device
     CPY_data_thread_basic(Pres, s0, Nvol, 1, dummy, ADD);
   }
   return ;}
 
   //////===from device to host
   if(GPU ==  3){
   ////qassert(sizeof(T0) == sizeof(T1));
   if(sizeof(T0) == sizeof(T1) and qlat::qnorm(ADD) <  1e-13){
     gpuErrchk(cudaMemcpyAsync(Pres, Psrc , Nvol*sizeof(T0), cudaMemcpyDeviceToHost));
     if(dummy)qacc_barrier(dummy);
   }else{
     qlat::vector_acc< T0 > buf;buf.resize(Nvol);T0* s0 = (T0*) qlat::get_data(buf).data();
     /////device to device
-    CPY_data_thread_basic(s0, Psrc, Nvol, 1, true);
+    CPY_data_thread_basic(s0, Psrc, Nvol, 1,  true, 0.0);
     /////host to host
     CPY_data_thread_basic(Pres, s0, Nvol, 0, false, ADD);
   }
   return ;}
 
   #else
   CPY_data_thread_basic(Pres, Psrc, Nvol, 0, false, ADD);
   #endif
+}
+
+template <typename T0, typename T1,  typename TInt>
+void cpy_data_thread(T0* Pres, const T1* Psrc, const TInt Nvol, int GPU=1, bool dummy=true, const double ADD = 0)
+{
+  cpy_data_threadT<T0, T1, TInt, double>(Pres, Psrc, Nvol, GPU, dummy, ADD);
+}
 
+template <typename T0, typename T1,  typename TInt>
+void cpy_data_threadC(T0* Pres, const T1* Psrc, const TInt Nvol, int GPU=1, bool dummy=true, const T1 ADD = 0)
+{
+  cpy_data_threadT<T0, T1, TInt, T1>(Pres, Psrc, Nvol, GPU, dummy, ADD);
 }
 
 template <typename Ty>
 void touch_GPU(Ty* Mres, long long Msize,long long offM = 0,long long size = -1, int mode = 1)
 {
   (void)Mres;
   (void)mode;
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_FFT_GPU.h` & `qlat-0.9/include/qlat/vector_utils/utils_FFT_GPU.h`

 * *Files 0% similar despite different names*

```diff
@@ -164,14 +164,15 @@
 
   /////====GPU parts
   #endif
   }else{
 
   if(MPI_para.size() == 3)
   {
+    #ifdef __QLAT_WITH_FFT_MPI__
     MPI_Comm_split(get_comm(), color_xyz, ranku, &fft_comm);
     for(int i=0;i<int(nv.size());i++){nrank[i] = nv[i];}
 
     if(single_type == 0){
     alloc_local = fftw_mpi_local_size_many(dim, nrank, howmany, block0, fft_comm, &local_n0, &local_0_start);
     fft_dat = fftw_malloc(alloc_local*bsize);
     plan_cpuD0 = fftw_mpi_plan_many_dft(dim,nrank, howmany, block0, block0, (fftw_complex*) fft_dat, (fftw_complex*) fft_dat,
@@ -188,15 +189,19 @@
     plan_cpuF1 = fftwf_mpi_plan_many_dft(dim,nrank, howmany, block0, block0, (fftwf_complex*) fft_dat, (fftwf_complex*) fft_dat,
               fft_comm, FFTW_BACKWARD, FFTW_MEASURE);
     }
   
     /////each node has data vol/("Nv[0]")
     MPI_datasize = datasize/(nrank[0]/block0);
     if(local_0_start != ranku or local_n0 != block0){abort_r("fft_mpi not correct !\n");}
-  }else{
+    #else
+    abort_r("fft_mpi not set! \n");
+    #endif
+  }
+  else{
 
     ////void* vb_dat = NULL;
     if(single_type == 0)fft_dat =  fftw_malloc(datasize);
     if(single_type == 1)fft_dat = fftwf_malloc(datasize);
 
     /////////"n" same layout for input, "istride" -- zyx(j) -- j*istride+k*idist , "idist" -- howmany(k) -- in+k*idist
     if(single_type == 0){
@@ -479,14 +484,18 @@
     ////print0("job size %d \n", int(job.size()));
     if(enable_MPI == 1 and dim == 3 and fd.my * fd.mx != 1){abort_r("mode not supported ! \n");}
     if(!(enable_MPI == 0 or enable_MPI == 1)){abort_r("enable_MPI not set yes! \n");};
 
     b0 = job[1];c0 = job[2];///////NEED_COPY = job[4];
     /////====Set up b0, c0
 
+    #ifndef __QLAT_WITH_FFT_MPI__
+    enable_MPI = 0;
+    #endif
+
     if(GPU){qassert(enable_MPI == 0);}
     NEED_COPY = 0;
     if(civ%(N_extra*c0) != 0 or GPU){NEED_COPY = 1;}
 
     int mode_rot = -2;
     if(enable_MPI == 0){N_extra = N0;if(dim == 3){mode_rot =  0;}if(dim == 4){mode_rot = 1;}}
     if(enable_MPI == 1){N_extra = N1;if(dim == 3){mode_rot = -1;}if(dim == 4){mode_rot = 0;}}
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_Matrix_prod.h` & `qlat-0.9/include/qlat/vector_utils/utils_Matrix_prod.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_Vec_redistribute.h` & `qlat-0.9/include/qlat/vector_utils/utils_Vec_redistribute.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_construction.h` & `qlat-0.9/include/qlat/vector_utils/utils_construction.h`

 * *Files 15% similar despite different names*

```diff
@@ -21,25 +21,28 @@
 #define USEQACC   1
 #else
 #define USEKERNEL 0
 #define USEGLOBAL 0
 #define USEQACC   0
 #endif
 
-#define EigenMTa std::vector<qlat::vector_acc<Ta > >
-#define EigenVTa qlat::vector_acc<Ta >
+#define EigenTy std::vector<qlat::vector_gpu<Ty > >
+
+///#define EigenMTa std::vector<qlat::vector_acc<Ta > >
+//#define EigenVTa qlat::vector_acc<Ta >
 #define EAy   Eigen::Map<Eigen::Array<Ty ,Eigen::Dynamic,1 > >
-#define EAa   Eigen::Map<Eigen::Array<Ta ,Eigen::Dynamic,1 > >
+//#define EAa   Eigen::Map<Eigen::Array<Ta ,Eigen::Dynamic,1 > >
 
 #include "utils_corr_prop.h"
 #include "utils_corr_meson.h"
 #include "utils_corr_baryon.h"
+#include "utils_corr_seq.h"
 
-
-#undef  EigenMTa
-#undef  EigenVTa
+#undef  EigenTy
+///#undef  EigenMTa
+//#undef  EigenVTa
 #undef  EAy
-#undef  EAa
+//#undef  EAa
 
 
 #endif
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_corr_baryon.h` & `qlat-0.9/include/qlat/vector_utils/utils_corr_baryon.h`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,528 @@
 #include "utils_reduce_vec.h"
 #include "utils_grid_src.h"
 #include "utils_io_vec.h"
 #include "utils_corr_prop.h"
 
 namespace qlat{
 
+////simple gpu version, under Yi-bo's implimentation
+///////Proton contractions, for checks only
+template <typename Ty>
+void proton_vectorE(std::vector<qpropT >& prop1, std::vector<qpropT >& prop2, std::vector<qpropT >& prop3,
+  qlat::vector_acc<Ty > &res, const ga_M &ga2,const int ind2, const ga_M &ga1, const int ind1, int clear=1){
+  TIMER("Proton_vectorE");
+  if(prop1.size() == 0){res.resize(0); return ;}
+  const qlat::Geometry &geo = prop1[0].geo();
+  fft_desc_basic& fd = get_fft_desc_basic_plan(geo);
+
+  ////ga2/ind2 for source, gam1/ind1 for sink
+  ////"[]|+N" type diagram
+  //check_prop_size(prop1);check_prop_size(prop2);check_prop_size(prop3);
+  int NTt  = fd.Nv[3];
+  LInt Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
+  int nmass = prop1.size();
+  qassert(prop1.size() == prop2.size());
+  qassert(prop1.size() == prop3.size());
+  if(clear == 1){ini_resE(res, nmass, fd);}
+  if(clear == 0){qassert(res.size() == long(nmass*NTt * Nxyz));}
+    
+  ////Prop format, src d-4, c-3, sink d-4, c-3, Nt, EigenVTa<Nxyz>
+  if(res.size()%NTt !=0 or res.size()==0){print0("Size of res wrong. \n");qassert(false);}
+
+  qlat::vector_acc<Ty* > p1 = EigenM_to_pointers(prop1);
+  qlat::vector_acc<Ty* > p2 = EigenM_to_pointers(prop2);
+  qlat::vector_acc<Ty* > p3 = EigenM_to_pointers(prop3);
+
+  Ty epsl[3][3];
+  for(int i=0;i<3;i++)for(int j=0;j<3;j++){epsl[i][j] = 0;}
+  for(int i=0;i<3;i++){epsl[i][i]=0;epsl[i][(i+1)%3]=Ty(1,0);epsl[i][(i+2)%3]=Ty(-1,0);}
+
+  for(int d2=0;d2<4;d2++)
+  for(int c21=0;c21<3;c21++)
+  for(int ib=1;ib<3;ib++)
+  {
+    int c22=(c21+ib)%3,c23=(c22+ib)%3;
+    for(int d1=0;d1<4;d1++)
+    for(int c11=0;c11<3;c11++)
+    for(int ia=1;ia<3;ia++)
+    {
+      int c12=(c11+ia)%3,c13=(c12+ia)%3;
+      Ty giE = epsl[c11][c12]*epsl[c21][c22]*ga1.g[d1]*ga2.g[d2];
+
+      #pragma omp parallel for
+      for(int ji=0;ji<nmass*NTt;ji++)
+      {
+        int massi = ji/NTt;
+        int ti    = ji%NTt;
+
+        int m1 = (ind2*3+c21)*12+ind1*3+c11;
+        int m2 = (ga2.ind[d2]*3+c22)*12+d1*3+c12;
+        int m3 = (d2*3+c23)*12+ga1.ind[d1]*3+c13;
+
+        int n1 = (ind2*3+c21)*12+ga1.ind[d1]*3+c11;
+        int n2 = (ga2.ind[d2]*3+c22)*12+d1*3+c12;
+        int n3 = (d2*3+c23)*12+ind1*3+c13;
+
+        Ty* tp1 = &p1[massi][(m1*NTt+ti)*Nxyz];
+        Ty* tp2 = &p2[massi][(m2*NTt+ti)*Nxyz];
+        Ty* tp3 = &p3[massi][(m3*NTt+ti)*Nxyz];
+        Ty* tn1 = &p1[massi][(n1*NTt+ti)*Nxyz];
+        Ty* tn2 = &p2[massi][(n2*NTt+ti)*Nxyz];
+        Ty* tn3 = &p3[massi][(n3*NTt+ti)*Nxyz];
+        Ty* tr0 = &(res.data()[(massi*NTt + ti)*Nxyz]);
+
+        #if USEQACC==1
+        qacc_forNB(i, long(Nxyz),{ tr0[i] -= ((tp1[i]*tp2[i]*tp3[i] + tn1[i]*tn2[i]*tn3[i])*giE); });
+        #else
+        EAy vp1(tp1,Nxyz);
+        EAy vp2(tp2,Nxyz);
+        EAy vp3(tp3,Nxyz);
+        EAy vn1(tn1,Nxyz);
+        EAy vn2(tn2,Nxyz);
+        EAy vn3(tn3,Nxyz);
+        EAy vr0(tr0,Nxyz);
+        vr0 -= ((vp1*vp2*vp3 + vn1*vn2*vn3)*giE);
+        #endif
+
+      }
+      qacc_barrier(dummy);
+    }
+  }
+
+}
+
+
+///proton sector corr with prop gwu convention
+template <typename Ty>
+void proton_vectorE(std::vector<qpropT >& prop1, std::vector<qpropT >& prop2, std::vector<qpropT >& prop3,
+        qlat::vector_acc<Ty > &res, const ga_M &ga1,int t0,int dT,int clear=1,int oppo=0){
+  TIMER("Proton_vectorE");
+  if(prop1.size() == 0){res.resize(0); return;}
+
+  int nmass = prop1.size();
+  if(prop1.size() == 0){res.resize(0); return ;}
+  const qlat::Geometry &geo = prop1[0].geo();
+  fft_desc_basic& fd = get_fft_desc_basic_plan(geo);
+
+  int NTt  = fd.Nv[3];
+  LInt Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
+
+  qassert(prop1.size() == prop2.size());
+  qassert(prop1.size() == prop3.size());
+
+  if(clear == 1){ini_resE(res,nmass,fd);}
+
+  //int nv = res.size();int Nsize = res[0].size();
+  qlat::vector_acc<Ty >  resE0;resE0.resize(res.size());
+  qlat::vector_acc<Ty >  resE1;resE1.resize(res.size());
+  ////qlat::set_zero(resE0);qlat::set_zero(resE1);
+
+  proton_vectorE(prop1,prop2,prop3,resE0,ga1,0,ga1,0,1);
+  proton_vectorE(prop1,prop2,prop3,resE0,ga1,1,ga1,1,0);
+  proton_vectorE(prop1,prop2,prop3,resE1,ga1,2,ga1,2,1);
+  proton_vectorE(prop1,prop2,prop3,resE1,ga1,3,ga1,3,0);
+
+  std::vector<int > map_sec = get_map_sec(dT,fd.nt);
+  //////int Nt = fd.Nt;
+
+  /////int t0 = 0;
+  int nt = fd.nt;
+  ///for(int massi=0;massi<nmass;massi++)
+  ///for(int ti = 0;ti<Nt;ti++)
+  #pragma omp parallel for
+  for(int ji=0;ji<nmass*NTt;ji++)
+  {
+    int massi = ji/NTt;
+    int ti    = ji%NTt;
+    int t = ti + fd.Pos0[fd.rank][3];
+    Ty* tr0 = &(res.data()[(massi*NTt+ti)*Nxyz]);
+    Ty* tv0 = &(resE0.data()[(massi*NTt+ti)*Nxyz]);
+    Ty* tv1 = &(resE1.data()[(massi*NTt+ti)*Nxyz]);
+
+    #if USEQACC==0
+    EAy r0(tr0,Nxyz);
+    EAy v0(tv0,Nxyz);
+    EAy v1(tv1,Nxyz);
+    #endif
+
+    if(map_sec[(t-t0+nt)%nt]%2==0)
+    {
+      #if USEQACC==1
+      if(oppo==0)qacc_forNB(i, long(Nxyz), { tr0[i] += tv0[i]; });
+      if(oppo==1)qacc_forNB(i, long(Nxyz), { tr0[i] += tv1[i]; });
+      #else
+      if(oppo==0){r0 += v0;}
+      if(oppo==1){r0 += v1;}
+      #endif
+
+    }
+    if(map_sec[(t-t0+nt)%nt]%2==1)
+    {
+      #if USEQACC==1
+      if(oppo==0)qacc_forNB(i, long(Nxyz), { tr0[i] += tv1[i]; });
+      if(oppo==1)qacc_forNB(i, long(Nxyz), { tr0[i] += tv0[i]; });
+      #else
+      if(oppo==0){r0 += v1;}
+      if(oppo==1){r0 += v0;}
+      #endif
+
+    }
+  }
+  qacc_barrier(dummy);
+}
+
+////container
+template <typename Ty>
+void proton_corrE(std::vector<qpropT >& prop1, std::vector<qpropT >& prop2, std::vector<qpropT >& prop3,
+  const ga_M &ga2,const int ind2, const ga_M &ga1,const int ind1,
+  qlat::vector_acc<Ty > &res, int clear=1,const Coordinate& mom = Coordinate()){
+  qlat::vector_acc<Ty > resE;
+  proton_vectorE(prop1,prop2,prop3,ga2,ind2,ga1,ind1,resE,1);
+  vec_corrE(resE,res,clear,mom);
+}
+
+////container
+template <typename Ty>
+void proton_corrE(std::vector<qpropT >& prop1, std::vector<qpropT >& prop2, std::vector<qpropT >& prop3,
+ qlat::vector_acc<Ty > &res, const ga_M &ga1,const int t0,const int dT,int clear=1,const Coordinate& mom = Coordinate()){
+  qlat::vector_acc<Ty >  resE;
+  proton_vectorE(prop1,prop2,prop3,resE, ga1, t0,dT,1);
+
+  vec_corrE(resE,res,clear,mom);
+}
+
+////simple gpu version
+/////A source gamma, B sink Gamma, G projections with fermion sign, mL shape of diagram
+template <typename Ty>
+void baryon_vectorE(std::vector<qpropT >& prop1, std::vector<qpropT >& prop2, std::vector<qpropT >& prop3,
+  qlat::vector_acc<Ty > &res, ga_M &A, ga_M &B, qlat::vector_acc<Ty > &G, qlat::vector_acc<int > &mL, int clear=1){
+  TIMER("Proton_vectorE");
+  if(prop1.size() == 0){res.resize(0); return ;}
+  ////check_prop_size(prop1);check_prop_size(prop2);check_prop_size(prop3);
+  const qlat::Geometry &geo = prop1[0].geo();
+  fft_desc_basic& fd = get_fft_desc_basic_plan(geo);
+
+  int NTt  = fd.Nv[3];
+  LInt Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
+  int nmass = prop1.size();
+  qassert(prop1.size() == prop2.size());
+  qassert(prop1.size() == prop3.size());
+  qassert(G.size()  == 16);
+  qassert(mL.size() == 3);
+  qassert(fd.order_ch == 0);
+  if(clear == 1){ini_resE(res,nmass,fd);}
+
+  ////if(res.size()%NTt !=0 or res.size()==0){print0("Size of res wrong. \n");qassert(false);}
+  if(res.size()==0){print0("Size of res wrong. \n");qassert(false);}
+
+  qlat::vector_acc<Ty* > p1 = EigenM_to_pointers(prop1);
+  qlat::vector_acc<Ty* > p2 = EigenM_to_pointers(prop2);
+  qlat::vector_acc<Ty* > p3 = EigenM_to_pointers(prop3);
+
+  Ty epsl[3][3];
+  for(int i=0;i<3;i++)for(int j=0;j<3;j++){epsl[i][j] = 0;}
+  for(int i=0;i<3;i++){epsl[i][i]=0;epsl[i][(i+1)%3]=1;epsl[i][(i+2)%3]=-1;}
+
+  //mL = {};
+  //std::vector<int > mL;mL.resize(3);
+  //mL[0] = 0;mL[1] = 1;mL[2] = 2;
+  std::vector<int > nmL;nmL.resize(3);
+  std::vector<int > bmL;bmL.resize(3);
+
+  {
+    for(int a1=0;a1<3;a1++)
+    for(int ia=1;ia<3;ia++)
+    for(int b1=0;b1<3;b1++)
+    for(int ib=1;ib<3;ib++)
+    {
+      int b2=(b1+ib)%3,b3=(b2+ib)%3;
+      int a2=(a1+ia)%3,a3=(a2+ia)%3;
+      for(int m2=0;m2<4;m2++)
+      for(int m1=0;m1<4;m1++)
+      for(int n2=0;n2<4;n2++)
+      for(int n1=0;n1<4;n1++)
+      {
+        Ty Gv =  G[m1*4+n1];
+        double norm = std::sqrt(Gv.real()*Gv.real() + Gv.imag()*Gv.imag());
+        if(norm < 1e-20)continue;
+
+        int m3 = A.ind[m2];
+        int n3 = B.ind[n2];
+        Ty giE = epsl[a1][a2]*epsl[b1][b2]*A.g[m2]*B.g[n2]*G[m1*4+n1];
+        nmL[0] = n1;nmL[1] = n2;nmL[2] = n3;
+        bmL[0] = b1;bmL[1] = b2;bmL[2] = b3;
+        int nm1 = nmL[mL[0]];
+        int nm2 = nmL[mL[1]];
+        int nm3 = nmL[mL[2]];
+
+        int bm1 = bmL[mL[0]];
+        int bm2 = bmL[mL[1]];
+        int bm3 = bmL[mL[2]];
+
+        #pragma omp parallel for
+        for(int ji=0;ji<nmass*NTt;ji++)
+        {
+          int massi = ji/NTt;
+          int ti    = ji%NTt;
+
+          int o1 = (m1*3+a1)*12+(nm1*3+bm1);
+          int o2 = (m2*3+a2)*12+(nm2*3+bm2);
+          int o3 = (m3*3+a3)*12+(nm3*3+bm3);
+
+          Ty* tp1 = &p1[massi][(o1*NTt+ti)*Nxyz];
+          Ty* tp2 = &p2[massi][(o2*NTt+ti)*Nxyz];
+          Ty* tp3 = &p3[massi][(o3*NTt+ti)*Nxyz];
+          Ty* tr0 = &(res.data()[(massi*NTt + ti)*Nxyz]);
+
+          #if USEQACC==1
+          qacc_forNB(i, long(Nxyz),{ tr0[i] += (tp1[i]*tp2[i]*tp3[i] * giE); });
+          #else
+          EAy vp1(tp1,Nxyz);
+          EAy vp2(tp2,Nxyz);
+          EAy vp3(tp3,Nxyz);
+          EAy vr0(tr0,Nxyz);
+          vr0 += (vp1*vp2*vp3 * giE);
+          #endif
+
+        }
+        qacc_barrier(dummy);
+      }
+    }
+  }
+}
+
+////3pt insertion version
+////A source gamma, B sink Gamma, G projections with fermion sign, mL shape of diagram
+template <typename Ty>
+void baryon_vectorE(std::vector<qpropT >& prop1, std::vector<qpropT >& prop2, std::vector<qpropT >& prop3,
+  std::vector<qpropT >& resP, ga_M &A, ga_M &B, qlat::vector_acc<Ty > &G, qlat::vector_acc<int > &mL, int insertion,int clear=1)
+{
+  TIMER("Baryon_vectorE_insertion");
+  if(prop1.size() == 0){resP.resize(0); return ;}
+  ////check_prop_size(prop1);check_prop_size(prop2);check_prop_size(prop3);
+  const qlat::Geometry &geo = prop1[0].geo();
+  fft_desc_basic& fd = get_fft_desc_basic_plan(geo);
+  qassert(insertion == 0 or insertion == 1 or insertion == 2);
+
+  int NTt  = fd.Nv[3];
+  LInt Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
+  const int nmass = prop1.size();
+  qassert(prop1.size() == prop2.size());
+  qassert(prop1.size() == prop3.size());
+  qassert(G.size()  == 16);
+  qassert(mL.size() == 3);
+  qassert(fd.order_ch == 0);
+
+  if(clear==1){
+    if(int(resP.size()) != nmass){resP.resize(nmass);}
+    for(int mi=0;mi<nmass;mi++){
+      if(!resP[mi].initialized){resP[mi].init(geo);}
+      else{qlat::set_zero(resP[mi]);}
+    }
+  }
+  qassert(int(resP.size()) == nmass);
+  for(int mi=0;mi<nmass;mi++){qassert(resP[mi].initialized);}
+
+  /////check_prop_size(resP);
+
+  qlat::vector_acc<Ty* > p1 = EigenM_to_pointers(prop1);
+  qlat::vector_acc<Ty* > p2 = EigenM_to_pointers(prop2);
+  qlat::vector_acc<Ty* > p3 = EigenM_to_pointers(prop3);
+  qlat::vector_acc<Ty* > rP = EigenM_to_pointers(resP);
+
+  Ty epsl[3][3];
+  for(int i=0;i<3;i++)for(int j=0;j<3;j++){epsl[i][j] = 0;}
+  for(int i=0;i<3;i++){epsl[i][i]=0;epsl[i][(i+1)%3]=1;epsl[i][(i+2)%3]=-1;}
+
+  std::vector<int > nmL;nmL.resize(3);
+  std::vector<int > bmL;bmL.resize(3);
+
+  {
+    for(int a1=0;a1<3;a1++)
+    for(int ia=1;ia<3;ia++)
+    for(int b1=0;b1<3;b1++)
+    for(int ib=1;ib<3;ib++)
+    {
+      int b2=(b1+ib)%3,b3=(b2+ib)%3;
+      int a2=(a1+ia)%3,a3=(a2+ia)%3;
+      for(int m2=0;m2<4;m2++)
+      for(int m1=0;m1<4;m1++)
+      for(int n2=0;n2<4;n2++)
+      for(int n1=0;n1<4;n1++)
+      {
+        Ty Gv =  G[m1*4+n1];
+        double norm = std::sqrt(Gv.real()*Gv.real() + Gv.imag()*Gv.imag());
+        if(norm < 1e-20)continue;
+
+        int m3 = A.ind[m2];
+        int n3 = B.ind[n2];
+        Ty giE = epsl[a1][a2]*epsl[b1][b2]*A.g[m2]*B.g[n2]*G[m1*4+n1];
+        nmL[0] = n1;nmL[1] = n2;nmL[2] = n3;
+        bmL[0] = b1;bmL[1] = b2;bmL[2] = b3;
+        int nm1 = nmL[mL[0]];
+        int nm2 = nmL[mL[1]];
+        int nm3 = nmL[mL[2]];
+
+        int bm1 = bmL[mL[0]];
+        int bm2 = bmL[mL[1]];
+        int bm3 = bmL[mL[2]];
+
+        #pragma omp parallel for
+        for(int ji=0;ji<nmass*NTt;ji++)
+        {
+          int massi = ji/NTt;
+          int ti    = ji%NTt;
+
+          int o1 = (m1*3+a1)*12+(nm1*3+bm1);
+          int o2 = (m2*3+a2)*12+(nm2*3+bm2);
+          int o3 = (m3*3+a3)*12+(nm3*3+bm3);
+
+          int r0 = 0;
+          if(insertion == 0){r0 = (m1*3+a1)*12+(nm1*3+bm1);}
+          if(insertion == 1){r0 = (m2*3+a2)*12+(nm2*3+bm2);}
+          if(insertion == 2){r0 = (m3*3+a3)*12+(nm3*3+bm3);}
+
+          Ty* tp1 = &p1[massi][(o1*NTt+ti)*Nxyz];
+          Ty* tp2 = &p2[massi][(o2*NTt+ti)*Nxyz];
+          Ty* tp3 = &p3[massi][(o3*NTt+ti)*Nxyz];
+          Ty* tr0 = &rP[massi][(r0*NTt+ti)*Nxyz];
+
+          #if USEQACC==1
+          if(insertion == 0)qacc_forNB(i, long(Nxyz),{ tr0[i] += (tp2[i]*tp3[i] * giE); });
+          if(insertion == 1)qacc_forNB(i, long(Nxyz),{ tr0[i] += (tp1[i]*tp3[i] * giE); });
+          if(insertion == 2)qacc_forNB(i, long(Nxyz),{ tr0[i] += (tp1[i]*tp2[i] * giE); });
+          #else
+          EAy vp1(tp1,Nxyz);
+          EAy vp2(tp2,Nxyz);
+          EAy vp3(tp3,Nxyz);
+          EAy vr0(tr0,Nxyz);
+          if(insertion == 0){vr0 += vp2*vp3 * giE;}
+          if(insertion == 1){vr0 += vp1*vp3 * giE;}
+          if(insertion == 2){vr0 += vp1*vp2 * giE;}
+          #endif
+        }
+        qacc_barrier(dummy);
+      }
+    }
+  }
+
+}
+
+template <typename Ty>
+void baryon_vectorE(std::vector<qpropT >& prop1, std::vector<qpropT >& prop2, std::vector<qpropT >& prop3,
+  std::vector< std::vector<qpropT > >& resP, const int ud, const std::vector<int >& map_sec, std::vector< std::vector<qpropT > >& buf) 
+{
+  if(prop1.size() == 0){resP.resize(0); return ;}
+  const qlat::Geometry &geo = prop1[0].geo();
+  fft_desc_basic& fd = get_fft_desc_basic_plan(geo);
+
+  const long Nt = fd.Nt;
+  const long Nxyz = fd.Nx * fd.Ny * fd.Nz;
+  ga_matrices_cps   ga_cps;
+  ga_M& A = ga_cps.ga[1][3];
+  ga_M& B = ga_cps.ga[1][3];
+
+  ////get all 4 prj
+  if(buf.size() != 16){buf.resize(16);}
+  for(int i=0;i<16;i++){
+    init_qpropT(buf[i], prop1.size(), geo);
+    clear_qpropT(buf[i]);
+  }
+  if(resP.size()!=4){resP.resize(4);}
+  for(int i=0;i<4;i++){
+    init_qpropT(resP[i], prop1.size(), geo);
+    {clear_qpropT(resP[i]);} ////must clear!
+  }
+
+  std::vector<Ty > factor(4);
+  factor[0] = 1.0/2.0;
+  //for(int i=1;i<4;i++){factor[i] = Ty(0.0, 1.0/2.0);}
+  for(int i=1;i<4;i++){factor[i] = Ty(1.0/2.0, 0.0);}  ///complex sign convention here?
+
+  std::vector<ga_M > gL(8);
+  gL[0] = ga_cps.ga[0][0];gL[1] = ga_cps.ga[0][4];
+
+  for(int i=1;i<4;i++){
+    gL[i*2 + 0] =                   ga_cps.ga[i][5]; ////need reverse or not
+    gL[i*2 + 1] = ga_cps.ga[0][4] * ga_cps.ga[i][5];
+  }
+
+  std::vector<int > udL = {0,0,  1};
+
+  qlat::vector_acc<Ty > G;G.resize(16);
+  qlat::vector_acc<int > mL;mL.resize(3);
+
+  //std::vector<int > inL = {0,0,  1,1,  2,2,  3,3,  0,2,  1,3,  2,0,  3,1 };
+  //for(int ind=0;ind<8;ind++)
+  //for(int insertion=0;insertion<3;insertion++)
+  //{   
+  //  if(udL[insertion] == ud) 
+  //  {   
+  //    int ind1 = inL[ind*2 + 0];
+  //    int ind2 = inL[ind*2 + 1];
+  //    clear_qv(G);G[ind2*4 + ind1] = +1.0/2.0; //// (1+r4)/2, could be non-zero for all elements...
+  //    mL[0] = 0;mL[1] = 1;mL[2] = 2;
+  //    baryon_vectorE(prop1, prop2, prop3, resP[0], A, B, G, mL, insertion, 0); 
+  //    ////baryon_vectorE(prop1,prop2,prop3, resE, ga2,ga1, G, mL, fd, 1); 
+  //    clear_qv(G);G[ind2*4 + ind1] = -1.0/2.0;
+  //    mL[0] = 1;mL[1] = 0;mL[2] = 2;
+  //    baryon_vectorE(prop1, prop2, prop3, resP[0], A, B, G, mL, insertion, 0); //// no clear sum
+  //  }   
+  //}
+
+  for(int ind=0;ind<16;ind++)
+  for(int insertion=0;insertion<3;insertion++)
+  {   
+    if(udL[insertion] == ud) 
+    {   
+      int ind1 = ind/4;
+      int ind2 = ind%4;
+      qlat::vector_acc<Ty > G;G.resize(16);
+      qlat::vector_acc<int > mL;mL.resize(3);
+      clear_qv(G);G[ind2*4 + ind1] = +1.0/1.0; //// (1+r4)/2, could be non-zero for all elements...
+      mL[0] = 0;mL[1] = 1;mL[2] = 2;
+      baryon_vectorE(prop1, prop2, prop3, buf[ind], A, B, G, mL, insertion, 0); 
+      ////baryon_vectorE(prop1,prop2,prop3, resE, ga2,ga1, G, mL, fd, 1); 
+      clear_qv(G);G[ind2*4 + ind1] = -1.0/1.0;
+      mL[0] = 1;mL[1] = 0;mL[2] = 2;
+      baryon_vectorE(prop1, prop2, prop3, buf[ind], A, B, G, mL, insertion, 0); //// no clear sum
+    }   
+  }
+
+
+  for(int prj=0;prj<4;prj++)
+  {
+    for(int ti = 0; ti < Nt; ti++)
+    {
+      int seci = map_sec[ti + fd.init]%2;
+      for(int si = 0; si < 2 ;si++)//// 1 + r4 sectors
+      for(int gd=0;gd<4;gd++)
+      {
+        Ty sign  = gL[prj*2 + si].g[gd]           * factor[prj];
+        int bind = gL[prj*2 + si].ind[gd]*4 + gd ; //// need reverse or not
+
+        if(seci == 1 and si == 1){sign = (-1.0) * sign;} //// reverse sign if seci == 1
+        for(int da = 0; da < 12*12; da++)
+        for(unsigned int vi = 0; vi < prop1.size();vi++)
+        {
+          Ty* src = (Ty*) qlat::get_data(buf[bind][vi]).data();
+          Ty* res = (Ty*) qlat::get_data(resP[prj][vi]).data();
+          const long off_d = da*Nt*Nxyz + ti*Nxyz;
+          cpy_data_threadC(&res[off_d], &src[off_d], Nxyz, 1, false, sign);
+        }
+        qacc_barrier(dummy);
+      }
+    }
+  }
+
+}
+
+
+
 #ifdef QLAT_USE_ACC
 template<typename Ty, int bfac, int Blocks>
 __global__ void baryon_vectorEV_global(Ty** p1, Ty** p2, Ty** p3, Ty* resP,
   char** gPP, unsigned char** oPP, const int* ivP,
   const int nmass, const int NTt, const long Nxyz, const int Ngv)
 {
   //unsigned long gi =  blockIdx.x*blockDim.x + threadIdx.x;
@@ -413,447 +927,92 @@
     }
   }
   #endif
 
 }
 
 ////container 
-template <typename Ta>
-void baryon_vectorEV(EigenMTa &prop1, EigenMTa &prop2, EigenMTa &prop3, EigenVTa &res,
-  ga_M &A, ga_M &B, qlat::vector_acc<Ta > &GV, qlat::vector_acc<int > &mLV,
-  fft_desc_basic &fd,int clear=1){
+template <typename Ty>
+void baryon_vectorEV(EigenTy& prop1, EigenTy& prop2, EigenTy& prop3,
+  qlat::vector_gpu<Ty > &res, ga_M &A, ga_M &B, qlat::vector_acc<Ty > &GV, qlat::vector_acc<int > &mLV,
+  fft_desc_basic& fd, int clear=1){
+
+  if(prop1.size() == 0){res.resize(0); return ;}
+  check_prop_size(prop1, fd);check_prop_size(prop2, fd);check_prop_size(prop3, fd);
+
   int NTt  = fd.Nv[3];
   long Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
-
-  check_prop_size(prop1);check_prop_size(prop2);check_prop_size(prop3);
-  int nmass = prop1.size()/(12*12*NTt);
+  ////check_prop_size(prop1);check_prop_size(prop2);check_prop_size(prop3);
+  int nmass = prop1.size();
   qassert(prop1.size() == prop2.size());
   qassert(prop1.size() == prop3.size());
   int Ngv = GV.size()/16;
-  long resL = Ngv * nmass*NTt * Nxyz;
+  const unsigned long resL = Ngv * nmass*NTt * Nxyz;
   if(clear == 1){if(res.size()!= resL){res.resize(resL); } }
   if(res.size() != resL){print0("Size of res wrong. \n");qassert(false);}
 
-  qlat::vector_acc<Ta* > prop1P = EigenM_to_pointers(prop1);
-  qlat::vector_acc<Ta* > prop2P = EigenM_to_pointers(prop2);
-  qlat::vector_acc<Ta* > prop3P = EigenM_to_pointers(prop3);
-  Ta** p1 = prop1P.data();
-  Ta** p2 = prop2P.data();
-  Ta** p3 = prop3P.data();
-  Ta* resP = res.data();
+  qlat::vector_acc<Ty* > prop1P = EigenM_to_pointers(prop1, Nxyz);
+  qlat::vector_acc<Ty* > prop2P = EigenM_to_pointers(prop2, Nxyz);
+  qlat::vector_acc<Ty* > prop3P = EigenM_to_pointers(prop3, Nxyz);
+  Ty** p1 = prop1P.data();
+  Ty** p2 = prop2P.data();
+  Ty** p3 = prop3P.data();
+  Ty* resP = res.data();
 
   baryon_vectorEV(p1, p2, p3, resP, nmass, A, B, GV, mLV, fd, clear);
 }
 
-////simple gpu version
-///////Proton contractions
-template <typename Ta>
-void proton_vectorE(EigenMTa &prop1, EigenMTa &prop2, EigenMTa &prop3,
-  const ga_M &ga2,const int ind2, const ga_M &ga1, const int ind1,
-      EigenVTa &res, fft_desc_basic &fd,int clear=1){
-  TIMER("Proton_vectorE");
-  ////ga2/ind2 for source, gam1/ind1 for sink
-  ////"[]|+N" type diagram
-  check_prop_size(prop1);check_prop_size(prop2);check_prop_size(prop3);
-  int NTt  = fd.Nv[3];
-  LInt Nxyz = prop1[0].size();
-  int nmass = prop1.size()/(12*12*NTt);
-  qassert(prop1.size() == prop2.size());
-  qassert(prop1.size() == prop3.size());
-  if(clear == 1){ini_resE(res,nmass,fd);}
-  if(clear == 0){qassert(res.size() == long(nmass*NTt * Nxyz));}
-    
-  ////Prop format, src d-4, c-3, sink d-4, c-3, Nt, EigenVTa<Nxyz>
-  if(res.size()%NTt !=0 or res.size()==0){print0("Size of res wrong. \n");qassert(false);}
-
-  Ta epsl[3][3];
-  for(int i=0;i<3;i++)for(int j=0;j<3;j++){epsl[i][j] = 0;}
-  for(int i=0;i<3;i++){epsl[i][i]=0;epsl[i][(i+1)%3]=Ta(1,0);epsl[i][(i+2)%3]=Ta(-1,0);}
-
-  for(int d2=0;d2<4;d2++)
-  for(int c21=0;c21<3;c21++)
-  for(int ib=1;ib<3;ib++)
-  {
-    int c22=(c21+ib)%3,c23=(c22+ib)%3;
-    for(int d1=0;d1<4;d1++)
-    for(int c11=0;c11<3;c11++)
-    for(int ia=1;ia<3;ia++)
-    {
-      int c12=(c11+ia)%3,c13=(c12+ia)%3;
-      Ta giE = epsl[c11][c12]*epsl[c21][c22]*ga1.g[d1]*ga2.g[d2];
-
-      #pragma omp parallel for
-      for(int ji=0;ji<nmass*NTt;ji++)
-      {
-        int massi = ji/NTt;
-        int ti    = ji%NTt;
-
-        int m1 = massi*12*12 + (ind2*3+c21)*12+ind1*3+c11;
-        int m2 = massi*12*12 + (ga2.ind[d2]*3+c22)*12+d1*3+c12;
-        int m3 = massi*12*12 + (d2*3+c23)*12+ga1.ind[d1]*3+c13;
-
-        int n1 = massi*12*12 + (ind2*3+c21)*12+ga1.ind[d1]*3+c11;
-        int n2 = massi*12*12 + (ga2.ind[d2]*3+c22)*12+d1*3+c12;
-        int n3 = massi*12*12 + (d2*3+c23)*12+ind1*3+c13;
-
-        Ta* tp1 = prop1[m1*NTt+ti].data();
-        Ta* tp2 = prop2[m2*NTt+ti].data();
-        Ta* tp3 = prop3[m3*NTt+ti].data();
-        Ta* tn1 = prop1[n1*NTt+ti].data();
-        Ta* tn2 = prop2[n2*NTt+ti].data();
-        Ta* tn3 = prop3[n3*NTt+ti].data();
-        Ta* tr0 = &(res.data()[(massi*NTt + ti)*Nxyz]);
-
-        #if USEQACC==1
-        qacc_forNB(i, long(Nxyz),{ tr0[i] -= ((tp1[i]*tp2[i]*tp3[i] + tn1[i]*tn2[i]*tn3[i])*giE); });
-        #else
-        EAa vp1(tp1,Nxyz);
-        EAa vp2(tp2,Nxyz);
-        EAa vp3(tp3,Nxyz);
-        EAa vn1(tn1,Nxyz);
-        EAa vn2(tn2,Nxyz);
-        EAa vn3(tn3,Nxyz);
-        EAa vr0(tr0,Nxyz);
-        vr0 -= ((vp1*vp2*vp3 + vn1*vn2*vn3)*giE);
-        #endif
 
-      }
-      qacc_barrier(dummy);
-    }
-  }
-
-}
-
-///container for 
-template <typename Ta>
-void proton_vectorE(EigenMTa &prop1, EigenMTa &prop2, EigenMTa &prop3,
-        EigenVTa &res, fft_desc_basic &fd, const ga_M &ga1,int t0,int dT,int clear=1,int oppo=0){
-  TIMER("Proton_vectorE");
-  int NTt  = fd.Nv[3];
-  LInt Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
-  int nmass = prop1.size()/(12*12*NTt);
-  qassert(prop1.size() == prop2.size());
-  qassert(prop1.size() == prop3.size());
-
-  if(clear == 1){ini_resE(res,nmass,fd);}
-
-  //int nv = res.size();int Nsize = res[0].size();
-  EigenVTa resE0;resE0.resize(res.size());
-  EigenVTa resE1;resE1.resize(res.size());
-  ////qlat::set_zero(resE0);qlat::set_zero(resE1);
-
-  proton_vectorE(prop1,prop2,prop3,ga1,0,ga1,0,resE0,fd,1);
-  proton_vectorE(prop1,prop2,prop3,ga1,1,ga1,1,resE0,fd,0);
-  proton_vectorE(prop1,prop2,prop3,ga1,2,ga1,2,resE1,fd,1);
-  proton_vectorE(prop1,prop2,prop3,ga1,3,ga1,3,resE1,fd,0);
-
-  std::vector<int > map_sec = get_sec_map(dT,fd.nt);
-  //////int Nt = fd.Nt;
-
-  /////int t0 = 0;
-  int nt = fd.nt;
-  ///for(int massi=0;massi<nmass;massi++)
-  ///for(int ti = 0;ti<Nt;ti++)
-  #pragma omp parallel for
-  for(int ji=0;ji<nmass*NTt;ji++)
-  {
-    int massi = ji/NTt;
-    int ti    = ji%NTt;
-    int t = ti + fd.Pos0[fd.rank][3];
-    Ta* tr0 = &(res.data()[(massi*NTt+ti)*Nxyz]);
-    Ta* tv0 = &(resE0.data()[(massi*NTt+ti)*Nxyz]);
-    Ta* tv1 = &(resE1.data()[(massi*NTt+ti)*Nxyz]);
-
-    #if USEQACC==0
-    EAa r0(tr0,Nxyz);
-    EAa v0(tv0,Nxyz);
-    EAa v1(tv1,Nxyz);
-    #endif
-
-    if(map_sec[(t-t0+nt)%nt]%2==0)
-    {
-      #if USEQACC==1
-      if(oppo==0)qacc_forNB(i, long(Nxyz), { tr0[i] += tv0[i]; });
-      if(oppo==1)qacc_forNB(i, long(Nxyz), { tr0[i] += tv1[i]; });
-      #else
-      if(oppo==0){r0 += v0;}
-      if(oppo==1){r0 += v1;}
-      #endif
-
-    }
-    if(map_sec[(t-t0+nt)%nt]%2==1)
-    {
-      #if USEQACC==1
-      if(oppo==0)qacc_forNB(i, long(Nxyz), { tr0[i] += tv1[i]; });
-      if(oppo==1)qacc_forNB(i, long(Nxyz), { tr0[i] += tv0[i]; });
-      #else
-      if(oppo==0){r0 += v1;}
-      if(oppo==1){r0 += v0;}
-      #endif
-
-    }
-  }
-  qacc_barrier(dummy);
-}
-
-////container
-template <typename Ta>
-void proton_corrE(EigenMTa &prop1, EigenMTa &prop2, EigenMTa &prop3,
-  const ga_M &ga2,const int ind2, const ga_M &ga1,const int ind1,
-  EigenVTa &res, fft_desc_basic &fd,int clear=1,const Coordinate& mom = Coordinate()){
-  EigenVTa resE;
-  proton_vectorE(prop1,prop2,prop3,ga2,ind2,ga1,ind1,resE,fd,1);
-  vec_corrE(resE,res,fd,clear,mom);
-}
-
-////container
-template <typename Ta>
-void proton_corrE(EigenMTa &prop1, EigenMTa &prop2, EigenMTa &prop3,
- EigenVTa &res, fft_desc_basic &fd, const ga_M &ga1,const int t0,const int dT,int clear=1,const Coordinate& mom = Coordinate()){
-  EigenVTa resE;
-  proton_vectorE(prop1,prop2,prop3,resE,fd, ga1, t0,dT,1);
-
-  vec_corrE(resE,res,fd,clear,mom);
-}
-
-
-////simple gpu version
-/////A source gamma, B sink Gamma, G projections with fermion sign, mL shape of diagram
-template <typename Ta>
-void baryon_vectorE(EigenMTa &prop1, EigenMTa &prop2, EigenMTa &prop3,
-  ga_M &A, ga_M &B, qlat::vector_acc<Ta > &G, qlat::vector_acc<int > &mL,
-        EigenVTa &res, fft_desc_basic &fd,int clear=1){
-  TIMER("Proton_vectorE");
-  check_prop_size(prop1);check_prop_size(prop2);check_prop_size(prop3);
-  int NTt  = fd.Nv[3];
-  LInt Nxyz = prop1[0].size();
-  int nmass = prop1.size()/(12*12*NTt);
-  qassert(prop1.size() == prop2.size());
-  qassert(prop1.size() == prop3.size());
-  qassert(G.size()  == 16);
-  qassert(mL.size() == 3);
-  if(clear == 1){ini_resE(res,nmass,fd);}
 
-  //if(res.size()%NTt !=0 or res.size()==0){print0("Size of res wrong. \n");qassert(false);}
-  if(res.size()==0){print0("Size of res wrong. \n");qassert(false);}
-
-  Ta epsl[3][3];
-  for(int i=0;i<3;i++)for(int j=0;j<3;j++){epsl[i][j] = 0;}
-  for(int i=0;i<3;i++){epsl[i][i]=0;epsl[i][(i+1)%3]=1;epsl[i][(i+2)%3]=-1;}
-
-  //mL = {};
-  //std::vector<int > mL;mL.resize(3);
-  //mL[0] = 0;mL[1] = 1;mL[2] = 2;
-  std::vector<int > nmL;nmL.resize(3);
-  std::vector<int > bmL;bmL.resize(3);
-
-  {
-    for(int a1=0;a1<3;a1++)
-    for(int ia=1;ia<3;ia++)
-    for(int b1=0;b1<3;b1++)
-    for(int ib=1;ib<3;ib++)
-    {
-      int b2=(b1+ib)%3,b3=(b2+ib)%3;
-      int a2=(a1+ia)%3,a3=(a2+ia)%3;
-      for(int m2=0;m2<4;m2++)
-      for(int m1=0;m1<4;m1++)
-      for(int n2=0;n2<4;n2++)
-      for(int n1=0;n1<4;n1++)
-      {
-        Ta Gv =  G[m1*4+n1];
-        double norm = std::sqrt(Gv.real()*Gv.real() + Gv.imag()*Gv.imag());
-        if(norm < 1e-20)continue;
-
-        int m3 = A.ind[m2];
-        int n3 = B.ind[n2];
-        Ta giE = epsl[a1][a2]*epsl[b1][b2]*A.g[m2]*B.g[n2]*G[m1*4+n1];
-        nmL[0] = n1;nmL[1] = n2;nmL[2] = n3;
-        bmL[0] = b1;bmL[1] = b2;bmL[2] = b3;
-        int nm1 = nmL[mL[0]];
-        int nm2 = nmL[mL[1]];
-        int nm3 = nmL[mL[2]];
-
-        int bm1 = bmL[mL[0]];
-        int bm2 = bmL[mL[1]];
-        int bm3 = bmL[mL[2]];
-
-        #pragma omp parallel for
-        for(int ji=0;ji<nmass*NTt;ji++)
-        {
-          int massi = ji/NTt;
-          int ti    = ji%NTt;
-
-          int o1 = massi*12*12 + (m1*3+a1)*12+(nm1*3+bm1);
-          int o2 = massi*12*12 + (m2*3+a2)*12+(nm2*3+bm2);
-          int o3 = massi*12*12 + (m3*3+a3)*12+(nm3*3+bm3);
-
-          Ta* tp1 = prop1[o1*NTt+ti].data();
-          Ta* tp2 = prop2[o2*NTt+ti].data();
-          Ta* tp3 = prop3[o3*NTt+ti].data();
-          Ta* tr0 = &(res.data()[(massi*NTt + ti)*Nxyz]);
-
-          #if USEQACC==1
-          qacc_forNB(i, long(Nxyz),{ tr0[i] += (tp1[i]*tp2[i]*tp3[i] * giE); });
-          #else
-          EAa vp1(tp1,Nxyz);
-          EAa vp2(tp2,Nxyz);
-          EAa vp3(tp3,Nxyz);
-          EAa vr0(tr0,Nxyz);
-          vr0 += (vp1*vp2*vp3 * giE);
-          #endif
-
-        }
-        qacc_barrier(dummy);
-      }
-    }
-  }
-
-}
-
-////3pt insertion version
-////A source gamma, B sink Gamma, G projections with fermion sign, mL shape of diagram
-template <typename Ta>
-void baryon_vectorE(EigenMTa &prop1, EigenMTa &prop2, EigenMTa &prop3,
-  ga_M &A, ga_M &B, qlat::vector_acc<Ta > &G, qlat::vector_acc<int > &mL, int insertion,
-        EigenMTa &resP, fft_desc_basic &fd,int clear=1)
-{
-  TIMER("Baryon_vectorE_insertion");
-  check_prop_size(prop1);check_prop_size(prop2);check_prop_size(prop3);
-  int NTt  = fd.Nv[3];
-  LInt Nxyz = prop1[0].size();
-  int nmass = prop1.size()/(12*12*NTt);
-  qassert(prop1.size() == prop2.size());
-  qassert(prop1.size() == prop3.size());
-  qassert(G.size()  == 16);
-  qassert(mL.size() == 3);
-  qassert(fd.order_ch == 0);
-
-  if(clear==1){ini_propE(resP,nmass,fd);}
-  /////check_prop_size(resP);
-
-  Ta epsl[3][3];
-  for(int i=0;i<3;i++)for(int j=0;j<3;j++){epsl[i][j] = 0;}
-  for(int i=0;i<3;i++){epsl[i][i]=0;epsl[i][(i+1)%3]=1;epsl[i][(i+2)%3]=-1;}
-
-  std::vector<int > nmL;nmL.resize(3);
-  std::vector<int > bmL;bmL.resize(3);
-
-  {
-    for(int a1=0;a1<3;a1++)
-    for(int ia=1;ia<3;ia++)
-    for(int b1=0;b1<3;b1++)
-    for(int ib=1;ib<3;ib++)
-    {
-      int b2=(b1+ib)%3,b3=(b2+ib)%3;
-      int a2=(a1+ia)%3,a3=(a2+ia)%3;
-      for(int m2=0;m2<4;m2++)
-      for(int m1=0;m1<4;m1++)
-      for(int n2=0;n2<4;n2++)
-      for(int n1=0;n1<4;n1++)
-      {
-        Ta Gv =  G[m1*4+n1];
-        double norm = std::sqrt(Gv.real()*Gv.real() + Gv.imag()*Gv.imag());
-        if(norm < 1e-20)continue;
-
-        int m3 = A.ind[m2];
-        int n3 = B.ind[n2];
-        Ta giE = epsl[a1][a2]*epsl[b1][b2]*A.g[m2]*B.g[n2]*G[m1*4+n1];
-        nmL[0] = n1;nmL[1] = n2;nmL[2] = n3;
-        bmL[0] = b1;bmL[1] = b2;bmL[2] = b3;
-        int nm1 = nmL[mL[0]];
-        int nm2 = nmL[mL[1]];
-        int nm3 = nmL[mL[2]];
-
-        int bm1 = bmL[mL[0]];
-        int bm2 = bmL[mL[1]];
-        int bm3 = bmL[mL[2]];
-
-        #pragma omp parallel for
-        for(int ji=0;ji<nmass*NTt;ji++)
-        {
-          int massi = ji/NTt;
-          int ti    = ji%NTt;
-
-          int o1 = massi*12*12 + (m1*3+a1)*12+(nm1*3+bm1);
-          int o2 = massi*12*12 + (m2*3+a2)*12+(nm2*3+bm2);
-          int o3 = massi*12*12 + (m3*3+a3)*12+(nm3*3+bm3);
-
-          int r0 = 0;
-          if(insertion == 0){r0 = massi*12*12 + (m1*3+a1)*12+(nm1*3+bm1);}
-          if(insertion == 1){r0 = massi*12*12 + (m2*3+a2)*12+(nm2*3+bm2);}
-          if(insertion == 2){r0 = massi*12*12 + (m3*3+a3)*12+(nm3*3+bm3);}
-
-          Ta* tp1 = prop1[o1*NTt+ti].data();
-          Ta* tp2 = prop2[o2*NTt+ti].data();
-          Ta* tp3 = prop3[o3*NTt+ti].data();
-          Ta* tr0 = resP[r0*NTt+ti].data();
-
-          #if USEQACC==1
-          if(insertion == 0)qacc_forNB(i, long(Nxyz),{ tr0[i] += (tp2[i]*tp3[i] * giE); });
-          if(insertion == 1)qacc_forNB(i, long(Nxyz),{ tr0[i] += (tp1[i]*tp3[i] * giE); });
-          if(insertion == 2)qacc_forNB(i, long(Nxyz),{ tr0[i] += (tp1[i]*tp2[i] * giE); });
-          #else
-          EAa vp1(tp1,Nxyz);
-          EAa vp2(tp2,Nxyz);
-          EAa vp3(tp3,Nxyz);
-          EAa vr0(tr0,Nxyz);
-          if(insertion == 0){vr0 += vp2*vp3 * giE;}
-          if(insertion == 1){vr0 += vp1*vp3 * giE;}
-          if(insertion == 2){vr0 += vp1*vp2 * giE;}
-          #endif
-        }
-        qacc_barrier(dummy);
-      }
-    }
-  }
-
-}
-
-template <typename Ta>
-void baryon_corrE(EigenMTa &prop1, EigenMTa &prop2, EigenMTa &prop3,
-   ga_M &ga2,int ind2,ga_M &ga1,int ind1,
-  EigenVTa &res, fft_desc_basic &fd,int clear=1,const Coordinate& mom = Coordinate())
+template <typename Ty>
+void baryon_corrE(EigenTy& prop1, EigenTy& prop2, EigenTy& prop3,
+  qlat::vector_gpu<Ty > &res,  ga_M &ga2,int ind2,ga_M &ga1,int ind1,
+  fft_desc_basic& fd, int clear=1,const Coordinate& mom = Coordinate())
 {
+  if(prop1.size() == 0){res.resize(0); return ;}
   int NTt  = fd.Nv[3];
   ////LInt Nxyz = prop1[0].size();
-  int nmass = prop1.size()/(12*12*NTt);
+  int nmass = prop1.size();
   ////int nt = fd.nt;
 
-  EigenVTa resE;
-  ini_resE(resE,nmass,fd);
+  qlat::vector_acc<Ty > resE;
+  ini_resE(resE, nmass,fd);
 
-  qlat::vector_acc<Ta > G;G.resize(16);
+  qlat::vector_acc<Ty > G;G.resize(16);
   qlat::vector_acc<int > mL;mL.resize(3);
 
   clear_qv(G);G[ind2*4 + ind1] = +1.0;
   mL[0] = 0;mL[1] = 1;mL[2] = 2;
-  baryon_vectorE(prop1,prop2,prop3, ga2,ga1, G, mL, resE, fd, 1);
+  baryon_vectorE(prop1,prop2,prop3, resE, ga2,ga1, G, mL, fd, 1);
   clear_qv(G);G[ind2*4 + ind1] = -1.0;
   mL[0] = 1;mL[1] = 0;mL[2] = 2;
-  baryon_vectorE(prop1,prop2,prop3, ga2,ga1, G, mL, resE, fd, 0);
+  baryon_vectorE(prop1,prop2,prop3, resE, ga2,ga1, G, mL, fd, 0);
 
   ////proton_vectorE(prop1,prop2,prop3,ga2,ind2,ga1,ind1,resE,fd,1);
 
   vec_corrE(resE,res,fd,clear,mom);
 }
 
-template <typename Ta>
-void Omega_corrE(EigenMTa &prop1, EigenMTa &prop2, EigenMTa &prop3,
-   ga_M &ga2,int ind2,ga_M &ga1,int ind1,
-  EigenVTa &res, fft_desc_basic &fd,int clear=1,const Coordinate& mom = Coordinate())
+template <typename Ty>
+void Omega_corrE(EigenTy& prop1, EigenTy& prop2, EigenTy& prop3,
+  qlat::vector_gpu<Ty > &res, ga_M &ga2,int ind2,ga_M &ga1,int ind1, int clear=1,const Coordinate& mom = Coordinate())
 {
+  if(prop1.size() == 0){res.resize(0); return ;}
+  const qlat::Geometry &geo = prop1[0].geo();
+  fft_desc_basic& fd = get_fft_desc_basic_plan(geo);
+
   int NTt  = fd.Nv[3];
   ///LInt Nxyz = prop1[0].size();
-  int nmass = prop1.size()/(12*12*NTt);
+  int nmass = prop1.size();
   ///int nt = fd.nt;
 
-  EigenVTa resE;
+  qlat::vector_acc<Ty > resE;
   ini_resE(resE,nmass,fd);
 
-  qlat::vector_acc<Ta > G;G.resize(16);
+  qlat::vector_acc<Ty > G;G.resize(16);
   qlat::vector_acc<int > mL;mL.resize(3);
 
   std::vector<int > dia;dia.resize(6);
   std::vector<int > sn ;sn.resize(6);
   dia[0] = 9012;sn[0] =  1;
   dia[1] = 9102;sn[1] = -1;
   dia[2] = 9021;sn[2] = -1;
@@ -861,15 +1020,15 @@
   dia[4] = 9210;sn[4] = -1;
   dia[5] = 9120;sn[5] =  1;
 
   for(int di=0;di<6;di++)
   {
     clear_qv(G);G[ind2*4 + ind1] = sn[di];
     mL[0] = (dia[di]/100)%10;mL[1] =  (dia[di]%100)/10;mL[2] = dia[di]%10;
-    baryon_vectorE(prop1,prop2,prop3, ga2,ga1, G, mL, resE, fd, 0);
+    baryon_vectorE(prop1,prop2,prop3, resE, ga2,ga1, G, mL, fd, 0);
   }
      
   ////clear_qv(G);G[ind2*4 + ind1] = +1.0;
   ////mL[0] = 0;mL[1] = 1;mL[2] = 2;
   ////baryon_vectorE(prop1,prop2,prop3, ga2,ga1, G, mL, resE, fd, 0);
 
   ////clear_qv(G);G[ind2*4 + ind1] = -1.0;
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_corr_meson.h` & `qlat-0.9/include/qlat/vector_utils/utils_corr_meson.h`

 * *Files 20% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 #include "utils_reduce_vec.h"
 #include "utils_grid_src.h"
 #include "utils_io_vec.h"
 #include "utils_corr_prop.h"
 
 namespace qlat{
 
-template <typename Ty, typename Ta >
-void meson_vectorE(std::vector<Propagator4dT<Ty > > &pV1, std::vector<Propagator4dT<Ty > > &pV2, ga_M &ga1,ga_M &ga2,
-        EigenVTa &res, qlat::fft_desc_basic &fd,int clear=1){
+////ga1 sink gammas, ga2 src gammas
+template <typename Td>
+void meson_vectorE(std::vector<Propagator4dT<Td > > &pV1, std::vector<Propagator4dT<Td > > &pV2, ga_M &ga1,ga_M &ga2,
+        qlat::vector_acc<qlat::ComplexT<Td > > &res, qlat::fft_desc_basic &fd,int clear=1){
   TIMER("Meson_vectorE");
   qassert(fd.order_ch == 0);
   ///////check_prop_size(prop1);check_prop_size(prop2);
   int  NTt  = fd.Nv[3];
   LInt Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
   int  nmass = pV1.size();
   if(nmass == 0){res.resize(0);return;}
@@ -31,125 +32,201 @@
   if(clear == 1){ini_resE(res,nmass,fd);}
 
   if(res.size()%NTt !=0 or res.size()==0){print0("Size of res wrong. \n");qassert(false);}
   qassert(pV1.size() == pV2.size());
 
   for(int mi=0;mi<nmass;mi++)
   {
-  Propagator4dT<Ty >& pL1 = pV1[mi];
-  Propagator4dT<Ty >& pL2 = pV2[mi];
+  Propagator4dT<Td >& pL1 = pV1[mi];
+  Propagator4dT<Td >& pL2 = pV2[mi];
 
   qacc_for(isp, long(pV1[0].geo().local_volume()),{ 
     int ti = isp/Nxyz;
     int xi = isp%Nxyz;
-      Ty pres;pres = 0.0;
+      qlat::ComplexT<Td > pres;pres = 0.0;
       const qlat::WilsonMatrix& p1 =  pL1.get_elem_offset(isp);
       const qlat::WilsonMatrix& p2 =  pL2.get_elem_offset(isp);
 
       for(int d1=0;d1<4;d1++)
       for(int c1=0;c1<3;c1++)
       for(int d2=0;d2<4;d2++)
       {
-      Ty g_tem = ga2.g[d2]*ga1.g[d1];
+      const qlat::ComplexT<Td > g_tem = ga2.g[d2]*ga1.g[d1];
       for(int c2=0;c2<3;c2++)
       {
         pres += g_tem * 
           p1(ga1.ind[d1]*3+c1,d2*3+c2) * qlat::qconj(p2(d1*3+c1,ga2.ind[d2]*3+c2)) ;
       }
       }
       res[(mi*NTt + ti)*Nxyz + xi%Nxyz] += pres;
   });
   }
 
 }
 
-template <typename Ta >
-void meson_vectorE(EigenMTa &prop1, EigenMTa &prop2, ga_M &ga1,ga_M &ga2,
-        EigenVTa &res, qlat::fft_desc_basic &fd,int clear=1, int invmode=1){
+template <typename Ty >
+void meson_vectorE(std::vector<qpropT >& prop1, std::vector<qpropT >& prop2, ga_M &ga1,ga_M &ga2,
+        qlat::vector_acc<Ty > &res, int clear=1, int invmode=1, const Ty factor = Ty(1.0, 0.0)){
   TIMER("Meson_vectorE");
-  check_prop_size(prop1);check_prop_size(prop2);
-  ///////check_prop_size(prop1);check_prop_size(prop2);
+  const qlat::Geometry &geo = prop1[0].geo();
+  fft_desc_basic& fd = get_fft_desc_basic_plan(geo);
+
   int  NTt  = fd.Nv[3];
   LInt Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
-  int  nmass = prop1.size()/(12*12*NTt);
+  int  nmass = prop1.size();  ////(12*12*NTt)
   if(nmass == 0){res.resize(0);return;}
+  if(clear == 1){ini_resE(res, nmass, fd);}
+  if(res.size()%NTt != 0 or res.size() == 0){print0("Size of res wrong. \n");qassert(false);}
 
-  if(clear == 1){ini_resE(res,nmass,fd);}
-
-  if(res.size()%NTt !=0 or res.size()==0){print0("Size of res wrong. \n");qassert(false);}
   qassert(prop1.size() == prop2.size());
+  qlat::vector_acc<Ty* > p1 = EigenM_to_pointers(prop1);
+  qlat::vector_acc<Ty* > p2 = EigenM_to_pointers(prop2);
 
   for(int d2=0;d2<4;d2++)
   for(int c2=0;c2<3;c2++)
   for(int d1=0;d1<4;d1++)
   for(int c1=0;c1<3;c1++)
   {
   //#pragma omp parallel for
   for(int ji=0;ji<nmass*NTt;ji++)
   {
     int massi = ji/NTt;
     int ti    = ji%NTt;
 
-    int off1 = massi*12*12 + (d2*3+c2)*12+ga1.ind[d1]*3+c1;
-    int off2 = massi*12*12 + (ga2.ind[d2]*3+c2)*12+d1*3+c1;
+    int off1 = (d2*3+c2)*12+ga1.ind[d1]*3+c1;
+    int off2 = (ga2.ind[d2]*3+c2)*12+d1*3+c1;
+
+    const Ty g_tem = ga2.g[d2]*ga1.g[d1];
 
-    Ta g_tem = ga2.g[d2]*ga1.g[d1];
+    Ty* tp1 = &p1[massi][(off1*NTt+ti) * Nxyz];
+    Ty* tp2 = &p2[massi][(off2*NTt+ti) * Nxyz];
 
-    Ta* tp1 = prop1[off1*NTt+ti].data();
-    Ta* tp2 = prop2[off2*NTt+ti].data();
-    Ta* tr0 = &((res.data())[(massi*NTt + ti)*Nxyz]);
+    Ty* tr0 = &((res.data())[(massi*NTt + ti)*Nxyz]);
 
     #if USEQACC==1
-    if(invmode == 1){qacc_forNB(i, long(Nxyz),{ tr0[i] += (tp1[i]*qlat::qconj(tp2[i]) * g_tem);});}
-    if(invmode == 0){qacc_forNB(i, long(Nxyz),{ tr0[i] += (tp1[i]*           (tp2[i]) * g_tem);});}
+    if(invmode == 1){qacc_forNB(i, long(Nxyz),{ tr0[i] += factor * (tp1[i]*qlat::qconj(tp2[i]) * g_tem);});}
+    if(invmode == 0){qacc_forNB(i, long(Nxyz),{ tr0[i] += factor * (tp1[i]*           (tp2[i]) * g_tem);});}
     #else
-    EAa vp1(tp1,Nxyz);
-    EAa vp2(tp2,Nxyz);
-    EAa vr0(tr0,Nxyz);
-    if(invmode == 1)vr0 += (vp1*vp2.conjugate() * g_tem);
-    if(invmode == 0)vr0 += (vp1*vp2             * g_tem);
+    EAy vp1(tp1,Nxyz);
+    EAy vp2(tp2,Nxyz);
+    EAy vr0(tr0,Nxyz);
+    if(invmode == 1)vr0 += factor * (vp1*vp2.conjugate() * g_tem);
+    if(invmode == 0)vr0 += factor * (vp1*vp2             * g_tem);
     #endif
   }
   qacc_barrier(dummy);
   }
-
 }
 
-template<typename Ty, typename Ta>
-void meson_corrE(std::vector<Propagator4dT<Ty > > &pV1, std::vector<Propagator4dT<Ty >> &pV2,  ga_M &ga1, ga_M &ga2,
-  EigenVTa &res, qlat::fft_desc_basic &fd,int clear=1,const Coordinate& mom = Coordinate(),int mode_GPU = 0){
-  ///int NTt  = fd.Nv[3];
-  ///LInt Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
-  int nmass = pV1.size();
-  ///int nt = fd.nt;
-
-  EigenVTa resE;
-  ini_resE(resE,nmass,fd);
-
-  if(mode_GPU == 0){
-    EigenMTa prop1;
-    EigenMTa prop2;
-    copy_prop4d_to_propE(prop1, pV1, fd);
-    copy_prop4d_to_propE(prop2, pV2, fd);
-    ////copy_propE(pV1,prop1, fd);
-    ////copy_propE(pV2,prop2, fd);
-    meson_vectorE(prop1,prop2,ga1,ga2,resE,fd,1);
-  }
-  if(mode_GPU == 1){meson_vectorE(pV1,pV2,ga1,ga2,resE,fd,1);}
-
-  vec_corrE(resE,res,fd, clear, mom);
-}
-
-template<typename Ta>
-void meson_corrE(EigenMTa &prop1,EigenMTa &prop2,  ga_M &ga1, ga_M &ga2,
-  EigenVTa &res, qlat::fft_desc_basic &fd,int clear=1,const Coordinate& mom = Coordinate()){
-  EigenVTa resE;
-  meson_vectorE(prop1,prop2,ga1,ga2,resE,fd,1);
-  vec_corrE(resE,res,fd, clear, mom);
-}
+/////merge to each gamma with sortted cases
+//template <typename Ty >
+//void meson_vectorE(std::vector<qpropT >& prop1, std::vector<qpropT >& prop2,
+//        qlat::vector_acc<Ty > &res, int clear=1, int invmode=1){
+//  TIMER("Meson_vectorE");
+//  const qlat::Geometry &geo = prop1[0].geo();
+//  fft_desc_basic& fd = get_fft_desc_basic_plan(geo);
+//
+//  int  NTt  = fd.Nv[3];
+//  LInt Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
+//  int  nmass = prop1.size();  ////(12*12*NTt)
+//  if(nmass == 0){res.resize(0);return;}
+//  if(clear == 1){ini_resE(res, nmass*16, fd);}
+//  if(res.size()%NTt != 0 or res.size() == 0){print0("Size of res wrong. \n");qassert(false);}
+//
+//  qassert(prop1.size() == prop2.size());
+//  qlat::vector_acc<Ty* > p1 = EigenM_to_pointers(prop1);
+//  qlat::vector_acc<Ty* > p2 = EigenM_to_pointers(prop2);
+//
+//  for(int ds=0;ds<4;ds++)
+//  for(int d2=0;d2<4;d2++)
+//  for(int d1=0;d1<4;d1++)
+//  for(int c2=0;c2<3;c2++)
+//  for(int c1=0;c1<3;c1++)
+//  {
+//  //#pragma omp parallel for
+//  for(int ji=0;ji<nmass*NTt;ji++)
+//  {
+//    int massi = ji/NTt;
+//    int ti    = ji%NTt;
+//    const int offdi = d2*4+d1;
+//
+//    int off1 = (ds*3+c2)*12+d2*3+c1;
+//    int off2 = (ds*3+c2)*12+d1*3+c1;
+//
+//    Ty* tp1 = &p1[massi][(off1*NTt+ti) * Nxyz];
+//    Ty* tp2 = &p2[massi][(off2*NTt+ti) * Nxyz];
+//
+//    Ty* tr0 = &((res.data())[((massi*16+offdi)*NTt + ti)*Nxyz]);
+//
+//    #if USEQACC==1
+//    if(invmode == 1){qacc_forNB(i, long(Nxyz),{ tr0[i] += (tp1[i]*qlat::qconj(tp2[i]));});}
+//    if(invmode == 0){qacc_forNB(i, long(Nxyz),{ tr0[i] += (tp1[i]*           (tp2[i]));});}
+//    #else
+//    EAy vp1(tp1,Nxyz);
+//    EAy vp2(tp2,Nxyz);
+//    EAy vr0(tr0,Nxyz);
+//    if(invmode == 1)vr0 += (vp1*vp2.conjugate());
+//    if(invmode == 0)vr0 += (vp1*vp2            );
+//    #endif
+//  }
+//  qacc_barrier(dummy);
+//  }
+//}
+
+//template <typename Ta >
+//void meson_vectorE(EigenMTa &prop1, EigenMTa &prop2, ga_M &ga1,ga_M &ga2,
+//        EigenVTa &res, qlat::fft_desc_basic &fd,int clear=1, int invmode=1){
+//  TIMER("Meson_vectorE");
+//  check_prop_size(prop1);check_prop_size(prop2);
+//  ///////check_prop_size(prop1);check_prop_size(prop2);
+//  int  NTt  = fd.Nv[3];
+//  LInt Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
+//  int  nmass = prop1.size()/(12*12*NTt);
+//  if(nmass == 0){res.resize(0);return;}
+//
+//  if(clear == 1){ini_resE(res,nmass,fd);}
+//
+//  if(res.size()%NTt !=0 or res.size()==0){print0("Size of res wrong. \n");qassert(false);}
+//  qassert(prop1.size() == prop2.size());
+//
+//  for(int d2=0;d2<4;d2++)
+//  for(int c2=0;c2<3;c2++)
+//  for(int d1=0;d1<4;d1++)
+//  for(int c1=0;c1<3;c1++)
+//  {
+//  //#pragma omp parallel for
+//  for(int ji=0;ji<nmass*NTt;ji++)
+//  {
+//    int massi = ji/NTt;
+//    int ti    = ji%NTt;
+//
+//    int off1 = massi*12*12 + (d2*3+c2)*12+ga1.ind[d1]*3+c1;
+//    int off2 = massi*12*12 + (ga2.ind[d2]*3+c2)*12+d1*3+c1;
+//
+//    Ta g_tem = ga2.g[d2]*ga1.g[d1];
+//
+//    Ta* tp1 = prop1[off1*NTt+ti].data();
+//    Ta* tp2 = prop2[off2*NTt+ti].data();
+//    Ta* tr0 = &((res.data())[(massi*NTt + ti)*Nxyz]);
+//
+//    #if USEQACC==1
+//    if(invmode == 1){qacc_forNB(i, long(Nxyz),{ tr0[i] += (tp1[i]*qlat::qconj(tp2[i]) * g_tem);});}
+//    if(invmode == 0){qacc_forNB(i, long(Nxyz),{ tr0[i] += (tp1[i]*           (tp2[i]) * g_tem);});}
+//    #else
+//    EAa vp1(tp1,Nxyz);
+//    EAa vp2(tp2,Nxyz);
+//    EAa vr0(tr0,Nxyz);
+//    if(invmode == 1)vr0 += (vp1*vp2.conjugate() * g_tem);
+//    if(invmode == 0)vr0 += (vp1*vp2             * g_tem);
+//    #endif
+//  }
+//  qacc_barrier(dummy);
+//  }
+//
+//}
 
 #ifdef QLAT_USE_ACC
 template <typename Ty, int invmode, int bfac, int Blocks>
 __global__ void meson_vectorEV_global(Ty** p1, Ty** p2, Ty* resP, 
   char** gPP, unsigned char** oPP, const int* ivP,
   const int nmass, const int NTt, const long Nxyz, const int Ngv){
   const unsigned long gi =  blockIdx.x;
@@ -421,220 +498,293 @@
   //if(mode==2)meson_vectorEV_kernel<Ty,1,0, BFACG>(p1, p2, resP, gPP, oPP, ivP, nmass, NTt, Nxyz, Ngv);
   //if(mode==3)meson_vectorEV_kernel<Ty,1,1, BFACG>(p1, p2, resP, gPP, oPP, ivP, nmass, NTt, Nxyz, Ngv);
   qacc_barrier(dummy);
   #endif
 
   #if USEKERNEL==0
   for(int iv=0;iv<Ngv;iv++){
-  int j1 = 0*Ngv*4 + iv*4 ;
-  int j2 = 1*Ngv*4 + iv*4 ;
-  Ty* gC1 = &(gC_P[j1]);
-  Ty* gC2 = &(gC_P[j2]);
-  unsigned char* gI1 = &(gI_P[j1]);
-  unsigned char* gI2 = &(gI_P[j2]);
-  long offR = iv*nmass*NTt * Nxyz;
-  for(int d2=0;d2<4;d2++)
-  for(int c2=0;c2<3;c2++)
-  for(int d1=0;d1<4;d1++)
-  for(int c1=0;c1<3;c1++)
-  {
-  #pragma omp parallel for
-  for(int ji=0;ji<nmass*NTt;ji++)
-  {
-    int massi = ji/NTt;
-    int ti    = ji%NTt;
-
-    int off1 = massi*12*12 + (d2*3+c2)*12+gI1[d1]*3+c1;
-    int off2 = massi*12*12 + (gI2[d2]*3+c2)*12+d1*3+c1;
+    int j1 = 0*Ngv*4 + iv*4 ;
+    int j2 = 1*Ngv*4 + iv*4 ;
+    Ty* gC1 = &(gC_P[j1]);
+    Ty* gC2 = &(gC_P[j2]);
+    unsigned char* gI1 = &(gI_P[j1]);
+    unsigned char* gI2 = &(gI_P[j2]);
+    long offR = iv*nmass*NTt * Nxyz;
+    for(int d2=0;d2<4;d2++)
+    for(int c2=0;c2<3;c2++)
+    for(int d1=0;d1<4;d1++)
+    for(int c1=0;c1<3;c1++)
+    {
+    #pragma omp parallel for
+    for(int ji=0;ji<nmass*NTt;ji++)
+    {
+      int massi = ji/NTt;
+      int ti    = ji%NTt;
 
-    Ty g_tem = gC2[d2]*gC1[d1];
+      int off1 = massi*12*12 + (d2*3+c2)*12+gI1[d1]*3+c1;
+      int off2 = massi*12*12 + (gI2[d2]*3+c2)*12+d1*3+c1;
 
-    Ty* tp1 = p1[off1*NTt+ti];
-    Ty* tp2 = p2[off2*NTt+ti];
-    Ty* tr0 = &(resP[offR + (massi*NTt + ti)*Nxyz]);
+      Ty g_tem = gC2[d2]*gC1[d1];
 
-    #if USEQACC==1
-    if(invmode == 1){qacc_forNB(i, long(Nxyz),{ tr0[i] += (tp1[i]*qlat::qconj(tp2[i]) * g_tem);});}
-    if(invmode == 0){qacc_forNB(i, long(Nxyz),{ tr0[i] += (tp1[i]*           (tp2[i]) * g_tem);});}
-    #else
-    EAy vp1(tp1,Nxyz);
-    EAy vp2(tp2,Nxyz);
-    EAy vr0(tr0,Nxyz);
-    if(invmode == 1)vr0 += (vp1*vp2.conjugate() * g_tem);
-    if(invmode == 0)vr0 += (vp1*vp2             * g_tem);
-    #endif
+      Ty* tp1 = p1[off1*NTt+ti];
+      Ty* tp2 = p2[off2*NTt+ti];
+      Ty* tr0 = &(resP[offR + (massi*NTt + ti)*Nxyz]);
+
+      #if USEQACC==1
+      if(invmode == 1){qacc_forNB(i, long(Nxyz),{ tr0[i] += (tp1[i]*qlat::qconj(tp2[i]) * g_tem);});}
+      if(invmode == 0){qacc_forNB(i, long(Nxyz),{ tr0[i] += (tp1[i]*           (tp2[i]) * g_tem);});}
+      #else
+      EAy vp1(tp1,Nxyz);
+      EAy vp2(tp2,Nxyz);
+      EAy vr0(tr0,Nxyz);
+      if(invmode == 1)vr0 += (vp1*vp2.conjugate() * g_tem);
+      if(invmode == 0)vr0 += (vp1*vp2             * g_tem);
+      #endif
 
-  }
-  qacc_barrier(dummy);
-  }
+    }
+    qacc_barrier(dummy);
+    }
   }
   #endif
 
 }
 
-template <typename Ta>
-void meson_vectorEV(EigenMTa &prop1, EigenMTa &prop2, EigenVTa &res, std::vector<ga_M > &ga1V, std::vector<ga_M > &ga2V,
-        qlat::fft_desc_basic &fd, int clear=1, int invmode=1){
-  check_prop_size(prop1);check_prop_size(prop2);
-  int  nmass = prop1.size()/(12*12*fd.Nv[3]);
+//template <typename Ta>
+//void meson_vectorEV(EigenMTa &prop1, EigenMTa &prop2, EigenVTa &res, std::vector<ga_M > &ga1V, std::vector<ga_M > &ga2V,
+//        qlat::fft_desc_basic &fd, int clear=1, int invmode=1){
+//  check_prop_size(prop1);check_prop_size(prop2);
+//  int  nmass = prop1.size()/(12*12*fd.Nv[3]);
+//  if(nmass == 0){res.resize(0);return;}
+//  int Ngv = ga1V.size();
+//  long resL = Ngv * nmass * fd.Nv[0]*fd.Nv[1]*fd.Nv[2] * fd.Nv[3];
+//  if(clear == 1){if(res.size()!= resL){res.resize(resL);}}
+//
+//  if(res.size() != resL){print0("Size of res wrong. \n");qassert(false);}
+//  qassert(prop1.size() == prop2.size());
+//
+//  qlat::vector_acc<Ta* > prop1P = EigenM_to_pointers(prop1);
+//  qlat::vector_acc<Ta* > prop2P = EigenM_to_pointers(prop2);
+//
+//  Ta** p1 = prop1P.data();
+//  Ta** p2 = prop2P.data();
+//  Ta* resP = res.data();
+//  meson_vectorEV(p1, p2, resP, nmass, ga1V, ga2V, fd, clear, invmode);
+//}
+
+template <typename Ty >
+void meson_vectorEV(EigenTy& prop1, EigenTy& prop2, qlat::vector_gpu<Ty > &res
+  ,std::vector<ga_M > &ga1V, std::vector<ga_M > &ga2V,
+  qlat::fft_desc_basic &fd, int clear=1, int invmode=1)
+{
+  check_prop_size(prop1, fd);check_prop_size(prop2, fd);
+  int  nmass = prop1.size();
   if(nmass == 0){res.resize(0);return;}
   int Ngv = ga1V.size();
-  long resL = Ngv * nmass * fd.Nv[0]*fd.Nv[1]*fd.Nv[2] * fd.Nv[3];
+  const unsigned long resL = Ngv * nmass * fd.Nv[0]*fd.Nv[1]*fd.Nv[2] * fd.Nv[3];
+  const long Nxyz= fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
   if(clear == 1){if(res.size()!= resL){res.resize(resL);}}
 
   if(res.size() != resL){print0("Size of res wrong. \n");qassert(false);}
   qassert(prop1.size() == prop2.size());
+  for(int mi=0;mi<nmass;mi++)
+  {
+    qassert(prop1[mi].size() == 12 * 12 * fd.Nvol);
+    qassert(prop2[mi].size() == 12 * 12 * fd.Nvol);
+  }
 
-  qlat::vector_acc<Ta* > prop1P = EigenM_to_pointers(prop1);
-  qlat::vector_acc<Ta* > prop2P = EigenM_to_pointers(prop2);
+  qlat::vector_acc<Ty* > prop1P = EigenM_to_pointers(prop1, Nxyz);
+  qlat::vector_acc<Ty* > prop2P = EigenM_to_pointers(prop2, Nxyz);
 
-  Ta** p1 = prop1P.data();
-  Ta** p2 = prop2P.data();
-  Ta* resP = res.data();
+  Ty** p1 = prop1P.data();
+  Ty** p2 = prop2P.data();
+  Ty* resP = res.data();
   meson_vectorEV(p1, p2, resP, nmass, ga1V, ga2V, fd, clear, invmode);
 }
 
-template <typename Ta>
-void meson_corr_write(Propagator4dT<Ta > &propVa, Propagator4dT<Ta > &propVb, int pos, std::vector<double > &write, int offw, const Geometry &geo, int a=0, int b=0, int c=0 , int d=0){
-  print_mem_info();
-  fft_desc_basic fd(geo);
-  //qlat::vector<int > nv, Nv, mv;
-  //geo_to_nv(geo, nv, Nv, mv);
-  int nt = fd.nt;
-
-  ///char output[500];
-  ///sprintf(output,   out_n.c_str());
-  ///print0("output %s \n", output);
-
-  EigenMTa propa,propb;
-  copy_prop4d_to_propE(propa, propVa, fd);
-  copy_prop4d_to_propE(propb, propVb, fd);
-  ////copy_propE(propVa, propa, fd );
-  ////copy_propE(propVb, propb, fd );
-
-  ///Coordinate xg1;
-  ///xg1[0] = pos/10000000;xg1[1] = (pos%10000000)/100000;xg1[2] = (pos%100000)/1000;xg1[3] = pos%1000;
-  int t0 = pos%1000;
-
-  EigenVTa res;ga_matrices_cps   ga_cps;
-  meson_corrE(propa, propb, ga_cps.ga[a][b],ga_cps.ga[c][d],  res, fd);
-  ///std::vector<double > write;write.resize(2*nt);
-  for(int ti=0;ti<nt;ti++)
-  {
-    double v0 = res[ti].real();
-    double v1 = res[ti].imag();
-    write[offw + ((ti- t0 +nt)%nt)*2+0]= v0;
-    write[offw + ((ti- t0 +nt)%nt)*2+1]= v1;
-  }
-  ////write_data(write,output);
 
-}
-
-void meson_corr_write(std::string prop_a, std::string prop_b, std::string src_n, std::string out_n, const Geometry &geo, int a=0, int b=0, int c=0 , int d=0){
-  print_mem_info();
-  fft_desc_basic fd(geo);
-  std::vector<qlat::vector_acc<Complexq > > propa,propb;
-  qlat::vector_acc<int > nv, Nv, mv;
-  geo_to_nv(geo, nv, Nv, mv);
-  int nt = nv[3];
-
-  qlat::FieldM<Complexq, 1> noi;
-  noi.init(geo);
-  Propagator4d propVa;propVa.init(geo);
-  Propagator4d propVb;propVb.init(geo);
-
-
-  char prop_na[500],prop_nb[500],noi_name[500];
-  char output[500];
-  sprintf(prop_na, "%s",prop_a.c_str() );
-  sprintf(prop_nb, "%s",prop_b.c_str() );
-
-  sprintf(noi_name ,"%s",src_n.c_str()  );
-  sprintf(output,   "%s",out_n.c_str());
-
-  print0("Noise %s \n",noi_name);
-  print0("Prop  %s %s \n",prop_na, prop_nb);
-  print0("output %s \n", output);
-
-  qlat::set_zero(noi);
-  load_gwu_noi(noi_name,noi);
-  load_gwu_prop(prop_na, propVa);
-  if(prop_a == prop_b){propVb = propVa;}
-  else{load_gwu_prop(prop_nb, propVb);}
-  
-  copy_prop4d_to_propE(propa, propVa, fd);
-  copy_prop4d_to_propE(propb, propVb, fd);
-  //copy_propE(propVa,propa, fd );
-  //copy_propE(propVb,propb, fd );
-
-  Coordinate pos;Coordinate off_L;
-  check_noise_pos(noi, pos, off_L);
-
-  ////Coordinate xg1;
-  ////xg1[0] = pos/10000000;xg1[1] = (pos%10000000)/100000;xg1[2] = (pos%100000)/1000;xg1[3] = pos%1000;
-
-  EigenV res;ga_matrices_cps   ga_cps;
-  meson_corrE(propa, propb, ga_cps.ga[a][b],ga_cps.ga[c][d],  res, fd);
-  std::vector<double > write;write.resize(2*nt);
-  for(unsigned int ti=0;ti<write.size()/2;ti++){
-    double v0 = res[ti].real();
-    double v1 = res[ti].imag();
-    write[((ti-pos[3]+nt)%nt)*2+0]= v0;
-    write[((ti-pos[3]+nt)%nt)*2+1]= v1;
-  }
-
-  write_data(write,output);
+template<typename Td, typename Ta>
+void meson_corrE(std::vector<Propagator4dT<Td > > &pV1, std::vector<Propagator4dT<Td >> &pV2,  ga_M &ga1, ga_M &ga2,
+  qlat::vector_acc<Ta > &res, qlat::fft_desc_basic &fd,int clear=1,const Coordinate& mom = Coordinate(),int mode_GPU = 0){
+  ///int NTt  = fd.Nv[3];
+  ///LInt Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
+  int nmass = pV1.size();
+  ///int nt = fd.nt;
 
-}
+  qlat::vector_acc<Ta > resE;
+  ini_resE(resE,nmass,fd);
 
-template <typename Ta>
-void print_meson(Propagator4dT<Ta > &propVa, Propagator4dT<Ta > &propVb, std::string tag=std::string(""), int a=0, int b=0, int c=0 , int d=0){
-  fft_desc_basic fd(propVa.geo());
-  int nt = fd.nt;
-
-  EigenMTa propa,propb;
-  copy_prop4d_to_propE(propa, propVa, fd);
-  copy_prop4d_to_propE(propb, propVb, fd);
-  ////copy_propE(propVa, propa, fd );
-  ////copy_propE(propVb, propb, fd );
-
-  EigenVTa res;ga_matrices_cps   ga_cps;
-  meson_corrE(propa, propb, ga_cps.ga[a][b],ga_cps.ga[c][d],  res, fd);
-  for(int ti=0;ti<nt;ti++)
-  {
-    double v0 = res[ti].real();
-    double v1 = res[ti].imag();
-    print0("%s ti %5d , v  %.8e   %.8e \n", tag.c_str(), ti, v0, v1);
+  if(mode_GPU == 0){
+    std::vector<qlat::vector_acc<Ta > > prop1;
+    std::vector<qlat::vector_acc<Ta > > prop2;
+    copy_prop4d_to_propE(prop1, pV1, fd);
+    copy_prop4d_to_propE(prop2, pV2, fd);
+    ////copy_propE(pV1,prop1, fd);
+    ////copy_propE(pV2,prop2, fd);
+    meson_vectorE(prop1,prop2,ga1,ga2,resE,fd,1);
   }
-}
+  if(mode_GPU == 1){meson_vectorE(pV1,pV2,ga1,ga2,resE,fd,1);}
 
-template<typename Ta>
-void print_pion(qlat::FieldM<Ta, 12*12 >& propM, const std::string& tag=std::string(""), double factor = 1.0){
-  const Geometry& geo = propM.geo();
-  fft_desc_basic fd(geo);
-
-  Propagator4dT<Ta > prop4d;prop4d.init(geo);
-  std::vector<qlat::vector_acc<Ta > > propE;
-
-  copy_noise_to_prop(propM, prop4d, 1);
-  copy_prop4d_to_propE(propE, prop4d, fd);
-  ////copy_propE(prop4d, propE, fd);
-
-  ga_matrices_cps   ga_cps;
-  EigenVTa res;EigenVTa corr;
-  meson_vectorE(propE, propE, ga_cps.ga[0][0], ga_cps.ga[0][0],res, fd);
-
-  vec_corrE(res, corr, fd, 1 );
-
-  int nv = corr.size()/fd.nt;
-  for(int iv=0;iv<nv;iv++)
-  for(int t=0;t<fd.nt;t++)
-  {
-    Ta v = corr[iv*fd.nt + t] * Ta(factor, 0.0);
-    print0("%s iv %d, t %d, v %.6e %.6e \n", tag.c_str(), iv, t, v.real(), v.imag());
-  }
+  vec_corrE(resE,res,fd, clear, mom);
 }
 
+template<typename Ty>
+void meson_corrE(std::vector<qpropT > &prop1, std::vector<qpropT > &prop2,  ga_M &ga1, ga_M &ga2,
+  qlat::vector_acc<Ty >& res, int clear=1,const Coordinate& mom = Coordinate()){
+  qlat::vector_acc<Ty > resE;
+
+  const qlat::Geometry &geo = prop1[0].geo();
+  fft_desc_basic& fd = get_fft_desc_basic_plan(geo);
+
+  meson_vectorE(prop1,prop2,ga1,ga2,resE,1);
+  vec_corrE(resE, res, fd, clear, mom);
+}
+
+//template <typename Ta>
+//void meson_corr_write(Propagator4dT<Ta > &propVa, Propagator4dT<Ta > &propVb, int pos, std::vector<double > &write, int offw, const Geometry &geo, int a=0, int b=0, int c=0 , int d=0){
+//  print_mem_info();
+//  fft_desc_basic fd(geo);
+//  //qlat::vector<int > nv, Nv, mv;
+//  //geo_to_nv(geo, nv, Nv, mv);
+//  int nt = fd.nt;
+//
+//  ///char output[500];
+//  ///sprintf(output,   out_n.c_str());
+//  ///print0("output %s \n", output);
+//
+//  EigenMTa propa,propb;
+//  copy_prop4d_to_propE(propa, propVa, fd);
+//  copy_prop4d_to_propE(propb, propVb, fd);
+//  ////copy_propE(propVa, propa, fd );
+//  ////copy_propE(propVb, propb, fd );
+//
+//  ///Coordinate xg1;
+//  ///xg1[0] = pos/10000000;xg1[1] = (pos%10000000)/100000;xg1[2] = (pos%100000)/1000;xg1[3] = pos%1000;
+//  int t0 = pos%1000;
+//
+//  EigenVTa res;ga_matrices_cps   ga_cps;
+//  meson_corrE(propa, propb, ga_cps.ga[a][b],ga_cps.ga[c][d],  res, fd);
+//  ///std::vector<double > write;write.resize(2*nt);
+//  for(int ti=0;ti<nt;ti++)
+//  {
+//    double v0 = res[ti].real();
+//    double v1 = res[ti].imag();
+//    write[offw + ((ti- t0 +nt)%nt)*2+0]= v0;
+//    write[offw + ((ti- t0 +nt)%nt)*2+1]= v1;
+//  }
+//  ////write_data(write,output);
+//
+//}
+
+//inline void meson_corr_write(std::string prop_a, std::string prop_b, std::string src_n, std::string out_n, const Geometry &geo, int a=0, int b=0, int c=0 , int d=0){
+//  print_mem_info();
+//
+//  qlat::vector_acc<int > nv, Nv, mv;
+//  geo_to_nv(geo, nv, Nv, mv);
+//  int nt = nv[3];
+//
+//  qlat::FieldM<Complexq, 1> noi;
+//  noi.init(geo);
+//  Propagator4d propVa;propVa.init(geo);
+//  Propagator4d propVb;propVb.init(geo);
+//
+//  char prop_na[500],prop_nb[500],noi_name[500];
+//  char output[500];
+//  sprintf(prop_na, "%s",prop_a.c_str() );
+//  sprintf(prop_nb, "%s",prop_b.c_str() );
+//
+//  sprintf(noi_name ,"%s",src_n.c_str()  );
+//  sprintf(output,   "%s",out_n.c_str());
+//
+//  print0("Noise %s \n",noi_name);
+//  print0("Prop  %s %s \n",prop_na, prop_nb);
+//  print0("output %s \n", output);
+//
+//  qlat::set_zero(noi);
+//  load_gwu_noi(noi_name,noi);
+//  load_gwu_prop(prop_na, propVa);
+//  if(prop_a == prop_b){propVb = propVa;}
+//  else{load_gwu_prop(prop_nb, propVb);}
+//  
+//  ////std::vector<qlat::vector_acc<Complexq > > propa,propb;
+//  std::vector<qprop > propa, propb;
+//  propa.resize(1);propa[0].init(geo);
+//  propb.resize(1);propb[0].init(geo);
+//  prop4d_to_qprop(propa[0], propVa);
+//  prop4d_to_qprop(propb[0], propVb);
+//
+//  Coordinate pos;Coordinate off_L;
+//  check_noise_pos(noi, pos, off_L);
+//
+//  ////Coordinate xg1;
+//  ////xg1[0] = pos/10000000;xg1[1] = (pos%10000000)/100000;xg1[2] = (pos%100000)/1000;xg1[3] = pos%1000;
+//
+//  qlat::vector_acc<qlat::Complex > res;ga_matrices_cps   ga_cps;
+//  meson_corrE(propa, propb, ga_cps.ga[a][b],ga_cps.ga[c][d],  res);
+//  std::vector<double > write;write.resize(2*nt);
+//  for(unsigned int ti=0;ti<write.size()/2;ti++){
+//    double v0 = res[ti].real();
+//    double v1 = res[ti].imag();
+//    write[((ti-pos[3]+nt)%nt)*2+0]= v0;
+//    write[((ti-pos[3]+nt)%nt)*2+1]= v1;
+//  }
+//
+//  write_data(write,output);
+//
+//}
+
+//template <typename Ta>
+//void print_meson(Propagator4dT<Ta > &propVa, Propagator4dT<Ta > &propVb, std::string tag=std::string(""), int a=0, int b=0, int c=0 , int d=0){
+//  const qlat::Geometry &geo = propVa.geo();
+//  fft_desc_basic& fd = get_fft_desc_basic_plan(geo);
+//
+//  int nt = fd.nt;
+//
+//  std::vector<qprop > propa, propb;
+//  propa.resize(1);propa[0].init(geo);
+//  propb.resize(1);propb[0].init(geo);
+//  prop4d_to_qprop(propa[0], propVa);
+//  prop4d_to_qprop(propb[0], propVb);
+//
+//  ////copy_propE(propVa, propa, fd );
+//  ////copy_propE(propVb, propb, fd );
+//
+//  qlat::vector_acc<qlat::Complex > res;ga_matrices_cps   ga_cps;
+//  meson_corrE(propa, propb, ga_cps.ga[a][b],ga_cps.ga[c][d],  res);
+//  for(int ti=0;ti<nt;ti++)
+//  {
+//    double v0 = res[ti].real();
+//    double v1 = res[ti].imag();
+//    print0("%s ti %5d , v  %.8e   %.8e \n", tag.c_str(), ti, v0, v1);
+//  }
+//}
+
+//template<typename Ta>
+//void print_pion(qlat::FieldM<Ta, 12*12 >& propM, const std::string& tag=std::string(""), double factor = 1.0){
+//  const Geometry& geo = propM.geo();
+//  fft_desc_basic fd(geo);
+//
+//  Propagator4dT<Ta > prop4d;prop4d.init(geo);
+//  std::vector<qlat::vector_acc<Ta > > propE;
+//
+//  copy_noise_to_prop(propM, prop4d, 1);
+//  copy_prop4d_to_propE(propE, prop4d, fd);
+//  ////copy_propE(prop4d, propE, fd);
+//
+//  ga_matrices_cps   ga_cps;
+//  EigenVTa res;EigenVTa corr;
+//  meson_vectorE(propE, propE, ga_cps.ga[0][0], ga_cps.ga[0][0],res, fd);
+//
+//  vec_corrE(res, corr, fd, 1 );
+//
+//  int nv = corr.size()/fd.nt;
+//  for(int iv=0;iv<nv;iv++)
+//  for(int t=0;t<fd.nt;t++)
+//  {
+//    Ta v = corr[iv*fd.nt + t] * Ta(factor, 0.0);
+//    print0("%s iv %d, t %d, v %.6e %.6e \n", tag.c_str(), iv, t, v.real(), v.imag());
+//  }
+//}
+
 }
 
 #endif
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_corr_prop.h` & `qlat-0.9/include/qlat/vector_utils/utils_corr_prop.h`

 * *Files 21% similar despite different names*

```diff
@@ -8,57 +8,251 @@
 #pragma once
 
 #include "utils_float_type.h"
 #include "utils_gammas.h"
 #include "utils_fft_desc.h"
 #include "utils_reduce_vec.h"
 #include "utils_grid_src.h"
+#include "utils_shift_vecs.h"
 
 namespace qlat{
 
 template<typename Ty>
-void prop4d_src_gamma(Propagator4dT<Ty >& prop, ga_M& ga,int dir = 0){
+void init_qpropT(std::vector<qpropT >& res, const unsigned int size, const Geometry& geo)
+{
+  if(res.size() != size){
+    res.resize(size);
+  }
+  for(unsigned int i=0;i<res.size();i++){
+    if(!res[i].initialized){res[i].init(geo);}
+  }
+
+}
+
+template<typename Ty>
+void clear_qpropT(std::vector<qpropT >& res)
+{
+  for(unsigned int i=0;i<res.size();i++){
+    qlat::set_zero(res[i]);
+  }
+}
+
+
+template<typename Td, int dir, bool conj>
+void prop4d_src_gammaT(Propagator4dT<Td >& prop, ga_M& ga){
+  TIMERA("prop4d_src_gamma");
   ////Rowmajor (a,b), b is continues in memory
   qacc_for(isp, long(prop.geo().local_volume()),{
-    qlat::WilsonMatrixT<Ty>& v0 =  prop.get_elem_offset(isp);
-    qlat::WilsonMatrixT<Ty>  v1 = v0;
+    qlat::WilsonMatrixT<Td>& v0 =  prop.get_elem_offset(isp);
+    qlat::WilsonMatrixT<Td>  v1 = v0;
 
-    for (int s = 0; s < 4; ++s)
+    for(int s = 0; s < 4; ++s)
     for(int c0 = 0;c0< 3 ; c0++)
-    for (int d0 = 0; d0 < 4; ++d0)
+    for(int d0 = 0; d0 < 4; ++d0)
+    {
+      /////Source multiply
+      if(dir==0)for(int c1=0;c1<3;c1++){
+        if(!conj){v0(s*3 + c0, ga.ind[d0]*3 + c1) = ga.g[d0] * v1(s*3 + c0, d0*3 + c1);}
+        if( conj){v0(s*3 + c0, ga.ind[d0]*3 + c1) = qlat::qconj(ga.g[d0] * v1(s*3 + c0, d0*3 + c1));}
+      }
+      /////Sink multiply
+      if(dir==1)for(int c1=0;c1<3;c1++){
+        if(!conj){v0(d0*3 + c0, s*3 + c1) = ga.g[d0] * v1(ga.ind[d0]*3 + c0, s*3 + c1);}
+        if( conj){v0(d0*3 + c0, s*3 + c1) = qlat::qconj(ga.g[d0] * v1(ga.ind[d0]*3 + c0, s*3 + c1));}
+      }
+    }
+  });
+}
+
+template<typename Td>
+void prop4d_src_gamma(Propagator4dT<Td >& prop, ga_M& ga, bool conj = false){
+  if(!conj){prop4d_src_gammaT<Td, 0, false>(prop, ga);}
+  if( conj){prop4d_src_gammaT<Td, 0, true >(prop, ga);}
+}
+template<typename Td>
+void prop4d_sink_gamma(Propagator4dT<Td >& prop, ga_M& ga, bool conj = false){
+  if(!conj){prop4d_src_gammaT<Td, 1, false>(prop, ga);}
+  if( conj){prop4d_src_gammaT<Td, 1, true >(prop, ga);}
+}
+
+template<typename Ty, int dir, bool conj>
+void qprop_src_gamma_T(Ty* res, ga_M& ga, const long Nsize){
+  TIMERA("qprop_src_gamma");
+  ////Rowmajor (a,b), b is continues in memory
+  ///Ty* res = (Ty*) qlat::get_data(prop1).data()
+  //const long Nsize = prop.geo().local_volume();
+  qacc_for(isp, Nsize,{
+    Ty src[12*12];
+    Ty buf[12*12];
+    for(int i=0;i<12*12;i++){src[i] = res[i*Nsize + isp];}
+
+    for(int d1 = 0;d1 < 4; d1++)
+    for(int c1 = 0;c1 < 3; c1++)
+    for(int d0 = 0;d0 < 4; d0++)
+    for(int c0 = 0;c0 < 3; c0++)
     {
       /////Source multiply
-      if(dir==0)for(int c1=0;c1<3;c1++)v0(s*3 + c0, ga.ind[d0]*3 + c1) = ga.g[d0] * v1(s*3 + c0, d0*3 + c1);
+      if(dir==0)
+      {
+        buf[(ga.ind[d1]*3 + c1) * 12 + d0*3 + c0] = ga.g[d1] * src[(d1*3 + c1 )*12 + d0*3 + c0];
+      }
       /////Sink multiply
-      if(dir==1)for(int c1=0;c1<3;c1++)v0(d0*3 + c0, s*3 + c1) = ga.g[d0] * v1(ga.ind[d0]*3 + c0, s*3 + c1);
+      if(dir==1)
+      {
+        buf[(d1*3 + c1)*12 + d0*3 + c0] = ga.g[d0] * src[(d1*3 + c1)*12 + ga.ind[d0]*3 + c0];
+      }
+    }
 
-      ///////Source multiply
-      //if(dir==0)for(int c1=0;c1<3;c1++)cp_C(v0(s*3 + c0, ga.ind[d0]*3 + c1), ga.g[d0] * v1(s*3 + c0, d0*3 + c1));
-      ///////Sink multiply
-      //if(dir==1)for(int c1=0;c1<3;c1++)cp_C(v0(d0*3 + c0, s*3 + c1), ga.g[d0] * v1(ga.ind[d0]*3 + c0, s*3 + c1));
+    for(int i=0;i<12*12;i++){
+      if(!conj){res[i*Nsize + isp] = buf[i];}
+      if( conj){res[i*Nsize + isp] = qlat::qconj(buf[i]);}
     }
   });
 }
 
 template<typename Ty>
-void prop4d_sink_gamma(Propagator4dT<Ty >& prop, ga_M& ga){
-  prop4d_src_gamma(prop, ga ,1);
+void qprop_src_gamma(qpropT& prop, ga_M& ga, bool conj = false){
+  Ty* res = (Ty*) qlat::get_data(prop).data();
+  const long Nsize = prop.geo().local_volume();
+  if(!conj)qprop_src_gamma_T<Ty, 0, false>(res, ga, Nsize);
+  if( conj)qprop_src_gamma_T<Ty, 0, true >(res, ga, Nsize);
+}
+
+
+template<typename Ty>
+void qprop_sink_gamma(qpropT& prop, ga_M& ga, bool conj = false){
+  Ty* res = (Ty*) qlat::get_data(prop).data();
+  const long Nsize = prop.geo().local_volume();
+  if(!conj)qprop_src_gamma_T<Ty, 1, false>(res, ga, Nsize);
+  if( conj)qprop_src_gamma_T<Ty, 1, true >(res, ga, Nsize);
+}
+
+template<typename Ty>
+void Gprop_src_gamma(EigenTy& prop, ga_M& ga, bool conj = false){
+  for(unsigned long iv=0;iv<prop.size();iv++)
+  {
+    Ty* res = (Ty*) qlat::get_data(prop[iv]).data();
+    if(!conj)qprop_src_gamma_T<Ty, 0, false>(res, ga, prop[iv].size()/(12*12));
+    if( conj)qprop_src_gamma_T<Ty, 0, true >(res, ga, prop[iv].size()/(12*12));
+  }
+}
+
+template<typename Ty>
+void Gprop_sink_gamma(EigenTy& prop, ga_M& ga, bool conj = false){
+  for(unsigned long iv=0;iv<prop.size();iv++)
+  {
+    Ty* res = (Ty*) qlat::get_data(prop[iv]).data();
+    if(!conj)qprop_src_gamma_T<Ty, 1, false>(res, ga, prop[iv].size()/(12*12));
+    if( conj)qprop_src_gamma_T<Ty, 1, true >(res, ga, prop[iv].size()/(12*12));
+  }
+}
+
+template<typename Ty>
+void qprop_move_dc_in(Ty* src, const qlat::Geometry &geo, const int dir = 1)
+{
+  move_index mv_civ;
+  const long sizeF = geo.local_volume();
+
+  if(dir == 1){mv_civ.move_civ_in( src, src, 1, 12*12, sizeF, 1, true);}
+  if(dir == 0){mv_civ.move_civ_out(src, src, 1, sizeF, 12*12, 1, true);}
+}
+
+template<typename Ty>
+void qprop_move_dc_in(qpropT& src, const int dir = 1)
+{
+  qassert(src.initialized);
+  qprop_move_dc_in((Ty*) qlat::get_data(src).data(), src.geo(), dir);
+}
+
+template<typename Ty>
+void qprop_move_dc_out(Ty* src, const qlat::Geometry &geo)
+{
+  qprop_move_dc_in(src, geo, 0);
 }
 
+template<typename Ty>
+void qprop_move_dc_out(qpropT& src)
+{
+  qprop_move_dc_in(src, 0);
+}
 
 template<typename Ty>
-void prop4d_cps_to_ps(Propagator4dT<Ty >& prop, int dir=0){
+void qprop_sub_add(std::vector<qpropT >& res, std::vector< qpropT >& s0, const Ty f0, const Ty f1)
+{
+  if(s0.size() == 0){res.resize(0); return ;}
+  const int Nvec = s0.size();
+  const qlat::Geometry &geo = s0[0].geo();
+  const long Nvol = geo.local_volume();
+
+  init_qpropT(res, Nvec, geo);
+  for(int vi=0;vi<Nvec;vi++)
+  {
+    Ty* p0 = (Ty* ) qlat::get_data(s0[vi]).data();
+    Ty* r0 = (Ty* ) qlat::get_data(res[vi]).data(); 
+    for(int dc=0;dc<12*12;dc++){
+      qacc_for(isp, geo.local_volume(),{
+        r0[dc*Nvol + isp] = r0[dc*Nvol + isp]*f0 + p0[dc*Nvol + isp] * f1;
+      });
+    }
+  }
+}
+
+template<typename Ty>
+void qprop_sub_add(std::vector<qpropT >& res, std::vector< qpropT >& s0, std::vector< qpropT >& s1, const Ty f0, const Ty f1)
+{
+  if(s0.size() == 0){res.resize(0); return ;}
+  qassert(s0.size() == s1.size());
+  const int Nvec = s0.size();
+  const qlat::Geometry &geo = s0[0].geo();
+  const long Nvol = geo.local_volume();
+
+  init_qpropT(res, Nvec, geo);
+  for(int vi=0;vi<Nvec;vi++)
+  {
+    Ty* p0 = (Ty* ) qlat::get_data(s0[vi]).data();
+    Ty* p1 = (Ty* ) qlat::get_data(s1[vi]).data(); 
+    Ty* r0 = (Ty* ) qlat::get_data(res[vi]).data(); 
+    for(int dc=0;dc<12*12;dc++){
+      qacc_for(isp, geo.local_volume(),{
+        r0[dc*Nvol + isp] = (p0[dc*Nvol + isp] + p1[dc*Nvol + isp] * f0) * f1;
+      });
+    }
+  }
+}
+
+template<typename Ty>
+void shift_vecs_cov_qpropT(std::vector< std::vector<qpropT > >& res, std::vector< qpropT >& s0, shift_vec& svec,
+  std::vector<std::vector<qpropT >>& buf)
+{
+  if(res.size() != 5){res.resize(5);}
+  if(buf.size() != 2){buf.resize(2);}
+  qprop_sub_add(res[0], s0, Ty(0.0,0.0), Ty(1.0,0.0) );////equal
+
+  init_qpropT(buf[0], s0.size(), s0[0].geo());
+  init_qpropT(buf[1], s0.size(), s0[0].geo());
+
+  for(int nu = 0; nu < 4 ; nu++)
+  {
+    shift_vecs_dir_qpropT(s0, buf[0], nu, +1, svec);
+    shift_vecs_dir_qpropT(s0, buf[1], nu, -1, svec);
+    qprop_sub_add(res[1 + nu], buf[0], buf[1], Ty(-1.0,0.0), Ty(1.0/2.0, 0.0) );////equal
+  }
+}
+
+
+template<typename Td>
+void prop4d_cps_to_ps(Propagator4dT<Td >& prop, int dir=0){
   /////sn is -1 for default
-  Ty sn =-1;if(dir == 1){sn= 1;}
-  const Ty sqrt2= Ty(std::sqrt(2.0), 0.0);
+  qlat::ComplexT<Td > sn =-1;if(dir == 1){sn= 1;}
+  const qlat::ComplexT<Td>sqrt2= qlat::ComplexT<Td>(std::sqrt(2.0), 0.0);
 
   ////Rowmajor (a,b), b is continues in memory
   qacc_for(isp, prop.geo().local_volume(),{
-    qlat::WilsonMatrixT<Ty >  v0 = prop.get_elem_offset(isp);
-    qlat::WilsonMatrixT<Ty >  v1 = prop.get_elem_offset(isp);
+    qlat::WilsonMatrixT<Td >  v0 = prop.get_elem_offset(isp);
+    qlat::WilsonMatrixT<Td >  v1 = prop.get_elem_offset(isp);
 
     int dr,d0,d1;
     /////Src rotation
     for (int s0 = 0; s0 < 4; ++s0)
     for(int c0 = 0;c0< 3 ; c0++)
     {
       dr=0;d0=1;d1=3;
@@ -87,36 +281,36 @@
       for(int c1=0;c1<3;c1++)v0(dr*3+c0, s0*3+c1) = ( v1(d0*3+c0, s0*3+c1)    + v1(d1*3+c0, s0*3+c1)*sn)/sqrt2;
     }
     prop.get_elem_offset(isp) = v0;
 
   });
 }
 
-template<typename Ty>
-void prop4d_ps_to_cps(Propagator4dT<Ty >& prop){
+template<typename Td>
+void prop4d_ps_to_cps(Propagator4dT<Td >& prop){
   prop4d_cps_to_ps(prop, 1);
 }
 
-template<typename Ty>
-void get_corr_pion(std::vector<qlat::FermionField4dT<Ty > > &prop,const Coordinate &x_ini, std::vector<double > &write ){
+template<typename Td>
+void get_corr_pion(std::vector<qlat::FermionField4dT<Td > > &prop,const Coordinate &x_ini, std::vector<double > &write ){
 
   const qlat::Geometry &geo = prop[0].geo();
 
   unsigned long Nvol = geo.local_volume();
   ///int Nt = geo.node_site[3];
   ///long Nsum = Nvol/Nt;
   int tini = x_ini[3];
 
-  qlat::vector_acc<Ty > res;res.resize(Nvol);
+  qlat::vector_acc<qlat::ComplexT<Td> > res;res.resize(Nvol);
 
   qacc_for(isp, long(Nvol),{
-    Ty buf(0.0,0.0);
+    qlat::ComplexT<Td> buf(0.0,0.0);
 
     for(int dc2=0;dc2<12;dc2++){
-      Ty* a = (Ty* ) &(prop[dc2].get_elem_offset(isp));
+      qlat::ComplexT<Td>* a = (qlat::ComplexT<Td>* ) &(prop[dc2].get_elem_offset(isp));
       for(int dc1=0;dc1<12;dc1++)
       {
         buf+=a[dc1]*qlat::qconj(a[dc1]);
       }
     }
     res[isp] = buf;
     ////src[isp] = buf[isp];
@@ -269,182 +463,230 @@
     Coordinate c;
     for(int j = 0;j<4;j++){c[j] = stringtonum(a[i*5 + j]);}
     posL.push_back(c);
   }
   return posL;
 }
 
-template<typename Ta>
-void shift_result_t(EigenVTa& Esrc, int nt, int tini){
+template<typename Ty>
+void shift_result_t(qlat::vector_acc<Ty >& Esrc, int nt, int tini){
   if(tini == 0){return ;}
   long Ntotal = Esrc.size();
   if(Ntotal %(nt) != 0){abort_r("Correlation function size wrong!\n");}
-  EigenVTa tmp;tmp.resize(Ntotal);
+  qlat::vector_acc<Ty > tmp;tmp.resize(Ntotal);
   qacc_for(i, Ntotal, {
     const int iv = i/nt;
     const int t  = i%nt;
     tmp[iv*nt + (t - tini + nt)%nt] = Esrc[iv*nt + (t)%nt];
   });
   cpy_data_thread(Esrc.data(), tmp.data(), tmp.size(), 1);
 }
 
-template<typename Ta>
-void ini_propE(EigenMTa &prop,int nmass, qlat::fft_desc_basic &fd, bool clear = true){
-  LInt Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
-  int NTt  = fd.Nv[3];
-  int do_resize = 0;
-  if(prop.size() != (LInt) (nmass*12*12*NTt)){do_resize = 1;}
-  for(unsigned int i=0;i<prop.size();i++){if((LInt) prop[i].size() != Nxyz){do_resize=1;}}
-
-  if(do_resize == 1)
+//template<typename Ta>
+//void ini_propE(EigenMTa &prop,int nmass, qlat::fft_desc_basic &fd, bool clear = true){
+//  LInt Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
+//  int NTt  = fd.Nv[3];
+//  int do_resize = 0;
+//  if(prop.size() != (LInt) (nmass*12*12*NTt)){do_resize = 1;}
+//  for(unsigned int i=0;i<prop.size();i++){if((LInt) prop[i].size() != Nxyz){do_resize=1;}}
+//
+//  if(do_resize == 1)
+//  {
+//    for(unsigned int i=0;i<prop.size();i++){prop[i].resize(0);}prop.resize(0);
+//    prop.resize(nmass*12*12*NTt);
+//    for(unsigned int i=0;i<prop.size();i++){
+//      prop[i].resize(Nxyz);
+//    }
+//  }
+//  if(clear){zeroE(prop);}
+//}
+
+//////default dir == 0 from prop4d to propE
+//template<typename Ty, typename Ta>
+//void copy_propE(std::vector<Ty* > &pV1, EigenMTa &prop, qlat::fft_desc_basic &fd, int dir=0){
+//  TIMER("Copy prop");
+//  qassert(fd.order_ch == 0);
+//  const LInt Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
+//  const int NTt  = fd.Nv[3];
+//  Geometry geo;fd.get_geo(geo);
+//  int nmass = 0;
+//  if(dir==0){nmass = pV1.size();ini_propE(prop,nmass,fd);}
+//  if(dir==1){
+//    nmass = prop.size()/(12*12*NTt);
+//    qassert(int(pV1.size()) == nmass);
+//    //if(pV1.size() != (LInt) nmass){
+//    //  pV1.resize(0);
+//    //  pV1.resize(nmass);for(int i=0;i<nmass;i++){pV1[i].init(geo);}
+//    //}
+//  }
+//
+//  for(int mi = 0;mi < nmass;mi++)
+//  {
+//    Ty* pv = pV1[mi];
+//    /////Propagator4dT<Ty >& pv = pV1[mi];
+//    qlat::vector_acc<Ta* > ps = EigenM_to_pointers(prop);
+//    qacc_for(isp, long(NTt*Nxyz),{
+//      int ti = isp/Nxyz;
+//      int xi = isp%Nxyz;
+//      /////qlat::WilsonMatrixT<Ty>& v0 =  pv.get_elem_offset(isp);
+//      Ty* v0 = &pv[isp * 12 * 12];
+//
+//      for(int c0 = 0;c0 < 3; c0++)
+//      for(int d0 = 0;d0 < 4; d0++)
+//      for(int c1 = 0;c1 < 3; c1++)
+//      for(int d1 = 0;d1 < 4; d1++)
+//      {
+//        LInt off = mi*12*12 + (d1*3+c1)*12+d0*3+c0;
+//        if(dir==0){ps[off*NTt+ti][xi] = v0[(d0*3 + c0)*12 +  d1*3 + c1];}
+//        if(dir==1){v0[(d0*3 + c0)*12 +  d1*3 + c1] = ps[off*NTt+ti][xi];}
+//      }
+//    });
+//  }
+//
+//}
+
+//template<typename Ty, typename Ta>
+//void copy_propE(Propagator4dT<Ty > &pV, EigenMTa &prop, qlat::fft_desc_basic &fd, int dir=0){
+//  int nmass = 1;
+//  if(dir==0){
+//    qassert(pV.initialized);
+//    ini_propE(prop,nmass,fd);
+//  }
+//  if(dir==1){
+//    nmass = prop.size()/(12*12*fd.Nv[3]);
+//    qassert(nmass == 1);
+//    if(!pV.initialized){
+//      Geometry geo;fd.get_geo(geo);
+//      pV.init(geo);
+//    }
+//  }
+//  std::vector<Ty* > PTy;PTy.resize(1);
+//  PTy[0] = (Ty*) (qlat::get_data(pV).data());
+//  copy_propE(PTy, prop, fd, dir);
+//}
+
+//template<typename Ty, typename Ta>
+//void copy_propE(std::vector<Propagator4dT<Ty > > &pV, EigenMTa &prop, qlat::fft_desc_basic &fd, int dir=0){
+//  int nmass = 0;
+//  if(dir==0){nmass = pV.size();ini_propE(prop,nmass,fd);}
+//  if(dir==1){
+//    nmass = prop.size()/(12*12*fd.Nv[3]);
+//    bool do_init = false;
+//    if(pV.size() != (LInt) nmass){do_init = true;}
+//    if(pV.size() > 0){if(!pV[0].initialized){do_init = true;}}
+//    if(do_init)
+//    {
+//      pV.resize(0);
+//      Geometry geo;fd.get_geo(geo);
+//      pV.resize(nmass);for(int i=0;i<nmass;i++){pV[i].init(geo);}
+//    }
+//  }
+//  std::vector<Ty* > PTy;PTy.resize(nmass);
+//  for(int im=0;im<nmass;im++){PTy[im] = (Ty*) (qlat::get_data(pV[im]).data());}
+//  copy_propE(PTy, prop, fd, dir);
+//}
+//
+//template<typename Ty, typename Ta>
+//void copy_prop4d_to_propE(EigenMTa &prop, std::vector<Propagator4dT<Ty > > &pV1, qlat::fft_desc_basic &fd){
+//  copy_propE(pV1, prop, fd, 0);
+//}
+//template<typename Ty, typename Ta>
+//void copy_propE_to_prop4d(std::vector<Propagator4dT<Ty > > &pV1, EigenMTa &prop, qlat::fft_desc_basic &fd){
+//  copy_propE(pV1, prop, fd, 1);
+//}
+//
+//template<typename Ty, typename Ta>
+//void copy_prop4d_to_propE(EigenMTa &prop, Propagator4dT<Ty > &pV1, qlat::fft_desc_basic &fd){
+//  copy_propE(pV1, prop, fd, 0);
+//}
+//template<typename Ty, typename Ta>
+//void copy_propE_to_prop4d(Propagator4dT<Ty > &pV1, EigenMTa &prop, qlat::fft_desc_basic &fd){
+//  copy_propE(pV1, prop, fd, 1);
+//}
+//
+
+template<typename Ty>
+void ini_propG(EigenTy& prop, const long nmass, size_t Nsize, bool clear = true){
+  if(long(prop.size()) != nmass){prop.resize(nmass);}
+  for(unsigned long i=0;i<prop.size();i++){
+    if(prop[i].size() != Nsize){
+      prop[i].resize(Nsize);
+    }
+    else{
+      if(clear){prop[i].set_zero();}
+    }
+  }
+}
+
+template <typename Ty >
+void check_prop_size(EigenTy& prop, fft_desc_basic& fd){
+  for(unsigned int i=0;i<prop.size();i++)
   {
-    for(unsigned int i=0;i<prop.size();i++){prop[i].resize(0);}prop.resize(0);
-    prop.resize(nmass*12*12*NTt);
-    for(unsigned int i=0;i<prop.size();i++){
-      prop[i].resize(Nxyz);
-    }
-  }
-  if(clear){zeroE(prop);}
-}
-
-////default dir == 0 from prop4d to propE
-template<typename Ty, typename Ta>
-void copy_propE(std::vector<Ty* > &pV1, EigenMTa &prop, qlat::fft_desc_basic &fd, int dir=0){
-  TIMER("Copy prop");
-  qassert(fd.order_ch == 0);
-  const LInt Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
-  const int NTt  = fd.Nv[3];
-  Geometry geo;fd.get_geo(geo);
-  int nmass = 0;
-  if(dir==0){nmass = pV1.size();ini_propE(prop,nmass,fd);}
-  if(dir==1){
-    nmass = prop.size()/(12*12*NTt);
-    qassert(int(pV1.size()) == nmass);
-    //if(pV1.size() != (LInt) nmass){
-    //  pV1.resize(0);
-    //  pV1.resize(nmass);for(int i=0;i<nmass;i++){pV1[i].init(geo);}
-    //}
-  }
-
-  for(int mi = 0;mi < nmass;mi++)
-  {
-    Ty* pv = pV1[mi];
-    /////Propagator4dT<Ty >& pv = pV1[mi];
-    qlat::vector_acc<Ta* > ps = EigenM_to_pointers(prop);
-    qacc_for(isp, long(NTt*Nxyz),{
-      int ti = isp/Nxyz;
-      int xi = isp%Nxyz;
-      /////qlat::WilsonMatrixT<Ty>& v0 =  pv.get_elem_offset(isp);
-      Ty* v0 = &pv[isp * 12 * 12];
-
-      for(int c0 = 0;c0 < 3; c0++)
-      for(int d0 = 0;d0 < 4; d0++)
-      for(int c1 = 0;c1 < 3; c1++)
-      for(int d1 = 0;d1 < 4; d1++)
-      {
-        LInt off = mi*12*12 + (d1*3+c1)*12+d0*3+c0;
-        if(dir==0){ps[off*NTt+ti][xi] = v0[(d0*3 + c0)*12 +  d1*3 + c1];}
-        if(dir==1){v0[(d0*3 + c0)*12 +  d1*3 + c1] = ps[off*NTt+ti][xi];}
-      }
-    });
-  }
-
-}
-
-template<typename Ty, typename Ta>
-void copy_propE(Propagator4dT<Ty > &pV, EigenMTa &prop, qlat::fft_desc_basic &fd, int dir=0){
-  int nmass = 1;
-  if(dir==0){
-    qassert(pV.initialized);
-    ini_propE(prop,nmass,fd);
-  }
-  if(dir==1){
-    nmass = prop.size()/(12*12*fd.Nv[3]);
-    qassert(nmass == 1);
-    if(!pV.initialized){
-      Geometry geo;fd.get_geo(geo);
-      pV.init(geo);
-    }
-  }
-  std::vector<Ty* > PTy;PTy.resize(1);
-  PTy[0] = (Ty*) (qlat::get_data(pV).data());
-  copy_propE(PTy, prop, fd, dir);
-}
-
-template<typename Ty, typename Ta>
-void copy_propE(std::vector<Propagator4dT<Ty > > &pV, EigenMTa &prop, qlat::fft_desc_basic &fd, int dir=0){
-  int nmass = 0;
-  if(dir==0){nmass = pV.size();ini_propE(prop,nmass,fd);}
-  if(dir==1){
-    nmass = prop.size()/(12*12*fd.Nv[3]);
-    bool do_init = false;
-    if(pV.size() != (LInt) nmass){do_init = true;}
-    if(pV.size() > 0){if(!pV[0].initialized){do_init = true;}}
-    if(do_init)
+    if(prop[0].size() != size_t(fd.Nvol)*12*12)
     {
-      pV.resize(0);
-      Geometry geo;fd.get_geo(geo);
-      pV.resize(nmass);for(int i=0;i<nmass;i++){pV[i].init(geo);}
+      print0("Size of Prop wrong. \n");
+      qassert(false);
     }
   }
-  std::vector<Ty* > PTy;PTy.resize(nmass);
-  for(int im=0;im<nmass;im++){PTy[im] = (Ty*) (qlat::get_data(pV[im]).data());}
-  copy_propE(PTy, prop, fd, dir);
-}
-
-template<typename Ty, typename Ta>
-void copy_prop4d_to_propE(EigenMTa &prop, std::vector<Propagator4dT<Ty > > &pV1, qlat::fft_desc_basic &fd){
-  copy_propE(pV1, prop, fd, 0);
-}
-template<typename Ty, typename Ta>
-void copy_propE_to_prop4d(std::vector<Propagator4dT<Ty > > &pV1, EigenMTa &prop, qlat::fft_desc_basic &fd){
-  copy_propE(pV1, prop, fd, 1);
-}
-
-template<typename Ty, typename Ta>
-void copy_prop4d_to_propE(EigenMTa &prop, Propagator4dT<Ty > &pV1, qlat::fft_desc_basic &fd){
-  copy_propE(pV1, prop, fd, 0);
-}
-template<typename Ty, typename Ta>
-void copy_propE_to_prop4d(Propagator4dT<Ty > &pV1, EigenMTa &prop, qlat::fft_desc_basic &fd){
-  copy_propE(pV1, prop, fd, 1);
 }
 
-template <typename Ta >
-void check_prop_size(EigenMTa &prop){
-  int sizep = prop.size();
-  if(sizep%(12*12) != 0 or sizep == 0)
+template <typename Ty >
+void copy_qprop_to_propG(EigenTy& res, std::vector<qpropT >& src, const qlat::Geometry &geo, int GPU = 1, int dir = 1)
+{
+  int nvec = 0;
+  if(dir == 1){
+    nvec = src.size();
+    res.resize(nvec);
+  }
+  if(dir == 0){
+    nvec = res.size();
+    src.resize(nvec);
+    for(int ni=0;ni<nvec;ni++){
+      src[ni].init(geo);
+      qassert(res[ni].size() == size_t(12*12*geo.local_volume()));
+    }
+  }
+  if(nvec == 0){return ;}
+  
+  for(int ni=0;ni<nvec;ni++)
   {
-    print0("Size of Prop wrong. \n");
-    qassert(false);
+    if(dir == 1){res[ni].copy_from((Complexq*) qlat::get_data(src[ni]).data(), 12*12*geo.local_volume(), GPU);}
+    if(dir == 0){res[ni].copy_to((Complexq*) qlat::get_data(src[ni]).data(), GPU);}
   }
 }
 
-template <typename Ta >
-void ini_resE(EigenVTa &res, int nmass, qlat::fft_desc_basic &fd){
+template <typename Ty >
+void copy_propG_to_qprop(std::vector<qpropT >& res, EigenTy& src, const qlat::Geometry &geo, int GPU = 1)
+{
+  copy_qprop_to_propG(src, res, geo, 0, GPU);
+}
+
+template <typename Ty >
+void ini_resE(qlat::vector_acc<Ty > &res, int nmass, qlat::fft_desc_basic &fd){
   int NTt  = fd.Nv[3];
   LInt Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
   int do_resize = 0;
   if((LInt) res.size() != (LInt) nmass*NTt * Nxyz){do_resize=1;}
   if(do_resize == 1)
   {
     res.resize(0);res.resize(nmass*NTt * Nxyz);
   }
   clear_qv(res);
 }
 
-inline std::vector<int >  get_sec_map(int dT,int nt){
+inline std::vector<int >  get_map_sec(int dT,int nt){
   std::vector<int > map_sec;map_sec.resize(nt);
   int secN = 2*nt/dT;double lensec = nt/(1.0*secN);
   int tcount = 0;
   int t0 = 0;
   for(int si=0;si<secN;si++)
   {
-    for(int t=t0;t <= (si+1)*lensec;t++)
+    for(int t=t0;t < (si+1)*lensec;t++)///boundary with the same sector?
     {
+      qassert(t < nt);
       map_sec[t] = si;
       tcount = tcount + 1;
     }
     t0 = tcount;
   }
   return map_sec;
 
@@ -633,11 +875,67 @@
     double v0 = 0.0;
     for(int i=0;i<3;i++){v0 += (2.0*PI * src[i] * pos[i]/Lat[i]);}
 
     phases[isp] = Ty(std::cos(v0), -1.0* std::sin(v0));
   }
 }
 
+/////V -- 12a x 12b   to   12b x 12a -- V
+template<typename Ty>
+void copy_qprop_to_propE(std::vector<qlat::vector_acc<Ty > >& Eprop, std::vector<qpropT >& src, int dir = 1){
+  TIMERA("copy_qprop_to_propE");
+  const int nmass = src.size();
+  std::vector<Ty* > ps;ps.resize(nmass);
+  
+  for(int mi=0;mi<nmass;mi++){
+    qassert(src[mi].initialized);
+    ps[mi] = (Ty*) qlat::get_data(src[mi]).data();
+  }
+
+  const qlat::Geometry &geo = src[0].geo();
+  fft_desc_basic& fd = get_fft_desc_basic_plan(geo);
+  if(dir == 1){ini_propE(Eprop, nmass, fd);}
+  
+  ///const long sizeF = geo.local_volume();
+  const long nvec  = Eprop.size()/nmass;
+  const long sizeF = Eprop[0].size();
+  qassert(nvec * sizeF == 12*12*geo.local_volume());
+
+  ////V x 12 a x 12 b to 12b x 12a x V
+  for(int mi=0;mi<nmass;mi++)
+  for(long i=0;i<nvec;i++)
+  {
+    if(dir == 1)cpy_data_thread(Eprop[mi*nvec + i].data(), &ps[mi][i*sizeF], sizeF, 1, false);
+    if(dir == 0)cpy_data_thread(&ps[mi][i*sizeF], Eprop[mi*nvec + i].data(), sizeF, 1, false);
+  }
+  qacc_barrier(dummy);
+}
+
+template<typename Ty>
+void copy_propE_to_qprop(std::vector<qpropT >& src, std::vector<qlat::vector_acc<Ty > >& Eprop){
+  copy_qprop_to_propE(Eprop, src, 0);
+}
+
+template<typename Ty>
+void noise_to_propT(qpropT& prop, qnoiT& noi){
+  qassert(noi.initialized);
+  const Geometry& geo = noi.geo();
+
+  if(!prop.initialized){prop.init(geo);}
+
+  Ty* res = (Ty*) qlat::get_data(prop).data();
+  Ty* src = (Ty*) qlat::get_data(noi ).data();
+
+  const long Nvol = geo.local_volume();
+
+  for(int d0=0;d0<12;d0++){
+    cpy_data_thread(&res[(d0*12+d0)*Nvol + 0], src, Nvol, 1, false);
+  }
+  qacc_barrier(dummy);
+
+}
+
+
 
 }
 
 #endif
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_eigensys.h` & `qlat-0.9/include/qlat/vector_utils/utils_eigensys.h`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 #include "utils_Matrix_prod.h"
 #include "utils_construction.h"
 #include "check_fun.h"
 #include "utils_smear_vecs.h"
 
 ///#define SUMMIT 0
 
-#define Elocal std::vector<qlat::vector<Complexq > >
 ////#define Vlocal qlat::vector_acc<Complexq >
+#define Elocal std::vector<qlat::vector<Complexq > >
 #define Vlocal qlat::vector_gpu<Complexq >
 #define EIGENERROR 1e-11
 
 namespace qlat{
 
 struct eigen_ov {
-  qlat::fft_desc_basic* fdp;
+  Geometry geo;
 
   Elocal Mvec;     //  nvec --> 2*bfac --> b_size*6
   Elocal Mvec_Sm;  //  Smeared eigensystem 
 
   bool enable_smearE;
 
   ////int Edouble;
@@ -84,15 +84,15 @@
   ////3pt function
   //EigenV alpha_list3pt;
   //EigenV alpha_list3ptC;
   //EigenV alpha3pt;
   //EigenV alpha3pt_ker_low;
 
   /////Construction and memory allocations
-  eigen_ov(qlat::fft_desc_basic &fd,int n_vec_or, long long bsize0=-1, double extra_mem_factor_set = 0.82);
+  eigen_ov(const Geometry& geo_,int n_vec_or, long long bsize0=-1, double extra_mem_factor_set = 0.82);
 
   void copy_evec_to_GPU(int nini);
   template <typename Ty >
   void copy_FieldM_to_Mvec(Ty* src, int ncur, int sm = 0, int dir = 1 , bool data_GPU = false);
   template <typename Ty >
   void copy_to_FieldM(Ty* src, int ncur, int sm = 0, bool data_GPU = false){
     copy_FieldM_to_Mvec(src, ncur, sm, 0, data_GPU);
@@ -149,15 +149,14 @@
   void setup_gpufac(int nprop=1);
   void allocate_GPU_mem(int nprop=1);
   void clear_GPU_mem(int cpu_also = 0);
 
   ~eigen_ov()
   {
     clear_GPU_mem(1);
-    fdp = NULL;
   }
 
 };
 
 void eigen_ov::setup_bfac(long long bsize0)
 {
   LInt bcut = 300;
@@ -204,18 +203,19 @@
   if(bfac%6 !=0){print0("Cannot understand sites on bfac %5ld, bsize %10ld, Total %10ld !\n",
     bfac, b_size, noden*6);abort_r("");}
   if((noden*6)%bfac !=0){print0("Cannot understand sites on node*6/Nt %10ld bfac %10ld!\n",noden*6/Nt,bfac);abort_r("");}
   if(bfac%(Nt*6) !=0){print0("Cannot understand sites on node %10ld bfac %10ld, tsize %5d!\n",noden,bfac,Nt);abort_r("");}
 
 }
 
-eigen_ov::eigen_ov(qlat::fft_desc_basic &fd,int n_vec_or, long long bsize0, double extra_mem_factor_set)
+eigen_ov::eigen_ov(const Geometry& geo_,int n_vec_or, long long bsize0, double extra_mem_factor_set)
 {
-  fdp  = &fd;
-  if(fd.order_ch != 0){abort_r("Currently not supported for change fd order.\n ");}
+  geo = geo_;
+  fft_desc_basic& fd = get_fft_desc_basic_plan(geo);
+  ///if(fd.order_ch != 0){abort_r("Currently not supported for change fd order.\n ");}
 
   rho = 1.5;
   Eeigenerror = EIGENERROR;
   num_zero = 0;
   one_minus_halfD = 1;
 
   nx = fd.nx;ny = fd.ny;nz = fd.nz;nt = fd.nt;
@@ -282,15 +282,15 @@
   if(totalD < mem_prop + 64*memV){
     print0("===GPU Memory too small, Total %.3e, prop %.3e, 30V %.3e, increase nodes! \n", totalD, mem_prop, 64*memV);
     qassert(false);
   }
 
   int vfac = ncutgpu;int vini = 8 * vfac;
   int vres = int((totalD*extra_mem_factor*sm_factor - mem_prop )/memV); 
-  if(fdp->rank != 0){vres=0;};sum_all_size(&vres, 1);
+  if(qlat::get_id_node() != 0){vres=0;};sum_all_size(&vres, 1);
   /////TODO Need global sum and average the final result?
   /////TODO need to test the continuous memory less thant 8GB
 
   if(vres > n_vec ){
     ncutgpu = 0;ncutbuf = n_vec;
     //ncutgpu = n_vec;ncutbuf = 0;
   }
@@ -352,15 +352,14 @@
   alpha_list.resize(0);eval_list.resize(0);
 
   /////ptmp.resize(0);stmp.resize(0);
   if(cpu_also == 1)
   {
     Mvec.resize(0);
     Mvec_Sm.resize(0);
-    fdp = NULL;
   }
 
   gpu_mem_set = false;
 }
 
 void eigen_ov::load_eivals(const std::string& enamev,double rho_or,double Eerr, int nini)
 {
@@ -425,15 +424,14 @@
 
 template <typename Ty >
 void eigen_ov::copy_FieldM_to_Mvec(qlat::FieldM<Ty , 12>& src, int ncur, int sm, int dir )
 {
   TIMERA("COPY Eigen Vectors Mvec");
   if(ncur >= n_vec){abort_r("Cannot copy to position larger than n_vec ! \n");}
   if(dir == 0){if(!src.initialized){
-    Geometry geo;fdp->get_geo(geo);
     src.init(geo);
   }}
   Ty* s0 = (Ty*) qlat::get_data(src).data();
   int data_GPU = 0; ////do copies only from CPU here
   copy_FieldM_to_Mvec(s0, ncur, sm, dir, data_GPU);
 }
 
@@ -567,43 +565,42 @@
 
 template <typename Tg >
 void eigen_ov::smear_eigen(const std::string& Ename_Sm,
   const GaugeFieldT<Tg >& gf, const double width, const int step,
   const CoordinateD& mom, const bool smear_in_time_dir)
 {
   TIMER("smear eigen system");
-  Geometry geo;fdp->get_geo(geo);
   ////load if exist
   if(Ename_Sm != std::string("NONE") and get_file_size_MPI(Ename_Sm.c_str(), true) != 0){
     load_eigen_Mvec(Ename_Sm, 1);
     return ;
   }
 
   long La = 2*bfac/BFAC_GROUP_CPU;
   long Lb = BFAC_GROUP_CPU*n_vec*long(b_size);
   print_mem_info("Before Eigen Memory Allocate");
   resize_EigenM(Mvec_Sm , La, Lb);enable_smearE = true;
   print_mem_info("Eigen Memory Allocate Done");
 
   const int each = 12;
-  long Ncopy = fdp->Nvol * 12;
+  long Ncopy = geo.local_volume() * 12;
   qlat::vector_gpu<Complexq > buf;buf.resize(each * Ncopy);
 
   move_index mv_idx;
   std::vector<long > job =  job_create(n_vec, each);
   for(LInt ji = 0; ji < job.size()/2 ; ji++)
   {
     int flag = 0;
     ////copy to buf
     for(int iv=0;iv<job[ji*2 + 1];iv++){copy_to_FieldM(&buf[iv*Ncopy], job[ji*2 + 0] + iv,  0, true);}
-    flag = 0;mv_idx.dojob(buf.data(), buf.data(), 1, each , fdp->Nvol*12, flag, 1, true);
+    flag = 0;mv_idx.dojob(buf.data(), buf.data(), 1, each , geo.local_volume()*12, flag, 1, true);
 
     smear_propagator_gwu_convension_inner<Complexq, 4,each  , Tg>(buf.data(), gf, width, step, mom, smear_in_time_dir);
 
-    flag = 1;mv_idx.dojob(buf.data(), buf.data(), 1, each , fdp->Nvol*12, flag, 1, true);
+    flag = 1;mv_idx.dojob(buf.data(), buf.data(), 1, each , geo.local_volume()*12, flag, 1, true);
     ////copy from buf
     for(int iv=0;iv<job[ji*2 + 1];iv++){copy_FieldM_to_Mvec(&buf[iv*Ncopy], job[ji*2 + 0] + iv,  1, 1, true);}
   }
 
   ////erase smear
   {
   /////const SmearPlanKey& skey = get_smear_plan_key<Complexq, 4, each>(gf.geo(), smear_in_time_dir);
@@ -615,15 +612,14 @@
     save_eigen_Mvec(Ename_Sm, 1);
   }
 }
 
 void eigen_ov::save_eigen_Mvec(const std::string& ename, int sm)
 {
   if(sm == 1 and enable_smearE == false){print0("Could not save smear eigen without set it up.");return ;}
-  Geometry geo;fdp->get_geo(geo);
   io_vec& io_use = get_io_vec_plan(geo);
 
   const int nini = 0;
   const int ntotal = nini + n_vec;
   const bool read = false;
   inputpara in_write_eigen;
   FILE* file_write  = open_eigensystem_file(ename.c_str(), nini, ntotal, read , io_use , in_write_eigen , 2);
@@ -644,16 +640,20 @@
   print_mem_info("Eigen Memory Write Done");
 }
 
 void eigen_ov::load_eigen_Mvec(const std::string& ename, int sm, int nini, int checknorm)
 {
   int ntotal = nini + n_vec;
   Ftype norm_err  = 1e-3;
+  std::string val = get_env(std::string("q_eigen_norm_err"));
+  if(val != ""){norm_err = stringtodouble(val);}
+  int print_norms = 0; 
+  val = get_env(std::string("q_eigen_print_norm"));
+  if(val != ""){print_norms = stringtonum(val);}
 
-  Geometry geo;fdp->get_geo(geo);
   io_vec& io_use = get_io_vec_plan(geo);
 
   long La = 2*bfac/BFAC_GROUP_CPU;
   long Lb = BFAC_GROUP_CPU*n_vec*long(b_size);
   print_mem_info("Before Eigen Memory Allocate");
   if(sm == 0){resize_EigenM(Mvec    , La, Lb);}
   if(sm == 1){resize_EigenM(Mvec_Sm , La, Lb);enable_smearE = true;}
@@ -673,16 +673,18 @@
     /////load from file
     load_eigensystem_vecs(file_read ,   buf, io_use , in_read_eigen , 0, job[ji*2 + 1]);
     ////copy to Mvec or Mvec_Sm
     for(int iv=0;iv<job[ji*2 + 1];iv++){
       if(checknorm == 1 and sm == 0){
         Ftype* Psrc = (Ftype*) qlat::get_data(buf[iv]).data();
         Ftype normf = get_norm_vec(Psrc, noden);
+        if(print_norms == 1){
+        print0("Eigen vector %8d, norm 1.0 + %+.8e flag . \n", int(job[ji*2 + 0] + iv + nini), normf - 1.0);}
         if(fabs(normf - 1.0) > norm_err){
-          print0("Eigen vector %d, norm %.3e wrong. \n", int(job[ji*2 + 0] + iv), normf);
+          print0("Eigen vector %d, norm 1.0 + %.8e wrong. \n", int(job[ji*2 + 0] + iv + nini), normf - 1.0);
           abort_r("");
         }
       }
 
       copy_FieldM_to_Mvec(buf[iv], job[ji*2 + 0] + iv, sm  );
     }
   }
@@ -786,14 +788,15 @@
 
 void eigen_ov::initialize_mass()
 {
   std::vector<double> mass;mass.push_back(0.0);
   initialize_mass(mass,12,one_minus_halfD);
 }
 
+
 void prop_L_device(eigen_ov& ei,Complexq *src,Complexq *props, int Ns, std::vector<double> &mass, int mode_sm = 0,int one_minus_halfD_or=1)
 {
   int mN   = mass.size();
 
   TIMER_FLOPS("==prop_L");
 
   long long Lat = ei.noden;
@@ -830,14 +833,15 @@
   int& ncutbuf     = ei.ncutbuf;
   int& num_zero    = ei.num_zero;
 
   bool dummy_test = false;
 
   int Ng = 0;if(ncutgpu!=0){Ng = ei.n_vec/ncutgpu + 1;}
   int nini = 0;
+  /////each group have ncutgpu of vectors
   for(int ng=0;ng<Ng + 1;ng++)
   {
     if(nini >= ei.n_vec)break;
     int  ncur = 0;
     if(nini>=ncutbuf){
       ncur = ncutgpu;
     }else{ncur = ncutbuf;}
@@ -845,21 +849,22 @@
     ei.copy_evec_to_GPU(nini);
 
     {
     long m = ncur;
     long n = Ns;
     long w = b_size;
 
-    TIMER_FLOPS("vec reduce");
-    long long vGb = 2*bfac*m*n*w;
-    int Fcount0   = 6 + 2;  
-    timer.flops  += vGb*Fcount0;
+    TIMERA("prop low vec reduce");
+    //TIMER_FLOPS("vec reduce");
+    //long long vGb = 2*bfac*m*n*w;
+    //int Fcount0   = 6 + 2;  
+    //timer.flops  += vGb*Fcount0;
 
     std::vector<long > jobA = job_create(2*bfac, ei.BFAC_GROUP_CPU);
-    if(nini > ncutbuf){jobA = job_create(2*bfac, ei.bfac_group);}
+    if(nini > ncutbuf){jobA = job_create(2*bfac, ei.bfac_group);} //// vector size groups
     for(LInt jobi=0;jobi < jobA.size()/2; jobi++)
     {
       long bini = jobA[jobi*2 + 0]; long bcut = jobA[jobi*2+1];
       Complexq* rp = &alpha_bfac[(bini + 0)*m*n + 0];
       Complexq* Ep = ei.getEigenP(nini, bini*b_size, sm0);
       Complexq* sp = &src[       (bini + 0)*n*w + 0];
       matrix_prod_gpu(Ep, sp, rp, m,n, w , bcut, true, dummy_test);
@@ -953,56 +958,58 @@
   ////print_sum(props, 2*bfac*  mN*Ns*b_size, "=====props", 1);
 
   /////untouch_GPU(ei.eval_list, ei.eval_list_size);
   //////#endif
 
 }
 
-////dir == 0, from src to EigenM res
-////dir == 1 from EigenM res to src
-template <typename Ty >
-void copy_eigen_prop_to_EigenM(Ty* src, EigenM& res, LInt b_size, int nmass, qlat::fft_desc_basic& fd, int dir = 0,int GPU = 1)
+////dir == 1, from src to EigenG res
+////dir == 0  from EigenG res to src
+template <typename T, typename Ty>
+void copy_eigen_prop_to_EigenG(std::vector<qlat::vector_gpu<Ty > >& res, T* src, 
+  LInt b_size, int nmass, qlat::fft_desc_basic& fd, int GPU = 1, int dir = 1)
 {
-  if(nmass == 0){return ;}
-  if(dir == 0){ini_propE(res, nmass, fd, false);}
+  if(nmass == 0){res.resize(0); return ;}
+  if(dir == 1){
+    ini_propG(res, nmass, 12*12*size_t(fd.Nvol), false);
+  }
 
-  int Ns    = 12*nmass;
+  int Ns    = nmass*12;
   int  NTt  = fd.Nv[3];
   LInt Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
   LInt total = 6*NTt*Nxyz;
   if(total % b_size != 0){abort_r("eigen system configurations wrong! \n");}
   LInt bfac = total/(b_size);
   LInt each  = Nxyz; if(b_size < Nxyz){each = b_size;}
   LInt group = (2*total)/each;
 
   //for(unsigned int d1=0;d1<12;d1++)
   //for(int ti=0; ti < NTt; ti++)
   for(int d0=0;d0<Ns;d0++)
   for(LInt gi=0;gi<group;gi++)
   {
+    int massi = d0/12;
+    int d0i   = d0%12;
     LInt mi = gi*each;
 
     ////index for res
     LInt d1 =  mi/(NTt*Nxyz);
     LInt ti = (mi/(Nxyz))%NTt;
     LInt vi =  mi%(Nxyz);
 
     ////index for src
     int chi = mi/(total);
     LInt xi = mi%(total);
     long bi = xi/b_size;
     long bj = xi%b_size;
 
-    Ty* s0       = &src[(chi*bfac+bi)*Ns*b_size  + d0*b_size + bj];
-    Complexq* tems = (Complexq*) qlat::get_data(res[(d0*12 + d1)*NTt+ti]).data();
-    Complexq* s1 = &tems[vi];
-    if(dir == 0){cpy_data_thread(s1, s0, each , GPU, false);}
-    if(dir == 1){cpy_data_thread(s0, s1, each , GPU, false);}
-
-    /////useS[(chi*bfac+bi)*Ns*b_size  + is*b_size + bj] = s0[(d0*12 + d1)*NTt+ti][vi];
+    T* s0   = &src[(chi*bfac+bi)*Ns*b_size  + d0*b_size + bj];
+    Ty* s1  = (Ty*) &res[massi][((d0i*12 + d1)*NTt+ti)*Nxyz + vi];
+    if(dir == 1){cpy_data_thread(s1, s0, each , GPU, false);}
+    if(dir == 0){cpy_data_thread(s0, s1, each , GPU, false);}
 
   }
   qacc_barrier(dummy);
 
 }
 
 /////res in format src 12* sink 12 --> Nt * Nxyz
@@ -1040,35 +1047,14 @@
   if(src.size() == 0){return ;}
   ////qlat::Geometry& geo = src[0].geo();
   long nV = src.size();
   if(res.size() != src.size()){res.resize(nV);}
   for(int iv=0;iv<nV;iv++)FieldM_src_to_FieldM_prop(src[iv], res[iv], GPU, false);
   qacc_barrier(dummy);
 
-  //bool do_ini = true;if(res.size() == src.size())if(res[src.size()-1].initialized){do_ini = false;}
-  //if(do_ini){res.resize(nV);for(int iv=0;iv<nV;iv++){res[iv].init(geo);}}
-
-  ////std::vector<int > nv, Nv, mv;
-  ////geo_to_nv(geo, nv, Nv,mv);
-  //long Ncopy = geo.local_volume();
-
-  //Ty* s0 = NULL; Ty* s1 = NULL;Ty* st = NULL;
-  //for(int iv=0;iv<nV;iv++)
-  //{
-  //  s0 = (Ty*) qlat::get_data(src[iv]).data();
-  //  st = (Ty*) qlat::get_data(res[iv]).data();
-  //  for(unsigned int d0=0;d0<12;d0++)
-  //  {
-  //    //////diagonal elements
-  //    s1 = &st[(d0*12+d0)*Ncopy + 0];
-  //    cpy_data_thread(s1, s0, Ncopy , GPU, false);
-  //  }
-  //}
-  //qacc_barrier(dummy);
-
 }
 
 ////assumed civ == n*12 with n the source indices, 12 the sink indices 
 template <typename Ty, int civ >
 void copy_eigen_src_to_FieldM(qlat::vector_gpu<Ty >& src, std::vector<qlat::FieldM<Ty , civ> >& res, LInt b_size, qlat::fft_desc_basic& fd, int dir = 0, int GPU = 1, bool rotate = false)
 {
   TIMERA("copy_eigen_src_to_FieldM");
@@ -1130,15 +1116,15 @@
     ////index for src
     int chi = mi/(total);
     LInt xi = mi%(total);
     long bi = xi/b_size;
     long bj = xi%b_size;
 
     s0 = &psrc[(chi*bfac+bi)*nV*b_size  + d0*b_size + bj];
-    st = (Complexq*) qlat::get_data(res[d0a]).data();
+    st = (Ty*) qlat::get_data(res[d0a]).data();
     s1 = &st[((d0b*12 + d1)*NTt+ti)*Nxyz + vi];
 
     if(dir == 0){cpy_data_thread(s1, s0, each , GPU, false);}
     if(dir == 1){cpy_data_thread(s0, s1, each , GPU, false);}
   }
 
   qacc_barrier(dummy);
@@ -1159,11 +1145,11 @@
 
 
 
 }
 
 #undef  Elocal
 #undef  EIGENERROR
-////#undef  Vlocal
+#undef  Vlocal
 
 #endif
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_fft_desc.h` & `qlat-0.9/include/qlat/vector_utils/utils_fft_desc.h`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,16 @@
     Nx =-1;  Ny =-1;  Nz =-1;  Nt =-1;
     mx =-1;  my =-1;  mz =-1;  mt =-1;
     ////Order change of memory within a node
   
     Nmpi  = qlat::get_num_node();
     rank  = qlat::get_id_node();
 
+    qassert(geo.node_site != qlat::Coordinate());
+
     ////set nv, Nv, mv, iniv
     geo_to_nv(geo, nv, Nv, mv);
 
     qlat::Coordinate ts = geo.coordinate_from_index(0);
     qlat::Coordinate gs = geo.coordinate_g_from_l(ts);
     iniv.resize(4);for(unsigned int i=0;i<4;i++){iniv[i] = gs[i];}
 
@@ -74,14 +76,16 @@
     set_variable();
     ////check_mem();
   }
 
   inline void set_variable();
   inline void print_info();
   inline long get_mi_curr(int dir=3);
+  inline long get_tmi_curr();
+  inline long get_xyzmi_curr();
   inline void check_mem();
   inline Coordinate coordinate_l_from_index(LInt isp) const;
   inline Coordinate coordinate_g_from_g_index(LInt isp) const ;
   inline Coordinate coordinate_g_from_index(LInt isp, int rank_set = -1) const;
   inline LInt index_g_from_local(LInt isp, int rank_set = -1) const;
   //////LInt index_g_from_g_coordinate(std::vector<int > pos);
   inline LInt index_g_from_g_coordinate(int t, int z, int y, int x) const;
@@ -133,14 +137,26 @@
     if(Nv[0] == nv[0]){re += tmi*mz*my*mx;}
     if(Nv[0] != nv[0]){re = re*(mt) + tmi;}
   }
 
   return re;
 }
 
+inline long fft_desc_basic::get_tmi_curr()
+{
+  int tmi = Pos0[rank][3]/Nt;
+  return tmi;
+}
+
+inline long fft_desc_basic::get_xyzmi_curr()
+{
+  return get_mi_curr(3);
+}
+
+
 inline Coordinate fft_desc_basic::coordinate_l_from_index(LInt isp) const
 {
   if(variable_set == -1){abort_r("fft_desc not set! \n");}
 
   ////std::vector<int > g0;g0.resize(4);for(int i=0;i<4;i++){g0[i] = 0;}
   Coordinate g0;for(int i=0;i<4;i++){g0[i] = 0;}
   g0[3] += isp/(Nv[0]*Nv[1]*Nv[2]);long tem = isp%(Nv[0]*Nv[1]*Nv[2]);
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_float_type.h` & `qlat-0.9/include/qlat/vector_utils/utils_float_type.h`

 * *Files 2% similar despite different names*

```diff
@@ -71,19 +71,19 @@
 
 /////May have some errors for python, mem buf, mem leak
 ////#define EigenM qlat::vector<Evector >
 #define EigenM  std::vector<Evector >
 ////
 
 #define qnoi qlat::FieldM<Complexq, 1>
-//////dim 12*12 --> Nt --> Nxyz
-#define qprop  qlat::FieldM<Complexq, 12*12>
-
 #define qnoiT qlat::FieldM<Ty, 1>
+
 //////dim 12*12 --> Nt --> Nxyz
+/////only memory size and geo are used, donot use others
+#define qprop   qlat::FieldM<Complexq, 12*12>
 #define qpropT  qlat::FieldM<Ty, 12*12>
 
 /////Fields for staggered fermion
 #define colorFD qlat::FieldM<Complex , 3>
 #define colorFF qlat::FieldM<Complexq, 3>
 #define colorFT qlat::FieldM<Ty, 3>
 
@@ -276,15 +276,23 @@
     if(dummy)qacc_barrier(dummy);
     return ;
   }
   #endif
 
   ////#pragma omp parallel for
   ////for(size_t isp=0;isp<size;isp++){  a[isp] = 0;}
-  memset((void*) a, 0, sizeof(Ty) * size);
+  const unsigned int Nv = omp_get_max_threads();
+  const unsigned int dN = (size + Nv - 1) / Nv;
+  #pragma omp parallel for
+  for(unsigned int isp=0;isp<Nv;isp++)
+  {
+    Ty* tmp = &a[isp * dN + 0];
+    const int step = isp*(dN+1) <= size ? dN : (size - isp*dN); 
+    memset((void*) tmp, 0, sizeof(Ty) * step);
+  }
 }
 
 template<typename Ty>
 void clear_qv(qlat::vector_acc<Ty > &G, bool dummy = true)
 {
   zero_Ty(G.data(), G.size(), 1 , dummy);
 }
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_gammas.h` & `qlat-0.9/include/qlat/vector_utils/utils_gammas.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_gaugefield.h` & `qlat-0.9/include/qlat/vector_utils/utils_gaugefield.h`

 * *Files 26% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 #include "general_funs.h"
 
 //////TODO
 
 namespace qlat
 {
 
-template <class T>
-void set_rand_link(GaugeFieldT<T> &gf, const int seed = -1)
+template <class Td>
+void set_rand_link(GaugeFieldT<Td> &gf, const int seed = -1)
 {
   if(seed == -1)
   {
     qacc_for(isp, gf.field.size(), { set_unit(gf.get_elem_offset(isp), 1.0);});
   }else{
     //T* res = (T*) gf.get_elem_offset(0).p;
     const Geometry& geo = gf.geo();
-    T* res = (T*) qlat::get_data(gf).data();
-    random_Ty(res, geo.local_volume()*geo.multiplicity*sizeof(ColorMatrixT<T>)/sizeof(T), 1, seed);
+    qlat::ComplexT<Td>* res = (qlat::ComplexT<Td>*) qlat::get_data(gf).data();
+    random_Ty(res, geo.local_volume()*geo.multiplicity*sizeof(ColorMatrixT<Td>)/(sizeof(Td)*2), 1, seed);
 
     //qacc_for(isp, gf.field.size(), { set_unit(gf.get_elem_offset(isp), 1.0);});
-    ColorMatrixT<T> unit;set_unit(unit, 1.0);
+    ColorMatrixT<Td> unit;set_unit(unit, 1.0);
     /////TODO This function cannot be done on GPU
     /////Eigen normalize/normalized problem 
     for(long isp=0;isp<gf.field.size();isp++)
     {
       gf.get_elem_offset(isp) = gf.get_elem_offset(isp) * (1/2.0) + unit;
       unitarize(gf.get_elem_offset(isp));
     }
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_grid_src.h` & `qlat-0.9/include/qlat/vector_utils/utils_grid_src.h`

 * *Files 9% similar despite different names*

```diff
@@ -143,15 +143,58 @@
     }
     ////Check Source Position
     fflush_MPI();
   }
 
 }
 
+template <typename Ty>
+void check_noise_high(qlat::FieldM<Ty, 1>& noise, std::vector<int >& sinkt, double& factor)
+{
+  const qlat::Geometry& geo = noise.geo();
+  ////const long Nvol = geo.local_volume();
+  fft_desc_basic& fd = get_fft_desc_basic_plan(geo);
+
+  const long Nxyz = fd.Nx*fd.Ny*fd.Nz;
+
+  std::vector<double > count;
+  count.resize(fd.nt);
+  for(int i=0;i<fd.nt;i++){count[i] = 0;}
+
+  qthread_for(ti, fd.Nt, {
+    const int tg = ti + fd.init;
+
+    for(long isp=0;isp<Nxyz;isp++)
+    {
+      const long off = ti * Nxyz + isp;
+      {
+        double tem_source =  qlat::qnorm(noise.get_elem_offset(off));
+        if(qnorm(tem_source)> 1e-3)
+        {
+          count[tg] += 1;
+        }
+      }
+    }
+  });
 
+  sum_all_size(count.data(), count.size());
+  sinkt.resize(0);
+  factor = -1;
+  for(int t=0;t<fd.nt;t++){
+    if(count[t] > 0){
+      if(factor == -1){
+        factor = count[t] / fd.vol;
+      }else{
+        qassert(factor == count[t] / fd.vol);
+      }
+      sinkt.push_back(t);
+    }
+  }
+
+}
 
 /////get positions by spatial setups
 inline void grid_list_pos(const Coordinate& off_L,qlat::vector_acc<long > &Ngrid)
 {
   TIMERA("===grid_list_pos===")
   if(off_L.size() != 4){abort_r("dimention of positions wrong!\n ");}
   int Ntot = off_L[0]*off_L[1]*off_L[2];
@@ -401,38 +444,38 @@
 
   if(printv >= 1){printf("rank %d, number of non-zeros %ld \n", qlat::get_id_node(), total);}
 
 }
 
 template <class Ty, int civ>
 void get_mix_color_src(qlat::FieldM<Ty , civ>& src, const Coordinate& sp, 
-  const std::vector<double >& phases, const FieldSelection& fsel, const int type_src = 0, int seed = 0)
+  const std::vector<double >& phases, const FieldSelection& fsel, const int type_src = 0, int seed = 0, const int offT = -1)
 {
   TIMER("get_mix_color_src");
   qassert(src.initialized);
   const qlat::Geometry& geo = src.geo();
   const long V_local = geo.local_volume();
 
   Ty* srcP = (Ty*) qlat::get_data(src).data();
-  zero_Ty(srcP, V_local*3, 0);
+  zero_Ty(srcP, V_local*civ, 0);
 
-  qlat::vector_acc<Ty > color_phases(3);
+  qlat::vector_acc<Ty > color_phases(phases.size());
   const int tsrc = sp[3];
-  for(int c=0;c<3;c++){
+  for(unsigned int c=0;c<color_phases.size();c++){
     double r = phases[c];
     color_phases[c] = Ty(std::cos(r), std::sin(r));
   }
   fft_desc_basic fd(geo);
 
   if(type_src == 0) ////point src
   {
     if(fd.coordinate_g_is_local(sp)){
       LInt isp = fd.index_l_from_g_coordinate(sp);
-      for(int c=0;c<3;c++){
-        srcP[isp*3 + c] = color_phases[c];
+      for(int c=0;c<civ;c++){
+        srcP[isp*civ + c] = color_phases[c];
       }
     }
   }
 
   if(type_src == 1) ////Wall src
   {
     std::vector<qlat::RngState > rsL;rsL.resize(omp_get_max_threads());
@@ -442,30 +485,30 @@
     }
     
     qthread_for(isp, geo.local_volume(), {
       Coordinate xl = geo.coordinate_from_index(isp);
       Coordinate xg = geo.coordinate_g_from_l(xl);
       if(xg[3] == tsrc){
         qlat::RngState& rs = rsL[omp_get_thread_num()];
-        for(int c=0;c<3;c++){
+        for(int c=0;c<civ;c++){
           double r = 2 * PI * qlat::u_rand_gen(rs);
-          srcP[isp*3 + c] = Ty(std::cos(r), std::sin(r));
+          srcP[isp*civ + c] = Ty(std::cos(r), std::sin(r));
         }
       }
     });
   }
 
   if(type_src == 11) ////Wall src tests
   {
     qacc_for(isp, geo.local_volume(), {
       Coordinate xl = geo.coordinate_from_index(isp);
       Coordinate xg = geo.coordinate_g_from_l(xl);
       if(xg[3] == tsrc)
-      for(int c=0;c<3;c++){
-        srcP[isp*3 + c] = color_phases[c];
+      for(int c=0;c<civ;c++){
+        srcP[isp*civ + c] = color_phases[c];
       }
     });
   }
 
   if(type_src == 2) ////sparse src
   {
     std::vector<qlat::RngState > rsL;rsL.resize(omp_get_max_threads());
@@ -477,25 +520,80 @@
     qthread_for(isp, geo.local_volume(), {
       const long rank = fsel.f_local_idx.get_elem_offset(isp);
       if(rank >= 0){
         const Coordinate xl  = geo.coordinate_from_index(isp);
         const Coordinate xg  = geo.coordinate_g_from_l(xl);
         if(xg[3] == tsrc){
           qlat::RngState& rs = rsL[omp_get_thread_num()];
-          for(int c=0;c<3;c++){
+          for(int c=0;c<civ;c++){
             double r = 2 * PI * qlat::u_rand_gen(rs);
-            srcP[isp*3 + c] = Ty(std::cos(r), std::sin(r));
+            srcP[isp*civ + c] = Ty(std::cos(r), std::sin(r));
           }
         }
       }
     }); 
   }
 
+  if(type_src == 20) ////T grid src, all spatial the same for momenta projections
+  {
+    qassert(offT > 0);qassert(fd.nt % offT == 0);
+    qassert(long(color_phases.size()) == fd.nt/offT * civ);
+    /////qlat::RngState rs = qlat::RngState(seed + type_src*10 + qlat::get_id_node() * 5);
+    Coordinate tem = sp;
+    for(int ti = 0; ti < fd.nt/offT; ti ++)
+    {
+      tem[3] = (sp[3] + ti * offT) % fd.nt;
+      if(fd.coordinate_g_is_local(tem)){
+        LInt isp = fd.index_l_from_g_coordinate(tem);
+        for(int c=0;c<civ;c++){
+          ////double r = 2 * PI * qlat::u_rand_gen(rs);
+          ////srcP[isp*civ + c] = Ty(std::cos(r), std::sin(r));;
+          srcP[isp*civ + c] = color_phases[ti*civ + c];
+        }
+      }
+    }
+  }
+
 
 }
 
+template <class Ty>
+void vec_apply_cut(qlat::vector_gpu<Ty >& res, const Coordinate& sp, const double rmax, const Geometry& geo)
+{
+  TIMER("vec_apply_cut");
+  if(rmax < 0 ){return ;}
+  const long V_local = geo.local_volume();
+  fft_desc_basic& fd = get_fft_desc_basic_plan(geo);
+
+  qlat::vector_acc<int > nv, mv, Nv;
+  geo_to_nv(geo, nv, Nv, mv);
+
+  const int Nxyz = fd.Nx * fd.Ny * fd.Nz;
+  const int Nt   = fd.Nt;
+  const double rmax2 = rmax * rmax;
+  const int civ = res.size() / (Nt*Nxyz);
+
+  Ty* srcP = (Ty*) qlat::get_data(res).data();
+  qacc_for(xi, Nxyz, {
+    Coordinate xl = geo.coordinate_from_index(xi);
+    Coordinate xg = geo.coordinate_g_from_l(xl);
+
+    double dis = 0.0;
+    for(int i=0;i<3;i++){
+      double tmp = (xg[i] - sp[i] + nv[i])%(nv[i]/2);
+      dis += tmp * tmp;
+    }
+
+    if(dis > rmax2)
+    for(int ci=0;ci<civ*Nt;ci++)
+    {
+      srcP[ci*Nxyz + xi] = 0.0;
+    }
+  });
+
+}
 
 }
 
 
 #endif
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_io_vec.h` & `qlat-0.9/include/qlat/vector_utils/utils_io_vec.h`

 * *Files 3% similar despite different names*

```diff
@@ -202,20 +202,21 @@
     ////print0("==io number %d \n", ionum);
   }
 
   for(int ni=0;ni<Nmpi;ni++){node_ioL[ni]=-1;}
   /////distribute ranks out nodes
   {
     /////sorted id according to nodes
-    std::vector<int> id_to_node = mk_id_node_list_for_shuffle_node();
-    int off = Nmpi/ionum;
+    std::vector<int> id_to_node = qlat::get_id_node_in_shuffle_list();
+    //int off = Nmpi/ionum;
     int countN = 0;
     for(int ni=0;ni<Nmpi;ni++){
-      if(ni%off==0 and countN < ionum){
-        //node_ioL[ni]=countN;
+      //if(ni%off==0 and countN < ionum)
+      if(countN < ionum){
+        ///node_ioL[ni]=countN;
         node_ioL[id_to_node[ni]]=countN;
         countN++;
       }
     }
   }
 
   ////fd = fft_desc_basic(geo); ///new ways
@@ -424,15 +425,17 @@
   timeval tm0,tm1,tm2,tm3;
   gettimeofday(&tm0, NULL);
   double mpi_t = 0.0;
 
   const std::vector<int >& node_ioL = io.node_ioL;
   int rank = io.rank;size_t vol = io.vol;int ionum=io.ionum;size_t noden=io.noden;
 
-  if(io.do_checksum){if(io.end_of_file == 0){abort_r("io_vec need end of file for check sum! \n ");}}
+  if(io.do_checksum){
+    if(io.end_of_file == 0){abort_r("io_vec need end of file for check sum! \n ");}
+  }
 
   size_t size_buf = gN*vol*dsize;
   char* buf=NULL;
   ////char* buf=NULL;if(node_ioL[rank]>=0){buf = new char[gN*vol*dsize];}
   //if(buf.size() != size_buf){buf.resize(size_buf);}
   if(node_ioL[rank]>=0){
     if(io.buf.size() != size_buf){
@@ -809,33 +812,37 @@
   
   double normd=0.0;double normf=0.0;
   int n_vec = 1;
   size_t noden = io_use.noden;
   size_t Fsize = io_use.Nmpi*(noden*12*2)*sizeof(float);
   FILE* file;
   double err = 1e-3;
+  bool do_checksum_buf = io_use.do_checksum;
 
   {
+  io_use.do_checksum = false;
   std::vector<double > prop_E;
   prop_E.resize(n_vec*12*noden*2);
 
   file = io_use.io_read(filename,"rb");
   io_use.io_off(file,iv*Fsize*2, false);
   read_kentucky_vector(file,(char*) &prop_E[0], n_vec*12*2,io_use, false, sizeof(double), false, 12*2);
   io_use.io_close(file);
 
   rotate_gwu_vec_file(&prop_E[0],n_vec,noden, false);
   gwu_to_cps_rotation_vec(&prop_E[0],n_vec,noden, false, true, true);
 
   normd = get_norm_vec(&prop_E[0],noden);
   }
 
+  io_use.do_checksum = do_checksum_buf;
   if(fabs(normd - 1.0) < err)return 0;
 
   {
+  io_use.do_checksum = false;
   std::vector<float > prop_E;
   prop_E.resize(n_vec*12*noden*2);
   file = io_use.io_read(filename,"rb");
   io_use.io_off(file,iv*Fsize, false);
 
   read_kentucky_vector(file,(char*) &prop_E[0], n_vec,io_use, true, 6*2*sizeof(double), true);
   io_use.io_close(file);
@@ -843,14 +850,15 @@
   rotate_gwu_vec_file(&prop_E[0],n_vec,noden, true);
   gwu_to_cps_rotation_vec(&prop_E[0],n_vec,noden, false, false, false);
 
   normf = get_norm_vec(&prop_E[0],noden);
   }
 
 
+  io_use.do_checksum = do_checksum_buf;
   if(fabs(normf - 1.0) < err)return 1;
 
   print0("Norm of vector double %.3e, %.3e.\n",normd,normd-1.0);
   print0("Norm of vector single %.3e, %.3e.\n",normf,normf-1.0);
   return -1;
 }
 /////================END of NO checksum read/write
@@ -1076,47 +1084,47 @@
   if(read==true){read_single = check_Eigen_file_type(filename, io_use, n1, check);}
   FILE* file = open_gwu_eigen(filename, io_use, read);
   load_gwu_eigen(file, res, io_use,n0,n1,check,read, read_single);
   io_use.io_close(file);
 }
 
 
-template<typename Ty>
-void load_gwu_eigen(const char *filename,std::vector<qlat::FermionField4dT<Ty> > &eigen,io_vec &io_use,int n0,int n1,bool check=true,bool read=true){
+template<typename Td>
+void load_gwu_eigen(const char *filename,std::vector<qlat::FermionField4dT<Td> > &eigen,io_vec &io_use,int n0,int n1,bool check=true,bool read=true){
   if(n1<n0 or n0<0){abort_r("Read number of eigen should be larger than 1. \n");}
-  if(sizeof(Ty) != 2*sizeof(double ) and sizeof(Ty) != 2*sizeof(float )){abort_r("Cannot understand the input format! \n");}
+  if(sizeof(Td) != sizeof(double ) and sizeof(Td) != sizeof(float )){abort_r("Cannot understand the input format! \n");}
 
   int n_vec = n1-n0;
   if(read==true){
     eigen.resize(0);
     eigen.resize(n_vec);
     for(int iv=0;iv<n_vec;iv++)eigen[iv].init(io_use.geop);
   }
 
-  if(sizeof(Ty) == 2*sizeof(double )){
+  if(sizeof(Td) == sizeof(double )){
     std::vector<double* > resp;resp.resize(n_vec);
     for(int iv=0;iv<n_vec;iv++){
       resp[iv]=(double*)(qlat::get_data(eigen[iv]).data());
     }
     load_gwu_eigen(filename,resp,io_use,n0,n1,check,read);
   }
 
-  if(sizeof(Ty) == 2*sizeof(float )){
+  if(sizeof(Td) == sizeof(float )){
     std::vector<float* > resp;resp.resize(n_vec);
     for(int iv=0;iv<n_vec;iv++){
       resp[iv]=(float*)(qlat::get_data(eigen[iv]).data());
     }
     load_gwu_eigen(filename,resp,io_use,n0,n1,check,read);
   }
 
   ////return eigen;
 }
 
-template<typename Ty>
-void save_gwu_eigen(const char *filename,std::vector<qlat::FermionField4dT<Ty> > &eigen,io_vec &io_use,int n0,int n1,bool check=true){
+template<typename Td>
+void save_gwu_eigen(const char *filename,std::vector<qlat::FermionField4dT<Td> > &eigen,io_vec &io_use,int n0,int n1,bool check=true){
   load_gwu_eigen(filename,eigen,io_use,n0,n1,check,false);
 }
 
 inline void load_gwu_eigen(const char *filename,EigenM &Mvec,io_vec &io_use,int n0,int n1,bool check=true,bool read=true)
 {
   if(n1<n0 or n0<0){abort_r("Read number of eigen should be larger than 1. \n");}
   int n_vec = n1-n0;
@@ -1137,18 +1145,18 @@
 
 inline void save_gwu_eigen(const char *filename,EigenM &Mvec,io_vec &io_use,int n0,int n1,bool check=true)
 {
   load_gwu_eigen(filename, Mvec,io_use,n0,n1,check,false);
 }
 
 
-template<typename Ty>
-void load_gwu_prop(const char *filename,std::vector<qlat::FermionField4dT<Ty> > &prop,io_vec &io_use,bool read=true){
+template<typename Td>
+void load_gwu_prop(const char *filename,std::vector<qlat::FermionField4dT<Td> > &prop,io_vec &io_use,bool read=true){
 
-  if(sizeof(Ty) != 2*sizeof(double ) and sizeof(Ty) != 2*sizeof(float )){abort_r("Cannot understand the input format! \n");}
+  if(sizeof(Td) != sizeof(double ) and sizeof(Td) != sizeof(float )){abort_r("Cannot understand the input format! \n");}
 
   size_t noden = io_use.noden;
   size_t Fsize = io_use.Nmpi*(noden*12*2)*sizeof(float);
 
   FILE* file;bool single = true;
   if(read==true){
   size_t sizen = get_file_size_MPI(filename);
@@ -1167,15 +1175,15 @@
   {
     ////Single vector read
     std::vector<float > prop_qlat;
     prop_qlat.resize(12*noden*12*2);
 
     if(read==false){
     for(int iv=0;iv<12;iv++){
-      Ty* res   = (Ty*) qlat::get_data(prop[iv]).data();
+      qlat::ComplexT<Td>* res   = (qlat::ComplexT<Td>*) qlat::get_data(prop[iv]).data();
       std::complex<float> *src = (std::complex<float>*) &prop_qlat[iv*noden*12*2];
       #pragma omp parallel for
       for(size_t isp=0;isp<noden*12;isp++)src[isp] = std::complex<float>(res[isp].real(),res[isp].imag());
     }
 
     ////Do not rotate source, in ps/ky base
     gwu_to_cps_rotation_vec(&prop_qlat[0], 12,noden, true, true, true, read);
@@ -1191,18 +1199,18 @@
     if(read==true){
     /////double precision eigen vector in ps base
     rotate_gwu_vec_file(&prop_qlat[0], 12,noden, true);
     ////Do not rotate source, in ps/ky base
     gwu_to_cps_rotation_vec(&prop_qlat[0], 12,noden, true, true, true);
 
     for(int iv=0;iv<12;iv++){
-      Ty* res   = (Ty*) qlat::get_data(prop[iv]).data();
+      qlat::ComplexT<Td>* res   = (qlat::ComplexT<Td>*) qlat::get_data(prop[iv]).data();
       std::complex<float> *src = (std::complex<float>*) &prop_qlat[iv*noden*12*2];
       #pragma omp parallel for
-      for(size_t isp=0;isp<noden*12;isp++)res[isp]= Ty(src[isp].real(),src[isp].imag());
+      for(size_t isp=0;isp<noden*12;isp++)res[isp]= qlat::ComplexT<Td>(src[isp].real(),src[isp].imag());
     }
     }
   }
 
   if(single == false)
   {
     std::vector<double > prop_qlat;
@@ -1214,167 +1222,163 @@
       
     ///double precision eigen vector in ps base
     rotate_gwu_vec_file(&prop_qlat[0], 12,noden, false);
     //Do not rotate source, 
     gwu_to_cps_rotation_vec(&prop_qlat[0], 12,noden, true, true,true);
 
     for(int iv=0;iv<12;iv++){
-      Ty* res = (Ty*) qlat::get_data(prop[iv]).data();
+      qlat::ComplexT<Td>* res = (qlat::ComplexT<Td>*) qlat::get_data(prop[iv]).data();
       std::complex<double> *src = (std::complex<double>*) &prop_qlat[iv*noden*12*2];
-      for(size_t isp=0;isp<noden*12;isp++)res[isp]= Ty(src[isp].real(),src[isp].imag());
+      for(size_t isp=0;isp<noden*12;isp++)res[isp]= qlat::ComplexT<Td>(src[isp].real(),src[isp].imag());
     }
 
   }
 }
 
-template<typename Ty>
-void save_gwu_prop(const char *filename,std::vector<qlat::FermionField4dT<Ty> > &prop,io_vec &io_use){
+template<typename Td>
+void save_gwu_prop(const char *filename,std::vector<qlat::FermionField4dT<Td> > &prop,io_vec &io_use){
   load_gwu_prop(filename,prop,io_use,false);
 }
 
 //////final result 12*12 --> Nt*Nxyz
-template<typename Ty>
-void load_gwu_prop(const char *filename, qpropT& res,io_vec &io_use,bool read=true){
+template<typename Td>
+void load_gwu_prop(const char *filename, qlat::FieldM<qlat::ComplexT<Td>, 12*12>& res,io_vec &io_use,bool read=true){
   if(read == true ){res.init(io_use.geop);}
   if(read == false){abort_r("Not supported! \n");}
 
   long sizeF = io_use.geop.local_volume();
 
-  std::vector<qlat::FermionField4dT<Ty> > prop;
+  std::vector<qlat::FermionField4dT<Td> > prop;
   load_gwu_prop(filename, prop, io_use, read);
 
   move_index mv_civ;
-  Ty* p0; Ty* p1;Ty* pt;
-  pt = (Ty*) qlat::get_data(res).data();
+  qlat::ComplexT<Td>* p0; qlat::ComplexT<Td>* p1;qlat::ComplexT<Td>* pt;
+  pt = (qlat::ComplexT<Td>*) qlat::get_data(res).data();
 
   for(int iv=0;iv<12;iv++){
-    p0 = (Ty*) qlat::get_data(prop[iv]).data();
-    p1 = (Ty*) &pt[iv*12*sizeF + 0];
+    p0 = (qlat::ComplexT<Td>*) qlat::get_data(prop[iv]).data();
+    p1 = (qlat::ComplexT<Td>*) &pt[iv*12*sizeF + 0];
     mv_civ.dojob(p0, p1, 1, 12, sizeF, 1, 1, false);
   }
 }
 
 /////V -- 12a x 12b   to   12b x 12a -- V
-template<class T, typename Ty>
-void prop4d_to_qprop(qpropT& res, Propagator4dT<T>& src, int dir = 1){
+template<class Ty, typename Td>
+void prop4d_to_qprop(qpropT& res, Propagator4dT<Td>& src, int dir = 1){
   TIMERA("prop4d_to_qprop");
   if(dir == 1){qassert(src.initialized);res.init(src.geo());}
   if(dir == 0){qassert(res.initialized);src.init(res.geo());}
 
   long sizeF = src.geo().local_volume();
 
   move_index mv_civ;
-  T* ps; Ty* pt;
-  ps = (T* ) qlat::get_data(src).data();
+  qlat::ComplexT<Td>* ps; Ty* pt;
+  ps = (qlat::ComplexT<Td>* ) qlat::get_data(src).data();
   pt = (Ty*) qlat::get_data(res).data();
 
   ////V x 12 a x 12 b to 12b x 12a x V
   if(dir == 1){
     qthread_for(isp, long(sizeF),{
-      T buf[12*12];for(unsigned int i=0;i<12*12;i++){buf[i] = ps[isp*12*12 + i];}
+      ALIGN qlat::ComplexT<Td> buf[12*12];for(unsigned int i=0;i<12*12;i++){buf[i] = ps[isp*12*12 + i];}
       for(unsigned int d0=0;d0<12;d0++)
       for(unsigned int d1=0;d1<12;d1++)
       {
         pt[(isp*12+d0)*12+d1] = buf[d1*12+d0];
       }
     });
     mv_civ.move_civ_out(pt, pt, 1, sizeF, 12*12, 1, false);
   }
   ////12 a x 12 b x V to V x 12b x 12a
   if(dir == 0){
     mv_civ.move_civ_in(pt, pt, 1, 12*12, sizeF, 1, false);
     qthread_for(isp, long(sizeF),{
-      T buf[12*12];for(unsigned int i=0;i<12*12;i++){buf[i] = pt[isp*12*12 + i];}
+      ALIGN qlat::ComplexT<Td> buf[12*12];for(unsigned int i=0;i<12*12;i++){buf[i] = pt[isp*12*12 + i];}
       for(unsigned int d0=0;d0<12;d0++)
       for(unsigned int d1=0;d1<12;d1++)
       {
         ps[(isp*12+d0)*12+d1] = buf[d1*12+d0];
       }
     });
   }
 }
 
-template<class T, typename Ty>
-void qprop_to_prop4d(Propagator4dT<T>& res, qpropT& src){
+template<typename Td, typename Ty>
+void qprop_to_prop4d(Propagator4dT<Td>& res, qpropT& src){
   prop4d_to_qprop(src, res, 0);
 }
 
-template<class T, typename Ty>
-void prop4d_to_Fermion(Propagator4dT<T>& prop,std::vector<qlat::FermionField4dT<Ty > > &buf, int dir=1){
+template<typename Td, typename Tc>
+void prop4d_to_Fermion(Propagator4dT<Td>& prop,std::vector<qlat::FermionField4dT<Tc > > &buf, int dir=1){
 
-  ////if(sizeof(Ty) != 2*sizeof(double ) and sizeof(Ty) != 2*sizeof(float )){abort_r("Cannot understand the input format! \n");}
   if(dir==1){buf.resize(0);buf.resize(12);for(int iv=0;iv<12;iv++){
     if(!buf[iv].initialized){buf[iv].init(prop.geo());}
   }}
   if(dir==0){qassert(buf.size() == 12);if(!prop.initialized){prop.init(buf[0].geo());}}
 
   #pragma omp parallel for
   for (long index = 0; index < prop.geo().local_volume(); ++index)
   {
-    qlat::WilsonMatrixT<T>& src =  prop.get_elem_offset(index);
+    qlat::WilsonMatrixT<Td>& src =  prop.get_elem_offset(index);
     for(int d0=0;d0<12;d0++)
     {
       ////v0(s*3 + c0, ga.ind[d0]*3 + c1)
-      Ty* res = (Ty*)&(buf[d0].get_elem_offset(index));
+      qlat::ComplexT<Tc>* res = (qlat::ComplexT<Tc>*)&(buf[d0].get_elem_offset(index));
       for(int d1=0;d1<12;d1++)
       {
         if(dir==1){res[d1] = src(d1, d0);}
         if(dir==0){src(d1, d0) = res[d1];}
       }
 
     }
   }
 
 }
 
-template<class T, typename Ty>
-void Fermion_to_prop4d(Propagator4dT<T>& prop, std::vector<qlat::FermionField4dT<Ty > > &buf){
+template<typename Td, typename Tc>
+void Fermion_to_prop4d(Propagator4dT<Td>& prop, std::vector<qlat::FermionField4dT<Tc > > &buf){
   qassert(buf.size() == 12);
   prop4d_to_Fermion(prop, buf, 0);
 }
 
-
-template <class T>
-void save_gwu_prop(const char *filename,Propagator4dT<T>& prop){
+template <typename Td>
+void save_gwu_prop(const char *filename,Propagator4dT<Td>& prop){
   qassert(prop.initialized);
   io_vec& io_use = get_io_vec_plan(prop.geo());
-  std::vector<qlat::FermionField4dT<qlat::ComplexF> > prop_qlat;
+  std::vector<qlat::FermionField4dT<Td > > prop_qlat;
   prop4d_to_Fermion(prop,prop_qlat, 1);
   save_gwu_prop(filename,prop_qlat,io_use);
   ///////load_gwu_prop(filename,prop,io_use,false);
 }
 
-template <class T>
-void save_gwu_prop(std::string &filename,Propagator4dT<T>& prop){
+template <typename Td>
+void save_gwu_prop(std::string &filename,Propagator4dT<Td>& prop){
   char tem[500];
   sprintf(tem,filename.c_str());
   save_gwu_prop(tem,prop);
 }
 
-template <class T>
-void load_gwu_prop(const char *filename,Propagator4dT<T>& prop){
+template <typename Td>
+void load_gwu_prop(const char *filename,Propagator4dT<Td>& prop){
   qassert(prop.initialized);
   io_vec& io_use = get_io_vec_plan(prop.geo());
-  std::vector<qlat::FermionField4dT<qlat::Complex > > prop_qlat;
+  std::vector<qlat::FermionField4dT<Td > > prop_qlat;
   load_gwu_prop(filename,prop_qlat,io_use);
   prop4d_to_Fermion(prop,prop_qlat, 0);
   ///////load_gwu_prop(filename,prop,io_use,false);
 }
 
-template <class T>
-void load_gwu_prop(std::string &filename,Propagator4dT<T>& prop){
+template <typename Td>
+void load_gwu_prop(std::string &filename,Propagator4dT<Td>& prop){
   char tem[500];
   sprintf(tem,filename.c_str());
   load_gwu_prop(tem,prop);
 }
 
-
-
-template <class T>
-void load_gwu_link(const char *filename,GaugeFieldT<T> &gf, bool read = true){
+template <typename Td>
+void load_gwu_link(const char *filename,GaugeFieldT<Td> &gf, bool read = true){
   io_vec io_use(gf.geo(),8);
   //if(sizeof(Ty) != 2*sizeof(double ) and sizeof(Ty) != 2*sizeof(float ))
   //{abort_r("Cannot understand the input format! \n");}
 
   size_t noden = io_use.noden;
   size_t Fsize = io_use.Nmpi*(4*9*noden*2)*sizeof(double);
 
@@ -1388,15 +1392,15 @@
     /////gf.init(*io_use.geop);
   }
 
 
   if(read == false)
   for (size_t index = 0; index < noden; ++index)
   {
-    ColorMatrixT<T>& res = gf.get_elem_offset(index*gf.geo().multiplicity+0);
+    ColorMatrixT<Td>& res = gf.get_elem_offset(index*gf.geo().multiplicity+0);
 
     for(int dir=0;dir<4;dir++)
     {
       for(int c0=0;c0<3;c0++)
       for(int c1=0;c1<3;c1++)
       {
         int dir0  = ((dir*3+c0)*3+c1)    ;
@@ -1419,37 +1423,37 @@
   /////Do not rotate source, 
   ///gwu_to_cps_rotation_vec(&link_qlat[0], 12,noden, true, true,true);
   ///4 dire --> c0 -- > c1
 
   if(read == true)
   for (size_t index = 0; index < noden; ++index)
   {
-    ColorMatrixT<T>& res = gf.get_elem_offset(index*gf.geo().multiplicity+0);
+    ColorMatrixT<Td>& res = gf.get_elem_offset(index*gf.geo().multiplicity+0);
 
     for(int dir=0;dir<4;dir++)
     {
       for(int c0=0;c0<3;c0++)
       for(int c1=0;c1<3;c1++)
       {
         int dir0  = ((dir*3+c0)*3+c1)    ;
         int dir1R = ((dir*3+c1)*3+c0)*2+0;
         int dir1I = ((dir*3+c1)*3+c0)*2+1;
-        res.p[dir0] = T(link_qlat[dir1R*noden + index], link_qlat[dir1I*noden + index]);
+        res.p[dir0] = qlat::ComplexT<Td>(link_qlat[dir1R*noden + index], link_qlat[dir1I*noden + index]);
       }
     }
   }
 }
 
-template <class T>
-void save_gwu_link(const char *filename,GaugeFieldT<T> &gf){
+template <class Td>
+void save_gwu_link(const char *filename,GaugeFieldT<Td> &gf){
   load_gwu_link(filename, gf, false);
 }
 
-template <class T>
-void load_gwu_link(std::string &filename,GaugeFieldT<T> &gf){
+template <class Td>
+void load_gwu_link(std::string &filename,GaugeFieldT<Td> &gf){
   char tem[500];
   sprintf(tem,filename.c_str());
   load_gwu_link(tem,gf);
 }
 
 
 template<typename Ty>
@@ -1505,24 +1509,24 @@
 }
 
 template<typename Ty>
 void save_gwu_noi(const char *filename,qlat::FieldM<Ty,1> &noi){
   load_gwu_noi(filename,noi,false);
 }
 
-template <class T>
-void save_gwu_noiP(const char *filename,Propagator4dT<T>& prop){
+template <typename Td>
+void save_gwu_noiP(const char *filename,Propagator4dT<Td>& prop){
   qlat::FieldM<qlat::Complex,1> noi;
   noi.init(prop.geo());
   qlat::set_zero(noi);
   
   size_t noden = prop.geo().local_volume();
   for (size_t index = 0; index < noden; ++index)
   {
-    qlat::WilsonMatrixT<T>&  src =  prop.get_elem_offset(index);
+    qlat::WilsonMatrixT<Td>&  src =  prop.get_elem_offset(index);
     double sum = 0.0;
     for(int d1=0;d1<12;d1++)
     for(int d0=0;d0<12;d0++)
     {
       sum += std::fabs(src(d1,d0).real());
       sum += std::fabs(src(d1,d0).imag());
     }
@@ -1531,46 +1535,46 @@
     if(sum >1e-8){noi.get_elem_offset(index) = 1.0*phase;}
   }
 
   save_gwu_noi(filename,noi);
   ///////load_gwu_prop(filename,prop,io_use,false);
 }
 
-template <class T>
-void save_gwu_noiP(std::string &filename,Propagator4dT<T>& prop){
+template <typename Td>
+void save_gwu_noiP(std::string &filename,Propagator4dT<Td>& prop){
   char tem[500];
   sprintf(tem,filename.c_str());
   save_gwu_noiP(tem,prop);
 }
 
-template <class T>
-void noi_to_propP(qlat::FieldM<qlat::Complex,1> &noi,Propagator4dT<T>& prop, int dir = 0){
+template <typename Td>
+void noi_to_propP(qlat::FieldM<qlat::Complex,1> &noi,Propagator4dT<Td>& prop, int dir = 0){
   for (long index = 0; index < prop.geo().local_volume(); ++index)
   {
-    qlat::WilsonMatrixT<T>& res =  prop.get_elem_offset(index);
+    qlat::WilsonMatrixT<Td>& res =  prop.get_elem_offset(index);
     if(dir==0)for(int d0=0;d0<12;d0++){res(d0,d0) = noi.get_elem_offset(index);}
     if(dir==1)for(int d0=0;d0<12;d0++){noi.get_elem_offset(index) = res(d0,d0);}
   }
 }
 
-template <class T>
-void load_gwu_noiP(const char *filename,Propagator4dT<T>& prop){
+template <typename Td>
+void load_gwu_noiP(const char *filename,Propagator4dT<Td>& prop){
   ////io_vec& io_use = get_io_vec_plan(prop.geo());
   qlat::FieldM<qlat::Complex,1> noi;
   noi.init(prop.geo());
   qlat::set_zero(noi);
   load_gwu_noi(filename,noi);
   prop.init(noi.geo());
 
   noi_to_propP(noi, prop, 0);
   
 }
 
-template <class T>
-void load_gwu_noiP(std::string &filename,Propagator4dT<T>& prop){
+template <typename Td>
+void load_gwu_noiP(std::string &filename,Propagator4dT<Td>& prop){
   char tem[500];
   sprintf(tem,filename.c_str());
   load_gwu_noiP(tem,prop);
 }
 
 /////================END of NO checksum read/write
 
@@ -1807,174 +1811,21 @@
   /////print0(" ionum off %zu, n0 %zu, n1 %zu, Vsize %zu, bsize %zu \n", off_file, size_t(n0), size_t(n1), Vsize, size_t(bsize));
 
   io_use.io_off(file, in.off_file, true);  ////shift file for the head
   load_qlat_noisesT(file, noises, io_use, in, n0, n1);
 
   close_file_qlat_noisesT(file, io_use, in);
 
-  //int bsize = sizeof(float );
-
-  //bool do_checksum = true;
-  //int N_noi = 1;
-  //if(bfac==1)rotate_bfac = false;
-  //int bfac_write = bfac;
-  //if(rotate_bfac)bfac_write = 1;
-  //bool Rendian = IO_ENDIAN;
-  //////int Nmpi = qlat::get_num_node();
-
-  //size_t off_file = 0;
-  //Geometry geo;
-  //if(read == true){
-  //  in.load_para(filename, false);
-
-  //  if(in.VECS_TYPE != VECS_TYPE){print0("Noise type wrong, file %s \n", filename);abort_r("");}
-  //  Coordinate total_site = Coordinate(in.nx, in.ny, in.nz, in.nt);
-  //  geo.init(total_site, 1);
-  //  qassert(in.nvec > 0);////qassert(in.bfac == bfac_write);
-
-  //  if(in.bfac != 1){qassert(in.bfac == bfac);}
-  //  bfac_write = in.bfac;
-
-  //  if(noises.size() != 0){noises.resize(0);}
-  //  int Ntotal = in.nvec/(bfac/bfac_write);
-  //  if(nread == -1)noises.resize(Ntotal);
-  //  else{
-  //    if(nread + nini > Ntotal){print0("Load noise number large, file %s \n", filename);abort_r("");}
-  //    noises.resize(nread);
-  //  }
-  //  for(LInt ni=0;ni<noises.size();ni++)noises[ni].init(geo);
-  //  N_noi = noises.size();
-  //  if(in.FILE_ENDIAN == std::string("BIGENDIAN")){   Rendian = false;}
-  //  if(in.FILE_ENDIAN == std::string("LITTLEENDIAN")){Rendian = true ;}
-  //}
-  //if(read == false){
-  //  in.VECS_TYPE = VECS_TYPE;
-  //  in.INFO_LIST  = INFO_LIST;
-  //  if(!IO_ENDIAN){in.FILE_ENDIAN = std::string("BIGENDIAN");}
-  //  if( IO_ENDIAN){in.FILE_ENDIAN = std::string("LITTLEENDIAN");}
-  //  N_noi = noises.size();
-  //  in.nvec = N_noi*(bfac/bfac_write);
-  //  if(N_noi < 1){print0("write noises size zero \n");return;}
-  //  geo = noises[0].geo();
-
-  //}
-  //if(bfac_write == bfac)rotate_bfac = false;
-
-  //io_vec io_use(geo, IO_DEFAULT, true, IO_THREAD, do_checksum);
-  //int io_gn = IO_GN;
-  //if(in.nvec/io_gn < 1){io_gn = 1;}
-
-  //if(read == true){
-  //  if(in.OBJECT != std::string("BEGIN_Vecs_HEAD")){abort_r("File head wrong");}
-  //  int type = get_save_type(in.save_type);
-  //  if(type == 0){bsize=sizeof(double);single_file=false;}
-  //  if(type == 1){bsize=sizeof(float) ;single_file=true; }
-
-  //  //////Check file sizes
-  //  size_t sizen = get_file_size_MPI(filename) - in.off_file;  //qassert(sizen == string_to_size(in.total_size));
-  //  if(sizen != string_to_size(in.total_size)){abort_r("FILE size not match with head !\n");}
-
-  //  size_t Vsize = io_use.Nmpi*size_t(io_use.noden*bfac*2);
-  //  size_t Fsize = (N_noi + nini)*Vsize*bsize;  //qassert(Fsize <= string_to_size(in.total_size));
-  //  if(Fsize > string_to_size(in.total_size)){abort_r("FILE size too small for vectors read !\n");}
-  //  if(Fsize != string_to_size(in.total_size)){io_use.do_checksum = false;}
-
-  //  //////Check file sizes
-
-  //  off_file = in.off_file + nini*Vsize*bsize;
-  //  io_use.end_of_file = sizen + in.off_file;
-  //}
-
-  //if(read == false){
-  //  in.nx = io_use.nx;in.ny = io_use.ny;in.nz = io_use.nz;in.nt = io_use.nt;
-  //  in.bfac = bfac_write;in.checksum = 0;
-  //  if(single_file==false){bsize=sizeof(double);in.save_type = std::string("Double");}
-  //  if(single_file==true ){bsize=sizeof(float) ;in.save_type = std::string("Single");}
-
-  //  size_t Fsize = N_noi* io_use.Nmpi*size_t(io_use.noden*bfac*2);
-  //  Fsize = Fsize*bsize;in.total_size = print_size(Fsize);
-  //  ////print0("size of file %zu \n", Fsize);
-  //  off_file = vecs_head_write(in, filename, true);
-  //  io_use.end_of_file = Fsize + off_file;
-  //}
-
-  //FILE* file=NULL;
-  //if(read==true )file = io_use.io_read(filename,"rb");
-  //if(read==false)file = io_use.io_read(filename,"wb");
-  //if(io_use.node_ioL[io_use.rank]>=0){fseek(file , off_file, SEEK_SET );} 
-
-  //int bufN = io_use.ionum;
-  ///////print0("ionum %d %d \n", io_use.ionum, N_noi);
-
-  //void* buf;
-  //buf = aligned_alloc_no_acc(bufN*bfac*io_use.noden * 2*bsize);
-  //qlat::Complex*  bufD = (qlat::Complex* ) buf;
-  //qlat::ComplexF* bufF = (qlat::ComplexF*) buf;
-
-
-  ////qlat::vector<qlat::Complex  > bufD;// buf.resize(bufN*bfac*io_use.noden );
-  ////qlat::vector<qlat::ComplexF > bufF;// buf.resize(bufN*bfac*io_use.noden );
-  ////if(!single_file)bufD.resize(bufN*bfac*io_use.noden);
-  ////if( single_file)bufF.resize(bufN*bfac*io_use.noden);
-
-  ////////false big endian, true small endian
-  //int bi = 0;
-  //for(int ni = 0; ni < N_noi; ni++)
-  //{
-  //  if(read==false){
-  //    if(!single_file)copy_noise_to_vec(noises[ni], &bufD[bi*bfac*io_use.noden], 1);
-  //    if( single_file)copy_noise_to_vec(noises[ni], &bufF[bi*bfac*io_use.noden], 1);}
-  //  bi = bi + 1;
-
-  //  if(bi == bufN or ni == (N_noi - 1)){
-  //  //if(read==false)if(rotate_bfac)reorder_civ((char*) buf,(char*) buf, bi, bfac, io_use.noden, 1, 2*bsize);
-  //  if(read==false)if(rotate_bfac)io_use.mv_civ.dojob((char*) buf,(char*) buf, bi, bfac, io_use.noden, 1, 2*bsize);
-
-  //  ////load_qlat_vecs(filename, &buf[0], io_use, bi*bfac/bfac_write, bfac_write, in, read, single_file);
-  //  read_kentucky_vector(file,(char*) buf, bi*bfac/bfac_write, io_use, Rendian, bfac_write*bsize*2, single_file, io_gn , read);
-
-  //  //if(read==true)if(rotate_bfac)reorder_civ((char*) buf,(char*) buf, bi, bfac, io_use.noden, 0, 2*bsize);
-  //  if(read==true)if(rotate_bfac)io_use.mv_civ.dojob((char*) buf,(char*) buf, bi, bfac, io_use.noden, 0, 2*bsize);
-  //  if(read==true)for(int nbi=0; nbi < bi; nbi++){int n0 = ni - bi + 1;
-  //  {
-  //    if(!single_file)copy_noise_to_vec(noises[n0 + nbi], &bufD[nbi*bfac*io_use.noden], 0);
-  //    if( single_file)copy_noise_to_vec(noises[n0 + nbi], &bufF[nbi*bfac*io_use.noden], 0);
-  //  }}
-
-  //  bi = 0;
-  //  }
-
-  //}
-
-  //io_use.io_close(file);
-
-  //if(read==false){in.checksum = io_use.full_crc;off_file = vecs_head_write(in, filename, false);}
-  //if(read==true and io_use.do_checksum==true){
-  //  if(in.checksum != io_use.full_crc){print0("File %s check sum wrong ! \n ", filename);abort_r("");}}
-
-  //bufD = NULL; bufF = NULL;
-  //free(buf);
-
-  //if(read==false){
-  //  for(int ni=0;ni<N_noi;ni++)copy_noise_to_vec(noises[ni], &buf[ni*bfac*io_use.noden], 1);
-  //}
-  ///////TODO, need split the jobs if N_noi is too large
-  //load_qlat_vecs(filename, &buf[0], io_use, N_noi, bfac_write, in, read, single_file, nini);
-  //if(read==true){
-  //  for(int ni=0;ni<N_noi;ni++)copy_noise_to_vec(noises[ni], &buf[ni*bfac*io_use.noden], 0);
-  //}
-
 }
 
 template <class T>
 void load_qlat_eigen(const char *filename, std::vector<qlat::FieldM<T, 12> > &noises, bool read , bool single_file=true, const std::string& INFO_LIST = std::string("NONE"),int n0 = 0, int n1=-1)
 {
   TIMERC("load/save qlat eigen");
   std::string VECS_TYPE = std::string("Eigen_system_nvec.12.tzyx.R/I");
-  ////int nread = -1;if(n1 > 0){qassert(n0 < n1); nread = n1 - n0;}
   load_qlat_noisesT(filename, noises, read, single_file, VECS_TYPE, INFO_LIST, n0, n1);
 }
 
 template <class T>
 void load_qlat_eigen(const char *filename, std::vector<qlat::FieldM<T, 12> > &noises, int n0=0,int n1=-1)
 {
   bool read = true; bool single_file = true; std::string INFO_LIST = std::string("NONE");
@@ -2062,27 +1913,27 @@
 
 template <class T, int bfac>
 void save_qlat_noise(const char *filename, qlat::FieldM<T, bfac> &noise, bool single_file=true, const std::string& INFO_LIST = std::string("NONE")){
   load_qlat_noise(filename, noise, false, single_file, INFO_LIST);
 }
 
 //////Assume memory allocated already
-template<class T, typename Ty>
-void copy_noise_to_prop(qlat::FieldM<T, 12*12>& noise, Propagator4dT<Ty>& prop, int dir=1)
+template<class T, typename Td>
+void copy_noise_to_prop(qlat::FieldM<T, 12*12>& noise, Propagator4dT<Td>& prop, int dir=1)
 {
   TIMERB("copy_noise_to_prop");
   if(dir == 1){prop.init(noise.geo());}
   if(dir == 0){noise.init(prop.geo());}
   T* noi = (T*) qlat::get_data(noise).data();
   #pragma omp parallel for 
   for (long index = 0; index < prop.geo().local_volume(); ++index)
   {
     ///qlat::WilsonMatrixT<T>& src =  prop.get_elem_offset(index);
     T* src   = (T*) &noi[index*12*12];
-    Ty* res  = &prop.get_elem_offset(index)(0,0);
+    qlat::ComplexT<Td>* res  = &prop.get_elem_offset(index)(0,0);
     
     for(int d0=0;d0<12;d0++)
     {
       for(int d1=0;d1<12;d1++)
       {
         //////copy to prop
         if(dir==0){src[d1*12+d0] = res[d0*12+d1];}
@@ -2092,36 +1943,36 @@
       }
 
     }
   }
 }
 
 //////Assume memory allocated already
-template<class T, typename Ty>
-void copy_noises_to_prop(std::vector<qlat::FieldM<T, 12*12> >& noises, Propagator4dT<Ty>& prop, int dir=1)
+template<class T, typename Td>
+void copy_noises_to_prop(std::vector<qlat::FieldM<T, 12*12> >& noises, Propagator4dT<Td>& prop, int dir=1)
 {
   TIMERB("copy_noises_to_prop");
   if(dir == 1){prop.init(noises[0].geo());}
   if(dir == 0){noises.resize(0);noises.resize(1);noises[0].init(prop.geo());}
   copy_noise_to_prop(noises[0], prop, dir);
 }
 
-template <class Ty>
-void load_qlat_prop(const char *filename, Propagator4dT<Ty>& prop, bool read=true, bool single_file=true){
+template <typename Td>
+void load_qlat_prop(const char *filename, Propagator4dT<Td>& prop, bool read=true, bool single_file=true){
   std::string VECS_TYPE = std::string("Propagator");
   std::string INFO_LIST  = std::string("src 12, sink 12, zyxt, R/I");
-  std::vector<qlat::FieldM<Ty, 12*12> > noises;
+  std::vector<qlat::FieldM<qlat::ComplexT<Td >, 12*12> > noises;
   if(read == false){copy_noises_to_prop(noises, prop, 0);}
   load_qlat_noisesT(filename, noises, read, single_file, VECS_TYPE, INFO_LIST);
   if(read == true){copy_noises_to_prop(noises, prop, 1);}
   
 }
 
-template <class Ty >
-void save_qlat_prop(const char *filename,Propagator4dT<Ty >& prop, bool single_file=true){
+template <typename Td >
+void save_qlat_prop(const char *filename,Propagator4dT<Td >& prop, bool single_file=true){
   load_qlat_prop(filename, prop, false, single_file);
 }
 
 /////nvec needed for checksum
 inline FILE* open_eigensystem_file(const char *filename, int nini, int nvec, bool read, io_vec& io_use, inputpara& in, int save_type = 3)
 {
   in.single_file = true;
@@ -2133,39 +1984,48 @@
     if(save_type != 0 and save_type != 1 and save_type != 2 and save_type != 3){abort_r("Save type unknown! \n ");}
     in.file_type = save_type;
   }
 
   if(in.file_type == 0 or in.file_type == 2){in.single_file = false;}
   if(in.file_type == 1 or in.file_type == 3){in.single_file = true ;}
 
+  if(in.file_type == 0 or in.file_type == 1){
+    io_use.do_checksum = false;
+  }
   if(in.file_type == 2 or in.file_type == 3){
     if(read == false){in.read_geo(io_use.geop);}
     int bfac_eigen = 12;
     std::string VECS_TYPE = std::string("Eigen_system_nvec.12.tzyx.R/I");
     std::string INFO_LIST = std::string("NONE");
     bool rotate_bfac = true;
     open_file_qlat_noisesT(filename, bfac_eigen, in, read, in.single_file, nvec, VECS_TYPE, INFO_LIST, rotate_bfac);
 
     if(io_use.end_of_file != 0){abort_r("Please close file first! \n");}
 
     io_use.end_of_file = in.end_of_file;
     io_use.do_checksum = in.do_checksum;
   }
 
+  if(in.nx != 0){qassert(io_use.nx == in.nx);}
+  if(in.ny != 0){qassert(io_use.ny == in.ny);}
+  if(in.nz != 0){qassert(io_use.nz == in.nz);}
+  if(in.nt != 0){qassert(io_use.nt == in.nt);}
+
   FILE* file=NULL;
   if(read==true )file = io_use.io_read(in.filename.c_str(),"rb");
   if(read==false)file = io_use.io_read(in.filename.c_str(),"wb");
 
   //////shift the file to nini position
   {
     size_t bsize = sizeof(double);int bfac = 12;
-    if(!in.single_file){bsize=sizeof(float) ;}
-    if( in.single_file){bsize=sizeof(double);}
-    size_t Vsize = size_t(in.nx)*in.ny*in.nz*in.nt*size_t(bfac*2);
+    if( in.single_file){bsize=sizeof(float) ;}
+    if(!in.single_file){bsize=sizeof(double);}
+    size_t Vsize = size_t(io_use.nx)*io_use.ny*io_use.nz*io_use.nt*size_t(bfac*2);
     size_t off_file = size_t(nini)*Vsize*bsize;
+    ////print0("off each %ld, nini %ld %ld %ld...\n", long(off_file), long(nini), long(Vsize), long(bsize));
     if(in.file_type == 2 or in.file_type == 3){off_file += in.off_file;}
     io_use.io_off(file, off_file, false);
   }
 
   return file;
 }
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_lms_funs.h` & `qlat-0.9/include/qlat/vector_utils/utils_lms_funs.h`

 * *Files 13% similar despite different names*

```diff
@@ -56,15 +56,15 @@
   qlat::vector_acc<Ty > EresH;qlat::vector_acc<Ty > EresL;qlat::vector_acc<Ty > EresA;
   qlat::vector_gpu<Ty > stmp, low_prop, high_prop;
   std::vector<qlat::FieldM<Ty , 12*12> > src_prop;
   std::vector<qlat::vector_gpu<Ty > > FFT_data;
   qlat::vector_gpu<Ty > resTa;
   qlat::vector_gpu<Ty > resZero;
   std::vector<qlat::FieldM<Ty, 1> > Vzero_data;
-  std::vector<qlat::vector_acc<Ty > > Eprop;
+  std::vector<qlat::vector_gpu<Ty > > Eprop;
 
   /////initial with src noise
 
   void free_buf(){
     EresH.resize(0);
     EresL.resize(0);
     EresA.resize(0);
@@ -75,15 +75,15 @@
     FFT_data.resize(0);
     resTa.resize(0);
     resZero.resize(0);
     Vzero_data.resize(0);
     Eprop.resize(0);
   }
 
-  void init(){
+  inline void init(){
     for(int i=0;i<4;i++){ini_pos[i] = 0;off_L[i] = 1;}
 
     SRC_PROP_WITH_LOW = 0;
     lms = 0;
     combineT = 0;
 
     ///0  pt to pt, 1 pt to sm, 2 sm to pt, 3 sm to sm
@@ -102,15 +102,15 @@
     name_zero        = std::string("NONE");
     save_zero_corr   = 1;
 
     INFO = std::string("NONE");
     INFOA.resize(0);
   }
 
-  void print(){
+  inline void print(){
     print0("===Source Info %s \n", INFO.c_str());
     print0("  prop with low %3d, lms %3d, combineT %3d \n", SRC_PROP_WITH_LOW, lms, combineT);
     print0("  init %5d %5d %5d %5d, grid %5d %5d %5d %5d \n", 
       ini_pos[0], ini_pos[1], ini_pos[2], ini_pos[3],
       off_L[0], off_L[1], off_L[2], off_L[3] );
 
     int save_vecs = 0; if(name_mom_vecs != std::string("NONE")){save_vecs = 1;}
@@ -145,33 +145,33 @@
     for(int iv=0;iv<nvec;iv++){res[iv*Mvol + i1] = src[iv*Nvol + i0];}
   });
 
   sum_all_size(res.data(), res.size(), 1);
 }
 
 template<typename Ty>
-void prop_to_vec(std::vector<qlat::vector_acc<Ty > >& Eprop, qlat::vector_gpu<Ty >& resTa, fft_desc_basic& fd)
+void prop_to_vec(std::vector<qlat::vector_gpu<Ty > >& Eprop, qlat::vector_gpu<Ty >& resTa, fft_desc_basic& fd)
 {
   TIMERB("Get corr vec");
-  check_prop_size(Eprop);
+  check_prop_size(Eprop, fd);
 
   ga_matrices_cps   ga_cps;
   ////ga_matrices_PS   ga_cps;
   std::vector<ga_M > gL;gL.resize(16);
   {int o=0;
   for(int i=0;i<6;i++){gL[o] = ga_cps.ga[0][i];o+=1;}
   for(int i=2;i<6;i++){gL[o] = ga_cps.ga[1][i];o+=1;}
   for(int i=3;i<6;i++){gL[o] = ga_cps.ga[2][i];o+=1;}
   for(int i=4;i<6;i++){gL[o] = ga_cps.ga[3][i];o+=1;}
   for(int i=5;i<6;i++){gL[o] = ga_cps.ga[4][i];o+=1;}}
 
   ///////===new contractions
   long NTt = fd.Nv[3];
   long Nxyz = fd.Nv[0]*fd.Nv[1]*fd.Nv[2];
-  int nmass = Eprop.size()/(12*12*NTt);
+  int nmass = Eprop.size();
 
   //qlat::vector_gpu<Ty > resT0, resT1;////, resTa;
   //resT0.resize(16 * nmass * NTt * Nxyz);
   //resT1.resize(16 * nmass * NTt * Nxyz);
   resTa.resize(32 * nmass * NTt * Nxyz);//qlat::set_zero(resTa);////resTa.set_zero();
 
   ////gamma matrix follow current prec
@@ -192,21 +192,17 @@
 
     G[1*16*16 + ioff*16 + ind2*4 + ind1] = -1.0;
     mL[1*16*3 + ioff*3 + 0] = 1;
     mL[1*16*3 + ioff*3 + 1] = 0;
     mL[1*16*3 + ioff*3 + 2] = 2;
   }
 
-  qlat::vector_acc<Ty* > propP = EigenM_to_pointers(Eprop);
+  qlat::vector_acc<Ty* > propP = EigenM_to_pointers(Eprop, Nxyz);
 
   ////cps to PS
-  //Geometry geo;fd.get_geo(geo);
-  //std::vector< Propagator4dT<Ty > > prop;prop.resize(nmass);
-  //for(unsigned int pi=0;pi<prop.size();pi++)prop[pi].init(geo);
-  //std::vector<qlat::vector_acc<Ty > > Eprop_tmp;
 
   Ty** p1 = propP.data();
 
   ////print0("Call!\n");
 
   Ty* ra = resTa.data();
   Ty* rb = &(resTa.data()[resTa.size()/2]);
@@ -218,15 +214,15 @@
   meson_vectorEV( p1, p1, ra, nmass, gL, gL, fd, 1);
 
   //cpy_data_thread( (resTa.data()              ), resT0.data(), resT0.size(), 1, true);
   //vec_corrE(resTa, Eres, fd, clear);
 }
 
 template<typename Ty>
-void prop_to_corr_mom0(std::vector<qlat::vector_acc<Ty > >& Eprop, qlat::vector_acc<Ty >& Eres, 
+void prop_to_corr_mom0(std::vector<qlat::vector_gpu<Ty > >& Eprop, qlat::vector_acc<Ty >& Eres, 
   fft_desc_basic& fd, qlat::vector_gpu<Ty >& resTa, int clear = 1)
 {
   prop_to_vec(Eprop, resTa, fd);  
   vec_corrE(resTa, Eres, fd, 0);
 }
 
 /////propH , pi --> 12*12 --> Nt*Nxyz
@@ -284,15 +280,15 @@
   std::vector<qlat::FieldM<Ty , 12*12> >& src_prop = srcI.src_prop;
   std::vector<qlat::vector_gpu<Ty > >& FFT_data = srcI.FFT_data;
 
   qlat::vector_gpu<Ty >& resTa = srcI.resTa;
   qlat::vector_gpu<Ty >& resZero = srcI.resZero;
 
   std::vector<qlat::FieldM<Ty, 1> >& Vzero_data = srcI.Vzero_data;
-  std::vector<qlat::vector_acc<Ty > >& Eprop = srcI.Eprop;
+  std::vector<qlat::vector_gpu<Ty > >& Eprop = srcI.Eprop;
 
   if(src_prop.size() != 1){src_prop.resize(1);}
   if(FFT_data.size() != 2){FFT_data.resize(2);}
   ///qlat::vector_gpu<Ty > stmp, low_prop, high_prop;
   ///std::vector<qlat::FieldM<Ty , 12*12> > src_prop;src_prop.resize(1);
   ///std::vector<qlat::vector_gpu<Ty > > FFT_data;FFT_data.resize(1 + 1);
 
@@ -342,43 +338,19 @@
     }
     if(flag_do_job == false){
       print0("Pass %s \n", srcI.name_zero_vecs.c_str());
       return ;
     }
   }
 
-  //if(saveFFT){
-  //  bool flag_do_job = false;
-  //  TIMER("saveFFT");
-  //  fft_fieldM(resTa.data(), 32*nmass, 1, geo, false);
-  //  mdat.pick_mom_from_vecs(FFT_data[0], resTa);
-  //  char namesm[500], nameQ[550], name_info[550], name_mom_tmp[100];
-  //  sprintf(name_sm, "%s", srcI.name_mom_vecs.c_str());
-  //  sprintf(nameQ, "%s.Gsrc", namesm );
-  //  sprintf(name_info, "%s.GInfo", namesm );
-
-  //  if(get_file_size_MPI(name_mom) == 0){flag_do_job = true;}
-  //  if(get_file_size_MPI(srcI.name_zero_vecs.c_str()) == 0){flag_do_job = true;}
-  //  for(int gi=0;  gi  < Nlms + 1; gi++){
-  //    sprintf(name_mom_tmp, "%09d", gi);
-  //    if(mdat.read(FFT_data, std::string(nameQ), std::string(namei)) == 0){flag_do_job = true;}
-  //  }
-  //  if(flag_do_job == false){return ;}
-  //}
-
   char key_T[1000], dimN[1000];
   sprintf(key_T, "%d", 1);sprintf(dimN , "src");
 
   std::string POS_LIST, POS_CUR;
   if(saveFFT){
-    //get_mom_single_node(mapA, mapB, geo, srcI.mom_cut);
-    //FFT_data.resize(Nfdata);FFT_data.set_zero();
-    //FFT_data_high.resize(Nfdata);FFT_data_high.set_zero();
-    //sprintf(key_T, "  %d   %d  %d  %d  %d %d %d %d", Nlms+1, 32, int(massL.size()), fd.nt, mc, mc, mc, 2);
-    //sprintf(dimN , "grids+1 operator masses nt pz py px complex");
     sprintf(key_T, "%d  %d  %d %d %d %d", int(massL.size()), fd.nt, mc, mc, mc, 2);
     sprintf(dimN , "masses nt pz py px complex");
   }
   std::string ktem(key_T);
   std::string dtem(dimN);
   corr_dat<Ta > mom_res(ktem, dtem);
   mom_res.INFOA = srcI.INFOA;
@@ -395,46 +367,29 @@
     copy_eigen_src_to_FieldM(stmp, src_prop, ei.b_size, fd, 1, GPU, rotate);
     prop_L_device(ei, stmp.data(), low_prop.data(), 12, massL, srcI.mode_eig_sm);
     high_prop -= low_prop;
   }
   /////reduce the high prop
 
   print0("Do high %s \n", POS_CUR.c_str());
-  copy_eigen_prop_to_EigenM(high_prop.data(), Eprop, ei.b_size, nmass, fd, 0, GPU);
+  copy_eigen_prop_to_EigenG(Eprop, high_prop.data(), ei.b_size, nmass, fd, GPU);
   prop_to_vec(Eprop, resTa, fd); 
   if(save_zero_corr){vec_corrE(resTa.data(), EresH, fd, nvecs, 0);}
 
   POS_CUR = std::string("");write_pos_to_string(POS_CUR, pos);POS_LIST += POS_CUR;
   if(savezero){
     resZero.resize(resTa.size());
     cpy_data_thread(resZero.data(), resTa.data(), resTa.size(), 1, true, -1.0*Nlms);
   }
   if(saveFFT){
     TIMER("saveFFT");
     fft_fieldM(resTa.data(), 32*nmass, 1, geo, false);
     mdat.pick_mom_from_vecs(FFT_data[0], resTa);
-    sprintf(name_mom_tmp, "%09d", 0);mdat.write( FFT_data[0], std::string(name_mom), name_mom_tmp, true );
-
-    //print0("norm0 %.8f \n", FFT_data[0].norm().real());
-
-    //sprintf(key_T, "%d  %d  %d %d %d %d",  int(massL.size()), fd.nt, mc, mc, mc, 2);
-    //sprintf(dimN , "masses nt pz py px complex");
-
-    //std::string ktem(key_T);
-    //std::string dtem(dimN);
-    //corr_dat<Ta > mom_tmp(ktem, dtem);
-    //mom_tmp.INFOA = srcI.INFOA;
-
-    //long Nfdata = long(32)*massL.size()*fd.nt*mc*mc*mc ;
-    //qlat::vector_gpu<Ty > FFT_data_high;FFT_data_high.resize(Nfdata);
-    //pick_mom_data(FFT_data_high, resTa, 32*nmass, mdat.mapA, mdat.mapB, geo);
-    //sprintf(name_mom, "%s.%05d.Gsrc", srcI.name_mom_vecs.c_str(),    0);
-    //mom_tmp.INFO_LIST = POS_CUR;mom_tmp.shift_zero();
-    //mom_tmp.write_corr(FFT_data_high.data(), FFT_data_high.size(), 3);
-    //mom_tmp.write_dat(name_mom);
+    sprintf(name_mom_tmp, "%09d", 0);
+    mdat.write( FFT_data[0], std::string(name_mom), name_mom_tmp, true );
   }
 
   print_mem_info();
 
   for(int gi=0;gi<Nlms;gi++){
     POS_CUR = std::string("");write_pos_to_string(POS_CUR, Ngrid[gi][0]);POS_LIST += POS_CUR;
     print0("Do, Nlms %5d, gi %5d, %s \n", Nlms, gi, POS_CUR.c_str());
@@ -456,55 +411,42 @@
 
     /////get low mode prop
     prop_L_device(ei, stmp.data(), low_prop.data(), 12, massL, srcI.mode_eig_sm);
 
     //////format suitable for contractions
     ////low mode corr contractions
     if(srcI.do_all_low == 1){
-      copy_eigen_prop_to_EigenM(low_prop.data(),  Eprop, ei.b_size, nmass, fd, 0, GPU);
+      copy_eigen_prop_to_EigenG(Eprop, low_prop.data(), ei.b_size, nmass, fd, GPU);
       prop_to_vec(Eprop, resTa, fd);  
       if(save_zero_corr){vec_corrE(resTa.data(), EresL, fd, nvecs, 0);}
       //Ty norm0 = low_prop.norm();
       //Ty norm1 = resTa.norm();
       //print0("Check value %.3f %.3f, %.3f %.3f, %.3f %.3f \n", EresL[0].real(), EresL[0].imag(), 
       //  norm0.real(), norm0.imag(), norm1.real(), norm1.imag());
     }
 
     low_prop += high_prop;
     //////format suitable for contractions
-    copy_eigen_prop_to_EigenM(low_prop.data(),  Eprop, ei.b_size, nmass, fd, 0, GPU);
+    copy_eigen_prop_to_EigenG(Eprop, low_prop.data(), ei.b_size, nmass, fd, GPU);
     prop_to_vec(Eprop, resTa, fd);
     if(save_zero_corr){vec_corrE(resTa.data(), EresA, fd, nvecs, 0);}
 
     if(savezero){resZero += resTa;}
     if(saveFFT){
       TIMER("saveFFT");
       fft_fieldM(resTa.data(), 32*nmass, 1, geo, false);
       mdat.pick_mom_from_vecs(FFT_data[1], resTa);
       FFT_data[1] -= FFT_data[0];
-      sprintf(name_mom_tmp, "%09d", gi + 1);mdat.write( FFT_data[1], std::string(name_mom), name_mom_tmp, false );
-      ////print0("norm0 %.8f \n", FFT_data[gi+1].norm().real());
-      //pick_mom_data(FFT_data, resTa, 32*nmass, mapA, mapB, geo);
-      //sprintf(name_mom, "%s.%05d.Gsrc", srcI.name_mom_vecs.c_str(), gi+1);
-      //mom_res.INFO_LIST = POS_CUR;mom_res.shift_zero();
-      //////subtract high mode
-      //mom_res.write_corr(FFT_data.data(), FFT_data.size(), 3);
-      //mom_res.write_dat(name_mom);
+      sprintf(name_mom_tmp, "%09d", gi + 1);
+      mdat.write( FFT_data[1], std::string(name_mom), name_mom_tmp, false );
     }
   }
 
   if(saveFFT){
     TIMER("saveFFT");
-    //sprintf(name_mom, "%s.Gsrc", srcI.name_mom_vecs.c_str());
-    //char name[500];bool clean = true;
-    //for(unsigned int i=0;i<FFT_data.size();i++){
-    //  sprintf(name, "%09d", i);if(i != 0){clean = false;}
-    //  mdat.write( FFT_data[i], std::string(name_mom), name, clean );
-    //}
-
     sprintf(name_mom, "%s.GInfo", srcI.name_mom_vecs.c_str());
     mom_res.INFO_LIST = POS_LIST;
     mom_res.write_dat(name_mom);
   }
 
   if(savezero){
     TIMER("lms savezero");
@@ -518,20 +460,14 @@
     for(unsigned int iv=0;iv<Vzero_data.size();iv++){
       Ty* resP = (Ty*) qlat::get_data(Vzero_data[iv]).data();
       cpy_data_thread(resP, &resZero[iv*geo.local_volume()], geo.local_volume(), 1, true);
     }
     save_qlat_noises(srcI.name_zero_vecs.c_str(), Vzero_data, true, POS_LIST);
   }
 
-  //if(saveFFT){
-  //  mom_res.INFO_LIST = POS_LIST;
-  //  mom_res.write_dat(srcI.name_mom_vecs.c_str());
-  //  mom_res.print_info();
-  //}
-
   if(save_zero_corr){
     if(shift_t == 1){
       shift_result_t(EresL, fd.nt, tini);
       shift_result_t(EresH, fd.nt, tini);
       shift_result_t(EresA, fd.nt, tini);
     }
     ////subtract high mode from EresA
@@ -541,36 +477,36 @@
     res.write_corr((Ty*) EresA.data(), EresA.size());
   }
 
   print_mem_info("END point_corr");
 }
 
 /////all to all prop naive do, test for all-to-all low eigen
-template<typename Ta>
-void test_all_prop_corr(std::vector<double >& massL, eigen_ov& ei, fft_desc_basic& fd, corr_dat<Ta >& res, int mode_sm = 0)
+template<typename Ty>
+void test_all_prop_corr(std::vector<double >& massL, eigen_ov& ei, fft_desc_basic& fd, corr_dat<Ty >& res, int mode_sm = 0)
 {
   /////if(propH.size() != src.size()*massL.size()){abort_r("prop size, mass size not match!\n");}
   Geometry geo;fd.get_geo(geo );
 
   int GPU = 1;
   int nmass = massL.size();
 
   std::vector<qnoi > src; src.resize(1);src[0].init(geo);
   EigenV Eres;Eres.resize(nmass*32*fd.nt);
   qlat::set_zero(Eres);
 
   ///std::vector<int > pos;pos.resize(src.size());qlat::vector_acc<int > off_L;
   ///check_noise_pos(src[0], pos[0], off_L);
   ///int tini = pos[0]%1000;
-  qlat::vector_gpu<Complexq > stmp, low_prop;
+  qlat::vector_gpu<Ty > stmp, low_prop;
   stmp.resize(fd.get_prop_size());
   low_prop.resize(nmass*fd.get_prop_size());
-  qlat::vector_gpu<Complexq > resTa;
+  qlat::vector_gpu<Ty > resTa;
   /////do corr
-  EigenM Eprop;
+  std::vector<qlat::vector_gpu<Ty > >  Eprop;
 
   int tini = 0;
   for(int zi=0;zi<fd.nz;zi++)
   for(int yi=0;yi<fd.ny;yi++)
   for(int xi=0;xi<fd.nx;xi++)
   {
     print0("===pos %d %d %d \n", zi, yi, xi);
@@ -585,26 +521,17 @@
         stmp[(di*12 + di)*fd.noden + indexL%fd.noden] = 1.0;
       }
     }
 
     /////get low mode prop
     prop_L_device(ei, stmp.data(), low_prop.data(), 12, massL, mode_sm);
 
-    copy_eigen_prop_to_EigenM(low_prop.data(),  Eprop, ei.b_size, nmass, fd, 0, GPU);
+    copy_eigen_prop_to_EigenG(Eprop, low_prop.data(),  ei.b_size, nmass, fd, GPU);
     prop_to_corr_mom0(Eprop, Eres, fd, resTa,  0); 
     shift_result_t(Eres, fd.nt, tini);
-
-    ////copy_eigen_prop_to_EigenM(high_prop.data(), Eprop, ei.b_size, nmass, fd, 0, GPU);
-    ////prop_to_corr(Eprop, Eres, fd, tini);  res.write_corr((Ftype*) &Eres[0], 2*Eres.size());
-
-    ////low_prop += high_prop;
-
-    ////copy_eigen_prop_to_EigenM(low_prop.data(),  Eprop, ei.b_size, nmass, fd, 0, GPU);
-    ////prop_to_corr(Eprop, Eres, fd, tini);  
-
   }
   for(int i=0;i<Eres.size();i++){Eres[i] = Eres[i]/(Ftype(fd.nx*fd.ny*fd.nz*1.0));}
   res.write_corr((Ftype*) &Eres[0], 2*Eres.size());
 }
 
 
 }
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_low_rho.h` & `qlat-0.9/include/qlat/vector_utils/utils_low_rho.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_momentum.h` & `qlat-0.9/include/qlat/vector_utils/utils_momentum.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_quda_inverter.h` & `qlat-0.9/include/qlat/vector_utils/utils_quda_inverter.h`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,15 @@
   quda::Dirac *dEig;
 
   std::vector<quda::Complex > evals_ZERO;
   std::vector<double        > evals_ERR ;
 
   std::vector<quda::ColorSpinorField *> kSpace;
   std::vector<quda::ColorSpinorField *> fSpace;
+  std::vector<quda::ColorSpinorField *> kSpace_cpu;
   std::vector<quda::Complex > evalsK;
   std::vector<quda::Complex > evalsF;
 
   std::vector<quda::ColorSpinorField *> ZSpace;
   std::vector<quda::Complex > evalsZ;
   ///std::vector<quda::ColorSpinorField *> evecs_;
   int spinor_site_size;
@@ -171,14 +172,15 @@
 
   quda::ColorSpinorField *csrc, *cres;
   //quda::ColorSpinorField *cpu_src, *cpu_res;
   quda::ColorSpinorField *gsrc, *gres;
   ///quda::ColorSpinorField *gsrcD, *gresD;
   quda::ColorSpinorField *gtmp1D, *gtmp2D;
   quda::ColorSpinorField *gtmp1F, *gtmp2F;
+  quda::ColorSpinorField *gadd; ////for low mode addition
 
   quda::ColorSpinorField *ctmp0, *ctmp1, *ctmp2;
   quda::ColorSpinorField *gtmp0, *gtmp1, *gtmp2;
   //quda::ColorSpinorField *gsrcF, *gresF; ////format to match gpu solver
   ///bool singleE;
 
   ////0 for wilson, clover, 1 for stagger
@@ -326,14 +328,15 @@
 
   clover_alloc = false;
   csrc = NULL; cres = NULL;
   gsrc = NULL; gres = NULL;
   //gsrcD= NULL; gresD= NULL;
   gtmp1D = NULL;gtmp2D = NULL;
   gtmp1F = NULL;gtmp2F = NULL;
+  gadd = NULL;
 
   ctmp0 = NULL; ctmp1 = NULL; ctmp2 = NULL;
   gtmp0 = NULL; gtmp1 = NULL; gtmp2 = NULL;
 
   eig_solveK = NULL;
   eig_solveF = NULL;
   mat = NULL;
@@ -414,22 +417,25 @@
 
   if(mode == 0 or mode == 2){
   //if(gsrcD != NULL){delete gsrcD;gsrcD=NULL;}if(gresD!= NULL){delete gresD;gresD=NULL;}
   if(gsrc  != NULL){delete gsrc ;gsrc =NULL;}if(gres != NULL){delete gres ;gres =NULL;}
   if(gtmp0 != NULL){delete gtmp0;gtmp0=NULL;}
 
   if(gtmp1 != NULL){delete gtmp1;gtmp1=NULL;}
-  if(gtmp2 != NULL){delete gtmp2;gtmp2=NULL;}}
+  if(gtmp2 != NULL){delete gtmp2;gtmp2=NULL;}
+  if(gadd  != NULL){delete gadd;gadd=NULL;}
+  }
 
   if(mode == 0 or mode == 3){
   if(gtmp1D!= NULL){delete gtmp1D;gtmp1D=NULL;}
   if(gtmp2D!= NULL){delete gtmp2D;gtmp2D=NULL;}
   if(gtmp1F!= NULL){delete gtmp1F;gtmp1F=NULL;}
   if(gtmp2F!= NULL){delete gtmp2F;gtmp2F=NULL;}}
 
+
 }
 
 void quda_inverter::alloc_csfield_gpu()
 {
   TIMER("alloc_csfield_gpu");
   free_csfield(2);
   quda::ColorSpinorParam cs_tmp(cs_gpu);
@@ -780,15 +786,19 @@
 
     if(split_save == 0)
     if(n1!=0){qlat::load_qlat_noisesT(filename0, eigF, read, single_file, VECS_TYPE, INFO_LIST,n0,n0+n1, false);}
     if(split_save == 1)
     if(n1!=0){qlat::load_qlat_noisesT(filename1, eigF, read, single_file, VECS_TYPE, INFO_LIST, 0,   n1, false);}
   }
 
+  /////===load to gpu
   if(read == true){
+  for (int i = 0; i < kSpace.size(); i++) delete kSpace[i];kSpace.resize(0);
+  for (int i = 0; i < fSpace.size(); i++) delete fSpace[i];fSpace.resize(0);
+
   eig_param.n_ev_deflate = ns0;eig_solveK = quda::EigenSolver::create(&eig_param, *mat_E, profileEigensolve);
   eig_param.n_ev_deflate = ns1;eig_solveF = quda::EigenSolver::create(&eig_param, *mat_E, profileEigensolve);
 
   for(int n = 0; n < ns0; n++){kSpace.push_back(quda::ColorSpinorField::Create(cs_gpuD));}
   for(int n = 0; n < ns1; n++){fSpace.push_back(quda::ColorSpinorField::Create(cs_gpuF));}
   for(int n = 0; n < n0; n++){
     qlat_cf_to_quda_cf((qlat::Complex*) ctmp0->V(), eigD[n]);
@@ -846,14 +856,15 @@
 
   //for (int i = 0; i < evecs_.size(); i++) delete evecs_[i];
   //evecs_.resize(0);
   //evecs.resize(0);
   for (int i = 0; i < kSpace.size(); i++) delete kSpace[i];kSpace.resize(0);
   for (int i = 0; i < fSpace.size(); i++) delete fSpace[i];fSpace.resize(0);
   for (int i = 0; i < ZSpace.size(); i++) delete ZSpace[i];ZSpace.resize(0);
+  for (int i = 0; i < kSpace_cpu.size(); i++) delete kSpace_cpu[i];kSpace_cpu.resize(0);
   evalsK.resize(0);
   evalsF.resize(0);
   evalsZ.resize(0);
   free_csfield();
 
   if(eig_solveF != NULL){delete eig_solveF;eig_solveF=NULL;}
   if(eig_solveK != NULL){delete eig_solveK;eig_solveK=NULL;}
@@ -1335,14 +1346,16 @@
 
 }
 
 void quda_inverter::setup_inv_mass(const double mass)
 {
   TIMER("setup_inv_mass");
   int verbos = 0;
+  std::string val = qlat::get_env(std::string("qlat_quda_verbos"));
+  if(val != ""){verbos = stringtonum(val);}
   if(verbos == 0)
   {
     inv_param.verbosity   = QUDA_SUMMARIZE;
   }
   else{
     setVerbosity(QUDA_VERBOSE);
     inv_param.verbosity   = QUDA_VERBOSE;
@@ -1625,15 +1638,26 @@
 
   if(nvec <= 0){errorQuda("Eigensystem need nvec largger than zero");}
   if(quda::comm_rank()== 0){printfQuda("Number of QUDA eigen vectors %d .\n", nvec);}
   eig_param = newQudaEigParam();
   eig_param.invert_param = &inv_param;
 
   ////===basice eig parameters
-  eig_param.eig_type = QUDA_EIG_TR_LANCZOS; ////or QUDA_EIG_IR_ARNOLDI
+  //QUDA_EIG_TR_LANCZOS,     // Thick restarted lanczos solver
+  //QUDA_EIG_BLK_TR_LANCZOS, // Block Thick restarted lanczos solver
+  //QUDA_EIG_IR_ARNOLDI,     // Implicitly Restarted Arnoldi solver
+  //QUDA_EIG_BLK_IR_ARNOLDI, // Block Implicitly Restarted Arnoldi solver
+  int eigensolve_type = 0;
+  std::string val = qlat::get_env(std::string("qlat_quda_eigensolve_type"));
+  if(val != ""){eigensolve_type = stringtonum(val);}
+  if(eigensolve_type == 0){eig_param.eig_type = QUDA_EIG_TR_LANCZOS; } // Thick restarted lanczos solver
+  if(eigensolve_type == 1){eig_param.eig_type = QUDA_EIG_BLK_TR_LANCZOS; } //Block Thick restarted lanczos solver
+  if(eigensolve_type == 2){eig_param.eig_type = QUDA_EIG_IR_ARNOLDI;} // Implicitly Restarted Arnoldi solver
+  if(eigensolve_type == 3){eig_param.eig_type = QUDA_EIG_BLK_IR_ARNOLDI;}  // Block Implicitly Restarted Arnoldi solver
+
   eig_param.spectrum = QUDA_SPECTRUM_SR_EIG;
   if ((eig_param.eig_type == QUDA_EIG_TR_LANCZOS || eig_param.eig_type == QUDA_EIG_BLK_TR_LANCZOS)
       && !(eig_param.spectrum == QUDA_SPECTRUM_LR_EIG || eig_param.spectrum == QUDA_SPECTRUM_SR_EIG)) {
     errorQuda("Only real spectrum type (LR or SR) can be passed to Lanczos type solver.");
   }
 
   // The solver will exit when n_conv extremal eigenpairs have converged
@@ -1729,14 +1753,16 @@
 
   if(compute){
     /////evecs = (void **)safe_malloc(nvec * sizeof(void *));
     //bool singleE = false;
     //if(compute == true ){singleE = false;}
     //if(compute == false){singleE = true;}
     evalsK.resize(nvec, 0.0);
+
+    ////for (int i = 0; i < kSpace_cpu.size(); i++) delete kSpace_cpu[i];kSpace_cpu.resize(0);
     for (int i = 0; i < nvec; i++){kSpace.push_back(quda::ColorSpinorField::Create(cs_gpuD));}
     fSpace.resize(0);evalsF.resize(0);
     //for (int i = 0; i < nvec; i++) { 
     //  if(singleE== false)kSpace.push_back(quda::ColorSpinorField::Create(cs_gpuD)); 
     //  if(singleE== true )kSpace.push_back(quda::ColorSpinorField::Create(cs_gpuF)); 
     //}
 
@@ -1754,14 +1780,23 @@
     mass_value = 0.0;
     for(int ni=0;ni<evals_ZERO.size();ni++)
     {
       evals_ZERO[ni] = evalsK[ni].real()/1.0 - 4.0 * mass * mass;
     }
     /////evals_ERR = (*eig_solveK).residua;
     evals_ERR.resize(evalsK.size(), 0.0);
+
+    //for (int i = 0; i < kSpace.size(); i++) delete kSpace[i];kSpace.resize(0);
+    //for(int i=0;i<nvec;i++)
+    //{
+    //  kSpace.push_back(quda::ColorSpinorField::Create(cs_gpuD));
+    //  *kSpace[i] = *kSpace_cpu[i];
+    //}
+
+    ////copy to GPU float and stuff, assummed all double
   }
 
 }
 
 void quda_inverter::update_eigen_mass(const double mass, bool force)
 {
   TIMER("update_eigen_mass");
@@ -2010,15 +2045,15 @@
     quda::blas::zero(*gtmp1);
     (*mat)(*gtmp1, *gres, *gtmp0, *gtmp2);
 
     quda::Complex srcn = quda::blas::norm2(*gsrc);
     quda::Complex resn = quda::blas::norm2(*gtmp1);
     quda::Complex evals  = quda::blas::cDotProduct(*gsrc, *gtmp1) / quda::blas::norm2(*gsrc);
     quda::Complex factor = sqrt(quda::blas::norm2(*gtmp1)) / sqrt(quda::blas::norm2(*gsrc));
-    quda::blas::caxpby(evals, *gsrc , n_unit, *gtmp1 );
+    quda::blas::caxpby(evals, *gsrc , n_unit, *gtmp1 ); ///tmp = ev*src + n * gtmp
     quda::Complex residual = sqrt(quda::blas::norm2(*gtmp1)/ quda::blas::norm2(*gsrc));
 
     quda::blas::zero(*gtmp1);
     (*mat)(*gtmp1, *gres, *gtmp0, *gtmp2);
     quda::Complex even_v  = quda::blas::cDotProduct((*gsrc).Even(), (*gtmp1).Even()) / quda::blas::norm2((*gsrc).Even());
     quda::blas::caxpby(even_v, (*gsrc).Even() , n_unit, (*gtmp1).Even() );
     quda::Complex res_e = sqrt(quda::blas::norm2((*gtmp1).Even())/ quda::blas::norm2((*gsrc).Even()));
@@ -2101,27 +2136,30 @@
     //(*gtmp1) = *gtmp2;
     //quda::blas::caxpby(m_unit, (*gres).Even() , n_unit, (*gtmp1).Even());
     //quda::Complex residual = quda::blas::norm2((*gtmp1).Even());
     //if(quda::comm_rank_global()== 0)printf("===Even %.3e, s %.1e %.1e, n %.1e %.1e \n", residual.real(), 
     //  s0_e.real(), s0_o.real(), n0_e.real(), n0_o.real());
   }
 
+  quda::Complex n_unit(1.0, 0.0);
   if(mode == 0){
     ////mode 0 write
     quda::blas::zero(*gres);
     int n_defl = 0;
     //*gtmp1 = *gsrc;
     /////Doe v_e
     quda::blas::zero((*gtmp1).Odd());
     dirac->Dslash((*gtmp1).Odd(), (*gsrc).Odd(), QUDA_EVEN_PARITY);
     quda::blas::ax(-1.0, (*gtmp1).Odd());
     (*gtmp1).Even() = (*gsrc).Even();
 
     if(gtmp1D == NULL){gtmp1D = new quda::ColorSpinorField(cs_gpuD);}
+    if(gtmp2D == NULL){gtmp2D = new quda::ColorSpinorField(cs_gpuD);}
     if(gtmp1F == NULL){gtmp1F = new quda::ColorSpinorField(cs_gpuF);}
+    if(gtmp2F == NULL){gtmp2F = new quda::ColorSpinorField(cs_gpuF);}
     //if(gtmp2D == NULL){gtmp2D = new quda::ColorSpinorField(cs_gpuD);}
     //if(gtmp2F == NULL){gtmp2F = new quda::ColorSpinorField(cs_gpuF);}
 
     for(int kf=0;kf<2;kf++)
     {
       std::vector<quda::ColorSpinorField *> eig_vecs;
       if(kf==0){n_defl = kSpace.size();eig_vecs.reserve(n_defl);for(int i=0;i<n_defl;i++){eig_vecs.push_back(kSpace[i]);}}
@@ -2152,18 +2190,22 @@
         A[i] = ( 2*m * ai - bi ) / (4*m*m + l*l);
         B[i] = -1.0 * ai/(4.0*m*m + l*l) - 2*m * bi/(l*l * (4*m*m + l*l));
       }
 
       ////std::vector<quda::ColorSpinorField *> sol;
       //sol.push_back(&(gres->Even()));
       quda::blas::caxpy(A.data(), eig_vecs, buf);
-      gres->Even() = *buf[0];
-      //sol[0] = &(gres->Odd());
+      /////gres->Even() = gres->Even() + *buf[0];
+      gtmp2->Even() = *buf[0];
+      quda::blas::caxpby(n_unit, gtmp2->Even() , n_unit, gres->Even());
+      ////sol[0] = &(gres->Odd());
       quda::blas::caxpy(B.data(), eig_vecs, buf);
-      gres->Odd() = *buf[0];
+      gtmp2->Odd()  = *buf[0];
+      quda::blas::caxpby(n_unit, gtmp2->Odd()  , n_unit, gres->Odd());
+      ////gres->Odd()  = gres->Odd() + *buf[0];
     }
 
     quda::blas::zero((*gtmp1).Odd());
     dirac->Dslash((*gtmp1).Odd(), (*gres).Odd(), QUDA_ODD_PARITY);
     quda::blas::ax(-1.0, (*gtmp1).Odd());
     (*gres).Odd() = (*gtmp1).Odd();
 
@@ -2517,22 +2559,41 @@
   if(qinv.fermion_type == 1)qinv.setup_mat_mass(mass);
   ///Ty* quda_src = (Ty*) qinv.csrc->V();
   ///Ty* quda_res = (Ty*) qinv.cres->V();
   qlat_cf_to_quda_cf((qlat::Complex*) qinv.csrc->V(), src);
 
   //Ty norm = norm_FieldM(prop);
   //print0("normp %.3e %.3e \n", norm.real(), norm.imag());
+  if(low_only == 0){
+    qinv.do_inv(qinv.cres->V(), qinv.csrc->V(), mass, err, niter, prec_type);
+  }
 
   if(low_only == 1){
     (*qinv.gsrc) = (*qinv.csrc);
     qinv.prepare_low_prop();
     (*qinv.cres) = (*qinv.gres);
   }
-  else{
+
+  if(low_only == 2){
+    if(qinv.gadd == NULL){
+      quda::ColorSpinorParam param(*qinv.gres);
+      qinv.gadd  = quda::ColorSpinorField::Create(param);
+    }
+
     qinv.do_inv(qinv.cres->V(), qinv.csrc->V(), mass, err, niter, prec_type);
+    (*qinv.gadd) = (*qinv.cres);
+
+    (*qinv.gsrc) = (*qinv.csrc);
+    qinv.prepare_low_prop();
+
+    quda::Complex n_unit(+1.0, 0.0);
+    quda::Complex p_unit(-1.0, 0.0);
+    quda::blas::caxpby(n_unit, *qinv.gadd  , p_unit, *qinv.gres);
+
+    (*qinv.cres) = (*qinv.gres);
   }
 
   if(!prop.initialized){prop.init(src.geo());} ////allocate mem for prop
   quda_cf_to_qlat_cf(prop, (qlat::Complex*) qinv.cres->V());
 
   //   norm = norm_FieldM(prop);
   //print0("normp %.3e %.3e \n", norm.real(), norm.imag());
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_read_txt.h` & `qlat-0.9/include/qlat/vector_utils/utils_read_txt.h`

 * *Files 0% similar despite different names*

```diff
@@ -1225,17 +1225,16 @@
     if(qlat::get_id_node()==node_control){
       file_open = fopen(filename, "wb");
       fseek( file_open , head_off , SEEK_SET );
     }
     ////return off_file ;
   }
 
-  inline crc32_t write_part(size_t off , size_t Psize, int type = 0)
+  inline crc32_t write_part(size_t off , size_t Psize)
   {
-    (void)type;
     qassert(head_off != 0);
     qassert(write_bsize > 0);
     qassert(write_type == 0 or write_type == 1);
     crc32_t crc32_tem = 0;
     if(qlat::get_id_node()==node_control){
       qassert(file_open != NULL);
       buf.resize(Psize * write_bsize);
@@ -1266,15 +1265,15 @@
       }
       ////correct the file if not all total is written
       if(total > total_write){
         print0("Write additional data \n");
         shift_off(total_write);
         size_t diff = total - total_write;
         const long cur = get_off();
-        crc32_t crc32_tem = write_part(cur, diff , node_control );
+        crc32_t crc32_tem = write_part(cur, diff );
         crc32_list.push_back(crc32_tem);
         crc32_size.push_back(diff * write_bsize);
         total_write += diff;
         Ns += 1;
       }
 
       /////calculate crc32 sum 
@@ -1302,15 +1301,15 @@
       size_t partF  = total / factor;
       size_t end_of_file = head_off + factor * partF*write_bsize;
 
       for(size_t fi=0;fi<factor;fi++)
       {
         size_t pos_file_cur = head_off + fi * partF*write_bsize;
         size_t off_data = fi * partF;
-        crc32_t crc32_tem = write_part(off_data, partF , node_control );
+        crc32_t crc32_tem = write_part(off_data, partF  );
         crc32_tem = crc32_combine(crc32_tem, 0, end_of_file - pos_file_cur - partF * write_bsize);
         crc32_total ^= crc32_tem;
       }
     }
 
     in_buf.checksum = crc32_total;
     update_info();
@@ -1394,15 +1393,15 @@
     if(!small_size){
       shift_off(double_size);
     }
     if( small_size)
     {
       qassert(write_bsize > 0);
       qassert(write_type == 0 or write_type == 1);
-      crc32_t crc32_tem = write_part(0, double_size , node_control );
+      crc32_t crc32_tem = write_part(0, double_size );
       crc32_list.push_back(crc32_tem);
       crc32_size.push_back(double_size * write_bsize);
       shift_off(0);
     }
 
   }
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_reduce_vec.h` & `qlat-0.9/include/qlat/vector_utils/utils_reduce_vec.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_shift_vecs.h` & `qlat-0.9/include/qlat/vector_utils/utils_shift_vecs.h`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #define UTILS_SHIFT_VECS_H
 #pragma once
 
 #include "general_funs.h"
 #include "utils_fft_desc.h"
 
 //////TODO
-//////GPU support, Ty template, shift of fieldM
+//////GPU support, Td template, shift of fieldM
 
 namespace qlat
 {
 
 struct shift_vec{
   int rank;int Nmpi;
   int nx,ny,nz,nt;
@@ -880,42 +880,42 @@
     srcP[bi] = (Ty*) qlat::get_data(src[bi]).data();
     resP[bi] = (Ty*) qlat::get_data(res[bi]).data();
   }
 
   svec.shift_vecs(srcP, resP, iDir , civ);
 }
 
-template <class Ty>
-void shift_fieldM(shift_vec& svec, std::vector<Propagator4dT<Ty >* >& src, std::vector<Propagator4dT<Ty >* >& res, std::vector<int >& iDir)
+template <class Td>
+void shift_fieldM(shift_vec& svec, std::vector<Propagator4dT<Td >* >& src, std::vector<Propagator4dT<Td >* >& res, std::vector<int >& iDir)
 {
   if(src.size() < 1)return;
   int biva_or = src.size();
 
-  std::vector<ComplexT<Ty>* > srcP;std::vector<ComplexT<Ty>* > resP;
+  std::vector<ComplexT<Td>* > srcP;std::vector<ComplexT<Td>* > resP;
   srcP.resize(biva_or);resP.resize(biva_or);
   for(int bi=0;bi<biva_or;bi++){
-    srcP[bi] = (ComplexT<Ty>*) qlat::get_data(*src[bi]).data();
-    resP[bi] = (ComplexT<Ty>*) qlat::get_data(*res[bi]).data();
+    srcP[bi] = (ComplexT<Td>*) qlat::get_data(*src[bi]).data();
+    resP[bi] = (ComplexT<Td>*) qlat::get_data(*res[bi]).data();
   }
   svec.shift_vecs(srcP, resP, iDir , 12*12);
 }
 
-template <class Ty>
-void shift_fieldM(shift_vec& svec, Propagator4dT<Ty >& src, Propagator4dT<Ty >& res, std::vector<int >& iDir)
+template <class Td>
+void shift_fieldM(shift_vec& svec, Propagator4dT<Td >& src, Propagator4dT<Td >& res, std::vector<int >& iDir)
 {
-  std::vector<Propagator4dT<Ty >* >srcP(1);srcP[0] = &src;
-  std::vector<Propagator4dT<Ty >* >resP(1);resP[0] = &res;
+  std::vector<Propagator4dT<Td >* >srcP(1);srcP[0] = &src;
+  std::vector<Propagator4dT<Td >* >resP(1);resP[0] = &res;
   shift_fieldM(svec, srcP, resP, iDir);
 }
 
-template <class Ty>
-void shift_fieldM(shift_vec& svec, std::vector<Propagator4dT<Ty > > & src, std::vector< Propagator4dT<Ty > >& res, std::vector<int >& iDir)
+template <class Td>
+void shift_fieldM(shift_vec& svec, std::vector<Propagator4dT<Td > > & src, std::vector< Propagator4dT<Td > >& res, std::vector<int >& iDir)
 {
-  std::vector<Propagator4dT<Ty >* >srcP(0);srcP.resize(src.size());
-  std::vector<Propagator4dT<Ty >* >resP(0);resP.resize(res.size());
+  std::vector<Propagator4dT<Td >* >srcP(0);srcP.resize(src.size());
+  std::vector<Propagator4dT<Td >* >resP(0);resP.resize(res.size());
   for(int i=0;i<src.size();i++){srcP[i] = &src[i];}
   for(int i=0;i<res.size();i++){resP[i] = &res[i];}
   shift_fieldM(svec, srcP, resP, iDir);
 }
 
 }
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_smear_vecs.h` & `qlat-0.9/include/qlat/vector_utils/utils_smear_vecs.h`

 * *Files 1% similar despite different names*

```diff
@@ -97,16 +97,15 @@
   }
 
   }
 
 }
 #endif
 
-
-
+////Ty must be complex
 template <typename Ty >
 struct smear_fun{
 
   Geometry geo;
   Geometry geo_ext;
   int dirL;
   bool smear_in_time_dir;
@@ -148,16 +147,16 @@
   void* gauge_check;
   crc32_t gauge_checksum;
   /////buffers
 
   bool  mem_setup_flag;
   qlat::vector_acc<qlat::Complex > mom_factors;
 
-  //template <class Tg>
-  //void setup(const GaugeFieldT<Tg >& gf, const CoordinateD& mom, const bool smear_in_time_dir){
+  //template <class Td>
+  //void setup(const GaugeFieldT<Td >& gf, const CoordinateD& mom, const bool smear_in_time_dir){
   //  qlat::vector_acc<qlat::Complex > momF(8);
   //  for (int i = 0; i < 8; ++i) {
   //    const int dir = i - 4;
   //    const double phase = dir >= 0 ? mom[dir] : -mom[-dir - 1];
   //    momF[i] = std::polar(1.0, -phase);
   //  }
   //  gauge_setup(gf, momF);
@@ -394,16 +393,16 @@
     }
     //shift_copy(f, recv_buffer , mapvq_recv, bfac);
     cpy_data_from_index(f, recv_buffer.data(), mapvq_recv[0].data(), mapvq_recv[1].data(), mapvq_recv[0].size(), bfac, GPU);
   }
 
   //void gauge_setup(qlat::vector_gpu<T >& gfE, const GaugeFieldT<Tg >& gf,
   //           const qlat::vector_acc<qlat::Complex >& momF = qlat::vector_acc<qlat::Complex >(), bool force_update = false);
-  template <class Tg>
-  void gauge_setup(const GaugeFieldT<Tg >& gf, const CoordinateD& mom_, bool force_update = false)
+  template <class Td>
+  void gauge_setup(const GaugeFieldT<Td >& gf, const CoordinateD& mom_, bool force_update = false)
   {
     qlat::vector_acc<qlat::Complex > momF(8);
     for (int i = 0; i < 8; ++i) {
       const int dir = i - 4;
       const double phase = dir >= 0 ? mom_[dir] : -mom_[-dir - 1];
       momF[i] = std::polar(1.0, -phase);
     }
@@ -412,26 +411,26 @@
     if(gauge_setup_flag == false){ update = true;}
     if(force_update){ update = true;}
     if(gauge.size() == 0){  update = true;}
     if(gauge_check != (void*) qlat::get_data(gf).data()){update = true;}
     if(mom_factors.size() != 8){update = true;}
     else{for(int i=0;i<momF.size();i++){if(momF[i]!=mom_factors[i]){update = true;}}}
 
-    crc32_t tmp_gauge_checksum = quick_checksum((Tg*) qlat::get_data(gf).data(), qlat::get_data_size(gf) / sizeof(Tg) );
+    crc32_t tmp_gauge_checksum = quick_checksum((Td*) qlat::get_data(gf).data(), qlat::get_data_size(gf) / sizeof(Td) );
     if(gauge_checksum != tmp_gauge_checksum ){update = true;}
 
     if(update){
       TIMERA("gauge setup");
       qassert(geo.total_site() == gf.geo().total_site());
       gauge.resize(2*4* gf.geo().local_volume() * 9);
       mom_factors = momF;
       extend_links_to_vecs(gauge.data(), gf, momF);
       gauge_setup_flag = true;
       gauge_check = (void*) qlat::get_data(gf).data();
-      gauge_checksum = quick_checksum((Tg*) qlat::get_data(gf).data(), qlat::get_data_size(gf) / sizeof(Tg));
+      gauge_checksum = quick_checksum((Td*) qlat::get_data(gf).data(), qlat::get_data_size(gf) / sizeof(Td));
       ///Need to redistribute when copied
       fft_copy = 0 ;
     }
   }
 
   void clear_mem(){
     #ifdef __CLEAR_SMEAR_MEM__
@@ -596,19 +595,19 @@
   skey.smear_in_time_dir = smear_in_time_dir;
   skey.prec = get_data_type<Ty >();
   return skey;
 }
 /////smear plan buffer related
 
 ////TODO need to change other parts for c0, c1
-template <class T, class Tg>
-void extend_links_to_vecs(T* resE, const GaugeFieldT<Tg >& gf, const qlat::vector_acc<qlat::Complex >& mom_factors=qlat::vector_acc<qlat::Complex >()){
+template <class T, class Td>
+void extend_links_to_vecs(T* resE, const GaugeFieldT<Td >& gf, const qlat::vector_acc<qlat::Complex >& mom_factors=qlat::vector_acc<qlat::Complex >()){
   TIMERB("extend_links_to_vecs");
   const Geometry& geo = gf.geo();
-  GaugeFieldT<Tg > gf1;
+  GaugeFieldT<Td > gf1;
   set_left_expanded_gauge_field(gf1, gf);
   const int dir_limit = 4;
   ////set up mom factors
   qlat::Complex* momF = NULL;
   qlat::vector_acc<qlat::Complex > buf_mom;buf_mom.resize(8);
   for(int i=0;i<buf_mom.size();i++){buf_mom[i] = 1;}
   if(mom_factors.size() == 0){momF = (qlat::Complex*) qlat::get_data(buf_mom).data();}
@@ -617,34 +616,35 @@
     momF = (qlat::Complex*) qlat::get_data(mom_factors).data();
   }
   ////set up mom factors
   //mom_factors()[dir + 4];
   qacc_for(index,  geo.local_volume(),{
     for (int dir = -dir_limit; dir < dir_limit; ++dir) {
       const Coordinate xl = geo.coordinate_from_index(index);
-      const ColorMatrixT<Tg > link =
+      const ColorMatrixT<Td > link =
           dir >= 0 ? gf1.get_elem(xl, dir)
-                   : (ColorMatrixT<Tg >)matrix_adjoint(
+                   : (ColorMatrixT<Td >)matrix_adjoint(
                          gf1.get_elem(coordinate_shifts(xl, dir), -dir - 1));
       ////convention used in gauss_smear_kernel CPU and gauss_smear_global4
       ////also in multiply_gauge of utils_shift_vecs.h
       for(int ci=0; ci<9; ci++){
         //resE[(index*dir_limit*2+ (dir+dir_limit))*9 + (ci%3)*3 + ci/3] = momF[dir + 4] * link.p[ci];
         resE[(index*dir_limit*2+ (dir+dir_limit))*9 + ci] = momF[dir + 4] * link.p[ci];
       }
     }
   });
 }
 
-template <class T, class Tg>
-void extend_links_to_vecs(qlat::vector_gpu<T >& gfE, const GaugeFieldT<Tg >& gf, const qlat::vector_acc<qlat::Complex >& mom_factors=qlat::vector_acc<qlat::Complex >()){
+template <class T, class Td>
+void extend_links_to_vecs(qlat::vector_gpu<T >& gfE, const GaugeFieldT<Td >& gf, const qlat::vector_acc<qlat::Complex >& mom_factors=qlat::vector_acc<qlat::Complex >()){
   gfE.resize(2*4* gf.geo().local_volume() * 9);
   extend_links_to_vecs(gfE.data(), gf, mom_factors);
 }
 
+/////T is double or float
 template <class T>
 void rotate_Vec_prop(Propagator4dT<T>& prop, qlat::vector_gpu<ComplexT<T> > &propT, unsigned int NVmpi, unsigned int groupP, int dir = 0)
 {
   TIMER("Rotate Vec prop");
   ///unsigned int NVmpi = fd.mz*fd.my*fd.mx;
   ///int groupP = (12+NVmpi-1)/NVmpi;
   qassert(groupP <= 12);qassert(groupP * NVmpi >= 12);
@@ -958,16 +958,17 @@
       if(dir == 0){res[off0] = buf[off1];}
       if(dir == 1){res[off1] = buf[off0];}
     }
   });
 }
 
 
-template <class Ty, int c0,int d0, class Tg>
-void smear_propagator_gwu_convension_inner(Ty* prop, const GaugeFieldT<Tg >& gf,
+////Td is double or float
+template <class Ty, int c0,int d0, class Td>
+void smear_propagator_gwu_convension_inner(Ty* prop, const GaugeFieldT<Td >& gf,
                       const double width, const int step, const CoordinateD& mom = CoordinateD(), const bool smear_in_time_dir = false, const int mode = 1)
 {
   TIMER_FLOPS("smear propagator");
   long long Tfloat = 0;
   ///double mem       = 0.0;
   Geometry geo = gf.geo();
   geo.multiplicity = 1;geo.eo=0;
@@ -1030,16 +1031,16 @@
     {TIMERC("Vec prop");smf.vec_rot->reorder(res, smf.prop_buf.data(), 1, c0*3*groupP , 100);}
     smf.mv_idx.dojob(res, res, 1, smf.NVmpi, Nvol_pre*c0*3, 0,  groupP , true);
     cpy_data_thread(prop, smf.prop.data(), smf.prop.size(), 1);
   }
   /////rotate_prop(prop, 1);
 }
 
-template <class Ty, class Tg>
-void smear_propagator_gwu_convension(qpropT& prop, const GaugeFieldT<Tg >& gf,
+template <class Ty, class Td>
+void smear_propagator_gwu_convension(qpropT& prop, const GaugeFieldT<Td >& gf,
                       const double width, const int step, const CoordinateD& mom = CoordinateD(), const bool smear_in_time_dir = false, const int mode = 1)
 {
   if (0 == step) {return;}
   const long Nvol = prop.geo().local_volume();
   Ty* src = (Ty*) qlat::get_data(prop).data();
   move_index mv_civ;int flag = 0;
   flag = 0;mv_civ.dojob(src, src, 1, 12*12, Nvol, flag, 1, false);
@@ -1050,70 +1051,70 @@
     for(int d0=0;d0<12*4;d0++)
     for(int c0=0;c0<   3;c0++)
     {
       src[isp*12*12 + c0*12*4 + d0] = buf[d0*3 + c0];
     }
   });
 
-  smear_propagator_gwu_convension_inner<Ty, 1, 12*4, Tg>(src, gf, width, step, mom, smear_in_time_dir, mode);
+  smear_propagator_gwu_convension_inner<Ty, 1, 12*4, Td>(src, gf, width, step, mom, smear_in_time_dir, mode);
 
   qacc_for(isp, Nvol, {
     ALIGN Ty buf[12*12];
     for(int i=0;i<12*12;i++){buf[i] = src[isp*12*12 + i];}
     for(int d0=0;d0<12*4;d0++)
     for(int c0=0;c0<   3;c0++)
     {
       src[isp*12*12 + d0*3 + c0] = buf[c0*12*4 + d0];
     }
   });
   flag = 1;mv_civ.dojob(src, src, 1, 12*12, Nvol, flag, 1, false);
 }
 
-template <class Ty, class Tg>
-void smear_propagator_gwu_convension(qlat::FieldM<Ty , 12>& prop, const GaugeFieldT<Tg >& gf,
+template <class Ty, class Td>
+void smear_propagator_gwu_convension(qlat::FieldM<ComplexT<Ty> , 12>& prop, const GaugeFieldT<Td >& gf,
                       const double width, const int step, const CoordinateD& mom = CoordinateD(), const bool smear_in_time_dir = false, const int mode = 1)
 {
   if (0 == step) {return;}
-  Ty* src = (Ty*) qlat::get_data(prop).data();
+  ComplexT<Ty>* src = (ComplexT<Ty>*) qlat::get_data(prop).data();
   qacc_for(isp, prop.geo().local_volume(), {
-    ALIGN Ty buf[12];
+    ALIGN ComplexT<Ty> buf[12];
     for(int i=0;i<12;i++){buf[i] = src[isp*12 + i];}
     for(int d0=0;d0<4;d0++)
     for(int c0=0;c0<   3;c0++)
     {
       src[isp*12 + c0*4 + d0] = buf[d0*3 + c0];
     }
   });
 
-  smear_propagator_gwu_convension_inner<Ty, 1, 4, Tg>(src, gf, width, step, mom, smear_in_time_dir, mode);
+  smear_propagator_gwu_convension_inner<ComplexT<Ty>, 1, 4, Td>(src, gf, width, step, mom, smear_in_time_dir, mode);
   qacc_for(isp, prop.geo().local_volume(), {
-    ALIGN Ty buf[12];
+    ALIGN ComplexT<Ty> buf[12];
     for(int i=0;i<12;i++){buf[i] = src[isp*12 + i];}
     for(int d0=0;d0<4;d0++)
     for(int c0=0;c0<   3;c0++)
     {
       src[isp*12 + d0*3 + c0] = buf[c0*4 + d0];
     }
   });
 }
 
 
-template <class Ty, class Tg>
-void smear_propagator_gwu_convension(Propagator4dT<Ty>& prop, const GaugeFieldT<Tg >& gf,
+template <class Ty, class Td>
+void smear_propagator_gwu_convension(Propagator4dT<Ty>& prop, const GaugeFieldT<Td >& gf,
                       const double width, const int step, const CoordinateD& mom = CoordinateD(), const bool smear_in_time_dir = false, const int mode = 1)
 {
   if (0 == step) {return;}
   rotate_prop(prop, 0);
   ComplexT<Ty>* src = (ComplexT<Ty>*) qlat::get_data(prop).data();
-  smear_propagator_gwu_convension_inner<ComplexT<Ty>, 1, 12*4, Tg>(src, gf, width, step, mom, smear_in_time_dir, mode);
+  smear_propagator_gwu_convension_inner<ComplexT<Ty>, 1, 12*4, Td>(src, gf, width, step, mom, smear_in_time_dir, mode);
   rotate_prop(prop, 1);
 }
 
-template <class T, class Tg>
-void smear_propagator_qlat_convension(Propagator4dT<T>& prop, const GaugeFieldT<Tg >& gf,
+template <class T, class Td>
+void smear_propagator_qlat_convension(Propagator4dT<T>& prop, const GaugeFieldT<Td >& gf,
                       const double coef, const int step, const CoordinateD& mom = CoordinateD(), const bool smear_in_time_dir = false, const int mode = 1)
 {
   if(coef <= 0){return ;}
   double width = 0.0;
   if(step <  0){width = coef;}////box smearings
   if(step >= 0){width = std::sqrt(coef*2*step/(3.0));}////gauss smearings
   smear_propagator_gwu_convension(prop, gf, width, step, mom, smear_in_time_dir, mode);
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_stagger_contractions.h` & `qlat-0.9/include/qlat/vector_utils/utils_stagger_contractions.h`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,12 @@
   {
     auto v0 = corr[ti] * factor;
     print0("ti %5d , cf cf^dagger %+.8e  %+.8e \n", ti, v0.real(), v0.imag());
   }
 
 }
 
-////P5_ij(x) = Xib_i(x) (-1)^(x+y+z+t) Xi_j(x)       :  g5 x g5 [Goldstone, exotic parity partner 0^{+-}]
-
 }
 
 
 #endif
```

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_test_unified.h` & `qlat-0.9/include/qlat/vector_utils/utils_test_unified.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/vector_utils/utils_vector_GPU.h` & `qlat-0.9/include/qlat/vector_utils/utils_vector_GPU.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/include/qlat/wilson-flow.h` & `qlat-0.9/include/qlat/wilson-flow.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/meson.build` & `qlat-0.9/meson.build`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-project('qlat', 'cpp',
-  version: '0.8',
+project('qlat', 'cpp', 'cython',
+  version: '0.9',
   license: 'GPL-3.0-or-later',
   default_options: [
     'warning_level=3',
     'cpp_std=c++14',
     'libdir=lib',
     'optimization=2',
     'debug=false',
+    'cython_language=cpp',
     ])
 
 add_project_arguments('-fno-strict-aliasing', language: ['c', 'cpp'])
 
 cpp = meson.get_compiler('cpp')
 
+fs = import('fs')
+
 py_mod = import('python')
 py3 = py_mod.find_installation('python3')
 message(py3.path())
 message(py3.get_install_dir())
 
 if get_option('use_cxx')
   message('use_cxx=true (use CXX compiler without additional MPI options.)')
```

### Comparing `qlat-0.8/pylib/auto_contractor/ama.py` & `qlat-0.9/pylib/auto_contractor/ama.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/auto_contractor/benchmark.py` & `qlat-0.9/pylib/auto_contractor/benchmark.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/auto_contractor/compile.py` & `qlat-0.9/pylib/auto_contractor/compile.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/auto_contractor/eval.py` & `qlat-0.9/pylib/auto_contractor/eval.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/auto_contractor/eval_sc_qlat.py` & `qlat-0.9/pylib/auto_contractor/eval_sc_qlat.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/auto_contractor/expr_arithmetic.py` & `qlat-0.9/pylib/auto_contractor/expr_arithmetic.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/auto_contractor/operators.py` & `qlat-0.9/pylib/auto_contractor/operators.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/auto_contractor/runtime.py` & `qlat-0.9/pylib/auto_contractor/runtime.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/auto_contractor/simulation.py` & `qlat-0.9/pylib/auto_contractor/simulation.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/auto_contractor/wick.py` & `qlat-0.9/pylib/auto_contractor/wick.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/contraction-field.cpp` & `qlat-0.9/pylib/cqlat/contraction-field.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/contraction-hvp.cpp` & `qlat-0.9/pylib/cqlat/contraction-hvp.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/contraction-pion.cpp` & `qlat-0.9/pylib/cqlat/contraction-pion.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/coordinate.cpp` & `qlat-0.9/pylib/cqlat/coordinate.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/exports.h` & `qlat-0.9/pylib/cqlat/exports.h`

 * *Files 0% similar despite different names*

```diff
@@ -222,16 +222,14 @@
 EXPORT_FUNCTION(qnorm_field)
 EXPORT_FUNCTION(qnorm_field_field)
 EXPORT_FUNCTION(qnorm_field_sfield)
 EXPORT_FUNCTION(qnorm_field_spfield)
 EXPORT_FUNCTION(qnorm_sfield)
 EXPORT_FUNCTION(qnorm_spfield)
 EXPORT_FUNCTION(qquit)
-EXPORT_FUNCTION(qremove_all_info)
-EXPORT_FUNCTION(qremove_info)
 EXPORT_FUNCTION(read_sfr_field)
 EXPORT_FUNCTION(read_sfr_sfield)
 EXPORT_FUNCTION(reflect_field)
 EXPORT_FUNCTION(refresh_expanded_1_field)
 EXPORT_FUNCTION(refresh_expanded_field)
 EXPORT_FUNCTION(release_lock)
 EXPORT_FUNCTION(save_complex_spfield)
```

### Comparing `qlat-0.8/pylib/cqlat/fermion-action.cpp` & `qlat-0.9/pylib/cqlat/fermion-action.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/field-double.cpp` & `qlat-0.9/pylib/cqlat/field-double.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/field-io.cpp` & `qlat-0.9/pylib/cqlat/field-io.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/field-selection.cpp` & `qlat-0.9/pylib/cqlat/field-selection.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/field-utils.cpp` & `qlat-0.9/pylib/cqlat/field-utils.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/field.cpp` & `qlat-0.9/pylib/cqlat/field.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/fields-io.cpp` & `qlat-0.9/pylib/cqlat/fields-io.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/gauge-action.cpp` & `qlat-0.9/pylib/cqlat/gauge-action.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/geometry.cpp` & `qlat-0.9/pylib/cqlat/geometry.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/hmc-stats.cpp` & `qlat-0.9/pylib/cqlat/hmc-stats.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/hmc.cpp` & `qlat-0.9/pylib/cqlat/hmc.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/init.cpp` & `qlat-0.9/pylib/cqlat/init.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/inverter.cpp` & `qlat-0.9/pylib/cqlat/inverter.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/lib.cpp` & `qlat-0.9/pylib/cqlat/lib.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/lib.h` & `qlat-0.9/pylib/cqlat/lib.h`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/mat.cpp` & `qlat-0.9/pylib/cqlat/mat.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/mpi.cpp` & `qlat-0.9/pylib/cqlat/mpi.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/propagator.cpp` & `qlat-0.9/pylib/cqlat/propagator.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/qcd.cpp` & `qlat-0.9/pylib/cqlat/qcd.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/scalar-action.cpp` & `qlat-0.9/pylib/cqlat/scalar-action.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/selected-field.cpp` & `qlat-0.9/pylib/cqlat/selected-field.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/selected-points.cpp` & `qlat-0.9/pylib/cqlat/selected-points.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/smear.cpp` & `qlat-0.9/pylib/cqlat/smear.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/topology.cpp` & `qlat-0.9/pylib/cqlat/topology.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/update.sh` & `qlat-0.9/pylib/cqlat/update.sh`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/cqlat/utils-io.cpp` & `qlat-0.9/pylib/cqlat/utils-io.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,9 @@
 #include "lib.h"
 
-EXPORT(qremove_info, {
-  using namespace qlat;
-  PyObject* p_path = NULL;
-  if (!PyArg_ParseTuple(args, "O", &p_path)) {
-    return NULL;
-  }
-  const std::string path = py_convert_data<std::string>(p_path);
-  const int ret = qremove_info(path);
-  return py_convert(ret);
-})
-
-EXPORT(qremove_all_info, {
-  using namespace qlat;
-  PyObject* p_path = NULL;
-  if (!PyArg_ParseTuple(args, "O", &p_path)) {
-    return NULL;
-  }
-  const std::string path = py_convert_data<std::string>(p_path);
-  const int ret = qremove_all_info(path);
-  return py_convert(ret);
-})
-
 EXPORT(qmkdir_sync_node, {
   using namespace qlat;
   PyObject* p_path = NULL;
   if (!PyArg_ParseTuple(args, "O", &p_path)) {
     return NULL;
   }
   const std::string path = py_convert_data<std::string>(p_path);
```

### Comparing `qlat-0.8/pylib/cqlat/wilson-flow.cpp` & `qlat-0.9/pylib/cqlat/wilson-flow.cpp`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/__init__.py` & `qlat-0.9/pylib/qlat/__init__.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/coordinate.py` & `qlat-0.9/pylib/qlat/coordinate.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/fermion_action.py` & `qlat-0.9/pylib/qlat/fermion_action.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/field.py` & `qlat-0.9/pylib/qlat/field.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/field_double.py` & `qlat-0.9/pylib/qlat/field_double.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/field_selection.py` & `qlat-0.9/pylib/qlat/field_selection.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/field_utils.py` & `qlat-0.9/pylib/qlat/field_utils.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/fields_io.py` & `qlat-0.9/pylib/qlat/fields_io.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/geometry.py` & `qlat-0.9/pylib/qlat/geometry.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/hmc.py` & `qlat-0.9/pylib/qlat/hmc.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/hmc_stats.py` & `qlat-0.9/pylib/qlat/hmc_stats.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/inverter.py` & `qlat-0.9/pylib/qlat/inverter.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/mat.py` & `qlat-0.9/pylib/qlat/mat.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/mpi.py` & `qlat-0.9/pylib/qlat/mpi.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/propagator.py` & `qlat-0.9/pylib/qlat/propagator.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/qcd.py` & `qlat-0.9/pylib/qlat/qcd.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/scalar_action.py` & `qlat-0.9/pylib/qlat/scalar_action.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/selected_field.py` & `qlat-0.9/pylib/qlat/selected_field.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/selected_points.py` & `qlat-0.9/pylib/qlat/selected_points.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/smear.py` & `qlat-0.9/pylib/qlat/smear.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/topology.py` & `qlat-0.9/pylib/qlat/topology.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/utils_io.py` & `qlat-0.9/pylib/qlat/utils_io.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat/wilson_flow.py` & `qlat-0.9/pylib/qlat/wilson_flow.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/qlat_gpt.py` & `qlat-0.9/pylib/qlat_gpt.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd.py` & `qlat-0.9/pylib/rbc_ukqcd.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/__init__.py` & `qlat-0.9/pylib/rbc_ukqcd_params/__init__.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_16IH2.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_16IH2.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_24D.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_24D.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_24DH.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_24DH.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_24IH01.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_24IH01.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_24IH02.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_24IH02.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_24IH03.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_24IH03.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_24IH04.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_24IH04.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_24IH05.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_24IH05.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_24IH1.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_24IH1.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_24IH2.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_24IH2.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_24IH3.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_24IH3.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_24IH4.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_24IH4.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_32D.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_32D.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_32Dfine.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_32Dfine.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_32IH01.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_32IH01.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_32IH1.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_32IH1.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_32IH2.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_32IH2.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_32IH3.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_32IH3.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_32IcoarseH01.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_32IcoarseH01.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_32IcoarseH02.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_32IcoarseH02.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_32IcoarseH1.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_32IcoarseH1.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_32IfineH.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_32IfineH.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_48I.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_48I.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_64I.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_64I.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/p_test.py` & `qlat-0.9/pylib/rbc_ukqcd_params/p_test.py`

 * *Files identical despite different names*

### Comparing `qlat-0.8/pylib/rbc_ukqcd_params/utils.py` & `qlat-0.9/pylib/rbc_ukqcd_params/utils.py`

 * *Files identical despite different names*

