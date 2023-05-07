# Comparing `tmp/xfields-0.9.3.tar.gz` & `tmp/xfields-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfields-0.9.3.tar", last modified: Mon Dec 19 18:09:18 2022, max compression
+gzip compressed data, was "xfields-0.9.4.tar", last modified: Tue Feb 21 16:19:14 2023, max compression
```

## Comparing `xfields-0.9.3.tar` & `xfields-0.9.4.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-12-19 18:09:18.472505 xfields-0.9.3/
--rw-r--r--   0 giadarol   (501) staff       (20)    11356 2022-06-24 09:16:10.000000 xfields-0.9.3/LICENSE
--rw-r--r--   0 giadarol   (501) staff       (20)      169 2021-11-28 06:28:52.000000 xfields-0.9.3/MANIFEST.in
--rw-r--r--   0 giadarol   (501) staff       (20)      604 2022-12-19 18:09:18.472107 xfields-0.9.3/PKG-INFO
--rw-r--r--   0 giadarol   (501) staff       (20)      115 2021-11-28 06:28:52.000000 xfields-0.9.3/README.md
--rw-r--r--   0 giadarol   (501) staff       (20)      115 2021-08-20 13:51:58.000000 xfields-0.9.3/pyproject.toml
--rw-r--r--   0 giadarol   (501) staff       (20)       38 2022-12-19 18:09:18.472633 xfields-0.9.3/setup.cfg
--rw-r--r--   0 giadarol   (501) staff       (20)     1630 2022-10-31 20:56:18.000000 xfields-0.9.3/setup.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-12-19 18:09:18.432481 xfields-0.9.3/xfields/
--rw-r--r--   0 giadarol   (501) staff       (20)     1494 2022-12-19 18:08:31.000000 xfields-0.9.3/xfields/__init__.py
--rw-r--r--   0 giadarol   (501) staff       (20)       22 2022-12-19 18:08:49.000000 xfields-0.9.3/xfields/_version.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-12-19 18:09:18.438208 xfields-0.9.3/xfields/beam_elements/
--rw-r--r--   0 giadarol   (501) staff       (20)      231 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/beam_elements/__init__.py
--rw-r--r--   0 giadarol   (501) staff       (20)     7930 2022-11-01 14:39:25.000000 xfields-0.9.3/xfields/beam_elements/beambeam2d.py
--rw-r--r--   0 giadarol   (501) staff       (20)    55874 2022-12-06 16:38:27.000000 xfields-0.9.3/xfields/beam_elements/beambeam3d.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-12-19 18:09:18.442356 xfields-0.9.3/xfields/beam_elements/beambeam_src/
--rw-r--r--   0 giadarol   (501) staff       (20)     1827 2022-08-13 07:48:47.000000 xfields-0.9.3/xfields/beam_elements/beambeam_src/beambeam.h
--rw-r--r--   0 giadarol   (501) staff       (20)     4493 2022-10-31 20:56:18.000000 xfields-0.9.3/xfields/beam_elements/beambeam_src/beambeam2d.h
--rw-r--r--   0 giadarol   (501) staff       (20)    11615 2022-11-30 14:38:54.000000 xfields-0.9.3/xfields/beam_elements/beambeam_src/beambeam3d.h
--rw-r--r--   0 giadarol   (501) staff       (20)     7358 2022-11-22 17:18:14.000000 xfields-0.9.3/xfields/beam_elements/beambeam_src/beambeam3d_methods_for_strongstrong.h
--rw-r--r--   0 giadarol   (501) staff       (20)     6471 2022-11-22 17:18:14.000000 xfields-0.9.3/xfields/beam_elements/beambeam_src/beambeam3d_ref_frame_changes.h
--rw-r--r--   0 giadarol   (501) staff       (20)     5276 2022-11-22 17:18:14.000000 xfields-0.9.3/xfields/beam_elements/beambeam_src/beambeam3d_transport_sigmas.h
--rw-r--r--   0 giadarol   (501) staff       (20)     4131 2022-08-13 07:48:56.000000 xfields-0.9.3/xfields/beam_elements/electroncloud.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-12-19 18:09:18.443187 xfields-0.9.3/xfields/beam_elements/electroncloud_src/
--rw-r--r--   0 giadarol   (501) staff       (20)     2147 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/beam_elements/electroncloud_src/electroncloud.h
--rw-r--r--   0 giadarol   (501) staff       (20)     5332 2022-08-13 07:48:56.000000 xfields-0.9.3/xfields/beam_elements/electronlens_interpolated.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-12-19 18:09:18.444409 xfields-0.9.3/xfields/beam_elements/electronlens_src/
--rw-r--r--   0 giadarol   (501) staff       (20)     2324 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/beam_elements/electronlens_src/electronlens_interpolated.h
--rw-r--r--   0 giadarol   (501) staff       (20)    12817 2022-11-01 14:39:25.000000 xfields-0.9.3/xfields/beam_elements/spacecharge.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-12-19 18:09:18.445640 xfields-0.9.3/xfields/beam_elements/spacecharge_src/
--rw-r--r--   0 giadarol   (501) staff       (20)     1930 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/beam_elements/spacecharge_src/spacecharge3d.h
--rw-r--r--   0 giadarol   (501) staff       (20)     1761 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/beam_elements/spacecharge_src/spacechargebigaussian.h
--rw-r--r--   0 giadarol   (501) staff       (20)    12282 2022-11-22 17:18:14.000000 xfields-0.9.3/xfields/beam_elements/temp_slicer.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-12-19 18:09:18.448279 xfields-0.9.3/xfields/config_tools/
--rw-r--r--   0 giadarol   (501) staff       (20)      353 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/config_tools/__init__.py
--rw-r--r--   0 giadarol   (501) staff       (20)     2870 2022-09-17 13:39:44.000000 xfields-0.9.3/xfields/config_tools/beambeam_config_tools.py
--rw-r--r--   0 giadarol   (501) staff       (20)     7376 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/config_tools/electroncloud_config_tools.py
--rw-r--r--   0 giadarol   (501) staff       (20)     7617 2022-08-13 07:48:56.000000 xfields-0.9.3/xfields/config_tools/spacecharge_config_tools.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-12-19 18:09:18.451191 xfields-0.9.3/xfields/fieldmaps/
--rw-r--r--   0 giadarol   (501) staff       (20)      369 2022-08-13 07:48:47.000000 xfields-0.9.3/xfields/fieldmaps/__init__.py
--rw-r--r--   0 giadarol   (501) staff       (20)     6569 2022-08-13 07:48:47.000000 xfields-0.9.3/xfields/fieldmaps/bigaussian.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-12-19 18:09:18.454774 xfields-0.9.3/xfields/fieldmaps/bigaussian_src/
--rw-r--r--   0 giadarol   (501) staff       (20)     4736 2022-11-22 17:18:14.000000 xfields-0.9.3/xfields/fieldmaps/bigaussian_src/bigaussian.h
--rw-r--r--   0 giadarol   (501) staff       (20)     1557 2022-11-22 17:18:14.000000 xfields-0.9.3/xfields/fieldmaps/bigaussian_src/compute_gx_gy.h
--rw-r--r--   0 giadarol   (501) staff       (20)      412 2022-11-01 14:39:25.000000 xfields-0.9.3/xfields/fieldmaps/bigaussian_src/faddeeva.h
--rw-r--r--   0 giadarol   (501) staff       (20)     9060 2022-11-01 14:39:25.000000 xfields-0.9.3/xfields/fieldmaps/bigaussian_src/faddeeva_cernlib.h
--rw-r--r--   0 giadarol   (501) staff       (20)   126939 2022-11-01 14:39:25.000000 xfields-0.9.3/xfields/fieldmaps/bigaussian_src/faddeeva_mit.h
--rw-r--r--   0 giadarol   (501) staff       (20)    25938 2022-08-13 07:48:56.000000 xfields-0.9.3/xfields/fieldmaps/interpolated.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-12-19 18:09:18.461037 xfields-0.9.3/xfields/fieldmaps/interpolated_src/
--rw-r--r--   0 giadarol   (501) staff       (20)      499 2021-08-20 13:51:58.000000 xfields-0.9.3/xfields/fieldmaps/interpolated_src/atomicadd.clh
--rw-r--r--   0 giadarol   (501) staff       (20)      383 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/fieldmaps/interpolated_src/atomicadd.h
--rw-r--r--   0 giadarol   (501) staff       (20)     1184 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/fieldmaps/interpolated_src/central_diff.h
--rw-r--r--   0 giadarol   (501) staff       (20)     5493 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/fieldmaps/interpolated_src/charge_deposition.h
--rw-r--r--   0 giadarol   (501) staff       (20)     6181 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/fieldmaps/interpolated_src/cubic_interpolators.h
--rw-r--r--   0 giadarol   (501) staff       (20)     4455 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/fieldmaps/interpolated_src/linear_interpolators.h
--rw-r--r--   0 giadarol   (501) staff       (20)    38318 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/fieldmaps/interpolated_src/tricubic_coefficients.h
--rw-r--r--   0 giadarol   (501) staff       (20)    20374 2022-08-13 07:48:56.000000 xfields-0.9.3/xfields/fieldmaps/tricubicinterpolated.py
--rw-r--r--   0 giadarol   (501) staff       (20)      263 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/general.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-12-19 18:09:18.464075 xfields-0.9.3/xfields/headers/
--rw-r--r--   0 giadarol   (501) staff       (20)     9132 2022-11-22 17:18:14.000000 xfields-0.9.3/xfields/headers/beamstrahlung_spectrum.h
--rw-r--r--   0 giadarol   (501) staff       (20)     1771 2022-11-22 17:18:14.000000 xfields-0.9.3/xfields/headers/constants.h
--rw-r--r--   0 giadarol   (501) staff       (20)     3685 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/headers/power_n.h
--rw-r--r--   0 giadarol   (501) staff       (20)     1710 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/headers/sincos.h
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-12-19 18:09:18.465756 xfields-0.9.3/xfields/longitudinal_profiles/
--rw-r--r--   0 giadarol   (501) staff       (20)      295 2022-08-13 07:48:47.000000 xfields-0.9.3/xfields/longitudinal_profiles/__init__.py
--rw-r--r--   0 giadarol   (501) staff       (20)      537 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/longitudinal_profiles/coasting.py
--rw-r--r--   0 giadarol   (501) staff       (20)     4951 2022-08-13 07:48:56.000000 xfields-0.9.3/xfields/longitudinal_profiles/qgaussian.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-12-19 18:09:18.466131 xfields-0.9.3/xfields/longitudinal_profiles/qgaussian_src/
--rw-r--r--   0 giadarol   (501) staff       (20)     2071 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/longitudinal_profiles/qgaussian_src/qgaussian.h
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-12-19 18:09:18.468138 xfields-0.9.3/xfields/solvers/
--rw-r--r--   0 giadarol   (501) staff       (20)      243 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/solvers/__init__.py
--rw-r--r--   0 giadarol   (501) staff       (20)      400 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/solvers/base.py
--rw-r--r--   0 giadarol   (501) staff       (20)     8363 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/solvers/fftsolvers.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-12-19 18:09:18.469536 xfields-0.9.3/xfields/test_support/
--rw-r--r--   0 giadarol   (501) staff       (20)      193 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/test_support/__init__.py
--rw-r--r--   0 giadarol   (501) staff       (20)     1648 2022-06-24 09:16:10.000000 xfields-0.9.3/xfields/test_support/temp_makepart.py
-drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2022-12-19 18:09:18.434472 xfields-0.9.3/xfields.egg-info/
--rw-r--r--   0 giadarol   (501) staff       (20)      604 2022-12-19 18:09:18.000000 xfields-0.9.3/xfields.egg-info/PKG-INFO
--rw-r--r--   0 giadarol   (501) staff       (20)     2508 2022-12-19 18:09:18.000000 xfields-0.9.3/xfields.egg-info/SOURCES.txt
--rw-r--r--   0 giadarol   (501) staff       (20)        1 2022-12-19 18:09:18.000000 xfields-0.9.3/xfields.egg-info/dependency_links.txt
--rw-r--r--   0 giadarol   (501) staff       (20)       70 2022-12-19 18:09:18.000000 xfields-0.9.3/xfields.egg-info/requires.txt
--rw-r--r--   0 giadarol   (501) staff       (20)        8 2022-12-19 18:09:18.000000 xfields-0.9.3/xfields.egg-info/top_level.txt
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2023-02-21 16:19:14.288213 xfields-0.9.4/
+-rw-r--r--   0 giadarol   (501) staff       (20)    11356 2022-06-24 09:16:10.000000 xfields-0.9.4/LICENSE
+-rw-r--r--   0 giadarol   (501) staff       (20)      169 2021-11-28 06:28:52.000000 xfields-0.9.4/MANIFEST.in
+-rw-r--r--   0 giadarol   (501) staff       (20)      604 2023-02-21 16:19:14.287908 xfields-0.9.4/PKG-INFO
+-rw-r--r--   0 giadarol   (501) staff       (20)      115 2021-11-28 06:28:52.000000 xfields-0.9.4/README.md
+-rw-r--r--   0 giadarol   (501) staff       (20)      115 2021-08-20 13:51:58.000000 xfields-0.9.4/pyproject.toml
+-rw-r--r--   0 giadarol   (501) staff       (20)       38 2023-02-21 16:19:14.288322 xfields-0.9.4/setup.cfg
+-rw-r--r--   0 giadarol   (501) staff       (20)     1630 2022-10-31 20:56:18.000000 xfields-0.9.4/setup.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2023-02-21 16:19:14.254796 xfields-0.9.4/xfields/
+-rw-r--r--   0 giadarol   (501) staff       (20)     1494 2023-02-21 16:18:44.000000 xfields-0.9.4/xfields/__init__.py
+-rw-r--r--   0 giadarol   (501) staff       (20)       22 2023-02-21 16:18:57.000000 xfields-0.9.4/xfields/_version.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2023-02-21 16:19:14.259501 xfields-0.9.4/xfields/beam_elements/
+-rw-r--r--   0 giadarol   (501) staff       (20)      231 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/beam_elements/__init__.py
+-rw-r--r--   0 giadarol   (501) staff       (20)     7989 2023-02-21 16:18:57.000000 xfields-0.9.4/xfields/beam_elements/beambeam2d.py
+-rw-r--r--   0 giadarol   (501) staff       (20)    55791 2023-02-21 16:18:57.000000 xfields-0.9.4/xfields/beam_elements/beambeam3d.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2023-02-21 16:19:14.263900 xfields-0.9.4/xfields/beam_elements/beambeam_src/
+-rw-r--r--   0 giadarol   (501) staff       (20)     1827 2022-08-13 07:48:47.000000 xfields-0.9.4/xfields/beam_elements/beambeam_src/beambeam.h
+-rw-r--r--   0 giadarol   (501) staff       (20)     4493 2022-10-31 20:56:18.000000 xfields-0.9.4/xfields/beam_elements/beambeam_src/beambeam2d.h
+-rw-r--r--   0 giadarol   (501) staff       (20)    11615 2023-01-03 20:12:27.000000 xfields-0.9.4/xfields/beam_elements/beambeam_src/beambeam3d.h
+-rw-r--r--   0 giadarol   (501) staff       (20)     7358 2022-11-22 17:18:14.000000 xfields-0.9.4/xfields/beam_elements/beambeam_src/beambeam3d_methods_for_strongstrong.h
+-rw-r--r--   0 giadarol   (501) staff       (20)     6471 2022-11-22 17:18:14.000000 xfields-0.9.4/xfields/beam_elements/beambeam_src/beambeam3d_ref_frame_changes.h
+-rw-r--r--   0 giadarol   (501) staff       (20)     5276 2022-11-22 17:18:14.000000 xfields-0.9.4/xfields/beam_elements/beambeam_src/beambeam3d_transport_sigmas.h
+-rw-r--r--   0 giadarol   (501) staff       (20)     4190 2023-02-21 16:18:57.000000 xfields-0.9.4/xfields/beam_elements/electroncloud.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2023-02-21 16:19:14.264670 xfields-0.9.4/xfields/beam_elements/electroncloud_src/
+-rw-r--r--   0 giadarol   (501) staff       (20)     2111 2023-02-21 16:18:57.000000 xfields-0.9.4/xfields/beam_elements/electroncloud_src/electroncloud.h
+-rw-r--r--   0 giadarol   (501) staff       (20)     5391 2023-02-21 16:18:57.000000 xfields-0.9.4/xfields/beam_elements/electronlens_interpolated.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2023-02-21 16:19:14.265178 xfields-0.9.4/xfields/beam_elements/electronlens_src/
+-rw-r--r--   0 giadarol   (501) staff       (20)     2340 2023-02-21 16:18:57.000000 xfields-0.9.4/xfields/beam_elements/electronlens_src/electronlens_interpolated.h
+-rw-r--r--   0 giadarol   (501) staff       (20)    12876 2023-02-21 16:18:57.000000 xfields-0.9.4/xfields/beam_elements/spacecharge.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2023-02-21 16:19:14.266398 xfields-0.9.4/xfields/beam_elements/spacecharge_src/
+-rw-r--r--   0 giadarol   (501) staff       (20)     1930 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/beam_elements/spacecharge_src/spacecharge3d.h
+-rw-r--r--   0 giadarol   (501) staff       (20)     1761 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/beam_elements/spacecharge_src/spacechargebigaussian.h
+-rw-r--r--   0 giadarol   (501) staff       (20)    12282 2022-11-22 17:18:14.000000 xfields-0.9.4/xfields/beam_elements/temp_slicer.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2023-02-21 16:19:14.268631 xfields-0.9.4/xfields/config_tools/
+-rw-r--r--   0 giadarol   (501) staff       (20)      353 2023-02-21 16:18:44.000000 xfields-0.9.4/xfields/config_tools/__init__.py
+-rw-r--r--   0 giadarol   (501) staff       (20)     2870 2023-02-21 16:18:44.000000 xfields-0.9.4/xfields/config_tools/beambeam_config_tools.py
+-rw-r--r--   0 giadarol   (501) staff       (20)     7454 2023-02-21 16:18:57.000000 xfields-0.9.4/xfields/config_tools/electroncloud_config_tools.py
+-rw-r--r--   0 giadarol   (501) staff       (20)     7572 2023-02-21 16:18:57.000000 xfields-0.9.4/xfields/config_tools/spacecharge_config_tools.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2023-02-21 16:19:14.270344 xfields-0.9.4/xfields/fieldmaps/
+-rw-r--r--   0 giadarol   (501) staff       (20)      369 2022-08-13 07:48:47.000000 xfields-0.9.4/xfields/fieldmaps/__init__.py
+-rw-r--r--   0 giadarol   (501) staff       (20)     6569 2022-08-13 07:48:47.000000 xfields-0.9.4/xfields/fieldmaps/bigaussian.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2023-02-21 16:19:14.273793 xfields-0.9.4/xfields/fieldmaps/bigaussian_src/
+-rw-r--r--   0 giadarol   (501) staff       (20)     4736 2022-11-22 17:18:14.000000 xfields-0.9.4/xfields/fieldmaps/bigaussian_src/bigaussian.h
+-rw-r--r--   0 giadarol   (501) staff       (20)     1557 2022-11-22 17:18:14.000000 xfields-0.9.4/xfields/fieldmaps/bigaussian_src/compute_gx_gy.h
+-rw-r--r--   0 giadarol   (501) staff       (20)      412 2022-11-01 14:39:25.000000 xfields-0.9.4/xfields/fieldmaps/bigaussian_src/faddeeva.h
+-rw-r--r--   0 giadarol   (501) staff       (20)     9060 2022-11-01 14:39:25.000000 xfields-0.9.4/xfields/fieldmaps/bigaussian_src/faddeeva_cernlib.h
+-rw-r--r--   0 giadarol   (501) staff       (20)   126939 2022-11-01 14:39:25.000000 xfields-0.9.4/xfields/fieldmaps/bigaussian_src/faddeeva_mit.h
+-rw-r--r--   0 giadarol   (501) staff       (20)    25938 2022-08-13 07:48:56.000000 xfields-0.9.4/xfields/fieldmaps/interpolated.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2023-02-21 16:19:14.280086 xfields-0.9.4/xfields/fieldmaps/interpolated_src/
+-rw-r--r--   0 giadarol   (501) staff       (20)      499 2021-08-20 13:51:58.000000 xfields-0.9.4/xfields/fieldmaps/interpolated_src/atomicadd.clh
+-rw-r--r--   0 giadarol   (501) staff       (20)      383 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/fieldmaps/interpolated_src/atomicadd.h
+-rw-r--r--   0 giadarol   (501) staff       (20)     1184 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/fieldmaps/interpolated_src/central_diff.h
+-rw-r--r--   0 giadarol   (501) staff       (20)     5493 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/fieldmaps/interpolated_src/charge_deposition.h
+-rw-r--r--   0 giadarol   (501) staff       (20)     6181 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/fieldmaps/interpolated_src/cubic_interpolators.h
+-rw-r--r--   0 giadarol   (501) staff       (20)     4455 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/fieldmaps/interpolated_src/linear_interpolators.h
+-rw-r--r--   0 giadarol   (501) staff       (20)    38318 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/fieldmaps/interpolated_src/tricubic_coefficients.h
+-rw-r--r--   0 giadarol   (501) staff       (20)    20374 2022-08-13 07:48:56.000000 xfields-0.9.4/xfields/fieldmaps/tricubicinterpolated.py
+-rw-r--r--   0 giadarol   (501) staff       (20)      263 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/general.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2023-02-21 16:19:14.283510 xfields-0.9.4/xfields/headers/
+-rw-r--r--   0 giadarol   (501) staff       (20)     9167 2023-02-21 16:18:57.000000 xfields-0.9.4/xfields/headers/beamstrahlung_spectrum.h
+-rw-r--r--   0 giadarol   (501) staff       (20)     1771 2022-11-22 17:18:14.000000 xfields-0.9.4/xfields/headers/constants.h
+-rw-r--r--   0 giadarol   (501) staff       (20)      367 2023-02-21 16:18:57.000000 xfields-0.9.4/xfields/headers/particle_states.h
+-rw-r--r--   0 giadarol   (501) staff       (20)     3685 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/headers/power_n.h
+-rw-r--r--   0 giadarol   (501) staff       (20)     1710 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/headers/sincos.h
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2023-02-21 16:19:14.285110 xfields-0.9.4/xfields/longitudinal_profiles/
+-rw-r--r--   0 giadarol   (501) staff       (20)      295 2022-08-13 07:48:47.000000 xfields-0.9.4/xfields/longitudinal_profiles/__init__.py
+-rw-r--r--   0 giadarol   (501) staff       (20)      537 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/longitudinal_profiles/coasting.py
+-rw-r--r--   0 giadarol   (501) staff       (20)     4951 2022-08-13 07:48:56.000000 xfields-0.9.4/xfields/longitudinal_profiles/qgaussian.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2023-02-21 16:19:14.285457 xfields-0.9.4/xfields/longitudinal_profiles/qgaussian_src/
+-rw-r--r--   0 giadarol   (501) staff       (20)     2071 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/longitudinal_profiles/qgaussian_src/qgaussian.h
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2023-02-21 16:19:14.286743 xfields-0.9.4/xfields/solvers/
+-rw-r--r--   0 giadarol   (501) staff       (20)      243 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/solvers/__init__.py
+-rw-r--r--   0 giadarol   (501) staff       (20)      400 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/solvers/base.py
+-rw-r--r--   0 giadarol   (501) staff       (20)     8363 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/solvers/fftsolvers.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2023-02-21 16:19:14.287456 xfields-0.9.4/xfields/test_support/
+-rw-r--r--   0 giadarol   (501) staff       (20)      193 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/test_support/__init__.py
+-rw-r--r--   0 giadarol   (501) staff       (20)     1648 2022-06-24 09:16:10.000000 xfields-0.9.4/xfields/test_support/temp_makepart.py
+drwxr-xr-x   0 giadarol   (501) staff       (20)        0 2023-02-21 16:19:14.256720 xfields-0.9.4/xfields.egg-info/
+-rw-r--r--   0 giadarol   (501) staff       (20)      604 2023-02-21 16:19:14.000000 xfields-0.9.4/xfields.egg-info/PKG-INFO
+-rw-r--r--   0 giadarol   (501) staff       (20)     2542 2023-02-21 16:19:14.000000 xfields-0.9.4/xfields.egg-info/SOURCES.txt
+-rw-r--r--   0 giadarol   (501) staff       (20)        1 2023-02-21 16:19:14.000000 xfields-0.9.4/xfields.egg-info/dependency_links.txt
+-rw-r--r--   0 giadarol   (501) staff       (20)       70 2023-02-21 16:19:14.000000 xfields-0.9.4/xfields.egg-info/requires.txt
+-rw-r--r--   0 giadarol   (501) staff       (20)        8 2023-02-21 16:19:14.000000 xfields-0.9.4/xfields.egg-info/top_level.txt
```

### Comparing `xfields-0.9.3/LICENSE` & `xfields-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/PKG-INFO` & `xfields-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xfields
-Version: 0.9.3
+Version: 0.9.4
 Summary: Field Maps and Particle In Cell
 Home-page: https://xsuite.readthedocs.io/
 Download-URL: https://pypi.python.org/pypi/xfields
 Author: G. Iadarola et al.
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
 Project-URL: Documentation, https://xsuite.readthedocs.io/
