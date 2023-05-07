# Comparing `tmp/movingpandas-0.9rc2.tar.gz` & `tmp/movingpandas-0.9rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\movingpandas-0.9rc2.tar", last modified: Tue Jan 11 19:52:47 2022, max compression
+gzip compressed data, was "movingpandas-0.9rc3.tar", last modified: Sun Mar  6 13:51:00 2022, max compression
```

## Comparing `movingpandas-0.9rc2.tar` & `movingpandas-0.9rc3.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2022-01-11 19:52:47.000000 movingpandas-0.9rc2/
--rw-rw-rw-   0        0        0    12490 2022-01-11 19:52:47.000000 movingpandas-0.9rc2/PKG-INFO
--rw-rw-rw-   0        0        0    10625 2022-01-11 12:36:22.000000 movingpandas-0.9rc2/README.md
-drwxrwxrwx   0        0        0        0 2022-01-11 19:52:47.000000 movingpandas-0.9rc2/movingpandas/
--rw-rw-rw-   0        0        0     1124 2022-01-11 19:52:44.000000 movingpandas-0.9rc2/movingpandas/__init__.py
--rw-rw-rw-   0        0        0     4767 2022-01-11 12:36:22.000000 movingpandas-0.9rc2/movingpandas/geometry_utils.py
--rw-rw-rw-   0        0        0     8483 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/overlay.py
--rw-rw-rw-   0        0        0     4325 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/point_clusterer.py
-drwxrwxrwx   0        0        0        0 2022-01-11 19:52:47.000000 movingpandas-0.9rc2/movingpandas/tests/
--rw-rw-rw-   0        0        0      344 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/tests/__init__.py
--rw-rw-rw-   0        0        0     3922 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/tests/test_geometry_utils.py
--rw-rw-rw-   0        0        0    10677 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/tests/test_overlay.py
--rw-rw-rw-   0        0        0     3218 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/tests/test_point_clusterer.py
--rw-rw-rw-   0        0        0     1284 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/tests/test_show_versions.py
--rw-rw-rw-   0        0        0    24785 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/tests/test_trajectory.py
--rw-rw-rw-   0        0        0     8904 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/tests/test_trajectory_aggregator.py
--rw-rw-rw-   0        0        0     3022 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/tests/test_trajectory_cleaner.py
--rw-rw-rw-   0        0        0    11702 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/tests/test_trajectory_collection.py
--rw-rw-rw-   0        0        0     4556 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/tests/test_trajectory_generalizer.py
--rw-rw-rw-   0        0        0     1915 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/tests/test_trajectory_plotter.py
--rw-rw-rw-   0        0        0     5256 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/tests/test_trajectory_smoother.py
--rw-rw-rw-   0        0        0    11476 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/tests/test_trajectory_splitter.py
--rw-rw-rw-   0        0        0     8619 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/tests/test_trajectory_stop_detector.py
--rw-rw-rw-   0        0        0     1163 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/time_range_utils.py
-drwxrwxrwx   0        0        0        0 2022-01-11 19:52:47.000000 movingpandas-0.9rc2/movingpandas/tools/
--rw-rw-rw-   0        0        0     3457 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/tools/_show_versions.py
--rw-rw-rw-   0        0        0    30789 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/trajectory.py
--rw-rw-rw-   0        0        0    10076 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/trajectory_aggregator.py
--rw-rw-rw-   0        0        0     2963 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/trajectory_cleaner.py
--rw-rw-rw-   0        0        0    13826 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/trajectory_collection.py
--rw-rw-rw-   0        0        0     8691 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/trajectory_generalizer.py
--rw-rw-rw-   0        0        0     6723 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/trajectory_plotter.py
--rw-rw-rw-   0        0        0     8681 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/trajectory_smoother.py
--rw-rw-rw-   0        0        0     7096 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/trajectory_splitter.py
--rw-rw-rw-   0        0        0     6284 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/trajectory_stop_detector.py
--rw-rw-rw-   0        0        0     1301 2022-01-11 12:36:23.000000 movingpandas-0.9rc2/movingpandas/trajectory_utils.py
-drwxrwxrwx   0        0        0        0 2022-01-11 19:52:47.000000 movingpandas-0.9rc2/movingpandas.egg-info/
--rw-rw-rw-   0        0        0    12490 2022-01-11 19:52:47.000000 movingpandas-0.9rc2/movingpandas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1363 2022-01-11 19:52:47.000000 movingpandas-0.9rc2/movingpandas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-11 19:52:47.000000 movingpandas-0.9rc2/movingpandas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2022-01-11 19:52:47.000000 movingpandas-0.9rc2/movingpandas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-01-11 19:52:47.000000 movingpandas-0.9rc2/movingpandas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      217 2022-01-11 19:52:47.000000 movingpandas-0.9rc2/setup.cfg
--rw-rw-rw-   0        0        0     1202 2022-01-11 19:52:34.000000 movingpandas-0.9rc2/setup.py
+drwxrwxrwx   0        0        0        0 2022-03-06 13:51:00.924180 movingpandas-0.9rc3/
+-rw-rw-rw-   0        0        0     1565 2022-01-12 13:53:29.000000 movingpandas-0.9rc3/LICENSE.txt
+-rw-rw-rw-   0        0        0    11294 2022-03-06 13:51:00.924180 movingpandas-0.9rc3/PKG-INFO
+-rw-rw-rw-   0        0        0    10625 2022-01-12 13:53:29.000000 movingpandas-0.9rc3/README.md
+drwxrwxrwx   0        0        0        0 2022-03-06 13:51:00.889180 movingpandas-0.9rc3/movingpandas/
+-rw-rw-rw-   0        0        0     1144 2022-03-06 13:44:59.000000 movingpandas-0.9rc3/movingpandas/__init__.py
+-rw-rw-rw-   0        0        0     4752 2022-02-16 17:36:34.000000 movingpandas-0.9rc3/movingpandas/geometry_utils.py
+-rw-rw-rw-   0        0        0     8514 2022-02-05 12:43:06.000000 movingpandas-0.9rc3/movingpandas/overlay.py
+-rw-rw-rw-   0        0        0     4325 2022-01-12 13:53:29.000000 movingpandas-0.9rc3/movingpandas/point_clusterer.py
+drwxrwxrwx   0        0        0        0 2022-03-06 13:51:00.921179 movingpandas-0.9rc3/movingpandas/tests/
+-rw-rw-rw-   0        0        0      344 2022-01-12 13:53:29.000000 movingpandas-0.9rc3/movingpandas/tests/__init__.py
+-rw-rw-rw-   0        0        0     4039 2022-02-16 17:36:34.000000 movingpandas-0.9rc3/movingpandas/tests/test_geometry_utils.py
+-rw-rw-rw-   0        0        0    10677 2022-01-12 13:53:29.000000 movingpandas-0.9rc3/movingpandas/tests/test_overlay.py
+-rw-rw-rw-   0        0        0     3218 2022-01-12 13:53:29.000000 movingpandas-0.9rc3/movingpandas/tests/test_point_clusterer.py
+-rw-rw-rw-   0        0        0     1284 2022-01-12 13:53:29.000000 movingpandas-0.9rc3/movingpandas/tests/test_show_versions.py
+-rw-rw-rw-   0        0        0    25338 2022-03-06 11:16:03.000000 movingpandas-0.9rc3/movingpandas/tests/test_trajectory.py
+-rw-rw-rw-   0        0        0     8904 2022-01-12 13:53:29.000000 movingpandas-0.9rc3/movingpandas/tests/test_trajectory_aggregator.py
+-rw-rw-rw-   0        0        0     3022 2022-01-12 13:53:29.000000 movingpandas-0.9rc3/movingpandas/tests/test_trajectory_cleaner.py
+-rw-rw-rw-   0        0        0    11796 2022-02-05 13:29:35.000000 movingpandas-0.9rc3/movingpandas/tests/test_trajectory_collection.py
+-rw-rw-rw-   0        0        0     5322 2022-03-06 10:28:43.000000 movingpandas-0.9rc3/movingpandas/tests/test_trajectory_generalizer.py
+-rw-rw-rw-   0        0        0     1915 2022-01-12 13:53:29.000000 movingpandas-0.9rc3/movingpandas/tests/test_trajectory_plotter.py
+-rw-rw-rw-   0        0        0     5256 2022-01-13 15:22:40.000000 movingpandas-0.9rc3/movingpandas/tests/test_trajectory_smoother.py
+-rw-rw-rw-   0        0        0    11476 2022-01-12 13:53:29.000000 movingpandas-0.9rc3/movingpandas/tests/test_trajectory_splitter.py
+-rw-rw-rw-   0        0        0     8619 2022-01-12 13:53:29.000000 movingpandas-0.9rc3/movingpandas/tests/test_trajectory_stop_detector.py
+-rw-rw-rw-   0        0        0     1163 2022-01-12 13:53:29.000000 movingpandas-0.9rc3/movingpandas/time_range_utils.py
+drwxrwxrwx   0        0        0        0 2022-03-06 13:51:00.922179 movingpandas-0.9rc3/movingpandas/tools/
+-rw-rw-rw-   0        0        0     3479 2022-03-06 09:31:32.000000 movingpandas-0.9rc3/movingpandas/tools/_show_versions.py
+-rw-rw-rw-   0        0        0    30873 2022-03-06 11:18:07.000000 movingpandas-0.9rc3/movingpandas/trajectory.py
+-rw-rw-rw-   0        0        0    10076 2022-01-12 13:53:29.000000 movingpandas-0.9rc3/movingpandas/trajectory_aggregator.py
+-rw-rw-rw-   0        0        0     2963 2022-01-12 13:53:29.000000 movingpandas-0.9rc3/movingpandas/trajectory_cleaner.py
+-rw-rw-rw-   0        0        0    14061 2022-03-06 10:07:05.000000 movingpandas-0.9rc3/movingpandas/trajectory_collection.py
+-rw-rw-rw-   0        0        0     9077 2022-03-06 10:57:32.000000 movingpandas-0.9rc3/movingpandas/trajectory_generalizer.py
+-rw-rw-rw-   0        0        0     6825 2022-01-15 15:09:42.000000 movingpandas-0.9rc3/movingpandas/trajectory_plotter.py
+-rw-rw-rw-   0        0        0     8681 2022-01-12 13:53:29.000000 movingpandas-0.9rc3/movingpandas/trajectory_smoother.py
+-rw-rw-rw-   0        0        0     7096 2022-01-12 13:53:29.000000 movingpandas-0.9rc3/movingpandas/trajectory_splitter.py
+-rw-rw-rw-   0        0        0     6504 2022-02-16 17:36:34.000000 movingpandas-0.9rc3/movingpandas/trajectory_stop_detector.py
+-rw-rw-rw-   0        0        0     1301 2022-01-12 13:53:29.000000 movingpandas-0.9rc3/movingpandas/trajectory_utils.py
+drwxrwxrwx   0        0        0        0 2022-03-06 13:51:00.907177 movingpandas-0.9rc3/movingpandas.egg-info/
+-rw-rw-rw-   0        0        0    11294 2022-03-06 13:51:00.000000 movingpandas-0.9rc3/movingpandas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1375 2022-03-06 13:51:00.000000 movingpandas-0.9rc3/movingpandas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-03-06 13:51:00.000000 movingpandas-0.9rc3/movingpandas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2022-03-06 13:51:00.000000 movingpandas-0.9rc3/movingpandas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2022-03-06 13:51:00.000000 movingpandas-0.9rc3/movingpandas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      217 2022-03-06 13:51:00.925179 movingpandas-0.9rc3/setup.cfg
+-rw-rw-rw-   0        0        0     1215 2022-03-06 13:50:29.000000 movingpandas-0.9rc3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `movingpandas-0.9rc2/PKG-INFO` & `movingpandas-0.9rc3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,178 +1,181 @@
 Metadata-Version: 2.1
 Name: movingpandas
-Version: 0.9rc2
-Summary: Implementation of Trajectory classes and functions built on top of GeoPandas
+Version: 0.9rc3
+Summary: MovingPandas implements Trajectory classes and corresponding methods for the analysis of movement data based on GeoPandas. Visit movingpandas.org for details.
 Home-page: https://github.com/anitagraser/movingpandas
 Author: Anita Graser
 Author-email: anitagraser@gmx.at
 License: UNKNOWN
-Description: # MovingPandas
-        
-        [![Project Status: Active â€“ The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
-        [![Tests](https://github.com/anitagraser/movingpandas/actions/workflows/tests.yaml/badge.svg)](https://github.com/anitagraser/movingpandas/actions/workflows/tests.yaml)
-        [![docs status](https://readthedocs.org/projects/movingpandas/badge/?version=master)](https://movingpandas.readthedocs.io/en/master/)
-        [![codecov](https://codecov.io/gh/anitagraser/movingpandas/branch/master/graph/badge.svg)](https://codecov.io/gh/anitagraser/movingpandas)
-        [![DOI](https://zenodo.org/badge/161995245.svg)](https://zenodo.org/badge/latestdoi/161995245)
-        [![pyOpenSci](https://camo.githubusercontent.com/63ff31cdb80a06361e53ac2b9ac0d184118ebd0b/68747470733a2f2f74696e7975726c2e636f6d2f7932326e62387570)](https://github.com/pyOpenSci/software-review/issues/18)
-        
-        <img align="right" src="https://anitagraser.github.io/movingpandas/assets/img/movingpandas.png">
-        
-        MovingPandas implements a Trajectory class and corresponding methods based on **[GeoPandas](https://geopandas.org)**.
-        
-        Visit **[movingpandas.org](http://movingpandas.org)** for details! 
-        
-        You can run **[MovingPandas examples](https://github.com/anitagraser/movingpandas-examples)** on MyBinder - no installation required: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/anitagraser/movingpandas-examples/main) (These examples use the latest MovingPandas release version.) 
-        
-        To try the cutting-edge dev version, use [this MyBinder link](https://mybinder.org/v2/gh/anitagraser/movingpandas/master?filepath=tutorials/1-getting-started.ipynb).
-        
-        ## Documentation
-        
-        The official documentation is hosted on **[ReadTheDocs](https://movingpandas.readthedocs.io)**
-        
-        ## Examples
-        
-        ### Trajectory plots
-        
-        ![movingpandas_animated](https://user-images.githubusercontent.com/590385/137953765-33f9ce1b-037c-4c86-82b2-0620de5ca28f.gif)
-        
-        ### Stop detection
-        
-        ![movingpandas_stop_detection](https://user-images.githubusercontent.com/590385/137953859-3df81568-eda8-4443-96b8-e82e15c03653.png)
-        
-        ### Trajectory generalization
-        
-        ![movingpandas_generalize](https://user-images.githubusercontent.com/590385/142756559-012a15fe-736c-474c-b244-0ee02090d592.gif)
-        
-        ### Trajectory aggregation
-        
-        ![movingpandas_ais](https://user-images.githubusercontent.com/590385/137953890-d43c7fe5-5aea-4e29-8ce1-f0d529c3220f.png)
-        
-        ## Installation
-        
-        MovingPandas for Python >= 3.7 and all it's dependencies are available from [conda-forge](https://anaconda.org/conda-forge/movingpandas) and can be installed using `conda install -c conda-forge movingpandas`.
-        
-        **Conda status**
-        
-        [![Conda Recipe](https://img.shields.io/badge/recipe-movingpandas-green.svg)](https://anaconda.org/conda-forge/movingpandas) 
-        [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/movingpandas.svg)](https://anaconda.org/conda-forge/movingpandas) 
-        [![Conda Version](https://img.shields.io/conda/vn/conda-forge/movingpandas.svg)](https://anaconda.org/conda-forge/movingpandas) 
-        [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/movingpandas.svg)](https://anaconda.org/conda-forge/movingpandas)
-        
-        Note that it is **NOT recommended** to install MovingPandas from [PyPI](https://pypi.org/project/movingpandas/)!
-        If you're on Windows or Mac, many GeoPandas / MovingPandas dependencies cannot be pip installed 
-        (for details see the corresponding notes in the [GeoPandas documentation](https://geopandas.readthedocs.io/en/latest/getting_started/install.html)).
-        On Ubuntu, pip install fails on cartopy with "Proj 4.9.0 must be installed".
-        
-        ## Development Installation 
-        
-        Use the following steps to run the notebooks using the current development version:
-        
-        ### Using conda
-        
-        **Linux/Mac**:  
-        
-        ```
-        conda env create -f environment.yml
-        ```
-        
-        **Windows**: 
-        
-        ```
-        conda config --add channels conda-forge
-        conda config --add channels defaults
-        conda config --set channel_priority strict
-        conda env create -f environment.yml
-        ```
-        
-        *On Windows, because conda-forge relies on some package built with defaults blas (like scipy) one must use the defaults channel on top of conda-forge and activate conda's new strict channel feature.* Source: https://github.com/conda-forge/gdal-feedstock/issues/269#issuecomment-473661530
-        
-        ### Using Anaconda
-        
-        1. Install Anaconda
-        2. Clone the movingpandas repository
-        3. In Anaconda Navigator | Environments | Import select the movingpandas environment.yml from the cloned directory:
-        
-        ![image](https://user-images.githubusercontent.com/590385/62143367-2db14c00-b2f0-11e9-8cb9-fb7993b7f62e.png)
-        
-        4. Wait until the environment is ready, then change to the Home tab and install Jupyter notebooks into the movingpandas environment
-        5. Launch Jupyter notebooks and navigate to the `movingpandas/tutorials` directory to execute them
-        6. Now you can run the notebooks, experiment with the code and adjust it to your own data
-        
-        Known issues:
-        
-        * On Windows, importing rasterio can lead to DLL errors. If this happens, downgrade the rasterio version to 1.0.13.
-        
-        ### Develop mode
-        
-        To install MovingPandas in ["develop" or "editable" mode](https://python-packaging-tutorial.readthedocs.io/en/latest/setup_py.html#develop-mode) you may use: 
-        
-        ```
-        python setup.py develop
-        ```
-        
-        ## Contributing to MovingPandas [![GitHub contributors](https://img.shields.io/github/contributors/anitagraser/movingpandas.svg)](https://github.com/anitagraser/movingpandas/graphs/contributors)
-        
-        All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.
-        
-        A detailed overview on how to contribute can be found in the [contributing guide](https://github.com/anitagraser/movingpandas/blob/master/CONTRIBUTING.md) on GitHub.
-        
-        ## Related Python Packages
-        
-        **For a more comprehensive list, including non-Python solutions, check https://github.com/anitagraser/movement-analysis-tools**
-        
-        [scikit-mobility](https://github.com/scikit-mobility/scikit-mobility) is a similar package which also deals with movement data. 
-        It implements TrajectoryDataFrames and FlowDataFrames on top of Pandas instead of GeoPandas. 
-        There is little overlap in the covered use cases and implemented functionality (comparing 
-        [MovingPandas tutorials](https://github.com/anitagraser/movingpandas/tree/master/tutorials) and 
-        [scikit-mobility tutorials](https://github.com/scikit-mobility/tutorials)). 
-        MovingPandas focuses on spatio-temporal data exploration with corresponding functions for data manipulation and analysis. 
-        scikit-mobility on the other hand focuses on computing human mobility metrics, generating synthetic trajectories 
-        and assessing privacy risks. Plotting is based on Folium. 
-        
-        [Traja](https://github.com/traja-team/traja) extends the capabilitis of Pandas DataFrames specific for animal trajectory analysis in 2D. Plots (static) are based on seaborn. 
-        
-        [PyMove](https://github.com/InsightLab/PyMove) provides functionality similar to MovingPandas. 
-        It implements PandasMoveDataFrames and DaskMoveDataFrame on top of Pandas and Dask DataFrames. Plotting is based on Folium. 
-        
-        [Tracktable](https://github.com/sandialabs/tracktable) is a related Python package with its core data structures and algorithms implemented in C++, i.e. it is not based on Pandas. Plotting is based on Cartopy (for still images) and Folium (for interactive rendering).
-        
-        ## Citation information
-        
-        Please cite [[0]](#publications) when using MovingPandas in your research and reference the appropriate release version. All releases of MovingPandas are listed on [Zenodo](https://doi.org/10.5281/zenodo.3710950) where you will find citation information, including DOIs.  
-        
-        ## Publications
-        
-        ### About MovingPandas
-        
-        [0] [Graser, A. (2019). MovingPandas: Efficient Structures for Movement Data in Python. GI_Forum â€’ Journal of Geographic Information Science 2019, 1-2019, 54-68. doi:10.1553/giscience2019_01_s54.](https://www.austriaca.at/rootcollection?arp=0x003aba2b)
-        
-        [1] [Graser, A. & Dragaschnig, M. (2020). Exploring movement data in notebook environments. Presented at MoVIS 2020, IEEE VIS 2020.](http://move.geog.ucsb.edu/wp-content/uploads/2020/10/MoVIS20_paper_4.pdf)
-        
-        ### Scientific Publications Referencing MovingPandas
-        
-        * [Pappalardo, L., Simini, F., Barlacchi, G., & Pellungrini, R. (2019). scikit-mobility: A Python library for the analysis, generation and risk assessment of mobility data. arXiv preprint arXiv:1907.07062.](https://arxiv.org/abs/1907.07062)
-        * [Graser, A. & Dragaschnig, M. (2020). Open Geospatial Tools for Movement Data Exploration. KN â€’ Journal of Cartography and Geographic Information, 70(1), 3-10. doi:10.1007/s42489-020-00039-y.](https://link.springer.com/article/10.1007/s42489-020-00039-y)
-        * [Kirkland, L. A., de Waal, A., & de Villiers, J. P. (2020). Evaluation of a Pure-Strategy Stackelberg Game for Wildlife Security in a Geospatial Framework. In Southern African Conference for Artificial Intelligence Research (pp. 101-118). Springer, Cham.](https://link.springer.com/chapter/10.1007/978-3-030-66151-9_7)
-        * [Depellegrin, D., Bastianini, M., Fadini, A., & Menegon, S. (2020). The effects of COVID-19 induced lockdown measures on maritime settings of a coastal region. Science of the Total Environment, 740, 140123.](https://doi.org/10.1016/j.scitotenv.2020.140123)
-        * [Graser, A. (2021). An exploratory data analysis protocol for identifying problems in continuous movement data. Journal of Location Based Services. doi:10.1080/17489725.2021.1900612.](https://doi.org/10.1080/17489725.2021.1900612)
-        * [Mehri, S., Alesheikh, A. A., & Basiri, A. (2021). A Contextual Hybrid Model for Vessel Movement Prediction. IEEE Access, 9, 45600-45613.](https://ieeexplore.ieee.org/abstract/document/9380635/)
-        
-        [Full Google Scholar list](https://scholar.google.com/scholar?oi=bibs&hl=en&cites=10366998261774464895)
-        
-        ### Teaching Material Referencing MovingPandas
-        
-        * [Aalto University. Spatial data science for sustainable development course](https://sustainability-gis.readthedocs.io/en/latest/lessons/L3/mobility-analytics.html)
-        
-        ### Workshop Videos
-        
-        * [Graser, A. (2019). Analyzing Movement Data with MovingPandas. Workshop at the OpenGeoHub summer school, MÃ¼nster, Germany.](http://www.youtube.com/watch?v=qeLQfnpJV1g)
-        
-        [![WorkshopVideo](https://user-images.githubusercontent.com/590385/67161044-f08cb100-f356-11e9-8799-f972175ec7f4.png)](http://www.youtube.com/watch?v=qeLQfnpJV1g "Anita Graser: Analyzing movement data")
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: smoothing
+License-File: LICENSE.txt
+
+# MovingPandas
+
+[![Project Status: Active â€“ The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
+[![Tests](https://github.com/anitagraser/movingpandas/actions/workflows/tests.yaml/badge.svg)](https://github.com/anitagraser/movingpandas/actions/workflows/tests.yaml)
+[![docs status](https://readthedocs.org/projects/movingpandas/badge/?version=master)](https://movingpandas.readthedocs.io/en/master/)
+[![codecov](https://codecov.io/gh/anitagraser/movingpandas/branch/master/graph/badge.svg)](https://codecov.io/gh/anitagraser/movingpandas)
+[![DOI](https://zenodo.org/badge/161995245.svg)](https://zenodo.org/badge/latestdoi/161995245)
+[![pyOpenSci](https://camo.githubusercontent.com/63ff31cdb80a06361e53ac2b9ac0d184118ebd0b/68747470733a2f2f74696e7975726c2e636f6d2f7932326e62387570)](https://github.com/pyOpenSci/software-review/issues/18)
+
+<img align="right" src="https://anitagraser.github.io/movingpandas/assets/img/movingpandas.png">
+
+MovingPandas implements a Trajectory class and corresponding methods based on **[GeoPandas](https://geopandas.org)**.
+
+Visit **[movingpandas.org](http://movingpandas.org)** for details! 
+
+You can run **[MovingPandas examples](https://github.com/anitagraser/movingpandas-examples)** on MyBinder - no installation required: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/anitagraser/movingpandas-examples/main) (These examples use the latest MovingPandas release version.) 
+
+To try the cutting-edge dev version, use [this MyBinder link](https://mybinder.org/v2/gh/anitagraser/movingpandas/master?filepath=tutorials/1-getting-started.ipynb).
+
+## Documentation
+
+The official documentation is hosted on **[ReadTheDocs](https://movingpandas.readthedocs.io)**
+
+## Examples
+
+### Trajectory plots
+
+![movingpandas_animated](https://user-images.githubusercontent.com/590385/137953765-33f9ce1b-037c-4c86-82b2-0620de5ca28f.gif)
+
+### Stop detection
+
+![movingpandas_stop_detection](https://user-images.githubusercontent.com/590385/137953859-3df81568-eda8-4443-96b8-e82e15c03653.png)
+
+### Trajectory generalization
+
+![movingpandas_generalize](https://user-images.githubusercontent.com/590385/142756559-012a15fe-736c-474c-b244-0ee02090d592.gif)
+
+### Trajectory aggregation
+
+![movingpandas_ais](https://user-images.githubusercontent.com/590385/137953890-d43c7fe5-5aea-4e29-8ce1-f0d529c3220f.png)
+
+## Installation
+
+MovingPandas for Python >= 3.7 and all it's dependencies are available from [conda-forge](https://anaconda.org/conda-forge/movingpandas) and can be installed using `conda install -c conda-forge movingpandas`.
+
+**Conda status**
+
+[![Conda Recipe](https://img.shields.io/badge/recipe-movingpandas-green.svg)](https://anaconda.org/conda-forge/movingpandas) 
+[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/movingpandas.svg)](https://anaconda.org/conda-forge/movingpandas) 
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/movingpandas.svg)](https://anaconda.org/conda-forge/movingpandas) 
+[![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/movingpandas.svg)](https://anaconda.org/conda-forge/movingpandas)
+
+Note that it is **NOT recommended** to install MovingPandas from [PyPI](https://pypi.org/project/movingpandas/)!
+If you're on Windows or Mac, many GeoPandas / MovingPandas dependencies cannot be pip installed 
+(for details see the corresponding notes in the [GeoPandas documentation](https://geopandas.readthedocs.io/en/latest/getting_started/install.html)).
+On Ubuntu, pip install fails on cartopy with "Proj 4.9.0 must be installed".
+
+## Development Installation 
+
+Use the following steps to run the notebooks using the current development version:
+
+### Using conda
+
+**Linux/Mac**:  
+
+```
+conda env create -f environment.yml
+```
+
+**Windows**: 
+
+```
+conda config --add channels conda-forge
+conda config --add channels defaults
+conda config --set channel_priority strict
+conda env create -f environment.yml
+```
+
+*On Windows, because conda-forge relies on some package built with defaults blas (like scipy) one must use the defaults channel on top of conda-forge and activate conda's new strict channel feature.* Source: https://github.com/conda-forge/gdal-feedstock/issues/269#issuecomment-473661530
+
+### Using Anaconda
+
+1. Install Anaconda
+2. Clone the movingpandas repository
+3. In Anaconda Navigator | Environments | Import select the movingpandas environment.yml from the cloned directory:
+
+![image](https://user-images.githubusercontent.com/590385/62143367-2db14c00-b2f0-11e9-8cb9-fb7993b7f62e.png)
+
+4. Wait until the environment is ready, then change to the Home tab and install Jupyter notebooks into the movingpandas environment
+5. Launch Jupyter notebooks and navigate to the `movingpandas/tutorials` directory to execute them
+6. Now you can run the notebooks, experiment with the code and adjust it to your own data
+
+Known issues:
+
+* On Windows, importing rasterio can lead to DLL errors. If this happens, downgrade the rasterio version to 1.0.13.
+
+### Develop mode
+
+To install MovingPandas in ["develop" or "editable" mode](https://python-packaging-tutorial.readthedocs.io/en/latest/setup_py.html#develop-mode) you may use: 
+
+```
+python setup.py develop
+```
+
+## Contributing to MovingPandas [![GitHub contributors](https://img.shields.io/github/contributors/anitagraser/movingpandas.svg)](https://github.com/anitagraser/movingpandas/graphs/contributors)
+
+All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.
+
+A detailed overview on how to contribute can be found in the [contributing guide](https://github.com/anitagraser/movingpandas/blob/master/CONTRIBUTING.md) on GitHub.
+
+## Related Python Packages
+
+**For a more comprehensive list, including non-Python solutions, check https://github.com/anitagraser/movement-analysis-tools**
+
+[scikit-mobility](https://github.com/scikit-mobility/scikit-mobility) is a similar package which also deals with movement data. 
+It implements TrajectoryDataFrames and FlowDataFrames on top of Pandas instead of GeoPandas. 
+There is little overlap in the covered use cases and implemented functionality (comparing 
+[MovingPandas tutorials](https://github.com/anitagraser/movingpandas/tree/master/tutorials) and 
+[scikit-mobility tutorials](https://github.com/scikit-mobility/tutorials)). 
+MovingPandas focuses on spatio-temporal data exploration with corresponding functions for data manipulation and analysis. 
+scikit-mobility on the other hand focuses on computing human mobility metrics, generating synthetic trajectories 
+and assessing privacy risks. Plotting is based on Folium. 
+
+[Traja](https://github.com/traja-team/traja) extends the capabilitis of Pandas DataFrames specific for animal trajectory analysis in 2D. Plots (static) are based on seaborn. 
+
+[PyMove](https://github.com/InsightLab/PyMove) provides functionality similar to MovingPandas. 
+It implements PandasMoveDataFrames and DaskMoveDataFrame on top of Pandas and Dask DataFrames. Plotting is based on Folium. 
+
+[Tracktable](https://github.com/sandialabs/tracktable) is a related Python package with its core data structures and algorithms implemented in C++, i.e. it is not based on Pandas. Plotting is based on Cartopy (for still images) and Folium (for interactive rendering).
+
+## Citation information
+
+Please cite [[0]](#publications) when using MovingPandas in your research and reference the appropriate release version. All releases of MovingPandas are listed on [Zenodo](https://doi.org/10.5281/zenodo.3710950) where you will find citation information, including DOIs.  
+
+## Publications
+
+### About MovingPandas
+
+[0] [Graser, A. (2019). MovingPandas: Efficient Structures for Movement Data in Python. GI_Forum â€’ Journal of Geographic Information Science 2019, 1-2019, 54-68. doi:10.1553/giscience2019_01_s54.](https://www.austriaca.at/rootcollection?arp=0x003aba2b)
+
+[1] [Graser, A. & Dragaschnig, M. (2020). Exploring movement data in notebook environments. Presented at MoVIS 2020, IEEE VIS 2020.](http://move.geog.ucsb.edu/wp-content/uploads/2020/10/MoVIS20_paper_4.pdf)
+
+### Scientific Publications Referencing MovingPandas
+
+* [Pappalardo, L., Simini, F., Barlacchi, G., & Pellungrini, R. (2019). scikit-mobility: A Python library for the analysis, generation and risk assessment of mobility data. arXiv preprint arXiv:1907.07062.](https://arxiv.org/abs/1907.07062)
+* [Graser, A. & Dragaschnig, M. (2020). Open Geospatial Tools for Movement Data Exploration. KN â€’ Journal of Cartography and Geographic Information, 70(1), 3-10. doi:10.1007/s42489-020-00039-y.](https://link.springer.com/article/10.1007/s42489-020-00039-y)
+* [Kirkland, L. A., de Waal, A., & de Villiers, J. P. (2020). Evaluation of a Pure-Strategy Stackelberg Game for Wildlife Security in a Geospatial Framework. In Southern African Conference for Artificial Intelligence Research (pp. 101-118). Springer, Cham.](https://link.springer.com/chapter/10.1007/978-3-030-66151-9_7)
+* [Depellegrin, D., Bastianini, M., Fadini, A., & Menegon, S. (2020). The effects of COVID-19 induced lockdown measures on maritime settings of a coastal region. Science of the Total Environment, 740, 140123.](https://doi.org/10.1016/j.scitotenv.2020.140123)
+* [Graser, A. (2021). An exploratory data analysis protocol for identifying problems in continuous movement data. Journal of Location Based Services. doi:10.1080/17489725.2021.1900612.](https://doi.org/10.1080/17489725.2021.1900612)
+* [Mehri, S., Alesheikh, A. A., & Basiri, A. (2021). A Contextual Hybrid Model for Vessel Movement Prediction. IEEE Access, 9, 45600-45613.](https://ieeexplore.ieee.org/abstract/document/9380635/)
+
+[Full Google Scholar list](https://scholar.google.com/scholar?oi=bibs&hl=en&cites=10366998261774464895)
+
+### Teaching Material Referencing MovingPandas
+
+* [Aalto University. Spatial data science for sustainable development course](https://sustainability-gis.readthedocs.io/en/latest/lessons/L3/mobility-analytics.html)
+
+### Workshop Videos
+
+* [Graser, A. (2019). Analyzing Movement Data with MovingPandas. Workshop at the OpenGeoHub summer school, MÃ¼nster, Germany.](http://www.youtube.com/watch?v=qeLQfnpJV1g)
+
+[![WorkshopVideo](https://user-images.githubusercontent.com/590385/67161044-f08cb100-f356-11e9-8799-f972175ec7f4.png)](http://www.youtube.com/watch?v=qeLQfnpJV1g "Anita Graser: Analyzing movement data")
+
+
```

