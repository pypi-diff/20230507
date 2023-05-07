# Comparing `tmp/bw2calc-2.0.dev7.tar.gz` & `tmp/bw2calc-2.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw2calc-2.0.dev7.tar", last modified: Sun May 22 10:45:42 2022, max compression
+gzip compressed data, was "bw2calc-2.0.dev8.tar", last modified: Tue Jun 28 06:19:14 2022, max compression
```

## Comparing `bw2calc-2.0.dev7.tar` & `bw2calc-2.0.dev8.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-05-22 10:45:42.734696 bw2calc-2.0.dev7/
--rw-r--r--   0 cmutel     (501) staff       (20)     1203 2022-02-07 18:55:26.000000 bw2calc-2.0.dev7/.gitignore
--rw-r--r--   0 cmutel     (501) staff       (20)    12464 2022-05-22 10:45:16.000000 bw2calc-2.0.dev7/CHANGES.md
--rw-r--r--   0 cmutel     (501) staff       (20)     3220 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/CODE_OF_CONDUCT.md
--rw-r--r--   0 cmutel     (501) staff       (20)     1474 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/LICENSE.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       86 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/MANIFEST.in
--rw-r--r--   0 cmutel     (501) staff       (20)     2093 2022-05-22 10:45:42.734091 bw2calc-2.0.dev7/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)      989 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/README.rst
--rw-r--r--   0 cmutel     (501) staff       (20)     3633 2022-04-29 20:50:58.000000 bw2calc-2.0.dev7/azure-pipelines.yml
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-05-22 10:45:42.634038 bw2calc-2.0.dev7/bw2calc/
--rw-r--r--   0 cmutel     (501) staff       (20)     1640 2022-05-03 08:10:09.000000 bw2calc-2.0.dev7/bw2calc/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)      813 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/bw2calc/dense_lca.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3625 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/bw2calc/dictionary_manager.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1457 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/bw2calc/errors.py
--rw-r--r--   0 cmutel     (501) staff       (20)     9118 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/bw2calc/graph_traversal.py
--rw-r--r--   0 cmutel     (501) staff       (20)    25473 2022-05-22 10:38:05.000000 bw2calc-2.0.dev7/bw2calc/lca.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1500 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/bw2calc/least_squares.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3817 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/bw2calc/log_utils.py
--rw-r--r--   0 cmutel     (501) staff       (20)     7327 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/bw2calc/monte_carlo.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2687 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/bw2calc/multi_lca.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3466 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/bw2calc/single_value_diagonal_matrix.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2331 2022-05-22 10:39:02.000000 bw2calc-2.0.dev7/bw2calc/utils.py
--rw-r--r--   0 cmutel     (501) staff       (20)       25 2022-05-22 10:45:22.000000 bw2calc-2.0.dev7/bw2calc/version.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-05-22 10:45:42.638822 bw2calc-2.0.dev7/bw2calc.egg-info/
--rw-r--r--   0 cmutel     (501) staff       (20)     2093 2022-05-22 10:45:41.000000 bw2calc-2.0.dev7/bw2calc.egg-info/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)     3290 2022-05-22 10:45:42.000000 bw2calc-2.0.dev7/bw2calc.egg-info/SOURCES.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2022-05-22 10:45:41.000000 bw2calc-2.0.dev7/bw2calc.egg-info/dependency_links.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       46 2022-05-22 10:45:42.000000 bw2calc-2.0.dev7/bw2calc.egg-info/requires.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        8 2022-05-22 10:45:42.000000 bw2calc-2.0.dev7/bw2calc.egg-info/top_level.txt
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-05-22 10:45:42.641133 bw2calc-2.0.dev7/dev/
--rw-r--r--   0 cmutel     (501) staff       (20)    25205 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/dev/lca_old.py
--rw-r--r--   0 cmutel     (501) staff       (20)       55 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/pytest.ini
--rw-r--r--   0 cmutel     (501) staff       (20)       92 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/requirements-test.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       46 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/requirements.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       38 2022-05-22 10:45:42.734968 bw2calc-2.0.dev7/setup.cfg
--rw-r--r--   0 cmutel     (501) staff       (20)     1471 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/setup.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-05-22 10:45:42.661737 bw2calc-2.0.dev7/tests/
--rw-r--r--   0 cmutel     (501) staff       (20)       24 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2889 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/dict_man.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-05-22 10:45:42.677639 bw2calc-2.0.dev7/tests/fixtures/
--rw-r--r--   0 cmutel     (501) staff       (20)        0 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2135 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/array_sequential.zip
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-05-22 10:45:42.682504 bw2calc-2.0.dev7/tests/fixtures/basic_fixture/
--rw-r--r--   0 cmutel     (501) staff       (20)      136 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/basic_fixture/biosphere.data.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      136 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/basic_fixture/biosphere.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)     2914 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/basic_fixture/datapackage.json
--rw-r--r--   0 cmutel     (501) staff       (20)      136 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/basic_fixture/eb-characterization.data.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      136 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/basic_fixture/eb-characterization.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      152 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/basic_fixture/technosphere.data.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      131 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/basic_fixture/technosphere.flip.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      152 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/basic_fixture/technosphere.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)     2120 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/basic_fixture.zip
--rw-r--r--   0 cmutel     (501) staff       (20)     2565 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/bw2io_example_db.zip
--rw-r--r--   0 cmutel     (501) staff       (20)      201 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/bw2io_example_db_mapping.json
--rw-r--r--   0 cmutel     (501) staff       (20)    11301 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/create_fixtures.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-05-22 10:45:42.685804 bw2calc-2.0.dev7/tests/fixtures/empty_biosphere/
--rw-r--r--   0 cmutel     (501) staff       (20)     1435 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/empty_biosphere/biosphere.zip
--rw-r--r--   0 cmutel     (501) staff       (20)       59 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/empty_biosphere/mapping.json
--rw-r--r--   0 cmutel     (501) staff       (20)      848 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/empty_biosphere/method.zip
--rw-r--r--   0 cmutel     (501) staff       (20)     1534 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/empty_biosphere/test_db.zip
--rw-r--r--   0 cmutel     (501) staff       (20)     1703 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/empty_biosphere.zip
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-05-22 10:45:42.691341 bw2calc-2.0.dev7/tests/fixtures/example_db/
--rw-r--r--   0 cmutel     (501) staff       (20)     1734 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/example_db/example_db.zip
--rw-r--r--   0 cmutel     (501) staff       (20)      854 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/example_db/ipcc.zip
--rw-r--r--   0 cmutel     (501) staff       (20)      449 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/example_db/mapping.json
--rw-r--r--   0 cmutel     (501) staff       (20)     1059 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/ipcc_simple.zip
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-05-22 10:45:42.694779 bw2calc-2.0.dev7/tests/fixtures/mc_basic/
--rw-r--r--   0 cmutel     (501) staff       (20)     1435 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/mc_basic/biosphere.zip
--rw-r--r--   0 cmutel     (501) staff       (20)       90 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/mc_basic/mapping.json
--rw-r--r--   0 cmutel     (501) staff       (20)      855 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/mc_basic/method.zip
--rw-r--r--   0 cmutel     (501) staff       (20)     1604 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/mc_basic/test_db.zip
--rw-r--r--   0 cmutel     (501) staff       (20)     3137 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/mc_basic.zip
--rw-r--r--   0 cmutel     (501) staff       (20)     2083 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/mc_complete.zip
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-05-22 10:45:42.697024 bw2calc-2.0.dev7/tests/fixtures/mc_saop/
--rw-r--r--   0 cmutel     (501) staff       (20)     1436 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/mc_saop/biosphere.zip
--rw-r--r--   0 cmutel     (501) staff       (20)       45 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/mc_saop/mapping.json
--rw-r--r--   0 cmutel     (501) staff       (20)     1559 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/mc_saop/saop.zip
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-05-22 10:45:42.702392 bw2calc-2.0.dev7/tests/fixtures/multi/
--rw-r--r--   0 cmutel     (501) staff       (20)     1712 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/multi/datapackage.json
--rw-r--r--   0 cmutel     (501) staff       (20)      226 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/multi/multi.0.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      176 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/multi/multi.0.samples.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      240 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/multi/multi.1.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      200 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/multi/multi.1.samples.npy
--rw-r--r--   0 cmutel     (501) staff       (20)     7444 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/presamples_basic.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-05-22 10:45:42.709896 bw2calc-2.0.dev7/tests/fixtures/seq/
--rw-r--r--   0 cmutel     (501) staff       (20)     1710 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/seq/datapackage.json
--rw-r--r--   0 cmutel     (501) staff       (20)      226 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/seq/seq.0.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      176 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/seq/seq.0.samples.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      240 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/seq/seq.1.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      200 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/seq/seq.1.samples.npy
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-05-22 10:45:42.712650 bw2calc-2.0.dev7/tests/fixtures/single-matrix/
--rw-r--r--   0 cmutel     (501) staff       (20)    15057 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/single-matrix/Test fixture.ipynb
--rw-r--r--   0 cmutel     (501) staff       (20)     2491 2022-04-29 18:08:40.000000 bw2calc-2.0.dev7/tests/fixtures/single-matrix/generate_fixture.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1056 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/single-matrix/sm-fixture.tar.bz2
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-05-22 10:45:42.722989 bw2calc-2.0.dev7/tests/fixtures/single-sample/
--rw-r--r--   0 cmutel     (501) staff       (20)     2475 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/single-sample/datapackage.json
--rw-r--r--   0 cmutel     (501) staff       (20)      226 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/single-sample/single-sample.0.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      144 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/single-sample/single-sample.0.samples.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      240 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/single-sample/single-sample.1.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      152 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/single-sample/single-sample.1.samples.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      136 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/single-sample/single-sample.2.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      136 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/single-sample/single-sample.2.samples.npy
--rw-r--r--   0 cmutel     (501) staff       (20)     1713 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/svdm.zip
--rw-r--r--   0 cmutel     (501) staff       (20)      968 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/fixtures/svdm2.zip
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-05-22 10:45:42.732795 bw2calc-2.0.dev7/tests/fixtures/unseeded/
--rw-r--r--   0 cmutel     (501) staff       (20)     1732 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/unseeded/datapackage.json
--rw-r--r--   0 cmutel     (501) staff       (20)      226 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/unseeded/unseeded.0.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      176 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/unseeded/unseeded.0.samples.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      240 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/unseeded/unseeded.1.indices.npy
--rw-r--r--   0 cmutel     (501) staff       (20)      200 2020-03-11 10:53:14.000000 bw2calc-2.0.dev7/tests/fixtures/unseeded/unseeded.1.samples.npy
--rw-r--r--   0 cmutel     (501) staff       (20)    48101 2022-05-22 10:43:45.000000 bw2calc-2.0.dev7/tests/lca.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3013 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/monte_carlo.py
--rw-r--r--   0 cmutel     (501) staff       (20)     8680 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/presamples.py
--rw-r--r--   0 cmutel     (501) staff       (20)      377 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/single_matrix.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3051 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/svdm.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1316 2022-04-01 11:27:21.000000 bw2calc-2.0.dev7/tests/utils.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-06-28 06:19:14.044063 bw2calc-2.0.dev8/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1203 2022-02-07 18:55:26.000000 bw2calc-2.0.dev8/.gitignore
+-rw-r--r--   0 cmutel     (501) staff       (20)    12695 2022-06-28 06:18:35.000000 bw2calc-2.0.dev8/CHANGES.md
+-rw-r--r--   0 cmutel     (501) staff       (20)     3220 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 cmutel     (501) staff       (20)     1474 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/LICENSE.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       86 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/MANIFEST.in
+-rw-r--r--   0 cmutel     (501) staff       (20)     2093 2022-06-28 06:19:14.043506 bw2calc-2.0.dev8/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)      989 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/README.rst
+-rw-r--r--   0 cmutel     (501) staff       (20)     4358 2022-06-28 06:02:09.000000 bw2calc-2.0.dev8/azure-pipelines.yml
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-06-28 06:19:13.960061 bw2calc-2.0.dev8/bw2calc/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1640 2022-05-03 08:10:09.000000 bw2calc-2.0.dev8/bw2calc/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      813 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/bw2calc/dense_lca.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3625 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/bw2calc/dictionary_manager.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1457 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/bw2calc/errors.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     9118 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/bw2calc/graph_traversal.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    25473 2022-05-22 10:38:05.000000 bw2calc-2.0.dev8/bw2calc/lca.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1500 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/bw2calc/least_squares.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3817 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/bw2calc/log_utils.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     7327 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/bw2calc/monte_carlo.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2840 2022-06-28 06:04:48.000000 bw2calc-2.0.dev8/bw2calc/multi_lca.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3466 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/bw2calc/single_value_diagonal_matrix.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2331 2022-05-22 10:39:02.000000 bw2calc-2.0.dev8/bw2calc/utils.py
+-rw-r--r--   0 cmutel     (501) staff       (20)       25 2022-06-28 06:18:22.000000 bw2calc-2.0.dev8/bw2calc/version.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-06-28 06:19:13.962676 bw2calc-2.0.dev8/bw2calc.egg-info/
+-rw-r--r--   0 cmutel     (501) staff       (20)     2093 2022-06-28 06:19:13.000000 bw2calc-2.0.dev8/bw2calc.egg-info/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)     3290 2022-06-28 06:19:13.000000 bw2calc-2.0.dev8/bw2calc.egg-info/SOURCES.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2022-06-28 06:19:13.000000 bw2calc-2.0.dev8/bw2calc.egg-info/dependency_links.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       59 2022-06-28 06:19:13.000000 bw2calc-2.0.dev8/bw2calc.egg-info/requires.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        8 2022-06-28 06:19:13.000000 bw2calc-2.0.dev8/bw2calc.egg-info/top_level.txt
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-06-28 06:19:13.963088 bw2calc-2.0.dev8/dev/
+-rw-r--r--   0 cmutel     (501) staff       (20)    25205 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/dev/lca_old.py
+-rw-r--r--   0 cmutel     (501) staff       (20)       55 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/pytest.ini
+-rw-r--r--   0 cmutel     (501) staff       (20)       53 2022-06-28 06:02:09.000000 bw2calc-2.0.dev8/requirements-test.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       67 2022-06-28 06:02:09.000000 bw2calc-2.0.dev8/requirements.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       38 2022-06-28 06:19:14.044213 bw2calc-2.0.dev8/setup.cfg
+-rw-r--r--   0 cmutel     (501) staff       (20)     1495 2022-06-28 06:06:35.000000 bw2calc-2.0.dev8/setup.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-06-28 06:19:13.972324 bw2calc-2.0.dev8/tests/
+-rw-r--r--   0 cmutel     (501) staff       (20)       24 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2889 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/dict_man.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-06-28 06:19:13.981475 bw2calc-2.0.dev8/tests/fixtures/
+-rw-r--r--   0 cmutel     (501) staff       (20)        0 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2135 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/array_sequential.zip
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-06-28 06:19:13.989103 bw2calc-2.0.dev8/tests/fixtures/basic_fixture/
+-rw-r--r--   0 cmutel     (501) staff       (20)      136 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/basic_fixture/biosphere.data.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      136 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/basic_fixture/biosphere.indices.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)     2914 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/basic_fixture/datapackage.json
+-rw-r--r--   0 cmutel     (501) staff       (20)      136 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/basic_fixture/eb-characterization.data.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      136 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/basic_fixture/eb-characterization.indices.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      152 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/basic_fixture/technosphere.data.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      131 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/basic_fixture/technosphere.flip.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      152 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/basic_fixture/technosphere.indices.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)     2120 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/basic_fixture.zip
+-rw-r--r--   0 cmutel     (501) staff       (20)     2565 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/bw2io_example_db.zip
+-rw-r--r--   0 cmutel     (501) staff       (20)      201 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/bw2io_example_db_mapping.json
+-rw-r--r--   0 cmutel     (501) staff       (20)    11301 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/create_fixtures.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-06-28 06:19:14.003056 bw2calc-2.0.dev8/tests/fixtures/empty_biosphere/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1435 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/empty_biosphere/biosphere.zip
+-rw-r--r--   0 cmutel     (501) staff       (20)       59 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/empty_biosphere/mapping.json
+-rw-r--r--   0 cmutel     (501) staff       (20)      848 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/empty_biosphere/method.zip
+-rw-r--r--   0 cmutel     (501) staff       (20)     1534 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/empty_biosphere/test_db.zip
+-rw-r--r--   0 cmutel     (501) staff       (20)     1703 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/empty_biosphere.zip
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-06-28 06:19:14.007938 bw2calc-2.0.dev8/tests/fixtures/example_db/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1734 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/example_db/example_db.zip
+-rw-r--r--   0 cmutel     (501) staff       (20)      854 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/example_db/ipcc.zip
+-rw-r--r--   0 cmutel     (501) staff       (20)      449 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/example_db/mapping.json
+-rw-r--r--   0 cmutel     (501) staff       (20)     1059 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/ipcc_simple.zip
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-06-28 06:19:14.020772 bw2calc-2.0.dev8/tests/fixtures/mc_basic/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1435 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/mc_basic/biosphere.zip
+-rw-r--r--   0 cmutel     (501) staff       (20)       90 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/mc_basic/mapping.json
+-rw-r--r--   0 cmutel     (501) staff       (20)      855 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/mc_basic/method.zip
+-rw-r--r--   0 cmutel     (501) staff       (20)     1604 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/mc_basic/test_db.zip
+-rw-r--r--   0 cmutel     (501) staff       (20)     3137 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/mc_basic.zip
+-rw-r--r--   0 cmutel     (501) staff       (20)     2083 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/mc_complete.zip
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-06-28 06:19:14.023146 bw2calc-2.0.dev8/tests/fixtures/mc_saop/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1436 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/mc_saop/biosphere.zip
+-rw-r--r--   0 cmutel     (501) staff       (20)       45 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/mc_saop/mapping.json
+-rw-r--r--   0 cmutel     (501) staff       (20)     1559 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/mc_saop/saop.zip
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-06-28 06:19:14.026824 bw2calc-2.0.dev8/tests/fixtures/multi/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1712 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/multi/datapackage.json
+-rw-r--r--   0 cmutel     (501) staff       (20)      226 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/multi/multi.0.indices.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      176 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/multi/multi.0.samples.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      240 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/multi/multi.1.indices.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      200 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/multi/multi.1.samples.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)     7444 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/presamples_basic.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-06-28 06:19:14.030757 bw2calc-2.0.dev8/tests/fixtures/seq/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1710 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/seq/datapackage.json
+-rw-r--r--   0 cmutel     (501) staff       (20)      226 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/seq/seq.0.indices.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      176 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/seq/seq.0.samples.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      240 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/seq/seq.1.indices.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      200 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/seq/seq.1.samples.npy
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-06-28 06:19:14.033326 bw2calc-2.0.dev8/tests/fixtures/single-matrix/
+-rw-r--r--   0 cmutel     (501) staff       (20)    15057 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/single-matrix/Test fixture.ipynb
+-rw-r--r--   0 cmutel     (501) staff       (20)     2491 2022-04-29 18:08:40.000000 bw2calc-2.0.dev8/tests/fixtures/single-matrix/generate_fixture.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1056 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/single-matrix/sm-fixture.tar.bz2
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-06-28 06:19:14.039053 bw2calc-2.0.dev8/tests/fixtures/single-sample/
+-rw-r--r--   0 cmutel     (501) staff       (20)     2475 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/single-sample/datapackage.json
+-rw-r--r--   0 cmutel     (501) staff       (20)      226 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/single-sample/single-sample.0.indices.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      144 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/single-sample/single-sample.0.samples.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      240 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/single-sample/single-sample.1.indices.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      152 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/single-sample/single-sample.1.samples.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      136 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/single-sample/single-sample.2.indices.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      136 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/single-sample/single-sample.2.samples.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)     1713 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/svdm.zip
+-rw-r--r--   0 cmutel     (501) staff       (20)      968 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/fixtures/svdm2.zip
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2022-06-28 06:19:14.042663 bw2calc-2.0.dev8/tests/fixtures/unseeded/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1732 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/unseeded/datapackage.json
+-rw-r--r--   0 cmutel     (501) staff       (20)      226 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/unseeded/unseeded.0.indices.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      176 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/unseeded/unseeded.0.samples.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      240 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/unseeded/unseeded.1.indices.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)      200 2020-03-11 10:53:14.000000 bw2calc-2.0.dev8/tests/fixtures/unseeded/unseeded.1.samples.npy
+-rw-r--r--   0 cmutel     (501) staff       (20)    48101 2022-05-22 10:43:45.000000 bw2calc-2.0.dev8/tests/lca.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3013 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/monte_carlo.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     8680 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/presamples.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      377 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/single_matrix.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3051 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/svdm.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1316 2022-04-01 11:27:21.000000 bw2calc-2.0.dev8/tests/utils.py
```

### Comparing `bw2calc-2.0.dev7/.gitignore` & `bw2calc-2.0.dev8/.gitignore`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/CHANGES.md` & `bw2calc-2.0.dev8/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 2.0.DEV8 (2022-06-28)
+
+* [#58 use logger at module level, not from LCA](https://github.com/brightway-lca/brightway2-calc/pull/58)
+* [#59 Fix a number of testing issues](https://github.com/brightway-lca/brightway2-calc/pull/59)
+
 ## 2.0.DEV7 (2022-05-22)
 
 * Add `LCA.keep_first_iteration` to make iteration simpler
 
 ## 2.0.DEV6 (2022-04-23)
 
 * Add an optional warning on LCA instantiation if excluding resources (arrays or distributions) which could be useful
```

