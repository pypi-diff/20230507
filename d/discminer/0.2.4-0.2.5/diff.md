# Comparing `tmp/discminer-0.2.4.tar.gz` & `tmp/discminer-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discminer-0.2.4.tar", last modified: Wed May  3 16:14:58 2023, max compression
+gzip compressed data, was "discminer-0.2.5.tar", last modified: Sun May  7 20:54:46 2023, max compression
```

## Comparing `discminer-0.2.4.tar` & `discminer-0.2.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-03 16:14:58.946268 discminer-0.2.4/
--rw-r--r--   0 aizquier  (8218)     5000     1074 2022-01-26 21:14:15.000000 discminer-0.2.4/LICENSE
--rw-r--r--   0 aizquier  (8218)     5000     7128 2023-05-03 16:14:58.946473 discminer-0.2.4/PKG-INFO
--rw-r--r--   0 aizquier  (8218)     5000     5343 2023-04-04 12:11:03.000000 discminer-0.2.4/README.md
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-03 16:14:58.920117 discminer-0.2.4/_mining/
--rw-r--r--   0 aizquier  (8218)     5000     5015 2023-04-21 12:25:29.000000 discminer-0.2.4/_mining/make_channels.py
--rw-r--r--   0 aizquier  (8218)     5000    10743 2023-04-03 12:56:52.000000 discminer-0.2.4/_mining/make_parfile.py
--rw-r--r--   0 aizquier  (8218)     5000     1057 2023-04-03 09:02:09.000000 discminer-0.2.4/_mining/make_single_moments.py
--rw-r--r--   0 aizquier  (8218)     5000     3447 2023-04-15 07:27:55.000000 discminer-0.2.4/_mining/plot_attributes_model.py
--rw-r--r--   0 aizquier  (8218)     5000     4007 2023-04-13 16:59:47.000000 discminer-0.2.4/_mining/plot_azimuthal_profiles.py
--rw-r--r--   0 aizquier  (8218)     5000     4476 2023-04-13 17:30:46.000000 discminer-0.2.4/_mining/plot_moment+offset.py
--rw-r--r--   0 aizquier  (8218)     5000     4425 2023-04-13 17:30:39.000000 discminer-0.2.4/_mining/plot_moment+residuals.py
--rw-r--r--   0 aizquier  (8218)     5000     6146 2023-04-14 21:07:52.000000 discminer-0.2.4/_mining/plot_peak_residuals.py
--rw-r--r--   0 aizquier  (8218)     5000    11249 2023-04-13 17:34:25.000000 discminer-0.2.4/_mining/plot_radial_profiles.py
--rw-r--r--   0 aizquier  (8218)     5000     5628 2023-04-13 17:29:19.000000 discminer-0.2.4/_mining/plot_residuals+all.py
--rw-r--r--   0 aizquier  (8218)     5000     4711 2023-04-13 17:41:59.000000 discminer-0.2.4/_mining/plot_residuals+deproj.py
--rw-r--r--   0 aizquier  (8218)     5000    10461 2023-04-21 12:25:57.000000 discminer-0.2.4/_mining/utils.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-03 16:14:58.932706 discminer-0.2.4/discminer/
--rw-r--r--   0 aizquier  (8218)     5000       34 2023-04-03 15:53:12.000000 discminer-0.2.4/discminer/__init__.py
--rw-r--r--   0 aizquier  (8218)     5000       22 2023-05-03 16:11:57.000000 discminer-0.2.4/discminer/_version.py
--rw-r--r--   0 aizquier  (8218)     5000     1812 2023-02-12 15:59:29.000000 discminer-0.2.4/discminer/cart.py
--rw-r--r--   0 aizquier  (8218)     5000      456 2022-11-24 22:45:25.000000 discminer-0.2.4/discminer/constants.py
--rw-r--r--   0 aizquier  (8218)     5000     8161 2023-04-26 17:22:27.000000 discminer-0.2.4/discminer/core.py
--rw-r--r--   0 aizquier  (8218)     5000    74149 2023-04-26 17:12:45.000000 discminer-0.2.4/discminer/cube.py
--rw-r--r--   0 aizquier  (8218)     5000    71090 2023-04-26 17:32:34.000000 discminer-0.2.4/discminer/disc2d.py
--rw-r--r--   0 aizquier  (8218)     5000     4147 2023-04-13 13:36:17.000000 discminer-0.2.4/discminer/grid.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-03 16:14:58.939831 discminer-0.2.4/discminer/icons/
--rw-r--r--   0 aizquier  (8218)     5000    19647 2021-06-29 11:43:47.000000 discminer-0.2.4/discminer/icons/button_box.png
--rw-r--r--   0 aizquier  (8218)     5000    72205 2021-06-29 11:43:47.000000 discminer-0.2.4/discminer/icons/button_cursor.jpeg
--rw-r--r--   0 aizquier  (8218)     5000    39306 2022-02-22 03:18:26.000000 discminer-0.2.4/discminer/icons/button_path.png
--rw-r--r--   0 aizquier  (8218)     5000    12142 2022-02-22 03:26:08.000000 discminer-0.2.4/discminer/icons/button_return.png
--rw-r--r--   0 aizquier  (8218)     5000   110584 2021-06-29 11:43:47.000000 discminer-0.2.4/discminer/icons/button_surface.png
--rw-r--r--   0 aizquier  (8218)     5000    11838 2021-06-29 11:43:47.000000 discminer-0.2.4/discminer/icons/button_trash.jpg
--rw-r--r--   0 aizquier  (8218)     5000      336 2021-06-29 11:43:47.000000 discminer-0.2.4/discminer/icons/logo.txt
--rw-r--r--   0 aizquier  (8218)     5000    12931 2023-04-02 20:42:03.000000 discminer-0.2.4/discminer/pick.py
--rw-r--r--   0 aizquier  (8218)     5000    29828 2023-05-03 15:29:17.000000 discminer-0.2.4/discminer/plottools.py
--rw-r--r--   0 aizquier  (8218)     5000    36007 2023-05-03 15:09:48.000000 discminer-0.2.4/discminer/rail.py
--rw-r--r--   0 aizquier  (8218)     5000   160740 2022-01-27 11:46:40.000000 discminer-0.2.4/discminer/testyapf.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-03 16:14:58.942021 discminer-0.2.4/discminer/tools/
--rw-r--r--   0 aizquier  (8218)     5000      569 2023-03-16 20:41:38.000000 discminer-0.2.4/discminer/tools/discminer.mplstyle
--rw-r--r--   0 aizquier  (8218)     5000    16972 2023-04-03 09:18:56.000000 discminer-0.2.4/discminer/tools/fit_kernel.py
--rw-r--r--   0 aizquier  (8218)     5000     6997 2023-04-04 09:09:51.000000 discminer-0.2.4/discminer/tools/utils.py
--rw-r--r--   0 aizquier  (8218)     5000      411 2022-11-24 22:45:39.000000 discminer-0.2.4/discminer/units.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-03 16:14:58.934418 discminer-0.2.4/discminer.egg-info/
--rw-r--r--   0 aizquier  (8218)     5000     7128 2023-05-03 16:14:58.000000 discminer-0.2.4/discminer.egg-info/PKG-INFO
--rw-r--r--   0 aizquier  (8218)     5000     1284 2023-05-03 16:14:58.000000 discminer-0.2.4/discminer.egg-info/SOURCES.txt
--rw-r--r--   0 aizquier  (8218)     5000        1 2023-05-03 16:14:58.000000 discminer-0.2.4/discminer.egg-info/dependency_links.txt
--rw-r--r--   0 aizquier  (8218)     5000      108 2023-05-03 16:14:58.000000 discminer-0.2.4/discminer.egg-info/requires.txt
--rw-r--r--   0 aizquier  (8218)     5000       10 2023-05-03 16:14:58.000000 discminer-0.2.4/discminer.egg-info/top_level.txt
--rw-r--r--   0 aizquier  (8218)     5000      151 2023-04-03 21:10:19.000000 discminer-0.2.4/pyproject.toml
--rw-r--r--   0 aizquier  (8218)     5000       74 2023-05-03 16:14:58.946931 discminer-0.2.4/setup.cfg
--rw-r--r--   0 aizquier  (8218)     5000     3219 2023-04-03 21:16:45.000000 discminer-0.2.4/setup.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-03 16:14:58.945362 discminer-0.2.4/template/
--rw-r--r--   0 aizquier  (8218)     5000     8550 2023-04-15 07:40:20.000000 discminer-0.2.4/template/README.rst
--rw-r--r--   0 aizquier  (8218)     5000     5072 2022-01-02 19:37:02.000000 discminer-0.2.4/template/download_MAPS.sh
--rw-r--r--   0 aizquier  (8218)     5000     1019 2023-04-03 09:07:58.000000 discminer-0.2.4/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt
--rw-r--r--   0 aizquier  (8218)     5000      617 2023-04-03 08:37:18.000000 discminer-0.2.4/template/prepare_data.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-07 20:54:46.481751 discminer-0.2.5/
+-rw-r--r--   0 aizquier  (8218)     5000     1074 2022-01-26 21:14:15.000000 discminer-0.2.5/LICENSE
+-rw-r--r--   0 aizquier  (8218)     5000     7128 2023-05-07 20:54:46.481951 discminer-0.2.5/PKG-INFO
+-rw-r--r--   0 aizquier  (8218)     5000     5343 2023-04-04 12:11:03.000000 discminer-0.2.5/README.md
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-07 20:54:46.456936 discminer-0.2.5/_mining/
+-rw-r--r--   0 aizquier  (8218)     5000     5015 2023-04-21 12:25:29.000000 discminer-0.2.5/_mining/make_channels.py
+-rw-r--r--   0 aizquier  (8218)     5000    10743 2023-04-03 12:56:52.000000 discminer-0.2.5/_mining/make_parfile.py
+-rw-r--r--   0 aizquier  (8218)     5000     1057 2023-04-03 09:02:09.000000 discminer-0.2.5/_mining/make_single_moments.py
+-rw-r--r--   0 aizquier  (8218)     5000     3447 2023-04-15 07:27:55.000000 discminer-0.2.5/_mining/plot_attributes_model.py
+-rw-r--r--   0 aizquier  (8218)     5000     4007 2023-04-13 16:59:47.000000 discminer-0.2.5/_mining/plot_azimuthal_profiles.py
+-rw-r--r--   0 aizquier  (8218)     5000     4476 2023-04-13 17:30:46.000000 discminer-0.2.5/_mining/plot_moment+offset.py
+-rw-r--r--   0 aizquier  (8218)     5000     4425 2023-04-13 17:30:39.000000 discminer-0.2.5/_mining/plot_moment+residuals.py
+-rw-r--r--   0 aizquier  (8218)     5000     6146 2023-04-14 21:07:52.000000 discminer-0.2.5/_mining/plot_peak_residuals.py
+-rw-r--r--   0 aizquier  (8218)     5000    11249 2023-04-13 17:34:25.000000 discminer-0.2.5/_mining/plot_radial_profiles.py
+-rw-r--r--   0 aizquier  (8218)     5000     5628 2023-04-13 17:29:19.000000 discminer-0.2.5/_mining/plot_residuals+all.py
+-rw-r--r--   0 aizquier  (8218)     5000     4711 2023-04-13 17:41:59.000000 discminer-0.2.5/_mining/plot_residuals+deproj.py
+-rw-r--r--   0 aizquier  (8218)     5000    10461 2023-04-21 12:25:57.000000 discminer-0.2.5/_mining/utils.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-07 20:54:46.468196 discminer-0.2.5/discminer/
+-rw-r--r--   0 aizquier  (8218)     5000       34 2023-04-03 15:53:12.000000 discminer-0.2.5/discminer/__init__.py
+-rw-r--r--   0 aizquier  (8218)     5000       22 2023-05-07 20:52:36.000000 discminer-0.2.5/discminer/_version.py
+-rw-r--r--   0 aizquier  (8218)     5000     2069 2023-05-05 17:33:30.000000 discminer-0.2.5/discminer/cart.py
+-rw-r--r--   0 aizquier  (8218)     5000      456 2022-11-24 22:45:25.000000 discminer-0.2.5/discminer/constants.py
+-rw-r--r--   0 aizquier  (8218)     5000     8161 2023-04-26 17:22:27.000000 discminer-0.2.5/discminer/core.py
+-rw-r--r--   0 aizquier  (8218)     5000    74149 2023-04-26 17:12:45.000000 discminer-0.2.5/discminer/cube.py
+-rw-r--r--   0 aizquier  (8218)     5000    71090 2023-04-26 17:32:34.000000 discminer-0.2.5/discminer/disc2d.py
+-rw-r--r--   0 aizquier  (8218)     5000     4147 2023-04-13 13:36:17.000000 discminer-0.2.5/discminer/grid.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-07 20:54:46.475297 discminer-0.2.5/discminer/icons/
+-rw-r--r--   0 aizquier  (8218)     5000    19647 2021-06-29 11:43:47.000000 discminer-0.2.5/discminer/icons/button_box.png
+-rw-r--r--   0 aizquier  (8218)     5000    72205 2021-06-29 11:43:47.000000 discminer-0.2.5/discminer/icons/button_cursor.jpeg
+-rw-r--r--   0 aizquier  (8218)     5000    39306 2022-02-22 03:18:26.000000 discminer-0.2.5/discminer/icons/button_path.png
+-rw-r--r--   0 aizquier  (8218)     5000    12142 2022-02-22 03:26:08.000000 discminer-0.2.5/discminer/icons/button_return.png
+-rw-r--r--   0 aizquier  (8218)     5000   110584 2021-06-29 11:43:47.000000 discminer-0.2.5/discminer/icons/button_surface.png
+-rw-r--r--   0 aizquier  (8218)     5000    11838 2021-06-29 11:43:47.000000 discminer-0.2.5/discminer/icons/button_trash.jpg
+-rw-r--r--   0 aizquier  (8218)     5000      336 2021-06-29 11:43:47.000000 discminer-0.2.5/discminer/icons/logo.txt
+-rw-r--r--   0 aizquier  (8218)     5000    12931 2023-04-02 20:42:03.000000 discminer-0.2.5/discminer/pick.py
+-rw-r--r--   0 aizquier  (8218)     5000    31514 2023-05-07 20:50:53.000000 discminer-0.2.5/discminer/plottools.py
+-rw-r--r--   0 aizquier  (8218)     5000    36007 2023-05-03 15:09:48.000000 discminer-0.2.5/discminer/rail.py
+-rw-r--r--   0 aizquier  (8218)     5000   160740 2022-01-27 11:46:40.000000 discminer-0.2.5/discminer/testyapf.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-07 20:54:46.477642 discminer-0.2.5/discminer/tools/
+-rw-r--r--   0 aizquier  (8218)     5000      569 2023-03-16 20:41:38.000000 discminer-0.2.5/discminer/tools/discminer.mplstyle
+-rw-r--r--   0 aizquier  (8218)     5000    16972 2023-04-03 09:18:56.000000 discminer-0.2.5/discminer/tools/fit_kernel.py
+-rw-r--r--   0 aizquier  (8218)     5000     6997 2023-04-04 09:09:51.000000 discminer-0.2.5/discminer/tools/utils.py
+-rw-r--r--   0 aizquier  (8218)     5000      411 2022-11-24 22:45:39.000000 discminer-0.2.5/discminer/units.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-07 20:54:46.469912 discminer-0.2.5/discminer.egg-info/
+-rw-r--r--   0 aizquier  (8218)     5000     7128 2023-05-07 20:54:46.000000 discminer-0.2.5/discminer.egg-info/PKG-INFO
+-rw-r--r--   0 aizquier  (8218)     5000     1284 2023-05-07 20:54:46.000000 discminer-0.2.5/discminer.egg-info/SOURCES.txt
+-rw-r--r--   0 aizquier  (8218)     5000        1 2023-05-07 20:54:46.000000 discminer-0.2.5/discminer.egg-info/dependency_links.txt
+-rw-r--r--   0 aizquier  (8218)     5000      108 2023-05-07 20:54:46.000000 discminer-0.2.5/discminer.egg-info/requires.txt
+-rw-r--r--   0 aizquier  (8218)     5000       10 2023-05-07 20:54:46.000000 discminer-0.2.5/discminer.egg-info/top_level.txt
+-rw-r--r--   0 aizquier  (8218)     5000      151 2023-04-03 21:10:19.000000 discminer-0.2.5/pyproject.toml
+-rw-r--r--   0 aizquier  (8218)     5000       74 2023-05-07 20:54:46.482391 discminer-0.2.5/setup.cfg
+-rw-r--r--   0 aizquier  (8218)     5000     3219 2023-04-03 21:16:45.000000 discminer-0.2.5/setup.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-05-07 20:54:46.481042 discminer-0.2.5/template/
+-rw-r--r--   0 aizquier  (8218)     5000     8550 2023-04-15 07:40:20.000000 discminer-0.2.5/template/README.rst
+-rw-r--r--   0 aizquier  (8218)     5000     5072 2022-01-02 19:37:02.000000 discminer-0.2.5/template/download_MAPS.sh
+-rw-r--r--   0 aizquier  (8218)     5000     1019 2023-04-03 09:07:58.000000 discminer-0.2.5/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt
+-rw-r--r--   0 aizquier  (8218)     5000      617 2023-04-03 08:37:18.000000 discminer-0.2.5/template/prepare_data.py
```

### Comparing `discminer-0.2.4/LICENSE` & `discminer-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/PKG-INFO` & `discminer-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discminer
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python package for parametric modelling of intensity channel maps from gas discs
 Home-page: https://github.com/andizq/discminer
 Author: Andres F. Izquierdo
 Author-email: andres.izquierdo.c@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/andizq/discminer/issues
 Project-URL: Source, https://github.com/andizq/discminer/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discminer Version: 0.2.4 Summary: Python package