### Comparing `movingpandas-0.9rc2/README.md` & `movingpandas-0.9rc3/README.md`

 * *Files identical despite different names*

### Comparing `movingpandas-0.9rc2/movingpandas/__init__.py` & `movingpandas-0.9rc3/movingpandas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,12 +24,12 @@
 from .trajectory_cleaner import OutlierCleaner  # noqa F401
 from .trajectory_stop_detector import TrajectoryStopDetector  # noqa F401
 from .point_clusterer import PointClusterer  # noqa F401
 from .tools._show_versions import show_versions  # noqa F401
 
 try:
     from .trajectory_smoother import KalmanSmootherCV  # noqa F401
-except ImportError:
-    pass
+except ImportError as e:
+    print(f"INFO: {e}")
 
 name = "movingpandas"
-__version__ = "0.9.rc2"
+__version__ = "0.9.rc3"
```

### Comparing `movingpandas-0.9rc2/movingpandas/geometry_utils.py` & `movingpandas-0.9rc3/movingpandas/geometry_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 from math import sin, cos, atan2, radians, degrees, sqrt, pi
-from shapely.geometry import MultiPoint, Point
+from shapely.geometry import Point
 from geopy import distance
 
 
 R_EARTH = 6371000  # radius of earth in meters
 C_EARTH = 2 * R_EARTH * pi  # circumference
 
 