```

### Comparing `xfields-0.9.3/setup.py` & `xfields-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/__init__.py` & `xfields-0.9.4/xfields/__init__.py`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/beam_elements/beambeam2d.py` & `xfields-0.9.4/xfields/beam_elements/beambeam2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
     }
 
     _extra_c_sources= [
         _pkg_root.joinpath('headers/constants.h'),
         _pkg_root.joinpath('headers/sincos.h'),
         _pkg_root.joinpath('headers/power_n.h'),
+        _pkg_root.joinpath('headers','particle_states.h'),
         _pkg_root.joinpath('fieldmaps/bigaussian_src/faddeeva.h'),
         '#define NOFIELDMAP', #TODO Remove this workaround
         _pkg_root.joinpath('fieldmaps/bigaussian_src/bigaussian.h'),
         '#undef NOFIELDMAP', #TODO Remove this workaround
         _pkg_root.joinpath('beam_elements/beambeam_src/beambeam2d.h'),
     ]
```

### Comparing `xfields-0.9.3/xfields/beam_elements/beambeam3d.py` & `xfields-0.9.4/xfields/beam_elements/beambeam3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,28 +96,29 @@
 
     }
 
     _internal_record_class = BeamBeamBiGaussian3DRecord
 
     _rename = {'flag_beamstrahlung': '_flag_beamstrahlung'}
 
