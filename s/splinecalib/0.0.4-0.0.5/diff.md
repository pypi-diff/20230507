# Comparing `tmp/splinecalib-0.0.4.tar.gz` & `tmp/splinecalib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splinecalib-0.0.4.tar", last modified: Fri Dec  2 17:54:51 2022, max compression
+gzip compressed data, was "splinecalib-0.0.5.tar", last modified: Sun May  7 19:32:08 2023, max compression
```

## Comparing `splinecalib-0.0.4.tar` & `splinecalib-0.0.5.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2022-12-02 17:54:51.750104 splinecalib-0.0.4/
--rw-r--r--   0 brianlucena   (501) staff       (20)     1822 2022-05-05 20:11:18.000000 splinecalib-0.0.4/.gitignore
--rw-r--r--   0 brianlucena   (501) staff       (20)     1069 2022-05-05 20:11:18.000000 splinecalib-0.0.4/LICENSE
--rw-r--r--   0 brianlucena   (501) staff       (20)      879 2022-12-02 17:54:51.749833 splinecalib-0.0.4/PKG-INFO
--rw-r--r--   0 brianlucena   (501) staff       (20)       51 2022-05-05 20:11:18.000000 splinecalib-0.0.4/README.md
-drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2022-12-02 17:54:51.697607 splinecalib-0.0.4/docs/
--rw-r--r--   0 brianlucena   (501) staff       (20)      638 2022-05-05 20:49:20.000000 splinecalib-0.0.4/docs/Makefile
--rw-r--r--   0 brianlucena   (501) staff       (20)      804 2022-05-05 20:49:20.000000 splinecalib-0.0.4/docs/make.bat
-drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2022-12-02 17:54:51.698133 splinecalib-0.0.4/docs/source/
--rw-r--r--   0 brianlucena   (501) staff       (20)     1894 2022-05-05 20:49:20.000000 splinecalib-0.0.4/docs/source/conf.py
--rw-r--r--   0 brianlucena   (501) staff       (20)      386 2022-05-05 20:55:01.000000 splinecalib-0.0.4/docs/source/index.rst
--rw-r--r--   0 brianlucena   (501) staff       (20)      108 2022-12-02 17:46:40.000000 splinecalib-0.0.4/pyproject.toml
--rw-r--r--   0 brianlucena   (501) staff       (20)       38 2022-12-02 17:54:51.750208 splinecalib-0.0.4/setup.cfg
--rw-r--r--   0 brianlucena   (501) staff       (20)     1352 2022-12-02 17:49:27.000000 splinecalib-0.0.4/setup.py
-drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2022-12-02 17:54:51.700229 splinecalib-0.0.4/splinecalib/
--rw-r--r--   0 brianlucena   (501) staff       (20)      152 2022-12-02 17:51:12.000000 splinecalib-0.0.4/splinecalib/__init__.py
--rw-r--r--   0 brianlucena   (501) staff       (20)     5786 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/calib_utils.py
--rw-r--r--   0 brianlucena   (501) staff       (20)   320695 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/loss_fun_c.c
--rw-r--r--   0 brianlucena   (501) staff       (20)     3792 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/loss_fun_c.pyx
--rw-r--r--   0 brianlucena   (501) staff       (20)    22515 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/splinecalib.py
-drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2022-12-02 17:54:51.703438 splinecalib-0.0.4/splinecalib/tests/
--rw-r--r--   0 brianlucena   (501) staff       (20)        0 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/__init__.py
-drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2022-12-02 17:54:51.748748 splinecalib-0.0.4/splinecalib/tests/data_for_tests/
--rw-r--r--   0 brianlucena   (501) staff       (20)   195349 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_2dplanes_727_cb1.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)   193560 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_2dplanes_727_cb2.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)   190016 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_2dplanes_727_cb3.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)   121622 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_2dplanes_727_rf.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)   124282 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_airlines_42493_cb1.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)   124277 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_airlines_42493_cb2.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)   124219 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_airlines_42493_cb3.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)   117033 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_airlines_42493_rf.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)    73600 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_mozilla4_1046_cb1.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)    72913 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_mozilla4_1046_cb2.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)    71946 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_mozilla4_1046_cb3.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)    29818 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_mozilla4_1046_rf.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)  3087605 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/mnist4_calib_set.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)   518938 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/mnist4_test_set.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)   195242 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_2dplanes_727_cb1.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)   193533 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_2dplanes_727_cb2.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)   189972 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_2dplanes_727_cb3.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)   122712 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_2dplanes_727_rf.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)   124277 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_airlines_42493_cb1.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)   124317 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_airlines_42493_cb2.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)   124157 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_airlines_42493_cb3.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)   117232 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_airlines_42493_rf.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)    73488 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_mozilla4_1046_cb1.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)    72856 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_mozilla4_1046_cb2.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)    71928 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_mozilla4_1046_cb3.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)    29893 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_mozilla4_1046_rf.csv
--rw-r--r--   0 brianlucena   (501) staff       (20)    11197 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/test_binary_datasets.py
--rw-r--r--   0 brianlucena   (501) staff       (20)      957 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/test_multiclass_datasets.py
--rw-r--r--   0 brianlucena   (501) staff       (20)     1709 2022-05-05 20:11:18.000000 splinecalib-0.0.4/splinecalib/tests/test_unity_prior.py
-drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2022-12-02 17:54:51.702021 splinecalib-0.0.4/splinecalib.egg-info/
--rw-r--r--   0 brianlucena   (501) staff       (20)      879 2022-12-02 17:54:51.000000 splinecalib-0.0.4/splinecalib.egg-info/PKG-INFO
--rw-r--r--   0 brianlucena   (501) staff       (20)     2207 2022-12-02 17:54:51.000000 splinecalib-0.0.4/splinecalib.egg-info/SOURCES.txt
--rw-r--r--   0 brianlucena   (501) staff       (20)        1 2022-12-02 17:54:51.000000 splinecalib-0.0.4/splinecalib.egg-info/dependency_links.txt
--rw-r--r--   0 brianlucena   (501) staff       (20)       23 2022-12-02 17:54:51.000000 splinecalib-0.0.4/splinecalib.egg-info/requires.txt
--rw-r--r--   0 brianlucena   (501) staff       (20)       23 2022-12-02 17:54:51.000000 splinecalib-0.0.4/splinecalib.egg-info/top_level.txt
+drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-05-07 19:32:08.032964 splinecalib-0.0.5/
+-rw-r--r--   0 brianlucena   (501) staff       (20)     1822 2022-05-05 20:11:18.000000 splinecalib-0.0.5/.gitignore
+-rw-r--r--   0 brianlucena   (501) staff       (20)     1069 2022-05-05 20:11:18.000000 splinecalib-0.0.5/LICENSE
+-rw-r--r--   0 brianlucena   (501) staff       (20)      859 2023-05-07 19:32:08.032622 splinecalib-0.0.5/PKG-INFO
+-rw-r--r--   0 brianlucena   (501) staff       (20)       51 2022-05-05 20:11:18.000000 splinecalib-0.0.5/README.md
+drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-05-07 19:32:08.005933 splinecalib-0.0.5/docs/
+-rw-r--r--   0 brianlucena   (501) staff       (20)      638 2022-05-05 20:49:20.000000 splinecalib-0.0.5/docs/Makefile
+-rw-r--r--   0 brianlucena   (501) staff       (20)      804 2022-05-05 20:49:20.000000 splinecalib-0.0.5/docs/make.bat
+drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-05-07 19:32:08.006549 splinecalib-0.0.5/docs/source/
+-rw-r--r--   0 brianlucena   (501) staff       (20)     1894 2022-05-05 20:49:20.000000 splinecalib-0.0.5/docs/source/conf.py
+-rw-r--r--   0 brianlucena   (501) staff       (20)      386 2022-05-05 20:55:01.000000 splinecalib-0.0.5/docs/source/index.rst
+-rw-r--r--   0 brianlucena   (501) staff       (20)      108 2022-12-02 17:46:40.000000 splinecalib-0.0.5/pyproject.toml
+-rw-r--r--   0 brianlucena   (501) staff       (20)       38 2023-05-07 19:32:08.033103 splinecalib-0.0.5/setup.cfg
+-rw-r--r--   0 brianlucena   (501) staff       (20)     1352 2023-05-07 19:31:04.000000 splinecalib-0.0.5/setup.py
+drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-05-07 19:32:08.008472 splinecalib-0.0.5/splinecalib/
+-rw-r--r--   0 brianlucena   (501) staff       (20)      152 2023-05-07 19:03:39.000000 splinecalib-0.0.5/splinecalib/__init__.py
+-rw-r--r--   0 brianlucena   (501) staff       (20)     5786 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/calib_utils.py
+-rw-r--r--   0 brianlucena   (501) staff       (20)   320695 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/loss_fun_c.c
+-rw-r--r--   0 brianlucena   (501) staff       (20)     3792 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/loss_fun_c.pyx
+-rw-r--r--   0 brianlucena   (501) staff       (20)    22513 2023-05-07 19:02:43.000000 splinecalib-0.0.5/splinecalib/splinecalib.py
+drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-05-07 19:32:08.011230 splinecalib-0.0.5/splinecalib/tests/
+-rw-r--r--   0 brianlucena   (501) staff       (20)        0 2023-05-07 19:24:08.000000 splinecalib-0.0.5/splinecalib/tests/__init__.py
+drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-05-07 19:32:08.032141 splinecalib-0.0.5/splinecalib/tests/data_for_tests/
+-rw-r--r--   0 brianlucena   (501) staff       (20)   195349 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_2dplanes_727_cb1.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)   193560 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_2dplanes_727_cb2.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)   190016 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_2dplanes_727_cb3.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)   121622 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_2dplanes_727_rf.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)   124282 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_airlines_42493_cb1.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)   124277 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_airlines_42493_cb2.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)   124219 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_airlines_42493_cb3.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)   117033 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_airlines_42493_rf.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)    73600 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_mozilla4_1046_cb1.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)    72913 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_mozilla4_1046_cb2.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)    71946 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_mozilla4_1046_cb3.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)    29818 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_mozilla4_1046_rf.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)   518938 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/mnist4_test_set.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)   195242 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_2dplanes_727_cb1.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)   193533 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_2dplanes_727_cb2.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)   189972 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_2dplanes_727_cb3.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)   122712 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_2dplanes_727_rf.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)   124277 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_airlines_42493_cb1.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)   124317 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_airlines_42493_cb2.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)   124157 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_airlines_42493_cb3.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)   117232 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_airlines_42493_rf.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)    73488 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_mozilla4_1046_cb1.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)    72856 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_mozilla4_1046_cb2.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)    71928 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_mozilla4_1046_cb3.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)    29893 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_mozilla4_1046_rf.csv
+-rw-r--r--   0 brianlucena   (501) staff       (20)     8837 2023-05-07 19:30:17.000000 splinecalib-0.0.5/splinecalib/tests/test_binary_datasets.py
+-rw-r--r--   0 brianlucena   (501) staff       (20)      957 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/test_multiclass_datasets.py
+-rw-r--r--   0 brianlucena   (501) staff       (20)     1709 2022-05-05 20:11:18.000000 splinecalib-0.0.5/splinecalib/tests/test_unity_prior.py
+drwxr-xr-x   0 brianlucena   (501) staff       (20)        0 2023-05-07 19:32:08.010067 splinecalib-0.0.5/splinecalib.egg-info/
+-rw-r--r--   0 brianlucena   (501) staff       (20)      859 2023-05-07 19:32:07.000000 splinecalib-0.0.5/splinecalib.egg-info/PKG-INFO
+-rw-r--r--   0 brianlucena   (501) staff       (20)     2153 2023-05-07 19:32:07.000000 splinecalib-0.0.5/splinecalib.egg-info/SOURCES.txt
+-rw-r--r--   0 brianlucena   (501) staff       (20)        1 2023-05-07 19:32:07.000000 splinecalib-0.0.5/splinecalib.egg-info/dependency_links.txt
+-rw-r--r--   0 brianlucena   (501) staff       (20)       23 2023-05-07 19:32:07.000000 splinecalib-0.0.5/splinecalib.egg-info/requires.txt
+-rw-r--r--   0 brianlucena   (501) staff       (20)       23 2023-05-07 19:32:07.000000 splinecalib-0.0.5/splinecalib.egg-info/top_level.txt
```

### Comparing `splinecalib-0.0.4/.gitignore` & `splinecalib-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/LICENSE` & `splinecalib-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/PKG-INFO` & `splinecalib-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: splinecalib
-Version: 0.0.4
+Version: 0.0.5
 Summary: SplineCalib is a Python package for calibrating ML models using smoothing splines.  See documentation at: https://splinecalib.readthedocs.io/
 Home-page: https://github.com/numeristical/splinecalib
 Author: Brian Lucena
 Author-email: brianlucena@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5
 License-File: LICENSE
 
 # splinecalib
 Location for the splinecalib package