+Metadata-Version: 2.1 Name: discminer Version: 0.2.5 Summary: Python package
 for parametric modelling of intensity channel maps from gas discs Home-page:
 https://github.com/andizq/discminer Author: Andres F. Izquierdo Author-email:
 andres.izquierdo.c@gmail.com License: UNKNOWN Project-URL: Bug Reports, https:/
 /github.com/andizq/discminer/issues Project-URL: Source, https://github.com/
 andizq/discminer/ Description:
  [https://raw.githubusercontent.com/andizq/andizq.github.io/master/discminer/
                              discminer_logo.jpeg]
```

### Comparing `discminer-0.2.4/README.md` & `discminer-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/_mining/make_channels.py` & `discminer-0.2.5/_mining/make_channels.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/_mining/make_parfile.py` & `discminer-0.2.5/_mining/make_parfile.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/_mining/make_single_moments.py` & `discminer-0.2.5/_mining/make_single_moments.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/_mining/plot_attributes_model.py` & `discminer-0.2.5/_mining/plot_attributes_model.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/_mining/plot_azimuthal_profiles.py` & `discminer-0.2.5/_mining/plot_azimuthal_profiles.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/_mining/plot_moment+offset.py` & `discminer-0.2.5/_mining/plot_moment+offset.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/_mining/plot_moment+residuals.py` & `discminer-0.2.5/_mining/plot_moment+residuals.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/_mining/plot_peak_residuals.py` & `discminer-0.2.5/_mining/plot_peak_residuals.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/_mining/plot_radial_profiles.py` & `discminer-0.2.5/_mining/plot_radial_profiles.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/_mining/plot_residuals+all.py` & `discminer-0.2.5/_mining/plot_residuals+all.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/_mining/plot_residuals+deproj.py` & `discminer-0.2.5/_mining/plot_residuals+deproj.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/_mining/utils.py` & `discminer-0.2.5/_mining/utils.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/discminer/cart.py` & `discminer-0.2.5/discminer/cart.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,22 @@
     R = coord['R']/au_to_m
     return au_to_m*(z0*(R/R0)**p*np.exp(-(R/Rb)**q))
 
 def z_lower_exp_tapered(coord, z0, p, Rb, q, R0=100):
     R = coord['R']/au_to_m
     return -au_to_m*(z0*(R/R0)**p*np.exp(-(R/Rb)**q))
 
