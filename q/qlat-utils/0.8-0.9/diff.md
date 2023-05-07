# Comparing `tmp/qlat_utils-0.8.tar.gz` & `tmp/qlat_utils-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlat_utils-0.8.tar", last modified: Sun Nov 27 17:51:16 2022, max compression
+gzip compressed data, was "qlat_utils-0.9.tar", last modified: Sat Dec 10 16:32:11 2022, max compression
```

## Comparing `qlat_utils-0.8.tar` & `qlat_utils-0.9.tar`

### file list

```diff
@@ -1,67 +1,73 @@
--rw-rw-r--   0        0        0    35092 1970-01-01 00:00:00.000000 qlat_utils-0.8/LICENSE
--rw-rw-r--   0        0        0       34 1970-01-01 00:00:00.000000 qlat_utils-0.8/README.md
--rwxrwxr-x   0        0        0      356 1970-01-01 00:00:00.000000 qlat_utils-0.8/bin/crc32
--rwxrwxr-x   0        0        0      267 1970-01-01 00:00:00.000000 qlat_utils-0.8/bin/lat-io-diff
--rwxrwxr-x   0        0        0      207 1970-01-01 00:00:00.000000 qlat_utils-0.8/bin/lat-io-glimpse
--rwxrwxr-x   0        0        0      257 1970-01-01 00:00:00.000000 qlat_utils-0.8/bin/pickle-glimpse
--rwxrwxr-x   0        0        0     4070 1970-01-01 00:00:00.000000 qlat_utils-0.8/bin/qar
--rwxrwxr-x   0        0        0     1096 1970-01-01 00:00:00.000000 qlat_utils-0.8/bin/qar-glimpse
--rwxrwxr-x   0        0        0       98 1970-01-01 00:00:00.000000 qlat_utils-0.8/bin/qlat-utils-include
--rw-rw-r--   0        0        0       55 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/meson.build
--rw-rw-r--   0        0        0     1550 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/array.h
--rw-rw-r--   0        0        0     2425 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/assert.h
--rw-rw-r--   0        0        0     4497 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/cache.h
--rw-rw-r--   0        0        0      986 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/compatible-endian.h
--rw-r--r--   0        0        0      207 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/compatible-omp.h
--rw-rw-r--   0        0        0     1061 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/complex.h
--rw-rw-r--   0        0        0       43 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/config.h
--rw-rw-r--   0        0        0     3145 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/core.h
--rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/crc32.h
--rw-rw-r--   0        0        0      943 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/eigen.h
--rw-rw-r--   0        0        0     3317 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/handle.h
--rw-rw-r--   0        0        0    16603 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/lat-io.h
--rw-rw-r--   0        0        0      920 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/meson.build
--rw-rw-r--   0        0        0     8389 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/py_convert.h
--rw-rw-r--   0        0        0     4990 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/qacc-func.h
--rw-rw-r--   0        0        0      480 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/qacc.h
--rw-rw-r--   0        0        0    22570 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/qar-cache.h
--rw-rw-r--   0        0        0    33580 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/qar.h
--rw-rw-r--   0        0        0     8946 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/qutils-extra.h
--rw-rw-r--   0        0        0    10976 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/qutils-io.h
--rw-rw-r--   0        0        0    14507 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/qutils-vec.h
--rw-rw-r--   0        0        0     3084 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/qutils.h
--rw-r--r--   0        0        0    10128 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/rng-state.h
--rw-r--r--   0        0        0    14882 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/sha256.h
--rw-rw-r--   0        0        0     8144 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/show.h
--rw-r--r--   0        0        0     2254 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/sprng-sha256.h
--rw-rw-r--   0        0        0    22330 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/timer.h
--rw-rw-r--   0        0        0    13450 1970-01-01 00:00:00.000000 qlat_utils-0.8/include/qlat-utils/vector.h
--rw-rw-r--   0        0        0      843 1970-01-01 00:00:00.000000 qlat_utils-0.8/meson.build
--rw-rw-r--   0        0        0     2520 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/cqlat_utils/exports.h
--rw-rw-r--   0        0        0     7602 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/cqlat_utils/lat-io.cpp
--rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/cqlat_utils/lib.cpp
--rw-rw-r--   0        0        0     2208 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/cqlat_utils/lib.h
--rw-rw-r--   0        0        0      369 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/cqlat_utils/meson.build
--rw-rw-r--   0        0        0     3280 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/cqlat_utils/qar.cpp
--rw-rw-r--   0        0        0     1654 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/cqlat_utils/rng-state.cpp
--rw-r--r--   0        0        0     3619 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/cqlat_utils/timer.cpp
--rwxr-xr-x   0        0        0      766 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/cqlat_utils/update.sh
--rw-rw-r--   0        0        0     6173 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/cqlat_utils/utils-io.cpp
--rw-rw-r--   0        0        0     1018 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/cqlat_utils/utils.cpp
--rw-rw-r--   0        0        0       43 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/meson.build
--rw-rw-r--   0        0        0      615 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/qlat_utils/__init__.py
--rw-rw-r--   0        0        0     1887 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/qlat_utils/cache.py
--rw-rw-r--   0        0        0      155 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/qlat_utils/cu.py
--rw-rw-r--   0        0        0    16937 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/qlat_utils/data.py
--rw-rw-r--   0        0        0      212 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/qlat_utils/get_include_dir.py
--rw-rw-r--   0        0        0     8238 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/qlat_utils/lat_io.py
--rw-rw-r--   0        0        0      200 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/qlat_utils/meson.build
--rw-rw-r--   0        0        0     5079 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/qlat_utils/parallel.py
--rw-rw-r--   0        0        0     2254 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/qlat_utils/qar.py
--rw-rw-r--   0        0        0     9534 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/qlat_utils/qplot.py
--rw-rw-r--   0        0        0     1624 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/qlat_utils/rng_state.py
--rw-rw-r--   0        0        0     3038 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/qlat_utils/timer.py
--rw-rw-r--   0        0        0     2599 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/qlat_utils/utils.py
--rw-rw-r--   0        0        0     4107 1970-01-01 00:00:00.000000 qlat_utils-0.8/pylib/qlat_utils/utils_io.py
--rw-rw-r--   0        0        0      387 1970-01-01 00:00:00.000000 qlat_utils-0.8/pyproject.toml
--rw-r--r--   0        0        0      275 1970-01-01 00:00:00.000000 qlat_utils-0.8/PKG-INFO
+-rw-rw-r--   0        0        0    35092 1970-01-01 00:00:00.000000 qlat_utils-0.9/LICENSE
+-rw-rw-r--   0        0        0       34 1970-01-01 00:00:00.000000 qlat_utils-0.9/README.md
+-rwxrwxr-x   0        0        0      356 1970-01-01 00:00:00.000000 qlat_utils-0.9/bin/crc32
+-rwxrwxr-x   0        0        0      267 1970-01-01 00:00:00.000000 qlat_utils-0.9/bin/lat-io-diff
+-rwxrwxr-x   0        0        0      207 1970-01-01 00:00:00.000000 qlat_utils-0.9/bin/lat-io-glimpse
+-rwxrwxr-x   0        0        0      257 1970-01-01 00:00:00.000000 qlat_utils-0.9/bin/pickle-glimpse
+-rwxrwxr-x   0        0        0     4070 1970-01-01 00:00:00.000000 qlat_utils-0.9/bin/qar
+-rwxrwxr-x   0        0        0     1096 1970-01-01 00:00:00.000000 qlat_utils-0.9/bin/qar-glimpse
+-rwxrwxr-x   0        0        0       98 1970-01-01 00:00:00.000000 qlat_utils-0.9/bin/qlat-utils-include
+-rw-rw-r--   0        0        0       55 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/meson.build
+-rw-rw-r--   0        0        0     1550 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/array.h
+-rw-rw-r--   0        0        0     2425 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/assert.h
+-rw-rw-r--   0        0        0     4497 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/cache.h
+-rw-rw-r--   0        0        0      986 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/compatible-endian.h
+-rw-r--r--   0        0        0      207 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/compatible-omp.h
+-rw-rw-r--   0        0        0     1061 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/complex.h
+-rw-rw-r--   0        0        0       43 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/config.h
+-rw-rw-r--   0        0        0     3145 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/core.h
+-rw-r--r--   0        0        0     4350 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/crc32.h
+-rw-rw-r--   0        0        0      943 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/eigen.h
+-rw-rw-r--   0        0        0     3317 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/handle.h
+-rw-rw-r--   0        0        0    16603 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/lat-io.h
+-rw-rw-r--   0        0        0      920 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/meson.build
+-rw-rw-r--   0        0        0     8389 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/py_convert.h
+-rw-rw-r--   0        0        0     4990 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/qacc-func.h
+-rw-rw-r--   0        0        0      480 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/qacc.h
+-rw-rw-r--   0        0        0    22570 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/qar-cache.h
+-rw-rw-r--   0        0        0    33580 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/qar.h
+-rw-rw-r--   0        0        0     8946 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/qutils-extra.h
+-rw-rw-r--   0        0        0    10976 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/qutils-io.h
+-rw-rw-r--   0        0        0    14507 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/qutils-vec.h
+-rw-rw-r--   0        0        0     2769 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/qutils.h
+-rw-r--r--   0        0        0    10128 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/rng-state.h
+-rw-r--r--   0        0        0    14882 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/sha256.h
+-rw-rw-r--   0        0        0     8144 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/show.h
+-rw-r--r--   0        0        0     2254 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/sprng-sha256.h
+-rw-rw-r--   0        0        0    22900 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/timer.h
+-rw-rw-r--   0        0        0    13450 1970-01-01 00:00:00.000000 qlat_utils-0.9/include/qlat-utils/vector.h
+-rw-rw-r--   0        0        0      899 1970-01-01 00:00:00.000000 qlat_utils-0.9/meson.build
+-rw-rw-r--   0        0        0     2466 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/cqlat_utils/exports.h
+-rw-rw-r--   0        0        0     7602 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/cqlat_utils/lat-io.cpp
+-rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/cqlat_utils/lib.cpp
+-rw-rw-r--   0        0        0     2208 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/cqlat_utils/lib.h
+-rw-rw-r--   0        0        0      369 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/cqlat_utils/meson.build
+-rw-rw-r--   0        0        0     3280 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/cqlat_utils/qar.cpp
+-rw-rw-r--   0        0        0     1654 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/cqlat_utils/rng-state.cpp
+-rw-r--r--   0        0        0     3358 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/cqlat_utils/timer.cpp
+-rwxr-xr-x   0        0        0      766 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/cqlat_utils/update.sh
+-rw-rw-r--   0        0        0     6082 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/cqlat_utils/utils-io.cpp
+-rw-rw-r--   0        0        0     1018 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/cqlat_utils/utils.cpp
+-rw-rw-r--   0        0        0       43 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/meson.build
+-rw-rw-r--   0        0        0       67 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/__init__.pxd
+-rw-rw-r--   0        0        0      414 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/__init__.py
+-rw-rw-r--   0        0        0      183 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/c.py
+-rw-rw-r--   0        0        0     1886 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/cache.py
+-rw-rw-r--   0        0        0      842 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/cp.pyx
+-rw-rw-r--   0        0        0    16937 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/data.py
+-rw-rw-r--   0        0        0      437 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/get_include_dir.py
+-rw-rw-r--   0        0        0     8237 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/lat_io.py
+-rw-rw-r--   0        0        0      802 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/meson.build
+-rw-rw-r--   0        0        0     5079 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/parallel.py
+-rw-rw-r--   0        0        0     2248 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/qar.py
+-rw-rw-r--   0        0        0     9973 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/qplot.py
+-rw-rw-r--   0        0        0     1623 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/rng_state.py
+-rw-rw-r--   0        0        0      360 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/timer.pxd
+-rw-rw-r--   0        0        0     2212 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/timer.py
+-rw-rw-r--   0        0        0      123 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/utils-io.cpp
+-rw-rw-r--   0        0        0       58 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/utils-io.h
+-rw-rw-r--   0        0        0     2598 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/utils.py
+-rw-rw-r--   0        0        0       65 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/utils_io.pxd
+-rw-rw-r--   0        0        0     4099 1970-01-01 00:00:00.000000 qlat_utils-0.9/pylib/qlat_utils/utils_io.py
+-rw-rw-r--   0        0        0      387 1970-01-01 00:00:00.000000 qlat_utils-0.9/pyproject.toml
+-rw-r--r--   0        0        0      275 1970-01-01 00:00:00.000000 qlat_utils-0.9/PKG-INFO
```

### Comparing `qlat_utils-0.8/LICENSE` & `qlat_utils-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/bin/qar` & `qlat_utils-0.9/bin/qar`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/bin/qar-glimpse` & `qlat_utils-0.9/bin/qar-glimpse`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/array.h` & `qlat_utils-0.9/include/qlat-utils/array.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/assert.h` & `qlat_utils-0.9/include/qlat-utils/assert.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/cache.h` & `qlat_utils-0.9/include/qlat-utils/cache.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/compatible-endian.h` & `qlat_utils-0.9/include/qlat-utils/compatible-endian.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/complex.h` & `qlat_utils-0.9/include/qlat-utils/complex.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/core.h` & `qlat_utils-0.9/include/qlat-utils/core.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/crc32.h` & `qlat_utils-0.9/include/qlat-utils/crc32.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/eigen.h` & `qlat_utils-0.9/include/qlat-utils/eigen.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/handle.h` & `qlat_utils-0.9/include/qlat-utils/handle.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/lat-io.h` & `qlat_utils-0.9/include/qlat-utils/lat-io.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/meson.build` & `qlat_utils-0.9/include/qlat-utils/meson.build`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/py_convert.h` & `qlat_utils-0.9/include/qlat-utils/py_convert.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/qacc-func.h` & `qlat_utils-0.9/include/qlat-utils/qacc-func.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/qar-cache.h` & `qlat_utils-0.9/include/qlat-utils/qar-cache.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/qar.h` & `qlat_utils-0.9/include/qlat-utils/qar.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/qutils-extra.h` & `qlat_utils-0.9/include/qlat-utils/qutils-extra.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/qutils-io.h` & `qlat_utils-0.9/include/qlat-utils/qutils-io.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/qutils-vec.h` & `qlat_utils-0.9/include/qlat-utils/qutils-vec.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/qutils.h` & `qlat_utils-0.9/include/qlat-utils/qutils.h`

 * *Files 9% similar despite different names*

