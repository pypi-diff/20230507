# Comparing `tmp/opstool-0.7.3.tar.gz` & `tmp/opstool-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opstool-0.7.3.tar", last modified: Fri Apr 14 09:19:37 2023, max compression
+gzip compressed data, was "opstool-0.8.0.tar", last modified: Sun May  7 06:04:22 2023, max compression
```

## Comparing `opstool-0.7.3.tar` & `opstool-0.8.0.tar`

### file list

```diff
@@ -1,55 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 09:19:37.701786 opstool-0.7.3/
--rw-rw-rw-   0        0        0    34817 2022-12-02 05:00:10.000000 opstool-0.7.3/LICENCE.txt
--rw-rw-rw-   0        0        0     6415 2023-04-14 09:19:37.701786 opstool-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     6005 2023-03-31 11:53:22.000000 opstool-0.7.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 09:19:37.701786 opstool-0.7.3/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-04-03 08:24:33.000000 opstool-0.7.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:19:37.672284 opstool-0.7.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 09:19:37.678043 opstool-0.7.3/src/opstool/
--rw-rw-rw-   0        0        0       23 2023-04-14 08:52:08.000000 opstool-0.7.3/src/opstool/__about__.py
--rw-rw-rw-   0        0        0      560 2023-03-30 08:46:47.000000 opstool-0.7.3/src/opstool/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:19:37.682979 opstool-0.7.3/src/opstool/analysis/
--rw-rw-rw-   0        0        0      147 2023-03-10 09:13:36.000000 opstool-0.7.3/src/opstool/analysis/__init__.py
--rw-rw-rw-   0        0        0    13381 2023-03-27 05:54:09.000000 opstool-0.7.3/src/opstool/analysis/_sec_analysis.py
--rw-rw-rw-   0        0        0    32716 2023-04-14 09:17:06.000000 opstool-0.7.3/src/opstool/analysis/_smart_analyze.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:19:37.690699 opstool-0.7.3/src/opstool/examples/
--rw-rw-rw-   0        0        0   365987 2022-12-25 13:36:57.000000 opstool-0.7.3/src/opstool/examples/ArchBridge.py
--rw-rw-rw-   0        0        0    96069 2023-01-06 03:19:00.000000 opstool-0.7.3/src/opstool/examples/ArchBridge2.py
--rw-rw-rw-   0        0        0   697240 2022-12-25 13:38:38.000000 opstool-0.7.3/src/opstool/examples/CableStayedBridge.py
--rw-rw-rw-   0        0        0   289022 2022-12-25 13:39:18.000000 opstool-0.7.3/src/opstool/examples/Dam.py
--rw-rw-rw-   0        0        0     1699 2022-12-25 13:39:55.000000 opstool-0.7.3/src/opstool/examples/DamBreak.py
--rw-rw-rw-   0        0        0   241484 2022-12-25 13:40:30.000000 opstool-0.7.3/src/opstool/examples/Frame3D.py
--rw-rw-rw-   0        0        0   901646 2022-12-25 13:41:16.000000 opstool-0.7.3/src/opstool/examples/Igloo.py
--rw-rw-rw-   0        0        0     2102 2022-12-25 13:41:50.000000 opstool-0.7.3/src/opstool/examples/Pier.py
--rw-rw-rw-   0        0        0     1813 2022-12-25 13:42:23.000000 opstool-0.7.3/src/opstool/examples/SDOF.py
--rw-rw-rw-   0        0        0   110248 2022-12-25 13:43:18.000000 opstool-0.7.3/src/opstool/examples/SuspensionBridge.py
--rw-rw-rw-   0        0        0        2 2022-12-02 13:20:45.000000 opstool-0.7.3/src/opstool/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:19:37.692695 opstool-0.7.3/src/opstool/preprocessing/
--rw-rw-rw-   0        0        0      838 2023-04-02 12:08:20.000000 opstool-0.7.3/src/opstool/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2895 2023-03-30 08:55:58.000000 opstool-0.7.3/src/opstool/preprocessing/geom_transf.py
--rw-rw-rw-   0        0        0     2493 2023-01-05 16:40:03.000000 opstool-0.7.3/src/opstool/preprocessing/load.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:19:37.695708 opstool-0.7.3/src/opstool/preprocessing/section/
--rw-rw-rw-   0        0        0      554 2023-04-02 12:05:56.000000 opstool-0.7.3/src/opstool/preprocessing/section/__init__.py
--rw-rw-rw-   0        0        0     1396 2023-04-14 09:09:55.000000 opstool-0.7.3/src/opstool/preprocessing/section/lib_sec_mesh.py
--rw-rw-rw-   0        0        0    56420 2023-04-14 09:13:37.000000 opstool-0.7.3/src/opstool/preprocessing/section/sec_mesh.py
--rw-rw-rw-   0        0        0    26219 2023-04-14 09:14:18.000000 opstool-0.7.3/src/opstool/preprocessing/section/var_sec_mesh.py
--rw-rw-rw-   0        0        0    53330 2023-03-30 08:56:24.000000 opstool-0.7.3/src/opstool/preprocessing/tcl2py.py
--rw-rw-rw-   0        0        0     5490 2023-03-30 08:58:00.000000 opstool-0.7.3/src/opstool/preprocessing/unit_system.py
--rw-rw-rw-   0        0        0     5547 2023-04-14 09:08:22.000000 opstool-0.7.3/src/opstool/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:19:37.701786 opstool-0.7.3/src/opstool/vis/
--rw-rw-rw-   0        0        0      483 2023-04-14 08:10:34.000000 opstool-0.7.3/src/opstool/vis/__init__.py
--rw-rw-rw-   0        0        0    28011 2023-04-14 08:54:12.000000 opstool-0.7.3/src/opstool/vis/_get_model_base.py
--rw-rw-rw-   0        0        0    92757 2023-04-14 08:56:23.000000 opstool-0.7.3/src/opstool/vis/_plotly_base.py
--rw-rw-rw-   0        0        0    55080 2023-04-14 08:59:00.000000 opstool-0.7.3/src/opstool/vis/_pyvista_base.py
--rw-rw-rw-   0        0        0    22788 2023-04-14 09:02:37.000000 opstool-0.7.3/src/opstool/vis/fiber_sec_vis.py
--rw-rw-rw-   0        0        0    32483 2023-04-14 09:04:43.000000 opstool-0.7.3/src/opstool/vis/get_model_data.py
--rw-rw-rw-   0        0        0    19952 2023-04-14 09:05:35.000000 opstool-0.7.3/src/opstool/vis/ops_vis_plotly.py
--rw-rw-rw-   0        0        0    20744 2023-04-14 09:06:18.000000 opstool-0.7.3/src/opstool/vis/ops_vis_pyvista.py
--rw-rw-rw-   0        0        0     7508 2023-04-14 09:06:33.000000 opstool-0.7.3/src/opstool/vis/quick_plot.py
--rw-rw-rw-   0        0        0     9535 2023-04-14 09:07:20.000000 opstool-0.7.3/src/opstool/vis/save_tikz.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:19:37.681032 opstool-0.7.3/src/opstool.egg-info/
--rw-rw-rw-   0        0        0     6415 2023-04-14 09:19:37.000000 opstool-0.7.3/src/opstool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1457 2023-04-14 09:19:37.000000 opstool-0.7.3/src/opstool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 09:19:37.000000 opstool-0.7.3/src/opstool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-04-14 09:19:37.000000 opstool-0.7.3/src/opstool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 09:19:37.000000 opstool-0.7.3/src/opstool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.738934 opstool-0.8.0/
+-rw-rw-rw-   0        0        0    34817 2022-12-02 05:00:10.000000 opstool-0.8.0/LICENCE.txt
+-rw-rw-rw-   0        0        0     6424 2023-05-07 06:04:22.738934 opstool-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6005 2023-03-31 11:53:22.000000 opstool-0.8.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-07 06:04:22.738934 opstool-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2023-05-07 06:04:08.000000 opstool-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.691089 opstool-0.8.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.691089 opstool-0.8.0/src/opstool/
+-rw-rw-rw-   0        0        0       23 2023-05-07 05:55:41.000000 opstool-0.8.0/src/opstool/__about__.py
+-rw-rw-rw-   0        0        0      560 2023-04-29 15:03:24.000000 opstool-0.8.0/src/opstool/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.707487 opstool-0.8.0/src/opstool/analysis/
+-rw-rw-rw-   0        0        0      147 2023-03-10 09:13:36.000000 opstool-0.8.0/src/opstool/analysis/__init__.py
+-rw-rw-rw-   0        0        0    13408 2023-05-02 13:56:05.000000 opstool-0.8.0/src/opstool/analysis/_sec_analysis.py
+-rw-rw-rw-   0        0        0    35206 2023-05-02 13:57:14.000000 opstool-0.8.0/src/opstool/analysis/_smart_analyze.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.707487 opstool-0.8.0/src/opstool/examples/
+-rw-rw-rw-   0        0        0   365987 2022-12-25 13:36:57.000000 opstool-0.8.0/src/opstool/examples/ArchBridge.py
+-rw-rw-rw-   0        0        0    96069 2023-01-06 03:19:00.000000 opstool-0.8.0/src/opstool/examples/ArchBridge2.py
+-rw-rw-rw-   0        0        0   697240 2022-12-25 13:38:38.000000 opstool-0.8.0/src/opstool/examples/CableStayedBridge.py
+-rw-rw-rw-   0        0        0   289022 2022-12-25 13:39:18.000000 opstool-0.8.0/src/opstool/examples/Dam.py
+-rw-rw-rw-   0        0        0     1699 2022-12-25 13:39:55.000000 opstool-0.8.0/src/opstool/examples/DamBreak.py
+-rw-rw-rw-   0        0        0   241484 2022-12-25 13:40:30.000000 opstool-0.8.0/src/opstool/examples/Frame3D.py
+-rw-rw-rw-   0        0        0    15435 2023-05-06 11:58:20.000000 opstool-0.8.0/src/opstool/examples/Frame3D2.py
+-rw-rw-rw-   0        0        0    54201 2023-05-06 11:47:25.000000 opstool-0.8.0/src/opstool/examples/GridFrame.py
+-rw-rw-rw-   0        0        0   901646 2022-12-25 13:41:16.000000 opstool-0.8.0/src/opstool/examples/Igloo.py
+-rw-rw-rw-   0        0        0     2102 2022-12-25 13:41:50.000000 opstool-0.8.0/src/opstool/examples/Pier.py
+-rw-rw-rw-   0        0        0     1813 2022-12-25 13:42:23.000000 opstool-0.8.0/src/opstool/examples/SDOF.py
+-rw-rw-rw-   0        0        0   110248 2022-12-25 13:43:18.000000 opstool-0.8.0/src/opstool/examples/SuspensionBridge.py
+-rw-rw-rw-   0        0        0        2 2022-12-02 13:20:45.000000 opstool-0.8.0/src/opstool/examples/__init__.py
+-rw-rw-rw-   0        0        0    16275 2023-05-06 19:15:36.000000 opstool-0.8.0/src/opstool/examples/shell3D.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.723716 opstool-0.8.0/src/opstool/preprocessing/
+-rw-rw-rw-   0        0        0      838 2023-04-02 12:08:20.000000 opstool-0.8.0/src/opstool/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2876 2023-05-02 14:24:57.000000 opstool-0.8.0/src/opstool/preprocessing/geom_transf.py
+-rw-rw-rw-   0        0        0     2266 2023-05-02 14:30:35.000000 opstool-0.8.0/src/opstool/preprocessing/load.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.728233 opstool-0.8.0/src/opstool/preprocessing/section/
+-rw-rw-rw-   0        0        0      554 2023-04-02 12:05:56.000000 opstool-0.8.0/src/opstool/preprocessing/section/__init__.py
+-rw-rw-rw-   0        0        0     1417 2023-05-02 13:57:22.000000 opstool-0.8.0/src/opstool/preprocessing/section/lib_sec_mesh.py
+-rw-rw-rw-   0        0        0    58277 2023-05-02 13:56:50.000000 opstool-0.8.0/src/opstool/preprocessing/section/sec_mesh.py
+-rw-rw-rw-   0        0        0    26107 2023-05-02 13:57:35.000000 opstool-0.8.0/src/opstool/preprocessing/section/var_sec_mesh.py
+-rw-rw-rw-   0        0        0    53330 2023-03-30 08:56:24.000000 opstool-0.8.0/src/opstool/preprocessing/tcl2py.py
+-rw-rw-rw-   0        0        0     5490 2023-03-30 08:58:00.000000 opstool-0.8.0/src/opstool/preprocessing/unit_system.py
+-rw-rw-rw-   0        0        0     6848 2023-05-06 15:12:02.000000 opstool-0.8.0/src/opstool/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.728233 opstool-0.8.0/src/opstool/vis/
+-rw-rw-rw-   0        0        0      494 2023-05-04 17:23:00.000000 opstool-0.8.0/src/opstool/vis/__init__.py
+-rw-rw-rw-   0        0        0    31743 2023-05-06 13:21:15.000000 opstool-0.8.0/src/opstool/vis/_get_model_base.py
+-rw-rw-rw-   0        0        0   101317 2023-05-06 12:18:34.000000 opstool-0.8.0/src/opstool/vis/_plotly_base.py
+-rw-rw-rw-   0        0        0    59718 2023-05-06 12:19:04.000000 opstool-0.8.0/src/opstool/vis/_pyvista_base.py
+-rw-rw-rw-   0        0        0    23046 2023-05-04 17:23:18.000000 opstool-0.8.0/src/opstool/vis/fiber_sec_vis.py
+-rw-rw-rw-   0        0        0    32818 2023-05-06 16:41:25.000000 opstool-0.8.0/src/opstool/vis/get_model_data.py
+-rw-rw-rw-   0        0        0    28069 2023-05-06 14:31:33.000000 opstool-0.8.0/src/opstool/vis/ops_vis_2d.py
+-rw-rw-rw-   0        0        0    24646 2023-05-06 08:18:30.000000 opstool-0.8.0/src/opstool/vis/ops_vis_plotly.py
+-rw-rw-rw-   0        0        0    21638 2023-05-03 06:58:59.000000 opstool-0.8.0/src/opstool/vis/ops_vis_pyvista.py
+-rw-rw-rw-   0        0        0    10257 2023-05-06 12:44:36.000000 opstool-0.8.0/src/opstool/vis/quick_plot.py
+-rw-rw-rw-   0        0        0     9601 2023-04-29 15:01:29.000000 opstool-0.8.0/src/opstool/vis/save_tikz.py
+drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.707487 opstool-0.8.0/src/opstool.egg-info/
+-rw-rw-rw-   0        0        0     6424 2023-05-07 06:04:22.000000 opstool-0.8.0/src/opstool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1730 2023-05-07 06:04:22.000000 opstool-0.8.0/src/opstool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 06:04:22.000000 opstool-0.8.0/src/opstool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-05-07 06:04:22.000000 opstool-0.8.0/src/opstool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-07 06:04:22.000000 opstool-0.8.0/src/opstool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 06:04:22.738934 opstool-0.8.0/tests/
+-rw-rw-rw-   0        0        0     2002 2023-01-18 14:49:51.000000 opstool-0.8.0/tests/test_dambreak.py
+-rw-rw-rw-   0        0        0     1705 2023-03-27 03:00:39.000000 opstool-0.8.0/tests/test_fiber_sec_vis.py
+-rw-rw-rw-   0        0        0     2997 2023-05-06 07:58:02.000000 opstool-0.8.0/tests/test_model_vis.py
+-rw-rw-rw-   0        0        0     2261 2023-03-29 06:45:30.000000 opstool-0.8.0/tests/test_sec_analysis.py
+-rw-rw-rw-   0        0        0    10302 2023-04-03 08:29:31.000000 opstool-0.8.0/tests/test_sec_mesh.py
+-rw-rw-rw-   0        0        0     1237 2023-05-06 09:45:10.000000 opstool-0.8.0/tests/test_temp.py
```

### Comparing `opstool-0.7.3/LICENCE.txt` & `opstool-0.8.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `opstool-0.7.3/PKG-INFO` & `opstool-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: opstool
-Version: 0.7.3
+Version: 0.8.0
 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992
 Author: Yexiang Yan
 Author-email: yexiang_yan@outlook.com
 License: GPL Licence
-Keywords: OpenSees seismic visualization
+Keywords: OpenSees Visualization Seismic Simulation
 Platform: any
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8.*
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 <p align="center">
   <font size=7><a href="https://github.com/yexiang1992/opstool">opstool</a></font>
   <p align="center"><font size=5 color=YellowGreen>modelling, visualization, post-processing for OpenSeesPy.</font></p>
 </p>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: opstool Version: 0.7.3 Summary: openseespy toolbox
+Metadata-Version: 2.1 Name: opstool Version: 0.8.0 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992 Author: Yexiang Yan Author-email:
-yexiang_yan@outlook.com License: GPL Licence Keywords: OpenSees seismic
-visualization Platform: any Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8.* Description-Content-Type: text/markdown License-File:
+yexiang_yan@outlook.com License: GPL Licence Keywords: OpenSees Visualization
+Seismic Simulation Platform: any Classifier: Programming Language :: Python ::
+3 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENCE.txt
                                     opstool
            modelling, visualization, post-processing for OpenSeesPy.
 [![pypi](https://img.shields.io/pypi/v/opstool)](https://pypi.org/project/
 opstool/) [![Downloads](https://static.pepy.tech/badge/opstool)](https://
 pepy.tech/project/opstool) [![Documentation Status](https://readthedocs.org/
 projects/opstool/badge/?version=latest)](https://opstool.readthedocs.io/en/
```

### Comparing `opstool-0.7.3/README.md` & `opstool-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `opstool-0.7.3/setup.py` & `opstool-0.8.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 
 from src.opstool import __version__
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
-    name='opstool',
+    name="opstool",
     version=__version__,
-    description='openseespy toolbox',
+    description="openseespy toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    author='Yexiang Yan',
-    author_email='yexiang_yan@outlook.com',
-    url='https://github.com/yexiang1992',
-    license='GPL Licence',
-    keywords='OpenSees seismic visualization',
-    platforms='any',
-    python_requires='>=3.8.*',
-    package_dir={'': 'src'},
-    packages=find_packages('src'),
+    author="Yexiang Yan",
+    author_email="yexiang_yan@outlook.com",
+    url="https://github.com/yexiang1992",
+    license="GPL Licence",
+    keywords="OpenSees Visualization Seismic Simulation",
+    platforms="any",
+    python_requires=">=3.8",
+    package_dir={"": "src"},
+    packages=find_packages("src"),
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
     install_requires=[
-        'matplotlib',
-        'numpy',
-        'openseespy>=3.4.0.1',
-        'plotly',
-        'pyvista>=0.38.2',
-        'sectionproperties>=2.1.5',
-        'shapely>=2.0.0',
-        'h5py',
-        'rich',
-        "triangle"
+        "matplotlib",
+        "numpy",
+        "openseespy>=3.4.0.1",
+        "plotly",
+        "pyvista>=0.38.2",
+        "sectionproperties>=2.1.5",
+        "shapely>=2.0.0",
+        "h5py",
+        "rich",
+        "triangle",
     ],
 )
```

### Comparing `opstool-0.7.3/src/opstool/__init__.py` & `opstool-0.8.0/src/opstool/__init__.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.3/src/opstool/analysis/_sec_analysis.py` & `opstool-0.8.0/src/opstool/analysis/_sec_analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,38 @@
-import numpy as np
 import matplotlib.pyplot as plt
+import numpy as np
 import openseespy.opensees as ops
+
 from ._smart_analyze import SmartAnalyze
 
 
 class MomentCurvature:
     """Moment-Curvature Analysis for Fiber Section in OpenSeesPy.
 
     Parameters
     ----------
     sec_tag : int,
         The previously defined section Tag.
     axial_force : float, optional
         Axial load, compression is negative, by default 0
     """
 
-    def __init__(self,
-                 sec_tag: int,
-                 axial_force: float = 0) -> None:
+    def __init__(self, sec_tag: int, axial_force: float = 0) -> None:
         self.P = axial_force
         self.sec_tag = sec_tag
         self.phi, self.M, self.FiberData = None, None, None
 
-    def analyze(self,
-                axis: str = "y",
-                max_phi: float = 1.0,
-                incr_phi: float = 1e-4,
-                post_peak_ratio: float = 0.7,
-                smart_analyze: bool = True):
+    def analyze(
+        self,
+        axis: str = "y",
+        max_phi: float = 1.0,
+        incr_phi: float = 1e-4,
+        post_peak_ratio: float = 0.8,
+        smart_analyze: bool = True,
+    ):
         """Performing Moment-Curvature Analysis.
 
         Parameters
         ----------
         axis : str, optional, "y" or "z"
             The axis of the section to be analyzed, by default "y".
         max_phi : float, optional
@@ -43,53 +44,59 @@
             i.e. a 30% drop after peak.
         smart_analyze : bool, optional
             Whether to use smart analysis options, by default True.
 
         .. note::
             The termination of the analysis depends on whichever reaches `max_phi` or `post_peak_ratio` first.
         """
-        self.phi, self.M, self.FiberData = _analyze(sec_tag=self.sec_tag,
-                                                    P=self.P,
-                                                    axis=axis,
-                                                    max_phi=max_phi,
-                                                    incr_phi=incr_phi,
-                                                    stop_ratio=post_peak_ratio,
-                                                    smart_analyze=smart_analyze)
+        self.phi, self.M, self.FiberData = _analyze(
+            sec_tag=self.sec_tag,
+            P=self.P,
+            axis=axis,
+            max_phi=max_phi,
+            incr_phi=incr_phi,
+            stop_ratio=post_peak_ratio,
+            smart_analyze=smart_analyze,
+        )
 
     def plot_M_phi(self):
-        """Plot the moment-curvature relationship.
-        """
+        """Plot the moment-curvature relationship."""
         _, ax = plt.subplots(1, 1, figsize=(10, 10 * 0.618))
         ax.plot(self.phi, self.M, lw=3, c="blue")
-        ax.set_title("$M-\phi$", fontsize=28,)
+        ax.set_title(
+            "$M-\phi$",
+            fontsize=28,
+        )
         ax.set_xlabel("$\phi$", fontsize=25)
         ax.set_ylabel("$M$", fontsize=25)
         plt.xticks(fontsize=15)
         plt.yticks(fontsize=15)
         ax.spines["bottom"].set_linewidth(1.2)
         ax.spines["left"].set_linewidth(1.2)
         ax.spines["right"].set_linewidth(1.2)
         ax.spines["top"].set_linewidth(1.2)
         plt.gcf().subplots_adjust(bottom=0.15)
         plt.show()
 
     def plot_fiber_responses(self):
-        """Plot the stress-strain histories for all fibers of each material.
-        """
+        """Plot the stress-strain histories for all fibers of each material."""
         fiber_data = self.FiberData
         matTags = np.unique(fiber_data[-1][:, 3])
 
-        _, axs = plt.subplots(
-            len(matTags), 1, figsize=(8, 3*len(matTags)))
+        _, axs = plt.subplots(len(matTags), 1, figsize=(8, 3 * len(matTags)))
         for mat, ax in zip(matTags, axs):
             idxs = np.argwhere(np.abs(fiber_data[-1][:, 3] - mat) < 1e-6)
             strain = fiber_data[:, idxs, -1]
             stress = fiber_data[:, idxs, -2]
             for i in range(len(idxs)):
-                ax.plot(strain[:, i, :], stress[:, i, :], lw=1, )
+                ax.plot(
+                    strain[:, i, :],
+                    stress[:, i, :],
+                    lw=1,
+                )
             ax.set_title(f"matTag = {mat:.0f}", fontsize=15)
             ax.tick_params(labelsize=12)
             ax.set_ylabel("stress", fontsize=16)
         ax.set_xlabel("strain", fontsize=16)
         plt.subplots_adjust(wspace=0.02, hspace=0.4)
         plt.tight_layout()
         plt.show()
@@ -151,18 +158,17 @@
         -------
         Shape-(n,m,6) Array.
             n is the length of moment and curvature array, m is the fiber number,
             6 contain ("yCoord", "zCoord", "area", 'mat', "stress", "strain")
         """
         return self.FiberData
 
-    def get_limit_state(self,
-                        matTag: int = 1,
-                        threshold: float = 0,
-                        use_peak_drop20: bool = False):
+    def get_limit_state(
+        self, matTag: int = 1, threshold: float = 0, use_peak_drop20: bool = False
+    ):
         """Get the curvature and moment corresponding to a certain limit state.
 
         Parameters
         ----------
         matTag : int, optional
             The OpenSeesPy material Tag used to determine the limit state., by default 1
         threshold : float, optional
@@ -180,41 +186,38 @@
         M = self.M
         fiber_data = self.FiberData
         if use_peak_drop20:
             idx = np.argmax(M)
             au = np.argwhere(M[idx:] <= np.max(M) * 0.80)
             if au.size == 0:
                 raise RuntimeError(
-                    "Peak strength does not drop 20%, please increase target ductility ratio!")
+                    "Peak strength does not drop 20%, please increase target ductility ratio!"
+                )
             else:
                 bu = np.min(au) + idx - 1
         else:
             idxu = np.argwhere(np.abs(fiber_data[-1][:, 3] - matTag) < 1e-6)
             eu = threshold
             if eu >= 0:
-                strain = np.array([np.max(data[idxu, -1])
-                                  for data in fiber_data])
+                strain = np.array([np.max(data[idxu, -1]) for data in fiber_data])
                 au = np.argwhere(strain >= eu)
             else:
-                strain = np.array([np.min(data[idxu, -1])
-                                  for data in fiber_data])
+                strain = np.array([np.min(data[idxu, -1]) for data in fiber_data])
                 au = np.argwhere(strain < eu)
             if len(au) == 0:
                 raise RuntimeError(
-                    "The ultimate strain is not reached, please increase target ductility ratio!")
+                    "The ultimate strain is not reached, please increase target ductility ratio!"
+                )
             else:
                 bu = np.min(au)
         Phi_u = phi[bu]
         M_u = M[bu]
         return Phi_u, M_u
 
-    def bilinearize(self, phiy: float,
-                    My: float,
-                    phiu: float,
-                    plot: bool = False):
+    def bilinearize(self, phiy: float, My: float, phiu: float, plot: bool = False):
         """Bilinear Approximation of Moment-Curvature Relation.
 
         Parameters
         ----------
         phiy : float
             The initial yield curvature.
         My : float
@@ -234,89 +237,108 @@
         M = self.M
         bu = np.argmin(np.abs(phiu - phi))
         Q = np.trapz(M[: bu + 1], phi[: bu + 1])
         k = My / phiy
         Phi_eq = (k * phiu - np.sqrt((k * phiu) ** 2 - 2 * k * Q)) / k
         M_eq = k * Phi_eq
 
-        M_new = np.insert(M[0: bu + 1], 0, 0, axis=None)
-        Phi_new = np.insert(phi[0: bu + 1], 0, 0, axis=None)
+        M_new = np.insert(M[0 : bu + 1], 0, 0, axis=None)
+        Phi_new = np.insert(phi[0 : bu + 1], 0, 0, axis=None)
 
         if plot:
             _, ax = plt.subplots(1, 1, figsize=(10, 10 * 0.618))
             ax.plot(Phi_new, M_new, lw=1.5, c="#2529d8")
-            ax.plot([0, phiy, Phi_eq, phiu],
-                    [0, My, M_eq, M_eq],
-                    lw=1.5, c='#de0f17')
-            ax.plot(phiy, My, "o", ms=12, mec="black",
-                    mfc='#0099e5', label="Initial Yield ($\phi_y$,$M_y$)")
-            ax.plot(Phi_eq, M_eq, "*", ms=15, mec="black",
-                    mfc='#ff4c4c', label="Equivalent Yield ($\phi_{{eq}}$,$M_{{eq}}$)")
+            ax.plot([0, phiy, Phi_eq, phiu], [0, My, M_eq, M_eq], lw=1.5, c="#de0f17")
+            ax.plot(
+                phiy,
+                My,
+                "o",
+                ms=12,
+                mec="black",
+                mfc="#0099e5",
+                label="Initial Yield ($\phi_y$,$M_y$)",
+            )
+            ax.plot(
+                Phi_eq,
+                M_eq,
+                "*",
+                ms=15,
+                mec="black",
+                mfc="#ff4c4c",
+                label="Equivalent Yield ($\phi_{{eq}}$,$M_{{eq}}$)",
+            )
             maxy = np.max(ax.get_yticks())
-            ax.vlines(phiu, 0, maxy, colors="#34bf49",
-                      linestyles="dashed", lw=0.75)
-            txt = (f"$\phi_y$={phiy:.3E}, $M_y$={My:.3E}\n"
-                   f"$\phi_{{eq}}$={Phi_eq:.3E}, $M_{{eq}}$={M_eq:.3E}\n"
-                   f"$\phi_{{u}}$={phiu:.3E}, $M_{{u}}$={M[bu]:.3E}")
-            ax.text(0.5, 0.4, txt, fontsize=15, ha='center',
-                    va='bottom', transform=ax.transAxes)
-            ax.set_title("Moment-Curvature", fontsize=22,)
+            ax.vlines(phiu, 0, maxy, colors="#34bf49", linestyles="dashed", lw=0.75)
+            txt = (
+                f"$\phi_y$={phiy:.3E}, $M_y$={My:.3E}\n"
+                f"$\phi_{{eq}}$={Phi_eq:.3E}, $M_{{eq}}$={M_eq:.3E}\n"
+                f"$\phi_{{u}}$={phiu:.3E}, $M_{{u}}$={M[bu]:.3E}"
+            )
+            ax.text(
+                0.5,
+                0.4,
+                txt,
+                fontsize=15,
+                ha="center",
+                va="bottom",
+                transform=ax.transAxes,
+            )
+            ax.set_title(
+                "Moment-Curvature",
+                fontsize=22,
+            )
             ax.set_xlabel("$\phi$", fontsize=20)
             ax.set_ylabel("$M$", fontsize=20)
             plt.xticks(fontsize=15)
             plt.yticks(fontsize=15)
             # ax.set_xlim(0, np.max(ax.get_xticks()))
             ax.set_ylim(0, maxy)
             ax.spines["bottom"].set_linewidth(1.2)
             ax.spines["left"].set_linewidth(1.2)
             ax.spines["right"].set_linewidth(1.2)
             ax.spines["top"].set_linewidth(1.2)
-            ax.legend(loc='lower center', fontsize=15)
+            ax.legend(loc="lower center", fontsize=15)
             plt.gcf().subplots_adjust(bottom=0.15)
             plt.show()
         return Phi_eq, M_eq
 
 
 def _create_model(sec_tag):
-    ops.model('basic', '-ndm', 3, '-ndf', 6)
+    ops.model("basic", "-ndm", 3, "-ndf", 6)
     ops.node(1, 0.0, 0.0, 0.0)
     ops.node(2, 0.0, 0.0, 0.0)
     ops.fix(1, 1, 1, 1, 1, 1, 1)
     ops.fix(2, 0, 1, 1, 1, 0, 0)
-    ops.element('zeroLengthSection', 1, 1, 2, sec_tag)
+    ops.element("zeroLengthSection", 1, 1, 2, sec_tag)
 
 
 def _create_axial_resp(p):
-    ops.timeSeries('Constant', 1)
-    ops.pattern('Plain', 1, 1)
-    ops.load(2, p, 0, 0, 0, 0, 0)    # nd  FX,  FY, Fz, MX, MY, MZ
+    ops.timeSeries("Constant", 1)
+    ops.pattern("Plain", 1, 1)
+    ops.load(2, p, 0, 0, 0, 0, 0)  # nd  FX,  FY, Fz, MX, MY, MZ
     ops.wipeAnalysis()
-    ops.system('SparseGeneral', '-piv')
-    ops.constraints('Plain')
-    ops.numberer('Plain')
-    ops.test('NormDispIncr', 1.0e-12, 10, 3)
-    ops.algorithm('Newton')
-    ops.integrator('LoadControl', 1 / 10)
-    ops.analysis('Static')
+    ops.system("SparseGeneral", "-piv")
+    ops.constraints("Plain")
+    ops.numberer("Plain")
+    ops.test("NormDispIncr", 1.0e-12, 10, 3)
+    ops.algorithm("Newton")
+    ops.integrator("LoadControl", 1 / 10)
+    ops.analysis("Static")
     ops.analyze(10)
-    ops.loadConst('-time', 0.0)
+    ops.loadConst("-time", 0.0)
 
 
-def _analyze(sec_tag,
-             P=0,
-             axis="y",
-             max_phi=1,
-             incr_phi=1e-4,
-             stop_ratio=0.7,
-             smart_analyze=True):
+def _analyze(
+    sec_tag, P=0, axis="y", max_phi=1, incr_phi=1e-5, stop_ratio=0.7, smart_analyze=True
+):
     _create_model(sec_tag=sec_tag)
     if P != 0:
         _create_axial_resp(P)
-    ops.timeSeries('Linear', 2)
-    ops.pattern('Plain', 2, 2)
+    ops.timeSeries("Linear", 2)
+    ops.pattern("Plain", 2, 2)
     if axis.lower() == "y":
         dof = 5
         ops.load(2, 0, 0, 0, 0, 1, 0)
     elif axis.lower() == "z":
         dof = 6
         ops.load(2, 0, 0, 0, 0, 0, 1)
     else:
@@ -325,18 +347,20 @@
     PHI = [0]
     FIBER_RESPONSES = [0]
     if smart_analyze:
         protocol = [max_phi]
         userControl = {
             "analysis": "Static",
             "testType": "NormDispIncr",
-            "testTol": 1.0e-10,
+            "testTol": 1.0e-8,
+            "tryAlterAlgoTypes": True,
+            "algoTypes": [10, 40, 30, 20],
             "relaxation": 0.5,
-            "minStep": 1.0e-8,
-            "printPer": 10,
+            "minStep": 1.0e-12,
+            "printPer": 10000000000,
             "debugMode": False,
         }
         analysis = SmartAnalyze(analysis_type="Static", **userControl)
         segs = analysis.static_split(protocol, maxStep=incr_phi)
         ii = 0
         while True:
             seg = segs[ii]
@@ -349,15 +373,15 @@
             if cond1 or cond2:
                 break
             PHI.append(ops.nodeDisp(2, dof))
             M.append(curr_M)
             FIBER_RESPONSES.append(_get_fiber_sec_data(ele_tag=1))
 
     else:
-        ops.integrator('DisplacementControl', 2, dof, incr_phi)
+        ops.integrator("DisplacementControl", 2, dof, incr_phi)
         while True:
             ops.analyze(1)
             curr_M = ops.getLoadFactor(2)
             curr_Phi = ops.nodeDisp(2, dof)
             cond1 = np.abs(curr_M) < np.max(np.abs(M)) * (stop_ratio - 0.02)
             cond2 = np.abs(curr_Phi) > max_phi
             if cond1 or cond2:
```

### Comparing `opstool-0.7.3/src/opstool/analysis/_smart_analyze.py` & `opstool-0.8.0/src/opstool/analysis/_smart_analyze.py`

 * *Files 16% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     algoTypes: list[int], default=[40, 10, 20, 30, 50, 60, 70, 90]
         A list of flags of the algorithms to be used during unconvergance.
         The integer flag is documented in the following section.
         Only useful when tryAlterAlgoTypes is True.
         The first flag will be used by default when tryAlterAlgoTypes is False.
         The algorithm command in the model will be ignored.
         If you need other algorithm, try a user-defined algorithm. See the following section.
-    UserAlgoArgs: list, 
+    UserAlgoArgs: list,
         User-defined algorithm parameters, 100 is required in algoTypes,
         and the parameters must be included in the list, for example:
         algoTypes = [10, 20, 100],
         UserAlgoArgs = ["KrylovNewton", "-iterate", "initial", "-maxDim", 20]
 
     .. tip::
         Algorithm type flag reference
@@ -184,54 +184,78 @@
     >>>                             )
     """
 
     def __init__(self, analysis_type="Transient", **kargs):
         if analysis_type not in ("Transient", "Static"):
             raise ValueError("analysis_type must Transient or Static!")
         # default
-        self.control = {'analysis': analysis_type, 'testType': "EnergyIncr", 'testTol': 1.0e-10,
-                        'testIterTimes': 10, 'testPrintFlag': 0, 'tryAddTestTimes': False,
-                        'normTol': 1.0e3, 'testIterTimesMore': 50, 'tryLooseTestTol': False,
-                        'looseTestTolTo': 1.0, 'tryAlterAlgoTypes': False,
-                        'algoTypes': [40, 10, 20, 30, 50, 60, 70, 90], "UserAlgoArgs": None,
-                        'initialStep': None, 'relaxation': 0.5, 'minStep': 1.0e-6,
-                        'printPer': 50, 'debugMode': False}
-        self.control['looseTestTolTo'] = 100 * self.control['testTol']
+        self.control = {
+            "analysis": analysis_type,
+            "testType": "EnergyIncr",
+            "testTol": 1.0e-10,
+            "testIterTimes": 10,
+            "testPrintFlag": 0,
+            "tryAddTestTimes": False,
+            "normTol": 1.0e3,
+            "testIterTimesMore": 50,
+            "tryLooseTestTol": False,
+            "looseTestTolTo": 1.0,
+            "tryAlterAlgoTypes": False,
+            "algoTypes": [40, 10, 20, 30, 50, 60, 70, 90],
+            "UserAlgoArgs": None,
+            "initialStep": None,
+            "relaxation": 0.5,
+            "minStep": 1.0e-6,
+            "printPer": 50,
+            "debugMode": False,
+        }
+        self.control["looseTestTolTo"] = 100 * self.control["testTol"]
         for name in kargs.keys():
             if name not in self.control.keys():
                 raise ValueError(f"arg {name} error!")
         self.control.update(kargs)
-        self.eps = 1.E-12
+        self.eps = 1.0e-12
         self.logo = "[bold magenta]SmartAnalyze:[/bold magenta]"
 
         # initial test commands
-        ops.test(self.control['testType'], self.control['testTol'],
-                 self.control['testIterTimes'], self.control['testPrintFlag'])
-        self._setAlgorithm(self.control['algoTypes'][0], self.control["UserAlgoArgs"])
-
-        self.current = {'startTime': time.time(), 'algoIndex': 0,
-                        'testIterTimes': self.control['testIterTimes'],
-                        'testTol': self.control['testTol'], 'counter': 0,
-                        'progress': 0, 'segs': 0, 'step': 0.0,
-                        'node': 0, 'dof': 0}
+        ops.test(
+            self.control["testType"],
+            self.control["testTol"],
+            self.control["testIterTimes"],
+            self.control["testPrintFlag"],
+        )
+        self._setAlgorithm(self.control["algoTypes"][0], self.control["UserAlgoArgs"])
+
+        self.current = {
+            "startTime": time.time(),
+            "algoIndex": 0,
+            "testIterTimes": self.control["testIterTimes"],
+            "testTol": self.control["testTol"],
+            "counter": 0,
+            "progress": 0,
+            "segs": 0,
+            "step": 0.0,
+            "node": 0,
+            "dof": 0,
+        }
 
     def transient_split(self, npts: int):
         """Step Segmentation for Transient Analysis.
         It is not necessary to use this method.
 
         Parameters
         ----------
         npts : int
             Total steps for transient analysis.
 
         Returns
         -------
         A list to loop.
         """
-        self.current['segs'] = npts
+        self.current["segs"] = npts
         return list(range(1, npts + 1))
 
     def static_split(self, targets: list, maxStep: float = None):
         """Returns a sequence of substeps for static analysis, for use in outer analysis loops.
         It is not necessary to use this method if you already have a load sequence.
 
         Parameters
@@ -249,15 +273,16 @@
 
         """
         targets = np.atleast_1d(targets)
         if targets.ndim != 1:
             raise ValueError("targets must be 1D!")
         if len(targets) == 1 and maxStep is None:
             raise ValueError(
-                "When targets has only one element, maxStep must be passed in!")
+                "When targets has only one element, maxStep must be passed in!"
+            )
         if targets[0] != 0.0:
             targets = np.insert(targets, 0, 0.0)
         if maxStep is None:
             maxStep = targets[1] - targets[0]
         # calcuate whole distance; divide the whole process into segments.
         distance = 0
         segs = []
@@ -280,66 +305,78 @@
                 segs.append(section - j * maxStep)
             else:
                 j = 0
                 while (-section - j * maxStep) > maxStep + self.eps:
                     segs.append(-maxStep)
                     j += 1
                 segs.append(section + j * maxStep)
-        self.current['segs'] = len(segs)
+        self.current["segs"] = len(segs)
         return segs
 
     def _get_time(self):
-        return time.time() - self.current['startTime']
+        return time.time() - self.current["startTime"]
 
     def TransientAnalyze(self, dt: float):
         """Single Step Transient Analysis.
 
         Parameters
         ----------
         dt : float
             Time Step.
 
         Returns
         -------
         Return 0 if successful, otherwise returns a negative number.
         """
-        if self.control['analysis'] != "Transient":
+        if self.control["analysis"] != "Transient":
             raise ValueError("Transient! Please check parameter input!")
-        self.control['initialStep'] = dt
+        self.control["initialStep"] = dt
 
-        ops.analysis(self.control['analysis'])
+        ops.analysis(self.control["analysis"])
 
-        ok = self._RecursiveAnalyze(self.control['initialStep'], 0, self.control['testIterTimes'],
-                                    self.control['testTol'], self.control.copy(), self.current.copy())
+        ok = self._RecursiveAnalyze(
+            self.control["initialStep"],
+            0,
+            self.control["testIterTimes"],
+            self.control["testTol"],
+            self.control.copy(),
+            self.current.copy(),
+        )
         if ok < 0:
             color = _get_random_color()
             custime = f"[{color}]{self._get_time():.3f}[/{color}]"
-            print(
-                f">>> {self.logo} Analyze failed. Time consumption: {custime} s.")
+            print(f">>> {self.logo} Analyze failed. Time consumption: {custime} s.")
             return ok
 
-        self.current['progress'] += 1
-        self.current['counter'] += 1
-        if self.current['segs'] > 0:
+        self.current["progress"] += 1
+        self.current["counter"] += 1
+        if self.current["segs"] > 0:
             color = _get_random_color()
-            if self.control['debugMode']:
+            if self.control["debugMode"]:
                 value1 = f"[bold {color}]{100 * self.current['progress'] / self.current['segs']:.3f}[/bold {color}]"
                 value2 = f"[bold {color}]{self._get_time():.3f}[/bold {color}]"
-                print(f"* {self.logo} progress {value1} %. Time consumption: {value2} s.")
-            elif self.current['counter'] >= self.control['printPer']:
+                print(
+                    f"* {self.logo} progress {value1} %. Time consumption: {value2} s."
+                )
+            elif self.current["counter"] >= self.control["printPer"]:
                 value1 = f"[bold {color}]{100 * self.current['progress'] / self.current['segs']:.3f}[/bold {color}]"
                 value2 = f"[bold {color}]{self._get_time():.3f}[/bold {color}]"
-                print(f"* {self.logo} progress {value1} %. Time consumption: {value2} s.")
-                self.current['counter'] = 0
-        if (self.current['segs'] > 0) and (self.current['progress'] >= self.current['segs']):
+                print(
+                    f"* {self.logo} progress {value1} %. Time consumption: {value2} s."
+                )
+                self.current["counter"] = 0
+        if (self.current["segs"] > 0) and (
+            self.current["progress"] >= self.current["segs"]
+        ):
             color = _get_random_color()
             custime = f"[{color}]{self._get_time():.3f}[/{color}]"
             print(
-                f">>> {self.logo} [{color}]Successfully finished[/{color}]! Time consumption: {custime} s.")
-            return 0
+                f">>> {self.logo} [{color}]Successfully finished[/{color}]! Time consumption: {custime} s."
+            )
+        return 0
 
     def StaticAnalyze(self, node: int, dof: int, seg: float):
         """Single step static analysis and applies to displacement control only.
 
         Parameters
         ----------
         node : int
@@ -349,56 +386,74 @@
         seg : float
             Each load step, i.e. each element returned by static_split.
 
         Returns
         -------
         Return 0 if successful, otherwise returns a negative number.
         """
-        if self.control['analysis'] != "Static":
+        if self.control["analysis"] != "Static":
             raise ValueError("Static! Please check parameter input!")
-        self.control['initialStep'] = seg
-        self.current['node'] = node
-        self.current['dof'] = dof
-        self.current['step'] = seg
+        self.control["initialStep"] = seg
+        self.current["node"] = node
+        self.current["dof"] = dof
+        self.current["step"] = seg
 
-        ops.integrator('DisplacementControl', node, dof, seg)
-        ops.analysis(self.control['analysis'])
+        ops.integrator("DisplacementControl", node, dof, seg)
+        ops.analysis(self.control["analysis"])
 
-        ok = self._RecursiveAnalyze(seg, 0, self.control['testIterTimes'], self.control['testTol'],
-                                    self.control.copy(), self.current.copy())
+        ok = self._RecursiveAnalyze(
+            seg,
+            0,
+            self.control["testIterTimes"],
+            self.control["testTol"],
+            self.control.copy(),
+            self.current.copy(),
+        )
         if ok < 0:
             color = _get_random_color()
             value = f"[bold {color}]{self._get_time():.3f}[/bold {color}]"
-            print(
-                f">>> {self.logo} Analyze failed. Time consumption: {value} s.")
+            print(f">>> {self.logo} Analyze failed. Time consumption: {value} s.")
             return -1
-        self.current['progress'] += 1
-        self.current['counter'] += 1
-        if self.current['segs'] > 0:
+        self.current["progress"] += 1
+        self.current["counter"] += 1
+        if self.current["segs"] > 0:
             color = _get_random_color()
-            if self.control['debugMode']:
+            if self.control["debugMode"]:
                 value1 = f"[bold {color}]{100 * self.current['progress'] / self.current['segs']:.3f}[/bold {color}]"
                 value2 = f"[bold {color}]{self._get_time():.3f}[/bold {color}]"
-                print(f"* {self.logo} progress {value1} %. Time consumption: {value2} s.")
-            elif self.current['counter'] >= self.control['printPer']:
+                print(
+                    f"* {self.logo} progress {value1} %. Time consumption: {value2} s."
+                )
+            elif self.current["counter"] >= self.control["printPer"]:
                 value1 = f"[bold {color}]{100 * self.current['progress'] / self.current['segs']:.3f}[/bold {color}]"
                 value2 = f"[bold {color}]{self._get_time():.3f}[/bold {color}]"
-                print(f"* {self.logo} progress {value1} %. Time consumption: {value2} s.")
-                self.current['counter'] = 0
-
-        if (self.current['segs'] > 0) and (self.current['progress'] >= self.current['segs']):
+                print(
+                    f"* {self.logo} progress {value1} %. Time consumption: {value2} s."
+                )
+                self.current["counter"] = 0
+
+        if (self.current["segs"] > 0) and (
+            self.current["progress"] >= self.current["segs"]
+        ):
             color = _get_random_color()
             value = f"[bold {color}]{self._get_time():.3f}[/bold {color}]"
             print(
-                f">>> {self.logo} [{color}]Successfully finished[/{color}]! Time consumption: {value} s.")
+                f">>> {self.logo} [{color}]Successfully finished[/{color}]! Time consumption: {value} s."
+            )
         return 0
 
-    def _RecursiveAnalyze(self, step: float, algoIndex: int,
-                          testIterTimes: int, testTol: float,
-                          vcontrol: dict, vcurrent: dict):
+    def _RecursiveAnalyze(
+        self,
+        step: float,
+        algoIndex: int,
+        testIterTimes: int,
+        testTol: float,
+        vcontrol: dict,
+        vcurrent: dict,
+    ):
         """RecursiveAnalyze.
 
         Parameters
         ----------
         step : float
             step size, dynamic analysis is dt;
             static analysis is the displacement of small loading section, <=maxStep
@@ -416,323 +471,462 @@
 
         Returns
         -------
         int
             Analysis flag, if < 0, analysis failed; elsewise = 0 success.
         """
 
-        if vcontrol['debugMode']:
+        if vcontrol["debugMode"]:
             color = _get_random_color()
-            values = f"[bold {color}]step=%.3e, algoIndex=%i, testIterTimes=%i, testTol=%.3e[/bold {color}]" % (
-                step, vcontrol['algoTypes'][algoIndex], testIterTimes, testTol)
+            values = (
+                f"[bold {color}]step=%.3e, algoIndex=%i, testIterTimes=%i, testTol=%.3e[/bold {color}]"
+                % (step, vcontrol["algoTypes"][algoIndex], testIterTimes, testTol)
+            )
             print(f"*** {self.logo} Run Recursive: {values}\n")
 
-        if algoIndex != vcurrent['algoIndex']:
+        if algoIndex != vcurrent["algoIndex"]:
             color = _get_random_color()
             values = f"[bold {color}]%i[/bold {color}]" % (
-                vcontrol['algoTypes'][algoIndex])
+                vcontrol["algoTypes"][algoIndex]
+            )
             print(f">>> {self.logo} Setting algorithm to {values}\n")
-            self._setAlgorithm(vcontrol['algoTypes'][algoIndex], self.control["UserAlgoArgs"])
-            vcurrent['algoIndex'] = algoIndex
+            self._setAlgorithm(
+                vcontrol["algoTypes"][algoIndex], self.control["UserAlgoArgs"]
+            )
+            vcurrent["algoIndex"] = algoIndex
 
-        if testIterTimes != vcurrent['testIterTimes'] or testTol != vcurrent['testTol']:
-            if testIterTimes != vcurrent['testIterTimes']:
+        if testIterTimes != vcurrent["testIterTimes"] or testTol != vcurrent["testTol"]:
+            if testIterTimes != vcurrent["testIterTimes"]:
                 color = _get_random_color()
                 values = f"[bold {color}]%i[/bold {color}]" % testIterTimes
-                print(
-                    f">>> {self.logo} Setting test iteration times to {values}\n")
-                vcurrent['testIterTimes'] = testIterTimes
-            if testTol != vcurrent['testTol']:
+                print(f">>> {self.logo} Setting test iteration times to {values}\n")
+                vcurrent["testIterTimes"] = testIterTimes
+            if testTol != vcurrent["testTol"]:
                 color = _get_random_color()
                 print(
-                    f">>> {self.logo} Setting test tolerance to [bold {color}]%f[/bold {color}]\n" % testTol)
-                vcurrent['testTol'] = testTol
-            ops.test(vcontrol['testType'], testTol,
-                     testIterTimes, vcontrol['testPrintFlag'])
+                    f">>> {self.logo} Setting test tolerance to [bold {color}]%f[/bold {color}]\n"
+                    % testTol
+                )
+                vcurrent["testTol"] = testTol
+            ops.test(
+                vcontrol["testType"], testTol, testIterTimes, vcontrol["testPrintFlag"]
+            )
         # static step size
-        if vcontrol['analysis'] == 'Static' and vcurrent['step'] != step:
+        if vcontrol["analysis"] == "Static" and vcurrent["step"] != step:
             color = _get_random_color()
             print(
-                f">>> {self.logo} Setting step to [bold {color}]%.3e[/bold {color}]\n" % step)
-            ops.integrator('DisplacementControl',
-                           vcurrent['node'], vcurrent['dof'], step)
-            vcurrent['step'] = step
+                f">>> {self.logo} Setting step to [bold {color}]%.3e[/bold {color}]\n"
+                % step
+            )
+            ops.integrator(
+                "DisplacementControl", vcurrent["node"], vcurrent["dof"], step
+            )
+            vcurrent["step"] = step
         # trial analyze once
-        if vcontrol['analysis'] == 'Static':
+        if vcontrol["analysis"] == "Static":
             ok = ops.analyze(1)
         else:
             ok = ops.analyze(1, step)
         if ok == 0:
             return 0
         # If not convergence, add test iteration times. Use current step, algorithm and test tolerance.
-        if vcontrol['tryAddTestTimes'] and testIterTimes != vcontrol['testIterTimesMore']:
+        if (
+            vcontrol["tryAddTestTimes"]
+            and testIterTimes != vcontrol["testIterTimesMore"]
+        ):
             norm = ops.testNorm()
             color = _get_random_color()
-            if norm[-1] < vcontrol['normTol']:
-                print(f">>> {self.logo} Adding test times to [bold {color}]%i[/bold {color}].\n" % (
-                    vcontrol['testIterTimesMore']))
-                return self._RecursiveAnalyze(step, algoIndex, vcontrol['testIterTimesMore'],
-                                              testTol, vcontrol, vcurrent)
+            if norm[-1] < vcontrol["normTol"]:
+                print(
+                    f">>> {self.logo} Adding test times to [bold {color}]%i[/bold {color}].\n"
+                    % (vcontrol["testIterTimesMore"])
+                )
+                return self._RecursiveAnalyze(
+                    step,
+                    algoIndex,
+                    vcontrol["testIterTimesMore"],
+                    testTol,
+                    vcontrol,
+                    vcurrent,
+                )
             else:
-                print(f">>> {self.logo} Not adding test times for norm [bold {color}]%.3e[/bold {color}].\n" % (
-                    norm[-1]))
+                print(
+                    f">>> {self.logo} Not adding test times for norm [bold {color}]%.3e[/bold {color}].\n"
+                    % (norm[-1])
+                )
 
         # Change algorithm. Set back test iteration times.
-        if vcontrol['tryAlterAlgoTypes'] and (algoIndex + 1) < len(vcontrol['algoTypes']):
+        if vcontrol["tryAlterAlgoTypes"] and (algoIndex + 1) < len(
+            vcontrol["algoTypes"]
+        ):
             algoIndex += 1
             color = _get_random_color()
-            print(f">>> {self.logo} Setting algorithm to [bold {color}]%i[/bold {color}].\n" % (
-                vcontrol['algoTypes'][algoIndex]))
-            return self._RecursiveAnalyze(step, algoIndex, testIterTimes, testTol, vcontrol, vcurrent)
+            print(
+                f">>> {self.logo} Setting algorithm to [bold {color}]%i[/bold {color}].\n"
+                % (vcontrol["algoTypes"][algoIndex])
+            )
+            return self._RecursiveAnalyze(
+                step, algoIndex, testIterTimes, testTol, vcontrol, vcurrent
+            )
 
         # If step length is too small, try add test tolerance. set algorithm and test iteration times back.
         # Split the current step into two steps.
-        stepNew = step * vcontrol['relaxation']
-        if 0 < stepNew < vcontrol['minStep']:
-            stepNew = vcontrol['minStep']
-        if 0 > stepNew > -vcontrol['minStep']:
-            stepNew = -vcontrol['minStep']
-        if np.abs(stepNew) < vcontrol['minStep']:
+        stepNew = step * vcontrol["relaxation"]
+        # if 0 < stepNew < vcontrol['minStep']:
+        #     stepNew = vcontrol['minStep']
+        # if 0 > stepNew > -vcontrol['minStep']:
+        #     stepNew = -vcontrol['minStep']
+        if np.abs(stepNew) < vcontrol["minStep"]:
             color = _get_random_color()
             print(
-                f">>> {self.logo} current step [bold {color}]%.3e[/bold {color}] beyond the min step!\n" % stepNew)
-            if vcontrol['tryLooseTestTol'] and vcurrent['testTol'] != vcontrol['looseTestTolTo']:
+                f">>> {self.logo} current step [bold {color}]%.3e[/bold {color}] beyond the min step!\n"
+                % stepNew
+            )
+            if (
+                vcontrol["tryLooseTestTol"]
+                and vcurrent["testTol"] != vcontrol["looseTestTolTo"]
+            ):
                 print(
-                    f"!!! {self.logo} Warning: [bold {color}]Loosing test tolerance[/bold {color}]\n")
-                return self._RecursiveAnalyze(step, 0, vcontrol['testIterTimes'],
-                                              vcontrol['looseTestTolTo'], vcontrol, vcurrent)
+                    f"!!! {self.logo} Warning: [bold {color}]Loosing test tolerance[/bold {color}]\n"
+                )
+                return self._RecursiveAnalyze(
+                    step,
+                    0,
+                    vcontrol["testIterTimes"],
+                    vcontrol["looseTestTolTo"],
+                    vcontrol,
+                    vcurrent,
+                )
             # Here, all methods have been tried. Return negative value.
             return -1
 
         stepRest = step - stepNew
         color = _get_random_color()
-        print(f">>> {self.logo} Dividing the current step [bold {color}]%.3e into %.3e and %.3e[/bold {color}]\n" % (
-            step, stepNew, stepRest))
+        print(
+            f">>> {self.logo} Dividing the current step [bold {color}]%.3e into %.3e and %.3e[/bold {color}]\n"
+            % (step, stepNew, stepRest)
+        )
         ok = self._RecursiveAnalyze(
-            stepNew, 0, testIterTimes, testTol, vcontrol, vcurrent)
+            stepNew, 0, testIterTimes, testTol, vcontrol, vcurrent
+        )
         if ok < 0:
             return -1
         ok = self._RecursiveAnalyze(
-            stepRest, 0, testIterTimes, testTol, vcontrol, vcurrent)
+            stepRest, 0, testIterTimes, testTol, vcontrol, vcurrent
+        )
         if ok < 0:
             return -1
         return 0
 
     def _setAlgorithm(self, algotype, user_algo_args: list = None):
         color = _get_random_color()
 
         def case0():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]Linear ...[/bold {color}]")
-            ops.algorithm('Linear')
+                f"> {self.logo} Setting algorithm to  [bold {color}]Linear ...[/bold {color}]"
+            )
+            ops.algorithm("Linear")
 
         def case1():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]Linear -initial ...[/bold {color}]")
-            ops.algorithm('Linear', "-Initial")
+                f"> {self.logo} Setting algorithm to  [bold {color}]Linear -initial ...[/bold {color}]"
+            )
+            ops.algorithm("Linear", "-Initial")
 
         def case2():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]Linear -secant ...[/bold {color}]")
-            ops.algorithm('Linear', "-Secant")
+                f"> {self.logo} Setting algorithm to  [bold {color}]Linear -secant ...[/bold {color}]"
+            )
+            ops.algorithm("Linear", "-Secant")
 
         def case3():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]Linear -factorOnce ...[/bold {color}]")
-            ops.algorithm('Linear', "-FactorOnce")
+                f"> {self.logo} Setting algorithm to  [bold {color}]Linear -factorOnce ...[/bold {color}]"
+            )
+            ops.algorithm("Linear", "-FactorOnce")
 
         def case4():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]Linear -initial -factorOnce ...[/bold {color}]")
-            ops.algorithm('Linear', "-Initial", "-FactorOnce")
+                f"> {self.logo} Setting algorithm to  [bold {color}]Linear -initial -factorOnce ...[/bold {color}]"
+            )
+            ops.algorithm("Linear", "-Initial", "-FactorOnce")
 
         def case5():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]Linear -secant -factorOnce ...[/bold {color}]")
-            ops.algorithm('Linear', "-Secant", "-FactorOnce")
+                f"> {self.logo} Setting algorithm to  [bold {color}]Linear -secant -factorOnce ...[/bold {color}]"
+            )
+            ops.algorithm("Linear", "-Secant", "-FactorOnce")
 
         def case10():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]Newton ...[/bold {color}]")
-            ops.algorithm('Newton')
+                f"> {self.logo} Setting algorithm to  [bold {color}]Newton ...[/bold {color}]"
+            )
+            ops.algorithm("Newton")
 
         def case11():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]Newton -initial ...[/bold {color}]")
-            ops.algorithm('Newton', "-Initial")
+                f"> {self.logo} Setting algorithm to  [bold {color}]Newton -initial ...[/bold {color}]"
+            )
+            ops.algorithm("Newton", "-Initial")
 
         def case12():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]Newton -initialThenCurrent ...[/bold {color}]")
-            ops.algorithm('Newton', "-intialThenCurrent")
+                f"> {self.logo} Setting algorithm to  [bold {color}]Newton -initialThenCurrent ...[/bold {color}]"
+            )
+            ops.algorithm("Newton", "-intialThenCurrent")
 
         def case13():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]Newton -Secant ...[/bold {color}]")
-            ops.algorithm('Newton', "-Secant")
+                f"> {self.logo} Setting algorithm to  [bold {color}]Newton -Secant ...[/bold {color}]"
+            )
+            ops.algorithm("Newton", "-Secant")
 
         def case20():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]NewtonLineSearch ...[/bold {color}]")
-            ops.algorithm('NewtonLineSearch')
+                f"> {self.logo} Setting algorithm to  [bold {color}]NewtonLineSearch ...[/bold {color}]"
+            )
+            ops.algorithm("NewtonLineSearch")
 
         def case21():
-            print(f"> {self.logo} Setting algorithm to "
-                  f"[bold {color}]NewtonLineSearch -type Bisection ...[/bold {color}]")
-            ops.algorithm('NewtonLineSearch', "-type", "Bisection")
+            print(
+                f"> {self.logo} Setting algorithm to "
+                f"[bold {color}]NewtonLineSearch -type Bisection ...[/bold {color}]"
+            )
+            ops.algorithm("NewtonLineSearch", "-type", "Bisection")
 
         def case22():
-            print(f"> {self.logo} Setting algorithm to "
-                  f"[bold {color}]NewtonLineSearch -type Secant ...[/bold {color}]")
-            ops.algorithm('NewtonLineSearch', "-type", "Secant")
+            print(
+                f"> {self.logo} Setting algorithm to "
+                f"[bold {color}]NewtonLineSearch -type Secant ...[/bold {color}]"
+            )
+            ops.algorithm("NewtonLineSearch", "-type", "Secant")
 
         def case23():
-            print(f"> {self.logo} Setting algorithm to "
-                  f"[bold {color}]NewtonLineSearch -type RegulaFalsi ...[/bold {color}]")
-            ops.algorithm('NewtonLineSearch', "-type", "RegulaFalsi")
+            print(
+                f"> {self.logo} Setting algorithm to "
+                f"[bold {color}]NewtonLineSearch -type RegulaFalsi ...[/bold {color}]"
+            )
+            ops.algorithm("NewtonLineSearch", "-type", "RegulaFalsi")
 
         def case24():
-            print(f"> {self.logo} Setting algorithm to "
-                  f"[bold {color}]NewtonLineSearch -type LinearInterpolated ...[/bold {color}]")
-            ops.algorithm('NewtonLineSearch', "-type", "LinearInterpolated")
+            print(
+                f"> {self.logo} Setting algorithm to "
+                f"[bold {color}]NewtonLineSearch -type LinearInterpolated ...[/bold {color}]"
+            )
+            ops.algorithm("NewtonLineSearch", "-type", "LinearInterpolated")
 
         def case25():
-            print(f"> {self.logo} Setting algorithm to "
-                  f"[bold {color}]NewtonLineSearch -type InitialInterpolated ...[/bold {color}]")
-            ops.algorithm('NewtonLineSearch', "-type", "InitialInterpolated")
+            print(
+                f"> {self.logo} Setting algorithm to "
+                f"[bold {color}]NewtonLineSearch -type InitialInterpolated ...[/bold {color}]"
+            )
+            ops.algorithm("NewtonLineSearch", "-type", "InitialInterpolated")
 
         def case30():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]Modified Newton ...[/bold {color}]")
-            ops.algorithm('ModifiedNewton')
+                f"> {self.logo} Setting algorithm to  [bold {color}]Modified Newton ...[/bold {color}]"
+            )
+            ops.algorithm("ModifiedNewton")
 
         def case31():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]ModifiedNewton -initial ...[/bold {color}]")
-            ops.algorithm('ModifiedNewton', "-initial")
+                f"> {self.logo} Setting algorithm to  [bold {color}]ModifiedNewton -initial ...[/bold {color}]"
+            )
+            ops.algorithm("ModifiedNewton", "-initial")
 
         def case32():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]ModifiedNewton -secant ...[/bold {color}]")
-            ops.algorithm('ModifiedNewton', "-secant")
+                f"> {self.logo} Setting algorithm to  [bold {color}]ModifiedNewton -secant ...[/bold {color}]"
+            )
+            ops.algorithm("ModifiedNewton", "-secant")
 
         def case40():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]KrylovNewton ...[/bold {color}]")
-            ops.algorithm('KrylovNewton')
+                f"> {self.logo} Setting algorithm to  [bold {color}]KrylovNewton ...[/bold {color}]"
+            )
+            ops.algorithm("KrylovNewton")
 
         def case41():
-            print(f"> {self.logo} Setting algorithm to "
-                  f"[bold {color}]KrylovNewton -iterate initial ...[/bold {color}]")
-            ops.algorithm('KrylovNewton', "-iterate", 'initial')
+            print(
+                f"> {self.logo} Setting algorithm to "
+                f"[bold {color}]KrylovNewton -iterate initial ...[/bold {color}]"
+            )
+            ops.algorithm("KrylovNewton", "-iterate", "initial")
 
         def case42():
-            print(f"> {self.logo} Setting algorithm to "
-                  f"[bold {color}]KrylovNewton -increment initial ...[/bold {color}]")
-            ops.algorithm('KrylovNewton', "-increment", 'initial')
+            print(
+                f"> {self.logo} Setting algorithm to "
+                f"[bold {color}]KrylovNewton -increment initial ...[/bold {color}]"
+            )
+            ops.algorithm("KrylovNewton", "-increment", "initial")
 
         def case43():
-            print(f"> {self.logo} Setting algorithm to "
-                  f"[bold {color}]KrylovNewton -iterate initial -increment initial ...[/bold {color}]")
-            ops.algorithm('KrylovNewton', "-iterate", 'initial', "-increment", 'initial')
+            print(
+                f"> {self.logo} Setting algorithm to "
+                f"[bold {color}]KrylovNewton -iterate initial -increment initial ...[/bold {color}]"
+            )
+            ops.algorithm(
+                "KrylovNewton", "-iterate", "initial", "-increment", "initial"
+            )
 
         def case44():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]KrylovNewton -maxDim 10[/bold {color}]")
-            ops.algorithm('KrylovNewton', "-maxDim", 10)
+                f"> {self.logo} Setting algorithm to  [bold {color}]KrylovNewton -maxDim 10[/bold {color}]"
+            )
+            ops.algorithm("KrylovNewton", "-maxDim", 10)
 
         def case45():
-            print(f"> {self.logo} Setting algorithm to "
-                  f"[bold {color}]KrylovNewton -iterate initial -increment initial -maxDim 10[/bold {color}]")
-            ops.algorithm('KrylovNewton', "-iterate", 'initial', "-increment", 'initial', "-maxDim", 10)
+            print(
+                f"> {self.logo} Setting algorithm to "
+                f"[bold {color}]KrylovNewton -iterate initial -increment initial -maxDim 10[/bold {color}]"
+            )
+            ops.algorithm(
+                "KrylovNewton",
+                "-iterate",
+                "initial",
+                "-increment",
+                "initial",
+                "-maxDim",
+                10,
+            )
 
         def case50():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]SecantNewton ...[/bold {color}]")
-            ops.algorithm('SecantNewton')
+                f"> {self.logo} Setting algorithm to  [bold {color}]SecantNewton ...[/bold {color}]"
+            )
+            ops.algorithm("SecantNewton")
 
         def case51():
-            print(f"> {self.logo} Setting algorithm to "
-                  f"[bold {color}]SecantNewton -iterate initial ...[/bold {color}]")
-            ops.algorithm('SecantNewton', "-iterate", 'initial')
+            print(
+                f"> {self.logo} Setting algorithm to "
+                f"[bold {color}]SecantNewton -iterate initial ...[/bold {color}]"
+            )
+            ops.algorithm("SecantNewton", "-iterate", "initial")
 
         def case52():
-            print(f"> {self.logo} Setting algorithm to "
-                  f"[bold {color}]SecantNewton -increment initial  ...[/bold {color}]")
-            ops.algorithm('SecantNewton', "-increment", 'initial')
+            print(
+                f"> {self.logo} Setting algorithm to "
+                f"[bold {color}]SecantNewton -increment initial  ...[/bold {color}]"
+            )
+            ops.algorithm("SecantNewton", "-increment", "initial")
 
         def case53():
-            print(f"> {self.logo} Setting algorithm to "
-                  f"[bold {color}]SecantNewton -iterate initial -increment initial ...[/bold {color}]")
-            ops.algorithm('SecantNewton', "-iterate", 'initial', "-increment", 'initial')
+            print(
+                f"> {self.logo} Setting algorithm to "
+                f"[bold {color}]SecantNewton -iterate initial -increment initial ...[/bold {color}]"
+            )
+            ops.algorithm(
+                "SecantNewton", "-iterate", "initial", "-increment", "initial"
+            )
 
         def case60():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]BFGS ...[/bold {color}]")
-            ops.algorithm('BFGS')
+                f"> {self.logo} Setting algorithm to  [bold {color}]BFGS ...[/bold {color}]"
+            )
+            ops.algorithm("BFGS")
 
         def case61():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]BFGS -initial...[/bold {color}]")
-            ops.algorithm('BFGS', "-initial")
+                f"> {self.logo} Setting algorithm to  [bold {color}]BFGS -initial...[/bold {color}]"
+            )
+            ops.algorithm("BFGS", "-initial")
 
         def case62():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]BFGS -secant ...[/bold {color}]")
-            ops.algorithm('BFGS', "-secant")
+                f"> {self.logo} Setting algorithm to  [bold {color}]BFGS -secant ...[/bold {color}]"
+            )
+            ops.algorithm("BFGS", "-secant")
 
         def case70():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]Broyden ...[/bold {color}]")
-            ops.algorithm('Broyden')
+                f"> {self.logo} Setting algorithm to  [bold {color}]Broyden ...[/bold {color}]"
+            )
+            ops.algorithm("Broyden")
 
         def case71():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]Broyden -initial ...[/bold {color}]")
-            ops.algorithm('Broyden', "-initial")
+                f"> {self.logo} Setting algorithm to  [bold {color}]Broyden -initial ...[/bold {color}]"
+            )
+            ops.algorithm("Broyden", "-initial")
 
         def case72():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]Broyden -secant ...[/bold {color}]")
-            ops.algorithm('Broyden', "-secant")
+                f"> {self.logo} Setting algorithm to  [bold {color}]Broyden -secant ...[/bold {color}]"
+            )
+            ops.algorithm("Broyden", "-secant")
 
         def case80():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]PeriodicNewton ...[/bold {color}]")
-            ops.algorithm('PeriodicNewton')
+                f"> {self.logo} Setting algorithm to  [bold {color}]PeriodicNewton ...[/bold {color}]"
+            )
+            ops.algorithm("PeriodicNewton")
 
         def case81():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]PeriodicNewton -maxDim, 10 ...[/bold {color}]")
-            ops.algorithm('PeriodicNewton', "-maxDim", 10)
+                f"> {self.logo} Setting algorithm to  [bold {color}]PeriodicNewton -maxDim, 10 ...[/bold {color}]"
+            )
+            ops.algorithm("PeriodicNewton", "-maxDim", 10)
 
         def case90():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]ExpressNewton ...[/bold {color}]")
-            ops.algorithm('ExpressNewton')
+                f"> {self.logo} Setting algorithm to  [bold {color}]ExpressNewton ...[/bold {color}]"
+            )
+            ops.algorithm("ExpressNewton")
 
         def case91():
             print(
-                f"> {self.logo} Setting algorithm to  [bold {color}]ExpressNewton -InitialTangent ...[/bold {color}]")
-            ops.algorithm('ExpressNewton', "-InitialTangent")
+                f"> {self.logo} Setting algorithm to  [bold {color}]ExpressNewton -InitialTangent ...[/bold {color}]"
+            )
+            ops.algorithm("ExpressNewton", "-InitialTangent")
 
         def case100():
             # User algorithm0
             if user_algo_args is not None:
                 ops.algorithm(*user_algo_args)
 
         def default():
             raise ValueError("!!! SmartAnalyze: ERROR! WRONG Algorithm Type!")
 
-        switch = {0: case0, 1: case1, 2: case2, 3: case3, 4: case4, 5: case5,
-                  10: case10, 11: case11, 12: case12, 13: case13,
-                  20: case20, 21: case21, 22: case22, 23: case23, 24: case24, 25: case25,
-                  30: case30, 31: case31, 32: case32,
-                  40: case40, 41: case41, 42: case42, 43: case43, 44: case44, 45: case45,
-                  50: case50, 51: case51, 52: case52, 53: case53,
-                  60: case60, 61: case61, 62: case62,
-                  70: case70, 71: case71, 72: case72,
-                  80: case80, 81: case81,
-                  90: case90, 91: case91,
-                  100: case100}
+        switch = {
+            0: case0,
+            1: case1,
+            2: case2,
+            3: case3,
+            4: case4,
+            5: case5,
+            10: case10,
+            11: case11,
+            12: case12,
+            13: case13,
+            20: case20,
+            21: case21,
+            22: case22,
+            23: case23,
+            24: case24,
+            25: case25,
+            30: case30,
+            31: case31,
+            32: case32,
+            40: case40,
+            41: case41,
+            42: case42,
+            43: case43,
+            44: case44,
+            45: case45,
+            50: case50,
+            51: case51,
+            52: case52,
+            53: case53,
+            60: case60,
+            61: case61,
+            62: case62,
+            70: case70,
+            71: case71,
+            72: case72,
+            80: case80,
+            81: case81,
+            90: case90,
+            91: case91,
+            100: case100,
+        }
 
         switch.get(algotype, default)()
```

### Comparing `opstool-0.7.3/src/opstool/examples/ArchBridge.py` & `opstool-0.8.0/src/opstool/examples/ArchBridge.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.3/src/opstool/examples/ArchBridge2.py` & `opstool-0.8.0/src/opstool/examples/ArchBridge2.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.3/src/opstool/examples/CableStayedBridge.py` & `opstool-0.8.0/src/opstool/examples/CableStayedBridge.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.3/src/opstool/examples/Dam.py` & `opstool-0.8.0/src/opstool/examples/Dam.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.3/src/opstool/examples/DamBreak.py` & `opstool-0.8.0/src/opstool/examples/DamBreak.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.3/src/opstool/examples/Frame3D.py` & `opstool-0.8.0/src/opstool/examples/Frame3D.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.3/src/opstool/examples/Igloo.py` & `opstool-0.8.0/src/opstool/examples/Igloo.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.3/src/opstool/examples/Pier.py` & `opstool-0.8.0/src/opstool/examples/Pier.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.3/src/opstool/examples/SDOF.py` & `opstool-0.8.0/src/opstool/examples/SDOF.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.3/src/opstool/examples/SuspensionBridge.py` & `opstool-0.8.0/src/opstool/examples/SuspensionBridge.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.3/src/opstool/preprocessing/__init__.py` & `opstool-0.8.0/src/opstool/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.3/src/opstool/preprocessing/geom_transf.py` & `opstool-0.8.0/src/opstool/preprocessing/geom_transf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import numpy as np
 import openseespy.opensees as ops
 
 
-def beam_geom_transf(nodeTagI: int, nodeTagJ: int, transfType: str,
-                     dI: list = None, dJ: list = None):
+def beam_geom_transf(
+    nodeTagI: int, nodeTagJ: int, transfType: str, dI: list = None, dJ: list = None
+):
     """Output the geometric transformation tag of the beam element according to the node tag previously defined.
     This function divide beam elements into two classes, vertical ones and non-vertical ones,
     vertical elements ``vecxz = [-1, 0, 0]``, and non-vertical elements ``vecxz = [0, 0, 1]``.
-    See `geomTransf commands doc <https://openseespydoc.readthedocs.io/en/latest/src/geomTransf.html>`_ 
+    See `geomTransf commands doc <https://openseespydoc.readthedocs.io/en/latest/src/geomTransf.html>`_
 
     Parameters
     ----------
     nodeTagI : int
         Previously defined I-end node tag.
     nodeTagJ : int
         Previously defined J-end node tag.
@@ -28,40 +29,42 @@
     -------
     int
         Geometric transformation tag that this function internally defined.
     """
     coordI, coordJ = ops.nodeCoord(nodeTagI), ops.nodeCoord(nodeTagJ)
     if len(coordI) < 3 or len(coordJ) < 3:
         raise ValueError("This geometric transformations only for 3D!")
-    if transfType not in ['Linear', 'PDelta', 'Corotational']:
+    if transfType not in ["Linear", "PDelta", "Corotational"]:
         raise ValueError(
-            "transfType must be one of ['Linear', 'PDelta', 'Corotational']!")
+            "transfType must be one of ['Linear', 'PDelta', 'Corotational']!"
+        )
     coordI = np.array(coordI)
     coordJ = np.array(coordJ)
     xaxis = coordJ - coordI
     global_z = [0, 0, 1]
-    cos_angle = xaxis.dot(global_z) / (np.linalg.norm(xaxis)
-                                       * np.linalg.norm(global_z))
-    if np.abs(1 - cos_angle ** 2) < 1e-10:
+    cos_angle = xaxis.dot(global_z) / (np.linalg.norm(xaxis) * np.linalg.norm(global_z))
+    if np.abs(1 - cos_angle**2) < 1e-10:
         tag = _creat_geom_transf(transfType, dI=dI, dJ=dJ, ver=True)
     else:
         tag = _creat_geom_transf(transfType, dI=dI, dJ=dJ, ver=False)
     return tag
 
 
-def _creat_geom_transf(transfType: str, dI: list = None, dJ: list = None, ver: bool = False):
+def _creat_geom_transf(
+    transfType: str, dI: list = None, dJ: list = None, ver: bool = False
+):
     CrdTransfTags = ops.getCrdTransfTags()
-    if CrdTransfTags:
-        tag = np.max(CrdTransfTags) + 1
+    if len(CrdTransfTags) > 0:
+        tag = int(np.max(CrdTransfTags) + 1)
     else:
         tag = 1
     if ver:
-        vecxz = [-1., 0., 0.]
+        vecxz = [-1.0, 0.0, 0.0]
     else:
-        vecxz = [0., 0., 1.]
+        vecxz = [0.0, 0.0, 1.0]
     if dI is None and dJ is None:
         ops.geomTransf(transfType, tag, *vecxz)
     elif dI and dJ:
-        ops.geomTransf(transfType, tag, *vecxz, '-jntOffset', *dI, *dJ)
+        ops.geomTransf(transfType, tag, *vecxz, "-jntOffset", *dI, *dJ)
     else:
         raise ValueError("dI and dJ must be both None or input at the same time!")
     return tag
```

### Comparing `opstool-0.7.3/src/opstool/preprocessing/load.py` & `opstool-0.8.0/src/opstool/preprocessing/load.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import numpy as np
 import openseespy.opensees as ops
 
 
-def gen_grav_load(ts_tag: int,
-                  pattern_tag: int,
-                  exclude_nodes: list = None,
-                  direction: str = "Z",
-                  factor: float = -9.81):
+def gen_grav_load(
+    ts_tag: int,
+    pattern_tag: int,
+    exclude_nodes: list = None,
+    direction: str = "Z",
+    factor: float = -9.81,
+):
     """Applying the gravity loads.
 
     Notes
     -----
     The mass values are from ``nodeMass(nodeTag)`` command, i.e., ones set in ``mass()`` command.
 
     Parameters
@@ -32,31 +34,32 @@
 
     Returns
     --------
     None
 
     """
     direction = direction.upper()
-    ops.timeSeries('Linear', int(ts_tag))
-    ops.pattern('Plain', int(pattern_tag), int(ts_tag))
+    ops.timeSeries("Linear", int(ts_tag))
+    ops.pattern("Plain", int(pattern_tag), int(ts_tag))
     node_tags = ops.getNodeTags()
     if exclude_nodes is not None:
         node_tags = [tag for tag in node_tags if tag not in exclude_nodes]
-    load_fact_6d = dict(Z=np.array([0.0, 0.0, factor, 0.0, 0.0, 0.0]),
-                        Y=np.array([0.0, factor, 0.0, 0.0, 0.0, 0.0]),
-                        X=np.array([factor, 0.0, 0.0, 0.0, 0.0, 0.0]),
-                        )
-    load_fact_3d = dict(Z=np.array([0.0, 0.0, factor]),
-                        Y=np.array([0.0, factor, 0]),
-                        X=np.array([factor, 0.0, 0.0]),
-                        )
-    load_fact_2d = dict(Y=np.array([0.0, factor]),
-                        X=np.array([factor, 0.0]),
-                        )
+    load_fact_6d = dict(
+        Z=np.array([0.0, 0.0, factor, 0.0, 0.0, 0.0]),
+        Y=np.array([0.0, factor, 0.0, 0.0, 0.0, 0.0]),
+        X=np.array([factor, 0.0, 0.0, 0.0, 0.0, 0.0]),
+    )
+    load_fact_3d = dict(
+        Z=np.array([0.0, 0.0, factor]),
+        Y=np.array([0.0, factor, 0]),
+        X=np.array([factor, 0.0, 0.0]),
+    )
+    load_fact_2d = dict(
+        Y=np.array([0.0, factor]),
+        X=np.array([factor, 0.0]),
+    )
     load_fact_1d = dict(X=np.array([factor, 0.0]))
-    load_fact = {6: load_fact_6d, 3: load_fact_3d,
-                 2: load_fact_2d, 1: load_fact_1d}
+    load_fact = {6: load_fact_6d, 3: load_fact_3d, 2: load_fact_2d, 1: load_fact_1d}
     for nodetag in node_tags:
         mass = np.array(ops.nodeMass(nodetag))
         loadValues = mass * load_fact[len(mass)][direction]
-        if np.sum(np.abs(loadValues)) > 1e-10:
-            ops.load(nodetag, *loadValues)
+        ops.load(nodetag, *loadValues)
```

### Comparing `opstool-0.7.3/src/opstool/preprocessing/section/__init__.py` & `opstool-0.8.0/src/opstool/preprocessing/section/__init__.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.3/src/opstool/preprocessing/section/sec_mesh.py` & `opstool-0.8.0/src/opstool/preprocessing/section/sec_mesh.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
     Returns
     -----------
     None
     """
 
     def __init__(self, sec_name: str = "My Section"):
-
         self.sec_name = sec_name
 
         # * mesh obj
         self.mesh_obj = None
         self.section = None
         self.points = None
         self.cells_map = dict()
@@ -151,22 +150,24 @@
         mesh_sizes = []
         if not self.color_map:
             for name in self.group_map.keys():
                 self.color_map[name] = _get_random_color()
         # mat_names = [geom.material.name for geom in self.group_map.values()]
         for name, geom in self.group_map.items():
             # if len(mat_names) != len(set(mat_names)):
-            geom.material = add_material(name=name,
-                                         elastic_modulus=geom.material.elastic_modulus,
-                                         poissons_ratio=geom.material.poissons_ratio,
-                                         yield_strength=geom.material.yield_strength,
-                                         density=geom.material.density,
-                                         color=self.color_map[name])
+            geom.material = add_material(
+                name=name,
+                elastic_modulus=geom.material.elastic_modulus,
+                poissons_ratio=geom.material.poissons_ratio,
+                yield_strength=geom.material.yield_strength,
+                density=geom.material.density,
+                color=self.color_map[name],
+            )
             geoms.append(geom)
-            mesh_sizes.append(self.mesh_size_map[name] / 10)
+            mesh_sizes.append(self.mesh_size_map[name])
         geom_obj = CompoundGeometry(geoms)
         mesh_obj = geom_obj.create_mesh(mesh_sizes=mesh_sizes)
         self.section = Section(geom_obj, time_info=False)
         self.mesh_obj = mesh_obj.mesh
         self._get_mesh_data()
         if plot_mesh:
             self.section.plot_mesh(materials=True, alpha=0.90)
@@ -265,15 +266,15 @@
             for data in self.rebar_data:
                 rebar_xy = data["rebar_xy"]
                 dia = data["dia"]
                 rebar_coords = []
                 rebar_areas = []
                 for xy in rebar_xy:
                     rebar_coords.append(xy)
-                    rebar_areas.append(np.pi / 4 * dia ** 2)
+                    rebar_areas.append(np.pi / 4 * dia**2)
                 all_rebar_area += np.sum(rebar_areas)
             rho_rebar = all_rebar_area / area
         else:
             rho_rebar = 0
         sec_props = dict(
             A=area,
             Asy=area_sx / Eref,
@@ -289,18 +290,21 @@
             J=j,
             phi=phi,
             mass=mass,
             rho_rebar=rho_rebar,
         )
         self.sec_props = sec_props
 
-    def get_sec_props(self, Eref: float = 1.0,
-                      Gref: float = None,
-                      display_results: bool = False,
-                      plot_centroids: bool = False):
+    def get_sec_props(
+        self,
+        Eref: float = 1.0,
+        Gref: float = None,
+        display_results: bool = False,
+        plot_centroids: bool = False,
+    ):
         """
         Solving Section Geometry Properties by Finite Element Method, by ``sectionproperties`` pacakge.
         See `sectionproperties doc <https://sectionproperties.readthedocs.io/en/latest/rst/post.html
         #getting-specific-section-properties>`_
 
         This command may be slower. If you don't need features such as shear area, you can use
         method :py:meth:`~opstool.preprocessing.SecMesh.get_frame_props`.
@@ -353,42 +357,71 @@
             Gref = 0.5 * Eref
         section = self.section
         section.calculate_geometric_properties()
         section.calculate_warping_properties()
         self._run_sec_props(Eref, Gref, section)
         if display_results:
             # section.display_results()
-            syms = ["A", "Asy", "Asz", "centroid", "Iy", "Iz", "Iyz",
-                    "Wyt", "Wyb", "Wzt", "Wzb", "J", "phi", "mass", "rho_rebar"]
-            defs = ["Cross-sectional area", "Shear area y-axis", "Shear area z-axis", "Elastic centroid",
-                    "Moment of inertia y-axis", "Moment of inertia z-axis", "Product of inertia",
-                    "Section moduli of top fibres y-axis", "Section moduli of bottom fibres y-axis",
-                    "Section moduli of top fibres z-axis", "Section moduli of bottom fibres z-axis",
-                    "Torsion constant", "Principal axis angle", "Section mass", "Ratio of reinforcement"]
+            syms = [
+                "A",
+                "Asy",
+                "Asz",
+                "centroid",
+                "Iy",
+                "Iz",
+                "Iyz",
+                "Wyt",
+                "Wyb",
+                "Wzt",
+                "Wzb",
+                "J",
+                "phi",
+                "mass",
+                "rho_rebar",
+            ]
+            defs = [
+                "Cross-sectional area",
+                "Shear area y-axis",
+                "Shear area z-axis",
+                "Elastic centroid",
+                "Moment of inertia y-axis",
+                "Moment of inertia z-axis",
+                "Product of inertia",
+                "Section moduli of top fibres y-axis",
+                "Section moduli of bottom fibres y-axis",
+                "Section moduli of top fibres z-axis",
+                "Section moduli of bottom fibres z-axis",
+                "Torsion constant",
+                "Principal axis angle",
+                "Section mass",
+                "Ratio of reinforcement",
+            ]
             table = Table(title="Section Properties")
             table.add_column("Symbol", style="cyan", no_wrap=True)
             table.add_column("Value", style="magenta")
             table.add_column("Definition", style="green")
             for sym_, def_ in zip(syms, defs):
                 if sym_ != "centroid":
                     table.add_row(sym_, f"{self.sec_props[sym_]:.3E}", def_)
                 else:
-                    table.add_row(sym_,
-                                  f"({self.sec_props[sym_][0]:.3E}, {self.sec_props[sym_][1]:.3E})",
-                                  def_)
+                    table.add_row(
+                        sym_,
+                        f"({self.sec_props[sym_][0]:.3E}, {self.sec_props[sym_][1]:.3E})",
+                        def_,
+                    )
             console = Console()
             console.print(table)
         if plot_centroids:
             section.plot_centroids()
         return self.sec_props
 
-    def get_frame_props(self, Eref: float = 1.0,
-                        Gref: float = None,
-                        display_results: bool = False):
-        """Calculates and returns the properties required for a frame analysis. 
+    def get_frame_props(
+        self, Eref: float = 1.0, Gref: float = None, display_results: bool = False
+    ):
+        """Calculates and returns the properties required for a frame analysis.
         See `sectionproperties doc <https://sectionproperties.readthedocs.io/en/latest/rst/api.html
         #sectionproperties.analysis.section.Section.calculate_frame_properties>`_
 
         This method is fast, but cannot calculate the shear area compared to the
         method :py:meth:`~opstool.preprocessing.SecMesh.get_sec_props`.
 
         Parameters
@@ -432,23 +465,23 @@
             the y-axis refers to the abscissa,
             and the z-axis refers to the ordinate direction.
         """
         if Gref is None:
             Gref = 0.5 * Eref
         # self.section.calculate_geometric_properties()
         (ea, ixx_c, iyy_c, ixy_c, j, phi) = self.section.calculate_frame_properties(
-            solver_type='direct')
+            solver_type="direct"
+        )
         cx, cy = self.section.get_c()
         mass, ga = 0, 0
         for el in self.section.elements:
             (area_, _, _, _, _, _, _, g, rho) = el.geometric_properties()
             mass += area_ * rho
             ga += area_ * g
-        self.section.section_props.calculate_centroidal_properties(
-            self.section.mesh)
+        self.section.section_props.calculate_centroidal_properties(self.section.mesh)
         zxx_plus, zxx_minus, zyy_plus, zyy_minus = self.section.get_z()
         E_eff = self.section.section_props.ea / self.section.section_props.area
         G_eff = ga / self.section.section_props.area
         area = ea / Eref
         if Eref != 1.0:  # composite section
             # St. Venant torsion constant
             j = G_eff / E_eff * j / Gref
@@ -457,15 +490,15 @@
             for data in self.rebar_data:
                 rebar_xy = data["rebar_xy"]
                 dia = data["dia"]
                 rebar_coords = []
                 rebar_areas = []
                 for xy in rebar_xy:
                     rebar_coords.append(xy)
-                    rebar_areas.append(np.pi / 4 * dia ** 2)
+                    rebar_areas.append(np.pi / 4 * dia**2)
                 all_rebar_area += np.sum(rebar_areas)
             rho_rebar = all_rebar_area / area
         else:
             rho_rebar = 0
         sec_props = dict(
             A=area,
             centroid=(cx, cy),
@@ -478,43 +511,76 @@
             Wzb=zyy_minus / Eref,
             J=j,
             phi=phi,
             mass=mass,
             rho_rebar=rho_rebar,
         )
         if display_results:
-            syms = ["A", "centroid", "Iy", "Iz", "Iyz",
-                    "Wyt", "Wyb", "Wzt", "Wzb", "J", "phi", "mass", "rho_rebar"]
-            defs = ["Cross-sectional area", "Elastic centroid",
-                    "Moment of inertia y-axis", "Moment of inertia z-axis", "Product of inertia",
-                    "Section moduli of top fibres y-axis", "Section moduli of bottom fibres y-axis",
-                    "Section moduli of top fibres z-axis", "Section moduli of bottom fibres z-axis",
-                    "Torsion constant", "Principal axis angle", "Section mass", "Ratio of reinforcement"]
+            syms = [
+                "A",
+                "centroid",
+                "Iy",
+                "Iz",
+                "Iyz",
+                "Wyt",
+                "Wyb",
+                "Wzt",
+                "Wzb",
+                "J",
+                "phi",
+                "mass",
+                "rho_rebar",
+            ]
+            defs = [
+                "Cross-sectional area",
+                "Elastic centroid",
+                "Moment of inertia y-axis",
+                "Moment of inertia z-axis",
+                "Product of inertia",
+                "Section moduli of top fibres y-axis",
+                "Section moduli of bottom fibres y-axis",
+                "Section moduli of top fibres z-axis",
+                "Section moduli of bottom fibres z-axis",
+                "Torsion constant",
+                "Principal axis angle",
+                "Section mass",
+                "Ratio of reinforcement",
+            ]
             table = Table(title="Frame Section Properties")
             table.add_column("Symbol", style="cyan", no_wrap=True)
             table.add_column("Value", style="magenta")
             table.add_column("Definition", style="green")
             for sym_, def_ in zip(syms, defs):
                 if sym_ != "centroid":
                     table.add_row(sym_, f"{sec_props[sym_]:.3E}", def_)
                 else:
-                    table.add_row(sym_,
-                                  f"({sec_props[sym_][0]:.3E}, {sec_props[sym_][1]:.3E})",
-                                  def_)
+                    table.add_row(
+                        sym_,
+                        f"({sec_props[sym_][0]:.3E}, {sec_props[sym_][1]:.3E})",
+                        def_,
+                    )
             console = Console()
             console.print(table)
         self.frame_sec_props = sec_props
         return sec_props
 
-    def get_stress(self, N: float = 0, Vy: float = 0, Vz: float = 0,
-                   Myy: float = 0, Mzz: float = 0, Mxx: float = 0,
-                   plot_stress: str = None,
-                   cmap: str = 'coolwarm', normalize: bool = True):
+    def get_stress(
+        self,
+        N: float = 0,
+        Vy: float = 0,
+        Vz: float = 0,
+        Myy: float = 0,
+        Mzz: float = 0,
+        Mxx: float = 0,
+        plot_stress: str = None,
+        cmap: str = "coolwarm",
+        normalize: bool = True,
+    ):
         """Calculates the cross-section stress resulting from design actions and returns
-        a list of dictionaries containing the cross-section stresses for each region by 
+        a list of dictionaries containing the cross-section stresses for each region by
         method :py:meth:`~opstool.preprocessing.SecMesh.assign_group`.
 
         .. note::
 
             This function is only available for elastic stress analysis, and reinforcement is ignored.
 
             The stresses are realistic only if you specify the correct material for each geometry region.
@@ -581,111 +647,209 @@
         list[dict]:
             A list of dictionaries containing the cross-section stresses for each region by
             method :py:meth:`~opstool.preprocessing.SecMesh.assign_group`.
         """
         plot_stress = plot_stress.lower()
         if (not self.frame_sec_props) and (not self.sec_props):
             _ = self.get_frame_props()
-        if self.section.section_props.omega is None and (Vy != 0 or Vz != 0 or Mxx != 0):
+        if self.section.section_props.omega is None and (
+            Vy != 0 or Vz != 0 or Mxx != 0
+        ):
             _ = self.get_sec_props()
-        stress_post = self.section.calculate_stress(N=N, Vx=Vy, Vy=Vz,
-                                                    Mxx=Myy, Myy=Mzz, Mzz=Mxx)
-        name_map = dict(xx="sig_zz", xy="sig_zx", xz="sig_zy", xyz="sig_zxy",
-                        p1="sig_1", p3="sig_3", vm="sig_vm", n_xx="sig_zz_n",
-                        myy_xx="sig_zz_mxx", mzz_xx="sig_zz_myy", m_xx="sig_zz_m",
-                        mxx_xy="sig_zx_mzz", mxx_xz="sig_zy_mzz", mxx_xyz="sig_zxy_mzz",
-                        vy_xy="sig_zx_vx", vy_xz="sig_zy_vx", vy_xyz="sig_zxy_vx",
-                        vz_xy="sig_zx_vy", vz_xz="sig_zy_vy", vz_xyz="sig_zxy_vy",
-                        v_xy="sig_zx_v", v_xz="sig_zy_v", v_xyz="sig_zxy_v")
+        stress_post = self.section.calculate_stress(
+            N=N, Vx=Vy, Vy=Vz, Mxx=Myy, Myy=Mzz, Mzz=Mxx
+        )
+        name_map = dict(
+            xx="sig_zz",
+            xy="sig_zx",
+            xz="sig_zy",
+            xyz="sig_zxy",
+            p1="sig_1",
+            p3="sig_3",
+            vm="sig_vm",
+            n_xx="sig_zz_n",
+            myy_xx="sig_zz_mxx",
+            mzz_xx="sig_zz_myy",
+            m_xx="sig_zz_m",
+            mxx_xy="sig_zx_mzz",
+            mxx_xz="sig_zy_mzz",
+            mxx_xyz="sig_zxy_mzz",
+            vy_xy="sig_zx_vx",
+            vy_xz="sig_zy_vx",
+            vy_xyz="sig_zxy_vx",
+            vz_xy="sig_zx_vy",
+            vz_xz="sig_zy_vy",
+            vz_xyz="sig_zxy_vy",
+            v_xy="sig_zx_v",
+            v_xz="sig_zy_v",
+            v_xyz="sig_zxy_v",
+        )
 
         if plot_stress:
             # ------------Primary Stress Plots
             if plot_stress == "n_xx":
-                stress_post.plot_stress_n_zz(title=r'Stress Contour Plot - $\sigma_{xx,N}$',
-                                             cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_n_zz(
+                    title=r"Stress Contour Plot - $\sigma_{xx,N}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "myy_xx":
-                stress_post.plot_stress_mxx_zz(title=r'Stress Contour Plot - $\sigma_{xx,Myy}$',
-                                               cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_mxx_zz(
+                    title=r"Stress Contour Plot - $\sigma_{xx,Myy}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "mzz_xx":
-                stress_post.plot_stress_myy_zz(title=r'Stress Contour Plot - $\sigma_{xx,Mzz}$',
-                                               cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_myy_zz(
+                    title=r"Stress Contour Plot - $\sigma_{xx,Mzz}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "m_xx":
-                stress_post.plot_stress_m_zz(title=r'Stress Contour Plot - $\sigma_{xx,\Sigma M}$',
-                                             cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_m_zz(
+                    title=r"Stress Contour Plot - $\sigma_{xx,\Sigma M}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "mxx_xy":
-                stress_post.plot_stress_mzz_zx(title='Stress Contour Plot - $\\tau_{xy,Mxx}$',
-                                               cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_mzz_zx(
+                    title="Stress Contour Plot - $\\tau_{xy,Mxx}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "mxx_xz":
-                stress_post.plot_stress_mzz_zy(title='Stress Contour Plot - $\\tau_{xz,Mxx}$',
-                                               cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_mzz_zy(
+                    title="Stress Contour Plot - $\\tau_{xz,Mxx}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "mxx_xyz":
-                stress_post.plot_stress_mzz_zxy(title='Stress Contour Plot - $\\tau_{xyz,Mxx}$',
-                                                cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_mzz_zxy(
+                    title="Stress Contour Plot - $\\tau_{xyz,Mxx}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "vy_xy":
-                stress_post.plot_stress_vx_zx(title='Stress Contour Plot - $\\tau_{xy,Vy}$',
-                                              cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_vx_zx(
+                    title="Stress Contour Plot - $\\tau_{xy,Vy}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "vy_xz":
-                stress_post.plot_stress_vx_zy(title='Stress Contour Plot - $\\tau_{xz,Vy}$',
-                                              cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_vx_zy(
+                    title="Stress Contour Plot - $\\tau_{xz,Vy}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "vy_xyz":
-                stress_post.plot_stress_vx_zxy(title=r"Stress Contour Plot - $\tau_{xyz,Vy}",
-                                               cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_vx_zxy(
+                    title=r"Stress Contour Plot - $\tau_{xyz,Vy}",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "vz_xy":
-                stress_post.plot_stress_vy_zx(title='Stress Contour Plot - $\\tau_{xy,Vz}$',
-                                              cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_vy_zx(
+                    title="Stress Contour Plot - $\\tau_{xy,Vz}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "vz_xz":
-                stress_post.plot_stress_vy_zy(title='Stress Contour Plot - $\\tau_{xz,Vz}$',
-                                              cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_vy_zy(
+                    title="Stress Contour Plot - $\\tau_{xz,Vz}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "vz_xyz":
-                stress_post.plot_stress_vy_zxy(title='Stress Contour Plot - $\\tau_{xyz,Vz}$',
-                                               cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_vy_zxy(
+                    title="Stress Contour Plot - $\\tau_{xyz,Vz}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "v_xy":
-                stress_post.plot_stress_v_zx(title='Stress Contour Plot - $\\tau_{xy,V}$',
-                                             cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_v_zx(
+                    title="Stress Contour Plot - $\\tau_{xy,V}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "v_xz":
-                stress_post.plot_stress_v_zy(title='Stress Contour Plot - $\\tau_{xz,V}$',
-                                             cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_v_zy(
+                    title="Stress Contour Plot - $\\tau_{xz,V}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "v_xyz":
-                stress_post.plot_stress_v_zxy(title='Stress Contour Plot - $\\tau_{xyz,V}$',
-                                              cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_v_zxy(
+                    title="Stress Contour Plot - $\\tau_{xyz,V}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             # ------------Combined Stress Plots
             elif plot_stress == "xx":
-                stress_post.plot_stress_zz(title=r'Stress Contour Plot - $\sigma_{xx}$',
-                                           cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_zz(
+                    title=r"Stress Contour Plot - $\sigma_{xx}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "xy":
-                stress_post.plot_stress_zx(title='Stress Contour Plot - $\\tau_{xy}$',
-                                           cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_zx(
+                    title="Stress Contour Plot - $\\tau_{xy}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "xz":
-                stress_post.plot_stress_zy(title='Stress Contour Plot - $\\tau_{xz}$',
-                                           cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_zy(
+                    title="Stress Contour Plot - $\\tau_{xz}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "xyz":
-                stress_post.plot_stress_zxy(title='Stress Contour Plot - $\\tau_{xyz}$',
-                                            cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_zxy(
+                    title="Stress Contour Plot - $\\tau_{xyz}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "p1":
-                stress_post.plot_stress_1(title=r'Stress Contour Plot - $\sigma_{1}$',
-                                          cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_1(
+                    title=r"Stress Contour Plot - $\sigma_{1}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "p3":
-                stress_post.plot_stress_3(title=r'Stress Contour Plot - $\sigma_{3}$',
-                                          cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_3(
+                    title=r"Stress Contour Plot - $\sigma_{3}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "vm":
-                stress_post.plot_stress_vm(title=r'Stress Contour Plot - $\sigma_{vM}$',
-                                           cmap=cmap, normalize=normalize)
+                stress_post.plot_stress_vm(
+                    title=r"Stress Contour Plot - $\sigma_{vM}$",
+                    cmap=cmap,
+                    normalize=normalize,
+                )
             elif plot_stress == "all":
                 for name in name_map.keys():
-                    _ = self.get_stress(N=N, Vy=Vy, Vz=Vz,
-                                        Myy=Myy, Mzz=Mzz, Mxx=Mxx, plot_stress=name,
-                                        cmap=cmap, normalize=normalize)
+                    _ = self.get_stress(
+                        N=N,
+                        Vy=Vy,
+                        Vz=Vz,
+                        Myy=Myy,
+                        Mzz=Mzz,
+                        Mxx=Mxx,
+                        plot_stress=name,
+                        cmap=cmap,
+                        normalize=normalize,
+                    )
             else:
                 raise ValueError("not supported plot_stress type!")
 
         stresses_temp = stress_post.get_stress()
         stresses = []
         for stress in stresses_temp:
             temp = dict()
-            temp['Region'] = stress['Material']
+            temp["Region"] = stress["Material"]
             for name, value in name_map.items():
                 temp["sig_" + name] = stress[value]
             stresses.append(temp)
         return stresses
 
     def centring(self):
         """
@@ -717,23 +881,21 @@
         None
         """
         theta = theta / 180 * np.pi
 
         if not self.is_centring:
             self.centring()
 
-        x_rot, y_rot = sec_rotation(
-            self.points[:, 0], self.points[:, 1], theta)
+        x_rot, y_rot = sec_rotation(self.points[:, 0], self.points[:, 1], theta)
         self.points[:, 0], self.points[:, 1] = x_rot, y_rot
 
         names = self.centers_map.keys()
         for name in names:
             x_rot, y_rot = sec_rotation(
-                self.centers_map[name][:, 0],
-                self.centers_map[name][:, 1], theta
+                self.centers_map[name][:, 0], self.centers_map[name][:, 1], theta
             )
             self.centers_map[name][:, 0], self.centers_map[name][:, 1] = x_rot, y_rot
         # rebar
         for i, data in enumerate(self.rebar_data):
             rebar_xy = self.rebar_data[i]["rebar_xy"]
             x_rot, y_rot = sec_rotation(rebar_xy[:, 0], rebar_xy[:, 1], theta)
             (
@@ -766,15 +928,15 @@
                 ops.fiber(center[0], center[1], area, matTag)
         # rebars
         for data in self.rebar_data:
             rebar_xy = data["rebar_xy"]
             dia = data["dia"]
             matTag = data["matTag"]
             for xy in rebar_xy:
-                area = np.pi / 4 * dia ** 2
+                area = np.pi / 4 * dia**2
                 ops.fiber(xy[0], xy[1], area, matTag)
 
     def to_file(self, output_path: str, secTag: int, GJ: float):
         """Output the opensees fiber code to file.
 
         Parameters
         -------------
@@ -822,15 +984,15 @@
             # rebar
             for data in self.rebar_data:
                 output.write("    # Define Rebar\n")
                 rebar_xy = data["rebar_xy"]
                 dia = data["dia"]
                 mat_tag = data["matTag"]
                 for xy in rebar_xy:
-                    area = np.pi / 4 * dia ** 2
+                    area = np.pi / 4 * dia**2
                     output.write(
                         f"    fiber {xy[0]:.3E} {xy[1]:.3E} {area:.3E} {mat_tag}\n"
                     )
             output.write("};    # end of fibersection definition")
 
     def _to_py(self, output_path, names, sec_tag, gj):
         with open(output_path, "w+") as output:
@@ -851,22 +1013,26 @@
             # rebar
             for data in self.rebar_data:
                 output.write("# Define Rebar\n")
                 rebar_xy = data["rebar_xy"]
                 dia = data["dia"]
                 mat_tag = data["matTag"]
                 for xy in rebar_xy:
-                    area = np.pi / 4 * dia ** 2
+                    area = np.pi / 4 * dia**2
                     output.write(
                         f"ops.fiber({xy[0]:.3E}, {xy[1]:.3E}, {area:.3E}, {mat_tag})\n"
                     )
 
-    def view(self, fill: bool = True, engine: str = "plotly",
-             save_html: str = "SecMesh.html",
-             on_notebook: bool = False):
+    def view(
+        self,
+        fill: bool = True,
+        engine: str = "plotly",
+        save_html: str = "SecMesh.html",
+        on_notebook: bool = False,
+    ):
         """Display the section mesh.
 
         Parameters
         -----------
         fill : bool, default=True
              Whether to fill the trangles.
         engine: str, default='plotly'
@@ -890,15 +1056,16 @@
         aspect_ratio = (np.max(y) - np.min(y)) / (np.max(x) - np.min(x))
         if engine.lower().startswith("m"):
             self._plot_mpl(fill, aspect_ratio)
         elif engine.lower().startswith("p"):
             self._plot_plotly(fill, aspect_ratio, save_html, on_notebook)
         else:
             raise ValueError(
-                f"not supported engine {engine}! optional, 'plotly' or 'matplotlib'!")
+                f"not supported engine {engine}! optional, 'plotly' or 'matplotlib'!"
+            )
 
     def _plot_mpl(self, fill, aspect_ratio):
         # matplotlib plot
         fig, ax = plt.subplots(figsize=(8, 8 * aspect_ratio))
         # ax.set_facecolor("#efefef")
         # view the mesh
         vertices = self.points  # the coords of each triangle vertex
@@ -924,28 +1091,24 @@
                     patches,
                     facecolors=self.color_map[name],
                     edgecolors="k",
                     linewidths=0.25,
                     zorder=-10,
                 )
                 ax.add_collection(coll)
-                ax.plot([], [], "^", label=name,
-                        color=self.color_map[name])
+                ax.plot([], [], "^", label=name, color=self.color_map[name])
 
         for data in self.rebar_data:
             color = data["color"]
             rebar_xy = data["rebar_xy"]
             dia = data["dia"]
             rebar_coords = []
             for xy in rebar_xy:
                 rebar_coords.append(xy)
-            patches = [
-                plt.Circle((xy[0], xy[1]), dia / 2)
-                for xy in rebar_coords
-            ]
+            patches = [plt.Circle((xy[0], xy[1]), dia / 2) for xy in rebar_coords]
             coll = PatchCollection(patches, facecolors=color)
             ax.add_collection(coll)
 
         # ax.set_aspect("equal")
         ax.set_title(self.sec_name, fontsize=26, fontfamily="SimSun")
         ax.legend(
             fontsize=18,
@@ -980,80 +1143,100 @@
                 x2, y2 = points0[1, :2]
                 x3, y3 = points0[2, :2]
                 area_ = 0.5 * np.abs(
                     x2 * y3 + x1 * y2 + x3 * y1 - x3 * y2 - x2 * y1 - x1 * y3
                 )
                 areas.append(area_)
                 centers.append(np.mean(points0, axis=0))
-                points = np.vstack(
-                    [points0, [points0[0]], [[np.NAN, np.NAN]]])
+                points = np.vstack([points0, [points0[0]], [[np.NAN, np.NAN]]])
                 face_points.append(points)
             face_points = np.vstack(face_points)
             areas = np.array(areas).reshape((len(areas), 1))
             center_areas = np.hstack([centers, areas])
-            center_areas_labels = [f"<b>xo:{d[0]:.2e}</b><br>yo:{d[1]:.2e}<br>area:{d[2]:.2e}"
-                                   for d in center_areas]
+            center_areas_labels = [
+                f"<b>xo:{d[0]:.2e}</b><br>yo:{d[1]:.2e}<br>area:{d[2]:.2e}"
+                for d in center_areas
+            ]
             n_cells_map[name] = len(center_areas_labels)
             if fill:
-                tplot.append(go.Scatter(x=face_points[:, 0], y=face_points[:, 1],
-                                        fill="toself", fillcolor=self.color_map[name],
-                                        line=dict(
-                                            color='black', width=0.75),
-                                        connectgaps=False, opacity=0.75,
-                                        hoverinfo="skip", ))
+                tplot.append(
+                    go.Scatter(
+                        x=face_points[:, 0],
+                        y=face_points[:, 1],
+                        fill="toself",
+                        fillcolor=self.color_map[name],
+                        line=dict(color="black", width=0.75),
+                        connectgaps=False,
+                        opacity=0.75,
+                        hoverinfo="skip",
+                    )
+                )
             else:
-                tplot.append(go.Scatter(x=face_points[:, 0], y=face_points[:, 1],
-                                        mode='lines',
-                                        line=dict(
-                                            color=self.color_map[name], width=1.2),
-                                        connectgaps=False,
-                                        hoverinfo="skip", ))
+                tplot.append(
+                    go.Scatter(
+                        x=face_points[:, 0],
+                        y=face_points[:, 1],
+                        mode="lines",
+                        line=dict(color=self.color_map[name], width=1.2),
+                        connectgaps=False,
+                        hoverinfo="skip",
+                    )
+                )
             # hover label
             tplot.append(
                 go.Scatter(
                     x=center_areas[:, 0],
                     y=center_areas[:, 1],
-                    marker=dict(size=0, color=self.color_map[name],
-                                symbol='diamond-open'),
+                    marker=dict(
+                        size=0, color=self.color_map[name], symbol="diamond-open"
+                    ),
                     mode="markers",
                     name=label,
                     customdata=center_areas_labels,
-                    hovertemplate='%{customdata}',
+                    hovertemplate="%{customdata}",
                 )
             )
         fig.add_traces(tplot)
         # rebars
         shapes = []
         for data in self.rebar_data:
             color = data["color"]
             rebar_xy = data["rebar_xy"]
             r = data["dia"] / 2
             for xo, yo in rebar_xy:
-                shapes.append(dict(type="circle",
-                                   xref="x", yref="y",
-                                   x0=xo - r, y0=yo - r, x1=xo + r, y1=yo + r,
-                                   line_color=color,
-                                   fillcolor=color,
-                                   ))
+                shapes.append(
+                    dict(
+                        type="circle",
+                        xref="x",
+                        yref="y",
+                        x0=xo - r,
+                        y0=yo - r,
+                        x1=xo + r,
+                        y1=yo + r,
+                        line_color=color,
+                        fillcolor=color,
+                    )
+                )
         # -------------------------------------
         txt = "Num. of Mesh: "
         for k, v in n_cells_map.items():
             txt += f"| {k}--{v} "
         txt += f"| total--{n_cells}"
         fig.update_layout(
             shapes=shapes,
             width=900,
             height=900 * aspect_ratio,
             template="plotly",
             autosize=True,
             showlegend=False,
-            scene=dict(aspectratio=dict(
-                x=1, y=aspect_ratio), aspectmode="data"),
-            title=dict(font=dict(family="courier", color='black', size=16),
-                       text=f"<b>{self.sec_name}</b> <br>" + f"{txt}")
+            scene=dict(aspectratio=dict(x=1, y=aspect_ratio), aspectmode="data"),
+            title=dict(
+                font=dict(family="courier", color="black", size=16),
+                text=f"<b>{self.sec_name}</b> <br>" + f"{txt}",
+            ),
         )
         fig.update_xaxes(tickfont_size=18, ticks="outside")
         fig.update_yaxes(tickfont_size=18, ticks="outside")
         if save_html:
             pio.write_html(fig, file=save_html, auto_open=True)
         if on_notebook:
             fig.show()
@@ -1064,23 +1247,23 @@
     A class to create the rebar point.
     """
 
     def __init__(self) -> None:
         self.rebar_data = []
 
     def add_rebar_line(
-            self,
-            points: list,
-            dia: float,
-            gap: float = 0.1,
-            n: int = None,
-            closure: bool = False,
-            matTag: int = None,
-            color: str = "black",
-            group_name: str = None,
+        self,
+        points: list,
+        dia: float,
+        gap: float = 0.1,
+        n: int = None,
+        closure: bool = False,
+        matTag: int = None,
+        color: str = "black",
+        group_name: str = None,
     ):
         """Add rebar along a line, can be a line or polygon.
 
         Parameters
         ----------
         points: list[list[float, float]]
             A list of rebar coords, [(x1, y1), (x2, y2),...,(xn, yn)]
@@ -1118,25 +1301,25 @@
         rebar_xy = _lines_subdivide(x, y, gap)
         data = dict(
             rebar_xy=rebar_xy, color=color, name=group_name, dia=dia, matTag=matTag
         )
         self.rebar_data.append(data)
 
     def add_rebar_circle(
-            self,
-            xo: list,
-            radius: float,
-            dia: float,
-            gap: float = 0.1,
-            n: int = None,
-            angle1: float = 0.0,
-            angle2: float = 360,
-            matTag: int = None,
-            color: str = "black",
-            group_name: str = None,
+        self,
+        xo: list,
+        radius: float,
+        dia: float,
+        gap: float = 0.1,
+        n: int = None,
+        angle1: float = 0.0,
+        angle2: float = 360,
+        matTag: int = None,
+        color: str = "black",
+        group_name: str = None,
     ):
         """Add the rebars along a circle.
 
         Parameters
         ----------
         xo: list[float, float]
             Center coords of circle, [(xc, yc)].
@@ -1194,25 +1377,25 @@
         Returns
         -------
         list[int]
             The number of rebars in each layer.
         """
         nums = []
         for data in self.rebar_data:
-            nums.append(len(data['rebar_xy']))
+            nums.append(len(data["rebar_xy"]))
         return nums
 
 
 def add_material(
-        name="default",
-        elastic_modulus=1,
-        poissons_ratio=0,
-        yield_strength=1,
-        density=1,
-        color="w",
+    name="default",
+    elastic_modulus=1,
+    poissons_ratio=0,
+    yield_strength=1,
+    density=1,
+    color="w",
 ):
     """Add a meterial.
 
     Parameters
     ----------
     name : str, default='default'
         meterial name.
@@ -1238,17 +1421,17 @@
         yield_strength=yield_strength,
         density=density,
         color=color,
     )
 
 
 def add_polygon(
-        outline: list,
-        holes: list = None,
-        material=None,
+    outline: list,
+    holes: list = None,
+    material=None,
 ):
     """Add polygon plane geom obj.
 
     Parameters
     ----------
     outline : list[list[float, float]]
         The coords list of polygon points, [(x1, y1), (x2, y2),...,(xn, yn)]
@@ -1268,21 +1451,21 @@
         material_ = material
     ply = Polygon(outline, holes)
     geometry = Geometry(geom=ply, material=material_)
     return geometry
 
 
 def add_circle(
-        xo: list,
-        radius: float,
-        holes=None,
-        angle1=0.0,
-        angle2=360,
-        n_sub=40,
-        material=None,
+    xo: list,
+    radius: float,
+    holes=None,
+    angle1=0.0,
+    angle2=360,
+    n_sub=40,
+    material=None,
 ):
     """Add the circle geom obj.
 
     Parameters
     ----------
     xo : list[float, float]
         Center coords, [(xc, yc)].
@@ -1308,16 +1491,15 @@
         material_ = None
     else:
         material_ = material
     angle1 = angle1 / 180 * np.pi
     angle2 = angle2 / 180 * np.pi
     x, y = xo[0], xo[1]
     angles = np.linspace(angle1, angle2, n_sub + 1)
-    points = [[x + radius * np.cos(ang), y + radius * np.sin(ang)]
-              for ang in angles]
+    points = [[x + radius * np.cos(ang), y + radius * np.sin(ang)] for ang in angles]
     ply = Polygon(points, holes)
     geometry = Geometry(geom=ply, material=material_)
     return geometry
 
 
 def _lines_subdivide(x, y, gap):
     """
```

### Comparing `opstool-0.7.3/src/opstool/preprocessing/section/var_sec_mesh.py` & `opstool-0.8.0/src/opstool/preprocessing/section/var_sec_mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from __future__ import annotations
 
 import re
 
 import numpy as np
 import pyvista as pv
+
 # from sectionproperties.pre.geometry import Geometry
 from shapely import LineString
 
 pv.set_plot_theme("document")
 
 
-def var_line_string(pointsi: list,
-                    pointsj: list,
-                    path: list, n_sec: float = 2,
-                    loc_sec: list | None = None,
-                    closure: bool = False,
-                    y_degree: int = 1, y_sym_plane: str = "j-0",
-                    z_degree: int = 2, z_sym_plane: str = "j-0"):
+def var_line_string(
+    pointsi: list,
+    pointsj: list,
+    path: list,
+    n_sec: float = 2,
+    loc_sec: list | None = None,
+    closure: bool = False,
+    y_degree: int = 1,
+    y_sym_plane: str = "j-0",
+    z_degree: int = 2,
+    z_sym_plane: str = "j-0",
+):
     """Returns the varied line string.
 
     Parameters
     ----------
     pointsi : list[list[float, float]]
         I end line points.
     pointsj : list[list[float, float]]
@@ -69,26 +75,33 @@
     linesj = LineString(pointsj)
     yi, zi = linesi.xy
     yj, zj = linesj.xy
     cum_points = []
     for x in cum_length:
         points_ = []
         for i in range(len(yi)):
-            y = _get_coord(0, yi[i], length, yj[i], x,
-                           degree=y_degree, sym_plane=y_sym_plane)
-            z = _get_coord(0, zi[i], length, zj[i], x,
-                           degree=z_degree, sym_plane=z_sym_plane)
+            y = _get_coord(
+                0, yi[i], length, yj[i], x, degree=y_degree, sym_plane=y_sym_plane
+            )
+            z = _get_coord(
+                0, zi[i], length, zj[i], x, degree=z_degree, sym_plane=z_sym_plane
+            )
             points_.append((y, z))
         cum_points.append(points_)
     return cum_points
 
 
-def vis_var_sec(sec_meshes: list, path: list,
-                n_sec: float = 2, loc_sec: list | None = None,
-                on_notebook: bool = False, show_outline: bool = True):
+def vis_var_sec(
+    sec_meshes: list,
+    path: list,
+    n_sec: float = 2,
+    loc_sec: list | None = None,
+    on_notebook: bool = False,
+    show_outline: bool = True,
+):
     """Visualize varied section meshes.
 
     .. warning::
         Please carefully check your section local axes.
         For visualization purposes, this function defaults to using vecxz=[-1,0,0] for vertical elements
         and vecxz=[0,0,1] for non-vertical ones.
 
@@ -111,56 +124,58 @@
     show_outline: bool, optional, by default False
         If True, display bound outline.
     """
     _, _, cum_coord = _get_path_len(path, n_sec, loc_sec)
     plotter = pv.Plotter(notebook=on_notebook)
     cum_coord = np.array(cum_coord, dtype=np.float32)
     point_plot1 = pv.PolyData(cum_coord)
-    plotter.add_mesh(point_plot1, color='black',
-                     point_size=5, render_points_as_spheres=True)
+    plotter.add_mesh(
+        point_plot1, color="black", point_size=5, render_points_as_spheres=True
+    )
     path = np.array(path, dtype=np.float32)
     point_plot2 = pv.PolyData(path)
-    plotter.add_mesh(point_plot2, color='#8f1402',
-                     point_size=10, render_points_as_spheres=True)
+    plotter.add_mesh(
+        point_plot2, color="#8f1402", point_size=10, render_points_as_spheres=True
+    )
     line_cells = []
     for i in range(len(path) - 1):
         line_cells.extend([2, i, i + 1])
 
     line_plot = _generate_mesh(path, line_cells, kind="line")
     plotter.add_mesh(
         line_plot,
-        color='black',
+        color="black",
         render_lines_as_tubes=False,
         line_width=2,
     )
     local_axes = _get_path_local_axes(path, n_sec, loc_sec)
     for i in range(len(sec_meshes)):
         sec_mesh = sec_meshes[i]
         center0 = cum_coord[i]
         _, vecy, vecz = local_axes[i]
         if not sec_mesh.is_centring:
             sec_mesh.centring()
         points = sec_mesh.points
-        points = (points[:, 0].reshape((-1, 1)) @ np.reshape(vecy, (1, 3)) +
-                  points[:, 1].reshape((-1, 1)) @ np.reshape(vecz, (1, 3)))
+        points = points[:, 0].reshape((-1, 1)) @ np.reshape(vecy, (1, 3)) + points[
+            :, 1
+        ].reshape((-1, 1)) @ np.reshape(vecz, (1, 3))
         points += center0
         for name, faces in sec_mesh.cells_map.items():
             faces = np.insert(faces, 0, values=3, axis=1)
-            face_plot = _generate_mesh(
-                points, faces, kind="face"
-            )
+            face_plot = _generate_mesh(points, faces, kind="face")
             plotter.add_mesh(
                 face_plot, color=sec_mesh.color_map[name], show_edges=True, opacity=1
             )
         for rdata in sec_mesh.rebar_data:
             color = rdata["color"]
             r = rdata["dia"] / 2
             rebar_xy = np.array(rdata["rebar_xy"])
-            rebar_xy = (rebar_xy[:, 0].reshape((-1, 1)) @ np.reshape(vecy, (1, 3)) +
-                        rebar_xy[:, 1].reshape((-1, 1)) @ np.reshape(vecz, (1, 3)))
+            rebar_xy = rebar_xy[:, 0].reshape((-1, 1)) @ np.reshape(
+                vecy, (1, 3)
+            ) + rebar_xy[:, 1].reshape((-1, 1)) @ np.reshape(vecz, (1, 3))
             rebar_xy += center0
             spheres = []
             for coord in rebar_xy:
                 spheres.append(pv.Sphere(radius=r, center=coord))
             merged = pv.MultiBlock(spheres)
             plotter.add_mesh(merged, color=color)
     if show_outline:
@@ -222,24 +237,24 @@
 
 
 def _get_coord(x1, y1, x2, y2, x, degree=1, sym_plane="j-0"):
     if degree == 1:
         y = y1 + (y2 - y1) * (x - x1) / (x2 - x1)
     elif degree == 2:
         d = float(re.findall(r"\d+\.?\d*", sym_plane)[0])
-        if sym_plane[0].lower() == 'j':
-            a = (y2 - y1) / (x2 ** 2 - x1 ** 2 - 2 * (x2 + d) * (x2 - x1))
+        if sym_plane[0].lower() == "j":
+            a = (y2 - y1) / (x2**2 - x1**2 - 2 * (x2 + d) * (x2 - x1))
             b = -2 * a * (x2 + d)
-            c = y1 - a * x1 ** 2 - b * x1
-            y = a * x ** 2 + b * x + c
-        elif sym_plane[0].lower() == 'i':
-            a = (y2 - y1) / (x2 ** 2 - x1 ** 2 - 2 * (x1 - d) * (x2 - x1))
+            c = y1 - a * x1**2 - b * x1
+            y = a * x**2 + b * x + c
+        elif sym_plane[0].lower() == "i":
+            a = (y2 - y1) / (x2**2 - x1**2 - 2 * (x1 - d) * (x2 - x1))
             b = -2 * a * (x1 - d)
-            c = y1 - a * x1 ** 2 - b * x1
-            y = a * x ** 2 + b * x + c
+            c = y1 - a * x1**2 - b * x1
+            y = a * x**2 + b * x + c
         else:
             raise ValueError(f"Error arg sym_plane={sym_plane}!")
     else:
         raise ValueError("Currently only support degree=1 or 2!")
     return y
 
 
@@ -419,14 +434,15 @@
         xi[6] = 0.433395394129247
         xi[7] = 0.679409568299024
         xi[8] = 0.865063366688985
         xi[9] = 0.973906528517172
     loc = 0.5 * (xi + 1.0)
     return loc
 
+
 # class VarSecMesh:
 #     """A class for generating meshes with variable fiber cross-sections.
 
 #     Parameters
 #     ----------
 #     meshi : Instance of the class ``SecMesh``.
 #         I end section.
```

### Comparing `opstool-0.7.3/src/opstool/preprocessing/tcl2py.py` & `opstool-0.8.0/src/opstool/preprocessing/tcl2py.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.3/src/opstool/preprocessing/unit_system.py` & `opstool-0.8.0/src/opstool/preprocessing/unit_system.py`

 * *Files identical despite different names*

### Comparing `opstool-0.7.3/src/opstool/vis/_get_model_base.py` & `opstool-0.8.0/src/opstool/vis/_get_model_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import numpy as np
 import openseespy.opensees as ops
 import triangle as tr
 
 from ..preprocessing.section.sec_mesh import SecMesh
-from ..utils import (ELE_TAG_PFEM, ELE_TAG_Beam, ELE_TAG_Brick, ELE_TAG_Link,
-                     ELE_TAG_Plane, ELE_TAG_Tetrahedron, ELE_TAG_Truss)
+from ..utils import (
+    ELE_TAG_PFEM,
+    ELE_TAG_Beam,
+    ELE_TAG_Brick,
+    ELE_TAG_Link,
+    ELE_TAG_Plane,
+    ELE_TAG_Tetrahedron,
+    ELE_TAG_Truss,
+)
 
 
 def get_node_coords():
     node_tags = ops.getNodeTags()
     num_node = len(node_tags)
     node_coords = np.zeros((num_node, 3))
     node_index = dict()  # key: nodeTag, value: index in Node_Coords
@@ -38,27 +45,78 @@
             fixities[dof - 1] = -1
         fixed_dofs.append(fixities)
     fixed_coords = np.array(fixed_coords)
     fixed_dofs = np.array(fixed_dofs)
     return fixed_nodes, fixed_coords, fixed_dofs
 
 
+def get_node_load(node_index):
+    patterns = ops.getPatterns()
+    info = []
+    data = []
+    for pattern in patterns:
+        nodetags = ops.getNodeLoadTags(pattern)
+        loaddata = ops.getNodeLoadData(pattern)
+        data.extend(loaddata)
+        for tag in nodetags:
+            ndm = ops.getNDM(tag)[0]
+            ndf = ops.getNDF(tag)[0]
+            idx = node_index[tag]
+            info.append([pattern, tag, ndm, ndf, idx])
+    return info, data
+
+
+def get_ele_load(node_index):
+    patterns = ops.getPatterns()
+    info = []
+    data = []
+    beam_local = []
+    for pattern in patterns:
+        eletags = ops.getEleLoadTags(pattern)
+        eleclasstags = ops.getEleLoadClassTags(pattern)
+        loaddata = ops.getEleLoadData(pattern)
+        data.extend(loaddata)
+        for tag, classtag in zip(eletags, eleclasstags):
+            ntags = ops.eleNodes(tag)
+            idx1, idx2 = node_index[ntags[0]], node_index[ntags[1]]
+            info.append([pattern, tag, classtag, idx1, idx2])
+            xlocal = ops.eleResponse(tag, "xaxis")
+            ylocal = ops.eleResponse(tag, "yaxis")
+            zlocal = ops.eleResponse(tag, "zaxis")
+            if xlocal:
+                beam_local.extend(np.array(xlocal) / np.linalg.norm(xlocal))
+            else:
+                beam_local.extend(np.array([0.0, 0.0, 0.0]))
+            if ylocal:
+                beam_local.extend(np.array(ylocal) / np.linalg.norm(ylocal))
+            else:
+                beam_local.extend(np.array([0.0, 0.0, 0.0]))
+            if zlocal:
+                beam_local.extend(np.array(zlocal) / np.linalg.norm(zlocal))
+            else:
+                beam_local.extend(np.array([0.0, 0.0, 0.0]))
+    info = np.array(info)
+    beam_local = np.reshape(beam_local, (-1, 9))
+    return info, data, beam_local
+
+
 def get_mp_constraint(node_coords, node_index):
     retained_nodes = ops.getRetainedNodes()
     points = []
     midpoints = []
     cells = []
     dofs = []
     for i, tag in enumerate(retained_nodes):
         constrained_nodes = ops.getConstrainedNodes(tag)
         for tag2 in constrained_nodes:
             points.append(node_coords[node_index[tag]])
             points.append(node_coords[node_index[tag2]])
             midpoints.append(
-                (node_coords[node_index[tag]] + node_coords[node_index[tag2]]) / 2)
+                (node_coords[node_index[tag]] + node_coords[node_index[tag2]]) / 2
+            )
             cells.extend([2, 2 * i, 2 * i + 1])
             dof = ops.getRetainedDOFs(tag, tag2)
             dofs.append(dof)
     if dofs:
         max_dof_dim = np.max([len(dof) for dof in dofs])
         new_dofs = []
         for dof in dofs:
@@ -94,40 +152,47 @@
     for i, ele in enumerate(ele_tags):
         ele_nodes = ops.eleNodes(ele)
         if len(ele_nodes) == 2 and ops.getEleClassTags(ele)[0] in ELE_TAG_Link:
             node_i, node_j = ele_nodes
             idx_i, idx_j = node_index[node_i], node_index[node_j]
             link_cells.extend([2, idx_i, idx_j])
             link_cells_tags.append(ele)
-            link_midpoints.append(
-                (node_coords[idx_i] + node_coords[idx_j]) / 2)
+            link_midpoints.append((node_coords[idx_i] + node_coords[idx_j]) / 2)
             link_lengths.append(
-                np.sqrt(np.sum((node_coords[idx_i] - node_coords[idx_j]) ** 2)))
+                np.sqrt(np.sum((node_coords[idx_i] - node_coords[idx_j]) ** 2))
+            )
             xlocal = ops.eleResponse(ele, "xaxis")
             ylocal = ops.eleResponse(ele, "yaxis")
             zlocal = ops.eleResponse(ele, "zaxis")
             if xlocal:
                 link_xlocal.append(np.array(xlocal) / np.linalg.norm(xlocal))
             else:
-                link_xlocal.append(np.array([0., 0., 0.]))
+                link_xlocal.append(np.array([0.0, 0.0, 0.0]))
             if ylocal:
                 link_ylocal.append(np.array(ylocal) / np.linalg.norm(ylocal))
             else:
-                link_ylocal.append(np.array([0., 0., 0.]))
+                link_ylocal.append(np.array([0.0, 0.0, 0.0]))
             if zlocal:
                 link_zlocal.append(np.array(zlocal) / np.linalg.norm(zlocal))
             else:
-                link_zlocal.append(np.array([0., 0., 0.]))
+                link_zlocal.append(np.array([0.0, 0.0, 0.0]))
     link_midpoints = np.array(link_midpoints)
     link_lengths = np.array(link_lengths)
     link_xlocal = np.array(link_xlocal)
     link_ylocal = np.array(link_ylocal)
     link_zlocal = np.array(link_zlocal)
-    return (link_cells, link_cells_tags, link_midpoints, link_lengths,
-            link_xlocal, link_ylocal, link_zlocal)
+    return (
+        link_cells,
+        link_cells_tags,
+        link_midpoints,
+        link_lengths,
+        link_xlocal,
+        link_ylocal,
+        link_zlocal,
+    )
 
 
 def get_beam_info(ele_tags, node_coords, node_index):
     beam_cells = []
     beam_cells_tags = []
     beam_midpoints = []
     beam_lengths = []
@@ -137,40 +202,47 @@
     for i, ele in enumerate(ele_tags):
         ele_nodes = ops.eleNodes(ele)
         if len(ele_nodes) == 2 and ops.getEleClassTags(ele)[0] in ELE_TAG_Beam:
             node_i, node_j = ele_nodes
             idx_i, idx_j = node_index[node_i], node_index[node_j]
             beam_cells.extend([2, idx_i, idx_j])
             beam_cells_tags.append(ele)
-            beam_midpoints.append(
-                (node_coords[idx_i] + node_coords[idx_j]) / 2)
+            beam_midpoints.append((node_coords[idx_i] + node_coords[idx_j]) / 2)
             beam_lengths.append(
-                np.sqrt(np.sum((node_coords[idx_i] - node_coords[idx_j]) ** 2)))
+                np.sqrt(np.sum((node_coords[idx_i] - node_coords[idx_j]) ** 2))
+            )
             xlocal = ops.eleResponse(ele, "xaxis")
             ylocal = ops.eleResponse(ele, "yaxis")
             zlocal = ops.eleResponse(ele, "zaxis")
             if xlocal:
                 beam_xlocal.append(np.array(xlocal) / np.linalg.norm(xlocal))
             else:
-                beam_xlocal.append(np.array([0., 0., 0.]))
-            if xlocal:
+                beam_xlocal.append(np.array([0.0, 0.0, 0.0]))
+            if ylocal:
                 beam_ylocal.append(np.array(ylocal) / np.linalg.norm(ylocal))
             else:
-                beam_ylocal.append(np.array([0., 0., 0.]))
+                beam_ylocal.append(np.array([0.0, 0.0, 0.0]))
             if zlocal:
                 beam_zlocal.append(np.array(zlocal) / np.linalg.norm(zlocal))
             else:
-                beam_zlocal.append(np.array([0., 0., 0.]))
+                beam_zlocal.append(np.array([0.0, 0.0, 0.0]))
     beam_midpoints = np.array(beam_midpoints)
     beam_lengths = np.array(beam_lengths)
     beam_xlocal = np.array(beam_xlocal)
     beam_ylocal = np.array(beam_ylocal)
     beam_zlocal = np.array(beam_zlocal)
-    return (beam_cells, beam_cells_tags, beam_midpoints, beam_lengths,
-            beam_xlocal, beam_ylocal, beam_zlocal)
+    return (
+        beam_cells,
+        beam_cells_tags,
+        beam_midpoints,
+        beam_lengths,
+        beam_xlocal,
+        beam_ylocal,
+        beam_zlocal,
+    )
 
 
 def get_beam_sec_info(sec_mesh: dict, node_coords, node_index):
     if not sec_mesh:
         return [], [], [], [], [], []
     for ele, mesh in sec_mesh.items():
         if not isinstance(mesh, SecMesh):
@@ -180,38 +252,62 @@
     for ele_tag, mesh in sec_mesh.items():
         ele_nodes = ops.eleNodes(ele_tag)
         node_i, node_j = ele_nodes
         idx_i, idx_j = node_index[node_i], node_index[node_j]
         coord_i, coord_j = node_coords[idx_i], node_coords[idx_j]
         ylocal = ops.eleResponse(ele_tag, "yaxis")
         zlocal = ops.eleResponse(ele_tag, "zaxis")
-        ylocal = np.array(ylocal) / np.linalg.norm(ylocal) if ylocal else np.array([0., 0., 0.])
-        zlocal = np.array(zlocal) / np.linalg.norm(zlocal) if zlocal else np.array([0., 0., 0.])
+        ylocal = (
+            np.array(ylocal) / np.linalg.norm(ylocal)
+            if ylocal
+            else np.array([0.0, 0.0, 0.0])
+        )
+        zlocal = (
+            np.array(zlocal) / np.linalg.norm(zlocal)
+            if zlocal
+            else np.array([0.0, 0.0, 0.0])
+        )
         for name in mesh.group_map.keys():
             geom = mesh.group_map[name].geom
             extp = np.array(geom.exterior.coords)
             extp -= np.array(mesh.center)
-            points = (extp[:, 0].reshape((-1, 1)) @ np.reshape(ylocal, (1, 3)) +
-                      extp[:, 1].reshape((-1, 1)) @ np.reshape(zlocal, (1, 3)))
+            points = extp[:, 0].reshape((-1, 1)) @ np.reshape(ylocal, (1, 3)) + extp[
+                :, 1
+            ].reshape((-1, 1)) @ np.reshape(zlocal, (1, 3))
             extpi, extpj = points + coord_i, points + coord_j
             nps = extp.shape[0]
             for i in range(nps - 1):
-                ext_cells.extend([4, len(ext_points) + i, len(ext_points) + i + nps,
-                                  len(ext_points) + i + nps + 1, len(ext_points) + i + 1])
+                ext_cells.extend(
+                    [
+                        4,
+                        len(ext_points) + i,
+                        len(ext_points) + i + nps,
+                        len(ext_points) + i + nps + 1,
+                        len(ext_points) + i + 1,
+                    ]
+                )
             ext_points.extend(list(np.vstack([extpi, extpj])))
             for intp_ in geom.interiors:
                 intp = np.array(intp_.coords)
                 intp -= mesh.center
-                points = (intp[:, 0].reshape((-1, 1)) @ np.reshape(ylocal, (1, 3)) +
-                          intp[:, 1].reshape((-1, 1)) @ np.reshape(zlocal, (1, 3)))
+                points = intp[:, 0].reshape((-1, 1)) @ np.reshape(
+                    ylocal, (1, 3)
+                ) + intp[:, 1].reshape((-1, 1)) @ np.reshape(zlocal, (1, 3))
                 intpi, intpj = points + coord_i, points + coord_j
                 nps = intp.shape[0]
                 for i in range(nps - 1):
-                    int_cells.extend([4, len(int_points) + i, len(int_points) + i + nps,
-                                      len(int_points) + i + nps + 1, len(int_points) + i + 1])
+                    int_cells.extend(
+                        [
+                            4,
+                            len(int_points) + i,
+                            len(int_points) + i + nps,
+                            len(int_points) + i + nps + 1,
+                            len(int_points) + i + 1,
+                        ]
+                    )
                 int_points.extend(list(np.vstack([intpi, intpj])))
             # sec mesh
             pts, seg, holes = [], [], []
             for i, p in enumerate(extp):
                 pts.append(p)
                 if i < len(extp) - 1:
                     seg.append([i, i + 1])
@@ -224,27 +320,35 @@
                         seg.append([len(pts), len(pts) + 1])
                     pts.append(p)
             pts, seg = np.array(pts), np.array(seg)
             if holes:
                 A = dict(vertices=pts, segments=seg, holes=holes)
             else:
                 A = dict(vertices=pts, segments=seg)
-            B = tr.triangulate(A, 'qpa1000000000')
-            vertices = B['vertices']
-            points = (vertices[:, 0].reshape((-1, 1)) @ np.reshape(ylocal, (1, 3)) +
-                      vertices[:, 1].reshape((-1, 1)) @ np.reshape(zlocal, (1, 3)))
+            B = tr.triangulate(A, "qpa1000000000")
+            vertices = B["vertices"]
+            points = vertices[:, 0].reshape((-1, 1)) @ np.reshape(
+                ylocal, (1, 3)
+            ) + vertices[:, 1].reshape((-1, 1)) @ np.reshape(zlocal, (1, 3))
             secpi, secpj = points + coord_i, points + coord_j
-            cells = B['triangles']
-            cells = np.vstack([len(sec_points) + cells, cells + len(vertices) + len(sec_points)])
+            cells = B["triangles"]
+            cells = np.vstack(
+                [len(sec_points) + cells, cells + len(vertices) + len(sec_points)]
+            )
             cells = np.insert(cells, 0, np.zeros(cells.shape[0]) + 3, axis=1)
             sec_points.extend(list(np.vstack([secpi, secpj])))
             sec_cells.append(cells)
-    return (np.array(ext_points), np.array(ext_cells),
-            np.array(int_points), np.array(int_cells),
-            np.array(sec_points), np.vstack(sec_cells))
+    return (
+        np.array(ext_points),
+        np.array(ext_cells),
+        np.array(int_points),
+        np.array(int_cells),
+        np.array(sec_points),
+        np.vstack(sec_cells),
+    )
 
 
 def get_other_line_info(ele_tags, node_index):
     other_line_cells = []
     other_line_cells_tags = []
     for i, ele in enumerate(ele_tags):
         ele_nodes = ops.eleNodes(ele)
@@ -278,54 +382,71 @@
         ele_nodes = ops.eleNodes(ele)
         class_tag = ops.getEleClassTags(ele)[0]
         if class_tag in ELE_TAG_Plane:
             if len(ele_nodes) in [6, 7]:
                 if class_tag in ELE_TAG_PFEM:
                     ele_nodes = [ele_nodes[1], ele_nodes[3], ele_nodes[5]]
                 else:
-                    ele_nodes = [ele_nodes[0], ele_nodes[3], ele_nodes[1],
-                                 ele_nodes[4], ele_nodes[2], ele_nodes[5]]
+                    ele_nodes = [
+                        ele_nodes[0],
+                        ele_nodes[3],
+                        ele_nodes[1],
+                        ele_nodes[4],
+                        ele_nodes[2],
+                        ele_nodes[5],
+                    ]
             elif len(ele_nodes) in [8, 9]:
-                ele_nodes = [ele_nodes[0], ele_nodes[4], ele_nodes[1], ele_nodes[5],
-                             ele_nodes[2], ele_nodes[6], ele_nodes[3], ele_nodes[7]]
+                ele_nodes = [
+                    ele_nodes[0],
+                    ele_nodes[4],
+                    ele_nodes[1],
+                    ele_nodes[5],
+                    ele_nodes[2],
+                    ele_nodes[6],
+                    ele_nodes[3],
+                    ele_nodes[7],
+                ]
             idxs = [node_index[tag_] for tag_ in ele_nodes]
             plane_cells.extend([len(idxs)] + idxs)
             plane_cells_tags.append(ele)
     return plane_cells, plane_cells_tags
 
 
 def get_tet_info(ele_tags, node_index):
     tetrahedron_cells = []
     tetrahedron_cells_tags = []
     for i, ele in enumerate(ele_tags):
         ele_nodes = ops.eleNodes(ele)
         class_tag = ops.getEleClassTags(ele)[0]
         if class_tag in ELE_TAG_Tetrahedron:  # tetrahedron
             if len(ele_nodes) == 8:  # FEMBubble 3D
-                ele_nodes = [ele_nodes[1], ele_nodes[3],
-                             ele_nodes[5], ele_nodes[7]]
+                ele_nodes = [ele_nodes[1], ele_nodes[3], ele_nodes[5], ele_nodes[7]]
             if len(ele_nodes) == 4:
                 node_i, node_j, node_k, node_l = ele_nodes
                 idx_i, idx_j = node_index[node_i], node_index[node_j]
                 idx_k, idx_l = node_index[node_k], node_index[node_l]
                 tetrahedron_cells.extend([3, idx_i, idx_j, idx_k])
                 tetrahedron_cells.extend([3, idx_i, idx_j, idx_l])
                 tetrahedron_cells.extend([3, idx_i, idx_k, idx_l])
                 tetrahedron_cells.extend([3, idx_j, idx_k, idx_l])
                 tetrahedron_cells_tags.append(ele)
             elif len(ele_nodes) == 10:
                 idxs = [node_index[tag_] for tag_ in ele_nodes]
                 tetrahedron_cells.extend(
-                    [6, idxs[0], idxs[4], idxs[1], idxs[5], idxs[2], idxs[6]])
+                    [6, idxs[0], idxs[4], idxs[1], idxs[5], idxs[2], idxs[6]]
+                )
                 tetrahedron_cells.extend(
-                    [6, idxs[0], idxs[4], idxs[1], idxs[8], idxs[3], idxs[7]])
+                    [6, idxs[0], idxs[4], idxs[1], idxs[8], idxs[3], idxs[7]]
+                )
                 tetrahedron_cells.extend(
-                    [6, idxs[2], idxs[5], idxs[1], idxs[8], idxs[3], idxs[9]])
+                    [6, idxs[2], idxs[5], idxs[1], idxs[8], idxs[3], idxs[9]]
+                )
                 tetrahedron_cells.extend(
-                    [6, idxs[2], idxs[6], idxs[0], idxs[7], idxs[3], idxs[9]])
+                    [6, idxs[2], idxs[6], idxs[0], idxs[7], idxs[3], idxs[9]]
+                )
                 tetrahedron_cells_tags.append(ele)
     return tetrahedron_cells, tetrahedron_cells_tags
 
 
 def get_bri_info(ele_tags, node_index):
     brick_cells = []
     brick_cells_tags = []
@@ -344,25 +465,31 @@
                 brick_cells.extend([4, idx3, idx4, idx8, idx7])
                 brick_cells_tags.append(ele)
             elif len(ele_nodes) == 20:
                 idx1, idx2, idx3, idx4, idx5, idx6, idx7 = idxs[:7]
                 idx8, idx9, idx10, idx11, idx12, idx13, idx14 = idxs[7:14]
                 idx15, idx16, idx17, idx18, idx19, idx20 = idxs[14:]
                 brick_cells.extend(
-                    [8, idx1, idx9, idx2, idx10, idx3, idx11, idx4, idx12])
+                    [8, idx1, idx9, idx2, idx10, idx3, idx11, idx4, idx12]
+                )
                 brick_cells.extend(
-                    [8, idx5, idx13, idx6, idx14, idx7, idx15, idx8, idx16])
+                    [8, idx5, idx13, idx6, idx14, idx7, idx15, idx8, idx16]
+                )
                 brick_cells.extend(
-                    [8, idx5, idx13, idx6, idx18, idx2, idx9, idx1, idx17])
+                    [8, idx5, idx13, idx6, idx18, idx2, idx9, idx1, idx17]
+                )
                 brick_cells.extend(
-                    [8, idx7, idx15, idx8, idx20, idx4, idx11, idx3, idx19])
+                    [8, idx7, idx15, idx8, idx20, idx4, idx11, idx3, idx19]
+                )
                 brick_cells.extend(
-                    [8, idx1, idx17, idx5, idx16, idx8, idx20, idx4, idx12])
+                    [8, idx1, idx17, idx5, idx16, idx8, idx20, idx4, idx12]
+                )
                 brick_cells.extend(
-                    [8, idx2, idx18, idx6, idx14, idx7, idx19, idx3, idx10])
+                    [8, idx2, idx18, idx6, idx14, idx7, idx19, idx3, idx10]
+                )
                 brick_cells_tags.append(ele)
     return brick_cells, brick_cells_tags
 
 
 # def get_all_face_info(ele_tags, node_coords, node_index):
 #     pass
 
@@ -375,15 +502,15 @@
         ele_midpoints.append(np.mean(node_coords[idxs], axis=0))
     return np.array(ele_midpoints)
 
 
 def get_bounds(node_coords):
     min_node = np.min(node_coords, axis=0)
     max_node = np.max(node_coords, axis=0)
-    space = (max_node - min_node) / 5
+    space = (max_node - min_node) / 12
     min_node = min_node - space
     max_node = max_node + space
     bounds = [
         min_node[0],
         max_node[0],
         min_node[1],
         max_node[1],
@@ -394,39 +521,58 @@
     min_bound = np.min(max_node - min_node)
     return bounds, max_bound, min_bound
 
 
 def get_model_info(sec_mesh: dict):
     # print(ops.constrainedDOFs())   constrainedDOFs
     node_coords, node_index, model_dims, node_tags = get_node_coords()
-    fixed_nodes, fixed_coords, fixed_dofs = get_node_fix(
-        node_coords, node_index)
+    fixed_nodes, fixed_coords, fixed_dofs = get_node_fix(node_coords, node_index)
     ctra_coords, ctra_midcoords, ctra_dofs, ctra_cells = get_mp_constraint(
-        node_coords, node_index)
+        node_coords, node_index
+    )
     ele_tags = ops.getEleTags()
     num_ele = len(ele_tags)
     truss_cells, truss_cells_tags = get_truss_info(ele_tags, node_index)
-    (link_cells, link_cells_tags, link_midpoints, link_lengths,
-     link_xlocal, link_ylocal, link_zlocal) = get_link_info(ele_tags, node_coords, node_index)
-    (beam_cells, beam_cells_tags, beam_midpoints, beam_lengths,
-     beam_xlocal, beam_ylocal, beam_zlocal) = get_beam_info(ele_tags, node_coords, node_index)
-    (ext_points, ext_cells, int_points,
-     int_cells, sec_points, sec_cells) = get_beam_sec_info(sec_mesh, node_coords, node_index)
-    other_line_cells, other_line_cells_tags = get_other_line_info(
-        ele_tags, node_index)
-    all_lines_cells, all_lines_cells_tags = get_all_line_info(
-        ele_tags, node_index)
+    (
+        link_cells,
+        link_cells_tags,
+        link_midpoints,
+        link_lengths,
+        link_xlocal,
+        link_ylocal,
+        link_zlocal,
+    ) = get_link_info(ele_tags, node_coords, node_index)
+    (
+        beam_cells,
+        beam_cells_tags,
+        beam_midpoints,
+        beam_lengths,
+        beam_xlocal,
+        beam_ylocal,
+        beam_zlocal,
+    ) = get_beam_info(ele_tags, node_coords, node_index)
+    (
+        ext_points,
+        ext_cells,
+        int_points,
+        int_cells,
+        sec_points,
+        sec_cells,
+    ) = get_beam_sec_info(sec_mesh, node_coords, node_index)
+    other_line_cells, other_line_cells_tags = get_other_line_info(ele_tags, node_index)
+    all_lines_cells, all_lines_cells_tags = get_all_line_info(ele_tags, node_index)
     plane_cells, plane_cells_tags = get_plane_info(ele_tags, node_index)
-    tetrahedron_cells, tetrahedron_cells_tags = get_tet_info(
-        ele_tags, node_index)
+    tetrahedron_cells, tetrahedron_cells_tags = get_tet_info(ele_tags, node_index)
     brick_cells, brick_cells_tags = get_bri_info(ele_tags, node_index)
     all_faces_cells = plane_cells + tetrahedron_cells + brick_cells
     all_faces_cells_tags = plane_cells_tags + tetrahedron_cells_tags + brick_cells_tags
     ele_midpoints = get_ele_mid(ele_tags, node_coords, node_index)
     bounds, max_bound, min_bound = get_bounds(node_coords)
+    node_load_info, node_load_data = get_node_load(node_index)
+    ele_load_info, ele_load_data, ele_load_locals = get_ele_load(node_index)
     model_info = dict()
     model_info["coord_no_deform"] = node_coords
     model_info["coord_ele_midpoints"] = ele_midpoints
     model_info["bound"] = bounds
     model_info["max_bound"] = max_bound
     model_info["min_bound"] = min_bound
     model_info["num_ele"] = num_ele
@@ -451,17 +597,22 @@
     model_info["line_sec_int_points"] = int_points
     model_info["line_sec_points"] = sec_points
     model_info["link_midpoints"] = link_midpoints
     model_info["link_lengths"] = link_lengths
     model_info["link_xlocal"] = link_xlocal
     model_info["link_ylocal"] = link_ylocal
     model_info["link_zlocal"] = link_zlocal
+    model_info["node_load_info"] = node_load_info
+    model_info["node_load_data"] = node_load_data
+    model_info["ele_load_info"] = ele_load_info
+    model_info["ele_load_data"] = ele_load_data
+    model_info["ele_load_locals"] = ele_load_locals
     cells = dict()
     cells["all_lines"] = all_lines_cells
-    cells['all_lines_tags'] = all_lines_cells_tags
+    cells["all_lines_tags"] = all_lines_cells_tags
     cells["all_faces"] = all_faces_cells
     cells["all_faces_tags"] = all_faces_cells_tags
     cells["plane"] = plane_cells
     cells["plane_tags"] = plane_cells_tags
     cells["tetrahedron"] = tetrahedron_cells
     cells["tetrahedron_tags"] = tetrahedron_cells_tags
     cells["brick"] = brick_cells
@@ -587,16 +738,28 @@
 
 
 def get_beam_resp(beam_tags):
     beam_resp_steps = []
     for eletag in beam_tags:
         local_forces = ops.eleResponse(eletag, "localForce")
         if len(local_forces) == 6:
-            local_forces = [local_forces[0], local_forces[1], 0, 0, 0, local_forces[2],
-                            local_forces[3], local_forces[4], 0, 0, 0, local_forces[5]]
+            local_forces = [
+                local_forces[0],
+                local_forces[1],
+                0,
+                0,
+                0,
+                local_forces[2],
+                local_forces[3],
+                local_forces[4],
+                0,
+                0,
+                0,
+                local_forces[5],
+            ]
         # for ii in range(6):
         #     local_forces[ii] = -local_forces[ii]
         beam_resp_steps.append(local_forces)
     beam_resp_steps = np.array(beam_resp_steps)
     return beam_resp_steps
 
 
@@ -604,16 +767,15 @@
     """
     Sort points counterclockwise
     """
     x0 = np.mean(x)
     y0 = np.mean(y)
     r = np.sqrt((x - x0) ** 2 + (y - y0) ** 2)
     angles = np.where(
-        (y - y0) >= 0, np.arccos((x - x0) / r),
-        4 * np.pi - np.arccos((x - x0) / r)
+        (y - y0) >= 0, np.arccos((x - x0) / r), 4 * np.pi - np.arccos((x - x0) / r)
     )
     mask = np.argsort(angles)
     x_max = np.max(x)
     if x[mask][0] != x_max:
         mask = np.roll(mask, 1)
     return mask
```

### Comparing `opstool-0.7.3/src/opstool/vis/_plotly_base.py` & `opstool-0.8.0/src/opstool/vis/_plotly_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import warnings
 
 import h5py
 import numpy as np
+import matplotlib.pyplot as plt
 import plotly.graph_objs as go
 import plotly.io as pio
 from plotly.subplots import make_subplots
+from matplotlib.colors import to_hex
 
 from ..utils import shape_dict
 
 
 def _make_faces(points, cells):
     face_line_points = []
     face_points = []
@@ -66,16 +68,15 @@
             vecj.append(len(face_points) + 5)
             veck.append(len(face_points) + 7)
         face_line_points.extend(list(data))
         face_points.extend(list(data0))
     face_line_points = np.array(face_line_points)
     face_points = np.array(face_points)
     face_mid_points = np.array(face_mid_points)
-    return (face_points, face_line_points, face_mid_points,
-            veci, vecj, veck)
+    return (face_points, face_line_points, face_mid_points, veci, vecj, veck)
 
 
 def _make_lines(points, cells):
     line_points = []
     line_mid_points = []
     for cell in cells:
         data0 = points[cell[1:], :]
@@ -84,169 +85,222 @@
         line_points.extend(list(data))
         line_mid_points.append(np.mean(data0, axis=0))
     line_points = np.array(line_points)
     line_mid_points = np.array(line_mid_points)
     return line_points, line_mid_points
 
 
-def _make_fix_node(model_info):
-    fixed_dofs = model_info["FixNodeDofs"]
-    fixed_coords = model_info["FixNodeCoords"]
-    beam_lengths = model_info["beam_lengths"]
-    if len(beam_lengths) > 0:
-        s = (np.max(beam_lengths) + np.min(beam_lengths)) / 20
-    else:
-        s = (model_info["max_bound"] + model_info["min_bound"]) / 100
-    points = []
-    for coord, dof in zip(fixed_coords, fixed_dofs):
-        x, y, z = coord
-        if dof[0] == -1:
-            points.extend([[x, y - s / 2, z], [x, y + s / 2, z],
-                           [x, y + s / 2, z - s], [x, y - s / 2, z - s],
-                           [x, y - s / 2, z], [np.NAN, np.NAN, np.NAN]])
-        if dof[1] == -1:
-            points.extend([[x - s / 2, y, z], [x + s / 2, y, z],
-                           [x + s / 2, y, z - s], [x - s / 2, y, z - s],
-                           [x - s / 2, y, z], [np.NAN, np.NAN, np.NAN]])
-        if dof[2] == -1:
-            points.extend([[x - s / 2, y - s / 2, z - s / 2], [x + s / 2, y - s / 2, z - s / 2],
-                           [x + s / 2, y + s / 2, z - s / 2], [x -
-                                                               s / 2, y + s / 2, z - s / 2],
-                           [x - s / 2, y - s / 2, z - s / 2], [np.NAN, np.NAN, np.NAN]])
-    points = np.array(points)
-    return points
-
-
 def _model_vis(
-        obj,
-        input_file: str = "ModelData.hdf5",
-        show_node_label: bool = False,
-        show_ele_label: bool = False,
-        show_local_crd: bool = False,
-        show_fix_node: bool = True,
-        show_constrain_dof: bool = False,
-        label_size: float = 8,
-        show_outline: bool = True,
-        opacity: float = 1.0,
-        save_html: str = 'ModelVis.html'
+    obj,
+    input_file: str = "ModelData.hdf5",
+    show_node_label: bool = False,
+    show_ele_label: bool = False,
+    show_local_crd: bool = False,
+    local_crd_alpha: float = 1.0,
+    show_fix_node: bool = True,
+    fix_node_alpha: float = 1.0,
+    show_load: bool = False,
+    load_alpha: float = 1.0,
+    show_constrain_dof: bool = False,
+    label_size: float = 8,
+    show_outline: bool = True,
+    opacity: float = 1.0,
+    save_html: str = "ModelVis.html",
 ):
     # read hdf5 file
     # -------------------------------------------
-    filename = obj.out_dir + '/' + input_file
+    filename = obj.out_dir + "/" + input_file
     model_info = dict()
     cells = dict()
     with h5py.File(filename, "r") as f:
         grp1 = f["ModelInfo"]
         for name in grp1.keys():
             model_info[name] = grp1[name][...]
         grp2 = f["Cell"]
         for name in grp2.keys():
             cells[name] = grp2[name][...]
     for name, value in cells.items():
         if "_tags" not in name:
             cells[name] = _reshape_cell(value)
-    fig = _plot_model(obj, model_info, cells,
-                      show_node_label=show_node_label,
-                      show_ele_label=show_ele_label,
-                      show_local_crd=show_local_crd,
-                      show_fix_node=show_fix_node,
-                      show_constrain_dof=show_constrain_dof,
-                      label_size=label_size,
-                      show_outline=show_outline,
-                      opacity=opacity)
+    fig = _plot_model(
+        obj,
+        model_info,
+        cells,
+        show_node_label=show_node_label,
+        show_ele_label=show_ele_label,
+        show_local_crd=show_local_crd,
+        local_crd_alpha=local_crd_alpha,
+        show_fix_node=show_fix_node,
+        fix_node_alpha=fix_node_alpha,
+        show_load=show_load,
+        load_alpha=load_alpha,
+        show_constrain_dof=show_constrain_dof,
+        label_size=label_size,
+        show_outline=show_outline,
+        opacity=opacity,
+    )
     if save_html:
         if not save_html.endswith(".html"):
             save_html += ".html"
         pio.write_html(fig, file=save_html, auto_open=True)
-    if obj.notebook:
-        fig.show()
+    return fig
 
 
-def _plot_model(obj, model_info, cells,
-                show_node_label: bool = False,
-                show_ele_label: bool = False,
-                show_local_crd: bool = False,
-                show_fix_node: bool = True,
-                show_constrain_dof: bool = False,
-                label_size: float = 8,
-                show_outline: bool = True,
-                opacity: float = 1.0, ):
+def _plot_model(
+    obj,
+    model_info,
+    cells,
+    show_node_label: bool = False,
+    show_ele_label: bool = False,
+    show_local_crd: bool = False,
+    local_crd_alpha: float = 1.0,
+    show_fix_node: bool = True,
+    fix_node_alpha: float = 1.0,
+    show_load: bool = False,
+    load_alpha: float = 1.0,
+    show_constrain_dof: bool = False,
+    label_size: float = 8,
+    show_outline: bool = True,
+    opacity: float = 1.0,
+):
     fig = go.Figure()
     plotter = []
     points_no_deform = model_info["coord_no_deform"]
     # >>> face plot
     face_cells = [cells["plane"], cells["tetrahedron"], cells["brick"]]
-    face_cells_tags = [cells["plane_tags"],
-                       cells["tetrahedron_tags"], cells["brick_tags"]]
+    face_cells_tags = [
+        cells["plane_tags"],
+        cells["tetrahedron_tags"],
+        cells["brick_tags"],
+    ]
     face_colors = [obj.color_face, obj.color_solid, obj.color_solid]
     names = ["plane", "tetrahedron", "brick"]
     for ii in range(len(face_cells)):
         if len(face_cells[ii]) > 0:
-            (face_points, face_line_points, face_mid_points,
-             veci, vecj, veck) = _make_faces(points_no_deform, face_cells[ii])
+            (
+                face_points,
+                face_line_points,
+                face_mid_points,
+                veci,
+                vecj,
+                veck,
+            ) = _make_faces(points_no_deform, face_cells[ii])
             x, y, z = face_points[:, 0], face_points[:, 1], face_points[:, 2]
-            plotter.append(go.Mesh3d(x=x, y=y, z=z, i=veci, j=vecj, k=veck,
-                                     name=names[ii], color=face_colors[ii],
-                                     opacity=opacity, hoverinfo="skip"))
+            plotter.append(
+                go.Mesh3d(
+                    x=x,
+                    y=y,
+                    z=z,
+                    i=veci,
+                    j=vecj,
+                    k=veck,
+                    name=names[ii],
+                    color=face_colors[ii],
+                    opacity=opacity,
+                    hoverinfo="skip",
+                )
+            )
             x, y, z = [face_line_points[:, j] for j in range(3)]
-            plotter.append(go.Scatter3d(x=x, y=y, z=z,
-                                        line=dict(color="black",
-                                                  width=obj.line_width / 2),
-                                        mode="lines", name=names[ii],
-                                        connectgaps=False, hoverinfo="skip"))
+            plotter.append(
+                go.Scatter3d(
+                    x=x,
+                    y=y,
+                    z=z,
+                    line=dict(color="black", width=obj.line_width / 2),
+                    mode="lines",
+                    name=names[ii],
+                    connectgaps=False,
+                    hoverinfo="skip",
+                )
+            )
             x, y, z = [face_mid_points[:, j] for j in range(3)]
             labels_ = [f"tag: {kk}" for kk in face_cells_tags[ii]]  # hover label
             plotter.append(
-                go.Scatter3d(x=x, y=y, z=z,
-                             marker=dict(size=obj.point_size, color=face_colors[ii],
-                                         symbol='circle-open'),
-                             mode="markers", name=names[ii],
-                             hovertemplate='<b>%{text}</b>', text=labels_, ))
+                go.Scatter3d(
+                    x=x,
+                    y=y,
+                    z=z,
+                    marker=dict(
+                        size=obj.point_size, color=face_colors[ii], symbol="circle-open"
+                    ),
+                    mode="markers",
+                    name=names[ii],
+                    hovertemplate="<b>%{text}</b>",
+                    text=labels_,
+                )
+            )
     # >>> line plot
-    line_cells = [cells["truss"], cells["link"],
-                  cells["beam"], cells["other_line"]]
-    line_cells_tags = [cells["truss_tags"], cells["link_tags"],
-                       cells["beam_tags"], cells["other_line_tags"]]
-    line_colors = [obj.color_truss, obj.color_link,
-                   obj.color_line, obj.color_line]
-    line_widths = [obj.line_width, 0.5 * obj.line_width,
-                   obj.line_width, obj.line_width]
+    line_cells = [cells["truss"], cells["link"], cells["beam"], cells["other_line"]]
+    line_cells_tags = [
+        cells["truss_tags"],
+        cells["link_tags"],
+        cells["beam_tags"],
+        cells["other_line_tags"],
+    ]
+    line_colors = [obj.color_truss, obj.color_link, obj.color_line, obj.color_line]
+    line_widths = [obj.line_width, 0.5 * obj.line_width, obj.line_width, obj.line_width]
     names = ["truss", "link", "beam", "other_line"]
     for i in range(len(line_cells)):
         if len(line_cells[i]) > 0:
-            line_points, line_mid_points = _make_lines(
-                points_no_deform, line_cells[i])
+            line_points, line_mid_points = _make_lines(points_no_deform, line_cells[i])
             x, y, z = line_points[:, 0], line_points[:, 1], line_points[:, 2]
-            plotter.append(go.Scatter3d(x=x, y=y, z=z,
-                                        line=dict(
-                                            color=line_colors[i], width=line_widths[i]),
-                                        mode="lines", name=names[i],
-                                        connectgaps=False, hoverinfo="skip"))
+            plotter.append(
+                go.Scatter3d(
+                    x=x,
+                    y=y,
+                    z=z,
+                    line=dict(color=line_colors[i], width=line_widths[i]),
+                    mode="lines",
+                    name=names[i],
+                    connectgaps=False,
+                    hoverinfo="skip",
+                )
+            )
             x, y, z = [line_mid_points[:, j] for j in range(3)]
             labels_ = [f"tag: {kk}" for kk in line_cells_tags[i]]  # hover label
-            plotter.append(go.Scatter3d(x=x, y=y, z=z,
-                                        marker=dict(size=obj.point_size, color=line_colors[i],
-                                                    symbol='circle-open'),
-                                        mode="markers", name=names[i],
-                                        hovertemplate='<b>%{text}</b>',
-                                        text=labels_, ))
+            plotter.append(
+                go.Scatter3d(
+                    x=x,
+                    y=y,
+                    z=z,
+                    marker=dict(
+                        size=obj.point_size, color=line_colors[i], symbol="circle-open"
+                    ),
+                    mode="markers",
+                    name=names[i],
+                    hovertemplate="<b>%{text}</b>",
+                    text=labels_,
+                )
+            )
     # point plot
     node_labels = [str(i) for i in model_info["NodeTags"]]
     x, y, z = [points_no_deform[:, j] for j in range(3)]
-    plotter.append(go.Scatter3d(x=x, y=y, z=z,
-                                marker=dict(size=obj.point_size,
-                                            color=obj.color_point),
-                                mode="markers", name="Node", customdata=node_labels,
-                                hovertemplate='<b>x: %{x}</b><br>y: %{y}<br>z: %{z} <br>tag: %{customdata}'))
+    plotter.append(
+        go.Scatter3d(
+            x=x,
+            y=y,
+            z=z,
+            marker=dict(size=obj.point_size, color=obj.color_point),
+            mode="markers",
+            name="Node",
+            customdata=node_labels,
+            hovertemplate="<b>x: %{x}</b><br>y: %{y}<br>z: %{z} <br>tag: %{customdata}",
+        )
+    )
 
     if show_node_label:
-        txt_plot = go.Scatter3d(x=x, y=y, z=z, text=node_labels,
-                                textfont=dict(color="#6e750e",
-                                              size=label_size),
-                                mode="text", name="Node Label")
+        txt_plot = go.Scatter3d(
+            x=x,
+            y=y,
+            z=z,
+            text=node_labels,
+            textfont=dict(color="#6e750e", size=label_size),
+            mode="text",
+            name="Node Label",
+        )
         plotter.append(txt_plot)
 
     if show_ele_label:
         ele_labels = [str(i) for i in model_info["EleTags"]]
         txt_plot = go.Scatter3d(
             x=model_info["coord_ele_midpoints"][:, 0],
             y=model_info["coord_ele_midpoints"][:, 1],
@@ -255,430 +309,791 @@
             textfont=dict(color="#650021", size=label_size),
             mode="text",
             name="Ele Label",
         )
         plotter.append(txt_plot)
 
     if show_fix_node:
-        fix_points = _make_fix_node(model_info)
+        fix_points = _make_fix_node(model_info, fix_node_alpha)
         if len(fix_points) > 0:
             x, y, z = fix_points[:, 0], fix_points[:, 1], fix_points[:, 2]
-            fix_plot = go.Scatter3d(x=x, y=y, z=z,
-                                    line=dict(color="#01ff07", width=2),
-                                    mode="lines", connectgaps=False, hoverinfo="skip")
+            fix_plot = go.Scatter3d(
+                x=x,
+                y=y,
+                z=z,
+                line=dict(color="#01ff07", width=2),
+                mode="lines",
+                connectgaps=False,
+                hoverinfo="skip",
+            )
             plotter.append(fix_plot)
         else:
             warnings.warn("Model has no fix nodes!")
 
     # local axes
     if show_local_crd:
-        beam_midpoints = model_info["beam_midpoints"]
-        beam_lengths = model_info["beam_lengths"]
-        if len(beam_midpoints) > 0:
-            beam_xlocal = model_info["beam_xlocal"]
-            beam_ylocal = model_info["beam_ylocal"]
-            beam_zlocal = model_info["beam_zlocal"]
-            length = (np.max(beam_lengths) + np.min(beam_lengths)) / 20
-            xcoords = beam_midpoints + length * beam_xlocal
-            ycoords = beam_midpoints + length * beam_ylocal
-            zcoords = beam_midpoints + length * beam_zlocal
-            localx_points = []
-            localy_points = []
-            localz_points = []
-            for i, midpoints in enumerate(beam_midpoints):
-                localx_points.append(midpoints)
-                localx_points.append(xcoords[i])
-                localx_points.append([np.NAN, np.NAN, np.NAN])
-                localy_points.append(midpoints)
-                localy_points.append(ycoords[i])
-                localy_points.append([np.NAN, np.NAN, np.NAN])
-                localz_points.append(midpoints)
-                localz_points.append(zcoords[i])
-                localz_points.append([np.NAN, np.NAN, np.NAN])
-            localx_points = np.array(localx_points)
-            localy_points = np.array(localy_points)
-            localz_points = np.array(localz_points)
-            plotter1 = go.Scatter3d(
-                x=localx_points[:, 0],
-                y=localx_points[:, 1],
-                z=localx_points[:, 2],
-                line=dict(color="#cf6275", width=obj.line_width * 1.5),
-                mode="lines",
-                connectgaps=False,
-                name='',
-                # customdata=['x'] * n_beam,
-                hovertemplate='<b>x</b>')
-            plotter2 = go.Scatter3d(
-                x=localy_points[:, 0],
-                y=localy_points[:, 1],
-                z=localy_points[:, 2],
-                line=dict(color="#04d8b2", width=obj.line_width * 1.5),
-                mode="lines",
-                connectgaps=False,
-                name='',
-                hovertemplate='<b>y</b>')
-            plotter3 = go.Scatter3d(
-                x=localz_points[:, 0],
-                y=localz_points[:, 1],
-                z=localz_points[:, 2],
-                line=dict(color="#9aae07", width=obj.line_width * 1.5),
-                mode="lines",
-                connectgaps=False,
-                name='',
-                hovertemplate='<b>z</b>')
-            plotter.extend([plotter1, plotter2, plotter3])
-        else:
-            warnings.warn(
-                "Model has no frame elements when show_local_crd=True!")
-        # link axes
-        link_midpoints = model_info["link_midpoints"]
-        link_lengths = model_info["link_lengths"]
-        if len(link_midpoints) > 0:
-            link_xlocal = model_info["link_xlocal"]
-            link_ylocal = model_info["link_ylocal"]
-            link_zlocal = model_info["link_zlocal"]
-            length = (np.max(link_lengths) + np.min(link_lengths)) / 6
-            xcoords = link_midpoints + length * link_xlocal
-            ycoords = link_midpoints + length * link_ylocal
-            zcoords = link_midpoints + length * link_zlocal
-            localx_points = []
-            localy_points = []
-            localz_points = []
-            for i, midpoints in enumerate(link_midpoints):
-                localx_points.append(midpoints)
-                localx_points.append(xcoords[i])
-                localx_points.append([np.NAN, np.NAN, np.NAN])
-                localy_points.append(midpoints)
-                localy_points.append(ycoords[i])
-                localy_points.append([np.NAN, np.NAN, np.NAN])
-                localz_points.append(midpoints)
-                localz_points.append(zcoords[i])
-                localz_points.append([np.NAN, np.NAN, np.NAN])
-            localx_points = np.array(localx_points)
-            localy_points = np.array(localy_points)
-            localz_points = np.array(localz_points)
-            plotter1 = go.Scatter3d(
-                x=localx_points[:, 0],
-                y=localx_points[:, 1],
-                z=localx_points[:, 2],
-                line=dict(color="#cf6275", width=obj.line_width * 1.5),
-                mode="lines",
-                connectgaps=False,
-                name='',
-                # customdata=['x'] * n_beam,
-                hovertemplate='<b>x</b>')
-            plotter2 = go.Scatter3d(
-                x=localy_points[:, 0],
-                y=localy_points[:, 1],
-                z=localy_points[:, 2],
-                line=dict(color="#04d8b2", width=obj.line_width * 1.5),
-                mode="lines",
-                connectgaps=False,
-                name='',
-                hovertemplate='<b>y</b>')
-            plotter3 = go.Scatter3d(
-                x=localz_points[:, 0],
-                y=localz_points[:, 1],
-                z=localz_points[:, 2],
-                line=dict(color="#9aae07", width=obj.line_width * 1.5),
-                mode="lines",
-                connectgaps=False,
-                name='',
-                hovertemplate='<b>z</b>')
-            plotter.extend([plotter1, plotter2, plotter3])
+        _show_local_axes(obj, plotter, model_info, local_crd_alpha)
     # mp constraint lines
     _show_mp_constraint(obj, plotter, model_info, show_constrain_dof)
-
+    if show_load:
+        _show_node_load(obj, plotter, model_info, load_alpha)
+        _show_ele_load(obj, plotter, model_info, load_alpha)
     fig.add_traces(plotter)
-
-    if np.max(np.abs(points_no_deform[:, -1])) < 1e-6:
-        eye = dict(x=0., y=-0.1, z=10)  # for 2D camera
-        scene = dict(camera=dict(
-            eye=eye, projection=dict(type="orthographic")))
+    if np.max(np.abs(points_no_deform[:, -1])) < 1e-10:
+        eye = dict(x=0.0, y=-0.1, z=10)  # for 2D camera
+        scene = dict(camera=dict(eye=eye, projection=dict(type="orthographic")))
     else:
         eye = dict(x=-3.5, y=-3.5, z=3.5)  # for 3D camera
-        scene = dict(aspectratio=dict(x=1, y=1, z=1), aspectmode="data",
-                     camera=dict(eye=eye, projection=dict(type="orthographic")))
+        scene = dict(
+            aspectratio=dict(x=1, y=1, z=1),
+            aspectmode="data",
+            camera=dict(eye=eye, projection=dict(type="orthographic")),
+        )
 
     fig.update_layout(
         template=obj.theme,
         autosize=True,
         showlegend=False,
         scene=scene,
-        title=dict(font=dict(family="courier", color='black', size=25),
-                   text=("<b>OpenSeesPy 3D View</b> <br>"
-                         f"Num. of Node: {model_info['num_node']} || Num. of Ele:{model_info['num_ele']}")
-                   )
+        title=dict(
+            font=dict(family="courier", color="black", size=25),
+            text=(
+                "<b>OpenSeesPy 3D View</b> <br>"
+                f"Num. of Node: {model_info['num_node']} || Num. of Ele:{model_info['num_ele']}"
+            ),
+        ),
     )
     if not show_outline:
         fig.update_layout(
-            scene=dict(xaxis={'showgrid': False, 'zeroline': False, 'visible': False},
-                       yaxis={'showgrid': False,
-                              'zeroline': False, 'visible': False},
-                       zaxis={'showgrid': False, 'zeroline': False, 'visible': False}, ),
+            scene=dict(
+                xaxis={"showgrid": False, "zeroline": False, "visible": False},
+                yaxis={"showgrid": False, "zeroline": False, "visible": False},
+                zaxis={"showgrid": False, "zeroline": False, "visible": False},
+            ),
         )
     return fig
 
 
+def _make_fix_node(model_info, alpha=1.0):
+    fixed_dofs = model_info["FixNodeDofs"]
+    fixed_coords = model_info["FixNodeCoords"]
+    beam_lengths = model_info["beam_lengths"]
+    D2 = True if np.max(model_info["model_dims"]) <= 2 else False
+    if len(beam_lengths) > 0:
+        s = np.mean(beam_lengths) / 10 * alpha
+    else:
+        s = (model_info["max_bound"] + model_info["min_bound"]) / 150 * alpha
+    points = []
+    for coord, dof in zip(fixed_coords, fixed_dofs):
+        x, y, z = coord
+        if D2:
+            z += s / 2
+            y -= s / 2
+        if dof[0] == -1:
+            points.extend(
+                [
+                    [x, y - s / 2, z],
+                    [x, y + s / 2, z],
+                    [x, y + s / 2, z - s],
+                    [x, y - s / 2, z - s],
+                    [x, y - s / 2, z],
+                    [np.NAN, np.NAN, np.NAN],
+                ]
+            )
+        if dof[1] == -1:
+            points.extend(
+                [
+                    [x - s / 2, y, z],
+                    [x + s / 2, y, z],
+                    [x + s / 2, y, z - s],
+                    [x - s / 2, y, z - s],
+                    [x - s / 2, y, z],
+                    [np.NAN, np.NAN, np.NAN],
+                ]
+            )
+        if dof[2] == -1:
+            points.extend(
+                [
+                    [x - s / 2, y - s / 2, z - s / 2],
+                    [x + s / 2, y - s / 2, z - s / 2],
+                    [x + s / 2, y + s / 2, z - s / 2],
+                    [x - s / 2, y + s / 2, z - s / 2],
+                    [x - s / 2, y - s / 2, z - s / 2],
+                    [np.NAN, np.NAN, np.NAN],
+                ]
+            )
+    points = np.array(points)
+    return points
+
+
+def _show_local_axes(obj, plotter, model_info, alpha: float = 1.0):
+    beam_midpoints = model_info["beam_midpoints"]
+    beam_lengths = model_info["beam_lengths"]
+    if len(beam_lengths) > 0:
+        xaxis = model_info["beam_xlocal"]
+        yaxis = model_info["beam_ylocal"]
+        zaxis = model_info["beam_zlocal"]
+        lengths = [np.mean(beam_lengths) / 5 * alpha] * len(beam_lengths)
+        arrow_heights = [0.4 * ll for ll in lengths]
+        arrow_widths = [0.8 * h for h in arrow_heights]
+        plotter.extend(
+            _make_lines_arrows(
+                beam_midpoints,
+                lengths,
+                xaxis,
+                yaxis,
+                zaxis,
+                "#cf6275",
+                "Local Axis",
+                ["x"] * len(beam_midpoints),
+                obj.line_width * 1.5,
+                arrow_heights,
+                arrow_widths,
+            )
+        )
+        plotter.extend(
+            _make_lines_arrows(
+                beam_midpoints,
+                lengths,
+                yaxis,
+                xaxis,
+                zaxis,
+                "#04d8b2",
+                "Local Axis",
+                ["y"] * len(beam_midpoints),
+                obj.line_width * 1.5,
+                arrow_heights,
+                arrow_widths,
+            )
+        )
+        plotter.extend(
+            _make_lines_arrows(
+                beam_midpoints,
+                lengths,
+                zaxis,
+                xaxis,
+                yaxis,
+                "#9aae07",
+                "Local Axis",
+                ["z"] * len(beam_midpoints),
+                obj.line_width * 1.5,
+                arrow_heights,
+                arrow_widths,
+            )
+        )
+
+    else:
+        warnings.warn("Model has no frame elements when show_local_crd=True!")
+    link_midpoints = model_info["link_midpoints"]
+    link_lengths = model_info["link_lengths"]
+    if len(link_midpoints) > 0:
+        xaxis = model_info["link_xlocal"]
+        yaxis = model_info["link_ylocal"]
+        zaxis = model_info["link_zlocal"]
+        lengths = [np.mean(link_lengths) / 3 * alpha] * len(link_midpoints)
+        arrow_heights = [0.4 * ll for ll in lengths]
+        arrow_widths = [0.8 * h for h in arrow_heights]
+        plotter.extend(
+            _make_lines_arrows(
+                link_midpoints,
+                lengths,
+                xaxis,
+                yaxis,
+                zaxis,
+                "#cf6275",
+                "Local Axis",
+                ["x"] * len(link_midpoints),
+                obj.line_width,
+                arrow_heights,
+                arrow_widths,
+            )
+        )
+        plotter.extend(
+            _make_lines_arrows(
+                link_midpoints,
+                lengths,
+                yaxis,
+                xaxis,
+                zaxis,
+                "#04d8b2",
+                "Local Axis",
+                ["y"] * len(link_midpoints),
+                obj.line_width,
+                arrow_heights,
+                arrow_widths,
+            )
+        )
+        plotter.extend(
+            _make_lines_arrows(
+                link_midpoints,
+                lengths,
+                zaxis,
+                xaxis,
+                yaxis,
+                "#9aae07",
+                "Local Axis",
+                ["z"] * len(link_midpoints),
+                obj.line_width,
+                arrow_heights,
+                arrow_widths,
+            )
+        )
+
+
+def _make_lines_arrows(
+    starts,
+    lengths,
+    xaxis,
+    yaxis,
+    zaxis,
+    color,
+    name,
+    hovers,
+    lw,
+    arrow_height,
+    arrow_width,
+):
+    coords = np.zeros_like(starts)
+    for i, midpoint in enumerate(starts):
+        coords[i] = midpoint + lengths[i] * xaxis[i]
+    local_points = []
+    labels = []
+    for i, midpoint in enumerate(starts):
+        local_points.append(midpoint)
+        local_points.append(coords[i])
+        local_points.append([np.NaN, np.NaN, np.NaN])
+        labels.extend([hovers[i]] * 3)
+    local_points = np.array(local_points)
+    line = go.Scatter3d(
+        x=local_points[:, 0],
+        y=local_points[:, 1],
+        z=local_points[:, 2],
+        line=dict(color=color, width=lw),
+        mode="lines",
+        connectgaps=False,
+        name=name,
+        hovertemplate="<b>%{text}</b>",
+        text=labels,
+        # hoverinfo="skip",
+    )
+    # arrows
+    angles = np.linspace(0, 2 * np.pi, 10)
+    num = len(starts)
+    points = []
+    ijk = []
+    labels = []
+    for i in range(num):
+        xs = (0.5 * arrow_width[i] * np.cos(angles)).reshape((-1, 1))
+        ys = (0.5 * arrow_width[i] * np.sin(angles)).reshape((-1, 1))
+        cen, ax, ay, az = coords[i], xaxis[i], yaxis[i], zaxis[i]
+        tips = cen + arrow_height[i] * ax
+        secs = xs @ np.reshape(ay, (1, 3)) + ys @ np.reshape(az, (1, 3))
+        secs += cen
+        for j in range(len(secs) - 1):
+            ijk.append([len(points) + j, len(points) + j + 1, len(points) + len(secs)])
+            ijk.append(
+                [len(points) + j, len(points) + j + 1, len(points) + len(secs) + 1]
+            )
+        ijk.append([len(points) + len(secs) - 1, len(points), len(points) + len(secs)])
+        ijk.append(
+            [len(points) + len(secs) - 1, len(points), len(points) + len(secs) + 1]
+        )
+        points.extend(np.vstack([secs, cen, tips]))
+        labels.extend([hovers[i]] * (len(secs) + 2))
+    points = np.array(points)
+    ijk = np.array(ijk)
+    arrow = go.Mesh3d(
+        x=points[:, 0],
+        y=points[:, 1],
+        z=points[:, 2],
+        i=ijk[:, 0],
+        j=ijk[:, 1],
+        k=ijk[:, 2],
+        color=color,
+        name=name,
+        text=labels,
+        hovertemplate="<b>%{text}",
+    )
+    return line, arrow
+
+
+def _show_node_load(obj, plotter, model_info, alpha: float = 1.0):
+    points = model_info["coord_no_deform"]
+    node_load_info = np.array(model_info["node_load_info"])
+    node_load_data = np.array(model_info["node_load_data"])
+    if len(node_load_info) == 0:
+        return None
+    loc, load_data = 0, []
+    for info in node_load_info:
+        ndm = info[2]
+        ndf = info[3]
+        data = node_load_data[loc : loc + ndf]
+        if ndm <= 2 and ndf <= 3:
+            load_data.append([data[0], data[1], 0])  # x, y
+        else:
+            load_data.append([data[0], data[1], data[2]])  # x, y, z
+        loc += ndf
+    load_data = np.array(load_data)
+    maxdata = np.max(np.abs(load_data))
+    beam_lengths = model_info["beam_lengths"]
+    if len(beam_lengths) > 0:
+        alpha_ = np.mean(beam_lengths) / maxdata / 2
+    else:
+        alpha_ = (model_info["max_bound"] + model_info["min_bound"]) / 20 / maxdata
+    alpha_ *= alpha
+    patterntags = np.unique(node_load_info[:, 0])
+    cmap = plt.get_cmap("Spectral")
+    colors = cmap(np.linspace(0, 1, len(patterntags)))
+    xyzlocals = [[1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]]
+    idxs = [[0, 1, 2], [1, 0, 2], [2, 0, 1]]
+    for p, ptag in enumerate(patterntags):
+        idx = np.abs(node_load_info[:, 0] - ptag) < 1e-3
+        coords = points[node_load_info[idx, -1]]
+        for i in range(3):
+            data = np.ravel(load_data[idx, i])
+            lengths = np.abs(data) * alpha_
+            arrow_heights = [0.4 * ll for ll in lengths]
+            arrow_widths = [0.6 * h for h in arrow_heights]
+            xaxis = np.reshape(xyzlocals[idxs[i][0]] * len(coords), (-1, 3))
+            yaxis = np.reshape(xyzlocals[idxs[i][1]] * len(coords), (-1, 3))
+            zaxis = np.reshape(xyzlocals[idxs[i][2]] * len(coords), (-1, 3))
+            new_coords = np.zeros_like(coords)
+            for j in range(len(xaxis)):
+                xaxis[j] *= np.sign(data[j])
+                new_coords[j] = coords[j] - 1.4 * lengths[j] * xaxis[j]
+            labels = [f"{d:.2e}" for d in data]
+            plotter.extend(
+                _make_lines_arrows(
+                    new_coords,
+                    lengths,
+                    xaxis,
+                    yaxis,
+                    zaxis,
+                    to_hex(colors[p]),
+                    f"<b>Pattern {ptag}</b><br>Nodal Load",
+                    labels,
+                    obj.line_width,
+                    arrow_heights,
+                    arrow_widths,
+                )
+            )
+
+
+def _show_ele_load(obj, plotter, model_info, alpha: float = 1.0):
+    points = model_info["coord_no_deform"]
+    ele_load_info = model_info["ele_load_info"]
+    ele_load_data = model_info["ele_load_data"]
+    ele_load_locals = model_info["ele_load_locals"]
+    if len(ele_load_info) == 0:
+        return None
+    patterntags = np.unique(ele_load_info[:, 0])
+    new_points = []
+    new_locals = []
+    new_ptags = []
+    load_data = []
+    loc = 0
+    for i, info in enumerate(ele_load_info):
+        ptag, _, classtag, nidx1, nidx2 = info
+        coord1, coord2 = points[nidx1], points[nidx2]
+        local_axis = ele_load_locals[i]
+        if classtag == 3:  # beamUniform2D, Wya <Wxa>
+            wy, wx = ele_load_data[loc : loc + 2]
+            wz = 0.0
+            n = 11
+            xl = np.linspace(0, 1, n)
+            wx, wy, wz = [wx] * n, [wy] * n, [wz] * n
+            localaxis = [local_axis] * n
+            new_ptags.extend([ptag] * n)
+            loc += 2
+        elif classtag == 12:  # beamUniform2D, Wya <Wxa> <aL> <bL> <Wyb> <Wxb>
+            wya, wyb, wxa, wxb, al, bl = ele_load_data[loc : loc + 6]
+            n = int((bl - al) / 0.1) + 1
+            xl = np.linspace(al, bl, n)
+            wy = np.interp(xl, [0, 1], [wya, wyb])
+            wx = np.interp(xl, [0, 1], [wxa, wxb])
+            wz = wy * 0
+            localaxis = [local_axis] * n
+            new_ptags.extend([ptag] * n)
+            loc += 6
+        elif classtag == 5:  # beamUniform3D wy, wz, wx
+            wy, wz, wx = ele_load_data[loc : loc + 3]
+            n = 11
+            xl = np.linspace(0, 1, n)
+            wx, wy, wz = [wx] * n, [wy] * n, [wz] * n
+            localaxis = [local_axis] * n
+            new_ptags.extend([ptag] * n)
+            loc += 3
+        elif classtag == 4:  # beamPoint2D, Py xL <Px>
+            wy, wx, xl = ele_load_data[loc : loc + 3]
+            wz = 0
+            localaxis = [local_axis]
+            new_ptags.append(ptag)
+            loc += 3
+        elif classtag == 6:  # beamPoint3D, Py, Pz, x, N
+            wy, wz, wx, xl = ele_load_data[loc : loc + 4]
+            localaxis = [local_axis]
+            new_ptags.append(ptag)
+            loc += 4
+        else:
+            warnings.warn(
+                "Currently load visualization only supports-->"
+                "<beamUniform2D,beamUniform3D,beamPoint2D,beamPoint3D>!"
+            )
+        xs = np.interp(xl, [0, 1], [coord1[0], coord2[0]])
+        ys = np.interp(xl, [0, 1], [coord1[1], coord2[1]])
+        zs = np.interp(xl, [0, 1], [coord1[2], coord2[2]])
+        new_points.append(np.column_stack([xs, ys, zs]))
+        new_locals.append(localaxis)
+        load_data.append(np.column_stack([wx, wy, wz]))
+    new_points = np.vstack(new_points)
+    new_locals = np.vstack(new_locals)
+    load_data = np.vstack(load_data)
+    new_ptags = np.array(new_ptags)
+    maxdata = np.max(np.abs(load_data))
+    beam_lengths = model_info["beam_lengths"]
+    if len(beam_lengths) > 0:
+        alpha_ = np.mean(beam_lengths) / maxdata / 2
+    else:
+        alpha_ = (model_info["max_bound"] + model_info["min_bound"]) / 20 / maxdata
+    alpha_ *= alpha
+    cmap = plt.get_cmap("rainbow")
+    colors = cmap(np.linspace(0, 1, len(patterntags)))
+    idxs = [[0, 1, 2], [3, 4, 5], [6, 7, 8]]
+    idxsidx = [[0, 1, 2], [1, 0, 2], [2, 0, 1]]
+    for p, ptag in enumerate(patterntags):
+        idx = np.abs(new_ptags - ptag) < 1e-3
+        coords = new_points[idx]
+        for i in range(3):
+            data = np.ravel(load_data[idx, i])
+            lengths = np.abs(data) * alpha_
+            arrow_heights = [0.4 * ll for ll in lengths]
+            arrow_widths = [0.6 * h for h in arrow_heights]
+            new_locals[idx, 3 * i : 3 * i + 3]
+            xaxis = new_locals[idx, idxs[idxsidx[i][0]]]
+            yaxis = new_locals[idx, idxs[idxsidx[i][1]]]
+            zaxis = new_locals[idx, idxs[idxsidx[i][2]]]
+            new_coords = np.zeros_like(coords)
+            for j in range(len(xaxis)):
+                xaxis[j] *= np.sign(data[j])
+                new_coords[j] = coords[j] - 1.4 * lengths[j] * xaxis[j]
+            labels = [f"{d:.2e}" for d in data]
+            plotter.extend(
+                _make_lines_arrows(
+                    new_coords,
+                    lengths,
+                    xaxis,
+                    yaxis,
+                    zaxis,
+                    to_hex(colors[p]),
+                    f"<b>Pattern {ptag}</b><br>Element Load",
+                    labels,
+                    obj.line_width,
+                    arrow_heights,
+                    arrow_widths,
+                )
+            )
+
+
 def _show_mp_constraint(obj, plotter, model_info, show_dofs):
     points = model_info["ConstrainedCoords"]
     cells = model_info["ConstrainedCells"]
     cells = _reshape_cell(cells)
     dofs = model_info["ConstrainedDofs"]
     dofs = ["".join([str(k) for k in dof if k != -1]) for dof in dofs]
     if len(cells) > 0:
         line_points, line_mid_points = _make_lines(points, cells)
         x, y, z = line_points[:, 0], line_points[:, 1], line_points[:, 2]
-        plotter.append(go.Scatter3d(x=x, y=y, z=z,
-                                    line=dict(
-                                        color=obj.color_constraint,
-                                        width=obj.line_width / 3),
-                                    mode="lines", name="mp constraint",
-                                    connectgaps=False, hoverinfo="skip"))
+        plotter.append(
+            go.Scatter3d(
+                x=x,
+                y=y,
+                z=z,
+                line=dict(color=obj.color_constraint, width=obj.line_width / 3),
+                mode="lines",
+                name="mp constraint",
+                connectgaps=False,
+                hoverinfo="skip",
+            )
+        )
         if show_dofs:
             x, y, z = [line_mid_points[:, j] for j in range(3)]
-            txt_plot = go.Scatter3d(x=x, y=y, z=z, text=dofs,
-                                    textfont=dict(color=obj.color_constraint,
-                                                  size=12),
-                                    mode="text", name="constraint dofs")
+            txt_plot = go.Scatter3d(
+                x=x,
+                y=y,
+                z=z,
+                text=dofs,
+                textfont=dict(color=obj.color_constraint, size=12),
+                mode="text",
+                name="constraint dofs",
+            )
             plotter.append(txt_plot)
 
 
 def _eigen_vis(
-        obj,
-        mode_tags: list,
-        input_file: str = 'EigenData.hdf5',
-        subplots: bool = False,
-        alpha: float = None,
-        show_outline: bool = False,
-        show_origin: bool = False,
-        opacity: float = 1.0,
-        show_face_line: bool = True,
-        save_html: str = "EigenVis"
+    obj,
+    mode_tags: list,
+    input_file: str = "EigenData.hdf5",
+    subplots: bool = False,
+    alpha: float = 1.0,
+    show_outline: bool = False,
+    show_origin: bool = False,
+    label_size: float = 15,
+    opacity: float = 1.0,
+    show_face_line: bool = True,
+    save_html: str = "EigenVis",
 ):
     # read
-    filename = obj.out_dir + '/' + input_file
+    filename = obj.out_dir + "/" + input_file
     eigen_data = dict()
     with h5py.File(filename, "r") as f:
         grp = f["EigenInfo"]
         for name, value in grp.items():
             eigen_data[name] = value[...]
     eigen_data["all_lines"] = _reshape_cell(eigen_data["all_lines"])
     eigen_data["all_faces"] = _reshape_cell(eigen_data["all_faces"])
 
     f = eigen_data["f"]
     eigenvector = eigen_data["eigenvector"]
     num_mode_tag = len(f)
     modei, modej = mode_tags
     modei, modej = int(modei), int(modej)
     if modej > num_mode_tag:
-        raise ValueError(
-            f"Insufficient number of modes in eigen file {filename}!")
+        raise ValueError(f"Insufficient number of modes in eigen file {filename}!")
 
     fig = go.Figure()
-    title = dict(font=dict(family="courier", color='black', size=25),
-                 text="<b>OpenSeesPy Eigen 3D View</b>"
-                 )
+    title = dict(
+        font=dict(family="courier", color="black", size=25),
+        text="<b>OpenSeesPy Eigen 3D View</b>",
+    )
     if show_outline:
-        off_axis = {'showgrid': True, 'zeroline': True, 'visible': True}
+        off_axis = {"showgrid": True, "zeroline": True, "visible": True}
     else:
-        off_axis = {'showgrid': False, 'zeroline': False, 'visible': False}
+        off_axis = {"showgrid": False, "zeroline": False, "visible": False}
 
     # !subplots
     if subplots:
         if modej - modei + 1 > 49:
-            raise ValueError(
-                "When subplots True, mode_tag range must < 49 for clarify"
-            )
+            raise ValueError("When subplots True, mode_tag range must < 49 for clarify")
         shape = shape_dict[modej - modei + 1]
-        specs = [[{'is_3d': True}
-                  for i in range(shape[1])] for j in range(shape[0])]
+        specs = [[{"is_3d": True} for i in range(shape[1])] for j in range(shape[0])]
         subplot_titles = []
         for i, idx in enumerate(range(modei, modej + 1)):
             txt = "Mode {}: T = {:.3f} s".format(idx, 1 / f[idx - 1])
             subplot_titles.append(txt)
 
-        fig = make_subplots(rows=shape[0], cols=shape[1],
-                            specs=specs, figure=fig,
-                            print_grid=False, subplot_titles=subplot_titles,
-                            horizontal_spacing=0.07 / shape[1],
-                            vertical_spacing=0.1 / shape[0],
-                            column_widths=[1] * shape[1],
-                            row_heights=[1] * shape[0]
-                            )
+        fig = make_subplots(
+            rows=shape[0],
+            cols=shape[1],
+            specs=specs,
+            figure=fig,
+            print_grid=False,
+            subplot_titles=subplot_titles,
+            horizontal_spacing=0.07 / shape[1],
+            vertical_spacing=0.1 / shape[0],
+            column_widths=[1] * shape[1],
+            row_heights=[1] * shape[0],
+        )
         for i, idx in enumerate(range(modei, modej + 1)):
             eigen_vec = eigenvector[idx - 1]
-            if alpha is None:
-                value_ = np.max(np.sqrt(np.sum(eigen_vec ** 2, axis=1)))
-                alpha_ = (
-                    eigen_data["max_bound"] / obj.bound_fact / value_
-                )
-            else:
-                alpha_ = alpha
+            value_ = np.max(np.sqrt(np.sum(eigen_vec**2, axis=1)))
+            alpha_ = eigen_data["max_bound"] / obj.bound_fact / value_
+            alpha_ *= alpha if alpha else alpha_
             eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
-            scalars = np.sqrt(np.sum(eigen_vec ** 2, axis=1))
+            scalars = np.sqrt(np.sum(eigen_vec**2, axis=1))
 
             idxi = int(np.ceil((i + 1) / shape[1]) - 1)
             idxj = int(i - idxi * shape[1])
             # ---------------------------------------------------------
             if show_origin:
                 points_origin = eigen_data["coord_no_deform"]
             else:
                 points_origin = None
-            plotter = _generate_all_mesh(points=eigen_points, scalars=scalars, opacity=opacity,
-                                         lines_cells=eigen_data["all_lines"],
-                                         face_cells=eigen_data["all_faces"],
-                                         coloraxis=f"coloraxis{i + 1}",
-                                         points_origin=points_origin,
-                                         point_size=obj.point_size,
-                                         line_width=obj.line_width,
-                                         show_face_line=show_face_line)
+            plotter = _generate_all_mesh(
+                points=eigen_points,
+                scalars=scalars,
+                opacity=opacity,
+                lines_cells=eigen_data["all_lines"],
+                face_cells=eigen_data["all_faces"],
+                coloraxis=f"coloraxis{i + 1}",
+                points_origin=points_origin,
+                point_size=obj.point_size,
+                line_width=obj.line_width,
+                show_face_line=show_face_line,
+            )
             fig.add_traces(plotter, rows=idxi + 1, cols=idxj + 1)
         if np.max(np.abs(eigen_data["coord_no_deform"][:, -1])) < 1e-8:
-            eye = dict(x=0., y=-0.1, z=10)  # for 2D camera
-            scene = dict(camera=dict(
-                eye=eye, projection=dict(type="orthographic")),
-                xaxis=off_axis, yaxis=off_axis, zaxis=off_axis)
+            eye = dict(x=0.0, y=-0.1, z=10)  # for 2D camera
+            scene = dict(
+                camera=dict(eye=eye, projection=dict(type="orthographic")),
+                xaxis=off_axis,
+                yaxis=off_axis,
+                zaxis=off_axis,
+            )
         else:
             eye = dict(x=-3.5, y=-3.5, z=3.5)  # for 3D camera
-            scene = dict(aspectratio=dict(x=1, y=1, z=1), aspectmode="data",
-                         camera=dict(eye=eye, projection=dict(
-                             type="orthographic")),
-                         xaxis=off_axis, yaxis=off_axis, zaxis=off_axis)
+            scene = dict(
+                aspectratio=dict(x=1, y=1, z=1),
+                aspectmode="data",
+                camera=dict(eye=eye, projection=dict(type="orthographic")),
+                xaxis=off_axis,
+                yaxis=off_axis,
+                zaxis=off_axis,
+            )
         scenes = dict()
         coloraxiss = dict()
         for k in range(shape[0] * shape[1]):
             coloraxiss[f"coloraxis{k + 1}"] = dict(
-                showscale=False, colorscale=obj.color_map)
+                showscale=False, colorscale=obj.color_map
+            )
             if k >= 1:
                 if np.max(np.abs(eigen_data["coord_no_deform"][:, -1])) < 1e-8:
-                    scenes[f"scene{k + 1}"] = dict(camera=dict(eye=eye,
-                                                               projection=dict(type="orthographic")),
-                                                   xaxis=off_axis, yaxis=off_axis, zaxis=off_axis)
+                    scenes[f"scene{k + 1}"] = dict(
+                        camera=dict(eye=eye, projection=dict(type="orthographic")),
+                        xaxis=off_axis,
+                        yaxis=off_axis,
+                        zaxis=off_axis,
+                    )
                 else:
-                    scenes[f"scene{k + 1}"] = dict(aspectratio=dict(x=1, y=1, z=1), aspectmode="data",
-                                                   camera=dict(eye=eye,
-                                                               projection=dict(type="orthographic")),
-                                                   xaxis=off_axis, yaxis=off_axis, zaxis=off_axis)
+                    scenes[f"scene{k + 1}"] = dict(
+                        aspectratio=dict(x=1, y=1, z=1),
+                        aspectmode="data",
+                        camera=dict(eye=eye, projection=dict(type="orthographic")),
+                        xaxis=off_axis,
+                        yaxis=off_axis,
+                        zaxis=off_axis,
+                    )
         fig.update_layout(
             title=title,
             template=obj.theme,
             autosize=True,
             showlegend=False,
             coloraxis=dict(showscale=False, colorscale=obj.color_map),
             scene=scene,
             **scenes,
-            **coloraxiss
+            **coloraxiss,
         )
     # !slider style
     else:
         n_data = None
         cmins = []
         cmaxs = []
         for i, idx in enumerate(range(modei, modej + 1)):
             step = idx - 1
             eigen_vec = eigenvector[step]
-            if alpha is None:
-                value_ = np.max(np.sqrt(np.sum(eigen_vec ** 2, axis=1)))
-                alpha_ = (
-                    eigen_data["max_bound"] / obj.bound_fact / value_
-                )
-            else:
-                alpha_ = alpha
+            value_ = np.max(np.sqrt(np.sum(eigen_vec**2, axis=1)))
+            alpha_ = eigen_data["max_bound"] / obj.bound_fact / value_
+            alpha_ *= alpha if alpha else alpha_
             eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
-            scalars = np.sqrt(np.sum(eigen_vec ** 2, axis=1))
+            scalars = np.sqrt(np.sum(eigen_vec**2, axis=1))
             cmins.append(np.min(scalars))
             cmaxs.append(np.max(scalars))
 
             # -------------------------------------------------------------
             # start plot
             if show_origin:
                 points_origin = eigen_data["coord_no_deform"]
             else:
                 points_origin = None
-            plotter = _generate_all_mesh(points=eigen_points, scalars=scalars, opacity=opacity,
-                                         lines_cells=eigen_data["all_lines"],
-                                         face_cells=eigen_data["all_faces"],
-                                         coloraxis=f"coloraxis{i + 1}",
-                                         points_origin=points_origin,
-                                         point_size=obj.point_size, line_width=obj.line_width,
-                                         show_face_line=show_face_line)
+            plotter = _generate_all_mesh(
+                points=eigen_points,
+                scalars=scalars,
+                opacity=opacity,
+                lines_cells=eigen_data["all_lines"],
+                face_cells=eigen_data["all_faces"],
+                coloraxis=f"coloraxis{i + 1}",
+                points_origin=points_origin,
+                point_size=obj.point_size,
+                line_width=obj.line_width,
+                show_face_line=show_face_line,
+            )
             fig.add_traces(plotter)
             if i == 0:
                 n_data = len(fig.data)
         for i in range(n_data, len(fig.data)):
             fig.data[i].visible = False
         # Create and add slider
         steps = []
         for i, idx in enumerate(range(modei, modej + 1)):
             txt = "Mode {}: T = {:.3f} s".format(idx, 1 / f[idx - 1])
             step = dict(
                 method="update",
-                args=[{"visible": [False] * len(fig.data)},
-                      {"title": txt}],  # layout attribute
+                args=[
+                    {"visible": [False] * len(fig.data)},
+                    {"title": txt},
+                ],  # layout attribute
                 label=str(idx),
             )
-            step["args"][0]["visible"][n_data *
-                                       i:n_data * (i + 1)] = [True] * n_data
+            step["args"][0]["visible"][n_data * i : n_data * (i + 1)] = [True] * n_data
             # Toggle i'th trace to "visible"
             steps.append(step)
-        sliders = [dict(
-            active=modej - modei + 1,
-            currentvalue={"prefix": "Mode: "},
-            pad={"t": 50},
-            steps=steps
-        )]
+        sliders = [
+            dict(
+                active=modej - modei + 1,
+                currentvalue={"prefix": "Mode: "},
+                pad={"t": 50},
+                steps=steps,
+            )
+        ]
         coloraxiss = {}
         for i in range(modej - modei + 1):
-            coloraxiss[f"coloraxis{i + 1}"] = dict(colorscale=obj.color_map,
-                                                   cmin=cmins[i],
-                                                   cmax=cmaxs[i],
-                                                   colorbar=dict(tickfont=dict(size=15)))
+            coloraxiss[f"coloraxis{i + 1}"] = dict(
+                colorscale=obj.color_map,
+                cmin=cmins[i],
+                cmax=cmaxs[i],
+                colorbar=dict(tickfont=dict(size=15)),
+            )
 
         if np.max(np.abs(eigen_data["coord_no_deform"][:, -1])) < 1e-8:
-            eye = dict(x=0., y=-0.1, z=10)  # for 2D camera
-            scene = dict(camera=dict(
-                eye=eye, projection=dict(type="orthographic")),
-                xaxis=off_axis, yaxis=off_axis, zaxis=off_axis)
+            eye = dict(x=0.0, y=-0.1, z=10)  # for 2D camera
+            scene = dict(
+                camera=dict(eye=eye, projection=dict(type="orthographic")),
+                xaxis=off_axis,
+                yaxis=off_axis,
+                zaxis=off_axis,
+            )
         else:
             eye = dict(x=-3.5, y=-3.5, z=3.5)  # for 3D camera
-            scene = dict(aspectratio=dict(x=1, y=1, z=1), aspectmode="data",
-                         camera=dict(eye=eye, projection=dict(
-                             type="orthographic")),
-                         xaxis=off_axis, yaxis=off_axis, zaxis=off_axis)
+            scene = dict(
+                aspectratio=dict(x=1, y=1, z=1),
+                aspectmode="data",
+                camera=dict(eye=eye, projection=dict(type="orthographic")),
+                xaxis=off_axis,
+                yaxis=off_axis,
+                zaxis=off_axis,
+            )
         fig.update_layout(
             template=obj.theme,
             autosize=True,
             showlegend=False,
             scene=scene,
             title=title,
             sliders=sliders,
-            **coloraxiss
+            **coloraxiss,
         )
     if save_html:
         if not save_html.endswith(".html"):
             save_html += ".html"
         pio.write_html(fig, file=save_html, auto_open=True)
-    if obj.notebook:
-        fig.show()
+    return fig
 
 
 def _eigen_anim(
-        obj,
-        mode_tag: int = 1,
-        input_file: str = 'EigenData.hdf5',
-        n_cycle: int = 5,
-        alpha: float = None,
-        show_outline: bool = False,
-        opacity: float = 1,
-        framerate: int = 3,
-        show_face_line: bool = True,
-        save_html: str = "EigenAnimation"
+    obj,
+    mode_tag: int = 1,
+    input_file: str = "EigenData.hdf5",
+    n_cycle: int = 5,
+    alpha: float = 1.0,
+    show_outline: bool = False,
+    label_size: float = 15,
+    opacity: float = 1,
+    framerate: int = 3,
+    show_face_line: bool = True,
+    save_html: str = "EigenAnimation",
 ):
-    filename = obj.out_dir + '/' + input_file
+    filename = obj.out_dir + "/" + input_file
     eigen_data = dict()
     with h5py.File(filename, "r") as f:
         grp = f["EigenInfo"]
         for name, value in grp.items():
             eigen_data[name] = value[...]
     eigen_data["all_lines"] = _reshape_cell(eigen_data["all_lines"])
     eigen_data["all_faces"] = _reshape_cell(eigen_data["all_faces"])
@@ -686,55 +1101,58 @@
     f = eigen_data["f"]
     eigenvector = eigen_data["eigenvector"]
     num_mode_tag = len(f)
     if mode_tag > num_mode_tag:
         raise ValueError("Insufficient number of modes in open file")
     eigen_vec = eigenvector[mode_tag - 1]
     f_ = f[mode_tag - 1]
-    if alpha is None:
-        value_ = np.max(np.sqrt(np.sum(eigen_vec ** 2, axis=1)))
-        alpha_ = (
-            eigen_data["max_bound"] / obj.bound_fact / value_
-        )
-    else:
-        alpha_ = alpha
+    value_ = np.max(np.sqrt(np.sum(eigen_vec**2, axis=1)))
+    alpha_ = eigen_data["max_bound"] / obj.bound_fact / value_
+    alpha_ *= alpha if alpha else alpha_
     eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
     anti_eigen_points = eigen_data["coord_no_deform"] - eigen_vec * alpha_
-    scalars = np.sqrt(np.sum(eigen_vec ** 2, axis=1))
-    plt_points = [anti_eigen_points,
-                  eigen_data["coord_no_deform"], eigen_points]
+    scalars = np.sqrt(np.sum(eigen_vec**2, axis=1))
+    plt_points = [anti_eigen_points, eigen_data["coord_no_deform"], eigen_points]
     index = [1] + [2, 0] * n_cycle
     nb_frames = len(index)
     times = int(nb_frames / framerate)
 
     # -----------------------------------------------------------------------------
     # start plot
     frames = []
     for k, idx in enumerate(index):
         points = plt_points[idx]
         xyz = (eigen_data["coord_no_deform"] - points) / alpha_
-        xyz_eigen = np.sqrt(np.sum(xyz ** 2, axis=1))
-        plotter = _generate_all_mesh(points=points, scalars=xyz_eigen,
-                                     point_size=obj.point_size, line_width=obj.line_width,
-                                     opacity=opacity,
-                                     lines_cells=eigen_data["all_lines"],
-                                     face_cells=eigen_data["all_faces"],
-                                     coloraxis="coloraxis",
-                                     show_face_line=show_face_line)
+        xyz_eigen = np.sqrt(np.sum(xyz**2, axis=1))
+        plotter = _generate_all_mesh(
+            points=points,
+            scalars=xyz_eigen,
+            point_size=obj.point_size,
+            line_width=obj.line_width,
+            opacity=opacity,
+            lines_cells=eigen_data["all_lines"],
+            face_cells=eigen_data["all_faces"],
+            coloraxis="coloraxis",
+            show_face_line=show_face_line,
+        )
         frames.append(go.Frame(data=plotter, name="step:" + str(k + 1)))
 
     fig = go.Figure(frames=frames)
     # Add data to be displayed before animation starts
-    plotter0 = _generate_all_mesh(points=plt_points[index[0]], scalars=scalars * 0,
-                                  point_size=obj.point_size, line_width=obj.line_width,
-                                  opacity=opacity,
-                                  lines_cells=eigen_data["all_lines"],
-                                  face_cells=eigen_data["all_faces"],
-                                  coloraxis="coloraxis",
-                                  show_face_line=show_face_line)
+    plotter0 = _generate_all_mesh(
+        points=plt_points[index[0]],
+        scalars=scalars * 0,
+        point_size=obj.point_size,
+        line_width=obj.line_width,
+        opacity=opacity,
+        lines_cells=eigen_data["all_lines"],
+        face_cells=eigen_data["all_faces"],
+        coloraxis="coloraxis",
+        show_face_line=show_face_line,
+    )
     fig.add_traces(plotter0)
 
     def frame_args(duration):
         return {
             "frame": {"duration": duration},
             "mode": "immediate",
             "fromcurrent": True,
@@ -755,32 +1173,33 @@
                 }
                 for k, f in enumerate(fig.frames)
             ],
         }
     ]
     # Layout
     if np.max(np.abs(eigen_data["coord_no_deform"][:, -1])) < 1e-8:
-        eye = dict(x=0., y=-0.1, z=10)  # for 2D camera
-        scene = dict(camera=dict(
-            eye=eye, projection=dict(type="orthographic")))
+        eye = dict(x=0.0, y=-0.1, z=10)  # for 2D camera
+        scene = dict(camera=dict(eye=eye, projection=dict(type="orthographic")))
     else:
         eye = dict(x=-3.5, y=-3.5, z=3.5)  # for 3D camera
-        scene = dict(aspectratio=dict(x=1, y=1, z=1), aspectmode="data",
-                     camera=dict(eye=eye, projection=dict(
-                         type="orthographic")))
+        scene = dict(
+            aspectratio=dict(x=1, y=1, z=1),
+            aspectmode="data",
+            camera=dict(eye=eye, projection=dict(type="orthographic")),
+        )
     txt = "<br> Mode {}: T = {:.3f} s".format(mode_tag, 1 / f_)
     fig.update_layout(
-        title=dict(font=dict(family="courier", color='black', size=25),
-                   text="<b>OpenSeesPy Eigen 3D View</b>" + txt
-                   ),
+        title=dict(
+            font=dict(family="courier", color="black", size=25),
+            text="<b>OpenSeesPy Eigen 3D View</b>" + txt,
+        ),
         template=obj.theme,
         autosize=True,
         showlegend=False,
-        coloraxis=dict(colorscale=obj.color_map,
-                       colorbar=dict(tickfont=dict(size=15))),
+        coloraxis=dict(colorscale=obj.color_map, colorbar=dict(tickfont=dict(size=15))),
         scene=scene,
         updatemenus=[
             {
                 "buttons": [
                     {
                         "args": [None, frame_args(times)],
                         "label": "&#9654;",  # play symbol
@@ -795,120 +1214,157 @@
                 "direction": "left",
                 "pad": {"r": 10, "t": 70},
                 "type": "buttons",
                 "x": 0.1,
                 "y": 0,
             }
         ],
-        sliders=sliders
+        sliders=sliders,
     )
     if not show_outline:
         fig.update_layout(
-            scene=dict(xaxis={'showgrid': False, 'zeroline': False, 'visible': False},
-                       yaxis={'showgrid': False,
-                              'zeroline': False, 'visible': False},
-                       zaxis={'showgrid': False, 'zeroline': False, 'visible': False}, ),
+            scene=dict(
+                xaxis={"showgrid": False, "zeroline": False, "visible": False},
+                yaxis={"showgrid": False, "zeroline": False, "visible": False},
+                zaxis={"showgrid": False, "zeroline": False, "visible": False},
+            ),
         )
 
     if save_html:
         if not save_html.endswith(".html"):
             save_html += ".html"
         pio.write_html(fig, file=save_html, auto_open=True)
-    if obj.notebook:
-        fig.show()
+    return fig
 
 
-def _react_vis(obj,
-               input_file: str = "NodeReactionStepData-1.hdf5",
-               slider: bool = False,
-               direction: str = "Fz",
-               show_values: bool = True,
-               show_outline: bool = False,
-               save_html: str = "ReactionVis"):
+def _react_vis(
+    obj,
+    input_file: str = "NodeReactionStepData-1.hdf5",
+    slider: bool = False,
+    direction: str = "Fz",
+    show_values: bool = True,
+    show_outline: bool = False,
+    save_html: str = "ReactionVis",
+):
     direct = direction.lower()
-    if direct not in ['fx', 'fy', 'fz', 'mx', 'my', 'mz']:
+    if direct not in ["fx", "fy", "fz", "mx", "my", "mz"]:
         raise ValueError(
-            "response must be one of ['Fx', 'Fy', 'Fz', 'Mx', 'My', 'Mz']!")
-    filename = obj.out_dir + '/' + input_file
+            "response must be one of ['Fx', 'Fy', 'Fz', 'Mx', 'My', 'Mz']!"
+        )
+    filename = obj.out_dir + "/" + input_file
     node_react_steps = []
     with h5py.File(filename, "r") as f:
         Nsteps = int(f["Nsteps"][...])
         node_coords = f["NodeReactCoords"][...]
-        model_dims = f['model_dims'][...]
+        model_dims = f["model_dims"][...]
         NodeTags = f["NodeReactTags"][...]
         num_nodes = node_coords.shape[0]
         grp = f["NodeReactSteps"]
         for i in range(Nsteps):
             node_react_steps.append(grp[f"step{i + 1}"][...])
     if np.max(model_dims) < 3:
         D2 = True
     else:
         D2 = False
     x, y, z = [node_coords[:, j] for j in range(3)]
-    max_bound = np.max(np.max(node_coords, axis=0) -
-                       np.min(node_coords, axis=0))
-    axis_dict = dict(fx=(1, 0., 0.), fy=(0., 1, 0.), fz=(0., 0., 1),
-                     mx=(1, 0., 0.), my=(0., 1, 0.), mz=(0., 0., 1))
-    color_dict = dict(fx="#d20962", fy="#f47721", fz="#7ac143",
-                      mx="#00a78e", my="#00bce4", mz="#7d3f98")
+    max_bound = np.max(np.max(node_coords, axis=0) - np.min(node_coords, axis=0))
+    axis_dict = dict(
+        fx=(1, 0.0, 0.0),
+        fy=(0.0, 1, 0.0),
+        fz=(0.0, 0.0, 1),
+        mx=(1, 0.0, 0.0),
+        my=(0.0, 1, 0.0),
+        mz=(0.0, 0.0, 1),
+    )
+    color_dict = dict(
+        fx="#d20962",
+        fy="#f47721",
+        fz="#7ac143",
+        mx="#00a78e",
+        my="#00bce4",
+        mz="#7d3f98",
+    )
     if D2:
         reactidx_dict = dict(fx=0, fy=1, fz=None, mx=None, my=None, mz=2)
     else:
         reactidx_dict = dict(fx=0, fy=1, fz=2, mx=3, my=4, mz=5)
 
     fig = go.Figure()
 
     def creat_plot(step):
         f = node_react_steps[step][:, reactidx_dict[direct]]
         idxmax, idxmin = np.argmax(f), np.argmin(f)
         # point plot
         labels = [
-            f"<b>tag: {tag}</b><br>{direction}: {fi:.3E}" for tag, fi in zip(NodeTags, f)]
-        point_plot = go.Scatter3d(x=x, y=y, z=z,
-                                  marker=dict(size=obj.point_size,
-                                              color=obj.color_point),
-                                  mode="markers", name="Node Reactions",
-                                  customdata=labels,
-                                  hovertemplate='%{customdata}')
+            f"<b>tag: {tag}</b><br>{direction}: {fi:.3E}"
+            for tag, fi in zip(NodeTags, f)
+        ]
+        point_plot = go.Scatter3d(
+            x=x,
+            y=y,
+            z=z,
+            marker=dict(size=obj.point_size, color=obj.color_point),
+            mode="markers",
+            name="Node Reactions",
+            customdata=labels,
+            hovertemplate="%{customdata}",
+        )
         fig.add_trace(point_plot)
         if show_values:
             labels = [f"{fi:.3E}" for fi in f]
-            txt_plot = go.Scatter3d(x=x, y=y, z=z, text=labels,
-                                    textfont=dict(color="#6e750e",
-                                                  size=10),
-                                    mode="text", hoverinfo='skip', )
+            txt_plot = go.Scatter3d(
+                x=x,
+                y=y,
+                z=z,
+                text=labels,
+                textfont=dict(color="#6e750e", size=10),
+                mode="text",
+                hoverinfo="skip",
+            )
             fig.add_trace(txt_plot)
         # max min point plot
         labels = [
-            f"<b>tag: {NodeTags[idx]}</b><br>{direction}: {f[idx]:.3E}" for idx in [idxmax, idxmin]]
-        point_plot2 = go.Scatter3d(x=x[[idxmax, idxmin]], y=y[[idxmax, idxmin]], z=z[[idxmax, idxmin]],
-                                   marker=dict(size=obj.point_size * 1.25,
-                                               color=obj.color_point,
-                                               symbol=['x'] * 2),
-                                   mode="markers", name="Node Reactions",
-                                   customdata=labels,
-                                   hovertemplate='%{customdata}')
+            f"<b>tag: {NodeTags[idx]}</b><br>{direction}: {f[idx]:.3E}"
+            for idx in [idxmax, idxmin]
+        ]
+        point_plot2 = go.Scatter3d(
+            x=x[[idxmax, idxmin]],
+            y=y[[idxmax, idxmin]],
+            z=z[[idxmax, idxmin]],
+            marker=dict(
+                size=obj.point_size * 1.25, color=obj.color_point, symbol=["x"] * 2
+            ),
+            mode="markers",
+            name="Node Reactions",
+            customdata=labels,
+            hovertemplate="%{customdata}",
+        )
         fig.add_trace(point_plot2)
         # line plot
         line_ends = np.zeros_like(node_coords)
         for i in range(num_nodes):
-            line_ends[i] = node_coords[i] - \
-                np.array(axis_dict[direct]) * \
-                max_bound / 30 * np.sign(f[i])
+            line_ends[i] = node_coords[i] - np.array(
+                axis_dict[direct]
+            ) * max_bound / 30 * np.sign(f[i])
         line_points = []
         line_cells = []
         for point1, point2 in zip(node_coords, line_ends):
             line_points.extend([point2, point1])
             line_cells.extend([2, len(line_points) - 2, len(line_points) - 1])
         line_cells = np.reshape(line_cells, (-1, 3))
-        line_plot = _generate_line_mesh(points=line_points, cells=line_cells,
-                                        line_width=obj.line_width * 2, color=color_dict[direct])
+        line_plot = _generate_line_mesh(
+            points=line_points,
+            cells=line_cells,
+            line_width=obj.line_width * 2,
+            color=color_dict[direct],
+        )
         fig.add_traces(line_plot)
-        arrow_plot = _creat_arrows(points=line_points, cells=line_cells,
-                                   color=color_dict[direct])
+        arrow_plot = _creat_arrows(
+            points=line_points, cells=line_cells, color=color_dict[direct]
+        )
         fig.add_traces(arrow_plot)
 
     if slider:
         n_data = None
         for step in range(Nsteps):
             creat_plot(step)
             if step == 0:
@@ -917,113 +1373,126 @@
         for i in range(0, len(fig.data) - n_data):
             fig.data[i].visible = False
         # ! Create and add slider
         steps = []
         for i in range(Nsteps):
             f = node_react_steps[i][:, reactidx_dict[direct]]
             idxmax, idxmin = np.argmax(f), np.argmin(f)
-            txt = (f"<b>Step {i + 1} {direction}</b>"
-                   f"<br>max={f[idxmax]:.3E} | nodeTag={NodeTags[idxmax]}"
-                   f"<br>min={f[idxmin]:.3E} | nodeTag={NodeTags[idxmin]}")
+            txt = (
+                f"<b>Step {i + 1} {direction}</b>"
+                f"<br>max={f[idxmax]:.3E} | nodeTag={NodeTags[idxmax]}"
+                f"<br>min={f[idxmin]:.3E} | nodeTag={NodeTags[idxmin]}"
+            )
             step = dict(
                 method="update",
-                args=[{"visible": [False] * len(fig.data)},
-                      {"title": txt}],  # layout attribute
+                args=[
+                    {"visible": [False] * len(fig.data)},
+                    {"title": txt},
+                ],  # layout attribute
                 label=str(i + 1),
             )
             idxi, idxj = n_data * i, n_data * (i + 1)
             step["args"][0]["visible"][idxi:idxj] = [True] * n_data
             # Toggle i'th trace to "visible"
             steps.append(step)
-        sliders = [dict(
-            active=Nsteps,
-            currentvalue={"prefix": "Step: "},
-            pad={"t": 50},
-            steps=steps
-        )]
+        sliders = [
+            dict(
+                active=Nsteps,
+                currentvalue={"prefix": "Step: "},
+                pad={"t": 50},
+                steps=steps,
+            )
+        ]
         if D2:
-            eye = dict(x=0., y=-0.1, z=10)  # for 2D camera
-            scene = dict(camera=dict(
-                eye=eye, projection=dict(type="orthographic")))
+            eye = dict(x=0.0, y=-0.1, z=10)  # for 2D camera
+            scene = dict(camera=dict(eye=eye, projection=dict(type="orthographic")))
         else:
             eye = dict(x=-3.5, y=-3.5, z=3.5)  # for 3D camera
-            scene = dict(aspectratio=dict(x=1, y=1, z=1), aspectmode="data",
-                         camera=dict(eye=eye, projection=dict(
-                             type="orthographic")))
+            scene = dict(
+                aspectratio=dict(x=1, y=1, z=1),
+                aspectmode="data",
+                camera=dict(eye=eye, projection=dict(type="orthographic")),
+            )
         fig.update_layout(
             template=obj.theme,
             autosize=True,
             showlegend=False,
             scene=scene,  # orthographic,perspective
-            title=dict(font=dict(family="courier", color='black', size=25),
-                       text=f"<b>OpenSeesPy Node Reactions View</b>"
-                       ),
+            title=dict(
+                font=dict(family="courier", color="black", size=25),
+                text="<b>OpenSeesPy Node Reactions View</b>",
+            ),
             sliders=sliders,
         )
     else:  # a sing step
-        idx = np.argmax([np.max(np.abs(react[:, reactidx_dict[direct]]))
-                         for react in node_react_steps])
+        idx = np.argmax(
+            [
+                np.max(np.abs(react[:, reactidx_dict[direct]]))
+                for react in node_react_steps
+            ]
+        )
         creat_plot(idx)
         f = node_react_steps[idx][:, reactidx_dict[direct]]
         idxmax, idxmin = np.argmax(f), np.argmin(f)
-        txt = (f"<b>OpenSeesPy Node Reactions View</b>"
-               f"<br>Step {i + 1} {direction}"
-               f"<br>max={f[idxmax]:.3E} | nodeTag={NodeTags[idxmax]}"
-               f"<br>min={f[idxmin]:.3E} | nodeTag={NodeTags[idxmin]}")
+        txt = (
+            f"<b>OpenSeesPy Node Reactions View</b>"
+            f"<br>Step {i + 1} {direction}"
+            f"<br>max={f[idxmax]:.3E} | nodeTag={NodeTags[idxmax]}"
+            f"<br>min={f[idxmin]:.3E} | nodeTag={NodeTags[idxmin]}"
+        )
         if D2:
-            eye = dict(x=0., y=-0.1, z=10)  # for 2D camera
-            scene = dict(camera=dict(
-                eye=eye, projection=dict(type="orthographic")))
+            eye = dict(x=0.0, y=-0.1, z=10)  # for 2D camera
+            scene = dict(camera=dict(eye=eye, projection=dict(type="orthographic")))
         else:
             eye = dict(x=-3.5, y=-3.5, z=3.5)  # for 3D camera
-            scene = dict(aspectratio=dict(x=1, y=1, z=1), aspectmode="data",
-                         camera=dict(eye=eye, projection=dict(
-                             type="orthographic")))
+            scene = dict(
+                aspectratio=dict(x=1, y=1, z=1),
+                aspectmode="data",
+                camera=dict(eye=eye, projection=dict(type="orthographic")),
+            )
         fig.update_layout(
             template=obj.theme,
             autosize=True,
             showlegend=False,
             scene=scene,  # orthographic,perspective
-            title=dict(font=dict(family="courier", color='black', size=25),
-                       text=txt
-                       ),
+            title=dict(font=dict(family="courier", color="black", size=25), text=txt),
         )
     if not show_outline:
         fig.update_layout(
-            scene=dict(xaxis={'showgrid': False, 'zeroline': False, 'visible': False},
-                       yaxis={'showgrid': False,
-                              'zeroline': False, 'visible': False},
-                       zaxis={'showgrid': False, 'zeroline': False, 'visible': False}, ),
+            scene=dict(
+                xaxis={"showgrid": False, "zeroline": False, "visible": False},
+                yaxis={"showgrid": False, "zeroline": False, "visible": False},
+                zaxis={"showgrid": False, "zeroline": False, "visible": False},
+            ),
         )
     if save_html:
         if not save_html.endswith(".html"):
             save_html += ".html"
         pio.write_html(fig, file=save_html, auto_open=True)
-    if obj.notebook:
-        fig.show()
+    return fig
 
 
 def _deform_vis(
-        obj,
-        input_file: str = "NodeRespStepData-1.hdf5",
-        slider: bool = False,
-        response: str = "disp",
-        alpha: float = None,
-        show_outline: bool = False,
-        show_origin: bool = False,
-        show_face_line: bool = True,
-        opacity: float = 1,
-        save_html: str = "DefoVis",
-        model_update: bool = False
+    obj,
+    input_file: str = "NodeRespStepData-1.hdf5",
+    slider: bool = False,
+    response: str = "disp",
+    alpha: float = 1.0,
+    show_outline: bool = False,
+    show_origin: bool = False,
+    show_face_line: bool = True,
+    opacity: float = 1,
+    save_html: str = "DefoVis",
+    model_update: bool = False,
 ):
     resp_type = response.lower()
-    if resp_type not in ['disp', 'vel', 'accel']:
+    if resp_type not in ["disp", "vel", "accel"]:
         raise ValueError("response must be 'disp', 'vel', or 'accel'!")
     # ------------------------------------------------
-    filename = obj.out_dir + '/' + input_file
+    filename = obj.out_dir + "/" + input_file
     model_info_steps = dict()
     cell_steps = dict()
     node_resp_steps = dict()
     with h5py.File(filename, "r") as f:
         n = int(f["Nsteps"][...])
         grp1 = f["ModelInfoSteps"]
         grp2 = f["CellSteps"]
@@ -1048,36 +1517,37 @@
             temp = []
             for i in range(n):
                 temp.append(value_[f"step{i + 1}"][...])
             node_resp_steps[name] = temp
 
     num_steps = len(node_resp_steps["disp"])
     # ! max response
-    max_resps = [np.max(np.sqrt(np.sum(resp_ ** 2, axis=1)))
-                 for resp_ in node_resp_steps[resp_type]]
+    max_resps = [
+        np.max(np.sqrt(np.sum(resp_**2, axis=1)))
+        for resp_ in node_resp_steps[resp_type]
+    ]
     max_step = np.argmax(max_resps)
     max_node_resp = node_resp_steps[resp_type][max_step]
-    scalars = np.sqrt(np.sum(max_node_resp ** 2, axis=1))
+    scalars = np.sqrt(np.sum(max_node_resp**2, axis=1))
     data = node_resp_steps[resp_type]
     cmin, cmax = np.min(scalars), np.max(scalars)
     if model_update:
         bounds = model_info_steps["bound"][0]
         model_dims = model_info_steps["model_dims"][0]
     else:
         bounds = model_info_steps["bound"]
         model_dims = model_info_steps["model_dims"]
     # scale factor
     if resp_type == "disp":
-        if alpha is None:
-            max_bound = np.max(
-                [bounds[1] - bounds[0], bounds[3] - bounds[2], bounds[5] - bounds[4]])
-            value = np.max(np.sqrt(np.sum(max_node_resp ** 2, axis=1)))
-            alpha_ = max_bound / obj.bound_fact / value
-        else:
-            alpha_ = alpha
+        max_bound = np.max(
+            [bounds[1] - bounds[0], bounds[3] - bounds[2], bounds[5] - bounds[4]]
+        )
+        value = np.max(np.sqrt(np.sum(max_node_resp**2, axis=1)))
+        alpha_ = max_bound / obj.bound_fact / value
+        alpha_ *= alpha if alpha else alpha_
     else:
         alpha_ = 0
     # ------------------------------------------------------------------------
     fig = go.Figure()
     # -------------------------------------------------------------------------
     if slider:
         n_data = None
@@ -1092,78 +1562,92 @@
                 faces_cells = _reshape_cell(cell_steps["all_faces"])
             node_resp = node_resp_steps[resp_type][step]
             node_deform_coords = alpha_ * node_resp + node_nodeform_coords
             if show_origin:
                 points_origin = node_nodeform_coords
             else:
                 points_origin = None
-            scalars = np.sqrt(np.sum(node_resp ** 2, axis=1))
-            plotter = _generate_all_mesh(points=node_deform_coords, scalars=scalars,
-                                         point_size=obj.point_size, line_width=obj.line_width,
-                                         opacity=opacity,
-                                         lines_cells=lines_cells,
-                                         face_cells=faces_cells,
-                                         coloraxis=f"coloraxis{step + 1}",
-                                         points_origin=points_origin,
-                                         show_face_line=show_face_line)
+            scalars = np.sqrt(np.sum(node_resp**2, axis=1))
+            plotter = _generate_all_mesh(
+                points=node_deform_coords,
+                scalars=scalars,
+                point_size=obj.point_size,
+                line_width=obj.line_width,
+                opacity=opacity,
+                lines_cells=lines_cells,
+                face_cells=faces_cells,
+                coloraxis=f"coloraxis{step + 1}",
+                points_origin=points_origin,
+                show_face_line=show_face_line,
+            )
             fig.add_traces(plotter)
             if step == 0:
                 n_data = len(fig.data)
         for i in range(0, len(fig.data) - n_data):
             fig.data[i].visible = False
         # ! Create and add slider
         steps = []
         for i in range(num_steps):
             maxx, maxy, maxz = np.max(data[i], axis=0)
             minx, miny, minz = np.min(data[i], axis=0)
-            txt = (f"<b>Step {i + 1} {response}</b>"
-                   f"<br>max.x={maxx:.2E} | min.x={minx:.2E}"
-                   f"<br>max.y={maxy:.2E} | min.y={miny:.2E}"
-                   f"<br>max.z={maxz:.2E} | min.z={minz:.2E}")
+            txt = (
+                f"<b>Step {i + 1} {response}</b>"
+                f"<br>max.x={maxx:.2E} | min.x={minx:.2E}"
+                f"<br>max.y={maxy:.2E} | min.y={miny:.2E}"
+                f"<br>max.z={maxz:.2E} | min.z={minz:.2E}"
+            )
             step = dict(
                 method="update",
-                args=[{"visible": [False] * len(fig.data)},
-                      {"title": txt}],  # layout attribute
+                args=[
+                    {"visible": [False] * len(fig.data)},
+                    {"title": txt},
+                ],  # layout attribute
                 label=str(i + 1),
             )
             idxi, idxj = n_data * i, n_data * (i + 1)
             step["args"][0]["visible"][idxi:idxj] = [True] * n_data
             # Toggle i'th trace to "visible"
             steps.append(step)
-        sliders = [dict(
-            active=num_steps,
-            currentvalue={"prefix": "Step: "},
-            pad={"t": 50},
-            steps=steps
-        )]
+        sliders = [
+            dict(
+                active=num_steps,
+                currentvalue={"prefix": "Step: "},
+                pad={"t": 50},
+                steps=steps,
+            )
+        ]
         coloraxiss = {}
         for i in range(num_steps):
-            coloraxiss[f"coloraxis{i + 1}"] = dict(colorscale=obj.color_map,
-                                                   cmin=cmin,
-                                                   cmax=cmax,
-                                                   colorbar=dict(tickfont=dict(size=15)))
+            coloraxiss[f"coloraxis{i + 1}"] = dict(
+                colorscale=obj.color_map,
+                cmin=cmin,
+                cmax=cmax,
+                colorbar=dict(tickfont=dict(size=15)),
+            )
         if np.max(model_dims) <= 2:
-            eye = dict(x=0., y=-0.1, z=10)  # for 2D camera
-            scene = dict(camera=dict(
-                eye=eye, projection=dict(type="orthographic")))
+            eye = dict(x=0.0, y=-0.1, z=10)  # for 2D camera
+            scene = dict(camera=dict(eye=eye, projection=dict(type="orthographic")))
         else:
             eye = dict(x=-3.5, y=-3.5, z=3.5)  # for 3D camera
-            scene = dict(aspectratio=dict(x=1, y=1, z=1), aspectmode="data",
-                         camera=dict(eye=eye, projection=dict(
-                             type="orthographic")))
+            scene = dict(
+                aspectratio=dict(x=1, y=1, z=1),
+                aspectmode="data",
+                camera=dict(eye=eye, projection=dict(type="orthographic")),
+            )
         fig.update_layout(
             template=obj.theme,
             autosize=True,
             showlegend=False,
             scene=scene,  # orthographic,perspective
-            title=dict(font=dict(family="courier", color='black', size=25),
-                       text="<b>OpenSeesPy Deformation 3D View</b>"
-                       ),
+            title=dict(
+                font=dict(family="courier", color="black", size=25),
+                text="<b>OpenSeesPy Deformation 3D View</b>",
+            ),
             sliders=sliders,
-            **coloraxiss
+            **coloraxiss,
         )
     # -------------------------------------------------------------------------
     else:  # plot a single step
         step = max_step
         if model_update:
             node_nodeform_coords = model_info_steps["coord_no_deform"][step]
             lines_cells = _reshape_cell(cell_steps["all_lines"][step])
@@ -1174,81 +1658,93 @@
             faces_cells = _reshape_cell(cell_steps["all_faces"])
         node_resp = node_resp_steps[resp_type][step]
         node_deform_coords = alpha_ * node_resp + node_nodeform_coords
         if show_origin:
             points_origin = node_nodeform_coords
         else:
             points_origin = None
-        scalars = np.sqrt(np.sum(node_resp ** 2, axis=1))
-        plotter = _generate_all_mesh(points=node_deform_coords, scalars=scalars,
-                                     point_size=obj.point_size, line_width=obj.line_width,
-                                     opacity=opacity,
-                                     lines_cells=lines_cells,
-                                     face_cells=faces_cells,
-                                     coloraxis="coloraxis",
-                                     points_origin=points_origin,
-                                     show_face_line=show_face_line)
+        scalars = np.sqrt(np.sum(node_resp**2, axis=1))
+        plotter = _generate_all_mesh(
+            points=node_deform_coords,
+            scalars=scalars,
+            point_size=obj.point_size,
+            line_width=obj.line_width,
+            opacity=opacity,
+            lines_cells=lines_cells,
+            face_cells=faces_cells,
+            coloraxis="coloraxis",
+            points_origin=points_origin,
+            show_face_line=show_face_line,
+        )
         fig.add_traces(plotter)
         if np.max(np.abs(node_deform_coords[:, -1])) < 1e-5:
-            eye = dict(x=0., y=-0.1, z=10)  # for 2D camera
-            scene = dict(camera=dict(
-                eye=eye, projection=dict(type="orthographic")))
+            eye = dict(x=0.0, y=-0.1, z=10)  # for 2D camera
+            scene = dict(camera=dict(eye=eye, projection=dict(type="orthographic")))
         else:
             eye = dict(x=-3.5, y=-3.5, z=3.5)  # for 3D camera
-            scene = dict(aspectratio=dict(x=1, y=1, z=1), aspectmode="data",
-                         camera=dict(eye=eye, projection=dict(
-                             type="orthographic")))
+            scene = dict(
+                aspectratio=dict(x=1, y=1, z=1),
+                aspectmode="data",
+                camera=dict(eye=eye, projection=dict(type="orthographic")),
+            )
         maxx, maxy, maxz = np.max(node_resp, axis=0)
         minx, miny, minz = np.min(node_resp, axis=0)
-        txt = (f"<br>Step {max_step + 1} {response}"
-               f"<br>max.x={maxx:.2E} | min.x={minx:.2E}"
-               f"<br>max.y={maxy:.2E} | min.y={miny:.2E}"
-               f"<br>max.z={maxz:.2E} | min.z={minz:.2E}")
+        txt = (
+            f"<br>Step {max_step + 1} {response}"
+            f"<br>max.x={maxx:.2E} | min.x={minx:.2E}"
+            f"<br>max.y={maxy:.2E} | min.y={miny:.2E}"
+            f"<br>max.z={maxz:.2E} | min.z={minz:.2E}"
+        )
         fig.update_layout(
             template=obj.theme,
             autosize=True,
             showlegend=False,
             scene=scene,
-            coloraxis=dict(colorscale=obj.color_map, cmin=cmin, cmax=cmax,
-                           colorbar=dict(tickfont=dict(size=15))),
-            title=dict(font=dict(family="courier", color='black', size=25),
-                       text="<b>OpenSeesPy Deformation 3D View</b>" + txt
-                       ),
+            coloraxis=dict(
+                colorscale=obj.color_map,
+                cmin=cmin,
+                cmax=cmax,
+                colorbar=dict(tickfont=dict(size=15)),
+            ),
+            title=dict(
+                font=dict(family="courier", color="black", size=25),
+                text="<b>OpenSeesPy Deformation 3D View</b>" + txt,
+            ),
         )
     if not show_outline:
         fig.update_layout(
-            scene=dict(xaxis={'showgrid': False, 'zeroline': False, 'visible': False},
-                       yaxis={'showgrid': False,
-                              'zeroline': False, 'visible': False},
-                       zaxis={'showgrid': False, 'zeroline': False, 'visible': False}, ),
+            scene=dict(
+                xaxis={"showgrid": False, "zeroline": False, "visible": False},
+                yaxis={"showgrid": False, "zeroline": False, "visible": False},
+                zaxis={"showgrid": False, "zeroline": False, "visible": False},
+            ),
         )
     if save_html:
         if not save_html.endswith(".html"):
             save_html += ".html"
         pio.write_html(fig, file=save_html, auto_open=True)
-    if obj.notebook:
-        fig.show()
+    return fig
 
 
 def _deform_anim(
-        obj,
-        input_file: str = "NodeRespStepData-1.hdf5",
-        response: str = "disp",
-        alpha: float = None,
-        show_outline: bool = False,
-        opacity: float = 1,
-        framerate: int = 24,
-        show_face_line: bool = True,
-        save_html: str = "DefoAnimation",
-        model_update: bool = False
+    obj,
+    input_file: str = "NodeRespStepData-1.hdf5",
+    response: str = "disp",
+    alpha: float = 1.0,
+    show_outline: bool = False,
+    opacity: float = 1,
+    framerate: int = 24,
+    show_face_line: bool = True,
+    save_html: str = "DefoAnimation",
+    model_update: bool = False,
 ):
     resp_type = response.lower()
-    if resp_type not in ['disp', 'vel', 'accel']:
+    if resp_type not in ["disp", "vel", "accel"]:
         raise ValueError("response must be 'disp', 'vel', or 'accel'!")
-    filename = obj.out_dir + '/' + input_file
+    filename = obj.out_dir + "/" + input_file
     model_info_steps = dict()
     cell_steps = dict()
     node_resp_steps = dict()
     with h5py.File(filename, "r") as f:
         n = int(f["Nsteps"][...])
         grp1 = f["ModelInfoSteps"]
         grp2 = f["CellSteps"]
@@ -1275,36 +1771,37 @@
                 temp.append(value_[f"step{i + 1}"][...])
             node_resp_steps[name] = temp
 
     num_steps = len(node_resp_steps["disp"])
     times = int(num_steps / framerate)
 
     # ! max response
-    max_resps = [np.max(np.sqrt(np.sum(resp_ ** 2, axis=1)))
-                 for resp_ in node_resp_steps[resp_type]]
+    max_resps = [
+        np.max(np.sqrt(np.sum(resp_**2, axis=1)))
+        for resp_ in node_resp_steps[resp_type]
+    ]
     max_step = np.argmax(max_resps)
     max_node_resp = node_resp_steps[resp_type][max_step]
-    scalars = np.sqrt(np.sum(max_node_resp ** 2, axis=1))
+    scalars = np.sqrt(np.sum(max_node_resp**2, axis=1))
     data = node_resp_steps[resp_type]
     cmin, cmax = np.min(scalars), np.max(scalars)
     if model_update:
         bounds = model_info_steps["bound"][0]
         model_dims = model_info_steps["model_dims"][0]
     else:
         bounds = model_info_steps["bound"]
         model_dims = model_info_steps["model_dims"]
     # scale factor
     if resp_type == "disp":
-        if alpha is None:
-            max_bound = np.max(
-                [bounds[1] - bounds[0], bounds[3] - bounds[2], bounds[5] - bounds[4]])
-            value = np.max(np.sqrt(np.sum(max_node_resp ** 2, axis=1)))
-            alpha_ = max_bound / obj.bound_fact / value
-        else:
-            alpha_ = alpha
+        max_bound = np.max(
+            [bounds[1] - bounds[0], bounds[3] - bounds[2], bounds[5] - bounds[4]]
+        )
+        value = np.max(np.sqrt(np.sum(max_node_resp**2, axis=1)))
+        alpha_ = max_bound / obj.bound_fact / value
+        alpha_ *= alpha if alpha else alpha_
     else:
         alpha_ = 0
 
     # -----------------------------------------------------------------------------
     # start plot
     def create_mesh(stepi):
         if model_update:
@@ -1313,22 +1810,26 @@
             faces_cells_ = _reshape_cell(cell_steps["all_faces"][stepi])
         else:
             node_nodeform_coords_ = model_info_steps["coord_no_deform"]
             lines_cells_ = _reshape_cell(cell_steps["all_lines"])
             faces_cells_ = _reshape_cell(cell_steps["all_faces"])
         node_resp_ = node_resp_steps[resp_type][stepi]
         node_deform_coords_ = alpha_ * node_resp_ + node_nodeform_coords_
-        scalars_ = np.sqrt(np.sum(node_resp_ ** 2, axis=1))
-        plotter_ = _generate_all_mesh(points=node_deform_coords_, scalars=scalars_,
-                                      point_size=obj.point_size, line_width=obj.line_width,
-                                      opacity=opacity,
-                                      lines_cells=lines_cells_,
-                                      face_cells=faces_cells_,
-                                      coloraxis="coloraxis",
-                                      show_face_line=show_face_line)
+        scalars_ = np.sqrt(np.sum(node_resp_**2, axis=1))
+        plotter_ = _generate_all_mesh(
+            points=node_deform_coords_,
+            scalars=scalars_,
+            point_size=obj.point_size,
+            line_width=obj.line_width,
+            opacity=opacity,
+            lines_cells=lines_cells_,
+            face_cells=faces_cells_,
+            coloraxis="coloraxis",
+            show_face_line=show_face_line,
+        )
         return plotter_
 
     frames = []
     for step in range(num_steps):
         plotter = create_mesh(step)
         frames.append(go.Frame(data=plotter, name="step:" + str(step + 1)))
 
@@ -1361,40 +1862,47 @@
             ],
         }
     ]
     # Layout
     for i in range(len(fig.frames)):
         maxx, maxy, maxz = np.max(data[i], axis=0)
         minx, miny, minz = np.min(data[i], axis=0)
-        txt = ("<b>OpenSeesPy Defo 3D View</b>"
-               f"<br>Step {i + 1} {response}"
-               f"<br>max.x={maxx:.2E} | min.x={minx:.2E}"
-               f"<br>max.y={maxy:.2E} | min.y={miny:.2E}"
-               f"<br>max.z={maxz:.2E} | min.z={minz:.2E}")
-        fig.frames[i]['layout'].update(title_text=txt)
+        txt = (
+            "<b>OpenSeesPy Defo 3D View</b>"
+            f"<br>Step {i + 1} {response}"
+            f"<br>max.x={maxx:.2E} | min.x={minx:.2E}"
+            f"<br>max.y={maxy:.2E} | min.y={miny:.2E}"
+            f"<br>max.z={maxz:.2E} | min.z={minz:.2E}"
+        )
+        fig.frames[i]["layout"].update(title_text=txt)
     if np.max(model_dims) < 3:
-        eye = dict(x=0., y=-0.1, z=10)  # for 2D camera
-        scene = dict(camera=dict(
-            eye=eye, projection=dict(type="orthographic")))
+        eye = dict(x=0.0, y=-0.1, z=10)  # for 2D camera
+        scene = dict(camera=dict(eye=eye, projection=dict(type="orthographic")))
     else:
         eye = dict(x=-3.5, y=-3.5, z=3.5)  # for 3D camera
-        scene = dict(aspectratio=dict(x=1, y=1, z=1), aspectmode="data",
-                     camera=dict(eye=eye, projection=dict(
-                         type="orthographic")))
+        scene = dict(
+            aspectratio=dict(x=1, y=1, z=1),
+            aspectmode="data",
+            camera=dict(eye=eye, projection=dict(type="orthographic")),
+        )
 
     fig.update_layout(
-        title=dict(font=dict(family="courier", color='black', size=25),
-                   text="<b>OpenSeesPy Defo 3D View</b>"),
+        title=dict(
+            font=dict(family="courier", color="black", size=25),
+            text="<b>OpenSeesPy Defo 3D View</b>",
+        ),
         template=obj.theme,
         autosize=True,
         showlegend=False,
-        coloraxis=dict(colorscale=obj.color_map,
-                       cmin=cmin,
-                       cmax=cmax,
-                       colorbar=dict(tickfont=dict(size=15))),
+        coloraxis=dict(
+            colorscale=obj.color_map,
+            cmin=cmin,
+            cmax=cmax,
+            colorbar=dict(tickfont=dict(size=15)),
+        ),
         scene=scene,
         updatemenus=[
             {
                 "buttons": [
                     {
                         "args": [None, frame_args(times)],
                         "label": "&#9654;",  # play symbol
@@ -1409,43 +1917,44 @@
                 "direction": "left",
                 "pad": {"r": 10, "t": 70},
                 "type": "buttons",
                 "x": 0.1,
                 "y": 0,
             }
         ],
-        sliders=sliders
+        sliders=sliders,
     )
     if not show_outline:
         fig.update_layout(
-            scene=dict(xaxis={'showgrid': False, 'zeroline': False, 'visible': False},
-                       yaxis={'showgrid': False,
-                              'zeroline': False, 'visible': False},
-                       zaxis={'showgrid': False, 'zeroline': False, 'visible': False}, ),
+            scene=dict(
+                xaxis={"showgrid": False, "zeroline": False, "visible": False},
+                yaxis={"showgrid": False, "zeroline": False, "visible": False},
+                zaxis={"showgrid": False, "zeroline": False, "visible": False},
+            ),
         )
 
     if save_html:
         if not save_html.endswith(".html"):
             save_html += ".html"
         pio.write_html(fig, file=save_html, auto_open=True)
-    if obj.notebook:
-        fig.show()
+    return fig
 
 
-def _frame_resp_vis(obj,
-                    input_file: str = "BeamRespStepData-1.hdf5",
-                    ele_tags: list = None,
-                    slider: bool = False,
-                    response: str = "Mz",
-                    show_values=True,
-                    alpha: float = None,
-                    opacity: float = 1,
-                    save_html: str = "FrameRespVis"
-                    ):
-    filename = obj.out_dir + '/' + input_file
+def _frame_resp_vis(
+    obj,
+    input_file: str = "BeamRespStepData-1.hdf5",
+    ele_tags: list = None,
+    slider: bool = False,
+    response: str = "Mz",
+    show_values=True,
+    alpha: float = 1.0,
+    opacity: float = 1,
+    save_html: str = "FrameRespVis",
+):
+    filename = obj.out_dir + "/" + input_file
     beam_infos = dict()
     beam_resp_step = dict()
     with h5py.File(filename, "r") as f:
         n = int(f["Nsteps"][...])
         grp1 = f["BeamInfos"]
         for name, value_ in grp1.items():
             beam_infos[name] = value_[...]
@@ -1453,75 +1962,81 @@
         for name, value_ in grp2.items():
             temp = []
             for i in range(n):
                 temp.append(value_[f"step{i + 1}"][...])
             beam_resp_step[name] = temp
 
     # -------------------------------------
-    beam_tags = beam_infos['beam_tags']
+    beam_tags = beam_infos["beam_tags"]
     if len(beam_tags) == 0:
         warnings.warn("Model has no frame elements!")
         return None
-    ylocals = beam_infos['ylocal']
-    zlocals = beam_infos['zlocal']
+    ylocals = beam_infos["ylocal"]
+    zlocals = beam_infos["zlocal"]
     ylocal_map = {beam_tags[i]: ylocals[i] for i in range(len(beam_tags))}
     zlocal_map = {beam_tags[i]: zlocals[i] for i in range(len(beam_tags))}
-    local_forces_step = beam_resp_step['localForces']
+    local_forces_step = beam_resp_step["localForces"]
     num_steps = len(local_forces_step)
 
     if ele_tags is None:
         ele_tags = beam_tags
-        beam_node_coords = beam_infos['beam_node_coords']
-        beam_cells = beam_infos['beam_cells']
+        beam_node_coords = beam_infos["beam_node_coords"]
+        beam_cells = beam_infos["beam_cells"]
         beam_cell_map = {beam_tags[i]: i for i in range(len(beam_tags))}
         idxs = range(len(beam_tags))
     else:
         ele_tags = np.atleast_1d(ele_tags)
         beam_node_coords = []
         beam_cells = []
         idxs = []
         beam_cell_map = {}
         for i, eletag in enumerate(ele_tags):
-            idx = beam_infos['beam_cell_map'][eletag]
+            idx = beam_infos["beam_cell_map"][eletag]
             idxs.append(idx)
             beam_cell_map[eletag] = i
-            nodei, nodej = beam_infos['beam_cells'][idx, 1:]
-            beam_node_coords.append(beam_infos['beam_node_coords'][nodei])
-            beam_node_coords.append(beam_infos['beam_node_coords'][nodej])
+            nodei, nodej = beam_infos["beam_cells"][idx, 1:]
+            beam_node_coords.append(beam_infos["beam_node_coords"][nodei])
+            beam_node_coords.append(beam_infos["beam_node_coords"][nodej])
             beam_cells.append([2, 2 * i, 2 * i + 1])
         beam_node_coords = np.array(beam_node_coords)
         beam_cells = np.array(beam_cells)
 
-    idx_plottype_map = dict(fx=[0, 6], fy=[1, 7], fz=[2, 8],
-                            my=[4, 10], mz=[5, 11], mx=[3, 9])
-    f_sign_map = dict(fx=[-1, 1], fy=[-1, 1], fz=[-1, 1],
-                      my=[1, -1], mz=[-1, 1], mx=[1, -1])
-    axis_sign_map = dict(fx=1, fy=1, fz=1,
-                         my=-1, mz=-1, mx=-1)
-    axis_map_map = dict(fx=zlocal_map, fy=ylocal_map, fz=zlocal_map,
-                        my=zlocal_map, mz=ylocal_map, mx=zlocal_map)
+    idx_plottype_map = dict(
+        fx=[0, 6], fy=[1, 7], fz=[2, 8], my=[4, 10], mz=[5, 11], mx=[3, 9]
+    )
+    f_sign_map = dict(
+        fx=[-1, 1], fy=[-1, 1], fz=[-1, 1], my=[1, -1], mz=[-1, 1], mx=[1, -1]
+    )
+    axis_sign_map = dict(fx=1, fy=1, fz=1, my=-1, mz=-1, mx=-1)
+    axis_map_map = dict(
+        fx=zlocal_map,
+        fy=ylocal_map,
+        fz=zlocal_map,
+        my=zlocal_map,
+        mz=ylocal_map,
+        mx=zlocal_map,
+    )
     idx_plottype = idx_plottype_map[response.lower()]
     axis_map = axis_map_map[response.lower()]
     axis_sign = axis_sign_map[response.lower()]
-    local_forces_step = [data[:, idx_plottype][idxs] * np.array(f_sign_map[response.lower()])
-                         for data in local_forces_step]  # new
+    local_forces_step = [
+        data[:, idx_plottype][idxs] * np.array(f_sign_map[response.lower()])
+        for data in local_forces_step
+    ]  # new
 
-    maxv = [np.max(np.abs(data))
-            for data in local_forces_step]
+    maxv = [np.max(np.abs(data)) for data in local_forces_step]
     maxstep = np.argmax(maxv)
     local_forces_max = local_forces_step[maxstep]
     cmin, cmax = np.min(local_forces_max), np.max(local_forces_max)
-    if alpha is None:
-        max_coord = np.max(beam_node_coords, axis=0)
-        min_coord = np.min(beam_node_coords, axis=0)
-        max_bound = np.max(max_coord - min_coord)
-        maxv = np.amax(np.abs(local_forces_max))
-        alpha_ = max_bound / maxv / obj.bound_fact
-    else:
-        alpha_ = alpha
+    max_coord = np.max(beam_node_coords, axis=0)
+    min_coord = np.min(beam_node_coords, axis=0)
+    max_bound = np.max(max_coord - min_coord)
+    maxv = np.amax(np.abs(local_forces_max))
+    alpha_ = max_bound / maxv / obj.bound_fact
+    alpha_ *= alpha if alpha else alpha_
 
     # ------------------------------------------------------------------------
     fig = go.Figure()
     # -------------------------------------------------------------------------
     if slider:
         n_data = None
         for step in range(num_steps):
@@ -1549,31 +2064,47 @@
                     resp_points.extend([coord1, coord2, coord3, coord4])
                     resp_cells.append([4, n, n + 1, n + 2, n + 3])
                     scalars.extend([f1_, f2_, f2_, f1_])
                 else:
                     ratio = np.abs(f2 / f1)
                     ratio = 1 / (ratio + 1)
                     coord0 = coord1 + (coord2 - coord1) * ratio
-                    resp_points.extend(
-                        [coord1, coord0, coord4, coord2, coord0, coord3])
+                    resp_points.extend([coord1, coord0, coord4, coord2, coord0, coord3])
                     resp_cells.append([3, n, n + 1, n + 2])
                     resp_cells.append([3, n + 3, n + 4, n + 5])
                     scalars.extend([f1_, 0, f1_, f2_, 0, f2_])
             labels = [f"{label:.2E}" for label in labels]
             label_poins = np.array(label_poins)
             resp_points = np.array(resp_points)
             scalars = np.array(scalars)
             # ----------------------------------------------------------------------------------------
-            line_plot = _generate_line_mesh(beam_node_coords, beam_cells, line_width=obj.line_width,
-                                            color="black", use_cmap=False)
-            resp_plot = _generate_face_mesh(resp_points, resp_cells, show_face_line=False, opacity=opacity,
-                                            use_cmap=True, scalars=scalars, coloraxis="coloraxis")
-            point_plot = _generate_point_mesh(resp_points, point_size=obj.point_size / 2,
-                                              use_cmap=True, hover_name=response,
-                                              scalars=scalars, coloraxis="coloraxis")
+            line_plot = _generate_line_mesh(
+                beam_node_coords,
+                beam_cells,
+                line_width=obj.line_width,
+                color="black",
+                use_cmap=False,
+            )
+            resp_plot = _generate_face_mesh(
+                resp_points,
+                resp_cells,
+                show_face_line=False,
+                opacity=opacity,
+                use_cmap=True,
+                scalars=scalars,
+                coloraxis="coloraxis",
+            )
+            point_plot = _generate_point_mesh(
+                resp_points,
+                point_size=obj.point_size / 2,
+                use_cmap=True,
+                hover_name=response,
+                scalars=scalars,
+                coloraxis="coloraxis",
+            )
             # resp_plot = _generate_line_mesh(resp_points, resp_cells, line_width=obj.line_width,
             #                                 use_cmap=True, scalars=scalars, coloraxis="coloraxis")
             fig.add_traces(line_plot + resp_plot + point_plot)
             if show_values:
                 txt_plot = go.Scatter3d(
                     x=label_poins[:, 0],
                     y=label_poins[:, 1],
@@ -1589,58 +2120,67 @@
         for i in range(0, len(fig.data) - n_data):
             fig.data[i].visible = False
         # ! Create and add slider
         steps = []
         for i in range(num_steps):
             maxx = np.max(local_forces_step[i])
             minx = np.min(local_forces_step[i])
-            txt = (f"<b>Step {i + 1} {response}</b>"
-                   f"<br>max.={maxx:.2E}|min.={minx:.2E}")
+            txt = (
+                f"<b>Step {i + 1} {response}</b>" f"<br>max.={maxx:.2E}|min.={minx:.2E}"
+            )
             step = dict(
                 method="update",
-                args=[{"visible": [False] * len(fig.data)},
-                      {"title": txt}],  # layout attribute
+                args=[
+                    {"visible": [False] * len(fig.data)},
+                    {"title": txt},
+                ],  # layout attribute
                 label=str(i + 1),
             )
             idxi, idxj = n_data * i, n_data * (i + 1)
             step["args"][0]["visible"][idxi:idxj] = [True] * n_data
             # Toggle i'th trace to "visible"
             steps.append(step)
-        sliders = [dict(
-            active=num_steps,
-            currentvalue={"prefix": "Step: "},
-            pad={"t": 50},
-            steps=steps
-        )]
+        sliders = [
+            dict(
+                active=num_steps,
+                currentvalue={"prefix": "Step: "},
+                pad={"t": 50},
+                steps=steps,
+            )
+        ]
         coloraxiss = {}
         for i in range(num_steps):
-            coloraxiss[f"coloraxis{i + 1}"] = dict(colorscale=obj.color_map,
-                                                   cmin=cmin,
-                                                   cmax=cmax,
-                                                   colorbar=dict(tickfont=dict(size=15)))
+            coloraxiss[f"coloraxis{i + 1}"] = dict(
+                colorscale=obj.color_map,
+                cmin=cmin,
+                cmax=cmax,
+                colorbar=dict(tickfont=dict(size=15)),
+            )
 
         if np.max(np.abs(beam_node_coords[:, -1])) < 1e-5:
-            eye = dict(x=0., y=-0.1, z=10)  # for 2D camera
-            scene = dict(camera=dict(
-                eye=eye, projection=dict(type="orthographic")))
+            eye = dict(x=0.0, y=-0.1, z=10)  # for 2D camera
+            scene = dict(camera=dict(eye=eye, projection=dict(type="orthographic")))
         else:
             eye = dict(x=-3.5, y=-3.5, z=3.5)  # for 3D camera
-            scene = dict(aspectratio=dict(x=1, y=1, z=1), aspectmode="data",
-                         camera=dict(eye=eye, projection=dict(
-                             type="orthographic")))
+            scene = dict(
+                aspectratio=dict(x=1, y=1, z=1),
+                aspectmode="data",
+                camera=dict(eye=eye, projection=dict(type="orthographic")),
+            )
         fig.update_layout(
             template=obj.theme,
             autosize=True,
             showlegend=False,
             scene=scene,
-            title=dict(font=dict(family="courier", color='black', size=25),
-                       text="<b>OpenSeesPy Frames Response 3D View</b>"
-                       ),
+            title=dict(
+                font=dict(family="courier", color="black", size=25),
+                text="<b>OpenSeesPy Frames Response 3D View</b>",
+            ),
             sliders=sliders,
-            **coloraxiss
+            **coloraxiss,
         )
     # -------------------------------------------------------------------------
     else:  # plot a single step
         local_forces = local_forces_step[maxstep]
         local_forces_scale = local_forces * alpha_
         # add force face cells
         # TODO if values symbol versa, need trangle
@@ -1664,31 +2204,47 @@
                 resp_points.extend([coord1, coord2, coord3, coord4])
                 resp_cells.append([4, n, n + 1, n + 2, n + 3])
                 scalars.extend([f1_, f2_, f2_, f1_])
             else:
                 ratio = np.abs(f2 / f1)
                 ratio = 1 / (ratio + 1)
                 coord0 = coord1 + (coord2 - coord1) * ratio
-                resp_points.extend(
-                    [coord1, coord0, coord4, coord2, coord0, coord3])
+                resp_points.extend([coord1, coord0, coord4, coord2, coord0, coord3])
                 resp_cells.append([3, n, n + 1, n + 2])
                 resp_cells.append([3, n + 3, n + 4, n + 5])
                 scalars.extend([f1_, 0, f1_, f2_, 0, f2_])
         labels = [f"{label:.2E}" for label in labels]
         label_poins = np.array(label_poins)
         resp_points = np.array(resp_points)
         scalars = np.array(scalars)
         # ----------------------------------------------------------------------------------------
-        line_plot = _generate_line_mesh(beam_node_coords, beam_cells, line_width=obj.line_width,
-                                        color="black", use_cmap=False)
-        resp_plot = _generate_face_mesh(resp_points, resp_cells, show_face_line=False, opacity=opacity,
-                                        use_cmap=True, scalars=scalars, coloraxis="coloraxis")
-        point_plot = _generate_point_mesh(resp_points, point_size=obj.point_size / 2,
-                                          use_cmap=True, hover_name=response,
-                                          scalars=scalars, coloraxis="coloraxis")
+        line_plot = _generate_line_mesh(
+            beam_node_coords,
+            beam_cells,
+            line_width=obj.line_width,
+            color="black",
+            use_cmap=False,
+        )
+        resp_plot = _generate_face_mesh(
+            resp_points,
+            resp_cells,
+            show_face_line=False,
+            opacity=opacity,
+            use_cmap=True,
+            scalars=scalars,
+            coloraxis="coloraxis",
+        )
+        point_plot = _generate_point_mesh(
+            resp_points,
+            point_size=obj.point_size / 2,
+            use_cmap=True,
+            hover_name=response,
+            scalars=scalars,
+            coloraxis="coloraxis",
+        )
         # resp_plot = _generate_line_mesh(resp_points, resp_cells, line_width=obj.line_width,
         #                                 use_cmap=True, scalars=scalars, coloraxis="coloraxis")
         fig.add_traces(line_plot + resp_plot + point_plot)
         if show_values:
             txt_plot = go.Scatter3d(
                 x=label_poins[:, 0],
                 y=label_poins[:, 1],
@@ -1696,81 +2252,102 @@
                 text=labels,
                 textfont=dict(color="#6e750e", size=8),
                 mode="text",
                 name=f"{response}",
             )
             fig.add_trace(txt_plot)
         if np.max(np.abs(beam_node_coords[:, -1])) < 1e-5:
-            eye = dict(x=0., y=-0.1, z=10)  # for 2D camera
-            scene = dict(camera=dict(
-                eye=eye, projection=dict(type="orthographic")))
+            eye = dict(x=0.0, y=-0.1, z=10)  # for 2D camera
+            scene = dict(camera=dict(eye=eye, projection=dict(type="orthographic")))
         else:
             eye = dict(x=-3.5, y=-3.5, z=3.5)  # for 3D camera
-            scene = dict(aspectratio=dict(x=1, y=1, z=1), aspectmode="data",
-                         camera=dict(eye=eye, projection=dict(
-                             type="orthographic")))
+            scene = dict(
+                aspectratio=dict(x=1, y=1, z=1),
+                aspectmode="data",
+                camera=dict(eye=eye, projection=dict(type="orthographic")),
+            )
         maxx = np.max(local_forces)
         minx = np.min(local_forces)
-        txt = (f"<br>Step {maxstep + 1} {response}"
-               f"<br>max.={maxx:.2E} | min.={minx:.2E}")
+        txt = (
+            f"<br>Step {maxstep + 1} {response}"
+            f"<br>max.={maxx:.2E} | min.={minx:.2E}"
+        )
         fig.update_layout(
             template=obj.theme,
             autosize=True,
             showlegend=False,
             scene=scene,
-            coloraxis=dict(colorscale=obj.color_map, cmin=cmin, cmax=cmax,
-                           colorbar=dict(tickfont=dict(size=15))),
-            title=dict(font=dict(family="courier", color='black', size=25),
-                       text="<b>OpenSeesPy Frames Response 3D View</b>" + txt
-                       ),
+            coloraxis=dict(
+                colorscale=obj.color_map,
+                cmin=cmin,
+                cmax=cmax,
+                colorbar=dict(tickfont=dict(size=15)),
+            ),
+            title=dict(
+                font=dict(family="courier", color="black", size=25),
+                text="<b>OpenSeesPy Frames Response 3D View</b>" + txt,
+            ),
         )
     fig.update_layout(
-        scene=dict(xaxis={'showgrid': False, 'zeroline': False, 'visible': False},
-                   yaxis={'showgrid': False,
-                          'zeroline': False, 'visible': False},
-                   zaxis={'showgrid': False, 'zeroline': False, 'visible': False}, ),
+        scene=dict(
+            xaxis={"showgrid": False, "zeroline": False, "visible": False},
+            yaxis={"showgrid": False, "zeroline": False, "visible": False},
+            zaxis={"showgrid": False, "zeroline": False, "visible": False},
+        ),
     )
     if save_html:
         if not save_html.endswith(".html"):
             save_html += ".html"
         pio.write_html(fig, file=save_html, auto_open=True)
-    if obj.notebook:
-        fig.show()
+    return fig
 
 
-def _generate_point_mesh(points, point_size=1, color='black',
-                         scalars=None, use_cmap=False, coloraxis=None,
-                         hover_name=''):
+def _generate_point_mesh(
+    points,
+    point_size=1,
+    color="black",
+    scalars=None,
+    use_cmap=False,
+    coloraxis=None,
+    hover_name="",
+):
     plotter = []
     if use_cmap:
         point_plot = go.Scatter3d(
             x=points[:, 0],
             y=points[:, 1],
             z=points[:, 2],
-            marker=dict(size=point_size, color=scalars,
-                        coloraxis=coloraxis),
+            marker=dict(size=point_size, color=scalars, coloraxis=coloraxis),
             mode="markers",
             name=hover_name,
             customdata=scalars,
-            hovertemplate='<b>%{customdata}</b>'
+            hovertemplate="<b>%{customdata}</b>"
             # hoverinfo="skip",
         )
     else:
         point_plot = go.Scatter3d(
             x=points[:, 0],
             y=points[:, 1],
             z=points[:, 2],
             marker=dict(size=point_size, color=color),
             mode="markers",
         )
     plotter.append(point_plot)
     return plotter
 
 
-def _generate_line_mesh(points, cells, line_width=1, color='blue', scalars=None, use_cmap=False, coloraxis=None):
+def _generate_line_mesh(
+    points,
+    cells,
+    line_width=1,
+    color="blue",
+    scalars=None,
+    use_cmap=False,
+    coloraxis=None,
+):
     """
     generate the mesh from the points and cell
     """
     points = np.array(points)
     cells = np.array(cells)
     plotter = []
     line_points = []
@@ -1781,17 +2358,21 @@
         data = np.vstack([data0, data1])
         line_points.extend(list(data))
         if use_cmap:
             line_scalars.extend(list(scalars[cell[1:]]) + [np.NAN])
     line_points = np.array(line_points)
     line_scalars = np.array(line_scalars)
     if use_cmap:
-        line_dict = dict(color=line_scalars, width=line_width,
-                         cmin=np.min(line_scalars), cmax=np.max(line_scalars),
-                         coloraxis=coloraxis)
+        line_dict = dict(
+            color=line_scalars,
+            width=line_width,
+            cmin=np.min(line_scalars),
+            cmax=np.max(line_scalars),
+            coloraxis=coloraxis,
+        )
     else:
         line_dict = dict(color=color, width=line_width)
     plt_obj = go.Scatter3d(
         x=line_points[:, 0],
         y=line_points[:, 1],
         z=line_points[:, 2],
         line=line_dict,
@@ -1799,17 +2380,25 @@
         connectgaps=False,
         hoverinfo="skip",
     )
     plotter.append(plt_obj)
     return plotter
 
 
-def _generate_face_mesh(points, cells, line_width=1,
-                        color='blue', scalars=None, use_cmap=False, coloraxis=None,
-                        show_face_line=False, opacity=0.75):
+def _generate_face_mesh(
+    points,
+    cells,
+    line_width=1,
+    color="blue",
+    scalars=None,
+    use_cmap=False,
+    coloraxis=None,
+    show_face_line=False,
+    opacity=0.75,
+):
     """
     generate the mesh from the points and cell
     """
     plotter = []
     face_line_points = []
     face_points = []
     face_scalars = []
@@ -1869,52 +2458,64 @@
         if use_cmap:
             face_scalars.extend(list(scalars[cell[1:]]))
     face_line_points = np.array(face_line_points)
     face_points = np.array(face_points)
     face_scalars = np.array(face_scalars)
     # plot new
     if use_cmap:
-        kargs = dict(text=face_scalars,
-                     intensity=face_scalars,
-                     cmin=np.min(scalars),
-                     cmax=np.max(scalars),
-                     coloraxis=coloraxis)
+        kargs = dict(
+            text=face_scalars,
+            intensity=face_scalars,
+            cmin=np.min(scalars),
+            cmax=np.max(scalars),
+            coloraxis=coloraxis,
+        )
     else:
         kargs = dict(color=color)
     plotter.append(
         go.Mesh3d(
             x=face_points[:, 0],
             y=face_points[:, 1],
             z=face_points[:, 2],
             i=veci,
             j=vecj,
             k=veck,
             opacity=opacity,
             hoverinfo="skip",
-            **kargs
+            **kargs,
         )
     )
     # face lines
     if show_face_line:
         plotter.append(
             go.Scatter3d(
                 x=face_line_points[:, 0],
                 y=face_line_points[:, 1],
                 z=face_line_points[:, 2],
-                line=dict(color='black', width=line_width / 2),
+                line=dict(color="black", width=line_width / 2),
                 mode="lines",
                 connectgaps=False,
                 hoverinfo="skip",
             )
         )
     return plotter
 
 
-def _generate_all_mesh(points, scalars, opacity, lines_cells, face_cells, point_size=1, line_width=1,
-                       points_origin=None, coloraxis="coloraxis", show_face_line=True):
+def _generate_all_mesh(
+    points,
+    scalars,
+    opacity,
+    lines_cells,
+    face_cells,
+    point_size=1,
+    line_width=1,
+    points_origin=None,
+    coloraxis="coloraxis",
+    show_face_line=True,
+):
     """
     Auxiliary function for generating all meshes
     """
     plotter = []
     # ------------------------------------------------------------------------
     # face plot
     if len(face_cells) > 0:
@@ -1989,15 +2590,15 @@
         # plot origin
         if points_origin is not None:
             plotter.append(
                 go.Scatter3d(
                     x=face_line_origin_points[:, 0],
                     y=face_line_origin_points[:, 1],
                     z=face_line_origin_points[:, 2],
-                    line=dict(color='gray', width=line_width / 2),
+                    line=dict(color="gray", width=line_width / 2),
                     mode="lines",
                     connectgaps=False,
                     hoverinfo="skip",
                 )
             )
         # plot new
         plotter.append(
@@ -2019,15 +2620,15 @@
         )
         if show_face_line:
             plotter.append(
                 go.Scatter3d(
                     x=face_line_points[:, 0],
                     y=face_line_points[:, 1],
                     z=face_line_points[:, 2],
-                    line=dict(color='black', width=line_width / 2),
+                    line=dict(color="black", width=line_width / 2),
                     mode="lines",
                     connectgaps=False,
                     hoverinfo="skip",
                 )
             )
     # ----------------------------
     # line plot
@@ -2052,57 +2653,59 @@
         # plot origin
         if points_origin is not None:
             plotter.append(
                 go.Scatter3d(
                     x=line_origin_points[:, 0],
                     y=line_origin_points[:, 1],
                     z=line_origin_points[:, 2],
-                    line=dict(color='gray', width=line_width / 2),
+                    line=dict(color="gray", width=line_width / 2),
                     mode="lines",
                     connectgaps=False,
                     hoverinfo="skip",
                 )
             )
         # plot new
         plotter.append(
             go.Scatter3d(
                 x=line_points[:, 0],
                 y=line_points[:, 1],
                 z=line_points[:, 2],
-                line=dict(color=line_scalars, width=line_width,
-                          cmin=np.min(scalars), cmax=np.max(scalars),
-                          coloraxis=coloraxis,
-                          ),
+                line=dict(
+                    color=line_scalars,
+                    width=line_width,
+                    cmin=np.min(scalars),
+                    cmax=np.max(scalars),
+                    coloraxis=coloraxis,
+                ),
                 text=line_scalars,
                 mode="lines",
                 connectgaps=False,
                 hoverinfo="skip",
             )
         )
     # ---------------------------------------
     # point plot
     point_plot = go.Scatter3d(
         x=points[:, 0],
         y=points[:, 1],
         z=points[:, 2],
-        marker=dict(size=point_size / 2, color=scalars,
-                    coloraxis=coloraxis),
+        marker=dict(size=point_size / 2, color=scalars, coloraxis=coloraxis),
         mode="markers",
-        name='',
+        name="",
         customdata=scalars,
-        hovertemplate='<b>%{customdata}</b>'
+        hovertemplate="<b>%{customdata}</b>"
         # hoverinfo="skip",
     )
     plotter.append(point_plot)
     return plotter
 
 
-def _creat_arrows(points, cells, color,
-                  arrow_tip_ratio=0.9, arrow_starting_ratio=1.0,
-                  anchor_tip=True):
+def _creat_arrows(
+    points, cells, color, arrow_tip_ratio=0.9, arrow_starting_ratio=1.0, anchor_tip=True
+):
     points = np.array(points)
     cells = np.array(cells)
     x, y, z = points[:, 0], points[:, 1], points[:, 2]
     x_, y_, z_ = [], [], []
     u, v, w = [], [], []
     for p in cells:
         x_.append(x[p[1]] + arrow_starting_ratio * (x[p[2]] - x[p[1]]))
@@ -2110,36 +2713,55 @@
         z_.append(z[p[1]] + arrow_starting_ratio * (z[p[2]] - z[p[1]]))
         u.append(arrow_tip_ratio * (x[p[2]] - x[p[1]]))
         v.append(arrow_tip_ratio * (y[p[2]] - y[p[1]]))
         w.append(arrow_tip_ratio * (z[p[2]] - z[p[1]]))
     arrow_plot = []
     for i in range(len(cells)):
         if anchor_tip:
-            arrow_plot.append(go.Cone(x=[x_[i]], y=[y_[i]], z=[z_[i]],
-                                      u=[u[i]], v=[v[i]], w=[w[i]],
-                                      sizemode="absolute",
-                                      anchor='tip', hoverinfo='skip',
-                                      showlegend=False, showscale=False,
-                                      colorscale=[[0, color], [1, color]]))
+            arrow_plot.append(
+                go.Cone(
+                    x=[x_[i]],
+                    y=[y_[i]],
+                    z=[z_[i]],
+                    u=[u[i]],
+                    v=[v[i]],
+                    w=[w[i]],
+                    sizemode="absolute",
+                    anchor="tip",
+                    hoverinfo="skip",
+                    showlegend=False,
+                    showscale=False,
+                    colorscale=[[0, color], [1, color]],
+                )
+            )
         else:
-            arrow_plot.append(go.Cone(x=[x_[i]], y=[y_[i]], z=[z_[i]],
-                                      u=[u[i]], v=[v[i]], w=[w[i]],
-                                      sizemode="absolute",
-                                      hoverinfo='skip',
-                                      showlegend=False, showscale=False,
-                                      colorscale=[[0, color], [1, color]]))
+            arrow_plot.append(
+                go.Cone(
+                    x=[x_[i]],
+                    y=[y_[i]],
+                    z=[z_[i]],
+                    u=[u[i]],
+                    v=[v[i]],
+                    w=[w[i]],
+                    sizemode="absolute",
+                    hoverinfo="skip",
+                    showlegend=False,
+                    showscale=False,
+                    colorscale=[[0, color], [1, color]],
+                )
+            )
     return arrow_plot
 
 
 def _reshape_cell(data):
     if len(data) > 0:
         i = 0
         data2 = []
         while True:
             n = data[i]
-            data2.append(data[i:i + n + 1])
+            data2.append(data[i : i + n + 1])
             i += n + 1
             if i >= len(data):
                 break
     else:
         data2 = []
     return data2
```

### Comparing `opstool-0.7.3/src/opstool/vis/_pyvista_base.py` & `opstool-0.8.0/src/opstool/vis/_pyvista_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,422 +1,703 @@
 import warnings
 
 import h5py
 import numpy as np
+import matplotlib.pyplot as plt
 import pyvista as pv
 
 from ..utils import check_file, shape_dict
 
 
 def _model_vis(
-        obj,
-        input_file: str = "ModelData.hdf5",
-        show_node_label: bool = False,
-        show_ele_label: bool = False,
-        show_local_crd: bool = False,
-        show_fix_node: bool = True,
-        show_constrain_dof: bool = False,
-        show_beam_sec: bool = False,
-        beam_sec_paras: dict = None,
-        label_size: float = 8,
-        show_outline: bool = True,
-        opacity: float = 1.0,
-        save_fig: str = 'ModelVis.svg'
+    obj,
+    input_file: str = "ModelData.hdf5",
+    show_node_label: bool = False,
+    show_ele_label: bool = False,
+    label_size: float = 10,
+    show_local_crd: bool = False,
+    local_crd_alpha: float = 1.0,
+    show_fix_node: bool = True,
+    fix_node_alpha: float = 1.0,
+    show_load: bool = False,
+    load_alpha: float = 1.0,
+    show_constrain_dof: bool = False,
+    show_beam_sec: bool = False,
+    beam_sec_paras: dict = None,
+    show_outline: bool = True,
+    opacity: float = 1.0,
+    save_fig: str = "ModelVis.svg",
 ):
-    filename = obj.out_dir + '/' + input_file
+    filename = obj.out_dir + "/" + input_file
     model_info = dict()
     cells = dict()
     with h5py.File(filename, "r") as f:
         grp1 = f["ModelInfo"]
         for name in grp1.keys():
             model_info[name] = grp1[name][...]
         grp2 = f["Cell"]
         for name in grp2.keys():
             cells[name] = grp2[name][...]
 
     plotter = pv.Plotter(notebook=obj.notebook, line_smoothing=True)
     _plot_model(obj, plotter, model_info, cells, opacity)
 
     txt = f"OpenSees 3D View\nNum. of Node:{model_info['num_node']}\nNum. of Ele:{model_info['num_ele']}"
-    plotter.add_text(txt, position="upper_right", font_size=10, font="courier")
+    plotter.add_text(txt, position="upper_right", font_size=12, font="courier")
     if show_outline:
-        if np.max(model_info["model_dims"]) <= 2:
-            show_zaxis = False
-        else:
-            show_zaxis = True
-        plotter.show_bounds(grid=False, location="outer",
-                            bounds=model_info["bound"], show_zaxis=show_zaxis)
+        show_zaxis = False if np.max(model_info["model_dims"]) <= 2 else True
+        plotter.show_bounds(
+            grid=False,
+            location="outer",
+            bounds=model_info["bound"],
+            show_zaxis=show_zaxis,
+        )
     if show_node_label:
         node_labels = ["N" + str(i) for i in model_info["NodeTags"]]
-        plotter.add_point_labels(model_info["coord_no_deform"], node_labels, text_color="white",
-                                 font_size=label_size, point_color=obj.color_point, bold=False,
-                                 render_points_as_spheres=True, point_size=1e-5, always_visible=True)
+        plotter.add_point_labels(
+            model_info["coord_no_deform"],
+            node_labels,
+            text_color="white",
+            font_size=label_size,
+            point_color=obj.color_point,
+            bold=False,
+            render_points_as_spheres=True,
+            point_size=1e-5,
+            always_visible=True,
+        )
     if show_ele_label:
         ele_labels = ["E" + str(i) for i in model_info["EleTags"]]
-        plotter.add_point_labels(model_info["coord_ele_midpoints"], ele_labels, text_color="#ff796c",
-                                 font_size=label_size, bold=False, always_visible=True)
+        plotter.add_point_labels(
+            model_info["coord_ele_midpoints"],
+            ele_labels,
+            text_color="#ff796c",
+            font_size=label_size,
+            bold=False,
+            always_visible=True,
+        )
     # local axes
     if show_local_crd:
-        _show_beam_local_axes(plotter, model_info)
-        _show_link_local_axes(plotter, model_info)
+        _show_beam_local_axes(
+            plotter, model_info, alpha=local_crd_alpha, label_size=label_size
+        )
+        _show_link_local_axes(
+            plotter, model_info, alpha=local_crd_alpha, label_size=label_size
+        )
     # fix nodes
     if show_fix_node:
-        _show_fix_node(plotter, model_info)
+        _show_fix_node(plotter, model_info, alpha=fix_node_alpha)
     if show_beam_sec:
-        beam_sec_paras_ = dict(color='#5170d7', opacity=0.25, texture=False)
+        beam_sec_paras_ = dict(color="#5170d7", opacity=0.25, texture=False)
         if beam_sec_paras is not None:
             beam_sec_paras_.update(beam_sec_paras)
         _show_beam_sec(plotter, model_info, cells, beam_sec_paras_)
     # mp constraint lines
     _show_mp_constraint(obj, plotter, model_info, show_constrain_dof)
+    if show_load:
+        _show_node_load(plotter, model_info, load_alpha)
+        _show_ele_load(plotter, model_info, load_alpha)
     plotter.add_axes()
     plotter.view_isometric()
     if np.max(model_info["model_dims"]) <= 2:
         plotter.view_xy(negative=False)
     if save_fig:
         plotter.save_graphic(save_fig)
-    plotter.enable_anti_aliasing('msaa')
+    plotter.enable_anti_aliasing("msaa")
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _show_mp_constraint(obj, plotter, model_info, show_dofs):
     points = model_info["ConstrainedCoords"]
     cells = model_info["ConstrainedCells"]
     midcoords = model_info["ConstrainedMidCoords"]
     dofs = model_info["ConstrainedDofs"]
     dofs = ["".join([str(k) for k in dof if k != -1]) for dof in dofs]
     if len(cells) > 0:
         mesh = _generate_mesh(points, cells, kind="line")
-        plotter.add_mesh(mesh, color=obj.color_constraint,
-                         render_lines_as_tubes=False, line_width=obj.line_width / 3)
+        plotter.add_mesh(
+            mesh,
+            color=obj.color_constraint,
+            render_lines_as_tubes=False,
+            line_width=obj.line_width / 3,
+        )
         if show_dofs:
-            plotter.add_point_labels(midcoords, dofs, text_color=obj.color_constraint,
-                                     font_size=12, bold=True, show_points=False,
-                                     always_visible=True, shape_opacity=0)
+            plotter.add_point_labels(
+                midcoords,
+                dofs,
+                text_color=obj.color_constraint,
+                font_size=12,
+                bold=True,
+                show_points=False,
+                always_visible=True,
+                shape_opacity=0,
+            )
 
 
 def _show_beam_sec(plotter, model_info, cells, paras):
     ext_points = model_info["line_sec_ext_points"]
     int_points = model_info["line_sec_int_points"]
     sec_points = model_info["line_sec_points"]
     ext_cells = cells["line_sec_ext"]
     int_cells = cells["line_sec_int"]
     sec_cells = cells["line_sec"]
-    if paras['texture']:
-        texture = pv.read_texture(paras['texture'])
+    if paras["texture"]:
+        texture = pv.read_texture(paras["texture"])
     else:
         texture = None
     if len(ext_cells) > 0:
-        ext = _generate_mesh(ext_points, ext_cells, kind='face')
+        ext = _generate_mesh(ext_points, ext_cells, kind="face")
         if texture is not None:
             ext.texture_map_to_plane(inplace=True)
-        plotter.add_mesh(ext, show_edges=False, color=paras['color'],
-                         opacity=paras['opacity'], texture=texture)
+        plotter.add_mesh(
+            ext,
+            show_edges=False,
+            color=paras["color"],
+            opacity=paras["opacity"],
+            texture=texture,
+        )
     if len(int_cells) > 0:
-        intt = _generate_mesh(int_points, int_cells, kind='face')
+        intt = _generate_mesh(int_points, int_cells, kind="face")
         if texture is not None:
             intt.texture_map_to_plane(inplace=True)
-        plotter.add_mesh(intt, show_edges=False, color=paras['color'],
-                         opacity=paras['opacity'], texture=texture)
+        plotter.add_mesh(
+            intt,
+            show_edges=False,
+            color=paras["color"],
+            opacity=paras["opacity"],
+            texture=texture,
+        )
     if len(sec_cells) > 0:
-        sec = _generate_mesh(sec_points, sec_cells, kind='face')
+        sec = _generate_mesh(sec_points, sec_cells, kind="face")
         if texture is not None:
             sec.texture_map_to_plane(inplace=True)
-        plotter.add_mesh(sec, show_edges=False, color=paras['color'],
-                         opacity=paras['opacity'], texture=texture)
+        plotter.add_mesh(
+            sec,
+            show_edges=False,
+            color=paras["color"],
+            opacity=paras["opacity"],
+            texture=texture,
+        )
+
 
+def _show_node_load(plotter, model_info, alpha: float = 1.0):
+    points = model_info["coord_no_deform"]
+    node_load_info = np.array(model_info["node_load_info"])
+    node_load_data = np.array(model_info["node_load_data"])
+    if len(node_load_info) == 0:
+        return None
+    loc, load_data = 0, []
+    for info in node_load_info:
+        ndm = info[2]
+        ndf = info[3]
+        data = node_load_data[loc : loc + ndf]
+        if ndm <= 2 and ndf <= 3:
+            load_data.append([data[0], data[1], 0])  # x, y
+        else:
+            load_data.append([data[0], data[1], data[2]])  # x, y, z
+        loc += ndf
+    load_data = np.array(load_data)
+    maxdata = np.max(np.abs(load_data))
+    beam_lengths = model_info["beam_lengths"]
+    if len(beam_lengths) > 0:
+        alpha_ = np.mean(beam_lengths) / maxdata / 2
+    else:
+        alpha_ = (model_info["max_bound"] + model_info["min_bound"]) / 20 / maxdata
+    alpha_ *= alpha
+    patterntags = np.unique(node_load_info[:, 0])
+    cmap = plt.get_cmap("Spectral")
+    colors = cmap(np.linspace(0, 1, len(patterntags)))
+    xyzlocals = [[1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]]
+    geom = pv.Arrow(
+        start=(-1.0, 0, 0), tip_length=0.25, tip_radius=0.1, shaft_radius=0.03
+    )
+    for p, ptag in enumerate(patterntags):
+        idx = np.abs(node_load_info[:, 0] - ptag) < 1e-3
+        coords = points[node_load_info[idx, -1]]
+        for i in range(3):
+            ply = pv.PolyData(coords)
+            data = np.ravel(load_data[idx, i])
+            ply["scalars"] = np.abs(data)
+            ply["vectors"] = np.reshape(xyzlocals[i] * len(coords), (-1, 3))
+            for j in range(len(ply["vectors"])):
+                ply["vectors"][j] *= np.sign(data[j])
+            glyphs = ply.glyph(
+                orient="vectors", scale="scalars", factor=alpha_, geom=geom
+            )
+            plotter.add_mesh(glyphs, show_scalar_bar=False, color=colors[p])
 
-def _show_beam_local_axes(plotter, model_info):
+
+def _show_ele_load(plotter, model_info, alpha: float = 1.0):
+    points = model_info["coord_no_deform"]
+    ele_load_info = model_info["ele_load_info"]
+    ele_load_data = model_info["ele_load_data"]
+    ele_load_locals = model_info["ele_load_locals"]
+    if len(ele_load_info) == 0:
+        return None
+    patterntags = np.unique(ele_load_info[:, 0])
+    new_points = []
+    new_locals = []
+    new_ptags = []
+    load_data = []
+    loc = 0
+    for i, info in enumerate(ele_load_info):
+        ptag, _, classtag, nidx1, nidx2 = info
+        coord1, coord2 = points[nidx1], points[nidx2]
+        local_axis = ele_load_locals[i]
+        if classtag == 3:  # beamUniform2D, Wya <Wxa>
+            wy, wx = ele_load_data[loc : loc + 2]
+            wz = 0.0
+            n = 11
+            xl = np.linspace(0, 1, n)
+            wx, wy, wz = [wx] * n, [wy] * n, [wz] * n
+            localaxis = [local_axis] * n
+            new_ptags.extend([ptag] * n)
+            loc += 2
+        elif classtag == 12:  # beamUniform2D, Wya <Wxa> <aL> <bL> <Wyb> <Wxb>
+            wya, wyb, wxa, wxb, al, bl = ele_load_data[loc : loc + 6]
+            n = int((bl - al) / 0.1) + 1
+            xl = np.linspace(al, bl, n)
+            wy = np.interp(xl, [0, 1], [wya, wyb])
+            wx = np.interp(xl, [0, 1], [wxa, wxb])
+            wz = wy * 0
+            localaxis = [local_axis] * n
+            new_ptags.extend([ptag] * n)
+            loc += 6
+        elif classtag == 5:  # beamUniform3D wy, wz, wx
+            wy, wz, wx = ele_load_data[loc : loc + 3]
+            n = 11
+            xl = np.linspace(0, 1, n)
+            wx, wy, wz = [wx] * n, [wy] * n, [wz] * n
+            localaxis = [local_axis] * n
+            new_ptags.extend([ptag] * n)
+            loc += 3
+        elif classtag == 4:  # beamPoint2D, Py xL <Px>
+            wy, wx, xl = ele_load_data[loc : loc + 3]
+            wz = 0
+            localaxis = [local_axis]
+            new_ptags.append(ptag)
+            loc += 3
+        elif classtag == 6:  # beamPoint3D, Py, Pz, x, N
+            wy, wz, wx, xl = ele_load_data[loc : loc + 4]
+            localaxis = [local_axis]
+            new_ptags.append(ptag)
+            loc += 4
+        else:
+            warnings.warn(
+                "Currently load visualization only supports-->"
+                "<beamUniform2D,beamUniform3D,beamPoint2D,beamPoint3D>!"
+            )
+        xs = np.interp(xl, [0, 1], [coord1[0], coord2[0]])
+        ys = np.interp(xl, [0, 1], [coord1[1], coord2[1]])
+        zs = np.interp(xl, [0, 1], [coord1[2], coord2[2]])
+        new_points.append(np.column_stack([xs, ys, zs]))
+        new_locals.append(localaxis)
+        load_data.append(np.column_stack([wx, wy, wz]))
+    new_points = np.vstack(new_points)
+    new_locals = np.vstack(new_locals)
+    load_data = np.vstack(load_data)
+    new_ptags = np.array(new_ptags)
+    maxdata = np.max(np.abs(load_data))
+    beam_lengths = model_info["beam_lengths"]
+    if len(beam_lengths) > 0:
+        alpha_ = np.mean(beam_lengths) / maxdata / 2
+    else:
+        alpha_ = (model_info["max_bound"] + model_info["min_bound"]) / 20 / maxdata
+    alpha_ *= alpha
+    cmap = plt.get_cmap("rainbow")
+    colors = cmap(np.linspace(0, 1, len(patterntags)))
+    geom = pv.Arrow(
+        start=(-1.0, 0, 0), tip_length=0.25, tip_radius=0.1, shaft_radius=0.03
+    )
+    for p, ptag in enumerate(patterntags):
+        idx = np.abs(new_ptags - ptag) < 1e-3
+        coords = new_points[idx]
+        for i in range(3):
+            ply = pv.PolyData(coords)
+            data = np.ravel(load_data[idx, i])
+            ply["scalars"] = np.abs(data)
+            ply["vectors"] = new_locals[idx, 3 * i : 3 * i + 3]
+            for j in range(len(ply["vectors"])):
+                ply["vectors"][j] *= np.sign(data[j])
+            glyphs = ply.glyph(
+                orient="vectors", scale="scalars", factor=alpha_, geom=geom
+            )
+            plotter.add_mesh(glyphs, show_scalar_bar=False, color=colors[p])
+
+
+def _show_beam_local_axes(
+    plotter, model_info, alpha: float = 1.0, label_size: float = 10
+):
     beam_xlocal = model_info["beam_xlocal"]
     beam_ylocal = model_info["beam_ylocal"]
     beam_zlocal = model_info["beam_zlocal"]
     beam_midpoints = model_info["beam_midpoints"]
     beam_lengths = model_info["beam_lengths"]
     if len(beam_lengths) > 0:
-        length = (np.max(beam_lengths) + np.min(beam_lengths)) / 20
-        _ = plotter.add_arrows(beam_midpoints, beam_xlocal,
-                               mag=length, color="#cf6275")
-        _ = plotter.add_arrows(beam_midpoints, beam_ylocal,
-                               mag=length, color="#04d8b2")
-        _ = plotter.add_arrows(beam_midpoints, beam_zlocal,
-                               mag=length, color="#9aae07")
+        length = np.mean(beam_lengths) / 6 * alpha
+        _ = plotter.add_arrows(beam_midpoints, beam_xlocal, mag=length, color="#cf6275")
+        _ = plotter.add_arrows(beam_midpoints, beam_ylocal, mag=length, color="#04d8b2")
+        _ = plotter.add_arrows(beam_midpoints, beam_zlocal, mag=length, color="#9aae07")
         plotter.add_point_labels(
             beam_midpoints + length * beam_xlocal,
-            ['x'] * beam_midpoints.shape[0],
+            ["x"] * beam_midpoints.shape[0],
+            font_size=label_size,
             text_color="#cf6275",
             bold=False,
             shape=None,
             render_points_as_spheres=True,
-            point_size=1.e-5,
+            point_size=1.0e-5,
             always_visible=True,
         )
         plotter.add_point_labels(
             beam_midpoints + length * beam_ylocal,
-            ['y'] * beam_midpoints.shape[0],
+            ["y"] * beam_midpoints.shape[0],
+            font_size=label_size,
             text_color="#04d8b2",
             bold=False,
             shape=None,
             render_points_as_spheres=True,
-            point_size=1.e-5,
+            point_size=1.0e-5,
             always_visible=True,
         )
         plotter.add_point_labels(
             beam_midpoints + length * beam_zlocal,
-            ['z'] * beam_midpoints.shape[0],
+            ["z"] * beam_midpoints.shape[0],
+            font_size=label_size,
             text_color="#9aae07",
             bold=False,
             shape=None,
             render_points_as_spheres=True,
-            point_size=1.e-5,
+            point_size=1.0e-5,
             always_visible=True,
         )
     else:
         warnings.warn("Model has no frame elements when show_local_crd=True!")
 
 
-def _show_link_local_axes(plotter, model_info):
+def _show_link_local_axes(
+    plotter, model_info, alpha: float = 1.0, label_size: float = 10
+):
     link_xlocal = model_info["link_xlocal"]
     link_ylocal = model_info["link_ylocal"]
     link_zlocal = model_info["link_zlocal"]
     link_midpoints = model_info["link_midpoints"]
     link_lengths = model_info["link_lengths"]
     if len(link_midpoints) > 0:
-        length = (np.max(link_lengths) + np.min(link_lengths)) / 6
-        _ = plotter.add_arrows(link_midpoints, link_xlocal,
-                               mag=length, color="#cf6275")
-        _ = plotter.add_arrows(link_midpoints, link_ylocal,
-                               mag=length, color="#04d8b2")
-        _ = plotter.add_arrows(link_midpoints, link_zlocal,
-                               mag=length, color="#9aae07")
+        length = np.mean(link_lengths) / 6 * alpha
+        _ = plotter.add_arrows(link_midpoints, link_xlocal, mag=length, color="#cf6275")
+        _ = plotter.add_arrows(link_midpoints, link_ylocal, mag=length, color="#04d8b2")
+        _ = plotter.add_arrows(link_midpoints, link_zlocal, mag=length, color="#9aae07")
         plotter.add_point_labels(
             link_midpoints + length * link_xlocal,
-            ['x'] * link_midpoints.shape[0],
+            ["x"] * link_midpoints.shape[0],
             text_color="#cf6275",
+            font_size=label_size,
             bold=False,
             shape=None,
             render_points_as_spheres=True,
-            point_size=1.e-5,
+            point_size=1.0e-5,
             always_visible=True,
         )
         plotter.add_point_labels(
             link_midpoints + length * link_ylocal,
-            ['y'] * link_midpoints.shape[0],
+            ["y"] * link_midpoints.shape[0],
             text_color="#04d8b2",
+            font_size=label_size,
             bold=False,
             shape=None,
             render_points_as_spheres=True,
-            point_size=1.e-5,
+            point_size=1.0e-5,
             always_visible=True,
         )
         plotter.add_point_labels(
             link_midpoints + length * link_zlocal,
-            ['z'] * link_midpoints.shape[0],
+            ["z"] * link_midpoints.shape[0],
             text_color="#9aae07",
+            font_size=label_size,
             bold=False,
             shape=None,
             render_points_as_spheres=True,
-            point_size=1.e-5,
+            point_size=1.0e-5,
             always_visible=True,
         )
     else:
         # warnings.warn("Model has no link elements!")
         pass
 
 
-def _show_fix_node(plotter, model_info):
+def _show_fix_node(plotter, model_info, alpha: float = 1.0):
     fixed_dofs = model_info["FixNodeDofs"]
     fixed_coords = model_info["FixNodeCoords"]
     beam_lengths = model_info["beam_lengths"]
+    D2 = True if np.max(model_info["model_dims"]) <= 2 else False
     if len(beam_lengths) > 0:
-        s = (np.max(beam_lengths) + np.min(beam_lengths)) / 20
+        s = np.mean(beam_lengths) / 6 * alpha
     else:
-        s = (model_info["max_bound"] + model_info["min_bound"]) / 100
+        s = (model_info["max_bound"] + model_info["min_bound"]) / 100 * alpha
     if len(fixed_coords) > 0:
         points, cells = [], []
         for coord, dof in zip(fixed_coords, fixed_dofs):
             x, y, z = coord
+            if D2:
+                z += s / 2
+                y -= s / 2
             if dof[0] == -1:
                 idx = len(points)
-                points.extend([[x, y - s / 2, z], [x, y + s / 2, z],
-                               [x, y + s / 2, z - s], [x, y - s / 2, z - s]])
-                cells.extend([2, idx, idx + 1, 2, idx + 1, idx + 2,
-                              2, idx + 2, idx + 3, 2, idx + 3, idx])
+                points.extend(
+                    [
+                        [x, y - s / 2, z],
+                        [x, y + s / 2, z],
+                        [x, y + s / 2, z - s],
+                        [x, y - s / 2, z - s],
+                    ]
+                )
+                cells.extend(
+                    [
+                        2,
+                        idx,
+                        idx + 1,
+                        2,
+                        idx + 1,
+                        idx + 2,
+                        2,
+                        idx + 2,
+                        idx + 3,
+                        2,
+                        idx + 3,
+                        idx,
+                    ]
+                )
             if dof[1] == -1:
                 idx = len(points)
-                points.extend([[x - s / 2, y, z], [x + s / 2, y, z],
-                               [x + s / 2, y, z - s], [x - s / 2, y, z - s]])
-                cells.extend([2, idx, idx + 1, 2, idx + 1, idx + 2,
-                              2, idx + 2, idx + 3, 2, idx + 3, idx])
+                points.extend(
+                    [
+                        [x - s / 2, y, z],
+                        [x + s / 2, y, z],
+                        [x + s / 2, y, z - s],
+                        [x - s / 2, y, z - s],
+                    ]
+                )
+                cells.extend(
+                    [
+                        2,
+                        idx,
+                        idx + 1,
+                        2,
+                        idx + 1,
+                        idx + 2,
+                        2,
+                        idx + 2,
+                        idx + 3,
+                        2,
+                        idx + 3,
+                        idx,
+                    ]
+                )
             if dof[2] == -1:
                 idx = len(points)
-                points.extend([[x - s / 2, y - s / 2, z - s / 2], [x + s / 2, y - s / 2, z - s / 2],
-                               [x + s / 2, y + s / 2, z - s / 2], [x - s / 2, y + s / 2, z - s / 2]])
-                cells.extend([2, idx, idx + 1, 2, idx + 1, idx + 2,
-                              2, idx + 2, idx + 3, 2, idx + 3, idx])
+                points.extend(
+                    [
+                        [x - s / 2, y - s / 2, z - s / 2],
+                        [x + s / 2, y - s / 2, z - s / 2],
+                        [x + s / 2, y + s / 2, z - s / 2],
+                        [x - s / 2, y + s / 2, z - s / 2],
+                    ]
+                )
+                cells.extend(
+                    [
+                        2,
+                        idx,
+                        idx + 1,
+                        2,
+                        idx + 1,
+                        idx + 2,
+                        2,
+                        idx + 2,
+                        idx + 3,
+                        2,
+                        idx + 3,
+                        idx,
+                    ]
+                )
         fix_plot = _generate_mesh(points, cells, kind="line")
-        plotter.add_mesh(fix_plot, color="#01ff07",
-                         render_lines_as_tubes=False, line_width=2)
+        plotter.add_mesh(
+            fix_plot, color="#01ff07", render_lines_as_tubes=False, line_width=2
+        )
     else:
         warnings.warn("Model has no fix nodes!")
 
 
+def _plot_model(obj, plotter, model_info, cells, opacity):
+    point_plot = pv.PolyData(model_info["coord_no_deform"])
+    plotter.add_mesh(
+        point_plot,
+        color=obj.color_point,
+        point_size=obj.point_size,
+        render_points_as_spheres=True,
+    )
+
+    if len(cells["truss"]) > 0:
+        truss_plot = _generate_mesh(
+            model_info["coord_no_deform"], cells["truss"], kind="line"
+        )
+        plotter.add_mesh(
+            truss_plot,
+            color=obj.color_truss,
+            render_lines_as_tubes=True,
+            line_width=obj.line_width,
+        )
+
+    if len(cells["link"]) > 0:
+        link_plot = _generate_mesh(
+            model_info["coord_no_deform"], cells["link"], kind="line"
+        )
+        plotter.add_mesh(
+            link_plot,
+            color=obj.color_link,
+            render_lines_as_tubes=False,
+            line_width=obj.line_width / 2,
+        )
+
+    if len(cells["beam"]) > 0:
+        beam_plot = _generate_mesh(
+            model_info["coord_no_deform"], cells["beam"], kind="line"
+        )
+        plotter.add_mesh(
+            beam_plot,
+            color=obj.color_line,
+            render_lines_as_tubes=True,
+            line_width=obj.line_width,
+        )
+
+    if len(cells["other_line"]) > 0:
+        other_line_plot = _generate_mesh(
+            model_info["coord_no_deform"], cells["other_line"], kind="line"
+        )
+        plotter.add_mesh(
+            other_line_plot,
+            color=obj.color_line,
+            render_lines_as_tubes=True,
+            line_width=obj.line_width,
+        )
+
+    if len(cells["plane"]) > 0:
+        face_plot = _generate_mesh(
+            model_info["coord_no_deform"], cells["plane"], kind="face"
+        )
+        plotter.add_mesh(
+            face_plot, color=obj.color_face, show_edges=True, opacity=opacity
+        )
+
+    if len(cells["tetrahedron"]) > 0:
+        tet_plot = _generate_mesh(
+            model_info["coord_no_deform"], cells["tetrahedron"], kind="face"
+        )
+        plotter.add_mesh(
+            tet_plot, color=obj.color_solid, show_edges=True, opacity=opacity
+        )
+
+    if len(cells["brick"]) > 0:
+        bri_plot = _generate_mesh(
+            model_info["coord_no_deform"], cells["brick"], kind="face"
+        )
+        plotter.add_mesh(
+            bri_plot, color=obj.color_solid, show_edges=True, opacity=opacity
+        )
+
+
 def _eigen_vis(
-        obj,
-        mode_tags: list,
-        input_file: str = 'EigenData.hdf5',
-        subplots: bool = False,
-        link_views: bool = True,
-        alpha: float = None,
-        show_outline: bool = False,
-        show_origin: bool = False,
-        opacity: float = 1.0,
-        show_face_line: bool = True,
-        save_fig: str = "EigenVis.svg"
+    obj,
+    mode_tags: list,
+    input_file: str = "EigenData.hdf5",
+    subplots: bool = False,
+    link_views: bool = True,
+    alpha: float = 1.0,
+    show_outline: bool = False,
+    show_origin: bool = False,
+    label_size: float = 15,
+    opacity: float = 1.0,
+    show_face_line: bool = True,
+    save_fig: str = "EigenVis.svg",
 ):
-    filename = obj.out_dir + '/' + input_file
+    filename = obj.out_dir + "/" + input_file
     eigen_data = dict()
     with h5py.File(filename, "r") as f:
         grp = f["EigenInfo"]
         for name, value in grp.items():
             eigen_data[name] = value[...]
-    # with shelve.open(filename) as db:
-    #     eigen_data = db["EigenInfo"]
 
     f = eigen_data["f"]
     eigenvector = eigen_data["eigenvector"]
+    show_zaxis = False if np.max(eigen_data["model_dims"]) <= 2 else True
     num_mode_tag = len(f)
     modei, modej = mode_tags
     modei, modej = int(modei), int(modej)
     if modej > num_mode_tag:
-        raise ValueError(
-            f"Insufficient number of modes in eigen file {filename}!")
+        raise ValueError(f"Insufficient number of modes in eigen file {filename}!")
+
+    # -----------------------------------------------------------------------
+    def create_mesh(idx, idxi=None, idxj=None):
+        if idxi is not None and idxj is not None:
+            plotter.subplot(idxi, idxj)
+        else:
+            plotter.clear_actors()
+        step = int(round(idx)) - 1
+        eigen_vec = eigenvector[step]
+        value_ = np.max(np.sqrt(np.sum(eigen_vec**2, axis=1)))
+        alpha_ = eigen_data["max_bound"] / obj.bound_fact / value_
+        alpha_ = alpha * alpha if alpha else alpha_
+        eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
+        scalars = np.sqrt(np.sum(eigen_vec**2, axis=1))
+        _ = _generate_all_mesh(
+            plotter,
+            eigen_points,
+            scalars,
+            opacity,
+            obj.color_map,
+            eigen_data["all_lines"],
+            eigen_data["all_faces"],
+            show_origin=show_origin,
+            points_origin=eigen_data["coord_no_deform"],
+            point_size=obj.point_size,
+            line_width=obj.line_width,
+            show_face_line=show_face_line,
+        )
+        # plotter.add_scalar_bar(fmt="%.3e", n_labels=10, label_font_size=12)
+        # txt = 'Mode {}\nf = {:.3f} Hz\nT = {:.3f} s'.format(mode_tag, f_, 1 / f_)
+        txt = "Mode {}\nT = {:.3f} s".format(step + 1, 1 / f[step])
+        plotter.add_text(
+            txt, position="upper_left", font_size=label_size, font="courier"
+        )
+        if show_outline:
+            plotter.show_bounds(
+                grid=False,
+                location="outer",
+                bounds=eigen_data["bound"],
+                show_zaxis=show_zaxis,
+                # color="black",
+            )
+        plotter.add_axes()
 
     # !subplots
     if subplots:
         if modej - modei + 1 > 49:
-            raise ValueError(
-                "When subplots True, mode_tag range must < 49 for clarify"
-            )
+            raise ValueError("When subplots True, mode_tag range must < 49 for clarify")
         shape = shape_dict[modej - modei + 1]
-        subplot_titles = []
-        for i, idx in enumerate(range(modei, modej + 1)):
-            txt = "Mode {}: T = {:.3f} s".format(idx, 1 / f[idx - 1])
-            subplot_titles.append(txt)
-
         plotter = pv.Plotter(notebook=obj.notebook, shape=shape, line_smoothing=True)
         for i, idx in enumerate(range(modei, modej + 1)):
-            eigen_vec = eigenvector[idx - 1]
-            if alpha is None:
-                value_ = np.max(np.sqrt(np.sum(eigen_vec ** 2, axis=1)))
-                alpha_ = (
-                    eigen_data["max_bound"] / obj.bound_fact / value_
-                )
-            else:
-                alpha_ = alpha
-            eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
-            scalars = np.sqrt(np.sum(eigen_vec ** 2, axis=1))
-
             idxi = int(np.ceil((i + 1) / shape[1]) - 1)
             idxj = int(i - idxi * shape[1])
-
-            # ------------------------------------------------------
-            plotter.subplot(idxi, idxj)
-
-            _ = _generate_all_mesh(
-                plotter,
-                eigen_points,
-                scalars,
-                opacity,
-                obj.color_map,
-                eigen_data["all_lines"],
-                eigen_data["all_faces"],
-                show_origin=show_origin,
-                points_origin=eigen_data["coord_no_deform"],
-                point_size=obj.point_size,
-                line_width=obj.line_width,
-                show_face_line=show_face_line
-            )
-
-            # plotter.add_scalar_bar(color='#000000', n_labels=10, label_font_size=8)
-            # txt = 'Mode {}\nf = {:.3f} Hz\nT = {:.3f} s'.format(i + 1, f[i], 1 / f[i])
-            txt = "Mode {} T = {:.3f} s".format(idx, 1 / f[idx - 1])
-            plotter.add_text(
-                txt,
-                position="upper_right",
-                font_size=15,
-                # color="black",
-                font="courier",
-            )
-            if show_outline:
-                plotter.show_bounds(
-                    grid=False,
-                    location="outer",
-                    bounds=eigen_data["bound"],
-                    show_zaxis=True,
-                    # color="black",
-                    font_size=10,
-                )
-            plotter.add_axes(color="black")
+            create_mesh(idx, idxi, idxj)
         if link_views:
             plotter.link_views()
     # !slide style
     else:
         plotter = pv.Plotter(notebook=obj.notebook, line_smoothing=True)
-
-        def create_mesh(value):
-            step = int(round(value)) - 1
-            eigen_vec = eigenvector[step]
-            if alpha is None:
-                value_ = np.max(np.sqrt(np.sum(eigen_vec ** 2, axis=1)))
-                alpha_ = (
-                    eigen_data["max_bound"] / obj.bound_fact / value_
-                )
-            else:
-                alpha_ = alpha
-            eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
-            scalars = np.sqrt(np.sum(eigen_vec ** 2, axis=1))
-            cmin = np.min(scalars)
-            cmax = np.max(scalars)
-            plotter.clear_actors()
-            _ = _generate_all_mesh(
-                plotter,
-                eigen_points,
-                scalars,
-                opacity,
-                obj.color_map,
-                eigen_data["all_lines"],
-                eigen_data["all_faces"],
-                show_origin=show_origin,
-                points_origin=eigen_data["coord_no_deform"],
-                point_size=obj.point_size,
-                line_width=obj.line_width,
-                show_face_line=show_face_line
-            )
-
-            plotter.add_scalar_bar(
-                fmt="%.3e", n_labels=10, label_font_size=12
-            )
-
-            # txt = 'Mode {}\nf = {:.3f} Hz\nT = {:.3f} s'.format(mode_tag, f_, 1 / f_)
-            txt = "Mode {}\nT = {:.3f} s".format(step + 1, 1 / f[step])
-            plotter.add_text(
-                txt, position="upper_left", font_size=15, font="courier"
-            )
-            if show_outline:
-                plotter.show_bounds(
-                    grid=False,
-                    location="outer",
-                    bounds=eigen_data["bound"],
-                    show_zaxis=True,
-                    # color="black",
-                )
-            plotter.add_axes()
-
-        slider = plotter.add_slider_widget(
+        plotter.add_slider_widget(
             create_mesh,
             [modei, modej],
             value=modei,
             pointa=(0.4, 0.9),
             pointb=(0.9, 0.9),
             title="Mode",
             title_opacity=1,
@@ -427,95 +708,85 @@
             tube_width=0.01,
         )
     plotter.view_isometric()
     if np.max(eigen_data["model_dims"]) <= 2:
         plotter.view_xy(negative=False)
     if save_fig:
         plotter.save_graphic(save_fig)
-    plotter.enable_anti_aliasing('msaa')
+    plotter.enable_anti_aliasing("msaa")
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _eigen_anim(
-        obj,
-        mode_tag: int = 1,
-        input_file: str = 'EigenData.hdf5',
-        n_cycle: int = 5,
-        alpha: float = None,
-        show_outline: bool = False,
-        opacity: float = 1,
-        framerate: int = 3,
-        show_face_line: bool = True,
-        save_fig: str = "EigenAnimation.gif"
+    obj,
+    mode_tag: int = 1,
+    input_file: str = "EigenData.hdf5",
+    n_cycle: int = 5,
+    label_size: float = 15,
+    alpha: float = None,
+    show_outline: bool = False,
+    opacity: float = 1,
+    framerate: int = 3,
+    show_face_line: bool = True,
+    save_fig: str = "EigenAnimation.gif",
 ):
-    filename = obj.out_dir + '/' + input_file
+    filename = obj.out_dir + "/" + input_file
     eigen_data = dict()
     with h5py.File(filename, "r") as f:
         grp = f["EigenInfo"]
         for name, value in grp.items():
             eigen_data[name] = value[...]
 
     f = eigen_data["f"]
     eigenvector = eigen_data["eigenvector"]
     num_mode_tag = len(f)
     if mode_tag > num_mode_tag:
         raise ValueError("Insufficient number of modes in open file")
     eigen_vec = eigenvector[mode_tag - 1]
     f_ = f[mode_tag - 1]
-    if alpha is None:
-        value_ = np.max(np.sqrt(np.sum(eigen_vec ** 2, axis=1)))
-        alpha_ = (
-            eigen_data["max_bound"] / obj.bound_fact / value_
-        )
-    else:
-        alpha_ = alpha
+    value_ = np.max(np.sqrt(np.sum(eigen_vec**2, axis=1)))
+    alpha_ = eigen_data["max_bound"] / obj.bound_fact / value_
+    alpha_ = alpha_ * alpha if alpha else alpha_
     eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
     anti_eigen_points = eigen_data["coord_no_deform"] - eigen_vec * alpha_
-    scalars = np.sqrt(np.sum(eigen_vec ** 2, axis=1))
-    plt_points = [anti_eigen_points,
-                  eigen_data["coord_no_deform"], eigen_points]
+    scalars = np.sqrt(np.sum(eigen_vec**2, axis=1))
+    plt_points = [anti_eigen_points, eigen_data["coord_no_deform"], eigen_points]
     # -----------------------------------------------------------------------------
     # start plot
     plotter = pv.Plotter(notebook=obj.notebook, line_smoothing=True)
 
-    if alpha is None:
-        value_ = np.max(np.sqrt(np.sum(eigen_vec ** 2, axis=1)))
-        alpha_ = (
-            eigen_data["max_bound"] / obj.bound_fact / value_
-        )
-    else:
-        alpha_ = alpha
+    value_ = np.max(np.sqrt(np.sum(eigen_vec**2, axis=1)))
+    alpha_ = eigen_data["max_bound"] / obj.bound_fact / value_
+    alpha_ = alpha_ * alpha if alpha else alpha_
     eigen_points = eigen_data["coord_no_deform"] + eigen_vec * alpha_
     anti_eigen_points = eigen_data["coord_no_deform"] - eigen_vec * alpha_
-    scalars = np.sqrt(np.sum(eigen_vec ** 2, axis=1))
-    point_plot, line_plot, face_plot = _generate_all_mesh(plotter,
-                                                          eigen_data["coord_no_deform"],
-                                                          scalars * 0,
-                                                          opacity,
-                                                          obj.color_map,
-                                                          eigen_data["all_lines"],
-                                                          eigen_data["all_faces"],
-                                                          show_origin=False,
-                                                          points_origin=eigen_data["coord_no_deform"],
-                                                          show_scalar_bar=True,
-                                                          point_size=obj.point_size,
-                                                          line_width=obj.line_width,
-                                                          show_face_line=show_face_line,
-                                                          )
-
-    plotter.add_scalar_bar(
-        fmt="%.3E", n_labels=10, label_font_size=12
+    scalars = np.sqrt(np.sum(eigen_vec**2, axis=1))
+    point_plot, line_plot, face_plot = _generate_all_mesh(
+        plotter,
+        eigen_data["coord_no_deform"],
+        scalars * 0,
+        opacity,
+        obj.color_map,
+        eigen_data["all_lines"],
+        eigen_data["all_faces"],
+        show_origin=False,
+        points_origin=eigen_data["coord_no_deform"],
+        show_scalar_bar=True,
+        point_size=obj.point_size,
+        line_width=obj.line_width,
+        show_face_line=show_face_line,
     )
 
+    plotter.add_scalar_bar(fmt="%.3E", n_labels=10, label_font_size=12)
+
     plotter.add_text(
-        "Mode {}\nf = {:.3f} Hz\nT = {:.3f} s".format(
-            mode_tag, f_, 1 / f_),
+        "Mode {}\nf = {:.3f} Hz\nT = {:.3f} s".format(mode_tag, f_, 1 / f_),
         position="upper_right",
-        font_size=15,
+        font_size=label_size,
         # color="black",
         font="courier",
     )
     if show_outline:
         plotter.show_bounds(
             grid=False,
             location="outer",
@@ -528,83 +799,90 @@
     plotter.view_isometric()
     if np.max(eigen_data["model_dims"]) <= 2:
         plotter.view_xy(negative=False)
 
     # animation
     # ----------------------------------------------------------------------------
     if save_fig.endswith(".gif"):
-        plotter.open_gif(save_fig, fps=framerate)
+        plotter.open_gif(save_fig, fps=framerate, palettesize=64)
     else:
-        plotter.open_movie(save_fig, framerate=framerate)
-    plt_points = [anti_eigen_points,
-                  eigen_data["coord_no_deform"], eigen_points]
+        plotter.open_movie(save_fig, framerate=framerate, quality=7)
+    plt_points = [anti_eigen_points, eigen_data["coord_no_deform"], eigen_points]
     render = False
     index = [2, 0] * n_cycle
     plotter.write_frame()  # write initial data
     for idx in index:
         points = plt_points[idx]
         xyz = (eigen_data["coord_no_deform"] - points) / alpha_
-        xyz_eigen = np.sqrt(np.sum(xyz ** 2, axis=1))
+        xyz_eigen = np.sqrt(np.sum(xyz**2, axis=1))
         if point_plot:
-            plotter.update_coordinates(
-                points, mesh=point_plot, render=render)
-            plotter.update_scalars(
-                scalars=xyz_eigen, mesh=point_plot, render=render)
+            plotter.update_coordinates(points, mesh=point_plot, render=render)
+            plotter.update_scalars(scalars=xyz_eigen, mesh=point_plot, render=render)
         if line_plot:
-            plotter.update_scalars(
-                scalars=xyz_eigen, mesh=line_plot, render=render)
-            plotter.update_coordinates(
-                points, mesh=line_plot, render=render)
+            plotter.update_scalars(scalars=xyz_eigen, mesh=line_plot, render=render)
+            plotter.update_coordinates(points, mesh=line_plot, render=render)
         if face_plot:
-            plotter.update_scalars(
-                scalars=xyz_eigen, mesh=face_plot, render=render)
-            plotter.update_coordinates(
-                points, mesh=face_plot, render=render)
+            plotter.update_scalars(scalars=xyz_eigen, mesh=face_plot, render=render)
+            plotter.update_coordinates(points, mesh=face_plot, render=render)
         plotter.update_scalar_bar_range(
             clim=[np.min(xyz_eigen), np.max(xyz_eigen)], name=None
         )
         plotter.write_frame()
     # ----------------------------------------------------------------------------------
-    plotter.enable_anti_aliasing('msaa')
+    plotter.enable_anti_aliasing("msaa")
     plotter.show(title=obj.title)
     plotter.close()
 
 
-def _react_vis(obj,
-               input_file: str = "NodeReactionStepData-1.hdf5",
-               slider: bool = False,
-               direction: str = "Fz",
-               show_values: bool = True,
-               show_outline: bool = False,
-               save_fig: str = "ReactionVis.svg"):
+def _react_vis(
+    obj,
+    input_file: str = "NodeReactionStepData-1.hdf5",
+    slider: bool = False,
+    direction: str = "Fz",
+    show_values: bool = True,
+    show_outline: bool = False,
+    save_fig: str = "ReactionVis.svg",
+):
     direct = direction.lower()
-    if direct not in ['fx', 'fy', 'fz', 'mx', 'my', 'mz']:
+    if direct not in ["fx", "fy", "fz", "mx", "my", "mz"]:
         raise ValueError(
-            "response must be one of ['Fx', 'Fy', 'Fz', 'Mx', 'My', 'Mz']!")
-    filename = obj.out_dir + '/' + input_file
+            "response must be one of ['Fx', 'Fy', 'Fz', 'Mx', 'My', 'Mz']!"
+        )
+    filename = obj.out_dir + "/" + input_file
     node_react_steps = []
     with h5py.File(filename, "r") as f:
         Nsteps = int(f["Nsteps"][...])
         node_coords = f["NodeReactCoords"][...]
-        model_dims = f['model_dims'][...]
+        model_dims = f["model_dims"][...]
         NodeTags = f["NodeReactTags"][...]
         num_nodes = node_coords.shape[0]
         grp = f["NodeReactSteps"]
         for i in range(Nsteps):
             node_react_steps.append(grp[f"step{i + 1}"][...])
     if np.max(model_dims) < 3:
         D2 = True
     else:
         D2 = False
-    max_bound = np.max(np.max(node_coords, axis=0) -
-                       np.min(node_coords, axis=0))
-    axis_dict = dict(fx=(1, 0., 0.), fy=(0., 1, 0.), fz=(0., 0., 1),
-                     mx=(1, 0., 0.), my=(0., 1, 0.), mz=(0., 0., 1))
-    color_dict = dict(fx="#d20962", fy="#f47721", fz="#7ac143",
-                      mx="#00a78e", my="#00bce4", mz="#7d3f98")
+    max_bound = np.max(np.max(node_coords, axis=0) - np.min(node_coords, axis=0))
+    axis_dict = dict(
+        fx=(1, 0.0, 0.0),
+        fy=(0.0, 1, 0.0),
+        fz=(0.0, 0.0, 1),
+        mx=(1, 0.0, 0.0),
+        my=(0.0, 1, 0.0),
+        mz=(0.0, 0.0, 1),
+    )
+    color_dict = dict(
+        fx="#d20962",
+        fy="#f47721",
+        fz="#7ac143",
+        mx="#00a78e",
+        my="#00bce4",
+        mz="#7d3f98",
+    )
     if D2:
         reactidx_dict = dict(fx=0, fy=1, fz=None, mx=None, my=None, mz=2)
     else:
         reactidx_dict = dict(fx=0, fy=1, fz=2, mx=3, my=4, mz=5)
 
     plotter = pv.Plotter(notebook=obj.notebook, line_smoothing=True)
 
@@ -620,55 +898,57 @@
             color=obj.color_point,
             point_size=obj.point_size,
             render_points_as_spheres=True,
         )
         point_plot2 = pv.PolyData(node_coords[[idxmax, idxmin]])
         plotter.add_mesh(
             point_plot2,
-            color='red',
+            color="red",
             point_size=obj.point_size * 2,
             render_points_as_spheres=True,
         )
         # arrow plot
         length = max_bound / 30
         axis = np.zeros_like(node_coords)
         for i in range(num_nodes):
             axis[i] = np.array(axis_dict[direct]) * np.sign(f[i])
         arrow_ends = node_coords - length * axis
-        _ = plotter.add_arrows(arrow_ends, axis,
-                               mag=length, color=color_dict[direct])
+        _ = plotter.add_arrows(arrow_ends, axis, mag=length, color=color_dict[direct])
         labels = [f"{data:.3E}" for data in f]
         plotter.add_point_labels(
             arrow_ends,
             labels,
             bold=False,
             shape=None,
             render_points_as_spheres=True,
-            point_size=1.e-5,
+            point_size=1.0e-5,
             always_visible=True,
         )
 
         plotter.add_text(
             "OpenSeesPy Node Reactions View",
             position="upper_left",
             shadow=True,
             font_size=16,
             # color="black",
             font="courier",
         )
-        txt = (f"Step {step + 1} {direction}\n"
-               f"max={f[idxmax]:.3E} | nodeTag={NodeTags[idxmax]}\n"
-               f"min={f[idxmin]:.3E} | nodeTag={NodeTags[idxmin]}")
-        plotter.add_text(txt,
-                         position="upper_right",
-                         shadow=True,
-                         font_size=12,
-                         # color="black",
-                         font="courier",
-                         )
+        txt = (
+            f"Step {step + 1} {direction}\n"
+            f"max={f[idxmax]:.3E} | nodeTag={NodeTags[idxmax]}\n"
+            f"min={f[idxmin]:.3E} | nodeTag={NodeTags[idxmin]}"
+        )
+        plotter.add_text(
+            txt,
+            position="upper_right",
+            shadow=True,
+            font_size=12,
+            # color="black",
+            font="courier",
+        )
 
         if show_outline:
             plotter.show_bounds(
                 grid=False,
                 location="outer",
                 show_zaxis=True,
                 # color="black",
@@ -688,45 +968,49 @@
             fmt="%.0f",
             title_height=0.03,
             slider_width=0.03,
             tube_width=0.01,
         )
     # -------------------------------------------------------------------------
     else:  # plot a single step
-        idx = np.argmax([np.max(np.abs(react[:, reactidx_dict[direct]]))
-                         for react in node_react_steps])
+        idx = np.argmax(
+            [
+                np.max(np.abs(react[:, reactidx_dict[direct]]))
+                for react in node_react_steps
+            ]
+        )
         create_mesh(idx + 1)
     plotter.view_isometric()
     if D2:
         plotter.view_xy(negative=False)
     if save_fig:
         plotter.save_graphic(save_fig)
-    plotter.enable_anti_aliasing('msaa')
+    plotter.enable_anti_aliasing("msaa")
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _deform_vis(
-        obj,
-        input_file: str = "NodeRespStepData-1.hdf5",
-        slider: bool = False,
-        response: str = "disp",
-        alpha: float = None,
-        show_outline: bool = False,
-        show_origin: bool = False,
-        show_face_line: bool = True,
-        opacity: float = 1,
-        save_fig: str = "DefoVis.svg",
-        model_update: bool = False
+    obj,
+    input_file: str = "NodeRespStepData-1.hdf5",
+    slider: bool = False,
+    response: str = "disp",
+    alpha: float = 1.0,
+    show_outline: bool = False,
+    show_origin: bool = False,
+    show_face_line: bool = True,
+    opacity: float = 1,
+    save_fig: str = "DefoVis.svg",
+    model_update: bool = False,
 ):
     resp_type = response.lower()
-    if resp_type not in ['disp', 'vel', 'accel']:
+    if resp_type not in ["disp", "vel", "accel"]:
         raise ValueError("response must be 'disp', 'vel', or 'accel'!")
 
-    filename = obj.out_dir + '/' + input_file
+    filename = obj.out_dir + "/" + input_file
     model_info_steps = dict()
     cell_steps = dict()
     node_resp_steps = dict()
     with h5py.File(filename, "r") as f:
         n = int(f["Nsteps"][...])
         grp1 = f["ModelInfoSteps"]
         grp2 = f["CellSteps"]
@@ -748,44 +1032,38 @@
                 cell_steps[name] = value_[...]
         grp3 = f["NodeRespSteps"]
         for name, value_ in grp3.items():
             temp = []
             for i in range(n):
                 temp.append(value_[f"step{i + 1}"][...])
             node_resp_steps[name] = temp
-
-    # with shelve.open(filename) as db:
-    #     model_info_steps = db["ModelInfoSteps"]
-    #     cell_steps = db["CellSteps"]
-    #     node_resp_steps = db["NodeRespSteps"]
-
     num_steps = len(node_resp_steps["disp"])
-
     # ! max response
-    max_resps = [np.max(np.sqrt(np.sum(resp_ ** 2, axis=1)))
-                 for resp_ in node_resp_steps[resp_type]]
+    max_resps = [
+        np.max(np.sqrt(np.sum(resp_**2, axis=1)))
+        for resp_ in node_resp_steps[resp_type]
+    ]
     max_step = np.argmax(max_resps)
     max_node_resp = node_resp_steps[resp_type][max_step]
-    scalars = np.sqrt(np.sum(max_node_resp ** 2, axis=1))
+    scalars = np.sqrt(np.sum(max_node_resp**2, axis=1))
     cmin, cmax = np.min(scalars), np.max(scalars)
     if model_update:
         bounds = model_info_steps["bound"][0]
         model_dims = model_info_steps["model_dims"][0]
     else:
         bounds = model_info_steps["bound"]
         model_dims = model_info_steps["model_dims"]
     # scale factor
     if resp_type == "disp":
-        if alpha is None:
-            max_bound = np.max(
-                [bounds[1] - bounds[0], bounds[3] - bounds[2], bounds[5] - bounds[4]])
-            value = np.max(np.sqrt(np.sum(max_node_resp ** 2, axis=1)))
-            alpha_ = max_bound / obj.bound_fact / value
-        else:
-            alpha_ = alpha
+        max_bound = np.max(
+            [bounds[1] - bounds[0], bounds[3] - bounds[2], bounds[5] - bounds[4]]
+        )
+        value = np.max(np.sqrt(np.sum(max_node_resp**2, axis=1)))
+        alpha_ = max_bound / obj.bound_fact / value
+        alpha_ = alpha_ * alpha if alpha else alpha_
     else:
         alpha_ = 0
     # ------------------------------------------------------------------------
     # Start plot
     # -------------------------------------------------------------------------
     plotter = pv.Plotter(notebook=obj.notebook, line_smoothing=True)
 
@@ -799,35 +1077,33 @@
         else:
             node_nodeform_coords = model_info_steps["coord_no_deform"]
             bounds = model_info_steps["bound"]
             lines_cells = cell_steps["all_lines"]
             faces_cells = cell_steps["all_faces"]
         node_resp = node_resp_steps[resp_type][step]
         node_deform_coords = alpha_ * node_resp + node_nodeform_coords
-        scalars = np.sqrt(np.sum(node_resp ** 2, axis=1))
+        scalars = np.sqrt(np.sum(node_resp**2, axis=1))
         plotter.clear_actors()  # !!!!!!
         _ = _generate_all_mesh(
             plotter,
             node_deform_coords,
             scalars,
             opacity,
             obj.color_map,
             lines_cells=lines_cells,
             face_cells=faces_cells,
             show_origin=show_origin,
             points_origin=node_nodeform_coords,
             point_size=obj.point_size,
             line_width=obj.line_width,
             show_face_line=show_face_line,
-            clim=[cmin, cmax]
+            clim=[cmin, cmax],
         )
 
-        plotter.add_scalar_bar(
-            fmt="%.3e", n_labels=10, label_font_size=12
-        )
+        plotter.add_scalar_bar(fmt="%.3e", n_labels=10, label_font_size=12)
 
         plotter.add_text(
             "OpenSees 3D View",
             position="upper_left",
             shadow=True,
             font_size=16,
             # color="black",
@@ -883,36 +1159,36 @@
     else:  # plot a single step
         create_mesh(max_step + 1)
     plotter.view_isometric()
     if np.max(model_dims) <= 2:
         plotter.view_xy(negative=False)
     if save_fig:
         plotter.save_graphic(save_fig)
-    plotter.enable_anti_aliasing('msaa')
+    plotter.enable_anti_aliasing("msaa")
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _deform_anim(
-        obj,
-        input_file: str = "NodeRespStepData-1.hdf5",
-        response: str = "disp",
-        alpha: float = None,
-        show_outline: bool = False,
-        opacity: float = 1,
-        framerate: int = 24,
-        show_face_line: bool = True,
-        save_fig: str = "DefoAnimation.gif",
-        model_update: bool = False
+    obj,
+    input_file: str = "NodeRespStepData-1.hdf5",
+    response: str = "disp",
+    alpha: float = 1.0,
+    show_outline: bool = False,
+    opacity: float = 1,
+    framerate: int = 24,
+    show_face_line: bool = True,
+    save_fig: str = "DefoAnimation.gif",
+    model_update: bool = False,
 ):
     resp_type = response.lower()
-    if resp_type not in ['disp', 'vel', 'accel']:
+    if resp_type not in ["disp", "vel", "accel"]:
         raise ValueError("response must be 'disp', 'vel', or 'accel'!")
 
-    filename = obj.out_dir + '/' + input_file
+    filename = obj.out_dir + "/" + input_file
     model_info_steps = dict()
     cell_steps = dict()
     node_resp_steps = dict()
     with h5py.File(filename, "r") as f:
         n = int(f["Nsteps"][...])
         grp1 = f["ModelInfoSteps"]
         grp2 = f["CellSteps"]
@@ -938,35 +1214,36 @@
             for i in range(n):
                 temp.append(value_[f"step{i + 1}"][...])
             node_resp_steps[name] = temp
 
     num_steps = len(node_resp_steps["disp"])
 
     # ! max response
-    max_resps = [np.max(np.sqrt(np.sum(resp_ ** 2, axis=1)))
-                 for resp_ in node_resp_steps[resp_type]]
+    max_resps = [
+        np.max(np.sqrt(np.sum(resp_**2, axis=1)))
+        for resp_ in node_resp_steps[resp_type]
+    ]
     max_step = np.argmax(max_resps)
     max_node_resp = node_resp_steps[resp_type][max_step]
-    scalars = np.sqrt(np.sum(max_node_resp ** 2, axis=1))
+    scalars = np.sqrt(np.sum(max_node_resp**2, axis=1))
     cmin, cmax = np.min(scalars), np.max(scalars)
     if model_update:
         bounds = model_info_steps["bound"][0]
         model_dims = model_info_steps["model_dims"][0]
     else:
         bounds = model_info_steps["bound"]
         model_dims = model_info_steps["model_dims"]
     # scale factor
     if resp_type == "disp":
-        if alpha is None:
-            max_bound = np.max(
-                [bounds[1] - bounds[0], bounds[3] - bounds[2], bounds[5] - bounds[4]])
-            value = np.max(np.sqrt(np.sum(max_node_resp ** 2, axis=1)))
-            alpha_ = max_bound / obj.bound_fact / value
-        else:
-            alpha_ = alpha
+        max_bound = np.max(
+            [bounds[1] - bounds[0], bounds[3] - bounds[2], bounds[5] - bounds[4]]
+        )
+        value = np.max(np.sqrt(np.sum(max_node_resp**2, axis=1)))
+        alpha_ = max_bound / obj.bound_fact / value
+        alpha_ = alpha_ * alpha if alpha else alpha_
     else:
         alpha_ = 0
     # -----------------------------------------------------------------------------
     # start plot
     plotter = pv.Plotter(notebook=obj.notebook, line_smoothing=True)
 
     def creat_mesh(step):
@@ -978,33 +1255,31 @@
         else:
             node_nodeform_coords = model_info_steps["coord_no_deform"]
             bounds = model_info_steps["bound"]
             lines_cells = cell_steps["all_lines"]
             faces_cells = cell_steps["all_faces"]
         node_resp = node_resp_steps[resp_type][step]
         node_deform_coords = alpha_ * node_resp + node_nodeform_coords
-        scalars = np.sqrt(np.sum(node_resp ** 2, axis=1))
+        scalars = np.sqrt(np.sum(node_resp**2, axis=1))
         plotter.clear_actors()  # !!!!!!
         point_plot, line_plot, face_plot = _generate_all_mesh(
             plotter,
             node_deform_coords,
             scalars,
             opacity,
             obj.color_map,
             lines_cells=lines_cells,
             face_cells=faces_cells,
             point_size=obj.point_size,
             line_width=obj.line_width,
             show_face_line=show_face_line,
-            clim=[cmin, cmax]
+            clim=[cmin, cmax],
         )
 
-        plotter.add_scalar_bar(
-            fmt="%.3e", n_labels=10, label_font_size=12
-        )
+        plotter.add_scalar_bar(fmt="%.3e", n_labels=10, label_font_size=12)
 
         txt = plotter.add_text(
             "peak of {}, step: {}\n"
             "min.x = {:.3E}  max.x = {:.3E}\n"
             "min.y = {:.3E}  max.y = {:.3E}\n"
             "min.z = {:.3E}  max.z = {:.3E}\n".format(
                 resp_type,
@@ -1045,106 +1320,113 @@
         plotter.open_movie(save_fig, framerate=framerate)
     # plotter.write_frame()  # write initial data
     for step in range(num_steps):
         _ = creat_mesh(step)
         plotter.write_frame()
 
     # ----------------------------------------------------------------------------------
-    plotter.enable_anti_aliasing('msaa')
+    plotter.enable_anti_aliasing("msaa")
     plotter.show(title=obj.title)
     plotter.close()
 
 
-def _frame_resp_vis(obj,
-                    input_file: str = "BeamRespStepData-1.hdf5",
-                    ele_tags: list = None,
-                    slider: bool = False,
-                    response: str = "Mz",
-                    show_values=True,
-                    alpha: float = None,
-                    opacity: float = 1,
-                    save_fig: str = "FrameRespVis.svg"
-                    ):
-    check_file(save_fig, ['.svg', '.eps', '.ps', 'pdf', '.tex'])
-    filename = obj.out_dir + '/' + input_file
+def _frame_resp_vis(
+    obj,
+    input_file: str = "BeamRespStepData-1.hdf5",
+    ele_tags: list = None,
+    slider: bool = False,
+    response: str = "Mz",
+    show_values=True,
+    alpha: float = 1.0,
+    opacity: float = 1,
+    save_fig: str = "FrameRespVis.svg",
+):
+    check_file(save_fig, [".svg", ".eps", ".ps", "pdf", ".tex"])
+    filename = obj.out_dir + "/" + input_file
     beam_infos = dict()
     beam_resp_step = dict()
     with h5py.File(filename, "r") as f:
         n = int(f["Nsteps"][...])
         grp1 = f["BeamInfos"]
         for name, value_ in grp1.items():
             beam_infos[name] = value_[...]
         grp2 = f["BeamRespSteps"]
         for name, value_ in grp2.items():
             temp = []
             for i in range(n):
                 temp.append(value_[f"step{i + 1}"][...])
             beam_resp_step[name] = temp
     # -------------------------------------
-    beam_tags = beam_infos['beam_tags']
+    beam_tags = beam_infos["beam_tags"]
     if len(beam_tags) == 0:
         warnings.warn("Model has no frame elements!")
         return None
-    ylocals = beam_infos['ylocal']
-    zlocals = beam_infos['zlocal']
+    ylocals = beam_infos["ylocal"]
+    zlocals = beam_infos["zlocal"]
     ylocal_map = {beam_tags[i]: ylocals[i] for i in range(len(beam_tags))}
     zlocal_map = {beam_tags[i]: zlocals[i] for i in range(len(beam_tags))}
-    local_forces_step = beam_resp_step['localForces']
+    local_forces_step = beam_resp_step["localForces"]
     num_steps = len(local_forces_step)
 
     if ele_tags is None:
         ele_tags = beam_tags
-        beam_node_coords = beam_infos['beam_node_coords']
-        beam_cells = beam_infos['beam_cells']
+        beam_node_coords = beam_infos["beam_node_coords"]
+        beam_cells = beam_infos["beam_cells"]
         beam_cell_map = {beam_tags[i]: i for i in range(len(beam_tags))}
         idxs = range(len(beam_tags))
     else:
         ele_tags = np.atleast_1d(ele_tags)
         beam_node_coords = []
         beam_cells = []
         idxs = []
         beam_cell_map = {}
         for i, eletag in enumerate(ele_tags):
-            idx = beam_infos['beam_cell_map'][eletag]
+            idx = beam_infos["beam_cell_map"][eletag]
             idxs.append(idx)
             beam_cell_map[eletag] = i
-            nodei, nodej = beam_infos['beam_cells'][idx, 1:]
-            beam_node_coords.append(beam_infos['beam_node_coords'][nodei])
-            beam_node_coords.append(beam_infos['beam_node_coords'][nodej])
+            nodei, nodej = beam_infos["beam_cells"][idx, 1:]
+            beam_node_coords.append(beam_infos["beam_node_coords"][nodei])
+            beam_node_coords.append(beam_infos["beam_node_coords"][nodej])
             beam_cells.append([2, 2 * i, 2 * i + 1])
         beam_node_coords = np.array(beam_node_coords)
         beam_cells = np.array(beam_cells)
 
-    idx_plottype_map = dict(fx=[0, 6], fy=[1, 7], fz=[2, 8],
-                            my=[4, 10], mz=[5, 11], mx=[3, 9])
-    f_sign_map = dict(fx=[-1, 1], fy=[-1, 1], fz=[-1, 1],
-                      my=[1, -1], mz=[-1, 1], mx=[1, -1])
-    axis_sign_map = dict(fx=1, fy=1, fz=1,
-                         my=-1, mz=-1, mx=-1)
-    axis_map_map = dict(fx=zlocal_map, fy=ylocal_map, fz=zlocal_map,
-                        my=zlocal_map, mz=ylocal_map, mx=zlocal_map)
+    idx_plottype_map = dict(
+        fx=[0, 6], fy=[1, 7], fz=[2, 8], my=[4, 10], mz=[5, 11], mx=[3, 9]
+    )
+    f_sign_map = dict(
+        fx=[-1, 1], fy=[-1, 1], fz=[-1, 1], my=[1, -1], mz=[-1, 1], mx=[1, -1]
+    )
+    axis_sign_map = dict(fx=1, fy=1, fz=1, my=-1, mz=-1, mx=-1)
+    axis_map_map = dict(
+        fx=zlocal_map,
+        fy=ylocal_map,
+        fz=zlocal_map,
+        my=zlocal_map,
+        mz=ylocal_map,
+        mx=zlocal_map,
+    )
     idx_plottype = idx_plottype_map[response.lower()]
     axis_map = axis_map_map[response.lower()]
     axis_sign = axis_sign_map[response.lower()]
-    local_forces_step = [data[:, idx_plottype][idxs] * np.array(f_sign_map[response.lower()])
-                         for data in local_forces_step]  # new
+    local_forces_step = [
+        data[:, idx_plottype][idxs] * np.array(f_sign_map[response.lower()])
+        for data in local_forces_step
+    ]  # new
 
-    maxv = [np.max(np.abs(data))
-            for data in local_forces_step]
+    maxv = [np.max(np.abs(data)) for data in local_forces_step]
     maxstep = np.argmax(maxv)
     local_forces_max = local_forces_step[maxstep]
     cmin, cmax = np.min(local_forces_max), np.max(local_forces_max)
-    if alpha is None:
-        max_coord = np.max(beam_node_coords, axis=0)
-        min_coord = np.min(beam_node_coords, axis=0)
-        max_bound = np.max(max_coord - min_coord)
-        maxv = np.amax(np.abs(local_forces_max))
-        alpha_ = max_bound / maxv / obj.bound_fact
-    else:
-        alpha_ = alpha
+    max_coord = np.max(beam_node_coords, axis=0)
+    min_coord = np.min(beam_node_coords, axis=0)
+    max_bound = np.max(max_coord - min_coord)
+    maxv = np.amax(np.abs(local_forces_max))
+    alpha_ = max_bound / maxv / obj.bound_fact
+    alpha_ = alpha_ * alpha if alpha else alpha_
 
     # ------------------------------------------------------------------------
     # start plot
     # -------------------------------------------------------------------------
     plotter = pv.Plotter(notebook=obj.notebook, line_smoothing=True)
 
     def create_mesh(value):
@@ -1173,16 +1455,15 @@
                 resp_points.extend([coord1, coord2, coord3, coord4])
                 resp_cells.extend([4, n, n + 1, n + 2, n + 3])
                 scalars.extend([f1_, f2_, f2_, f1_])
             else:
                 ratio = np.abs(f2 / f1)
                 ratio = 1 / (ratio + 1)
                 coord0 = coord1 + (coord2 - coord1) * ratio
-                resp_points.extend(
-                    [coord1, coord0, coord4, coord2, coord0, coord3])
+                resp_points.extend([coord1, coord0, coord4, coord2, coord0, coord3])
                 resp_cells.extend([3, n, n + 1, n + 2])
                 resp_cells.extend([3, n + 3, n + 4, n + 5])
                 scalars.extend([f1_, 0, f1_, f2_, 0, f2_])
         labels = [f"{label:.2E}" for label in labels]
         label_poins = np.array(label_poins)
         resp_points = np.array(resp_points)
         scalars = np.array(scalars)
@@ -1192,16 +1473,15 @@
         plotter.add_mesh(
             point_plot,
             color=obj.color_point,
             point_size=obj.point_size,
             render_points_as_spheres=True,
             show_scalar_bar=False,
         )
-        line_plot = _generate_mesh(
-            beam_node_coords, beam_cells, kind="line")
+        line_plot = _generate_mesh(beam_node_coords, beam_cells, kind="line")
         plotter.add_mesh(
             line_plot,
             color="black",
             render_lines_as_tubes=True,
             line_width=obj.line_width / 3,
             show_scalar_bar=False,
         )
@@ -1215,15 +1495,18 @@
             clim=[cmin, cmax],
             show_edges=False,
             opacity=opacity,
             interpolate_before_map=True,
             show_scalar_bar=False,
         )
         plotter.add_scalar_bar(
-            fmt="%.3e", n_labels=10, label_font_size=12, title=response,
+            fmt="%.3e",
+            n_labels=10,
+            label_font_size=12,
+            title=response,
         )
         plotter.add_axes()
         plotter.add_text(
             "OpenSees 3D View",
             position="upper_left",
             font_size=15,
             # color="black",
@@ -1270,15 +1553,15 @@
     else:  # plot a single step
         create_mesh(maxstep + 1)
     plotter.view_isometric()
     if np.max(np.abs(beam_node_coords[:, -1])) < 1e-5:
         plotter.view_xy(negative=False)
     if save_fig:
         plotter.save_graphic(save_fig)
-    plotter.enable_anti_aliasing('msaa')
+    plotter.enable_anti_aliasing("msaa")
     plotter.show(title=obj.title)
     plotter.close()
 
 
 def _generate_mesh(points, cells, kind="line"):
     """
     generate the mesh from the points and cells
@@ -1293,28 +1576,28 @@
         pltr.faces = cells
     else:
         raise ValueError(f"not supported {kind}!")
     return pltr
 
 
 def _generate_all_mesh(
-        plotter,
-        points,
-        scalars,
-        opacity,
-        colormap,
-        lines_cells,
-        face_cells,
-        show_origin=False,
-        points_origin=None,
-        show_scalar_bar=False,
-        point_size=1,
-        line_width=1,
-        show_face_line=True,
-        clim=None
+    plotter,
+    points,
+    scalars,
+    opacity,
+    colormap,
+    lines_cells,
+    face_cells,
+    show_origin=False,
+    points_origin=None,
+    show_scalar_bar=False,
+    point_size=1,
+    line_width=1,
+    show_face_line=True,
+    clim=None,
 ):
     """
     Auxiliary function for generating all meshes
     """
     if clim is None:
         clim = [np.min(scalars), np.max(scalars)]
     sargs = dict(
@@ -1339,17 +1622,15 @@
     #     render_points_as_spheres=True,
     #     show_scalar_bar=show_scalar_bar,
     #     scalar_bar_args=sargs,
     # )
     point_plot = None
     if len(lines_cells) > 0:
         if show_origin:
-            line_plot_origin = _generate_mesh(
-                points_origin, lines_cells, kind="line"
-            )
+            line_plot_origin = _generate_mesh(points_origin, lines_cells, kind="line")
             plotter.add_mesh(
                 line_plot_origin,
                 color="gray",
                 line_width=line_width / 2,
                 show_scalar_bar=False,
             )
         line_plot = _generate_mesh(points, lines_cells, kind="line")
@@ -1365,17 +1646,15 @@
             line_width=line_width,
         )
     else:
         line_plot = None
 
     if len(face_cells) > 0:
         if show_origin:
-            face_plot_origin = _generate_mesh(
-                points_origin, face_cells, kind="face"
-            )
+            face_plot_origin = _generate_mesh(points_origin, face_cells, kind="face")
             plotter.add_mesh(
                 face_plot_origin,
                 color="gray",
                 style="wireframe",
                 show_scalar_bar=False,
                 show_edges=True,
                 line_width=line_width / 3,
@@ -1392,85 +1671,7 @@
             interpolate_before_map=True,
             show_scalar_bar=show_scalar_bar,
         )
     else:
         face_plot = None
 
     return point_plot, line_plot, face_plot
-
-
-def _plot_model(obj, plotter, model_info, cells, opacity):
-    point_plot = pv.PolyData(model_info["coord_no_deform"])
-    plotter.add_mesh(
-        point_plot,
-        color=obj.color_point,
-        point_size=obj.point_size,
-        render_points_as_spheres=True,
-    )
-
-    if len(cells["truss"]) > 0:
-        truss_plot = _generate_mesh(
-            model_info["coord_no_deform"], cells["truss"], kind="line"
-        )
-        plotter.add_mesh(
-            truss_plot,
-            color=obj.color_truss,
-            render_lines_as_tubes=True,
-            line_width=obj.line_width,
-        )
-
-    if len(cells["link"]) > 0:
-        link_plot = _generate_mesh(
-            model_info["coord_no_deform"], cells["link"], kind="line"
-        )
-        plotter.add_mesh(
-            link_plot,
-            color=obj.color_link,
-            render_lines_as_tubes=False,
-            line_width=obj.line_width / 2,
-        )
-
-    if len(cells["beam"]) > 0:
-        beam_plot = _generate_mesh(
-            model_info["coord_no_deform"], cells["beam"], kind="line"
-        )
-        plotter.add_mesh(
-            beam_plot,
-            color=obj.color_line,
-            render_lines_as_tubes=True,
-            line_width=obj.line_width,
-        )
-
-    if len(cells["other_line"]) > 0:
-        other_line_plot = _generate_mesh(
-            model_info["coord_no_deform"], cells["other_line"], kind="line"
-        )
-        plotter.add_mesh(
-            other_line_plot,
-            color=obj.color_line,
-            render_lines_as_tubes=True,
-            line_width=obj.line_width,
-        )
-
-    if len(cells["plane"]) > 0:
-        face_plot = _generate_mesh(
-            model_info["coord_no_deform"], cells["plane"], kind="face"
-        )
-        plotter.add_mesh(
-            face_plot, color=obj.color_face, show_edges=True, opacity=opacity
-        )
-
-    if len(cells["tetrahedron"]) > 0:
-        tet_plot = _generate_mesh(
-            model_info["coord_no_deform"], cells["tetrahedron"], kind="face"
-        )
-        plotter.add_mesh(
-            tet_plot, color=obj.color_solid, show_edges=True, opacity=opacity
-        )
-
-    if len(cells["brick"]) > 0:
-        bri_plot = _generate_mesh(
-            model_info["coord_no_deform"], cells["brick"], kind="face"
-        )
-        plotter.add_mesh(
-            bri_plot, color=obj.color_solid, show_edges=True, opacity=opacity
-        )
```

### Comparing `opstool-0.7.3/src/opstool/vis/fiber_sec_vis.py` & `opstool-0.8.0/src/opstool/vis/fiber_sec_vis.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,41 +34,47 @@
         Transparency of mesh.
 
     Returns
     --------
     FiberSecVis instance.
     """
 
-    def __init__(self,
-                 results_dir: str = "opstool_output",
-                 input_file: str = "FiberRespStepData-1.hdf5",
-                 line_width: float = 0.75, line_color: str = 'k',
-                 colormap: str = "viridis", opacity: float = 0.75):
+    def __init__(
+        self,
+        results_dir: str = "opstool_output",
+        input_file: str = "FiberRespStepData-1.hdf5",
+        line_width: float = 0.75,
+        line_color: str = "k",
+        colormap: str = "viridis",
+        opacity: float = 0.75,
+    ):
         self.lw = line_width
         self.lc = line_color
         self.cmap = colormap
         self.opacity = opacity
         self.out_dir = results_dir
 
-        filename = self.out_dir + '/' + input_file
+        filename = self.out_dir + "/" + input_file
         self.fiber_sec_step_data = dict()
         with h5py.File(filename, "r") as f:
             n = f["Nsteps"][...]
             grp = f["FiberRespSteps"]
             for name in grp.keys():
                 temp = []
                 for i in range(n):
                     temp.append(grp[name][f"step{i + 1}"][...])
                 self.fiber_sec_step_data[name] = temp
         self.key_names = self.fiber_sec_step_data.keys()
 
-    def sec_vis(self,
-                ele_tag: int, sec_tag: int,
-                mat_color: dict = None,
-                ):
+    def sec_vis(
+        self,
+        ele_tag: int,
+        sec_tag: int,
+        mat_color: dict = None,
+    ):
         """plot the fiber section.
 
         Parameters
         ------------
         ele_tag: int
             The element tag to which the section is to be displayed.
         sec_tag: int
@@ -86,40 +92,40 @@
             raise ValueError("ele_tag and sec_tag not in set_fiber_secs()!")
         fiber_data = self.fiber_sec_step_data[key][0][:, :6]
 
         plt.style.use("seaborn")
         # plt.style.use('ggplot')
         fig, ax = plt.subplots(figsize=(6, 6))
         txt = f"ele--sec: {ele_tag}--{sec_tag}\n"
-        _plot_fiber_sec(ax, fiber_data, txt, self.lc,
-                        self.lw, self.cmap, self.opacity, mat_color)
+        _plot_fiber_sec(
+            ax, fiber_data, txt, self.lc, self.lw, self.cmap, self.opacity, mat_color
+        )
         plt.show()
 
-    def _get_fiber_data(self,
-                        key: str,
-                        step: int = None,
-                        show_variable: str = "strain",
-                        show_mats=None,
-                        ):
-
+    def _get_fiber_data(
+        self,
+        key: str,
+        step: int = None,
+        show_variable: str = "strain",
+        show_mats=None,
+    ):
         if key not in self.key_names:
             raise ValueError("ele_tag and sec_tag not in set_fiber_secs()!")
         fiber_step_data = self.fiber_sec_step_data[key]
         fiber_step_data = np.array(fiber_step_data)
 
         if step is None:
             max_resp = []
             for data in fiber_step_data:
                 mat_tags = np.array(data[:, 3], dtype=int)
                 if show_mats is not None:
                     show_mats = np.atleast_1d(show_mats)
                     matidx = []
                     for mat in show_mats:
-                        matidx.append(np.argwhere(
-                            np.abs(mat_tags - mat) < 1e-8))
+                        matidx.append(np.argwhere(np.abs(mat_tags - mat) < 1e-8))
                     matidx = np.vstack(matidx)
                 else:
                     matidx = np.argwhere(np.abs(mat_tags - mat_tags) < 1e-8)
                 if show_variable.lower() == "stress":
                     max_resp.append(np.max(np.abs(data[matidx, 4])))
                 elif show_variable.lower() == "strain":
                     max_resp.append(np.max(np.abs(data[matidx, 5])))
@@ -155,20 +161,22 @@
             raise ValueError("show_variable must be 'stress' or 'strain'!")
 
         ylocs = fiber_data[:, 0]
         zlocs = fiber_data[:, 1]
         areas = fiber_data[:, 2]
         return fiber_data, step_, matidx, vmin, vmax, ylocs, zlocs, areas
 
-    def resp_vis(self,
-                 ele_tag: int, sec_tag: int,
-                 step: int = None,
-                 show_variable: str = "strain",
-                 show_mats=None,
-                 ):
+    def resp_vis(
+        self,
+        ele_tag: int,
+        sec_tag: int,
+        step: int = None,
+        show_variable: str = "strain",
+        show_mats=None,
+    ):
         """fiber section response vis.
 
         Parameters
         -----------
         ele_tag: int
             The element tag to which the section is to be displayed.
         sec_tag: int
@@ -187,16 +195,24 @@
         """
         key = f"{ele_tag}-{sec_tag}"
         if key not in self.key_names:
             raise ValueError("ele_tag and sec_tag not in set_fiber_secs()!")
         # fiber_step_data = fiber_sec_step_data[self.key]
         # fiber_step_data = np.array(fiber_step_data)
 
-        fiber_data, step_, matidx, vmin, vmax, ylocs, zlocs, areas = self._get_fiber_data(
-            key, step, show_variable, show_mats)
+        (
+            fiber_data,
+            step_,
+            matidx,
+            vmin,
+            vmax,
+            ylocs,
+            zlocs,
+            areas,
+        ) = self._get_fiber_data(key, step, show_variable, show_mats)
         ymin, ymax = np.min(ylocs), np.max(ylocs)
         zmin, zmax = np.min(zlocs), np.max(zlocs)
         space_y = (ymax - ymin) / 10
         space_z = (zmax - zmin) / 10
         aspect_ratio = (zmax - zmin) / (ymax - ymin)
         ys_ = ylocs[matidx].ravel()
         zs_ = zlocs[matidx].ravel()
@@ -217,51 +233,60 @@
         plt.style.use("seaborn")
         # plt.style.use('ggplot')
         fig, ax = plt.subplots(figsize=(6, 6 * aspect_ratio))
         patches = [
             plt.Circle((yloc, zloc), np.sqrt(area / np.pi))
             for yloc, zloc, area in zip(ys_, zs_, areas_)
         ]
-        coll = matplotlib.collections.PatchCollection(
-            patches, alpha=self.opacity)
+        coll = matplotlib.collections.PatchCollection(patches, alpha=self.opacity)
         coll.set_ec(self.lc)
         coll.set_lw(self.lw)
         coll.set_cmap(self.cmap)
         coll.set_clim(vmin, vmax)
         coll.set_array(colors)
         ax.add_collection(coll)
         # -------------------------------------------
         #  color bar
-        clb = fig.colorbar(coll, ax=ax, format="%.2E",
-                           use_gridspec=True, location='bottom',
-                           fraction=0.15, aspect=16)
+        clb = fig.colorbar(
+            coll,
+            ax=ax,
+            format="%.2E",
+            use_gridspec=True,
+            location="bottom",
+            fraction=0.15,
+            aspect=16,
+        )
         clb.set_label(show_variable, fontsize=12)
         clb.ax.tick_params(labelsize=9)
         # -----------------------------
         ax.set_aspect(aspect_ratio)
         ax.set_xlim(ymin - space_y, ymax + space_y)
         ax.set_ylim(zmin - space_z, zmax + space_z)
         ax.set_xlabel("y", fontsize=15)
         ax.set_ylabel("z", fontsize=15)
         plt.xticks(fontsize=12)
         plt.yticks(fontsize=12)
-        txt = (f"ele--sec: {ele_tag}--{sec_tag} | step: {step_ + 1}\n"
-               f"$\\rm M_z$={mz:.2E} | $\\rm M_y$={my:.2E} | $\\rm P$={p:.2E} \n"
-               f"$\\rm \\phi_z$={ez:.2E} | $\\rm \\phi_y$={ey:.2E} | $\\rm \\epsilon$={eps:.2E}")
+        txt = (
+            f"ele--sec: {ele_tag}--{sec_tag} | step: {step_ + 1}\n"
+            f"$\\rm M_z$={mz:.2E} | $\\rm M_y$={my:.2E} | $\\rm P$={p:.2E} \n"
+            f"$\\rm \\phi_z$={ez:.2E} | $\\rm \\phi_y$={ey:.2E} | $\\rm \\epsilon$={eps:.2E}"
+        )
         ax.set_title(txt, fontsize=12)
         plt.tight_layout()
         plt.show()
 
-    def animation(self,
-                  output_file: str,
-                  ele_tag: int, sec_tag: int,
-                  show_variable: str = "strain",
-                  show_mats=None,
-                  framerate: int = 24,
-                  ):
+    def animation(
+        self,
+        output_file: str,
+        ele_tag: int,
+        sec_tag: int,
+        show_variable: str = "strain",
+        show_mats=None,
+        framerate: int = 24,
+    ):
         """fiber section response animation.
 
         Parameters
         ----------
         output_file: str
             The output file name, must end with .gif.
         ele_tag: int
@@ -280,18 +305,34 @@
         None
         """
         key = f"{ele_tag}-{sec_tag}"
         if key not in self.key_names:
             raise ValueError("ele_tag and sec_tag not in set_fiber_secs()!")
         fiber_step_data = self.fiber_sec_step_data[key]
 
-        fiber_data, step_max, matidx, vmin, vmax, ylocs, zlocs, areas = self._get_fiber_data(
-            key, None, show_variable, show_mats)
-        fiber_data, step0, matidx, vmin0, vmax0, ylocs, zlocs, areas = self._get_fiber_data(
-            key, 1, show_variable, show_mats)
+        (
+            fiber_data,
+            step_max,
+            matidx,
+            vmin,
+            vmax,
+            ylocs,
+            zlocs,
+            areas,
+        ) = self._get_fiber_data(key, None, show_variable, show_mats)
+        (
+            fiber_data,
+            step0,
+            matidx,
+            vmin0,
+            vmax0,
+            ylocs,
+            zlocs,
+            areas,
+        ) = self._get_fiber_data(key, 1, show_variable, show_mats)
         ymin, ymax = np.min(ylocs), np.max(ylocs)
         zmin, zmax = np.min(zlocs), np.max(zlocs)
         space_y = (ymax - ymin) / 10
         space_z = (zmax - zmin) / 10
         aspect_ratio = (zmax - zmin) / (ymax - ymin)
         my = fiber_data[matidx, 12][0, 0]
         mz = fiber_data[matidx, 11][0, 0]
@@ -304,92 +345,106 @@
         plt.style.use("seaborn")
         # plt.style.use('ggplot')
         fig, ax = plt.subplots(figsize=(8, 8 * aspect_ratio))
         patches = [
             plt.Circle((yloc, zloc), np.sqrt(area / np.pi))
             for yloc, zloc, area in zip(ylocs[matidx], zlocs[matidx], areas[matidx])
         ]
-        coll = matplotlib.collections.PatchCollection(
-            patches, alpha=self.opacity)
+        coll = matplotlib.collections.PatchCollection(patches, alpha=self.opacity)
         coll.set_ec(self.lc)
         coll.set_lw(self.lw)
         coll.set_cmap(self.cmap)
         coll.set_clim(vmin, vmax)
         ax.add_collection(coll)
         # -------------------------------------------
         #  color bar
-        clb = fig.colorbar(coll, ax=ax, format="%.2E",
-                           use_gridspec=True, location='bottom',
-                           fraction=0.15, aspect=16)
+        clb = fig.colorbar(
+            coll,
+            ax=ax,
+            format="%.2E",
+            use_gridspec=True,
+            location="bottom",
+            fraction=0.15,
+            aspect=16,
+        )
         clb.set_label(show_variable, fontsize=12)
         clb.ax.tick_params(labelsize=9)
         # -----------------------------
         ax.set_aspect(aspect_ratio)
         ax.set_xlim(ymin - space_y, ymax + space_y)
         ax.set_ylim(zmin - space_z, zmax + space_z)
         ax.set_xlabel("y", fontsize=15)
         ax.set_ylabel("z", fontsize=15)
         plt.xticks(fontsize=12)
         plt.yticks(fontsize=12)
-        txt = (f"ele--sec: {ele_tag}--{sec_tag} | step: {1}\n"
-               f"$\\rm M_z$={mz:.2E} | $\\rm M_y$={my:.2E} | $\\rm P$={p:.2E} \n"
-               f"$\\rm \\phi_z$={ez:.2E} | $\\rm \\phi_y$={ey:.2E} | $\\rm \\epsilon$={eps:.2E}")
+        txt = (
+            f"ele--sec: {ele_tag}--{sec_tag} | step: {1}\n"
+            f"$\\rm M_z$={mz:.2E} | $\\rm M_y$={my:.2E} | $\\rm P$={p:.2E} \n"
+            f"$\\rm \\phi_z$={ez:.2E} | $\\rm \\phi_y$={ey:.2E} | $\\rm \\epsilon$={eps:.2E}"
+        )
         title = ax.set_title(txt, fontsize=12)
 
         # --------------------------------------------
         def animate(step):
             fiber_data_i = np.array(fiber_step_data[step])
             mat_tagsi = np.array(fiber_data_i[:, 3], dtype=int)
             if show_mats is not None:
                 matidx_i = []
                 for mat_ in show_mats:
-                    matidx_i.append(np.argwhere(
-                        np.abs(mat_tagsi - mat_) < 1e-8))
+                    matidx_i.append(np.argwhere(np.abs(mat_tagsi - mat_) < 1e-8))
                 matidx_i = np.vstack(matidx_i)
             else:
                 matidx_i = np.argwhere(np.abs(mat_tagsi - mat_tagsi) < 1e-8)
 
             # if show_variable == "stress":
             #     vmini = np.min(fiber_data_i[matidx_i, 4])
             #     vmaxi = np.max(fiber_data_i[matidx_i, 4])
             # elif show_variable == "strain":
             #     vmini = np.min(fiber_data_i[matidx_i, 5])
             #     vmaxi = np.max(fiber_data_i[matidx_i, 5])
             # else:
             #     raise ValueError("")
 
-            stressi, straini = fiber_data_i[matidx_i, 4].ravel(), fiber_data_i[matidx_i, 5].ravel()
+            stressi, straini = (
+                fiber_data_i[matidx_i, 4].ravel(),
+                fiber_data_i[matidx_i, 5].ravel(),
+            )
             myi = fiber_data_i[0, 12]
             mzi = fiber_data_i[0, 11]
             pi = fiber_data_i[0, 10]
             eyi = fiber_data_i[0, 8]
             ezi = fiber_data_i[0, 7]
             epsi = fiber_data_i[0, 6]
             colors = stressi if show_variable == "stress" else straini
             coll.set_array(colors)
             coll.set_clim(vmin, vmax)
-            txti = (f"ele--sec: {ele_tag}--{sec_tag} | step: {step + 1}\n"
-                    f"$\\rm M_z$={mzi:.2E} | $\\rm M_y$={myi:.2E} | $\\rm P$={pi:.2E} \n"
-                    f"$\\rm \\phi_z$={ezi:.2E} | $\\rm \\phi_y$={eyi:.2E} | $\\rm \\epsilon$={epsi:.2E}")
+            txti = (
+                f"ele--sec: {ele_tag}--{sec_tag} | step: {step + 1}\n"
+                f"$\\rm M_z$={mzi:.2E} | $\\rm M_y$={myi:.2E} | $\\rm P$={pi:.2E} \n"
+                f"$\\rm \\phi_z$={ezi:.2E} | $\\rm \\phi_y$={eyi:.2E} | $\\rm \\epsilon$={epsi:.2E}"
+            )
             title.set_text(txti)
             # clb.set_ticks(clb.get_ticks())
             # clb.set_ticklabels(
             #     [f"{label:.2E}" for label in clb.get_ticks()], fontsize=13)
             # clb.set_label(show_variable, fontsize=16)
 
         ani = animation.FuncAnimation(
             fig, animate, frames=len(fiber_step_data), blit=False
         )
         plt.show()
         ani.save(output_file, fps=framerate)  # need ffmpeg
 
-    def force_defo_vis(self,
-                       ele_tag: int, sec_tag: int,
-                       force_type: str = "Mz",
-                       defo_type: str = "Phiz"):
+    def force_defo_vis(
+        self,
+        ele_tag: int,
+        sec_tag: int,
+        force_type: str = "Mz",
+        defo_type: str = "Phiz",
+    ):
         """fiber section response vis.
 
         Parameters
         -----------
         ele_tag: int
             The element tag to which the section is to be displayed.
         sec_tag: int
@@ -417,34 +472,45 @@
         forces = []
         defos = []
         for fiber_data in fiber_sec_step:
             forces.append(fiber_data[0, foidx])
             defos.append(fiber_data[0, defoidx])
 
         force_label_map = dict(p="$\\rm P$", mz="$\\rm M_z$", my="$\\rm M_y$")
-        defo_label_map = dict(eps="$\\rm \\epsilon$", phiz="$\\rm \\phi_z$", phiy="$\\rm \\phi_y$")
+        defo_label_map = dict(
+            eps="$\\rm \\epsilon$", phiz="$\\rm \\phi_z$", phiy="$\\rm \\phi_y$"
+        )
         fig, ax = plt.subplots(figsize=(6, 6 * 0.618))
-        ax.plot(defos, forces, lw=1.75, c="blue", )
+        ax.plot(
+            defos,
+            forces,
+            lw=1.75,
+            c="blue",
+        )
         ax.set_ylabel(force_label_map[force_type.lower()], fontsize=16)
         ax.set_xlabel(defo_label_map[defo_type.lower()], fontsize=16)
         plt.xticks(fontsize=12)
         plt.yticks(fontsize=12)
         txt = f"ele--sec: {ele_tag}--{sec_tag}\n"
         ax.set_title(txt, fontsize=15)
         plt.show()
 
         return np.array(defos), np.array(forces)
 
 
-def plot_fiber_sec(ele_sec: list,
-                   results_dir: str = "opstool_output",
-                   input_file: str = 'FiberData.hdf5',
-                   line_width: float = 0.75, line_color: str = 'k',
-                   colormap: str = "viridis", opacity: float = 0.75,
-                   mat_color: dict = None, ):
+def plot_fiber_sec(
+    ele_sec: list,
+    results_dir: str = "opstool_output",
+    input_file: str = "FiberData.hdf5",
+    line_width: float = 0.75,
+    line_color: str = "k",
+    colormap: str = "viridis",
+    opacity: float = 0.75,
+    mat_color: dict = None,
+):
     """plot the fiber section geometry.
 
     Parameters
     ------------
     results_dir: str, default="opstool_output"
         The dir that results saved.
     input_file: str, default='FiberData.hdf5'
@@ -470,15 +536,15 @@
 
     Returns
     ----------
     None
 
     """
     lw, lc = line_width, line_color
-    filename = results_dir + '/' + input_file
+    filename = results_dir + "/" + input_file
     fiber_sec_data = {}
     with h5py.File(filename, "r") as f:
         for name, value in f.items():
             fiber_sec_data[name] = value[...]
     n_sec = len(ele_sec)
     shape = shape_dict[n_sec]
     figsize = 5 * shape[1], 4 * shape[0]
@@ -499,15 +565,15 @@
         txt = f"ele--sec: {ele_tag}--{sec_tag}\n"
         _plot_fiber_sec(ax, fiber_data, txt, lc, lw, colormap, opacity, mat_color)
     if shape[0] * shape[1] > n_sec:
         for i in range(n_sec, shape[0] * shape[1]):
             idxi = int(np.ceil((i + 1) / shape[1]) - 1)
             idxj = int(i - idxi * shape[1])
             ax = axs[idxi, idxj]
-            with plt.style.context('classic'):
+            with plt.style.context("classic"):
                 ax.set_visible(False)
 
     plt.subplots_adjust(hspace=0.3)
     plt.show()
 
 
 def _plot_fiber_sec(ax, fiber_data, title, lc, lw, cmap, opacity, mat_color):
@@ -529,16 +595,15 @@
     # --------------------------------------------------------------
     # start plot
     # --------------------------------------------------------------
     patches = [
         plt.Circle((yloc, zloc), np.sqrt(area / np.pi))
         for yloc, zloc, area in zip(ylocs, zlocs, areas)
     ]
-    coll = matplotlib.collections.PatchCollection(
-        patches, alpha=opacity)
+    coll = matplotlib.collections.PatchCollection(patches, alpha=opacity)
     coll.set_array(scalars)
     coll.set_ec(lc)
     coll.set_lw(lw)
     coll.set_cmap(cmap)
     ax.add_collection(coll)
 
     # If mat_color
@@ -560,9 +625,8 @@
             ax.add_collection(coll)
     ax.set_aspect(aspect_ratio)
     ax.set_xlim(ymin - space_y, ymax + space_y)
     ax.set_ylim(zmin - space_z, zmax + space_z)
     ax.set_xlabel("y", fontsize=16)
     ax.set_ylabel("z", fontsize=16)
     ax.tick_params(labelsize=12)
-    ax.text(0.5, 1.0, title, ha='center', fontsize=15,
-            va='top', transform=ax.transAxes)
+    ax.text(0.5, 1.0, title, ha="center", fontsize=15, va="top", transform=ax.transAxes)
```

### Comparing `opstool-0.7.3/src/opstool/vis/get_model_data.py` & `opstool-0.8.0/src/opstool/vis/get_model_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,30 +7,35 @@
 import h5py
 import numpy as np
 import openseespy.opensees as ops
 from numpy.typing import ArrayLike
 from rich import print
 
 from ..utils import check_file
-from ._get_model_base import (get_beam_info2, get_beam_resp, get_model_info,
-                              get_node_coords, get_node_react, get_node_resp)
+from ._get_model_base import (
+    get_beam_info2,
+    get_beam_resp,
+    get_model_info,
+    get_node_coords,
+    get_node_react,
+    get_node_resp,
+)
 
 
 class GetFEMdata:
     """
     Get the data in the ``openseespy`` current domain.
 
     Parameters
     ----------
     results_dir: str, default="opstool_output"
         The directory that results to save.
     """
 
     def __init__(self, results_dir: str = "opstool_output"):
-
         self.out_dir = results_dir
         if not os.path.exists(self.out_dir):
             os.makedirs(self.out_dir)
 
         self.model_info = dict()
         self.get_model_data_finished = False
 
@@ -49,38 +54,49 @@
         self.node_resp_steps = dict()
         self.step_node_track = 0
         # node reactions
         self.node_react_steps = []
         self.step_react_track = 0
 
         self.beam_infos = dict()
-        self.beam_resp_names = ['localForces']
+        self.beam_resp_names = ["localForces"]
         # 'basicDeformations'
         self.beam_resp_step = dict()
         # ["N_1", "Vy_1", "Vz_1", "T_1", "My_1", "Mz_1",
         #  "N_2", "Vy_2", "Vz_2", "T_2", "My_2", "Mz_2"]
         # ["eps", "thetaZ_1", "thetaZ_2", "thetaY_1", "thetaY_2", "thetaX"]
         self.step_beam_track = 0
 
         # On/Off and Tracking for Model Updates
         self.model_update = False
+        self.resp_step_track = 0
 
         # self.reset_model_state()
         # self.reset_eigen_state()
         self.reset_steps_state()
 
         # fiber section data
         self.fiber_sec_tags = []
         self.fiber_sec_data = dict()
         self.fiber_sec_step_data = dict()
         self.step_fiber_track = 0
 
         # terminal print colors
-        colors = ['#00aeff', '#3369e7', '#8e43e7', '#b84592', '#ff4f81',
-                  '#ff6c5f', '#ffc168', '#2dde98', '#1cc7d0', '#49a942']
+        colors = [
+            "#00aeff",
+            "#3369e7",
+            "#8e43e7",
+            "#b84592",
+            "#ff4f81",
+            "#ff6c5f",
+            "#ffc168",
+            "#2dde98",
+            "#1cc7d0",
+            "#49a942",
+        ]
         self.colors_cycle = cycle(colors)
 
     def reset_model_state(self):
         """Reset the state of results extract of model data."""
         for name in self.model_info.keys():
             self.model_info[name] = None
         for name in self.cells.keys():
@@ -92,16 +108,16 @@
             self.eigen[name] = None
 
     def _reset_model_step(self):
         for name in self.model_info.keys():
             self.model_info_steps[name] = []
         for name in self.cells.keys():
             self.cells_steps[name] = []
-        self.model_info_steps['step_track'] = 0
-        self.cells_steps['step_track'] = 0
+        self.model_info_steps["step_track"] = 0
+        self.cells_steps["step_track"] = 0
 
     def _reset_node_react(self):
         self.step_react_track = 0
         self.node_react_steps = []
 
     def _reset_node_resp(self):
         self.step_node_track = 0
@@ -128,21 +144,23 @@
         """
 
         self._reset_model_step()
         self._reset_node_react()
         self._reset_node_resp()
         self._reset_beam_step()
         self._reset_fiber_step()
+        self.resp_step_track = 0
 
         # Truss Element Analysis Step Response Data
 
         # Beam Element Analysis Step Response Data
 
-    def get_model_data(self, beam_sec: dict = None,
-                       save_file: Union[str, bool] = "ModelData.hdf5"):
+    def get_model_data(
+        self, beam_sec: dict = None, save_file: Union[str, bool] = "ModelData.hdf5"
+    ):
         """Get data from the current model domain.
         The data will saved to file ``results_dir`` + ``save_file`` in hdf5 style.
 
         Parameters
         -----------
         beam_sec: dict, default=None
             Specifies the section geometry for some beam or truss elements for 3D rendering.
@@ -154,37 +172,38 @@
 
             .. warning::
                 Be careful not to include any path, only filename,
                 the file will be saved to the directory ``results_dir``.
 
         """
         if save_file:
-            check_file(save_file, ['.hdf5', '.h5', '.he5'])
+            check_file(save_file, [".hdf5", ".h5", ".he5"])
         # --------------------------------
         model_info, cells = get_model_info(sec_mesh=beam_sec)
         self.model_info.update(model_info)
         self.cells.update(cells)
         self.get_model_data_finished = True
         if save_file:
-            output_filename = self.out_dir + '/' + save_file
+            output_filename = self.out_dir + "/" + save_file
             with h5py.File(output_filename, "w") as f:
                 grp1 = f.create_group("ModelInfo")
                 for name, value in self.model_info.items():
                     grp1.create_dataset(name, data=value)
                 grp2 = f.create_group("Cell")
                 for name, value in self.cells.items():
                     grp2.create_dataset(name, data=value)
             print(
-                f"Model data saved in [bold {next(self.colors_cycle)}]{output_filename}[/]!")
+                f"Model data saved in [bold {next(self.colors_cycle)}]{output_filename}[/]!"
+            )
 
     def get_eigen_data(
-            self,
-            mode_tag: int = 1,
-            solver: str = "-genBandArpack",
-            save_file: str = 'EigenData.hdf5',
+        self,
+        mode_tag: int = 1,
+        solver: str = "-genBandArpack",
+        save_file: str = "EigenData.hdf5",
     ):
         """Get eigenvalue Analysis Data.
         The data will saved to file ``results_dir`` + ``save_file``.
 
         Parameters
         ----------
         mode_tag: int
@@ -202,15 +221,15 @@
 
         Returns
         -------
         None
         """
         # ----------------------------------
         if save_file:
-            check_file(save_file, ['.hdf5', '.h5', '.he5'])
+            check_file(save_file, [".hdf5", ".h5", ".he5"])
         self.get_model_data(save_file=False)
         self.reset_eigen_state()
         # ----------------------------------
         ops.wipeAnalysis()
         if mode_tag == 1:
             eigen_values = ops.eigen(solver, 2)[:1]
         else:
@@ -240,29 +259,32 @@
             eigenvectors.append(eigen_vector)
         self.eigen["eigenvector"] = eigenvectors
 
         self.eigen.update(self.model_info)
         self.eigen.update(self.cells)
         # ----------------------------------------------------------------
         if save_file:
-            output_filename = self.out_dir + '/' + save_file
+            output_filename = self.out_dir + "/" + save_file
             with h5py.File(output_filename, "w") as f:
                 grp = f.create_group("EigenInfo")
                 for name, value in self.eigen.items():
                     grp.create_dataset(name, data=value)
             print(
-                f"Eigen data saved in [bold {next(self.colors_cycle)}]{output_filename}[/] !")
+                f"Eigen data saved in [bold {next(self.colors_cycle)}]{output_filename}[/]!"
+            )
 
-    def get_node_react_step(self,
-                            dynamic: bool = False,
-                            rayleigh: bool = False,
-                            num_steps: int = 10000000000000,
-                            total_time: float = 10000000000000,
-                            stop_cond: bool = False,
-                            save_file: Union[str, bool] = "NodeReactionStepData-1.hdf5", ):
+    def get_node_react_step(
+        self,
+        dynamic: bool = False,
+        rayleigh: bool = False,
+        num_steps: int = 10000000000000,
+        total_time: float = 10000000000000,
+        stop_cond: bool = False,
+        save_file: Union[str, bool] = "NodeReactionStepData-1.hdf5",
+    ):
         """Get one step the node reactions data.
 
         Parameters
         ----------
         dynamic : bool, optional, by default False
             If True, include dynamic effects.
         rayleigh : bool, optional, by default False
@@ -286,28 +308,33 @@
                 Be careful not to include any path, only filename,
                 the file will be saved to the directory ``results_dir``.
                 You need to specify different suffixes to distinguish between the different analysis cases.
                 Such as "NodeReactionStepData-1.hdf5", "NodeReactionStepData-2.hdf5", etc.
         """
         args = []
         if dynamic:
-            args.append('-dynamic')
+            args.append("-dynamic")
         if rayleigh:
-            args.append('-rayleigh')
+            args.append("-rayleigh")
         ops.reactions(*args)
         fixed_nodes = ops.getFixedNodes()
         self.node_react_steps.append(get_node_react(fixed_nodes))
         self.step_react_track += 1
         # --------------------------------
         if save_file:
-            if self.step_node_track >= num_steps or ops.getTime() >= total_time or stop_cond:
-                output_filename = self.out_dir + '/' + save_file
+            if (
+                self.step_node_track >= num_steps
+                or ops.getTime() >= total_time
+                or stop_cond
+            ):
+                output_filename = self.out_dir + "/" + save_file
                 self._save_node_react_step(output_filename, "w")
                 print(
-                    f"Node reaction data saved in [bold {next(self.colors_cycle)}]{output_filename}[/] !")
+                    f"Node reaction data saved in [bold {next(self.colors_cycle)}]{output_filename}[/]!"
+                )
 
     def _save_node_react_step(self, filename: str, mode: str = "w"):
         _, _, model_dims, _ = get_node_coords()
         fixed_nodes = ops.getFixedNodes()
         node_coords = np.zeros((len(fixed_nodes), 3))
         for i, tag in enumerate(fixed_nodes):
             coord = ops.nodeCoord(tag)
@@ -323,23 +350,24 @@
                 f.create_dataset("Nsteps", data=n)
             if "model_dims" not in f.keys():
                 f.create_dataset("model_dims", data=model_dims)
             f.create_dataset("NodeReactCoords", data=node_coords)
             f.create_dataset("NodeReactTags", data=fixed_nodes)
             grp = f.create_group("NodeReactSteps")
             for i in range(n):
-                grp.create_dataset(
-                    f"step{i + 1}", data=self.node_react_steps[i])
+                grp.create_dataset(f"step{i + 1}", data=self.node_react_steps[i])
 
-    def get_node_resp_step(self,
-                           num_steps: int = 10000000000000,
-                           total_time: float = 10000000000000,
-                           stop_cond: bool = False,
-                           save_file: Union[str, bool] = "NodeRespStepData-1.hdf5",
-                           model_update: bool = False):
+    def get_node_resp_step(
+        self,
+        num_steps: int = 10000000000000,
+        total_time: float = 10000000000000,
+        stop_cond: bool = False,
+        save_file: Union[str, bool] = "NodeRespStepData-1.hdf5",
+        model_update: bool = False,
+    ):
         """Get the node response data one step.
 
         .. note::
             You need to call this function at each analysis step in OpenSees.
             The advantage is that you can modify the iterative algorithm at
             each analysis step to facilitate convergence.
 
@@ -372,92 +400,95 @@
             For example, some elements and nodes were removed.
 
         Returns
         -------
         None
         """
         if save_file:
-            check_file(save_file, ['.hdf5', '.h5', '.he5'])
+            check_file(save_file, [".hdf5", ".h5", ".he5"])
         if model_update:
             self.get_model_data(save_file=False)
         else:
             if not self.get_model_data_finished:
                 self.get_model_data()
 
         node_tags = self.model_info["NodeTags"]
-        (node_disp, node_vel, node_accel,
-         node_deform_coord) = get_node_resp(node_tags)
+        (node_disp, node_vel, node_accel, node_deform_coord) = get_node_resp(node_tags)
 
         self.node_resp_steps["disp"].append(node_disp)
         self.node_resp_steps["vel"].append(node_vel)
         self.node_resp_steps["accel"].append(node_accel)
 
         if model_update:
-            if self.step_node_track == self.model_info_steps['step_track']:
+            if self.step_node_track == 0:
+                self._reset_model_step()
+            if self.step_node_track == self.model_info_steps["step_track"]:
                 for name in self.model_info.keys():
                     self.model_info_steps[name].append(self.model_info[name])
-                self.model_info_steps['step_track'] += 1
-            if self.step_node_track == self.cells_steps['step_track']:
+                self.model_info_steps["step_track"] += 1
+            if self.step_node_track == self.cells_steps["step_track"]:
                 for name in self.cells.keys():
                     self.cells_steps[name].append(self.cells[name])
-                self.cells_steps['step_track'] += 1
+                self.cells_steps["step_track"] += 1
         else:
             if self.step_node_track == 0:
                 self.model_info_steps.update(self.model_info)
                 self.cells_steps.update(self.cells)
         # --------------------------------
         self.model_update = model_update
         self.step_node_track += 1
         # --------------------------------
         if save_file:
-            if self.step_node_track >= num_steps or ops.getTime() >= total_time or stop_cond:
-                output_filename = self.out_dir + '/' + save_file
+            if (
+                self.step_node_track >= num_steps
+                or ops.getTime() >= total_time
+                or stop_cond
+            ):
+                output_filename = self.out_dir + "/" + save_file
                 self._save_node_resp_step(output_filename, "w")
                 print(
-                    f"Node response data saved in [bold {next(self.colors_cycle)}]{output_filename}[/] !")
+                    f"Node response data saved in [bold {next(self.colors_cycle)}]{output_filename}[/]!"
+                )
 
-    def _save_node_resp_step(self,
-                             filename: str,
-                             mode: str = "w"):
+    def _save_node_resp_step(self, filename: str, mode: str = "w"):
         with h5py.File(filename, mode) as f:
-            n = len(self.node_resp_steps['disp'])
+            n = len(self.node_resp_steps["disp"])
             if "Nsteps" not in f.keys():
                 f.create_dataset("Nsteps", data=n)
             grp1 = f.create_group("ModelInfoSteps")
             grp2 = f.create_group("CellSteps")
             grp3 = f.create_group("NodeRespSteps")
             for name, value in self.model_info_steps.items():
-                if name not in ['step_track']:
+                if name not in ["step_track"]:
                     if self.model_update:
                         subgrp = grp1.create_group(name)
                         for i in range(n):
-                            subgrp.create_dataset(
-                                f"step{i + 1}", data=value[i])
+                            subgrp.create_dataset(f"step{i + 1}", data=value[i])
                     else:
                         grp1.create_dataset(name, data=value)
             for name, value in self.cells_steps.items():
-                if name not in ['step_track']:
+                if name not in ["step_track"]:
                     if self.model_update:
                         subgrp = grp2.create_group(name)
                         for i in range(n):
-                            subgrp.create_dataset(
-                                f"step{i + 1}", data=value[i])
+                            subgrp.create_dataset(f"step{i + 1}", data=value[i])
                     else:
                         grp2.create_dataset(name, data=value)
             for name, value in self.node_resp_steps.items():
                 subgrp = grp3.create_group(name)
                 for i in range(n):
                     subgrp.create_dataset(f"step{i + 1}", data=value[i])
 
-    def get_frame_resp_step(self,
-                            num_steps: int = 10000000000000,
-                            total_time: float = 10000000000000,
-                            stop_cond: bool = False,
-                            save_file: Union[str, bool] = "BeamRespStepData-1.hdf5"
-                            ):
+    def get_frame_resp_step(
+        self,
+        num_steps: int = 10000000000000,
+        total_time: float = 10000000000000,
+        stop_cond: bool = False,
+        save_file: Union[str, bool] = "BeamRespStepData-1.hdf5",
+    ):
         """Get the response data one step.
 
         .. note::
             You need to call this function at each analysis step in OpenSees.
             The advantage is that you can modify the iterative algorithm at
             each analysis step to facilitate convergence.
 
@@ -485,53 +516,67 @@
                 Such as "BeamRespStepData-1.hdf5", "BeamRespStepData-2.hdf5", etc.
 
         Returns
         -------
         None
         """
         if save_file:
-            check_file(save_file, ['.hdf5', '.h5', '.he5'])
+            check_file(save_file, [".hdf5", ".h5", ".he5"])
 
-        (beam_tags, beam_node_coords, beam_cells,
-         xlocals, ylocals, zlocals, bounds) = get_beam_info2()
-        self.beam_infos['beam_tags'] = beam_tags
-        self.beam_infos['beam_node_coords'] = beam_node_coords
-        self.beam_infos['beam_cells'] = beam_cells
-        self.beam_infos['xlocal'] = xlocals
-        self.beam_infos['ylocal'] = ylocals
-        self.beam_infos['zlocal'] = zlocals
-        self.beam_infos['bounds'] = bounds
+        (
+            beam_tags,
+            beam_node_coords,
+            beam_cells,
+            xlocals,
+            ylocals,
+            zlocals,
+            bounds,
+        ) = get_beam_info2()
+        self.beam_infos["beam_tags"] = beam_tags
+        self.beam_infos["beam_node_coords"] = beam_node_coords
+        self.beam_infos["beam_cells"] = beam_cells
+        self.beam_infos["xlocal"] = xlocals
+        self.beam_infos["ylocal"] = ylocals
+        self.beam_infos["zlocal"] = zlocals
+        self.beam_infos["bounds"] = bounds
 
         beam_resp_steps = get_beam_resp(beam_tags)
-        self.beam_resp_step['localForces'].append(beam_resp_steps)
+        self.beam_resp_step["localForces"].append(beam_resp_steps)
         # ----------------------------------------------------------------
         self.step_beam_track += 1
         # ------------------------------------------
         if save_file:
-            if self.step_beam_track >= num_steps or ops.getTime() >= total_time or stop_cond:
-                output_filename = self.out_dir + '/' + save_file
+            if (
+                self.step_beam_track >= num_steps
+                or ops.getTime() >= total_time
+                or stop_cond
+            ):
+                output_filename = self.out_dir + "/" + save_file
                 self._save_frame_resp_step(output_filename, "w")
                 print(
-                    f"Frame elements response data saved in [bold {next(self.colors_cycle)}]{output_filename}[/] !")
+                    f"Frame elements response data saved in [bold {next(self.colors_cycle)}]{output_filename}[/]!"
+                )
 
     def _save_frame_resp_step(self, filename: str, mode: str = "w"):
         with h5py.File(filename, mode) as f:
-            n = len(self.beam_resp_step['localForces'])
+            n = len(self.beam_resp_step["localForces"])
             if "Nsteps" not in f.keys():
                 f.create_dataset("Nsteps", data=n)
             grp1 = f.create_group("BeamInfos")
             grp2 = f.create_group("BeamRespSteps")
             for name, value in self.beam_infos.items():
                 grp1.create_dataset(name, data=value)
             for name, value in self.beam_resp_step.items():
                 subgrp = grp2.create_group(name)
                 for i in range(n):
                     subgrp.create_dataset(f"step{i + 1}", data=value[i])
 
-    def get_fiber_data(self, ele_sec: list, save_file: Union[str, bool] = 'FiberData.hdf5'):
+    def get_fiber_data(
+        self, ele_sec: list, save_file: Union[str, bool] = "FiberData.hdf5"
+    ):
         """Get data from the section assigned by parameter ele_sec.
 
         Parameters
         ----------
         ele_sec: list[tuple[int, int]]
             A list or tuple composed of element tag and sectag.
             e.g., [(ele1, sec1), (ele2, sec2), ... , (elen, secn)],
@@ -545,41 +590,44 @@
                 the file will be saved to the directory ``results_dir``.
 
         Returns
         -------
         None
         """
         if save_file:
-            check_file(save_file, ['.hdf5', '.h5', '.he5'])
+            check_file(save_file, [".hdf5", ".h5", ".he5"])
         self.fiber_sec_tags.extend(ele_sec)
         for ele_sec_i in self.fiber_sec_tags:
             key = f"{ele_sec_i[0]}-{ele_sec_i[1]}"
             self.fiber_sec_data[key] = []
 
         # get data
         for ele_sec_i in self.fiber_sec_tags:
             ele_tag = ele_sec_i[0]
             sec_tag = ele_sec_i[1]
             key = f"{ele_sec_i[0]}-{ele_sec_i[1]}"
             fiber_data = _get_fiber_sec_data(ele_tag, sec_tag)
             self.fiber_sec_data[key] = fiber_data
         # ---------------------------------------------
         if save_file:
-            output_filename = self.out_dir + '/' + save_file
+            output_filename = self.out_dir + "/" + save_file
             with h5py.File(output_filename, "w") as f:
                 for name, value in self.fiber_sec_data.items():
                     f.create_dataset(name, data=value)
             print(
-                f"Fiber section data saved in [bold {next(self.colors_cycle)}]{output_filename}[/] !")
+                f"Fiber section data saved in [bold {next(self.colors_cycle)}]{output_filename}[/]!"
+            )
 
-    def get_fiber_resp_step(self,
-                            num_steps: int = 10000000000000,
-                            total_time: float = 10000000000000,
-                            stop_cond: bool = False,
-                            save_file: Union[str, bool] = "FiberRespStepData-1.hdf5"):
+    def get_fiber_resp_step(
+        self,
+        num_steps: int = 10000000000000,
+        total_time: float = 10000000000000,
+        stop_cond: bool = False,
+        save_file: Union[str, bool] = "FiberRespStepData-1.hdf5",
+    ):
         """Get analysis results data for fiber section one step.
 
         Parameters
         ----------
         num_steps: int, default=10000000000000
             Total number of steps, set to determine when to save data.
         total_time: float, default=10000000000000
@@ -602,59 +650,74 @@
                 Such as "FiberRespStepData-1.hdf5", "FiberRespStepData-2.hdf5", etc.
 
         Returns
         -------
         None
         """
         if save_file:
-            check_file(save_file, ['.hdf5', '.h5', '.he5'])
+            check_file(save_file, [".hdf5", ".h5", ".he5"])
 
         if self.step_fiber_track == 0:
             for ele_sec_i in self.fiber_sec_tags:
                 key = f"{ele_sec_i[0]}-{ele_sec_i[1]}"
                 self.fiber_sec_step_data[key] = []
 
         for ele_sec_i in self.fiber_sec_tags:
             ele_tag = ele_sec_i[0]
             sec_tag = ele_sec_i[1]
             key = f"{ele_sec_i[0]}-{ele_sec_i[1]}"
             fiber_data = _get_fiber_sec_data(ele_tag, sec_tag)
             defo_fo = ops.eleResponse(
-                ele_tag, "section", sec_tag, "forceAndDeformation")
+                ele_tag, "section", sec_tag, "forceAndDeformation"
+            )
             if len(defo_fo) == 4:
-                defo_fo = [defo_fo[0], defo_fo[1], 0., 0.,
-                           defo_fo[2], defo_fo[3], 0., 0.]
+                defo_fo = [
+                    defo_fo[0],
+                    defo_fo[1],
+                    0.0,
+                    0.0,
+                    defo_fo[2],
+                    defo_fo[3],
+                    0.0,
+                    0.0,
+                ]
             sec_defo_fo = np.array([defo_fo] * len(fiber_data), dtype=float)
             data = np.hstack([fiber_data, sec_defo_fo])
             self.fiber_sec_step_data[key].append(data)
         # ------------------------
         self.step_fiber_track += 1
         # ------------------------
         if save_file:
-            if self.step_fiber_track >= num_steps or ops.getTime() >= total_time or stop_cond:
-                output_filename = self.out_dir + '/' + save_file
+            if (
+                self.step_fiber_track >= num_steps
+                or ops.getTime() >= total_time
+                or stop_cond
+            ):
+                output_filename = self.out_dir + "/" + save_file
                 self._save_fiber_resp_step(output_filename, "w")
                 print(
-                    f"Fiber section responses data saved in [bold {next(self.colors_cycle)}]{output_filename}[/] !")
+                    f"Fiber section responses data saved in [bold {next(self.colors_cycle)}]{output_filename}[/]!"
+                )
 
     def _save_fiber_resp_step(self, filename: str, mode: str = "w"):
         with h5py.File(filename, mode) as f:
             if "Nsteps" not in f.keys():
                 f.create_dataset("Nsteps", data=self.step_fiber_track)
             grp = f.create_group("FiberRespSteps")
             for name, value in self.fiber_sec_step_data.items():
                 subgrp = grp.create_group(name)
                 for i in range(self.step_fiber_track):
                     subgrp.create_dataset(f"step{i + 1}", data=value[i])
 
-    def get_resp_step(self,
-                      dynamic: bool = False,
-                      rayleigh: bool = False,
-                      model_update: bool = False,
-                      ):
+    def get_resp_step(
+        self,
+        dynamic: bool = False,
+        rayleigh: bool = False,
+        model_update: bool = False,
+    ):
         """Get all currently supported responses in one step.
 
         .. note::
                 This method needs to be used in conjunction with :meth:`opstool.vis.GetFEMdata.save_resp_all`.
 
         Parameters
         ----------
@@ -662,26 +725,25 @@
             If True, node reactions will include dynamic effects.
         rayleigh : bool, optional, by default False
             If True, node reactions will include rayleigh damping.
         model_update: bool, optional, by default False
             whether to update the model domain data at each analysis step,
             this will be useful if model data has changed.
             For example, some elements and nodes were removed.
-            This parameter is currently only valid for getting node response data, i.e., 
+            This parameter is currently only valid for getting node response data, i.e.,
             :meth:`opstool.vis.GetFEMdata.get_node_resp_step`.
         """
         self.get_node_resp_step(save_file=False, model_update=model_update)
-        self.get_node_react_step(
-            dynamic=dynamic, rayleigh=rayleigh, save_file=False)
+        self.get_node_react_step(dynamic=dynamic, rayleigh=rayleigh, save_file=False)
         self.get_frame_resp_step(save_file=False)
         self.get_fiber_resp_step(save_file=False)
 
-    def save_resp_all(self,
-                      save_file: str = "RespStepData-1.hdf5",
-                      reset_state: bool = True):
+    def save_resp_all(
+        self, save_file: str = "RespStepData-1.hdf5", reset_state: bool = True
+    ):
         """Save all responses data for all analysis steps at once.
         This means you need to call it after the loop is over.
 
         Parameters
         ----------
         save_file : str, optional, by default "RespStepData-1.hdf5"
             The file name that data saved.
@@ -692,29 +754,30 @@
                 the file will be saved to the directory ``results_dir``.
                 You need to specify different suffixes to distinguish between the different analysis cases.
                 Such as "RespStepData-1.hdf5", "RespStepData-2.hdf5", etc.
 
         reset_state : bool, optional, by default True
             If True, the response data from previous analysis cases will be cleared, otherwise it will be included.
         """
-        filename = self.out_dir + '/' + save_file
+        filename = self.out_dir + "/" + save_file
         if os.path.isfile(filename):
             os.remove(filename)
         if self.node_resp_steps["disp"]:
             self._save_node_resp_step(filename, "w")
         if self.node_react_steps:
             self._save_node_react_step(filename, "a")
-        if self.beam_resp_step['localForces']:
+        if self.beam_resp_step["localForces"]:
             self._save_frame_resp_step(filename, "a")
         if self.fiber_sec_step_data:
             self._save_fiber_resp_step(filename, "a")
         if reset_state:
             self.reset_steps_state()
         print(
-            f"All responses data saved in [bold {next(self.colors_cycle)}]{filename}[/] !")
+            f"All responses data saved in [bold {next(self.colors_cycle)}]{filename}[/]!"
+        )
 
 
 def _get_fiber_sec_data(ele_tag: int, sec_tag: int = 1):
     """Get the fiber sec data for a beam element.
 
     Parameters
     ----------
```

### Comparing `opstool-0.7.3/src/opstool/vis/ops_vis_plotly.py` & `opstool-0.8.0/src/opstool/vis/ops_vis_pyvista.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,72 @@
 """
-Visualizing OpenSeesPy model
+Visualizing OpenSeesPy model based on pyvista
 """
 
-from ._plotly_base import (_deform_anim, _deform_vis, _eigen_anim, _eigen_vis,
-                           _frame_resp_vis, _model_vis, _react_vis)
+import pyvista as pv
 
-
-class OpsVisPlotly:
-    """A class to visualize OpenSeesPy model based on plotly.
+from ..utils import check_file
+from ._pyvista_base import (
+    _deform_anim,
+    _deform_vis,
+    _eigen_anim,
+    _eigen_vis,
+    _frame_resp_vis,
+    _model_vis,
+    _react_vis,
+)
+
+
+class OpsVisPyvista:
+    """A class to visualize OpenSeesPy model based on
+    `pyvista <https://docs.pyvista.org/index.html>`_.
 
     Parameters
-    ----------
-    point_size: float
+    -----------
+    point_size: float, default=1
         The render size of node.
-    line_width: float
-        The width of line element;
+    line_width: float, default=3
+        The width of line element.
     colors_dict: dict,
         The dict for ele color, default color you can see by the class attribute ``default_colors``.
-    theme: str, default=plotly
-        Plot theme, optional "plotly", "plotly_white", "plotly_dark", "ggplot2", "seaborn", "simple_white", "none".
+    theme: str, default='document'
+        Plot theme for pyvista, optional 'default', 'paraview', 'document', 'dark'.
     color_map: str, default="jet"
-        color map to display the cloud plot. Optional, [‘aggrnyl’, ‘agsunset’, ‘algae’, ‘amp’, ‘armyrose’, ‘balance’,
-        ‘blackbody’, ‘bluered’, ‘blues’, ‘blugrn’, ‘bluyl’, ‘brbg’, ‘brwnyl’, ‘bugn’, ‘bupu’, ‘burg’, ‘burgyl’,
-        ‘cividis’, ‘curl’, ‘darkmint’, ‘deep’, ‘delta’, ‘dense’, ‘earth’, ‘edge’, ‘electric’, ‘emrld’, ‘fall’,
-        ‘geyser’, ‘gnbu’, ‘gray’, ‘greens’, ‘greys’, ‘haline’, ‘hot’, ‘hsv’, ‘ice’, ‘icefire’, ‘inferno’, ‘jet’,
-        ‘magenta’, ‘magma’, ‘matter’, ‘mint’, ‘mrybm’, ‘mygbm’, ‘oranges’, ‘orrd’, ‘oryel’, ‘oxy’, ‘peach’, ‘phase’,
-        ‘picnic’, ‘pinkyl’, ‘piyg’, ‘plasma’, ‘plotly3’, ‘portland’, ‘prgn’, ‘pubu’, ‘pubugn’, ‘puor’, ‘purd’, ‘purp’,
-        ‘purples’, ‘purpor’, ‘rainbow’, ‘rdbu’, ‘rdgy’, ‘rdpu’, ‘rdylbu’, ‘rdylgn’, ‘redor’, ‘reds’, ‘solar’,
-        ‘spectral’, ‘speed’, ‘sunset’, ‘sunsetdark’, ‘teal’, ‘tealgrn’, ‘tealrose’, ‘tempo’, ‘temps’, ‘thermal’,
-        ‘tropic’, ‘turbid’, ‘turbo’, ‘twilight’, ‘viridis’, ‘ylgn’, ‘ylgnbu’, ‘ylorbr’, ‘ylorrd’].
+        color map to display the cloud plot for pyvista.
+        optional 'jet', 'rainbow', 'hot', 'afmhot', 'copper', 'winter', 'cool', 'coolwarm', 'gist_earth',
+        'bone', 'binary', 'gray', or any
+        `Matplotlib colormap <https://matplotlib.org/stable/tutorials/colors/colormaps.html>`_ .
     on_notebook: bool, default=False
-        Whether work in a jupyter notebook.
+        Whether work in a notebook.
     results_dir: str, default="opstool_output"
         The dir that results saved.
 
     Returns
-    -------
+    --------
     None
     """
 
     def __init__(
         self,
-        point_size: float = 5,
-        line_width: float = 5,
+        point_size: float = 1,
+        line_width: float = 3,
         colors_dict: dict = None,
-        theme: str = "plotly",
+        theme: str = "document",
         color_map: str = "jet",
         on_notebook: bool = False,
-        results_dir: str = "opstool_output"
+        results_dir: str = "opstool_output",
     ):
         # ------------------------------
         self.point_size = point_size
         self.line_width = line_width
-        self.title = "OpenSeesVispy"
+        self.title = "opstool"
         # Initialize the color dict
         colors = dict(
             point="#580f41",
-            line="#037ef3",
+            line="#0504aa",
             face="#00c16e",
             solid="#0cb9c1",
             truss="#7552cc",
             link="#01ff07",
             constraint="#00ffff",
         )
         if colors_dict is not None:
@@ -68,37 +74,43 @@
         self.default_colors = colors
         self.color_point = colors["point"]
         self.color_line = colors["line"]
         self.color_face = colors["face"]
         self.color_solid = colors["solid"]
         self.color_truss = colors["truss"]
         self.color_link = colors["link"]
-        self.color_constraint = colors['constraint']
+        self.color_constraint = colors["constraint"]
         # -------------------------------------------------
         self.theme = theme
+        pv.set_plot_theme(theme)
         self.color_map = color_map
-
         self.notebook = on_notebook
         # -------------------------------------------------
         self.out_dir = results_dir
         # -------------------------------------------------
-        self.bound_fact = 30
+        self.bound_fact = 20
 
     def model_vis(
         self,
         input_file: str = "ModelData.hdf5",
         show_node_label: bool = False,
         show_ele_label: bool = False,
+        label_size: float = 10,
         show_local_crd: bool = False,
+        local_crd_alpha: float = 1.0,
         show_fix_node: bool = True,
+        fix_node_alpha: float = 1.0,
+        show_load: bool = False,
+        load_alpha: float = 1.0,
         show_constrain_dof: bool = False,
-        label_size: float = 8,
+        show_beam_sec: bool = False,
+        beam_sec_paras: dict = None,
         show_outline: bool = True,
         opacity: float = 1.0,
-        save_html: str = 'ModelVis.html'
+        save_fig: str = "ModelVis.svg",
     ):
         """
         Visualize the model in the current domain.
 
         Parameters
         ----------
         input_file: str, default = "ModelData.hdf5",
@@ -111,56 +123,98 @@
 
         show_node_label: bool, default=False
             Whether to display the node label.
         show_ele_label: bool, default=False
             Whether to display the ele label.
         show_local_crd: bool, default=False
             Whether to display the local axes of beam and link elements.
+        local_crd_alpha: float, default=1.0
+            On existing displays, the scaling factor for the local axis sizes.
         show_fix_node: bool, default=True
             Whether to display the fix nodes.
+        fix_node_alpha: float, default=1.0
+            On existing displays, the scaling factor for the boundary symbol sizes.
+        show_load: bool, default = False
+            Whether to display node and beam element loads.
+            The sizes of the arrow are related to the size of its load.
+            If you want to further control the size, you can use `load_alpha`.
+            Currently only supported beam element load types include
+            <beamUniform2D, beamUniform3D, beamPoint2D, beamPoint3D>.
+
+            .. note::
+                Please make sure that all dofs (or directions) have values
+                when adding the ``load`` or ``eleLoad`` command,
+                even if the value is 0.
+
+        load_alpha: float, default = 1.0
+            On existing displays, the scaling factor for the load arrow sizes.
         show_constrain_dof: bool, default=False
             Whether to display labels for constrained degrees of freedom.
+        show_beam_sec: bool default = False
+            Whether to render the 3d section of beam or truss elements.
+            If True, the Arg `beam_sec` in :py:meth:`opstool.vis.GetFEMdata.get_model_data`
+            must be assigned in advance.
+        beam_sec_paras: dict defalut = None,
+            A dict to control beam section render, optional key: color, opacity, texture.
+            For texture, you can pass an image file with color=None,
+            if texture is None, it will be ignored.
         label_size: float, default=8
-            The foontsize of node and ele label.
+            The foontsize of node and ele labels, as well as local axis labels.
         show_outline: bool, default=True
             Whether to show the axis frame.
         opacity: float, default=1.0
             Plane and solid element transparency.
-        save_html: str, default='ModelVis.html'
-            The html file name to output. If False, the html file will not be generated.
+        save_fig: str, default='ModelVis.svg'
+            The file name to output. If False or None, the file will not be generated.
+            The supported formats are:
+
+            * '.svg'
+            * '.eps'
+            * '.ps'
+            * '.pdf'
+            * '.tex'
 
         Returns
         --------
         None
-
         """
-        _model_vis(self,
-                   input_file=input_file,
-                   show_node_label=show_node_label,
-                   show_ele_label=show_ele_label,
-                   show_local_crd=show_local_crd,
-                   show_fix_node=show_fix_node,
-                   show_constrain_dof=show_constrain_dof,
-                   label_size=label_size,
-                   show_outline=show_outline,
-                   opacity=opacity,
-                   save_html=save_html
-                   )
+        check_file(save_fig, [".svg", ".eps", ".ps", "pdf", ".tex"])
+        _model_vis(
+            self,
+            input_file=input_file,
+            show_node_label=show_node_label,
+            show_ele_label=show_ele_label,
+            show_local_crd=show_local_crd,
+            local_crd_alpha=local_crd_alpha,
+            show_fix_node=show_fix_node,
+            fix_node_alpha=fix_node_alpha,
+            show_load=show_load,
+            load_alpha=load_alpha,
+            show_constrain_dof=show_constrain_dof,
+            show_beam_sec=show_beam_sec,
+            beam_sec_paras=beam_sec_paras,
+            label_size=label_size,
+            show_outline=show_outline,
+            opacity=opacity,
+            save_fig=save_fig,
+        )
 
     def eigen_vis(
         self,
         mode_tags: list,
-        input_file: str = 'EigenData.hdf5',
+        input_file: str = "EigenData.hdf5",
         subplots: bool = False,
-        alpha: float = None,
+        link_views: bool = True,
+        alpha: float = 1.0,
         show_outline: bool = False,
         show_origin: bool = False,
+        label_size: float = 15,
         opacity: float = 1.0,
         show_face_line: bool = True,
-        save_html: str = "EigenVis"
+        save_fig: str = "EigenVis.svg",
     ):
         """Eigenvalue Analysis Visualization.
 
         Parameters
         ----------
         mode_tags: list[int], or tuple[int]
             Mode tags to be shown, if list or tuple [mode1, mode2], display the multiple modes from mode1 to mode2.
@@ -169,114 +223,135 @@
             :py:meth:`opstool.vis.GetFEMdata.get_eigen_data`.
 
             .. warning::
                 Be careful not to include any path, only filename,
                 the file will be loaded from the directory ``results_dir``.
 
         subplots: bool, default=False
-            If True, subplots in a figure. If False, plot in a slide style.
-        alpha: float, default=None
-            Model scaling factor, the default value is 1/5 of the model boundary according to the maximum deformation.
+            If True, subplots in a figure. If False, plot in a slider style.
+        link_views: bool, default=True
+            If True, link the views’ cameras, only usefuly when subplots is True.
+        alpha: float, default=1.0
+            Model scaling factor, scale further on existing display.
         show_outline: bool, default=True
             Whether to display the axes.
         show_origin: bool, default=False
             Whether to show undeformed shape.
         opacity: float, default=1.0
             Plane and solid element transparency.
         show_face_line: bool, default=True
             If True, the edges of plate and solid elements will be displayed.
-        save_html: str, default='EigenVis.html'
-            The html file name to output. If False, the html file will not be generated.
+        save_fig: str, default='EigenVis.svg'
+            The file name to output. If False or None, the file will not be generated.
+            The supported formats are:
+
+            * '.svg'
+            * '.eps'
+            * '.ps'
+            * '.pdf'
+            * '.tex'
 
         Returns
-        -------
+        --------
         None
         """
-        _eigen_vis(self,
-                   mode_tags=mode_tags,
-                   input_file=input_file,
-                   subplots=subplots,
-                   alpha=alpha,
-                   show_outline=show_outline,
-                   show_origin=show_origin,
-                   opacity=opacity,
-                   show_face_line=show_face_line,
-                   save_html=save_html)
+        check_file(save_fig, [".svg", ".eps", ".ps", "pdf", ".tex"])
+        _eigen_vis(
+            self,
+            mode_tags=mode_tags,
+            input_file=input_file,
+            subplots=subplots,
+            link_views=link_views,
+            alpha=alpha,
+            show_outline=show_outline,
+            show_origin=show_origin,
+            label_size=label_size,
+            opacity=opacity,
+            show_face_line=show_face_line,
+            save_fig=save_fig,
+        )
 
     def eigen_anim(
         self,
         mode_tag: int = 1,
-        input_file: str = 'EigenData.hdf5',
+        input_file: str = "EigenData.hdf5",
         n_cycle: int = 5,
-        alpha: float = None,
+        alpha: float = 1.0,
         show_outline: bool = False,
+        label_size: float = 15,
         opacity: float = 1,
         framerate: int = 3,
         show_face_line: bool = True,
-        save_html: str = "EigenAnimation"
+        save_fig: str = "EigenAnimation.gif",
     ):
         """Animation of Modal Analysis.
 
         Parameters
         ----------
         mode_tag: int
             The mode tag.
         input_file: str, default = 'EigenData.hdf5',
             The filename that eigen data saved by
             :py:meth:`opstool.vis.GetFEMdata.get_eigen_data`.
 
             .. warning::
                 Be careful not to include any path, only filename,
                 the file will be loaded from the directory ``results_dir``.
-        
+
         n_cycle: int, default = 5,
             The number of cycles in the positive and negative directions of the modal deformation.
-        alpha: float, default=None
-            Scaling factor, the default value is 1/5 of the model boundary according to the maximum deformation.
+        alpha: float, default=1.0
+            Scaling factor, scale further on existing display.
         show_outline: bool, default=False
             Whether to display the axes.
         opacity: float, default=1.0
             Plane and solid element transparency.
         framerate: int
             The number of frames per second.
         show_face_line: bool, default=True
             If True, the edges of plate and solid elements will be displayed.
-        save_html: str, default='EigenAnimation.html'
-            The html file name to output. If False, the html file will not be generated.
+        save_fig: str, default='EigenAnimation.gif'
+            The output file name, must end with `.gif` or `.mp4`.
+            You can export to any folder, such as "C:mydir/myfile.gif", but the folder `mydir` must exist.
 
         Returns
-        -------
+        --------
         None
         """
-        _eigen_anim(self,
-                    mode_tag=mode_tag,
-                    input_file=input_file,
-                    n_cycle=n_cycle,
-                    alpha=alpha,
-                    show_outline=show_outline,
-                    opacity=opacity,
-                    framerate=framerate,
-                    show_face_line=show_face_line,
-                    save_html=save_html
-                    )
-
-    def react_vis(self,
-                  input_file: str = "NodeReactionStepData-1.hdf5",
-                  slider: bool = False,
-                  direction: str = "Fz",
-                  show_values: bool = True,
-                  show_outline: bool = False,
-                  save_html: str = "ReactionVis"):
+        check_file(save_fig, [".gif", ".mp4"])
+        _eigen_anim(
+            self,
+            mode_tag=mode_tag,
+            input_file=input_file,
+            n_cycle=n_cycle,
+            alpha=alpha,
+            show_outline=show_outline,
+            label_size=label_size,
+            opacity=opacity,
+            framerate=framerate,
+            show_face_line=show_face_line,
+            save_fig=save_fig,
+        )
+
+    def react_vis(
+        self,
+        input_file: str = "NodeReactionStepData-1.hdf5",
+        slider: bool = False,
+        direction: str = "Fz",
+        show_values: bool = True,
+        show_outline: bool = False,
+        save_fig: str = "ReactionVis.svg",
+    ):
         """Plot the node reactions.
 
         Parameters
         ----------
         input_file : str, optional, default="NodeReactionStepData-1.hdf5"
             The filename that eigen data saved by
-            :py:meth:`opstool.vis.GetFEMdata.get_node_react_step` or 
+            :py:meth:`opstool.vis.GetFEMdata.get_node_react_step` or
             :py:meth:`opstool.vis.GetFEMdata.save_resp_all`.
 
             .. warning::
                 Be careful not to include any path, only filename,
                 the file will be loaded from the directory ``results_dir``.
 
         slider: bool, default=False
@@ -285,196 +360,222 @@
         direction : str, optional, by default "Fz"
             Type of reaction, if 2D, only be one of ['Fx', 'Fy', 'Mz'];
             if 3D, one of ['Fx', 'Fy', 'Fz', 'Mx', 'My', 'Mz']
         show_values : bool, optional, by default True
             If True, will show the reaction values.
         show_outline: bool, default=False
             Whether to display the axes.
-        save_html: str, default='ReactionVis.html'
-            The html file name to output. If False, the html file will not be generated.
+        save_fig: str, default='ReactionVis.svg'
+            The output file name, must end with `.gif` or `.mp4`.
+            You can export to any folder, such as "C:mydir/myfile.gif", but the folder `mydir` must exist.
         """
-        _react_vis(self, input_file=input_file,
-                   slider=slider,
-                   direction=direction,
-                   show_values=show_values,
-                   show_outline=show_outline,
-                   save_html=save_html)
-
+        _react_vis(
+            self,
+            input_file=input_file,
+            slider=slider,
+            direction=direction,
+            show_values=show_values,
+            show_outline=show_outline,
+            save_fig=save_fig,
+        )
 
     def deform_vis(
         self,
         input_file: str = "NodeRespStepData-1.hdf5",
         slider: bool = False,
         response: str = "disp",
-        alpha: float = None,
+        alpha: float = 1.0,
         show_outline: bool = False,
         show_origin: bool = False,
         show_face_line: bool = True,
         opacity: float = 1,
-        save_html: str = "DefoVis",
-        model_update: bool = False
+        save_fig: str = "DefoVis.svg",
+        model_update: bool = False,
     ):
         """Visualize the deformation of the model at a certain analysis step.
 
         Parameters
         ----------
         input_file: str, default = "NodeRespStepData-1.hdf5",
             The filename that node responses data saved by
-            :py:meth:`opstool.vis.GetFEMdata.get_node_resp_step` or 
-            :py:meth:`opstool.vis.GetFEMdata.save_resp_all`.
+            :py:meth:`opstool.vis.GetFEMdata.get_node_resp_step`.
 
             .. warning::
                 Be careful not to include any path, only filename,
                 the file will be loaded from the directory ``results_dir``.
 
         slider: bool, default=False
             If True, responses in all steps will display by slider style.
             If False, the step that max response will display.
         response: str, default='disp'
             Response type. Optional, "disp", "vel", "accel".
-        alpha: float, default=None
-            Scaling factor, the default value is 1/5 of the model boundary according to the maximum deformation.
+        alpha: float, default=1.0
+            Scaling factor, scale further on existing display.
         show_outline: bool, default=False
             Whether to display the axes.
         show_origin: bool, default=False
             Whether to show undeformed shape.
         show_face_line: bool, default=True
             If True, the edges of plate and solid elements will be displayed.
         opacity: float, default=1.0
             Plane and solid element transparency.
-        save_html: str, default='DefoVis.html'
-            The html file name to output. If False, the html file will not be generated.
+        save_fig: str, default='DefoVis.svg'
+            The file name to output. If False or None, the file will not be generated.
+            The supported formats are:
+
+            * '.svg'
+            * '.eps'
+            * '.ps'
+            * '.pdf'
+            * '.tex'
+
         model_update: bool, default False
             whether to update the model domain data at each analysis step,
             this will be useful if model data has changed.
             For example, some elements and nodes were removed.
             This parameter must same as that in :py:meth:`opstool.vis.GetFEMdata.get_node_resp_step`.
 
         Returns
-        -------
+        --------
         None
         """
-        _deform_vis(self,
-                    input_file=input_file,
-                    slider=slider,
-                    response=response,
-                    alpha=alpha,
-                    show_outline=show_outline,
-                    show_origin=show_origin,
-                    show_face_line=show_face_line,
-                    opacity=opacity,
-                    save_html=save_html,
-                    model_update=model_update
-                    )
+        check_file(save_fig, [".svg", ".eps", ".ps", "pdf", ".tex"])
+        _deform_vis(
+            self,
+            input_file=input_file,
+            slider=slider,
+            response=response,
+            alpha=alpha,
+            show_outline=show_outline,
+            show_origin=show_origin,
+            show_face_line=show_face_line,
+            opacity=opacity,
+            save_fig=save_fig,
+            model_update=model_update,
+        )
 
     def deform_anim(
         self,
         input_file: str = "NodeRespStepData-1.hdf5",
         response: str = "disp",
-        alpha: float = None,
+        alpha: float = 1.0,
         show_outline: bool = False,
         opacity: float = 1,
         framerate: int = 24,
         show_face_line: bool = True,
-        save_html: str = "DefoAnimation",
-        model_update: bool = False
+        save_fig: str = "DefoAnimation.gif",
+        model_update: bool = False,
     ):
         """Deformation animation of the model.
 
         Parameters
         ----------
         input_file: str, default = "NodeRespStepData-1.hdf5",
             The filename that node responses data saved by
-            :py:meth:`opstool.vis.GetFEMdata.get_node_resp_step` or 
-            :py:meth:`opstool.vis.GetFEMdata.save_resp_all`.
+            :py:meth:`opstool.vis.GetFEMdata.get_node_resp_step`.
 
             .. warning::
                 Be careful not to include any path, only filename,
                 the file will be loaded from the directory ``results_dir``.
 
         response: str, default='disp'
             Response type. Optional, "disp", "vel", "accel".
-        alpha: float, default=None
-            Scaling factor, the default value is 1/5 of the model boundary according to the maximum deformation.
+        alpha: float, default=1.0
+            Scaling factor, scale further on existing display.
         show_outline: bool, default=False
             Whether to display the axes.
         show_face_line: bool, default=True
             If True, the edges of plate and solid elements will be displayed.
         framerate: int, default=24
             The number of frames per second.
         opacity: float, default=1.0
             Plane and solid element transparency.
-        save_html: str, default='DefoAnimation.html'
-            The html file name to output. If False, the html file will not be generated.
+        save_fig: str, default='DefoAnimation.gif'
+            The output file name, must end with `.gif` or `.mp4`.
+            You can export to any folder, such as "C:mydir/myfile.gif", but the folder `mydir` must exist.
         model_update: bool, default False
             whether to update the model domain data at each analysis step,
             this will be useful if model data has changed.
             For example, some elements and nodes were removed.
             This parameter must same as that in :py:meth:`opstool.vis.GetFEMdata.get_node_resp_step`.
 
         Returns
-        -------
+        --------
         None
         """
+        check_file(save_fig, [".gif", ".mp4"])
+        _deform_anim(
+            self,
+            input_file=input_file,
+            response=response,
+            alpha=alpha,
+            show_outline=show_outline,
+            opacity=opacity,
+            framerate=framerate,
+            show_face_line=show_face_line,
+            save_fig=save_fig,
+            model_update=model_update,
+        )
 
-        _deform_anim(self,
-                     input_file=input_file,
-                     response=response,
-                     alpha=alpha,
-                     show_outline=show_outline,
-                     opacity=opacity,
-                     framerate=framerate,
-                     show_face_line=show_face_line,
-                     save_html=save_html,
-                     model_update=model_update
-                     )
-
-    def frame_resp_vis(self,
-                       input_file: str = "BeamRespStepData-1.hdf5",
-                       ele_tags: list = None,
-                       slider: bool = False,
-                       response: str = "Mz",
-                       show_values=True,
-                       alpha: float = None,
-                       opacity: float = 1,
-                       save_html: str = "FrameRespVis"
-                       ):
+    def frame_resp_vis(
+        self,
+        input_file: str = "BeamRespStepData-1.hdf5",
+        ele_tags: list = None,
+        slider: bool = False,
+        response: str = "Mz",
+        show_values=True,
+        alpha: float = 1.0,
+        opacity: float = 1,
+        save_fig: str = "FrameRespVis.svg",
+    ):
         """
         Display the force response of frame elements.
 
         Parameters
         ----------
         input_file: str, default = "BeamRespStepData-1.hdf5",
             The filename that beam frame elements responses data saved by
-            :py:meth:`opstool.vis.GetFEMdata.get_frame_resp_step` or 
-            :py:meth:`opstool.vis.GetFEMdata.save_resp_all`.
+            :py:meth:`opstool.vis.GetFEMdata.get_frame_resp_step`.
 
             .. warning::
                 Be careful not to include any path, only filename,
                 the file will be loaded from the directory ``results_dir``.
 
         ele_tags: int or list[int], default=None
             Element tags to display, if None, all frame elements will display.
         slider: bool, default=False
             If True, responses in all steps will display by slider style.
             If False, the step that max response will display.
         response: str, default='Mz'
             Response type. Optional, "Fx", "Fy", "Fz", "My", "Mz", "Mx".
         show_values: bool, default=True
             If True, will show the response values.
-        alpha: float, default=None
-            Scaling factor.
+        alpha: float, default=1.0
+            Scaling factor, scale further on existing display..
         opacity: float, default=1.0
             Plane and solid element transparency.
-        save_html: str, default='FrameRespVis.html'
-            The html file name to output. If False, the html file will not be generated.
+        save_fig: str, default='FrameRespVis.svg'
+            The file name to output. If False or None, the file will not be generated.
+            The supported formats are:
+
+            * '.svg'
+            * '.eps'
+            * '.ps'
+            * '.pdf'
+            * '.tex'
+
+        Returns
+        --------
+        None
         """
-        _frame_resp_vis(self,
-                        input_file=input_file,
-                        ele_tags=ele_tags,
-                        slider=slider,
-                        response=response,
-                        show_values=show_values,
-                        alpha=alpha,
-                        opacity=opacity,
-                        save_html=save_html
-                        )
+        check_file(save_fig, [".svg", ".eps", ".ps", "pdf", ".tex"])
+        _frame_resp_vis(
+            self,
+            input_file=input_file,
+            ele_tags=ele_tags,
+            slider=slider,
+            response=response,
+            show_values=show_values,
+            alpha=alpha,
+            opacity=opacity,
+            save_fig=save_fig,
+        )
```

### Comparing `opstool-0.7.3/src/opstool/vis/ops_vis_pyvista.py` & `opstool-0.8.0/src/opstool/vis/ops_vis_plotly.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,73 @@
 """
-Visualizing OpenSeesPy model based on pyvista
+Visualizing OpenSeesPy model
 """
+import plotly.io as pio
+from ._plotly_base import (
+    _deform_anim,
+    _deform_vis,
+    _eigen_anim,
+    _eigen_vis,
+    _frame_resp_vis,
+    _model_vis,
+    _react_vis,
+)
 
-import pyvista as pv
 
-from ..utils import check_file
-from ._pyvista_base import (_deform_anim, _deform_vis, _eigen_anim, _eigen_vis,
-                            _frame_resp_vis, _model_vis, _react_vis)
-
-
-class OpsVisPyvista:
-    """A class to visualize OpenSeesPy model based on
-    `pyvista <https://docs.pyvista.org/index.html>`_.
+class OpsVisPlotly:
+    """A class to visualize OpenSeesPy model based on plotly.
 
     Parameters
-    -----------
-    point_size: float, default=1
+    ----------
+    point_size: float
         The render size of node.
-    line_width: float, default=3
-        The width of line element.
+    line_width: float
+        The width of line element;
     colors_dict: dict,
         The dict for ele color, default color you can see by the class attribute ``default_colors``.
-    theme: str, default='document'
-        Plot theme for pyvista, optional 'default', 'paraview', 'document', 'dark'.
+    theme: str, default=plotly
+        Plot theme, optional "plotly", "plotly_white", "plotly_dark", "ggplot2", "seaborn", "simple_white", "none".
     color_map: str, default="jet"
-        color map to display the cloud plot for pyvista.
-        optional 'jet', 'rainbow', 'hot', 'afmhot', 'copper', 'winter', 'cool', 'coolwarm', 'gist_earth',
-        'bone', 'binary', 'gray', or any
-        `Matplotlib colormap <https://matplotlib.org/stable/tutorials/colors/colormaps.html>`_ .
+        color map to display the cloud plot. Optional, [‘aggrnyl’, ‘agsunset’, ‘algae’, ‘amp’, ‘armyrose’, ‘balance’,
+        ‘blackbody’, ‘bluered’, ‘blues’, ‘blugrn’, ‘bluyl’, ‘brbg’, ‘brwnyl’, ‘bugn’, ‘bupu’, ‘burg’, ‘burgyl’,
+        ‘cividis’, ‘curl’, ‘darkmint’, ‘deep’, ‘delta’, ‘dense’, ‘earth’, ‘edge’, ‘electric’, ‘emrld’, ‘fall’,
+        ‘geyser’, ‘gnbu’, ‘gray’, ‘greens’, ‘greys’, ‘haline’, ‘hot’, ‘hsv’, ‘ice’, ‘icefire’, ‘inferno’, ‘jet’,
+        ‘magenta’, ‘magma’, ‘matter’, ‘mint’, ‘mrybm’, ‘mygbm’, ‘oranges’, ‘orrd’, ‘oryel’, ‘oxy’, ‘peach’, ‘phase’,
+        ‘picnic’, ‘pinkyl’, ‘piyg’, ‘plasma’, ‘plotly3’, ‘portland’, ‘prgn’, ‘pubu’, ‘pubugn’, ‘puor’, ‘purd’, ‘purp’,
+        ‘purples’, ‘purpor’, ‘rainbow’, ‘rdbu’, ‘rdgy’, ‘rdpu’, ‘rdylbu’, ‘rdylgn’, ‘redor’, ‘reds’, ‘solar’,
+        ‘spectral’, ‘speed’, ‘sunset’, ‘sunsetdark’, ‘teal’, ‘tealgrn’, ‘tealrose’, ‘tempo’, ‘temps’, ‘thermal’,
+        ‘tropic’, ‘turbid’, ‘turbo’, ‘twilight’, ‘viridis’, ‘ylgn’, ‘ylgnbu’, ‘ylorbr’, ‘ylorrd’].
     on_notebook: bool, default=False
-        Whether work in a notebook.
+        Whether work in a jupyter notebook.
+
+        .. note::
+            This argument is deprecated since v0.8.0, you can call the ``show`` method to display figure.
+
     results_dir: str, default="opstool_output"
         The dir that results saved.
 
     Returns
-    --------
+    -------
     None
     """
 
     def __init__(
         self,
-        point_size: float = 1,
-        line_width: float = 3,
+        point_size: float = 2,
+        line_width: float = 4,
         colors_dict: dict = None,
-        theme: str = 'document',
+        theme: str = "plotly",
         color_map: str = "jet",
         on_notebook: bool = False,
-        results_dir: str = "opstool_output"
+        results_dir: str = "opstool_output",
     ):
         # ------------------------------
         self.point_size = point_size
         self.line_width = line_width
-        self.title = "opstool"
-        # Initialize the color dict
+        self.title = "OpenSeesVispy"
         colors = dict(
             point="#580f41",
             line="#0504aa",
             face="#00c16e",
             solid="#0cb9c1",
             truss="#7552cc",
             link="#01ff07",
@@ -67,39 +78,85 @@
         self.default_colors = colors
         self.color_point = colors["point"]
         self.color_line = colors["line"]
         self.color_face = colors["face"]
         self.color_solid = colors["solid"]
         self.color_truss = colors["truss"]
         self.color_link = colors["link"]
-        self.color_constraint = colors['constraint']
-        # -------------------------------------------------
+        self.color_constraint = colors["constraint"]
         self.theme = theme
-        pv.set_plot_theme(theme)
         self.color_map = color_map
         self.notebook = on_notebook
-        # -------------------------------------------------
         self.out_dir = results_dir
-        # -------------------------------------------------
-        self.bound_fact = 20
+        self.bound_fact = 30
+
+    def write_html(self, fig, filepath, **kwargs):
+        """Write a figure to an HTML file representation.
+
+        .. note::
+            Added since v0.8.0.
+            The purpose is to replace the argument ``save_html`` in various visualization method.
+
+        Parameters
+        -----------
+        fig: Figure object.
+        filepath: str, output file path.
+            A string representing a local file path or a writeable object
+            (e.g. a pathlib.Path object or an open file descriptor).
+        kwargs:
+            Available key parameters see
+            https://plotly.com/python-api-reference/generated/plotly.io.write_html.html?highlight=write#plotly.io.write_html.
+        """
+        pio.write_html(fig, filepath, **kwargs)
+
+    def show(self, fig, *args, **kwargs):
+        """Show a figure using either the default renderer(s) or the renderer(s) specified by the renderer argument.
+
+        .. note::
+            Added since v0.8.0.
+
+        Parameters
+        ----------
+        fig : Figure object.
+        renderer : str or None (default None)
+            A string containing the names of one or more registered renderers (separated by ‘+’ characters) or None.
+            If None, then the default renderers specified in plotly.io.renderers.default are used.
+        validate : bool (default True))
+            True if the figure should be validated before being shown, False otherwise.
+        width : int or float
+            An integer or float that determines the number of pixels wide the plot is.
+            The default is set in plotly.js.
+        height : int or float
+            An integer or float that determines the number of pixels wide the plot is.
+            The default is set in plotly.js.
+        config : dict
+            A dict of parameters to configure the figure. The defaults are set in plotly.js.
+
+        Returns
+        --------
+        None
+        """
+        fig.show(*args, **kwargs)
 
     def model_vis(
         self,
         input_file: str = "ModelData.hdf5",
         show_node_label: bool = False,
         show_ele_label: bool = False,
         show_local_crd: bool = False,
+        local_crd_alpha: float = 1.0,
         show_fix_node: bool = True,
+        fix_node_alpha: float = 1.0,
+        show_load: bool = False,
+        load_alpha: float = 1.0,
         show_constrain_dof: bool = False,
-        show_beam_sec: bool = False,
-        beam_sec_paras: dict = None,
         label_size: float = 8,
         show_outline: bool = True,
         opacity: float = 1.0,
-        save_fig: str = None
+        save_html: str = None,
     ):
         """
         Visualize the model in the current domain.
 
         Parameters
         ----------
         input_file: str, default = "ModelData.hdf5",
@@ -112,74 +169,85 @@
 
         show_node_label: bool, default=False
             Whether to display the node label.
         show_ele_label: bool, default=False
             Whether to display the ele label.
         show_local_crd: bool, default=False
             Whether to display the local axes of beam and link elements.
+        local_crd_alpha: float, default=1.0
+            On existing displays, the scaling factor for the local axis sizes.
         show_fix_node: bool, default=True
             Whether to display the fix nodes.
+        fix_node_alpha: float, default=1.0
+            On existing displays, the scaling factor for the boundary symbol sizes.
+        show_load: bool, default = False
+            Whether to display node and beam element loads.
+            The sizes of the arrow are related to the size of its load.
+            If you want to further control the size, you can use `load_alpha`.
+            Currently only supported beam element load types include
+            <beamUniform2D, beamUniform3D, beamPoint2D, beamPoint3D>.
+
+            .. note::
+                Please make sure that all dofs (or directions) have values
+                when adding the ``load`` or ``eleLoad`` command,
+                even if the value is 0.
+
+        load_alpha: float, default = 1.0
+            On existing displays, the scaling factor for the load arrow sizes.
         show_constrain_dof: bool, default=False
             Whether to display labels for constrained degrees of freedom.
-        show_beam_sec: bool default = False
-            Whether to render the 3d section of beam or truss elements.
-            If True, the Arg `beam_sec` in :py:meth:`opstool.vis.GetFEMdata.get_model_data`
-            must be assigned in advance.
-        beam_sec_paras: dict defalut = None,
-            A dict to control beam section render, optional key: color, opacity, texture.
-            For texture, you can pass an image file with color=None,
-            if texture is None, it will be ignored.
         label_size: float, default=8
             The foontsize of node and ele label.
         show_outline: bool, default=True
             Whether to show the axis frame.
         opacity: float, default=1.0
             Plane and solid element transparency.
-        save_fig: str, default='ModelVis.svg'
-            The file name to output. If False or None, the file will not be generated.
-            The supported formats are:
-
-            * '.svg'
-            * '.eps'
-            * '.ps'
-            * '.pdf'
-            * '.tex'
+        save_html: str, default=None
+            The html file name to output. If False, the html file will not be generated.
+
+            .. note::
+                This argument is deprecated since v0.8.0, you can call the ``write_html`` method to
+                write an html file.
 
         Returns
         --------
-        None
+        Plotly Figure object
+            You can call the ``write_html`` method to output an html file, and the ``show`` method will display it.
+
         """
-        check_file(save_fig, ['.svg', '.eps', '.ps', 'pdf', '.tex'])
-        _model_vis(self,
-                   input_file=input_file,
-                   show_node_label=show_node_label,
-                   show_ele_label=show_ele_label,
-                   show_local_crd=show_local_crd,
-                   show_fix_node=show_fix_node,
-                   show_constrain_dof=show_constrain_dof,
-                   show_beam_sec=show_beam_sec,
-                   beam_sec_paras=beam_sec_paras,
-                   label_size=label_size,
-                   show_outline=show_outline,
-                   opacity=opacity,
-                   save_fig=save_fig
-                   )
+        return _model_vis(
+            self,
+            input_file=input_file,
+            show_node_label=show_node_label,
+            show_ele_label=show_ele_label,
+            show_local_crd=show_local_crd,
+            local_crd_alpha=local_crd_alpha,
+            show_fix_node=show_fix_node,
+            fix_node_alpha=fix_node_alpha,
+            show_load=show_load,
+            load_alpha=load_alpha,
+            show_constrain_dof=show_constrain_dof,
+            label_size=label_size,
+            show_outline=show_outline,
+            opacity=opacity,
+            save_html=save_html,
+        )
 
     def eigen_vis(
         self,
         mode_tags: list,
-        input_file: str = 'EigenData.hdf5',
+        input_file: str = "EigenData.hdf5",
         subplots: bool = False,
-        link_views: bool = True,
-        alpha: float = None,
+        alpha: float = 1.0,
         show_outline: bool = False,
         show_origin: bool = False,
+        label_size: float = 15,
         opacity: float = 1.0,
         show_face_line: bool = True,
-        save_fig: str = "EigenVis.svg"
+        save_html: str = None,
     ):
         """Eigenvalue Analysis Visualization.
 
         Parameters
         ----------
         mode_tags: list[int], or tuple[int]
             Mode tags to be shown, if list or tuple [mode1, mode2], display the multiple modes from mode1 to mode2.
@@ -188,67 +256,63 @@
             :py:meth:`opstool.vis.GetFEMdata.get_eigen_data`.
 
             .. warning::
                 Be careful not to include any path, only filename,
                 the file will be loaded from the directory ``results_dir``.
 
         subplots: bool, default=False
-            If True, subplots in a figure. If False, plot in a slider style.
-        link_views: bool, default=True
-            If True, link the views’ cameras, only usefuly when subplots is True.
-        alpha: float, default=None
-            Model scaling factor, the default value is 1/5 of the model boundary according to the maximum deformation.
+            If True, subplots in a figure. If False, plot in a slide style.
+        alpha: float, default=1.0
+            Model scaling factor, scale further on existing display.
         show_outline: bool, default=True
             Whether to display the axes.
         show_origin: bool, default=False
             Whether to show undeformed shape.
         opacity: float, default=1.0
             Plane and solid element transparency.
         show_face_line: bool, default=True
             If True, the edges of plate and solid elements will be displayed.
-        save_fig: str, default='EigenVis.svg'
-            The file name to output. If False or None, the file will not be generated.
-            The supported formats are:
-
-            * '.svg'
-            * '.eps'
-            * '.ps'
-            * '.pdf'
-            * '.tex'
+        save_html: str, default=None
+            The html file name to output. If False, the html file will not be generated.
+
+            .. note::
+                This argument is deprecated since v0.8.0, you can call the ``write_html`` method to
+                write an html file.
 
         Returns
         --------
-        None
+        Plotly Figure object
+            You can call the ``write_html`` method to output an html file, and the ``show`` method will display it.
         """
-        check_file(save_fig, ['.svg', '.eps', '.ps', 'pdf', '.tex'])
-        _eigen_vis(
+        return _eigen_vis(
             self,
             mode_tags=mode_tags,
             input_file=input_file,
             subplots=subplots,
-            link_views=link_views,
             alpha=alpha,
             show_outline=show_outline,
             show_origin=show_origin,
+            label_size=label_size,
             opacity=opacity,
             show_face_line=show_face_line,
-            save_fig=save_fig
+            save_html=save_html,
         )
 
     def eigen_anim(
         self,
         mode_tag: int = 1,
-        input_file: str = 'EigenData.hdf5',
+        input_file: str = "EigenData.hdf5",
         n_cycle: int = 5,
-        alpha: float = None,
+        alpha: float = 1.0,
         show_outline: bool = False,
+        label_size: float = 15,
         opacity: float = 1,
         framerate: int = 3,
         show_face_line: bool = True,
-        save_fig: str = "EigenAnimation.gif"
+        save_html: str = None,
     ):
         """Animation of Modal Analysis.
 
         Parameters
         ----------
         mode_tag: int
             The mode tag.
@@ -258,59 +322,66 @@
 
             .. warning::
                 Be careful not to include any path, only filename,
                 the file will be loaded from the directory ``results_dir``.
 
         n_cycle: int, default = 5,
             The number of cycles in the positive and negative directions of the modal deformation.
-        alpha: float, default=None
-            Scaling factor, the default value is 1/5 of the model boundary according to the maximum deformation.
+        alpha: float, default=1.0
+            Model scaling factor, scale further on existing display.
         show_outline: bool, default=False
             Whether to display the axes.
         opacity: float, default=1.0
             Plane and solid element transparency.
         framerate: int
             The number of frames per second.
         show_face_line: bool, default=True
             If True, the edges of plate and solid elements will be displayed.
-        save_fig: str, default='EigenAnimation.gif'
-            The output file name, must end with `.gif` or `.mp4`.
-            You can export to any folder, such as "C:mydir/myfile.gif", but the folder `mydir` must exist.
+        save_html: str, default=None
+            The html file name to output. If False, the html file will not be generated.
+
+            .. note::
+                This argument is deprecated since v0.8.0, you can call the ``write_html`` method to
+                write an html file.
 
         Returns
         --------
-        None
+        Plotly Figure object
+            You can call the ``write_html`` method to output an html file, and the ``show`` method will display it.
         """
-        check_file(save_fig, ['.gif', '.mp4'])
-        _eigen_anim(self,
-                    mode_tag=mode_tag,
-                    input_file=input_file,
-                    n_cycle=n_cycle,
-                    alpha=alpha,
-                    show_outline=show_outline,
-                    opacity=opacity,
-                    framerate=framerate,
-                    show_face_line=show_face_line,
-                    save_fig=save_fig
-                    )
-    
-    def react_vis(self,
-                  input_file: str = "NodeReactionStepData-1.hdf5",
-                  slider: bool = False,
-                  direction: str = "Fz",
-                  show_values: bool = True,
-                  show_outline: bool = False,
-                  save_fig: str = "ReactionVis.svg"):
+        return _eigen_anim(
+            self,
+            mode_tag=mode_tag,
+            input_file=input_file,
+            n_cycle=n_cycle,
+            alpha=alpha,
+            show_outline=show_outline,
+            label_size=label_size,
+            opacity=opacity,
+            framerate=framerate,
+            show_face_line=show_face_line,
+            save_html=save_html,
+        )
+
+    def react_vis(
+        self,
+        input_file: str = "NodeReactionStepData-1.hdf5",
+        slider: bool = False,
+        direction: str = "Fz",
+        show_values: bool = True,
+        show_outline: bool = False,
+        save_html: str = None,
+    ):
         """Plot the node reactions.
 
         Parameters
         ----------
         input_file : str, optional, default="NodeReactionStepData-1.hdf5"
             The filename that eigen data saved by
-            :py:meth:`opstool.vis.GetFEMdata.get_node_react_step` or 
+            :py:meth:`opstool.vis.GetFEMdata.get_node_react_step` or
             :py:meth:`opstool.vis.GetFEMdata.save_resp_all`.
 
             .. warning::
                 Be careful not to include any path, only filename,
                 the file will be loaded from the directory ``results_dir``.
 
         slider: bool, default=False
@@ -319,217 +390,232 @@
         direction : str, optional, by default "Fz"
             Type of reaction, if 2D, only be one of ['Fx', 'Fy', 'Mz'];
             if 3D, one of ['Fx', 'Fy', 'Fz', 'Mx', 'My', 'Mz']
         show_values : bool, optional, by default True
             If True, will show the reaction values.
         show_outline: bool, default=False
             Whether to display the axes.
-        save_fig: str, default='ReactionVis.svg'
-            The output file name, must end with `.gif` or `.mp4`.
-            You can export to any folder, such as "C:mydir/myfile.gif", but the folder `mydir` must exist.
-        """
-        _react_vis(self, input_file=input_file,
-                   slider=slider,
-                   direction=direction,
-                   show_values=show_values,
-                   show_outline=show_outline,
-                   save_fig=save_fig)
+        save_html: str, default=None
+            The html file name to output. If False, the html file will not be generated.
+
+            .. note::
+                This argument is deprecated since v0.8.0, you can call the ``write_html`` method to
+                write an html file.
+
+        Returns
+        --------
+        Plotly Figure object
+            You can call the ``write_html`` method to output an html file, and the ``show`` method will display it.
+        """
+        return _react_vis(
+            self,
+            input_file=input_file,
+            slider=slider,
+            direction=direction,
+            show_values=show_values,
+            show_outline=show_outline,
+            save_html=save_html,
+        )
 
     def deform_vis(
         self,
         input_file: str = "NodeRespStepData-1.hdf5",
         slider: bool = False,
         response: str = "disp",
-        alpha: float = None,
+        alpha: float = 1.0,
         show_outline: bool = False,
         show_origin: bool = False,
         show_face_line: bool = True,
         opacity: float = 1,
-        save_fig: str = "DefoVis.svg",
-        model_update: bool = False
+        save_html: str = None,
+        model_update: bool = False,
     ):
         """Visualize the deformation of the model at a certain analysis step.
 
         Parameters
         ----------
         input_file: str, default = "NodeRespStepData-1.hdf5",
             The filename that node responses data saved by
-            :py:meth:`opstool.vis.GetFEMdata.get_node_resp_step`.
+            :py:meth:`opstool.vis.GetFEMdata.get_node_resp_step` or
+            :py:meth:`opstool.vis.GetFEMdata.save_resp_all`.
 
             .. warning::
                 Be careful not to include any path, only filename,
                 the file will be loaded from the directory ``results_dir``.
 
         slider: bool, default=False
             If True, responses in all steps will display by slider style.
             If False, the step that max response will display.
         response: str, default='disp'
             Response type. Optional, "disp", "vel", "accel".
-        alpha: float, default=None
-            Scaling factor, the default value is 1/5 of the model boundary according to the maximum deformation.
+        alpha: float, default=1.0
+            Model scaling factor, scale further on existing display.
         show_outline: bool, default=False
             Whether to display the axes.
         show_origin: bool, default=False
             Whether to show undeformed shape.
         show_face_line: bool, default=True
             If True, the edges of plate and solid elements will be displayed.
         opacity: float, default=1.0
             Plane and solid element transparency.
-        save_fig: str, default='DefoVis.svg'
-            The file name to output. If False or None, the file will not be generated.
-            The supported formats are:
-
-            * '.svg'
-            * '.eps'
-            * '.ps'
-            * '.pdf'
-            * '.tex'
+        save_html: str, default=None
+            The html file name to output. If False, the html file will not be generated.
+
+            .. note::
+                This argument is deprecated since v0.8.0, you can call the ``write_html`` method to
+                write an html file.
 
         model_update: bool, default False
             whether to update the model domain data at each analysis step,
             this will be useful if model data has changed.
             For example, some elements and nodes were removed.
             This parameter must same as that in :py:meth:`opstool.vis.GetFEMdata.get_node_resp_step`.
 
         Returns
         --------
-        None
+        Plotly Figure object
+            You can call the ``write_html`` method to output an html file, and the ``show`` method will display it.
         """
-        check_file(save_fig, ['.svg', '.eps', '.ps', 'pdf', '.tex'])
-        _deform_vis(
+        return _deform_vis(
             self,
             input_file=input_file,
             slider=slider,
             response=response,
             alpha=alpha,
             show_outline=show_outline,
             show_origin=show_origin,
             show_face_line=show_face_line,
             opacity=opacity,
-            save_fig=save_fig,
-            model_update=model_update
+            save_html=save_html,
+            model_update=model_update,
         )
 
     def deform_anim(
         self,
         input_file: str = "NodeRespStepData-1.hdf5",
         response: str = "disp",
-        alpha: float = None,
+        alpha: float = 1.0,
         show_outline: bool = False,
         opacity: float = 1,
         framerate: int = 24,
         show_face_line: bool = True,
-        save_fig: str = "DefoAnimation.gif",
-        model_update: bool = False
+        save_html: str = None,
+        model_update: bool = False,
     ):
         """Deformation animation of the model.
 
         Parameters
         ----------
         input_file: str, default = "NodeRespStepData-1.hdf5",
             The filename that node responses data saved by
-            :py:meth:`opstool.vis.GetFEMdata.get_node_resp_step`.
+            :py:meth:`opstool.vis.GetFEMdata.get_node_resp_step` or
+            :py:meth:`opstool.vis.GetFEMdata.save_resp_all`.
 
             .. warning::
                 Be careful not to include any path, only filename,
                 the file will be loaded from the directory ``results_dir``.
 
         response: str, default='disp'
             Response type. Optional, "disp", "vel", "accel".
-        alpha: float, default=None
-            Scaling factor, the default value is 1/5 of the model boundary according to the maximum deformation.
+        alpha: float, default=1.0
+            Model scaling factor, scale further on existing display.
         show_outline: bool, default=False
             Whether to display the axes.
         show_face_line: bool, default=True
             If True, the edges of plate and solid elements will be displayed.
         framerate: int, default=24
             The number of frames per second.
         opacity: float, default=1.0
             Plane and solid element transparency.
-        save_fig: str, default='DefoAnimation.gif'
-            The output file name, must end with `.gif` or `.mp4`.
-            You can export to any folder, such as "C:mydir/myfile.gif", but the folder `mydir` must exist.
+        save_html: str, default=None
+            The html file name to output. If False, the html file will not be generated.
+
+            .. note::
+                This argument is deprecated since v0.8.0, you can call the ``write_html`` method to
+                write an html file.
+
         model_update: bool, default False
             whether to update the model domain data at each analysis step,
             this will be useful if model data has changed.
             For example, some elements and nodes were removed.
             This parameter must same as that in :py:meth:`opstool.vis.GetFEMdata.get_node_resp_step`.
 
         Returns
         --------
-        None
+        Plotly Figure object
+            You can call the ``write_html`` method to output an html file, and the ``show`` method will display it.
         """
-        check_file(save_fig, ['.gif', '.mp4'])
-        _deform_anim(
+
+        return _deform_anim(
             self,
             input_file=input_file,
             response=response,
             alpha=alpha,
             show_outline=show_outline,
             opacity=opacity,
             framerate=framerate,
             show_face_line=show_face_line,
-            save_fig=save_fig,
-            model_update=model_update
+            save_html=save_html,
+            model_update=model_update,
         )
 
-    def frame_resp_vis(self,
-                       input_file: str = "BeamRespStepData-1.hdf5",
-                       ele_tags: list = None,
-                       slider: bool = False,
-                       response: str = "Mz",
-                       show_values=True,
-                       alpha: float = None,
-                       opacity: float = 1,
-                       save_fig: str = "FrameRespVis.svg"
-                       ):
+    def frame_resp_vis(
+        self,
+        input_file: str = "BeamRespStepData-1.hdf5",
+        ele_tags: list = None,
+        slider: bool = False,
+        response: str = "Mz",
+        show_values=True,
+        alpha: float = 1.0,
+        opacity: float = 1,
+        save_html: str = None,
+    ):
         """
         Display the force response of frame elements.
 
         Parameters
         ----------
         input_file: str, default = "BeamRespStepData-1.hdf5",
             The filename that beam frame elements responses data saved by
-            :py:meth:`opstool.vis.GetFEMdata.get_frame_resp_step`.
+            :py:meth:`opstool.vis.GetFEMdata.get_frame_resp_step` or
+            :py:meth:`opstool.vis.GetFEMdata.save_resp_all`.
 
             .. warning::
                 Be careful not to include any path, only filename,
                 the file will be loaded from the directory ``results_dir``.
 
         ele_tags: int or list[int], default=None
             Element tags to display, if None, all frame elements will display.
         slider: bool, default=False
             If True, responses in all steps will display by slider style.
             If False, the step that max response will display.
         response: str, default='Mz'
             Response type. Optional, "Fx", "Fy", "Fz", "My", "Mz", "Mx".
         show_values: bool, default=True
             If True, will show the response values.
-        alpha: float, default=None
-            Scaling factor.
+        alpha: float, default=1.0
+            Model scaling factor, scale further on existing display.
         opacity: float, default=1.0
             Plane and solid element transparency.
-        save_fig: str, default='FrameRespVis.svg'
-            The file name to output. If False or None, the file will not be generated.
-            The supported formats are:
-
-            * '.svg'
-            * '.eps'
-            * '.ps'
-            * '.pdf'
-            * '.tex'
+        save_html: str, default=None
+            The html file name to output. If False, the html file will not be generated.
+
+            .. note::
+                This argument is deprecated since v0.8.0, you can call the ``write_html`` method to
+                write an html file.
 
         Returns
         --------
-        None
+        Plotly Figure object
+            You can call the ``write_html`` method to output an html file, and the ``show`` method will display it.
         """
-        check_file(save_fig, ['.svg', '.eps', '.ps', 'pdf', '.tex'])
-        _frame_resp_vis(self,
-                        input_file=input_file,
-                        ele_tags=ele_tags,
-                        slider=slider,
-                        response=response,
-                        show_values=show_values,
-                        alpha=alpha,
-                        opacity=opacity,
-                        save_fig=save_fig
-                        )
+        return _frame_resp_vis(
+            self,
+            input_file=input_file,
+            ele_tags=ele_tags,
+            slider=slider,
+            response=response,
+            show_values=show_values,
+            alpha=alpha,
+            opacity=opacity,
+            save_html=save_html,
+        )
```

### Comparing `opstool-0.7.3/src/opstool/vis/save_tikz.py` & `opstool-0.8.0/src/opstool/vis/save_tikz.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,147 +13,152 @@
 
 
 def _write_head(file, width=12, height=30, d3: bool = True):
     with open(file, "w", encoding="utf8") as f:
         f.write("% This file was created by opstool, all rights reserved!\n")
         f.write("\\documentclass{standalone}\n")
         f.write("\\usepackage[dvipsnames, svgnames, x11names]{xcolor}\n")
-        f.write(
-            "\\usepackage[left=0cm,top=0cm,right=0cm,nohead,nofoot]{geometry}\n")
+        f.write("\\usepackage[left=0cm,top=0cm,right=0cm,nohead,nofoot]{geometry}\n")
         f.write("\\usepackage{tikz}\n")
         if d3:
             f.write("\\usepackage{tikz-3dplot}\n")
         f.write("\\usepackage[siunitx]{circuitikz} %[symbols]\n")
         f.write("\\usepackage[outline]{contour} % glow around text\n")
         f.write("\\usetikzlibrary{arrows,arrows.meta}\n")
         f.write("\\usetikzlibrary{decorations.markings}\n")
         f.write("\\usepackage[active,tightpage]{preview}\n")
         f.write("\\PreviewEnvironment{tikzpicture}\n")
         if d3:
             # 120 degree azimuth and 30 degree of elevation
             f.write("\\tdplotsetmaincoords{120}{30}\n")
         f.write("\\setlength\\PreviewBorder{2mm}\n\n")
         f.write(
-            f"\\geometry{{paperwidth={width}cm, paperheight={height}cm, margin=0cm}}\n")
+            f"\\geometry{{paperwidth={width}cm, paperheight={height}cm, margin=0cm}}\n"
+        )
         f.write(
-            f"\n\\tikzstyle{{link}}=[R,color={COLORS['link']},thick,{COLORS['link']}]\n")
+            f"\n\\tikzstyle{{link}}=[R,color={COLORS['link']},thick,{COLORS['link']}]\n"
+        )
         f.write(
-            f"\\tikzstyle{{constraint}}=[short,color={COLORS['constraint']},thick,{COLORS['constraint']}]\n")
+            f"\\tikzstyle{{constraint}}=[short,color={COLORS['constraint']},thick,{COLORS['constraint']}]\n"
+        )
         f.write("\n\\begin{document}\n")
         if d3:
-            f.write(
-                "\n\\begin{tikzpicture}[tdplot_main_coords]\n\n")
+            f.write("\n\\begin{tikzpicture}[tdplot_main_coords]\n\n")
         else:
             f.write("\n\\begin{tikzpicture}\n\n")
 
 
 def _write_end(file):
     with open(file, "a", encoding="utf8") as f:
         f.write(r"\n\end{tikzpicture}\n")
         f.write(r"\n\end{document}\n")
 
 
 def _def_points(file, points, d3):
     with open(file, "a", encoding="utf8") as f:
         if d3:
             for i, p in enumerate(points):
-                f.write(
-                    f"\\coordinate (P{i}) at ({p[0]}, {p[1]}, {p[2]});\n")
+                f.write(f"\\coordinate (P{i}) at ({p[0]}, {p[1]}, {p[2]});\n")
         else:
             for i, p in enumerate(points):
-                f.write(
-                    f"\\coordinate (P{i}) at ({p[0]}, {p[1]});\n")
+                f.write(f"\\coordinate (P{i}) at ({p[0]}, {p[1]});\n")
 
 
 def _write_points(file, points, size, opacity=1.0, color="black"):
     with open(file, "a", encoding="utf8") as f:
         for i, p in enumerate(points):
             f.write(
-                f"\\shade[ball color={color}, fill opacity={opacity}] (P{i}) circle ({size}pt);\n")
+                f"\\shade[ball color={color}, fill opacity={opacity}] (P{i}) circle ({size}pt);\n"
+            )
 
 
-def _write_lines(file, cells, line_width, opacity,
-                 line_color="black"):
+def _write_lines(file, cells, line_width, opacity, line_color="black"):
     cells = np.reshape(cells, (-1, 3))
     if len(cells) > 0:
         with open(file, "a", encoding="utf8") as f:
             for cell in cells:
                 idx1 = cell[1]
                 idx2 = cell[2]
                 f.write(
                     f"\\draw[{line_color},line width={line_width}pt, opacity={opacity}] "
-                    f"(P{idx1}) -- (P{idx2});\n")
+                    f"(P{idx1}) -- (P{idx2});\n"
+                )
                 # if line_type.lower() == "link":
                 #     f.write(
                 #         f"\draw[line width={line_width}pt] "
                 #         f"(P{idx1}) to[link] (P{idx2});\n")
                 # else:
                 #     f.write(
                 #         f"\draw[{line_color},line width={line_width}pt] "
                 #         f"(P{idx1}) -- (P{idx2});\n")
 
 
-def _write_constraint(file, model_info, scale, line_width, d3,
-                      line_color="black"):
+def _write_constraint(file, model_info, scale, line_width, d3, line_color="black"):
     points = model_info["ConstrainedCoords"] * scale
     cells = model_info["ConstrainedCells"]
     cells = np.reshape(cells, (-1, 3))
     midcoords = model_info["ConstrainedMidCoords"] * scale
     dofs = model_info["ConstrainedDofs"]
     dofs = ["".join([str(k) for k in dof]) for dof in dofs]
     if len(cells) > 0:
         if d3:
             with open(file, "a", encoding="utf8") as f:
                 for cell, mp, dof in zip(cells, midcoords, dofs):
                     p1 = points[cell[1]]
                     p2 = points[cell[2]]
                     f.write(
                         f"\\draw[{line_color},line width={line_width}pt] "
-                        f"({p1[0]}, {p1[1]}, {p1[2]}) to[constraint] ({p2[0]}, {p2[1]}, {p2[2]});\n")
+                        f"({p1[0]}, {p1[1]}, {p1[2]}) to[constraint] ({p2[0]}, {p2[1]}, {p2[2]});\n"
+                    )
                     # f.write(
                     #     f"\path ({mp[0]}, {mp[1]}, {mp[2]}) "
                     #     f"node[above,{line_color},font=\\fontsize{{{label_size}pt}}{{{label_size}pt}}] {{{dof}}};\n")
         else:
             with open(file, "a", encoding="utf8") as f:
                 for cell, mp, dof in zip(cells, midcoords, dofs):
                     p1 = points[cell[1]]
                     p2 = points[cell[2]]
                     f.write(
                         f"\\draw[{line_color},line width={line_width}pt] "
-                        f"({p1[0]}, {p1[1]}) to[constraint] ({p2[0]}, {p2[1]});\n")
+                        f"({p1[0]}, {p1[1]}) to[constraint] ({p2[0]}, {p2[1]});\n"
+                    )
                     # f.write(
                     #     f"\path ({mp[0]}, {mp[1]}) "
                     #     f"node[above,{line_color},font=\\fontsize{{{label_size}pt}}{{{label_size}pt}}] {{{dof}}};\n")
 
 
 def _write_faces(file, cells, color, opacity):
     if len(cells) > 0:
         with open(file, "a", encoding="utf8") as f:
             i = 0
             while i < len(cells):
                 num = cells[i]
-                idxs = cells[i + 1:i + num + 1]
-                i += num+1
+                idxs = cells[i + 1 : i + num + 1]
+                i += num + 1
                 txt = ""
                 for idx in idxs:
                     txt += f"(P{idx}) -- "
                 txt += "cycle;\n"
                 f.write(
-                    f"\\draw [line width=1pt, draw=black, fill={color}, fill opacity={opacity}]\n" + txt)
-
-
-def save_tikz(input_file: str,
-              output_file: str = "ModelData.tex",
-              point_size: float = 5,
-              line_width: float = 3,
-              face_opacity: float = 0.6,
-              solid_opacity: float = 0.6,
-              point_opacity: float = 0.8,
-              line_opacity: float = 1.0,
-              color_dict: dict = None,):
+                    f"\\draw [line width=1pt, draw=black, "
+                    f"fill={color}, fill opacity={opacity}]\n" + txt
+                )
+
+
+def save_tikz(
+    input_file: str,
+    output_file: str = "ModelData.tex",
+    point_size: float = 5,
+    line_width: float = 3,
+    face_opacity: float = 0.6,
+    solid_opacity: float = 0.6,
+    point_opacity: float = 0.8,
+    line_opacity: float = 1.0,
+    color_dict: dict = None,
+):
     """Save the ``OpenSeesPy`` model data as a ``tikz`` command file in ``latex``,
     and then you can open it in your local tex editor, or run it online in ``overleaf``.
 
     Parameters
     ----------
     input_file : str
         The input model data file, e.g., "opstool_output/ModelData.hdf5".
@@ -201,25 +206,43 @@
     points *= scale
     # write head
     _write_head(output_file, width=paperwidth, height=paperheight, d3=D3)
     # plot
     _def_points(output_file, points, d3=D3)
     cell_types = ["truss", "link", "beam", "other_line"]
     keys = ["truss", "link", "line", "line"]
-    widths = [line_width, line_width/2, line_width, line_width]
+    widths = [line_width, line_width / 2, line_width, line_width]
     for ctype, key, width in zip(cell_types, keys, widths):
-        _write_lines(output_file, cells[ctype],
-                     line_width=width, opacity=line_opacity,
-                     line_color=COLORS[key])
-    _write_constraint(output_file, model_info, scale, line_width=line_width / 2,
-                      d3=D3, line_color=COLORS['constraint'])
-    _write_faces(output_file, cells["plane"],
-                 color=COLORS['face'], opacity=face_opacity)
-    _write_faces(output_file, cells["tetrahedron"],
-                 color=COLORS['solid'], opacity=solid_opacity)
-    _write_faces(output_file, cells["brick"],
-                 color=COLORS['solid'], opacity=solid_opacity)
-    _write_points(output_file, points, size=point_size,
-                  opacity=point_opacity, color=COLORS['point'])
+        _write_lines(
+            output_file,
+            cells[ctype],
+            line_width=width,
+            opacity=line_opacity,
+            line_color=COLORS[key],
+        )
+    _write_constraint(
+        output_file,
+        model_info,
+        scale,
+        line_width=line_width / 2,
+        d3=D3,
+        line_color=COLORS["constraint"],
+    )
+    _write_faces(
+        output_file, cells["plane"], color=COLORS["face"], opacity=face_opacity
+    )
+    _write_faces(
+        output_file, cells["tetrahedron"], color=COLORS["solid"], opacity=solid_opacity
+    )
+    _write_faces(
+        output_file, cells["brick"], color=COLORS["solid"], opacity=solid_opacity
+    )
+    _write_points(
+        output_file,
+        points,
+        size=point_size,
+        opacity=point_opacity,
+        color=COLORS["point"],
+    )
 
     # write end
     _write_end(output_file)
```

### Comparing `opstool-0.7.3/src/opstool.egg-info/PKG-INFO` & `opstool-0.8.0/src/opstool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: opstool
-Version: 0.7.3
+Version: 0.8.0
 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992
 Author: Yexiang Yan
 Author-email: yexiang_yan@outlook.com
 License: GPL Licence
-Keywords: OpenSees seismic visualization
+Keywords: OpenSees Visualization Seismic Simulation
 Platform: any
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8.*
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 <p align="center">
   <font size=7><a href="https://github.com/yexiang1992/opstool">opstool</a></font>
   <p align="center"><font size=5 color=YellowGreen>modelling, visualization, post-processing for OpenSeesPy.</font></p>
 </p>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: opstool Version: 0.7.3 Summary: openseespy toolbox
+Metadata-Version: 2.1 Name: opstool Version: 0.8.0 Summary: openseespy toolbox
 Home-page: https://github.com/yexiang1992 Author: Yexiang Yan Author-email:
-yexiang_yan@outlook.com License: GPL Licence Keywords: OpenSees seismic
-visualization Platform: any Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8.* Description-Content-Type: text/markdown License-File:
+yexiang_yan@outlook.com License: GPL Licence Keywords: OpenSees Visualization
+Seismic Simulation Platform: any Classifier: Programming Language :: Python ::
+3 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENCE.txt
                                     opstool
            modelling, visualization, post-processing for OpenSeesPy.
 [![pypi](https://img.shields.io/pypi/v/opstool)](https://pypi.org/project/
 opstool/) [![Downloads](https://static.pepy.tech/badge/opstool)](https://
 pepy.tech/project/opstool) [![Documentation Status](https://readthedocs.org/
 projects/opstool/badge/?version=latest)](https://opstool.readthedocs.io/en/
```

### Comparing `opstool-0.7.3/src/opstool.egg-info/SOURCES.txt` & `opstool-0.8.0/src/opstool.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -14,19 +14,22 @@
 src/opstool/analysis/_smart_analyze.py
 src/opstool/examples/ArchBridge.py
 src/opstool/examples/ArchBridge2.py
 src/opstool/examples/CableStayedBridge.py
 src/opstool/examples/Dam.py
 src/opstool/examples/DamBreak.py
 src/opstool/examples/Frame3D.py
+src/opstool/examples/Frame3D2.py
+src/opstool/examples/GridFrame.py
 src/opstool/examples/Igloo.py
 src/opstool/examples/Pier.py
 src/opstool/examples/SDOF.py
 src/opstool/examples/SuspensionBridge.py
 src/opstool/examples/__init__.py
+src/opstool/examples/shell3D.py
 src/opstool/preprocessing/__init__.py
 src/opstool/preprocessing/geom_transf.py
 src/opstool/preprocessing/load.py
 src/opstool/preprocessing/tcl2py.py
 src/opstool/preprocessing/unit_system.py
 src/opstool/preprocessing/section/__init__.py
 src/opstool/preprocessing/section/lib_sec_mesh.py
@@ -34,11 +37,18 @@
 src/opstool/preprocessing/section/var_sec_mesh.py
 src/opstool/vis/__init__.py
 src/opstool/vis/_get_model_base.py
 src/opstool/vis/_plotly_base.py
 src/opstool/vis/_pyvista_base.py
 src/opstool/vis/fiber_sec_vis.py
 src/opstool/vis/get_model_data.py
+src/opstool/vis/ops_vis_2d.py
 src/opstool/vis/ops_vis_plotly.py
 src/opstool/vis/ops_vis_pyvista.py
 src/opstool/vis/quick_plot.py
-src/opstool/vis/save_tikz.py
+src/opstool/vis/save_tikz.py
+tests/test_dambreak.py
+tests/test_fiber_sec_vis.py
+tests/test_model_vis.py
+tests/test_sec_analysis.py
+tests/test_sec_mesh.py
+tests/test_temp.py
```