@@ -141,17 +141,17 @@
 
 
 def mrr_diagonal(geom, spherical=False):
     """
     Calculate the length of the diagonal of the minimum rotated rectangle of
     the input geometry.
     """
-    if len(geom) == 1:
+    if isinstance(geom, Point):
         return 0
     if len(geom) == 2:
         return _measure_distance(geom[0], geom[1], spherical)
-    mrr = MultiPoint(geom).minimum_rotated_rectangle
+    mrr = geom.minimum_rotated_rectangle
     try:  # usually mrr is a Polygon
         x, y = mrr.exterior.coords.xy
     except AttributeError:  # thrown if mrr is a LineString
         return _measure_distance(Point(mrr.coords[0]), Point(mrr.coords[-1], spherical))
     return _measure_distance(Point(x[0], y[0]), Point(x[2], y[2]), spherical)
```

### Comparing `movingpandas-0.9rc2/movingpandas/overlay.py` & `movingpandas-0.9rc3/movingpandas/overlay.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,19 +93,21 @@
 def create_entry_and_exit_points(traj, range):
     """
     Returns a dataframe with inserted entry and exit points according to the
     provided SpatioTemporalRange.
     """
     if type(range) != SpatioTemporalRange:
         raise TypeError("Input range has to be a SpatioTemporalRange!")