-
-
```

### Comparing `splinecalib-0.0.4/docs/Makefile` & `splinecalib-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/docs/make.bat` & `splinecalib-0.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/docs/source/conf.py` & `splinecalib-0.0.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/setup.py` & `splinecalib-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 setuptools.setup(
     author="Brian Lucena",
     author_email="brianlucena@gmail.com",
     name='splinecalib',
     license="MIT",
     license_files=['LICENSE'],
     description="SplineCalib is a Python package for calibrating ML models using smoothing splines.  See documentation at: https://splinecalib.readthedocs.io/",
-    version='0.0.4',
+    version='0.0.5',
     long_description=README,
     url='https://github.com/numeristical/splinecalib',
     packages=['splinecalib'],
     package_dir={'splinecalib':
                  'splinecalib'},
     python_requires=">=3.5",
     install_requires=[
```

### Comparing `splinecalib-0.0.4/splinecalib/calib_utils.py` & `splinecalib-0.0.5/splinecalib/calib_utils.py`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/loss_fun_c.c` & `splinecalib-0.0.5/splinecalib/loss_fun_c.c`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/loss_fun_c.pyx` & `splinecalib-0.0.5/splinecalib/loss_fun_c.pyx`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/splinecalib.py` & `splinecalib-0.0.5/splinecalib/splinecalib.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,21 +57,21 @@
 
     random_state : 
         If desired, can specify the random state for the generation
         of the stratified folds. Default is 42.
 
     unity_prior : bool
         If True, routine will add synthetic data along the axis y=x as
-        a "prior" distribution that favors that function.  Default is False.
+        a "prior" distribution that favors that function.  Default is True.
 
     unity_prior_weight : 
         Ignored if unity_prior=False.  The total weight of data points added 
         when unity_prior is set to True.  Bigger values will force the calibration
-        curve closer to the line y=x. Default is 10, meaning the synthetic data in 
-        total counts as much weight as 10 data points.
+        curve closer to the line y=x. Default is 20, meaning the synthetic data in 
+        total counts as much weight as 20 data points.
 
     unity_prior_gridpts : 'default' or list-like
         Ignored if unity_prior = False. Which points to use in order to create 
         synthetic data along the line y=x.  'default' will choose something reasonable.
 
     logodds_scale : bool, Default is True
         Whether or not to transform the x-values to the log odds
@@ -120,16 +120,16 @@
     ----------
 
     Lucena, B. Spline-Based Probability Calibration. https://arxiv.org/abs/1809.07751
    """
     def __init__(self,method='L-BFGS-B',
                  knot_sample_size = 30, add_knots = 'auto',
                  reg_param_vec = 'default', cv_spline=5, random_state=42,
-                 unity_prior=False, unity_prior_gridpts='default', 
-                 unity_prior_weight=10, max_iter=1000, tol=.0001,
+                 unity_prior=True, unity_prior_gridpts='default', 
+                 unity_prior_weight=20, max_iter=1000, tol=.0001,
                  logodds_scale=True, logodds_eps='auto', reg_prec=4,
                  force_knot_endpts=True, param_search_mode='fast'):
         self.knot_sample_size = knot_sample_size
         self.add_knots = add_knots
         if (type(self.add_knots)==str) and (self.add_knots == 'auto'):
             self.add_knots = np.linspace(.1,.9,9)
         if (type(reg_param_vec)==str) and (reg_param_vec == 'default'):
```

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_2dplanes_727_cb1.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_2dplanes_727_cb1.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_2dplanes_727_cb2.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_2dplanes_727_cb2.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_2dplanes_727_cb3.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_2dplanes_727_cb3.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_2dplanes_727_rf.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_2dplanes_727_rf.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_airlines_42493_cb1.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_airlines_42493_cb1.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_airlines_42493_cb2.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_airlines_42493_cb2.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_airlines_42493_cb3.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_airlines_42493_cb3.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_airlines_42493_rf.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_airlines_42493_rf.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_mozilla4_1046_cb1.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_mozilla4_1046_cb1.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_mozilla4_1046_cb2.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_mozilla4_1046_cb2.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_mozilla4_1046_cb3.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_mozilla4_1046_cb3.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/calibset_mozilla4_1046_rf.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/calibset_mozilla4_1046_rf.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/mnist4_test_set.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/mnist4_test_set.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_2dplanes_727_cb1.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_2dplanes_727_cb1.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_2dplanes_727_cb2.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_2dplanes_727_cb2.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_2dplanes_727_cb3.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_2dplanes_727_cb3.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_2dplanes_727_rf.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_2dplanes_727_rf.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_airlines_42493_cb1.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_airlines_42493_cb1.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_airlines_42493_cb2.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_airlines_42493_cb2.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_airlines_42493_cb3.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_airlines_42493_cb3.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_airlines_42493_rf.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_airlines_42493_rf.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_mozilla4_1046_cb1.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_mozilla4_1046_cb1.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_mozilla4_1046_cb2.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_mozilla4_1046_cb2.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_mozilla4_1046_cb3.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_mozilla4_1046_cb3.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/data_for_tests/testset_mozilla4_1046_rf.csv` & `splinecalib-0.0.5/splinecalib/tests/data_for_tests/testset_mozilla4_1046_rf.csv`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/test_binary_datasets.py` & `splinecalib-0.0.5/splinecalib/tests/test_binary_datasets.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os.path as op
 import numpy as np
 import pandas as pd
 import splinecalib as splc
-import betacal as bc
+# import betacal as bc
 from sklearn.metrics import roc_auc_score, log_loss
 
 data_path = op.join(splc.__path__[0], 'tests/data_for_tests')
 
 
 def test_calibration_mozilla4_1046_rf():
     """
@@ -22,20 +22,15 @@
     preds_test = test_set.iloc[:,0].to_numpy()
     y_test = test_set.iloc[:,1].to_numpy()
     sc = splc.SplineCalib()
     sc.fit(preds_calib_set, y_calib_set)
     preds_test_calibrated = sc.calibrate(preds_test)
     ll_calib = log_loss(y_test, preds_test_calibrated)
 
-    bc1 = bc.BetaCalibration()
-    bc1.fit(preds_calib_set, y_calib_set)
-    bc_preds_test_calibrated = bc1.predict(preds_test)
-    bc_ll_calib = log_loss(y_test, bc_preds_test_calibrated)
-
-    assert(ll_calib<bc_ll_calib)
+    assert(ll_calib<0.127)
 
 def test_calibration_mozilla4_1046_cb1():
     """
     We test the default settings and 
     ensure that the resulting log-loss gives good performance
 
     """
@@ -47,20 +42,15 @@
     preds_test = test_set.iloc[:,0].to_numpy()
     y_test = test_set.iloc[:,1].to_numpy()
     sc = splc.SplineCalib()
     sc.fit(preds_calib_set, y_calib_set)
     preds_test_calibrated = sc.calibrate(preds_test)
     ll_calib = log_loss(y_test, preds_test_calibrated)
 
-    bc1 = bc.BetaCalibration()
-    bc1.fit(preds_calib_set, y_calib_set)
-    bc_preds_test_calibrated = bc1.predict(preds_test)
-    bc_ll_calib = log_loss(y_test, bc_preds_test_calibrated)
-
-    assert(ll_calib<bc_ll_calib*1.01)
+    assert(ll_calib<0.139)
 
 def test_calibration_mozilla4_1046_cb2():
     """
     We test the default settings and 
     ensure that the resulting log-loss gives good performance
 
     """
@@ -72,20 +62,15 @@
     preds_test = test_set.iloc[:,0].to_numpy()
     y_test = test_set.iloc[:,1].to_numpy()
     sc = splc.SplineCalib()
     sc.fit(preds_calib_set, y_calib_set)
     preds_test_calibrated = sc.calibrate(preds_test)
     ll_calib = log_loss(y_test, preds_test_calibrated)
 
-    bc1 = bc.BetaCalibration()
-    bc1.fit(preds_calib_set, y_calib_set)
-    bc_preds_test_calibrated = bc1.predict(preds_test)
-    bc_ll_calib = log_loss(y_test, bc_preds_test_calibrated)
-
-    assert(ll_calib<bc_ll_calib)
+    assert(ll_calib<0.158)
 
 def test_calibration_mozilla4_1046_cb3():
     """
     We test the default settings and 
     ensure that the resulting log-loss gives good performance
 
     """
@@ -97,20 +82,15 @@
     preds_test = test_set.iloc[:,0].to_numpy()
     y_test = test_set.iloc[:,1].to_numpy()
     sc = splc.SplineCalib()
     sc.fit(preds_calib_set, y_calib_set)
     preds_test_calibrated = sc.calibrate(preds_test)
     ll_calib = log_loss(y_test, preds_test_calibrated)
 
-    bc1 = bc.BetaCalibration()
-    bc1.fit(preds_calib_set, y_calib_set)
-    bc_preds_test_calibrated = bc1.predict(preds_test)
-    bc_ll_calib = log_loss(y_test, bc_preds_test_calibrated)
-
-    assert(ll_calib<bc_ll_calib)
+    assert(ll_calib<0.177)
 
 def test_calibration_airlines_42493_rf():
     """
     We test the default settings and 
     ensure that the resulting log-loss gives good performance
 
     """
@@ -122,20 +102,15 @@
     preds_test = test_set.iloc[:,0].to_numpy()
     y_test = test_set.iloc[:,1].to_numpy()
     sc = splc.SplineCalib()
     sc.fit(preds_calib_set, y_calib_set)
     preds_test_calibrated = sc.calibrate(preds_test)
     ll_calib = log_loss(y_test, preds_test_calibrated)
 
-    bc1 = bc.BetaCalibration()
-    bc1.fit(preds_calib_set, y_calib_set)
-    bc_preds_test_calibrated = bc1.predict(preds_test)
-    bc_ll_calib = log_loss(y_test, bc_preds_test_calibrated)
-
-    assert(ll_calib<bc_ll_calib)
+    assert(ll_calib<0.680)
 
 def test_calibration_airlines_42493_cb1():
     """
     We test the default settings and 
     ensure that the resulting log-loss gives good performance
 
     """
@@ -147,20 +122,15 @@
     preds_test = test_set.iloc[:,0].to_numpy()
     y_test = test_set.iloc[:,1].to_numpy()
     sc = splc.SplineCalib()
     sc.fit(preds_calib_set, y_calib_set)
     preds_test_calibrated = sc.calibrate(preds_test)
     ll_calib = log_loss(y_test, preds_test_calibrated)
 
-    bc1 = bc.BetaCalibration()
-    bc1.fit(preds_calib_set, y_calib_set)
-    bc_preds_test_calibrated = bc1.predict(preds_test)
-    bc_ll_calib = log_loss(y_test, bc_preds_test_calibrated)
-
-    assert(ll_calib<bc_ll_calib)
+    assert(ll_calib<0.669)
 
 def test_calibration_airlines_42493_cb2():
     """
     We test the default settings and 
     ensure that the resulting log-loss gives good performance
 
     """
@@ -172,20 +142,15 @@
     preds_test = test_set.iloc[:,0].to_numpy()
     y_test = test_set.iloc[:,1].to_numpy()
     sc = splc.SplineCalib()
     sc.fit(preds_calib_set, y_calib_set)
     preds_test_calibrated = sc.calibrate(preds_test)
     ll_calib = log_loss(y_test, preds_test_calibrated)
 
-    bc1 = bc.BetaCalibration()
-    bc1.fit(preds_calib_set, y_calib_set)
-    bc_preds_test_calibrated = bc1.predict(preds_test)
-    bc_ll_calib = log_loss(y_test, bc_preds_test_calibrated)
-
-    assert(ll_calib<bc_ll_calib)
+    assert(ll_calib<0.669)
 
 def test_calibration_airlines_42493_cb3():
     """
     We test the default settings and 
     ensure that the resulting log-loss gives good performance
 
     """
@@ -197,20 +162,15 @@
     preds_test = test_set.iloc[:,0].to_numpy()
     y_test = test_set.iloc[:,1].to_numpy()
     sc = splc.SplineCalib()
     sc.fit(preds_calib_set, y_calib_set)
     preds_test_calibrated = sc.calibrate(preds_test)
     ll_calib = log_loss(y_test, preds_test_calibrated)
 
-    bc1 = bc.BetaCalibration()
-    bc1.fit(preds_calib_set, y_calib_set)
-    bc_preds_test_calibrated = bc1.predict(preds_test)
-    bc_ll_calib = log_loss(y_test, bc_preds_test_calibrated)
-
-    assert(ll_calib<bc_ll_calib)
+    assert(ll_calib<0.669)
 
 def test_calibration_2dplanes_727_rf():
     """
     We test the default settings and 
     ensure that the resulting log-loss gives good performance
 
     """
@@ -222,20 +182,15 @@
     preds_test = test_set.iloc[:,0].to_numpy()
     y_test = test_set.iloc[:,1].to_numpy()
     sc = splc.SplineCalib()
     sc.fit(preds_calib_set, y_calib_set)
     preds_test_calibrated = sc.calibrate(preds_test)
     ll_calib = log_loss(y_test, preds_test_calibrated)
 
-    bc1 = bc.BetaCalibration()
-    bc1.fit(preds_calib_set, y_calib_set)
-    bc_preds_test_calibrated = bc1.predict(preds_test)
-    bc_ll_calib = log_loss(y_test, bc_preds_test_calibrated)
-
-    assert(ll_calib<bc_ll_calib)
+    assert(ll_calib<0.183)
 
 def test_calibration_2dplanes_727_cb1():
     """
     We test the default settings and 
     ensure that the resulting log-loss gives good performance
 
     """
@@ -247,20 +202,15 @@
     preds_test = test_set.iloc[:,0].to_numpy()
     y_test = test_set.iloc[:,1].to_numpy()
     sc = splc.SplineCalib()
     sc.fit(preds_calib_set, y_calib_set)
     preds_test_calibrated = sc.calibrate(preds_test)
     ll_calib = log_loss(y_test, preds_test_calibrated)
 
-    bc1 = bc.BetaCalibration()
-    bc1.fit(preds_calib_set, y_calib_set)
-    bc_preds_test_calibrated = bc1.predict(preds_test)
-    bc_ll_calib = log_loss(y_test, bc_preds_test_calibrated)
-
-    assert(ll_calib<bc_ll_calib*1.01)
+    assert(ll_calib<0.150)
 
 def test_calibration_2dplanes_727_cb2():
     """
     We test the default settings and 
     ensure that the resulting log-loss gives good performance
 
     """
@@ -272,20 +222,15 @@
     preds_test = test_set.iloc[:,0].to_numpy()
     y_test = test_set.iloc[:,1].to_numpy()
     sc = splc.SplineCalib()
     sc.fit(preds_calib_set, y_calib_set)
     preds_test_calibrated = sc.calibrate(preds_test)
     ll_calib = log_loss(y_test, preds_test_calibrated)
 
-    bc1 = bc.BetaCalibration()
-    bc1.fit(preds_calib_set, y_calib_set)
-    bc_preds_test_calibrated = bc1.predict(preds_test)
-    bc_ll_calib = log_loss(y_test, bc_preds_test_calibrated)
-
-    assert(ll_calib<bc_ll_calib)
+    assert(ll_calib<0.151)
 
 def test_calibration_2dplanes_727_cb3():
     """
     We test the default settings and 
     ensure that the resulting log-loss gives good performance
 
     """
@@ -297,17 +242,12 @@
     preds_test = test_set.iloc[:,0].to_numpy()
     y_test = test_set.iloc[:,1].to_numpy()
     sc = splc.SplineCalib()
     sc.fit(preds_calib_set, y_calib_set)
     preds_test_calibrated = sc.calibrate(preds_test)
     ll_calib = log_loss(y_test, preds_test_calibrated)
 
-    bc1 = bc.BetaCalibration()
-    bc1.fit(preds_calib_set, y_calib_set)
-    bc_preds_test_calibrated = bc1.predict(preds_test)
-    bc_ll_calib = log_loss(y_test, bc_preds_test_calibrated)
-
-    assert(ll_calib<bc_ll_calib)
+    assert(ll_calib<0.167)
```

### Comparing `splinecalib-0.0.4/splinecalib/tests/test_multiclass_datasets.py` & `splinecalib-0.0.5/splinecalib/tests/test_multiclass_datasets.py`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib/tests/test_unity_prior.py` & `splinecalib-0.0.5/splinecalib/tests/test_unity_prior.py`

 * *Files identical despite different names*

### Comparing `splinecalib-0.0.4/splinecalib.egg-info/PKG-INFO` & `splinecalib-0.0.5/splinecalib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: splinecalib
-Version: 0.0.4
+Version: 0.0.5
 Summary: SplineCalib is a Python package for calibrating ML models using smoothing splines.  See documentation at: https://splinecalib.readthedocs.io/
 Home-page: https://github.com/numeristical/splinecalib
 Author: Brian Lucena
 Author-email: brianlucena@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.5
 License-File: LICENSE
 
 # splinecalib
 Location for the splinecalib package
-
-
```

### Comparing `splinecalib-0.0.4/splinecalib.egg-info/SOURCES.txt` & `splinecalib-0.0.5/splinecalib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 splinecalib/tests/data_for_tests/calibset_airlines_42493_cb2.csv
 splinecalib/tests/data_for_tests/calibset_airlines_42493_cb3.csv
 splinecalib/tests/data_for_tests/calibset_airlines_42493_rf.csv
 splinecalib/tests/data_for_tests/calibset_mozilla4_1046_cb1.csv
 splinecalib/tests/data_for_tests/calibset_mozilla4_1046_cb2.csv
 splinecalib/tests/data_for_tests/calibset_mozilla4_1046_cb3.csv
 splinecalib/tests/data_for_tests/calibset_mozilla4_1046_rf.csv
-splinecalib/tests/data_for_tests/mnist4_calib_set.csv
 splinecalib/tests/data_for_tests/mnist4_test_set.csv
 splinecalib/tests/data_for_tests/testset_2dplanes_727_cb1.csv
 splinecalib/tests/data_for_tests/testset_2dplanes_727_cb2.csv
 splinecalib/tests/data_for_tests/testset_2dplanes_727_cb3.csv
 splinecalib/tests/data_for_tests/testset_2dplanes_727_rf.csv
 splinecalib/tests/data_for_tests/testset_airlines_42493_cb1.csv
 splinecalib/tests/data_for_tests/testset_airlines_42493_cb2.csv
```