+    _depends_on = [xt.RandomUniform]
+
     _extra_c_sources= [
         _pkg_root.joinpath('headers/constants.h'),
         _pkg_root.joinpath('headers/sincos.h'),
         _pkg_root.joinpath('headers/power_n.h'),
+        _pkg_root.joinpath('headers','particle_states.h'),
         _pkg_root.joinpath('fieldmaps/bigaussian_src/faddeeva.h'),
         '#define NOFIELDMAP', #TODO Remove this workaround
         _pkg_root.joinpath('fieldmaps/bigaussian_src/bigaussian.h'),
         '#undef NOFIELDMAP', #TODO Remove this workaround
         _pkg_root.joinpath('beam_elements/beambeam_src/beambeam3d_transport_sigmas.h'),
         _pkg_root.joinpath('beam_elements/beambeam_src/beambeam3d_ref_frame_changes.h'),
 
         # beamstrahlung
-        xp.general._pkg_root.joinpath('random_number_generator/rng_src/base_rng.h'),
-        xp.general._pkg_root.joinpath('random_number_generator/rng_src/local_particle_rng.h'),
         _pkg_root.joinpath('headers/beamstrahlung_spectrum.h'),
 
         _pkg_root.joinpath('beam_elements/beambeam_src/beambeam3d.h'),
         _pkg_root.joinpath('beam_elements/beambeam_src/beambeam3d_methods_for_strongstrong.h'),
 
    ]