+
+    index = traj.df.index
     # Create row at entry point with attributes from previous row = pad
-    row0 = traj.df.iloc[traj.df.index.get_loc(range.t_0, method="pad")].copy()
+    row0 = traj.df.iloc[index.get_indexer([range.t_0], method="pad")[0]].copy()
     row0["geometry"] = range.pt_0
     # Create row at exit point
-    rown = traj.df.iloc[traj.df.index.get_loc(range.t_n, method="pad")].copy()
+    rown = traj.df.iloc[index.get_indexer([range.t_n], method="pad")[0]].copy()
     rown["geometry"] = range.pt_n
     # Insert rows
     temp_df = traj.df.copy()
 
     try:
         temp_df.loc[range.t_0] = row0
     except ValueError as err:
```

### Comparing `movingpandas-0.9rc2/movingpandas/point_clusterer.py` & `movingpandas-0.9rc3/movingpandas/point_clusterer.py`

 * *Files identical despite different names*

### Comparing `movingpandas-0.9rc2/movingpandas/tests/test_geometry_utils.py` & `movingpandas-0.9rc3/movingpandas/tests/test_geometry_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import pytest
 from math import sqrt
-from shapely.geometry import Point
+from shapely.geometry import MultiPoint, Point
 from movingpandas.geometry_utils import (
     azimuth,
     calculate_initial_compass_bearing,
     angular_difference,
     mrr_diagonal,
     measure_distance_geodesic,
     measure_distance_euclidean,
@@ -68,17 +68,20 @@
         assert angular_difference(-45, 45) == 90
 
     def test_anglular_difference_twonegative(self):
         assert angular_difference(-200, -160) == 40
 
     def test_mrr_diagonal(self):
         assert mrr_diagonal(
-            [Point(0, 0), Point(0, 2), Point(2, 0), Point(2, 2)]
+            MultiPoint([Point(0, 0), Point(0, 2), Point(2, 0), Point(2, 2)])
         ) == sqrt(8)
 
+    def test_mrr_diagonal_one_point(self):
+        assert mrr_diagonal(Point(2, 3)) == 0
+
     def test_euclidean_distance(self):
         assert (measure_distance_euclidean(Point(0, 0), Point(0, 1))) == 1
 
     def test_spherical_distance(self):
         assert measure_distance_spherical(
             Point(-74.00597, 40.71427), Point(-118.24368, 34.05223)
         ) == pytest.approx(3935735)
```

### Comparing `movingpandas-0.9rc2/movingpandas/tests/test_overlay.py` & `movingpandas-0.9rc3/movingpandas/tests/test_overlay.py`

 * *Files identical despite different names*

### Comparing `movingpandas-0.9rc2/movingpandas/tests/test_point_clusterer.py` & `movingpandas-0.9rc3/movingpandas/tests/test_point_clusterer.py`

 * *Files identical despite different names*

### Comparing `movingpandas-0.9rc2/movingpandas/tests/test_show_versions.py` & `movingpandas-0.9rc3/movingpandas/tests/test_show_versions.py`

 * *Files identical despite different names*

### Comparing `movingpandas-0.9rc2/movingpandas/tests/test_trajectory.py` & `movingpandas-0.9rc3/movingpandas/tests/test_trajectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,14 +261,20 @@
     def test_add_direction(self):
         traj = make_traj(
             [Node(0, 0), Node(6, 0, day=2), Node(6, -6, day=3), Node(-6, -6, day=4)]
         )
         traj.add_direction()
         assert traj.df[DIRECTION_COL_NAME].tolist() == [90.0, 90.0, 180.0, 270]
 
+    def test_add_direction_only_adds_direction_col_and_doesnt_otherwise_alter_df(self):
+        traj = self.default_traj_metric_5.copy()
+        traj.add_direction()
+        traj.df = traj.df.drop(columns=[DIRECTION_COL_NAME])
+        assert_frame_equal(self.default_traj_metric_5.df, traj.df)
+
     def test_add_direction_latlon(self):
         traj = make_traj([Node(0, 0), Node(10, 10, day=2)], CRS_LATLON)
         traj.add_direction()
         result = traj.df[DIRECTION_COL_NAME].tolist()
         assert result[0] == pytest.approx(44.561451413257714, 5)
         assert result[1] == pytest.approx(44.561451413257714, 5)
 
@@ -446,14 +452,21 @@
     def test_hvplot_exists(self):
         import holoviews
 
         plot = self.default_traj_latlon.hvplot(geo=True)
         assert isinstance(plot, holoviews.core.overlay.Overlay)
         assert len(plot.Path.ddims) == 2
 
+    def test_hvplot_with_speed_exists(self):
+        import holoviews
+
+        plot = self.default_traj_latlon.hvplot(geo=True, c="speed")
+        assert isinstance(plot, holoviews.core.overlay.Overlay)
+        assert len(plot.Path.ddims) == 3
+
     def test_hvplot_exists_without_crs(self):
         import holoviews
 
         traj = make_traj([Node(0, 0), Node(10, 10, day=2)], None)
         plot = traj.hvplot()
         assert isinstance(plot, holoviews.core.overlay.Overlay)
```

### Comparing `movingpandas-0.9rc2/movingpandas/tests/test_trajectory_aggregator.py` & `movingpandas-0.9rc3/movingpandas/tests/test_trajectory_aggregator.py`

 * *Files identical despite different names*

### Comparing `movingpandas-0.9rc2/movingpandas/tests/test_trajectory_cleaner.py` & `movingpandas-0.9rc3/movingpandas/tests/test_trajectory_cleaner.py`

 * *Files identical despite different names*

### Comparing `movingpandas-0.9rc2/movingpandas/tests/test_trajectory_collection.py` & `movingpandas-0.9rc3/movingpandas/tests/test_trajectory_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,25 +100,27 @@
         assert locs.iloc[0].geometry in [Point(0, 0), Point(10, 10)]
         assert locs.iloc[0].id in [1, 2]
         assert locs.iloc[0].obj == "A"
         assert locs.iloc[0].val in [9, 10]
         assert locs.iloc[0].val2 in ["a", "e"]
         assert locs.iloc[1].geometry in [Point(0, 0), Point(10, 10)]
         assert locs.iloc[0].geometry != locs.iloc[1].geometry
+        assert isinstance(locs, GeoDataFrame)
 
     def test_get_end_locations(self):
         locs = self.collection.get_end_locations()
         assert len(locs) == 2
         assert locs.iloc[0].geometry in [Point(9, 9), Point(190, 10)]
         assert locs.iloc[0].id in [1, 2]
         assert locs.iloc[0].obj == "A"
         assert locs.iloc[0].val in [4, 3]
         assert locs.iloc[0].val2 in ["d", "h"]
         assert locs.iloc[1].geometry in [Point(9, 9), Point(190, 10)]
         assert locs.iloc[0].geometry != locs.iloc[1].geometry
+        assert isinstance(locs, GeoDataFrame)
 
     def test_get_intersecting(self):
         polygon = Polygon([(-1, -1), (-1, 1), (1, 1), (1, -1), (-1, -1)])
         collection = self.collection.get_intersecting(polygon)
         assert len(collection) == 1
         assert collection.trajectories[0] == self.collection.trajectories[0]
```

### Comparing `movingpandas-0.9rc2/movingpandas/tests/test_trajectory_generalizer.py` & `movingpandas-0.9rc3/movingpandas/tests/test_trajectory_generalizer.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import pandas as pd
 from geopandas import GeoDataFrame
 from shapely.geometry import Point
 from fiona.crs import from_epsg
 from datetime import datetime, timedelta
 from .test_trajectory import make_traj, Node
+from movingpandas.trajectory import Trajectory
 from movingpandas.trajectory_collection import TrajectoryCollection
 from movingpandas.trajectory_generalizer import (
     MaxDistanceGeneralizer,
     MinDistanceGeneralizer,
     MinTimeDeltaGeneralizer,
     DouglasPeuckerGeneralizer,
     TopDownTimeRatioGeneralizer,
@@ -18,14 +19,27 @@
 
 CRS_METRIC = from_epsg(31256)
 CRS_LATLON = from_epsg(4326)
 
 
 class TestTrajectoryGeneralizer:
     def setup_method(self):
+        self.nodes = [
+            Node(0, 0, day=1),
+            Node(1, 0.1, day=2),
+            Node(2, 0.2, day=3),
+            Node(3, 0, day=4),
+            Node(3, 3, day=5),
+        ]
+        self.traj = make_traj(self.nodes)
+        df = pd.DataFrame(
+            [{"xxx": n.geometry, "t": n.t} for n in self.nodes]
+        ).set_index("t")
+        geo_df = GeoDataFrame(df, geometry="xxx", crs=CRS_METRIC)
+        self.traj_other_geometry_column_names = Trajectory(geo_df, 1)
         df = pd.DataFrame(
             [
                 [1, "A", Point(0, 0), datetime(2018, 1, 1, 12, 0, 0), 9, "a"],
                 [1, "A", Point(6, 0), datetime(2018, 1, 1, 12, 6, 0), 5, "b"],
                 [1, "A", Point(6, 6), datetime(2018, 1, 1, 14, 10, 0), 2, "c"],
                 [1, "A", Point(9, 9), datetime(2018, 1, 1, 14, 15, 0), 4, "d"],
                 [2, "A", Point(10, 10), datetime(2018, 1, 1, 12, 0, 0), 10, "e"],
@@ -35,61 +49,55 @@
             ],
             columns=["id", "obj", "geometry", "t", "val", "val2"],
         ).set_index("t")
         self.geo_df = GeoDataFrame(df, crs=CRS_METRIC)
         self.collection = TrajectoryCollection(self.geo_df, "id", obj_id_col="obj")
 
     def test_douglas_peucker(self):
-        nodes = [
-            Node(0, 0, day=1),
-            Node(1, 0.1, day=2),
-            Node(2, 0.2, day=3),
-            Node(3, 0, day=4),
-            Node(3, 3, day=5),
-        ]
-        traj = make_traj(nodes)
-        result = DouglasPeuckerGeneralizer(traj).generalize(tolerance=1)
-        assert result == make_traj([nodes[0], nodes[3], nodes[4]])
+        result = DouglasPeuckerGeneralizer(self.traj).generalize(tolerance=1)
+        assert result == make_traj([self.nodes[0], self.nodes[3], self.nodes[4]])
+
+    def test_douglas_peucker_for_other_geometry_column_names(self):
+        result = DouglasPeuckerGeneralizer(
+            self.traj_other_geometry_column_names
+        ).generalize(tolerance=1)
+        assert result == make_traj([self.nodes[0], self.nodes[3], self.nodes[4]])
 
     def test_tdtr(self):
-        nodes = [
-            Node(0, 0, day=1),
-            Node(1, 0.1, day=2),
-            Node(2, 0.2, day=3),
-            Node(3, 0, day=4),
-            Node(3, 3, day=5),
-        ]
-        traj = make_traj(nodes)
-        result = TopDownTimeRatioGeneralizer(traj).generalize(tolerance=1)
-        assert result == make_traj([nodes[0], nodes[3], nodes[4]])
+        result = TopDownTimeRatioGeneralizer(self.traj).generalize(tolerance=1)
+        assert result == make_traj([self.nodes[0], self.nodes[3], self.nodes[4]])
 
     def test_tdtr_different_than_dp(self):
         nodes = [
             Node(),
             Node(1, 0.1, hour=1),
             Node(1, 2, hour=7),
             Node(2, 2, hour=15),
             Node(3, 0, hour=16),
             Node(3, 3, hour=17),
         ]
         traj = make_traj(nodes)
         result = TopDownTimeRatioGeneralizer(traj).generalize(tolerance=1)
         assert result == make_traj([nodes[0], nodes[2], nodes[3], nodes[4], nodes[5]])
 
+    def test_tdtr_for_other_geometry_column_names(self):
+        result = TopDownTimeRatioGeneralizer(
+            self.traj_other_geometry_column_names
+        ).generalize(tolerance=1)
+        assert result == make_traj([self.nodes[0], self.nodes[3], self.nodes[4]])
+
     def test_max_distance(self):
-        nodes = [
-            Node(0, 0, day=1),
-            Node(1, 0.1, day=2),
-            Node(2, 0.2, day=3),
-            Node(3, 0, day=4),
-            Node(3, 3, day=5),
-        ]
-        traj = make_traj(nodes)
-        result = MaxDistanceGeneralizer(traj).generalize(tolerance=1)
-        assert result == make_traj([nodes[0], nodes[3], nodes[4]])
+        result = MaxDistanceGeneralizer(self.traj).generalize(tolerance=1)
+        assert result == make_traj([self.nodes[0], self.nodes[3], self.nodes[4]])
+
+    def test_max_distance_for_other_geometry_column_names(self):
+        result = MaxDistanceGeneralizer(
+            self.traj_other_geometry_column_names
+        ).generalize(tolerance=1)
+        assert result == make_traj([self.nodes[0], self.nodes[3], self.nodes[4]])
 
     def test_min_time_delta(self):
         nodes = [
             Node(),
             Node(1, 0.1, minute=6),
             Node(2, 0.2, minute=10),
             Node(3, 0, minute=30),
```

### Comparing `movingpandas-0.9rc2/movingpandas/tests/test_trajectory_plotter.py` & `movingpandas-0.9rc3/movingpandas/tests/test_trajectory_plotter.py`

 * *Files identical despite different names*

### Comparing `movingpandas-0.9rc2/movingpandas/tests/test_trajectory_smoother.py` & `movingpandas-0.9rc3/movingpandas/tests/test_trajectory_smoother.py`

 * *Files identical despite different names*

### Comparing `movingpandas-0.9rc2/movingpandas/tests/test_trajectory_splitter.py` & `movingpandas-0.9rc3/movingpandas/tests/test_trajectory_splitter.py`

 * *Files identical despite different names*

### Comparing `movingpandas-0.9rc2/movingpandas/tests/test_trajectory_stop_detector.py` & `movingpandas-0.9rc3/movingpandas/tests/test_trajectory_stop_detector.py`

 * *Files identical despite different names*

### Comparing `movingpandas-0.9rc2/movingpandas/time_range_utils.py` & `movingpandas-0.9rc3/movingpandas/time_range_utils.py`

 * *Files identical despite different names*

### Comparing `movingpandas-0.9rc2/movingpandas/tools/_show_versions.py` & `movingpandas-0.9rc3/movingpandas/tools/_show_versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
         "pyproj",
         "matplotlib",
         "mapclassify",
         "geopy",
         "holoviews",
         "hvplot",
         "geoviews",
+        "stonesoup",
     ]
 
     def get_version(module):
         return module.__version__
 
     deps_info = {}
```

### Comparing `movingpandas-0.9rc2/movingpandas/trajectory.py` & `movingpandas-0.9rc3/movingpandas/trajectory.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,17 +469,17 @@
         -------
         Pandas series
             Row of the DataFrame at time t
         """
         try:
             return self.df.loc[t]
         except KeyError:
-            return self.df.iloc[
-                self.df.index.sort_values().drop_duplicates().get_loc(t, method=method)
-            ]
+            index = self.df.index.sort_values().drop_duplicates()
+            idx = index.get_indexer([t], method=method)[0]
+            return self.df.iloc[idx]
 
     def interpolate_position_at(self, t):
         """
         Compute and return interpolated position at time t.
 
         Parameters
         ----------
@@ -754,14 +754,15 @@
                 "Use overwrite=True to overwrite exiting values."
             )
         self._add_prev_pt()
         self.df[DIRECTION_COL_NAME] = self.df.apply(self._compute_heading, axis=1)
         self.df.at[self.get_start_time(), DIRECTION_COL_NAME] = self.df.iloc[1][
             DIRECTION_COL_NAME
         ]
+        self.df.drop(columns=["prev_pt"], inplace=True)
 
     def add_distance(self, overwrite=False):
         """
         Add distance column and values to the trajectory's DataFrame.
 
         Distance is calculated as CRS units, except if the CRS is geographic
         (e.g. EPSG:4326 WGS84) then distance is calculated in meters.
```

### Comparing `movingpandas-0.9rc2/movingpandas/trajectory_aggregator.py` & `movingpandas-0.9rc3/movingpandas/trajectory_aggregator.py`

 * *Files identical despite different names*

### Comparing `movingpandas-0.9rc2/movingpandas/trajectory_cleaner.py` & `movingpandas-0.9rc3/movingpandas/trajectory_cleaner.py`

 * *Files identical despite different names*

### Comparing `movingpandas-0.9rc2/movingpandas/trajectory_collection.py` & `movingpandas-0.9rc3/movingpandas/trajectory_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,14 +190,24 @@
         -------
         Trajectory
         """
         for traj in self:
             if traj.id == traj_id:
                 return traj
 
+    def get_geom_column_name(self):
+        """
+        Return name of the geometry column
+
+        Returns
+        -------
+        string
+        """
+        return self.trajectories[0].get_geom_column_name()
+
     def get_locations_at(self, t):
         """
         Returns GeoDataFrame with trajectory locations at the specified timestamp
 
         Parameters
         ----------
         t : datetime.datetime
@@ -214,15 +224,15 @@
             elif t == "end":
                 x = traj.get_row_at(traj.get_end_time())
             else:
                 if t < traj.get_start_time() or t > traj.get_end_time():
                     continue
                 x = traj.get_row_at(t)
             gdf = gdf.append(x)
-        return gdf
+        return GeoDataFrame(gdf)
 
     def get_start_locations(self):
         """
         Returns GeoDataFrame with trajectory start locations
 
         Returns
         -------
```

### Comparing `movingpandas-0.9rc2/movingpandas/trajectory_generalizer.py` & `movingpandas-0.9rc3/movingpandas/trajectory_generalizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         Create TrajectoryGeneralizer
 
         Parameters
         ----------
         traj : Trajectory or TrajectoryCollection
         """
         self.traj = traj
+        self.traj_col_name = traj.get_geom_column_name()
 
     def generalize(self, tolerance):
         """
         Generalize the input Trajectory/TrajectoryCollection.
 
         Parameters
         ----------
@@ -183,14 +184,20 @@
 class DouglasPeuckerGeneralizer(TrajectoryGeneralizer):
     """
     Generalizes using Douglas-Peucker algorithm (as implemented in shapely/Geos).
 
     tolerance : float
         Distance tolerance in trajectory CRS units
 
+    References
+    ----------
+    * Douglas, D., & Peucker, T. (1973). Algorithms for the reduction of the number
+      of points required to represent a digitized line or its caricature.
+      The Canadian Cartographer 10(2), 112–122. doi:10.3138/FM57-6770-U75U-7727.
+
     Examples
     --------
 
     >>> mpd.DouglasPeuckerGeneralizer(traj).generalize(tolerance=1.0)
     """
 
     def _generalize_traj(self, traj, tolerance):
@@ -234,31 +241,35 @@
     Examples
     --------
 
     >>> mpd.TopDownTimeRatioGeneralizer(traj).generalize(tolerance=1.0)
     """
 
     def _generalize_traj(self, traj, tolerance):
-        return Trajectory(self.td_tr(traj.df.copy(), tolerance), traj.id)
+        generalized = self.td_tr(traj.df.copy(), tolerance)
+        return Trajectory(generalized, traj.id)
 
     def td_tr(self, df, tolerance):
         if len(df) <= 2:
             return df
         else:
             de = (
                 df.index.max().to_pydatetime() - df.index.min().to_pydatetime()
             ).total_seconds()
 
-            dx = df.geometry.iloc[-1].x - df.geometry.iloc[0].x
-            dy = df.geometry.iloc[-1].y - df.geometry.iloc[0].y
+            t0 = df.index.min().to_pydatetime()
+
+            pt0 = df[self.traj_col_name].iloc[0]
+            ptn = df[self.traj_col_name].iloc[-1]
+
+            dx = ptn.x - pt0.x
+            dy = ptn.y - pt0.y
 
             dists = df.apply(
-                lambda rec: self._dist_from_calced(
-                    rec, df.index.min().to_pydatetime(), df.geometry.iloc[0], de, dx, dy
-                ),
+                lambda rec: self._dist_from_calced(rec, t0, pt0, de, dx, dy),
                 axis=1,
             )
 
             if dists.max() > tolerance:
                 return pd.concat(
                     [
                         self.td_tr(
@@ -271,8 +282,8 @@
                 )
             else:
                 return df.iloc[[0, -1]]
 
     def _dist_from_calced(self, rec, start_t, start_geom, de, dx, dy):
         di = (rec.name - start_t).total_seconds()
         calced = Point(start_geom.x + dx * di / de, start_geom.y + dy * di / de)
-        return rec.geometry.distance(calced)
+        return rec[self.traj_col_name].distance(calced)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `movingpandas-0.9rc2/movingpandas/trajectory_plotter.py` & `movingpandas-0.9rc3/movingpandas/trajectory_plotter.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 
         self.width = kwargs.pop("width", 900)
         self.height = kwargs.pop("height", 700)
         self.figsize = kwargs.pop("figsize", None)
         self.column = kwargs.get("column", None)
         self.column = kwargs.get("c", self.column)
         self.ax = kwargs.pop("ax", None)
-        self.column_to_color = kwargs.pop("column_to_color", None)
+        self.colormap = kwargs.pop("colormap", None)
+        self.colormap = kwargs.pop("column_to_color", self.colormap)
 
         self.min_value = self.kwargs.get("vmin", None)
         self.max_value = self.kwargs.get("vmax", None)
 
         self.overlay = None
         self.hvplot_is_geo = kwargs.pop("geo", True)
         self.hvplot_tiles = kwargs.pop("tiles", "OSM")
@@ -47,17 +48,17 @@
         line_gdf = line_gdf.rename(columns={"line": "geometry"}).set_geometry(
             "geometry"
         )
         return line_gdf
 
     def _plot_trajectory(self, traj):
         temp_df = self._make_line_df(traj)
-        if self.column and self.column_to_color:
+        if self.column and self.colormap:
             try:
-                color = self.column_to_color[traj.df[self.column].max()]
+                color = self.colormap[traj.df[self.column].max()]
             except KeyError:
                 color = "grey"
             return temp_df.plot(ax=self.ax, color=color, *self.args, **self.kwargs)
         else:
             self.kwargs.pop("vmin", None)
             self.kwargs.pop("vmax", None)
             return temp_df.plot(
@@ -66,29 +67,30 @@
                 vmax=self.max_value,
                 *self.args,
                 **self.kwargs
             )
 
     def _hvplot_trajectory(self, traj):
         line_gdf = self._make_line_df(traj)
-        if not traj.is_latlon and traj.crs is not None:
+        if self.hvplot_is_geo and not traj.is_latlon and traj.crs is not None:
             line_gdf = line_gdf.to_crs(epsg=4326)
         if self.column and isinstance(self.column, str):
             self.kwargs["c"] = dim(
                 self.column
             )  # fixes https://github.com/anitagraser/movingpandas/issues/71
-        if self.column and self.column_to_color:
+        if self.column and self.colormap:
             try:
-                color = self.column_to_color[traj.df[self.column].max()]
+                color = self.colormap[traj.df[self.column].max()]
             except KeyError:
                 color = "grey"
             return line_gdf.hvplot(
                 color=color,
                 geo=self.hvplot_is_geo,
                 tiles=self.hvplot_tiles,
+                label=traj.df[self.column].max(),
                 *self.args,
                 **self.kwargs
             )
         else:
             return line_gdf.hvplot(
                 geo=self.hvplot_is_geo,
                 tiles=self.hvplot_tiles,
```

### Comparing `movingpandas-0.9rc2/movingpandas/trajectory_smoother.py` & `movingpandas-0.9rc3/movingpandas/trajectory_smoother.py`

 * *Files identical despite different names*

### Comparing `movingpandas-0.9rc2/movingpandas/trajectory_splitter.py` & `movingpandas-0.9rc3/movingpandas/trajectory_splitter.py`

 * *Files identical despite different names*

### Comparing `movingpandas-0.9rc2/movingpandas/trajectory_stop_detector.py` & `movingpandas-0.9rc3/movingpandas/trajectory_stop_detector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 
 from geopandas import GeoDataFrame
+from shapely.geometry import MultiPoint
 from .trajectory import Trajectory
 from .trajectory_collection import TrajectoryCollection
 from .geometry_utils import mrr_diagonal
 from .trajectory_utils import convert_time_ranges_to_segments
 from .time_range_utils import TemporalRangeWithTrajId
 
 
@@ -55,33 +56,36 @@
                 result.append(time_range)
         return result
 
     def _process_traj(self, traj, max_diameter, min_duration):
         detected_stops = []
         segment_geoms = []
         segment_times = []
+        geom = MultiPoint()
         is_stopped = False
         previously_stopped = False
-        geom_column_name = traj.get_geom_column_name()
 
-        for index, row in traj.df.iterrows():
-            segment_geoms.append(row[geom_column_name])
+        for index, data in traj.df[traj.get_geom_column_name()].iteritems():
+            segment_geoms.append(data)
+            geom = geom.union(data)
             segment_times.append(index)
 
             if not is_stopped:  # remove points to the specified min_duration
                 while (
                     len(segment_geoms) > 2
                     and segment_times[-1] - segment_times[0] >= min_duration
                 ):
                     segment_geoms.pop(0)
                     segment_times.pop(0)
+                # after removing extra points, re-generate geometry
+                geom = MultiPoint(segment_geoms)
 
             if (
                 len(segment_geoms) > 1
-                and mrr_diagonal(segment_geoms, traj.is_latlon) < max_diameter
+                and mrr_diagonal(geom, traj.is_latlon) < max_diameter
             ):
                 is_stopped = True
             else:
                 is_stopped = False
 
             if len(segment_geoms) > 1:
                 segment_end = segment_times[-2]
@@ -91,14 +95,15 @@
                         segment_end - segment_begin >= min_duration
                     ):  # detected end of a stop
                         detected_stops.append(
                             TemporalRangeWithTrajId(segment_begin, segment_end, traj.id)
                         )
                         segment_geoms = []
                         segment_times = []
+                        geom = MultiPoint()
 
             previously_stopped = is_stopped
 
         if is_stopped and segment_times[-1] - segment_times[0] >= min_duration:
             detected_stops.append(
                 TemporalRangeWithTrajId(segment_times[0], segment_times[-1], traj.id)
             )
```

### Comparing `movingpandas-0.9rc2/movingpandas/trajectory_utils.py` & `movingpandas-0.9rc3/movingpandas/trajectory_utils.py`

 * *Files identical despite different names*

### Comparing `movingpandas-0.9rc2/movingpandas.egg-info/PKG-INFO` & `movingpandas-0.9rc3/movingpandas.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,178 +1,181 @@
 Metadata-Version: 2.1
 Name: movingpandas
-Version: 0.9rc2
-Summary: Implementation of Trajectory classes and functions built on top of GeoPandas
+Version: 0.9rc3
+Summary: MovingPandas implements Trajectory classes and corresponding methods for the analysis of movement data based on GeoPandas. Visit movingpandas.org for details.
 Home-page: https://github.com/anitagraser/movingpandas
 Author: Anita Graser
 Author-email: anitagraser@gmx.at
 License: UNKNOWN
-Description: # MovingPandas
-        
-        [![Project Status: Active â€“ The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
-        [![Tests](https://github.com/anitagraser/movingpandas/actions/workflows/tests.yaml/badge.svg)](https://github.com/anitagraser/movingpandas/actions/workflows/tests.yaml)
-        [![docs status](https://readthedocs.org/projects/movingpandas/badge/?version=master)](https://movingpandas.readthedocs.io/en/master/)
-        [![codecov](https://codecov.io/gh/anitagraser/movingpandas/branch/master/graph/badge.svg)](https://codecov.io/gh/anitagraser/movingpandas)
-        [![DOI](https://zenodo.org/badge/161995245.svg)](https://zenodo.org/badge/latestdoi/161995245)
-        [![pyOpenSci](https://camo.githubusercontent.com/63ff31cdb80a06361e53ac2b9ac0d184118ebd0b/68747470733a2f2f74696e7975726c2e636f6d2f7932326e62387570)](https://github.com/pyOpenSci/software-review/issues/18)
-        
-        <img align="right" src="https://anitagraser.github.io/movingpandas/assets/img/movingpandas.png">
-        
-        MovingPandas implements a Trajectory class and corresponding methods based on **[GeoPandas](https://geopandas.org)**.
-        
-        Visit **[movingpandas.org](http://movingpandas.org)** for details! 
-        
-        You can run **[MovingPandas examples](https://github.com/anitagraser/movingpandas-examples)** on MyBinder - no installation required: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/anitagraser/movingpandas-examples/main) (These examples use the latest MovingPandas release version.) 
-        
-        To try the cutting-edge dev version, use [this MyBinder link](https://mybinder.org/v2/gh/anitagraser/movingpandas/master?filepath=tutorials/1-getting-started.ipynb).
-        
-        ## Documentation
-        
-        The official documentation is hosted on **[ReadTheDocs](https://movingpandas.readthedocs.io)**
-        
-        ## Examples
-        
-        ### Trajectory plots
-        
-        ![movingpandas_animated](https://user-images.githubusercontent.com/590385/137953765-33f9ce1b-037c-4c86-82b2-0620de5ca28f.gif)
-        
-        ### Stop detection
-        
-        ![movingpandas_stop_detection](https://user-images.githubusercontent.com/590385/137953859-3df81568-eda8-4443-96b8-e82e15c03653.png)
-        
-        ### Trajectory generalization
-        
-        ![movingpandas_generalize](https://user-images.githubusercontent.com/590385/142756559-012a15fe-736c-474c-b244-0ee02090d592.gif)
-        
-        ### Trajectory aggregation
-        
-        ![movingpandas_ais](https://user-images.githubusercontent.com/590385/137953890-d43c7fe5-5aea-4e29-8ce1-f0d529c3220f.png)
-        
-        ## Installation
-        
-        MovingPandas for Python >= 3.7 and all it's dependencies are available from [conda-forge](https://anaconda.org/conda-forge/movingpandas) and can be installed using `conda install -c conda-forge movingpandas`.
-        
-        **Conda status**
-        
-        [![Conda Recipe](https://img.shields.io/badge/recipe-movingpandas-green.svg)](https://anaconda.org/conda-forge/movingpandas) 
-        [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/movingpandas.svg)](https://anaconda.org/conda-forge/movingpandas) 
-        [![Conda Version](https://img.shields.io/conda/vn/conda-forge/movingpandas.svg)](https://anaconda.org/conda-forge/movingpandas) 
-        [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/movingpandas.svg)](https://anaconda.org/conda-forge/movingpandas)
-        
-        Note that it is **NOT recommended** to install MovingPandas from [PyPI](https://pypi.org/project/movingpandas/)!
-        If you're on Windows or Mac, many GeoPandas / MovingPandas dependencies cannot be pip installed 
-        (for details see the corresponding notes in the [GeoPandas documentation](https://geopandas.readthedocs.io/en/latest/getting_started/install.html)).
-        On Ubuntu, pip install fails on cartopy with "Proj 4.9.0 must be installed".
-        
-        ## Development Installation 
-        
-        Use the following steps to run the notebooks using the current development version:
-        
-        ### Using conda
-        
-        **Linux/Mac**:  
-        
-        ```
-        conda env create -f environment.yml
-        ```
-        
-        **Windows**: 
-        
-        ```
-        conda config --add channels conda-forge
-        conda config --add channels defaults
-        conda config --set channel_priority strict
-        conda env create -f environment.yml
-        ```
-        
-        *On Windows, because conda-forge relies on some package built with defaults blas (like scipy) one must use the defaults channel on top of conda-forge and activate conda's new strict channel feature.* Source: https://github.com/conda-forge/gdal-feedstock/issues/269#issuecomment-473661530
-        
-        ### Using Anaconda
-        
-        1. Install Anaconda
-        2. Clone the movingpandas repository
-        3. In Anaconda Navigator | Environments | Import select the movingpandas environment.yml from the cloned directory:
-        
-        ![image](https://user-images.githubusercontent.com/590385/62143367-2db14c00-b2f0-11e9-8cb9-fb7993b7f62e.png)
-        
-        4. Wait until the environment is ready, then change to the Home tab and install Jupyter notebooks into the movingpandas environment
-        5. Launch Jupyter notebooks and navigate to the `movingpandas/tutorials` directory to execute them
-        6. Now you can run the notebooks, experiment with the code and adjust it to your own data
-        
-        Known issues:
-        
-        * On Windows, importing rasterio can lead to DLL errors. If this happens, downgrade the rasterio version to 1.0.13.
-        
-        ### Develop mode
-        
-        To install MovingPandas in ["develop" or "editable" mode](https://python-packaging-tutorial.readthedocs.io/en/latest/setup_py.html#develop-mode) you may use: 
-        
-        ```
-        python setup.py develop
-        ```
-        
-        ## Contributing to MovingPandas [![GitHub contributors](https://img.shields.io/github/contributors/anitagraser/movingpandas.svg)](https://github.com/anitagraser/movingpandas/graphs/contributors)
-        
-        All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.
-        
-        A detailed overview on how to contribute can be found in the [contributing guide](https://github.com/anitagraser/movingpandas/blob/master/CONTRIBUTING.md) on GitHub.
-        
-        ## Related Python Packages
-        
-        **For a more comprehensive list, including non-Python solutions, check https://github.com/anitagraser/movement-analysis-tools**
-        
-        [scikit-mobility](https://github.com/scikit-mobility/scikit-mobility) is a similar package which also deals with movement data. 
-        It implements TrajectoryDataFrames and FlowDataFrames on top of Pandas instead of GeoPandas. 
-        There is little overlap in the covered use cases and implemented functionality (comparing 
-        [MovingPandas tutorials](https://github.com/anitagraser/movingpandas/tree/master/tutorials) and 
-        [scikit-mobility tutorials](https://github.com/scikit-mobility/tutorials)). 
-        MovingPandas focuses on spatio-temporal data exploration with corresponding functions for data manipulation and analysis. 
-        scikit-mobility on the other hand focuses on computing human mobility metrics, generating synthetic trajectories 
-        and assessing privacy risks. Plotting is based on Folium. 
-        
-        [Traja](https://github.com/traja-team/traja) extends the capabilitis of Pandas DataFrames specific for animal trajectory analysis in 2D. Plots (static) are based on seaborn. 
-        
-        [PyMove](https://github.com/InsightLab/PyMove) provides functionality similar to MovingPandas. 
-        It implements PandasMoveDataFrames and DaskMoveDataFrame on top of Pandas and Dask DataFrames. Plotting is based on Folium. 
-        
-        [Tracktable](https://github.com/sandialabs/tracktable) is a related Python package with its core data structures and algorithms implemented in C++, i.e. it is not based on Pandas. Plotting is based on Cartopy (for still images) and Folium (for interactive rendering).
-        
-        ## Citation information
-        
-        Please cite [[0]](#publications) when using MovingPandas in your research and reference the appropriate release version. All releases of MovingPandas are listed on [Zenodo](https://doi.org/10.5281/zenodo.3710950) where you will find citation information, including DOIs.  
-        
-        ## Publications
-        
-        ### About MovingPandas
-        
-        [0] [Graser, A. (2019). MovingPandas: Efficient Structures for Movement Data in Python. GI_Forum â€’ Journal of Geographic Information Science 2019, 1-2019, 54-68. doi:10.1553/giscience2019_01_s54.](https://www.austriaca.at/rootcollection?arp=0x003aba2b)
-        
-        [1] [Graser, A. & Dragaschnig, M. (2020). Exploring movement data in notebook environments. Presented at MoVIS 2020, IEEE VIS 2020.](http://move.geog.ucsb.edu/wp-content/uploads/2020/10/MoVIS20_paper_4.pdf)
-        
-        ### Scientific Publications Referencing MovingPandas
-        
-        * [Pappalardo, L., Simini, F., Barlacchi, G., & Pellungrini, R. (2019). scikit-mobility: A Python library for the analysis, generation and risk assessment of mobility data. arXiv preprint arXiv:1907.07062.](https://arxiv.org/abs/1907.07062)
-        * [Graser, A. & Dragaschnig, M. (2020). Open Geospatial Tools for Movement Data Exploration. KN â€’ Journal of Cartography and Geographic Information, 70(1), 3-10. doi:10.1007/s42489-020-00039-y.](https://link.springer.com/article/10.1007/s42489-020-00039-y)
-        * [Kirkland, L. A., de Waal, A., & de Villiers, J. P. (2020). Evaluation of a Pure-Strategy Stackelberg Game for Wildlife Security in a Geospatial Framework. In Southern African Conference for Artificial Intelligence Research (pp. 101-118). Springer, Cham.](https://link.springer.com/chapter/10.1007/978-3-030-66151-9_7)
-        * [Depellegrin, D., Bastianini, M., Fadini, A., & Menegon, S. (2020). The effects of COVID-19 induced lockdown measures on maritime settings of a coastal region. Science of the Total Environment, 740, 140123.](https://doi.org/10.1016/j.scitotenv.2020.140123)
-        * [Graser, A. (2021). An exploratory data analysis protocol for identifying problems in continuous movement data. Journal of Location Based Services. doi:10.1080/17489725.2021.1900612.](https://doi.org/10.1080/17489725.2021.1900612)
-        * [Mehri, S., Alesheikh, A. A., & Basiri, A. (2021). A Contextual Hybrid Model for Vessel Movement Prediction. IEEE Access, 9, 45600-45613.](https://ieeexplore.ieee.org/abstract/document/9380635/)
-        
-        [Full Google Scholar list](https://scholar.google.com/scholar?oi=bibs&hl=en&cites=10366998261774464895)
-        
-        ### Teaching Material Referencing MovingPandas
-        
-        * [Aalto University. Spatial data science for sustainable development course](https://sustainability-gis.readthedocs.io/en/latest/lessons/L3/mobility-analytics.html)
-        
-        ### Workshop Videos
-        
-        * [Graser, A. (2019). Analyzing Movement Data with MovingPandas. Workshop at the OpenGeoHub summer school, MÃ¼nster, Germany.](http://www.youtube.com/watch?v=qeLQfnpJV1g)
-        
-        [![WorkshopVideo](https://user-images.githubusercontent.com/590385/67161044-f08cb100-f356-11e9-8799-f972175ec7f4.png)](http://www.youtube.com/watch?v=qeLQfnpJV1g "Anita Graser: Analyzing movement data")
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: smoothing
+License-File: LICENSE.txt
+
+# MovingPandas
+
+[![Project Status: Active â€“ The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
+[![Tests](https://github.com/anitagraser/movingpandas/actions/workflows/tests.yaml/badge.svg)](https://github.com/anitagraser/movingpandas/actions/workflows/tests.yaml)
+[![docs status](https://readthedocs.org/projects/movingpandas/badge/?version=master)](https://movingpandas.readthedocs.io/en/master/)
+[![codecov](https://codecov.io/gh/anitagraser/movingpandas/branch/master/graph/badge.svg)](https://codecov.io/gh/anitagraser/movingpandas)
+[![DOI](https://zenodo.org/badge/161995245.svg)](https://zenodo.org/badge/latestdoi/161995245)
+[![pyOpenSci](https://camo.githubusercontent.com/63ff31cdb80a06361e53ac2b9ac0d184118ebd0b/68747470733a2f2f74696e7975726c2e636f6d2f7932326e62387570)](https://github.com/pyOpenSci/software-review/issues/18)
+
+<img align="right" src="https://anitagraser.github.io/movingpandas/assets/img/movingpandas.png">
+
+MovingPandas implements a Trajectory class and corresponding methods based on **[GeoPandas](https://geopandas.org)**.
+
+Visit **[movingpandas.org](http://movingpandas.org)** for details! 
+
+You can run **[MovingPandas examples](https://github.com/anitagraser/movingpandas-examples)** on MyBinder - no installation required: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/anitagraser/movingpandas-examples/main) (These examples use the latest MovingPandas release version.) 
+
+To try the cutting-edge dev version, use [this MyBinder link](https://mybinder.org/v2/gh/anitagraser/movingpandas/master?filepath=tutorials/1-getting-started.ipynb).
+
+## Documentation
+
+The official documentation is hosted on **[ReadTheDocs](https://movingpandas.readthedocs.io)**
+
+## Examples
+
+### Trajectory plots
+
+![movingpandas_animated](https://user-images.githubusercontent.com/590385/137953765-33f9ce1b-037c-4c86-82b2-0620de5ca28f.gif)
+
+### Stop detection
+
+![movingpandas_stop_detection](https://user-images.githubusercontent.com/590385/137953859-3df81568-eda8-4443-96b8-e82e15c03653.png)
+
+### Trajectory generalization
+
+![movingpandas_generalize](https://user-images.githubusercontent.com/590385/142756559-012a15fe-736c-474c-b244-0ee02090d592.gif)
+
+### Trajectory aggregation
+
+![movingpandas_ais](https://user-images.githubusercontent.com/590385/137953890-d43c7fe5-5aea-4e29-8ce1-f0d529c3220f.png)
+
+## Installation
+
+MovingPandas for Python >= 3.7 and all it's dependencies are available from [conda-forge](https://anaconda.org/conda-forge/movingpandas) and can be installed using `conda install -c conda-forge movingpandas`.
+
+**Conda status**
+
+[![Conda Recipe](https://img.shields.io/badge/recipe-movingpandas-green.svg)](https://anaconda.org/conda-forge/movingpandas) 
+[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/movingpandas.svg)](https://anaconda.org/conda-forge/movingpandas) 
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/movingpandas.svg)](https://anaconda.org/conda-forge/movingpandas) 
+[![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/movingpandas.svg)](https://anaconda.org/conda-forge/movingpandas)
+
+Note that it is **NOT recommended** to install MovingPandas from [PyPI](https://pypi.org/project/movingpandas/)!
+If you're on Windows or Mac, many GeoPandas / MovingPandas dependencies cannot be pip installed 
+(for details see the corresponding notes in the [GeoPandas documentation](https://geopandas.readthedocs.io/en/latest/getting_started/install.html)).
+On Ubuntu, pip install fails on cartopy with "Proj 4.9.0 must be installed".
+
+## Development Installation 
+
+Use the following steps to run the notebooks using the current development version:
+
+### Using conda
+
+**Linux/Mac**:  
+
+```
+conda env create -f environment.yml
+```
+
+**Windows**: 
+
+```
+conda config --add channels conda-forge
+conda config --add channels defaults
+conda config --set channel_priority strict
+conda env create -f environment.yml
+```
+
+*On Windows, because conda-forge relies on some package built with defaults blas (like scipy) one must use the defaults channel on top of conda-forge and activate conda's new strict channel feature.* Source: https://github.com/conda-forge/gdal-feedstock/issues/269#issuecomment-473661530
+
+### Using Anaconda
+
+1. Install Anaconda
+2. Clone the movingpandas repository
+3. In Anaconda Navigator | Environments | Import select the movingpandas environment.yml from the cloned directory:
+
+![image](https://user-images.githubusercontent.com/590385/62143367-2db14c00-b2f0-11e9-8cb9-fb7993b7f62e.png)
+
+4. Wait until the environment is ready, then change to the Home tab and install Jupyter notebooks into the movingpandas environment
+5. Launch Jupyter notebooks and navigate to the `movingpandas/tutorials` directory to execute them
+6. Now you can run the notebooks, experiment with the code and adjust it to your own data
+
+Known issues:
+
+* On Windows, importing rasterio can lead to DLL errors. If this happens, downgrade the rasterio version to 1.0.13.
+
+### Develop mode
+
+To install MovingPandas in ["develop" or "editable" mode](https://python-packaging-tutorial.readthedocs.io/en/latest/setup_py.html#develop-mode) you may use: 
+
+```
+python setup.py develop
+```
+
+## Contributing to MovingPandas [![GitHub contributors](https://img.shields.io/github/contributors/anitagraser/movingpandas.svg)](https://github.com/anitagraser/movingpandas/graphs/contributors)
+
+All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.
+
+A detailed overview on how to contribute can be found in the [contributing guide](https://github.com/anitagraser/movingpandas/blob/master/CONTRIBUTING.md) on GitHub.
+
+## Related Python Packages
+
+**For a more comprehensive list, including non-Python solutions, check https://github.com/anitagraser/movement-analysis-tools**
+
+[scikit-mobility](https://github.com/scikit-mobility/scikit-mobility) is a similar package which also deals with movement data. 
+It implements TrajectoryDataFrames and FlowDataFrames on top of Pandas instead of GeoPandas. 
+There is little overlap in the covered use cases and implemented functionality (comparing 
+[MovingPandas tutorials](https://github.com/anitagraser/movingpandas/tree/master/tutorials) and 
+[scikit-mobility tutorials](https://github.com/scikit-mobility/tutorials)). 
+MovingPandas focuses on spatio-temporal data exploration with corresponding functions for data manipulation and analysis. 
+scikit-mobility on the other hand focuses on computing human mobility metrics, generating synthetic trajectories 
+and assessing privacy risks. Plotting is based on Folium. 
+
+[Traja](https://github.com/traja-team/traja) extends the capabilitis of Pandas DataFrames specific for animal trajectory analysis in 2D. Plots (static) are based on seaborn. 
+
+[PyMove](https://github.com/InsightLab/PyMove) provides functionality similar to MovingPandas. 
+It implements PandasMoveDataFrames and DaskMoveDataFrame on top of Pandas and Dask DataFrames. Plotting is based on Folium. 
+
+[Tracktable](https://github.com/sandialabs/tracktable) is a related Python package with its core data structures and algorithms implemented in C++, i.e. it is not based on Pandas. Plotting is based on Cartopy (for still images) and Folium (for interactive rendering).
+
+## Citation information
+
+Please cite [[0]](#publications) when using MovingPandas in your research and reference the appropriate release version. All releases of MovingPandas are listed on [Zenodo](https://doi.org/10.5281/zenodo.3710950) where you will find citation information, including DOIs.  
+
+## Publications
+
+### About MovingPandas
+
+[0] [Graser, A. (2019). MovingPandas: Efficient Structures for Movement Data in Python. GI_Forum â€’ Journal of Geographic Information Science 2019, 1-2019, 54-68. doi:10.1553/giscience2019_01_s54.](https://www.austriaca.at/rootcollection?arp=0x003aba2b)
+
+[1] [Graser, A. & Dragaschnig, M. (2020). Exploring movement data in notebook environments. Presented at MoVIS 2020, IEEE VIS 2020.](http://move.geog.ucsb.edu/wp-content/uploads/2020/10/MoVIS20_paper_4.pdf)
+
+### Scientific Publications Referencing MovingPandas
+
+* [Pappalardo, L., Simini, F., Barlacchi, G., & Pellungrini, R. (2019). scikit-mobility: A Python library for the analysis, generation and risk assessment of mobility data. arXiv preprint arXiv:1907.07062.](https://arxiv.org/abs/1907.07062)
+* [Graser, A. & Dragaschnig, M. (2020). Open Geospatial Tools for Movement Data Exploration. KN â€’ Journal of Cartography and Geographic Information, 70(1), 3-10. doi:10.1007/s42489-020-00039-y.](https://link.springer.com/article/10.1007/s42489-020-00039-y)
+* [Kirkland, L. A., de Waal, A., & de Villiers, J. P. (2020). Evaluation of a Pure-Strategy Stackelberg Game for Wildlife Security in a Geospatial Framework. In Southern African Conference for Artificial Intelligence Research (pp. 101-118). Springer, Cham.](https://link.springer.com/chapter/10.1007/978-3-030-66151-9_7)
+* [Depellegrin, D., Bastianini, M., Fadini, A., & Menegon, S. (2020). The effects of COVID-19 induced lockdown measures on maritime settings of a coastal region. Science of the Total Environment, 740, 140123.](https://doi.org/10.1016/j.scitotenv.2020.140123)
+* [Graser, A. (2021). An exploratory data analysis protocol for identifying problems in continuous movement data. Journal of Location Based Services. doi:10.1080/17489725.2021.1900612.](https://doi.org/10.1080/17489725.2021.1900612)
+* [Mehri, S., Alesheikh, A. A., & Basiri, A. (2021). A Contextual Hybrid Model for Vessel Movement Prediction. IEEE Access, 9, 45600-45613.](https://ieeexplore.ieee.org/abstract/document/9380635/)
+
+[Full Google Scholar list](https://scholar.google.com/scholar?oi=bibs&hl=en&cites=10366998261774464895)
+
+### Teaching Material Referencing MovingPandas
+
+* [Aalto University. Spatial data science for sustainable development course](https://sustainability-gis.readthedocs.io/en/latest/lessons/L3/mobility-analytics.html)
+
+### Workshop Videos
+
+* [Graser, A. (2019). Analyzing Movement Data with MovingPandas. Workshop at the OpenGeoHub summer school, MÃ¼nster, Germany.](http://www.youtube.com/watch?v=qeLQfnpJV1g)
+
+[![WorkshopVideo](https://user-images.githubusercontent.com/590385/67161044-f08cb100-f356-11e9-8799-f972175ec7f4.png)](http://www.youtube.com/watch?v=qeLQfnpJV1g "Anita Graser: Analyzing movement data")
+
+
```

### Comparing `movingpandas-0.9rc2/movingpandas.egg-info/SOURCES.txt` & `movingpandas-0.9rc3/movingpandas.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 README.md
 setup.cfg
 setup.py
 movingpandas/__init__.py
 movingpandas/geometry_utils.py
 movingpandas/overlay.py
 movingpandas/point_clusterer.py
```

### Comparing `movingpandas-0.9rc2/setup.py` & `movingpandas-0.9rc3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 # Packages that MovingPandas uses explicitly:
 INSTALL_REQUIRES = [
-    'numpy', 'matplotlib', 'shapely<1.8',  # Geoviews is not yet compatible with shapely-1.8.0 https://github.com/holoviz/geoviews/issues/533
-    'pandas', 'geopandas', 'hvplot', 'bokeh', 'cartopy', 'geoviews', 'pyproj', 'geopy']
+    'numpy', 'matplotlib', 'shapely', 'pandas', 'geopandas', 'hvplot', 'bokeh', 'cartopy', 'geoviews', 'pyproj', 'geopy']
 
 setuptools.setup(
     name="movingpandas",
-    version="0.9.rc2",
+    version="0.9.rc3",
     author="Anita Graser",
     author_email="anitagraser@gmx.at",
-    description="Implementation of Trajectory classes and functions built on top of GeoPandas",
+    description="MovingPandas implements Trajectory classes and corresponding methods "
+                "for the analysis of movement data based on GeoPandas. "
+                "Visit movingpandas.org for details.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/anitagraser/movingpandas",
     packages=[
         "movingpandas",
         "movingpandas.tools",
         "movingpandas.tests",
```