```diff
@@ -106,28 +106,14 @@
 template <class M>
 void clear(std::vector<M>& vec)
 {
   std::vector<M> empty;
   std::swap(empty, vec);
 }
 
-template <class K>
-bool has(const std::set<K>& m, const K& key)
-{
-  typename std::set<K>::const_iterator it = m.find(key);
-  return it != m.end();
-}
-
-template <class K, class M>
-bool has(const std::map<K, M>& m, const K& key)
-{
-  typename std::map<K, M>::const_iterator it = m.find(key);
-  return it != m.end();
-}
-
 // -------------------
 
 qacc bool is_big_endian()
 {
 #if defined(__BYTE_ORDER) && (__BYTE_ORDER != 0) && \
     (__BYTE_ORDER == __BIG_ENDIAN)
   return true;
```

### Comparing `qlat_utils-0.8/include/qlat-utils/rng-state.h` & `qlat_utils-0.9/include/qlat-utils/rng-state.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/sha256.h` & `qlat_utils-0.9/include/qlat-utils/sha256.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/show.h` & `qlat_utils-0.9/include/qlat-utils/show.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/sprng-sha256.h` & `qlat_utils-0.9/include/qlat-utils/sprng-sha256.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/include/qlat-utils/timer.h` & `qlat_utils-0.9/include/qlat-utils/timer.h`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 #include <cstdarg>
 #include <cstdio>
 #include <cstdlib>
 #include <cstring>
 #include <cmath>
 #include <string>
 #include <vector>
