# Comparing `tmp/peegy-1.3.7.tar.gz` & `tmp/peegy-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peegy-1.3.7.tar", last modified: Mon Apr 17 15:31:37 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `peegy-1.3.7.tar` & `peegy-1.4.3.tar`

### file list

```diff
@@ -1,214 +1,184 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.256821 peegy-1.3.7/
--rw-rw-rw-   0 root         (0) root         (0)     1040 2023-04-17 15:12:09.000000 peegy-1.3.7/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1150 2023-04-17 15:31:37.255821 peegy-1.3.7/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.144813 peegy-1.3.7/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10796 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_abr_peak_detection.py
--rw-rw-rw-   0 root         (0) root         (0)    17277 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_acc_eog_removal_template_.py
--rw-rw-rw-   0 root         (0) root         (0)    10930 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_acc_peak_detection.py
--rw-rw-rw-   0 root         (0) root         (0)     8276 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_acc_peak_detection_bootstrap.py
--rw-rw-rw-   0 root         (0) root         (0)    10923 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_acc_peak_detection_filters.py
--rw-rw-rw-   0 root         (0) root         (0)    12109 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_acc_video.py
--rw-rw-rw-   0 root         (0) root         (0)    12378 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_acc_weighted_average.py
--rw-rw-rw-   0 root         (0) root         (0)    10304 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_acc_weighted_vs_standard_average.py
--rw-rw-rw-   0 root         (0) root         (0)    15471 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_assr_dss_frequency_domain_bias_test.py
--rw-rw-rw-   0 root         (0) root         (0)    12503 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_assr_dss_time_domain_bias_test.py
--rw-rw-rw-   0 root         (0) root         (0)     9505 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_assr_f_test.py
--rw-rw-rw-   0 root         (0) root         (0)    11144 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_assr_ht2_test.py
--rw-rw-rw-   0 root         (0) root         (0)    11861 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_assr_ht2_test_weighted_average.py
--rw-rw-rw-   0 root         (0) root         (0)     8671 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_assr_ht2_test_wrong_bias_frequnecy.py
--rw-rw-rw-   0 root         (0) root         (0)     6918 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_assr_no_layout.py
--rw-rw-rw-   0 root         (0) root         (0)     6851 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_assr_phase_locking_value_test.py
--rw-rw-rw-   0 root         (0) root         (0)    12611 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_ffr_artifact_removal.py
--rw-rw-rw-   0 root         (0) root         (0)     7895 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_using_own_data_trials.py
--rw-rw-rw-   0 root         (0) root         (0)     7952 2023-04-17 15:12:09.000000 peegy-1.3.7/examples/example_using_own_raw_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.145814 peegy-1.3.7/peegy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.154814 peegy-1.3.7/peegy/definitions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/definitions/channel_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)    31413 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/definitions/edf_bdf_reader.py
--rw-rw-rw-   0 root         (0) root         (0)    57262 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/definitions/eegReaderAbstractClasses.py
--rw-rw-rw-   0 root         (0) root         (0)     9074 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/definitions/eeg_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     7273 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/definitions/events.py
--rw-rw-rw-   0 root         (0) root         (0)     1287 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/definitions/tables.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.156814 peegy-1.3.7/peegy/directories/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/directories/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2322 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/directories/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.160815 peegy-1.3.7/peegy/io/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20916 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/edf_bdf_reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.162815 peegy-1.3.7/peegy/io/eeg/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/eeg/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7491 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/eeg/reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.163815 peegy-1.3.7/peegy/io/external_tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/external_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.168815 peegy-1.3.7/peegy/io/external_tools/aep_gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/external_tools/aep_gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7276 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/external_tools/aep_gui/aep_matlab_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    11573 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/external_tools/aep_gui/dataReadingTools.py
--rw-rw-rw-   0 root         (0) root         (0)     4782 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/external_tools/aep_gui/extsys_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     5188 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py
--rw-rw-rw-   0 root         (0) root         (0)    20273 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/external_tools/file_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     4695 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/generic_csv_reader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.172815 peegy-1.3.7/peegy/io/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10450 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/storage/data_storage_reading_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    16923 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/storage/data_storage_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    29181 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/storage/plot_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     4621 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/synergy_reader.py
--rw-rw-rw-   0 root         (0) root         (0)     1428 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/io/xml_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.185816 peegy-1.3.7/peegy/layouts/
--rw-rw-rw-   0 root         (0) root         (0)    10895 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/KIT-160.lay
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5612 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi128.lay
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi16.lay
--rw-rw-rw-   0 root         (0) root         (0)     7045 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi160.lay
--rw-rw-rw-   0 root         (0) root         (0)    11339 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi256.lay
--rw-rw-rw-   0 root         (0) root         (0)     1379 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi32.lay
--rw-rw-rw-   0 root         (0) root         (0)     1469 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi32_2_EXT.lay
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi32_fnirs_MP.lay
--rw-rw-rw-   0 root         (0) root         (0)      957 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi32_fnirs_jaime.lay
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi64.lay
--rw-rw-rw-   0 root         (0) root         (0)     2860 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi64_2_EXT.lay
--rw-rw-rw-   0 root         (0) root         (0)     2903 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/biosemi64_3_EXT.lay
--rw-rw-rw-   0 root         (0) root         (0)      597 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/emotive14.lay
--rw-rw-rw-   0 root         (0) root         (0)     5248 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/layouts.py
--rw-rw-rw-   0 root         (0) root         (0)     3821 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/layouts/neuroscan64.lay
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.188817 peegy-1.3.7/peegy/plot/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    50150 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/plot/eeg_ave_epochs_plot_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     3001 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/plot/eeg_plot_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.188817 peegy-1.3.7/peegy/processing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.189817 peegy-1.3.7/peegy/processing/events/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3067 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/events/event_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.205818 peegy-1.3.7/peegy/processing/pipe/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3601 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/attach.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.206818 peegy-1.3.7/peegy/processing/pipe/bootstrap/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/bootstrap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12254 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/bootstrap/bootstrap.py
--rw-rw-rw-   0 root         (0) root         (0)    25813 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     1988 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/detection.py
--rw-rw-rw-   0 root         (0) root         (0)    30969 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/epochs.py
--rw-rw-rw-   0 root         (0) root         (0)    33757 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/general.py
--rw-rw-rw-   0 root         (0) root         (0)     9032 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/interpolation.py
--rw-rw-rw-   0 root         (0) root         (0)    13088 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/io.py
--rw-rw-rw-   0 root         (0) root         (0)     5252 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)    15881 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/plot.py
--rw-rw-rw-   0 root         (0) root         (0)     6983 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/regression.py
--rw-rw-rw-   0 root         (0) root         (0)    22084 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/simulate.py
--rw-rw-rw-   0 root         (0) root         (0)    38597 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/spatial_filtering.py
--rw-rw-rw-   0 root         (0) root         (0)    27211 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)     6463 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/storage.py
--rw-rw-rw-   0 root         (0) root         (0)    10453 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/pipe/time_frequency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.208818 peegy-1.3.7/peegy/processing/statistics/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/statistics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6175 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/statistics/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)    14461 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/statistics/eeg_statistic_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.211818 peegy-1.3.7/peegy/processing/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/system/memory.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/system/progress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.214819 peegy-1.3.7/peegy/processing/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.216819 peegy-1.3.7/peegy/processing/tools/detection/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/detection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8780 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/detection/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     9602 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/detection/time_domain_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    20468 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/eeg_epoch_operators.py
--rw-rw-rw-   0 root         (0) root         (0)    69736 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/epochs_processing_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.218819 peegy-1.3.7/peegy/processing/tools/filters/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/filters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15600 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/filters/eegFiltering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.219819 peegy-1.3.7/peegy/processing/tools/filters/eog_tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/filters/eog_tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19679 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/filters/eog_tools/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2123 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/filters/resampling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.220819 peegy-1.3.7/peegy/processing/tools/filters/spatial_filtering/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/filters/spatial_filtering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1581 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/filters/spatial_filtering/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     6169 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.221819 peegy-1.3.7/peegy/processing/tools/fitting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/fitting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/fitting/fitting_functions.py
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/math_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.222819 peegy-1.3.7/peegy/processing/tools/multiprocessing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/multiprocessing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6448 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.224819 peegy-1.3.7/peegy/processing/tools/template_generator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/template_generator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13598 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/template_generator/auditory_waveforms.py
--rw-rw-rw-   0 root         (0) root         (0)    37074 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/template_generator/h0.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.224819 peegy-1.3.7/peegy/processing/tools/video/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/video/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1330 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/video/recording.py
--rw-rw-rw-   0 root         (0) root         (0)    48703 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/processing/tools/weightedAverage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.249821 peegy-1.3.7/peegy/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.251821 peegy-1.3.7/peegy/test/artifact_removal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/artifact_removal/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3258 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/artifact_removal/ir_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4867 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/artifact_removal/regression_artifact_removal.py
--rw-rw-rw-   0 root         (0) root         (0)     4857 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/artifact_removal/xcorr_artifact_removal.py
--rw-rw-rw-   0 root         (0) root         (0)     1945 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/dss_unit_tests.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/eeg_test_resampling.py
--rw-rw-rw-   0 root         (0) root         (0)     3638 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/javerager_test.py
--rw-rw-rw-   0 root         (0) root         (0)      871 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/read_data_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3406 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_assr_moving_average.py
--rw-rw-rw-   0 root         (0) root         (0)     2709 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_average_spectrogram_power.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_biosemi_class.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_biosemi_reader.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_bootstraping.py
--rw-rw-rw-   0 root         (0) root         (0)     1218 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_edf_reader.py
--rw-rw-rw-   0 root         (0) root         (0)      564 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_eeg_notch_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2490 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_eog_removal_correlation.py
--rw-rw-rw-   0 root         (0) root         (0)     3472 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_eog_template_removal.py
--rw-rw-rw-   0 root         (0) root         (0)     2012 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_eog_template_valderrama_20118.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_et_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2582 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_fir_filter_mt.py
--rw-rw-rw-   0 root         (0) root         (0)     1603 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_fir_filter_ols.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_fiter_mt.py
--rw-rw-rw-   0 root         (0) root         (0)     5716 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_freq_noise_estimation.py
--rw-rw-rw-   0 root         (0) root         (0)     3476 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_freq_noise_estimation_plots.py
--rw-rw-rw-   0 root         (0) root         (0)     1749 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_frequency_average_epochs.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_generic_reader.py
--rw-rw-rw-   0 root         (0) root         (0)     2032 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_hotelling_t2.py
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_ica_average_epochs.py
--rw-rw-rw-   0 root         (0) root         (0)      684 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_multiprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     2373 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_noise_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_norm_corr.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_parse_processing_chain.py
--rw-rw-rw-   0 root         (0) root         (0)     2587 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_peakdetection.py
--rw-rw-rw-   0 root         (0) root         (0)     2431 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_phase_locking_value.py
--rw-rw-rw-   0 root         (0) root         (0)     6025 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_pooled_freq_noise_estimation.py
--rw-rw-rw-   0 root         (0) root         (0)     2968 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_scrolling.py
--rw-rw-rw-   0 root         (0) root         (0)     5499 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_spatial_filtering_example1.py
--rw-rw-rw-   0 root         (0) root         (0)     1286 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_spatial_filtering_example6.py
--rw-rw-rw-   0 root         (0) root         (0)     6047 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_spatial_filtering_freq_domain.py
--rw-rw-rw-   0 root         (0) root         (0)     7065 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_spatial_filtering_freq_domain_2.py
--rw-rw-rw-   0 root         (0) root         (0)     8319 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_w_average_epochs.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/test/test_xml_to_dict.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.252821 peegy-1.3.7/peegy/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.252821 peegy-1.3.7/peegy/tools/aep_gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/tools/aep_gui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.253821 peegy-1.3.7/peegy/tools/signal_generator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/tools/signal_generator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4417 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/tools/signal_generator/noise_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.254821 peegy-1.3.7/peegy/tools/units/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/tools/units/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      629 2023-04-17 15:12:09.000000 peegy-1.3.7/peegy/tools/units/unit_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.147814 peegy-1.3.7/peegy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1150 2023-04-17 15:31:36.000000 peegy-1.3.7/peegy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6684 2023-04-17 15:31:37.000000 peegy-1.3.7/peegy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 15:31:37.000000 peegy-1.3.7/peegy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      527 2023-04-17 15:31:37.000000 peegy-1.3.7/peegy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-17 15:31:37.000000 peegy-1.3.7/peegy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 15:31:37.256821 peegy-1.3.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2297 2023-04-17 15:12:09.000000 peegy-1.3.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 15:31:37.255821 peegy-1.3.7/test_data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 15:12:09.000000 peegy-1.3.7/test_data/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/.gitattributes
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 peegy-1.4.3/.gitlab-ci.yml
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 peegy-1.4.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 peegy-1.4.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 peegy-1.4.3/MANIFEST.in
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 peegy-1.4.3/Readme.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/__init__.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 peegy-1.4.3/requirements.txt
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 peegy-1.4.3/setup.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/README.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/__init__.py
+-rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_abr_peak_detection.py
+-rw-r--r--   0        0        0    17277 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_acc_eog_removal_template_.py
+-rw-r--r--   0        0        0    10930 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_acc_peak_detection.py
+-rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_acc_peak_detection_bootstrap.py
+-rw-r--r--   0        0        0    10923 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_acc_peak_detection_filters.py
+-rw-r--r--   0        0        0    12109 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_acc_video.py
+-rw-r--r--   0        0        0    12378 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_acc_weighted_average.py
+-rw-r--r--   0        0        0    10304 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_acc_weighted_vs_standard_average.py
+-rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_assr_dss_frequency_domain_bias_test.py
+-rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_assr_dss_time_domain_bias_test.py
+-rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_assr_f_test.py
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_assr_ht2_test.py
+-rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_assr_ht2_test_weighted_average.py
+-rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_assr_ht2_test_wrong_bias_frequnecy.py
+-rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_assr_no_layout.py
+-rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_assr_phase_locking_value_test.py
+-rw-r--r--   0        0        0    12611 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_ffr_artifact_removal.py
+-rw-r--r--   0        0        0     7895 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_using_own_data_trials.py
+-rw-r--r--   0        0        0     7952 2020-02-02 00:00:00.000000 peegy-1.4.3/examples/example_using_own_raw_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/definitions/__init__.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/definitions/channel_definitions.py
+-rw-r--r--   0        0        0    31413 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/definitions/edf_bdf_reader.py
+-rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/definitions/eegReaderAbstractClasses.py
+-rw-r--r--   0        0        0     9074 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/definitions/eeg_definitions.py
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/definitions/events.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/definitions/tables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/directories/__init__.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/directories/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/__init__.py
+-rw-r--r--   0        0        0    20913 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/edf_bdf_reader.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/generic_csv_reader.py
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/synergy_reader.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/xml_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/eeg/__init__.py
+-rw-r--r--   0        0        0     7491 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/eeg/reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/external_tools/__init__.py
+-rw-r--r--   0        0        0    20273 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/external_tools/file_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/external_tools/aep_gui/__init__.py
+-rw-r--r--   0        0        0     7276 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/external_tools/aep_gui/aep_matlab_tools.py
+-rw-r--r--   0        0        0    11573 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/external_tools/aep_gui/dataReadingTools.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/external_tools/aep_gui/extsys_tools.py
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/storage/__init__.py
+-rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/storage/data_storage_reading_tools.py
+-rw-r--r--   0        0        0    16923 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/storage/data_storage_tools.py
+-rw-r--r--   0        0        0    29698 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/io/storage/plot_tools.py
+-rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/KIT-160.lay
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/__init__.py
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi128.lay
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi16.lay
+-rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi160.lay
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi256.lay
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi32.lay
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi32_2_EXT.lay
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi32_fnirs_MP.lay
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi32_fnirs_jaime.lay
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi64.lay
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi64_2_EXT.lay
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/biosemi64_3_EXT.lay
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/emotive14.lay
+-rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/layouts.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/layouts/neuroscan64.lay
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/plot/__init__.py
+-rw-r--r--   0        0        0    50141 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/plot/eeg_ave_epochs_plot_tools.py
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/plot/eeg_plot_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/events/__init__.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/events/event_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/__init__.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/attach.py
+-rw-r--r--   0        0        0    27695 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/definitions.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/detection.py
+-rw-r--r--   0        0        0    31500 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/epochs.py
+-rw-r--r--   0        0        0    33830 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/general.py
+-rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/interpolation.py
+-rw-r--r--   0        0        0    13123 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/io.py
+-rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/pipeline.py
+-rw-r--r--   0        0        0    15881 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/plot.py
+-rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/regression.py
+-rw-r--r--   0        0        0    22084 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/simulate.py
+-rw-r--r--   0        0        0    38597 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/spatial_filtering.py
+-rw-r--r--   0        0        0    27211 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/statistics.py
+-rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/storage.py
+-rw-r--r--   0        0        0    10453 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/time_frequency.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/bootstrap/__init__.py
+-rw-r--r--   0        0        0    22128 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/pipe/bootstrap/bootstrap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/statistics/__init__.py
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/statistics/definitions.py
+-rw-r--r--   0        0        0    14458 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/statistics/eeg_statistic_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/system/__init__.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/system/memory.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/system/progress.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/__init__.py
+-rw-r--r--   0        0        0    20462 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/eeg_epoch_operators.py
+-rw-r--r--   0        0        0    69736 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/epochs_processing_tools.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/math_tools.py
+-rw-r--r--   0        0        0    48694 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/weightedAverage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/detection/__init__.py
+-rw-r--r--   0        0        0     8780 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/detection/definitions.py
+-rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/detection/time_domain_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/filters/__init__.py
+-rw-r--r--   0        0        0    15588 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/filters/eegFiltering.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/filters/resampling.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/filters/eog_tools/__init__.py
+-rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/filters/eog_tools/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/filters/spatial_filtering/__init__.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/filters/spatial_filtering/definitions.py
+-rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/fitting/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/fitting/fitting_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/multiprocessing/__init__.py
+-rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/template_generator/__init__.py
+-rw-r--r--   0        0        0    13598 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/template_generator/auditory_waveforms.py
+-rw-r--r--   0        0        0    37074 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/template_generator/h0.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/video/__init__.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/processing/tools/video/recording.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/__init__.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/dss_unit_tests.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/eeg_test_resampling.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/javerager_test.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/read_data_test.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_assr_moving_average.py
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_average_spectrogram_power.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_biosemi_class.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_biosemi_reader.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_bootstraping.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_edf_reader.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_eeg_notch_filter.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_eog_removal_correlation.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_eog_template_removal.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_eog_template_valderrama_20118.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_et_tools.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_filter.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_fir_filter_mt.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_fir_filter_ols.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_fiter_mt.py
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_freq_noise_estimation.py
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_freq_noise_estimation_plots.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_frequency_average_epochs.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_generic_reader.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_hotelling_t2.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_ica_average_epochs.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_multiprocessing.py
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_noise_generator.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_norm_corr.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_parse_processing_chain.py
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_peakdetection.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_phase_locking_value.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_pooled_freq_noise_estimation.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_scrolling.py
+-rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_spatial_filtering_example1.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_spatial_filtering_example6.py
+-rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_spatial_filtering_freq_domain.py
+-rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_spatial_filtering_freq_domain_2.py
+-rw-r--r--   0        0        0     8319 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_w_average_epochs.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_xml_to_dict.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/artifact_removal/__init__.py
+-rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/artifact_removal/ir_test.py
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/artifact_removal/regression_artifact_removal.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/artifact_removal/xcorr_artifact_removal.py
+-rw-r--r--   0        0        0  1182949 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/test/test_data/eog_blinks_valderrama_et_al_2018.mat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/tools/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/tools/aep_gui/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/tools/signal_generator/__init__.py
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/tools/signal_generator/noise_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/tools/units/__init__.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 peegy-1.4.3/peegy/tools/units/unit_tools.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 peegy-1.4.3/.gitignore
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 peegy-1.4.3/LICENSE.txt
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 peegy-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 peegy-1.4.3/PKG-INFO
```

