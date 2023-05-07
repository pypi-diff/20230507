# Comparing `tmp/napari-laptrack-0.1.0.tar.gz` & `tmp/napari-laptrack-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-laptrack-0.1.0.tar", last modified: Mon Apr 10 14:50:34 2023, max compression
+gzip compressed data, was "napari-laptrack-0.2.0.tar", last modified: Sun May  7 13:02:57 2023, max compression
```

## Comparing `napari-laptrack-0.1.0.tar` & `napari-laptrack-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 14:50:34.346173 napari-laptrack-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-04-10 14:50:34.261953 napari-laptrack-0.1.0/.github/
-drwxrwxrwx   0        0        0        0 2023-04-10 14:50:34.274987 napari-laptrack-0.1.0/.github/workflows/
--rw-rw-rw-   0        0        0     3163 2023-04-10 14:30:22.000000 napari-laptrack-0.1.0/.github/workflows/test_and_deploy.yml
--rw-rw-rw-   0        0        0     1038 2023-04-10 14:28:37.000000 napari-laptrack-0.1.0/.gitignore
--rw-rw-rw-   0        0        0     1514 2023-04-10 12:50:50.000000 napari-laptrack-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      127 2023-04-10 12:50:50.000000 napari-laptrack-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8447 2023-04-10 14:50:34.345171 napari-laptrack-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7466 2023-04-10 14:42:07.000000 napari-laptrack-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 14:50:34.301056 napari-laptrack-0.1.0/docs/
--rw-rw-rw-   0        0        0  8205386 2023-04-10 12:53:02.000000 napari-laptrack-0.1.0/docs/calibzapwfixed.tif
--rw-rw-rw-   0        0        0   212004 2023-04-10 14:18:01.000000 napari-laptrack-0.1.0/docs/convert2d_t.png
--rw-rw-rw-   0        0        0   230368 2023-04-10 14:21:25.000000 napari-laptrack-0.1.0/docs/labeling_vol.png
--rw-rw-rw-   0        0        0   319760 2023-04-10 14:27:02.000000 napari-laptrack-0.1.0/docs/result.png
--rw-rw-rw-   0        0        0    69446 2023-04-10 14:02:33.000000 napari-laptrack-0.1.0/docs/track_id_image_0.png
--rw-rw-rw-   0        0        0    69505 2023-04-10 14:03:21.000000 napari-laptrack-0.1.0/docs/track_id_image_1.png
--rw-rw-rw-   0        0        0   149731 2023-04-10 14:04:08.000000 napari-laptrack-0.1.0/docs/tracks_layer.png
-drwxrwxrwx   0        0        0        0 2023-04-10 14:50:34.304063 napari-laptrack-0.1.0/napari_laptrack/
--rw-rw-rw-   0        0        0      146 2023-04-10 13:48:17.000000 napari-laptrack-0.1.0/napari_laptrack/__init__.py
--rw-rw-rw-   0        0        0     3688 2023-04-10 13:57:38.000000 napari-laptrack-0.1.0/napari_laptrack/_function.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:50:34.344169 napari-laptrack-0.1.0/napari_laptrack/_tests/
--rw-rw-rw-   0        0        0        0 2023-04-10 12:50:50.000000 napari-laptrack-0.1.0/napari_laptrack/_tests/__init__.py
--rw-rw-rw-   0        0        0       87 2023-04-10 12:50:50.000000 napari-laptrack-0.1.0/napari_laptrack/_tests/test_function.py
-drwxrwxrwx   0        0        0        0 2023-04-10 14:50:34.341161 napari-laptrack-0.1.0/napari_laptrack.egg-info/
--rw-rw-rw-   0        0        0     8447 2023-04-10 14:50:33.000000 napari-laptrack-0.1.0/napari_laptrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      637 2023-04-10 14:50:34.000000 napari-laptrack-0.1.0/napari_laptrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 14:50:33.000000 napari-laptrack-0.1.0/napari_laptrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-10 14:50:33.000000 napari-laptrack-0.1.0/napari_laptrack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      129 2023-04-10 14:50:33.000000 napari-laptrack-0.1.0/napari_laptrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-10 14:50:33.000000 napari-laptrack-0.1.0/napari_laptrack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-04-10 14:49:52.000000 napari-laptrack-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 14:50:34.346173 napari-laptrack-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1733 2023-04-10 13:51:23.000000 napari-laptrack-0.1.0/setup.py
--rw-rw-rw-   0        0        0      832 2023-04-10 14:30:22.000000 napari-laptrack-0.1.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-05-07 13:02:57.611023 napari-laptrack-0.2.0/
+-rw-rw-rw-   0        0        0      427 2023-05-07 12:57:17.000000 napari-laptrack-0.2.0/.flake8
+drwxrwxrwx   0        0        0        0 2023-05-07 13:02:57.437569 napari-laptrack-0.2.0/.github/
+drwxrwxrwx   0        0        0        0 2023-05-07 13:02:57.455616 napari-laptrack-0.2.0/.github/workflows/
+-rw-rw-rw-   0        0        0     1663 2023-05-07 12:57:17.000000 napari-laptrack-0.2.0/.github/workflows/test_and_deploy.yml
+-rw-rw-rw-   0        0        0     1046 2023-05-07 12:57:17.000000 napari-laptrack-0.2.0/.gitignore
+-rw-rw-rw-   0        0        0     1141 2023-05-07 12:57:17.000000 napari-laptrack-0.2.0/.pre-commit-config.yaml
+-rw-rw-rw-   0        0        0     1514 2023-04-10 12:50:50.000000 napari-laptrack-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      127 2023-04-10 12:50:50.000000 napari-laptrack-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8525 2023-05-07 13:02:57.610020 napari-laptrack-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7537 2023-05-07 12:57:17.000000 napari-laptrack-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 13:02:57.547858 napari-laptrack-0.2.0/docs/
+-rw-rw-rw-   0        0        0  8205386 2023-04-10 12:53:02.000000 napari-laptrack-0.2.0/docs/calibzapwfixed.tif
+-rw-rw-rw-   0        0        0   212004 2023-04-10 14:18:01.000000 napari-laptrack-0.2.0/docs/convert2d_t.png
+-rw-rw-rw-   0        0        0   230368 2023-04-10 14:21:25.000000 napari-laptrack-0.2.0/docs/labeling_vol.png
+-rw-rw-rw-   0        0        0   319760 2023-04-10 14:27:02.000000 napari-laptrack-0.2.0/docs/result.png
+-rw-rw-rw-   0        0        0    69446 2023-04-10 14:02:33.000000 napari-laptrack-0.2.0/docs/track_id_image_0.png
+-rw-rw-rw-   0        0        0    69505 2023-04-10 14:03:21.000000 napari-laptrack-0.2.0/docs/track_id_image_1.png
+-rw-rw-rw-   0        0        0   149731 2023-04-10 14:04:08.000000 napari-laptrack-0.2.0/docs/tracks_layer.png
+drwxrwxrwx   0        0        0        0 2023-05-07 13:02:57.551869 napari-laptrack-0.2.0/napari_laptrack/
+-rw-rw-rw-   0        0        0      411 2023-05-07 13:01:32.000000 napari-laptrack-0.2.0/napari_laptrack/__init__.py
+-rw-rw-rw-   0        0        0     6460 2023-05-07 12:57:17.000000 napari-laptrack-0.2.0/napari_laptrack/_function.py
+drwxrwxrwx   0        0        0        0 2023-05-07 13:02:57.608015 napari-laptrack-0.2.0/napari_laptrack/_tests/
+-rw-rw-rw-   0        0        0        0 2023-04-10 12:50:50.000000 napari-laptrack-0.2.0/napari_laptrack/_tests/__init__.py
+-rw-rw-rw-   0        0        0      423 2023-05-07 12:57:17.000000 napari-laptrack-0.2.0/napari_laptrack/_tests/test_function.py
+drwxrwxrwx   0        0        0        0 2023-05-07 13:02:57.606010 napari-laptrack-0.2.0/napari_laptrack.egg-info/
+-rw-rw-rw-   0        0        0     8525 2023-05-07 13:02:56.000000 napari-laptrack-0.2.0/napari_laptrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      669 2023-05-07 13:02:57.000000 napari-laptrack-0.2.0/napari_laptrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 13:02:56.000000 napari-laptrack-0.2.0/napari_laptrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-07 13:02:56.000000 napari-laptrack-0.2.0/napari_laptrack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      129 2023-05-07 13:02:56.000000 napari-laptrack-0.2.0/napari_laptrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-07 13:02:56.000000 napari-laptrack-0.2.0/napari_laptrack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-04-10 14:49:52.000000 napari-laptrack-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 13:02:57.611023 napari-laptrack-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1756 2023-05-07 13:01:32.000000 napari-laptrack-0.2.0/setup.py
+-rw-rw-rw-   0        0        0      845 2023-05-07 12:57:17.000000 napari-laptrack-0.2.0/tox.ini
```

### Comparing `napari-laptrack-0.1.0/.gitignore` & `napari-laptrack-0.2.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -75,8 +75,8 @@
 # OS
 .DS_Store
 
 # written by setuptools_scm
 */_version.py
 
 .idea/
