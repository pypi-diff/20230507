# Comparing `tmp/cellpy-1.0.0a3.tar.gz` & `tmp/cellpy-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellpy-1.0.0a3.tar", last modified: Thu May  4 13:01:03 2023, max compression
+gzip compressed data, was "cellpy-1.0.0a4.tar", last modified: Sat May  6 22:11:53 2023, max compression
```

## Comparing `cellpy-1.0.0a3.tar` & `cellpy-1.0.0a4.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:03.083461 cellpy-1.0.0a3/
--rw-rw-rw-   0        0        0      503 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/AUTHORS.rst
--rw-rw-rw-   0        0        0     3086 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     3908 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/HISTORY.rst
--rw-rw-rw-   0        0        0     1089 2021-12-21 09:11:58.000000 cellpy-1.0.0a3/LICENSE
--rw-rw-rw-   0        0        0      645 2022-05-27 12:07:50.000000 cellpy-1.0.0a3/MANIFEST.in
--rw-rw-rw-   0        0        0     6518 2023-05-04 13:01:03.082460 cellpy-1.0.0a3/PKG-INFO
--rw-rw-rw-   0        0        0     1872 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.227799 cellpy-1.0.0a3/cellpy/
--rw-rw-rw-   0        0        0      805 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/__init__.py
--rw-rw-rw-   0        0        0       25 2023-05-04 13:00:22.000000 cellpy-1.0.0a3/cellpy/_version.py
--rw-rw-rw-   0        0        0    51949 2023-05-02 11:55:35.000000 cellpy-1.0.0a3/cellpy/cli.py
--rw-rw-rw-   0        0        0     1228 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.256840 cellpy-1.0.0a3/cellpy/internals/
--rw-rw-rw-   0        0        0        0 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/internals/__init__.py
--rw-rw-rw-   0        0        0    26690 2023-05-04 11:47:01.000000 cellpy-1.0.0a3/cellpy/internals/core.py
--rw-rw-rw-   0        0        0     4838 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/log.py
--rw-rw-rw-   0        0        0     1750 2021-12-21 09:11:58.000000 cellpy-1.0.0a3/cellpy/logging.json
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.277877 cellpy-1.0.0a3/cellpy/parameters/
--rw-rw-rw-   0        0        0     3183 2023-05-02 11:51:31.000000 cellpy-1.0.0a3/cellpy/parameters/.cellpy_prms_default.conf
--rw-rw-rw-   0        0        0        2 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/parameters/__init__.py
--rw-rw-rw-   0        0        0    23361 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/parameters/internal_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.283879 cellpy-1.0.0a3/cellpy/parameters/legacy/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a3/cellpy/parameters/legacy/__init__.py
--rw-rw-rw-   0        0        0    24146 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/parameters/legacy/update_headers.py
--rw-rw-rw-   0        0        0    12142 2023-05-02 11:42:19.000000 cellpy-1.0.0a3/cellpy/parameters/prmreader.py
--rw-rw-rw-   0        0        0    12220 2023-05-02 11:49:22.000000 cellpy-1.0.0a3/cellpy/parameters/prms.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.309923 cellpy-1.0.0a3/cellpy/readers/
--rw-rw-rw-   0        0        0        2 2021-12-21 09:11:58.000000 cellpy-1.0.0a3/cellpy/readers/__init__.py
--rw-rw-rw-   0        0        0   227868 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/cellreader.py
--rw-rw-rw-   0        0        0    39447 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/core.py
--rw-rw-rw-   0        0        0    22998 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/dbreader.py
--rw-rw-rw-   0        0        0    13468 2023-05-04 11:58:58.000000 cellpy-1.0.0a3/cellpy/readers/filefinder.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.387862 cellpy-1.0.0a3/cellpy/readers/instruments/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a3/cellpy/readers/instruments/__init__.py
--rw-rw-rw-   0        0        0    50849 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/arbin_res.py
--rw-rw-rw-   0        0        0    19381 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql.py
--rw-rw-rw-   0        0        0    21062 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql_7.py
--rw-rw-rw-   0        0        0    11134 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql_csv.py
--rw-rw-rw-   0        0        0     7126 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql_h5.py
--rw-rw-rw-   0        0        0     9883 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql_xlsx.py
--rw-rw-rw-   0        0        0    27501 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/base.py
--rw-rw-rw-   0        0        0    22693 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/biologics_mpr.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.417245 cellpy-1.0.0a3/cellpy/readers/instruments/configurations/
--rw-rw-rw-   0        0        0     6607 2022-06-03 19:58:41.000000 cellpy-1.0.0a3/cellpy/readers/instruments/configurations/__init__.py
--rw-rw-rw-   0        0        0     1700 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_four.py
--rw-rw-rw-   0        0        0     4084 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_one.py
--rw-rw-rw-   0        0        0     1990 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_three.py
--rw-rw-rw-   0        0        0     1788 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_two.py
--rw-rw-rw-   0        0        0     3549 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_zero.py
--rw-rw-rw-   0        0        0     2132 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/configurations/neware_txt_zero.py
--rw-rw-rw-   0        0        0    10327 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/custom.py
--rw-rw-rw-   0        0        0     3760 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/ext_nda_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.425247 cellpy-1.0.0a3/cellpy/readers/instruments/loader_specific_modules/
--rw-rw-rw-   0        0        0        0 2022-06-03 19:58:41.000000 cellpy-1.0.0a3/cellpy/readers/instruments/loader_specific_modules/__init__.py
--rw-rw-rw-   0        0        0    22115 2022-06-03 19:58:41.000000 cellpy-1.0.0a3/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
--rw-rw-rw-   0        0        0     1067 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/local_instrument.py
--rw-rw-rw-   0        0        0    12886 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/maccor_txt.py
--rw-rw-rw-   0        0        0     3488 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/neware_txt.py
--rw-rw-rw-   0        0        0    16769 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/pec_csv.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.439260 cellpy-1.0.0a3/cellpy/readers/instruments/processors/
--rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-1.0.0a3/cellpy/readers/instruments/processors/__init__.py
--rw-rw-rw-   0        0        0    15265 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/processors/post_processors.py
--rw-rw-rw-   0        0        0     1450 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/instruments/processors/pre_processors.py
--rw-rw-rw-   0        0        0    26852 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/readers/sql_dbreader.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.502372 cellpy-1.0.0a3/cellpy/utils/
--rw-rw-rw-   0        0        0      192 2021-12-21 09:11:58.000000 cellpy-1.0.0a3/cellpy/utils/__init__.py
--rw-rw-rw-   0        0        0    48182 2023-05-03 09:31:40.000000 cellpy-1.0.0a3/cellpy/utils/batch.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.551372 cellpy-1.0.0a3/cellpy/utils/batch_tools/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/__init__.py
--rw-rw-rw-   0        0        0     7578 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_analyzers.py
--rw-rw-rw-   0        0        0    19566 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_core.py
--rw-rw-rw-   0        0        0    40001 2023-05-03 09:29:45.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_experiments.py
--rw-rw-rw-   0        0        0     2931 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_exporters.py
--rw-rw-rw-   0        0        0    13636 2023-05-02 11:59:40.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_helpers.py
--rw-rw-rw-   0        0        0    27683 2023-05-02 13:39:36.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_journals.py
--rw-rw-rw-   0        0        0    29066 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_plotters.py
--rw-rw-rw-   0        0        0      245 2021-12-21 09:11:58.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_reporters.py
--rw-rw-rw-   0        0        0     3339 2022-05-27 12:03:59.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/dumpers.py
--rw-rw-rw-   0        0        0     9872 2023-05-02 10:20:24.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/engines.py
--rw-rw-rw-   0        0        0     5294 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/batch_tools/sqlite_from_excel_db.py
--rw-rw-rw-   0        0        0    63308 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/collectors.py
--rw-rw-rw-   0        0        0    45461 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/collectors_old.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.558373 cellpy-1.0.0a3/cellpy/utils/data/
--rw-rw-rw-   0        0        0  3700143 2023-05-03 22:26:41.000000 cellpy-1.0.0a3/cellpy/utils/data/20160805_test001_45_cc.h5
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.579371 cellpy-1.0.0a3/cellpy/utils/data/raw/
--rw-rw-rw-   0        0        0  1613824 2021-12-21 09:11:58.000000 cellpy-1.0.0a3/cellpy/utils/data/raw/20160805_test001_45_cc_01.res
--rw-rw-rw-   0        0        0      260 2022-05-27 12:07:50.000000 cellpy-1.0.0a3/cellpy/utils/diagnostics.py
--rw-rw-rw-   0        0        0    79016 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/easyplot.py
--rw-rw-rw-   0        0        0     1576 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/example_data.py
--rw-rw-rw-   0        0        0    39446 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/helpers.py
--rw-rw-rw-   0        0        0    38967 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/ica.py
--rw-rw-rw-   0        0        0      189 2022-05-27 12:07:50.000000 cellpy-1.0.0a3/cellpy/utils/live.py
--rw-rw-rw-   0        0        0    24037 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/ocv_rlx.py
--rw-rw-rw-   0        0        0    45397 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/plotutils.py
--rw-rw-rw-   0        0        0     1787 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/cellpy/utils/processor.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.248839 cellpy-1.0.0a3/cellpy.egg-info/
--rw-rw-rw-   0        0        0     6518 2023-05-04 13:01:01.000000 cellpy-1.0.0a3/cellpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7846 2023-05-04 13:01:02.000000 cellpy-1.0.0a3/cellpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 13:01:01.000000 cellpy-1.0.0a3/cellpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 13:01:01.000000 cellpy-1.0.0a3/cellpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-04 13:00:59.000000 cellpy-1.0.0a3/cellpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      337 2023-05-04 13:01:01.000000 cellpy-1.0.0a3/cellpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-04 13:01:01.000000 cellpy-1.0.0a3/cellpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.606375 cellpy-1.0.0a3/docs/
--rw-rw-rw-   0        0        0     6939 2022-09-20 08:21:07.000000 cellpy-1.0.0a3/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.177629 cellpy-1.0.0a3/docs/_build/
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.176629 cellpy-1.0.0a3/docs/_build/.doctrees/
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.622371 cellpy-1.0.0a3/docs/_build/.doctrees/nbsphinx/
--rw-rw-rw-   0        0        0    15014 2023-04-30 13:53:57.000000 cellpy-1.0.0a3/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
--rw-rw-rw-   0        0        0    14599 2023-04-30 13:53:57.000000 cellpy-1.0.0a3/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
--rw-rw-rw-   0        0        0    13527 2023-04-30 13:53:57.000000 cellpy-1.0.0a3/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
--rw-rw-rw-   0        0        0    25669 2023-04-30 13:54:02.000000 cellpy-1.0.0a3/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.696856 cellpy-1.0.0a3/docs/_build/_images/
--rw-rw-rw-   0        0        0    15014 2023-04-27 15:02:55.000000 cellpy-1.0.0a3/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
--rw-rw-rw-   0        0        0    14599 2023-04-27 15:02:55.000000 cellpy-1.0.0a3/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
--rw-rw-rw-   0        0        0    13527 2023-04-27 15:02:55.000000 cellpy-1.0.0a3/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
--rw-rw-rw-   0        0        0    25669 2023-04-27 15:03:02.000000 cellpy-1.0.0a3/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
--rw-rw-rw-   0        0        0    11678 2023-04-29 14:19:31.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png
--rw-rw-rw-   0        0        0    22040 2023-04-29 14:33:27.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png
--rw-rw-rw-   0        0        0    21790 2023-04-29 14:26:00.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png
--rw-rw-rw-   0        0        0    32991 2023-04-29 14:26:01.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png
--rw-rw-rw-   0        0        0    32991 2023-04-30 20:02:23.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png
--rw-rw-rw-   0        0        0     7231 2023-04-29 14:12:31.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png
--rw-rw-rw-   0        0        0    13360 2023-04-29 14:36:26.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png
--rw-rw-rw-   0        0        0    21790 2023-04-30 20:02:22.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png
--rw-rw-rw-   0        0        0     5391 2023-04-29 14:10:02.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png
--rw-rw-rw-   0        0        0    20826 2023-04-29 14:29:06.000000 cellpy-1.0.0a3/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png
--rw-rw-rw-   0        0        0    88743 2023-04-19 13:49:30.000000 cellpy-1.0.0a3/docs/_build/_images/templates_jupyterlab_001.png
--rw-rw-rw-   0        0        0   296908 2022-05-27 12:07:51.000000 cellpy-1.0.0a3/docs/_build/_images/tutorials_utils_plotting_fig1.png
--rw-rw-rw-   0        0        0    54588 2022-05-27 12:07:51.000000 cellpy-1.0.0a3/docs/_build/_images/tutorials_utils_plotting_fig2.png
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.708851 cellpy-1.0.0a3/docs/_build/_static/
--rw-rw-rw-   0        0        0      286 2023-04-25 11:20:36.000000 cellpy-1.0.0a3/docs/_build/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a3/docs/_build/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a3/docs/_build/_static/plus.png
--rw-rw-rw-   0        0        0     1695 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/adapted_readme.rst
--rw-rw-rw-   0        0        0    10731 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.741848 cellpy-1.0.0a3/docs/developers_guide/
--rw-rw-rw-   0        0        0     1334 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/developers_guide/dev_cellpy_data_structure.rst
--rw-rw-rw-   0        0        0     5904 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/developers_guide/dev_cellpy_folder_structure.rst
--rw-rw-rw-   0        0        0      935 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/developers_guide/dev_cellpy_packaging_pypi.rst
--rw-rw-rw-   0        0        0     3009 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/developers_guide/dev_cellpy_setup.rst
--rw-rw-rw-   0        0        0     1821 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/developers_guide/dev_conda_package.rst
--rw-rw-rw-   0        0        0     2136 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/developers_guide/dev_docs.rst
--rw-rw-rw-   0        0        0     5218 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/developers_guide/dev_loaders_and_instruments.rst
--rw-rw-rw-   0        0        0     1768 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/developers_guide/dev_various.rst
--rw-rw-rw-   0        0        0      326 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/developers_guide/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.766850 cellpy-1.0.0a3/docs/examples_and_tutorials/
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.797848 cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/
--rw-rw-rw-   0        0        0    15786 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst
--rw-rw-rw-   0        0        0     3909 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst
--rw-rw-rw-   0        0        0     5485 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst
--rw-rw-rw-   0        0        0     4465 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst
--rw-rw-rw-   0        0        0     5908 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/05_configuring.rst
--rw-rw-rw-   0        0        0     1052 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/06_pandas.rst
--rw-rw-rw-   0        0        0     1102 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst
--rw-rw-rw-   0        0        0     8224 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst
--rw-rw-rw-   0        0        0      484 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/basics.rst
--rw-rw-rw-   0        0        0      366 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/examples.rst
--rw-rw-rw-   0        0        0      174 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.816847 cellpy-1.0.0a3/docs/examples_and_tutorials/loaders/
--rw-rw-rw-   0        0        0       49 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/loaders/01_arbin.rst
--rw-rw-rw-   0        0        0       52 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/loaders/02_maccor.rst
--rw-rw-rw-   0        0        0       43 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/loaders/03_PEC.rst
--rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/loaders/04_Neware.rst
--rw-rw-rw-   0        0        0       62 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/loaders/05_biologics.rst
--rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/loaders/06_custom.rst
--rw-rw-rw-   0        0        0      260 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/loaders.rst
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.181153 cellpy-1.0.0a3/docs/examples_and_tutorials/notebooks/
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.974146 cellpy-1.0.0a3/docs/examples_and_tutorials/notebooks/images/
--rw-rw-rw-   0        0        0    88743 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png
--rw-rw-rw-   0        0        0    95663 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png
--rw-rw-rw-   0        0        0      231 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/notebooks.rst
--rw-rw-rw-   0        0        0     1797 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/tips_and_tricks.rst
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:02.998377 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/
--rw-rw-rw-   0        0        0     4388 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/batch.rst
--rw-rw-rw-   0        0        0       59 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/collectors.rst
--rw-rw-rw-   0        0        0       53 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/easyplot.rst
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:03.005398 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/figures/
--rw-rw-rw-   0        0        0   296908 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png
--rw-rw-rw-   0        0        0    54588 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png
--rw-rw-rw-   0        0        0     1219 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/ica.rst
--rw-rw-rw-   0        0        0     2063 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/plotting.rst
--rw-rw-rw-   0        0        0      338 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/templates.rst
--rw-rw-rw-   0        0        0     1379 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst
--rw-rw-rw-   0        0        0      371 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/examples_and_tutorials/utils.rst
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:03.012399 cellpy-1.0.0a3/docs/figures/
--rw-rw-rw-   0        0        0     9981 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/figures/cellpy-icon-bw.png
--rw-rw-rw-   0        0        0    10302 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/figures/cellpy-logo-v1.png
--rw-rw-rw-   0        0        0      593 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:03.035463 cellpy-1.0.0a3/docs/main_description/
--rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/main_description/authors.rst
--rw-rw-rw-   0        0        0       37 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/main_description/contributing.rst
--rw-rw-rw-   0        0        0    16327 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/main_description/formats.rst
--rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/main_description/history.rst
--rw-rw-rw-   0        0        0      182 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/main_description/index.rst
--rw-rw-rw-   0        0        0     4288 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/main_description/installation.rst
--rw-rw-rw-   0        0        0     3444 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/main_description/usage.rst
--rwxrwxrwx   0        0        0     6701 2022-09-20 08:21:07.000000 cellpy-1.0.0a3/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-04 13:01:03.079462 cellpy-1.0.0a3/docs/source/
--rw-rw-rw-   0        0        0      367 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.internals.rst
--rw-rw-rw-   0        0        0      447 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.parameters.legacy.rst
--rw-rw-rw-   0        0        0      847 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.parameters.rst
--rw-rw-rw-   0        0        0     1911 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.readers.instruments.configurations.rst
--rw-rw-rw-   0        0        0      631 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.readers.instruments.loader_specific_modules.rst
--rw-rw-rw-   0        0        0      783 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.readers.instruments.processors.rst
--rw-rw-rw-   0        0        0     3413 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.readers.instruments.rst
--rw-rw-rw-   0        0        0     1139 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.readers.rst
--rw-rw-rw-   0        0        0      721 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.rst
--rw-rw-rw-   0        0        0     2610 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.utils.batch_tools.rst
--rw-rw-rw-   0        0        0     2222 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/docs/source/cellpy.utils.rst
--rw-rw-rw-   0        0        0       62 2023-05-01 10:14:23.000000 cellpy-1.0.0a3/docs/source/modules.rst
--rw-rw-rw-   0        0        0      281 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 13:01:03.084462 cellpy-1.0.0a3/setup.cfg
--rw-rw-rw-   0        0        0     2952 2023-05-01 18:24:45.000000 cellpy-1.0.0a3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.202692 cellpy-1.0.0a4/
+-rw-rw-rw-   0        0        0      503 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3086 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     3908 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/HISTORY.rst
+-rw-rw-rw-   0        0        0     1089 2021-12-21 09:11:58.000000 cellpy-1.0.0a4/LICENSE
+-rw-rw-rw-   0        0        0      645 2022-05-27 12:07:50.000000 cellpy-1.0.0a4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6518 2023-05-06 22:11:53.201691 cellpy-1.0.0a4/PKG-INFO
+-rw-rw-rw-   0        0        0     1872 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.903094 cellpy-1.0.0a4/cellpy/
+-rw-rw-rw-   0        0        0      805 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/__init__.py
+-rw-rw-rw-   0        0        0       25 2023-05-06 22:11:31.000000 cellpy-1.0.0a4/cellpy/_version.py
+-rw-rw-rw-   0        0        0    53597 2023-05-06 21:51:58.000000 cellpy-1.0.0a4/cellpy/cli.py
+-rw-rw-rw-   0        0        0     1228 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.916098 cellpy-1.0.0a4/cellpy/internals/
+-rw-rw-rw-   0        0        0        0 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/internals/__init__.py
+-rw-rw-rw-   0        0        0    27994 2023-05-06 21:51:58.000000 cellpy-1.0.0a4/cellpy/internals/core.py
+-rw-rw-rw-   0        0        0     4838 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/log.py
+-rw-rw-rw-   0        0        0     1750 2021-12-21 09:11:58.000000 cellpy-1.0.0a4/cellpy/logging.json
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.924095 cellpy-1.0.0a4/cellpy/parameters/
+-rw-rw-rw-   0        0        0     3183 2023-05-02 11:51:31.000000 cellpy-1.0.0a4/cellpy/parameters/.cellpy_prms_default.conf
+-rw-rw-rw-   0        0        0        2 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/parameters/__init__.py
+-rw-rw-rw-   0        0        0    23784 2023-05-06 21:51:58.000000 cellpy-1.0.0a4/cellpy/parameters/internal_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.926095 cellpy-1.0.0a4/cellpy/parameters/legacy/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a4/cellpy/parameters/legacy/__init__.py
+-rw-rw-rw-   0        0        0    24146 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/parameters/legacy/update_headers.py
+-rw-rw-rw-   0        0        0    12142 2023-05-02 11:42:19.000000 cellpy-1.0.0a4/cellpy/parameters/prmreader.py
+-rw-rw-rw-   0        0        0    12220 2023-05-02 11:49:22.000000 cellpy-1.0.0a4/cellpy/parameters/prms.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.936093 cellpy-1.0.0a4/cellpy/readers/
+-rw-rw-rw-   0        0        0        2 2021-12-21 09:11:58.000000 cellpy-1.0.0a4/cellpy/readers/__init__.py
+-rw-rw-rw-   0        0        0   233026 2023-05-06 21:51:58.000000 cellpy-1.0.0a4/cellpy/readers/cellreader.py
+-rw-rw-rw-   0        0        0    39537 2023-05-06 21:51:58.000000 cellpy-1.0.0a4/cellpy/readers/core.py
+-rw-rw-rw-   0        0        0    22998 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/dbreader.py
+-rw-rw-rw-   0        0        0    13825 2023-05-06 21:51:58.000000 cellpy-1.0.0a4/cellpy/readers/filefinder.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.963094 cellpy-1.0.0a4/cellpy/readers/instruments/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a4/cellpy/readers/instruments/__init__.py
+-rw-rw-rw-   0        0        0    50849 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/arbin_res.py
+-rw-rw-rw-   0        0        0    19381 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql.py
+-rw-rw-rw-   0        0        0    21062 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql_7.py
+-rw-rw-rw-   0        0        0    11134 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql_csv.py
+-rw-rw-rw-   0        0        0     7126 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql_h5.py
+-rw-rw-rw-   0        0        0     9883 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql_xlsx.py
+-rw-rw-rw-   0        0        0    27501 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/base.py
+-rw-rw-rw-   0        0        0    22693 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/biologics_mpr.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.976095 cellpy-1.0.0a4/cellpy/readers/instruments/configurations/
+-rw-rw-rw-   0        0        0     6607 2022-06-03 19:58:41.000000 cellpy-1.0.0a4/cellpy/readers/instruments/configurations/__init__.py
+-rw-rw-rw-   0        0        0     1700 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_four.py
+-rw-rw-rw-   0        0        0     4084 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_one.py
+-rw-rw-rw-   0        0        0     1990 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_three.py
+-rw-rw-rw-   0        0        0     1788 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_two.py
+-rw-rw-rw-   0        0        0     3549 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_zero.py
+-rw-rw-rw-   0        0        0     2132 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/configurations/neware_txt_zero.py
+-rw-rw-rw-   0        0        0    10327 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/custom.py
+-rw-rw-rw-   0        0        0     3760 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/ext_nda_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.979095 cellpy-1.0.0a4/cellpy/readers/instruments/loader_specific_modules/
+-rw-rw-rw-   0        0        0        0 2022-06-03 19:58:41.000000 cellpy-1.0.0a4/cellpy/readers/instruments/loader_specific_modules/__init__.py
+-rw-rw-rw-   0        0        0    22115 2022-06-03 19:58:41.000000 cellpy-1.0.0a4/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
+-rw-rw-rw-   0        0        0     1067 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/local_instrument.py
+-rw-rw-rw-   0        0        0    12886 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/maccor_txt.py
+-rw-rw-rw-   0        0        0     3488 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/neware_txt.py
+-rw-rw-rw-   0        0        0    16769 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/pec_csv.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.984093 cellpy-1.0.0a4/cellpy/readers/instruments/processors/
+-rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-1.0.0a4/cellpy/readers/instruments/processors/__init__.py
+-rw-rw-rw-   0        0        0    15265 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/processors/post_processors.py
+-rw-rw-rw-   0        0        0     1450 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/processors/pre_processors.py
+-rw-rw-rw-   0        0        0    26852 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/sql_dbreader.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.006094 cellpy-1.0.0a4/cellpy/utils/
+-rw-rw-rw-   0        0        0      192 2021-12-21 09:11:58.000000 cellpy-1.0.0a4/cellpy/utils/__init__.py
+-rw-rw-rw-   0        0        0    48182 2023-05-03 09:31:40.000000 cellpy-1.0.0a4/cellpy/utils/batch.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.025619 cellpy-1.0.0a4/cellpy/utils/batch_tools/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/__init__.py
+-rw-rw-rw-   0        0        0     7578 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_analyzers.py
+-rw-rw-rw-   0        0        0    19566 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_core.py
+-rw-rw-rw-   0        0        0    41058 2023-05-06 21:51:58.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_experiments.py
+-rw-rw-rw-   0        0        0     2931 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_exporters.py
+-rw-rw-rw-   0        0        0    14090 2023-05-06 21:51:58.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_helpers.py
+-rw-rw-rw-   0        0        0    27683 2023-05-02 13:39:36.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_journals.py
+-rw-rw-rw-   0        0        0    29066 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_plotters.py
+-rw-rw-rw-   0        0        0      245 2021-12-21 09:11:58.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_reporters.py
+-rw-rw-rw-   0        0        0     3339 2022-05-27 12:03:59.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/dumpers.py
+-rw-rw-rw-   0        0        0     9872 2023-05-02 10:20:24.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/engines.py
+-rw-rw-rw-   0        0        0     5294 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/sqlite_from_excel_db.py
+-rw-rw-rw-   0        0        0    63308 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/collectors.py
+-rw-rw-rw-   0        0        0    45461 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/collectors_old.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.027174 cellpy-1.0.0a4/cellpy/utils/data/
+-rw-rw-rw-   0        0        0  3700143 2023-05-06 21:47:28.000000 cellpy-1.0.0a4/cellpy/utils/data/20160805_test001_45_cc.h5
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.037175 cellpy-1.0.0a4/cellpy/utils/data/raw/
+-rw-rw-rw-   0        0        0  1613824 2021-12-21 09:11:58.000000 cellpy-1.0.0a4/cellpy/utils/data/raw/20160805_test001_45_cc_01.res
+-rw-rw-rw-   0        0        0      260 2022-05-27 12:07:50.000000 cellpy-1.0.0a4/cellpy/utils/diagnostics.py
+-rw-rw-rw-   0        0        0    79016 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/easyplot.py
+-rw-rw-rw-   0        0        0     1576 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/example_data.py
+-rw-rw-rw-   0        0        0    39446 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/helpers.py
+-rw-rw-rw-   0        0        0    38991 2023-05-06 21:51:58.000000 cellpy-1.0.0a4/cellpy/utils/ica.py
+-rw-rw-rw-   0        0        0      189 2022-05-27 12:07:50.000000 cellpy-1.0.0a4/cellpy/utils/live.py
+-rw-rw-rw-   0        0        0    24037 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/ocv_rlx.py
+-rw-rw-rw-   0        0        0    45397 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/plotutils.py
+-rw-rw-rw-   0        0        0     1787 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/processor.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.913095 cellpy-1.0.0a4/cellpy.egg-info/
+-rw-rw-rw-   0        0        0     6518 2023-05-06 22:11:52.000000 cellpy-1.0.0a4/cellpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7846 2023-05-06 22:11:52.000000 cellpy-1.0.0a4/cellpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 22:11:52.000000 cellpy-1.0.0a4/cellpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 22:11:52.000000 cellpy-1.0.0a4/cellpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 22:11:51.000000 cellpy-1.0.0a4/cellpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      337 2023-05-06 22:11:52.000000 cellpy-1.0.0a4/cellpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-06 22:11:52.000000 cellpy-1.0.0a4/cellpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.051174 cellpy-1.0.0a4/docs/
+-rw-rw-rw-   0        0        0     6939 2022-09-20 08:21:07.000000 cellpy-1.0.0a4/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.880095 cellpy-1.0.0a4/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.879096 cellpy-1.0.0a4/docs/_build/.doctrees/
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.057175 cellpy-1.0.0a4/docs/_build/.doctrees/nbsphinx/
+-rw-rw-rw-   0        0        0    15014 2023-04-30 13:53:57.000000 cellpy-1.0.0a4/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
+-rw-rw-rw-   0        0        0    14599 2023-04-30 13:53:57.000000 cellpy-1.0.0a4/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
+-rw-rw-rw-   0        0        0    13527 2023-04-30 13:53:57.000000 cellpy-1.0.0a4/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
+-rw-rw-rw-   0        0        0    25669 2023-04-30 13:54:02.000000 cellpy-1.0.0a4/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.090690 cellpy-1.0.0a4/docs/_build/_images/
+-rw-rw-rw-   0        0        0    15014 2023-04-27 15:02:55.000000 cellpy-1.0.0a4/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
+-rw-rw-rw-   0        0        0    14599 2023-04-27 15:02:55.000000 cellpy-1.0.0a4/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
+-rw-rw-rw-   0        0        0    13527 2023-04-27 15:02:55.000000 cellpy-1.0.0a4/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
+-rw-rw-rw-   0        0        0    25669 2023-04-27 15:03:02.000000 cellpy-1.0.0a4/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
+-rw-rw-rw-   0        0        0    11678 2023-04-29 14:19:31.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png
+-rw-rw-rw-   0        0        0    22040 2023-04-29 14:33:27.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png
+-rw-rw-rw-   0        0        0    21790 2023-04-29 14:26:00.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png
+-rw-rw-rw-   0        0        0    32991 2023-04-29 14:26:01.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png
+-rw-rw-rw-   0        0        0    32991 2023-04-30 20:02:23.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png
+-rw-rw-rw-   0        0        0     7231 2023-04-29 14:12:31.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png
+-rw-rw-rw-   0        0        0    13360 2023-04-29 14:36:26.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png
+-rw-rw-rw-   0        0        0    21790 2023-04-30 20:02:22.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png
+-rw-rw-rw-   0        0        0     5391 2023-04-29 14:10:02.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png
+-rw-rw-rw-   0        0        0    20826 2023-04-29 14:29:06.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png
+-rw-rw-rw-   0        0        0    88743 2023-04-19 13:49:30.000000 cellpy-1.0.0a4/docs/_build/_images/templates_jupyterlab_001.png
+-rw-rw-rw-   0        0        0   296908 2022-05-27 12:07:51.000000 cellpy-1.0.0a4/docs/_build/_images/tutorials_utils_plotting_fig1.png
+-rw-rw-rw-   0        0        0    54588 2022-05-27 12:07:51.000000 cellpy-1.0.0a4/docs/_build/_images/tutorials_utils_plotting_fig2.png
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.094692 cellpy-1.0.0a4/docs/_build/_static/
+-rw-rw-rw-   0        0        0      286 2023-04-25 11:20:36.000000 cellpy-1.0.0a4/docs/_build/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a4/docs/_build/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a4/docs/_build/_static/plus.png
+-rw-rw-rw-   0        0        0     1695 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/adapted_readme.rst
+-rw-rw-rw-   0        0        0    10731 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.108692 cellpy-1.0.0a4/docs/developers_guide/
+-rw-rw-rw-   0        0        0     1334 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/developers_guide/dev_cellpy_data_structure.rst
+-rw-rw-rw-   0        0        0     5904 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/developers_guide/dev_cellpy_folder_structure.rst
+-rw-rw-rw-   0        0        0      935 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/developers_guide/dev_cellpy_packaging_pypi.rst
+-rw-rw-rw-   0        0        0     3009 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/developers_guide/dev_cellpy_setup.rst
+-rw-rw-rw-   0        0        0     1821 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/developers_guide/dev_conda_package.rst
+-rw-rw-rw-   0        0        0     2136 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/developers_guide/dev_docs.rst
+-rw-rw-rw-   0        0        0     5218 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/developers_guide/dev_loaders_and_instruments.rst
+-rw-rw-rw-   0        0        0     1768 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/developers_guide/dev_various.rst
+-rw-rw-rw-   0        0        0      326 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/developers_guide/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.120691 cellpy-1.0.0a4/docs/examples_and_tutorials/
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.134693 cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/
+-rw-rw-rw-   0        0        0    15786 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst
+-rw-rw-rw-   0        0        0     3909 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst
+-rw-rw-rw-   0        0        0     5485 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst
+-rw-rw-rw-   0        0        0     4465 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst
+-rw-rw-rw-   0        0        0     5908 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/05_configuring.rst
+-rw-rw-rw-   0        0        0     1052 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/06_pandas.rst
+-rw-rw-rw-   0        0        0     1102 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst
+-rw-rw-rw-   0        0        0     8224 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst
+-rw-rw-rw-   0        0        0      484 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/basics.rst
+-rw-rw-rw-   0        0        0      366 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/examples.rst
+-rw-rw-rw-   0        0        0      174 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.144700 cellpy-1.0.0a4/docs/examples_and_tutorials/loaders/
+-rw-rw-rw-   0        0        0       49 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/loaders/01_arbin.rst
+-rw-rw-rw-   0        0        0       52 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/loaders/02_maccor.rst
+-rw-rw-rw-   0        0        0       43 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/loaders/03_PEC.rst
+-rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/loaders/04_Neware.rst
+-rw-rw-rw-   0        0        0       62 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/loaders/05_biologics.rst
+-rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/loaders/06_custom.rst
+-rw-rw-rw-   0        0        0      260 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/loaders.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.881095 cellpy-1.0.0a4/docs/examples_and_tutorials/notebooks/
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.148700 cellpy-1.0.0a4/docs/examples_and_tutorials/notebooks/images/
+-rw-rw-rw-   0        0        0    88743 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png
+-rw-rw-rw-   0        0        0    95663 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png
+-rw-rw-rw-   0        0        0      231 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/notebooks.rst
+-rw-rw-rw-   0        0        0     1797 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/tips_and_tricks.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.159689 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/
+-rw-rw-rw-   0        0        0     4388 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/batch.rst
+-rw-rw-rw-   0        0        0       59 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/collectors.rst
+-rw-rw-rw-   0        0        0       53 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/easyplot.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.165691 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/figures/
+-rw-rw-rw-   0        0        0   296908 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png
+-rw-rw-rw-   0        0        0    54588 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png
+-rw-rw-rw-   0        0        0     1219 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/ica.rst
+-rw-rw-rw-   0        0        0     2063 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/plotting.rst
+-rw-rw-rw-   0        0        0      338 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/templates.rst
+-rw-rw-rw-   0        0        0     1379 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst
+-rw-rw-rw-   0        0        0      371 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.169691 cellpy-1.0.0a4/docs/figures/
+-rw-rw-rw-   0        0        0     9981 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/figures/cellpy-icon-bw.png
+-rw-rw-rw-   0        0        0    10302 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/figures/cellpy-logo-v1.png
+-rw-rw-rw-   0        0        0      593 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.180692 cellpy-1.0.0a4/docs/main_description/
+-rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/main_description/authors.rst
+-rw-rw-rw-   0        0        0       37 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/main_description/contributing.rst
+-rw-rw-rw-   0        0        0    16327 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/main_description/formats.rst
+-rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/main_description/history.rst
+-rw-rw-rw-   0        0        0      182 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/main_description/index.rst
+-rw-rw-rw-   0        0        0     4288 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/main_description/installation.rst
+-rw-rw-rw-   0        0        0     3444 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/main_description/usage.rst
+-rwxrwxrwx   0        0        0     6701 2022-09-20 08:21:07.000000 cellpy-1.0.0a4/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.200692 cellpy-1.0.0a4/docs/source/
+-rw-rw-rw-   0        0        0      367 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.internals.rst
+-rw-rw-rw-   0        0        0      447 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.parameters.legacy.rst
+-rw-rw-rw-   0        0        0      847 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.parameters.rst
+-rw-rw-rw-   0        0        0     1911 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.readers.instruments.configurations.rst
+-rw-rw-rw-   0        0        0      631 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.readers.instruments.loader_specific_modules.rst
+-rw-rw-rw-   0        0        0      783 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.readers.instruments.processors.rst
+-rw-rw-rw-   0        0        0     3413 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.readers.instruments.rst
+-rw-rw-rw-   0        0        0     1139 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.readers.rst
+-rw-rw-rw-   0        0        0      721 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.rst
+-rw-rw-rw-   0        0        0     2610 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.utils.batch_tools.rst
+-rw-rw-rw-   0        0        0     2222 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.utils.rst
+-rw-rw-rw-   0        0        0       62 2023-05-01 10:14:23.000000 cellpy-1.0.0a4/docs/source/modules.rst
+-rw-rw-rw-   0        0        0      281 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 22:11:53.202692 cellpy-1.0.0a4/setup.cfg
+-rw-rw-rw-   0        0        0     2952 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/setup.py
```

### Comparing `cellpy-1.0.0a3/CONTRIBUTING.rst` & `cellpy-1.0.0a4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/HISTORY.rst` & `cellpy-1.0.0a4/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/LICENSE` & `cellpy-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/MANIFEST.in` & `cellpy-1.0.0a4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/PKG-INFO` & `cellpy-1.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpy
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Extract and manipulate data from battery data testers.
 Home-page: https://github.com/jepegit/cellpy
 Author: Jan Petter Maehlen
 Author-email: jepe@ife.no
 License: MIT license
 Keywords: cellpy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cellpy-1.0.0a3/README.rst` & `cellpy-1.0.0a4/README.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/__init__.py` & `cellpy-1.0.0a4/cellpy/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/cli.py` & `cellpy-1.0.0a4/cellpy/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,1688 +1,1686 @@
-import base64
-import getpass
-import logging
-import os
-import pathlib
-from pprint import pprint
-import re
-import subprocess
-import sys
-from typing import Union
-import urllib
-from pathlib import Path
-
-import click
-import pkg_resources
-from github import Github
-
-import cellpy._version
-from cellpy.exceptions import ConfigFileNotWritten
-from cellpy.parameters import prmreader
-from cellpy.parameters.internal_settings import OTHERPATHS
-from cellpy.internals.core import OtherPath
-
-VERSION = cellpy._version.__version__
-REPO = "jepegit/cellpy"
-USER = "jepegit"
-GITHUB_PWD_VAR_NAME = "GD_PWD"
-
-
-def save_prm_file(prm_filename):
-    """saves (writes) the prms to file"""
-    prmreader._write_prm_file(prm_filename)
-
-
-def get_package_prm_dir():
-    """gets the folder where the cellpy package lives"""
-    prm_dir = pkg_resources.resource_filename("cellpy", "parameters")
-    return pathlib.Path(prm_dir)
-
-
-def get_default_config_file_path(init_filename=None):
-    """gets the path to the default config-file"""
-    prm_dir = get_package_prm_dir()
-    if not init_filename:
-        init_filename = prmreader.DEFAULT_FILENAME
-    src = prm_dir / init_filename
-    return src
-
-
-def get_dst_file(user_dir, init_filename):
-    user_dir = pathlib.Path(user_dir)
-    dst_file = user_dir / init_filename
-    return dst_file
-
-
-def check_if_needed_modules_exists():
-    pass
-
-
-def modify_config_file():
-    pass
-
-
-def create_cellpy_folders():
-    pass
-
-
-@click.group("cellpy")
-def cli():
-    pass
-
-
-# ----------------------- setup --------------------------------------
-@click.command()
-@click.option(
-    "--interactive",
-    "-i",
-    is_flag=True,
-    default=False,
-    help="Allows you to specify div. folders and setting.",
-)
-@click.option(
-    "--not-relative",
-    "-nr",
-    is_flag=True,
-    default=False,
-    help="If root-dir is given, put it directly in the root (/) folder"
-    " i.e. don't put it in your home directory. Defaults to False. Remark"
-    " that if you specifically write a path name instead of selecting the"
-    " suggested default, the path you write will be used as is.",
-)
-@click.option(
-    "--dry-run",
-    "-dr",
-    is_flag=True,
-    default=False,
-    help="Run setup in dry mode (only print - do not execute). This is"
-    " typically used when developing and testing cellpy. Defaults to"
-    " False.",
-)
-@click.option(
-    "--reset",
-    "-r",
-    is_flag=True,
-    default=False,
-    help="Do not suggest path defaults based on your current configuration-file",
-)
-@click.option(
-    "--root-dir",
-    "-d",
-    default=None,
-    type=click.Path(),
-    help="Use custom root dir. If not given, your home directory"
-    " will be used as the top level where cellpy-folders"
-    " will be put. The folder path must follow"
-    " directly after this option (if used). Example:\n"
-    " $ cellpy setup -d 'MyDir'",
-)
-@click.option(
-    "--folder-name",
-    "-n",
-    default=None,
-    type=click.Path(),
-    help="",
-)
-@click.option(
-    "--test_user", "-t", default=None, help="Fake name for fake user (for testing)"
-)
-def setup(interactive, not_relative, dry_run, reset, root_dir, folder_name, test_user):
-    """This will help you to set up cellpy."""
-
-    click.echo("[cellpy] (setup)")
-    click.echo(f"[cellpy] root-dir: {root_dir}")
-
-    # generate variables
-    init_filename = prmreader.create_custom_init_filename()
-    user_dir, dst_file = prmreader.get_user_dir_and_dst(init_filename)
-
-    if dry_run:
-        click.echo("Create custom init filename and get user_dir and destination")
-        click.echo(f"Got the following parameters:")
-        click.echo(f" - init_filename: {init_filename}")
-        click.echo(f" - user_dir: {user_dir}")
-        click.echo(f" - dst_file: {dst_file}")
-        click.echo(f" - not_relative: {not_relative}")
-
-    if root_dir and not interactive:
-        click.echo("[cellpy] custom root-dir can only be used in interactive mode")
-        click.echo("[cellpy] -> setting interactive mode")
-        interactive = True
-
-    if not root_dir:
-        root_dir = user_dir
-        # root_dir = pathlib.Path(os.getcwd())
-    root_dir = pathlib.Path(root_dir)
-
-    if dry_run:
-        click.echo(f" - root_dir: {root_dir}")
-
-    if test_user:
-        click.echo(f"[cellpy] (setup) DEV-MODE test_user: {test_user}")
-        init_filename = prmreader.create_custom_init_filename(test_user)
-        user_dir = root_dir
-        dst_file = get_dst_file(user_dir, init_filename)
-        click.echo(f"[cellpy] (setup) DEV-MODE user_dir: {user_dir}")
-        click.echo(f"[cellpy] (setup) DEV-MODE dst_file: {dst_file}")
-
-    if not pathlib.Path(dst_file).is_file():
-        click.echo(f"[cellpy] {dst_file} not found -> I will make one for you!")
-        reset = True
-
-    if interactive:
-        click.echo(" interactive mode ".center(80, "-"))
-        _update_paths(
-            custom_dir=root_dir,
-            relative_home=not not_relative,
-            default_dir=folder_name,
-            dry_run=dry_run,
-            reset=reset,
-        )
-        _write_config_file(user_dir, dst_file, init_filename, dry_run)
-        _check(dry_run=dry_run)
-
-    else:
-        if reset:
-            _update_paths(
-                user_dir,
-                False,
-                default_dir=folder_name,
-                dry_run=dry_run,
-                reset=True,
-                silent=True,
-            )
-        _write_config_file(user_dir, dst_file, init_filename, dry_run)
-        _check(dry_run=dry_run)
-
-
-def _update_paths(
-    custom_dir=None,
-    relative_home=True,
-    reset=False,
-    dry_run=False,
-    default_dir=None,
-    silent=False,
-):
-    # please, refactor me :-(
-
-    h = prmreader.get_user_dir()
-
-    if default_dir is None:
-        default_dir = "cellpy_data"
-
-    if dry_run:
-        click.echo(f" - default_dir: {default_dir}")
-        click.echo(f" - custom_dir: {custom_dir}")
-        click.echo(f" - retalive_home: {relative_home}")
-
-    if custom_dir:
-        reset = True
-        if relative_home:
-            h = h / custom_dir
-        if not custom_dir.parts[-1] == default_dir:
-            h = h / default_dir
-
-    if not reset:
-        outdatadir = pathlib.Path(prmreader.prms.Paths.outdatadir)
-        rawdatadir = OtherPath(prmreader.prms.Paths.rawdatadir)
-        cellpydatadir = OtherPath(prmreader.prms.Paths.cellpydatadir)
-        filelogdir = pathlib.Path(prmreader.prms.Paths.filelogdir)
-        examplesdir = pathlib.Path(prmreader.prms.Paths.examplesdir)
-        db_path = pathlib.Path(prmreader.prms.Paths.db_path)
-        db_filename = prmreader.prms.Paths.db_filename
-        notebookdir = pathlib.Path(prmreader.prms.Paths.notebookdir)
-        batchfiledir = pathlib.Path(prmreader.prms.Paths.batchfiledir)
-        templatedir = pathlib.Path(prmreader.prms.Paths.templatedir)
-        instrumentdir = pathlib.Path(prmreader.prms.Paths.instrumentsdir)
-    else:
-        outdatadir = "out"
-        rawdatadir = "raw"
-        cellpydatadir = "cellpyfiles"
-        filelogdir = "logs"
-        examplesdir = "examples"
-        db_path = "db"
-        db_filename = "cellpy_db.xlsx"
-        notebookdir = "notebooks"
-        batchfiledir = "batchfiles"
-        templatedir = "templates"
-        instrumentdir = "instruments"
-
-    outdatadir = h / outdatadir
-    rawdatadir = h / rawdatadir
-    cellpydatadir = h / cellpydatadir
-    filelogdir = h / filelogdir
-    examplesdir = h / examplesdir
-    db_path = h / db_path
-    notebookdir = h / notebookdir
-    batchfiledir = h / batchfiledir
-    templatedir = h / templatedir
-    instrumentdir = h / instrumentdir
-
-    if dry_run:
-        click.echo(f" - base (h): {h}")
-
-    if not silent:
-        outdatadir = _ask_about_path(
-            "where to output processed data and results", outdatadir
-        )
-        rawdatadir = _ask_about_otherpath("where your raw data are located", rawdatadir)
-        cellpydatadir = _ask_about_otherpath("where to put cellpy-files", cellpydatadir)
-        filelogdir = _ask_about_path("where to dump the log-files", filelogdir)
-        examplesdir = _ask_about_path(
-            "where to download cellpy examples and tests", examplesdir
-        )
-        db_path = _ask_about_path("what folder your db file lives in", db_path)
-        db_filename = _ask_about_name("the name of your db-file", db_filename)
-        notebookdir = _ask_about_path(
-            "where to put your jupyter notebooks", notebookdir
-        )
-        batchfiledir = _ask_about_path("where to put your batch files", batchfiledir)
-        templatedir = _ask_about_path("where to put your batch files", templatedir)
-        instrumentdir = _ask_about_path("where to put your batch files", instrumentdir)
-
-    # update folders based on suggestions
-    for d in [
-        outdatadir,
-        rawdatadir,
-        cellpydatadir,
-        filelogdir,
-        examplesdir,
-        notebookdir,
-        db_path,
-        batchfiledir,
-        templatedir,
-        instrumentdir,
-    ]:
-        if not dry_run:
-            _create_dir(d)
-        else:
-            click.echo(f"dry run (so I did not create {d})")
-
-    # update config-file based on suggestions
-    prmreader.prms.Paths.outdatadir = str(outdatadir)
-    prmreader.prms.Paths.rawdatadir = str(rawdatadir)
-    prmreader.prms.Paths.cellpydatadir = str(cellpydatadir)
-    prmreader.prms.Paths.filelogdir = str(filelogdir)
-    prmreader.prms.Paths.examplesdir = str(examplesdir)
-    prmreader.prms.Paths.db_path = str(db_path)
-    prmreader.prms.Paths.db_filename = str(db_filename)
-    prmreader.prms.Paths.notebookdir = str(notebookdir)
-    prmreader.prms.Paths.batchfiledir = str(batchfiledir)
-    prmreader.prms.Paths.templatedir = str(templatedir)
-    prmreader.prms.Paths.instrumentdir = str(instrumentdir)
-
-
-def _ask_about_path(q, p):
-    click.echo(f"\n[cellpy] (setup) input {q}")
-    click.echo(f"[cellpy] (setup) current: {p}")
-    new_path = input("[cellpy] (setup) [KEEP/new value] >>> ").strip()
-    if not new_path:
-        new_path = p
-    return pathlib.Path(new_path)
-
-
-def _ask_about_otherpath(q, p):
-    click.echo(f"\n[cellpy] (setup) input {q}")
-    click.echo(f"[cellpy] (setup) current: {p}")
-    new_path = input("[cellpy] (setup) [KEEP/new value] >>> ").strip()
-    if not new_path:
-        new_path = p
-    return OtherPath(new_path)
-
-
-def _ask_about_name(q, n):
-    click.echo(f"\n[cellpy] (setup) input {q}")
-    click.echo(f"[cellpy] (setup) current: {n}")
-    new_name = input("[cellpy] (setup) [KEEP/new value] >>> ").strip()
-    if not new_name:
-        new_name = n
-    return new_name
-
-
-def _create_dir(path, confirm=True, parents=True, exist_ok=True):
-    if isinstance(path, OtherPath):
-        if path.is_external:
-            return path
-    o = path.resolve()
-    if not o.is_dir():
-        o_parent = o.parent
-        create_dir = True
-        if confirm:
-            if not o_parent.is_dir():
-                create_dir = input(
-                    f"\n[cellpy] (setup) {o_parent} does not exist. Create it [y]/n ?"
-                )
-                if not create_dir:
-                    create_dir = True
-                elif create_dir in ["y", "Y"]:
-                    create_dir = True
-                else:
-                    create_dir = False
-
-        if create_dir:
-            try:
-                o.mkdir(parents=parents, exist_ok=exist_ok)
-                click.echo(f"[cellpy] (setup) Created {o}")
-            except FileExistsError:
-                click.echo(f"[cellpy] (setup) {o} already exists.")
-            except FileNotFoundError:
-                click.echo(f"[cellpy] (setup) {o} not available.")
-            except Exception as e:
-                click.echo(f"[cellpy] (setup) WARNING! Could not create {o}.")
-                logging.debug(e)
-                click.echo(f"[cellpy] (setup) ...continuing anyway.")
-        else:
-            click.echo(f"[cellpy] (setup) Could not create {o}")
-    return o
-
-
-def _check_import_cellpy():
-    try:
-        import cellpy
-        from cellpy import log
-        from cellpy.readers import cellreader
-
-        return True
-    except:
-        return False
-
-
-def _check_import_pyodbc():
-    import platform
-
-    from cellpy.parameters import prms
-
-    ODBC = prms._odbc
-    SEARCH_FOR_ODBC_DRIVERS = prms._search_for_odbc_driver
-
-    use_subprocess = prms.Instruments.Arbin.use_subprocess
-    detect_subprocess_need = prms.Instruments.Arbin.detect_subprocess_need
-    click.echo(f" reading prms")
-    click.echo(f" - ODBC: {ODBC}")
-    click.echo(f" - SEARCH_FOR_ODBC_DRIVERS: {SEARCH_FOR_ODBC_DRIVERS}")
-    click.echo(f" - use_subprocess: {use_subprocess}")
-    click.echo(f" - detect_subprocess_need: {detect_subprocess_need}")
-    click.echo(f" - stated office version: {prms.Instruments.Arbin.office_version}")
-
-    click.echo(" checking system")
-    is_posix = False
-    is_macos = False
-    if os.name == "posix":
-        is_posix = True
-        click.echo(f" - running on posix")
-    current_platform = platform.system()
-    if current_platform == "Darwin":
-        is_macos = True
-        click.echo(f" - running on a mac")
-
-    python_version, os_version = platform.architecture()
-    click.echo(f" - python version: {python_version}")
-    click.echo(f" - os version: {os_version}")
-
-    if not is_posix:
-        if not prms.Instruments.Arbin.sub_process_path:
-            sub_process_path = str(prms._sub_process_path)
-        else:
-            sub_process_path = str(prms.Instruments.Arbin.sub_process_path)
-        click.echo(f" stated path to sub-process: {sub_process_path}")
-        if not os.path.isfile(sub_process_path):
-            click.echo(f" - OBS! missing")
-
-    if is_posix:
-        click.echo(" checking existence of mdb-export")
-        sub_process_path = "mdb-export"
-        from subprocess import PIPE, run
-
-        command = ["command", "-v", sub_process_path]
-
-        try:
-            result = run(command, stdout=PIPE, stderr=PIPE, universal_newlines=True)
-            if result.returncode == 0:
-                click.echo(f" - found it: {result.stdout}")
-            else:
-                click.echo(f" - failed finding it")
-
-            if is_macos:
-                driver = "/usr/local/lib/libmdbodbc.dylib"
-                click.echo(f" looks like you are on a mac (driver set to\n {driver})")
-                if not os.path.isfile(driver):
-                    click.echo(" - but cannot find it!")
-                    return False
-            return True
-
-        except AssertionError:
-            click.echo(" - not found")
-            return False
-
-    # not posix - checking for odbc drivers
-    # 1) checking if you have defined one
-    try:
-        driver = prms.Instruments.Arbin.odbc_driver
-        if not driver:
-            raise AttributeError
-        click.echo("You have defined an odbc driver in your conifg file")
-        click.echo(f"driver: {driver}")
-    except AttributeError:
-        click.echo("FYI: you have not defined any odbc_driver(s)")
-        click.echo(
-            "(The name of the driver from the configuration file is "
-            "used as a backup when cellpy cannot locate a driver by itself)"
-        )
-
-    use_ado = False
-
-    if ODBC == "ado":
-        use_ado = True
-        click.echo(" you stated that you prefer the ado loader")
-        click.echo(" checking if adodbapi is installed")
-        try:
-            import adodbapi as dbloader
-        except ImportError:
-            use_ado = False
-            click.echo(" Failed! Try setting pyodbc as your loader or install")
-            click.echo(" adodbapi (http://adodbapi.sourceforge.net/)")
-
-    if not use_ado:
-        if ODBC == "pyodbc":
-            click.echo(" you stated that you prefer the pyodbc loader")
-            try:
-                import pyodbc as dbloader
-            except ImportError:
-                click.echo(" Failed! Could not import it.")
-                click.echo(" Try 'pip install pyodbc'")
-                dbloader = None
-
-        elif ODBC == "pypyodbc":
-            click.echo(" you stated that you prefer the pypyodbc loader")
-            try:
-                import pypyodbc as dbloader
-            except ImportError:
-                click.echo(" Failed! Could not import it.")
-                click.echo(" try 'pip install pypyodbc'")
-                click.echo(" or set pyodbc as your loader in your prm file")
-                click.echo(" (and install it)")
-                dbloader = None
-
-    click.echo(" searching for odbc drivers")
-    try:
-        drivers = [
-            driver
-            for driver in dbloader.drivers()
-            if "Microsoft Access Driver" in driver
-        ]
-        click.echo(f"Found these: {drivers}")
-        driver = drivers[0]
-        click.echo(f"odbc driver: {driver}")
-        return True
-
-    except IndexError as e:
-        logging.debug("Unfortunately, it seems the list of drivers is emtpy.")
-        click.echo(
-            "\nCould not find any odbc-drivers suitable for .res-type files. "
-            "Check out the homepage of pydobc for info on installing drivers"
-        )
-        click.echo(
-            "One solution that might work is downloading "
-            "the Microsoft Access database engine "
-            "(in correct bytes (32 or 64)) "
-            "from:\n"
-            "https://www.microsoft.com/en-us/download/details.aspx?id=13255"
-        )
-        click.echo("Or install mdbtools and set it up (check the cellpy docs for help)")
-        click.echo("\n")
-        return False
-
-
-def _check_config_file():
-    prm_file_name = _configloc()
-    prm_dict = prmreader._read_prm_file_without_updating(prm_file_name)
-    try:
-        prm_paths = prm_dict["Paths"]
-        required_dirs = [
-            "cellpydatadir",
-            "examplesdir",
-            "filelogdir",
-            "notebookdir",
-            "outdatadir",
-            "rawdatadir",
-            "batchfiledir",
-            "templatedir",
-            "db_path",
-        ]
-        missing = 0
-        for k in required_dirs:
-            value = prm_paths.get(k, None)
-            click.echo(f"{k}: {value}")
-            # splitting this into two if-statements to make it easier to debug if OtherPath changes
-            if k in OTHERPATHS:
-                print(
-                    f"skipping check for external {k} (for now)"
-                )
-                # if not OtherPath(
-                #     value
-                # ).is_dir():  # Assuming OtherPath returns True if it is external.
-                #     missing += 1
-                #     click.echo("COULD NOT CONNECT!")
-                #     click.echo(f"({value} is not a directory)")
-            elif value and not pathlib.Path(value).is_dir():
-                missing += 1
-                click.echo("COULD NOT CONNECT!")
-                click.echo(f"({value} is not a directory)")
-            if not value:
-                missing += 1
-                click.echo("MISSING")
-
-        value = prm_paths.get("db_filename", None)
-        click.echo(f"db_filename: {value}")
-        if not value:
-            missing += 1
-            click.echo("MISSING")
-
-        if missing:
-            return False
-        else:
-            return True
-
-    except Exception as e:
-        click.echo("Following error occurred:")
-        click.echo(e)
-        return False
-
-
-def _check(dry_run=False):
-    click.echo(" checking ".center(80, "="))
-    if dry_run:
-        click.echo("*** dry-run: skipping the test")
-        return
-    failed_checks = 0
-    number_of_checks = 0
-
-    def sub_check(check_type, check_func):
-        failed = 0
-        click.echo(f"[cellpy] * - Checking {check_type}")
-        if check_func():
-            click.echo(f"[cellpy] -> succeeded!")
-        else:
-            click.echo("f[cellpy] -> failed!!!!")
-            failed = 1
-        click.echo(80 * "-")
-        return failed
-
-    check_types = ["cellpy imports", "importing pyodbc", "configuration (prm) file"]
-    check_funcs = [_check_import_cellpy, _check_import_pyodbc, _check_config_file]
-
-    for ct, cf in zip(check_types, check_funcs):
-        try:
-            failed_checks += sub_check(ct, cf)
-        except Exception as e:
-            click.echo(f"[cellpy] check raised an exception ({e})")
-        number_of_checks += 1
-    succeeded_checks = number_of_checks - failed_checks
-    if failed_checks > 0:
-        click.echo(f"[cellpy] OH NO!!! You (or I) failed!")
-        click.echo(f"[cellpy] Failed {failed_checks} out of {number_of_checks} checks.")
-    else:
-        click.echo(
-            f"[cellpy] Succeeded {succeeded_checks} out of {number_of_checks} checks."
-        )
-    click.echo(80 * "=")
-
-
-def _write_config_file(user_dir, dst_file, init_filename, dry_run):
-    click.echo(" update configuration ".center(80, "-"))
-    click.echo("[cellpy] (setup) Writing configurations to user directory:")
-    click.echo(f"\n         {user_dir}\n")
-
-    if os.path.isfile(dst_file):
-        click.echo("[cellpy] (setup) File already exists!")
-        click.echo("[cellpy] (setup) Keeping most of the old configuration parameters")
-    try:
-        if dry_run:
-            click.echo(
-                f"*** dry-run: skipping actual saving of {dst_file} ***", color="red"
-            )
-        else:
-            click.echo(f"[cellpy] (setup) Saving file ({dst_file})")
-            save_prm_file(dst_file)
-
-    except ConfigFileNotWritten:
-        click.echo("[cellpy] (setup) Something went wrong! Could not write the file")
-        click.echo(
-            "[cellpy] (setup) Trying to write a file"
-            + f"called {prmreader.DEFAULT_FILENAME} instead"
-        )
-
-        try:
-            user_dir, dst_file = prmreader.get_user_dir_and_dst(init_filename)
-            if dry_run:
-                click.echo(
-                    f"*** dry-run: skipping actual saving of {dst_file} ***",
-                    color="red",
-                )
-            else:
-                save_prm_file(dst_file)
-
-        except ConfigFileNotWritten:
-            _txt = "[cellpy] (setup) No, that did not work either.\n"
-            _txt += "[cellpy] (setup) Well, guess you have to talk to the developers."
-            click.echo(_txt)
-    else:
-        click.echo(f"[cellpy] (setup) Configuration file written!")
-        click.echo(
-            f"[cellpy] (setup) OK! Now you can edit it. For example by "
-            f"issuing \n\n         [your-favourite-editor] {init_filename}\n"
-        )
-
-
-# ----------------------- edit ---------------------------------------
-@click.command()
-@click.option(
-    "--default-editor",
-    "-e",
-    default=None,
-    type=str,
-    help="try to use this editor instead (e.g. notepad.exe)",
-)
-def edit(default_editor):
-    """Edit your cellpy config file."""
-
-    config_file = _configloc()
-    if config_file:
-        config_file_str = str(config_file.resolve())
-
-        if default_editor is not None:
-            args = [default_editor, config_file_str]
-            click.echo(f"[cellpy] (edit) Calling '{default_editor}'")
-            try:
-                subprocess.call(args)
-            except:
-                click.echo(f"[cellpy] (edit) Failed!")
-                click.echo(
-                    "[cellpy] (edit) Try 'cellpy edit -e notepad.exe' if you are on Windows"
-                )
-
-        if default_editor is None:
-            try:
-                import editor
-
-                editor.edit(filename=config_file_str)
-            except ImportError:
-                click.echo(f"[cellpy] (edit) Failed!")
-                click.echo(
-                    f"[cellpy] (edit) Searching for editors uses the python-editor package"
-                )
-                click.echo(f"[cellpy] (edit) Possible fixes:")
-                click.echo(
-                    f"[cellpy] (edit) - provide a default editor "
-                    f"using the -e option (e.g. cellpy edit -e notepad.exe)"
-                )
-                click.echo(
-                    f"[cellpy] (edit) - install teh python-editor package "
-                    f"(pip install python-editor)"
-                )
-
-
-# ----------------------- info ---------------------------------------
-@click.command()
-@click.option("--version", "-v", is_flag=True, help="Print version information.")
-@click.option(
-    "--configloc", "-l", is_flag=True, help="Print full path to the config file."
-)
-@click.option("--params", "-p", is_flag=True, help="Dump all parameters to screen.")
-@click.option(
-    "--check",
-    "-c",
-    is_flag=True,
-    help="Do a sanity check to see if things" " works as they should.",
-)
-def info(version, configloc, params, check):
-    """This will give you some valuable information about your cellpy."""
-    complete_info = True
-
-    if check:
-        complete_info = False
-        _check()
-
-    if version:
-        complete_info = False
-        _version()
-
-    if configloc:
-        complete_info = False
-        _configloc()
-
-    if params:
-        complete_info = False
-        _dump_params()
-
-    if complete_info:
-        _version()
-        _configloc()
-
-
-# ----------------------- run ----------------------------------------
-@click.command()
-@click.option(
-    "--journal",
-    "-j",
-    is_flag=True,
-    help="Run a batch job defined in the given journal-file",
-)
-@click.option("--key", "-k", is_flag=True, help="Run a batch job defined by batch-name")
-@click.option(
-    "--folder",
-    "-f",
-    is_flag=True,
-    help="Run all batch jobs iteratively in a given folder",
-)
-@click.option(
-    "--cellpy-project",
-    "-p",
-    is_flag=True,
-    help="Use PaperMill to run the notebook(s) within the given project folder "
-    "(will only work properly if the notebooks can be sorted in correct run-order by 'sorted'). "
-    "Warning! since we are using `click` - the NAME will be 'converted' when it is loaded "
-    "(same as print(name) does) - "
-    "so you can't use backslash ('\\') as normal in windows (use either '/' or '\\\\' instead).",
-)
-@click.option("--debug", "-d", is_flag=True, help="Run in debug mode.")
-@click.option("--silent", "-s", is_flag=True, help="Run in silent mode.")
-@click.option("--raw", is_flag=True, help="Force loading raw-file(s).")
-@click.option("--cellpyfile", is_flag=True, help="Force cellpy-file(s).")
-@click.option("--minimal", is_flag=True, help="Minimal processing.")
-@click.option(
-    "--nom-cap",
-    default=None,
-    type=float,
-    help="nominal capacity (used in calculating rates etc)",
-)
-@click.option(
-    "--batch_col",
-    default=None,
-    type=str,
-    help="batch column (if selecting running from db)",
-)
-@click.option(
-    "--project",
-    default=None,
-    type=str,
-    help="name of the project (if selecting running from db)",
-)
-@click.option("--list", "-l", "list_", is_flag=True, help="List batch-files.")
-@click.argument("name", default="NONE")
-def run(
-    journal,
-    key,
-    folder,
-    cellpy_project,
-    debug,
-    silent,
-    raw,
-    cellpyfile,
-    minimal,
-    nom_cap,
-    batch_col,
-    project,
-    list_,
-    name,
-):
-    """Run a cellpy process (batch-job, edit db, ...).
-
-    You can use this to launch specific applications.
-
-    Examples:
-
-        edit your cellpy database
-
-           cellpy run db
-
-        run a batch job described in a journal file
-
-           cellpy run -j my_experiment.json
-
-    """
-    if list_:
-        _run_list(name)
-        return
-
-    if name == "NONE":
-        click.echo(
-            "Usage: cellpy run [OPTIONS] NAME\n"
-            "Try 'cellpy run --help' for help.\n\n"
-            "Error: Missing argument 'NAME'."
-        )
-        sys.exit(-1)
-
-    if debug:
-        click.echo("[cellpy] (run) debug mode on")
-
-    if silent:
-        click.echo("[cellpy] (run) silent mode on")
-
-    click.echo("[cellpy]\n")
-
-    if cellpy_project:
-        _run_project(name)
-
-    elif journal:
-        _run_journal(name, debug, silent, raw, cellpyfile, minimal, nom_cap)
-
-    elif folder:
-        _run_journals(name, debug, silent, raw, cellpyfile, minimal)
-
-    elif key:
-        _run_from_db(
-            name,
-            debug,
-            silent,
-            raw,
-            cellpyfile,
-            minimal,
-            nom_cap,
-            batch_col,
-            project,
-        )
-
-    elif name.lower() == "db":
-        _run_db(debug, silent)
-
-    else:
-        _run(name, debug, silent)
-
-
-def _run_from_db(
-    name,
-    debug,
-    silent,
-    raw,
-    cellpyfile,
-    minimal,
-    nom_cap,
-    batch_col,
-    project,
-):
-    click.echo(
-        f"running from db \nkey={name}, batch_col={batch_col}, project={project}"
-    )
-
-    kwargs = dict()
-    kwargs["name"] = name
-
-    if debug:
-        kwargs["default_log_level"] = "DEBUG"
-    if not minimal:
-        kwargs["export_raw"] = False
-        kwargs["export_cycles"] = False
-        kwargs["export_ica"] = False
-
-    if batch_col is not None:
-        kwargs["batch_col"] = batch_col
-    if project is None:
-        kwargs["project"] = "various"
-    else:
-        kwargs["project"] = project
-
-    click.echo("Warming up ...")
-
-    from cellpy.utils import batch
-
-    click.echo("  - starting batch processing")
-    b = batch.process_batch(
-        force_raw_file=raw,
-        force_cellpy=cellpyfile,
-        nom_cap=nom_cap,
-        backend="matplotlib",
-        **kwargs,
-    )
-
-    if b is not None and not silent:
-        print(b)
-    click.echo("---")
-
-
-def _run_journal(file_name, debug, silent, raw, cellpyfile, minimal, nom_cap):
-    click.echo(f"running journal {file_name}")
-    # click.echo(f" --debug [{debug}]")
-    # click.echo(f" --silent [{silent}]")
-    # click.echo(f" --raw [{raw}]")
-    # click.echo(f" --cellpyfile [{cellpyfile}]")
-    # click.echo(f" --minimal [{minimal}]")
-    # click.echo(f" --nom_cap [{nom_cap}] {type(nom_cap)}")
-
-    kwargs = dict()
-    if debug:
-        kwargs["default_log_level"] = "DEBUG"
-    if not minimal:
-        kwargs["export_raw"] = False
-        kwargs["export_cycles"] = False
-        kwargs["export_ica"] = False
-
-    from cellpy import prms
-    from cellpy.utils import batch
-
-    batchfiledir = pathlib.Path(prms.Paths.batchfiledir)
-    file = pathlib.Path(file_name)
-    if not file.is_file():
-        click.echo(f"file_name={file_name} not found - looking into batchfiledir")
-        if not batchfiledir.is_dir():
-            click.echo("batchfiledir not found - aborting")
-            return
-        file = batchfiledir / file.name
-
-    if not file.is_file():
-        click.echo(f"{file} not found - aborting")
-        return
-
-    b = batch.process_batch(
-        file,
-        force_raw_file=raw,
-        force_cellpy=cellpyfile,
-        nom_cap=nom_cap,
-        backend="matplotlib",
-        **kwargs,
-    )
-    if b is not None and not silent:
-        print(b)
-    click.echo("---")
-
-
-def _run_list(batchfiledir):
-    from cellpy import prms
-
-    if batchfiledir == "NONE" or batchfiledir is None:
-        batchfiledir = pathlib.Path(prms.Paths.batchfiledir)
-    else:
-        batchfiledir = pathlib.Path(batchfiledir).resolve()
-
-    if batchfiledir.is_dir():
-        click.echo(f"Content of '{batchfiledir}':\n")
-        i = 0
-        for i, f in enumerate(batchfiledir.glob("cellpy*.json")):
-            click.echo(f"{f.name}")
-        if i:
-            print(f"\nnumber of batch-files located: {i}")
-        else:
-            print("No batch-files found in this directory.")
-    else:
-        click.echo(f"{batchfiledir} not found.")
-
-
-def _run_journals(folder_name, debug, silent, raw, cellpyfile, minimal):
-    click.echo(f"running journals in {folder_name}")
-    # click.echo(f" --debug [{debug}]")
-    # click.echo(f" --silent [{silent}]")
-    # click.echo(f" --raw [{raw}]")
-    # click.echo(f" --cellpyfile [{cellpyfile}]")
-    # click.echo(f" --minimal [{minimal}]")
-
-    kwargs = dict()
-    if debug:
-        kwargs["default_log_level"] = "DEBUG"
-    if not minimal:
-        kwargs["export_raw"] = False
-        kwargs["export_cycles"] = False
-        kwargs["export_ica"] = False
-
-    from cellpy.utils import batch
-
-    folder_name = pathlib.Path(folder_name).resolve()
-
-    if not folder_name.is_dir():
-        click.echo(f"{folder_name} not found - aborting")
-        return
-
-    batch.iterate_batches(
-        folder_name, force_raw_file=raw, force_cellpy=cellpyfile, silent=True, **kwargs
-    )
-    click.echo("---")
-
-
-def _run_project(our_new_project, **kwargs):
-    try:
-        import papermill as pm
-    except ImportError:
-        click.echo(
-            "[cellpy]: You need to install papermill for automatically execute the notebooks."
-        )
-        click.echo("[cellpy]: You can install it using pip like this:")
-        click.echo(" >> pip install papermill")
-        return
-    our_new_project = pathlib.Path(our_new_project)
-    click.echo(f"[cellpy]: trying to run notebooks in {our_new_project}")
-    notebooks = sorted(list(our_new_project.glob("*.ipynb")))
-    for notebook in notebooks:
-        click.echo(f"[cellpy - papermill] running {notebook.name}")
-        pm.execute_notebook(notebook, notebook, parameters=kwargs)
-
-
-def _run(name, debug, silent):
-    click.echo(f"running {name}")
-    click.echo(f" --debug [{debug}]")
-    click.echo(f" --silent [{silent}]")
-
-
-def _run_db(debug, silent):
-    import platform
-
-    from cellpy import prms
-
-    if not silent:
-        click.echo(f"running database editor")
-    if debug:
-        click.echo("running in debug-mode, but nothing to tell")
-
-    db_path = Path(prms.Paths.db_path) / prms.Paths.db_filename
-
-    if platform.system() == "Windows":
-        try:
-            os.system(f'start excel "{str(db_path)}"')
-        except Exception as e:
-            click.echo("Something went wrong trying to open")
-            click.echo(db_path)
-            print()
-            print(e)
-
-    elif platform.system() == "Linux":
-        click.echo("RUNNING LINUX")
-        # not tested
-        subprocess.check_call(["open", "-a", "Microsoft Excel", db_path])
-
-    elif platform.system() == "Darwin":
-        click.echo(f" - running on a mac")
-        subprocess.check_call(["open", "-a", "Microsoft Excel", db_path])
-
-    else:
-        print("RUNNING SOMETHING ELSE")
-        print(platform.system())
-        # not tested
-        subprocess.check_call(["open", "-a", "Microsoft Excel", db_path])
-
-
-# ----------------------- pull ---------------------------------------
-@click.command()
-@click.option("--tests", "-t", is_flag=True, help="Download test-files from repo.")
-@click.option(
-    "--examples", "-e", is_flag=True, help="Download example-files from repo."
-)
-@click.option("--clone", "-c", is_flag=True, help="Clone the full repo.")
-@click.option("--directory", "-d", default=None, help="Save into custom directory DIR")
-@click.option("--password", "-p", default=None, help="Password option for the repo")
-def pull(tests, examples, clone, directory, password):
-    """Download examples or tests from the big internet (needs git)."""
-    if directory is not None:
-        click.echo(f"[cellpy] (pull) custom directory: {directory}")
-    else:
-        directory = pathlib.Path(prmreader.prms.Paths.examplesdir)
-
-    if password is not None:
-        click.echo("DEV MODE: password provided")
-    if clone:
-        _clone_repo(directory, password)
-    else:
-        if tests:
-            _pull_tests(directory, password)
-        if examples:
-            _pull_examples(directory, password)
-        else:
-            click.echo(
-                f"[cellpy] (pull) Nothing selected for pulling. "
-                f"Please select an option (--tests,--examples, -clone, ...) "
-            )
-
-
-def _clone_repo(directory, password):
-    directory = pathlib.Path(directory)
-    txt = "[cellpy] The plan is that this "
-    txt += "[cellpy] cmd will pull (clone) the cellpy repo.\n"
-    txt += "[cellpy] For now it only prints the link to the git-hub\n"
-    txt += "[cellpy] repository:\n"
-    txt += "[cellpy]\n"
-    txt += "[cellpy] https://github.com/jepegit/cellpy.git\n"
-    txt += "[cellpy]\n"
-    click.echo(txt)
-
-
-def _pull_tests(directory, pw=None):
-    txt = (
-        "[cellpy] (pull) Pulling tests from",
-        " https://github.com/jepegit/cellpy.git",
-    )
-    click.echo(txt)
-    _pull(gdirpath="tests", rootpath=directory, pw=pw)
-    _pull(gdirpath="testdata", rootpath=directory, pw=pw)
-
-
-def _pull_examples(directory, pw):
-    txt = (
-        "[cellpy] (pull) Pulling examples from",
-        " https://github.com/jepegit/cellpy.git",
-    )
-    click.echo(txt)
-    _pull(gdirpath="examples", rootpath=directory, pw=pw)
-
-
-def _version():
-    txt = "[cellpy] version: " + str(VERSION)
-    click.echo(txt)
-
-
-def _configloc():
-    _, config_file_name = prmreader.get_user_dir_and_dst()
-    click.echo("[cellpy] ->%s" % config_file_name)
-    if not os.path.isfile(config_file_name):
-        click.echo("[cellpy] File does not exist!")
-    else:
-        return config_file_name
-
-
-def _dump_params():
-    click.echo("[cellpy] Dumping parameters to screen:\n")
-    prmreader.info()
-
-
-def _download_g_blob(name, local_path):
-    import urllib.request
-
-    dirs = local_path.parent
-    if not dirs.is_dir():
-        click.echo(f"[cellpy] (pull) creating dir: {dirs}")
-        dirs.mkdir(parents=True)
-
-    filename, headers = urllib.request.urlretrieve(
-        name.download_url, filename=local_path
-    )
-    click.echo(f"[cellpy] (pull) downloaded blob: {filename}")
-
-
-def _parse_g_dir(repo, gdirpath):
-    """parses a repo directory two-levels deep"""
-    for f in repo.get_contents(gdirpath):
-        if f.type == "dir":
-            for sf in repo.get_contents(f.path):
-                yield sf
-        else:
-            yield f
-
-
-def _get_user_name():
-    return "jepegit"
-
-
-def _get_pw(method):
-    if method == "ask":
-        return getpass.getpass()
-    elif method == "env":
-        return os.environ.get(GITHUB_PWD_VAR_NAME, None)
-
-    else:
-        return None
-
-
-def _pull(gdirpath="examples", rootpath=None, u=None, pw=None):
-    if rootpath is None:
-        rootpath = prmreader.prms.Paths.examplesdir
-
-    rootpath = pathlib.Path(rootpath)
-
-    ndirpath = rootpath / gdirpath
-
-    if pw is not None:
-        click.echo(" DEV MODE ".center(80, "-"))
-        u = _get_user_name()
-        if pw == "ask":
-            click.echo("   - ask for password")
-            pw = _get_pw(pw)
-        elif pw == "env":
-            click.echo("   - check environ for password ")
-            pw = _get_pw(pw)
-            click.echo("   - got something")
-            if pw is None:
-                click.echo("   - only None")
-                u = None
-
-    g = Github(u, pw)
-    repo = g.get_repo(REPO)
-
-    click.echo(f"[cellpy] (pull) pulling {gdirpath}")
-    click.echo(f"[cellpy] (pull) -> {ndirpath}")
-
-    if not ndirpath.is_dir():
-        click.echo(f"[cellpy] (pull) creating dir: {ndirpath}")
-        ndirpath.mkdir(parents=True)
-
-    for gfile in _parse_g_dir(repo, gdirpath):
-        gfilename = pathlib.Path(gfile.path)
-        nfilename = rootpath / gfilename
-
-        _download_g_blob(gfile, nfilename)
-
-
-def _get_default_template():
-    template = "standard"
-    try:
-        template = prmreader.prms.Batch.template
-    except:
-        logging.debug("You dont have any default template defined in you .conf file")
-    return template
-
-
-def _read_local_templates(local_templates_path=None):
-    if local_templates_path is None:
-        local_templates_path = pathlib.Path(prmreader.prms.Paths.templatedir)
-    templates = {}
-    for p in list(local_templates_path.rglob("cellpy_cookie*.zip")):
-        label = p.stem.strip()[len("cellpy_cookie_") :]
-        templates[label] = (str(p), None)
-    logging.debug(f"Found the following templates: {templates}")
-    return templates
-
-
-# ----------------------- new ----------------------------------------
-@click.command()
-@click.option("--template", "-t", help="Provide template name.")
-@click.option("--directory", "-d", default=None, help="Create in custom directory.")
-@click.option(
-    "--project",
-    "-p",
-    default=None,
-    help="Provide project name (i.e. sub-directory name).",
-)
-@click.option(
-    "--experiment",
-    "-e",
-    default=None,
-    help="Provide experiment name (i.e. lookup-value).",
-)
-@click.option(
-    "--local-user-template",
-    "-u",
-    is_flag=True,
-    default=False,
-    help="Use local template from the templates directory.",
-)
-@click.option("--serve", "-s", "serve_", is_flag=True, help="Run Jupyter.")
-@click.option(
-    "--run",
-    "-r",
-    "run_",
-    is_flag=True,
-    help="Use PaperMill to run the notebook(s) from the template "
-    "(will only work properly if the notebooks can be sorted in correct run-order by 'sorted'.",
-)
-@click.option(
-    "--lab",
-    "-j",
-    is_flag=True,
-    help="Use Jupyter Lab instead of Notebook when serving.",
-)
-@click.option(
-    "--list", "-l", "list_", is_flag=True, help="List available templates and exit."
-)
-def new(
-    template,
-    directory,
-    project,
-    experiment,
-    local_user_template,
-    serve_,
-    run_,
-    lab,
-    list_,
-):
-    """Set up a batch experiment (might need git installed)."""
-    _new(
-        template,
-        directory=directory,
-        project_dir=project,
-        session_id=experiment,
-        local_user_template=local_user_template,
-        serve_=serve_,
-        run_=run_,
-        lab=lab,
-        list_=list_,
-    )
-
-
-def _new(
-    template: str,
-    directory: Union[Path, str, None] = None,
-    project_dir: Union[str, None] = None,
-    local_user_template: bool = False,
-    serve_: bool = False,
-    run_: bool = False,
-    lab: bool = False,
-    list_: bool = False,
-    session_id: str = "experiment_001",
-    no_input: bool = False,
-    cookie_directory: str = "",
-):
-    """Set up a batch experiment (might need git installed).
-
-    Args:
-        template: short-name of template.
-        directory: the directory for your cellpy projects.
-        local_user_template: use local template if True.
-        serve_: serve the notebook after creation if True.
-        run_: run the notebooks using papermill if True.
-        lab: use jupyter-lab instead of jupyter notebook if True.
-        list_: list all available templates and return if True.
-        project_dir: your project directory.
-        session_id: the lookup value.
-        no_input: accept defaults if True (only valid when providing project_dir and session_id)
-        cookie_directory: name of the directory for your cookie (inside the repository or zip file).
-    Returns:
-        None
-    """
-
-    from cellpy.parameters import prms
-
-    if list_:
-        click.echo(f"\n[cellpy] batch templates")
-
-        default_template = _get_default_template()
-        local_templates = _read_local_templates()
-        local_templates_path = prmreader.prms.Paths.templatedir
-        registered_templates = prms._registered_templates
-        click.echo(f"[cellpy] - default: {default_template}")
-        click.echo("[cellpy] - registered templates (on github):")
-        for label, link in registered_templates.items():
-            click.echo(f"\t\t{label:18s} {link}")
-
-        if local_templates:
-            click.echo(f"[cellpy] - local templates ({local_templates_path}):")
-            for label, link in local_templates.items():
-                click.echo(f"\t\t{label:18s} {link}")
-        else:
-            click.echo(f"[cellpy] - local templates ({local_templates_path}): none")
-
-        return
-
-    if project_dir is None or session_id is None:
-        no_input = False
-
-    if not template:
-        template = _get_default_template()
-
-    if lab:
-        server = "lab"
-    else:
-        server = "notebook"
-
-    try:
-        import cookiecutter.exceptions
-        import cookiecutter.main
-        import cookiecutter.prompt
-
-    except ModuleNotFoundError:
-        click.echo("Could not import cookiecutter.")
-        click.echo("Try installing it, for example by writing:")
-        click.echo("\npip install cookiecutter\n")
-
-    click.echo(f"Template: {template}")
-    if local_user_template:
-        # forcing using local template
-        templates = _read_local_templates()
-
-        if not templates:
-            click.echo(
-                "You asked me to use a local template, but you have none. Aborting."
-            )
-            return
-    else:
-        templates = prms._registered_templates
-        if local_templates := _read_local_templates():
-            templates.update(local_templates)
-
-    if not template.lower() in templates.keys():
-        click.echo("This template does not exist. Aborting.")
-        return
-
-    if directory is None:
-        logging.debug("no dir given")
-        directory = prms.Paths.notebookdir
-
-    if not os.path.isdir(directory):
-        click.echo("Sorry. This did not work as expected!")
-        click.echo(f" - {directory} does not exist")
-        return
-
-    directory = Path(directory)
-    selected_project_dir = None
-
-    if project_dir:
-        selected_project_dir = directory / project_dir
-        if not selected_project_dir.is_dir():
-            if cookiecutter.prompt.read_user_yes_no(
-                f"{project_dir} does not exist. Create?", "yes"
-            ):
-                os.mkdir(selected_project_dir)
-                click.echo(f"Created {selected_project_dir}")
-
-            else:
-                selected_project_dir = None
-                click.echo(f"Select another directory instead")
-
-    if not selected_project_dir:
-        project_dirs = [
-            d.name
-            for d in directory.iterdir()
-            if d.is_dir() and not d.name.startswith(".")
-        ]
-        project_dirs.insert(0, "[create new dir]")
-
-        project_dir = cookiecutter.prompt.read_user_choice(
-            "project folder", project_dirs
-        )
-
-        if project_dir == "[create new dir]":
-            default_name = "cellpy_project"
-            temp_default_name = default_name
-            for j in range(999):
-                if temp_default_name in project_dirs:
-                    temp_default_name = default_name + str(j + 1).zfill(3)
-                else:
-                    default_name = temp_default_name
-                    break
-
-            project_dir = cookiecutter.prompt.read_user_variable(
-                "New name", default_name
-            )
-            try:
-                os.mkdir(directory / project_dir)
-                click.echo(f"created {project_dir}")
-            except FileExistsError:
-                click.echo("OK - but this directory already exists!")
-        selected_project_dir = directory / project_dir
-
-    # get a list of all folders
-    existing_projects = os.listdir(selected_project_dir)
-
-    os.chdir(selected_project_dir)
-    cellpy_version = cellpy.__version__
-
-    try:
-        selected_template, cookie_dir = templates[template.lower()]
-
-        if cookie_directory:
-            cookie_dir = cookie_directory
-        if not cookie_dir:
-            cookie_dir = template.lower()
-
-        cookiecutter.main.cookiecutter(
-            selected_template,
-            extra_context={
-                "author_name": os.getlogin(),
-                "project_name": project_dir,
-                "cellpy_version": cellpy_version,
-                "session_id": session_id,
-            },
-            no_input=no_input,
-            directory=cookie_dir,
-        )
-    except cookiecutter.exceptions.OutputDirExistsException as e:
-        click.echo("Sorry. This did not work as expected!")
-        click.echo(" - cookiecutter refused to create the project")
-        click.echo(e)
-
-    if serve_:
-        os.chdir(directory)
-        _serve(server)
-
-    if run_:
-        try:
-            import papermill as pm
-        except ImportError:
-            click.echo(
-                "[cellpy]: You need to install papermill for automatically execute the notebooks."
-            )
-            click.echo("[cellpy]: You can install it using pip like this:")
-            click.echo(" >> pip install papermill")
-            return
-        new_existing_projects = os.listdir(selected_project_dir)
-        our_new_projects = list(set(new_existing_projects) - set(existing_projects))
-
-        if not len(our_new_projects):
-            click.echo(
-                "[cellpy]: Sorry, could not deiced what is the new project "
-                "- so I don't dare to try to execute automatically."
-            )
-            return
-        our_new_project = selected_project_dir / our_new_projects[0]
-
-        _run_project(our_new_project)
-
-
-def _serve(server):
-    click.echo(f"serving with jupyter {server}")
-    subprocess.run(["jupyter", server], check=True)
-    click.echo("Finished serving.")
-
-
-# ----------------------- serve ---------------------------------------
-@click.command()
-@click.option("--lab", "-l", is_flag=True, help="Use Jupyter Lab instead of Notebook")
-@click.option("--directory", "-d", default=None, help="Start in custom directory DIR")
-def serve(lab, directory):
-    """Start a Jupyter server."""
-
-    from cellpy.parameters import prms
-
-    if directory is None:
-        directory = prms.Paths.notebookdir
-    elif directory == "home":
-        directory = Path().home()
-    elif directory == "here":
-        directory = Path(os.getcwd())
-
-    if not os.path.isdir(directory):
-        click.echo("Sorry. This did not work as expected!")
-        click.echo(f" - {directory} does not exist")
-        return
-
-    if lab:
-        server = "lab"
-    else:
-        server = "notebook"
-
-    os.chdir(directory)
-    _serve(server)
-
-
-cli.add_command(setup)
-cli.add_command(info)
-cli.add_command(edit)
-cli.add_command(pull)
-cli.add_command(run)
-cli.add_command(new)
-cli.add_command(serve)
-
-
-# tests etc
-def _main_pull():
-    if sys.platform == "win32":
-        rootpath = pathlib.Path(r"C:\Temp\cellpy_user")
-    else:
-        rootpath = pathlib.Path("/Users/jepe/scripting/tmp/cellpy_test_user")
-    _pull_examples(rootpath, pw="env")
-    _pull_tests(rootpath, pw="env")
-    # _pull(gdirpath="examples", rootpath=rootpath, u="ask", pw="ask")
-    # _pull(gdirpath="tests", rootpath=rootpath, u="ask", pw="ask")
-    # _pull(gdirpath="testdata", rootpath=rootpath, u="ask", pw="ask")
-
-
-def _main():
-    file_name = prmreader.create_custom_init_filename()
-    click.echo(file_name)
-    user_directory, destination_file_name = prmreader.get_user_dir_and_dst(file_name)
-    click.echo(user_directory)
-    click.echo(destination_file_name)
-    click.echo("trying to save it")
-    save_prm_file(destination_file_name + "_dummy")
-
-    click.echo(" Testing setup ".center(80, "="))
-    setup(["--interactive", "--reset"])
-
-
-def _cli_setup_interactive():
-    from click.testing import CliRunner
-
-    if sys.platform == "win32":
-        root_dir = r"C:\Temp\cellpy_user"
-    else:
-        root_dir = "/Users/jepe/scripting/tmp/cellpy_test_user"
-    testuser = "tester"
-    init_filename = prmreader.create_custom_init_filename(testuser)
-    dst_file = get_dst_file(root_dir, init_filename)
-    init_file = pathlib.Path(dst_file)
-    opts = list()
-    opts.append("setup")
-    opts.append("-i")
-    # opts.append("-nr")
-    opts.append("-r")
-    opts.extend(["-d", root_dir])
-    opts.extend(["-t", testuser])
-
-    input_str = "\n"  # out
-    input_str += "\n"  # rawdatadir
-    input_str += "\n"  # cellpyfiles
-    input_str += "\n"  # log
-    input_str += "\n"  # examples
-    input_str += "\n"  # dbfolder
-    input_str += "\n"  # dbfile
-    runner = CliRunner()
-    result = runner.invoke(cli, opts, input=input_str)
-
-    click.echo(" out ".center(80, "."))
-    click.echo(result.output)
-    from pprint import pprint
-
-    pprint(prmreader.prms.Paths)
-    click.echo(" conf-file ".center(80, "."))
-    click.echo(init_file)
-    click.echo()
-    with init_file.open() as f:
-        for line in f.readlines():
-            click.echo(line.strip())
-
-
-def check_it(var=None):
-    import pathlib
-    import sys
-
-    p_env = pathlib.Path(sys.prefix)
-    print(p_env.name)
-    new(list_=True)
-
-
-if __name__ == "__main__":
-    u1 = os.getlogin()
-    u2 = os.path.expanduser("~")
-    u3 = os.environ.get("USERNAME")
-
-    print(u1)
-    print(u2)
-    print(u3)
-    # check_it()
-    # click.echo("\n\n", " RUNNING MAIN PULL ".center(80, "*"), "\n")
-    # _main_pull()
-    # click.echo("ok")
+import base64
+import getpass
+import logging
+import os
+import pathlib
+from pprint import pprint
+import re
+import subprocess
+import sys
+from typing import Union
+import urllib
+from pathlib import Path
+
+import click
+import pkg_resources
+from github import Github
+
+import cellpy._version
+from cellpy.exceptions import ConfigFileNotWritten
+from cellpy.parameters import prmreader
+from cellpy.parameters.internal_settings import OTHERPATHS
+from cellpy.internals.core import OtherPath
+
+VERSION = cellpy._version.__version__
+REPO = "jepegit/cellpy"
+USER = "jepegit"
+GITHUB_PWD_VAR_NAME = "GD_PWD"
+
+
+def save_prm_file(prm_filename):
+    """saves (writes) the prms to file"""
+    prmreader._write_prm_file(prm_filename)
+
+
+def get_package_prm_dir():
+    """gets the folder where the cellpy package lives"""
+    prm_dir = pkg_resources.resource_filename("cellpy", "parameters")
+    return pathlib.Path(prm_dir)
+
+
+def get_default_config_file_path(init_filename=None):
+    """gets the path to the default config-file"""
+    prm_dir = get_package_prm_dir()
+    if not init_filename:
+        init_filename = prmreader.DEFAULT_FILENAME
+    src = prm_dir / init_filename
+    return src
+
+
+def get_dst_file(user_dir, init_filename):
+    user_dir = pathlib.Path(user_dir)
+    dst_file = user_dir / init_filename
+    return dst_file
+
+
+def check_if_needed_modules_exists():
+    pass
+
+
+def modify_config_file():
+    pass
+
+
+def create_cellpy_folders():
+    pass
+
+
+@click.group("cellpy")
+def cli():
+    pass
+
+
+# ----------------------- setup --------------------------------------
+@click.command()
+@click.option(
+    "--interactive",
+    "-i",
+    is_flag=True,
+    default=False,
+    help="Allows you to specify div. folders and setting.",
+)
+@click.option(
+    "--not-relative",
+    "-nr",
+    is_flag=True,
+    default=False,
+    help="If root-dir is given, put it directly in the root (/) folder"
+    " i.e. don't put it in your home directory. Defaults to False. Remark"
+    " that if you specifically write a path name instead of selecting the"
+    " suggested default, the path you write will be used as is.",
+)
+@click.option(
+    "--dry-run",
+    "-dr",
+    is_flag=True,
+    default=False,
+    help="Run setup in dry mode (only print - do not execute). This is"
+    " typically used when developing and testing cellpy. Defaults to"
+    " False.",
+)
+@click.option(
+    "--reset",
+    "-r",
+    is_flag=True,
+    default=False,
+    help="Do not suggest path defaults based on your current configuration-file",
+)
+@click.option(
+    "--root-dir",
+    "-d",
+    default=None,
+    type=click.Path(),
+    help="Use custom root dir. If not given, your home directory"
+    " will be used as the top level where cellpy-folders"
+    " will be put. The folder path must follow"
+    " directly after this option (if used). Example:\n"
+    " $ cellpy setup -d 'MyDir'",
+)
+@click.option(
+    "--folder-name",
+    "-n",
+    default=None,
+    type=click.Path(),
+    help="",
+)
+@click.option(
+    "--test_user", "-t", default=None, help="Fake name for fake user (for testing)"
+)
+def setup(interactive, not_relative, dry_run, reset, root_dir, folder_name, test_user):
+    """This will help you to set up cellpy."""
+
+    click.echo("[cellpy] (setup)")
+    click.echo(f"[cellpy] root-dir: {root_dir}")
+
+    # generate variables
+    init_filename = prmreader.create_custom_init_filename()
+    user_dir, dst_file = prmreader.get_user_dir_and_dst(init_filename)
+
+    if dry_run:
+        click.echo("Create custom init filename and get user_dir and destination")
+        click.echo(f"Got the following parameters:")
+        click.echo(f" - init_filename: {init_filename}")
+        click.echo(f" - user_dir: {user_dir}")
+        click.echo(f" - dst_file: {dst_file}")
+        click.echo(f" - not_relative: {not_relative}")
+
+    if root_dir and not interactive:
+        click.echo("[cellpy] custom root-dir can only be used in interactive mode")
+        click.echo("[cellpy] -> setting interactive mode")
+        interactive = True
+
+    if not root_dir:
+        root_dir = user_dir
+        # root_dir = pathlib.Path(os.getcwd())
+    root_dir = pathlib.Path(root_dir)
+
+    if dry_run:
+        click.echo(f" - root_dir: {root_dir}")
+
+    if test_user:
+        click.echo(f"[cellpy] (setup) DEV-MODE test_user: {test_user}")
+        init_filename = prmreader.create_custom_init_filename(test_user)
+        user_dir = root_dir
+        dst_file = get_dst_file(user_dir, init_filename)
+        click.echo(f"[cellpy] (setup) DEV-MODE user_dir: {user_dir}")
+        click.echo(f"[cellpy] (setup) DEV-MODE dst_file: {dst_file}")
+
+    if not pathlib.Path(dst_file).is_file():
+        click.echo(f"[cellpy] {dst_file} not found -> I will make one for you!")
+        reset = True
+
+    if interactive:
+        click.echo(" interactive mode ".center(80, "-"))
+        _update_paths(
+            custom_dir=root_dir,
+            relative_home=not not_relative,
+            default_dir=folder_name,
+            dry_run=dry_run,
+            reset=reset,
+        )
+        _write_config_file(user_dir, dst_file, init_filename, dry_run)
+        _check(dry_run=dry_run)
+
+    else:
+        if reset:
+            _update_paths(
+                user_dir,
+                False,
+                default_dir=folder_name,
+                dry_run=dry_run,
+                reset=True,
+                silent=True,
+            )
+        _write_config_file(user_dir, dst_file, init_filename, dry_run)
+        _check(dry_run=dry_run)
+
+
+def _update_paths(
+    custom_dir=None,
+    relative_home=True,
+    reset=False,
+    dry_run=False,
+    default_dir=None,
+    silent=False,
+):
+    # please, refactor me :-(
+
+    h = prmreader.get_user_dir()
+
+    if default_dir is None:
+        default_dir = "cellpy_data"
+
+    if dry_run:
+        click.echo(f" - default_dir: {default_dir}")
+        click.echo(f" - custom_dir: {custom_dir}")
+        click.echo(f" - retalive_home: {relative_home}")
+
+    if custom_dir:
+        reset = True
+        if relative_home:
+            h = h / custom_dir
+        if not custom_dir.parts[-1] == default_dir:
+            h = h / default_dir
+
+    if not reset:
+        outdatadir = pathlib.Path(prmreader.prms.Paths.outdatadir)
+        rawdatadir = OtherPath(prmreader.prms.Paths.rawdatadir)
+        cellpydatadir = OtherPath(prmreader.prms.Paths.cellpydatadir)
+        filelogdir = pathlib.Path(prmreader.prms.Paths.filelogdir)
+        examplesdir = pathlib.Path(prmreader.prms.Paths.examplesdir)
+        db_path = pathlib.Path(prmreader.prms.Paths.db_path)
+        db_filename = prmreader.prms.Paths.db_filename
+        notebookdir = pathlib.Path(prmreader.prms.Paths.notebookdir)
+        batchfiledir = pathlib.Path(prmreader.prms.Paths.batchfiledir)
+        templatedir = pathlib.Path(prmreader.prms.Paths.templatedir)
+        instrumentdir = pathlib.Path(prmreader.prms.Paths.instrumentsdir)
+    else:
+        outdatadir = "out"
+        rawdatadir = "raw"
+        cellpydatadir = "cellpyfiles"
+        filelogdir = "logs"
+        examplesdir = "examples"
+        db_path = "db"
+        db_filename = "cellpy_db.xlsx"
+        notebookdir = "notebooks"
+        batchfiledir = "batchfiles"
+        templatedir = "templates"
+        instrumentdir = "instruments"
+
+    outdatadir = h / outdatadir
+    rawdatadir = h / rawdatadir
+    cellpydatadir = h / cellpydatadir
+    filelogdir = h / filelogdir
+    examplesdir = h / examplesdir
+    db_path = h / db_path
+    notebookdir = h / notebookdir
+    batchfiledir = h / batchfiledir
+    templatedir = h / templatedir
+    instrumentdir = h / instrumentdir
+
+    if dry_run:
+        click.echo(f" - base (h): {h}")
+
+    if not silent:
+        outdatadir = _ask_about_path(
+            "where to output processed data and results", outdatadir
+        )
+        rawdatadir = _ask_about_otherpath("where your raw data are located", rawdatadir)
+        cellpydatadir = _ask_about_otherpath("where to put cellpy-files", cellpydatadir)
+        filelogdir = _ask_about_path("where to dump the log-files", filelogdir)
+        examplesdir = _ask_about_path(
+            "where to download cellpy examples and tests", examplesdir
+        )
+        db_path = _ask_about_path("what folder your db file lives in", db_path)
+        db_filename = _ask_about_name("the name of your db-file", db_filename)
+        notebookdir = _ask_about_path(
+            "where to put your jupyter notebooks", notebookdir
+        )
+        batchfiledir = _ask_about_path("where to put your batch files", batchfiledir)
+        templatedir = _ask_about_path("where to put your batch files", templatedir)
+        instrumentdir = _ask_about_path("where to put your batch files", instrumentdir)
+
+    # update folders based on suggestions
+    for d in [
+        outdatadir,
+        rawdatadir,
+        cellpydatadir,
+        filelogdir,
+        examplesdir,
+        notebookdir,
+        db_path,
+        batchfiledir,
+        templatedir,
+        instrumentdir,
+    ]:
+        if not dry_run:
+            _create_dir(d)
+        else:
+            click.echo(f"dry run (so I did not create {d})")
+
+    # update config-file based on suggestions
+    prmreader.prms.Paths.outdatadir = str(outdatadir)
+    prmreader.prms.Paths.rawdatadir = str(rawdatadir)
+    prmreader.prms.Paths.cellpydatadir = str(cellpydatadir)
+    prmreader.prms.Paths.filelogdir = str(filelogdir)
+    prmreader.prms.Paths.examplesdir = str(examplesdir)
+    prmreader.prms.Paths.db_path = str(db_path)
+    prmreader.prms.Paths.db_filename = str(db_filename)
+    prmreader.prms.Paths.notebookdir = str(notebookdir)
+    prmreader.prms.Paths.batchfiledir = str(batchfiledir)
+    prmreader.prms.Paths.templatedir = str(templatedir)
+    prmreader.prms.Paths.instrumentdir = str(instrumentdir)
+
+
+def _ask_about_path(q, p):
+    click.echo(f"\n[cellpy] (setup) input {q}")
+    click.echo(f"[cellpy] (setup) current: {p}")
+    new_path = input("[cellpy] (setup) [KEEP/new value] >>> ").strip()
+    if not new_path:
+        new_path = p
+    return pathlib.Path(new_path)
+
+
+def _ask_about_otherpath(q, p):
+    click.echo(f"\n[cellpy] (setup) input {q}")
+    click.echo(f"[cellpy] (setup) current: {p}")
+    new_path = input("[cellpy] (setup) [KEEP/new value] >>> ").strip()
+    if not new_path:
+        new_path = p
+    return OtherPath(new_path)
+
+
+def _ask_about_name(q, n):
+    click.echo(f"\n[cellpy] (setup) input {q}")
+    click.echo(f"[cellpy] (setup) current: {n}")
+    new_name = input("[cellpy] (setup) [KEEP/new value] >>> ").strip()
+    if not new_name:
+        new_name = n
+    return new_name
+
+
+def _create_dir(path, confirm=True, parents=True, exist_ok=True):
+    if isinstance(path, OtherPath):
+        if path.is_external:
+            return path
+    o = path.resolve()
+    if not o.is_dir():
+        o_parent = o.parent
+        create_dir = True
+        if confirm:
+            if not o_parent.is_dir():
+                create_dir = input(
+                    f"\n[cellpy] (setup) {o_parent} does not exist. Create it [y]/n ?"
+                )
+                if not create_dir:
+                    create_dir = True
+                elif create_dir in ["y", "Y"]:
+                    create_dir = True
+                else:
+                    create_dir = False
+
+        if create_dir:
+            try:
+                o.mkdir(parents=parents, exist_ok=exist_ok)
+                click.echo(f"[cellpy] (setup) Created {o}")
+            except FileExistsError:
+                click.echo(f"[cellpy] (setup) {o} already exists.")
+            except FileNotFoundError:
+                click.echo(f"[cellpy] (setup) {o} not available.")
+            except Exception as e:
+                click.echo(f"[cellpy] (setup) WARNING! Could not create {o}.")
+                logging.debug(e)
+                click.echo(f"[cellpy] (setup) ...continuing anyway.")
+        else:
+            click.echo(f"[cellpy] (setup) Could not create {o}")
+    return o
+
+
+def _check_import_cellpy():
+    try:
+        import cellpy
+        from cellpy import log
+        from cellpy.readers import cellreader
+
+        return True
+    except:
+        return False
+
+
+def _check_import_pyodbc():
+    import platform
+
+    from cellpy.parameters import prms
+
+    ODBC = prms._odbc
+    SEARCH_FOR_ODBC_DRIVERS = prms._search_for_odbc_driver
+
+    use_subprocess = prms.Instruments.Arbin.use_subprocess
+    detect_subprocess_need = prms.Instruments.Arbin.detect_subprocess_need
+    click.echo(f" reading prms")
+    click.echo(f" - ODBC: {ODBC}")
+    click.echo(f" - SEARCH_FOR_ODBC_DRIVERS: {SEARCH_FOR_ODBC_DRIVERS}")
+    click.echo(f" - use_subprocess: {use_subprocess}")
+    click.echo(f" - detect_subprocess_need: {detect_subprocess_need}")
+    click.echo(f" - stated office version: {prms.Instruments.Arbin.office_version}")
+
+    click.echo(" checking system")
+    is_posix = False
+    is_macos = False
+    if os.name == "posix":
+        is_posix = True
+        click.echo(f" - running on posix")
+    current_platform = platform.system()
+    if current_platform == "Darwin":
+        is_macos = True
+        click.echo(f" - running on a mac")
+
+    python_version, os_version = platform.architecture()
+    click.echo(f" - python version: {python_version}")
+    click.echo(f" - os version: {os_version}")
+
+    if not is_posix:
+        if not prms.Instruments.Arbin.sub_process_path:
+            sub_process_path = str(prms._sub_process_path)
+        else:
+            sub_process_path = str(prms.Instruments.Arbin.sub_process_path)
+        click.echo(f" stated path to sub-process: {sub_process_path}")
+        if not os.path.isfile(sub_process_path):
+            click.echo(f" - OBS! missing")
+
+    if is_posix:
+        click.echo(" checking existence of mdb-export")
+        sub_process_path = "mdb-export"
+        from subprocess import PIPE, run
+
+        command = ["command", "-v", sub_process_path]
+
+        try:
+            result = run(command, stdout=PIPE, stderr=PIPE, universal_newlines=True)
+            if result.returncode == 0:
+                click.echo(f" - found it: {result.stdout}")
+            else:
+                click.echo(f" - failed finding it")
+
+            if is_macos:
+                driver = "/usr/local/lib/libmdbodbc.dylib"
+                click.echo(f" looks like you are on a mac (driver set to\n {driver})")
+                if not os.path.isfile(driver):
+                    click.echo(" - but cannot find it!")
+                    return False
+            return True
+
+        except AssertionError:
+            click.echo(" - not found")
+            return False
+
+    # not posix - checking for odbc drivers
+    # 1) checking if you have defined one
+    try:
+        driver = prms.Instruments.Arbin.odbc_driver
+        if not driver:
+            raise AttributeError
+        click.echo("You have defined an odbc driver in your conifg file")
+        click.echo(f"driver: {driver}")
+    except AttributeError:
+        click.echo("FYI: you have not defined any odbc_driver(s)")
+        click.echo(
+            "(The name of the driver from the configuration file is "
+            "used as a backup when cellpy cannot locate a driver by itself)"
+        )
+
+    use_ado = False
+
+    if ODBC == "ado":
+        use_ado = True
+        click.echo(" you stated that you prefer the ado loader")
+        click.echo(" checking if adodbapi is installed")
+        try:
+            import adodbapi as dbloader
+        except ImportError:
+            use_ado = False
+            click.echo(" Failed! Try setting pyodbc as your loader or install")
+            click.echo(" adodbapi (http://adodbapi.sourceforge.net/)")
+
+    if not use_ado:
+        if ODBC == "pyodbc":
+            click.echo(" you stated that you prefer the pyodbc loader")
+            try:
+                import pyodbc as dbloader
+            except ImportError:
+                click.echo(" Failed! Could not import it.")
+                click.echo(" Try 'pip install pyodbc'")
+                dbloader = None
+
+        elif ODBC == "pypyodbc":
+            click.echo(" you stated that you prefer the pypyodbc loader")
+            try:
+                import pypyodbc as dbloader
+            except ImportError:
+                click.echo(" Failed! Could not import it.")
+                click.echo(" try 'pip install pypyodbc'")
+                click.echo(" or set pyodbc as your loader in your prm file")
+                click.echo(" (and install it)")
+                dbloader = None
+
+    click.echo(" searching for odbc drivers")
+    try:
+        drivers = [
+            driver
+            for driver in dbloader.drivers()
+            if "Microsoft Access Driver" in driver
+        ]
+        click.echo(f"Found these: {drivers}")
+        driver = drivers[0]
+        click.echo(f"odbc driver: {driver}")
+        return True
+
+    except IndexError as e:
+        logging.debug("Unfortunately, it seems the list of drivers is emtpy.")
+        click.echo(
+            "\nCould not find any odbc-drivers suitable for .res-type files. "
+            "Check out the homepage of pydobc for info on installing drivers"
+        )
+        click.echo(
+            "One solution that might work is downloading "
+            "the Microsoft Access database engine "
+            "(in correct bytes (32 or 64)) "
+            "from:\n"
+            "https://www.microsoft.com/en-us/download/details.aspx?id=13255"
+        )
+        click.echo("Or install mdbtools and set it up (check the cellpy docs for help)")
+        click.echo("\n")
+        return False
+
+
+def _check_config_file():
+    prm_file_name = _configloc()
+    prm_dict = prmreader._read_prm_file_without_updating(prm_file_name)
+    try:
+        prm_paths = prm_dict["Paths"]
+        required_dirs = [
+            "cellpydatadir",
+            "examplesdir",
+            "filelogdir",
+            "notebookdir",
+            "outdatadir",
+            "rawdatadir",
+            "batchfiledir",
+            "templatedir",
+            "db_path",
+        ]
+        missing = 0
+        for k in required_dirs:
+            value = prm_paths.get(k, None)
+            click.echo(f"{k}: {value}")
+            # splitting this into two if-statements to make it easier to debug if OtherPath changes
+            if k in OTHERPATHS:
+                print(f"skipping check for external {k} (for now)")
+                # if not OtherPath(
+                #     value
+                # ).is_dir():  # Assuming OtherPath returns True if it is external.
+                #     missing += 1
+                #     click.echo("COULD NOT CONNECT!")
+                #     click.echo(f"({value} is not a directory)")
+            elif value and not pathlib.Path(value).is_dir():
+                missing += 1
+                click.echo("COULD NOT CONNECT!")
+                click.echo(f"({value} is not a directory)")
+            if not value:
+                missing += 1
+                click.echo("MISSING")
+
+        value = prm_paths.get("db_filename", None)
+        click.echo(f"db_filename: {value}")
+        if not value:
+            missing += 1
+            click.echo("MISSING")
+
+        if missing:
+            return False
+        else:
+            return True
+
+    except Exception as e:
+        click.echo("Following error occurred:")
+        click.echo(e)
+        return False
+
+
+def _check(dry_run=False):
+    click.echo(" checking ".center(80, "="))
+    if dry_run:
+        click.echo("*** dry-run: skipping the test")
+        return
+    failed_checks = 0
+    number_of_checks = 0
+
+    def sub_check(check_type, check_func):
+        failed = 0
+        click.echo(f"[cellpy] * - Checking {check_type}")
+        if check_func():
+            click.echo(f"[cellpy] -> succeeded!")
+        else:
+            click.echo("f[cellpy] -> failed!!!!")
+            failed = 1
+        click.echo(80 * "-")
+        return failed
+
+    check_types = ["cellpy imports", "importing pyodbc", "configuration (prm) file"]
+    check_funcs = [_check_import_cellpy, _check_import_pyodbc, _check_config_file]
+
+    for ct, cf in zip(check_types, check_funcs):
+        try:
+            failed_checks += sub_check(ct, cf)
+        except Exception as e:
+            click.echo(f"[cellpy] check raised an exception ({e})")
+        number_of_checks += 1
+    succeeded_checks = number_of_checks - failed_checks
+    if failed_checks > 0:
+        click.echo(f"[cellpy] OH NO!!! You (or I) failed!")
+        click.echo(f"[cellpy] Failed {failed_checks} out of {number_of_checks} checks.")
+    else:
+        click.echo(
+            f"[cellpy] Succeeded {succeeded_checks} out of {number_of_checks} checks."
+        )
+    click.echo(80 * "=")
+
+
+def _write_config_file(user_dir, dst_file, init_filename, dry_run):
+    click.echo(" update configuration ".center(80, "-"))
+    click.echo("[cellpy] (setup) Writing configurations to user directory:")
+    click.echo(f"\n         {user_dir}\n")
+
+    if os.path.isfile(dst_file):
+        click.echo("[cellpy] (setup) File already exists!")
+        click.echo("[cellpy] (setup) Keeping most of the old configuration parameters")
+    try:
+        if dry_run:
+            click.echo(
+                f"*** dry-run: skipping actual saving of {dst_file} ***", color="red"
+            )
+        else:
+            click.echo(f"[cellpy] (setup) Saving file ({dst_file})")
+            save_prm_file(dst_file)
+
+    except ConfigFileNotWritten:
+        click.echo("[cellpy] (setup) Something went wrong! Could not write the file")
+        click.echo(
+            "[cellpy] (setup) Trying to write a file"
+            + f"called {prmreader.DEFAULT_FILENAME} instead"
+        )
+
+        try:
+            user_dir, dst_file = prmreader.get_user_dir_and_dst(init_filename)
+            if dry_run:
+                click.echo(
+                    f"*** dry-run: skipping actual saving of {dst_file} ***",
+                    color="red",
+                )
+            else:
+                save_prm_file(dst_file)
+
+        except ConfigFileNotWritten:
+            _txt = "[cellpy] (setup) No, that did not work either.\n"
+            _txt += "[cellpy] (setup) Well, guess you have to talk to the developers."
+            click.echo(_txt)
+    else:
+        click.echo(f"[cellpy] (setup) Configuration file written!")
+        click.echo(
+            f"[cellpy] (setup) OK! Now you can edit it. For example by "
+            f"issuing \n\n         [your-favourite-editor] {init_filename}\n"
+        )
+
+
+# ----------------------- edit ---------------------------------------
+@click.command()
+@click.option(
+    "--default-editor",
+    "-e",
+    default=None,
+    type=str,
+    help="try to use this editor instead (e.g. notepad.exe)",
+)
+def edit(default_editor):
+    """Edit your cellpy config file."""
+
+    config_file = _configloc()
+    if config_file:
+        config_file_str = str(config_file.resolve())
+
+        if default_editor is not None:
+            args = [default_editor, config_file_str]
+            click.echo(f"[cellpy] (edit) Calling '{default_editor}'")
+            try:
+                subprocess.call(args)
+            except:
+                click.echo(f"[cellpy] (edit) Failed!")
+                click.echo(
+                    "[cellpy] (edit) Try 'cellpy edit -e notepad.exe' if you are on Windows"
+                )
+
+        if default_editor is None:
+            try:
+                import editor
+
+                editor.edit(filename=config_file_str)
+            except ImportError:
+                click.echo(f"[cellpy] (edit) Failed!")
+                click.echo(
+                    f"[cellpy] (edit) Searching for editors uses the python-editor package"
+                )
+                click.echo(f"[cellpy] (edit) Possible fixes:")
+                click.echo(
+                    f"[cellpy] (edit) - provide a default editor "
+                    f"using the -e option (e.g. cellpy edit -e notepad.exe)"
+                )
+                click.echo(
+                    f"[cellpy] (edit) - install teh python-editor package "
+                    f"(pip install python-editor)"
+                )
+
+
+# ----------------------- info ---------------------------------------
+@click.command()
+@click.option("--version", "-v", is_flag=True, help="Print version information.")
+@click.option(
+    "--configloc", "-l", is_flag=True, help="Print full path to the config file."
+)
+@click.option("--params", "-p", is_flag=True, help="Dump all parameters to screen.")
+@click.option(
+    "--check",
+    "-c",
+    is_flag=True,
+    help="Do a sanity check to see if things" " works as they should.",
+)
+def info(version, configloc, params, check):
+    """This will give you some valuable information about your cellpy."""
+    complete_info = True
+
+    if check:
+        complete_info = False
+        _check()
+
+    if version:
+        complete_info = False
+        _version()
+
+    if configloc:
+        complete_info = False
+        _configloc()
+
+    if params:
+        complete_info = False
+        _dump_params()
+
+    if complete_info:
+        _version()
+        _configloc()
+
+
+# ----------------------- run ----------------------------------------
+@click.command()
+@click.option(
+    "--journal",
+    "-j",
+    is_flag=True,
+    help="Run a batch job defined in the given journal-file",
+)
+@click.option("--key", "-k", is_flag=True, help="Run a batch job defined by batch-name")
+@click.option(
+    "--folder",
+    "-f",
+    is_flag=True,
+    help="Run all batch jobs iteratively in a given folder",
+)
+@click.option(
+    "--cellpy-project",
+    "-p",
+    is_flag=True,
+    help="Use PaperMill to run the notebook(s) within the given project folder "
+    "(will only work properly if the notebooks can be sorted in correct run-order by 'sorted'). "
+    "Warning! since we are using `click` - the NAME will be 'converted' when it is loaded "
+    "(same as print(name) does) - "
+    "so you can't use backslash ('\\') as normal in windows (use either '/' or '\\\\' instead).",
+)
+@click.option("--debug", "-d", is_flag=True, help="Run in debug mode.")
+@click.option("--silent", "-s", is_flag=True, help="Run in silent mode.")
+@click.option("--raw", is_flag=True, help="Force loading raw-file(s).")
+@click.option("--cellpyfile", is_flag=True, help="Force cellpy-file(s).")
+@click.option("--minimal", is_flag=True, help="Minimal processing.")
+@click.option(
+    "--nom-cap",
+    default=None,
+    type=float,
+    help="nominal capacity (used in calculating rates etc)",
+)
+@click.option(
+    "--batch_col",
+    default=None,
+    type=str,
+    help="batch column (if selecting running from db)",
+)
+@click.option(
+    "--project",
+    default=None,
+    type=str,
+    help="name of the project (if selecting running from db)",
+)
+@click.option("--list", "-l", "list_", is_flag=True, help="List batch-files.")
+@click.argument("name", default="NONE")
+def run(
+    journal,
+    key,
+    folder,
+    cellpy_project,
+    debug,
+    silent,
+    raw,
+    cellpyfile,
+    minimal,
+    nom_cap,
+    batch_col,
+    project,
+    list_,
+    name,
+):
+    """Run a cellpy process (batch-job, edit db, ...).
+
+    You can use this to launch specific applications.
+
+    Examples:
+
+        edit your cellpy database
+
+           cellpy run db
+
+        run a batch job described in a journal file
+
+           cellpy run -j my_experiment.json
+
+    """
+    if list_:
+        _run_list(name)
+        return
+
+    if name == "NONE":
+        click.echo(
+            "Usage: cellpy run [OPTIONS] NAME\n"
+            "Try 'cellpy run --help' for help.\n\n"
+            "Error: Missing argument 'NAME'."
+        )
+        sys.exit(-1)
+
+    if debug:
+        click.echo("[cellpy] (run) debug mode on")
+
+    if silent:
+        click.echo("[cellpy] (run) silent mode on")
+
+    click.echo("[cellpy]\n")
+
+    if cellpy_project:
+        _run_project(name)
+
+    elif journal:
+        _run_journal(name, debug, silent, raw, cellpyfile, minimal, nom_cap)
+
+    elif folder:
+        _run_journals(name, debug, silent, raw, cellpyfile, minimal)
+
+    elif key:
+        _run_from_db(
+            name,
+            debug,
+            silent,
+            raw,
+            cellpyfile,
+            minimal,
+            nom_cap,
+            batch_col,
+            project,
+        )
+
+    elif name.lower() == "db":
+        _run_db(debug, silent)
+
+    else:
+        _run(name, debug, silent)
+
+
+def _run_from_db(
+    name,
+    debug,
+    silent,
+    raw,
+    cellpyfile,
+    minimal,
+    nom_cap,
+    batch_col,
+    project,
+):
+    click.echo(
+        f"running from db \nkey={name}, batch_col={batch_col}, project={project}"
+    )
+
+    kwargs = dict()
+    kwargs["name"] = name
+
+    if debug:
+        kwargs["default_log_level"] = "DEBUG"
+    if not minimal:
+        kwargs["export_raw"] = False
+        kwargs["export_cycles"] = False
+        kwargs["export_ica"] = False
+
+    if batch_col is not None:
+        kwargs["batch_col"] = batch_col
+    if project is None:
+        kwargs["project"] = "various"
+    else:
+        kwargs["project"] = project
+
+    click.echo("Warming up ...")
+
+    from cellpy.utils import batch
+
+    click.echo("  - starting batch processing")
+    b = batch.process_batch(
+        force_raw_file=raw,
+        force_cellpy=cellpyfile,
+        nom_cap=nom_cap,
+        backend="matplotlib",
+        **kwargs,
+    )
+
+    if b is not None and not silent:
+        print(b)
+    click.echo("---")
+
+
+def _run_journal(file_name, debug, silent, raw, cellpyfile, minimal, nom_cap):
+    click.echo(f"running journal {file_name}")
+    # click.echo(f" --debug [{debug}]")
+    # click.echo(f" --silent [{silent}]")
+    # click.echo(f" --raw [{raw}]")
+    # click.echo(f" --cellpyfile [{cellpyfile}]")
+    # click.echo(f" --minimal [{minimal}]")
+    # click.echo(f" --nom_cap [{nom_cap}] {type(nom_cap)}")
+
+    kwargs = dict()
+    if debug:
+        kwargs["default_log_level"] = "DEBUG"
+    if not minimal:
+        kwargs["export_raw"] = False
+        kwargs["export_cycles"] = False
+        kwargs["export_ica"] = False
+
+    from cellpy import prms
+    from cellpy.utils import batch
+
+    batchfiledir = pathlib.Path(prms.Paths.batchfiledir)
+    file = pathlib.Path(file_name)
+    if not file.is_file():
+        click.echo(f"file_name={file_name} not found - looking into batchfiledir")
+        if not batchfiledir.is_dir():
+            click.echo("batchfiledir not found - aborting")
+            return
+        file = batchfiledir / file.name
+
+    if not file.is_file():
+        click.echo(f"{file} not found - aborting")
+        return
+
+    b = batch.process_batch(
+        file,
+        force_raw_file=raw,
+        force_cellpy=cellpyfile,
+        nom_cap=nom_cap,
+        backend="matplotlib",
+        **kwargs,
+    )
+    if b is not None and not silent:
+        print(b)
+    click.echo("---")
+
+
+def _run_list(batchfiledir):
+    from cellpy import prms
+
+    if batchfiledir == "NONE" or batchfiledir is None:
+        batchfiledir = pathlib.Path(prms.Paths.batchfiledir)
+    else:
+        batchfiledir = pathlib.Path(batchfiledir).resolve()
+
+    if batchfiledir.is_dir():
+        click.echo(f"Content of '{batchfiledir}':\n")
+        i = 0
+        for i, f in enumerate(batchfiledir.glob("cellpy*.json")):
+            click.echo(f"{f.name}")
+        if i:
+            print(f"\nnumber of batch-files located: {i}")
+        else:
+            print("No batch-files found in this directory.")
+    else:
+        click.echo(f"{batchfiledir} not found.")
+
+
+def _run_journals(folder_name, debug, silent, raw, cellpyfile, minimal):
+    click.echo(f"running journals in {folder_name}")
+    # click.echo(f" --debug [{debug}]")
+    # click.echo(f" --silent [{silent}]")
+    # click.echo(f" --raw [{raw}]")
+    # click.echo(f" --cellpyfile [{cellpyfile}]")
+    # click.echo(f" --minimal [{minimal}]")
+
+    kwargs = dict()
+    if debug:
+        kwargs["default_log_level"] = "DEBUG"
+    if not minimal:
+        kwargs["export_raw"] = False
+        kwargs["export_cycles"] = False
+        kwargs["export_ica"] = False
+
+    from cellpy.utils import batch
+
+    folder_name = pathlib.Path(folder_name).resolve()
+
+    if not folder_name.is_dir():
+        click.echo(f"{folder_name} not found - aborting")
+        return
+
+    batch.iterate_batches(
+        folder_name, force_raw_file=raw, force_cellpy=cellpyfile, silent=True, **kwargs
+    )
+    click.echo("---")
+
+
+def _run_project(our_new_project, **kwargs):
+    try:
+        import papermill as pm
+    except ImportError:
+        click.echo(
+            "[cellpy]: You need to install papermill for automatically execute the notebooks."
+        )
+        click.echo("[cellpy]: You can install it using pip like this:")
+        click.echo(" >> pip install papermill")
+        return
+    our_new_project = pathlib.Path(our_new_project)
+    click.echo(f"[cellpy]: trying to run notebooks in {our_new_project}")
+    notebooks = sorted(list(our_new_project.glob("*.ipynb")))
+    for notebook in notebooks:
+        click.echo(f"[cellpy - papermill] running {notebook.name}")
+        pm.execute_notebook(notebook, notebook, parameters=kwargs)
+
+
+def _run(name, debug, silent):
+    click.echo(f"running {name}")
+    click.echo(f" --debug [{debug}]")
+    click.echo(f" --silent [{silent}]")
+
+
+def _run_db(debug, silent):
+    import platform
+
+    from cellpy import prms
+
+    if not silent:
+        click.echo(f"running database editor")
+    if debug:
+        click.echo("running in debug-mode, but nothing to tell")
+
+    db_path = Path(prms.Paths.db_path) / prms.Paths.db_filename
+
+    if platform.system() == "Windows":
+        try:
+            os.system(f'start excel "{str(db_path)}"')
+        except Exception as e:
+            click.echo("Something went wrong trying to open")
+            click.echo(db_path)
+            print()
+            print(e)
+
+    elif platform.system() == "Linux":
+        click.echo("RUNNING LINUX")
+        # not tested
+        subprocess.check_call(["open", "-a", "Microsoft Excel", db_path])
+
+    elif platform.system() == "Darwin":
+        click.echo(f" - running on a mac")
+        subprocess.check_call(["open", "-a", "Microsoft Excel", db_path])
+
+    else:
+        print("RUNNING SOMETHING ELSE")
+        print(platform.system())
+        # not tested
+        subprocess.check_call(["open", "-a", "Microsoft Excel", db_path])
+
+
+# ----------------------- pull ---------------------------------------
+@click.command()
+@click.option("--tests", "-t", is_flag=True, help="Download test-files from repo.")
+@click.option(
+    "--examples", "-e", is_flag=True, help="Download example-files from repo."
+)
+@click.option("--clone", "-c", is_flag=True, help="Clone the full repo.")
+@click.option("--directory", "-d", default=None, help="Save into custom directory DIR")
+@click.option("--password", "-p", default=None, help="Password option for the repo")
+def pull(tests, examples, clone, directory, password):
+    """Download examples or tests from the big internet (needs git)."""
+    if directory is not None:
+        click.echo(f"[cellpy] (pull) custom directory: {directory}")
+    else:
+        directory = pathlib.Path(prmreader.prms.Paths.examplesdir)
+
+    if password is not None:
+        click.echo("DEV MODE: password provided")
+    if clone:
+        _clone_repo(directory, password)
+    else:
+        if tests:
+            _pull_tests(directory, password)
+        if examples:
+            _pull_examples(directory, password)
+        else:
+            click.echo(
+                f"[cellpy] (pull) Nothing selected for pulling. "
+                f"Please select an option (--tests,--examples, -clone, ...) "
+            )
+
+
+def _clone_repo(directory, password):
+    directory = pathlib.Path(directory)
+    txt = "[cellpy] The plan is that this "
+    txt += "[cellpy] cmd will pull (clone) the cellpy repo.\n"
+    txt += "[cellpy] For now it only prints the link to the git-hub\n"
+    txt += "[cellpy] repository:\n"
+    txt += "[cellpy]\n"
+    txt += "[cellpy] https://github.com/jepegit/cellpy.git\n"
+    txt += "[cellpy]\n"
+    click.echo(txt)
+
+
+def _pull_tests(directory, pw=None):
+    txt = (
+        "[cellpy] (pull) Pulling tests from",
+        " https://github.com/jepegit/cellpy.git",
+    )
+    click.echo(txt)
+    _pull(gdirpath="tests", rootpath=directory, pw=pw)
+    _pull(gdirpath="testdata", rootpath=directory, pw=pw)
+
+
+def _pull_examples(directory, pw):
+    txt = (
+        "[cellpy] (pull) Pulling examples from",
+        " https://github.com/jepegit/cellpy.git",
+    )
+    click.echo(txt)
+    _pull(gdirpath="examples", rootpath=directory, pw=pw)
+
+
+def _version():
+    txt = "[cellpy] version: " + str(VERSION)
+    click.echo(txt)
+
+
+def _configloc():
+    _, config_file_name = prmreader.get_user_dir_and_dst()
+    click.echo("[cellpy] ->%s" % config_file_name)
+    if not os.path.isfile(config_file_name):
+        click.echo("[cellpy] File does not exist!")
+    else:
+        return config_file_name
+
+
+def _dump_params():
+    click.echo("[cellpy] Dumping parameters to screen:\n")
+    prmreader.info()
+
+
+def _download_g_blob(name, local_path):
+    import urllib.request
+
+    dirs = local_path.parent
+    if not dirs.is_dir():
+        click.echo(f"[cellpy] (pull) creating dir: {dirs}")
+        dirs.mkdir(parents=True)
+
+    filename, headers = urllib.request.urlretrieve(
+        name.download_url, filename=local_path
+    )
+    click.echo(f"[cellpy] (pull) downloaded blob: {filename}")
+
+
+def _parse_g_dir(repo, gdirpath):
+    """parses a repo directory two-levels deep"""
+    for f in repo.get_contents(gdirpath):
+        if f.type == "dir":
+            for sf in repo.get_contents(f.path):
+                yield sf
+        else:
+            yield f
+
+
+def _get_user_name():
+    return "jepegit"
+
+
+def _get_pw(method):
+    if method == "ask":
+        return getpass.getpass()
+    elif method == "env":
+        return os.environ.get(GITHUB_PWD_VAR_NAME, None)
+
+    else:
+        return None
+
+
+def _pull(gdirpath="examples", rootpath=None, u=None, pw=None):
+    if rootpath is None:
+        rootpath = prmreader.prms.Paths.examplesdir
+
+    rootpath = pathlib.Path(rootpath)
+
+    ndirpath = rootpath / gdirpath
+
+    if pw is not None:
+        click.echo(" DEV MODE ".center(80, "-"))
+        u = _get_user_name()
+        if pw == "ask":
+            click.echo("   - ask for password")
+            pw = _get_pw(pw)
+        elif pw == "env":
+            click.echo("   - check environ for password ")
+            pw = _get_pw(pw)
+            click.echo("   - got something")
+            if pw is None:
+                click.echo("   - only None")
+                u = None
+
+    g = Github(u, pw)
+    repo = g.get_repo(REPO)
+
+    click.echo(f"[cellpy] (pull) pulling {gdirpath}")
+    click.echo(f"[cellpy] (pull) -> {ndirpath}")
+
+    if not ndirpath.is_dir():
+        click.echo(f"[cellpy] (pull) creating dir: {ndirpath}")
+        ndirpath.mkdir(parents=True)
+
+    for gfile in _parse_g_dir(repo, gdirpath):
+        gfilename = pathlib.Path(gfile.path)
+        nfilename = rootpath / gfilename
+
+        _download_g_blob(gfile, nfilename)
+
+
+def _get_default_template():
+    template = "standard"
+    try:
+        template = prmreader.prms.Batch.template
+    except:
+        logging.debug("You dont have any default template defined in you .conf file")
+    return template
+
+
+def _read_local_templates(local_templates_path=None):
+    if local_templates_path is None:
+        local_templates_path = pathlib.Path(prmreader.prms.Paths.templatedir)
+    templates = {}
+    for p in list(local_templates_path.rglob("cellpy_cookie*.zip")):
+        label = p.stem.strip()[len("cellpy_cookie_") :]
+        templates[label] = (str(p), None)
+    logging.debug(f"Found the following templates: {templates}")
+    return templates
+
+
+# ----------------------- new ----------------------------------------
+@click.command()
+@click.option("--template", "-t", help="Provide template name.")
+@click.option("--directory", "-d", default=None, help="Create in custom directory.")
+@click.option(
+    "--project",
+    "-p",
+    default=None,
+    help="Provide project name (i.e. sub-directory name).",
+)
+@click.option(
+    "--experiment",
+    "-e",
+    default=None,
+    help="Provide experiment name (i.e. lookup-value).",
+)
+@click.option(
+    "--local-user-template",
+    "-u",
+    is_flag=True,
+    default=False,
+    help="Use local template from the templates directory.",
+)
+@click.option("--serve", "-s", "serve_", is_flag=True, help="Run Jupyter.")
+@click.option(
+    "--run",
+    "-r",
+    "run_",
+    is_flag=True,
+    help="Use PaperMill to run the notebook(s) from the template "
+    "(will only work properly if the notebooks can be sorted in correct run-order by 'sorted'.",
+)
+@click.option(
+    "--lab",
+    "-j",
+    is_flag=True,
+    help="Use Jupyter Lab instead of Notebook when serving.",
+)
+@click.option(
+    "--list", "-l", "list_", is_flag=True, help="List available templates and exit."
+)
+def new(
+    template,
+    directory,
+    project,
+    experiment,
+    local_user_template,
+    serve_,
+    run_,
+    lab,
+    list_,
+):
+    """Set up a batch experiment (might need git installed)."""
+    _new(
+        template,
+        directory=directory,
+        project_dir=project,
+        session_id=experiment,
+        local_user_template=local_user_template,
+        serve_=serve_,
+        run_=run_,
+        lab=lab,
+        list_=list_,
+    )
+
+
+def _new(
+    template: str,
+    directory: Union[Path, str, None] = None,
+    project_dir: Union[str, None] = None,
+    local_user_template: bool = False,
+    serve_: bool = False,
+    run_: bool = False,
+    lab: bool = False,
+    list_: bool = False,
+    session_id: str = "experiment_001",
+    no_input: bool = False,
+    cookie_directory: str = "",
+):
+    """Set up a batch experiment (might need git installed).
+
+    Args:
+        template: short-name of template.
+        directory: the directory for your cellpy projects.
+        local_user_template: use local template if True.
+        serve_: serve the notebook after creation if True.
+        run_: run the notebooks using papermill if True.
+        lab: use jupyter-lab instead of jupyter notebook if True.
+        list_: list all available templates and return if True.
+        project_dir: your project directory.
+        session_id: the lookup value.
+        no_input: accept defaults if True (only valid when providing project_dir and session_id)
+        cookie_directory: name of the directory for your cookie (inside the repository or zip file).
+    Returns:
+        None
+    """
+
+    from cellpy.parameters import prms
+
+    if list_:
+        click.echo(f"\n[cellpy] batch templates")
+
+        default_template = _get_default_template()
+        local_templates = _read_local_templates()
+        local_templates_path = prmreader.prms.Paths.templatedir
+        registered_templates = prms._registered_templates
+        click.echo(f"[cellpy] - default: {default_template}")
+        click.echo("[cellpy] - registered templates (on github):")
+        for label, link in registered_templates.items():
+            click.echo(f"\t\t{label:18s} {link}")
+
+        if local_templates:
+            click.echo(f"[cellpy] - local templates ({local_templates_path}):")
+            for label, link in local_templates.items():
+                click.echo(f"\t\t{label:18s} {link}")
+        else:
+            click.echo(f"[cellpy] - local templates ({local_templates_path}): none")
+
+        return
+
+    if project_dir is None or session_id is None:
+        no_input = False
+
+    if not template:
+        template = _get_default_template()
+
+    if lab:
+        server = "lab"
+    else:
+        server = "notebook"
+
+    try:
+        import cookiecutter.exceptions
+        import cookiecutter.main
+        import cookiecutter.prompt
+
+    except ModuleNotFoundError:
+        click.echo("Could not import cookiecutter.")
+        click.echo("Try installing it, for example by writing:")
+        click.echo("\npip install cookiecutter\n")
+
+    click.echo(f"Template: {template}")
+    if local_user_template:
+        # forcing using local template
+        templates = _read_local_templates()
+
+        if not templates:
+            click.echo(
+                "You asked me to use a local template, but you have none. Aborting."
+            )
+            return
+    else:
+        templates = prms._registered_templates
+        if local_templates := _read_local_templates():
+            templates.update(local_templates)
+
+    if not template.lower() in templates.keys():
+        click.echo("This template does not exist. Aborting.")
+        return
+
+    if directory is None:
+        logging.debug("no dir given")
+        directory = prms.Paths.notebookdir
+
+    if not os.path.isdir(directory):
+        click.echo("Sorry. This did not work as expected!")
+        click.echo(f" - {directory} does not exist")
+        return
+
+    directory = Path(directory)
+    selected_project_dir = None
+
+    if project_dir:
+        selected_project_dir = directory / project_dir
+        if not selected_project_dir.is_dir():
+            if cookiecutter.prompt.read_user_yes_no(
+                f"{project_dir} does not exist. Create?", "yes"
+            ):
+                os.mkdir(selected_project_dir)
+                click.echo(f"Created {selected_project_dir}")
+
+            else:
+                selected_project_dir = None
+                click.echo(f"Select another directory instead")
+
+    if not selected_project_dir:
+        project_dirs = [
+            d.name
+            for d in directory.iterdir()
+            if d.is_dir() and not d.name.startswith(".")
+        ]
+        project_dirs.insert(0, "[create new dir]")
+
+        project_dir = cookiecutter.prompt.read_user_choice(
+            "project folder", project_dirs
+        )
+
+        if project_dir == "[create new dir]":
+            default_name = "cellpy_project"
+            temp_default_name = default_name
+            for j in range(999):
+                if temp_default_name in project_dirs:
+                    temp_default_name = default_name + str(j + 1).zfill(3)
+                else:
+                    default_name = temp_default_name
+                    break
+
+            project_dir = cookiecutter.prompt.read_user_variable(
+                "New name", default_name
+            )
+            try:
+                os.mkdir(directory / project_dir)
+                click.echo(f"created {project_dir}")
+            except FileExistsError:
+                click.echo("OK - but this directory already exists!")
+        selected_project_dir = directory / project_dir
+
+    # get a list of all folders
+    existing_projects = os.listdir(selected_project_dir)
+
+    os.chdir(selected_project_dir)
+    cellpy_version = cellpy.__version__
+
+    try:
+        selected_template, cookie_dir = templates[template.lower()]
+
+        if cookie_directory:
+            cookie_dir = cookie_directory
+        if not cookie_dir:
+            cookie_dir = template.lower()
+
+        cookiecutter.main.cookiecutter(
+            selected_template,
+            extra_context={
+                "author_name": os.getlogin(),
+                "project_name": project_dir,
+                "cellpy_version": cellpy_version,
+                "session_id": session_id,
+            },
+            no_input=no_input,
+            directory=cookie_dir,
+        )
+    except cookiecutter.exceptions.OutputDirExistsException as e:
+        click.echo("Sorry. This did not work as expected!")
+        click.echo(" - cookiecutter refused to create the project")
+        click.echo(e)
+
+    if serve_:
+        os.chdir(directory)
+        _serve(server)
+
+    if run_:
+        try:
+            import papermill as pm
+        except ImportError:
+            click.echo(
+                "[cellpy]: You need to install papermill for automatically execute the notebooks."
+            )
+            click.echo("[cellpy]: You can install it using pip like this:")
+            click.echo(" >> pip install papermill")
+            return
+        new_existing_projects = os.listdir(selected_project_dir)
+        our_new_projects = list(set(new_existing_projects) - set(existing_projects))
+
+        if not len(our_new_projects):
+            click.echo(
+                "[cellpy]: Sorry, could not deiced what is the new project "
+                "- so I don't dare to try to execute automatically."
+            )
+            return
+        our_new_project = selected_project_dir / our_new_projects[0]
+
+        _run_project(our_new_project)
+
+
+def _serve(server):
+    click.echo(f"serving with jupyter {server}")
+    subprocess.run(["jupyter", server], check=True)
+    click.echo("Finished serving.")
+
+
+# ----------------------- serve ---------------------------------------
+@click.command()
+@click.option("--lab", "-l", is_flag=True, help="Use Jupyter Lab instead of Notebook")
+@click.option("--directory", "-d", default=None, help="Start in custom directory DIR")
+def serve(lab, directory):
+    """Start a Jupyter server."""
+
+    from cellpy.parameters import prms
+
+    if directory is None:
+        directory = prms.Paths.notebookdir
+    elif directory == "home":
+        directory = Path().home()
+    elif directory == "here":
+        directory = Path(os.getcwd())
+
+    if not os.path.isdir(directory):
+        click.echo("Sorry. This did not work as expected!")
+        click.echo(f" - {directory} does not exist")
+        return
+
+    if lab:
+        server = "lab"
+    else:
+        server = "notebook"
+
+    os.chdir(directory)
+    _serve(server)
+
+
+cli.add_command(setup)
+cli.add_command(info)
+cli.add_command(edit)
+cli.add_command(pull)
+cli.add_command(run)
+cli.add_command(new)
+cli.add_command(serve)
+
+
+# tests etc
+def _main_pull():
+    if sys.platform == "win32":
+        rootpath = pathlib.Path(r"C:\Temp\cellpy_user")
+    else:
+        rootpath = pathlib.Path("/Users/jepe/scripting/tmp/cellpy_test_user")
+    _pull_examples(rootpath, pw="env")
+    _pull_tests(rootpath, pw="env")
+    # _pull(gdirpath="examples", rootpath=rootpath, u="ask", pw="ask")
+    # _pull(gdirpath="tests", rootpath=rootpath, u="ask", pw="ask")
+    # _pull(gdirpath="testdata", rootpath=rootpath, u="ask", pw="ask")
+
+
+def _main():
+    file_name = prmreader.create_custom_init_filename()
+    click.echo(file_name)
+    user_directory, destination_file_name = prmreader.get_user_dir_and_dst(file_name)
+    click.echo(user_directory)
+    click.echo(destination_file_name)
+    click.echo("trying to save it")
+    save_prm_file(destination_file_name + "_dummy")
+
+    click.echo(" Testing setup ".center(80, "="))
+    setup(["--interactive", "--reset"])
+
+
+def _cli_setup_interactive():
+    from click.testing import CliRunner
+
+    if sys.platform == "win32":
+        root_dir = r"C:\Temp\cellpy_user"
+    else:
+        root_dir = "/Users/jepe/scripting/tmp/cellpy_test_user"
+    testuser = "tester"
+    init_filename = prmreader.create_custom_init_filename(testuser)
+    dst_file = get_dst_file(root_dir, init_filename)
+    init_file = pathlib.Path(dst_file)
+    opts = list()
+    opts.append("setup")
+    opts.append("-i")
+    # opts.append("-nr")
+    opts.append("-r")
+    opts.extend(["-d", root_dir])
+    opts.extend(["-t", testuser])
+
+    input_str = "\n"  # out
+    input_str += "\n"  # rawdatadir
+    input_str += "\n"  # cellpyfiles
+    input_str += "\n"  # log
+    input_str += "\n"  # examples
+    input_str += "\n"  # dbfolder
+    input_str += "\n"  # dbfile
+    runner = CliRunner()
+    result = runner.invoke(cli, opts, input=input_str)
+
+    click.echo(" out ".center(80, "."))
+    click.echo(result.output)
+    from pprint import pprint
+
+    pprint(prmreader.prms.Paths)
+    click.echo(" conf-file ".center(80, "."))
+    click.echo(init_file)
+    click.echo()
+    with init_file.open() as f:
+        for line in f.readlines():
+            click.echo(line.strip())
+
+
+def check_it(var=None):
+    import pathlib
+    import sys
+
+    p_env = pathlib.Path(sys.prefix)
+    print(p_env.name)
+    new(list_=True)
+
+
+if __name__ == "__main__":
+    u1 = os.getlogin()
+    u2 = os.path.expanduser("~")
+    u3 = os.environ.get("USERNAME")
+
+    print(u1)
+    print(u2)
+    print(u3)
+    # check_it()
+    # click.echo("\n\n", " RUNNING MAIN PULL ".center(80, "*"), "\n")
+    # _main_pull()
+    # click.echo("ok")
```

### Comparing `cellpy-1.0.0a3/cellpy/exceptions.py` & `cellpy-1.0.0a4/cellpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/internals/core.py` & `cellpy-1.0.0a4/cellpy/internals/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,687 +1,710 @@
-"""This module contains div classes etc that are not really connected to cellpy."""
-
-from dataclasses import dataclass
-import fnmatch
-import logging
-import os
-import pathlib
-import shutil
-import stat
-import tempfile
-import time
-import warnings
-from typing import (
-    Any,
-    Tuple,
-    Dict,
-    List,
-    Union,
-    TypeVar,
-    Generator,
-    Optional,
-    Iterable,
-    Callable,
-    Type,
-    cast,
-)
-
-import fabric
-
-from cellpy.exceptions import UnderDefined
-
-S = TypeVar("S", bound="OtherPath")
-URI_PREFIXES = ["ssh:", "sftp:", "scp:", "http:", "https:", "ftp:", "ftps:", "smb:"]
-IMPLEMENTED_PROTOCOLS = ["ssh:", "sftp:", "scp:"]
-# name of environment variable that holds the key file and password:
-ENV_VAR_CELLPY_KEY_FILENAME = "CELLPY_KEY_FILENAME"
-ENV_VAR_CELLPY_PASSWORD = "CELLPY_PASSWORD"
-
-
-@dataclass
-class ExternalStatResult:
-    """Mock of os.stat_result."""
-
-    # st_mode: int = 0
-    # st_ino: int = 0
-    # st_dev: int = 0
-    # st_nlink: int = 0
-    # st_uid: int = 0
-    # st_gid: int = 0
-    st_size: int = 0
-    st_mtime: int = 0
-    st_atime: int = 0
-    st_ctime: Optional[int] = None
-
-
-def _clean_up_original_path_string(path_string):
-    if not isinstance(path_string, str):
-        if isinstance(path_string, OtherPath):
-            logging.debug(f"path is an OtherPath object")
-            if hasattr(path_string, "original"):
-                logging.debug(f"path has an original attribute")
-                path_string = path_string.original
-            else:
-                logging.debug(f"path does not have an original attribute")
-                path_string = str(path_string)
-
-        elif isinstance(path_string, pathlib.PosixPath):
-            path_string = "/".join(path_string.parts)
-        elif isinstance(path_string, pathlib.WindowsPath):
-            parts = list(path_string.parts)
-            if not parts:
-                parts = [""]
-            parts[0] = parts[0].replace("\\", "")
-            path_string = "/".join(parts)
-        else:
-            logging.debug(f"unknown path type: {type(path_string)}")
-            path_string = str(path_string)
-    return path_string
-
-
-def _check_external(path_string: str) -> Tuple[str, bool, str, str]:
-    # path_sep = "\\" if os.name == "nt" else "/"
-    _is_external = False
-    _location = ""
-    _uri_prefix = ""
-    for prefix in URI_PREFIXES:
-        if path_string.startswith(prefix):
-            path_string = path_string.replace(prefix, "")
-            path_string = path_string.lstrip("/")
-            _is_external = True
-            _uri_prefix = prefix + "//"
-            _location, *rest = path_string.split("/")
-            path_string = "/" + "/".join(rest)
-            break
-    path_string = path_string or "."
-    # fix for windows paths:
-    path_string = path_string.replace("\\", "/")
-    # fix for posix paths:
-    path_string = path_string.replace("//", "/")
-    return path_string, _is_external, _uri_prefix, _location
-
-
-class OtherPath(pathlib.Path):
-    """A pathlib.Path subclass that can handle external paths.
-
-    Additional attributes:
-        is_external (bool): is True if the path is external.
-        location (str): the location of the external path (e.g. a server name).
-        uri_prefix (str): the prefix of the external path (e.g. scp:// or sftp://).
-        raw_path (str): the path without any uri_prefix or location.
-        original (str): the original path string.
-        full_path (str): the full path (including uri_prefix and location).
-    Additional methods:
-        copy (method): a method for copying the file to a local path.
-    Overrides (only if is_external is True):
-        glob (method): a method for globbing external paths.
-        rglob (method): a method for 'recursive' globbing external paths (max one extra level deep).
-    """
-
-    _flavour = (
-        pathlib._windows_flavour if os.name == "nt" else pathlib._posix_flavour
-    )  # noqa
-
-    def __new__(cls, *args, **kwargs):
-        if args:
-            path, *args = args
-        else:
-            path = "."
-            logging.debug("initiating OtherPath without any arguments")
-        if not path:
-            logging.debug("initiating OtherPath with empty path")
-            path = "."
-        if isinstance(path, OtherPath) and hasattr(path, "_original"):
-            logging.debug(f"path is OtherPath")
-            path = path._original
-        logging.debug(f"checked if path is OtherPath")
-
-        path = _clean_up_original_path_string(path)
-        assert isinstance(path, str), "path must be a string"
-        cls.__original = path
-        cls._pathlib_doc = super().__doc__
-        path = _check_external(path)[0]
-        return super().__new__(cls, path, *args, **kwargs)
-
-    def __init__(self, *args, **kwargs):
-        logging.debug("Running __init__ for OtherPath")
-        _path_string, *args = args
-        if not _path_string:
-            path_string = "."
-        else:
-            path_string = self.__original
-        self._original = self.__original
-        self._check_external(path_string)
-        # pathlib.PurePath and Path for Python 3.12 seems to have an __init__ method
-        # where it sets self._raw_path from the input argument, but this is not the case
-        # for Python 3.11, 10, and 9. Those do not have their own __init__ method (and
-        # does not have a self._raw_path attribute).
-        # Instead of running e.g. super().__init__(self._raw_other_path) we do this
-        # instead (which is what the __init__ method does in Python 3.12):
-        self._raw_path = self._raw_other_path
-        self.__doc__ += f"\nOriginal documentation:\n\n{self._pathlib_doc}"
-        self._wrap_methods()  # dynamically wrapping methods - should gradually be replaced by hard-coded methods.
-
-    def _wrap_methods(self):
-        logging.debug("Running _wrap_methods for OtherPath")
-        existing_methods = self.__class__.__dict__.keys()
-        parent_methods_that_works_also_on_external_paths = []  # "parents", "parts"
-        parent_methods_that_returns_other_paths = []
-
-        for m in sorted(dir(pathlib.Path)):
-            if m.startswith("_"):
-                continue
-            if (
-                m in existing_methods
-                or m in parent_methods_that_works_also_on_external_paths
-            ):
-                continue
-            method = getattr(pathlib.Path, m)
-            if m in parent_methods_that_returns_other_paths:
-                setattr(self.__class__, m, self._wrap_and_morph_method(method))
-            if callable(method):
-                setattr(self.__class__, m, self._wrap_callable_method(method))
-            else:
-                setattr(self.__class__, m, self._wrap_non_callable(method))
-
-    def _wrap_and_morph_method(self, method):
-        if self.is_external:
-            return lambda *args, **kwargs: self
-        else:
-            return lambda *args, **kwargs: OtherPath(*args, **kwargs)
-
-    def _wrap_callable_method(self, method, default_return_value=True):
-        if self.is_external:
-            return lambda *args, **kwargs: default_return_value
-        else:
-            return method
-
-    def _wrap_non_callable(self, attr, default_return_value=None):
-        if self.is_external:
-            return default_return_value
-        else:
-            return attr
-
-    def _check_external(self, path_string):
-        logging.debug("Running _check_external for OtherPath")
-        (
-            path_string,
-            self._is_external,
-            self._uri_prefix,
-            self._location,
-        ) = _check_external(path_string)
-        logging.debug(f"self._is_external: {self._is_external}")
-        logging.debug(f"self._uri_prefix: {self._uri_prefix}")
-        logging.debug(f"self._location: {self._location}")
-        logging.debug(f"path_string: {path_string}")
-        self._raw_other_path = path_string
-
-    def __div__(self, other: Union[str, S]) -> S:
-        if self.is_external:
-            path = f"{self._original}/{other}"
-            return OtherPath(path)
-        path = pathlib.Path(self._original).__truediv__(other)
-        return OtherPath(path)
-
-    def __truediv__(self, other: Union[str, S]) -> S:
-        if self.is_external:
-            path = f"{self._original}/{other}"
-            return OtherPath(path)
-        path = pathlib.Path(self._original).__truediv__(other)
-        return OtherPath(path)
-
-    def __rtruediv__(self: S, key: Union[str, S]) -> S:
-        if self.is_external:
-            raise TypeError(f"Cannot use rtruediv on external paths.")
-        path = pathlib.Path(self._original).__rtruediv__(key)
-        return OtherPath(path)
-
-    def __str__(self: S) -> str:
-        if hasattr(self, "_original") and self.is_external:
-            logging.debug("external path, returning _original")
-            return self._original
-        return super().__str__()
-
-    def __repr__(self: S) -> str:
-        if hasattr(self, "_original"):
-            if self.is_external:
-                logging.debug("external path, returning _original")
-            return f"OtherPath('{self._original}')"
-        else:
-            return super().__repr__()
-
-    def _glob(self, glob_str: str, **kwargs) -> Generator:
-        testing = kwargs.pop("testing", False)
-        search_in_sub_dirs = kwargs.pop("search_in_sub_dirs", False)
-        if self.is_external:
-            connect_kwargs, host = self._get_connection_info(testing)
-            paths = self._glob_with_fabric(
-                host, connect_kwargs, glob_str, search_in_sub_dirs=search_in_sub_dirs
-            )
-            return (OtherPath(f"{self._original.rstrip('/')}/{p}") for p in paths)
-        paths = pathlib.Path(self._original).glob(glob_str)
-        return (OtherPath(p) for p in paths)
-
-    def glob(self, glob_str: str, *args, **kwargs) -> Generator:
-        return self._glob(glob_str, search_in_sub_dirs=False, **kwargs)
-
-    def rglob(self, glob_str: str, *args, **kwargs) -> Generator:
-        return self._glob(glob_str, search_in_sub_dirs=True, **kwargs)
-
-    def _listdir(self, levels: int, **kwargs) -> Generator:
-        if self.is_external:
-            testing = kwargs.pop("testing", False)
-            connect_kwargs, host = self._get_connection_info(testing)
-            paths = self._listdir_with_fabric(host, connect_kwargs, levels)
-            return (OtherPath(p) for p in paths)
-
-        if self.is_dir():
-            return (OtherPath(f"{self.full_path}/{p}") for p in os.listdir(self._original))
-
-    def listdir(self: S, levels: int = 1, **kwargs) -> Generator:
-        """List the contents of the directory.
-
-        Args:
-            levels (int, optional): How many sublevels to list. Defaults to 1.
-                If you want to list all sublevels, use `listdir(levels=-1)`.
-                If you want to list only the current level (no subdirectories),
-                use `listdir(levels=0)`.
-
-        Returns:
-            Generator: Generator of OtherPath objects.
-
-        """
-        return self._listdir(levels, **kwargs)
-
-    def resolve(self: S, *args, **kwargs) -> S:
-        """Resolve the path."""
-        if self.is_external:
-            logging.debug(f"Cannot resolve external paths. Returning self. ({self})")
-            return OtherPath(self._original)
-        resolved_path = pathlib.Path(self._original).resolve(*args, **kwargs)
-        return OtherPath(resolved_path)
-
-    def is_dir(self: S, *args, **kwargs) -> bool:
-        """Check if path is a directory."""
-        if self.is_external:
-            logging.warning(
-                f"Cannot check if dir exists for external paths! Assuming it exists."
-            )
-            return True
-        return super().is_dir()
-
-    def is_file(self: S, *args, **kwargs) -> bool:
-        """Check if path is a file."""
-        if self.is_external:
-            logging.warning(
-                f"Cannot check if file exists for external paths! Assuming it exists."
-            )
-            return True
-        return super().is_file()
-
-    def exists(self: S, *args, **kwargs) -> bool:
-        """Check if path exists."""
-        if self.is_external:
-            logging.warning(
-                f"Cannot check if path exists for external paths! Assuming it exists."
-            )
-            return True
-        return super().exists()
-
-    @property
-    def parent(self: S) -> S:
-        """Return the parent directory of the path."""
-        if self.is_external:
-            return OtherPath(self._original.rsplit("/", 1)[0])
-        return OtherPath(super().parent)
-
-    @property
-    def name(self: S):
-        """Return the parent directory of the path."""
-        return super().name
-
-    @property
-    def suffix(self) -> str:
-        """Return the suffix of the path."""
-        return super().suffix
-
-    @property
-    def suffixes(self) -> List[str]:
-        """Return the suffixes of the path."""
-        return super().suffixes
-
-    @property
-    def stem(self) -> str:
-        """Return the stem of the path."""
-        return super().stem
-
-    def with_suffix(self: S, suffix: str) -> S:
-        """Return a new path with the suffix changed."""
-        if self.is_external:
-            logging.warning(
-                "This is method (`with_suffix`) not tested for external paths!"
-            )
-            return OtherPath(self._original.rsplit(".", 1)[0] + suffix)
-        return OtherPath(super().with_suffix(suffix))
-
-    def with_name(self: S, name: str) -> S:
-        """Return a new path with the name changed."""
-        if self.is_external:
-            logging.warning(
-                "This method (`with_name`) is not tested for external paths!"
-            )
-            return OtherPath(self._original.rsplit("/", 1)[0] + "/" + name)
-        return OtherPath(super().with_name(name))
-
-    def with_stem(self: S, stem: str) -> S:
-        """Return a new path with the stem changed."""
-        if self.is_external:
-            logging.warning(
-                "This method (`with_stem`) is not tested for external paths!"
-            )
-            return OtherPath(self._original.rsplit("/", 1)[0] + "/" + stem)
-        return OtherPath(super().with_stem(stem))
-
-    def absolute(self: S) -> S:
-        if self.is_external:
-            logging.warning(
-                "This method (`absolute`) is not implemented yet for external paths! Returning self."
-            )
-            return OtherPath(self._original)
-        return OtherPath(super().absolute())
-
-    def samefile(self: S, other_path: Union[str, pathlib.Path, S]) -> bool:
-        if self.is_external:
-            logging.warning(
-                "This method (`absolute`) is not implemented yet for external paths! Returning True."
-            )
-            return True
-        return super().samefile(other_path)
-
-    def iterdir(self, *args, **kwargs):
-        if self.is_external:
-            logging.warning(
-                f"Cannot run `iterdir` yet for external paths! Returning None."
-            )
-            return
-        else:
-            return (OtherPath(p) for p in super().iterdir())
-
-    @property
-    def parents(self, *args, **kwargs):
-        if self.is_external:
-            logging.warning(
-                f"Cannot run `parents` yet for external paths! Returning None."
-            )
-            return
-        return super().parents
-
-    def stat(self, *args, **kwargs):
-        testing = kwargs.pop("testing", False)
-        if self.is_external:
-            # logging.warning(f"Cannot run `stat` for external paths! Returning stat_result object with only zeros.")
-            try:
-                connect_kwargs, host = self._get_connection_info(testing)
-            except UnderDefined as e:
-                logging.debug(f"UnderDefined error: {e}")
-                logging.debug("Returning stat_result object with only zeros.")
-                return ExternalStatResult()
-            try:
-                return self._stat_with_fabric(host, connect_kwargs)
-            except FileNotFoundError:
-                logging.debug(
-                    "File not found! Returning stat_result object with only zeros."
-                )
-                return ExternalStatResult()
-
-        return super().stat()
-
-    def joinpath(self, *args, **kwargs):
-        logging.warning(f"Cannot run 'joinpath' for OtherPath!")
-        return OtherPath(self._original)
-
-    def readlink(self, *args, **kwargs):
-        logging.warning(f"Cannot run 'readlink' for OtherPath!")
-        return
-
-    def match(self, *args, **kwargs):
-        logging.warning(f"Cannot run 'match' for OtherPath!")
-        return
-
-    def cwd(self):
-        logging.warning(f"Cannot run 'match' for OtherPath!")
-        return
-
-    def group(self):
-        logging.warning(f"Cannot run 'group' for OtherPath!")
-        return
-
-    @property
-    def owner(self, *args, **kwargs):
-        logging.warning(f"Cannot get 'owner' for OtherPath!")
-        return
-
-    def lchmod(self, *args, **kwargs):
-        logging.warning(f"Cannot run 'lchmod' for OtherPath!")
-        return OtherPath(self._original)
-
-    @property
-    def original(self: S) -> str:
-        return self._original
-
-    @property
-    def raw_path(self: S) -> str:
-        # this will return a leading slash for some edge cases
-        return self._raw_other_path
-
-    @property
-    def full_path(self: S) -> str:
-        if self.is_external:
-            return f"{self._uri_prefix}{self._location}{self._raw_other_path}"
-        return self._original
-
-    @property
-    def pathlike_location(self: S) -> S:
-        """Return the location of the external path as a pathlike object."""
-
-        if self.is_external:
-            return OtherPath(f"{self._uri_prefix}{self._location}")
-        return OtherPath(super().drive)
-
-    @property
-    def is_external(self: S) -> bool:
-        if not hasattr(self, "_is_external"):
-            logging.warning("OBS! OtherPath object missing _is_external attribute!")
-            logging.warning("This should not happen. Please report this bug!")
-            logging.warning(
-                "(most likely means that pathlib.Path has changed and that it now has "
-                "another attribute or method that returns a new pathlib.Path object or "
-                "that you have used a method that is not supported yet)"
-            )
-            # return False
-        return self._is_external
-
-    @property
-    def uri_prefix(self) -> str:
-        """Return the uri prefix for the external path (e.g ``ssh://``)."""
-        return self._uri_prefix
-
-    @property
-    def location(self) -> str:
-        """Return the location of the external path (e.g ``user@server.com``)."""
-        return self._location
-
-    def as_uri(self) -> str:
-        """Return the path as a uri (e.g. ``scp://user@server.com/home/data/my_file.txt``)."""
-        if self._is_external:
-            return f"{self._uri_prefix}{self._location}/{'/'.join(list(super().parts)[1:])}"
-        return super().as_uri()
-
-    def copy(
-        self, destination: Optional[pathlib.Path] = None, testing=False
-    ) -> pathlib.Path:
-        """Copy the file to a destination."""
-        if destination is None:
-            destination = pathlib.Path(tempfile.gettempdir())
-        else:
-            destination = pathlib.Path(destination)
-        path_of_copied_file = destination / self.name
-
-        if not self.is_external:
-            shutil.copy2(self, destination)
-        else:
-            connect_kwargs, host = self._get_connection_info(testing)
-            self._copy_with_fabric(host, connect_kwargs, destination)
-
-        return path_of_copied_file
-
-    def _get_connection_info(self, testing: bool = False) -> Tuple[Dict, str]:
-        host = self.location
-        uri_prefix = self.uri_prefix.replace("//", "")
-        if uri_prefix not in URI_PREFIXES:
-            raise ValueError(f"uri_prefix {uri_prefix} not recognized")
-        if uri_prefix not in IMPLEMENTED_PROTOCOLS:
-            raise ValueError(
-                f"uri_prefix {uri_prefix.replace(':', '')} not implemented yet"
-            )
-        password = os.getenv(ENV_VAR_CELLPY_PASSWORD, None)
-        key_filename = os.getenv(ENV_VAR_CELLPY_KEY_FILENAME, None)
-        if password is None and key_filename is None:
-            raise UnderDefined(
-                f"You must define either {ENV_VAR_CELLPY_PASSWORD} "
-                f"or {ENV_VAR_CELLPY_KEY_FILENAME} environment variables."
-            )
-        if key_filename is not None:
-            key_filename = pathlib.Path(key_filename).expanduser().resolve()
-            connect_kwargs = {"key_filename": str(key_filename)}
-            logging.debug(f"got key_filename")
-            if not testing:
-                if not pathlib.Path(key_filename).is_file():
-                    raise FileNotFoundError(f"Could not find key file {key_filename}")
-        else:
-            connect_kwargs = {"password": password}
-        return connect_kwargs, host
-
-    def _copy_with_fabric(
-        self, host: str, connect_kwargs: dict, destination: Union[str, S, pathlib.Path]
-    ):
-        with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
-            try:
-                t1 = time.time()
-                conn.get(self.raw_path, str(destination / self.name))
-                logging.debug(f"copying took {time.time() - t1:.2f} seconds")
-            except FileNotFoundError as e:
-                raise FileNotFoundError(
-                    f"Could not find file {self.raw_path} on {host}"
-                ) from e
-
-    def _stat_with_fabric(self, host: str, connect_kwargs: dict) -> ExternalStatResult:
-        with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
-            try:
-                t1 = time.time()
-                sftp_conn = conn.sftp()
-                stat_result = sftp_conn.stat(self.raw_path)
-                logging.debug(f"stat took {time.time() - t1:.2f} seconds")
-                return ExternalStatResult(
-                    st_size=stat_result.st_size,
-                    st_atime=stat_result.st_atime,
-                    st_mtime=stat_result.st_mtime,
-                )
-            except FileNotFoundError as e:
-                raise FileNotFoundError(
-                    f"Could not find file {self.raw_path} on {host}"
-                ) from e
-
-    def _listdir_with_fabric(
-        self: S,
-        host: str,
-        connect_kwargs: dict,
-        levels: int = 1,
-    ) -> List[str]:
-        """List the contents of a directory through sftp."""
-
-        path_separator = "/"  # only supports unix-like systems
-        t1 = time.time()
-        with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
-            try:
-                t1 = time.time()
-                sftp_conn = conn.sftp()
-                sftp_conn.chdir(self.raw_path)
-                sub_dirs = [f"{self.raw_path}{path_separator}{f}" for f in sftp_conn.listdir() if stat.S_ISDIR(sftp_conn.stat(f).st_mode)]
-                files = [f"{self.raw_path}{path_separator}{f}" for f in sftp_conn.listdir() if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)]
-                while levels != 0:
-                    new_sub_dirs = []
-                    for sub_dir in sub_dirs:
-                        try:
-                            sftp_conn.chdir(sub_dir)
-                            _new_sub_dirs = [f"{sub_dir}{path_separator}{f}" for f in sftp_conn.listdir() if stat.S_ISDIR(sftp_conn.stat(f).st_mode)]
-                            new_files = [f"{sub_dir}{path_separator}{f}" for f in sftp_conn.listdir() if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)]
-                            files += new_files
-                            new_sub_dirs += _new_sub_dirs
-                            sftp_conn.chdir(self.raw_path)
-                        except FileNotFoundError:
-                            logging.debug(f"Could not look in {sub_dir}: FileNotFoundError")
-                        pass
-                    sub_dirs = new_sub_dirs
-                    if len(sub_dirs) == 0:
-                        break
-                    levels -= 1
-
-                logging.debug(f"globbing took {time.time() - t1:.2f} seconds")
-                return files
-            except FileNotFoundError as e:
-                raise FileNotFoundError(
-                    f"Could not find file {self.raw_path} on {host}"
-                ) from e
-
-    def _glob_with_fabric(
-        self: S,
-        host: str,
-        connect_kwargs: dict,
-        glob_str: str,
-        search_in_sub_dirs: bool = False,
-    ) -> List[str]:
-        # TODO: update this so that it works faster (need some linux magic)
-        path_separator = "/"
-        with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
-            try:
-                t1 = time.time()
-                sftp_conn = conn.sftp()
-                sftp_conn.chdir(self.raw_path)
-                if search_in_sub_dirs:  # recursive globbing one level down
-                    sub_dirs = [
-                        f
-                        for f in sftp_conn.listdir()
-                        if stat.S_ISDIR(sftp_conn.stat(f).st_mode)
-                    ]
-                    files = [
-                        f
-                        for f in sftp_conn.listdir()
-                        if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)
-                    ]
-                    filtered_files = fnmatch.filter(files, glob_str)
-                    for sub_dir in sub_dirs:
-                        try:
-                            sftp_conn.chdir(sub_dir)
-                            new_files = [
-                                f
-                                for f in sftp_conn.listdir()
-                                if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)
-                            ]
-                            new_filtered_files = fnmatch.filter(new_files, glob_str)
-                            new_filtered_files = [
-                                f"{sub_dir}{path_separator}{f}" for f in new_filtered_files
-                            ]
-                            filtered_files += new_filtered_files
-                            sftp_conn.chdir("..")
-                        except FileNotFoundError:
-                            logging.debug(f"Could not look in {sub_dir}: FileNotFoundError")
-                            pass
-                else:
-                    files = sftp_conn.listdir()
-                    filtered_files = fnmatch.filter(files, glob_str)
-                logging.debug(f"globbing took {time.time() - t1:.2f} seconds")
-                return filtered_files
-            except FileNotFoundError as e:
-                raise FileNotFoundError(
-                    f"Could not find file {self.raw_path} on {host}"
-                ) from e
+"""This module contains div classes etc that are not really connected to cellpy."""
+
+from dataclasses import dataclass
+import fnmatch
+import logging
+import os
+import pathlib
+import shutil
+import stat
+import tempfile
+import time
+import warnings
+from typing import (
+    Any,
+    Tuple,
+    Dict,
+    List,
+    Union,
+    TypeVar,
+    Generator,
+    Optional,
+    Iterable,
+    Callable,
+    Type,
+    cast,
+)
+
+import fabric
+
+from cellpy.exceptions import UnderDefined
+
+S = TypeVar("S", bound="OtherPath")
+URI_PREFIXES = ["ssh:", "sftp:", "scp:", "http:", "https:", "ftp:", "ftps:", "smb:"]
+IMPLEMENTED_PROTOCOLS = ["ssh:", "sftp:", "scp:"]
+# name of environment variable that holds the key file and password:
+ENV_VAR_CELLPY_KEY_FILENAME = "CELLPY_KEY_FILENAME"
+ENV_VAR_CELLPY_PASSWORD = "CELLPY_PASSWORD"
+
+
+@dataclass
+class ExternalStatResult:
+    """Mock of os.stat_result."""
+
+    # st_mode: int = 0
+    # st_ino: int = 0
+    # st_dev: int = 0
+    # st_nlink: int = 0
+    # st_uid: int = 0
+    # st_gid: int = 0
+    st_size: int = 0
+    st_mtime: int = 0
+    st_atime: int = 0
+    st_ctime: Optional[int] = None
+
+
+def _clean_up_original_path_string(path_string):
+    if not isinstance(path_string, str):
+        if isinstance(path_string, OtherPath):
+            logging.debug(f"path is an OtherPath object")
+            if hasattr(path_string, "original"):
+                logging.debug(f"path has an original attribute")
+                path_string = path_string.original
+            else:
+                logging.debug(f"path does not have an original attribute")
+                path_string = str(path_string)
+
+        elif isinstance(path_string, pathlib.PosixPath):
+            path_string = "/".join(path_string.parts)
+        elif isinstance(path_string, pathlib.WindowsPath):
+            parts = list(path_string.parts)
+            if not parts:
+                parts = [""]
+            parts[0] = parts[0].replace("\\", "")
+            path_string = "/".join(parts)
+        else:
+            logging.debug(f"unknown path type: {type(path_string)}")
+            path_string = str(path_string)
+    return path_string
+
+
+def _check_external(path_string: str) -> Tuple[str, bool, str, str]:
+    # path_sep = "\\" if os.name == "nt" else "/"
+    _is_external = False
+    _location = ""
+    _uri_prefix = ""
+    for prefix in URI_PREFIXES:
+        if path_string.startswith(prefix):
+            path_string = path_string.replace(prefix, "")
+            path_string = path_string.lstrip("/")
+            _is_external = True
+            _uri_prefix = prefix + "//"
+            _location, *rest = path_string.split("/")
+            path_string = "/" + "/".join(rest)
+            break
+    path_string = path_string or "."
+    # fix for windows paths:
+    path_string = path_string.replace("\\", "/")
+    # fix for posix paths:
+    path_string = path_string.replace("//", "/")
+    return path_string, _is_external, _uri_prefix, _location
+
+
+class OtherPath(pathlib.Path):
+    """A pathlib.Path subclass that can handle external paths.
+
+    Additional attributes:
+        is_external (bool): is True if the path is external.
+        location (str): the location of the external path (e.g. a server name).
+        uri_prefix (str): the prefix of the external path (e.g. scp:// or sftp://).
+        raw_path (str): the path without any uri_prefix or location.
+        original (str): the original path string.
+        full_path (str): the full path (including uri_prefix and location).
+    Additional methods:
+        copy (method): a method for copying the file to a local path.
+    Overrides (only if is_external is True):
+        glob (method): a method for globbing external paths.
+        rglob (method): a method for 'recursive' globbing external paths (max one extra level deep).
+    """
+
+    _flavour = (
+        pathlib._windows_flavour if os.name == "nt" else pathlib._posix_flavour
+    )  # noqa
+
+    def __new__(cls, *args, **kwargs):
+        if args:
+            path, *args = args
+        else:
+            path = "."
+            logging.debug("initiating OtherPath without any arguments")
+        if not path:
+            logging.debug("initiating OtherPath with empty path")
+            path = "."
+        if isinstance(path, OtherPath) and hasattr(path, "_original"):
+            logging.debug(f"path is OtherPath")
+            path = path._original
+        logging.debug(f"checked if path is OtherPath")
+
+        path = _clean_up_original_path_string(path)
+        assert isinstance(path, str), "path must be a string"
+        cls.__original = path
+        cls._pathlib_doc = super().__doc__
+        path = _check_external(path)[0]
+        return super().__new__(cls, path, *args, **kwargs)
+
+    def __init__(self, *args, **kwargs):
+        logging.debug("Running __init__ for OtherPath")
+        _path_string, *args = args
+        if not _path_string:
+            path_string = "."
+        else:
+            path_string = self.__original
+        self._original = self.__original
+        self._check_external(path_string)
+        # pathlib.PurePath and Path for Python 3.12 seems to have an __init__ method
+        # where it sets self._raw_path from the input argument, but this is not the case
+        # for Python 3.11, 10, and 9. Those do not have their own __init__ method (and
+        # does not have a self._raw_path attribute).
+        # Instead of running e.g. super().__init__(self._raw_other_path) we do this
+        # instead (which is what the __init__ method does in Python 3.12):
+        self._raw_path = self._raw_other_path
+        self.__doc__ += f"\nOriginal documentation:\n\n{self._pathlib_doc}"
+        self._wrap_methods()  # dynamically wrapping methods - should gradually be replaced by hard-coded methods.
+
+    def _wrap_methods(self):
+        logging.debug("Running _wrap_methods for OtherPath")
+        existing_methods = self.__class__.__dict__.keys()
+        parent_methods_that_works_also_on_external_paths = []  # "parents", "parts"
+        parent_methods_that_returns_other_paths = []
+
+        for m in sorted(dir(pathlib.Path)):
+            if m.startswith("_"):
+                continue
+            if (
+                m in existing_methods
+                or m in parent_methods_that_works_also_on_external_paths
+            ):
+                continue
+            method = getattr(pathlib.Path, m)
+            if m in parent_methods_that_returns_other_paths:
+                setattr(self.__class__, m, self._wrap_and_morph_method(method))
+            if callable(method):
+                setattr(self.__class__, m, self._wrap_callable_method(method))
+            else:
+                setattr(self.__class__, m, self._wrap_non_callable(method))
+
+    def _wrap_and_morph_method(self, method):
+        if self.is_external:
+            return lambda *args, **kwargs: self
+        else:
+            return lambda *args, **kwargs: OtherPath(*args, **kwargs)
+
+    def _wrap_callable_method(self, method, default_return_value=True):
+        if self.is_external:
+            return lambda *args, **kwargs: default_return_value
+        else:
+            return method
+
+    def _wrap_non_callable(self, attr, default_return_value=None):
+        if self.is_external:
+            return default_return_value
+        else:
+            return attr
+
+    def _check_external(self, path_string):
+        logging.debug("Running _check_external for OtherPath")
+        (
+            path_string,
+            self._is_external,
+            self._uri_prefix,
+            self._location,
+        ) = _check_external(path_string)
+        logging.debug(f"self._is_external: {self._is_external}")
+        logging.debug(f"self._uri_prefix: {self._uri_prefix}")
+        logging.debug(f"self._location: {self._location}")
+        logging.debug(f"path_string: {path_string}")
+        self._raw_other_path = path_string
+
+    def __div__(self, other: Union[str, S]) -> S:
+        if self.is_external:
+            path = f"{self._original}/{other}"
+            return OtherPath(path)
+        path = pathlib.Path(self._original).__truediv__(other)
+        return OtherPath(path)
+
+    def __truediv__(self, other: Union[str, S]) -> S:
+        if self.is_external:
+            path = f"{self._original}/{other}"
+            return OtherPath(path)
+        path = pathlib.Path(self._original).__truediv__(other)
+        return OtherPath(path)
+
+    def __rtruediv__(self: S, key: Union[str, S]) -> S:
+        if self.is_external:
+            raise TypeError(f"Cannot use rtruediv on external paths.")
+        path = pathlib.Path(self._original).__rtruediv__(key)
+        return OtherPath(path)
+
+    def __str__(self: S) -> str:
+        if hasattr(self, "_original") and self.is_external:
+            logging.debug("external path, returning _original")
+            return self._original
+        return super().__str__()
+
+    def __repr__(self: S) -> str:
+        if hasattr(self, "_original"):
+            if self.is_external:
+                logging.debug("external path, returning _original")
+            return f"OtherPath('{self._original}')"
+        else:
+            return super().__repr__()
+
+    def _glob(self, glob_str: str, **kwargs) -> Generator:
+        testing = kwargs.pop("testing", False)
+        search_in_sub_dirs = kwargs.pop("search_in_sub_dirs", False)
+        if self.is_external:
+            connect_kwargs, host = self._get_connection_info(testing)
+            paths = self._glob_with_fabric(
+                host, connect_kwargs, glob_str, search_in_sub_dirs=search_in_sub_dirs
+            )
+            return (OtherPath(f"{self._original.rstrip('/')}/{p}") for p in paths)
+        paths = pathlib.Path(self._original).glob(glob_str)
+        return (OtherPath(p) for p in paths)
+
+    def glob(self, glob_str: str, *args, **kwargs) -> Generator:
+        return self._glob(glob_str, search_in_sub_dirs=False, **kwargs)
+
+    def rglob(self, glob_str: str, *args, **kwargs) -> Generator:
+        return self._glob(glob_str, search_in_sub_dirs=True, **kwargs)
+
+    def _listdir(self, levels: int, **kwargs) -> Generator:
+        if self.is_external:
+            testing = kwargs.pop("testing", False)
+            connect_kwargs, host = self._get_connection_info(testing)
+            paths = self._listdir_with_fabric(host, connect_kwargs, levels)
+            return (OtherPath(p) for p in paths)
+
+        if self.is_dir():
+            return (
+                OtherPath(f"{self.full_path}/{p}") for p in os.listdir(self._original)
+            )
+
+    def listdir(self: S, levels: int = 1, **kwargs) -> Generator:
+        """List the contents of the directory.
+
+        Args:
+            levels (int, optional): How many sublevels to list. Defaults to 1.
+                If you want to list all sublevels, use `listdir(levels=-1)`.
+                If you want to list only the current level (no subdirectories),
+                use `listdir(levels=0)`.
+
+        Returns:
+            Generator: Generator of OtherPath objects.
+
+        """
+        return self._listdir(levels, **kwargs)
+
+    def resolve(self: S, *args, **kwargs) -> S:
+        """Resolve the path."""
+        if self.is_external:
+            logging.debug(f"Cannot resolve external paths. Returning self. ({self})")
+            return OtherPath(self._original)
+        resolved_path = pathlib.Path(self._original).resolve(*args, **kwargs)
+        return OtherPath(resolved_path)
+
+    def is_dir(self: S, *args, **kwargs) -> bool:
+        """Check if path is a directory."""
+        if self.is_external:
+            logging.warning(
+                f"Cannot check if dir exists for external paths! Assuming it exists."
+            )
+            return True
+        return super().is_dir()
+
+    def is_file(self: S, *args, **kwargs) -> bool:
+        """Check if path is a file."""
+        if self.is_external:
+            logging.warning(
+                f"Cannot check if file exists for external paths! Assuming it exists."
+            )
+            return True
+        return super().is_file()
+
+    def exists(self: S, *args, **kwargs) -> bool:
+        """Check if path exists."""
+        if self.is_external:
+            logging.warning(
+                f"Cannot check if path exists for external paths! Assuming it exists."
+            )
+            return True
+        return super().exists()
+
+    @property
+    def parent(self: S) -> S:
+        """Return the parent directory of the path."""
+        if self.is_external:
+            return OtherPath(self._original.rsplit("/", 1)[0])
+        return OtherPath(super().parent)
+
+    @property
+    def name(self: S):
+        """Return the parent directory of the path."""
+        return super().name
+
+    @property
+    def suffix(self) -> str:
+        """Return the suffix of the path."""
+        return super().suffix
+
+    @property
+    def suffixes(self) -> List[str]:
+        """Return the suffixes of the path."""
+        return super().suffixes
+
+    @property
+    def stem(self) -> str:
+        """Return the stem of the path."""
+        return super().stem
+
+    def with_suffix(self: S, suffix: str) -> S:
+        """Return a new path with the suffix changed."""
+        if self.is_external:
+            logging.warning(
+                "This is method (`with_suffix`) not tested for external paths!"
+            )
+            return OtherPath(self._original.rsplit(".", 1)[0] + suffix)
+        return OtherPath(super().with_suffix(suffix))
+
+    def with_name(self: S, name: str) -> S:
+        """Return a new path with the name changed."""
+        if self.is_external:
+            logging.warning(
+                "This method (`with_name`) is not tested for external paths!"
+            )
+            return OtherPath(self._original.rsplit("/", 1)[0] + "/" + name)
+        return OtherPath(super().with_name(name))
+
+    def with_stem(self: S, stem: str) -> S:
+        """Return a new path with the stem changed."""
+        if self.is_external:
+            logging.warning(
+                "This method (`with_stem`) is not tested for external paths!"
+            )
+            return OtherPath(self._original.rsplit("/", 1)[0] + "/" + stem)
+        return OtherPath(super().with_stem(stem))
+
+    def absolute(self: S) -> S:
+        if self.is_external:
+            logging.warning(
+                "This method (`absolute`) is not implemented yet for external paths! Returning self."
+            )
+            return OtherPath(self._original)
+        return OtherPath(super().absolute())
+
+    def samefile(self: S, other_path: Union[str, pathlib.Path, S]) -> bool:
+        if self.is_external:
+            logging.warning(
+                "This method (`absolute`) is not implemented yet for external paths! Returning True."
+            )
+            return True
+        return super().samefile(other_path)
+
+    def iterdir(self, *args, **kwargs):
+        if self.is_external:
+            logging.warning(
+                f"Cannot run `iterdir` yet for external paths! Returning None."
+            )
+            return
+        else:
+            return (OtherPath(p) for p in super().iterdir())
+
+    @property
+    def parents(self, *args, **kwargs):
+        if self.is_external:
+            logging.warning(
+                f"Cannot run `parents` yet for external paths! Returning None."
+            )
+            return
+        return super().parents
+
+    def stat(self, *args, **kwargs):
+        testing = kwargs.pop("testing", False)
+        if self.is_external:
+            # logging.warning(f"Cannot run `stat` for external paths! Returning stat_result object with only zeros.")
+            try:
+                connect_kwargs, host = self._get_connection_info(testing)
+            except UnderDefined as e:
+                logging.debug(f"UnderDefined error: {e}")
+                logging.debug("Returning stat_result object with only zeros.")
+                return ExternalStatResult()
+            try:
+                return self._stat_with_fabric(host, connect_kwargs)
+            except FileNotFoundError:
+                logging.debug(
+                    "File not found! Returning stat_result object with only zeros."
+                )
+                return ExternalStatResult()
+
+        return super().stat()
+
+    def joinpath(self, *args, **kwargs):
+        logging.warning(f"Cannot run 'joinpath' for OtherPath!")
+        return OtherPath(self._original)
+
+    def readlink(self, *args, **kwargs):
+        logging.warning(f"Cannot run 'readlink' for OtherPath!")
+        return
+
+    def match(self, *args, **kwargs):
+        logging.warning(f"Cannot run 'match' for OtherPath!")
+        return
+
+    def cwd(self):
+        logging.warning(f"Cannot run 'match' for OtherPath!")
+        return
+
+    def group(self):
+        logging.warning(f"Cannot run 'group' for OtherPath!")
+        return
+
+    @property
+    def owner(self, *args, **kwargs):
+        logging.warning(f"Cannot get 'owner' for OtherPath!")
+        return
+
+    def lchmod(self, *args, **kwargs):
+        logging.warning(f"Cannot run 'lchmod' for OtherPath!")
+        return OtherPath(self._original)
+
+    @property
+    def original(self: S) -> str:
+        return self._original
+
+    @property
+    def raw_path(self: S) -> str:
+        # this will return a leading slash for some edge cases
+        return self._raw_other_path
+
+    @property
+    def full_path(self: S) -> str:
+        if self.is_external:
+            return f"{self._uri_prefix}{self._location}{self._raw_other_path}"
+        return self._original
+
+    @property
+    def pathlike_location(self: S) -> S:
+        """Return the location of the external path as a pathlike object."""
+
+        if self.is_external:
+            return OtherPath(f"{self._uri_prefix}{self._location}")
+        return OtherPath(super().drive)
+
+    @property
+    def is_external(self: S) -> bool:
+        if not hasattr(self, "_is_external"):
+            logging.warning("OBS! OtherPath object missing _is_external attribute!")
+            logging.warning("This should not happen. Please report this bug!")
+            logging.warning(
+                "(most likely means that pathlib.Path has changed and that it now has "
+                "another attribute or method that returns a new pathlib.Path object or "
+                "that you have used a method that is not supported yet)"
+            )
+            # return False
+        return self._is_external
+
+    @property
+    def uri_prefix(self) -> str:
+        """Return the uri prefix for the external path (e.g ``ssh://``)."""
+        return self._uri_prefix
+
+    @property
+    def location(self) -> str:
+        """Return the location of the external path (e.g ``user@server.com``)."""
+        return self._location
+
+    def as_uri(self) -> str:
+        """Return the path as a uri (e.g. ``scp://user@server.com/home/data/my_file.txt``)."""
+        if self._is_external:
+            return f"{self._uri_prefix}{self._location}/{'/'.join(list(super().parts)[1:])}"
+        return super().as_uri()
+
+    def copy(
+        self, destination: Optional[pathlib.Path] = None, testing=False
+    ) -> pathlib.Path:
+        """Copy the file to a destination."""
+        if destination is None:
+            destination = pathlib.Path(tempfile.gettempdir())
+        else:
+            destination = pathlib.Path(destination)
+        path_of_copied_file = destination / self.name
+
+        if not self.is_external:
+            shutil.copy2(self, destination)
+        else:
+            connect_kwargs, host = self._get_connection_info(testing)
+            self._copy_with_fabric(host, connect_kwargs, destination)
+
+        return path_of_copied_file
+
+    def _get_connection_info(self, testing: bool = False) -> Tuple[Dict, str]:
+        host = self.location
+        uri_prefix = self.uri_prefix.replace("//", "")
+        if uri_prefix not in URI_PREFIXES:
+            raise ValueError(f"uri_prefix {uri_prefix} not recognized")
+        if uri_prefix not in IMPLEMENTED_PROTOCOLS:
+            raise ValueError(
+                f"uri_prefix {uri_prefix.replace(':', '')} not implemented yet"
+            )
+        password = os.getenv(ENV_VAR_CELLPY_PASSWORD, None)
+        key_filename = os.getenv(ENV_VAR_CELLPY_KEY_FILENAME, None)
+        if password is None and key_filename is None:
+            raise UnderDefined(
+                f"You must define either {ENV_VAR_CELLPY_PASSWORD} "
+                f"or {ENV_VAR_CELLPY_KEY_FILENAME} environment variables."
+            )
+        if key_filename is not None:
+            key_filename = pathlib.Path(key_filename).expanduser().resolve()
+            connect_kwargs = {"key_filename": str(key_filename)}
+            logging.debug(f"got key_filename")
+            if not testing:
+                if not pathlib.Path(key_filename).is_file():
+                    raise FileNotFoundError(f"Could not find key file {key_filename}")
+        else:
+            connect_kwargs = {"password": password}
+        return connect_kwargs, host
+
+    def _copy_with_fabric(
+        self, host: str, connect_kwargs: dict, destination: Union[str, S, pathlib.Path]
+    ):
+        with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
+            try:
+                t1 = time.time()
+                conn.get(self.raw_path, str(destination / self.name))
+                logging.debug(f"copying took {time.time() - t1:.2f} seconds")
+            except FileNotFoundError as e:
+                raise FileNotFoundError(
+                    f"Could not find file {self.raw_path} on {host}"
+                ) from e
+
+    def _stat_with_fabric(self, host: str, connect_kwargs: dict) -> ExternalStatResult:
+        with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
+            try:
+                t1 = time.time()
+                sftp_conn = conn.sftp()
+                stat_result = sftp_conn.stat(self.raw_path)
+                logging.debug(f"stat took {time.time() - t1:.2f} seconds")
+                return ExternalStatResult(
+                    st_size=stat_result.st_size,
+                    st_atime=stat_result.st_atime,
+                    st_mtime=stat_result.st_mtime,
+                )
+            except FileNotFoundError as e:
+                raise FileNotFoundError(
+                    f"Could not find file {self.raw_path} on {host}"
+                ) from e
+
+    def _listdir_with_fabric(
+        self: S,
+        host: str,
+        connect_kwargs: dict,
+        levels: int = 1,
+    ) -> List[str]:
+        """List the contents of a directory through sftp."""
+
+        path_separator = "/"  # only supports unix-like systems
+        t1 = time.time()
+        with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
+            try:
+                t1 = time.time()
+                sftp_conn = conn.sftp()
+                sftp_conn.chdir(self.raw_path)
+                sub_dirs = [
+                    f"{self.raw_path}{path_separator}{f}"
+                    for f in sftp_conn.listdir()
+                    if stat.S_ISDIR(sftp_conn.stat(f).st_mode)
+                ]
+                files = [
+                    f"{self.raw_path}{path_separator}{f}"
+                    for f in sftp_conn.listdir()
+                    if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)
+                ]
+                while levels != 0:
+                    new_sub_dirs = []
+                    for sub_dir in sub_dirs:
+                        try:
+                            sftp_conn.chdir(sub_dir)
+                            _new_sub_dirs = [
+                                f"{sub_dir}{path_separator}{f}"
+                                for f in sftp_conn.listdir()
+                                if stat.S_ISDIR(sftp_conn.stat(f).st_mode)
+                            ]
+                            new_files = [
+                                f"{sub_dir}{path_separator}{f}"
+                                for f in sftp_conn.listdir()
+                                if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)
+                            ]
+                            files += new_files
+                            new_sub_dirs += _new_sub_dirs
+                            sftp_conn.chdir(self.raw_path)
+                        except FileNotFoundError:
+                            logging.debug(
+                                f"Could not look in {sub_dir}: FileNotFoundError"
+                            )
+                        pass
+                    sub_dirs = new_sub_dirs
+                    if len(sub_dirs) == 0:
+                        break
+                    levels -= 1
+
+                logging.debug(f"globbing took {time.time() - t1:.2f} seconds")
+                return files
+            except FileNotFoundError as e:
+                raise FileNotFoundError(
+                    f"Could not find file {self.raw_path} on {host}"
+                ) from e
+
+    def _glob_with_fabric(
+        self: S,
+        host: str,
+        connect_kwargs: dict,
+        glob_str: str,
+        search_in_sub_dirs: bool = False,
+    ) -> List[str]:
+        # TODO: update this so that it works faster (need some linux magic)
+        path_separator = "/"
+        with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
+            try:
+                t1 = time.time()
+                sftp_conn = conn.sftp()
+                sftp_conn.chdir(self.raw_path)
+                if search_in_sub_dirs:  # recursive globbing one level down
+                    sub_dirs = [
+                        f
+                        for f in sftp_conn.listdir()
+                        if stat.S_ISDIR(sftp_conn.stat(f).st_mode)
+                    ]
+                    files = [
+                        f
+                        for f in sftp_conn.listdir()
+                        if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)
+                    ]
+                    filtered_files = fnmatch.filter(files, glob_str)
+                    for sub_dir in sub_dirs:
+                        try:
+                            sftp_conn.chdir(sub_dir)
+                            new_files = [
+                                f
+                                for f in sftp_conn.listdir()
+                                if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)
+                            ]
+                            new_filtered_files = fnmatch.filter(new_files, glob_str)
+                            new_filtered_files = [
+                                f"{sub_dir}{path_separator}{f}"
+                                for f in new_filtered_files
+                            ]
+                            filtered_files += new_filtered_files
+                            sftp_conn.chdir("..")
+                        except FileNotFoundError:
+                            logging.debug(
+                                f"Could not look in {sub_dir}: FileNotFoundError"
+                            )
+                            pass
+                else:
+                    files = sftp_conn.listdir()
+                    filtered_files = fnmatch.filter(files, glob_str)
+                logging.debug(f"globbing took {time.time() - t1:.2f} seconds")
+                return filtered_files
+            except FileNotFoundError as e:
+                raise FileNotFoundError(
+                    f"Could not find file {self.raw_path} on {host}"
+                ) from e
```

### Comparing `cellpy-1.0.0a3/cellpy/log.py` & `cellpy-1.0.0a4/cellpy/log.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/logging.json` & `cellpy-1.0.0a4/cellpy/logging.json`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/parameters/.cellpy_prms_default.conf` & `cellpy-1.0.0a4/cellpy/parameters/.cellpy_prms_default.conf`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/parameters/internal_settings.py` & `cellpy-1.0.0a4/cellpy/parameters/internal_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Internal settings and definitions and functions for getting them."""
 import logging
 import warnings
 from collections import UserDict
-from dataclasses import dataclass, fields
+from dataclasses import dataclass, fields, asdict
 from typing import List, Optional
 
+import pandas as pd
+
 from cellpy import prms
 
 CELLPY_FILE_VERSION = 8
 MINIMUM_CELLPY_FILE_VERSION = 4
 STEP_TABLE_VERSION = 5
 RAW_TABLE_VERSION = 5
 SUMMARY_TABLE_VERSION = 7
@@ -111,14 +113,27 @@
                 logging.debug(f"{k} -> {v}")
                 setattr(self, k, v)
             else:
                 logging.debug(f"{k}:{v} ->")
                 not_digested[k] = v
         return not_digested
 
+    def to_frame(self):
+        """Converts to pandas dataframe"""
+        df = pd.DataFrame.from_dict(asdict(self), orient="index")
+        df.index.name = "key"
+        n_rows, n_cols = df.shape
+        if n_cols == 1:
+            columns = ["value"]
+        else:
+            columns = [f"value_{i:02}" for i in range(n_cols)]
+        df.columns = columns
+
+        return df
+
 
 @dataclass
 class CellpyMetaCommon(CellpyMeta):
     # about test
     cell_name: Optional[str] = None  # used as property
     start_datetime: Optional[str] = None
     time_zone: Optional[str] = None
```

### Comparing `cellpy-1.0.0a3/cellpy/parameters/legacy/update_headers.py` & `cellpy-1.0.0a4/cellpy/parameters/legacy/update_headers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/parameters/prmreader.py` & `cellpy-1.0.0a4/cellpy/parameters/prmreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/parameters/prms.py` & `cellpy-1.0.0a4/cellpy/parameters/prms.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/cellreader.py` & `cellpy-1.0.0a4/cellpy/readers/cellreader.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import csv
 import itertools
 import logging
 import numbers
 import os
 import sys
 import time
+import datetime
 import warnings
 from pathlib import Path
 from typing import Union, Sequence, List
 from dataclasses import asdict
 
 import numpy as np
 import pandas as pd
@@ -3085,14 +3086,15 @@
             txt += " Could not save it!"
             logging.debug(e)
             warnings.warn(f"Unhandled exception raised: {e}")
         logging.info(txt)
         logging.debug(f"(dt: {(time.time() - time_00):4.2f}s)")
 
     def _export_steptable(self, data, setname=None, sep=None, outname=None):
+        # TODO 259: rename to _export_steps_csv
         time_00 = time.time()
         lastname = "_steps.csv"
         if sep is None:
             sep = self.sep
         if outname is None:
             outname = setname + lastname
         txt = outname
@@ -3102,14 +3104,93 @@
         except Exception as e:
             txt += " Could not save it!"
             logging.debug(e)
             warnings.warn(f"Unhandled exception raised: {e}")
         logging.info(txt)
         logging.debug(f"(dt: {(time.time() - time_00):4.2f}s)")
 
+    def to_excel(self, filename=None, cycles=None, raw=False, steps=True):
+        """Saves the data as .xlsx file(s).
+
+        Args:
+            filename: name of the Excel file.
+            cycles: (None, bool, or list of ints) export voltage-capacity curves if given.
+            raw: (bool) export raw-data if True.
+            steps: (bool) export steps if True.
+        """
+        # TODO: allow for giving or extending to_excel_method_kwargs and get_cap_method_kwargs
+        #  currently hard-coded:
+        to_excel_method_kwargs = {"index": True, "header": True}
+        get_cap_method_kwargs = {
+            "method": "forth-and-forth",
+            "label_cycle_number": True,
+            "categorical_column": True,
+            "interpolated": True,
+            "number_of_points": 1000,
+            "capacity_then_voltage": True,
+        }
+
+        if filename is None:
+            pre = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
+            filename = f"{pre}_cellpy.xlsx"
+            filename = Path(filename).resolve()
+            logging.critical(f"generating filename: {filename}")
+
+        summary_frame = self.data.summary
+        meta_common_frame = self.data.meta_common.to_frame()
+        meta_test_dependent_frame = self.data.meta_test_dependent.to_frame()
+
+        with pd.ExcelWriter(filename, engine="openpyxl") as writer:
+            meta_common_frame.to_excel(
+                writer, sheet_name="meta_common", **to_excel_method_kwargs
+            )
+            meta_test_dependent_frame.to_excel(
+                writer, sheet_name="meta_test_dependent", **to_excel_method_kwargs
+            )
+            summary_frame.to_excel(
+                writer, sheet_name="summary", **to_excel_method_kwargs
+            )
+
+            if raw:
+                logging.debug("exporting raw data")
+                raw = self.data.raw
+                max_len = 1_048_576
+                if len(raw) < max_len:
+                    raw.to_excel(writer, sheet_name="raw", **to_excel_method_kwargs)
+                else:
+                    logging.warning(
+                        "Raw data is too large to fit in one sheet. "
+                        "Splitting raw data into chunks. This is not tested yet"
+                    )
+                    n_chunks = len(raw) // max_len + 1
+                    for i in range(n_chunks):
+                        raw.iloc[i * max_len : (i + 1) * max_len].to_excel(
+                            writer, sheet_name=f"raw_{i:02}", **to_excel_method_kwargs
+                        )
+
+            if steps:
+                logging.debug("exporting steps")
+                # TODO: step-table has a columns called "index" at the moment,
+                #  so setting index=False for dataframe.to_excel
+                #  Maybe best to make sure that step table does not have a column called "index" in the future?
+                self.data.steps.to_excel(
+                    writer, sheet_name="steps", index=False, header=True
+                )
+            if cycles:
+                logging.debug("exporting cycles")
+                if cycles is True:
+                    cycles = self.get_cycle_numbers()
+                for cycle in cycles:
+                    _curves = self.get_cap(cycle=cycle, **get_cap_method_kwargs)
+                    _curves.to_excel(
+                        writer,
+                        sheet_name=f"cycle_{cycle:03}",
+                        **to_excel_method_kwargs,
+                    )
+
     def to_csv(
         self,
         datadir=None,
         sep=None,
         cycles=False,
         raw=True,
         summary=True,
@@ -3765,30 +3846,31 @@
         return v
 
     def get_dcap(
         self,
         cycle=None,
         converter=None,
         mode="gravimetric",
-        return_dataframe=False,
+        return_dataframe=True,
         **kwargs,
     ):
-        """Returns discharge_capacity and voltage for the selected cycle
+        """Returns discharge-capacity and voltage for the selected cycle
         Args:
             cycle (int): cycle number.
-            converter (string): defaults to None.
-            mode (string): defaults to "gravimetric".
+            converter (float): a multiplication factor that converts the values to specific values (i.e.
+                from Ah to mAh/g). If not provided (or None), the factor is obtained from the
+                self.get_converter_to_specific() method.
+            mode (string): 'gravimetric', 'areal' or 'absolute'. Defaults to 'gravimetric'.
+                Used if converter is not provided (or None).
             return_dataframe (bool): if True: returns pd.DataFrame instead of capacity, voltage series.
+            **kwargs:
         Returns:
-            discharge_capacity, voltage (pd.Series).
+            discharge_capacity, voltage (pd.Series or pd.DataFrame if return_dataframe is True).
 
         """
-        # TODO: update docstring on purpose of "converter" and "mode"
-        #  TODO - jepe: should return a DataFrame as default
-        #   but remark that we then have to update e.g. batch_helpers.py
 
         if converter is None:
             converter = self.get_converter_to_specific(mode=mode)
 
         dc, v = self._get_cap(cycle, "discharge", converter=converter, **kwargs)
         if return_dataframe:
             cycle_df = pd.concat([v, dc], axis=1)
@@ -3797,30 +3879,30 @@
             return dc, v
 
     def get_ccap(
         self,
         cycle=None,
         converter=None,
         mode="gravimetric",
-        return_dataframe=False,
+        return_dataframe=True,
         **kwargs,
     ):
-        """Returns charge_capacity and voltage for the selected cycle.
+        """Returns charge-capacity and voltage for the selected cycle.
         Args:
             cycle (int): cycle number.
-            converter (string): defaults to None.
-            mode (string): defaults to "gravimetric".
+            converter (float): a multiplication factor that converts the values to specific values (i.e.
+                from Ah to mAh/g). If not provided (or None), the factor is obtained from the
+                self.get_converter_to_specific() method.
+            mode (string): 'gravimetric', 'areal' or 'absolute'. Defaults to 'gravimetric'.
+                Used if converter is not provided (or None).
             return_dataframe (bool): if True: returns pd.DataFrame instead of capacity, voltage series.
         Returns:
-            charge_capacity, voltage (pd.Series).
+            charge_capacity, voltage (pandas.Series or pandas.DataFrame if return_dataframe is True).
 
         """
-        # TODO: update docstring on purpose of "converter" and "mode"
-        # TODO - jepe: should return a DataFrame as default
-        #   (but remark that we then have to update e.g. batch_helpers.py)
 
         if converter is None:
             converter = self.get_converter_to_specific(mode=mode)
         cc, v = self._get_cap(cycle, "charge", converter=converter, **kwargs)
 
         if return_dataframe:
             cycle_df = pd.concat([v, cc], axis=1)
@@ -3840,14 +3922,15 @@
         interpolated=False,
         dx=0.1,
         number_of_points=None,
         ignore_errors=True,
         dynamic=False,
         inter_cycle_shift=True,
         interpolate_along_cap=False,
+        capacity_then_voltage=False,
         **kwargs,
     ):
         """Gets the capacity for the run.
 
         Args:
             cycle (int): cycle number.
             method (string): how the curves are given
@@ -3878,19 +3961,21 @@
             ignore_errors (bool): don't break out of loop if an error occurs.
             dynamic: for dynamic retrieving data from cellpy-file.
                 [NOT IMPLEMENTED YET]
             inter_cycle_shift (bool): cumulative shifts between consecutive
                 cycles. Defaults to True.
             interpolate_along_cap (bool): interpolate along capacity axis instead
                 of along the voltage axis. Defaults to False.
+            capacity_then_voltage (bool): return capacity and voltage instead of
+                voltage and capacity. Defaults to False.
 
         Returns:
             pandas.DataFrame ((cycle) voltage, capacity, (direction (-1, 1)))
             unless split is explicitly set to True. Then it returns a tuple
-            with capacity (mAh/g) and voltage.
+            with capacity and voltage.
         """
 
         # TODO: allow for fixing the interpolation range (so that it is possible
         #   to run the function on several cells and have a common x-axis
 
         # if cycle is not given, then this function should
         # iterate through cycles
@@ -3927,19 +4012,21 @@
         initial = True
         for current_cycle in cycle:
             error = False
             try:
                 cc, cv = self.get_ccap(
                     current_cycle,
                     converter=specific_converter,
+                    return_dataframe=False,
                     **kwargs,
                 )
                 dc, dv = self.get_dcap(
                     current_cycle,
                     converter=specific_converter,
+                    return_dataframe=False,
                     **kwargs,
                 )
 
             except NullData as e:
                 error = True
                 logging.debug(e)
                 if not ignore_errors:
@@ -4087,15 +4174,19 @@
                             c.insert(0, "cycle", current_cycle)
                             # c["cycle"] = current_cycle
                             # c = c[["cycle", "voltage", "capacity", "direction"]]
                         if cycle_df.empty:
                             cycle_df = c
                         else:
                             cycle_df = pd.concat([cycle_df, c], axis=0)
-
+                    if capacity_then_voltage:
+                        cols = cycle_df.columns.to_list()
+                        new_cols = [cols.pop(cols.index("capacity")), cols.pop(cols.index("voltage"))]
+                        new_cols.extend(cols)
+                        cycle_df = cycle_df[new_cols]
                 else:
                     logging.warning("returning non-dataframe")
                     c = pd.concat([_first_step_c, _last_step_c], axis=0)
                     v = pd.concat([_first_step_v, _last_step_v], axis=0)
 
                     capacity = pd.concat([capacity, c], axis=0)
                     voltage = pd.concat([voltage, v], axis=0)
@@ -5914,9 +6005,30 @@
                 print(f"{a}: {v}")
     # print("Here we have it")
     # print(c.data.summary.columns)
     # print(c.data.steps.columns)
     # print(c.data.raw.columns)
 
 
+def load_and_save_to_excel():
+    from pathlib import Path
+
+    print(" loading cellpy file and saving to excel ".center(80, "="))
+
+    raw_file = Path("../../testdata/data/20160805_test001_45_cc_01.res")
+    cellpy_file = Path("../../tmp/20160805_test001_45_cc.h5")
+    excel_file = Path("../../tmp/20160805_test001_45_cc.xlsx")
+
+    c = get(raw_file, mass=1.0, nominal_capacity=3579)
+    print("loaded ...")
+    c.to_excel(excel_file)
+    print("saved ...")
+
+    c.save(cellpy_file)
+    c2 = get(cellpy_file)
+    print("loaded again ...")
+    c2.to_excel(excel_file, raw=True, cycles=True)
+    print("saved again ...")
+
+
 if __name__ == "__main__":
-    save_and_load_cellpy_file()
+    load_and_save_to_excel()
```

### Comparing `cellpy-1.0.0a3/cellpy/readers/core.py` & `cellpy-1.0.0a4/cellpy/readers/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -848,21 +848,23 @@
         try:
             if direction == "charge":
                 q, v = cell.get_ccap(
                     cycle,
                     trim_taper_steps=trim_taper_steps,
                     steps_to_skip=steps_to_skip,
                     steptable=steptable,
+                    return_dataframe=False,
                 )
             else:
                 q, v = cell.get_dcap(
                     cycle,
                     trim_taper_steps=trim_taper_steps,
                     steps_to_skip=steps_to_skip,
                     steptable=steptable,
+                    return_dataframe=False,
                 )
 
         except NullData as e:
             logging.warning(e)
             d = pd.DataFrame()
             d.name = cycle
             charge_list.append(d)
```

### Comparing `cellpy-1.0.0a3/cellpy/readers/dbreader.py` & `cellpy-1.0.0a4/cellpy/readers/dbreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/filefinder.py` & `cellpy-1.0.0a4/cellpy/readers/filefinder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,355 +1,356 @@
-# -*- coding: utf-8 -*-
-
-import fnmatch
-import glob
-import logging
-import os
-import pathlib
-import time
-from typing import Optional, Union, List, Tuple
-import warnings
-
-import cellpy.exceptions
-from cellpy.parameters import prms
-from cellpy.internals.core import OtherPath
-
-
-# TODO: @jepe - add function for dumping the raw-file directory to a file,
-#   for example an sqlite db or a json file,
-#   and add function for reading and searching in the dumped file
-
-# TODO: @jepe - add function for searching in cloud storage (dropbox, google drive etc)
-# TODO: @jepe - add function for searching in database (sqlite, postgresql etc)
-
-def list_raw_file_directory(
-    raw_file_dir: Union[OtherPath, pathlib.Path, str, None] = None,
-    project_dir: Union[OtherPath, pathlib.Path, str, None] = None,
-    extension: Optional[str] = None,
-    levels: Optional[int] = 1,
-    only_filename: Optional[bool] = False,
-    with_prefix: Optional[bool] = True,
-):
-    """Dumps the raw-file directory to a list.
-
-    Args:
-        raw_file_dir(path): optional, directory where to look for run-files
-            (default: read prm-file)
-        project_dir(path): optional, subdirectory in raw_file_dir to look for run-files
-        extension (str): optional, extension of run-files (without the '.'). If
-            not given, all files will be listed.
-        levels (int, optional): How many sublevels to list. Defaults to 1.
-            If you want to list all sublevels, use `listdir(levels=-1)`.
-            If you want to list only the current level (no subdirectories),
-            use `listdir(levels=0)`.
-        only_filename (bool, optional): If True, only the file names will be
-            returned. Defaults to False.
-        with_prefix (bool, optional): If True, the full path to the files including
-            the prefix and the location (e.g. 'scp://user@server.com/...')
-            will be returned. Defaults to True.
-
-    Returns:
-        list of str: list of file paths (only the actual file names).
-
-    Notes:
-        This function might be rather slow and memory consuming if you have
-        a lot of files in your raw-file directory. If you have a lot of files,
-        you might want to consider running this function in a separate process
-        (e.g. in a separate python script or using multiprocessing).
-
-        The function currently returns the full path to the files from the
-        root directory. It does not include the prefix (e.g. ssh://).
-        Future versions might change this to either include the prefix or
-        return the files relative to the ``raw_file_dir`` directory.
-    """
-
-    file_list = []
-
-    if raw_file_dir is None:
-        raw_file_dir = prms.Paths.rawdatadir
-
-    # 'dressing' the raw_file_dir in a list in case we want to
-    # search in several folders (not implemented yet):
-    if not isinstance(raw_file_dir, (list, tuple)):
-        raw_file_dir = [OtherPath(raw_file_dir)]
-    else:
-        raw_file_dir = [OtherPath(d) for d in raw_file_dir]
-
-    if project_dir is not None:
-        raw_file_dir = [r / project_dir for r in raw_file_dir]
-
-    for d in raw_file_dir:
-        _file_list = d.listdir(levels=levels)
-        if extension is not None:
-            logging.debug(f"filtering for extension: {extension}")
-            _file_list = fnmatch.filter(_file_list, f"*.{extension}")
-        if only_filename:
-            logging.debug("only returning the file names")
-            _file_list = [f.name for f in _file_list]
-        elif with_prefix:
-            logging.debug("adding prefix to file names")
-            logging.debug(f"{d.pathlike_location=}")
-            _file_list = [d.pathlike_location / f for f in _file_list]
-
-        file_list.extend(_file_list)
-
-    return file_list
-
-
-def search_for_files(
-    run_name: str,
-    raw_extension: Optional[str] = None,
-    cellpy_file_extension: Optional[str] = None,
-    raw_file_dir: Union[OtherPath, pathlib.Path, str, None] = None,
-    project_dir: Union[OtherPath, pathlib.Path, str, None] = None,
-    cellpy_file_dir: Union[OtherPath, pathlib.Path, str, None] = None,
-    prm_filename: Union[pathlib.Path, str, None] = None,
-    file_name_format: Optional[str] = None,
-    reg_exp: Optional[str] = None,
-    sub_folders: Optional[bool] = True,
-    file_list: Optional[List[str]] = None,
-    pre_path: Union[OtherPath, pathlib.Path, str, None] = None,
-) -> Tuple[List[str], str]:
-    """Searches for files (raw-data files and cellpy-files).
-
-
-    Args:
-        run_name(str): run-file identification.
-        raw_extension(str): optional, extension of run-files (without the '.').
-        cellpy_file_extension(str): optional, extension for cellpy files
-            (without the '.').
-        raw_file_dir(path): optional, directory where to look for run-files
-            (default: read prm-file)
-        project_dir(path): optional, subdirectory in raw_file_dir to look for run-files
-            (default: read prm-file)
-        cellpy_file_dir(path): optional, directory where to look for
-            cellpy-files (default: read prm-file)
-        prm_filename(path): optional parameter file can be given.
-        file_name_format(str): format of raw-file names or a glob pattern
-            (default: YYYYMMDD_[name]EEE_CC_TT_RR).
-        reg_exp(str): use regular expression instead (defaults to None).
-        sub_folders (bool): perform search also in sub-folders.
-        file_list (list of str): perform the search within a given list
-            of filenames instead of searching the folder(s). The list should
-            not contain the full filepath (only the actual file names). If
-            you want to provide the full path, you will have to modify the
-            file_name_format or reg_exp accordingly.
-        pre_path (path or str): path to prepend the list of files selected
-             from the file_list.
-
-
-    Returns:
-        run-file names (list of strings) and cellpy-file-name (str of full path).
-    """
-
-    # TODO: @jepe - use reg_exp
-    # TODO: @jepe - allow for searching in cloud
-    # TODO: @jepe - how to implement searching in db?
-    # TODO: update prms and conf file to allow for setting if search should be done in
-    #  sub-folders, several folders, db, cloud etc
-    # TODO: @jepe - find a way to implement automatic file_list creation in a top level func.
-    logging.debug(f"searching for {run_name}")
-    version = 0.4
-    t0 = time.time()
-
-    if reg_exp is None:
-        reg_exp = prms.FileNames.reg_exp
-
-    if raw_extension is None:
-        raw_extension = prms.FileNames.raw_extension
-
-    if raw_extension is None:
-        raw_extension = prms.FileNames.raw_extension
-
-    if cellpy_file_extension is None:
-        cellpy_file_extension = prms.FileNames.cellpy_file_extension
-
-    # backward compatibility check:
-    if cellpy_file_extension.startswith("."):
-        warnings.warn(
-            "Deprecation warning: cellpy_file_extension should not include the '.'"
-        )
-        cellpy_file_extension = cellpy_file_extension[1:]
-
-    if raw_file_dir is None:
-        raw_file_dir = prms.Paths.rawdatadir
-
-    if file_name_format is None:
-        file_name_format = prms.FileNames.file_name_format
-
-    # 'dressing' the raw_file_dir in a list in case we want to
-    # search in several folders (not implemented yet):
-    if not isinstance(raw_file_dir, (list, tuple)):
-        raw_file_dir = [OtherPath(raw_file_dir)]
-    else:
-        raw_file_dir = [OtherPath(d) for d in raw_file_dir]
-
-    if project_dir is not None:
-        raw_file_dir = [r / project_dir for r in raw_file_dir]
-
-    if reg_exp:
-        logging.warning(f"Got reg_exp: {reg_exp}")
-        logging.warning("Sorry, but using reg exp is not implemented yet.")
-
-    if prm_filename is not None:
-        logging.debug("Sorry, reading prm file is not implemented yet.")
-
-    if cellpy_file_dir is None:
-        cellpy_file_dir = OtherPath(prms.Paths.cellpydatadir)
-    else:
-        cellpy_file_dir = OtherPath(cellpy_file_dir)
-
-    if file_name_format is None and reg_exp is None:
-        try:
-            # To be implemented in version 0.5:
-            file_name_format = prms.FileNames.file_name_format
-        except AttributeError:
-            file_name_format = "YYYYMMDD_[name]EEE_CC_TT_RR"
-
-    if file_name_format.upper() == "YYYYMMDD_[NAME]EEE_CC_TT_RR":
-        # backward compatibility check
-        if raw_extension.startswith("."):
-            warnings.warn(
-                "Deprecation warning: raw_extension should not include the '.'"
-            )
-            raw_extension = raw_extension[1:]
-            warnings.warn(f"Removing it -> {raw_extension}")
-        # TODO: give warning/error-message if run_name contains more than one file (due to duplicate in db)
-        glob_text_raw = f"{run_name}*.{raw_extension}"
-    else:
-        glob_text_raw = file_name_format
-
-    logging.debug(f"searching for raw files in: {raw_file_dir}")
-    logging.debug(f"searching for {run_name}")
-    logging.debug(f"using glob {glob_text_raw}")
-
-    cellpy_file = f"{run_name}.{cellpy_file_extension}"
-    cellpy_file = cellpy_file_dir / cellpy_file
-    # Not sure if for example pandas can handle OtherPath objects:
-    cellpy_file = cellpy_file.full_path
-
-    logging.debug(f"generated cellpy filename {cellpy_file}")
-
-    if file_list is not None:
-        if len(raw_file_dir) > 1:
-            logging.info("you provided several raw file directories")
-        logging.debug("searching within provided list of files")
-        run_files = fnmatch.filter(file_list, glob_text_raw)
-        if pre_path is not None:
-            pre_path = OtherPath(pre_path)
-            run_files = list(map(lambda x: pre_path / x, run_files))
-    else:
-        run_files = []
-        for d in raw_file_dir:
-            if d.is_external:
-                logging.debug("external file")
-            if not d.is_dir():
-                warnings.warn("your raw file directory cannot be accessed!")
-                # raise cellpy.exceptions.IOError("your raw file directory cannot be accessed!")
-                _run_files = []
-            else:
-                logging.debug(f"checking in folder {d}")
-                logging.debug(f"{sub_folders=}")
-                if sub_folders:
-                    _run_files = d.rglob(glob_text_raw)
-
-                else:
-                    _run_files = d.glob(glob_text_raw)
-
-                _run_files = [str(_f.resolve()) for _f in _run_files]
-                _run_files.sort()
-            run_files.extend(_run_files)
-
-    return run_files, cellpy_file
-
-
-def check_01():
-    import dotenv
-    from cellpy import log
-
-    log.setup_logging(default_level="DEBUG")
-    dotenv.load_dotenv(r"C:\scripting\cellpy\local\.env_cellpy_local")
-    print("searching for files")
-    my_run_name = "20160805_test001_45_cc"
-    # my_run_name = "20210218_Seam08_02_01_cc"
-    my_raw_file_dir = OtherPath(
-        f"scp://{os.getenv('CELLPY_HOST')}/home/{os.getenv('CELLPY_USER')}/tmp/"
-    )
-    # my_raw_file_dir = OtherPath(r"C:\scripting\processing_cellpy\raw")
-    my_cellpy_file_dir = OtherPath("C:/scripting/processing_cellpy/data/")
-    f = search_for_files(
-        my_run_name, raw_file_dir=my_raw_file_dir, cellpy_file_dir=my_cellpy_file_dir
-    )
-    print(f)
-    #
-    # print(my_raw_file_dir)
-    # print(my_raw_file_dir.is_dir())
-    # print(my_raw_file_dir.raw_path)
-
-
-def check_02():
-    import dotenv
-    import fabric
-    import stat
-
-    dotenv.load_dotenv(r"C:\scripting\cellpy\local\.env_cellpy_local")
-    host = os.getenv("CELLPY_HOST")
-    user = os.getenv("CELLPY_USER")
-    key_file = os.getenv("CELLPY_KEY_FILENAME")
-    print(f"host: {host}")
-    print(f"user: {user}")
-    connect_kwargs = {"key_filename": key_file}
-
-    with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
-        sftp_conn = conn.sftp()
-        sftp_conn.chdir("tmp")
-        print("===================")
-        for fileattr in sftp_conn.listdir_attr():
-            if stat.S_ISDIR(fileattr.st_mode):
-                print(f"dir: {fileattr.filename}")
-            else:
-                print(f"file: {fileattr.filename}")
-        print("===================")
-        glob_str = "20*.res"
-        sub_dirs = [
-            f for f in sftp_conn.listdir() if stat.S_ISDIR(sftp_conn.stat(f).st_mode)
-        ]
-        files = [
-            f
-            for f in sftp_conn.listdir()
-            if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)
-        ]
-        filtered_files = fnmatch.filter(files, glob_str)
-        for sub_dir in sub_dirs:
-            sftp_conn.chdir(sub_dir)
-            new_files = [
-                f
-                for f in sftp_conn.listdir()
-                if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)
-            ]
-            new_filtered_files = fnmatch.filter(new_files, glob_str)
-            new_filtered_files = [
-                f"{sub_dir}{path_separator}{f}" for f in new_filtered_files
-            ]
-            filtered_files += new_filtered_files
-            sftp_conn.chdir("..")
-
-        for f in filtered_files:
-            print(f"file: {f} of type {type(f)}")
-
-
-def check_03():
-    from cellpy import prms
-    from pprint import pprint
-
-    prms.Paths.rawdatadir = r"C:\scripting\processing_cellpy\raw"
-    file_list = list_raw_file_directory(
-        raw_file_dir=None,
-        project_dir=None,
-        extension="hei",
-    )
-    for f in file_list:
-        print(f"{f} type: {type(f)} path: {f.full_path}")
-
-
-if __name__ == "__main__":
-    check_03()
+# -*- coding: utf-8 -*-
+
+import fnmatch
+import glob
+import logging
+import os
+import pathlib
+import time
+from typing import Optional, Union, List, Tuple
+import warnings
+
+import cellpy.exceptions
+from cellpy.parameters import prms
+from cellpy.internals.core import OtherPath
+
+
+# TODO: @jepe - add function for dumping the raw-file directory to a file,
+#   for example an sqlite db or a json file,
+#   and add function for reading and searching in the dumped file
+
+# TODO: @jepe - add function for searching in cloud storage (dropbox, google drive etc)
+# TODO: @jepe - add function for searching in database (sqlite, postgresql etc)
+
+
+def list_raw_file_directory(
+    raw_file_dir: Union[OtherPath, pathlib.Path, str, None] = None,
+    project_dir: Union[OtherPath, pathlib.Path, str, None] = None,
+    extension: Optional[str] = None,
+    levels: Optional[int] = 1,
+    only_filename: Optional[bool] = False,
+    with_prefix: Optional[bool] = True,
+):
+    """Dumps the raw-file directory to a list.
+
+    Args:
+        raw_file_dir(path): optional, directory where to look for run-files
+            (default: read prm-file)
+        project_dir(path): optional, subdirectory in raw_file_dir to look for run-files
+        extension (str): optional, extension of run-files (without the '.'). If
+            not given, all files will be listed.
+        levels (int, optional): How many sublevels to list. Defaults to 1.
+            If you want to list all sublevels, use `listdir(levels=-1)`.
+            If you want to list only the current level (no subdirectories),
+            use `listdir(levels=0)`.
+        only_filename (bool, optional): If True, only the file names will be
+            returned. Defaults to False.
+        with_prefix (bool, optional): If True, the full path to the files including
+            the prefix and the location (e.g. 'scp://user@server.com/...')
+            will be returned. Defaults to True.
+
+    Returns:
+        list of str: list of file paths (only the actual file names).
+
+    Notes:
+        This function might be rather slow and memory consuming if you have
+        a lot of files in your raw-file directory. If you have a lot of files,
+        you might want to consider running this function in a separate process
+        (e.g. in a separate python script or using multiprocessing).
+
+        The function currently returns the full path to the files from the
+        root directory. It does not include the prefix (e.g. ssh://).
+        Future versions might change this to either include the prefix or
+        return the files relative to the ``raw_file_dir`` directory.
+    """
+
+    file_list = []
+
+    if raw_file_dir is None:
+        raw_file_dir = prms.Paths.rawdatadir
+
+    # 'dressing' the raw_file_dir in a list in case we want to
+    # search in several folders (not implemented yet):
+    if not isinstance(raw_file_dir, (list, tuple)):
+        raw_file_dir = [OtherPath(raw_file_dir)]
+    else:
+        raw_file_dir = [OtherPath(d) for d in raw_file_dir]
+
+    if project_dir is not None:
+        raw_file_dir = [r / project_dir for r in raw_file_dir]
+
+    for d in raw_file_dir:
+        _file_list = d.listdir(levels=levels)
+        if extension is not None:
+            logging.debug(f"filtering for extension: {extension}")
+            _file_list = fnmatch.filter(_file_list, f"*.{extension}")
+        if only_filename:
+            logging.debug("only returning the file names")
+            _file_list = [f.name for f in _file_list]
+        elif with_prefix:
+            logging.debug("adding prefix to file names")
+            logging.debug(f"{d.pathlike_location=}")
+            _file_list = [d.pathlike_location / f for f in _file_list]
+
+        file_list.extend(_file_list)
+
+    return file_list
+
+
+def search_for_files(
+    run_name: str,
+    raw_extension: Optional[str] = None,
+    cellpy_file_extension: Optional[str] = None,
+    raw_file_dir: Union[OtherPath, pathlib.Path, str, None] = None,
+    project_dir: Union[OtherPath, pathlib.Path, str, None] = None,
+    cellpy_file_dir: Union[OtherPath, pathlib.Path, str, None] = None,
+    prm_filename: Union[pathlib.Path, str, None] = None,
+    file_name_format: Optional[str] = None,
+    reg_exp: Optional[str] = None,
+    sub_folders: Optional[bool] = True,
+    file_list: Optional[List[str]] = None,
+    pre_path: Union[OtherPath, pathlib.Path, str, None] = None,
+) -> Tuple[List[str], str]:
+    """Searches for files (raw-data files and cellpy-files).
+
+
+    Args:
+        run_name(str): run-file identification.
+        raw_extension(str): optional, extension of run-files (without the '.').
+        cellpy_file_extension(str): optional, extension for cellpy files
+            (without the '.').
+        raw_file_dir(path): optional, directory where to look for run-files
+            (default: read prm-file)
+        project_dir(path): optional, subdirectory in raw_file_dir to look for run-files
+            (default: read prm-file)
+        cellpy_file_dir(path): optional, directory where to look for
+            cellpy-files (default: read prm-file)
+        prm_filename(path): optional parameter file can be given.
+        file_name_format(str): format of raw-file names or a glob pattern
+            (default: YYYYMMDD_[name]EEE_CC_TT_RR).
+        reg_exp(str): use regular expression instead (defaults to None).
+        sub_folders (bool): perform search also in sub-folders.
+        file_list (list of str): perform the search within a given list
+            of filenames instead of searching the folder(s). The list should
+            not contain the full filepath (only the actual file names). If
+            you want to provide the full path, you will have to modify the
+            file_name_format or reg_exp accordingly.
+        pre_path (path or str): path to prepend the list of files selected
+             from the file_list.
+
+
+    Returns:
+        run-file names (list of strings) and cellpy-file-name (str of full path).
+    """
+
+    # TODO: @jepe - use reg_exp
+    # TODO: @jepe - allow for searching in cloud
+    # TODO: @jepe - how to implement searching in db?
+    # TODO: update prms and conf file to allow for setting if search should be done in
+    #  sub-folders, several folders, db, cloud etc
+    # TODO: @jepe - find a way to implement automatic file_list creation in a top level func.
+    logging.debug(f"searching for {run_name}")
+    version = 0.4
+    t0 = time.time()
+
+    if reg_exp is None:
+        reg_exp = prms.FileNames.reg_exp
+
+    if raw_extension is None:
+        raw_extension = prms.FileNames.raw_extension
+
+    if raw_extension is None:
+        raw_extension = prms.FileNames.raw_extension
+
+    if cellpy_file_extension is None:
+        cellpy_file_extension = prms.FileNames.cellpy_file_extension
+
+    # backward compatibility check:
+    if cellpy_file_extension.startswith("."):
+        warnings.warn(
+            "Deprecation warning: cellpy_file_extension should not include the '.'"
+        )
+        cellpy_file_extension = cellpy_file_extension[1:]
+
+    if raw_file_dir is None:
+        raw_file_dir = prms.Paths.rawdatadir
+
+    if file_name_format is None:
+        file_name_format = prms.FileNames.file_name_format
+
+    # 'dressing' the raw_file_dir in a list in case we want to
+    # search in several folders (not implemented yet):
+    if not isinstance(raw_file_dir, (list, tuple)):
+        raw_file_dir = [OtherPath(raw_file_dir)]
+    else:
+        raw_file_dir = [OtherPath(d) for d in raw_file_dir]
+
+    if project_dir is not None:
+        raw_file_dir = [r / project_dir for r in raw_file_dir]
+
+    if reg_exp:
+        logging.warning(f"Got reg_exp: {reg_exp}")
+        logging.warning("Sorry, but using reg exp is not implemented yet.")
+
+    if prm_filename is not None:
+        logging.debug("Sorry, reading prm file is not implemented yet.")
+
+    if cellpy_file_dir is None:
+        cellpy_file_dir = OtherPath(prms.Paths.cellpydatadir)
+    else:
+        cellpy_file_dir = OtherPath(cellpy_file_dir)
+
+    if file_name_format is None and reg_exp is None:
+        try:
+            # To be implemented in version 0.5:
+            file_name_format = prms.FileNames.file_name_format
+        except AttributeError:
+            file_name_format = "YYYYMMDD_[name]EEE_CC_TT_RR"
+
+    if file_name_format.upper() == "YYYYMMDD_[NAME]EEE_CC_TT_RR":
+        # backward compatibility check
+        if raw_extension.startswith("."):
+            warnings.warn(
+                "Deprecation warning: raw_extension should not include the '.'"
+            )
+            raw_extension = raw_extension[1:]
+            warnings.warn(f"Removing it -> {raw_extension}")
+        # TODO: give warning/error-message if run_name contains more than one file (due to duplicate in db)
+        glob_text_raw = f"{run_name}*.{raw_extension}"
+    else:
+        glob_text_raw = file_name_format
+
+    logging.debug(f"searching for raw files in: {raw_file_dir}")
+    logging.debug(f"searching for {run_name}")
+    logging.debug(f"using glob {glob_text_raw}")
+
+    cellpy_file = f"{run_name}.{cellpy_file_extension}"
+    cellpy_file = cellpy_file_dir / cellpy_file
+    # Not sure if for example pandas can handle OtherPath objects:
+    cellpy_file = cellpy_file.full_path
+
+    logging.debug(f"generated cellpy filename {cellpy_file}")
+
+    if file_list is not None:
+        if len(raw_file_dir) > 1:
+            logging.info("you provided several raw file directories")
+        logging.debug("searching within provided list of files")
+        run_files = fnmatch.filter(file_list, glob_text_raw)
+        if pre_path is not None:
+            pre_path = OtherPath(pre_path)
+            run_files = list(map(lambda x: pre_path / x, run_files))
+    else:
+        run_files = []
+        for d in raw_file_dir:
+            if d.is_external:
+                logging.debug("external file")
+            if not d.is_dir():
+                warnings.warn("your raw file directory cannot be accessed!")
+                # raise cellpy.exceptions.IOError("your raw file directory cannot be accessed!")
+                _run_files = []
+            else:
+                logging.debug(f"checking in folder {d}")
+                logging.debug(f"{sub_folders=}")
+                if sub_folders:
+                    _run_files = d.rglob(glob_text_raw)
+
+                else:
+                    _run_files = d.glob(glob_text_raw)
+
+                _run_files = [str(_f.resolve()) for _f in _run_files]
+                _run_files.sort()
+            run_files.extend(_run_files)
+
+    return run_files, cellpy_file
+
+
+def check_01():
+    import dotenv
+    from cellpy import log
+
+    log.setup_logging(default_level="DEBUG")
+    dotenv.load_dotenv(r"C:\scripting\cellpy\local\.env_cellpy_local")
+    print("searching for files")
+    my_run_name = "20160805_test001_45_cc"
+    # my_run_name = "20210218_Seam08_02_01_cc"
+    my_raw_file_dir = OtherPath(
+        f"scp://{os.getenv('CELLPY_HOST')}/home/{os.getenv('CELLPY_USER')}/tmp/"
+    )
+    # my_raw_file_dir = OtherPath(r"C:\scripting\processing_cellpy\raw")
+    my_cellpy_file_dir = OtherPath("C:/scripting/processing_cellpy/data/")
+    f = search_for_files(
+        my_run_name, raw_file_dir=my_raw_file_dir, cellpy_file_dir=my_cellpy_file_dir
+    )
+    print(f)
+    #
+    # print(my_raw_file_dir)
+    # print(my_raw_file_dir.is_dir())
+    # print(my_raw_file_dir.raw_path)
+
+
+def check_02():
+    import dotenv
+    import fabric
+    import stat
+
+    dotenv.load_dotenv(r"C:\scripting\cellpy\local\.env_cellpy_local")
+    host = os.getenv("CELLPY_HOST")
+    user = os.getenv("CELLPY_USER")
+    key_file = os.getenv("CELLPY_KEY_FILENAME")
+    print(f"host: {host}")
+    print(f"user: {user}")
+    connect_kwargs = {"key_filename": key_file}
+
+    with fabric.Connection(host, connect_kwargs=connect_kwargs) as conn:
+        sftp_conn = conn.sftp()
+        sftp_conn.chdir("tmp")
+        print("===================")
+        for fileattr in sftp_conn.listdir_attr():
+            if stat.S_ISDIR(fileattr.st_mode):
+                print(f"dir: {fileattr.filename}")
+            else:
+                print(f"file: {fileattr.filename}")
+        print("===================")
+        glob_str = "20*.res"
+        sub_dirs = [
+            f for f in sftp_conn.listdir() if stat.S_ISDIR(sftp_conn.stat(f).st_mode)
+        ]
+        files = [
+            f
+            for f in sftp_conn.listdir()
+            if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)
+        ]
+        filtered_files = fnmatch.filter(files, glob_str)
+        for sub_dir in sub_dirs:
+            sftp_conn.chdir(sub_dir)
+            new_files = [
+                f
+                for f in sftp_conn.listdir()
+                if not stat.S_ISDIR(sftp_conn.stat(f).st_mode)
+            ]
+            new_filtered_files = fnmatch.filter(new_files, glob_str)
+            new_filtered_files = [
+                f"{sub_dir}{path_separator}{f}" for f in new_filtered_files
+            ]
+            filtered_files += new_filtered_files
+            sftp_conn.chdir("..")
+
+        for f in filtered_files:
+            print(f"file: {f} of type {type(f)}")
+
+
+def check_03():
+    from cellpy import prms
+    from pprint import pprint
+
+    prms.Paths.rawdatadir = r"C:\scripting\processing_cellpy\raw"
+    file_list = list_raw_file_directory(
+        raw_file_dir=None,
+        project_dir=None,
+        extension="hei",
+    )
+    for f in file_list:
+        print(f"{f} type: {type(f)} path: {f.full_path}")
+
+
+if __name__ == "__main__":
+    check_03()
```

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/arbin_res.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/arbin_res.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql_7.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql_7.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql_csv.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql_csv.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql_h5.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql_h5.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/arbin_sql_xlsx.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql_xlsx.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/base.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/base.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/biologics_mpr.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/biologics_mpr.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/configurations/__init__.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_four.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_four.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_one.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_one.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_three.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_three.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_two.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_two.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/configurations/maccor_txt_zero.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_zero.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/configurations/neware_txt_zero.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/configurations/neware_txt_zero.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/custom.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/custom.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/ext_nda_reader.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/ext_nda_reader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/local_instrument.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/local_instrument.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/maccor_txt.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/maccor_txt.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/neware_txt.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/neware_txt.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/pec_csv.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/pec_csv.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/processors/post_processors.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/processors/post_processors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/instruments/processors/pre_processors.py` & `cellpy-1.0.0a4/cellpy/readers/instruments/processors/pre_processors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/readers/sql_dbreader.py` & `cellpy-1.0.0a4/cellpy/readers/sql_dbreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/batch.py` & `cellpy-1.0.0a4/cellpy/utils/batch.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_analyzers.py` & `cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_analyzers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_core.py` & `cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_core.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_experiments.py` & `cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_experiments.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,995 +1,1002 @@
-import ast
-import logging
-import os
-import pathlib
-import sys
-import warnings
-
-import pandas as pd
-from tqdm.auto import tqdm
-
-import cellpy
-from cellpy import prms
-from cellpy.parameters.internal_settings import get_headers_journal, get_headers_summary
-from cellpy.readers import cellreader
-from cellpy.internals.core import OtherPath
-from cellpy.utils.batch_tools import batch_helpers as helper
-from cellpy.utils.batch_tools.batch_core import BaseExperiment
-from cellpy.utils.batch_tools.batch_journals import LabJournal
-
-hdr_journal = get_headers_journal()
-hdr_summary = get_headers_summary()
-
-
-class CyclingExperiment(BaseExperiment):
-    """Load experimental data into memory.
-
-    This is a re-implementation of the old batch behaviour where
-    all the data-files are processed sequentially (and optionally exported)
-    while the summary tables are kept and processed. This implementation
-    also saves the step tables (for later use when using look-up
-    functionality).
-
-
-    Attributes:
-        journal (:obj: LabJournal): information about the experiment.
-        force_cellpy (bool): tries only to load the cellpy-file if True.
-        force_raw (bool): loads raw-file(s) even though appropriate cellpy-file
-           exists if True.
-        save_cellpy (bool): saves a cellpy-file for each cell if True.
-        accept_errors (bool): in case of error, dont raise an exception, but
-           continue to the next file if True.
-        all_in_memory (bool): store the cellpydata-objects in memory if True.
-        export_cycles (bool): export voltage-capacity curves if True.
-        shifted_cycles (bool): set this to True if you want to export the
-           voltage-capacity curves using the shifted-cycles option (only valid
-           if you set export_cycles to True).
-        export_raw (bool): export the raw-data if True.
-        export_ica (bool): export dq-dv curves if True.
-        last_cycle (int): sets the last cycle (i.e. the highest cycle number)
-           that you would like to process dq-dv on). Use all if None (the
-           default value).
-        selected_summaries (list): a list of summary labels defining what
-           summary columns to make joint summaries from (optional).
-        errors (dict): contains a dictionary listing all the errors encountered.
-
-    Args:
-        db_reader (str or object): custom db_reader (see doc on db_reader).
-
-    Example:
-
-
-    """
-
-    def __init__(self, *args, **kwargs):
-        db_reader = kwargs.pop("db_reader", "default")
-        super().__init__(*args)
-        self.journal = LabJournal(db_reader=db_reader)
-        self.errors = dict()
-        self.log = dict()
-
-        self.force_cellpy = False
-        self.force_raw = False
-        self.force_recalc = False
-        self.save_cellpy = True
-        self.accept_errors = False
-        self.all_in_memory = False
-
-        self.export_cycles = False
-        self.shifted_cycles = False
-        self.export_raw = True
-        self.export_ica = False
-        self.last_cycle = None
-        self.nom_cap = None
-        self.instrument = None
-        self.custom_data_folder = None
-
-        self.selected_summaries = None
-
-    def _repr_html_(self):
-        txt = f"<h2>CyclingExperiment-object</h2> id={hex(id(self))}"
-        txt += "<h3>Main attributes</h3>"
-        txt += f"""
-        <table>
-            <thead>
-                <tr>
-                    <th>Attribute</th>
-                    <th>Value</th>
-                </tr>
-            </thead>
-            <tbody>
-                <tr><td><b>force_cellpy</b></td><td>{self.force_cellpy}</td></tr>
-                <tr><td><b>force_raw</b></td><td>{self.force_raw}</td></tr>
-                <tr><td><b>force_recalc</b></td><td>{self.force_recalc}</td></tr>
-                <tr><td><b>save_cellpy</b></td><td>{self.save_cellpy}</td></tr>
-                <tr><td><b>accept_errors</b></td><td>{self.accept_errors}</td></tr>
-                <tr><td><b>all_in_memory</b></td><td>{self.all_in_memory}</td></tr>
-                <tr><td><b>export_cycles</b></td><td>{self.export_cycles}</td></tr>
-                <tr><td><b>shifted_cycles</b></td><td>{self.shifted_cycles}</td></tr>
-                <tr><td><b>export_raw</b></td><td>{self.export_raw}</td></tr>
-                <tr><td><b>export_ica</b></td><td>{self.export_ica}</td></tr>
-                <tr><td><b>last_cycle</b></td><td>{self.last_cycle}</td></tr>
-                <tr><td><b>nom_cap</b></td><td>{self.nom_cap}</td></tr>
-                <tr><td><b>instrument</b></td><td>{self.instrument}</td></tr>
-                <tr><td><b>custom_data_folder</b></td><td>{self.custom_data_folder}</td></tr>
-                <tr><td><b>selected_summaries</b></td><td>{self.selected_summaries}</td></tr>
-            </tbody>
-        </table>
-        """
-        txt += "<h3>Cells</h3>"
-        txt += f"<p><b>data</b>: contains {len(self)} cells.</p>"
-        return txt
-
-    @staticmethod
-    def _get_cell_spec_from_page(indx: int, row: pd.Series) -> dict:
-        # Edit this if we decide to make "argument families", e.g. loader_split or merger_recalc.
-
-        PRM_SPLITTER = ";"
-        EQUAL_SIGN = "="
-
-        def _arg_parser(text: str) -> None:
-            individual_specs = text.split(PRM_SPLITTER)
-            for p in individual_specs:
-                p, a = p.split(EQUAL_SIGN)
-
-        logging.debug(f"getting cell_spec from journal pages ({indx})")
-        try:
-            cell_spec = row[hdr_journal.argument]
-            logging.debug(cell_spec)
-            if not isinstance(cell_spec, dict):
-                raise TypeError("the cell spec argument is not a dictionary")
-        except Exception as e:
-            logging.warning(f"could not get cell spec for {indx}")
-            logging.warning(f"error message: {e}")
-            return {}
-
-        # converting from str if needed
-        for spec in cell_spec:
-            if isinstance(cell_spec[spec], str):
-                if cell_spec[spec].lower() == "true":
-                    cell_spec[spec] = True
-                elif cell_spec[spec].lower() == "false":
-                    cell_spec[spec] = False
-                elif cell_spec[spec].lower() == "none":
-                    cell_spec[spec] = None
-                else:
-                    try:
-                        logging.debug(
-                            f"Using ast.literal_eval to convert cell-spec value from str '{cell_spec[spec]}'"
-                        )
-                        cell_spec[spec] = ast.literal_eval(cell_spec[spec])
-                    except ValueError as e:
-                        logging.warning(
-                            f"ERROR! Could not convert from str to python object!"
-                        )
-                        logging.debug(e)
-        return cell_spec
-
-    def update(self, all_in_memory=None, cell_specs=None, logging_mode=None, accept_errors=None, **kwargs):
-        """Updates the selected datasets.
-
-        Args:
-            all_in_memory (bool): store the `cellpydata` in memory (default
-                False)
-            cell_specs (dict of dicts): individual arguments pr. cell. The `cellspecs` key-word argument
-                dictionary will override the **kwargs and the parameters from the journal pages
-                for the indicated cell.
-            logging_mode (str): sets the logging mode for the loader(s).
-            accept_errors (bool): if True, the loader will continue even if it encounters errors.
-
-            kwargs:
-                transferred all the way to the instrument loader, if not
-                picked up earlier. Remark that you can obtain the same pr. cell by
-                providing a `cellspecs` dictionary. The kwargs have precedence over the
-                parameters given in the journal pages, but will be overridden by parameters
-                given by `cellspecs`.
-
-                Merging:
-                    recalc (Bool): set to False if you don't want automatic "recalc" of
-                        cycle numbers etc. when merging several data-sets.
-                Loading:
-                    selector (dict): selector-based parameters sent to the cellpy-file loader (hdf5) if
-                    loading from raw is not necessary (or turned off).
-
-                Debugging:
-                    debug (Bool): set to True if you want to run in debug mode (should never be used by non-developers).
-
-        Debug-mode:
-                 - runs only for the first item in your journal
-
-        Examples:
-            >>> # Don't perform recalculation of cycle numbers etc. when merging
-            >>> # All cells:
-            >>> b.update(recalc=False)
-            >>> # For specific cell(s):
-            >>> cell_specs_cell_01 = {"name_of_cell_01": {"recalc": False}}
-            >>> b.update(cell_specs=cell_specs_cell_01)
-
-        """
-
-        # TODO: implement experiment.last_cycle
-        accept_errors = accept_errors or self.accept_errors
-
-        debugging = kwargs.pop("debug", False)
-        testing = kwargs.pop("testing", False)
-
-        # --- cleaning up attributes / arguments etc ---
-        force_cellpy = kwargs.pop("force_cellpy", self.force_cellpy)
-        force_raw = kwargs.pop("force_raw", self.force_raw)
-
-        logging.info("[update experiment]")
-        if all_in_memory is not None:
-            self.all_in_memory = all_in_memory
-
-        logging.info(f"Additional keyword arguments: {kwargs}")
-        selector = kwargs.get("selector", None)
-
-        pages = self.journal.pages
-        if self.nom_cap:
-            warnings.warn(
-                "Setting nominal capacity through attributes will be deprecated soon since it modifies "
-                "the journal pages."
-            )
-            pages[hdr_journal.nom_cap] = self.nom_cap
-
-        if self.instrument:
-            warnings.warn(
-                "Setting instrument through attributes will be deprecated soon since it modifies the journal pages."
-            )
-            pages[hdr_journal.instrument] = self.instrument
-
-        if x := kwargs.pop("instrument", None):
-            warnings.warn(
-                "Setting instrument through params will be deprecated soon since it modifies the journal pages."
-                "Future version will require instrument in the journal pages."
-            )
-            pages[hdr_journal.instrument] = x
-
-        if pages.empty:
-            raise Exception("your journal is empty")
-
-        # --- init ---
-        summary_frames = dict()
-        cell_data_frames = dict()
-        number_of_runs = len(pages)
-        logging.debug(f"You have {number_of_runs} cells in your journal")
-        counter = 0
-        errors = []
-
-        pbar = tqdm(list(pages.iterrows()), file=sys.stdout, leave=False)
-
-        if debugging:
-            pbar = tqdm(list(pages.iterrows())[0:1], file=sys.stdout, leave=False)
-
-        # --- iterating ---
-        # TODO: create a multiprocessing pool and get one statusbar pr cell
-        for index, row in pbar:
-            counter += 1
-            h_txt = f"{index}"
-            n_txt = f"loading {counter}"
-            l_txt = f"starting to process file # {counter} ({index})"
-            pbar.set_description(n_txt, refresh=True)
-            cell_spec_page = self._get_cell_spec_from_page(index, row)
-
-            if cell_specs is not None:
-                cell_spec = cell_specs.get(index, dict())
-            else:
-                cell_spec = dict()
-
-            cell_spec = {**cell_spec_page, **kwargs, **cell_spec}
-            l_txt += f" cell_spec: {cell_spec}"
-            logging.debug(l_txt)
-
-            # --- UPDATING ARGUMENTS ---
-            filename = None
-            instrument = None
-            cellpy_file = OtherPath(row[hdr_journal.cellpy_file_name])
-            _cellpy_file = None
-            if not force_raw and cellpy_file.is_file():
-                _cellpy_file = cellpy_file
-                logging.debug(f"Got cellpy file: {_cellpy_file}")
-            if not force_cellpy:
-                filename = row[hdr_journal.raw_file_names]
-                instrument = row[hdr_journal.instrument]
-
-            cycle_mode = row[hdr_journal.cell_type]
-            mass = row[hdr_journal.mass]
-            nom_cap = row[hdr_journal.nom_cap]
-
-            loading = None
-            area = None
-            if hdr_journal.loading in row:
-                loading = row[hdr_journal.loading]
-            if hdr_journal.area in row:
-                area = row[hdr_journal.area]
-
-            summary_kwargs = {
-                "use_cellpy_stat_file": prms.Reader.use_cellpy_stat_file,
-            }
-
-            step_kwargs = {}
-            if not filename and not force_cellpy:
-                logging.info(
-                    f"Raw file(s) not given in the journal.pages for index={index}"
-                )
-                errors.append(index)
-                continue
-
-            elif not cellpy_file and force_cellpy:
-                logging.info(
-                    f"Cellpy file not given in the journal.pages for index={index}"
-                )
-                errors.append(index)
-                continue
-
-            else:
-                logging.info(f"Processing {index}")
-
-            logging.info("loading cell")
-            try:
-                logging.debug("inside try: running cellpy.get")
-                cell_data = cellpy.get(
-                    filename=filename,
-                    instrument=instrument,
-                    cellpy_file=_cellpy_file,
-                    cycle_mode=cycle_mode,
-                    mass=mass,
-                    nom_cap=nom_cap,
-                    loading=loading,
-                    area=area,
-                    step_kwargs=step_kwargs,
-                    summary_kwargs=summary_kwargs,
-                    selector=selector,
-                    logging_mode=logging_mode,
-                    testing=testing,
-                    **cell_spec,
-                )
-                logging.info("loaded cell")
-
-            except Exception as e:
-                logging.info("Failed to load: " + str(e))
-                errors.append("update:" + str(index))
-                h_txt += " [-]"
-                pbar.set_postfix_str(s=h_txt, refresh=True)
-                if not accept_errors:
-                    raise e
-                continue
-
-            if cell_data.empty:
-                logging.info("...not loaded...")
-                logging.debug("Data is empty. Could not load cell!")
-                errors.append("check:" + str(index))
-                h_txt += " [-]"
-                pbar.set_postfix_str(s=h_txt, refresh=True)
-                continue
-
-            logging.info("...loaded successfully...")
-            h_txt += " [OK]"
-            pbar.set_postfix_str(s=h_txt, refresh=True)
-            summary_tmp = cell_data.data.summary
-            logging.info("Trying to get summary_data")
-
-            if cell_data.data.steps is None or self.force_recalc:
-                logging.info("Running make_step_table")
-                n_txt = f"steps {counter}"
-                pbar.set_description(n_txt, refresh=True)
-                cell_data.make_step_table()
-
-            if summary_tmp is None or self.force_recalc:
-                logging.info("Running make_summary")
-                n_txt = f"summary {counter}"
-                pbar.set_description(n_txt, refresh=True)
-                cell_data.make_summary(find_end_voltage=True, find_ir=True)
-
-            # some clean-ups (might not be needed anymore):
-            if not summary_tmp.index.name == hdr_summary.cycle_index:
-                logging.debug("Setting index to Cycle_Index")
-                # check if it is a byte-string
-                if b"Cycle_Index" in summary_tmp.columns:
-                    logging.debug("Seems to be a byte-string in the column-headers")
-                    summary_tmp.rename(
-                        columns={b"Cycle_Index": "Cycle_Index"}, inplace=True
-                    )
-                try:
-                    summary_tmp.set_index("cycle_index", inplace=True)
-                except KeyError:
-                    logging.debug("cycle_index already an index")
-
-            summary_frames[index] = summary_tmp
-
-            if self.all_in_memory:
-                cell_data_frames[index] = cell_data
-            else:
-                cell_data_frames[index] = cellreader.CellpyCell(initialize=True)
-                cell_data_frames[index].data.steps = cell_data.data.steps
-
-            if self.save_cellpy:
-                logging.info("saving to cellpy-format")
-                n_txt = f"saving {counter}"
-                pbar.set_description(n_txt, refresh=True)
-                if self.custom_data_folder is not None:
-                    print("Save to custom data-folder not implemented yet")
-                    print(f"Saving to {row.cellpy_file_name} instead")
-                if not row.fixed:
-                    logging.info("saving cell to %s" % row.cellpy_file_name)
-                    cell_data.ensure_step_table = True
-                    try:
-                        cell_data.save(row.cellpy_file_name)
-                    except Exception as e:
-                        logging.error("saving file failed")
-                        logging.error(e)
-
-                else:
-                    logging.debug("saving cell skipped (set to 'fixed' in info_df)")
-            else:
-                logging.info("You opted to not save to cellpy-format")
-                logging.info("It is usually recommended to save to cellpy-format:")
-                logging.info(" >>> b.experiment.save_cellpy = True")
-                logging.info(
-                    "Without the cellpy-files, you cannot select specific cells"
-                )
-                logging.info("if you did not opt to store all in memory")
-
-            if self.export_raw or self.export_cycles:
-                export_text = "exporting"
-                if self.export_raw:
-                    export_text += " [raw]"
-                if self.export_cycles:
-                    export_text += " [cycles]"
-                logging.info(export_text)
-                n_txt = f"{export_text} {counter}"
-                pbar.set_description(n_txt, refresh=True)
-                cell_data.to_csv(
-                    self.journal.raw_dir,
-                    sep=prms.Reader.sep,
-                    cycles=self.export_cycles,
-                    shifted=self.shifted_cycles,
-                    raw=self.export_raw,
-                    last_cycle=self.last_cycle,
-                )
-
-            if self.export_ica:
-                logging.info("exporting [ica]")
-                try:
-                    helper.export_dqdv(
-                        cell_data,
-                        savedir=self.journal.raw_dir,
-                        sep=prms.Reader.sep,
-                        last_cycle=self.last_cycle,
-                    )
-                except Exception as e:
-                    logging.error("Could not make/export dq/dv data")
-                    logging.debug(
-                        "Failed to make/export " "dq/dv data (%s): %s" % (index, str(e))
-                    )
-                    errors.append("ica:" + str(index))
-
-        self.errors["update"] = errors
-        self.summary_frames = summary_frames
-        self.cell_data_frames = cell_data_frames
-
-    def parallel_update(
-        self, all_in_memory=None, cell_specs=None, logging_mode=None, **kwargs
-    ):
-        """Updates the selected datasets in parallel.
-
-        Args:
-            all_in_memory (bool): store the `cellpydata` in memory (default
-                False)
-            cell_specs (dict of dicts): individual arguments pr. cell. The `cellspecs` key-word argument
-                dictionary will override the **kwargs and the parameters from the journal pages
-                for the indicated cell.
-            logging_mode (str): sets the logging mode for the loader(s).
-
-            kwargs:
-                transferred all the way to the instrument loader, if not
-                picked up earlier. Remark that you can obtain the same pr. cell by
-                providing a `cellspecs` dictionary. The kwargs have precedence over the
-                parameters given in the journal pages, but will be overridden by parameters
-                given by `cellspecs`.
-
-                Merging:
-                    recalc (Bool): set to False if you don't want automatic "recalc" of
-                        cycle numbers etc. when merging several data-sets.
-                Loading:
-                    selector (dict): selector-based parameters sent to the cellpy-file loader (hdf5) if
-                    loading from raw is not necessary (or turned off).
-
-                Debugging:
-                    debug (Bool): set to True if you want to run in debug mode (should never be used by non-developers).
-
-        Debug-mode:
-                 - runs only for the first item in your journal
-
-        Examples:
-            >>> # Don't perform recalculation of cycle numbers etc. when merging
-            >>> # All cells:
-            >>> b.update(recalc=False)
-            >>> # For specific cell(s):
-            >>> cell_specs_cell_01 = {"name_of_cell_01": {"recalc": False}}
-            >>> b.update(cell_specs=cell_specs_cell_01)
-
-        """
-        status = "PROD"  # set this to DEV when developing this
-        async_mode = "threading"
-        logging.debug("PARALLEL UPDATE")
-        # TODO: implement experiment.last_cycle
-        if status != "DEV":
-            print("SORRY - MULTIPROCESSING IS NOT IMPLEMENTED PROPERLY YET")
-            return self.update(
-                all_in_memory=all_in_memory,
-                cell_specs=cell_specs,
-                logging_mode=logging_mode,
-                **kwargs,
-            )
-
-        import concurrent.futures
-        import multiprocessing
-
-        max_number_processes = multiprocessing.cpu_count()
-
-        if async_mode == "threading":
-            pool_executor = concurrent.futures.ThreadPoolExecutor
-        else:
-            pool_executor = concurrent.futures.ProcessPoolExecutor
-
-        debugging = kwargs.pop("debug", False)
-
-        # --- cleaning up attributes / arguments etc ---
-        force_cellpy = kwargs.pop("force_cellpy", self.force_cellpy)
-        force_raw = kwargs.pop("force_raw", self.force_raw)
-
-        logging.info("[update experiment]")
-        if all_in_memory is not None:
-            self.all_in_memory = all_in_memory
-
-        logging.info(f"Additional keyword arguments: {kwargs}")
-        selector = kwargs.get("selector", None)
-
-        pages = self.journal.pages
-        if self.nom_cap:
-            warnings.warn(
-                "Setting nominal capacity through attributes will be deprecated soon since it modifies "
-                "the journal pages."
-            )
-            pages[hdr_journal.nom_cap] = self.nom_cap
-
-        if self.instrument:
-            warnings.warn(
-                "Setting instrument through attributes will be deprecated soon since it modifies the journal pages."
-            )
-            pages[hdr_journal.instrument] = self.instrument
-
-        if x := kwargs.pop("instrument", None):
-            warnings.warn(
-                "Setting instrument through params will be deprecated soon since it modifies the journal pages."
-                "Future version will require instrument in the journal pages."
-            )
-            pages[hdr_journal.instrument] = x
-
-        if pages.empty:
-            raise Exception("your journal is empty")
-
-        # --- init ---
-        summary_frames = dict()
-        cell_data_frames = dict()
-        number_of_runs = len(pages)
-        logging.debug(f"You have {number_of_runs} cells in your journal")
-        counter = 0
-        errors = []
-
-        pbar = tqdm(list(pages.iterrows()), file=sys.stdout, leave=False)
-
-        if debugging:
-            pbar = tqdm(list(pages.iterrows())[0:1], file=sys.stdout, leave=False)
-
-        # --- iterating ---
-        # TODO: create a multiprocessing pool and get one statusbar pr cell
-        params = []
-        with pool_executor(max_number_processes) as executor:
-            for index, row in pages.iterrows():
-                counter += 1
-                cell_spec_page = self._get_cell_spec_from_page(index, row)
-
-                if cell_specs is not None:
-                    cell_spec = cell_specs.get(index, dict())
-                else:
-                    cell_spec = dict()
-
-                cell_spec = {**cell_spec_page, **kwargs, **cell_spec}
-
-                # --- UPDATING ARGUMENTS ---
-                filename = None
-                instrument = None
-                cellpy_file = OtherPath(row[hdr_journal.cellpy_file_name])
-                _cellpy_file = None
-                if not force_raw and cellpy_file.is_file():
-                    _cellpy_file = cellpy_file
-                    logging.debug(f"Got cellpy file: {_cellpy_file}")
-                if not force_cellpy:
-                    filename = row[hdr_journal.raw_file_names]
-                    instrument = row[hdr_journal.instrument]
-
-                cycle_mode = row[hdr_journal.cell_type]
-                mass = row[hdr_journal.mass]
-                nom_cap = row[hdr_journal.nom_cap]
-
-                loading = None
-                area = None
-                if hdr_journal.loading in row:
-                    loading = row[hdr_journal.loading]
-                if hdr_journal.area in row:
-                    area = row[hdr_journal.area]
-
-                summary_kwargs = {
-                    "use_cellpy_stat_file": prms.Reader.use_cellpy_stat_file,
-                }
-
-                step_kwargs = {}
-                if not filename and not force_cellpy:
-                    logging.info(
-                        f"Raw file(s) not given in the journal.pages for index={index}"
-                    )
-                    errors.append(index)
-                    continue
-
-                elif not cellpy_file and force_cellpy:
-                    logging.info(
-                        f"Cellpy file not given in the journal.pages for index={index}"
-                    )
-                    errors.append(index)
-                    continue
-
-                else:
-                    logging.info(f"Processing {index}")
-
-                logging.info("loading cell")
-                params.append(
-                    dict(
-                        filename=filename,
-                        instrument=instrument,
-                        cellpy_file=_cellpy_file,
-                        cycle_mode=cycle_mode,
-                        mass=mass,
-                        nom_cap=nom_cap,
-                        loading=loading,
-                        area=area,
-                        step_kwargs=step_kwargs,
-                        summary_kwargs=summary_kwargs,
-                        selector=selector,
-                        logging_mode=logging_mode,
-                        testing=False,
-                        **cell_spec,
-                    )
-                )
-
-            pool = [executor.submit(cellpy.get, **param) for param in params]
-            for i in concurrent.futures.as_completed(pool):
-                cell_data = i.result()
-                if cell_data.empty:
-                    logging.info("...not loaded...")
-                    logging.debug("Data is empty. Could not load cell!")
-                    errors.append("check:" + str(index))
-
-                logging.info("...loaded successfully...")
-                summary_tmp = cell_data.data.summary
-                logging.info("Trying to get summary_data")
-
-                if cell_data.data.steps is None or self.force_recalc:
-                    logging.info("Running make_step_table")
-                    cell_data.make_step_table()
-
-                if summary_tmp is None or self.force_recalc:
-                    logging.info("Running make_summary")
-                    cell_data.make_summary(find_end_voltage=True, find_ir=True)
-
-                # some clean-ups (might not be needed anymore):
-                if not summary_tmp.index.name == hdr_summary.cycle_index:
-                    logging.debug("Setting index to Cycle_Index")
-                    # check if it is a byte-string
-                    if b"Cycle_Index" in summary_tmp.columns:
-                        logging.debug("Seems to be a byte-string in the column-headers")
-                        summary_tmp.rename(
-                            columns={b"Cycle_Index": "Cycle_Index"}, inplace=True
-                        )
-                    try:
-                        summary_tmp.set_index("cycle_index", inplace=True)
-                    except KeyError:
-                        logging.debug("cycle_index already an index")
-
-                summary_frames[index] = summary_tmp
-
-                if self.all_in_memory:
-                    cell_data_frames[index] = cell_data
-                else:
-                    cell_data_frames[index] = cellreader.CellpyCell(initialize=True)
-                    cell_data_frames[index].data.steps = cell_data.data.steps
-
-                if self.save_cellpy:
-                    logging.info("saving to cellpy-format")
-                    n_txt = f"saving {counter}"
-                    pbar.set_description(n_txt, refresh=True)
-                    if self.custom_data_folder is not None:
-                        print("Save to custom data-folder not implemented yet")
-                        print(f"Saving to {row.cellpy_file_name} instead")
-                    if not row.fixed:
-                        logging.info("saving cell to %s" % row.cellpy_file_name)
-                        cell_data.ensure_step_table = True
-                        try:
-                            cell_data.save(row.cellpy_file_name)
-                        except Exception as e:
-                            logging.error("saving file failed")
-                            logging.error(e)
-
-                    else:
-                        logging.debug("saving cell skipped (set to 'fixed' in info_df)")
-                else:
-                    logging.info("You opted to not save to cellpy-format")
-                    logging.info("It is usually recommended to save to cellpy-format:")
-                    logging.info(" >>> b.experiment.save_cellpy = True")
-                    logging.info(
-                        "Without the cellpy-files, you cannot select specific cells"
-                    )
-                    logging.info("if you did not opt to store all in memory")
-
-                if self.export_raw or self.export_cycles:
-                    export_text = "exporting"
-                    if self.export_raw:
-                        export_text += " [raw]"
-                    if self.export_cycles:
-                        export_text += " [cycles]"
-                    logging.info(export_text)
-                    n_txt = f"{export_text} {counter}"
-                    pbar.set_description(n_txt, refresh=True)
-                    cell_data.to_csv(
-                        self.journal.raw_dir,
-                        sep=prms.Reader.sep,
-                        cycles=self.export_cycles,
-                        shifted=self.shifted_cycles,
-                        raw=self.export_raw,
-                        last_cycle=self.last_cycle,
-                    )
-
-                if self.export_ica:
-                    logging.info("exporting [ica]")
-                    try:
-                        helper.export_dqdv(
-                            cell_data,
-                            savedir=self.journal.raw_dir,
-                            sep=prms.Reader.sep,
-                            last_cycle=self.last_cycle,
-                        )
-                    except Exception as e:
-                        logging.error("Could not make/export dq/dv data")
-                        logging.debug(
-                            "Failed to make/export "
-                            "dq/dv data (%s): %s" % (index, str(e))
-                        )
-                        errors.append("ica:" + str(index))
-
-        self.errors["update"] = errors
-        self.summary_frames = summary_frames
-        self.cell_data_frames = cell_data_frames
-
-    def export_cellpy_files(self, path=None, **kwargs):
-        """Export all cellpy-files to a given path.
-
-        Remarks:
-            This method can only export to local folders
-            (OtherPath objects are not formally supported, but
-            might still work if the path is local).
-
-        Args:
-            path (str, pathlib.Path): path to export to (default: current working directory)
-        """
-        if path is None:
-            path = "."
-        errors = []
-        path = pathlib.Path(path)
-        cell_names = self.cell_names
-        for cell_name in cell_names:
-            cellpy_file_name = self.journal.pages.loc[
-                cell_name, hdr_journal.cellpy_file_name
-            ]
-            cellpy_file_name = path / pathlib.Path(cellpy_file_name).name
-            print(f"Exporting {cell_name} to {cellpy_file_name}")
-            try:
-                c = self.data[cell_name]
-            except TypeError as e:
-                errors.append(f"could not extract data for {cell_name} - linking")
-                self._link_cellpy_file(cell_name)
-
-            c.save(cellpy_file_name, **kwargs)
-        self.errors["export_cellpy_files"] = errors
-
-    @property
-    def cell_names(self):
-        """Returns a list of cell-names (strings)"""
-        try:
-            return [key for key in self.cell_data_frames]
-        except TypeError:
-            return None
-
-    def status(self):
-        print("\n")
-        print(" STATUS ".center(80, "="))
-        print(self)
-        print(" summary frames ".center(80, "-"))
-        if self.summary_frames is not None:
-            for key in self.summary_frames:
-                print(f" {{{key}}}")
-        print(" memory dumped ".center(80, "-"))
-        if self.memory_dumped is not None:
-            for key in self.memory_dumped:
-                print(f"{key}: {type(self.memory_dumped[key])}")
-        print(80 * "=")
-
-    def link(self, **kwargs):
-        """Ensure that an appropriate link to the cellpy-files exists for
-        each cell.
-
-        The experiment will then contain a CellpyCell object for each cell
-        (in the cell_data_frames attribute) with only the step-table stored.
-
-        Remark that running update persists the summary frames instead (or
-        everything in case you specify all_in_memory=True).
-        This might be considered "a strange and unexpected behaviour". Sorry
-        for that (but the authors of this package is also a bit strange...).
-
-        (OK, I will change it. Soon.)
-
-        **kwargs: passed to _link_cellpy_file
-            max_cycle (int): maximum cycle number to link/load (remark that the
-                cellpy objects will get the property overwrite_able set to False
-                if you give a max_cycle to prevent accidentally saving a "truncated"
-                file (use c.save(filename, overwrite=True) to force overwrite))
-
-
-        """
-        logging.info("[establishing links]")
-        logging.debug("checking and establishing link to data")
-
-        errors = []
-
-        for cell_label in self.journal.pages.index:
-            logging.debug(f"trying to link {cell_label}")
-            try:
-                self._link_cellpy_file(cell_label, **kwargs)
-            except IOError as e:
-                logging.warning(e)
-                e_txt = f"{cell_label}: links not established - try update instead"
-                logging.warning(e_txt)
-                errors.append(e_txt)
-
-        self.errors["link"] = errors
-
-    def recalc(
-        self,
-        save=True,
-        step_opts=None,
-        summary_opts=None,
-        indexes=None,
-        calc_steps=True,
-        testing=False,
-    ):
-        """Run make_step_table and make_summary on all cells.
-
-        Args:
-            save (bool): Save updated cellpy-files if True.
-            step_opts (dict): parameters to inject to make_steps.
-            summary_opts (dict): parameters to inject to make_summary.
-            indexes (list): Only recalculate for given indexes (i.e. list of cell-names).
-            calc_steps (bool): Run make_steps before making the summary.
-            testing (bool): Only for testing purposes.
-
-        Returns:
-            None
-        """
-
-        # TODO: option (default) to only recalc if the values (mass, nom_cap,...) have changed
-        errors = []
-        log = []
-        if testing:
-            pbar = tqdm(
-                list(self.journal.pages.iloc[0:2, :].iterrows()),
-                file=sys.stdout,
-                leave=False,
-            )
-        elif indexes is not None:
-            pbar = tqdm(
-                list(self.journal.pages.loc[indexes, :].iterrows()),
-                file=sys.stdout,
-                leave=False,
-            )
-        else:
-            pbar = tqdm(
-                list(self.journal.pages.iterrows()), file=sys.stdout, leave=False
-            )
-        for indx, row in pbar:
-            nom_cap = row[hdr_journal.nom_cap]
-            mass = row[hdr_journal.mass]
-            pbar.set_description(indx)
-            try:
-                c = self.data[indx]
-            except TypeError as e:
-                e_txt = (
-                    f"could not extract data for {indx} - have you forgotten to link?"
-                )
-                errors.append(e_txt)
-                warnings.warn(e_txt)
-
-            else:
-                if nom_cap:
-                    c.set_nom_cap(nom_cap)
-                if mass:
-                    c.set_mass(mass)
-                try:
-                    if calc_steps:
-                        pbar.set_postfix_str(s="steps", refresh=True)
-                        if step_opts is not None:
-                            c.make_step_table(**step_opts)
-                        else:
-                            c.make_step_table()
-
-                    pbar.set_postfix_str(s="summary", refresh=True)
-                    if summary_opts is not None:
-                        c.make_summary(**summary_opts)
-                    else:
-                        c.make_summary(find_end_voltage=True, find_ir=True)
-
-                except Exception as e:
-                    e_txt = f"recalculating for {indx} failed!"
-                    errors.append(e_txt)
-                    warnings.warn(e_txt)
-                else:
-                    if save:
-                        # remark! got a win error when trying to save (hdf5-file in use) (must fix this)
-                        pbar.set_postfix_str(s="save", refresh=True)
-                        try:
-                            c.save(row.cellpy_file_name)
-                            log.append(f"saved {indx} to {row.cellpy_file_name}")
-                        except Exception as e:
-                            e_txt = f"saving {indx} to {row.cellpy_file_name} failed!"
-                            errors.append(e_txt)
-                            warnings.warn(e_txt)
-        self.errors["recalc"] = errors
-        self.log["recalc"] = log
-
-
-class ImpedanceExperiment(BaseExperiment):
-    def __init__(self):
-        super().__init__()
-
-
-class LifeTimeExperiment(BaseExperiment):
-    def __init__(self):
-        super().__init__()
-
-
-if __name__ == "__main__":
-    from pathlib import Path
-    import os
-    import pandas as pd
-    import numpy as np
-    import seaborn as sns
-    import plotly.express as px
-
-    import cellpy
-    from cellpy.utils import batch, helpers, plotutils
-
-    project_dir = Path("../../../testdata/batch_project")
-    print(f"{project_dir.resolve()=}")
-    journal = project_dir / "test_project.json"
-    journal = journal.resolve()
-    print(f"{journal=}")
-    assert project_dir.is_dir()
-    assert journal.is_file()
-    os.chdir(project_dir)
-
-    print(f"cellpy version: {cellpy.__version__}")
-    cellpy.log.setup_logging("INFO")
-
-    b = batch.from_journal(journal)
-    b.update()
-
-    print("Ended OK")
+import ast
+import logging
+import os
+import pathlib
+import sys
+import warnings
+
+import pandas as pd
+from tqdm.auto import tqdm
+
+import cellpy
+from cellpy import prms
+from cellpy.parameters.internal_settings import get_headers_journal, get_headers_summary
+from cellpy.readers import cellreader
+from cellpy.internals.core import OtherPath
+from cellpy.utils.batch_tools import batch_helpers as helper
+from cellpy.utils.batch_tools.batch_core import BaseExperiment
+from cellpy.utils.batch_tools.batch_journals import LabJournal
+
+hdr_journal = get_headers_journal()
+hdr_summary = get_headers_summary()
+
+
+class CyclingExperiment(BaseExperiment):
+    """Load experimental data into memory.
+
+    This is a re-implementation of the old batch behaviour where
+    all the data-files are processed sequentially (and optionally exported)
+    while the summary tables are kept and processed. This implementation
+    also saves the step tables (for later use when using look-up
+    functionality).
+
+
+    Attributes:
+        journal (:obj: LabJournal): information about the experiment.
+        force_cellpy (bool): tries only to load the cellpy-file if True.
+        force_raw (bool): loads raw-file(s) even though appropriate cellpy-file
+           exists if True.
+        save_cellpy (bool): saves a cellpy-file for each cell if True.
+        accept_errors (bool): in case of error, dont raise an exception, but
+           continue to the next file if True.
+        all_in_memory (bool): store the cellpydata-objects in memory if True.
+        export_cycles (bool): export voltage-capacity curves if True.
+        shifted_cycles (bool): set this to True if you want to export the
+           voltage-capacity curves using the shifted-cycles option (only valid
+           if you set export_cycles to True).
+        export_raw (bool): export the raw-data if True.
+        export_ica (bool): export dq-dv curves if True.
+        last_cycle (int): sets the last cycle (i.e. the highest cycle number)
+           that you would like to process dq-dv on). Use all if None (the
+           default value).
+        selected_summaries (list): a list of summary labels defining what
+           summary columns to make joint summaries from (optional).
+        errors (dict): contains a dictionary listing all the errors encountered.
+
+    Args:
+        db_reader (str or object): custom db_reader (see doc on db_reader).
+
+    Example:
+
+
+    """
+
+    def __init__(self, *args, **kwargs):
+        db_reader = kwargs.pop("db_reader", "default")
+        super().__init__(*args)
+        self.journal = LabJournal(db_reader=db_reader)
+        self.errors = dict()
+        self.log = dict()
+
+        self.force_cellpy = False
+        self.force_raw = False
+        self.force_recalc = False
+        self.save_cellpy = True
+        self.accept_errors = False
+        self.all_in_memory = False
+
+        self.export_cycles = False
+        self.shifted_cycles = False
+        self.export_raw = True
+        self.export_ica = False
+        self.last_cycle = None
+        self.nom_cap = None
+        self.instrument = None
+        self.custom_data_folder = None
+
+        self.selected_summaries = None
+
+    def _repr_html_(self):
+        txt = f"<h2>CyclingExperiment-object</h2> id={hex(id(self))}"
+        txt += "<h3>Main attributes</h3>"
+        txt += f"""
+        <table>
+            <thead>
+                <tr>
+                    <th>Attribute</th>
+                    <th>Value</th>
+                </tr>
+            </thead>
+            <tbody>
+                <tr><td><b>force_cellpy</b></td><td>{self.force_cellpy}</td></tr>
+                <tr><td><b>force_raw</b></td><td>{self.force_raw}</td></tr>
+                <tr><td><b>force_recalc</b></td><td>{self.force_recalc}</td></tr>
+                <tr><td><b>save_cellpy</b></td><td>{self.save_cellpy}</td></tr>
+                <tr><td><b>accept_errors</b></td><td>{self.accept_errors}</td></tr>
+                <tr><td><b>all_in_memory</b></td><td>{self.all_in_memory}</td></tr>
+                <tr><td><b>export_cycles</b></td><td>{self.export_cycles}</td></tr>
+                <tr><td><b>shifted_cycles</b></td><td>{self.shifted_cycles}</td></tr>
+                <tr><td><b>export_raw</b></td><td>{self.export_raw}</td></tr>
+                <tr><td><b>export_ica</b></td><td>{self.export_ica}</td></tr>
+                <tr><td><b>last_cycle</b></td><td>{self.last_cycle}</td></tr>
+                <tr><td><b>nom_cap</b></td><td>{self.nom_cap}</td></tr>
+                <tr><td><b>instrument</b></td><td>{self.instrument}</td></tr>
+                <tr><td><b>custom_data_folder</b></td><td>{self.custom_data_folder}</td></tr>
+                <tr><td><b>selected_summaries</b></td><td>{self.selected_summaries}</td></tr>
+            </tbody>
+        </table>
+        """
+        txt += "<h3>Cells</h3>"
+        txt += f"<p><b>data</b>: contains {len(self)} cells.</p>"
+        return txt
+
+    @staticmethod
+    def _get_cell_spec_from_page(indx: int, row: pd.Series) -> dict:
+        # Edit this if we decide to make "argument families", e.g. loader_split or merger_recalc.
+
+        PRM_SPLITTER = ";"
+        EQUAL_SIGN = "="
+
+        def _arg_parser(text: str) -> None:
+            individual_specs = text.split(PRM_SPLITTER)
+            for p in individual_specs:
+                p, a = p.split(EQUAL_SIGN)
+
+        logging.debug(f"getting cell_spec from journal pages ({indx})")
+        try:
+            cell_spec = row[hdr_journal.argument]
+            logging.debug(cell_spec)
+            if not isinstance(cell_spec, dict):
+                raise TypeError("the cell spec argument is not a dictionary")
+        except Exception as e:
+            logging.warning(f"could not get cell spec for {indx}")
+            logging.warning(f"error message: {e}")
+            return {}
+
+        # converting from str if needed
+        for spec in cell_spec:
+            if isinstance(cell_spec[spec], str):
+                if cell_spec[spec].lower() == "true":
+                    cell_spec[spec] = True
+                elif cell_spec[spec].lower() == "false":
+                    cell_spec[spec] = False
+                elif cell_spec[spec].lower() == "none":
+                    cell_spec[spec] = None
+                else:
+                    try:
+                        logging.debug(
+                            f"Using ast.literal_eval to convert cell-spec value from str '{cell_spec[spec]}'"
+                        )
+                        cell_spec[spec] = ast.literal_eval(cell_spec[spec])
+                    except ValueError as e:
+                        logging.warning(
+                            f"ERROR! Could not convert from str to python object!"
+                        )
+                        logging.debug(e)
+        return cell_spec
+
+    def update(
+        self,
+        all_in_memory=None,
+        cell_specs=None,
+        logging_mode=None,
+        accept_errors=None,
+        **kwargs,
+    ):
+        """Updates the selected datasets.
+
+        Args:
+            all_in_memory (bool): store the `cellpydata` in memory (default
+                False)
+            cell_specs (dict of dicts): individual arguments pr. cell. The `cellspecs` key-word argument
+                dictionary will override the **kwargs and the parameters from the journal pages
+                for the indicated cell.
+            logging_mode (str): sets the logging mode for the loader(s).
+            accept_errors (bool): if True, the loader will continue even if it encounters errors.
+
+            kwargs:
+                transferred all the way to the instrument loader, if not
+                picked up earlier. Remark that you can obtain the same pr. cell by
+                providing a `cellspecs` dictionary. The kwargs have precedence over the
+                parameters given in the journal pages, but will be overridden by parameters
+                given by `cellspecs`.
+
+                Merging:
+                    recalc (Bool): set to False if you don't want automatic "recalc" of
+                        cycle numbers etc. when merging several data-sets.
+                Loading:
+                    selector (dict): selector-based parameters sent to the cellpy-file loader (hdf5) if
+                    loading from raw is not necessary (or turned off).
+
+                Debugging:
+                    debug (Bool): set to True if you want to run in debug mode (should never be used by non-developers).
+
+        Debug-mode:
+                 - runs only for the first item in your journal
+
+        Examples:
+            >>> # Don't perform recalculation of cycle numbers etc. when merging
+            >>> # All cells:
+            >>> b.update(recalc=False)
+            >>> # For specific cell(s):
+            >>> cell_specs_cell_01 = {"name_of_cell_01": {"recalc": False}}
+            >>> b.update(cell_specs=cell_specs_cell_01)
+
+        """
+
+        # TODO: implement experiment.last_cycle
+        accept_errors = accept_errors or self.accept_errors
+
+        debugging = kwargs.pop("debug", False)
+        testing = kwargs.pop("testing", False)
+
+        # --- cleaning up attributes / arguments etc ---
+        force_cellpy = kwargs.pop("force_cellpy", self.force_cellpy)
+        force_raw = kwargs.pop("force_raw", self.force_raw)
+
+        logging.info("[update experiment]")
+        if all_in_memory is not None:
+            self.all_in_memory = all_in_memory
+
+        logging.info(f"Additional keyword arguments: {kwargs}")
+        selector = kwargs.get("selector", None)
+
+        pages = self.journal.pages
+        if self.nom_cap:
+            warnings.warn(
+                "Setting nominal capacity through attributes will be deprecated soon since it modifies "
+                "the journal pages."
+            )
+            pages[hdr_journal.nom_cap] = self.nom_cap
+
+        if self.instrument:
+            warnings.warn(
+                "Setting instrument through attributes will be deprecated soon since it modifies the journal pages."
+            )
+            pages[hdr_journal.instrument] = self.instrument
+
+        if x := kwargs.pop("instrument", None):
+            warnings.warn(
+                "Setting instrument through params will be deprecated soon since it modifies the journal pages."
+                "Future version will require instrument in the journal pages."
+            )
+            pages[hdr_journal.instrument] = x
+
+        if pages.empty:
+            raise Exception("your journal is empty")
+
+        # --- init ---
+        summary_frames = dict()
+        cell_data_frames = dict()
+        number_of_runs = len(pages)
+        logging.debug(f"You have {number_of_runs} cells in your journal")
+        counter = 0
+        errors = []
+
+        pbar = tqdm(list(pages.iterrows()), file=sys.stdout, leave=False)
+
+        if debugging:
+            pbar = tqdm(list(pages.iterrows())[0:1], file=sys.stdout, leave=False)
+
+        # --- iterating ---
+        # TODO: create a multiprocessing pool and get one statusbar pr cell
+        for index, row in pbar:
+            counter += 1
+            h_txt = f"{index}"
+            n_txt = f"loading {counter}"
+            l_txt = f"starting to process file # {counter} ({index})"
+            pbar.set_description(n_txt, refresh=True)
+            cell_spec_page = self._get_cell_spec_from_page(index, row)
+
+            if cell_specs is not None:
+                cell_spec = cell_specs.get(index, dict())
+            else:
+                cell_spec = dict()
+
+            cell_spec = {**cell_spec_page, **kwargs, **cell_spec}
+            l_txt += f" cell_spec: {cell_spec}"
+            logging.debug(l_txt)
+
+            # --- UPDATING ARGUMENTS ---
+            filename = None
+            instrument = None
+            cellpy_file = OtherPath(row[hdr_journal.cellpy_file_name])
+            _cellpy_file = None
+            if not force_raw and cellpy_file.is_file():
+                _cellpy_file = cellpy_file
+                logging.debug(f"Got cellpy file: {_cellpy_file}")
+            if not force_cellpy:
+                filename = row[hdr_journal.raw_file_names]
+                instrument = row[hdr_journal.instrument]
+
+            cycle_mode = row[hdr_journal.cell_type]
+            mass = row[hdr_journal.mass]
+            nom_cap = row[hdr_journal.nom_cap]
+
+            loading = None
+            area = None
+            if hdr_journal.loading in row:
+                loading = row[hdr_journal.loading]
+            if hdr_journal.area in row:
+                area = row[hdr_journal.area]
+
+            summary_kwargs = {
+                "use_cellpy_stat_file": prms.Reader.use_cellpy_stat_file,
+            }
+
+            step_kwargs = {}
+            if not filename and not force_cellpy:
+                logging.info(
+                    f"Raw file(s) not given in the journal.pages for index={index}"
+                )
+                errors.append(index)
+                continue
+
+            elif not cellpy_file and force_cellpy:
+                logging.info(
+                    f"Cellpy file not given in the journal.pages for index={index}"
+                )
+                errors.append(index)
+                continue
+
+            else:
+                logging.info(f"Processing {index}")
+
+            logging.info("loading cell")
+            try:
+                logging.debug("inside try: running cellpy.get")
+                cell_data = cellpy.get(
+                    filename=filename,
+                    instrument=instrument,
+                    cellpy_file=_cellpy_file,
+                    cycle_mode=cycle_mode,
+                    mass=mass,
+                    nom_cap=nom_cap,
+                    loading=loading,
+                    area=area,
+                    step_kwargs=step_kwargs,
+                    summary_kwargs=summary_kwargs,
+                    selector=selector,
+                    logging_mode=logging_mode,
+                    testing=testing,
+                    **cell_spec,
+                )
+                logging.info("loaded cell")
+
+            except Exception as e:
+                logging.info("Failed to load: " + str(e))
+                errors.append("update:" + str(index))
+                h_txt += " [-]"
+                pbar.set_postfix_str(s=h_txt, refresh=True)
+                if not accept_errors:
+                    raise e
+                continue
+
+            if cell_data.empty:
+                logging.info("...not loaded...")
+                logging.debug("Data is empty. Could not load cell!")
+                errors.append("check:" + str(index))
+                h_txt += " [-]"
+                pbar.set_postfix_str(s=h_txt, refresh=True)
+                continue
+
+            logging.info("...loaded successfully...")
+            h_txt += " [OK]"
+            pbar.set_postfix_str(s=h_txt, refresh=True)
+            summary_tmp = cell_data.data.summary
+            logging.info("Trying to get summary_data")
+
+            if cell_data.data.steps is None or self.force_recalc:
+                logging.info("Running make_step_table")
+                n_txt = f"steps {counter}"
+                pbar.set_description(n_txt, refresh=True)
+                cell_data.make_step_table()
+
+            if summary_tmp is None or self.force_recalc:
+                logging.info("Running make_summary")
+                n_txt = f"summary {counter}"
+                pbar.set_description(n_txt, refresh=True)
+                cell_data.make_summary(find_end_voltage=True, find_ir=True)
+
+            # some clean-ups (might not be needed anymore):
+            if not summary_tmp.index.name == hdr_summary.cycle_index:
+                logging.debug("Setting index to Cycle_Index")
+                # check if it is a byte-string
+                if b"Cycle_Index" in summary_tmp.columns:
+                    logging.debug("Seems to be a byte-string in the column-headers")
+                    summary_tmp.rename(
+                        columns={b"Cycle_Index": "Cycle_Index"}, inplace=True
+                    )
+                try:
+                    summary_tmp.set_index("cycle_index", inplace=True)
+                except KeyError:
+                    logging.debug("cycle_index already an index")
+
+            summary_frames[index] = summary_tmp
+
+            if self.all_in_memory:
+                cell_data_frames[index] = cell_data
+            else:
+                cell_data_frames[index] = cellreader.CellpyCell(initialize=True)
+                cell_data_frames[index].data.steps = cell_data.data.steps
+
+            if self.save_cellpy:
+                logging.info("saving to cellpy-format")
+                n_txt = f"saving {counter}"
+                pbar.set_description(n_txt, refresh=True)
+                if self.custom_data_folder is not None:
+                    print("Save to custom data-folder not implemented yet")
+                    print(f"Saving to {row.cellpy_file_name} instead")
+                if not row.fixed:
+                    logging.info("saving cell to %s" % row.cellpy_file_name)
+                    cell_data.ensure_step_table = True
+                    try:
+                        cell_data.save(row.cellpy_file_name)
+                    except Exception as e:
+                        logging.error("saving file failed")
+                        logging.error(e)
+
+                else:
+                    logging.debug("saving cell skipped (set to 'fixed' in info_df)")
+            else:
+                logging.info("You opted to not save to cellpy-format")
+                logging.info("It is usually recommended to save to cellpy-format:")
+                logging.info(" >>> b.experiment.save_cellpy = True")
+                logging.info(
+                    "Without the cellpy-files, you cannot select specific cells"
+                )
+                logging.info("if you did not opt to store all in memory")
+
+            if self.export_raw or self.export_cycles:
+                export_text = "exporting"
+                if self.export_raw:
+                    export_text += " [raw]"
+                if self.export_cycles:
+                    export_text += " [cycles]"
+                logging.info(export_text)
+                n_txt = f"{export_text} {counter}"
+                pbar.set_description(n_txt, refresh=True)
+                cell_data.to_csv(
+                    self.journal.raw_dir,
+                    sep=prms.Reader.sep,
+                    cycles=self.export_cycles,
+                    shifted=self.shifted_cycles,
+                    raw=self.export_raw,
+                    last_cycle=self.last_cycle,
+                )
+
+            if self.export_ica:
+                logging.info("exporting [ica]")
+                try:
+                    helper.export_dqdv(
+                        cell_data,
+                        savedir=self.journal.raw_dir,
+                        sep=prms.Reader.sep,
+                        last_cycle=self.last_cycle,
+                    )
+                except Exception as e:
+                    logging.error("Could not make/export dq/dv data")
+                    logging.debug(
+                        "Failed to make/export " "dq/dv data (%s): %s" % (index, str(e))
+                    )
+                    errors.append("ica:" + str(index))
+
+        self.errors["update"] = errors
+        self.summary_frames = summary_frames
+        self.cell_data_frames = cell_data_frames
+
+    def parallel_update(
+        self, all_in_memory=None, cell_specs=None, logging_mode=None, **kwargs
+    ):
+        """Updates the selected datasets in parallel.
+
+        Args:
+            all_in_memory (bool): store the `cellpydata` in memory (default
+                False)
+            cell_specs (dict of dicts): individual arguments pr. cell. The `cellspecs` key-word argument
+                dictionary will override the **kwargs and the parameters from the journal pages
+                for the indicated cell.
+            logging_mode (str): sets the logging mode for the loader(s).
+
+            kwargs:
+                transferred all the way to the instrument loader, if not
+                picked up earlier. Remark that you can obtain the same pr. cell by
+                providing a `cellspecs` dictionary. The kwargs have precedence over the
+                parameters given in the journal pages, but will be overridden by parameters
+                given by `cellspecs`.
+
+                Merging:
+                    recalc (Bool): set to False if you don't want automatic "recalc" of
+                        cycle numbers etc. when merging several data-sets.
+                Loading:
+                    selector (dict): selector-based parameters sent to the cellpy-file loader (hdf5) if
+                    loading from raw is not necessary (or turned off).
+
+                Debugging:
+                    debug (Bool): set to True if you want to run in debug mode (should never be used by non-developers).
+
+        Debug-mode:
+                 - runs only for the first item in your journal
+
+        Examples:
+            >>> # Don't perform recalculation of cycle numbers etc. when merging
+            >>> # All cells:
+            >>> b.update(recalc=False)
+            >>> # For specific cell(s):
+            >>> cell_specs_cell_01 = {"name_of_cell_01": {"recalc": False}}
+            >>> b.update(cell_specs=cell_specs_cell_01)
+
+        """
+        status = "PROD"  # set this to DEV when developing this
+        async_mode = "threading"
+        logging.debug("PARALLEL UPDATE")
+        # TODO: implement experiment.last_cycle
+        if status != "DEV":
+            print("SORRY - MULTIPROCESSING IS NOT IMPLEMENTED PROPERLY YET")
+            return self.update(
+                all_in_memory=all_in_memory,
+                cell_specs=cell_specs,
+                logging_mode=logging_mode,
+                **kwargs,
+            )
+
+        import concurrent.futures
+        import multiprocessing
+
+        max_number_processes = multiprocessing.cpu_count()
+
+        if async_mode == "threading":
+            pool_executor = concurrent.futures.ThreadPoolExecutor
+        else:
+            pool_executor = concurrent.futures.ProcessPoolExecutor
+
+        debugging = kwargs.pop("debug", False)
+
+        # --- cleaning up attributes / arguments etc ---
+        force_cellpy = kwargs.pop("force_cellpy", self.force_cellpy)
+        force_raw = kwargs.pop("force_raw", self.force_raw)
+
+        logging.info("[update experiment]")
+        if all_in_memory is not None:
+            self.all_in_memory = all_in_memory
+
+        logging.info(f"Additional keyword arguments: {kwargs}")
+        selector = kwargs.get("selector", None)
+
+        pages = self.journal.pages
+        if self.nom_cap:
+            warnings.warn(
+                "Setting nominal capacity through attributes will be deprecated soon since it modifies "
+                "the journal pages."
+            )
+            pages[hdr_journal.nom_cap] = self.nom_cap
+
+        if self.instrument:
+            warnings.warn(
+                "Setting instrument through attributes will be deprecated soon since it modifies the journal pages."
+            )
+            pages[hdr_journal.instrument] = self.instrument
+
+        if x := kwargs.pop("instrument", None):
+            warnings.warn(
+                "Setting instrument through params will be deprecated soon since it modifies the journal pages."
+                "Future version will require instrument in the journal pages."
+            )
+            pages[hdr_journal.instrument] = x
+
+        if pages.empty:
+            raise Exception("your journal is empty")
+
+        # --- init ---
+        summary_frames = dict()
+        cell_data_frames = dict()
+        number_of_runs = len(pages)
+        logging.debug(f"You have {number_of_runs} cells in your journal")
+        counter = 0
+        errors = []
+
+        pbar = tqdm(list(pages.iterrows()), file=sys.stdout, leave=False)
+
+        if debugging:
+            pbar = tqdm(list(pages.iterrows())[0:1], file=sys.stdout, leave=False)
+
+        # --- iterating ---
+        # TODO: create a multiprocessing pool and get one statusbar pr cell
+        params = []
+        with pool_executor(max_number_processes) as executor:
+            for index, row in pages.iterrows():
+                counter += 1
+                cell_spec_page = self._get_cell_spec_from_page(index, row)
+
+                if cell_specs is not None:
+                    cell_spec = cell_specs.get(index, dict())
+                else:
+                    cell_spec = dict()
+
+                cell_spec = {**cell_spec_page, **kwargs, **cell_spec}
+
+                # --- UPDATING ARGUMENTS ---
+                filename = None
+                instrument = None
+                cellpy_file = OtherPath(row[hdr_journal.cellpy_file_name])
+                _cellpy_file = None
+                if not force_raw and cellpy_file.is_file():
+                    _cellpy_file = cellpy_file
+                    logging.debug(f"Got cellpy file: {_cellpy_file}")
+                if not force_cellpy:
+                    filename = row[hdr_journal.raw_file_names]
+                    instrument = row[hdr_journal.instrument]
+
+                cycle_mode = row[hdr_journal.cell_type]
+                mass = row[hdr_journal.mass]
+                nom_cap = row[hdr_journal.nom_cap]
+
+                loading = None
+                area = None
+                if hdr_journal.loading in row:
+                    loading = row[hdr_journal.loading]
+                if hdr_journal.area in row:
+                    area = row[hdr_journal.area]
+
+                summary_kwargs = {
+                    "use_cellpy_stat_file": prms.Reader.use_cellpy_stat_file,
+                }
+
+                step_kwargs = {}
+                if not filename and not force_cellpy:
+                    logging.info(
+                        f"Raw file(s) not given in the journal.pages for index={index}"
+                    )
+                    errors.append(index)
+                    continue
+
+                elif not cellpy_file and force_cellpy:
+                    logging.info(
+                        f"Cellpy file not given in the journal.pages for index={index}"
+                    )
+                    errors.append(index)
+                    continue
+
+                else:
+                    logging.info(f"Processing {index}")
+
+                logging.info("loading cell")
+                params.append(
+                    dict(
+                        filename=filename,
+                        instrument=instrument,
+                        cellpy_file=_cellpy_file,
+                        cycle_mode=cycle_mode,
+                        mass=mass,
+                        nom_cap=nom_cap,
+                        loading=loading,
+                        area=area,
+                        step_kwargs=step_kwargs,
+                        summary_kwargs=summary_kwargs,
+                        selector=selector,
+                        logging_mode=logging_mode,
+                        testing=False,
+                        **cell_spec,
+                    )
+                )
+
+            pool = [executor.submit(cellpy.get, **param) for param in params]
+            for i in concurrent.futures.as_completed(pool):
+                cell_data = i.result()
+                if cell_data.empty:
+                    logging.info("...not loaded...")
+                    logging.debug("Data is empty. Could not load cell!")
+                    errors.append("check:" + str(index))
+
+                logging.info("...loaded successfully...")
+                summary_tmp = cell_data.data.summary
+                logging.info("Trying to get summary_data")
+
+                if cell_data.data.steps is None or self.force_recalc:
+                    logging.info("Running make_step_table")
+                    cell_data.make_step_table()
+
+                if summary_tmp is None or self.force_recalc:
+                    logging.info("Running make_summary")
+                    cell_data.make_summary(find_end_voltage=True, find_ir=True)
+
+                # some clean-ups (might not be needed anymore):
+                if not summary_tmp.index.name == hdr_summary.cycle_index:
+                    logging.debug("Setting index to Cycle_Index")
+                    # check if it is a byte-string
+                    if b"Cycle_Index" in summary_tmp.columns:
+                        logging.debug("Seems to be a byte-string in the column-headers")
+                        summary_tmp.rename(
+                            columns={b"Cycle_Index": "Cycle_Index"}, inplace=True
+                        )
+                    try:
+                        summary_tmp.set_index("cycle_index", inplace=True)
+                    except KeyError:
+                        logging.debug("cycle_index already an index")
+
+                summary_frames[index] = summary_tmp
+
+                if self.all_in_memory:
+                    cell_data_frames[index] = cell_data
+                else:
+                    cell_data_frames[index] = cellreader.CellpyCell(initialize=True)
+                    cell_data_frames[index].data.steps = cell_data.data.steps
+
+                if self.save_cellpy:
+                    logging.info("saving to cellpy-format")
+                    n_txt = f"saving {counter}"
+                    pbar.set_description(n_txt, refresh=True)
+                    if self.custom_data_folder is not None:
+                        print("Save to custom data-folder not implemented yet")
+                        print(f"Saving to {row.cellpy_file_name} instead")
+                    if not row.fixed:
+                        logging.info("saving cell to %s" % row.cellpy_file_name)
+                        cell_data.ensure_step_table = True
+                        try:
+                            cell_data.save(row.cellpy_file_name)
+                        except Exception as e:
+                            logging.error("saving file failed")
+                            logging.error(e)
+
+                    else:
+                        logging.debug("saving cell skipped (set to 'fixed' in info_df)")
+                else:
+                    logging.info("You opted to not save to cellpy-format")
+                    logging.info("It is usually recommended to save to cellpy-format:")
+                    logging.info(" >>> b.experiment.save_cellpy = True")
+                    logging.info(
+                        "Without the cellpy-files, you cannot select specific cells"
+                    )
+                    logging.info("if you did not opt to store all in memory")
+
+                if self.export_raw or self.export_cycles:
+                    export_text = "exporting"
+                    if self.export_raw:
+                        export_text += " [raw]"
+                    if self.export_cycles:
+                        export_text += " [cycles]"
+                    logging.info(export_text)
+                    n_txt = f"{export_text} {counter}"
+                    pbar.set_description(n_txt, refresh=True)
+                    cell_data.to_csv(
+                        self.journal.raw_dir,
+                        sep=prms.Reader.sep,
+                        cycles=self.export_cycles,
+                        shifted=self.shifted_cycles,
+                        raw=self.export_raw,
+                        last_cycle=self.last_cycle,
+                    )
+
+                if self.export_ica:
+                    logging.info("exporting [ica]")
+                    try:
+                        helper.export_dqdv(
+                            cell_data,
+                            savedir=self.journal.raw_dir,
+                            sep=prms.Reader.sep,
+                            last_cycle=self.last_cycle,
+                        )
+                    except Exception as e:
+                        logging.error("Could not make/export dq/dv data")
+                        logging.debug(
+                            "Failed to make/export "
+                            "dq/dv data (%s): %s" % (index, str(e))
+                        )
+                        errors.append("ica:" + str(index))
+
+        self.errors["update"] = errors
+        self.summary_frames = summary_frames
+        self.cell_data_frames = cell_data_frames
+
+    def export_cellpy_files(self, path=None, **kwargs):
+        """Export all cellpy-files to a given path.
+
+        Remarks:
+            This method can only export to local folders
+            (OtherPath objects are not formally supported, but
+            might still work if the path is local).
+
+        Args:
+            path (str, pathlib.Path): path to export to (default: current working directory)
+        """
+        if path is None:
+            path = "."
+        errors = []
+        path = pathlib.Path(path)
+        cell_names = self.cell_names
+        for cell_name in cell_names:
+            cellpy_file_name = self.journal.pages.loc[
+                cell_name, hdr_journal.cellpy_file_name
+            ]
+            cellpy_file_name = path / pathlib.Path(cellpy_file_name).name
+            print(f"Exporting {cell_name} to {cellpy_file_name}")
+            try:
+                c = self.data[cell_name]
+            except TypeError as e:
+                errors.append(f"could not extract data for {cell_name} - linking")
+                self._link_cellpy_file(cell_name)
+
+            c.save(cellpy_file_name, **kwargs)
+        self.errors["export_cellpy_files"] = errors
+
+    @property
+    def cell_names(self):
+        """Returns a list of cell-names (strings)"""
+        try:
+            return [key for key in self.cell_data_frames]
+        except TypeError:
+            return None
+
+    def status(self):
+        print("\n")
+        print(" STATUS ".center(80, "="))
+        print(self)
+        print(" summary frames ".center(80, "-"))
+        if self.summary_frames is not None:
+            for key in self.summary_frames:
+                print(f" {{{key}}}")
+        print(" memory dumped ".center(80, "-"))
+        if self.memory_dumped is not None:
+            for key in self.memory_dumped:
+                print(f"{key}: {type(self.memory_dumped[key])}")
+        print(80 * "=")
+
+    def link(self, **kwargs):
+        """Ensure that an appropriate link to the cellpy-files exists for
+        each cell.
+
+        The experiment will then contain a CellpyCell object for each cell
+        (in the cell_data_frames attribute) with only the step-table stored.
+
+        Remark that running update persists the summary frames instead (or
+        everything in case you specify all_in_memory=True).
+        This might be considered "a strange and unexpected behaviour". Sorry
+        for that (but the authors of this package is also a bit strange...).
+
+        (OK, I will change it. Soon.)
+
+        **kwargs: passed to _link_cellpy_file
+            max_cycle (int): maximum cycle number to link/load (remark that the
+                cellpy objects will get the property overwrite_able set to False
+                if you give a max_cycle to prevent accidentally saving a "truncated"
+                file (use c.save(filename, overwrite=True) to force overwrite))
+
+
+        """
+        logging.info("[establishing links]")
+        logging.debug("checking and establishing link to data")
+
+        errors = []
+
+        for cell_label in self.journal.pages.index:
+            logging.debug(f"trying to link {cell_label}")
+            try:
+                self._link_cellpy_file(cell_label, **kwargs)
+            except IOError as e:
+                logging.warning(e)
+                e_txt = f"{cell_label}: links not established - try update instead"
+                logging.warning(e_txt)
+                errors.append(e_txt)
+
+        self.errors["link"] = errors
+
+    def recalc(
+        self,
+        save=True,
+        step_opts=None,
+        summary_opts=None,
+        indexes=None,
+        calc_steps=True,
+        testing=False,
+    ):
+        """Run make_step_table and make_summary on all cells.
+
+        Args:
+            save (bool): Save updated cellpy-files if True.
+            step_opts (dict): parameters to inject to make_steps.
+            summary_opts (dict): parameters to inject to make_summary.
+            indexes (list): Only recalculate for given indexes (i.e. list of cell-names).
+            calc_steps (bool): Run make_steps before making the summary.
+            testing (bool): Only for testing purposes.
+
+        Returns:
+            None
+        """
+
+        # TODO: option (default) to only recalc if the values (mass, nom_cap,...) have changed
+        errors = []
+        log = []
+        if testing:
+            pbar = tqdm(
+                list(self.journal.pages.iloc[0:2, :].iterrows()),
+                file=sys.stdout,
+                leave=False,
+            )
+        elif indexes is not None:
+            pbar = tqdm(
+                list(self.journal.pages.loc[indexes, :].iterrows()),
+                file=sys.stdout,
+                leave=False,
+            )
+        else:
+            pbar = tqdm(
+                list(self.journal.pages.iterrows()), file=sys.stdout, leave=False
+            )
+        for indx, row in pbar:
+            nom_cap = row[hdr_journal.nom_cap]
+            mass = row[hdr_journal.mass]
+            pbar.set_description(indx)
+            try:
+                c = self.data[indx]
+            except TypeError as e:
+                e_txt = (
+                    f"could not extract data for {indx} - have you forgotten to link?"
+                )
+                errors.append(e_txt)
+                warnings.warn(e_txt)
+
+            else:
+                if nom_cap:
+                    c.set_nom_cap(nom_cap)
+                if mass:
+                    c.set_mass(mass)
+                try:
+                    if calc_steps:
+                        pbar.set_postfix_str(s="steps", refresh=True)
+                        if step_opts is not None:
+                            c.make_step_table(**step_opts)
+                        else:
+                            c.make_step_table()
+
+                    pbar.set_postfix_str(s="summary", refresh=True)
+                    if summary_opts is not None:
+                        c.make_summary(**summary_opts)
+                    else:
+                        c.make_summary(find_end_voltage=True, find_ir=True)
+
+                except Exception as e:
+                    e_txt = f"recalculating for {indx} failed!"
+                    errors.append(e_txt)
+                    warnings.warn(e_txt)
+                else:
+                    if save:
+                        # remark! got a win error when trying to save (hdf5-file in use) (must fix this)
+                        pbar.set_postfix_str(s="save", refresh=True)
+                        try:
+                            c.save(row.cellpy_file_name)
+                            log.append(f"saved {indx} to {row.cellpy_file_name}")
+                        except Exception as e:
+                            e_txt = f"saving {indx} to {row.cellpy_file_name} failed!"
+                            errors.append(e_txt)
+                            warnings.warn(e_txt)
+        self.errors["recalc"] = errors
+        self.log["recalc"] = log
+
+
+class ImpedanceExperiment(BaseExperiment):
+    def __init__(self):
+        super().__init__()
+
+
+class LifeTimeExperiment(BaseExperiment):
+    def __init__(self):
+        super().__init__()
+
+
+if __name__ == "__main__":
+    from pathlib import Path
+    import os
+    import pandas as pd
+    import numpy as np
+    import seaborn as sns
+    import plotly.express as px
+
+    import cellpy
+    from cellpy.utils import batch, helpers, plotutils
+
+    project_dir = Path("../../../testdata/batch_project")
+    print(f"{project_dir.resolve()=}")
+    journal = project_dir / "test_project.json"
+    journal = journal.resolve()
+    print(f"{journal=}")
+    assert project_dir.is_dir()
+    assert journal.is_file()
+    os.chdir(project_dir)
+
+    print(f"cellpy version: {cellpy.__version__}")
+    cellpy.log.setup_logging("INFO")
+
+    b = batch.from_journal(journal)
+    b.update()
+
+    print("Ended OK")
```

### Comparing `cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_exporters.py` & `cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_exporters.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_helpers.py` & `cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,377 +1,381 @@
-import csv
-import itertools
-import logging
-import os
-import warnings
-
-import pandas as pd
-
-import cellpy.parameters.internal_settings
-from cellpy import filefinder, prms
-from cellpy.readers import core
-from cellpy.exceptions import ExportFailed, NullData, WrongFileVersion
-
-# logger = logging.getLogger(__name__)
-from cellpy.parameters.internal_settings import headers_step_table
-
-hdr_summary = cellpy.parameters.internal_settings.get_headers_summary()
-hdr_journal = cellpy.parameters.internal_settings.get_headers_journal()
-
-
-CELL_TYPE_IDS = ["cc", "ec", "eth"]
-
-
-def look_up_and_get(cellpy_file_name, table_name, root=None, max_cycle=None):
-    """Extracts table from cellpy hdf5-file."""
-
-    # infoname = '/CellpyData/info'
-    # dataname = '/CellpyData/dfdata'
-    # summaryname = '/CellpyData/dfsummary'
-    # fidname = '/CellpyData/fidtable'
-    # stepname = '/CellpyData/step_table'
-
-    if root is None:
-        root = "/CellpyData"
-    table_path = "/".join([root, table_name])
-
-    logging.debug(f"look_up_and_get({cellpy_file_name}, {table_name}")
-    store = pd.HDFStore(cellpy_file_name)
-    # max_cycle is not implemented properly yet
-    # TODO: implement max_cycle
-    try:
-        if max_cycle and table_name == prms._cellpyfile_step:
-            _cycle_header = headers_step_table.cycle
-            cycles = store.select(table_path, where="columns=[_cycle_header]")
-            _where = cycles[_cycle_header] <= max_cycle
-            table = store.select(table_path, where=_where)
-        else:
-            table = store.select(table_path)
-        store.close()
-    except KeyError as e:
-        logging.warning("Could not read the table")
-        store.close()
-        raise WrongFileVersion(e)
-    return table
-
-
-def create_folder_structure(project_name, batch_name):
-    """This function creates a folder structure for the batch project.
-
-    The folder structure consists of main working folder ``project_name`
-    located in the ``outdatadir`` (as defined in the cellpy configuration file)
-    with a sub-folder named ``batch_name``. It also creates a folder
-    inside the ``batch_name`` folder for storing the raw data.
-    If the folders does not exist, they will be made. The function also returns
-    the name of the info-df.
-
-    Args:
-        project_name: name of the project
-        batch_name: name of the batch
-
-    Returns: (info_file, (project_dir, batch_dir, raw_dir))
-
-    """
-    out_data_dir = prms.Paths.outdatadir
-    project_dir = os.path.join(out_data_dir, project_name)
-    batch_dir = os.path.join(project_dir, batch_name)
-    raw_dir = os.path.join(batch_dir, "raw_data")
-
-    # create folders
-    if not os.path.isdir(project_dir):
-        os.mkdir(project_dir)
-    if not os.path.isdir(batch_dir):
-        os.mkdir(batch_dir)
-    if not os.path.isdir(raw_dir):
-        os.mkdir(raw_dir)
-
-    # create file-name for the info_df (json)
-    info_file = "cellpy_batch_%s.json" % batch_name
-    info_file = os.path.join(project_dir, info_file)
-    return info_file, (project_dir, batch_dir, raw_dir)
-
-
-def create_factory():
-    instrument_factory = core.InstrumentFactory()
-    instruments = core.find_all_instruments()
-    for instrument_id, instrument in instruments.items():
-        instrument_factory.register_builder(instrument_id, instrument)
-    return instrument_factory
-
-
-def find_files(info_dict, file_list=None, pre_path=None, sub_folders=None, **kwargs):
-    """Find files using cellpy.filefinder.
-
-    Args:
-        info_dict: journal pages.
-        file_list: list of files names to search through.
-        pre_path: path to prepend found files from file_list (if file_list is given).
-        sub_folders (bool): perform search also in sub-folders.
-
-    **kwargs (filefinder.search_for_files):
-        run_name(str): run-file identification.
-        raw_extension(str): optional, extension of run-files (without the '.').
-        cellpy_file_extension(str): optional, extension for cellpy files
-            (without the '.').
-        raw_file_dir(path): optional, directory where to look for run-files
-            (default: read prm-file)
-        cellpy_file_dir(path): optional, directory where to look for
-            cellpy-files (default: read prm-file)
-        prm_filename(path): optional parameter file can be given.
-        file_name_format(str): format of raw-file names or a glob pattern
-            (default: YYYYMMDD_[name]EEE_CC_TT_RR).
-        reg_exp(str): use regular expression instead (defaults to None).
-        file_list (list of str): perform the search within a given list
-            of filenames instead of searching the folder(s). The list should
-            not contain the full filepath (only the actual file names). If
-            you want to provide the full path, you will have to modify the
-            file_name_format or reg_exp accordingly.
-        pre_path (path or str): path to prepend the list of files selected
-             from the file_list.
-
-    Returns:
-        info_dict
-    """
-    sub_folders = sub_folders or prms.FileNames.sub_folders
-    instrument_factory = create_factory()
-    # searches for the raw data files and the cellpyfile-name
-    # TODO: implement faster file searching
-    # TODO: implement option for not searching for raw-file names if force_cellpy is True
-    for i, run_name in enumerate(info_dict[hdr_journal["filename"]]):
-        try:
-            instrument = info_dict[hdr_journal["instrument"]][i]
-            raw_ext = instrument_factory.query(instrument, "raw_ext")
-            if raw_ext:
-                prms.FileNames.raw_extension = raw_ext
-        except IndexError:
-            warnings.warn(f"no instrument given for {run_name}")
-
-        logging.debug(f"checking for {run_name}")
-        raw_files, cellpyfile = filefinder.search_for_files(
-            run_name, file_list=file_list, pre_path=pre_path, sub_folders=sub_folders, **kwargs
-        )
-        if not raw_files:
-            raw_files = None
-        info_dict[hdr_journal["raw_file_names"]].append(raw_files)
-        info_dict[hdr_journal["cellpy_file_name"]].append(cellpyfile)
-
-    return info_dict
-
-
-def fix_groups(groups):
-    """Takes care of strange group numbers."""
-    _groups = []
-    unique_groups = list(set(groups))
-    lookup = {}
-    for i, g in enumerate(unique_groups):
-        lookup[g] = i + 1
-    for i, g in enumerate(groups):
-        _groups.append(lookup[g])
-    return _groups
-
-
-def save_multi(data, file_name, sep=";"):
-    """Convenience function for storing data column-wise in a csv-file."""
-    logging.debug("saving multi")
-    with open(file_name, "w", newline="") as f:
-        logging.debug(f"{file_name} opened")
-        writer = csv.writer(f, delimiter=sep)
-        try:
-            writer.writerows(itertools.zip_longest(*data))
-            logging.info(f"{file_name} OK")
-        except Exception as e:
-            logging.info(f"Exception encountered in batch._save_multi: {e}")
-            raise ExportFailed
-        logging.debug("wrote rows using itertools in _save_multi")
-
-
-def make_unique_groups(info_df):
-    """This function cleans up the group numbers a bit."""
-    # fixes group numbering
-    unique_g = info_df[hdr_journal.group].unique()
-    unique_g = sorted(unique_g)
-    new_unique_g = list(range(len(unique_g)))
-    info_df[hdr_journal.sub_group] = info_df[hdr_journal.group] * 0
-    for i, j in zip(unique_g, new_unique_g):
-        counter = 1
-        for indx, row in info_df.loc[info_df[hdr_journal.group] == i].iterrows():
-            info_df.at[indx, hdr_journal.sub_group] = counter
-            counter += 1
-        info_df.loc[info_df[hdr_journal.group] == i, hdr_journal.group] = j + 1
-    return info_df
-
-
-def _remove_date_and_celltype(
-    label,
-):
-    parts = label.split("_")
-    parts.pop(0)
-    if parts[-1] in CELL_TYPE_IDS:
-        parts.pop(-1)
-    return "_".join(parts)
-
-
-def create_labels(label, *args):
-    """Returns a re-formatted label (currently it only removes the dates
-    from the run-name)"""
-    return _remove_date_and_celltype(label)
-
-
-def create_selected_summaries_dict(summaries_list):
-    """Creates a dictionary with summary column headers.
-
-    Examples:
-        >>> summaries_to_output = ["discharge_capacity_gravimetric", "charge_capacity_gravimetric"]
-        >>> summaries_to_output_dict = create_selected_summaries_dict(
-        >>>    summaries_to_output
-        >>> )
-        >>> print(summaries_to_output_dict)
-        {'discharge_capacity_gravimetric': "discharge_capacity_gravimetric",
-               'charge_capacity_gravimetric': "discharge_capacity_gravimetric"}
-
-    Args:
-        summaries_list: list containing cellpy summary column id names
-
-    Returns: dictionary of the form {cellpy id name: cellpy summary
-        header name,}
-
-    """
-    selected_summaries = dict()
-    for h in summaries_list:
-        selected_summaries[h] = hdr_summary[h]
-    return selected_summaries
-
-
-def pick_summary_data(key, summary_df, selected_summaries):
-    """picks the selected pandas.DataFrame"""
-
-    selected_summaries_dict = create_selected_summaries_dict(selected_summaries)
-    value = selected_summaries_dict[key]
-    return summary_df.iloc[:, summary_df.columns.get_level_values(1) == value]
-
-
-def join_summaries(summary_frames, selected_summaries, keep_old_header=False):
-    """parse the summaries and combine based on column (selected_summaries)"""
-    if not summary_frames:
-        raise NullData("No summaries available to join")
-    selected_summaries_dict = create_selected_summaries_dict(selected_summaries)
-    out = []
-    frames = []
-    keys = []  # test-name
-
-    for key in summary_frames:
-        keys.append(key)
-        if summary_frames[key].empty:
-            logging.debug("Empty summary_frame encountered")
-
-        frames.append(summary_frames[key])
-
-    summary_df = pd.concat(frames, keys=keys, axis=1, sort=True)
-
-    for key, value in selected_summaries_dict.items():
-        _summary_df = summary_df.iloc[
-            :, summary_df.columns.get_level_values(1) == value
-        ]
-        _summary_df.name = key
-
-        if not keep_old_header:
-            try:
-                _summary_df.columns = _summary_df.columns.droplevel(-1)
-            except AttributeError as e:
-                logging.debug("could not drop level from frame")
-                logging.debug(e)
-
-        out.append(_summary_df)
-    logging.debug("finished joining summaries")
-
-    return out
-
-
-def generate_folder_names(name, project):
-    """Creates sensible folder names."""
-
-    out_data_dir = prms.Paths.outdatadir
-    project_dir = os.path.join(out_data_dir, project)
-    batch_dir = os.path.join(project_dir, name)
-    raw_dir = os.path.join(batch_dir, "raw_data")
-    return out_data_dir, project_dir, batch_dir, raw_dir
-
-
-def _extract_dqdv(cell_data, extract_func, last_cycle):
-    """Simple wrapper around the cellpy.utils.ica.dqdv function."""
-
-    from cellpy.utils.ica import dqdv
-
-    list_of_cycles = cell_data.get_cycle_numbers()
-    if last_cycle is not None:
-        list_of_cycles = [c for c in list_of_cycles if c <= int(last_cycle)]
-        logging.debug(f"only processing up to cycle {last_cycle}")
-        logging.debug(f"you have {len(list_of_cycles)} cycles to process")
-    out_data = []
-    for cycle in list_of_cycles:
-        try:
-            c, v = extract_func(cycle)
-            v, dq = dqdv(v, c)
-            v = v.tolist()
-            dq = dq.tolist()
-        except NullData as e:
-            v = list()
-            dq = list()
-            logging.info(" Ups! Could not process this (cycle %i)" % cycle)
-            logging.info(" %s" % e)
-
-        header_x = "dQ cycle_no %i" % cycle
-        header_y = "voltage cycle_no %i" % cycle
-        dq.insert(0, header_x)
-        v.insert(0, header_y)
-
-        out_data.append(v)
-        out_data.append(dq)
-    return out_data
-
-
-def export_dqdv(cell_data, savedir, sep, last_cycle=None):
-    """Exports dQ/dV data from a CellpyCell instance.
-
-    Args:
-        cell_data: CellpyCell instance
-        savedir: path to the folder where the files should be saved
-        sep: separator for the .csv-files.
-        last_cycle: only export up to this cycle (if not None)
-    """
-    logging.debug("exporting dqdv")
-    filename = cell_data.data.loaded_from
-    no_merged_sets = ""
-    firstname, extension = os.path.splitext(filename)
-    firstname += no_merged_sets
-    if savedir:
-        firstname = os.path.join(savedir, os.path.basename(firstname))
-        logging.debug(f"savedir is true: {firstname}")
-
-    outname_charge = firstname + "_dqdv_charge.csv"
-    outname_discharge = firstname + "_dqdv_discharge.csv"
-
-    list_of_cycles = cell_data.get_cycle_numbers()
-    number_of_cycles = len(list_of_cycles)
-    logging.debug("%s: you have %i cycles" % (filename, number_of_cycles))
-
-    # extracting charge
-    out_data = _extract_dqdv(cell_data, cell_data.get_ccap, last_cycle)
-    logging.debug("extracted ica for charge")
-    try:
-        save_multi(data=out_data, file_name=outname_charge, sep=sep)
-    except ExportFailed as e:
-        logging.info("could not export ica for charge")
-        warnings.warn(f"ExportFailed exception raised: {e}")
-    else:
-        logging.debug("saved ica for charge")
-
-    # extracting discharge
-    out_data = _extract_dqdv(cell_data, cell_data.get_dcap, last_cycle)
-    logging.debug("extracted ica for discharge")
-    try:
-        save_multi(data=out_data, file_name=outname_discharge, sep=sep)
-    except ExportFailed as e:
-        logging.info("could not export ica for discharge")
-        warnings.warn(f"ExportFailed exception raised: {e}")
-    else:
-        logging.debug("saved ica for discharge")
+import csv
+import itertools
+import logging
+import os
+import warnings
+
+import pandas as pd
+
+import cellpy.parameters.internal_settings
+from cellpy import filefinder, prms
+from cellpy.readers import core
+from cellpy.exceptions import ExportFailed, NullData, WrongFileVersion
+
+# logger = logging.getLogger(__name__)
+from cellpy.parameters.internal_settings import headers_step_table
+
+hdr_summary = cellpy.parameters.internal_settings.get_headers_summary()
+hdr_journal = cellpy.parameters.internal_settings.get_headers_journal()
+
+
+CELL_TYPE_IDS = ["cc", "ec", "eth"]
+
+
+def look_up_and_get(cellpy_file_name, table_name, root=None, max_cycle=None):
+    """Extracts table from cellpy hdf5-file."""
+
+    # infoname = '/CellpyData/info'
+    # dataname = '/CellpyData/dfdata'
+    # summaryname = '/CellpyData/dfsummary'
+    # fidname = '/CellpyData/fidtable'
+    # stepname = '/CellpyData/step_table'
+
+    if root is None:
+        root = "/CellpyData"
+    table_path = "/".join([root, table_name])
+
+    logging.debug(f"look_up_and_get({cellpy_file_name}, {table_name}")
+    store = pd.HDFStore(cellpy_file_name)
+    # max_cycle is not implemented properly yet
+    # TODO: implement max_cycle
+    try:
+        if max_cycle and table_name == prms._cellpyfile_step:
+            _cycle_header = headers_step_table.cycle
+            cycles = store.select(table_path, where="columns=[_cycle_header]")
+            _where = cycles[_cycle_header] <= max_cycle
+            table = store.select(table_path, where=_where)
+        else:
+            table = store.select(table_path)
+        store.close()
+    except KeyError as e:
+        logging.warning("Could not read the table")
+        store.close()
+        raise WrongFileVersion(e)
+    return table
+
+
+def create_folder_structure(project_name, batch_name):
+    """This function creates a folder structure for the batch project.
+
+    The folder structure consists of main working folder ``project_name`
+    located in the ``outdatadir`` (as defined in the cellpy configuration file)
+    with a sub-folder named ``batch_name``. It also creates a folder
+    inside the ``batch_name`` folder for storing the raw data.
+    If the folders does not exist, they will be made. The function also returns
+    the name of the info-df.
+
+    Args:
+        project_name: name of the project
+        batch_name: name of the batch
+
+    Returns: (info_file, (project_dir, batch_dir, raw_dir))
+
+    """
+    out_data_dir = prms.Paths.outdatadir
+    project_dir = os.path.join(out_data_dir, project_name)
+    batch_dir = os.path.join(project_dir, batch_name)
+    raw_dir = os.path.join(batch_dir, "raw_data")
+
+    # create folders
+    if not os.path.isdir(project_dir):
+        os.mkdir(project_dir)
+    if not os.path.isdir(batch_dir):
+        os.mkdir(batch_dir)
+    if not os.path.isdir(raw_dir):
+        os.mkdir(raw_dir)
+
+    # create file-name for the info_df (json)
+    info_file = "cellpy_batch_%s.json" % batch_name
+    info_file = os.path.join(project_dir, info_file)
+    return info_file, (project_dir, batch_dir, raw_dir)
+
+
+def create_factory():
+    instrument_factory = core.InstrumentFactory()
+    instruments = core.find_all_instruments()
+    for instrument_id, instrument in instruments.items():
+        instrument_factory.register_builder(instrument_id, instrument)
+    return instrument_factory
+
+
+def find_files(info_dict, file_list=None, pre_path=None, sub_folders=None, **kwargs):
+    """Find files using cellpy.filefinder.
+
+    Args:
+        info_dict: journal pages.
+        file_list: list of files names to search through.
+        pre_path: path to prepend found files from file_list (if file_list is given).
+        sub_folders (bool): perform search also in sub-folders.
+
+    **kwargs (filefinder.search_for_files):
+        run_name(str): run-file identification.
+        raw_extension(str): optional, extension of run-files (without the '.').
+        cellpy_file_extension(str): optional, extension for cellpy files
+            (without the '.').
+        raw_file_dir(path): optional, directory where to look for run-files
+            (default: read prm-file)
+        cellpy_file_dir(path): optional, directory where to look for
+            cellpy-files (default: read prm-file)
+        prm_filename(path): optional parameter file can be given.
+        file_name_format(str): format of raw-file names or a glob pattern
+            (default: YYYYMMDD_[name]EEE_CC_TT_RR).
+        reg_exp(str): use regular expression instead (defaults to None).
+        file_list (list of str): perform the search within a given list
+            of filenames instead of searching the folder(s). The list should
+            not contain the full filepath (only the actual file names). If
+            you want to provide the full path, you will have to modify the
+            file_name_format or reg_exp accordingly.
+        pre_path (path or str): path to prepend the list of files selected
+             from the file_list.
+
+    Returns:
+        info_dict
+    """
+    sub_folders = sub_folders or prms.FileNames.sub_folders
+    instrument_factory = create_factory()
+    # searches for the raw data files and the cellpyfile-name
+    # TODO: implement faster file searching
+    # TODO: implement option for not searching for raw-file names if force_cellpy is True
+    for i, run_name in enumerate(info_dict[hdr_journal["filename"]]):
+        try:
+            instrument = info_dict[hdr_journal["instrument"]][i]
+            raw_ext = instrument_factory.query(instrument, "raw_ext")
+            if raw_ext:
+                prms.FileNames.raw_extension = raw_ext
+        except IndexError:
+            warnings.warn(f"no instrument given for {run_name}")
+
+        logging.debug(f"checking for {run_name}")
+        raw_files, cellpyfile = filefinder.search_for_files(
+            run_name,
+            file_list=file_list,
+            pre_path=pre_path,
+            sub_folders=sub_folders,
+            **kwargs,
+        )
+        if not raw_files:
+            raw_files = None
+        info_dict[hdr_journal["raw_file_names"]].append(raw_files)
+        info_dict[hdr_journal["cellpy_file_name"]].append(cellpyfile)
+
+    return info_dict
+
+
+def fix_groups(groups):
+    """Takes care of strange group numbers."""
+    _groups = []
+    unique_groups = list(set(groups))
+    lookup = {}
+    for i, g in enumerate(unique_groups):
+        lookup[g] = i + 1
+    for i, g in enumerate(groups):
+        _groups.append(lookup[g])
+    return _groups
+
+
+def save_multi(data, file_name, sep=";"):
+    """Convenience function for storing data column-wise in a csv-file."""
+    logging.debug("saving multi")
+    with open(file_name, "w", newline="") as f:
+        logging.debug(f"{file_name} opened")
+        writer = csv.writer(f, delimiter=sep)
+        try:
+            writer.writerows(itertools.zip_longest(*data))
+            logging.info(f"{file_name} OK")
+        except Exception as e:
+            logging.info(f"Exception encountered in batch._save_multi: {e}")
+            raise ExportFailed
+        logging.debug("wrote rows using itertools in _save_multi")
+
+
+def make_unique_groups(info_df):
+    """This function cleans up the group numbers a bit."""
+    # fixes group numbering
+    unique_g = info_df[hdr_journal.group].unique()
+    unique_g = sorted(unique_g)
+    new_unique_g = list(range(len(unique_g)))
+    info_df[hdr_journal.sub_group] = info_df[hdr_journal.group] * 0
+    for i, j in zip(unique_g, new_unique_g):
+        counter = 1
+        for indx, row in info_df.loc[info_df[hdr_journal.group] == i].iterrows():
+            info_df.at[indx, hdr_journal.sub_group] = counter
+            counter += 1
+        info_df.loc[info_df[hdr_journal.group] == i, hdr_journal.group] = j + 1
+    return info_df
+
+
+def _remove_date_and_celltype(
+    label,
+):
+    parts = label.split("_")
+    parts.pop(0)
+    if parts[-1] in CELL_TYPE_IDS:
+        parts.pop(-1)
+    return "_".join(parts)
+
+
+def create_labels(label, *args):
+    """Returns a re-formatted label (currently it only removes the dates
+    from the run-name)"""
+    return _remove_date_and_celltype(label)
+
+
+def create_selected_summaries_dict(summaries_list):
+    """Creates a dictionary with summary column headers.
+
+    Examples:
+        >>> summaries_to_output = ["discharge_capacity_gravimetric", "charge_capacity_gravimetric"]
+        >>> summaries_to_output_dict = create_selected_summaries_dict(
+        >>>    summaries_to_output
+        >>> )
+        >>> print(summaries_to_output_dict)
+        {'discharge_capacity_gravimetric': "discharge_capacity_gravimetric",
+               'charge_capacity_gravimetric': "discharge_capacity_gravimetric"}
+
+    Args:
+        summaries_list: list containing cellpy summary column id names
+
+    Returns: dictionary of the form {cellpy id name: cellpy summary
+        header name,}
+
+    """
+    selected_summaries = dict()
+    for h in summaries_list:
+        selected_summaries[h] = hdr_summary[h]
+    return selected_summaries
+
+
+def pick_summary_data(key, summary_df, selected_summaries):
+    """picks the selected pandas.DataFrame"""
+
+    selected_summaries_dict = create_selected_summaries_dict(selected_summaries)
+    value = selected_summaries_dict[key]
+    return summary_df.iloc[:, summary_df.columns.get_level_values(1) == value]
+
+
+def join_summaries(summary_frames, selected_summaries, keep_old_header=False):
+    """parse the summaries and combine based on column (selected_summaries)"""
+    if not summary_frames:
+        raise NullData("No summaries available to join")
+    selected_summaries_dict = create_selected_summaries_dict(selected_summaries)
+    out = []
+    frames = []
+    keys = []  # test-name
+
+    for key in summary_frames:
+        keys.append(key)
+        if summary_frames[key].empty:
+            logging.debug("Empty summary_frame encountered")
+
+        frames.append(summary_frames[key])
+
+    summary_df = pd.concat(frames, keys=keys, axis=1, sort=True)
+
+    for key, value in selected_summaries_dict.items():
+        _summary_df = summary_df.iloc[
+            :, summary_df.columns.get_level_values(1) == value
+        ]
+        _summary_df.name = key
+
+        if not keep_old_header:
+            try:
+                _summary_df.columns = _summary_df.columns.droplevel(-1)
+            except AttributeError as e:
+                logging.debug("could not drop level from frame")
+                logging.debug(e)
+
+        out.append(_summary_df)
+    logging.debug("finished joining summaries")
+
+    return out
+
+
+def generate_folder_names(name, project):
+    """Creates sensible folder names."""
+
+    out_data_dir = prms.Paths.outdatadir
+    project_dir = os.path.join(out_data_dir, project)
+    batch_dir = os.path.join(project_dir, name)
+    raw_dir = os.path.join(batch_dir, "raw_data")
+    return out_data_dir, project_dir, batch_dir, raw_dir
+
+
+def _extract_dqdv(cell_data, extract_func, last_cycle):
+    """Simple wrapper around the cellpy.utils.ica.dqdv function."""
+
+    from cellpy.utils.ica import dqdv
+
+    list_of_cycles = cell_data.get_cycle_numbers()
+    if last_cycle is not None:
+        list_of_cycles = [c for c in list_of_cycles if c <= int(last_cycle)]
+        logging.debug(f"only processing up to cycle {last_cycle}")
+        logging.debug(f"you have {len(list_of_cycles)} cycles to process")
+    out_data = []
+    for cycle in list_of_cycles:
+        try:
+            c, v = extract_func(cycle, return_dataframe=False)
+            v, dq = dqdv(v, c)
+            v = v.tolist()
+            dq = dq.tolist()
+        except NullData as e:
+            v = list()
+            dq = list()
+            logging.info(" Ups! Could not process this (cycle %i)" % cycle)
+            logging.info(" %s" % e)
+
+        header_x = "dQ cycle_no %i" % cycle
+        header_y = "voltage cycle_no %i" % cycle
+        dq.insert(0, header_x)
+        v.insert(0, header_y)
+
+        out_data.append(v)
+        out_data.append(dq)
+    return out_data
+
+
+def export_dqdv(cell_data, savedir, sep, last_cycle=None):
+    """Exports dQ/dV data from a CellpyCell instance.
+
+    Args:
+        cell_data: CellpyCell instance
+        savedir: path to the folder where the files should be saved
+        sep: separator for the .csv-files.
+        last_cycle: only export up to this cycle (if not None)
+    """
+    logging.debug("exporting dqdv")
+    filename = cell_data.data.loaded_from
+    no_merged_sets = ""
+    firstname, extension = os.path.splitext(filename)
+    firstname += no_merged_sets
+    if savedir:
+        firstname = os.path.join(savedir, os.path.basename(firstname))
+        logging.debug(f"savedir is true: {firstname}")
+
+    outname_charge = firstname + "_dqdv_charge.csv"
+    outname_discharge = firstname + "_dqdv_discharge.csv"
+
+    list_of_cycles = cell_data.get_cycle_numbers()
+    number_of_cycles = len(list_of_cycles)
+    logging.debug("%s: you have %i cycles" % (filename, number_of_cycles))
+
+    # extracting charge
+    out_data = _extract_dqdv(cell_data, cell_data.get_ccap, last_cycle)
+    logging.debug("extracted ica for charge")
+    try:
+        save_multi(data=out_data, file_name=outname_charge, sep=sep)
+    except ExportFailed as e:
+        logging.info("could not export ica for charge")
+        warnings.warn(f"ExportFailed exception raised: {e}")
+    else:
+        logging.debug("saved ica for charge")
+
+    # extracting discharge
+    out_data = _extract_dqdv(cell_data, cell_data.get_dcap, last_cycle)
+    logging.debug("extracted ica for discharge")
+    try:
+        save_multi(data=out_data, file_name=outname_discharge, sep=sep)
+    except ExportFailed as e:
+        logging.info("could not export ica for discharge")
+        warnings.warn(f"ExportFailed exception raised: {e}")
+    else:
+        logging.debug("saved ica for discharge")
```

### Comparing `cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_journals.py` & `cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_journals.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/batch_tools/batch_plotters.py` & `cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_plotters.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/batch_tools/dumpers.py` & `cellpy-1.0.0a4/cellpy/utils/batch_tools/dumpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/batch_tools/engines.py` & `cellpy-1.0.0a4/cellpy/utils/batch_tools/engines.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/batch_tools/sqlite_from_excel_db.py` & `cellpy-1.0.0a4/cellpy/utils/batch_tools/sqlite_from_excel_db.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/collectors.py` & `cellpy-1.0.0a4/cellpy/utils/collectors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/collectors_old.py` & `cellpy-1.0.0a4/cellpy/utils/collectors_old.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/data/20160805_test001_45_cc.h5` & `cellpy-1.0.0a4/cellpy/utils/data/20160805_test001_45_cc.h5`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/data/raw/20160805_test001_45_cc_01.res` & `cellpy-1.0.0a4/cellpy/utils/data/raw/20160805_test001_45_cc_01.res`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/easyplot.py` & `cellpy-1.0.0a4/cellpy/utils/easyplot.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/example_data.py` & `cellpy-1.0.0a4/cellpy/utils/example_data.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/helpers.py` & `cellpy-1.0.0a4/cellpy/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/ica.py` & `cellpy-1.0.0a4/cellpy/utils/ica.py`

 * *Files 0% similar despite different names*

```diff
@@ -983,15 +983,15 @@
 
     cell = _get_a_cell_to_play_with()
     cycle = 5
     print("looking at cycle %i" % cycle)
 
     # ---------- processing and plotting ----------------
     fig, (ax1, ax2) = plt.subplots(2, 1)
-    capacity, voltage = cell.get_ccap(cycle)
+    capacity, voltage = cell.get_ccap(cycle, return_dataframe=False)
     ax1.plot(capacity, voltage, "b.-", label="raw")
     converter = Converter()
     converter.set_data(capacity, voltage)
     converter.inspect_data()
     converter.pre_process_data()
     ax1.plot(
         converter.capacity_preprocessed,
```

### Comparing `cellpy-1.0.0a3/cellpy/utils/ocv_rlx.py` & `cellpy-1.0.0a4/cellpy/utils/ocv_rlx.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/plotutils.py` & `cellpy-1.0.0a4/cellpy/utils/plotutils.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy/utils/processor.py` & `cellpy-1.0.0a4/cellpy/utils/processor.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/cellpy.egg-info/PKG-INFO` & `cellpy-1.0.0a4/cellpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpy
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Extract and manipulate data from battery data testers.
 Home-page: https://github.com/jepegit/cellpy
 Author: Jan Petter Maehlen
 Author-email: jepe@ife.no
 License: MIT license
 Keywords: cellpy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cellpy-1.0.0a3/cellpy.egg-info/SOURCES.txt` & `cellpy-1.0.0a4/cellpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/Makefile` & `cellpy-1.0.0a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png` & `cellpy-1.0.0a4/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png` & `cellpy-1.0.0a4/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png` & `cellpy-1.0.0a4/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png` & `cellpy-1.0.0a4/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png` & `cellpy-1.0.0a4/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png` & `cellpy-1.0.0a4/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png` & `cellpy-1.0.0a4/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png` & `cellpy-1.0.0a4/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png` & `cellpy-1.0.0a4/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png` & `cellpy-1.0.0a4/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png` & `cellpy-1.0.0a4/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png` & `cellpy-1.0.0a4/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png` & `cellpy-1.0.0a4/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png` & `cellpy-1.0.0a4/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png` & `cellpy-1.0.0a4/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png` & `cellpy-1.0.0a4/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png` & `cellpy-1.0.0a4/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png` & `cellpy-1.0.0a4/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/_images/templates_jupyterlab_001.png` & `cellpy-1.0.0a4/docs/_build/_images/templates_jupyterlab_001.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/_images/tutorials_utils_plotting_fig1.png` & `cellpy-1.0.0a4/docs/_build/_images/tutorials_utils_plotting_fig1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/_build/_images/tutorials_utils_plotting_fig2.png` & `cellpy-1.0.0a4/docs/_build/_images/tutorials_utils_plotting_fig2.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/adapted_readme.rst` & `cellpy-1.0.0a4/docs/adapted_readme.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/conf.py` & `cellpy-1.0.0a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/developers_guide/dev_cellpy_data_structure.rst` & `cellpy-1.0.0a4/docs/developers_guide/dev_cellpy_data_structure.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/developers_guide/dev_cellpy_folder_structure.rst` & `cellpy-1.0.0a4/docs/developers_guide/dev_cellpy_folder_structure.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/developers_guide/dev_cellpy_packaging_pypi.rst` & `cellpy-1.0.0a4/docs/developers_guide/dev_cellpy_packaging_pypi.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/developers_guide/dev_cellpy_setup.rst` & `cellpy-1.0.0a4/docs/developers_guide/dev_cellpy_setup.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/developers_guide/dev_conda_package.rst` & `cellpy-1.0.0a4/docs/developers_guide/dev_conda_package.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/developers_guide/dev_docs.rst` & `cellpy-1.0.0a4/docs/developers_guide/dev_docs.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/developers_guide/dev_loaders_and_instruments.rst` & `cellpy-1.0.0a4/docs/developers_guide/dev_loaders_and_instruments.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/developers_guide/dev_various.rst` & `cellpy-1.0.0a4/docs/developers_guide/dev_various.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst` & `cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst` & `cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst` & `cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst` & `cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/05_configuring.rst` & `cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/05_configuring.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/06_pandas.rst` & `cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/06_pandas.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst` & `cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst` & `cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png` & `cellpy-1.0.0a4/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png` & `cellpy-1.0.0a4/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/examples_and_tutorials/tips_and_tricks.rst` & `cellpy-1.0.0a4/docs/examples_and_tutorials/tips_and_tricks.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/examples_and_tutorials/utils/batch.rst` & `cellpy-1.0.0a4/docs/examples_and_tutorials/utils/batch.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png` & `cellpy-1.0.0a4/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png` & `cellpy-1.0.0a4/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/examples_and_tutorials/utils/ica.rst` & `cellpy-1.0.0a4/docs/examples_and_tutorials/utils/ica.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/examples_and_tutorials/utils/plotting.rst` & `cellpy-1.0.0a4/docs/examples_and_tutorials/utils/plotting.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst` & `cellpy-1.0.0a4/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/figures/cellpy-icon-bw.png` & `cellpy-1.0.0a4/docs/figures/cellpy-icon-bw.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/figures/cellpy-logo-v1.png` & `cellpy-1.0.0a4/docs/figures/cellpy-logo-v1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/index.rst` & `cellpy-1.0.0a4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/main_description/formats.rst` & `cellpy-1.0.0a4/docs/main_description/formats.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/main_description/installation.rst` & `cellpy-1.0.0a4/docs/main_description/installation.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/main_description/usage.rst` & `cellpy-1.0.0a4/docs/main_description/usage.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/make.bat` & `cellpy-1.0.0a4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/source/cellpy.parameters.rst` & `cellpy-1.0.0a4/docs/source/cellpy.parameters.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/source/cellpy.readers.instruments.configurations.rst` & `cellpy-1.0.0a4/docs/source/cellpy.readers.instruments.configurations.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/source/cellpy.readers.instruments.loader_specific_modules.rst` & `cellpy-1.0.0a4/docs/source/cellpy.readers.instruments.loader_specific_modules.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/source/cellpy.readers.instruments.processors.rst` & `cellpy-1.0.0a4/docs/source/cellpy.readers.instruments.processors.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/source/cellpy.readers.instruments.rst` & `cellpy-1.0.0a4/docs/source/cellpy.readers.instruments.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/source/cellpy.readers.rst` & `cellpy-1.0.0a4/docs/source/cellpy.readers.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/source/cellpy.rst` & `cellpy-1.0.0a4/docs/source/cellpy.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/source/cellpy.utils.batch_tools.rst` & `cellpy-1.0.0a4/docs/source/cellpy.utils.batch_tools.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/docs/source/cellpy.utils.rst` & `cellpy-1.0.0a4/docs/source/cellpy.utils.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a3/setup.py` & `cellpy-1.0.0a4/setup.py`

 * *Files identical despite different names*