+def z_upper_powerlaw(coord, z0, p, Rb, q, R0=100):
+    R = coord['R']/au_to_m
+    return au_to_m*(z0*(R/R0)**p - Rb*(R/R0)**q)
+
+def z_lower_powerlaw(coord, z0, p, Rb, q, R0=100):
+    R = coord['R']/au_to_m
+    return -au_to_m*(z0*(R/R0)**p - Rb*(R/R0)**q)
+
 #****************
 #CUSTOM INTENSITY
 #****************
 def intensity_powerlaw_rout(coord, I0=30.0, R0=100, p=-0.4, z0=100, q=0.3, Rout=500):
     if 'R' not in coord.keys(): R = hypot_func(coord['x'], coord['y'])
     else: R = coord['R']
     z = coord['z']
```

### Comparing `discminer-0.2.4/discminer/core.py` & `discminer-0.2.5/discminer/core.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/discminer/cube.py` & `discminer-0.2.5/discminer/cube.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/discminer/disc2d.py` & `discminer-0.2.5/discminer/disc2d.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/discminer/grid.py` & `discminer-0.2.5/discminer/grid.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/discminer/icons/button_box.png` & `discminer-0.2.5/discminer/icons/button_box.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/discminer/icons/button_cursor.jpeg` & `discminer-0.2.5/discminer/icons/button_cursor.jpeg`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/discminer/icons/button_path.png` & `discminer-0.2.5/discminer/icons/button_path.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/discminer/icons/button_return.png` & `discminer-0.2.5/discminer/icons/button_return.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/discminer/icons/button_surface.png` & `discminer-0.2.5/discminer/icons/button_surface.png`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/discminer/icons/button_trash.jpg` & `discminer-0.2.5/discminer/icons/button_trash.jpg`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/discminer/pick.py` & `discminer-0.2.5/discminer/pick.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/discminer/plottools.py` & `discminer-0.2.5/discminer/plottools.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 ===========
 """
 import os
 import copy
 import matplotlib
 import numpy as np
 from math import ceil
+import astropy.units as u
 import matplotlib.pyplot as plt
 import matplotlib.patches as patches
 from collections.abc import Iterable
-from .tools.utils import weighted_std
+
+from .tools.utils import weighted_std, InputError
 from .tools.fit_kernel import _gauss
 from .grid import GridTools
-        
+
 SMALL_SIZE = 10
 MEDIUM_SIZE = 15
 BIGGER_SIZE = 22
 
 _residuals_colors = {
     'velocity': ["#"+tmp for tmp in ["000b14","004f8f","1f9aff","fff7db","ff5a47","cc0033","140200"]],
     'linewidth': ["#"+tmp for tmp in ["000b14","036407","81ae71","fff7db","ff5a47","cc0033","140200"]],
@@ -129,16 +131,16 @@
     Examples
     ----------
     fig, ax = plt.subplots(1,1)
     hex_list = ['#0091ad', '#fffffc', '#ffd166']
     x, y = np.mgrid[-5:5:0.05, -5:5:0.05]                                
     z = (np.sqrt(x**2 + y**2) + np.sin(x**2 + y**2))
     im = ax.imshow(z, cmap=get_continuous_cmap(hex_list))                                                         
-    fig.colorbar(im)                                                                                                                                                                      
-    ax.yaxis.set_major_locator(plt.NullLocator()) # remove y axis ticks                                                                                                                               
+    fig.colorbar(im)  
+    ax.yaxis.set_major_locator(plt.NullLocator()) # remove y axis ticks 
     ax.xaxis.set_major_locator(plt.NullLocator()) # remove x axis ticks
     plt.show()
     """
 
     rgb_list = [matplotlib.colors.to_rgb(i) for i in hex_list]
     if float_list is None: float_list = np.linspace(0,1,len(rgb_list))
 
@@ -364,51 +366,103 @@
         text_nsky(xn[ii], yn[ii])
     else:
         text_nsky(xni, yni)
 
     return xni, yni
 
 def make_substructures(ax, gaps=[], rings=[], kinks=[],
-                       twodim=False, polar=False, make_legend=False,
+                       twodim=False,
+                       coords='disc', polar=False,
+                       model=None, surface='upper', #relevant if coords='sky'
+                       make_legend=False,                       
                        label_gaps=False, label_rings=False, label_kinks=False,
                        kwargs_gaps={}, kwargs_rings={}, kwargs_kinks={}, func1d='axvline'):
+    
     '''Overlay ring-like (if twodim) or vertical lines (if not twodim) to illustrate the radial location of substructures in the disc'''
     kwargs_g = dict(color='0.2', ls='--', lw=1.7, dash_capstyle='round', dashes=(3.0, 2.5), alpha=1.0)
     kwargs_r = dict(color='0.2', ls='-', lw=1.7, dash_capstyle='round', alpha=1.0)
     kwargs_k = dict(color='purple', ls=':', lw=2.5, dash_capstyle='round', dashes=(0.5, 1.5), alpha=0.9)
     kwargs_g.update(kwargs_gaps)
     kwargs_r.update(kwargs_rings)
-    kwargs_k.update(kwargs_kinks)        
+    kwargs_k.update(kwargs_kinks)
+    
     if twodim:
         nphi = 100
         phi = np.linspace(0, 2*np.pi, nphi)
         phi_deg = np.degrees(phi-np.pi)
         subst_fmt = zip([gaps, rings, kinks],
                         ['D%d', 'B%d', 'K%d'],
                         [label_gaps, label_rings, label_kinks],
                         [kwargs_g['color'], kwargs_r['color'], kwargs_k['color']])
-        if polar:
-            for R in gaps: ax.plot(phi_deg, [R]*nphi, **kwargs_g)
-            for R in rings: ax.plot(phi_deg, [R]*nphi, **kwargs_r)
-            for R in kinks: ax.plot(phi_deg, [R]*nphi, **kwargs_k)
-
-            for subst, fmt, label, color in subst_fmt:
-                if label:
-                    _make_text_2D(ax, subst, posx=-45, fmt=fmt, color=color)                
-        else:
-            cos_phi = np.cos(phi)
-            sin_phi = np.sin(phi)
-            for R in gaps: ax.plot(R*cos_phi, R*sin_phi, **kwargs_g)
-            for R in rings: ax.plot(R*cos_phi, R*sin_phi, **kwargs_r)
-            for R in kinks: ax.plot(R*cos_phi, R*sin_phi, **kwargs_k)
-
-            for subst, fmt, label, color in subst_fmt:
-                if label:
-                    _make_text_2D(ax, subst, sposy=-1, fmt=fmt, color=color)
+
+        if coords in ['disc', 'disk']:
+
+            if polar:
+                for R in gaps: ax.plot(phi_deg, [R]*nphi, **kwargs_g)
+                for R in rings: ax.plot(phi_deg, [R]*nphi, **kwargs_r)
+                for R in kinks: ax.plot(phi_deg, [R]*nphi, **kwargs_k)
+
+                for subst, fmt, label, color in subst_fmt:
+                    if label:
+                        _make_text_2D(ax, subst, posx=-45, fmt=fmt, color=color)                
+            else:
+                cos_phi = np.cos(phi)
+                sin_phi = np.sin(phi)
+                for R in gaps: ax.plot(R*cos_phi, R*sin_phi, **kwargs_g)
+                for R in rings: ax.plot(R*cos_phi, R*sin_phi, **kwargs_r)
+                for R in kinks: ax.plot(R*cos_phi, R*sin_phi, **kwargs_k)
+                
+                for subst, fmt, label, color in subst_fmt:
+                    if label:
+                        _make_text_2D(ax, subst, sposy=-1, fmt=fmt, color=color)
+                        
+        elif coords=='sky':
+            if model is None:
+                raise InputError(
+                    model, "model must be a discminer model instance"
+                )
+
+            au_m = u.au.to('m')
+            get_sky_from_disc_coords = GridTools.get_sky_from_disc_coords
+            cont_gaps, cont_rings, cont_kinks = [], [], []
+
+            incl = model.params['orientation']['incl']
+            PA = model.params['orientation']['PA']
+            xc = model.params['orientation']['xc']
+            yc = model.params['orientation']['yc']
+            orient = (incl, PA, xc, yc)
+            
+            get_z = lambda r: model.z_upper_func({'R': r*au_m}, **model.params['height_%s'%surface])/au_m
+            get_0 = lambda r: 0
+
+            if surface=='midplane':
+                get_fz = get_0
+            else:
+                get_fz = get_z
+                
+            for gap in gaps:
+                z = get_fz(gap)
+                x_cont, y_cont,_ = get_sky_from_disc_coords(gap, phi, z, *orient)
+                ax.plot(x_cont, y_cont, **kwargs_g)
+                
+            for ring in rings:
+                z = get_fz(ring)
+                x_cont, y_cont,_ = get_sky_from_disc_coords(ring, phi, z, *orient)
+                ax.plot(x_cont, y_cont, **kwargs_r)
+                
+            for kink in kinks:
+                z = get_fz(kink)
+                x_cont, y_cont,_ = get_sky_from_disc_coords(kink, phi, z, *orient)
+                ax.plot(x_cont, y_cont, **kwargs_k)
             
+        else:
+            raise InputError(
+                coords, "coords must be 'disc' [or 'disk'] or 'sky'"
+            )
+
     else:
         if func1d=='axvline': func1d=ax.axvline
         elif func1d=='axhline': func1d=ax.axhline            
         for R in gaps: func1d(R, **kwargs_g)
         for R in rings: func1d(R, **kwargs_r)
         for R in kinks: func1d(R, **kwargs_k)
```