+#include <map>
+#include <set>
 
 #ifdef USE_PAPI
 #include <papi.h>
 #endif
 
 #ifdef _OPENMP
 #include <omp.h>
@@ -279,14 +281,28 @@
   for (int i = 0; i < n_threads; i++) {
     flops += flopses[i];
   }
 #endif
   return flops;
 }
 
+template <class K>
+bool has(const std::set<K>& m, const K& key)
+{
+  typename std::set<K>::const_iterator it = m.find(key);
+  return it != m.end();
+}
+
+template <class K, class M>
+bool has(const std::map<K, M>& m, const K& key)
+{
+  typename std::map<K, M>::const_iterator it = m.find(key);
+  return it != m.end();
+}
+
 API inline void initialize_papi()
 {
 #ifdef USE_PAPI
   static bool initialized = false;
   if (initialized) {
     return;
   }
@@ -302,14 +318,16 @@
   std::string fname;
   double dtime;
   double accumulated_time;
   long long dflops;
   long long accumulated_flops;
   int call_times;
   //
+  TimerInfo() { init(); }
+  //
   void init()
   {
     fname = "Unknown";
     reset();
   }
   //
   void reset()
@@ -391,37 +409,45 @@
   return p1->accumulated_time < p2->accumulated_time;
 }
 
 struct API Timer {
   const char* cname;
   long info_index;
   bool is_using_total_flops;
-  long isRunning;
+  long is_running;
   double start_time;
   double stop_time;
   long long start_flops;
   long long stop_flops;
   long long flops;
   //
+  API static std::map<std::string, long>& get_timer_info_index_map()
+  {
+    static std::map<std::string, long> timer_info_index_map;
+    return timer_info_index_map;
+  }
+  //
   API static std::vector<TimerInfo>& get_timer_database()
   {
     static std::vector<TimerInfo> timer_database;
     return timer_database;
   }
   //
   API static std::vector<std::vector<TimerInfo> >& get_timer_database_history()
   {
     static std::vector<std::vector<TimerInfo> > timer_database_history;
     return timer_database_history;
   }
+  //
   API static std::vector<double>& get_start_time_history()
   {
     static std::vector<double> history;
     return history;
   }
+  //
   API static std::vector<long>&
   get_max_call_times_for_always_show_info_history()
   {
     static std::vector<long> history;
     return history;
   }
   //
@@ -564,54 +590,52 @@
   void init()
   {
     cname = "Timer";
     is_using_total_flops = true;
     get_start_time();
     initialize_papi();
     info_index = -1;
-    isRunning = 0;
+    is_running = 0;
   }
   void init(const std::string& fname_str)
   {
+    std::map<std::string, long>& tiim = get_timer_info_index_map();
     std::vector<TimerInfo>& tdb = get_timer_database();
-    const long size = tdb.size();
-    for (long i = 0; i < size; i++) {
-      if (fname_str == tdb[i].fname) {
-        info_index = i;
-        return;
-      }
+    if (has(tiim, fname_str)) {
+      info_index = tiim[fname_str];
+    } else {
+      info_index = tdb.size();
+      tiim[fname_str] = info_index;
+      TimerInfo info;
+      info.fname = fname_str;
+      tdb.push_back(info);
     }
-    info_index = tdb.size();
-    TimerInfo info;
-    tdb.push_back(info);
-    tdb[info_index].init();
-    tdb[info_index].fname = fname_str;
   }
   void init(const std::string& cname_str, const std::string& fname_str)
   {
     std::string fname = "";
     fname += cname_str;
     fname += "::";
     fname += fname_str;
     init(fname);
   }
   //
   void start(bool verbose = false)
   {
     get_timer_stack().push_back(info_index);
-    if (isRunning > 0) {
-      isRunning += 1;
+    if (is_running > 0) {
+      is_running += 1;
       return;
-    } else if (isRunning == 0) {
-      isRunning = 1;
+    } else if (is_running == 0) {
+      is_running = 1;
     } else {
       TimerInfo& info = get_timer_database()[info_index];
       info.show_avg_always("debug", max_function_name_length_shown());
-      displayln(ssprintf("%s::%s ERROR: isRunning=%d", cname,
-                         info.fname.c_str(), isRunning));
+      displayln(ssprintf("%s::%s ERROR: is_running=%d", cname,
+                         info.fname.c_str(), is_running));
       Timer::display_stack();
       qassert(false);
     }
     TimerInfo& info = get_timer_database()[info_index];
     info.call_times++;
     if (verbose_level() > 0) {
       if (verbose ||
@@ -634,23 +658,23 @@
     if (not(t_stack.back() == info_index)) {
       displayln(ssprintf("%s::%s ERROR: stack is corrupted", cname,
                          info.fname.c_str()));
       Timer::display_stack();
       qassert(false);
     }
     t_stack.pop_back();
-    if (isRunning <= 0) {
+    if (is_running <= 0) {
       info.show_avg_always("debug", max_function_name_length_shown());
-      displayln(ssprintf("%s::%s ERROR: isRunning=%d", cname,
-                         info.fname.c_str(), isRunning));
+      displayln(ssprintf("%s::%s ERROR: is_running=%d", cname,
+                         info.fname.c_str(), is_running));
       Timer::display_stack();
       qassert(false);
     }
-    isRunning -= 1;
-    if (isRunning != 0) {
+    is_running -= 1;
+    if (is_running != 0) {
       return;
     }
     stop_time = get_time();
     if (is_using_total_flops) {
       stop_flops = get_total_flops();
     } else {
       stop_flops = start_flops + flops;
@@ -690,40 +714,40 @@
       timer_noflop.start();
       timer_test.start();
       timer_test.stop();
       timer_noflop.stop();
     }
   }
   //
-  API static void display(const std::string& str = "")
+  API static void display(const std::string& tag = "")
   {
     double total_time = get_total_time();
     const std::vector<TimerInfo>& tdb = get_timer_database();
     const std::vector<std::vector<TimerInfo> >& tdb_history =
         get_timer_database_history();
     std::vector<const TimerInfo*> db;
     const long tdbsize = tdb.size();
     for (long i = 0; i < tdbsize; i++) {
       db.push_back(&tdb[i]);
     }
     std::sort(db.begin(), db.end(), compare_time_info_p);
     displayln_info(ssprintf(
         "Timer::display-start: %s (level=%ld) fname : time%% number of calls; "
         "Avg,Tot sec; Avg,Tot flops; Gflops",
-        str.c_str(), (long)tdb_history.size()));
+        tag.c_str(), (long)tdb_history.size()));
     const long dbsize = db.size();
     for (long i = 0; i < dbsize; i++) {
       if (db[i]->call_times > 0) {
         db[i]->show_avg("display", max_function_name_length_shown());
       }
     }
     displayln_info(ssprintf(
         "Timer::display-end:   %s (level=%ld) --------------------- total %.4E "
         "sec ----------------------",
-        str.c_str(), (long)tdb_history.size(), total_time));
+        tag.c_str(), (long)tdb_history.size(), total_time));
   }
   //
   API static void autodisplay(const double time)
   {
     static double last_time = get_start_time();
     if (time - last_time > minimum_autodisplay_interval()) {
       last_time = time;
```

### Comparing `qlat_utils-0.8/include/qlat-utils/vector.h` & `qlat_utils-0.9/include/qlat-utils/vector.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/meson.build` & `qlat_utils-0.9/meson.build`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-project('qlat-utils', 'cpp',
-  version: '0.8',
+project('qlat-utils', 'cpp', 'cython',
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
 
 omp = dependency('openmp').as_system()
 zlib = dependency('zlib').as_system()
```

### Comparing `qlat_utils-0.8/pylib/cqlat_utils/exports.h` & `qlat_utils-0.9/pylib/cqlat_utils/exports.h`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 EXPORT_FUNCTION(check_all_files_crc32_info)
 EXPORT_FUNCTION(clear_all_caches)
 EXPORT_FUNCTION(compute_crc32)
 EXPORT_FUNCTION(displayln_malloc_stats)
 EXPORT_FUNCTION(does_file_exist)
 EXPORT_FUNCTION(does_file_exist_qar)
 EXPORT_FUNCTION(does_regular_file_exist_qar)
-EXPORT_FUNCTION(flush)
 EXPORT_FUNCTION(free_lat_data)
 EXPORT_FUNCTION(free_rng)
 EXPORT_FUNCTION(free_timer)
 EXPORT_FUNCTION(g_rand_gen)
 EXPORT_FUNCTION(get_actual_start_time)
 EXPORT_FUNCTION(get_all_caches_info)
 EXPORT_FUNCTION(get_dim_indices_lat_data)
@@ -65,15 +64,14 @@
 EXPORT_FUNCTION(set_rng)
 EXPORT_FUNCTION(set_sub_lat_data)
 EXPORT_FUNCTION(set_zero_lat_data)
 EXPORT_FUNCTION(show_lat_data)
 EXPORT_FUNCTION(start_timer)
 EXPORT_FUNCTION(stop_timer)
 EXPORT_FUNCTION(timer_autodisplay)
-EXPORT_FUNCTION(timer_display)
 EXPORT_FUNCTION(timer_display_stack)
 EXPORT_FUNCTION(timer_display_stack_always)
 EXPORT_FUNCTION(timer_fork)
 EXPORT_FUNCTION(timer_merge)
 EXPORT_FUNCTION(timer_reset)
 EXPORT_FUNCTION(u_rand_gen)
 EXPORT_FUNCTION(verbose_level)
```

### Comparing `qlat_utils-0.8/pylib/cqlat_utils/lat-io.cpp` & `qlat_utils-0.9/pylib/cqlat_utils/lat-io.cpp`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/pylib/cqlat_utils/lib.cpp` & `qlat_utils-0.9/pylib/cqlat_utils/lib.cpp`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/pylib/cqlat_utils/lib.h` & `qlat_utils-0.9/pylib/cqlat_utils/lib.h`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/pylib/cqlat_utils/qar.cpp` & `qlat_utils-0.9/pylib/cqlat_utils/qar.cpp`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/pylib/cqlat_utils/rng-state.cpp` & `qlat_utils-0.9/pylib/cqlat_utils/rng-state.cpp`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/pylib/cqlat_utils/timer.cpp` & `qlat_utils-0.9/pylib/cqlat_utils/timer.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -61,28 +61,14 @@
     return NULL;
   }
   Timer& timer = py_convert_type<Timer>(p_timer);
   timer.flops = flops;
   Py_RETURN_NONE;
 })
 
-EXPORT(timer_display, {
-  using namespace qlat;
-  PyObject* p_str = NULL;
-  if (!PyArg_ParseTuple(args, "|O", &p_str)) {
-    return NULL;
-  }
-  std::string str;
-  if (p_str != NULL) {
-    py_convert(str, p_str);
-  }
-  Timer::display(str);
-  Py_RETURN_NONE;
-})
-
 EXPORT(timer_autodisplay, {
   using namespace qlat;
   Timer::autodisplay();
   Py_RETURN_NONE;
 })
 
 EXPORT(timer_reset, {
```

### Comparing `qlat_utils-0.8/pylib/cqlat_utils/update.sh` & `qlat_utils-0.9/pylib/cqlat_utils/update.sh`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/pylib/cqlat_utils/utils-io.cpp` & `qlat_utils-0.9/pylib/cqlat_utils/utils-io.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 #include "lib.h"
 
 #include <qlat-utils/qar-cache.h>
 
-EXPORT(flush, {
-  using namespace qlat;
-  fflush(get_output_file());
-  Py_RETURN_NONE;
-})
-
 EXPORT(qremove, {
   using namespace qlat;
   PyObject* p_path = NULL;
   if (!PyArg_ParseTuple(args, "O", &p_path)) {
     return NULL;
   }
   const std::string path = py_convert_data<std::string>(p_path);
```

### Comparing `qlat_utils-0.8/pylib/cqlat_utils/utils.cpp` & `qlat_utils-0.9/pylib/cqlat_utils/utils.cpp`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/pylib/qlat_utils/cache.py` & `qlat_utils-0.9/pylib/qlat_utils/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from qlat_utils.timer import *
 
-import qlat_utils.cu as cu
+import qlat_utils.c as cu
 
 # Usage:
 # cache_x = q.mk_cache("xx")
 # q.clean_cache(cache_x)
 # cache_x[key] = value
 # val = cache_x[key]
 # key in cache_x
```

### Comparing `qlat_utils-0.8/pylib/qlat_utils/data.py` & `qlat_utils-0.9/pylib/qlat_utils/data.py`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/pylib/qlat_utils/lat_io.py` & `qlat_utils-0.9/pylib/qlat_utils/lat_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import qlat_utils.cu as cu
+import qlat_utils.c as cu
 
 import numpy as np
 
 from qlat_utils.utils_io import *
 
 class LatData:
```

### Comparing `qlat_utils-0.8/pylib/qlat_utils/parallel.py` & `qlat_utils-0.9/pylib/qlat_utils/parallel.py`

 * *Files identical despite different names*

### Comparing `qlat_utils-0.8/pylib/qlat_utils/qar.py` & `qlat_utils-0.9/pylib/qlat_utils/qar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import qlat_utils.cu as cu
+import qlat_utils.c as cu
 
-from qlat_utils.cu import get_qar_multi_vol_max_size
-from qlat_utils.cu import does_regular_file_exist_qar
-from qlat_utils.cu import does_file_exist_qar
-from qlat_utils.cu import qcat
-from qlat_utils.cu import qcat_bytes
+from qlat_utils.c import get_qar_multi_vol_max_size
+from qlat_utils.c import does_regular_file_exist_qar
+from qlat_utils.c import does_file_exist_qar
+from qlat_utils.c import qcat
+from qlat_utils.c import qcat_bytes
 
 from qlat_utils.timer import *
 
 @timer
 def qar_create(path_qar, path_folder, *, is_remove_folder_after = False):
     return cu.qar_create(path_qar, path_folder, is_remove_folder_after)
```

### Comparing `qlat_utils-0.8/pylib/qlat_utils/qplot.py` & `qlat_utils-0.9/pylib/qlat_utils/qplot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+__all__ = [
+        'show_datatable', 'read_datatable',
+        'save_datatable', 'load_datatable',
+        'azip',
+        'plot_save', 'plot_view',
+        'gnuplot_png_density',
+        'plot_save_display_width',
+        'display_img',
+        ]
+
 import numpy as np
 import os
 import sys
 import shutil
 import tempfile
 import subprocess
 
@@ -205,15 +215,23 @@
 
 def display_img(fn, *, width = None):
     from IPython.display import HTML, display
     displayln_info(0, f"display_img: fn='{fn}'")
     show_width = ""
     if width is not None:
         show_width = f"width='{width}'"
-    display(HTML(data = f"<img src='{fn}' {show_width} />"))
+    try:
+      import google.colab
+      is_in_colab = True
+    except:
+      is_in_colab = False
+    if not is_in_colab:
+        display(HTML(data = f"<img src='{fn}' {show_width} />"))
+    else:
+        display(Image(filename = fn, width = width))
 
 plot_save_display_width = None
 
 @timer
 def plot_save(
         fn = None,
         dts = None,
```

### Comparing `qlat_utils-0.8/pylib/qlat_utils/rng_state.py` & `qlat_utils-0.9/pylib/qlat_utils/rng_state.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import qlat_utils.cu as cu
+import qlat_utils.c as cu
 
 class RngState:
 
 	# self.cdata
 
     def __init__(self, x = None, y = None):
         if x is None:
```

### Comparing `qlat_utils-0.8/pylib/qlat_utils/timer.py` & `qlat_utils-0.9/pylib/qlat_utils/timer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-import qlat_utils.cu as cu
+import qlat_utils.c as cu
 
-from qlat_utils.cu import get_id_node, get_num_node
-from qlat_utils.cu import timer_reset, timer_fork, timer_merge
-from qlat_utils.cu import verbose_level
-from qlat_utils.cu import get_actual_start_time, get_start_time, get_time
-from qlat_utils.cu import flush
+from qlat_utils.c import get_id_node, get_num_node
+from qlat_utils.c import timer_reset, timer_fork, timer_merge
+from qlat_utils.c import verbose_level
+from qlat_utils.c import get_actual_start_time, get_start_time, get_time
+from qlat_utils.c import flush
+from qlat_utils.c import timer, timer_verbose
+from qlat_utils.c import timer_display
 
 import functools
 
 timer_total_flops = {}
 
 def acc_timer_flops(fname, flops):
     if fname in timer_total_flops:
@@ -47,42 +49,14 @@
         cu.stop_timer(self, is_verbose)
 
     def set_flops(self, flops):
         if self.cdata is None:
             return
         cu.set_flops_timer(self, flops)
 
-def timer(func):
-    fname = "py:" + func.__name__
-    qtimer = Timer(fname)
-    @functools.wraps(func)
-    def qtimer_func(*args, **kwargs):
-        qtimer.start()
-        start_flops = timer_total_flops[fname]
-        ret = func(*args, **kwargs)
-        stop_flops = timer_total_flops[fname]
-        qtimer.set_flops(stop_flops - start_flops)
-        qtimer.stop()
-        return ret
-    return qtimer_func
-
-def timer_verbose(func):
-    fname = "py:" + func.__name__
-    qtimer = Timer(fname, True)
-    @functools.wraps(func)
-    def qtimer_func(*args, **kwargs):
-        qtimer.start()
-        start_flops = timer_total_flops[fname]
-        ret = func(*args, **kwargs)
-        stop_flops = timer_total_flops[fname]
-        qtimer.set_flops(stop_flops - start_flops)
-        qtimer.stop()
-        return ret
-    return qtimer_func
-
 def displayln(level, *args):
     if isinstance(level, int):
         if level <= verbose_level():
             print(*args, flush=True)
     else:
         print(level, *args, flush=True)
 
@@ -97,18 +71,14 @@
 
 def get_total_time():
     return get_time() - get_start_time()
 
 def get_actual_total_time():
     return get_time() - get_actual_start_time()
 
-def timer_display(*params):
-    cu.timer_display(*params)
-    flush()
-
 def timer_autodisplay():
     cu.timer_autodisplay()
     flush()
 
 def timer_display_stack():
     cu.timer_display_stack()
     flush()
```

### Comparing `qlat_utils-0.8/pylib/qlat_utils/utils.py` & `qlat_utils-0.9/pylib/qlat_utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import qlat_utils.cu as cu
+import qlat_utils.c as cu
 
 from qlat_utils.cache import *
 from qlat_utils.rng_state import *
 
 import math
 import sys
 import os
```

### Comparing `qlat_utils-0.8/pylib/qlat_utils/utils_io.py` & `qlat_utils-0.9/pylib/qlat_utils/utils_io.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import qlat_utils.cu as cu
+import qlat_utils.c as cu
 
 import os
 import pickle
 
-from qlat_utils.cu import qremove
-from qlat_utils.cu import qremove_all
-from qlat_utils.cu import qmkdir, qmkdir_info
-from qlat_utils.cu import does_file_exist
-from qlat_utils.cu import is_directory
-from qlat_utils.cu import is_regular_file
-from qlat_utils.cu import qrename, qrename_info
-from qlat_utils.cu import qls
-from qlat_utils.cu import qls_all
+from qlat_utils.c import qremove
+from qlat_utils.c import qremove_all
+from qlat_utils.c import qmkdir, qmkdir_info
+from qlat_utils.c import does_file_exist
+from qlat_utils.c import is_directory
+from qlat_utils.c import is_regular_file
+from qlat_utils.c import qrename, qrename_info
+from qlat_utils.c import qls
+from qlat_utils.c import qls_all
 
 from qlat_utils.qar import *
 
 @timer
 def qmkdirs(path):
     os.makedirs(path, exist_ok=True)
 
@@ -109,21 +109,21 @@
         save_pickle_obj(obj, path)
     else:
         obj = load_pickle_obj(path)
     return obj
 
 def qremove_info(path):
     if get_num_node() != 1:
-        import cqlat as c
+        import qlat.c as c
         return c.qremove_info(path)
     return qremove(path)
 
 def qremove_all_info(path):
     if get_num_node() != 1:
-        import cqlat as c
+        import qlat.c as c
         return c.qremove_all_info(path)
     return qremove_all(path)
 
 def qmkdir_sync_node(path):
     if get_num_node() != 1:
         import cqlat as c
         return c.qmkdir_sync_node(path)
```