### Comparing `peegy-1.3.7/LICENSE.txt` & `peegy-1.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/examples/example_abr_peak_detection.py` & `peegy-1.4.3/examples/example_abr_peak_detection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/examples/example_acc_eog_removal_template_.py` & `peegy-1.4.3/examples/example_acc_eog_removal_template_.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/examples/example_acc_peak_detection.py` & `peegy-1.4.3/examples/example_acc_peak_detection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/examples/example_acc_peak_detection_bootstrap.py` & `peegy-1.4.3/examples/example_acc_peak_detection_bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,21 +149,22 @@
                                             roi_windows=roi_windows,
                                             weighted_average=False)
 
 # bootstrap the pipe
 pipeline['bootstrap'] = Bootstrap(at_each_bootstrap_do=pipeline_bootstrap,
                                   n_bootstraps=100,
                                   event_code=1.0,
+                                  n_jobs=1,
                                   bootstrap_targets=[
                                       BootstrapTarget(
-                                          table_name='hotelling_t2_time',
+                                          test_name='HT2',
                                           group_by=['channel', 'label', 'ini_time', 'end_time'],
                                           target_values=['f']),
                                       BootstrapTarget(
-                                          table_name='f_test_time',
+                                          test_name='Fmp',
                                           group_by=['channel', 'label', 'ini_time', 'end_time'],
                                           target_values=['f'])])
 pipeline.run()
 
 # now we save our data to a database
 subject_info = SubjectInformation(subject_id='Test_Subject')
 measurement_info = MeasurementInformation(
```

### Comparing `peegy-1.3.7/examples/example_acc_peak_detection_filters.py` & `peegy-1.4.3/examples/example_acc_peak_detection_filters.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/examples/example_acc_video.py` & `peegy-1.4.3/examples/example_acc_video.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/examples/example_acc_weighted_average.py` & `peegy-1.4.3/examples/example_acc_weighted_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/examples/example_acc_weighted_vs_standard_average.py` & `peegy-1.4.3/examples/example_acc_weighted_vs_standard_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/examples/example_assr_dss_frequency_domain_bias_test.py` & `peegy-1.4.3/examples/example_assr_dss_frequency_domain_bias_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
-.. _tut-assr-ht2-test-frequency-bias-sim:
+.. _tut-assr-ht2-test-frequency-dss-bias-sim:
 
-##################################################
-ASSR using DSS in the frequency-domain (Simulated)
-##################################################
+#####################################################################
+ASSR using DSS and bootstrapping in the frequency-domain (Simulated)
+#####################################################################
 
 In this example we simulate a low-frequency ASSR, and we assess its significance using the Hotelling's T2 test and
 F-test.
 The background-noise is pink (controlled by noise attenuation = 3) and the presence of the signal is controlled by
 return_noise_only=False (if True, only the noise is returned).
 The signal is equal in all channels so that the detection rate obtained by keeping components can be assessed.
 The spatial filter is biased using the covariance obtained in the frequency-domain.
-This example shows that biasing in the frequency-domain requires > 16 components (about half channels) to keep the
-false detection rate under 5%
+Here, DSS is set-up to preserve only the first component, resulting in a very agressive filter prone to show biases in
+absence of a target signal. To avoid this bias towards false positive a bootstrap approach is used.
+To assess the false positive rate, the parameter return_noise_only should be set to True.
 
 .. contents:: Page contents
    :local:
    :depth: 2
 """
 # Enable below for interactive backend
 # import matplotlib
@@ -110,15 +111,15 @@
 # Plot components in the frequency-domain
 # ---------------------------------------
 # Spatial filter is a applied in the frequency-domain
 
 pipeline['dss_time_epochs'] = CreateAndApplySpatialFilter(pipeline['time_epochs'],
                                                           sf_join_frequencies=join_frequencies,
                                                           test_frequencies=test_frequencies,
-                                                          sf_components=np.arange(17),
+                                                          sf_components=np.arange(1),
                                                           projection_domain=Domain.frequency,
                                                           block_size=10,
                                                           return_figures=True,
                                                           delta_frequency=2 * u.Hz,
                                                           plot_y_lim=[0, 5])
 pipeline.run()
 
@@ -167,21 +168,22 @@
                                                          n_fft=int(epoch_length * fs),
                                                          weight_frequencies=assr_frequency,
                                                          test_frequencies=test_frequencies,
                                                          delta_frequency=2 * u.Hz)
 
 # bootstrap the pipe
 pipeline['bootstrap'] = Bootstrap(
+    n_jobs=1,
     at_each_bootstrap_do=pipeline_bootstrap,
     n_bootstraps=100,
     epoch_length=epoch_length,
     event_code=1.0,
     bootstrap_targets=[
         BootstrapTarget(
-            table_name='hotelling_t2_freq',
+            test_name='HT2',
             group_by=['channel', 'frequency_tested'],
             target_values=['f'])])
 
 pipeline.run()
 # %%
 # Compute global field power (GFP)
 # ---------------------------------------
```

### Comparing `peegy-1.3.7/examples/example_assr_dss_time_domain_bias_test.py` & `peegy-1.4.3/examples/example_assr_dss_time_domain_bias_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/examples/example_assr_f_test.py` & `peegy-1.4.3/examples/example_assr_f_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/examples/example_assr_ht2_test.py` & `peegy-1.4.3/examples/example_assr_ht2_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/examples/example_assr_ht2_test_weighted_average.py` & `peegy-1.4.3/examples/example_assr_ht2_test_weighted_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/examples/example_assr_ht2_test_wrong_bias_frequnecy.py` & `peegy-1.4.3/examples/example_assr_ht2_test_wrong_bias_frequnecy.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/examples/example_assr_no_layout.py` & `peegy-1.4.3/examples/example_assr_no_layout.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/examples/example_assr_phase_locking_value_test.py` & `peegy-1.4.3/examples/example_assr_phase_locking_value_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/examples/example_ffr_artifact_removal.py` & `peegy-1.4.3/examples/example_ffr_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/examples/example_using_own_data_trials.py` & `peegy-1.4.3/examples/example_using_own_data_trials.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/examples/example_using_own_raw_data.py` & `peegy-1.4.3/examples/example_using_own_raw_data.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/definitions/channel_definitions.py` & `peegy-1.4.3/peegy/definitions/channel_definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/definitions/edf_bdf_reader.py` & `peegy-1.4.3/peegy/definitions/edf_bdf_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/definitions/eegReaderAbstractClasses.py` & `peegy-1.4.3/peegy/definitions/eegReaderAbstractClasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         print('get_channel_by_label not defined')
         return
 
     def set_reference(self):
         # if auto_detect_reference:
         #     ref_channels = [channels[self.detect_ref_channel(epochs)]]
         print(('Referencing data to: %s' % ' '.join(map(str, [_ch.label for _ch in self.ref_channels]))))
-        reference = np.zeros(self.epochs_raw.shape[0::2], dtype=np.float)
+        reference = np.zeros(self.epochs_raw.shape[0::2], dtype=float)
         count = 0.0
         for ref_ch in self.ref_channels:
             for i, ch in enumerate(self.channels):
                 if ch.__dict__ == ref_ch.__dict__:
                     reference += self.epochs_raw[:, i, :]
                     count += 1.0
                     #  remove reference if only one is provided
```

### Comparing `peegy-1.3.7/peegy/definitions/eeg_definitions.py` & `peegy-1.4.3/peegy/definitions/eeg_definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/definitions/events.py` & `peegy-1.4.3/peegy/definitions/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     def interpolate_events(self, scaling_factor=1.0, code=None, events_mask=None):
         """
         This function interpolates time events between consecutive event. The time position of new events is defined
         by the scaling factor. For example, an scaling_factor of 2.0 will add a new trigger event exactly in the middle
         time between two events
         :param scaling_factor: a float that determine the number of new events that will be generated
         :param code: event code to be interpolated
-        :param events_mask: integer value used to masker triggers codes. This is useful to ignore triggers inputs avove
+        :param events_mask: integer value used to masker triggers codes. This is useful to ignore triggers inputs above
         a particular value. For example, if only the first 8 trigger inputs were used (max decimal value is 255), in a
         system with 16 trigger inputs, then the masker could be set to 255 to ignore any trigger from trigger inputs 9
         to 16.
         :return: new an Events class containing the new interpolated events
         """
         self.mask = events_mask
         _times = self.get_events_time(code=code)
```

### Comparing `peegy-1.3.7/peegy/definitions/tables.py` & `peegy-1.4.3/peegy/definitions/tables.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/directories/tools.py` & `peegy-1.4.3/peegy/directories/tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/io/edf_bdf_reader.py` & `peegy-1.4.3/peegy/io/edf_bdf_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
     data_channel = np.zeros((buffer_size_data, len(channels) - 1), dtype=np.float32)
     event_channel = np.zeros((buffer_size_data, 1), dtype=np.float32)
 
     event_channel_annotations = None
     if annotated_event_channel:
         event_channel_annotations = np.zeros((buffer_size_events * 3, 1), dtype=np.uint8)
     # buffer to store events as additional channel
-    sys_code_channel = np.zeros((buffer_size_data,), dtype=np.float)
+    sys_code_channel = np.zeros((buffer_size_data,), dtype=float)
     record_length = np.int64(np.sum(header['number_samples_per_record']) * 3)
     _time = ini_time
     with open(header['file_name'], 'rb') as f:
         # skip first 256 bytes + 256 * N channels
         header_off_set = 256 * (1 + header['n_channels'])
         ch_offsets = np.cumsum((np.concatenate(([0], header['number_samples_per_record']))))
         for nr in range(records_to_read):
```

### Comparing `peegy-1.3.7/peegy/io/eeg/reader.py` & `peegy-1.4.3/peegy/io/eeg/reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/io/external_tools/aep_gui/aep_matlab_tools.py` & `peegy-1.4.3/peegy/io/external_tools/aep_gui/aep_matlab_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/io/external_tools/aep_gui/dataReadingTools.py` & `peegy-1.4.3/peegy/io/external_tools/aep_gui/dataReadingTools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/io/external_tools/aep_gui/extsys_tools.py` & `peegy-1.4.3/peegy/io/external_tools/aep_gui/extsys_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py` & `peegy-1.4.3/peegy/io/external_tools/aep_gui/medel_stimuli_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/io/external_tools/file_tools.py` & `peegy-1.4.3/peegy/io/external_tools/file_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/io/generic_csv_reader.py` & `peegy-1.4.3/peegy/io/generic_csv_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/io/storage/data_storage_reading_tools.py` & `peegy-1.4.3/peegy/io/storage/data_storage_reading_tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,39 +43,52 @@
     def __getitem__(self, key):
         return super(PandasDataPages, self).__getitem__(key)
 
 
 def sqlite_tables_to_pandas(database_path: str = None,
                             tables: [str] = None) -> pd.DataFrame:
     """
-    This function will return a pandas dataframe containing the desired tables from a pEEGy .slite database.
+    This function will return a pandas dataframe containing the desired tables from a pEEGy .sqlite database.
     A pEEGy database will always contain a table 'subjects', 'measurement_info' , 'stimuli', 'recording'.
     Each subject will be linked to measurement by their id. Similarly, each measurement will be linked to each stimulus
     by its id.
     Any other table, for example, recording, waveforms, hotelling_t2_time, hotelling_t2_freq, f_test_time, f_test_freq,
     or other tables created by the user, will be uniquely related to each subject, measurement, recording, and stimuli
     by id_subject, id_measurement, id_recording, and _id_stimuli, respectively.
     This function will provide a user-friendly pandas dataframe by pooling together this information by indexing the
     corresponding ids to their respective values.
     :param database_path: path to the database from which we will read the tables
-    :param tables: a list of strings containing the tables we can't to read. Make sure these tables are present in the
+    :param tables: a list of strings containing the tables want to read. Make sure these tables are present in the
     database
     :return: a pandas dataframe with the respective tables.
     """
     out = PandasDataPages()
     db = sqlite3.connect(database_path)
+    cursor = db.cursor()
+    cursor.execute("SELECT name FROM sqlite_master WHERE type='table';")
+    all_tables = [_tables[0] for _tables in cursor.fetchall()]
+    extra_tables = ''
+    extra_outputs = ''
+    if 'recording' in all_tables:
+        extra_tables = extra_tables.join('JOIN recording REC ON REC.id_measurement = MES.id ')
+        extra_outputs = extra_outputs.join('{:}.*, '.format('REC'))
+
     for _table in tables:
         df = pd.read_sql_query('SELECT SUB.*, '
                                'MES.*, '
                                'STI.*, '
+                               '{:}'
                                'TAB.* '
                                'FROM subjects as SUB '
                                'JOIN measurement_info MES ON (MES.id_subject = SUB.id) '
                                'JOIN stimuli STI ON STI.id_measurement = MES.id '
-                               'JOIN {:} as TAB ON TAB.id_stimuli == STI.id'.format(_table),
+                               '{:}'
+                               'JOIN {:} as TAB ON TAB.id_stimuli == STI.id'.format(extra_outputs,
+                                                                                    extra_tables,
+                                                                                    _table),
                                db)
         out[_table] = df
     return out
 
 
 def sqlite_waveforms_to_pandas(database_path: str = None,
                                group_factors: [str] = None,
@@ -111,19 +124,27 @@
     dataframe. The tables should contain 'subjects', 'measurement_info' , 'stimuli', 'recording' columns so they can
     be joined.
     :param channels: list of string specifying for which channels you want to extract the waveforms. If empty, all
     channels will be returned.
     :return: a pandas dataframe with the data grouped by group_factors.
     """
     db = sqlite3.connect(database_path)
+    cursor = db.cursor()
+    cursor.execute("SELECT name FROM sqlite_master WHERE type='table';")
+    all_tables = [_tables[0] for _tables in cursor.fetchall()]
+
     if channels is not None:
         channels_str = ','.join(['"{:}"'.format(_ch) for _ch in channels])
         channels_str = 'WAVE.channel IN ({:}) and'.format(channels_str)
     extra_tables = ''
     extra_outputs = ''
+    if 'recording' in all_tables:
+        extra_tables = extra_tables.join('JOIN recording REC ON REC.id_measurement = MES.id ')
+        extra_outputs = extra_outputs.join('{:}.*, '.format('REC'))
+
     if tables is not None:
         extra_tables = extra_tables.join(['JOIN {:} ON {:}.id_stimuli = STI.id '.format(_tab, _tab) for
                                           _tab in tables])
         extra_outputs = extra_outputs.join(['{:}.*, '.format(_tab) for
                                             _tab in tables])
     df = pd.read_sql_query(
         'SELECT SUB.*, '
```

### Comparing `peegy-1.3.7/peegy/io/storage/data_storage_tools.py` & `peegy-1.4.3/peegy/io/storage/data_storage_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/io/storage/plot_tools.py` & `peegy-1.4.3/peegy/io/storage/plot_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,38 +77,43 @@
     df = copy.copy(dataframe)
     df.reset_index(inplace=True, drop=True)
     _rows_and_cols = []
     # n_rows = 1
     # n_cols = 1
     row_conditions = np.array([1])
     col_conditions = np.array([1])
+    # unique_row_domains = False
+    # unique_col_domains = False
     if rows_by is not None:
         _rows_and_cols.append(rows_by)
         row_conditions = df[rows_by].astype("category").cat.categories
-        # row_domains = df.iloc[df[rows_by].index.values]['domain']
+        row_domains = df.iloc[df[rows_by].index]['domain'].unique()
+        unique_row_domains = row_domains.size == 1
         n_rows = row_conditions.size
     else:
         df.loc[:, 'dummy_row'] = 1
         _rows_and_cols.append('dummy_row')
         # row_domains = df['domain']
         n_rows = 1
     idx_rows = np.arange(row_conditions.size)
     if cols_by is not None:
         _rows_and_cols.append(cols_by)
         col_conditions = df[cols_by].astype("category").cat.categories
+        # col_domains = df.iloc[df[cols_by].index]['domain'].unique()
+        # unique_col_domains = col_domains.size == 1
         # col_domains = df.iloc[df[cols_by].index.values]['domain']
         n_cols = col_conditions.size
     else:
         df.loc[:, 'dummy_col'] = 1
         _rows_and_cols.append('dummy_col')
         n_cols = 1
         # col_domains = df['domain']
     idx_cols = np.arange(col_conditions.size)
 
-    common_x_axis = np.unique(col_conditions).size == 1
+    # common_x_axis = np.unique(col_conditions).size == 1
     groups = df.groupby(_rows_and_cols)
     fig_out, ax = plt.subplots(n_rows, n_cols)
     gs = gridspec.GridSpec(n_rows, n_cols)
     for _id, ((_current_row_group, _current_col_group), _group) in enumerate(groups):
         _current_group = _group
         if blend_subcategories:
             _current_group = _group.iloc[[0]].copy().reset_index()
@@ -210,33 +215,35 @@
             if show_sd:
                 ax.fill_between(x.value,
                                 (y_mean - y_sd).value,
                                 (y_mean + y_sd).value,
                                 alpha=sd_alpha,
                                 edgecolor="none",
                                 facecolor=_colors(_i))
-            if _idx_col == n_cols - 1:
-                ax_row_label = ax.twinx()
-                ax_row_label.set_ylabel(_current_row_group, size=fontsize)
-                ax_row_label.set_yticklabels([])
-                ax_row_label.tick_params(
-                    axis='y',  # changes apply to the x-axis
-                    which='both',  # both major and minor ticks are affected
-                    right=False,  # ticks along the bottom edge are off
-                    left=False,  # ticks along the top edge are off
-                    labelleft=True)
+
+            _last_col_ax = plt.subplot(gs[_idx_row, n_cols - 1])
+            ax_row_label = _last_col_ax.twinx()
+            ax_row_label.set_ylabel(_current_row_group, size=fontsize)
+            ax_row_label.set_yticklabels([])
+            ax_row_label.tick_params(
+                axis='y',  # changes apply to the x-axis
+                which='both',  # both major and minor ticks are affected
+                right=False,  # ticks along the bottom edge are off
+                left=False,  # ticks along the top edge are off
+                labelleft=True)
 
             if _domain == 'time':
                 if time_xlim is not None:
                     ax.set_xlim(time_xlim)
                 if time_ylim is not None:
                     ax.set_ylim(time_ylim)
                 if time_vmarkers is not None:
                     [ax.axvline(_t, color='k', linestyle=':', linewidth=0.5) for _t in time_vmarkers]
-                ax.set_xlabel('Time [{:}]'.format(x_unit.unit), size=fontsize)
+                ax.set_xlabel('Time [{:}]'.format(x.unit), size=fontsize)
+
             if _domain == 'frequency':
                 if freq_xlim is not None:
                     ax.set_xlim(freq_xlim)
                 if freq_ylim is not None:
                     ax.set_ylim(freq_ylim)
                 if freq_vmarkers is not None:
                     if freq_vmarkers_style is None:
@@ -246,39 +253,49 @@
                         [ax.plot(_f, y_max * 0.93,
                                  color='g',
                                  marker=freq_vmarkers_style,
                                  markersize=3) for _f in freq_vmarkers]
                 ax.set_xlabel('Frequency [{:}]'.format(x.unit), size=fontsize)
             handles, labels = ax.get_legend_handles_labels()
             if len(labels) > 1 and show_legend:
-                fig_out.legend(handles,
-                               labels,
-                               loc='upper center',
-                               fontsize=8,
-                               frameon=False,
-                               ncol=len(labels))
+                ax.legend(handles,
+                          labels,
+                          loc='upper center',
+                          fontsize=8,
+                          frameon=False,
+                          ncol=len(labels))
+
+    all_axes = fig_out.get_axes()
+    all_axis_with_data = np.all([ax.has_data() for ax in all_axes])
+
     if ylabel is None:
         if y_unit_to is not None:
             fig_out.supylabel('Amplitude [{:}]'.format(y_unit_to), size=fontsize)
     else:
         fig_out.supylabel(ylabel, size=fontsize)
-    if common_x_axis and _domain == 'time' and x_unit_to is not None:
-        fig_out.supxlabel('Time [{:}]'.format(x_unit_to), size=fontsize)
-    if common_x_axis and _domain == 'frequency' and x_unit_to is not None:
-        fig_out.supxlabel('Frequency [{:}]'.format(x_unit_to), size=fontsize)
+    if unique_row_domains and all_axis_with_data and np.all(row_domains == 'time'):
+        fig_out.supxlabel('Time [{:}]'.format(_x_unit_to), size=fontsize)
+    if unique_row_domains and all_axis_with_data and np.all(row_domains == 'frequency'):
+        fig_out.supxlabel('Frequency [{:}]'.format(_x_unit_to), size=fontsize)
 
-    all_axes = fig_out.get_axes()
     for ax in all_axes:
+        if not ax.has_data():
+            ax.get_xaxis().set_visible(False)
+            ax.set_xticklabels([])
+            ax.set_yticklabels([])
+            ax.set_xlabel('')
+            continue
         ax.spines['top'].set_visible(False)
-        if not ax.get_subplotspec().is_last_row():  # and row_domains.unique().size == 1:
+        if unique_row_domains and all_axis_with_data and not ax.get_subplotspec().is_last_row():
             ax.set_xticklabels([])
             ax.set_xlabel('')
         ax.spines['left'].set_visible(True)
         ax.spines['right'].set_visible(False)
         ax.tick_params(labelsize=6)
+
     inch = 2.54
     fig_out.set_size_inches(12.0 / inch, 2.25 * len(row_conditions) / inch)
     fig_out.subplots_adjust(top=0.98, bottom=0.08, hspace=0.0, left=0.15, right=0.95)
     return fig_out
 
 
 def plot_topographic_maps(dataframe: pd.DataFrame = None,
@@ -289,15 +306,15 @@
                           channels_column: str = 'channel',
                           title: str = '',
                           topographic_value: str = None,
                           layout: str = None,
                           title_by: str = 'row',
                           title_v_offset: float = 0.0,
                           fontsize: float = 6,
-                          grid_size: np.complex = 600j,
+                          grid_size: np.complex_ = 600j,
                           color_map_label: str = None,
                           normalize: bool = False,
                           show_sensors: bool = True,
                           show_sensor_label: bool = False,
                           n_contour_levels: int = 35,
                           max_topographic_value: float = None,
                           min_topographic_value: float = None,
@@ -501,15 +518,15 @@
 
 
 def get_topographic_maps(df,
                          subject_id_column: str = 'subject_id',
                          channels_column: str = 'channel',
                          topographic_value: str = None,
                          layout: str = None,
-                         grid_size: np.complex = 600j,
+                         grid_size: np.complex_ = 600j,
                          apply_function: object = None,
                          fun_args: dict = {}):
     _lay = Layout()
     _layout = _lay.get_layout(file_name=layout)
     _layout = np.array([_l for _l in _layout if _l.label not in ['COMNT', 'SCALE']])
     _single_responses = np.array([])
 
@@ -549,15 +566,15 @@
 
 def get_topographic_maps_as_df(dataframe: pd.DataFrame = None,
                                group_by: [str] = None,
                                subject_id_column: str = 'subject_id',
                                channels_column: str = 'channel',
                                topographic_value: str = None,
                                layout: str = None,
-                               grid_size: np.complex = 600j,
+                               grid_size: np.complex_ = 600j,
                                apply_function: object = np.mean,
                                fun_args: dict = {}
                                ) -> pd.DataFrame:
     """
     This function will plot the waveforms contained in a pandas dataframe read using the sqlite_waveforms_to_pandas
     function of pEEGy.
     The rows and columns of the output plot are specified by the factors of the dataframe.
```

### Comparing `peegy-1.3.7/peegy/io/synergy_reader.py` & `peegy-1.4.3/peegy/io/synergy_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/io/xml_tools.py` & `peegy-1.4.3/peegy/io/xml_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/layouts/KIT-160.lay` & `peegy-1.4.3/peegy/layouts/KIT-160.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/layouts/biosemi128.lay` & `peegy-1.4.3/peegy/layouts/biosemi128.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/layouts/biosemi16.lay` & `peegy-1.4.3/peegy/layouts/biosemi16.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/layouts/biosemi160.lay` & `peegy-1.4.3/peegy/layouts/biosemi160.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/layouts/biosemi256.lay` & `peegy-1.4.3/peegy/layouts/biosemi256.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/layouts/biosemi32.lay` & `peegy-1.4.3/peegy/layouts/biosemi32.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/layouts/biosemi32_2_EXT.lay` & `peegy-1.4.3/peegy/layouts/biosemi32_2_EXT.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/layouts/biosemi32_fnirs_MP.lay` & `peegy-1.4.3/peegy/layouts/biosemi32_fnirs_MP.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/layouts/biosemi32_fnirs_jaime.lay` & `peegy-1.4.3/peegy/layouts/biosemi32_fnirs_jaime.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/layouts/biosemi64.lay` & `peegy-1.4.3/peegy/layouts/biosemi64.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/layouts/biosemi64_2_EXT.lay` & `peegy-1.4.3/peegy/layouts/biosemi64_2_EXT.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/layouts/biosemi64_3_EXT.lay` & `peegy-1.4.3/peegy/layouts/biosemi64_3_EXT.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/layouts/emotive14.lay` & `peegy-1.4.3/peegy/layouts/emotive14.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/layouts/layouts.py` & `peegy-1.4.3/peegy/layouts/layouts.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/layouts/neuroscan64.lay` & `peegy-1.4.3/peegy/layouts/neuroscan64.lay`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/plot/eeg_ave_epochs_plot_tools.py` & `peegy-1.4.3/peegy/plot/eeg_ave_epochs_plot_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -986,17 +986,17 @@
                 gc.collect()
             else:
                 figures.append(fig)
     return figures
 
 
 def eeg_save_time_slice(data: np.array = np.array([]),
-                        fs: np.float = 0,
+                        fs: float = 0,
                         channels: np.array([EegChannel]) = np.array([EegChannel()]),
-                        time_length: np.float = 4.0,
+                        time_length: float = 4.0,
                         title: str = '',
                         file_name: str = ''):
     buffer_size = np.floor(np.minimum(time_length * fs, data.shape[0])).astype(int)
     fig, ax1 = plt.subplots()
     font = {'size': 6}
     plt.rc('font', **font)
     offset_vector = 10 * np.arange(data.shape[1])
@@ -1028,15 +1028,15 @@
     ax2.spines["right"].set_position(("axes", - 0.1))
     fig.savefig(file_name)
     plt.close(fig)
     gc.collect()
 
 
 def get_cdf(epochs_ave: DataNode = DataNode(),
-            x_val: np.float = None,
+            x_val: float = None,
             domain=Domain.time,
             **kwargs):
     idx_elec = np.where(np.array([ch.x for ch in epochs_ave.channels]))[0]
     # remove electrodes without a label
     if domain == Domain.time:
         potentials = epochs_ave.data[epochs_ave.time_to_samples(x_val), idx_elec]
     if domain == Domain.frequency:
```

### Comparing `peegy-1.3.7/peegy/plot/eeg_plot_tools.py` & `peegy-1.4.3/peegy/plot/eeg_plot_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/events/event_tools.py` & `peegy-1.4.3/peegy/processing/events/event_tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,21 +37,21 @@
 
 def join_triggers(all_triggers=np.array([])):
     """
     this function join two or more sets of triggers passed in a numpy array
     :param all_triggers: all_triggers: array of triggers
     :return: a new trigger with joined elements
     """
-    code = np.array([], dtype=np.int)
-    idx = np.array([], dtype=np.int)
+    code = np.array([], dtype=int)
+    idx = np.array([], dtype=int)
     dur = np.array([])
-    dur_samples = np.array([], dtype=np.int)
-    min_distance = np.array([], dtype=np.int)
-    max_distance = np.array([], dtype=np.int)
-    position = np.array([], dtype=np.int)
+    dur_samples = np.array([], dtype=int)
+    min_distance = np.array([], dtype=int)
+    max_distance = np.array([], dtype=int)
+    position = np.array([], dtype=int)
 
     for events in all_triggers:
         code = np.append(events['code'], code)
         idx = np.append(events['idx'], idx)
         dur = np.append(events['dur'], dur)
         dur_samples = np.append(events['dur_samples'], dur_samples)
         min_distance = np.append(events['min_distance'], min_distance)
```

### Comparing `peegy-1.3.7/peegy/processing/pipe/attach.py` & `peegy-1.4.3/peegy/processing/pipe/attach.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/pipe/definitions.py` & `peegy-1.4.3/peegy/processing/pipe/definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -285,23 +285,23 @@
         _min_time, _max_time = None, None
         if self.events.get_events_code(code=event_code).size:
             _n_events = self.events.get_events_code(code=event_code).size
             _min_time = self.events.get_events_time(code=event_code).min()
             _max_time = self.events.get_events_time(code=event_code).max()
         if n_events is None:
             n_events = _n_events
-        if min_time:
+        if min_time is not None:
             _min_time = min_time
 
         if max_time is not None:
             _max_time = max_time
 
-        if not _min_time:
+        if _min_time is None:
             _min_time = 0 * u.s
-        if not _max_time:
+        if _max_time is None:
             _max_time = self._data.shape[0] / self.fs
 
         if n_events:
             if epoch_length is None:
                 epoch_length = ((_max_time - _min_time) / n_events)
             new_event_times = np.sort(
                 _min_time + np.random.rand(n_events) * (_max_time - _min_time - epoch_length))
@@ -336,21 +336,67 @@
                  keep_input_node=True,
                  **kwargs):
         self.input_process: InputOutputProcess = input_process if input_process is not None else self  # Input data
         # must be InputOutputProcess class
         self.function_args: dict = kwargs
         self.input_node: DataNode = None
         self.output_node: DataNode = None
-        self.process_parameters: dict = kwargs  # dict with all the parameters used in process function
-        self.keep_input_node: bool = keep_input_node
-        self.figures: [plt.Figure] = None
-        self.name: str = None
-        self.ready = False
-        if self.name is None:
-            self.name = self.__class__.__name__
+        self._process_parameters: dict = kwargs  # dict with all the parameters used in process function
+        self._keep_input_node: bool = keep_input_node
+        self._figures: [plt.Figure] = None
+        self._name: str = None
+        self._ready = False
+        if self._name is None:
+            self._name = self.__class__.__name__
+        self._calling_parameters = None
+        self._figures_path = None
+        if 'calling_parameters' in kwargs.keys():
+            self._calling_parameters = kwargs['calling_parameters']
+
+    def get_process_parameters(self):
+        return self._process_parameters
+
+    def set_process_parameters(self, value):
+        self._process_parameters = value
+    process_parameters = property(get_process_parameters, set_process_parameters)
+
+    def get_keep_input_node(self):
+        return self._keep_input_node
+
+    def set_keep_input_node(self, value):
+        self._keep_input_node = value
+    keep_input_node = property(get_keep_input_node, set_keep_input_node)
+
+    def get_figures(self):
+        return self._figures
+
+    def set_figures(self, value):
+        self._figures = value
+    figures = property(get_figures, set_figures)
+
+    def get_figures_path(self):
+        return self._figures_path
+
+    def set_figures_path(self, value):
+        self._figures_path = value
+    figures_path = property(get_figures_path, set_figures_path)
+
+    def get_name(self):
+        return self._name
+
+    def set_name(self, value):
+        self._name = value
+    name = property(get_name, set_name)
+
+    def get_ready(self):
+        return self._ready
+
+    def set_ready(self, value):
+        self._ready = value
+    ready = property(get_ready, set_ready)
 
     def transform_data(self):
         return 'core method to generate output data'
 
     def run(self):
         self.input_node = self.input_process.output_node
         callable_list = [_i for _i in dir(DataNode) if callable(getattr(DataNode, _i))]
@@ -391,14 +437,23 @@
                                         )
         out = InputOutputQtFigure(figure=win)
         if interactive:
             win.show()
             pg.QtGui.QGuiApplication.instance().exec_()
         return out
 
+    def get_input_parameters(self):
+        all_input_variables = list(inspect.signature(self.__init__).parameters.keys())
+        # all_locals = self.__init__.__code__.co_varnames
+        # attributes = [a for a in dir(self.input_node) if not (a.startswith('__') or a.startswith('_')) and
+        #               a not in callable_list and a not in properties_list]
+        parameters = {key: self.__dict__[key] for key in all_input_variables if key in self.__dict__.keys()}
+
+        return parameters
+
 
 def plot_input_output_process(input_output_process: InputOutputProcess = None,
                               plot_input: bool = False,
                               plot_output: bool = True,
                               ch_to_plot: [str] = None,
                               de_mean=False):
     """
```

### Comparing `peegy-1.3.7/peegy/processing/pipe/detection.py` & `peegy-1.4.3/peegy/processing/pipe/detection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/pipe/epochs.py` & `peegy-1.4.3/peegy/processing/pipe/epochs.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     def __init__(self, input_process=InputOutputProcess,
                  pre_stimulus_interval: u.quantity.Quantity = None,
                  post_stimulus_interval: u.quantity.Quantity = None,
                  baseline_correction_ini_time: u.quantity.Quantity = None,
                  baseline_correction_end_time: u.quantity.Quantity = None,
                  event_code: float = None,
                  base_line_correction: bool = False,
+                 at: u.Quantity = None,
                  demean: bool = True,
                  events_mask: int = None,
                  **kwargs):
         """
         This class will take a n*m matrix into a k*m*p, where p (number of trials) is determined by the number of
         triggers used to split the data
         :param input_process: InputOutputProcess Class
@@ -44,14 +45,16 @@
         :param baseline_correction_ini_time: initial time (relative to trigger) to compute the mean for baseline
         correction. For example, if trigger is at zero, and you want to compute the baseline correction from -200 ms you
         can set baseline_correction_ini_time = -200 * u.ms
         :param baseline_correction_end_time: end time (relative to trigger) to compute the mean for baseline
         correction. For example, if trigger is at zero, and you want to compute the baseline correction
         between -200 * ms and -50 ms, you can set baseline_correction_ini_time = -200 * u.ms and
         baseline_correction_end_time = -50 * u.ms
+        :param at: an array of with times to use as event marks. When at is not empty, these time stamps will be used
+        to epoch the data. Event codes from the input_process will be ignored.
         :param demean: whether to remove the mean from each epoch
         :param events_mask: integer value used to masker triggers codes. This is useful to ignore triggers inputs above
         a particular value. For example, if only the first 8 trigger inputs were used (max decimal value is 255), in a
         system with 16 trigger inputs, then the masker could be set to 255 to ignore any trigger from trigger inputs 9
         to 16
         :param kwargs: extra parameters to be passed to the superclass
         """
@@ -60,50 +63,57 @@
         self.post_stimulus_interval = set_default_unit(post_stimulus_interval, u.s)
         self.event_code = event_code
         self.base_line_correction = base_line_correction
         self.demean = demean
         self.events_mask = events_mask
         self.baseline_correction_ini_time = baseline_correction_ini_time
         self.baseline_correction_end_time = baseline_correction_end_time
+        self.at = at
 
     def transform_data(self):
         if self.event_code is None:
             print('no event code was provided')
             return
         data = self.input_node.data
         baseline_correction_ini_time = 0.0 * u.s if self.baseline_correction_ini_time is None else \
             self.baseline_correction_ini_time
         pre_stimulus_interval = 0.0 * u.s if self.pre_stimulus_interval is None else self.pre_stimulus_interval
         self.input_node.events.mask = self.events_mask
-        events_index = self.input_node.events.get_events_index(code=self.event_code,
-                                                               fs=self.input_node.fs)
+        if self.at is None:
+            events_index = self.input_node.events.get_events_index(code=self.event_code,
+                                                                   fs=self.input_node.fs)
+        else:
+            events_index = self.input_node.x_to_samples(self.at)
         post_stimulus_interval = self.post_stimulus_interval
         baseline_correction_end_time = 0.0 * u.s if self.baseline_correction_end_time is None else \
             self.baseline_correction_end_time
         if self.post_stimulus_interval is None:
             post_stimulus_interval = np.percentile(np.diff(events_index), 90) / self.input_node.fs
 
         # ensure sufficient data for baseline-correction
         if baseline_correction_ini_time < 0:
             pre_stimulus_interval = np.maximum(pre_stimulus_interval, np.abs(baseline_correction_ini_time))
         if baseline_correction_end_time > 0:
             post_stimulus_interval = np.maximum(post_stimulus_interval, baseline_correction_end_time)
 
-        buffer_size = np.int((post_stimulus_interval + pre_stimulus_interval) * self.input_node.fs)
+        buffer_size = int((post_stimulus_interval + pre_stimulus_interval) * self.input_node.fs)
         events_index = events_index - int((pre_stimulus_interval - self.input_node.x_offset) * self.input_node.fs)
-        events_index = events_index[events_index >= 0]
+        total_indexes = events_index.size
+        # ensure positive index
+        _idx_to_keep = np.logical_and(events_index >= 0,
+                                      events_index + buffer_size <= self.input_node.data.shape[0])
+        events_index = events_index[_idx_to_keep]
+        possible_indexes = events_index.size
+        if possible_indexes < total_indexes:
+            print("{:} events ignored as data length won't fit epoch length".format(
+                total_indexes - possible_indexes))
         epochs = np.zeros((buffer_size, self.input_node.data.shape[1], events_index.size), dtype=np.float32)
         print('There are {:} events with code {:}'.format(events_index.shape[0], self.event_code))
-        for i, _event in enumerate(tqdm(events_index, desc='Epoching data')):
+        for i, _event in enumerate(tqdm(events_index, desc='Epoching data', miniters=0)):
             # ensure that blocks match buffer size
-            if _event + buffer_size > self.input_node.data.shape[0]:
-                epochs = epochs[:, :, list(range(i))]
-                print("{:} events ignored as data length won't fit epoch length".format(
-                    events_index.shape[0] - i))
-                break
             epochs[:, :, i] = data[_event:_event + buffer_size, :]
         epochs = epochs * data.unit
         print('A total of {:} epochs were obtained using event code {:}, each with a duration of {:.3f}'.format(
             epochs.shape[2],
             self.event_code,
             (buffer_size / self.input_node.fs).to(u.s)))
         if self.demean:
@@ -169,15 +179,15 @@
             _idx_to_keep = np.logical_and(_idx_to_keep, np.all(to_keep, axis=0).flatten())
             print('{:} epochs out of {:} will be kept based on a {:} percentage rejection'.format(
                 np.all(to_keep, axis=0).sum(),
                 _data.shape[2],
                 self.rejection_percentage))
 
         if self.rejection_threshold is not None:
-            # now we find epochs indexes across channels which are avove threshold
+            # now we find epochs indexes across channels which are above threshold
             _max_amp = np.max(np.abs(_data), axis=0)
             to_keep = _max_amp <= self.rejection_threshold
             _idx_to_keep = np.logical_and(_idx_to_keep, np.all(to_keep, axis=0).flatten())
             print('{:} epochs out of {:} will be kept based on a {:} rejection threshold'.format(
                 np.all(to_keep, axis=0).sum(),
                 _data.shape[2],
                 self.rejection_threshold))
@@ -196,16 +206,16 @@
             _idx_to_keep = np.logical_and(_idx_to_keep, np.all(to_keep, axis=0).flatten())
             print('Rejecting a total of {:} epochs, corresponding to {:.2f}% above {:} std'.format(
                 np.sum(~_idx_to_keep), _std_percentage, self.std_threshold))
         # print some information and reject epochs
         _p_rejected = 100 * (1 - np.sum(_idx_to_keep) / _data.shape[2])
         print('Percentage of total epochs rejected {:.2f}%'.format(_p_rejected))
         if _p_rejected == 100:
-            raise Exception('All epochs were rejected!! check rejection level '
-                            '(currently {:}) and run again'.format(self.rejection_percentage))
+            print('All epochs were rejected!! check rejection level '
+                  '(currently {:}) and run again'.format(self.rejection_percentage))
 
         self.output_node.data = _data[:, :, _idx_to_keep.flatten()]
 
 
 class RemoveBadChannelsEpochsBased(InputOutputProcess):
     def __init__(self, input_process=InputOutputProcess,
                  threshold: float = 300.0,
```

### Comparing `peegy-1.3.7/peegy/processing/pipe/general.py` & `peegy-1.4.3/peegy/processing/pipe/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,19 +328,19 @@
             data = self.input_node.data
         step_size = np.maximum(int(self.interval * self.input_node.fs), 1)
         _samples = np.arange(0, self.input_node.data.shape[0], step_size).astype(int)
         sub_data = data[_samples, :]
         # compute dc component
         _dc_component = np.mean(np.abs(sub_data), axis=0)
         bad_channels = np.where(_dc_component > self.amp_thr)[0]
-        _others_idx = np.array([idx for idx in np.arange(sub_data.shape[1]) if idx not in bad_channels], dtype=np.int)
+        _others_idx = np.array([idx for idx in np.arange(sub_data.shape[1]) if idx not in bad_channels], dtype=int)
         a_std = np.std(sub_data[:, _others_idx], axis=0)
         thr_ci = self.thr_sd * np.std(a_std) + np.mean(a_std)
         n_ch_idx = np.where(a_std > thr_ci)[0]
-        bad_idx = _others_idx[n_ch_idx] if n_ch_idx.size else np.array([], dtype=np.int)
+        bad_idx = _others_idx[n_ch_idx] if n_ch_idx.size else np.array([], dtype=int)
         bad_channels = np.concatenate((bad_channels, bad_idx))
         _bad_channels_index = np.unique(bad_channels)
         self.output_node.data = self.input_node.data.copy()
         self.output_node.delete_channel_by_idx(_bad_channels_index)
 
 
 class RemoveBadChannels(InputOutputProcess):
@@ -601,13 +601,15 @@
         _epoch_samples = evoked_response.output_node.data.shape[0]
         evoked_data = evoked_response.output_node.data
         if self.fade_in_out:
             fade_window = fade_in_out_window(n_samples=_epoch_samples,
                                              fraction=0.05)
             evoked_data = evoked_data * fade_window
 
-        for _events in self.input_node.events.get_events_index(self.event_code, fs=self.input_node.fs):
-            _ini = _events
-            _end = np.minimum(_events + _epoch_samples, data.shape[0])
-            _er = evoked_data[0: _end - _ini, :]
-            data[_ini: _end, :] = data[_ini: _end, :] - _er
+        for _event_idx in self.input_node.events.get_events_index(self.event_code, fs=self.input_node.fs):
+            _ini = _event_idx
+            _end = np.minimum(_event_idx + _epoch_samples, data.shape[0])
+            _b_size = _end - _ini
+            if _b_size > 0:
+                _er = evoked_data[0: _end - _ini, :]
+                data[_ini: _end, :] = data[_ini: _end, :] - _er
         self.output_node.data = data
```

### Comparing `peegy-1.3.7/peegy/processing/pipe/interpolation.py` & `peegy-1.4.3/peegy/processing/pipe/interpolation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/pipe/io.py` & `peegy-1.4.3/peegy/processing/pipe/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,30 +208,30 @@
         """
         super(GenericInputData, self).__init__()
         self.data = set_default_unit(copy.copy(data), u.uV)
         self.fs = set_default_unit(fs, u.Hz)
         self.event_times = set_default_unit(event_times, u.s)
         self.event_code = event_code
         self.output_node = None
-        figures_path = figures_path if figures_path is not None else str(Path.home()) + '{:}'.format(sep +
-                                                                                                     'peegy' +
-                                                                                                     sep +
-                                                                                                     'test' +
-                                                                                                     sep +
-                                                                                                     'figures')
+        self.figures_path = figures_path if figures_path is not None else str(Path.home()) + '{:}'.format(sep +
+                                                                                                          'peegy' +
+                                                                                                          sep +
+                                                                                                          'test' +
+                                                                                                          sep +
+                                                                                                          'figures')
         self.figures_subset_folder = figures_subset_folder
 
         _ch = []
         n_channels = self.data.shape[1]
         [_ch.append(ChannelItem(label='CH_{:}'.format(i), idx=i)) for i in range(n_channels)]
         layout = np.array(_ch)
         self.input_node = DataNode(fs=fs,
                                    domain=Domain.time,
                                    layout=layout,
-                                   paths=DirectoryPaths(file_path=figures_path,
+                                   paths=DirectoryPaths(file_path=self.figures_path,
                                                         delete_all=False,
                                                         delete_figures=False,
                                                         figures_subset_folder=figures_subset_folder)
                                    )
 
     def run(self):
         events = np.array([])
```

### Comparing `peegy-1.3.7/peegy/processing/pipe/pipeline.py` & `peegy-1.4.3/peegy/processing/pipe/pipeline.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/pipe/plot.py` & `peegy-1.4.3/peegy/processing/pipe/plot.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/pipe/regression.py` & `peegy-1.4.3/peegy/processing/pipe/regression.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/pipe/simulate.py` & `peegy-1.4.3/peegy/processing/pipe/simulate.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/pipe/spatial_filtering.py` & `peegy-1.4.3/peegy/processing/pipe/spatial_filtering.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/pipe/statistics.py` & `peegy-1.4.3/peegy/processing/pipe/statistics.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/pipe/storage.py` & `peegy-1.4.3/peegy/processing/pipe/storage.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/pipe/time_frequency.py` & `peegy-1.4.3/peegy/processing/pipe/time_frequency.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/statistics/definitions.py` & `peegy-1.4.3/peegy/processing/statistics/definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/statistics/eeg_statistic_tools.py` & `peegy-1.4.3/peegy/processing/statistics/eeg_statistic_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     return f_value, f_critic, df_num, df_den, p_value
 
 
 def phase_locking_value(
         data: np.array = None,
         alpha: float = 0.05,
         weights: np.array = None,
-        eps: np.float = np.finfo(float).eps) -> np.array:
+        eps: float = np.finfo(float).eps) -> np.array:
     """
     Compute phase-locking value (PLV) using Rayleigh test
     :param data: time x channels x trials numpy array in the time domain
     :param alpha: float indicating the alpha value for significance
     :param weights: trial by trial weights
     :param eps: machine numerical precision used to prevent dividing by zero
     :return: phase-locking value (frequency x channels), z-scores (frequency x channels), z_critic (float), p_values
```

### Comparing `peegy-1.3.7/peegy/processing/system/progress.py` & `peegy-1.4.3/peegy/processing/system/progress.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from tqdm.auto import tqdm
 from joblib import Parallel
 
 
 class ParallelTqdm(Parallel):
-    def __init__(self, use_tqdm=True, total=None, desc='', *args, **kwargs):
+    def __init__(self,
+                 use_tqdm=True,
+                 total=None,
+                 desc='',
+                 colour='blue',
+                 *args, **kwargs):
         self._use_tqdm = use_tqdm
         self._total = total
         self._desc = desc
+        self._colour = colour
         super().__init__(*args, **kwargs)
 
     def __call__(self, *args, **kwargs):
         with tqdm(disable=not self._use_tqdm,
                   total=self._total,
-                  desc=self._desc) as self._pbar:
+                  desc=self._desc,
+                  colour=self._colour) as self._pbar:
             return Parallel.__call__(self, *args, **kwargs)
 
     def print_progress(self):
         if self._total is None:
             self._pbar.total = self.n_dispatched_tasks
         self._pbar.n = self.n_completed_tasks
         self._pbar.refresh()
```

### Comparing `peegy-1.3.7/peegy/processing/tools/detection/definitions.py` & `peegy-1.4.3/peegy/processing/tools/detection/definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/tools/detection/time_domain_tools.py` & `peegy-1.4.3/peegy/processing/tools/detection/time_domain_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/tools/eeg_epoch_operators.py` & `peegy-1.4.3/peegy/processing/tools/eeg_epoch_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         x = x[:, :, None]
     if np.mod(x.shape[0], 2) == 0:
         fft_size = int((x.shape[0] / 2) + 1)
     else:
         fft_size = int((x.shape[0] + 1) / 2)
 
     freq = np.arange(fft_size) / float(x.shape[0])
-    freq_filt = np.zeros(shape=(fft_size, 1), dtype=np.float)
+    freq_filt = np.zeros(shape=(fft_size, 1), dtype=float)
     for f_bin in et_find_freq_bin(freq, normalized_frequencies):
         freq_filt[f_bin] = 1.0
 
     c = 0
     tw = 0
     for i in np.arange(x.shape[2]):
         yy = et_multi_shift(y[:, :, i], shifts)
@@ -287,15 +287,15 @@
         x = x[:, :, None]
     if np.mod(x.shape[0], 2) == 0:
         fft_size = int((x.shape[0] / 2) + 1)
     else:
         fft_size = int((x.shape[0] + 1) / 2)
 
     freq = np.arange(fft_size) / (float(x.shape[0]))
-    freq_filt = np.zeros(shape=(fft_size, 1), dtype=np.float)
+    freq_filt = np.zeros(shape=(fft_size, 1), dtype=float)
     for f_bin in et_find_freq_bin(freq, normalized_frequencies):
         freq_filt[f_bin] = 1.0
     if w.size == 0:
         w = np.ones(x.shape)
         # w = w / np.sum(w, axis=2, keepdims=True)
     # normalize weights
     # w = w / np.sum(w ** 2, axis=2, keepdims=True)
```

### Comparing `peegy-1.3.7/peegy/processing/tools/epochs_processing_tools.py` & `peegy-1.4.3/peegy/processing/tools/epochs_processing_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/tools/filters/eegFiltering.py` & `peegy-1.4.3/peegy/processing/tools/filters/eegFiltering.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,16 +74,16 @@
 
     if not n_jobs:
         n_jobs = np.maximum(multiprocessing.cpu_count(), 1)
     else:
         n_jobs = np.minimum(multiprocessing.cpu_count(), n_jobs)
     if not ch_per_block:
         _virtual_memory = psu.virtual_memory()
-        ch_per_block = np.maximum(1, np.int(_virtual_memory.available /
-                                            (data.nbytes / data.shape[1]) * 0.1))
+        ch_per_block = np.maximum(1, int(_virtual_memory.available /
+                                         (data.nbytes / data.shape[1]) * 0.1))
     ch_per_block = np.minimum(data.shape[1], ch_per_block)
     print(('filtering ' + str(ch_per_block) + ' channels per block'))
 
     for _bl in np.arange((np.ceil(data.shape[1]) / ch_per_block)):
         p = []
         pos_ini = int(_bl * ch_per_block)
         pos_end = int(np.minimum((_bl + 1) * ch_per_block, data.shape[1]))
@@ -148,16 +148,16 @@
 
     if not n_jobs:
         n_jobs = np.maximum(multiprocessing.cpu_count(), 1)
     else:
         n_jobs = np.minimum(multiprocessing.cpu_count(), n_jobs)
     if not ch_per_block:
         _virtual_memory = psu.virtual_memory()
-        ch_per_block = np.maximum(1, np.int(_virtual_memory.available /
-                                            (data.nbytes / data.shape[1]) * 0.1))
+        ch_per_block = np.maximum(1, int(_virtual_memory.available /
+                                         (data.nbytes / data.shape[1]) * 0.1))
     ch_per_block = np.minimum(data.shape[1], ch_per_block)
     print(('filtering ' + str(ch_per_block) + ' channels per block'))
 
     for _bl in tqdm(np.arange((np.ceil(data.shape[1]) / ch_per_block)), desc='Filter'):
         p = []
         pos_ini = int(_bl * ch_per_block)
         pos_end = int(np.minimum((_bl + 1) * ch_per_block, data.shape[1]))
```

### Comparing `peegy-1.3.7/peegy/processing/tools/filters/eog_tools/tools.py` & `peegy-1.4.3/peegy/processing/tools/filters/eog_tools/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 def crest_factor(x: np.array = None):
     return 20.0 * np.log10(np.max(np.abs(x)) / rms(x))
 
 
 def unitary_step(x: np.array = None):
-    return (x > 0).astype(np.float)
+    return (x > 0).astype(float)
 
 
 def generate_eog_template(eog_data: np.array = None,
                           fs: u.Quantity = None,
                           template_width: u.Quantity = 0.5 * u.s,
                           low_pass: u.Quantity = 20 * u.Hz,
                           crest_factor_threshold=10,
```

### Comparing `peegy-1.3.7/peegy/processing/tools/filters/resampling.py` & `peegy-1.4.3/peegy/processing/tools/filters/resampling.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/tools/filters/spatial_filtering/definitions.py` & `peegy-1.4.3/peegy/processing/tools/filters/spatial_filtering/definitions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py` & `peegy-1.4.3/peegy/processing/tools/filters/spatial_filtering/spatial_filtering.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py` & `peegy-1.4.3/peegy/processing/tools/multiprocessing/multiprocessesing_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     filtered_data = data
     if not n_jobs:
         n_jobs = np.maximum(joblib.cpu_count(), 1)
     else:
         n_jobs = np.minimum(joblib.cpu_count(), n_jobs)
     if not ch_per_block:
         _virtual_memory = psu.virtual_memory()
-        ch_per_block = np.maximum(1, np.int(_virtual_memory.available /
-                                            (filtered_data.nbytes / filtered_data.shape[1]) * 0.1))
+        ch_per_block = np.maximum(1, int(_virtual_memory.available /
+                                         (filtered_data.nbytes / filtered_data.shape[1]) * 0.1))
     ch_per_block = np.minimum(filtered_data.shape[1], ch_per_block)
     # print('filtering {:} channels per block'.format(ch_per_block))
     padding_size = ((0, b.size - 1), *((0, 0),) * (filtered_data.ndim - 1))
     padding_value = (((0, 0),) * filtered_data.ndim)
     filtered_data = np.pad(filtered_data, padding_size,
                            'constant',
                            constant_values=padding_value)
@@ -65,15 +65,15 @@
         sub_pos_ini = []
         sub_pos_end = []
         for _t in range(_n_jobs):
             sub_pos_ini.append(int(pos_ini + _ch_per_thread * _t))
             sub_pos_end.append(int(np.minimum(pos_end, pos_ini + _ch_per_thread * (_t + 1))))
 
         ParallelTqdm(total=_n_jobs,
-                     desc='Parallel filtering',
+                     desc='Parallel filtering/worker',
                      n_jobs=_n_jobs,
                      mmap_mode='w+',
                      backend='threading')(
             joblib.delayed(filt_worker_ovs)(filtered_data, sub_pos_ini[_i], sub_pos_end[_i], b) for
             _i in range(_n_jobs))
         # print('Filtered channels: {:} to {:}'.format(pos_ini, pos_end - 1))
 
@@ -105,16 +105,16 @@
     filtered_data = data
     if not n_jobs:
         n_jobs = np.maximum(joblib.cpu_count(), 1)
     else:
         n_jobs = np.minimum(joblib.cpu_count(), n_jobs)
     if not ch_per_block:
         _virtual_memory = psu.virtual_memory()
-        ch_per_block = np.maximum(1, np.int(_virtual_memory.available /
-                                            (filtered_data.nbytes / filtered_data.shape[1]) * 0.1))
+        ch_per_block = np.maximum(1, int(_virtual_memory.available /
+                                         (filtered_data.nbytes / filtered_data.shape[1]) * 0.1))
     ch_per_block = np.minimum(filtered_data.shape[1], ch_per_block)
     print('filtering {:} channels per block'.format(ch_per_block))
 
     for _bl in np.arange((np.ceil(filtered_data.shape[1]) / ch_per_block)):
         pos_ini = int(_bl * ch_per_block)
         pos_end = int(np.minimum((_bl + 1) * ch_per_block, filtered_data.shape[1]))
         _b_size = pos_end - pos_ini
```

### Comparing `peegy-1.3.7/peegy/processing/tools/template_generator/auditory_waveforms.py` & `peegy-1.4.3/peegy/processing/tools/template_generator/auditory_waveforms.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/tools/template_generator/h0.json` & `peegy-1.4.3/peegy/processing/tools/template_generator/h0.json`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/tools/video/recording.py` & `peegy-1.4.3/peegy/processing/tools/video/recording.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/processing/tools/weightedAverage.py` & `peegy-1.4.3/peegy/processing/tools/weightedAverage.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         self._filter_hp = np.array([])
         self._filter_lp = np.array([])
         self._self_win_size = 0
         self.__w_average = np.array([])
         self.__s_average = np.array([])
         self._fft = np.array([], dtype=np.complex128)
         self._fft_frequencies = np.array([])
-        self._frequency_bin = np.array([], dtype=np.int)
+        self._frequency_bin = np.array([], dtype=int)
         self._tracked_frequency_bin = []
         self._block_ave = np.array([])
         self._ave_under_noise_source = np.array([])
         self._block_ave_sweep_count = np.array([])
         self._ave_under_noise_source_sweep_count = np.array([])
         self._split_index = 0
         self._s_snr = np.array([])
@@ -863,15 +863,15 @@
             self.axis[n_col] = win.addPlot(row=1, col=n_col)
             self.axis[n_col].addLegend()
             if n_col == 0:
                 self.axis[n_col].setLabel('bottom', "Time [ms]")
                 self.axis[n_col].setLabel('left', "Amplitude")
                 self.axis[n_col].setXRange(self.time[0] * 1000, self.time[-1] * 1000)
                 [self.axis[n_col].addItem(pg.InfiniteLine(_pos)) for _pos in self._analysis_window * 1000.]
-                dammy_data = np.zeros((self.time.size, self.splits), dtype=np.float)
+                dammy_data = np.zeros((self.time.size, self.splits), dtype=float)
 
                 for _i in range(self.splits):
                     name_legend = 'S_ave' if _i == 0 else None
                     self._time_curves_s.append(self.axis[n_col].plot(self.time, dammy_data[:, _i] -
                                                                      _i * self.channels_offset,
                                                                      pen=pg.intColor(0, 2), name=name_legend))
 
@@ -881,15 +881,15 @@
                     self.axis[n_col].addItem(text_item)
                     name_legend = 'W_ave' if _i == 0 else None
                     self._time_curves_w.append(self.axis[n_col].plot(self.time, dammy_data[:, _i] -
                                                                      _i * self.channels_offset,
                                                                      pen=pg.intColor(1, 2), name=name_legend))
             if n_col == 1:
                 for _i in range(self.splits):
-                    dammy_data = np.zeros((self._fft_frequencies.size, self.splits), dtype=np.float)
+                    dammy_data = np.zeros((self._fft_frequencies.size, self.splits), dtype=float)
                     name_legend = 'S_ave' if _i == 0 else None
                     self._freq_curves_s.append(self.axis[n_col].plot(self._fft_frequencies, dammy_data[:, _i] -
                                                                      _i * self.channels_offset,
                                                                      pen=pg.intColor(0, 2), name=name_legend))
                     name_legend = 'W_ave' if _i == 0 else None
                     self._freq_curves_w.append(self.axis[n_col].plot(self._fft_frequencies, dammy_data[:, _i] -
                                                                      _i * self.channels_offset,
```

### Comparing `peegy-1.3.7/peegy/test/artifact_removal/ir_test.py` & `peegy-1.4.3/peegy/test/artifact_removal/ir_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/artifact_removal/regression_artifact_removal.py` & `peegy-1.4.3/peegy/test/artifact_removal/regression_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/artifact_removal/xcorr_artifact_removal.py` & `peegy-1.4.3/peegy/test/artifact_removal/xcorr_artifact_removal.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/dss_unit_tests.py` & `peegy-1.4.3/peegy/test/dss_unit_tests.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/eeg_test_resampling.py` & `peegy-1.4.3/peegy/test/eeg_test_resampling.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/javerager_test.py` & `peegy-1.4.3/peegy/test/javerager_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/read_data_test.py` & `peegy-1.4.3/peegy/test/read_data_test.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_assr_moving_average.py` & `peegy-1.4.3/peegy/test/test_assr_moving_average.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_average_spectrogram_power.py` & `peegy-1.4.3/peegy/test/test_average_spectrogram_power.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_biosemi_class.py` & `peegy-1.4.3/peegy/test/test_biosemi_class.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_biosemi_reader.py` & `peegy-1.4.3/peegy/test/test_biosemi_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_bootstraping.py` & `peegy-1.4.3/peegy/test/test_bootstraping.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_edf_reader.py` & `peegy-1.4.3/peegy/test/test_edf_reader.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_eeg_notch_filter.py` & `peegy-1.4.3/peegy/test/test_eeg_notch_filter.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_eog_removal_correlation.py` & `peegy-1.4.3/peegy/test/test_eog_removal_correlation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_eog_template_removal.py` & `peegy-1.4.3/peegy/test/test_eog_template_removal.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import astropy.units as u
 import matplotlib
 if 'Qt5Agg' in matplotlib.rcsetup.all_backends:
     matplotlib.use('Qt5Agg')
 
 
 def unitary_step(x: np.array = None):
-    return (x > 0).astype(np.float)
+    return (x > 0).astype(float)
 
 
 np.random.seed(7123)
 n_ch = 10
 fs = 16384.0 * u.Hz
 recording_time = 180
 eog_rate = 1 / 4 * u.Hz
```

### Comparing `peegy-1.3.7/peegy/test/test_eog_template_valderrama_20118.py` & `peegy-1.4.3/peegy/test/test_eog_template_valderrama_20118.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_et_tools.py` & `peegy-1.4.3/peegy/test/test_et_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_filter.py` & `peegy-1.4.3/peegy/test/test_filter.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_fir_filter_mt.py` & `peegy-1.4.3/peegy/test/test_fir_filter_mt.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_fir_filter_ols.py` & `peegy-1.4.3/peegy/test/test_fir_filter_ols.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_fiter_mt.py` & `peegy-1.4.3/peegy/test/test_fiter_mt.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_freq_noise_estimation.py` & `peegy-1.4.3/peegy/test/test_freq_noise_estimation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_freq_noise_estimation_plots.py` & `peegy-1.4.3/peegy/test/test_freq_noise_estimation_plots.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_frequency_average_epochs.py` & `peegy-1.4.3/peegy/test/test_frequency_average_epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_hotelling_t2.py` & `peegy-1.4.3/peegy/test/test_hotelling_t2.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_ica_average_epochs.py` & `peegy-1.4.3/peegy/test/test_ica_average_epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_multiprocessing.py` & `peegy-1.4.3/peegy/test/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_noise_generator.py` & `peegy-1.4.3/peegy/test/test_noise_generator.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_norm_corr.py` & `peegy-1.4.3/peegy/test/test_norm_corr.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_peakdetection.py` & `peegy-1.4.3/peegy/test/test_peakdetection.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_phase_locking_value.py` & `peegy-1.4.3/peegy/test/test_phase_locking_value.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_pooled_freq_noise_estimation.py` & `peegy-1.4.3/peegy/test/test_pooled_freq_noise_estimation.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_scrolling.py` & `peegy-1.4.3/peegy/test/test_scrolling.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_spatial_filtering_example1.py` & `peegy-1.4.3/peegy/test/test_spatial_filtering_example1.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_spatial_filtering_example6.py` & `peegy-1.4.3/peegy/test/test_spatial_filtering_example6.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_spatial_filtering_freq_domain.py` & `peegy-1.4.3/peegy/test/test_spatial_filtering_freq_domain.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_spatial_filtering_freq_domain_2.py` & `peegy-1.4.3/peegy/test/test_spatial_filtering_freq_domain_2.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/test/test_w_average_epochs.py` & `peegy-1.4.3/peegy/test/test_w_average_epochs.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/tools/signal_generator/noise_functions.py` & `peegy-1.4.3/peegy/tools/signal_generator/noise_functions.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/peegy/tools/units/unit_tools.py` & `peegy-1.4.3/peegy/tools/units/unit_tools.py`

 * *Files identical despite different names*

### Comparing `peegy-1.3.7/setup.py` & `peegy-1.4.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 import os
+from importlib.metadata import version
+__version__ = version(__package__)
 
 
 def run_setup():
     _folder = os.path.dirname(os.path.realpath(__file__))
     requirement_path = _folder + os.path.sep + 'requirements.txt'
     install_requires = []
     if os.path.isfile(requirement_path):
         with open(requirement_path) as f:
             install_requires = f.read().splitlines()
-    version = open('VERSION').read()
     setup(name="peegy",
           install_requires=install_requires,
           setup_requires=['gitpython'],
-          version=version,
+          version=__version__,
           packages=find_packages(),
           author="Jaime A. Undurraga",
           author_email="jaime.undurraga@gmail.com",
           description="Tools to pipeline bulk analyses of EEG and other modalities.",
           long_description="""
           Set of tools for processing EEG data data using bdf/edf file format. These can be extended to other modalities
-          too. The overall goal is to produce processing pipelines to process many data in a systematic and reproducible 
-          way. This package includes several statistical, visualization, and output tools to generate consistent SQLITE
+          too. The overall goal is to produce easy processing pipelines to perform batch data analyses in a systematic 
+          and reproducible manner. 
+          This package includes several statistical, visualization, and output tools to generate consistent SQLITE
           databases. 
           """,
           license="MIT",
           url="https://jundurraga.gitlab.io/peegy/",
 
           package_data={'': ['*.lay', '*.json']},
           include_package_data=True,
           classifiers=[
               'Development Status :: 3 - Alpha',
               'Environment :: Console',
               'Intended Audience :: Science/Research',
-              'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+              'License :: OSI Approved :: MIT License',
               'Operating System :: MacOS :: MacOS X',
               'Operating System :: Microsoft :: Windows :: Windows 10',
               'Operating System :: POSIX :: Linux',
               'Programming Language :: Python :: 3',
               'Topic :: Scientific/Engineering :: Bio-Informatics'
               ]
           )
-    update_git_hash_version()
+    # update_git_hash_version()
 
 
 def update_git_hash_version():
     """Return version with local version identifier."""
     import git
     repo = git.Repo(search_parent_directories=True)
     sha = repo.head.object.hexsha
```