```

### Comparing `xfields-0.9.3/xfields/beam_elements/beambeam_src/beambeam.h` & `xfields-0.9.4/xfields/beam_elements/beambeam_src/beambeam.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/beam_elements/beambeam_src/beambeam2d.h` & `xfields-0.9.4/xfields/beam_elements/beambeam_src/beambeam2d.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/beam_elements/beambeam_src/beambeam3d.h` & `xfields-0.9.4/xfields/beam_elements/beambeam_src/beambeam3d.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/beam_elements/beambeam_src/beambeam3d_methods_for_strongstrong.h` & `xfields-0.9.4/xfields/beam_elements/beambeam_src/beambeam3d_methods_for_strongstrong.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/beam_elements/beambeam_src/beambeam3d_ref_frame_changes.h` & `xfields-0.9.4/xfields/beam_elements/beambeam_src/beambeam3d_ref_frame_changes.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/beam_elements/beambeam_src/beambeam3d_transport_sigmas.h` & `xfields-0.9.4/xfields/beam_elements/beambeam_src/beambeam3d_transport_sigmas.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/beam_elements/electroncloud.py` & `xfields-0.9.4/xfields/beam_elements/electroncloud.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         'dipolar_ptau_kick': xo.Float64,
         'length': xo.Float64,
         #'fieldmap': TriCubicInterpolatedFieldMapData,
         'fieldmap': xo.Ref(TriCubicInterpolatedFieldMap._XoStruct),
         }
 
     _extra_c_sources = [
+        _pkg_root.joinpath('headers','particle_states.h'),
         _pkg_root.joinpath('fieldmaps/interpolated_src/tricubic_coefficients.h'),
         _pkg_root.joinpath('fieldmaps/interpolated_src/cubic_interpolators.h'),
         _pkg_root.joinpath('beam_elements/electroncloud_src/electroncloud.h'),
     ]
 
     def __init__(self,
                  _context=None,
```

### Comparing `xfields-0.9.3/xfields/beam_elements/electroncloud_src/electroncloud.h` & `xfields-0.9.4/xfields/beam_elements/electroncloud_src/electroncloud.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,27 +20,26 @@
     TriCubicInterpolatedFieldMapData fmap = ElectronCloudData_getp_fieldmap(el);
     //start_per_particle_block (part0->part)
     const double x = LocalParticle_get_x(part);
     const double y = LocalParticle_get_y(part);
     const double zeta = LocalParticle_get_zeta(part);
 
     double const beta0 = LocalParticle_get_beta0(part);
-    double const rvv = LocalParticle_get_rvv(part);
 
     double const tau = zeta / beta0;
 
     double dphi_dx=0;
     double dphi_dy=0;
     double dphi_dtau=0;
 
     if( TriCubicInterpolatedFieldMap_interpolate_grad(fmap,
         x - x_shift, y - y_shift, tau - tau_shift,
         &dphi_dx, &dphi_dy, &dphi_dtau)
       ){
-          LocalParticle_set_state(part, -11); // Stop tracking particle if it escapes the interpolation grid.
+          LocalParticle_set_state(part, XF_OUTSIDE_INTERPOL); // Stop tracking particle if it escapes the interpolation grid.
       }
 
     const double px_kick = - dphi_dx * length - ElectronCloudData_get_dipolar_px_kick(el);
     const double py_kick = - dphi_dy * length - ElectronCloudData_get_dipolar_py_kick(el);
     const double ptau_kick = - dphi_dtau * length - ElectronCloudData_get_dipolar_ptau_kick(el);
 
     // TODO: implement kicks for particles with different charge and or mass
```

### Comparing `xfields-0.9.3/xfields/beam_elements/electronlens_interpolated.py` & `xfields-0.9.4/xfields/beam_elements/electronlens_interpolated.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
                'current':  xo.Float64,
                'length':   xo.Float64,
                'voltage':  xo.Float64,
                "fieldmap": TriCubicInterpolatedFieldMap,
               }
 
     _extra_c_sources = [
+        _pkg_root.joinpath('headers','particle_states.h'),
         _pkg_root.joinpath('fieldmaps/interpolated_src/tricubic_coefficients.h'),
         _pkg_root.joinpath('fieldmaps/interpolated_src/cubic_interpolators.h'),
         _pkg_root.joinpath('beam_elements/electronlens_src/electronlens_interpolated.h'),
     ]
 
     def __init__(self,
                  _context=None,
```

### Comparing `xfields-0.9.3/xfields/beam_elements/electronlens_src/electronlens_interpolated.h` & `xfields-0.9.4/xfields/beam_elements/electronlens_src/electronlens_interpolated.h`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         double dphi_dy=0;
         double dphi_dtau=0;
         
         if( TriCubicInterpolatedFieldMap_interpolate_grad(fmap, 
             x, y, 0.,
             &dphi_dx, &dphi_dy, &dphi_dtau)
           ){
-              LocalParticle_set_state(part, -11); // Stop tracking particle if it escapes the interpolation grid.
+              LocalParticle_set_state(part, XF_OUTSIDE_INTERPOL); // Stop tracking particle if it escapes the interpolation grid.
           }
 
 	    const double q0 = LocalParticle_get_q0(part);
 	    const double mass0 = LocalParticle_get_mass0(part);
 	    //const double chi = LocalParticle_get_chi(part);
 	    const double beta0 = LocalParticle_get_beta0(part);
 	    const double gamma0 = LocalParticle_get_gamma0(part);
```

### Comparing `xfields-0.9.3/xfields/beam_elements/spacecharge.py` & `xfields-0.9.4/xfields/beam_elements/spacecharge.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     _xofields = {
         'fieldmap': xo.Ref(TriLinearInterpolatedFieldMap),
         'length': xo.Float64,
         }
 
     _extra_c_sources = [
         _pkg_root.joinpath('headers/constants.h'),
+        _pkg_root.joinpath('headers','particle_states.h'),
         _pkg_root.joinpath('fieldmaps/interpolated_src/linear_interpolators.h'),
         _pkg_root.joinpath('beam_elements/spacecharge_src/spacecharge3d.h'),
     ]
 
     def copy(self, _context=None, _buffer=None, _offset=None):
         if _buffer is not self._buffer:
             raise NotImplementedError