### Comparing `bw2calc-2.0.dev7/CODE_OF_CONDUCT.md` & `bw2calc-2.0.dev8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/LICENSE.txt` & `bw2calc-2.0.dev8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/PKG-INFO` & `bw2calc-2.0.dev8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw2calc
-Version: 2.0.dev7
+Version: 2.0.dev8
 Home-page: https://bitbucket.org/cmutel/brightway2-calc
 Author: Chris Mutel
 Author-email: cmutel@gmail.com
 License: NewBSD 3-clause; LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `bw2calc-2.0.dev7/README.rst` & `bw2calc-2.0.dev8/README.rst`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/azure-pipelines.yml` & `bw2calc-2.0.dev8/azure-pipelines.yml`

 * *Files 24% similar despite different names*

```diff
@@ -17,19 +17,23 @@
     displayName: Add conda to PATH
 
   - bash: conda create --yes --quiet --name bw2
     displayName: Create Anaconda environment
 
   - bash: |
       source activate bw2
-      conda install --yes --quiet -c defaults -c conda-forge -c cmutel -c haasad --name bw2 python=$PYTHON_VERSION numpy bw_processing matrix_utils pandas scipy psutil pypardiso pytest peewee brightway2 pytest pytest-azurepipelines">=1.0.2" pytest-cov
+      conda install --yes --quiet -c defaults -c conda-forge -c cmutel -c haasad --name bw2 python=$PYTHON_VERSION numpy bw_processing bw2data matrix_utils pandas scipy psutil pypardiso pytest peewee pytest pytest-azurepipelines">=1.0.2" pytest-cov
     displayName: Install Anaconda packages
 
   - bash: |
       source activate bw2
