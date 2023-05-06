# Comparing `tmp/cellpy-1.0.0a4.tar.gz` & `tmp/cellpy-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellpy-1.0.0a4.tar", last modified: Sat May  6 22:11:53 2023, max compression
+gzip compressed data, was "cellpy-1.0.0a5.tar", last modified: Sat May  6 22:21:01 2023, max compression
```

## Comparing `cellpy-1.0.0a4.tar` & `cellpy-1.0.0a5.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.202692 cellpy-1.0.0a4/
--rw-rw-rw-   0        0        0      503 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/AUTHORS.rst
--rw-rw-rw-   0        0        0     3086 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     3908 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/HISTORY.rst
--rw-rw-rw-   0        0        0     1089 2021-12-21 09:11:58.000000 cellpy-1.0.0a4/LICENSE
--rw-rw-rw-   0        0        0      645 2022-05-27 12:07:50.000000 cellpy-1.0.0a4/MANIFEST.in
--rw-rw-rw-   0        0        0     6518 2023-05-06 22:11:53.201691 cellpy-1.0.0a4/PKG-INFO
--rw-rw-rw-   0        0        0     1872 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.903094 cellpy-1.0.0a4/cellpy/
--rw-rw-rw-   0        0        0      805 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/__init__.py
--rw-rw-rw-   0        0        0       25 2023-05-06 22:11:31.000000 cellpy-1.0.0a4/cellpy/_version.py
--rw-rw-rw-   0        0        0    53597 2023-05-06 21:51:58.000000 cellpy-1.0.0a4/cellpy/cli.py
--rw-rw-rw-   0        0        0     1228 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.916098 cellpy-1.0.0a4/cellpy/internals/
--rw-rw-rw-   0        0        0        0 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/internals/__init__.py
--rw-rw-rw-   0        0        0    27994 2023-05-06 21:51:58.000000 cellpy-1.0.0a4/cellpy/internals/core.py
--rw-rw-rw-   0        0        0     4838 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/log.py
--rw-rw-rw-   0        0        0     1750 2021-12-21 09:11:58.000000 cellpy-1.0.0a4/cellpy/logging.json
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.924095 cellpy-1.0.0a4/cellpy/parameters/
--rw-rw-rw-   0        0        0     3183 2023-05-02 11:51:31.000000 cellpy-1.0.0a4/cellpy/parameters/.cellpy_prms_default.conf
--rw-rw-rw-   0        0        0        2 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/parameters/__init__.py
--rw-rw-rw-   0        0        0    23784 2023-05-06 21:51:58.000000 cellpy-1.0.0a4/cellpy/parameters/internal_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.926095 cellpy-1.0.0a4/cellpy/parameters/legacy/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a4/cellpy/parameters/legacy/__init__.py
--rw-rw-rw-   0        0        0    24146 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/parameters/legacy/update_headers.py
--rw-rw-rw-   0        0        0    12142 2023-05-02 11:42:19.000000 cellpy-1.0.0a4/cellpy/parameters/prmreader.py
--rw-rw-rw-   0        0        0    12220 2023-05-02 11:49:22.000000 cellpy-1.0.0a4/cellpy/parameters/prms.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.936093 cellpy-1.0.0a4/cellpy/readers/
--rw-rw-rw-   0        0        0        2 2021-12-21 09:11:58.000000 cellpy-1.0.0a4/cellpy/readers/__init__.py
--rw-rw-rw-   0        0        0   233026 2023-05-06 21:51:58.000000 cellpy-1.0.0a4/cellpy/readers/cellreader.py
--rw-rw-rw-   0        0        0    39537 2023-05-06 21:51:58.000000 cellpy-1.0.0a4/cellpy/readers/core.py
--rw-rw-rw-   0        0        0    22998 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/dbreader.py
--rw-rw-rw-   0        0        0    13825 2023-05-06 21:51:58.000000 cellpy-1.0.0a4/cellpy/readers/filefinder.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.963094 cellpy-1.0.0a4/cellpy/readers/instruments/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a4/cellpy/readers/instruments/__init__.py
--rw-rw-rw-   0        0        0    50849 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/arbin_res.py
--rw-rw-rw-   0        0        0    19381 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql.py
--rw-rw-rw-   0        0        0    21062 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql_7.py
--rw-rw-rw-   0        0        0    11134 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql_csv.py
--rw-rw-rw-   0        0        0     7126 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql_h5.py
--rw-rw-rw-   0        0        0     9883 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql_xlsx.py
--rw-rw-rw-   0        0        0    27501 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/base.py
--rw-rw-rw-   0        0        0    22693 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/biologics_mpr.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.976095 cellpy-1.0.0a4/cellpy/readers/instruments/configurations/
--rw-rw-rw-   0        0        0     6607 2022-06-03 19:58:41.000000 cellpy-1.0.0a4/cellpy/readers/instruments/configurations/__init__.py
--rw-rw-rw-   0        0        0     1700 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_four.py
--rw-rw-rw-   0        0        0     4084 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_one.py
--rw-rw-rw-   0        0        0     1990 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_three.py
--rw-rw-rw-   0        0        0     1788 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_two.py
--rw-rw-rw-   0        0        0     3549 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_zero.py
--rw-rw-rw-   0        0        0     2132 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/configurations/neware_txt_zero.py
--rw-rw-rw-   0        0        0    10327 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/custom.py
--rw-rw-rw-   0        0        0     3760 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/ext_nda_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.979095 cellpy-1.0.0a4/cellpy/readers/instruments/loader_specific_modules/
--rw-rw-rw-   0        0        0        0 2022-06-03 19:58:41.000000 cellpy-1.0.0a4/cellpy/readers/instruments/loader_specific_modules/__init__.py
--rw-rw-rw-   0        0        0    22115 2022-06-03 19:58:41.000000 cellpy-1.0.0a4/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
--rw-rw-rw-   0        0        0     1067 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/local_instrument.py
--rw-rw-rw-   0        0        0    12886 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/maccor_txt.py
--rw-rw-rw-   0        0        0     3488 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/neware_txt.py
--rw-rw-rw-   0        0        0    16769 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/pec_csv.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.984093 cellpy-1.0.0a4/cellpy/readers/instruments/processors/
--rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-1.0.0a4/cellpy/readers/instruments/processors/__init__.py
--rw-rw-rw-   0        0        0    15265 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/processors/post_processors.py
--rw-rw-rw-   0        0        0     1450 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/instruments/processors/pre_processors.py
--rw-rw-rw-   0        0        0    26852 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/readers/sql_dbreader.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.006094 cellpy-1.0.0a4/cellpy/utils/
--rw-rw-rw-   0        0        0      192 2021-12-21 09:11:58.000000 cellpy-1.0.0a4/cellpy/utils/__init__.py
--rw-rw-rw-   0        0        0    48182 2023-05-03 09:31:40.000000 cellpy-1.0.0a4/cellpy/utils/batch.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.025619 cellpy-1.0.0a4/cellpy/utils/batch_tools/
--rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/__init__.py
--rw-rw-rw-   0        0        0     7578 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_analyzers.py
--rw-rw-rw-   0        0        0    19566 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_core.py
--rw-rw-rw-   0        0        0    41058 2023-05-06 21:51:58.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_experiments.py
--rw-rw-rw-   0        0        0     2931 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_exporters.py
--rw-rw-rw-   0        0        0    14090 2023-05-06 21:51:58.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_helpers.py
--rw-rw-rw-   0        0        0    27683 2023-05-02 13:39:36.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_journals.py
--rw-rw-rw-   0        0        0    29066 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_plotters.py
--rw-rw-rw-   0        0        0      245 2021-12-21 09:11:58.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_reporters.py
--rw-rw-rw-   0        0        0     3339 2022-05-27 12:03:59.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/dumpers.py
--rw-rw-rw-   0        0        0     9872 2023-05-02 10:20:24.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/engines.py
--rw-rw-rw-   0        0        0     5294 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/batch_tools/sqlite_from_excel_db.py
--rw-rw-rw-   0        0        0    63308 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/collectors.py
--rw-rw-rw-   0        0        0    45461 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/collectors_old.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.027174 cellpy-1.0.0a4/cellpy/utils/data/
--rw-rw-rw-   0        0        0  3700143 2023-05-06 21:47:28.000000 cellpy-1.0.0a4/cellpy/utils/data/20160805_test001_45_cc.h5
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.037175 cellpy-1.0.0a4/cellpy/utils/data/raw/
--rw-rw-rw-   0        0        0  1613824 2021-12-21 09:11:58.000000 cellpy-1.0.0a4/cellpy/utils/data/raw/20160805_test001_45_cc_01.res
--rw-rw-rw-   0        0        0      260 2022-05-27 12:07:50.000000 cellpy-1.0.0a4/cellpy/utils/diagnostics.py
--rw-rw-rw-   0        0        0    79016 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/easyplot.py
--rw-rw-rw-   0        0        0     1576 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/example_data.py
--rw-rw-rw-   0        0        0    39446 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/helpers.py
--rw-rw-rw-   0        0        0    38991 2023-05-06 21:51:58.000000 cellpy-1.0.0a4/cellpy/utils/ica.py
--rw-rw-rw-   0        0        0      189 2022-05-27 12:07:50.000000 cellpy-1.0.0a4/cellpy/utils/live.py
--rw-rw-rw-   0        0        0    24037 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/ocv_rlx.py
--rw-rw-rw-   0        0        0    45397 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/plotutils.py
--rw-rw-rw-   0        0        0     1787 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/cellpy/utils/processor.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.913095 cellpy-1.0.0a4/cellpy.egg-info/
--rw-rw-rw-   0        0        0     6518 2023-05-06 22:11:52.000000 cellpy-1.0.0a4/cellpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7846 2023-05-06 22:11:52.000000 cellpy-1.0.0a4/cellpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 22:11:52.000000 cellpy-1.0.0a4/cellpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 22:11:52.000000 cellpy-1.0.0a4/cellpy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 22:11:51.000000 cellpy-1.0.0a4/cellpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      337 2023-05-06 22:11:52.000000 cellpy-1.0.0a4/cellpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-06 22:11:52.000000 cellpy-1.0.0a4/cellpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.051174 cellpy-1.0.0a4/docs/
--rw-rw-rw-   0        0        0     6939 2022-09-20 08:21:07.000000 cellpy-1.0.0a4/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.880095 cellpy-1.0.0a4/docs/_build/
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.879096 cellpy-1.0.0a4/docs/_build/.doctrees/
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.057175 cellpy-1.0.0a4/docs/_build/.doctrees/nbsphinx/
--rw-rw-rw-   0        0        0    15014 2023-04-30 13:53:57.000000 cellpy-1.0.0a4/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
--rw-rw-rw-   0        0        0    14599 2023-04-30 13:53:57.000000 cellpy-1.0.0a4/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
--rw-rw-rw-   0        0        0    13527 2023-04-30 13:53:57.000000 cellpy-1.0.0a4/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
--rw-rw-rw-   0        0        0    25669 2023-04-30 13:54:02.000000 cellpy-1.0.0a4/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.090690 cellpy-1.0.0a4/docs/_build/_images/
--rw-rw-rw-   0        0        0    15014 2023-04-27 15:02:55.000000 cellpy-1.0.0a4/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
--rw-rw-rw-   0        0        0    14599 2023-04-27 15:02:55.000000 cellpy-1.0.0a4/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
--rw-rw-rw-   0        0        0    13527 2023-04-27 15:02:55.000000 cellpy-1.0.0a4/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
--rw-rw-rw-   0        0        0    25669 2023-04-27 15:03:02.000000 cellpy-1.0.0a4/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
--rw-rw-rw-   0        0        0    11678 2023-04-29 14:19:31.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png
--rw-rw-rw-   0        0        0    22040 2023-04-29 14:33:27.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png
--rw-rw-rw-   0        0        0    21790 2023-04-29 14:26:00.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png
--rw-rw-rw-   0        0        0    32991 2023-04-29 14:26:01.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png
--rw-rw-rw-   0        0        0    32991 2023-04-30 20:02:23.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png
--rw-rw-rw-   0        0        0     7231 2023-04-29 14:12:31.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png
--rw-rw-rw-   0        0        0    13360 2023-04-29 14:36:26.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png
--rw-rw-rw-   0        0        0    21790 2023-04-30 20:02:22.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png
--rw-rw-rw-   0        0        0     5391 2023-04-29 14:10:02.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png
--rw-rw-rw-   0        0        0    20826 2023-04-29 14:29:06.000000 cellpy-1.0.0a4/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png
--rw-rw-rw-   0        0        0    88743 2023-04-19 13:49:30.000000 cellpy-1.0.0a4/docs/_build/_images/templates_jupyterlab_001.png
--rw-rw-rw-   0        0        0   296908 2022-05-27 12:07:51.000000 cellpy-1.0.0a4/docs/_build/_images/tutorials_utils_plotting_fig1.png
--rw-rw-rw-   0        0        0    54588 2022-05-27 12:07:51.000000 cellpy-1.0.0a4/docs/_build/_images/tutorials_utils_plotting_fig2.png
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.094692 cellpy-1.0.0a4/docs/_build/_static/
--rw-rw-rw-   0        0        0      286 2023-04-25 11:20:36.000000 cellpy-1.0.0a4/docs/_build/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a4/docs/_build/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a4/docs/_build/_static/plus.png
--rw-rw-rw-   0        0        0     1695 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/adapted_readme.rst
--rw-rw-rw-   0        0        0    10731 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/conf.py
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.108692 cellpy-1.0.0a4/docs/developers_guide/
--rw-rw-rw-   0        0        0     1334 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/developers_guide/dev_cellpy_data_structure.rst
--rw-rw-rw-   0        0        0     5904 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/developers_guide/dev_cellpy_folder_structure.rst
--rw-rw-rw-   0        0        0      935 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/developers_guide/dev_cellpy_packaging_pypi.rst
--rw-rw-rw-   0        0        0     3009 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/developers_guide/dev_cellpy_setup.rst
--rw-rw-rw-   0        0        0     1821 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/developers_guide/dev_conda_package.rst
--rw-rw-rw-   0        0        0     2136 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/developers_guide/dev_docs.rst
--rw-rw-rw-   0        0        0     5218 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/developers_guide/dev_loaders_and_instruments.rst
--rw-rw-rw-   0        0        0     1768 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/developers_guide/dev_various.rst
--rw-rw-rw-   0        0        0      326 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/developers_guide/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.120691 cellpy-1.0.0a4/docs/examples_and_tutorials/
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.134693 cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/
--rw-rw-rw-   0        0        0    15786 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst
--rw-rw-rw-   0        0        0     3909 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst
--rw-rw-rw-   0        0        0     5485 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst
--rw-rw-rw-   0        0        0     4465 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst
--rw-rw-rw-   0        0        0     5908 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/05_configuring.rst
--rw-rw-rw-   0        0        0     1052 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/06_pandas.rst
--rw-rw-rw-   0        0        0     1102 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst
--rw-rw-rw-   0        0        0     8224 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst
--rw-rw-rw-   0        0        0      484 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/basics.rst
--rw-rw-rw-   0        0        0      366 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/examples.rst
--rw-rw-rw-   0        0        0      174 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.144700 cellpy-1.0.0a4/docs/examples_and_tutorials/loaders/
--rw-rw-rw-   0        0        0       49 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/loaders/01_arbin.rst
--rw-rw-rw-   0        0        0       52 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/loaders/02_maccor.rst
--rw-rw-rw-   0        0        0       43 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/loaders/03_PEC.rst
--rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/loaders/04_Neware.rst
--rw-rw-rw-   0        0        0       62 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/loaders/05_biologics.rst
--rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/loaders/06_custom.rst
--rw-rw-rw-   0        0        0      260 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/loaders.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:52.881095 cellpy-1.0.0a4/docs/examples_and_tutorials/notebooks/
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.148700 cellpy-1.0.0a4/docs/examples_and_tutorials/notebooks/images/
--rw-rw-rw-   0        0        0    88743 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png
--rw-rw-rw-   0        0        0    95663 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png
--rw-rw-rw-   0        0        0      231 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/notebooks.rst
--rw-rw-rw-   0        0        0     1797 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/tips_and_tricks.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.159689 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/
--rw-rw-rw-   0        0        0     4388 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/batch.rst
--rw-rw-rw-   0        0        0       59 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/collectors.rst
--rw-rw-rw-   0        0        0       53 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/easyplot.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.165691 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/figures/
--rw-rw-rw-   0        0        0   296908 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png
--rw-rw-rw-   0        0        0    54588 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png
--rw-rw-rw-   0        0        0     1219 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/ica.rst
--rw-rw-rw-   0        0        0     2063 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/plotting.rst
--rw-rw-rw-   0        0        0      338 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/templates.rst
--rw-rw-rw-   0        0        0     1379 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst
--rw-rw-rw-   0        0        0      371 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/examples_and_tutorials/utils.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.169691 cellpy-1.0.0a4/docs/figures/
--rw-rw-rw-   0        0        0     9981 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/figures/cellpy-icon-bw.png
--rw-rw-rw-   0        0        0    10302 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/figures/cellpy-logo-v1.png
--rw-rw-rw-   0        0        0      593 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.180692 cellpy-1.0.0a4/docs/main_description/
--rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/main_description/authors.rst
--rw-rw-rw-   0        0        0       37 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/main_description/contributing.rst
--rw-rw-rw-   0        0        0    16327 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/main_description/formats.rst
--rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/main_description/history.rst
--rw-rw-rw-   0        0        0      182 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/main_description/index.rst
--rw-rw-rw-   0        0        0     4288 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/main_description/installation.rst
--rw-rw-rw-   0        0        0     3444 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/main_description/usage.rst
--rwxrwxrwx   0        0        0     6701 2022-09-20 08:21:07.000000 cellpy-1.0.0a4/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-06 22:11:53.200692 cellpy-1.0.0a4/docs/source/
--rw-rw-rw-   0        0        0      367 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.internals.rst
--rw-rw-rw-   0        0        0      447 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.parameters.legacy.rst
--rw-rw-rw-   0        0        0      847 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.parameters.rst
--rw-rw-rw-   0        0        0     1911 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.readers.instruments.configurations.rst
--rw-rw-rw-   0        0        0      631 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.readers.instruments.loader_specific_modules.rst
--rw-rw-rw-   0        0        0      783 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.readers.instruments.processors.rst
--rw-rw-rw-   0        0        0     3413 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.readers.instruments.rst
--rw-rw-rw-   0        0        0     1139 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.readers.rst
--rw-rw-rw-   0        0        0      721 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.rst
--rw-rw-rw-   0        0        0     2610 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.utils.batch_tools.rst
--rw-rw-rw-   0        0        0     2222 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/docs/source/cellpy.utils.rst
--rw-rw-rw-   0        0        0       62 2023-05-01 10:14:23.000000 cellpy-1.0.0a4/docs/source/modules.rst
--rw-rw-rw-   0        0        0      281 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 22:11:53.202692 cellpy-1.0.0a4/setup.cfg
--rw-rw-rw-   0        0        0     2952 2023-05-01 18:24:45.000000 cellpy-1.0.0a4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.212099 cellpy-1.0.0a5/
+-rw-rw-rw-   0        0        0      503 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3086 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     3908 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/HISTORY.rst
+-rw-rw-rw-   0        0        0     1089 2021-12-21 09:11:58.000000 cellpy-1.0.0a5/LICENSE
+-rw-rw-rw-   0        0        0      645 2022-05-27 12:07:50.000000 cellpy-1.0.0a5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6518 2023-05-06 22:21:01.211098 cellpy-1.0.0a5/PKG-INFO
+-rw-rw-rw-   0        0        0     1872 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:00.972647 cellpy-1.0.0a5/cellpy/
+-rw-rw-rw-   0        0        0      805 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/__init__.py
+-rw-rw-rw-   0        0        0       25 2023-05-06 22:20:47.000000 cellpy-1.0.0a5/cellpy/_version.py
+-rw-rw-rw-   0        0        0    53597 2023-05-06 21:51:58.000000 cellpy-1.0.0a5/cellpy/cli.py
+-rw-rw-rw-   0        0        0     1228 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:00.987157 cellpy-1.0.0a5/cellpy/internals/
+-rw-rw-rw-   0        0        0        0 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/internals/__init__.py
+-rw-rw-rw-   0        0        0    27994 2023-05-06 21:51:58.000000 cellpy-1.0.0a5/cellpy/internals/core.py
+-rw-rw-rw-   0        0        0     4838 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/log.py
+-rw-rw-rw-   0        0        0     1750 2021-12-21 09:11:58.000000 cellpy-1.0.0a5/cellpy/logging.json
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:00.994744 cellpy-1.0.0a5/cellpy/parameters/
+-rw-rw-rw-   0        0        0     3183 2023-05-02 11:51:31.000000 cellpy-1.0.0a5/cellpy/parameters/.cellpy_prms_default.conf
+-rw-rw-rw-   0        0        0        2 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/parameters/__init__.py
+-rw-rw-rw-   0        0        0    23784 2023-05-06 21:51:58.000000 cellpy-1.0.0a5/cellpy/parameters/internal_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:00.997677 cellpy-1.0.0a5/cellpy/parameters/legacy/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a5/cellpy/parameters/legacy/__init__.py
+-rw-rw-rw-   0        0        0    24146 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/parameters/legacy/update_headers.py
+-rw-rw-rw-   0        0        0    12142 2023-05-02 11:42:19.000000 cellpy-1.0.0a5/cellpy/parameters/prmreader.py
+-rw-rw-rw-   0        0        0    12220 2023-05-02 11:49:22.000000 cellpy-1.0.0a5/cellpy/parameters/prms.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.005667 cellpy-1.0.0a5/cellpy/readers/
+-rw-rw-rw-   0        0        0        2 2021-12-21 09:11:58.000000 cellpy-1.0.0a5/cellpy/readers/__init__.py
+-rw-rw-rw-   0        0        0   233026 2023-05-06 21:51:58.000000 cellpy-1.0.0a5/cellpy/readers/cellreader.py
+-rw-rw-rw-   0        0        0    39537 2023-05-06 21:51:58.000000 cellpy-1.0.0a5/cellpy/readers/core.py
+-rw-rw-rw-   0        0        0    22998 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/dbreader.py
+-rw-rw-rw-   0        0        0    13825 2023-05-06 21:51:58.000000 cellpy-1.0.0a5/cellpy/readers/filefinder.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.025668 cellpy-1.0.0a5/cellpy/readers/instruments/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a5/cellpy/readers/instruments/__init__.py
+-rw-rw-rw-   0        0        0    50849 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/arbin_res.py
+-rw-rw-rw-   0        0        0    19381 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/arbin_sql.py
+-rw-rw-rw-   0        0        0    21062 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/arbin_sql_7.py
+-rw-rw-rw-   0        0        0    11134 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/arbin_sql_csv.py
+-rw-rw-rw-   0        0        0     7126 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/arbin_sql_h5.py
+-rw-rw-rw-   0        0        0     9883 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/arbin_sql_xlsx.py
+-rw-rw-rw-   0        0        0    27501 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/base.py
+-rw-rw-rw-   0        0        0    22693 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/biologics_mpr.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.034675 cellpy-1.0.0a5/cellpy/readers/instruments/configurations/
+-rw-rw-rw-   0        0        0     6607 2022-06-03 19:58:41.000000 cellpy-1.0.0a5/cellpy/readers/instruments/configurations/__init__.py
+-rw-rw-rw-   0        0        0     1700 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/configurations/maccor_txt_four.py
+-rw-rw-rw-   0        0        0     4084 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/configurations/maccor_txt_one.py
+-rw-rw-rw-   0        0        0     1990 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/configurations/maccor_txt_three.py
+-rw-rw-rw-   0        0        0     1788 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/configurations/maccor_txt_two.py
+-rw-rw-rw-   0        0        0     3549 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/configurations/maccor_txt_zero.py
+-rw-rw-rw-   0        0        0     2132 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/configurations/neware_txt_zero.py
+-rw-rw-rw-   0        0        0    10327 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/custom.py
+-rw-rw-rw-   0        0        0     3760 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/ext_nda_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.036678 cellpy-1.0.0a5/cellpy/readers/instruments/loader_specific_modules/
+-rw-rw-rw-   0        0        0        0 2022-06-03 19:58:41.000000 cellpy-1.0.0a5/cellpy/readers/instruments/loader_specific_modules/__init__.py
+-rw-rw-rw-   0        0        0    22115 2022-06-03 19:58:41.000000 cellpy-1.0.0a5/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py
+-rw-rw-rw-   0        0        0     1067 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/local_instrument.py
+-rw-rw-rw-   0        0        0    12886 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/maccor_txt.py
+-rw-rw-rw-   0        0        0     3488 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/neware_txt.py
+-rw-rw-rw-   0        0        0    16769 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/pec_csv.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.041363 cellpy-1.0.0a5/cellpy/readers/instruments/processors/
+-rw-rw-rw-   0        0        0        0 2022-05-27 12:07:50.000000 cellpy-1.0.0a5/cellpy/readers/instruments/processors/__init__.py
+-rw-rw-rw-   0        0        0    15265 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/processors/post_processors.py
+-rw-rw-rw-   0        0        0     1450 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/instruments/processors/pre_processors.py
+-rw-rw-rw-   0        0        0    26852 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/readers/sql_dbreader.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.059832 cellpy-1.0.0a5/cellpy/utils/
+-rw-rw-rw-   0        0        0      192 2021-12-21 09:11:58.000000 cellpy-1.0.0a5/cellpy/utils/__init__.py
+-rw-rw-rw-   0        0        0    48182 2023-05-03 09:31:40.000000 cellpy-1.0.0a5/cellpy/utils/batch.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.075831 cellpy-1.0.0a5/cellpy/utils/batch_tools/
+-rw-rw-rw-   0        0        0        0 2021-12-21 09:11:58.000000 cellpy-1.0.0a5/cellpy/utils/batch_tools/__init__.py
+-rw-rw-rw-   0        0        0     7578 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/utils/batch_tools/batch_analyzers.py
+-rw-rw-rw-   0        0        0    19566 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/utils/batch_tools/batch_core.py
+-rw-rw-rw-   0        0        0    41058 2023-05-06 21:51:58.000000 cellpy-1.0.0a5/cellpy/utils/batch_tools/batch_experiments.py
+-rw-rw-rw-   0        0        0     2931 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/utils/batch_tools/batch_exporters.py
+-rw-rw-rw-   0        0        0    14090 2023-05-06 21:51:58.000000 cellpy-1.0.0a5/cellpy/utils/batch_tools/batch_helpers.py
+-rw-rw-rw-   0        0        0    27683 2023-05-02 13:39:36.000000 cellpy-1.0.0a5/cellpy/utils/batch_tools/batch_journals.py
+-rw-rw-rw-   0        0        0    29066 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/utils/batch_tools/batch_plotters.py
+-rw-rw-rw-   0        0        0      245 2021-12-21 09:11:58.000000 cellpy-1.0.0a5/cellpy/utils/batch_tools/batch_reporters.py
+-rw-rw-rw-   0        0        0     3339 2022-05-27 12:03:59.000000 cellpy-1.0.0a5/cellpy/utils/batch_tools/dumpers.py
+-rw-rw-rw-   0        0        0     9872 2023-05-02 10:20:24.000000 cellpy-1.0.0a5/cellpy/utils/batch_tools/engines.py
+-rw-rw-rw-   0        0        0     5294 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/utils/batch_tools/sqlite_from_excel_db.py
+-rw-rw-rw-   0        0        0    63308 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/utils/collectors.py
+-rw-rw-rw-   0        0        0    45461 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/utils/collectors_old.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.076831 cellpy-1.0.0a5/cellpy/utils/data/
+-rw-rw-rw-   0        0        0  3700143 2023-05-06 21:47:28.000000 cellpy-1.0.0a5/cellpy/utils/data/20160805_test001_45_cc.h5
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.081349 cellpy-1.0.0a5/cellpy/utils/data/raw/
+-rw-rw-rw-   0        0        0  1613824 2021-12-21 09:11:58.000000 cellpy-1.0.0a5/cellpy/utils/data/raw/20160805_test001_45_cc_01.res
+-rw-rw-rw-   0        0        0      260 2022-05-27 12:07:50.000000 cellpy-1.0.0a5/cellpy/utils/diagnostics.py
+-rw-rw-rw-   0        0        0    79016 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/utils/easyplot.py
+-rw-rw-rw-   0        0        0     1576 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/utils/example_data.py
+-rw-rw-rw-   0        0        0    39446 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/utils/helpers.py
+-rw-rw-rw-   0        0        0    38991 2023-05-06 21:51:58.000000 cellpy-1.0.0a5/cellpy/utils/ica.py
+-rw-rw-rw-   0        0        0      189 2022-05-27 12:07:50.000000 cellpy-1.0.0a5/cellpy/utils/live.py
+-rw-rw-rw-   0        0        0    24037 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/utils/ocv_rlx.py
+-rw-rw-rw-   0        0        0    45397 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/utils/plotutils.py
+-rw-rw-rw-   0        0        0     1787 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/cellpy/utils/processor.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:00.985156 cellpy-1.0.0a5/cellpy.egg-info/
+-rw-rw-rw-   0        0        0     6518 2023-05-06 22:21:00.000000 cellpy-1.0.0a5/cellpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7846 2023-05-06 22:21:00.000000 cellpy-1.0.0a5/cellpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 22:21:00.000000 cellpy-1.0.0a5/cellpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 22:21:00.000000 cellpy-1.0.0a5/cellpy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 22:20:59.000000 cellpy-1.0.0a5/cellpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      337 2023-05-06 22:21:00.000000 cellpy-1.0.0a5/cellpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-06 22:21:00.000000 cellpy-1.0.0a5/cellpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.089348 cellpy-1.0.0a5/docs/
+-rw-rw-rw-   0        0        0     6939 2022-09-20 08:21:07.000000 cellpy-1.0.0a5/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:00.952534 cellpy-1.0.0a5/docs/_build/
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:00.951534 cellpy-1.0.0a5/docs/_build/.doctrees/
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.094339 cellpy-1.0.0a5/docs/_build/.doctrees/nbsphinx/
+-rw-rw-rw-   0        0        0    15014 2023-04-30 13:53:57.000000 cellpy-1.0.0a5/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
+-rw-rw-rw-   0        0        0    14599 2023-04-30 13:53:57.000000 cellpy-1.0.0a5/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
+-rw-rw-rw-   0        0        0    13527 2023-04-30 13:53:57.000000 cellpy-1.0.0a5/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
+-rw-rw-rw-   0        0        0    25669 2023-04-30 13:54:02.000000 cellpy-1.0.0a5/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.118854 cellpy-1.0.0a5/docs/_build/_images/
+-rw-rw-rw-   0        0        0    15014 2023-04-27 15:02:55.000000 cellpy-1.0.0a5/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png
+-rw-rw-rw-   0        0        0    14599 2023-04-27 15:02:55.000000 cellpy-1.0.0a5/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png
+-rw-rw-rw-   0        0        0    13527 2023-04-27 15:02:55.000000 cellpy-1.0.0a5/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png
+-rw-rw-rw-   0        0        0    25669 2023-04-27 15:03:02.000000 cellpy-1.0.0a5/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png
+-rw-rw-rw-   0        0        0    11678 2023-04-29 14:19:31.000000 cellpy-1.0.0a5/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png
+-rw-rw-rw-   0        0        0    22040 2023-04-29 14:33:27.000000 cellpy-1.0.0a5/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png
+-rw-rw-rw-   0        0        0    21790 2023-04-29 14:26:00.000000 cellpy-1.0.0a5/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png
+-rw-rw-rw-   0        0        0    32991 2023-04-29 14:26:01.000000 cellpy-1.0.0a5/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png
+-rw-rw-rw-   0        0        0    32991 2023-04-30 20:02:23.000000 cellpy-1.0.0a5/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png
+-rw-rw-rw-   0        0        0     7231 2023-04-29 14:12:31.000000 cellpy-1.0.0a5/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png
+-rw-rw-rw-   0        0        0    13360 2023-04-29 14:36:26.000000 cellpy-1.0.0a5/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png
+-rw-rw-rw-   0        0        0    21790 2023-04-30 20:02:22.000000 cellpy-1.0.0a5/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png
+-rw-rw-rw-   0        0        0     5391 2023-04-29 14:10:02.000000 cellpy-1.0.0a5/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png
+-rw-rw-rw-   0        0        0    20826 2023-04-29 14:29:06.000000 cellpy-1.0.0a5/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png
+-rw-rw-rw-   0        0        0    88743 2023-04-19 13:49:30.000000 cellpy-1.0.0a5/docs/_build/_images/templates_jupyterlab_001.png
+-rw-rw-rw-   0        0        0   296908 2022-05-27 12:07:51.000000 cellpy-1.0.0a5/docs/_build/_images/tutorials_utils_plotting_fig1.png
+-rw-rw-rw-   0        0        0    54588 2022-05-27 12:07:51.000000 cellpy-1.0.0a5/docs/_build/_images/tutorials_utils_plotting_fig2.png
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.121854 cellpy-1.0.0a5/docs/_build/_static/
+-rw-rw-rw-   0        0        0      286 2023-04-25 11:20:36.000000 cellpy-1.0.0a5/docs/_build/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a5/docs/_build/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-25 11:20:36.000000 cellpy-1.0.0a5/docs/_build/_static/plus.png
+-rw-rw-rw-   0        0        0     1695 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/adapted_readme.rst
+-rw-rw-rw-   0        0        0    10731 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/conf.py
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.134368 cellpy-1.0.0a5/docs/developers_guide/
+-rw-rw-rw-   0        0        0     1334 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/developers_guide/dev_cellpy_data_structure.rst
+-rw-rw-rw-   0        0        0     5904 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/developers_guide/dev_cellpy_folder_structure.rst
+-rw-rw-rw-   0        0        0      935 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/developers_guide/dev_cellpy_packaging_pypi.rst
+-rw-rw-rw-   0        0        0     3009 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/developers_guide/dev_cellpy_setup.rst
+-rw-rw-rw-   0        0        0     1821 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/developers_guide/dev_conda_package.rst
+-rw-rw-rw-   0        0        0     2136 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/developers_guide/dev_docs.rst
+-rw-rw-rw-   0        0        0     5218 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/developers_guide/dev_loaders_and_instruments.rst
+-rw-rw-rw-   0        0        0     1768 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/developers_guide/dev_various.rst
+-rw-rw-rw-   0        0        0      326 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/developers_guide/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.145367 cellpy-1.0.0a5/docs/examples_and_tutorials/
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.157366 cellpy-1.0.0a5/docs/examples_and_tutorials/basic_interactions/
+-rw-rw-rw-   0        0        0    15786 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst
+-rw-rw-rw-   0        0        0     3909 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst
+-rw-rw-rw-   0        0        0     5485 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst
+-rw-rw-rw-   0        0        0     4465 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst
+-rw-rw-rw-   0        0        0     5908 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/basic_interactions/05_configuring.rst
+-rw-rw-rw-   0        0        0     1052 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/basic_interactions/06_pandas.rst
+-rw-rw-rw-   0        0        0     1102 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst
+-rw-rw-rw-   0        0        0     8224 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst
+-rw-rw-rw-   0        0        0      484 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/basics.rst
+-rw-rw-rw-   0        0        0      366 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/examples.rst
+-rw-rw-rw-   0        0        0      174 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.165367 cellpy-1.0.0a5/docs/examples_and_tutorials/loaders/
+-rw-rw-rw-   0        0        0       49 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/loaders/01_arbin.rst
+-rw-rw-rw-   0        0        0       52 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/loaders/02_maccor.rst
+-rw-rw-rw-   0        0        0       43 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/loaders/03_PEC.rst
+-rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/loaders/04_Neware.rst
+-rw-rw-rw-   0        0        0       62 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/loaders/05_biologics.rst
+-rw-rw-rw-   0        0        0       54 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/loaders/06_custom.rst
+-rw-rw-rw-   0        0        0      260 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/loaders.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:00.954534 cellpy-1.0.0a5/docs/examples_and_tutorials/notebooks/
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.168367 cellpy-1.0.0a5/docs/examples_and_tutorials/notebooks/images/
+-rw-rw-rw-   0        0        0    88743 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png
+-rw-rw-rw-   0        0        0    95663 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png
+-rw-rw-rw-   0        0        0      231 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/notebooks.rst
+-rw-rw-rw-   0        0        0     1797 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/tips_and_tricks.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.177883 cellpy-1.0.0a5/docs/examples_and_tutorials/utils/
+-rw-rw-rw-   0        0        0     4388 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/utils/batch.rst
+-rw-rw-rw-   0        0        0       59 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/utils/collectors.rst
+-rw-rw-rw-   0        0        0       53 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/utils/easyplot.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.180884 cellpy-1.0.0a5/docs/examples_and_tutorials/utils/figures/
+-rw-rw-rw-   0        0        0   296908 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png
+-rw-rw-rw-   0        0        0    54588 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png
+-rw-rw-rw-   0        0        0     1219 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/utils/ica.rst
+-rw-rw-rw-   0        0        0     2063 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/utils/plotting.rst
+-rw-rw-rw-   0        0        0      338 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/utils/templates.rst
+-rw-rw-rw-   0        0        0     1379 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst
+-rw-rw-rw-   0        0        0      371 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/examples_and_tutorials/utils.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.182882 cellpy-1.0.0a5/docs/figures/
+-rw-rw-rw-   0        0        0     9981 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/figures/cellpy-icon-bw.png
+-rw-rw-rw-   0        0        0    10302 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/figures/cellpy-logo-v1.png
+-rw-rw-rw-   0        0        0      593 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/index.rst
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.192883 cellpy-1.0.0a5/docs/main_description/
+-rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/main_description/authors.rst
+-rw-rw-rw-   0        0        0       37 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/main_description/contributing.rst
+-rw-rw-rw-   0        0        0    16327 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/main_description/formats.rst
+-rw-rw-rw-   0        0        0       32 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/main_description/history.rst
+-rw-rw-rw-   0        0        0      182 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/main_description/index.rst
+-rw-rw-rw-   0        0        0     4288 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/main_description/installation.rst
+-rw-rw-rw-   0        0        0     3444 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/main_description/usage.rst
+-rwxrwxrwx   0        0        0     6701 2022-09-20 08:21:07.000000 cellpy-1.0.0a5/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-06 22:21:01.209098 cellpy-1.0.0a5/docs/source/
+-rw-rw-rw-   0        0        0      367 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/source/cellpy.internals.rst
+-rw-rw-rw-   0        0        0      447 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/source/cellpy.parameters.legacy.rst
+-rw-rw-rw-   0        0        0      847 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/source/cellpy.parameters.rst
+-rw-rw-rw-   0        0        0     1911 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/source/cellpy.readers.instruments.configurations.rst
+-rw-rw-rw-   0        0        0      631 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/source/cellpy.readers.instruments.loader_specific_modules.rst
+-rw-rw-rw-   0        0        0      783 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/source/cellpy.readers.instruments.processors.rst
+-rw-rw-rw-   0        0        0     3413 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/source/cellpy.readers.instruments.rst
+-rw-rw-rw-   0        0        0     1139 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/source/cellpy.readers.rst
+-rw-rw-rw-   0        0        0      721 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/source/cellpy.rst
+-rw-rw-rw-   0        0        0     2610 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/source/cellpy.utils.batch_tools.rst
+-rw-rw-rw-   0        0        0     2222 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/docs/source/cellpy.utils.rst
+-rw-rw-rw-   0        0        0       62 2023-05-01 10:14:23.000000 cellpy-1.0.0a5/docs/source/modules.rst
+-rw-rw-rw-   0        0        0      281 2023-05-01 18:24:45.000000 cellpy-1.0.0a5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 22:21:01.212099 cellpy-1.0.0a5/setup.cfg
+-rw-rw-rw-   0        0        0     2929 2023-05-06 22:19:45.000000 cellpy-1.0.0a5/setup.py
```

### Comparing `cellpy-1.0.0a4/CONTRIBUTING.rst` & `cellpy-1.0.0a5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/HISTORY.rst` & `cellpy-1.0.0a5/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/LICENSE` & `cellpy-1.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/MANIFEST.in` & `cellpy-1.0.0a5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/PKG-INFO` & `cellpy-1.0.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpy
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: Extract and manipulate data from battery data testers.
 Home-page: https://github.com/jepegit/cellpy
 Author: Jan Petter Maehlen
 Author-email: jepe@ife.no
 License: MIT license
 Keywords: cellpy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cellpy-1.0.0a4/README.rst` & `cellpy-1.0.0a5/README.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/__init__.py` & `cellpy-1.0.0a5/cellpy/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/cli.py` & `cellpy-1.0.0a5/cellpy/cli.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/exceptions.py` & `cellpy-1.0.0a5/cellpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/internals/core.py` & `cellpy-1.0.0a5/cellpy/internals/core.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/log.py` & `cellpy-1.0.0a5/cellpy/log.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/logging.json` & `cellpy-1.0.0a5/cellpy/logging.json`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/parameters/.cellpy_prms_default.conf` & `cellpy-1.0.0a5/cellpy/parameters/.cellpy_prms_default.conf`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/parameters/internal_settings.py` & `cellpy-1.0.0a5/cellpy/parameters/internal_settings.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/parameters/legacy/update_headers.py` & `cellpy-1.0.0a5/cellpy/parameters/legacy/update_headers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/parameters/prmreader.py` & `cellpy-1.0.0a5/cellpy/parameters/prmreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/parameters/prms.py` & `cellpy-1.0.0a5/cellpy/parameters/prms.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/cellreader.py` & `cellpy-1.0.0a5/cellpy/readers/cellreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/core.py` & `cellpy-1.0.0a5/cellpy/readers/core.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/dbreader.py` & `cellpy-1.0.0a5/cellpy/readers/dbreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/filefinder.py` & `cellpy-1.0.0a5/cellpy/readers/filefinder.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/arbin_res.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/arbin_res.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/arbin_sql.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql_7.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/arbin_sql_7.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql_csv.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/arbin_sql_csv.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql_h5.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/arbin_sql_h5.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/arbin_sql_xlsx.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/arbin_sql_xlsx.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/base.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/base.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/biologics_mpr.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/biologics_mpr.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/configurations/__init__.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_four.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/configurations/maccor_txt_four.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_one.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/configurations/maccor_txt_one.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_three.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/configurations/maccor_txt_three.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_two.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/configurations/maccor_txt_two.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/configurations/maccor_txt_zero.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/configurations/maccor_txt_zero.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/configurations/neware_txt_zero.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/configurations/neware_txt_zero.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/custom.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/custom.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/ext_nda_reader.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/ext_nda_reader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/loader_specific_modules/biologic_file_format.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/local_instrument.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/local_instrument.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/maccor_txt.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/maccor_txt.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/neware_txt.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/neware_txt.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/pec_csv.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/pec_csv.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/processors/post_processors.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/processors/post_processors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/instruments/processors/pre_processors.py` & `cellpy-1.0.0a5/cellpy/readers/instruments/processors/pre_processors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/readers/sql_dbreader.py` & `cellpy-1.0.0a5/cellpy/readers/sql_dbreader.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/batch.py` & `cellpy-1.0.0a5/cellpy/utils/batch.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_analyzers.py` & `cellpy-1.0.0a5/cellpy/utils/batch_tools/batch_analyzers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_core.py` & `cellpy-1.0.0a5/cellpy/utils/batch_tools/batch_core.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_experiments.py` & `cellpy-1.0.0a5/cellpy/utils/batch_tools/batch_experiments.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_exporters.py` & `cellpy-1.0.0a5/cellpy/utils/batch_tools/batch_exporters.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_helpers.py` & `cellpy-1.0.0a5/cellpy/utils/batch_tools/batch_helpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_journals.py` & `cellpy-1.0.0a5/cellpy/utils/batch_tools/batch_journals.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/batch_tools/batch_plotters.py` & `cellpy-1.0.0a5/cellpy/utils/batch_tools/batch_plotters.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/batch_tools/dumpers.py` & `cellpy-1.0.0a5/cellpy/utils/batch_tools/dumpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/batch_tools/engines.py` & `cellpy-1.0.0a5/cellpy/utils/batch_tools/engines.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/batch_tools/sqlite_from_excel_db.py` & `cellpy-1.0.0a5/cellpy/utils/batch_tools/sqlite_from_excel_db.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/collectors.py` & `cellpy-1.0.0a5/cellpy/utils/collectors.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/collectors_old.py` & `cellpy-1.0.0a5/cellpy/utils/collectors_old.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/data/20160805_test001_45_cc.h5` & `cellpy-1.0.0a5/cellpy/utils/data/20160805_test001_45_cc.h5`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/data/raw/20160805_test001_45_cc_01.res` & `cellpy-1.0.0a5/cellpy/utils/data/raw/20160805_test001_45_cc_01.res`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/easyplot.py` & `cellpy-1.0.0a5/cellpy/utils/easyplot.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/example_data.py` & `cellpy-1.0.0a5/cellpy/utils/example_data.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/helpers.py` & `cellpy-1.0.0a5/cellpy/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/ica.py` & `cellpy-1.0.0a5/cellpy/utils/ica.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/ocv_rlx.py` & `cellpy-1.0.0a5/cellpy/utils/ocv_rlx.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/plotutils.py` & `cellpy-1.0.0a5/cellpy/utils/plotutils.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy/utils/processor.py` & `cellpy-1.0.0a5/cellpy/utils/processor.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/cellpy.egg-info/PKG-INFO` & `cellpy-1.0.0a5/cellpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellpy
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: Extract and manipulate data from battery data testers.
 Home-page: https://github.com/jepegit/cellpy
 Author: Jan Petter Maehlen
 Author-email: jepe@ife.no
 License: MIT license
 Keywords: cellpy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cellpy-1.0.0a4/cellpy.egg-info/SOURCES.txt` & `cellpy-1.0.0a5/cellpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/Makefile` & `cellpy-1.0.0a5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png` & `cellpy-1.0.0a5/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png` & `cellpy-1.0.0a5/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png` & `cellpy-1.0.0a5/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png` & `cellpy-1.0.0a5/docs/_build/.doctrees/nbsphinx/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png` & `cellpy-1.0.0a5/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_6_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png` & `cellpy-1.0.0a5/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_7_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png` & `cellpy-1.0.0a5/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_get_cap_8_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png` & `cellpy-1.0.0a5/docs/_build/_images/examples_and_tutorials_notebooks_tutorial_simple_plot_2_0.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png` & `cellpy-1.0.0a5/docs/_build/_images/graphviz-22185705e237fa530df24e4af50cb25833165e25.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png` & `cellpy-1.0.0a5/docs/_build/_images/graphviz-246f2486cd940f2ea40a07f847c86c22b2607ca8.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png` & `cellpy-1.0.0a5/docs/_build/_images/graphviz-42e9bc826d476a3d361a7f410e989ed34dc1aa85.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png` & `cellpy-1.0.0a5/docs/_build/_images/graphviz-619216a42370fd49669c083549129b8470c8fae1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png` & `cellpy-1.0.0a5/docs/_build/_images/graphviz-6412a7c74952b4793798e9032f5bc4e7a1ab70c1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png` & `cellpy-1.0.0a5/docs/_build/_images/graphviz-6deb64a460668e8ef9bf0ca653314119adeeae66.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png` & `cellpy-1.0.0a5/docs/_build/_images/graphviz-83b62e03ef369ff0a30f027892dba95b91ea8b6c.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png` & `cellpy-1.0.0a5/docs/_build/_images/graphviz-8ec82d564b1a6ea5b95a36a4a213f7a78aaedc63.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png` & `cellpy-1.0.0a5/docs/_build/_images/graphviz-ce8a9fe2ba01194aed847e0248d749db4093aca1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png` & `cellpy-1.0.0a5/docs/_build/_images/graphviz-e94a5352318e02fcc5ef1f813e02a526c39af791.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/_images/templates_jupyterlab_001.png` & `cellpy-1.0.0a5/docs/_build/_images/templates_jupyterlab_001.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/_images/tutorials_utils_plotting_fig1.png` & `cellpy-1.0.0a5/docs/_build/_images/tutorials_utils_plotting_fig1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/_build/_images/tutorials_utils_plotting_fig2.png` & `cellpy-1.0.0a5/docs/_build/_images/tutorials_utils_plotting_fig2.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/adapted_readme.rst` & `cellpy-1.0.0a5/docs/adapted_readme.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/conf.py` & `cellpy-1.0.0a5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/developers_guide/dev_cellpy_data_structure.rst` & `cellpy-1.0.0a5/docs/developers_guide/dev_cellpy_data_structure.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/developers_guide/dev_cellpy_folder_structure.rst` & `cellpy-1.0.0a5/docs/developers_guide/dev_cellpy_folder_structure.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/developers_guide/dev_cellpy_packaging_pypi.rst` & `cellpy-1.0.0a5/docs/developers_guide/dev_cellpy_packaging_pypi.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/developers_guide/dev_cellpy_setup.rst` & `cellpy-1.0.0a5/docs/developers_guide/dev_cellpy_setup.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/developers_guide/dev_conda_package.rst` & `cellpy-1.0.0a5/docs/developers_guide/dev_conda_package.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/developers_guide/dev_docs.rst` & `cellpy-1.0.0a5/docs/developers_guide/dev_docs.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/developers_guide/dev_loaders_and_instruments.rst` & `cellpy-1.0.0a5/docs/developers_guide/dev_loaders_and_instruments.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/developers_guide/dev_various.rst` & `cellpy-1.0.0a5/docs/developers_guide/dev_various.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst` & `cellpy-1.0.0a5/docs/examples_and_tutorials/basic_interactions/01_getting_started_tutorial.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst` & `cellpy-1.0.0a5/docs/examples_and_tutorials/basic_interactions/02_read_cell_data.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst` & `cellpy-1.0.0a5/docs/examples_and_tutorials/basic_interactions/03_more_about_get.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst` & `cellpy-1.0.0a5/docs/examples_and_tutorials/basic_interactions/04_other_interactions.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/05_configuring.rst` & `cellpy-1.0.0a5/docs/examples_and_tutorials/basic_interactions/05_configuring.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/06_pandas.rst` & `cellpy-1.0.0a5/docs/examples_and_tutorials/basic_interactions/06_pandas.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst` & `cellpy-1.0.0a5/docs/examples_and_tutorials/basic_interactions/07_data_mining.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst` & `cellpy-1.0.0a5/docs/examples_and_tutorials/basic_interactions/08_the_cellpy_cmd.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png` & `cellpy-1.0.0a5/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_001.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png` & `cellpy-1.0.0a5/docs/examples_and_tutorials/notebooks/images/templates_jupyterlab_002.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/examples_and_tutorials/tips_and_tricks.rst` & `cellpy-1.0.0a5/docs/examples_and_tutorials/tips_and_tricks.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/examples_and_tutorials/utils/batch.rst` & `cellpy-1.0.0a5/docs/examples_and_tutorials/utils/batch.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png` & `cellpy-1.0.0a5/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png` & `cellpy-1.0.0a5/docs/examples_and_tutorials/utils/figures/tutorials_utils_plotting_fig2.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/examples_and_tutorials/utils/ica.rst` & `cellpy-1.0.0a5/docs/examples_and_tutorials/utils/ica.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/examples_and_tutorials/utils/plotting.rst` & `cellpy-1.0.0a5/docs/examples_and_tutorials/utils/plotting.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst` & `cellpy-1.0.0a5/docs/examples_and_tutorials/utils/tut_ocv_rlx.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/figures/cellpy-icon-bw.png` & `cellpy-1.0.0a5/docs/figures/cellpy-icon-bw.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/figures/cellpy-logo-v1.png` & `cellpy-1.0.0a5/docs/figures/cellpy-logo-v1.png`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/index.rst` & `cellpy-1.0.0a5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/main_description/formats.rst` & `cellpy-1.0.0a5/docs/main_description/formats.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/main_description/installation.rst` & `cellpy-1.0.0a5/docs/main_description/installation.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/main_description/usage.rst` & `cellpy-1.0.0a5/docs/main_description/usage.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/make.bat` & `cellpy-1.0.0a5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/source/cellpy.parameters.rst` & `cellpy-1.0.0a5/docs/source/cellpy.parameters.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/source/cellpy.readers.instruments.configurations.rst` & `cellpy-1.0.0a5/docs/source/cellpy.readers.instruments.configurations.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/source/cellpy.readers.instruments.loader_specific_modules.rst` & `cellpy-1.0.0a5/docs/source/cellpy.readers.instruments.loader_specific_modules.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/source/cellpy.readers.instruments.processors.rst` & `cellpy-1.0.0a5/docs/source/cellpy.readers.instruments.processors.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/source/cellpy.readers.instruments.rst` & `cellpy-1.0.0a5/docs/source/cellpy.readers.instruments.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/source/cellpy.readers.rst` & `cellpy-1.0.0a5/docs/source/cellpy.readers.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/source/cellpy.rst` & `cellpy-1.0.0a5/docs/source/cellpy.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/source/cellpy.utils.batch_tools.rst` & `cellpy-1.0.0a5/docs/source/cellpy.utils.batch_tools.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/docs/source/cellpy.utils.rst` & `cellpy-1.0.0a5/docs/source/cellpy.utils.rst`

 * *Files identical despite different names*