```

### Comparing `xfields-0.9.3/xfields/beam_elements/spacecharge_src/spacecharge3d.h` & `xfields-0.9.4/xfields/beam_elements/spacecharge_src/spacecharge3d.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/beam_elements/spacecharge_src/spacechargebigaussian.h` & `xfields-0.9.4/xfields/beam_elements/spacecharge_src/spacechargebigaussian.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/beam_elements/temp_slicer.py` & `xfields-0.9.4/xfields/beam_elements/temp_slicer.py`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/config_tools/beambeam_config_tools.py` & `xfields-0.9.4/xfields/config_tools/beambeam_config_tools.py`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/config_tools/electroncloud_config_tools.py` & `xfields-0.9.4/xfields/config_tools/electroncloud_config_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                                                 iy1:iy2, :].transpose(1, 0, 2)
         for ll in range(8):
             phi_slice[:, :, ll] *= scale[ll]
         index_offset = 8 * nx * ny * (iz - iz1)
         len_slice = phi_slice.shape[0] * \
             phi_slice.shape[1] * phi_slice.shape[2]
         fieldmap._phi_taylor[index_offset:index_offset +
-                             len_slice] = phi_slice.flatten()
+                             len_slice] = fieldmap._context.nparray_to_context_array(phi_slice.flatten())
     ##########################################################################
     # for iz in range(iz1, iz2):
     #     if (iz-iz1)/nz > kk:
     #         while (iz-iz1)/nz > kk:
     #             kk += 0.1
     #         print(f"{int(np.round(100*kk)):d}%..")
     #     phi_slice = ff[f"slices/slice{iz}/phi"][ix1:ix2, iy1:iy2,:]