+      # We have a conda based testing environment at this point, but to test with the conda package
+      # we need to build it first, and use conda install --use-local for example.
+      # This can be fixed later. TODO:
+      pip install -e .
       pytest --cov=bw2calc --cov-report=xml --cov-report=html
     displayName: pytest
 
   - task: PublishCodeCoverageResults@1
     inputs:
       codeCoverageTool: Cobertura
       summaryFileLocation: '$(System.DefaultWorkingDirectory)/**/coverage.xml'
@@ -45,27 +49,44 @@
         python.version: '3.10'
       Python39:
         python.version: '3.9'
       Python38:
         python.version: '3.8'
 
   steps:
-  - bash: |
-      python --version
-      pip --version
-      pip install --pre numpy bw_processing matrix_utils pandas scipy psutil pypardiso pytest peewee brightway2 pytest pytest-azurepipelines">=1.0.2" pytest-cov
-      echo "which pytest"
-      which pytest
-      echo "pytest version"
-      pytest --version
-    displayName: Install Pip packages
+    - bash: |
+        pip install virtualenv
+        virtualenv bw2
+      displayName: create virtualenv
+
+    - bash: |
+        source bw2/bin/activate      
+        pip install -U pip
+        pip --version
+      displayName: Update pip in virtualenv
+
+    - bash: |
+        source bw2/bin/activate      
+        python --version
+        pip --version
+        pip install --pre numpy bw_processing bw2data matrix_utils pandas scipy psutil pypardiso pytest peewee pytest pytest-azurepipelines">=1.0.2" pytest-cov
+        echo "which pytest: "
+        which pytest
+        echo "pytest version: "
+        pytest --version
+        echo "isntalled packages: "
+        pip list
+      displayName: Install testing dependencies
+
+    - bash: |
+        source bw2/bin/activate      
+        pip install -e .
+        pytest --cov=bw2calc --color=yes -v --cov-report html
+      displayName: Run pytest
 