-
+.vscode/
```

### Comparing `napari-laptrack-0.1.0/LICENSE` & `napari-laptrack-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-laptrack-0.1.0/PKG-INFO` & `napari-laptrack-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-laptrack
-Version: 0.1.0
+Version: 0.2.0
 Summary: Tracking particles in Napari, based on the LapTrack library
 Home-page: https://github.com/haesleinhuepf/napari_laptrack
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -16,132 +16,139 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# napari_laptrack
+# napari-laptrack
 
-[![License](https://img.shields.io/pypi/l/napari_laptrack.svg?color=green)](https://github.com/haesleinhuepf/napari_laptrack/raw/master/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/napari_laptrack.svg?color=green)](https://pypi.org/project/napari_laptrack)
-[![Python Version](https://img.shields.io/pypi/pyversions/napari_laptrack.svg?color=green)](https://python.org)
-[![tests](https://github.com/haesleinhuepf/napari_laptrack/workflows/tests/badge.svg)](https://github.com/haesleinhuepf/napari_laptrack/actions)
-[![codecov](https://codecov.io/gh/haesleinhuepf/napari_laptrack/branch/master/graph/badge.svg)](https://codecov.io/gh/haesleinhuepf/napari_laptrack)
-[![Development Status](https://img.shields.io/pypi/status/napari_laptrack.svg)](https://en.wikipedia.org/wiki/Software_release_life_cycle#Alpha)
-[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari_laptrack)](https://napari-hub.org/plugins/napari_laptrack)
+[![License](https://img.shields.io/pypi/l/napari-laptrack.svg?color=green)](https://github.com/haesleinhuepf/napari-laptrack/raw/master/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/napari-laptrack.svg?color=green)](https://pypi.org/project/napari-laptrack)
+[![Python Version](https://img.shields.io/pypi/pyversions/napari-laptrack.svg?color=green)](https://python.org)
+[![tests](https://github.com/haesleinhuepf/napari-laptrack/workflows/tests/badge.svg)](https://github.com/haesleinhuepf/napari-laptrack/actions)
+[![codecov](https://codecov.io/gh/haesleinhuepf/napari-laptrack/branch/master/graph/badge.svg)](https://codecov.io/gh/haesleinhuepf/napari-laptrack)
+[![Development Status](https://img.shields.io/pypi/status/napari-laptrack.svg)](https://en.wikipedia.org/wiki/Software_release_life_cycle#Alpha)
+[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-laptrack)](https://napari-hub.org/plugins/napari-laptrack)
 
-Tracking particles in Napari, using the [LabTrack](https://laptrack.readthedocs.io/en/latest/usage.html) library.
+Tracking particles in Napari, using the [LapTrack](https://laptrack.readthedocs.io/en/latest/usage.html) library.
 This plugin is young and has just limited functionality. Contributions are welcome.
 
-
 ## Installation instructions
 
 It is recommended to use this napari-plugin together with [devbio-napari](https://github.com/haesleinhuepf/devbio-napari).
 Install both using mamba-forge ([download here](https://github.com/conda-forge/miniforge#mambaforge)) by running these commands line-by line from the terminal:
 
 ```
 mamba create --name napari-laptrack-env -c conda-forge python=3.9 devbio-napari
+```
+
+```
 mamba activate napari-laptrack-env
+```
+
+```
 pip install napari-laptrack
 ```
 
 ## Usage
 
-The starting point for napari-laptrack is a 4D image layer and a corresponding labels layer. 
+The starting point for napari-laptrack is a 4D image layer and a corresponding labels layer.
 The following procedure demonstrates how to start from a 2D+t image stack, convert it in the right format and segment the labels.
 Afterwards, napari-laptrack is demonstrated. Depending on your input data, you may skip some of the initial steps.
 
 ### Example data
 
-We demonstrate the procedure using the example dataset `File > Open Samples > clesperanto > CalibZAPWfixed` which should be available if you installed [devbio-napari](https://github.com/haesleinhuepf/devbio-napari). 
+We demonstrate the procedure using the example dataset `File > Open Samples > clesperanto > CalibZAPWfixed` which should be available if you installed [devbio-napari](https://github.com/haesleinhuepf/devbio-napari).
 You can also download it from [zenodo](https://zenodo.org/record/5090508#.ZDQZ9nZBxaQ).
 
 ### 4D+t input data.
 
-In case your image data comes as 3D-stack, you must convert it in the format 4D+t with shape [t,1,y,x] first. 
-You can do this using the menu `Tools > Utilities > Convert 3D stack to 2d+t timelapse`, which is part of the [napari-time-slicer](https://www.napari-hub.org/plugins/napari-time-slicer) plugin. 
-It will create a new layer named `2D+t <original name>`. After this conversion, you can delete the original image layer, which is recommended to avoid confusion due to too many layers. 
+In case your image data comes as 3D-stack, you must convert it in the format 4D+t with shape [t,1,y,x] first.
+You can do this using the menu `Tools > Utilities > Convert 3D stack to 2d+t timelapse`, which is part of the [napari-time-slicer](https://www.napari-hub.org/plugins/napari-time-slicer) plugin.
+It will create a new layer named `2D+t <original name>`. After this conversion, you can delete the original image layer, which is recommended to avoid confusion due to too many layers.
 For deleting the original layer, select it and hit the trash-bin button.
 
 ![img.png](https://github.com/haesleinhuepf/napari-laptrack/raw/main/docs/convert2d_t.png)
 
 ### Object segmentation
 
-Various segmentation algorithms are available in Napari (see the [Napari-hub](https://www.napari-hub.org/?search=segmentation&sort=relevance&page=1)). 
+Various segmentation algorithms are available in Napari (see the [Napari-hub](https://www.napari-hub.org/?search=segmentation&sort=relevance&page=1)).
 In principle all algorithms are compatible if they produce a 3D+t label image as result.
-In this tutorial, we use the [Voronoi-Otsu-Labeling algorithm](https://haesleinhuepf.github.io/BioImageAnalysisNotebooks/20_image_segmentation/11_voronoi_otsu_labeling.html) implemented using [clesperanto](https://github.com/clEsperanto/pyclesperanto_prototype). 
+In this tutorial, we use the [Voronoi-Otsu-Labeling algorithm](https://haesleinhuepf.github.io/BioImageAnalysisNotebooks/20_image_segmentation/11_voronoi_otsu_labeling.html) implemented using [clesperanto](https://github.com/clEsperanto/pyclesperanto_prototype).
 It is available from the menu `Tools > Segmentation / labeling`.
 
 ![img.png](https://github.com/haesleinhuepf/napari-laptrack/raw/main/docs/labeling_vol.png)
 
 ### Tracking labeled objects
 
-Now that we have a 3D+t image and a corresponding label-image, we can start tracking the objects. 
+Now that we have a 3D+t image and a corresponding label-image, we can start tracking the objects.
 Centroid-based tracking is available from the menu `Tracking > Track labeled objects (centroid-based, LapTrack)`.
-After tracking, multiple new layers will be added to Napari, which are explained in detail below. 
-Furthermore, a table will open containing the columns `centroid-0/1/2` with spatial positions of the labels. 
-The table also contain colums `label`, `frame` and `track_id`. 
-All labels which belong to the same track, but to different frames, have the same `track_id`. 
+After tracking, multiple new layers will be added to Napari, which are explained in detail below.
+Furthermore, a table will open containing the columns `centroid-0/1/2` with spatial positions of the labels.
+The table also contain colums `label`, `frame` and `track_id`.
+All labels which belong to the same track, but to different frames, have the same `track_id`.
 In some cases, also layers named `Stack 4D <original layer name>` are created. This is done to store the labels which were analysed. These layers are technically duplicates of the original layers which were computed on-the-fly.
 
 ![img.png](https://github.com/haesleinhuepf/napari-laptrack/raw/main/docs/result.png)
 
 ### The Tracks layer
 
 The tracks layer visualizes the travel path of the labels' centroids over time. [Read more about the Tracks layer in the Napari documentation](https://napari.org/stable/howtos/layers/tracks.html).
 
 ![img.png](https://github.com/haesleinhuepf/napari-laptrack/raw/main/docs/tracks_layer.png)
 
 ### The Track-ID image
-One result of the plugin is a Track-ID image. This is a label image where objects have the same label / color over time. 
+
+One result of the plugin is a Track-ID image. This is a label image where objects have the same label / color over time.
 This image is not suited for many quantitative label-measurment methods because it is non-sequentially labeled.
 
 As example, two subsequent frames are shown:
 
 ![img.png](https://github.com/haesleinhuepf/napari-laptrack/raw/main/docs/track_id_image_0.png)
 
 ![img.png](https://github.com/haesleinhuepf/napari-laptrack/raw/main/docs/track_id_image_1.png)
 
 ## Similar and related plugins
 
 There are other napari-plugins and python packages which allow tracking particles, visualizing tracking data and quantiative measurements of tracks:
-* [arboretum](https://github.com/lowe-lab-ucl/arboretum)
-* [btrack](https://github.com/quantumjot/btrack)
-* [ultrack](https://github.com/royerlab/ultrack)
-* [napari-stracking](https://www.napari-hub.org/plugins/napari-stracking)
-* [napari-tracks-reader](https://www.napari-hub.org/plugins/napari-tracks-reader)
-* [vollseg-napari-trackmate](https://www.napari-hub.org/plugins/vollseg-napari-trackmate)
-* [palmari](https://www.napari-hub.org/plugins/palmari)
-* [napari-amdtrk](https://www.napari-hub.org/plugins/napari-amdtrk)
 
+- [arboretum](https://github.com/lowe-lab-ucl/arboretum)
+- [btrack](https://github.com/quantumjot/btrack)
+- [ultrack](https://github.com/royerlab/ultrack)
+- [napari-stracking](https://www.napari-hub.org/plugins/napari-stracking)
+- [napari-tracks-reader](https://www.napari-hub.org/plugins/napari-tracks-reader)
+- [vollseg-napari-trackmate](https://www.napari-hub.org/plugins/vollseg-napari-trackmate)
+- [palmari](https://www.napari-hub.org/plugins/palmari)
+- [napari-amdtrk](https://www.napari-hub.org/plugins/napari-amdtrk)
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
-
 ## License
 
 Distributed under the terms of the [BSD-3] license,
-"napari_laptrack" is free and open source software
+"napari-laptrack" is free and open source software
 
 ## Issues
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
+<!-- prettier-ignore-start -->
 [napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
 [MIT]: http://opensource.org/licenses/MIT
 [BSD-3]: http://opensource.org/licenses/BSD-3-Clause
 [GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
 [GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
 [Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/haesleinhuepf/cookiecutter-napari-assistant-plugin
-[file an issue]: https://github.com/haesleinhuepf/napari_laptrack/issues
+[file an issue]: https://github.com/haesleinhuepf/napari-laptrack/issues
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
+<!-- prettier-ignore-end -->
```

### Comparing `napari-laptrack-0.1.0/README.md` & `napari-laptrack-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,125 +1,132 @@
-# napari_laptrack
+# napari-laptrack
 
-[![License](https://img.shields.io/pypi/l/napari_laptrack.svg?color=green)](https://github.com/haesleinhuepf/napari_laptrack/raw/master/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/napari_laptrack.svg?color=green)](https://pypi.org/project/napari_laptrack)
-[![Python Version](https://img.shields.io/pypi/pyversions/napari_laptrack.svg?color=green)](https://python.org)
-[![tests](https://github.com/haesleinhuepf/napari_laptrack/workflows/tests/badge.svg)](https://github.com/haesleinhuepf/napari_laptrack/actions)
-[![codecov](https://codecov.io/gh/haesleinhuepf/napari_laptrack/branch/master/graph/badge.svg)](https://codecov.io/gh/haesleinhuepf/napari_laptrack)
-[![Development Status](https://img.shields.io/pypi/status/napari_laptrack.svg)](https://en.wikipedia.org/wiki/Software_release_life_cycle#Alpha)
-[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari_laptrack)](https://napari-hub.org/plugins/napari_laptrack)
+[![License](https://img.shields.io/pypi/l/napari-laptrack.svg?color=green)](https://github.com/haesleinhuepf/napari-laptrack/raw/master/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/napari-laptrack.svg?color=green)](https://pypi.org/project/napari-laptrack)
+[![Python Version](https://img.shields.io/pypi/pyversions/napari-laptrack.svg?color=green)](https://python.org)
+[![tests](https://github.com/haesleinhuepf/napari-laptrack/workflows/tests/badge.svg)](https://github.com/haesleinhuepf/napari-laptrack/actions)
+[![codecov](https://codecov.io/gh/haesleinhuepf/napari-laptrack/branch/master/graph/badge.svg)](https://codecov.io/gh/haesleinhuepf/napari-laptrack)
+[![Development Status](https://img.shields.io/pypi/status/napari-laptrack.svg)](https://en.wikipedia.org/wiki/Software_release_life_cycle#Alpha)
+[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-laptrack)](https://napari-hub.org/plugins/napari-laptrack)
 
-Tracking particles in Napari, using the [LabTrack](https://laptrack.readthedocs.io/en/latest/usage.html) library.
+Tracking particles in Napari, using the [LapTrack](https://laptrack.readthedocs.io/en/latest/usage.html) library.
 This plugin is young and has just limited functionality. Contributions are welcome.
 
-
 ## Installation instructions
 
 It is recommended to use this napari-plugin together with [devbio-napari](https://github.com/haesleinhuepf/devbio-napari).
 Install both using mamba-forge ([download here](https://github.com/conda-forge/miniforge#mambaforge)) by running these commands line-by line from the terminal:
 
 ```
 mamba create --name napari-laptrack-env -c conda-forge python=3.9 devbio-napari
+```
+
+```
 mamba activate napari-laptrack-env
+```
+
+```
 pip install napari-laptrack
 ```
 
 ## Usage
 
-The starting point for napari-laptrack is a 4D image layer and a corresponding labels layer. 
+The starting point for napari-laptrack is a 4D image layer and a corresponding labels layer.
 The following procedure demonstrates how to start from a 2D+t image stack, convert it in the right format and segment the labels.
 Afterwards, napari-laptrack is demonstrated. Depending on your input data, you may skip some of the initial steps.
 
 ### Example data
 
-We demonstrate the procedure using the example dataset `File > Open Samples > clesperanto > CalibZAPWfixed` which should be available if you installed [devbio-napari](https://github.com/haesleinhuepf/devbio-napari). 
+We demonstrate the procedure using the example dataset `File > Open Samples > clesperanto > CalibZAPWfixed` which should be available if you installed [devbio-napari](https://github.com/haesleinhuepf/devbio-napari).
 You can also download it from [zenodo](https://zenodo.org/record/5090508#.ZDQZ9nZBxaQ).
 
 ### 4D+t input data.
 
-In case your image data comes as 3D-stack, you must convert it in the format 4D+t with shape [t,1,y,x] first. 
-You can do this using the menu `Tools > Utilities > Convert 3D stack to 2d+t timelapse`, which is part of the [napari-time-slicer](https://www.napari-hub.org/plugins/napari-time-slicer) plugin. 
-It will create a new layer named `2D+t <original name>`. After this conversion, you can delete the original image layer, which is recommended to avoid confusion due to too many layers. 
+In case your image data comes as 3D-stack, you must convert it in the format 4D+t with shape [t,1,y,x] first.
+You can do this using the menu `Tools > Utilities > Convert 3D stack to 2d+t timelapse`, which is part of the [napari-time-slicer](https://www.napari-hub.org/plugins/napari-time-slicer) plugin.
+It will create a new layer named `2D+t <original name>`. After this conversion, you can delete the original image layer, which is recommended to avoid confusion due to too many layers.
 For deleting the original layer, select it and hit the trash-bin button.
 
 ![img.png](https://github.com/haesleinhuepf/napari-laptrack/raw/main/docs/convert2d_t.png)
 
 ### Object segmentation
 
-Various segmentation algorithms are available in Napari (see the [Napari-hub](https://www.napari-hub.org/?search=segmentation&sort=relevance&page=1)). 
+Various segmentation algorithms are available in Napari (see the [Napari-hub](https://www.napari-hub.org/?search=segmentation&sort=relevance&page=1)).
 In principle all algorithms are compatible if they produce a 3D+t label image as result.
-In this tutorial, we use the [Voronoi-Otsu-Labeling algorithm](https://haesleinhuepf.github.io/BioImageAnalysisNotebooks/20_image_segmentation/11_voronoi_otsu_labeling.html) implemented using [clesperanto](https://github.com/clEsperanto/pyclesperanto_prototype). 
+In this tutorial, we use the [Voronoi-Otsu-Labeling algorithm](https://haesleinhuepf.github.io/BioImageAnalysisNotebooks/20_image_segmentation/11_voronoi_otsu_labeling.html) implemented using [clesperanto](https://github.com/clEsperanto/pyclesperanto_prototype).
 It is available from the menu `Tools > Segmentation / labeling`.
 
 ![img.png](https://github.com/haesleinhuepf/napari-laptrack/raw/main/docs/labeling_vol.png)
 
 ### Tracking labeled objects
 
-Now that we have a 3D+t image and a corresponding label-image, we can start tracking the objects. 
+Now that we have a 3D+t image and a corresponding label-image, we can start tracking the objects.
 Centroid-based tracking is available from the menu `Tracking > Track labeled objects (centroid-based, LapTrack)`.
-After tracking, multiple new layers will be added to Napari, which are explained in detail below. 
-Furthermore, a table will open containing the columns `centroid-0/1/2` with spatial positions of the labels. 
-The table also contain colums `label`, `frame` and `track_id`. 
-All labels which belong to the same track, but to different frames, have the same `track_id`. 
+After tracking, multiple new layers will be added to Napari, which are explained in detail below.
+Furthermore, a table will open containing the columns `centroid-0/1/2` with spatial positions of the labels.
+The table also contain colums `label`, `frame` and `track_id`.
+All labels which belong to the same track, but to different frames, have the same `track_id`.
 In some cases, also layers named `Stack 4D <original layer name>` are created. This is done to store the labels which were analysed. These layers are technically duplicates of the original layers which were computed on-the-fly.
 
 ![img.png](https://github.com/haesleinhuepf/napari-laptrack/raw/main/docs/result.png)
 
 ### The Tracks layer
 
 The tracks layer visualizes the travel path of the labels' centroids over time. [Read more about the Tracks layer in the Napari documentation](https://napari.org/stable/howtos/layers/tracks.html).
 
 ![img.png](https://github.com/haesleinhuepf/napari-laptrack/raw/main/docs/tracks_layer.png)
 
 ### The Track-ID image
-One result of the plugin is a Track-ID image. This is a label image where objects have the same label / color over time. 
+
+One result of the plugin is a Track-ID image. This is a label image where objects have the same label / color over time.
 This image is not suited for many quantitative label-measurment methods because it is non-sequentially labeled.
 
 As example, two subsequent frames are shown:
 
 ![img.png](https://github.com/haesleinhuepf/napari-laptrack/raw/main/docs/track_id_image_0.png)
 
 ![img.png](https://github.com/haesleinhuepf/napari-laptrack/raw/main/docs/track_id_image_1.png)
 
 ## Similar and related plugins
 
 There are other napari-plugins and python packages which allow tracking particles, visualizing tracking data and quantiative measurements of tracks:
-* [arboretum](https://github.com/lowe-lab-ucl/arboretum)
-* [btrack](https://github.com/quantumjot/btrack)
-* [ultrack](https://github.com/royerlab/ultrack)
-* [napari-stracking](https://www.napari-hub.org/plugins/napari-stracking)
-* [napari-tracks-reader](https://www.napari-hub.org/plugins/napari-tracks-reader)
-* [vollseg-napari-trackmate](https://www.napari-hub.org/plugins/vollseg-napari-trackmate)
-* [palmari](https://www.napari-hub.org/plugins/palmari)
-* [napari-amdtrk](https://www.napari-hub.org/plugins/napari-amdtrk)
 
+- [arboretum](https://github.com/lowe-lab-ucl/arboretum)
+- [btrack](https://github.com/quantumjot/btrack)
+- [ultrack](https://github.com/royerlab/ultrack)
+- [napari-stracking](https://www.napari-hub.org/plugins/napari-stracking)
+- [napari-tracks-reader](https://www.napari-hub.org/plugins/napari-tracks-reader)
+- [vollseg-napari-trackmate](https://www.napari-hub.org/plugins/vollseg-napari-trackmate)
+- [palmari](https://www.napari-hub.org/plugins/palmari)
+- [napari-amdtrk](https://www.napari-hub.org/plugins/napari-amdtrk)
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
-
 ## License
 
 Distributed under the terms of the [BSD-3] license,
-"napari_laptrack" is free and open source software
+"napari-laptrack" is free and open source software
 
 ## Issues
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
+<!-- prettier-ignore-start -->
 [napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
 [MIT]: http://opensource.org/licenses/MIT
 [BSD-3]: http://opensource.org/licenses/BSD-3-Clause
 [GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
 [GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
 [Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/haesleinhuepf/cookiecutter-napari-assistant-plugin
-[file an issue]: https://github.com/haesleinhuepf/napari_laptrack/issues
+[file an issue]: https://github.com/haesleinhuepf/napari-laptrack/issues
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
+<!-- prettier-ignore-end -->
```

### Comparing `napari-laptrack-0.1.0/docs/calibzapwfixed.tif` & `napari-laptrack-0.2.0/docs/calibzapwfixed.tif`

 * *Files identical despite different names*

### Comparing `napari-laptrack-0.1.0/docs/convert2d_t.png` & `napari-laptrack-0.2.0/docs/convert2d_t.png`

 * *Files identical despite different names*

### Comparing `napari-laptrack-0.1.0/docs/labeling_vol.png` & `napari-laptrack-0.2.0/docs/labeling_vol.png`

 * *Files identical despite different names*

### Comparing `napari-laptrack-0.1.0/docs/result.png` & `napari-laptrack-0.2.0/docs/result.png`

 * *Files identical despite different names*

### Comparing `napari-laptrack-0.1.0/docs/track_id_image_0.png` & `napari-laptrack-0.2.0/docs/track_id_image_0.png`

 * *Files identical despite different names*

### Comparing `napari-laptrack-0.1.0/docs/track_id_image_1.png` & `napari-laptrack-0.2.0/docs/track_id_image_1.png`

 * *Files identical despite different names*

### Comparing `napari-laptrack-0.1.0/docs/tracks_layer.png` & `napari-laptrack-0.2.0/docs/tracks_layer.png`

 * *Files identical despite different names*

### Comparing `napari-laptrack-0.1.0/napari_laptrack.egg-info/PKG-INFO` & `napari-laptrack-0.2.0/napari_laptrack.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-laptrack
-Version: 0.1.0
+Version: 0.2.0
 Summary: Tracking particles in Napari, based on the LapTrack library
 Home-page: https://github.com/haesleinhuepf/napari_laptrack
 Author: Robert Haase
 Author-email: robert.haase@tu-dresden.de
 License: BSD-3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
@@ -16,132 +16,139 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# napari_laptrack
+# napari-laptrack
 
-[![License](https://img.shields.io/pypi/l/napari_laptrack.svg?color=green)](https://github.com/haesleinhuepf/napari_laptrack/raw/master/LICENSE)
-[![PyPI](https://img.shields.io/pypi/v/napari_laptrack.svg?color=green)](https://pypi.org/project/napari_laptrack)
-[![Python Version](https://img.shields.io/pypi/pyversions/napari_laptrack.svg?color=green)](https://python.org)
-[![tests](https://github.com/haesleinhuepf/napari_laptrack/workflows/tests/badge.svg)](https://github.com/haesleinhuepf/napari_laptrack/actions)
-[![codecov](https://codecov.io/gh/haesleinhuepf/napari_laptrack/branch/master/graph/badge.svg)](https://codecov.io/gh/haesleinhuepf/napari_laptrack)
-[![Development Status](https://img.shields.io/pypi/status/napari_laptrack.svg)](https://en.wikipedia.org/wiki/Software_release_life_cycle#Alpha)
-[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari_laptrack)](https://napari-hub.org/plugins/napari_laptrack)
+[![License](https://img.shields.io/pypi/l/napari-laptrack.svg?color=green)](https://github.com/haesleinhuepf/napari-laptrack/raw/master/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/napari-laptrack.svg?color=green)](https://pypi.org/project/napari-laptrack)
+[![Python Version](https://img.shields.io/pypi/pyversions/napari-laptrack.svg?color=green)](https://python.org)
+[![tests](https://github.com/haesleinhuepf/napari-laptrack/workflows/tests/badge.svg)](https://github.com/haesleinhuepf/napari-laptrack/actions)
+[![codecov](https://codecov.io/gh/haesleinhuepf/napari-laptrack/branch/master/graph/badge.svg)](https://codecov.io/gh/haesleinhuepf/napari-laptrack)
+[![Development Status](https://img.shields.io/pypi/status/napari-laptrack.svg)](https://en.wikipedia.org/wiki/Software_release_life_cycle#Alpha)
+[![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-laptrack)](https://napari-hub.org/plugins/napari-laptrack)
 
-Tracking particles in Napari, using the [LabTrack](https://laptrack.readthedocs.io/en/latest/usage.html) library.
+Tracking particles in Napari, using the [LapTrack](https://laptrack.readthedocs.io/en/latest/usage.html) library.
 This plugin is young and has just limited functionality. Contributions are welcome.
 
-
 ## Installation instructions
 
 It is recommended to use this napari-plugin together with [devbio-napari](https://github.com/haesleinhuepf/devbio-napari).
 Install both using mamba-forge ([download here](https://github.com/conda-forge/miniforge#mambaforge)) by running these commands line-by line from the terminal:
 
 ```
 mamba create --name napari-laptrack-env -c conda-forge python=3.9 devbio-napari
+```
+
+```
 mamba activate napari-laptrack-env
+```
+
+```
 pip install napari-laptrack
 ```
 
 ## Usage
 
-The starting point for napari-laptrack is a 4D image layer and a corresponding labels layer. 
+The starting point for napari-laptrack is a 4D image layer and a corresponding labels layer.
 The following procedure demonstrates how to start from a 2D+t image stack, convert it in the right format and segment the labels.
 Afterwards, napari-laptrack is demonstrated. Depending on your input data, you may skip some of the initial steps.
 
 ### Example data
 
-We demonstrate the procedure using the example dataset `File > Open Samples > clesperanto > CalibZAPWfixed` which should be available if you installed [devbio-napari](https://github.com/haesleinhuepf/devbio-napari). 
+We demonstrate the procedure using the example dataset `File > Open Samples > clesperanto > CalibZAPWfixed` which should be available if you installed [devbio-napari](https://github.com/haesleinhuepf/devbio-napari).
 You can also download it from [zenodo](https://zenodo.org/record/5090508#.ZDQZ9nZBxaQ).
 
 ### 4D+t input data.
 
-In case your image data comes as 3D-stack, you must convert it in the format 4D+t with shape [t,1,y,x] first. 
-You can do this using the menu `Tools > Utilities > Convert 3D stack to 2d+t timelapse`, which is part of the [napari-time-slicer](https://www.napari-hub.org/plugins/napari-time-slicer) plugin. 
-It will create a new layer named `2D+t <original name>`. After this conversion, you can delete the original image layer, which is recommended to avoid confusion due to too many layers. 
+In case your image data comes as 3D-stack, you must convert it in the format 4D+t with shape [t,1,y,x] first.
+You can do this using the menu `Tools > Utilities > Convert 3D stack to 2d+t timelapse`, which is part of the [napari-time-slicer](https://www.napari-hub.org/plugins/napari-time-slicer) plugin.
+It will create a new layer named `2D+t <original name>`. After this conversion, you can delete the original image layer, which is recommended to avoid confusion due to too many layers.
 For deleting the original layer, select it and hit the trash-bin button.
 
 ![img.png](https://github.com/haesleinhuepf/napari-laptrack/raw/main/docs/convert2d_t.png)
 
 ### Object segmentation
 
-Various segmentation algorithms are available in Napari (see the [Napari-hub](https://www.napari-hub.org/?search=segmentation&sort=relevance&page=1)). 
+Various segmentation algorithms are available in Napari (see the [Napari-hub](https://www.napari-hub.org/?search=segmentation&sort=relevance&page=1)).
 In principle all algorithms are compatible if they produce a 3D+t label image as result.
-In this tutorial, we use the [Voronoi-Otsu-Labeling algorithm](https://haesleinhuepf.github.io/BioImageAnalysisNotebooks/20_image_segmentation/11_voronoi_otsu_labeling.html) implemented using [clesperanto](https://github.com/clEsperanto/pyclesperanto_prototype). 
+In this tutorial, we use the [Voronoi-Otsu-Labeling algorithm](https://haesleinhuepf.github.io/BioImageAnalysisNotebooks/20_image_segmentation/11_voronoi_otsu_labeling.html) implemented using [clesperanto](https://github.com/clEsperanto/pyclesperanto_prototype).
 It is available from the menu `Tools > Segmentation / labeling`.
 
 ![img.png](https://github.com/haesleinhuepf/napari-laptrack/raw/main/docs/labeling_vol.png)
 
 ### Tracking labeled objects
 
-Now that we have a 3D+t image and a corresponding label-image, we can start tracking the objects. 
+Now that we have a 3D+t image and a corresponding label-image, we can start tracking the objects.
 Centroid-based tracking is available from the menu `Tracking > Track labeled objects (centroid-based, LapTrack)`.
-After tracking, multiple new layers will be added to Napari, which are explained in detail below. 
-Furthermore, a table will open containing the columns `centroid-0/1/2` with spatial positions of the labels. 
-The table also contain colums `label`, `frame` and `track_id`. 
-All labels which belong to the same track, but to different frames, have the same `track_id`. 
+After tracking, multiple new layers will be added to Napari, which are explained in detail below.
+Furthermore, a table will open containing the columns `centroid-0/1/2` with spatial positions of the labels.
+The table also contain colums `label`, `frame` and `track_id`.
+All labels which belong to the same track, but to different frames, have the same `track_id`.
 In some cases, also layers named `Stack 4D <original layer name>` are created. This is done to store the labels which were analysed. These layers are technically duplicates of the original layers which were computed on-the-fly.
 
 ![img.png](https://github.com/haesleinhuepf/napari-laptrack/raw/main/docs/result.png)
 
 ### The Tracks layer
 
 The tracks layer visualizes the travel path of the labels' centroids over time. [Read more about the Tracks layer in the Napari documentation](https://napari.org/stable/howtos/layers/tracks.html).
 
 ![img.png](https://github.com/haesleinhuepf/napari-laptrack/raw/main/docs/tracks_layer.png)
 
 ### The Track-ID image
-One result of the plugin is a Track-ID image. This is a label image where objects have the same label / color over time. 
+
+One result of the plugin is a Track-ID image. This is a label image where objects have the same label / color over time.
 This image is not suited for many quantitative label-measurment methods because it is non-sequentially labeled.
 
 As example, two subsequent frames are shown:
 
 ![img.png](https://github.com/haesleinhuepf/napari-laptrack/raw/main/docs/track_id_image_0.png)
 
 ![img.png](https://github.com/haesleinhuepf/napari-laptrack/raw/main/docs/track_id_image_1.png)
 
 ## Similar and related plugins
 
 There are other napari-plugins and python packages which allow tracking particles, visualizing tracking data and quantiative measurements of tracks:
-* [arboretum](https://github.com/lowe-lab-ucl/arboretum)
-* [btrack](https://github.com/quantumjot/btrack)
-* [ultrack](https://github.com/royerlab/ultrack)
-* [napari-stracking](https://www.napari-hub.org/plugins/napari-stracking)
-* [napari-tracks-reader](https://www.napari-hub.org/plugins/napari-tracks-reader)
-* [vollseg-napari-trackmate](https://www.napari-hub.org/plugins/vollseg-napari-trackmate)
-* [palmari](https://www.napari-hub.org/plugins/palmari)
-* [napari-amdtrk](https://www.napari-hub.org/plugins/napari-amdtrk)
 
+- [arboretum](https://github.com/lowe-lab-ucl/arboretum)
+- [btrack](https://github.com/quantumjot/btrack)
+- [ultrack](https://github.com/royerlab/ultrack)
+- [napari-stracking](https://www.napari-hub.org/plugins/napari-stracking)
+- [napari-tracks-reader](https://www.napari-hub.org/plugins/napari-tracks-reader)
+- [vollseg-napari-trackmate](https://www.napari-hub.org/plugins/vollseg-napari-trackmate)
+- [palmari](https://www.napari-hub.org/plugins/palmari)
+- [napari-amdtrk](https://www.napari-hub.org/plugins/napari-amdtrk)
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
-
 ## License
 
 Distributed under the terms of the [BSD-3] license,
-"napari_laptrack" is free and open source software
+"napari-laptrack" is free and open source software
 
 ## Issues
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
+<!-- prettier-ignore-start -->
 [napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
 [MIT]: http://opensource.org/licenses/MIT
 [BSD-3]: http://opensource.org/licenses/BSD-3-Clause
 [GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
 [GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
 [Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
 [Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/haesleinhuepf/cookiecutter-napari-assistant-plugin
-[file an issue]: https://github.com/haesleinhuepf/napari_laptrack/issues
+[file an issue]: https://github.com/haesleinhuepf/napari-laptrack/issues
 [napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
 [PyPI]: https://pypi.org/
+<!-- prettier-ignore-end -->
```

### Comparing `napari-laptrack-0.1.0/napari_laptrack.egg-info/SOURCES.txt` & `napari-laptrack-0.2.0/napari_laptrack.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+.flake8
 .gitignore
+.pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 tox.ini
 .github/workflows/test_and_deploy.yml
```

### Comparing `napari-laptrack-0.1.0/setup.py` & `napari-laptrack-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-
-import os
 import codecs
-from setuptools import setup, find_packages
+import os
+
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
-    return codecs.open(file_path, encoding='utf-8').read()
+    return codecs.open(file_path, encoding="utf-8").read()
 
 
 # Add your dependencies in requirements.txt
 # Note: you can add test-specific requirements in tox.ini
 requirements = []
-with open('requirements.txt') as f:
+with open("requirements.txt") as f:
     for line in f:
         stripped = line.split("#")[0].strip()
         if len(stripped) > 0:
             requirements.append(stripped)
 
 setup(
-    name='napari-laptrack',
-    author='Robert Haase',
-    author_email='robert.haase@tu-dresden.de',
-    license='BSD-3',
-    url='https://github.com/haesleinhuepf/napari_laptrack',
-    description='Tracking particles in Napari, based on the LapTrack library',
-    long_description=read('README.md'),
-    long_description_content_type='text/markdown',
+    name="napari-laptrack",
+    author="Robert Haase",
+    author_email="robert.haase@tu-dresden.de",
+    license="BSD-3",
+    url="https://github.com/haesleinhuepf/napari_laptrack",
+    description="Tracking particles in Napari, based on the LapTrack library",
+    long_description=read("README.md"),
+    long_description_content_type="text/markdown",
     packages=find_packages(),
-    python_requires='>=3.6',
+    python_requires=">=3.6",
     install_requires=requirements,
-    version="0.1.0",
-    setup_requires=['setuptools_scm'],
+    version="0.2.0",
+    setup_requires=["setuptools_scm"],
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Science/Research',
-        'Framework :: napari',
-        'Topic :: Scientific/Engineering :: Image Processing',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Operating System :: OS Independent',
-        'License :: OSI Approved :: BSD License',
+        "Development Status :: 2 - Pre-Alpha",
+        "Intended Audience :: Science/Research",
+        "Framework :: napari",
+        "Topic :: Scientific/Engineering :: Image Processing",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Operating System :: OS Independent",
+        "License :: OSI Approved :: BSD License",
     ],
     entry_points={
-        'napari.plugin': [
-            'napari_laptrack = napari_laptrack',
+        "napari.plugin": [
+            "napari_laptrack = napari_laptrack",
         ],
     },
 )
```