@@ -115,15 +115,15 @@
         assert fieldmaps is not None
         for key in fieldmaps.keys():
             fieldmap = fieldmaps[key]
             dipolar_kicks[key] = electroncloud_dipolar_kicks_of_fieldmap(
                 fieldmap=fieldmap, p0c=line.particle_ref.p0c)
 
     length_factor = ecloud_strength / \
-        (line.particle_ref.p0c * line.particle_ref.beta0)
+        (line.particle_ref.p0c[0] * line.particle_ref.beta0[0])
     part = twiss["particle_on_co"].copy()
     for ii, el_name in enumerate(twiss["name"]):
         if 'ecloud' in el_name:
             # naming format is "ecloud.ecloud_type.sector.index_in_sector",
             # e.g.  ecloud.mb.78.38
             ecloud_type = el_name.split(".")[1]
             length = ecloud_info[ecloud_type][el_name]["length"] * \
@@ -146,15 +146,15 @@
 
 
 def electroncloud_dipolar_kicks_of_fieldmap(fieldmap=None, p0c=None):
 
     assert p0c is not None
     assert fieldmap is not None
 
-    part = xp.Particles(p0c=p0c)
+    part = xp.Particles(_context=fieldmap._context, p0c=p0c)
     ecloud = xf.ElectronCloud(
         length=1,
         fieldmap=fieldmap,
         _buffer=fieldmap._buffer)
     ecloud.track(part)
     px = part.px[0]
     py = part.py[0]