-  - bash: |
-      pytest --cov=bw2calc --color=yes -v --cov-report html
-    displayName: pytest
 
 - job:
   displayName: macOS-1015-38-conda
   pool:
     vmImage: 'macOS-1015'
   strategy:
     matrix:
@@ -82,19 +103,20 @@
     displayName: Add conda to PATH
 
   - bash: conda create --yes --quiet --name bw2
     displayName: Create Anaconda environment
 
   - bash: |
       source activate bw2
-      conda install --yes --quiet -c defaults -c conda-forge -c cmutel -c haasad --name bw2 python=$PYTHON_VERSION numpy bw_processing matrix_utils pandas scipy psutil pypardiso pytest peewee brightway2 pytest pytest-azurepipelines">=1.0.2" pytest-cov
+      conda install --yes --quiet -c defaults -c conda-forge -c cmutel -c haasad --name bw2 python=$PYTHON_VERSION numpy bw_processing bw2data matrix_utils pandas scipy psutil pypardiso pytest peewee pytest pytest-azurepipelines">=1.0.2" pytest-cov
     displayName: Install Anaconda packages
 
   - bash: |
       source activate bw2
+      pip install -e .
       pytest --cov=bw2calc --cov-report=xml --cov-report=html
     displayName: pytest
 
 - job:
   displayName: windows-2019-conda
   pool:
     vmImage: 'windows-2019'