### Comparing `cellpy-1.0.0a4/setup.py` & `cellpy-1.0.0a5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,114 +1,117 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""Setup script for PyPI packaging
-
-This script is used for creating the PyPI package.
-
-$ python setup.py sdist # create gzip distr (source dist)
-$ python setup.py bdist_wheel # create build
-$ twine upload dist/* # upload to PyPI
-"""
-import os
-
-from setuptools import find_packages, setup
-
-with open("README.rst") as readme_file:
-    readme = readme_file.read()
-
-with open("HISTORY.rst") as history_file:
-    history = history_file.read()
-
-included_packages = find_packages(
-    exclude=[
-        "build",
-        "docs",
-        "templates",
-        "tests",
-        "examples",
-        "dev_data",
-        "dev_utils",
-        "testdata",
-        "recipe",
-        ".github",
-        ".pytest_cache",
-    ]
-)
-
-# TODO: update this
-requirements = [
-    "scipy",
-    "numpy>=1.16.4",
-    "pandas>=1.5.0",
-    "python-box",
-    "setuptools",
-    "ruamel.yaml",
-    "matplotlib",
-    "openpyxl",
-    "click",
-    "PyGithub",
-    "tqdm",
-    "pint",
-    'pyodbc;platform_system=="windows"',
-    "sqlalchemy>=2.0.0",
-    'sqlalchemy-access;platform_system=="windows"',
-    "python-dotenv",
-    "fabric",
-    # 'tables', # not available by pip
-]
-
-test_requirements = [
-    "lmfit",
-    "pytest",
-]
-
-extra_req_batch = ["ipython", "jupyter", "plotly", "seaborn", "kaleido==0.1.*"]
-extra_req_fit = ["lmfit"]
-extra_req_all = extra_req_batch + extra_req_fit
-
-extra_requirements = {
-    "batch": extra_req_batch,
-    "fit": extra_req_fit,
-    "all": extra_req_all,
-}
-name = "cellpy"
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-user_dir = os.path.expanduser("~")
-
-version_ns = {}
-with open(os.path.join(here, name, "_version.py")) as f:
-    exec(f.read(), {}, version_ns)
-
-description = "Extract and manipulate data from battery data testers."
-
-setup(
-    name=name,
-    version=version_ns["__version__"],
-    description=description,
-    long_description=readme + "\n\n" + history,
-    author="Jan Petter Maehlen",
-    author_email="jepe@ife.no",
-    url="https://github.com/jepegit/cellpy",
-    packages=included_packages,
-    package_dir={"cellpy": "cellpy"},
-    package_data={"parameters": [".cellpy_prms_default.conf"]},
-    entry_points={"console_scripts": ["cellpy=cellpy.cli:cli"]},
-    include_package_data=True,
-    install_requires=requirements,
-    license="MIT license",
-    zip_safe=False,
-    keywords="cellpy",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: MIT License",
-        "Natural Language :: English",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-    ],
-    test_suite="tests",
-    tests_require=test_requirements,
-    extras_require=extra_requirements,
-)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+"""Setup script for PyPI packaging
+
+This script is used for creating the PyPI package.
+
+$ python setup.py sdist # create gzip distr (source dist)
+$ python setup.py bdist_wheel # create build
+$ twine upload dist/* # upload to PyPI
+"""
+import os
+
+from setuptools import find_packages, setup
+
+with open("README.rst") as readme_file:
+    readme = readme_file.read()
+
+with open("HISTORY.rst") as history_file:
+    history = history_file.read()
+
+included_packages = find_packages(
+    exclude=[
+        "build",
+        "docs",
+        "templates",
+        "tests",
+        "examples",
+        "dev_data",
+        "dev_utils",
+        "testdata",
+        "recipe",
+        ".github",
+        ".pytest_cache",
+    ]
+)
+
+# TODO: update this
+requirements = [
+    "scipy",
+    "numpy>=1.16.4",
+    "pandas>=1.5.0",
+    "python-box",
+    "setuptools",
+    "ruamel.yaml",
+    "matplotlib",
+    "openpyxl",
+    "click",
+    "PyGithub",
+    "tqdm",
+    "pint",
+    'pyodbc;platform_system=="windows"',
+    "sqlalchemy>=2.0.0",
+    'sqlalchemy-access;platform_system=="windows"',
+    "python-dotenv",
+    "fabric",
+    # 'tables', # not available by pip
+]
+
+test_requirements = [
+    "lmfit",
+    "pytest",
+]
+
+extra_req_batch = ["ipython", "jupyter", "plotly", "seaborn", "kaleido==0.1.*"]
+extra_req_fit = ["lmfit"]
+extra_req_all = extra_req_batch + extra_req_fit
+
+extra_requirements = {
+    "batch": extra_req_batch,
+    "fit": extra_req_fit,
+    "all": extra_req_all,
+}
+name = "cellpy"
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+user_dir = os.path.expanduser("~")
+
+version_ns = {}
+with open(os.path.join(here, name, "_version.py")) as f:
+    exec(f.read(), {}, version_ns)
+
+description = "Extract and manipulate data from battery data testers."
+
+setup(
+    name=name,
+    version=version_ns["__version__"],
+    description=description,
+    long_description=readme + "\n\n" + history,
+    author="Jan Petter Maehlen",
+    author_email="jepe@ife.no",
+    url="https://github.com/jepegit/cellpy",
+    packages=included_packages,
+    package_dir={"cellpy": "cellpy"},
+    package_data={"parameters": [".cellpy_prms_default.conf"],
+                  "utils/data": ["*.h5"],
+                  "utils/data/raw": ["*.res"],},
+
+    entry_points={"console_scripts": ["cellpy=cellpy.cli:cli"]},
+    include_package_data=True,
+    install_requires=requirements,
+    license="MIT license",
+    zip_safe=False,
+    keywords="cellpy",
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Science/Research",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
+    test_suite="tests",
+    tests_require=test_requirements,
+    extras_require=extra_requirements,
+)
```