```

### Comparing `xfields-0.9.3/xfields/config_tools/spacecharge_config_tools.py` & `xfields-0.9.4/xfields/config_tools/spacecharge_config_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import pandas as pd
 
 from ..beam_elements.spacecharge import SpaceChargeBiGaussian
 from ..beam_elements.spacecharge import SpaceCharge3D
 
 import xpart as xp
 import xtrack as xt
-from xtrack.line import _is_thick, _is_drift
 
 def install_spacecharge_frozen(line, particle_ref, longitudinal_profile,
                                nemitt_x, nemitt_y, sigma_z,
                                num_spacecharge_interactions,
                                tol_spacecharge_position,
                                s_spacecharge=None):
```

### Comparing `xfields-0.9.3/xfields/fieldmaps/bigaussian.py` & `xfields-0.9.4/xfields/fieldmaps/bigaussian.py`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/fieldmaps/bigaussian_src/bigaussian.h` & `xfields-0.9.4/xfields/fieldmaps/bigaussian_src/bigaussian.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/fieldmaps/bigaussian_src/compute_gx_gy.h` & `xfields-0.9.4/xfields/fieldmaps/bigaussian_src/compute_gx_gy.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/fieldmaps/bigaussian_src/faddeeva_cernlib.h` & `xfields-0.9.4/xfields/fieldmaps/bigaussian_src/faddeeva_cernlib.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/fieldmaps/bigaussian_src/faddeeva_mit.h` & `xfields-0.9.4/xfields/fieldmaps/bigaussian_src/faddeeva_mit.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/fieldmaps/interpolated.py` & `xfields-0.9.4/xfields/fieldmaps/interpolated.py`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/fieldmaps/interpolated_src/central_diff.h` & `xfields-0.9.4/xfields/fieldmaps/interpolated_src/central_diff.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/fieldmaps/interpolated_src/charge_deposition.h` & `xfields-0.9.4/xfields/fieldmaps/interpolated_src/charge_deposition.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/fieldmaps/interpolated_src/cubic_interpolators.h` & `xfields-0.9.4/xfields/fieldmaps/interpolated_src/cubic_interpolators.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/fieldmaps/interpolated_src/linear_interpolators.h` & `xfields-0.9.4/xfields/fieldmaps/interpolated_src/linear_interpolators.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/fieldmaps/interpolated_src/tricubic_coefficients.h` & `xfields-0.9.4/xfields/fieldmaps/interpolated_src/tricubic_coefficients.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/fieldmaps/tricubicinterpolated.py` & `xfields-0.9.4/xfields/fieldmaps/tricubicinterpolated.py`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/headers/beamstrahlung_spectrum.h` & `xfields-0.9.4/xfields/headers/beamstrahlung_spectrum.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,20 +30,20 @@
     double xcrit = c1 * pow(energy*1e-9, 2.0) * rho_inv;  // [1] ecrit/E magnitude of quantum correction, in guineapig: xcrit (C) = ξ (doc) = upsbar (C++)
     (*ecrit) = xcrit * energy*1e-9;  // [GeV]
     //double omega_crit = (*ecrit)/HBAR_GEVS;  // [1/s] = 1.5 * gamma**3 * cst.c / rho
     //double upsilon = 2.0/3.0 * (*ecrit) / (energy*1e-9);  // [1] beamstrahlung parameter for single macropart
     double p0 = 25.4 * energy*1e-9 * dz * rho_inv;  // [1]  Fr * dz, specific for 1 macropart
  
     // eliminate region A in p0*g-v plane (=normalize with p0 = reject 1-p0 (p0<1) fraction of cases = y axis of p0*g-v plane is now spanning 0--p0=1
-    if (LocalParticle_generate_random_double(part) > p0){return 0;}
+    if (RandomUniform_generate(part) > p0){return 0;}
 
     // 2 random numbers to calculate g(v, xcrit)
-    double p = LocalParticle_generate_random_double(part);  // if this is 1, then it corresponds to p0 on original p0*g-v plane
+    double p = RandomUniform_generate(part);  // if this is 1, then it corresponds to p0 on original p0*g-v plane
     double v;
-    while((v=LocalParticle_generate_random_double(part))==0); // draw a nonzero random number, variable of the beamstrahlung spectrum
+    while((v=RandomUniform_generate(part))==0); // draw a nonzero random number, variable of the beamstrahlung spectrum
     double v2 = v*v;
     double v3 = v2*v;
     double y = v3 / (1.0 - v3);
     double denom = 1.0 - ( 1.0 - xcrit ) * v3;
 
     // calculate beamstrahlung spectrum coefficients, depending the value of y
     double g1, g2;
@@ -144,35 +144,35 @@
             // update bending radius, macropart energy and gamma
             rho_inv *= energy/(energy - e_photon*1e9);
             energy  -= e_photon*1e9;
             gamma   *= (energy - e_photon*1e9)/energy;
 
             // some error handling
             if (e_photon_array[j]<=0.0){
-		printf("photon emitted with negative energy: E_photon=%g [eV], E_macropart=%g [eV], photon ID: %d, max_photons: %d\n", e_photon*1e9, energy, j, max_photons);
-       	    }
+                printf("photon emitted with negative energy: E_photon=%g [eV], E_macropart=%g [eV], photon ID: %d, max_photons: %d\n", e_photon*1e9, energy, j, max_photons);
+            }
 
             // increment photon counter
             j++;
 
             // break loop and flag part as dead
-       	    if (j>=1000){
-	    	printf("too many photons produced by one particle (photon ID: %d)\n", j);
-	    	//exit(-1);  // doesnt work on GPU
-                LocalParticle_set_state(part, -12); // used to flag this kind of loss
+            if (j>=1000){
+                printf("too many photons produced by one particle (photon ID: %d)\n", j);
+                //exit(-1);  // doesnt work on GPU
+                LocalParticle_set_state(part, XF_TOO_MANY_PHOTONS); // used to flag this kind of loss
                 break;
-	    }
+            }
 
         }
     }
 
 
     // update electron energy
     if (energy == 0.0){
-        LocalParticle_set_state(part, -12); // used to flag this kind of loss
+        LocalParticle_set_state(part, XT_LOST_ALL_E_IN_SYNRAD); // used to flag this kind of loss
     }else{
        LocalParticle_add_to_energy(part, energy-initial_energy, 0);
     }
     double energy_loss = energy-initial_energy;
 
     return energy_loss;
 }
```