@@ -112,14 +134,15 @@
     displayName: Add conda to PATH
 
   - script: conda create --yes --quiet --name bw2
     displayName: Create Anaconda environment
 
   - script: |
       call activate bw2
-      conda install --yes --quiet -c defaults -c conda-forge -c cmutel -c haasad --name bw2 python=%PYTHON_VERSION% numpy bw_processing matrix_utils pandas scipy psutil pypardiso pytest peewee brightway2 pytest pytest-azurepipelines">=1.0.2" pytest-cov
+      conda install --yes --quiet -c defaults -c conda-forge -c cmutel -c haasad --name bw2 python=%PYTHON_VERSION% numpy bw_processing bw2data matrix_utils pandas scipy psutil pypardiso pytest peewee pytest pytest-azurepipelines">=1.0.2" pytest-cov
     displayName: Install Anaconda packages
 
   - script: |
       call activate bw2
+      pip install -e .
       pytest --cov=bw2calc --cov-report=xml --cov-report=html
     displayName: pytest
```

### Comparing `bw2calc-2.0.dev7/bw2calc/__init__.py` & `bw2calc-2.0.dev8/bw2calc/__init__.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/bw2calc/dense_lca.py` & `bw2calc-2.0.dev8/bw2calc/dense_lca.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/bw2calc/dictionary_manager.py` & `bw2calc-2.0.dev8/bw2calc/dictionary_manager.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/bw2calc/errors.py` & `bw2calc-2.0.dev8/bw2calc/errors.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/bw2calc/graph_traversal.py` & `bw2calc-2.0.dev8/bw2calc/graph_traversal.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/bw2calc/lca.py` & `bw2calc-2.0.dev8/bw2calc/lca.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/bw2calc/least_squares.py` & `bw2calc-2.0.dev8/bw2calc/least_squares.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/bw2calc/log_utils.py` & `bw2calc-2.0.dev8/bw2calc/log_utils.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/bw2calc/monte_carlo.py` & `bw2calc-2.0.dev8/bw2calc/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/bw2calc/multi_lca.py` & `bw2calc-2.0.dev8/bw2calc/multi_lca.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,20 @@
+import logging
 import numpy as np