### Comparing `discminer-0.2.4/discminer/rail.py` & `discminer-0.2.5/discminer/rail.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/discminer/testyapf.py` & `discminer-0.2.5/discminer/testyapf.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/discminer/tools/discminer.mplstyle` & `discminer-0.2.5/discminer/tools/discminer.mplstyle`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/discminer/tools/fit_kernel.py` & `discminer-0.2.5/discminer/tools/fit_kernel.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/discminer/tools/utils.py` & `discminer-0.2.5/discminer/tools/utils.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/discminer.egg-info/PKG-INFO` & `discminer-0.2.5/discminer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discminer
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python package for parametric modelling of intensity channel maps from gas discs
 Home-page: https://github.com/andizq/discminer
 Author: Andres F. Izquierdo
 Author-email: andres.izquierdo.c@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/andizq/discminer/issues
 Project-URL: Source, https://github.com/andizq/discminer/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discminer Version: 0.2.4 Summary: Python package
+Metadata-Version: 2.1 Name: discminer Version: 0.2.5 Summary: Python package
 for parametric modelling of intensity channel maps from gas discs Home-page:
 https://github.com/andizq/discminer Author: Andres F. Izquierdo Author-email:
 andres.izquierdo.c@gmail.com License: UNKNOWN Project-URL: Bug Reports, https:/
 /github.com/andizq/discminer/issues Project-URL: Source, https://github.com/
 andizq/discminer/ Description:
  [https://raw.githubusercontent.com/andizq/andizq.github.io/master/discminer/
                              discminer_logo.jpeg]
```

### Comparing `discminer-0.2.4/discminer.egg-info/SOURCES.txt` & `discminer-0.2.5/discminer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/setup.py` & `discminer-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/template/README.rst` & `discminer-0.2.5/template/README.rst`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/template/download_MAPS.sh` & `discminer-0.2.5/template/download_MAPS.sh`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt` & `discminer-0.2.5/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt`

 * *Files identical despite different names*

### Comparing `discminer-0.2.4/template/prepare_data.py` & `discminer-0.2.5/template/prepare_data.py`

 * *Files identical despite different names*