### Comparing `xfields-0.9.3/xfields/headers/constants.h` & `xfields-0.9.4/xfields/headers/constants.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/headers/power_n.h` & `xfields-0.9.4/xfields/headers/power_n.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/headers/sincos.h` & `xfields-0.9.4/xfields/headers/sincos.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/longitudinal_profiles/coasting.py` & `xfields-0.9.4/xfields/longitudinal_profiles/coasting.py`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/longitudinal_profiles/qgaussian.py` & `xfields-0.9.4/xfields/longitudinal_profiles/qgaussian.py`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/longitudinal_profiles/qgaussian_src/qgaussian.h` & `xfields-0.9.4/xfields/longitudinal_profiles/qgaussian_src/qgaussian.h`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/solvers/fftsolvers.py` & `xfields-0.9.4/xfields/solvers/fftsolvers.py`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields/test_support/temp_makepart.py` & `xfields-0.9.4/xfields/test_support/temp_makepart.py`

 * *Files identical despite different names*

### Comparing `xfields-0.9.3/xfields.egg-info/PKG-INFO` & `xfields-0.9.4/xfields.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xfields
-Version: 0.9.3
+Version: 0.9.4
 Summary: Field Maps and Particle In Cell
 Home-page: https://xsuite.readthedocs.io/
 Download-URL: https://pypi.python.org/pypi/xfields
 Author: G. Iadarola et al.
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
 Project-URL: Documentation, https://xsuite.readthedocs.io/
```

### Comparing `xfields-0.9.3/xfields.egg-info/SOURCES.txt` & `xfields-0.9.4/xfields.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 xfields/fieldmaps/interpolated_src/central_diff.h
 xfields/fieldmaps/interpolated_src/charge_deposition.h
 xfields/fieldmaps/interpolated_src/cubic_interpolators.h
 xfields/fieldmaps/interpolated_src/linear_interpolators.h
 xfields/fieldmaps/interpolated_src/tricubic_coefficients.h
 xfields/headers/beamstrahlung_spectrum.h
 xfields/headers/constants.h
+xfields/headers/particle_states.h
 xfields/headers/power_n.h
 xfields/headers/sincos.h
 xfields/longitudinal_profiles/__init__.py
 xfields/longitudinal_profiles/coasting.py
 xfields/longitudinal_profiles/qgaussian.py
 xfields/longitudinal_profiles/qgaussian_src/qgaussian.h
 xfields/solvers/__init__.py
```