-from bw2data import calculation_setups
+try:
+    from bw2data import calculation_setups
+except ImportError:
+    calculation_setups = None
 
 from .lca import LCA
 
 
+logger = logging.getLogger("bw2calc")
+
+
 class InventoryMatrices:
     def __init__(self, biosphere_matrix, supply_arrays):
         self.biosphere_matrix = biosphere_matrix
         self.supply_arrays = supply_arrays
 
     def __getitem__(self, fu_index):
         if fu_index is Ellipsis:
@@ -25,24 +32,24 @@
 
     Initialization creates `self.results`, which is a NumPy array of LCA scores, with rows of functional units and columns of LCIA methods. Ordering is the same as in the `calculation_setup`.
 
     """
 
     def __init__(self, cs_name, log_config=None):
         if calculation_setups is None:
-            raise ImportError
+            raise ImportError("`bw2data` is required for this functionality")
         assert cs_name in calculation_setups
         try:
             cs = calculation_setups[cs_name]
         except KeyError:
             raise ValueError("{} is not a known `calculation_setup`.".format(cs_name))
         self.func_units = cs["inv"]
         self.methods = cs["ia"]
         self.lca = LCA(demand=self.all, method=self.methods[0], log_config=log_config)
-        self.lca.logger.info(
+        logger.info(
             {
                 "message": "Started MultiLCA calculation",
                 "methods": list(self.methods),
                 "functional units": [wrap_functional_unit(o) for o in self.func_units],
             }
         )
         self.lca.lci()
```

### Comparing `bw2calc-2.0.dev7/bw2calc/single_value_diagonal_matrix.py` & `bw2calc-2.0.dev8/bw2calc/single_value_diagonal_matrix.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/bw2calc/utils.py` & `bw2calc-2.0.dev8/bw2calc/utils.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/bw2calc.egg-info/PKG-INFO` & `bw2calc-2.0.dev8/bw2calc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw2calc
-Version: 2.0.dev7
+Version: 2.0.dev8
 Home-page: https://bitbucket.org/cmutel/brightway2-calc
 Author: Chris Mutel
 Author-email: cmutel@gmail.com
 License: NewBSD 3-clause; LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `bw2calc-2.0.dev7/bw2calc.egg-info/SOURCES.txt` & `bw2calc-2.0.dev8/bw2calc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/dev/lca_old.py` & `bw2calc-2.0.dev8/dev/lca_old.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/setup.py` & `bw2calc-2.0.dev8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     packages=["bw2calc"],
     author="Chris Mutel",
     author_email="cmutel@gmail.com",
     license="NewBSD 3-clause; LICENSE.txt",
     url="https://bitbucket.org/cmutel/brightway2-calc",
     install_requires=[
         "bw_processing",
+        "matrix_utils",
         "numpy",
         "pandas",
         "scipy",
         "stats_arrays",
     ],
     long_description=open('README.rst').read(),
     classifiers=[
```

### Comparing `bw2calc-2.0.dev7/tests/dict_man.py` & `bw2calc-2.0.dev8/tests/dict_man.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/array_sequential.zip` & `bw2calc-2.0.dev8/tests/fixtures/array_sequential.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/basic_fixture/datapackage.json` & `bw2calc-2.0.dev8/tests/fixtures/basic_fixture/datapackage.json`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/basic_fixture.zip` & `bw2calc-2.0.dev8/tests/fixtures/basic_fixture.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/bw2io_example_db.zip` & `bw2calc-2.0.dev8/tests/fixtures/bw2io_example_db.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/create_fixtures.py` & `bw2calc-2.0.dev8/tests/fixtures/create_fixtures.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/empty_biosphere/biosphere.zip` & `bw2calc-2.0.dev8/tests/fixtures/empty_biosphere/biosphere.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/empty_biosphere/method.zip` & `bw2calc-2.0.dev8/tests/fixtures/empty_biosphere/method.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/empty_biosphere/test_db.zip` & `bw2calc-2.0.dev8/tests/fixtures/empty_biosphere/test_db.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/empty_biosphere.zip` & `bw2calc-2.0.dev8/tests/fixtures/empty_biosphere.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/example_db/example_db.zip` & `bw2calc-2.0.dev8/tests/fixtures/example_db/example_db.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/example_db/ipcc.zip` & `bw2calc-2.0.dev8/tests/fixtures/example_db/ipcc.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/ipcc_simple.zip` & `bw2calc-2.0.dev8/tests/fixtures/ipcc_simple.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/mc_basic/biosphere.zip` & `bw2calc-2.0.dev8/tests/fixtures/mc_basic/biosphere.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/mc_basic/method.zip` & `bw2calc-2.0.dev8/tests/fixtures/mc_basic/method.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/mc_basic/test_db.zip` & `bw2calc-2.0.dev8/tests/fixtures/mc_basic/test_db.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/mc_basic.zip` & `bw2calc-2.0.dev8/tests/fixtures/mc_basic.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/mc_complete.zip` & `bw2calc-2.0.dev8/tests/fixtures/mc_complete.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/mc_saop/biosphere.zip` & `bw2calc-2.0.dev8/tests/fixtures/mc_saop/biosphere.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/mc_saop/saop.zip` & `bw2calc-2.0.dev8/tests/fixtures/mc_saop/saop.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/multi/datapackage.json` & `bw2calc-2.0.dev8/tests/fixtures/multi/datapackage.json`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/presamples_basic.py` & `bw2calc-2.0.dev8/tests/fixtures/presamples_basic.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/seq/datapackage.json` & `bw2calc-2.0.dev8/tests/fixtures/seq/datapackage.json`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/single-matrix/Test fixture.ipynb` & `bw2calc-2.0.dev8/tests/fixtures/single-matrix/Test fixture.ipynb`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/single-matrix/generate_fixture.py` & `bw2calc-2.0.dev8/tests/fixtures/single-matrix/generate_fixture.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/single-matrix/sm-fixture.tar.bz2` & `bw2calc-2.0.dev8/tests/fixtures/single-matrix/sm-fixture.tar.bz2`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/single-sample/datapackage.json` & `bw2calc-2.0.dev8/tests/fixtures/single-sample/datapackage.json`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/svdm.zip` & `bw2calc-2.0.dev8/tests/fixtures/svdm.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/svdm2.zip` & `bw2calc-2.0.dev8/tests/fixtures/svdm2.zip`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/fixtures/unseeded/datapackage.json` & `bw2calc-2.0.dev8/tests/fixtures/unseeded/datapackage.json`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/lca.py` & `bw2calc-2.0.dev8/tests/lca.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/monte_carlo.py` & `bw2calc-2.0.dev8/tests/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/presamples.py` & `bw2calc-2.0.dev8/tests/presamples.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/svdm.py` & `bw2calc-2.0.dev8/tests/svdm.py`

 * *Files identical despite different names*

### Comparing `bw2calc-2.0.dev7/tests/utils.py` & `bw2calc-2.0.dev8/tests/utils.py`

 * *Files identical despite different names*

