# Comparing `tmp/pygama-1.2.0.tar.gz` & `tmp/pygama-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygama-1.2.0.tar", last modified: Fri Jan 20 09:57:57 2023, max compression
+gzip compressed data, was "pygama-1.3.0.tar", last modified: Sun May  7 09:40:56 2023, max compression
```

## Comparing `pygama-1.2.0.tar` & `pygama-1.3.0.tar`

### file list

```diff
@@ -1,220 +1,255 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.056035 pygama-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-20 09:57:45.000000 pygama-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-01-20 09:57:57.056035 pygama-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-01-20 09:57:45.000000 pygama-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-01-20 09:57:45.000000 pygama-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-01-20 09:57:57.056035 pygama-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-20 09:57:45.000000 pygama-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.032035 pygama-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.036035 pygama-1.2.0/src/pygama/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-20 09:57:56.000000 pygama-1.2.0/src/pygama/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.036035 pygama-1.2.0/src/pygama/dsp/
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7632 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/build_dsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    71045 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processing_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.040035 pygama-1.2.0/src/pygama/dsp/processors/
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/bl_subtract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/dplms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/dwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/fftw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/fixed_time_pickoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/gaussian_filter1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/get_multi_local_extrema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/linear_slope_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/log_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/min_max.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/moving_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/multi_a_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/multi_t_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/param_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/peak_snr_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/pole_zero.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/presum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/pulse_injector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/saturation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/soft_pileup_corr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/time_over_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/time_point_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/trap_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/upsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/wiener_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/processors/windower.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/dsp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.040035 pygama-1.2.0/src/pygama/evt/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/evt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/evt/build_tcm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/evt/tcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.040035 pygama-1.2.0/src/pygama/flow/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52599 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/flow/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11011 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/flow/datagroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    20266 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/flow/file_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.040035 pygama-1.2.0/src/pygama/hit/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/hit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/hit/build_hit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.044035 pygama-1.2.0/src/pygama/lgdo/
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/lgdo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/lgdo/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/lgdo/arrayofequalsizedarrays.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/lgdo/fixedsizearray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/lgdo/lgdo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/lgdo/lgdo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    51176 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/lgdo/lh5_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/lgdo/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/lgdo/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/lgdo/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/lgdo/vectorofvectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/lgdo/waveform_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.044035 pygama-1.2.0/src/pygama/math/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/math/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    38829 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/math/peak_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/math/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/math/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.044035 pygama-1.2.0/src/pygama/pargen/
--rw-r--r--   0 runner    (1001) docker     (123)    46009 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/pargen/AoE_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/pargen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/pargen/cuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/pargen/data_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/pargen/dsp_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    26769 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/pargen/ecal_th.py
--rw-r--r--   0 runner    (1001) docker     (123)    52601 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/pargen/energy_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)    71568 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/pargen/energy_optimisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/pargen/extract_tau.py
--rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/pargen/mse_psd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.048035 pygama-1.2.0/src/pygama/raw/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.048035 pygama-1.2.0/src/pygama/raw/buffer_processor/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/buffer_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/buffer_processor/buffer_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/buffer_processor/lh5_buffer_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9157 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/build_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/data_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/data_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.048035 pygama-1.2.0/src/pygama/raw/fc/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/fc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/fc/fc_config_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/fc/fc_event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/fc/fc_status_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/fc/fc_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.048035 pygama-1.2.0/src/pygama/raw/orca/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/orca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/orca/orca_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21484 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/orca/orca_digitizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/orca/orca_flashcam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/orca/orca_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/orca/orca_header_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/orca/orca_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/orca/orca_run_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/orca/orca_streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17574 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/raw/raw_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.048035 pygama-1.2.0/src/pygama/vis/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/vis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.048035 pygama-1.2.0/src/pygama/vis/mpl/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/vis/mpl/clint.mpl
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/vis/mpl/root.mpl
--rw-r--r--   0 runner    (1001) docker     (123)    22354 2023-01-20 09:57:45.000000 pygama-1.2.0/src/pygama/vis/waveform_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.036035 pygama-1.2.0/src/pygama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-01-20 09:57:56.000000 pygama-1.2.0/src/pygama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-01-20 09:57:57.000000 pygama-1.2.0/src/pygama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 09:57:56.000000 pygama-1.2.0/src/pygama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-20 09:57:56.000000 pygama-1.2.0/src/pygama.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 09:57:56.000000 pygama-1.2.0/src/pygama.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-01-20 09:57:56.000000 pygama-1.2.0/src/pygama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-20 09:57:56.000000 pygama-1.2.0/src/pygama.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.048035 pygama-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.048035 pygama-1.2.0/tests/dsp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.048035 pygama-1.2.0/tests/dsp/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/dsp/configs/icpc-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/dsp/configs/numpy-parsing.json
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/dsp/configs/sipm-dplms-config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/dsp/configs/sipm-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/dsp/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.052035 pygama-1.2.0/tests/dsp/processors/
--rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/dsp/processors/dplms_noise_mat.dat
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/dsp/processors/test_dplms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/dsp/processors/test_dwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/dsp/processors/test_fixed_time_pickoff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/dsp/processors/test_get_multi_local_extrema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/dsp/processors/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/dsp/test_build_dsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/dsp/test_list_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/dsp/test_numpy_constants_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/dsp/test_processing_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/dsp/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.052035 pygama-1.2.0/tests/flow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.052035 pygama-1.2.0/tests/flow/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/flow/configs/data-loader-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/flow/configs/filedb-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/flow/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/flow/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/flow/test_filedb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.052035 pygama-1.2.0/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/functional/test_l200_dataproc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/functional/test_teststand_dataproc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.052035 pygama-1.2.0/tests/hit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.052035 pygama-1.2.0/tests/hit/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/hit/configs/basic-hit-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/hit/configs/spms-hit-a-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/hit/configs/spms-hit-config.json
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/hit/configs/spms-hit-multi-config.json
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/hit/test_build_hit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.052035 pygama-1.2.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/integration/test_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.052035 pygama-1.2.0/tests/lgdo/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/lgdo/test_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/lgdo/test_arrayofequalsizedarrays.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/lgdo/test_fixedsizearray.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/lgdo/test_lgdo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/lgdo/test_lh5_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/lgdo/test_lh5_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/lgdo/test_representations.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/lgdo/test_scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/lgdo/test_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/lgdo/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/lgdo/test_table_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/lgdo/test_vectorofvectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/lgdo/test_waveform_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.052035 pygama-1.2.0/tests/math/
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/math/test_fwhm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.052035 pygama-1.2.0/tests/pargen/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/pargen/test_ecal.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/pargen/test_energy_optimization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.056035 pygama-1.2.0/tests/raw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.056035 pygama-1.2.0/tests/raw/buffer_processor/
--rw-r--r--   0 runner    (1001) docker     (123)    53808 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/buffer_processor/test_buffer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.056035 pygama-1.2.0/tests/raw/buffer_processor/test_buffer_processor_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/buffer_processor/test_buffer_processor_configs/raw_out_spec_no_proc.json
--rw-r--r--   0 runner    (1001) docker     (123)    42678 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/buffer_processor/test_lh5_buffer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.056035 pygama-1.2.0/tests/raw/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/configs/fc-out-spec.json
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/configs/orca-out-spec-cli.json
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/configs/orca-out-spec.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.056035 pygama-1.2.0/tests/raw/fc/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/fc/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/fc/test_fc_config_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/fc/test_fc_event_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/fc/test_fc_status_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/fc/test_fc_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.056035 pygama-1.2.0/tests/raw/orca/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/orca/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/orca/test_or_run_decoder_for_run.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/orca/test_orca_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/test_build_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/raw/test_raw_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.056035 pygama-1.2.0/tests/vis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:57:57.056035 pygama-1.2.0/tests/vis/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/vis/configs/hpge-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-01-20 09:57:45.000000 pygama-1.2.0/tests/vis/test_waveform_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 09:40:47.000000 pygama-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-07 09:40:56.440826 pygama-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-07 09:40:47.000000 pygama-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-07 09:40:47.000000 pygama-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-07 09:40:56.440826 pygama-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-07 09:40:47.000000 pygama-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.416826 pygama-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.420826 pygama-1.3.0/src/pygama/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 09:40:56.000000 pygama-1.3.0/src/pygama/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12151 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.420826 pygama-1.3.0/src/pygama/dsp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/build_dsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71519 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processing_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.424826 pygama-1.3.0/src/pygama/dsp/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/bl_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/dplms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/dwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/fftw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/fixed_time_pickoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/gaussian_filter1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/get_multi_local_extrema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/linear_slope_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/log_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/min_max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/moving_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/multi_a_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/multi_t_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/param_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/peak_snr_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/pole_zero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/presum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/pulse_injector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/saturation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/soft_pileup_corr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/time_over_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/time_point_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/trap_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/wiener_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/processors/windower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/dsp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.424826 pygama-1.3.0/src/pygama/evt/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/evt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/evt/build_tcm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/evt/tcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.424826 pygama-1.3.0/src/pygama/flow/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60726 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/flow/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26986 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/flow/file_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/flow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.424826 pygama-1.3.0/src/pygama/hit/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/hit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/hit/build_hit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.428826 pygama-1.3.0/src/pygama/lgdo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/arrayofequalsizedarrays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.428826 pygama-1.3.0/src/pygama/lgdo/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/compression/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/compression/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/compression/radware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/compression/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/compression/varlen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/encoded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/fixedsizearray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/lgdo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/lgdo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68140 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/lh5_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21858 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/vectorofvectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/lgdo/waveform_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.428826 pygama-1.3.0/src/pygama/math/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/math/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38829 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/math/peak_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/math/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/math/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.428826 pygama-1.3.0/src/pygama/pargen/
+-rw-r--r--   0 runner    (1001) docker     (123)    46542 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/AoE_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13991 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/cuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/data_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/dsp_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33112 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/ecal_th.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52594 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/energy_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72502 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/energy_optimisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/extract_tau.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/pargen/mse_psd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.428826 pygama-1.3.0/src/pygama/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.432826 pygama-1.3.0/src/pygama/raw/buffer_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/buffer_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13831 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/buffer_processor/buffer_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/buffer_processor/lh5_buffer_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/build_raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.432826 pygama-1.3.0/src/pygama/raw/compass/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/compass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/compass/compass_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/compass/compass_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/compass/compass_header_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/compass/compass_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/data_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/data_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.432826 pygama-1.3.0/src/pygama/raw/fc/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/fc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/fc/fc_config_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/fc/fc_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/fc/fc_status_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/fc/fc_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.432826 pygama-1.3.0/src/pygama/raw/orca/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/orca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/orca/orca_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/orca/orca_digitizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33100 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/orca/orca_flashcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/orca/orca_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/orca/orca_header_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/orca/orca_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/orca/orca_run_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/orca/orca_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17834 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/raw/raw_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.432826 pygama-1.3.0/src/pygama/vis/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/vis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.432826 pygama-1.3.0/src/pygama/vis/mpl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/vis/mpl/clint.mpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/vis/mpl/root.mpl
+-rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-05-07 09:40:47.000000 pygama-1.3.0/src/pygama/vis/waveform_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.420826 pygama-1.3.0/src/pygama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-07 09:40:56.000000 pygama-1.3.0/src/pygama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-07 09:40:56.000000 pygama-1.3.0/src/pygama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:40:56.000000 pygama-1.3.0/src/pygama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-07 09:40:56.000000 pygama-1.3.0/src/pygama.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:40:56.000000 pygama-1.3.0/src/pygama.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-07 09:40:56.000000 pygama-1.3.0/src/pygama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 09:40:56.000000 pygama-1.3.0/src/pygama.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.432826 pygama-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.432826 pygama-1.3.0/tests/dsp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.432826 pygama-1.3.0/tests/dsp/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/configs/icpc-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/configs/numpy-parsing.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/configs/sipm-dplms-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/configs/sipm-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/dsp/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)    14296 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/processors/dplms_noise_mat.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/processors/test_dplms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/processors/test_dwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/processors/test_fixed_time_pickoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/processors/test_get_multi_local_extrema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/processors/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/test_build_dsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/test_list_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/test_numpy_constants_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/test_processing_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/dsp/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/flow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/flow/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/flow/configs/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/flow/configs/data-loader-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/flow/configs/filedb-config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/flow/configs/nested/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/flow/configs/nested/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/flow/configs/nested/data-loader-config-nested.json
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/flow/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/flow/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/flow/test_filedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/flow/test_flow_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/functional/test_l200_dataproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/functional/test_teststand_dataproc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/hit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/hit/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/hit/configs/basic-hit-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/hit/configs/spms-hit-a-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/hit/configs/spms-hit-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/hit/configs/spms-hit-multi-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/hit/test_build_hit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/integration/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/lgdo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/lgdo/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/compression/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/lgdo/compression/sigcompress/
+-rw-r--r--   0 runner    (1001) docker     (123)    23516 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/compression/sigcompress/special-wf-clipped.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/compression/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47033 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/compression/test_radware_sigcompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/compression/test_str2wfcodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/compression/test_uleb128_zigzag_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_arrayofequalsizedarrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_encoded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_fixedsizearray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_lgdo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_lh5_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25869 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_lh5_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_table_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_vectorofvectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/lgdo/test_waveform_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.436826 pygama-1.3.0/tests/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/math/test_fwhm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/pargen/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/pargen/test_ecal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/pargen/test_energy_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/raw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/raw/buffer_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)    56908 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/buffer_processor/test_buffer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/raw/buffer_processor/test_buffer_processor_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/buffer_processor/test_buffer_processor_configs/raw_out_spec_no_proc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    42875 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/buffer_processor/test_lh5_buffer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/raw/compass/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/compass/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/compass/test_compass_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/compass/test_compass_header_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/compass/test_compass_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/raw/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/configs/fc-out-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/configs/orca-out-spec-cli.json
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/configs/orca-out-spec.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/raw/fc/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/fc/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/fc/test_fc_config_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/fc/test_fc_event_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/fc/test_fc_status_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/fc/test_fc_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/raw/orca/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/orca/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/orca/test_or_run_decoder_for_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/orca/test_orca_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/test_build_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/test_daq_to_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/raw/test_raw_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/vis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:40:56.440826 pygama-1.3.0/tests/vis/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/vis/configs/hpge-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-07 09:40:47.000000 pygama-1.3.0/tests/vis/test_waveform_browser.py
```

### Comparing `pygama-1.2.0/LICENSE` & `pygama-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/PKG-INFO` & `pygama-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygama
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python package for decoding and processing digitizer data
 Home-page: https://github.com/legend-exp/pygama
 Author: The LEGEND collaboration
 Maintainer: The LEGEND collaboration
 License: GPL-3.0
 Project-URL: Documentation, https://pygama.readthedocs.io
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pygama-1.2.0/README.md` & `pygama-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/setup.cfg` & `pygama-1.3.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -30,28 +30,30 @@
 
 [options]
 packages = find:
 install_requires = 
 	PyWavelets
 	colorlog
 	h5py>=3.2.0
+	hdf5plugin
 	iminuit
 	matplotlib
-	numba!=0.53.*,!=0.54.*
+	numba!=0.53.*,!=0.54.*,!=0.57
 	numexpr
 	numpy>=1.21
 	pandas>=1.4.4
 	parse
 	pint
 	pyfcutils
 	pyfftw
 	scikit-learn
-	scipy
+	scipy>=1.0.1
 	tables
 	tqdm
+	xmltodict
 python_requires = >=3.9
 include_package_data = True
 package_dir = 
 	= src
 zip_safe = False
 
 [options.packages.find]
```

### Comparing `pygama-1.2.0/src/pygama/cli.py` & `pygama-1.3.0/src/pygama/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,21 +88,24 @@
     parser_lh5ls.add_argument(
         "lh5_file",
         help="""Input LH5 file.""",
     )
     parser_lh5ls.add_argument(
         "lh5_group", nargs="?", help="""LH5 group.""", default="/"
     )
+    parser_lh5ls.add_argument(
+        "--attributes", "-a", action="store_true", help="""Print HDF5 attributes too"""
+    )
     parser_lh5ls.set_defaults(func=lh5_show_cli)
 
 
 def lh5_show_cli(args):
     """Passes command line arguments to :func:`.lgdo.lh5_store.show`."""
 
-    show(args.lh5_file, args.lh5_group)
+    show(args.lh5_file, args.lh5_group, attrs=args.attributes)
 
 
 def add_build_raw_parser(subparsers):
     """Configure :func:`.raw.build_raw.build_raw` command line interface"""
 
     parser_d2r = subparsers.add_parser(
         "build-raw", description="""Convert data into LEGEND HDF5 (LH5) raw format"""
```

### Comparing `pygama-1.2.0/src/pygama/dsp/__init__.py` & `pygama-1.3.0/src/pygama/dsp/__init__.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/build_dsp.py` & `pygama-1.3.0/src/pygama/dsp/build_dsp.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,19 @@
         hasattr(lh5_tables, "__iter__")
         and all(isinstance(el, str) for el in lh5_tables)
     ):
         raise RuntimeError("lh5_tables must be None, a string, or a list of strings")
 
     # check if group points to raw data; sometimes 'raw' is nested, e.g g024/raw
     for i, tb in enumerate(lh5_tables):
-        if "raw" not in tb and lh5.ls(lh5_file, f"{tb}/raw"):
+        if (
+            "raw" not in tb
+            and not isinstance(raw_store.gimme_file(lh5_file, "r")[tb], h5py.Dataset)
+            and lh5.ls(lh5_file, f"{tb}/raw")
+        ):
             lh5_tables[i] = f"{tb}/raw"
         elif not lh5.ls(lh5_file, tb):
             del lh5_tables[i]
 
     if len(lh5_tables) == 0:
         raise RuntimeError(f"could not find any valid LH5 table in {f_raw}")
```

### Comparing `pygama-1.2.0/src/pygama/dsp/errors.py` & `pygama-1.3.0/src/pygama/dsp/errors.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processing_chain.py` & `pygama-1.3.0/src/pygama/dsp/processing_chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -964,15 +964,14 @@
         proc_chain: ProcessingChain,
         func: np.ufunc,
         params: list[str],
         kw_params: dict = None,
         signature: str = None,
         types: list[str] = None,
     ) -> None:
-
         assert (
             isinstance(proc_chain, ProcessingChain)
             and callable(func)
             and isinstance(params, list)
         )
 
         if kw_params is None:
@@ -1188,15 +1187,15 @@
             elif isinstance(param, str):
                 # Convert string into integer buffer if appropriate
                 if np.issubdtype(dtype, np.integer):
                     try:
                         param = np.frombuffer(param.encode("ascii"), dtype).reshape(
                             shape
                         )
-                    except (ValueError):
+                    except ValueError:
                         raise ProcessingChainError(
                             f"could not convert string '{param}' into"
                             f"byte-array of type {dtype} and shape {shape}"
                         )
 
             elif param is not None:
                 # Convert scalar to right type, including units
@@ -1242,26 +1241,38 @@
 class UnitConversionManager(ProcessorManager):
     """A special processor manager for handling converting variables between unit systems."""
 
     @vectorize(nopython=True, cache=True)
     def convert(buf_in, offset_in, offset_out, period_ratio):  # noqa: N805
         return (buf_in + offset_in) * period_ratio - offset_out
 
+    @vectorize(nopython=True, cache=True)
+    def convert_int(buf_in, offset_in, offset_out, period_ratio):  # noqa: N805
+        tmp = (buf_in + offset_in) * period_ratio - offset_out
+        ret = round(tmp)
+        if np.abs(tmp - ret) < 1.0e-5:
+            return ret
+        else:
+            raise DSPFatal("Cannot convert to integer")
+
     def __init__(self, var: ProcChainVar, unit: str | Unit) -> None:
         # reference back to our processing chain
         self.proc_chain = var.proc_chain
         # callable function used to process data
-        self.processor = UnitConversionManager.convert
+        if np.issubdtype(var.dtype, np.integer):
+            self.processor = UnitConversionManager.convert_int
+        else:
+            self.processor = UnitConversionManager.convert
         # list of parameters prior to converting to internal representation
         self.params = [var, unit]
         self.kw_params = {}
 
         from_buffer, from_grid = var._buffer[0]
         period_ratio = from_grid.get_period(unit.period)
-        self.out_buffer = np.zeros_like(from_buffer, dtype="float64")
+        self.out_buffer = np.zeros_like(from_buffer, dtype=var.dtype)
         self.args = [
             from_buffer,
             from_grid.get_offset(),
             unit.get_offset(),
             period_ratio,
             self.out_buffer,
         ]
@@ -1733,21 +1744,21 @@
     log.debug(f"processed output parameters: {out_par_list}")
 
     # Now add all of the input buffers from lh5_in (and also the clk time)
     for input_par in input_par_list:
         buf_in = lh5_in.get(input_par)
         if buf_in is None:
             log.warning(
-                f"I don't know what to do with {input_par}. Building output without it!"
+                f"I don't know what to do with '{input_par}'. Building output without it!"
             )
         try:
             proc_chain.link_input_buffer(input_par, buf_in)
         except Exception as e:
             raise ProcessingChainError(
-                f"Exception raised while linking input buffer {input_par}."
+                f"Exception raised while linking input buffer '{input_par}'."
             ) from e
 
     # now add the processors
     for proc_par in proc_par_list:
         recipe = processors[proc_par]
         try:
             module = importlib.import_module(recipe["module"])
```

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/__init__.py` & `pygama-1.3.0/src/pygama/dsp/processors/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 from .dplms import dplms
 from .dwt import discrete_wavelet_transform
 from .fftw import dft, inv_dft, psd
 from .fixed_time_pickoff import fixed_time_pickoff
 from .gaussian_filter1d import gaussian_filter1d
 from .get_multi_local_extrema import get_multi_local_extrema
 from .histogram import histogram, histogram_stats
-from .linear_slope_fit import linear_slope_fit
+from .linear_slope_fit import linear_slope_diff, linear_slope_fit
 from .log_check import log_check
 from .min_max import min_max
 from .moving_windows import (
     avg_current,
     moving_window_left,
     moving_window_multi,
     moving_window_right,
@@ -105,14 +105,15 @@
     "psd",
     "fixed_time_pickoff",
     "gaussian_filter1d",
     "get_multi_local_extrema",
     "histogram",
     "histogram_stats",
     "linear_slope_fit",
+    "linear_slope_diff",
     "log_check",
     "min_max",
     "avg_current",
     "moving_window_left",
     "moving_window_multi",
     "moving_window_right",
     "multi_a_filter",
```

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/bl_subtract.py` & `pygama-1.3.0/src/pygama/dsp/processors/bl_subtract.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/convolutions.py` & `pygama-1.3.0/src/pygama/dsp/processors/convolutions.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/dwt.py` & `pygama-1.3.0/src/pygama/dsp/processors/dwt.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/fftw.py` & `pygama-1.3.0/src/pygama/dsp/processors/fftw.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/fixed_time_pickoff.py` & `pygama-1.3.0/src/pygama/dsp/processors/fixed_time_pickoff.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/gaussian_filter1d.py` & `pygama-1.3.0/src/pygama/dsp/processors/gaussian_filter1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,14 @@
         "(n),(m)",
         **nb_kwargs(
             cache=False,
             forceobj=True,
         ),
     )
     def gaussian_filter1d_out(wf_in, wf_out):
-
         # Have to create an array to enable the reflect mode
         # Extend the signal on the left and right by at least half of the length of the kernel
 
         wf_in = numpy.asarray(wf_in)
 
         # Short warning message if kernel is larger than signal, in which case signal can't be convolved
```

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/get_multi_local_extrema.py` & `pygama-1.3.0/src/pygama/dsp/processors/get_multi_local_extrema.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,15 +126,14 @@
 
     # now loop over data
     # left to right search
     if (search_direction == 0) or (search_direction > 1):
         find_max = True
         imax, imin = 0, 0
         for i in range(len(w_in)):
-
             if w_in[i] > w_in[imax]:
                 imax = i
             if w_in[i] < w_in[imin]:
                 imin = i
             if find_max:
                 # if the sample is less than the current max by more than a_delta_in,
                 # declare the previous one a maximum, then set this as the new "min"
@@ -161,15 +160,14 @@
                     find_max = True
 
     # right to left search
     if search_direction > 0:
         find_max = True
         imax, imin = len(w_in) - 1, len(w_in) - 1
         for i in range(len(w_in) - 1, -1, -1):
-
             if w_in[i] > w_in[imax]:
                 imax = i
             if w_in[i] < w_in[imin]:
                 imin = i
             if find_max:
                 # if the sample is less than the current max by more than a_delta_in,
                 # declare the previous one a maximum, then set this as the new "min"
@@ -208,15 +206,14 @@
         n_max_out[0] = n_max_right_counter
         n_min_out[0] = n_min_right_counter
         vt_max_out[:] = right_vt_max
         vt_min_out[:] = right_vt_min
 
     # conservative search (only extrema found in both directions)
     elif search_direction == 2:
-
         # sort the right search result. Left search should be already sorted
         right_vt_max = np.sort(right_vt_max)
         right_vt_min = np.sort(right_vt_min)
 
         rge_right = (right_vt_max[~np.isnan(right_vt_max)]).astype(np.int_)
         rge_left = (left_vt_max[~np.isnan(left_vt_max)]).astype(np.int_)
```

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/histogram.py` & `pygama-1.3.0/src/pygama/dsp/processors/histogram.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     ],
     "(n),(m),(p)",
     **nb_kwargs,
 )
 def histogram(
     w_in: np.ndarray, weights_out: np.ndarray, borders_out: np.ndarray
 ) -> None:
-
     """Produces and returns an histogram of the waveform.
 
     Parameters
     ----------
     w_in
         Data to be histogrammed.
     weights_out
@@ -93,15 +92,14 @@
     weights_in: np.ndarray,
     edges_in: np.ndarray,
     mode_out: int,
     max_out: float,
     fwhm_out: float,
     max_in: float,
 ) -> None:
-
     """Compute useful histogram-related quantities.
 
     Parameters
     ----------
     weights_in
         histogram weights.
     edges_in
```

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/linear_slope_fit.py` & `pygama-1.3.0/src/pygama/dsp/processors/linear_slope_fit.py`

 * *Files 26% similar despite different names*

```diff
@@ -71,7 +71,67 @@
         sum_y += w_in[i]
 
     stdev /= isum - 1
     np.sqrt(stdev, stdev)
 
     slope[0] = (isum * sum_xy - sum_x * sum_y) / (isum * sum_x2 - sum_x * sum_x)
     intercept[0] = (sum_y - sum_x * slope[0]) / isum
+
+
+@guvectorize(
+    [
+        "void(float32[:], float32[:], float32[:], float32[:], float32[:])",
+        "void(float64[:], float64[:], float64[:], float64[:], float64[:])",
+    ],
+    "(n),(),()->(),()",
+    **nb_kwargs,
+)
+def linear_slope_diff(
+    w_in: np.ndarray, slope: float, intercept: float, mean: float, rms: float
+) -> None:
+    """
+    Calculate the mean, standard deviation, slope and y-intercept of waveform.
+
+    Uses Welford's method and linear regression.
+
+    Parameters
+    ----------
+    w_in
+        the input waveform.
+    mean
+        the mean of the waveform.
+    stdev
+        the standard deviation of the waveform.
+    slope
+        the slope of the linear fit.
+    intercept
+        the intercept of the linear fit.
+
+    JSON Configuration Example
+    --------------------------
+
+    .. code-block :: json
+
+        "bl_mean, bl_std, bl_slope, bl_intercept": {
+            "function": "linear_slope_fit",
+            "module": "pygama.dsp.processors",
+            "args": ["wf_blsub[0:1650]", "bl_mean", "bl_std", "bl_slope", "bl_intercept"],
+            "unit": ["ADC", "ADC", "ADC", "ADC"],
+        }
+    """
+    mean[0] = np.nan
+    rms[0] = np.nan
+
+    if np.isnan(w_in).any() or np.isnan(slope) or np.isnan(intercept):
+        return
+
+    mean[0] = rms[0] = 0
+    isum = len(w_in)
+
+    for i in range(0, len(w_in), 1):
+        # the mean and standard deviation
+        temp = w_in[i] - (slope * i + intercept)
+        mean += temp / (i + 1)
+        rms += temp * temp
+
+    rms /= isum - 1
+    np.sqrt(rms, rms)
```

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/log_check.py` & `pygama-1.3.0/src/pygama/dsp/processors/log_check.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/min_max.py` & `pygama-1.3.0/src/pygama/dsp/processors/min_max.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/moving_windows.py` & `pygama-1.3.0/src/pygama/dsp/processors/moving_windows.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/multi_a_filter.py` & `pygama-1.3.0/src/pygama/dsp/processors/multi_a_filter.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/multi_t_filter.py` & `pygama-1.3.0/src/pygama/dsp/processors/multi_t_filter.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/optimize.py` & `pygama-1.3.0/src/pygama/dsp/processors/optimize.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/param_lookup.py` & `pygama-1.3.0/src/pygama/dsp/processors/param_lookup.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/peak_snr_threshold.py` & `pygama-1.3.0/src/pygama/dsp/processors/peak_snr_threshold.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/pole_zero.py` & `pygama-1.3.0/src/pygama/dsp/processors/pole_zero.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/presum.py` & `pygama-1.3.0/src/pygama/dsp/processors/presum.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/pulse_injector.py` & `pygama-1.3.0/src/pygama/dsp/processors/pulse_injector.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/saturation.py` & `pygama-1.3.0/src/pygama/dsp/processors/saturation.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/soft_pileup_corr.py` & `pygama-1.3.0/src/pygama/dsp/processors/soft_pileup_corr.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/time_over_threshold.py` & `pygama-1.3.0/src/pygama/dsp/processors/time_over_threshold.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/time_point_thresh.py` & `pygama-1.3.0/src/pygama/dsp/processors/time_point_thresh.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/trap_filters.py` & `pygama-1.3.0/src/pygama/dsp/processors/trap_filters.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/upsampler.py` & `pygama-1.3.0/src/pygama/dsp/processors/upsampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
                 w_out[t_out] = w_in[t_in]
             t_out += 1
 
 
 @guvectorize(
     ["void(float32[:], char, float32[:])", "void(float64[:], char, float64[:])"],
     "(n),(),(m)",
-    nopython=True,
     **nb_kwargs,
 )
 def interpolating_upsampler(
     w_in: np.ndarray, mode_in: np.int8, w_out: np.ndarray
 ) -> None:
     """Upsamples the waveform.
```

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/wiener_filter.py` & `pygama-1.3.0/src/pygama/dsp/processors/wiener_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,14 @@
 
     fft_superpulse = np.fft.fft(superpulse)
     fft_noise_wf = np.fft.fft(noise_wf)
 
     # Create the point spread function for the detector's response
 
     def psf(superpulse, fft_superpulse):
-
         delta = np.zeros_like(superpulse)
         arg_max = np.argmax(superpulse)
         delta[arg_max] = np.amax(superpulse)
 
         return fft_superpulse / np.fft.fft(delta)
 
     # Now create the wiener filter in the frequency domain
```

### Comparing `pygama-1.2.0/src/pygama/dsp/processors/windower.py` & `pygama-1.3.0/src/pygama/dsp/processors/windower.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/dsp/utils.py` & `pygama-1.3.0/src/pygama/dsp/utils.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/evt/build_tcm.py` & `pygama-1.3.0/src/pygama/evt/build_tcm.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 
 import pygama.evt.tcm as ptcm
 import pygama.lgdo as lgdo
 
 
 def build_tcm(
-    input_tables: list[tuple[str, str]],
+    input_tables: list[tuple[str, str | list[str]]],
     coin_col: str,
     hash_func: str = r"\d+",
     coin_window: float = 0,
     window_ref: str = "last",
     out_file: str = None,
     out_name: str = "tcm",
     wo_mode: str = "write_safe",
@@ -24,15 +24,16 @@
     :class:`~.flow.data_loader.DataLoader`.
 
     Parameters
     ----------
     input_tables
         each entry is ``(filename, table_name_pattern)``. All tables matching
         ``table_name_pattern`` in ``filename`` will be added to the list of
-        input tables.
+        input tables. ``table_name_pattern`` can be replaced with a list of
+        patterns to be searched for in the file
     coin_col
         the name of the column in each tables used to build coincidences. All
         tables must contain a column with this name.
     hash_func
         mapping of table names to integers for use in the TCM.  `hash_func` is
         a regexp pattern that acts on each table name. The default `hash_func`
         ``r"\d+"`` pulls the first integer out of the table name. Setting to
@@ -55,31 +56,34 @@
     """
     # hash_func: later can add list or dict or a function(str) --> int.
 
     store = lgdo.LH5Store()
     coin_data = []
     array_ids = []
     all_tables = []
-    for filename, pattern in input_tables:
-        tables = lgdo.ls(filename, lh5_group=pattern)
-        for table in tables:
-            all_tables.append(table)
-            array_id = len(array_ids)
-            if hash_func is not None:
-                if isinstance(hash_func, str):
-                    array_id = int(re.search(hash_func, table).group())
+    for filename, patterns in input_tables:
+        if isinstance(patterns, str):
+            patterns = [patterns]
+        for pattern in patterns:
+            tables = lgdo.ls(filename, lh5_group=pattern)
+            for table in tables:
+                all_tables.append(table)
+                array_id = len(array_ids)
+                if hash_func is not None:
+                    if isinstance(hash_func, str):
+                        array_id = int(re.search(hash_func, table).group())
+                    else:
+                        raise NotImplementedError(
+                            f"hash_func of type {type(hash_func).__name__}"
+                        )
                 else:
-                    raise NotImplementedError(
-                        f"hash_func of type {type(hash_func).__name__}"
-                    )
-            else:
-                array_id = len(all_tables) - 1
-            table = table + "/" + coin_col
-            coin_data.append(store.read_object(table, filename)[0].nda)
-            array_ids.append(array_id)
+                    array_id = len(all_tables) - 1
+                table = table + "/" + coin_col
+                coin_data.append(store.read_object(table, filename)[0].nda)
+                array_ids.append(array_id)
 
     tcm_cols = ptcm.generate_tcm_cols(
         coin_data, coin_window=coin_window, window_ref=window_ref, array_ids=array_ids
     )
 
     for key in tcm_cols:
         tcm_cols[key] = lgdo.Array(nda=tcm_cols[key])
```

### Comparing `pygama-1.2.0/src/pygama/evt/tcm.py` & `pygama-1.3.0/src/pygama/evt/tcm.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,22 +14,24 @@
     array_ids: list[int] = None,
     array_idxs: list[int] = None,
 ) -> dict[np.ndarray]:
     r"""Generate the columns of a time coincidence map.
 
     Generate the columns of a time coincidence map from a list of arrays of
     coincidence data (e.g. hit times from different channels). Returns 3
-    equal-length :class:`numpy.ndarray`\ s containing the coincidence index
-    (e.g. event number), array ID (e.g. channel number), and array index (e.g.
-    hit ID). These can be used to retrieve other data at the same tier as the
-    input data into coincidence structures.
+    :class:`numpy.ndarray`\ s representing a vector-of-vector-like structure:
+    two flattened arrays ``array_id`` (e.g. channel number) and  ``array_idx``
+    (e.g. hit ID) that specify the location in the input ``coin_data`` of each
+    datum belonging to a coincidence event, and a ``cumulative_length`` array
+    that specifies which rows of the other two output arrays correspond to
+    which coincidence event. These can be used to retrieve other data at the
+    same tier as the input data into coincidence structures.
 
     Makes use of :func:`pandas.concat`, :meth:`pandas.DataFrame.sort_values`,
-    :meth:`pandas.DataFrame.groupby`, and
-    :meth:`pandas.DataFrame.cumsum`/:meth:`pandas.DataFrame.count` functions:
+    and :meth:`pandas.DataFrame.diff` functions:
 
     - pull data into a :class:`pandas.DataFrame`
     - sort events by strictly ascending value of `coin_col`
     - group hits if the difference in `coin_data` is less than `coin_window`
 
     Parameters
     ----------
@@ -54,28 +56,29 @@
     array_idxs
         if provided, use these values in places of the ``DataFrame`` index for
         the return values of `array_idx`.
 
     Returns
     -------
     col_dict
-        keys are ``coin_idx``, ``array_id``, and  ``array_idx``. ``coin_idx``
-        specifies which rows of the output arrays correspond to the which
-        coincidence event ``array_id`` and ``array_idx`` specify the location
-        in ``coin_data`` of each datum belonging to the coincidence event.
+        keys are ``cumulative_length``, ``array_id``, and  ``array_idx``.
+        ``cumulative_length`` specifies which rows of the other two output
+        arrays correspond to which coincidence event. ``array_id`` and
+        ``array_idx`` specify the location in ``coin_data`` of each datum
+        belonging to the coincidence event.
     """
     dfs = []
     for ii, array in enumerate(coin_data):
         array = np.array(array)
         array_id = array_ids[ii] if array_ids is not None else ii
         array_id = np.full_like(array, array_id)
         col_dict = {"array_id": array_id, "coin_data": array}
         if array_idxs is not None:
             col_dict["array_idx"] = array_idxs[ii]
-        dfs.append(pd.DataFrame(col_dict, copy=False))
+        dfs.append(pd.DataFrame(col_dict, copy=False))  # don't copy the data!
 
     # concat and sort
     tcm = pd.concat(dfs).sort_values(["coin_data", "array_id"])
 
     # compute coin_data diffs
     tcm["dcoin"] = tcm["coin_data"].diff()
```

### Comparing `pygama-1.2.0/src/pygama/flow/data_loader.py` & `pygama-1.3.0/src/pygama/flow/data_loader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,30 @@
-"""
-Routines for high-level data loading and skimming.
-"""
+"""Routines for high-level data loading and skimming."""
+
 from __future__ import annotations
 
 import json
 import logging
 import os
 import re
 import string
 from itertools import product
 from keyword import iskeyword
+from typing import Iterator
 
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 
-from pygama.flow.file_db import FileDB
-from pygama.lgdo import (
-    Array,
-    ArrayOfEqualSizedArrays,
-    LH5Store,
-    Struct,
-    Table,
-    WaveformTable,
-)
+from pygama.lgdo import Array, LH5Iterator, LH5Store, Struct, Table, lgdo_utils
 from pygama.lgdo.vectorofvectors import build_cl, explode_arrays, explode_cl
+from pygama.vis import WaveformBrowser
+
+from . import utils
+from .file_db import FileDB
 
 log = logging.getLogger(__name__)
 
 
 class DataLoader:
     """Facilitate loading of processed data across several tiers.
 
@@ -37,14 +33,15 @@
     processing tier.
 
     Example JSON configuration file:
 
     .. code-block:: json
 
         {
+            "filedb": "path/to/filedb.h5"
             "levels": {
                 "hit": {
                     "tiers": ["raw", "dsp", "hit"]
                 },
                 "tcm": {
                     "tiers": ["tcm"],
                     "parent": "hit",
@@ -54,64 +51,78 @@
                         "parent_tb": "array_id",
                         "parent_idx": "array_idx"
                     }
                 },
                 "evt": {
                     "tiers": ["evt"]
                 }
-            },
-            "channel_map": {}
+            }
         }
 
 
     Examples
     --------
 
     >>> from pygama.flow import DataLoader
-    >>> dl = DataLoader("loader-config.json", "filedb-config.json")
+    >>> dl = DataLoader("loader-config.json")
     >>> dl.set_files("file_status == 26 and timestamp == '20220716T130443Z'")
     >>> dl.set_datastreams([3, 6, 8], "ch")
     >>> dl.set_cuts({"hit": "daqenergy > 1000 and AoE > 3", "evt": "muon_veto == False"})
     >>> dl.set_output(fmt="pd.DataFrame", columns=["daqenergy", "channel"])
     >>> data = dl.load()
 
+    Be careful, :meth:`.load()` loads data in memory regardless of its size. If
+    loading a lot of data (e.g. waveforms), you might want to do it in chunks.
+    :class:`.next()` does exactly this:
+
+    >>> for chunk in dl.load():
+    ...   run_my_processing(chunk)
 
     Advanced Usage:
 
     >>> from pygama.flow import DataLoader
-    >>> dl = DataLoader("loader-config.json", "filedb-config.json")
+    >>> dl = DataLoader("loader-config.json", filedb="filedb-config.json")  # or any value accepted by the FileDB constructor
     >>> dl.set_files("all")
     >>> dl.set_datastreams([0], "ch")
     >>> dl.set_cuts({"hit": "wf_max > 30000"})
     >>> el = dl.build_entry_list(tcm_level="tcm", mode="any")
     >>> el.query("hit_table == 20", inplace=True)
     >>> dl.set_output(fmt="pd.DataFrame", columns=["daqenergy", "channel"])
     >>> data = dl.load(el)
     """
 
     def __init__(
         self,
         config: str | dict,
-        filedb: str | dict | FileDB,
+        filedb: str | dict | FileDB = None,
         file_query: str = None,
     ) -> None:
         """
         Parameters
         ----------
         config
-            configuration dictionary or JSON file, see above for specifications.
+            configuration dictionary or JSON file, see above for a specification.
+            Accepts strings in the following format: ::
+
+              path/to/config.json[field1/field2/...]]
+
+            to specify the location of the :class:`DataLoader` configuration in
+            the ``config.json`` dictionary, if not at the first level.
 
         filedb
             the loader needs a file database. It can be specified in multiple ways:
 
             - an instance of :class:`.FileDB`.
             - an LH5 file containing a :class:`.FileDB` (see also
               :meth:`.FileDB.to_disk`).
             - a :class:`.FileDB` configuration dictionary or JSON file.
 
+            If ``None``, uses the value of the ``filedb`` key in `config` to
+            instantiate a :class:`.FileDB` object.
+
         file_query
             string query that should operate on columns of a :class:`.FileDB`.
 
         Note
         ----
         No data is loaded in memory at this point.
         """
@@ -120,49 +131,91 @@
         self.filedb: FileDB = None
         self.file_list: list = None
         self.table_list = None
         self.cuts = None
         self.merge_files = True
         self.output_format = "lgdo.Table"
         self.output_columns = None
+        self.aoesa_to_vov = False
         self.data = None
 
+        # already set FileDB, if supplied
         if isinstance(filedb, FileDB):
             self.filedb = filedb
-        else:
+        elif filedb is not None:
             self.filedb = FileDB(filedb)
 
         # load things if available
         if config is not None:
-            if isinstance(config, str):
-                with open(config) as f:
-                    config = json.load(f)
             self.set_config(config)
 
         # set the file_list
         if file_query is not None:
             self.file_list = list(self.filedb.df.query(file_query).index)
 
-    # --------- Get/Set/Reset Functions ----------#
+    def set_config(self, config: dict | str) -> None:
+        """Load configuration dictionary.
 
-    def set_config(self, config: dict) -> None:
-        """Load configuration dictionary."""
+        ``$_`` expands to the config file location, if possible, otherwise the
+        current working directory.
+        """
+
+        # define directory for $_ path substitution later in the config
+        # - if a JSON file is provided, it is set to the directory where the
+        #   file is located
+        # - if a dict is provided, it is set to the current directory
+        config_dir = os.getcwd()
+        if isinstance(config, str):
+            # the config string supports this syntax:
+            #  file.json[level1/level2[/...]]
+            # to specify where the data loader config shall be found in the
+            # json file
+            config_loc = None
+            m = re.match(r"^(.*)\[(.*)\]$", config)
+            if m is not None:
+                g = m.groups()
+                config = g[0]
+                config_loc = g[1].split("/")
+
+            # if a directory is provided, try looking for a file named
+            # config.json
+            if os.path.isdir(config):
+                config_dir = config
+                config = os.path.join(config, "config.json")
+            else:
+                config_dir = os.path.dirname(config)
+
+            with open(config) as f:
+                config = json.load(f)
+
+            if config_loc is not None:
+                for loc in config_loc:
+                    config = config[loc]
+
+        # look for info in configuration if FileDB is not set
+        if self.filedb is None:
+            # expand $_ variables
+            value = lgdo_utils.expand_vars(
+                config["filedb"], substitute={"_": config_dir}
+            )
+            self.filedb = FileDB(value)
 
         if not os.path.isdir(self.filedb.data_dir):
             raise FileNotFoundError(
                 f"{self.filedb.data_dir} (path to data root directory in FileDB) does not exist"
             )
 
         self.config = config
         self.data_dir = self.filedb.data_dir
         self.levels = list(config["levels"].keys())
         self.tiers = {}
         self.cut_priority = {}
         self.evts = {}
         self.tcms = {}
+
         for level in self.levels:
             self.tiers[level] = config["levels"][level]["tiers"]
             # Set cut priority
             if "parent" in config["levels"][level].keys():  # This level is a TCM
                 parent = config["levels"][level]["parent"]
                 child = config["levels"][level]["child"]
                 self.tcms[level] = config["levels"][level]
@@ -174,23 +227,14 @@
                 if "tcm_cols" not in config["levels"][level].keys():
                     log.warning(
                         f"TCM levels, e.g. {level}, need to specify the TCM lookup columns"
                     )
             else:
                 self.cut_priority[level] = 0
 
-        # Set channel map
-        if isinstance(config["channel_map"], dict):
-            self.channel_map = config["channel_map"]
-        elif isinstance(config["channel_map"], str):
-            with open(config["channel_map"]) as f:
-                self.channel_map = json.load(f)
-        else:
-            log.warning("Channel map must be dict or path to JSON file")
-
     def set_files(self, query: str | list[str]) -> None:
         """Apply a file selection.
 
         Sets `self.file_list`, which is a list of indices corresponding to the
         rows in the file database.
 
         Parameters
@@ -237,15 +281,14 @@
     def get_file_list(self) -> pd.DataFrame:
         """
         Returns a copy of the file database with its dataframe pared down to
         the current file list.
         """
         return self.filedb.df.iloc[self.file_list]
 
-    # TODO Make this able to handle more complicated requests
     def set_datastreams(self, ds: list | tuple | np.ndarray, word: str) -> None:
         """Apply selection on data streams (or channels).
 
         Sets `self.table_list`.
 
         Parameters
         ----------
@@ -319,57 +362,69 @@
                     self.cuts[key] = value
         elif isinstance(cuts, list):
             raise NotImplementedError
             self.cuts = {}
             # TODO Parse strings to match column names so you don't have to specify which level it is
 
     def set_output(
-        self, fmt: str = None, merge_files: bool = None, columns: list = None
+        self,
+        fmt: str = None,
+        merge_files: bool = None,
+        columns: list = None,
+        aoesa_to_vov: bool = None,
     ) -> None:
         """
         Set the parameters for the output format of load
 
         Parameters
         ---------
         fmt
             ``lgdo.Table`` or ``pd.DataFrame``.
         merge_files
-            If ``True``, information from multiple files will be merged into
+            if ``True``, information from multiple files will be merged into
             one table.
         columns
-            The columns that should be copied into the output.
+            the columns that should be copied into the output.
+        aoesa_to_vov
+            output :class:`.ArrayOfEqualSizedArrays` as :class:`.VectorOfVectors`.
 
         Example
         -------
-        >>> dl.set_output(fmt="pd.DataFrame", merge_files=False, columns=["daqenergy", "trapEmax", "channel"])
+        >>> dl.set_output(
+        ...   fmt="pd.DataFrame",
+        ...   merge_files=False,
+        ...   columns=["daqenergy", "trapEmax", "channel"]
+        ... )
         """
         if fmt not in ["lgdo.Table", "pd.DataFrame", None]:
             raise ValueError(f"'{fmt}' output format not supported")
 
         if fmt is not None:
             self.output_format = fmt
         if merge_files is not None:
             self.merge_files = merge_files
         if columns is not None:
             self.output_columns = columns
+        if aoesa_to_vov is not None:
+            self.aoesa_to_vov = aoesa_to_vov
 
     def reset(self):
-        """Resets all fields to their default values, as if this is a newly
-        created data loader.
+        """Resets all fields to their default values.
+
+        As if this is a newly created data loader.
         """
         self.file_list = None
         self.table_list = None
         self.cuts = None
         self.merge_files = True
         self.output_format = "lgdo.Table"
         self.output_columns = None
+        self.aoesa_to_vov = False
         self.data = None
 
-    # ------------- Applying Cuts/Loading Data --------------#
-
     # TODO: mode
     def build_entry_list(
         self,
         tcm_level: str = None,
         tcm_table: int | str = None,
         mode: str = "only",
         save_output_columns: bool = False,
@@ -494,16 +549,20 @@
                 self.filedb.tier_dirs[tcm_tier].lstrip("/"),
                 self.filedb.df.iloc[file][f"{tcm_tier}_file"].lstrip("/"),
             )
 
             if not os.path.exists(tcm_path):
                 raise FileNotFoundError(f"Can't find TCM file for {tcm_level}")
 
-            tcm_table_name = self.get_table_name(tcm_tier, tcm_tb)
-            tcm_lgdo, _ = sto.read_object(tcm_table_name, tcm_path)
+            tcm_table_name = self.filedb.get_table_name(tcm_tier, tcm_tb)
+            try:
+                tcm_lgdo, _ = sto.read_object(tcm_table_name, tcm_path)
+            except KeyError:
+                log.warning(f"Cannot find table {tcm_table_name} in file {tcm_path}")
+                continue
             # Have to do some hacky stuff until I get a get_dataframe() method
             tcm_lgdo[self.tcms[tcm_level]["tcm_cols"]["child_idx"]] = Array(
                 nda=explode_cl(tcm_lgdo["cumulative_length"].nda)
             )
             tcm_lgdo.pop("cumulative_length")
             tcm_tb = Table(col_dict=tcm_lgdo)
             f_entries = tcm_tb.get_dataframe()
@@ -547,21 +606,27 @@
                         tier_path = os.path.join(
                             self.data_dir,
                             self.filedb.tier_dirs[tier].lstrip("/"),
                             self.filedb.df.loc[file, f"{tier}_file"].lstrip("/"),
                         )
                         if tier in col_tiers[file]["tables"].keys():
                             if tb in col_tiers[file]["tables"][tier]:
-                                table_name = self.get_table_name(tier, tb)
-                                tier_table, _ = sto.read_object(
-                                    table_name,
-                                    tier_path,
-                                    field_mask=cut_cols[level],
-                                    idx=idx_mask.tolist(),
-                                )
+                                table_name = self.filedb.get_table_name(tier, tb)
+                                try:
+                                    tier_table, _ = sto.read_object(
+                                        table_name,
+                                        tier_path,
+                                        field_mask=cut_cols[level],
+                                        idx=idx_mask.tolist(),
+                                    )
+                                except KeyError:
+                                    log.warning(
+                                        f"Cannot find {table_name} in file {tier_path}"
+                                    )
+                                    continue
                                 if tb_table is None:
                                     tb_table = tier_table
                                 else:
                                     tb_table.join(tier_table)
                     if tb_table is None:
                         continue
                     tb_df = tb_table.get_dataframe()
@@ -572,15 +637,15 @@
                     if mode == "only":
                         keep_idx = idx_match.index
                         drop_idx = set.symmetric_difference(
                             set(tcm_idx), list(keep_idx)
                         )
                         f_entries.drop(drop_idx, inplace=True)
                     elif mode == "any":
-                        evts = idx_match[f"{child}_idx"].unique()
+                        evts = list(idx_match[f"{child}_idx"].unique())
                         keep_idx = f_entries.query(f"{child}_idx in {evts}").index
                         drop = set.symmetric_difference(
                             set(f_entries.index), list(keep_idx)
                         )
                         if drop_idx is None:
                             drop_idx = drop
                         else:
@@ -588,32 +653,33 @@
                     else:
                         raise ValueError("mode must be either 'any' or 'only'")
 
                     if save_output_columns:
                         for col in tb_df.columns:
                             if col in for_output:
                                 f_entries.loc[keep_idx, col] = tb_df[col].tolist()
-                    # end for each table loop
-                # end for each level loop
+
             if mode == "any":
-                f_entries.drop(drop_idx, inplace=True)
+                if drop_idx is not None:
+                    f_entries.drop(index=drop_idx, inplace=True)
+
             f_entries.reset_index(inplace=True, drop=True)
+
             if in_memory:
                 entries[file] = f_entries
             if output_file:
                 # Convert f_entries DataFrame to Struct
                 f_dict = f_entries.to_dict("list")
                 f_struct = Struct(f_dict)
                 if self.merge_files:
                     sto.write_object(f_struct, "entries", output_file, wo_mode="a")
                 else:
                     sto.write_object(
                         f_struct, f"entries/{file}", output_file, wo_mode="a"
                     )
-            # end for each file loop
 
         if in_memory:
             if self.merge_files:
                 entries = pd.concat(entries.values(), ignore_index=True)
             return entries
 
     def build_hit_entries(
@@ -684,21 +750,22 @@
                 total=len(self.file_list),
                 delay=2,
                 unit=" keys",
             )
 
         # now we loop over the files in our list
         for file in self.file_list:
-
             if log.getEffectiveLevel() >= logging.INFO:
                 progress_bar.update()
-                progress_bar.set_postfix(key=self.filedb.df.iloc[file]["timestamp"])
+                progress_bar.set_postfix(
+                    key=self.filedb.df.iloc[file][self.filedb.sortby]
+                )
 
             log.debug(
-                f"building entry list for cycle {self.filedb.df.iloc[file]['timestamp']}"
+                f"building entry list for cycle {self.filedb.df.iloc[file][self.filedb.sortby]}"
             )
 
             # this dataframe will be associated with the file and will contain
             # the columns needed for the cut as well as the columns requested
             # for the output
             f_entries = pd.DataFrame(columns=entry_cols)
 
@@ -719,16 +786,20 @@
                     # reconstruct absolute path to tier file
                     tier_path = os.path.join(
                         self.data_dir,
                         self.filedb.tier_dirs[tier].lstrip("/"),
                         self.filedb.df.iloc[file][f"{tier}_file"].lstrip("/"),
                     )
                     # now read how many rows are there in the file
-                    table_name = self.get_table_name(tier, tb)
-                    n_rows = sto.read_n_rows(table_name, tier_path)
+                    table_name = self.filedb.get_table_name(tier, tb)
+                    try:
+                        n_rows = sto.read_n_rows(table_name, tier_path)
+                    except KeyError:
+                        log.warning(f"Cannot find {table_name} in file {tier_path}")
+                        continue
                     tb_df = pd.DataFrame(
                         {
                             f"{low_level}_idx": np.arange(n_rows),
                             f"{low_level}_table": tb,
                         }
                     )
                     if self.merge_files:
@@ -745,18 +816,24 @@
                             tier_path = os.path.join(
                                 self.data_dir,
                                 self.filedb.tier_dirs[tier].lstrip("/"),
                                 self.filedb.df.iloc[file][f"{tier}_file"].lstrip("/"),
                             )
 
                             # load the data from the tier file, just the columns needed for the cut
-                            table_name = self.get_table_name(tier, tb)
-                            tier_tb, _ = sto.read_object(
-                                table_name, tier_path, field_mask=cut_cols
-                            )
+                            table_name = self.filedb.get_table_name(tier, tb)
+                            try:
+                                tier_tb, _ = sto.read_object(
+                                    table_name, tier_path, field_mask=cut_cols
+                                )
+                            except KeyError:
+                                log.warning(
+                                    f"Cannot find {table_name} in file {tier_path}"
+                                )
+                                continue
                             # join eveything in one table
                             if tb_table is None:
                                 tb_table = tier_tb
                             else:
                                 tb_table.join(tier_tb)
 
                     if tb_table is None:
@@ -790,30 +867,87 @@
             progress_bar.close()
 
         if in_memory:
             if self.merge_files:
                 entries = pd.concat(entries.values(), ignore_index=True)
             return entries
 
-    # TODO : support chunked reading of entry_list from disk
+    def next(
+        self, entry_list: pd.DataFrame = None, chunk_size: int = 10000, **kwargs
+    ) -> Iterator[Table | Struct | pd.DataFrame]:
+        """Loads the requested data from disk in chunks.
+
+        This method should be used instead of :meth:`.load` to handle large
+        data sets.
+
+        Note
+        ----
+        It is a user responsibility to optimize the chunk size in order to
+        achieve best performance.
+
+        Parameters
+        ----------
+        chunk_size
+            number of entries to load at each iteration. Adapt based on the
+            size of each entry and the amount of memory available on the
+            system.
+        entry_list, **kwargs
+            keyword argument forwarded to :meth:`.load`.
+
+        Returns
+        -------
+        data
+            see :meth:`.load`.
+
+        Examples
+        --------
+        >>> for chunk in dl.next():
+        >>>    # 'chunk' has the same type of the output of dl.load()
+
+        See Also
+        --------
+        .load
+        """
+        if entry_list is None:
+            entry_list = self.build_entry_list(
+                tcm_level=kwargs.get("tcm_level", None), save_output_columns=True
+            )
+
+        start = stop = 0
+        etot = len(entry_list)
+        while stop < etot:
+            start = stop
+
+            if stop + chunk_size > etot:
+                stop = etot
+            else:
+                stop += chunk_size
+
+            yield self.load(
+                entry_list=entry_list[start:stop].reset_index(drop=True), **kwargs
+            )
+
     def load(
         self,
         entry_list: pd.DataFrame = None,
         in_memory: bool = True,
         output_file: str = None,
         orientation: str = "hit",
         tcm_level: str = None,
     ) -> None | Table | Struct | pd.DataFrame:
-        """Loads the requested columns in `self.output_columns` for the entries
-        in the given `entry_list`.
+        """Loads the requested data from disk.
+
+        Loads the requested columns in `self.output_columns` for the entries in
+        the given `entry_list`.
 
         Parameters
         ----------
         entry_list
-            the output of :meth:`.build_entry_list`.
+            the output of :meth:`.build_entry_list`. If ``None``, builds it
+            according to the current configuration.
         in_memory
             if ``True``, returns the loaded data in memory and stores in
             `self.data`.
         output_file
             if not ``None``, writes the loaded data to the specified file.
         orientation
             specifies the orientation of the output table. Can be ``hit`` or
@@ -871,99 +1005,51 @@
             child = None
             load_levels = [parent]
         else:
             parent = self.tcms[tcm_level]["parent"]
             child = self.tcms[tcm_level]["child"]
             load_levels = [parent, child]
 
-        def explode_evt_cols(el, tier_table):
+        def explode_evt_cols(el: pd.DataFrame, tier_table: Table):
             # Explode columns from "evt"-style levels, untested
             # Will only work if column has an "nda" attribute
             cum_length = build_cl(el[f"{child}_idx"])
             exp_cols = explode_arrays(
                 cum_length,
                 [a.nda for a in tier_table.values()],
             )
             tier_table.update(zip(tier_table.keys(), exp_cols))
             return tier_table
 
-        def fill_col_dict(tier_table, col_dict, tcm_idx):
-            # Put the information from the tier_table (after the columns have been exploded)
-            # into col_dict, which will be turned into the final Table
-            for col in tier_table.keys():
-                if isinstance(tier_table[col], Array):
-                    # Allocate memory for column for all channels
-                    if col not in col_dict.keys():
-                        col_dict[col] = np.empty(
-                            table_length,
-                            dtype=tier_table[col].dtype,
-                        )
-                    col_dict[col][tcm_idx] = tier_table[col].nda
-
-                elif isinstance(tier_table[col], WaveformTable):
-                    wf_table = tier_table[col]
-                    if isinstance(
-                        wf_table["values"],
-                        ArrayOfEqualSizedArrays,
-                    ):
-                        # Allocate memory for columns for all channels
-                        if "wf_dt" not in col_dict.keys():
-                            col_dict["wf_t0"] = np.empty(
-                                table_length,
-                                dtype=wf_table["t0"].dtype,
-                            )
-                            col_dict["wf_dt"] = np.empty(
-                                table_length,
-                                dtype=wf_table["dt"].dtype,
-                            )
-                            col_dict["wf_values"] = np.empty(
-                                (
-                                    table_length,
-                                    wf_table["values"].nda.shape[1],
-                                ),
-                                dtype=wf_table["values"].dtype,
-                            )
-                        col_dict["wf_t0"][tcm_idx] = wf_table["t0"].nda
-                        col_dict["wf_dt"][tcm_idx] = wf_table["dt"].nda
-                        col_dict["wf_values"][tcm_idx] = wf_table["values"].nda
-                    else:  # wf_values is a VectorOfVectors
-                        log.warning(
-                            "not sure how to handle waveforms with values "
-                            f"of type {type(tier_table[col]['values'])} yet"
-                        )
-                else:
-                    log.warning(
-                        f"not sure how to handle column {col} "
-                        f"of type {type(tier_table[col])} yet"
-                    )
-            return col_dict
-
         sto = LH5Store()
 
         if self.merge_files:
             tables = entry_list[f"{parent}_table"].unique()
             field_mask = []
             for col in self.output_columns:
                 if col not in entry_list.columns:
                     field_mask.append(col)
 
             col_tiers = self.get_tiers_for_col(field_mask)
             col_dict = entry_list.to_dict("list")
+            attr_dict = {}
+            for key in col_dict:
+                attr_dict[key] = None
             table_length = len(entry_list)
 
             for tb, level in product(tables, load_levels):
                 gb = entry_list.query(f"{parent}_table == {tb}").groupby("file")
                 files = list(gb.groups.keys())
                 el_idx = list(gb.groups.values())
                 idx_mask = [list(entry_list.loc[i, f"{level}_idx"]) for i in el_idx]
 
                 for tier in self.tiers[level]:
                     if tb not in col_tiers[tier]:
                         continue
-                    tb_name = self.get_table_name(tier, tb)
+                    tb_name = self.filedb.get_table_name(tier, tb)
                     tier_paths = [
                         os.path.join(
                             self.data_dir,
                             self.filedb.tier_dirs[tier].lstrip("/"),
                             self.filedb.df.iloc[file][f"{tier}_file"].lstrip("/"),
                         )
                         for file in files
@@ -975,24 +1061,25 @@
                         idx=idx_mask,
                         field_mask=field_mask,
                     )
 
                     if level == child:
                         explode_evt_cols(entry_list, tier_table)
 
-                    col_dict = fill_col_dict(
+                    col_dict, attr_dict = utils.fill_col_dict(
                         tier_table,
                         col_dict,
+                        attr_dict,
                         [idx for idx_list in el_idx for idx in idx_list],
+                        table_length,
+                        self.aoesa_to_vov,
                     )
+
             # Convert col_dict to lgdo.Table
-            for col in col_dict.keys():
-                nda = np.array(col_dict[col])
-                col_dict[col] = Array(nda=nda)
-            f_table = Table(col_dict=col_dict)
+            f_table = utils.dict_to_table(col_dict=col_dict, attr_dict=attr_dict)
 
             if output_file:
                 sto.write_object(f_table, "merged_data", output_file, wo_mode="o")
             if in_memory:
                 if self.output_format == "lgdo.Table":
                     return f_table
                 elif self.output_format == "pd.DataFrame":
@@ -1011,86 +1098,94 @@
                     total=len(entry_list),
                     delay=2,
                     unit=" keys",
                 )
 
             # now loop over the output of build_entry_list()
             for file, f_entries in entry_list.items():
-
                 if log.getEffectiveLevel() >= logging.INFO:
                     progress_bar.update()
-                    progress_bar.set_postfix(key=self.filedb.df.iloc[file]["timestamp"])
+                    progress_bar.set_postfix(
+                        key=self.filedb.df.iloc[file][self.filedb.sortby]
+                    )
 
                 log.debug(
-                    f"loading data for cycle key {self.filedb.df.iloc[file]['timestamp']}"
+                    f"loading data for cycle key {self.filedb.df.iloc[file][self.filedb.sortby]}"
                 )
 
                 field_mask = []
 
                 for col in self.output_columns:
                     if col not in f_entries.columns:
                         field_mask.append(col)
 
                 col_tiers = self.get_tiers_for_col(field_mask)
                 col_dict = f_entries.to_dict("list")
+                attr_dict = {}
+                for key in col_dict:
+                    attr_dict[key] = None
                 table_length = len(f_entries)
 
                 log.debug(f"will load new columns {field_mask}")
 
                 # loop through each table in entry list and
                 # loop through each level we're asked to load from
                 for tb, level in product(
                     f_entries[f"{parent}_table"].unique(), load_levels
                 ):
                     tcm_idx = f_entries.query(f"{parent}_table == {tb}").index
                     idx_mask = f_entries.loc[tcm_idx, f"{level}_idx"].tolist()
 
                     # loop over tiers in the level
                     for tier in self.tiers[level]:
-
                         if tb not in col_tiers[file]["tables"][tier]:
                             continue
 
                         log.debug(
-                            f"...for stream '{self.get_table_name(tier, tb)}' (at {level} level)"
+                            f"...for stream '{self.filedb.get_table_name(tier, tb)}' (at {level} level)"
                         )
 
                         # path to tier file
                         tier_path = os.path.join(
                             self.data_dir,
                             self.filedb.tier_dirs[tier].lstrip("/"),
                             self.filedb.df.iloc[file][f"{tier}_file"].lstrip("/"),
                         )
                         # this should not happen
                         if not os.path.exists(tier_path):
                             raise FileNotFoundError(tier_path)
 
-                        table_name = self.get_table_name(tier, tb)
+                        table_name = self.filedb.get_table_name(tier, tb)
                         tier_table, _ = sto.read_object(
                             table_name,
                             tier_path,
                             idx=idx_mask,
                             field_mask=field_mask,
                         )
+
                         if level == child:
                             explode_evt_cols(f_entries, tier_table)
 
-                        col_dict = fill_col_dict(tier_table, col_dict, tcm_idx)
+                        col_dict, attr_dict = utils.fill_col_dict(
+                            tier_table,
+                            col_dict,
+                            attr_dict,
+                            tcm_idx,
+                            table_length,
+                            self.aoesa_to_vov,
+                        )
                         # end tb loop
 
                 # Convert col_dict to lgdo.Table
-                for col in col_dict.keys():
-                    nda = np.array(col_dict[col])
-                    col_dict[col] = Array(nda=nda)
-                f_table = Table(col_dict=col_dict)
+                f_table = utils.dict_to_table(col_dict, attr_dict)
 
                 if in_memory:
                     load_out[file] = f_table
                 if output_file:
-                    sto.write_object(f_table, f"file{file}", output_file, wo_mode="o")
+                    sto.write_object(f_table, f"{file}", output_file, wo_mode="o")
                 # end file loop
 
             if log.getEffectiveLevel() >= logging.INFO:
                 progress_bar.close()
 
             if in_memory:
                 if self.output_format == "lgdo.Table":
@@ -1151,15 +1246,15 @@
                                     self.data_dir,
                                     self.filedb.tier_dirs[tier].lstrip("/"),
                                     self.filedb.df.iloc[file][f"{tier}_file"].lstrip(
                                         "/"
                                     ),
                                 )
                                 if os.path.exists(tier_path):
-                                    table_name = self.get_table_name(tier, tb)
+                                    table_name = self.filedb.get_table_name(tier, tb)
                                     tier_table, _ = sto.read_object(
                                         table_name,
                                         tier_path,
                                         idx=idx_mask,
                                         field_mask=field_mask,
                                     )
                                     for col in tier_table.keys():
@@ -1181,14 +1276,103 @@
                         load_out[file] = load_out[file].get_dataframe()
                     return load_out
                 else:
                     raise ValueError(
                         f"'{self.output_format}' output format not supported"
                     )
 
+    def load_iterator(
+        self,
+        entry_list: pd.DataFrame = None,
+        tcm_level: str = None,
+        buffer_len: int = 3200,
+    ) -> LH5Iterator:
+        """Creates an :class:LH5Iterator that will load the requested columns
+        in `self.output_columns` for the entries in the given `entry_list` in
+        chunks. This is more memory efficient than filling a whole table and
+        is recommended for use when loading waveforms.
+
+        Parameters
+        ----------
+        entry_list
+            the output of :meth:`.build_entry_list`. If ``None``, builds it
+            according to the current configuration.
+        tcm_level
+            which TCM was used to create the ``entry_list``.
+        buffer_len
+            how many entries to load in a single chunk
+
+        Returns
+        -------
+        data
+            LH5 Iterator, which yields (lh5 table, entry, n_entries) when
+            iterated over.
+        """
+        if entry_list is None:
+            entry_list = self.build_entry_list(
+                tcm_level=tcm_level, save_output_columns=True
+            )
+
+        if tcm_level is None:
+            parent = self.levels[0]
+            child = None
+            load_levels = [parent]
+        else:
+            parent = self.tcms[tcm_level]["parent"]
+            child = self.tcms[tcm_level]["child"]
+            load_levels = [parent, child]
+
+        if self.merge_files:
+            tables = entry_list[f"{parent}_table"].unique()
+            field_mask = []
+            for col in self.output_columns:
+                if col not in entry_list.columns:
+                    field_mask.append(col)
+
+            col_tiers = self.get_tiers_for_col(field_mask)
+
+            lh5_it = None
+            for level in load_levels:
+                for tier in self.tiers[level]:
+                    # Build list of files/tables/entries
+                    lh5_files = []
+                    tb_names = []
+                    idx_list = []
+                    for tb in tables:
+                        if tb not in col_tiers[tier]:
+                            continue
+                        gb = entry_list.query(f"{parent}_table == {tb}").groupby("file")
+                        lh5_files += [
+                            os.path.join(
+                                self.filedb.tier_dirs[tier].lstrip("/"),
+                                self.filedb.df.iloc[file][f"{tier}_file"].lstrip("/"),
+                            )
+                            for file in gb.groups.keys()
+                        ]
+                        tb_names += [self.filedb.get_table_name(tier, tb)] * len(gb)
+                        idx_list += [
+                            list(entry_list.loc[i, f"{level}_idx"])
+                            for i in gb.groups.values()
+                        ]
+
+                    # Create iterator for this tier and friend to other tiers
+                    lh5_it = LH5Iterator(
+                        lh5_files=lh5_files,
+                        groups=tb_names,
+                        base_path=self.data_dir,
+                        entry_list=idx_list,
+                        field_mask=field_mask,
+                        buffer_len=buffer_len,
+                        friend=lh5_it,
+                    )
+
+            return lh5_it
+        else:  # not merge_files
+            raise NotImplementedError
+
     def load_detector(self, det_id):
         """
         special version of `load` designed to retrieve all file files, tables,
         column names, and potentially calibration/dsp parameters relevant to one
         single detector.
         """
         raise NotImplementedError
@@ -1215,21 +1399,94 @@
 
     def skim_waveforms(self, mode: str = "hit", hit_list=None, evt_list=None):
         """
         handle this one separately because waveforms can easily fill up memory.
         """
         raise NotImplementedError
 
-    def browse(self, query, dsp_config=None):
+    # TODO: automatically get the dsp_config/par_database used for
+    #   processing when these are set to None
+    def browse(
+        self,
+        entry_list: pd.DataFrame = None,
+        dsp_config=None,
+        par_database: str | dict = None,
+        aux_values: pd.DataFrame = None,
+        lines: str | list[str] = "waveform",
+        styles: dict[str, list] | str = None,
+        legend: str | list[str] = None,
+        legend_opts: dict = None,
+        n_drawn: int = 1,
+        x_unit: pint.Unit | str = None,  # noqa: F821
+        x_lim: tuple[float | str | pint.Quantity] = None,  # noqa: F821
+        y_lim: tuple[float | str | pint.Quantity] = None,  # noqa: F821
+        norm: str = None,
+        align: str = None,
+        buffer_len: int = 128,
+        block_width: int = 8,
+    ):
         """
-        Interface between DataLoader and WaveformBrowser.
+        Interface between :class:DataLoader and :class:WaveformBrowser.
         """
-        raise NotImplementedError
+        if entry_list is None:
+            entry_list = self.build_entry_list()
+
+        parent = self.levels[0]
+        tables = entry_list[f"{parent}_table"].unique()
+
+        lh5_it = None
+        for tier in self.tiers[parent]:
+            # Build list of files/tables/entries
+            lh5_files = []
+            tb_names = []
+            idx_list = []
+            for tb in tables:
+                gb = entry_list.query(f"{parent}_table == {tb}").groupby("file")
+                lh5_files += [
+                    os.path.join(
+                        self.filedb.tier_dirs[tier].lstrip("/"),
+                        self.filedb.df.iloc[file][f"{tier}_file"].lstrip("/"),
+                    )
+                    for file in gb.groups.keys()
+                ]
+                tb_names += [self.filedb.get_table_name(tier, tb)] * len(gb)
+                idx_list += [
+                    list(entry_list.loc[i, f"{parent}_idx"]) for i in gb.groups.values()
+                ]
+
+            # Create iterator for this tier and friend to other tiers
+            lh5_it = LH5Iterator(
+                lh5_files=lh5_files,
+                groups=tb_names,
+                base_path=self.data_dir,
+                entry_list=idx_list,
+                buffer_len=buffer_len,
+                field_mask={"tracelist": False},
+                friend=lh5_it,
+            )
+
+        return WaveformBrowser(
+            lh5_it,
+            dsp_config=dsp_config,
+            database=par_database,
+            aux_values=aux_values,
+            lines=lines,
+            styles=styles,
+            legend=legend,
+            legend_opts=legend_opts,
+            n_drawn=n_drawn,
+            x_unit=x_unit,
+            x_lim=x_lim,
+            y_lim=y_lim,
+            norm=norm,
+            align=align,
+            buffer_len=buffer_len,
+            block_width=block_width,
+        )
 
-    # -------------- Helper Functions ----------------#
     def get_tiers_for_col(
         self, columns: list | np.ndarray, merge_files: bool = None
     ) -> dict:
         """For each column given, get the tiers and tables in that tier where
         that column can be found.
 
         Parameters
@@ -1306,33 +1563,17 @@
                                         set(self.filedb.columns[col_idx]), set(columns)
                                     )
                                     for c in col_in_tier:
                                         col_tiers[file]["columns"][c] = tier
 
         return col_tiers
 
-    def get_table_name(self, tier: str, tb: str) -> str:
-        """Get the table name for a tier given its table identifier.
-
-        Parameters
-        ----------
-        tier
-            specify the tier whose table format will be used.
-        tb
-            the table identifier that will be passed to the table format.
-
-        Returns
-        -------
-        table_name
-            the name of the table in `tier` with table identifier `tb`
-        """
-        template = self.filedb.table_format[tier]
-        fm = string.Formatter()
-        parse_arr = np.array(list(fm.parse(template)))
-        names = list(parse_arr[:, 1])
-        if len(names) > 0:
-            keyword = names[0]
-            args = {keyword: tb}
-            table_name = template.format(**args)
-        else:
-            table_name = template
-        return table_name
+    def __repr__(self) -> str:
+        return (
+            "DataLoader("
+            f"cuts={self.cuts}, "
+            f"merge_files={self.merge_files}, "
+            f'output_format="{self.output_format}", '
+            f"output_columns={self.output_columns}, "
+            f"aoesa_to_vov={self.aoesa_to_vov}"
+            ")"
+        )
```

### Comparing `pygama-1.2.0/src/pygama/flow/datagroup.py` & `pygama-1.3.0/src/pygama/pargen/dsp_optimize.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,321 +1,379 @@
-#!/usr/bin/env python3
-import itertools
-import json
-import os
-from collections import OrderedDict
-from pathlib import Path
-from string import Formatter
+import logging
+import multiprocessing as mp
+from collections import namedtuple
+from multiprocessing import get_context
+from pprint import pprint
 
-import pandas as pd
-from parse import parse
+import numpy as np
 
+from pygama.dsp import build_processing_chain
 
-class DataGroup:
-    """
-    A class to create an in-memory or on-disk set of files, according to the
-    LEGEND data convention.  Typically requires a JSON config file with:
+log = logging.getLogger(__name__)
 
-      - path to DAQ and LH5 directories
-      - format strings for daq/lh5 files
-      - partitions for the LH5 data directory
 
-    Reference: https://docs.legend-exp.org/index.php/apps/files/?dir=/LEGEND%20Documents/Technical%20Documents/Analysis&fileid=9140#pdfviewer
+def run_one_dsp(
+    tb_data, dsp_config, db_dict=None, fom_function=None, verbosity=0, fom_kwargs=None
+):
     """
-    def __init__(self, config=None, nfiles=None, load=False):
-        """
-        DOCME
-        """
-        # master table
-        self.fileDB = None
+    run one iteration of DSP on tb_data
 
-        # typical usage: JSON config file
-        if config is not None:
-            self.set_config(os.path.expandvars(config))
+    Optionally returns a value for optimization
 
-        # limit number of files (useful for debug & testing)
-        self.nfiles = nfiles
+    Parameters
+    ----------
+    tb_data : lh5 Table
+        An input table of lh5 data. Typically a selection is made prior to
+        sending tb_data to this function: optimization typically doesn't have to
+        run over all data
+    dsp_config : dict
+        Specifies the DSP to be performed for this iteration (see
+        build_processing_chain()) and the list of output variables to appear in
+        the output table
+    db_dict : dict (optional)
+        DSP parameters database. See build_processing_chain for formatting info
+    fom_function : function or None (optional)
+        When given the output lh5 table of this DSP iteration, the
+        fom_function must return a scalar figure-of-merit value upon which the
+        optimization will be based. Should accept verbosity as a second argument
+    verbosity : int (optional)
+        verbosity for the processing chain and fom_function calls
+    fom_kwargs
+        any keyword arguments to pass to the fom
+
+    Returns
+    -------
+    figure_of_merit : float
+        If fom_function is not None, returns figure-of-merit value for the DSP iteration
+    tb_out : lh5 Table
+        If fom_function is None, returns the output lh5 table for the DSP iteration
+    """
 
-        # load a pre-existing set of keys.  should be True by default
-        if load:
-            self.load_df()
+    pc, lh5_col_names, tb_out = build_processing_chain(
+        tb_data, dsp_config, db_dict=db_dict
+    )
+    pc.execute()
+    if fom_function is not None:
+        if fom_kwargs is not None:
+            return fom_function(tb_out, verbosity, fom_kwargs)
+        else:
+            return fom_function(tb_out, verbosity)
+    else:
+        return tb_out
+
+
+ParGridDimension = namedtuple("ParGridDimension", "name parameter value_strs")
+
+
+class ParGrid:
+    """Parameter Grid class
+    Each ParGrid entry corresponds to a dsp parameter to be varied.
+    The ntuples must follow the pattern:
+    ( name parameter value_strs) : ( str, str, list of str)
+    where name and parameter are the same as 'db.name.parameter' in the processing chain,
+    value_strs is the array of strings to set the argument to.
+    """
 
+    def __init__(self):
+        self.dims = []
 
-    def set_config(self, config):
-        """
-        DOCME
-        """
-        with open(config) as f:
-            self.config = json.load(f)
+    def add_dimension(self, name, parameter, value_strs):
+        self.dims.append(ParGridDimension(name, parameter, value_strs))
 
-        # experiment name
-        self.experiment = self.config['experiment']
+    def get_n_dimensions(self):
+        return len(self.dims)
 
-        # experiment-specific runDB.  optional but recommended
-        self.f_runDB = os.path.expandvars(self.config['runDB'])
-        if os.path.exists(self.f_runDB):
-            with open(self.f_runDB) as f:
-                self.runDB = json.load(f, object_pairs_hook=OrderedDict)
-
-        # experiment-specific fileDB (h5 list of file keys)
-        self.f_fileDB = os.path.expandvars(self.config['fileDB'])
-        self.config['fileDB'] = os.path.expandvars(self.config['fileDB'])
-
-        # set DAQ data directory
-        self.daq_dir = os.path.expandvars(self.config['daq_dir'])
-        self.daq_ignore = self.config['daq_ignore']
-        if not os.path.isdir(self.daq_dir):
-            print('Warning, DAQ directory not found:', self.daq_dir)
-
-        # set LH5 data directory
-        self.lh5_dir = os.path.expandvars(self.config['lh5_dir'])
-        if not os.path.isdir(self.lh5_dir):
-            print('Warning, LH5 directory not found:', self.lh5_dir)
-
-        # optional: set a user directory (useful for testing file processing)
-        if 'lh5_user' in self.config:
-            self.lh5_user_dir = os.path.expandvars(self.config['lh5_user'])
-            if not os.path.isdir(self.lh5_user_dir):
-                print('Warning, LH5 user directory not found:', self.lh5_user_dir)
-
-        # optional: run selection json file
-        if 'runSelectionDB' in self.config:
-            f_runsel = os.path.expandvars(self.config['runSelectionDB'])
-            if not os.path.exists(f_runsel):
-                print('Warning, run selection file not found:', f_runsel)
+    def get_n_points_of_dim(self, i):
+        return len(self.dims[i].value_strs)
+
+    def get_shape(self):
+        shape = ()
+        for i in range(self.get_n_dimensions()):
+            shape += (self.get_n_points_of_dim(i),)
+        return shape
+
+    def get_n_grid_points(self):
+        return np.prod(self.get_shape())
+
+    def get_par_meshgrid(self, copy=False, sparse=False):
+        """return a meshgrid of parameter values
+        Always uses Matrix indexing (natural for par grid) so that
+        mg[i1][i2][...] corresponds to index order in self.dims
+        Note copy is False by default as opposed to numpy default of True
+        """
+        axes = []
+        for i in range(self.get_n_dimensions()):
+            axes.append(self.dims[i].values_strs)
+        return np.meshgrid(*axes, copy, sparse, indexing="ij")
+
+    def get_zero_indices(self):
+        return np.zeros(self.get_n_dimensions(), dtype=np.uint32)
+
+    def iterate_indices(self, indices):
+        """iterate given indices [i1, i2, ...] by one.
+        For easier iteration. The convention here is arbitrary, but its the
+        order the arrays would be traversed in a series of nested for loops in
+        the order appearin in dims (first dimension is first for loop, etc):
+        Return False when the grid runs out of indices. Otherwise returns True.
+        """
+        for iD in reversed(range(self.get_n_dimensions())):
+            indices[iD] += 1
+            if indices[iD] < self.get_n_points_of_dim(iD):
+                return True
+            indices[iD] = 0
+        return False
+
+    # def check_indices(self, indices):
+    #    for iD in reversed(range(self.get_n_dimensions())):
+    #        if indices[iD] < self.get_n_points_of_dim(iD): return True
+    #        indices[iD] = 0
+    #    return False
+
+    def get_data(self, i_dim, i_par):
+        name = self.dims[i_dim].name
+        parameter = self.dims[i_dim].parameter
+        value_str = self.dims[i_dim].value_strs[i_par]
+        return name, parameter, value_str
+
+    def print_data(self, indices):
+        print_string = f"Grid point at indices {indices}:"
+        for i_dim, i_par in enumerate(indices):
+            name, parameter, value_str = self.get_data(i_dim, i_par)
+            print_string += f"\n {name}.{parameter} = {value_str}"
+        return print_string
+
+    def set_dsp_pars(self, db_dict, indices):
+        if db_dict is None:
+            db_dict = {}
+        for i_dim, i_par in enumerate(indices):
+            name, parameter, value_str = self.get_data(i_dim, i_par)
+            if name not in db_dict.keys():
+                db_dict[name] = {parameter: value_str}
             else:
-                with open(f_runsel) as f:
-                    self.runSelectionDB = json.load(f)
-
-        # get LH5 subdirectory names
-        self.tier_dirs = self.config['tier_dirs']
-        self.subsystems = self.config['subsystems']
-        self.run_types = self.config['run_types']
-        self.evt_dirs = self.config['evt_dirs']
-
-        # get format strings for unique keys, DAQ files, and LH5 files
-        self.unique_key = self.config['unique_key']
-        self.daq_template = self.config['daq_template']
-        self.lh5_template = self.config['lh5_template']
-
-
-    def lh5_dir_setup(self, user_dir=False):
-        """
-        generate paths to LH5 data directories, using `self.lh5_dir`
-        if user_dir is True, create them in `self.lh5_user` instead.
-        """
-        dirs = []
-        lh5_dir = self.lh5_user if user_dir else self.lh5_dir
+                db_dict[name][parameter] = value_str
+        return db_dict
 
-        # directories for hit-level data
-        t, r, s = self.tier_dirs, self.run_types, self.subsystems
-        for tier, subs, rtp in itertools.product(t, s, r):
-            dirname = f'{lh5_dir}/{tier}/{subs}/{rtp}'
-            print(dirname)
-            dirs.append(dirname)
-
-        # directories for event-level data
-        for dir in self.evt_dirs:
-            dirname = f'{lh5_dir}/{dir}'
-            print(dirname)
-            dirs.append(dirname)
-
-        print('Base LH5 path:', lh5_dir)
-        ans = input('Create directories here? (y/n)')
-        if ans.lower() == 'y':
-            for d in dirs:
-                Path(d).mkdir(parents=True, exist_ok=True)
 
+def run_grid(
+    tb_data, dsp_config, grid, fom_function, db_dict=None, verbosity=1, **fom_kwargs
+):
+    """Extract a table of optimization values for a grid of DSP parameters
+    The grid argument defines a list of parameters and values over which to run
+    the DSP defined in dsp_config on tb_data. At each point, a scalar
+    figure-of-merit is extracted.
+
+    Returns a N-dimensional ndarray of figure-of-merit values, where the array
+    axes are in the order they appear in grid.
+
+    Parameters
+    ----------
+    tb_data : lh5 Table
+        An input table of lh5 data. Typically a selection is made prior to
+        sending tb_data to this function: optimization typically doesn't have to
+        run over all data
+    dsp_config : dict
+        Specifies the DSP to be performed (see build_processing_chain()) and the
+        list of output variables to appear in the output table for each grid point
+    grid : ParGrid
+        See ParGrid class for format
+    fom_function : function
+        When given the output lh5 table of this DSP iteration, the fom_function
+        must return a scalar figure-of-merit. Should accept verbosity as a
+        second keyword argument
+    db_dict : dict (optional)
+        DSP parameters database. See build_processing_chain for formatting info
+    verbosity : int (optional)
+        verbosity for the processing chain and fom_function calls
+    **fom_kwargs
+        Any keyword arguments for fom_function
+
+    Returns
+    -------
+    grid_values : ndarray of floats
+        An N-dimensional numpy ndarray whose Mth axis corresponds to the Mth row
+        of the grid argument
+    """
 
-    def scan_daq_dir(self, verbose=False):
-        """
-        scan the DAQ directory and build a DataFrame of file keys.
-        don't make any experiment-specific choices here.
-        """
-        dt = self.daq_template
-        di = self.daq_ignore
-
-        file_keys = []
-        stop_walk = False
-        n_files = 0
-
-        for path, folders, files in os.walk(self.daq_dir):
-
-            n_files += len(files)
-
-            for f in files:
-
-                # in some cases, we need information from the path name
-                if '/' in self.daq_template:
-                    f_tmp = path.replace(self.daq_dir,'') + '/' + f
+    grid_values = np.ndarray(shape=grid.get_shape(), dtype="O")
+    iii = grid.get_zero_indices()
+    log.info("starting grid calculations...")
+    while True:
+        db_dict = grid.set_dsp_pars(db_dict, iii)
+        if verbosity > 1:
+            pprint(dsp_config)
+        log.debug(grid.print_data(iii))
+        grid_values[tuple(iii)] = run_one_dsp(
+            tb_data,
+            dsp_config,
+            db_dict=db_dict,
+            fom_function=fom_function,
+            verbosity=verbosity,
+            fom_kwargs=fom_kwargs,
+        )
+        log.debug("value:", grid_values[tuple(iii)])
+        if not grid.iterate_indices(iii):
+            break
+    return grid_values
+
+
+def run_grid_point(
+    tb_data,
+    dsp_config,
+    grids,
+    fom_function,
+    iii,
+    db_dict=None,
+    verbosity=1,
+    fom_kwargs=None,
+):
+    """
+    Runs a single grid point for the index specified
+    """
+    if not isinstance(grids, list):
+        grids = [grids]
+    for index, grid in zip(iii, grids):
+        db_dict = grid.set_dsp_pars(db_dict, index)
+
+    log.debug(db_dict)
+    for i, grid in enumerate(grids):
+        log.debug(grid.print_data(iii[i]))
+    tb_out = run_one_dsp(tb_data, dsp_config, db_dict=db_dict, verbosity=verbosity)
+    res = np.ndarray(shape=len(grids), dtype="O")
+    if fom_function:
+        for i in range(len(grids)):
+            if fom_kwargs[i] is not None:
+                if len(fom_function) > 1:
+                    res[i] = fom_function[i](tb_out, verbosity, fom_kwargs[i])
                 else:
-                    f_tmp = f
-
-                # check if we should ignore this file
-                if len(di) > 0 and any(ig in f_tmp for ig in di):
-                    continue
-
-                finfo = parse(self.daq_template, f_tmp)
-                if finfo is not None:
-                    finfo = finfo.named # convert to dict
-                    finfo['daq_dir'] = path.replace(self.daq_dir,'') # sub-dir
-                    finfo['daq_file'] = f
-                    file_keys.append(finfo)
-
-                # limit number of files (debug mode)
-                if self.nfiles is not None and len(file_keys) >= self.nfiles:
-                    stop_walk = True
-                if stop_walk:
-                    break
-            if stop_walk:
-                break
-
-        if n_files == 0:
-            print("no daq files found...")
-            return
-
-        if len(file_keys) == 0:
-            print("no daq files matched pattern", self.daq_template)
-            return
-
-        # create the main DataFrame
-        self.fileDB = pd.DataFrame(file_keys)
-
-        # grab the unique key and sort the DataFrame by it
-        fk = lambda x: self.unique_key.format_map(x)
-        self.fileDB['unique_key'] = self.fileDB.apply(fk, axis=1)
-
-        # reorder cols to match the daq_template string
-        cols = ['unique_key']
-        cols.extend([fn for _,fn,_,_ in Formatter().parse(dt) if fn is not None])
-        cols.extend(['daq_dir','daq_file'])
-        self.fileDB = self.fileDB[cols]
-
-        # convert cols to numeric dtypes where possible
-        for col in self.fileDB.columns:
-            if col != 'YYmmdd' and col != 'hhmmss':
-             try:
-                self.fileDB[col] = pd.to_numeric(self.fileDB[col])
-             except:
-                pass
-
-        if verbose:
-            print(self.fileDB.to_string())
-
-
-    def save_keys(self, fname=None):
-        """
-        default: save the unique_key and the relative path to the DAQ file,
-        as a CSV file.  this will probably change in the future, but at least
-        this way we can:
-
-          - easily get a list of available DAQ files
-          - regenerate the DataFrame from scan_daq_dir by parsing format string
-        """
-        if fname is None:
-            fname = self.f_fileDB
-        print('Saving file key list to: ', fname)
-
-        df_keys = self.fileDB
-        df_keys['rel_daq_path'] = df_keys['daq_dir'] + '/' + df_keys['daq_file']
-
-        # export to csv
-        df_keys[['unique_key','rel_daq_path']].to_csv(fname, index=False)
-
-
-    def load_keys(self, fname=None):
-        """
-        load a list of file keys and parse data into columns according to
-        the format string
-        """
-        if fname is None:
-            fname = self.f_fileDB
-        print('Loading file key list from:', fname)
-
-        df_keys = pd.read_csv(fname)
-
-        dt = self.daq_template
-        cols = [fn for _,fn,_,_ in Formatter().parse(dt) if fn is not None]
-
-        def parse_key(row):
-            """ extract variables from format string from daq_path """
-            tmp = row['rel_daq_path'].split('/')
-            daq_dir = '/'.join(t for t in tmp[:-1])
-            daq_file = tmp[-1]
-            unique_key = row['unique_key']
-            if '/' in self.daq_template:
-                finfo = parse(self.daq_template, row['rel_daq_path']).named
+                    res[i] = fom_function[0](tb_out, verbosity, fom_kwargs[i])
             else:
-                finfo = parse(self.daq_template, daq_file).named
-            row = pd.Series(finfo)
-            row['unique_key'] = unique_key
-            row['daq_dir'] = daq_dir
-            row['daq_file'] = daq_file
-            return row
-
-        self.fileDB = df_keys.apply(parse_key, axis=1)
-
-        # reorder cols to match the daq_template string
-        cols = ['unique_key']
-        cols.extend([fn for _,fn,_,_ in Formatter().parse(dt) if fn is not None])
-        cols.extend(['daq_dir','daq_file'])
-        self.fileDB = self.fileDB[cols]
-
-
-    def save_df(self, fname=None):
-        """
-        save the current self.fileDB dataframe. If we've added extra columns
-        specific to an experiment (outside this class), this will preserve them.
-        """
-        if fname is None:
-            fname = self.f_fileDB
-        print('Saving file key list to: ', fname)
-        # self.fileDB.to_json(fname, indent=2)
-        self.fileDB.to_hdf(fname, key='file_keys')
+                if len(fom_function) > 1:
+                    res[i] = fom_function[i](tb_out, verbosity)
+                else:
+                    res[i] = fom_function[0](tb_out, verbosity)
+        log.debug("value:", res)
+        out = {"indexes": [tuple(ii) for ii in iii], "results": res}
 
-
-    def load_df(self, fname=None):
-        """
-        DOCME
-        """
-        if fname is None: fname = self.f_fileDB
-        self.fileDB = pd.read_hdf(fname, key='file_keys')
+    else:
+        out = {"indexes": [tuple(ii) for ii in iii], "results": tb_out}
+    return out
 
 
-    def get_lh5_cols(self):
-        """
-        compute the LH5 filenames.
+def get_grid_points(grid):
+    """
+    Generates a list of the indices of all possible grid points
+    """
+    out = []
+    iii = [gri.get_zero_indices() for gri in grid]
+    complete = np.full(len(grid), False)
+    while True:
+        out.append([tuple(ii) for ii in iii])
+
+        for i, gri in enumerate(zip(iii, grid)):
+            if not gri[1].iterate_indices(gri[0]):
+                log.info(f"{i} grid end")
+                iii[i] = gri[1].get_zero_indices()
+                complete[i] = True
+        if all(complete):
+            break
+    return out
+
+
+def run_grid_multiprocess_parallel(
+    tb_data,
+    dsp_config,
+    grid,
+    fom_function,
+    db_dict=None,
+    verbosity=1,
+    processes=5,
+    fom_kwargs=None,
+):
+    """
+    run one iteration of DSP on tb_data with multiprocessing, can handle
+    multiple grids if they are the same dimensions
 
-        need to generate the file names, and then figure out which folder
-        to store them in.  probably best to separate these tasks
-        """
-        if 'runtype' not in self.fileDB.columns:
-            print("You must add a 'runtype' column to the file key DF.")
-            exit()
-
-        def get_files(row):
-            tmp = row.to_dict()
-            for tier in self.tier_dirs:
-
-                # get filename
-                tmp['tier'] = tier
-
-                # leave subsystem unspecified
-                if self.subsystems != ['']:
-                    tmp['sysn'] = '{sysn}'
-
-                # set the filename.  might have a '{sysn}' string present
-                row[f'{tier}_file'] = self.lh5_template.format_map(tmp)
-
-                # compute file path.
-                # daq_to_raw outputs a file for each subsystem, and we
-                # handle this here by leaving a regex in the file string
-                path = f'/{tier}'
-                if self.subsystems != [""]:
-                    path += '/{sysn}'
-                if row['runtype'] in self.run_types:
-                    path += f"/{row['runtype']}"
+    Optionally returns a value for optimization
 
-                row[f'{tier}_path'] = path
-            return row
+    Parameters
+    ----------
+    tb_data : lh5 Table
+        An input table of lh5 data. Typically a selection is made prior to
+        sending tb_data to this function: optimization typically doesn't have to
+        run over all data
+    dsp_config : dict
+        Specifies the DSP to be performed for this iteration (see
+        build_processing_chain()) and the list of output variables to appear in
+        the output table
+    grid : pargrid, list of pargrids
+        Grids to run optimization on
+    db_dict : dict (optional)
+        DSP parameters database. See build_processing_chain for formatting info
+    fom_function : function or None (optional)
+        When given the output lh5 table of this DSP iteration, the
+        fom_function must return a scalar figure-of-merit value upon which the
+        optimization will be based. Should accept verbosity as a second argument.
+        If multiple grids provided can either pass one fom to have it run for each grid
+        or a list of fom to run different fom on each grid.
+    verbosity : int (optional)
+        verbosity for the processing chain and fom_function calls
+    processes : int
+        DOCME
+    fom_kwargs
+        any keyword arguments to pass to the fom,
+        if multiple grids given will need to be a list of the fom_kwargs for each grid
+
+    Returns
+    -------
+    figure_of_merit : float
+        If fom_function is not None, returns figure-of-merit value for the DSP iteration
+    tb_out : lh5 Table
+        If fom_function is None, returns the output lh5 table for the DSP iteration
+    """
 
-        self.fileDB = self.fileDB.apply(get_files, axis=1)
+    if not isinstance(grid, list):
+        grid = [grid]
+    if not isinstance(fom_function, list) and fom_function is not None:
+        fom_function = [fom_function]
+    if not isinstance(fom_kwargs, list):
+        fom_kwargs = [fom_kwargs for gri in grid]
+    grid_values = []
+    shapes = [gri.get_shape() for gri in grid]
+    if fom_function is not None:
+        for i in range(len(grid)):
+            grid_values.append(np.ndarray(shape=shapes[i], dtype="O"))
+    else:
+        grid_lengths = np.array([gri.get_n_grid_points() for gri in grid])
+        grid_values.append(np.ndarray(shape=shapes[np.argmax(grid_lengths)], dtype="O"))
+    grid_list = get_grid_points(grid)
+    pool = mp.Pool(processes=processes)
+    results = [
+        pool.apply_async(
+            run_grid_point,
+            args=(
+                tb_data,
+                dsp_config,
+                grid,
+                fom_function,
+                np.asarray(gl),
+                db_dict,
+                verbosity,
+                fom_kwargs,
+            ),
+        )
+        for gl in grid_list
+    ]
+
+    for result in results:
+        res = result.get()
+        indexes = res["indexes"]
+        if fom_function is not None:
+            for i in range(len(grid)):
+                index = indexes[i]
+                if grid_values[i][index] is None:
+                    grid_values[i][index] = res["results"][i]
+        else:
+            grid_values[0][indexes[0]] = {f"{indexes[0]}": res["results"]}
+
+    pool.close()
+    pool.join()
+    return grid_values
```

### Comparing `pygama-1.2.0/src/pygama/flow/file_db.py` & `pygama-1.3.0/src/pygama/flow/file_db.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,29 @@
-"""
-Utilities for LH5 file inventory.
-"""
+"""Utilities for LH5 file inventory."""
 from __future__ import annotations
 
 import json
 import logging
 import os
 import re
 import string
 import warnings
-from datetime import datetime, timezone
 
 import h5py
 import numpy as np
 import pandas as pd
 from parse import parse
 
-from pygama.lgdo import Array, LH5Store, Scalar, VectorOfVectors
-from pygama.lgdo.lh5_store import ls
+from pygama import lgdo
+from pygama.lgdo import Array, Scalar, VectorOfVectors
+from pygama.lgdo import lh5_store as lh5
 
-log = logging.getLogger(__name__)
-
-
-def to_datetime(key: str) -> datetime:
-    """Convert LEGEND cycle key to :class:`~datetime.datetime`.
-
-    Assumes `key` is formatted as ``YYYYMMDDTHHMMSSZ`` (UTC).
-    """
-    m = re.match(r"^(\d{4})(\d{2})(\d{2})T(\d{2})(\d{2})(\d{2})Z$", key)
-    if m is None:
-        raise ValueError(f"Could not parse '{key}' as a datetime object")
-    else:
-        g = [int(el) for el in m.groups()]
-        return datetime(*g, tzinfo=timezone.utc)
+from . import utils
 
-
-def to_unixtime(key: str) -> int:
-    """Convert LEGEND cycle key to `POSIX timestamp <https://en.wikipedia.org/wiki/Unix_time>`_."""
-    return int(to_datetime(key).timestamp())
+log = logging.getLogger(__name__)
 
 
 class FileDB:
     """LH5 file database.
 
     A class containing a :class:`pandas.DataFrame` that has additional
     functions to scan the data directory, fill the dataframe's columns with
@@ -110,46 +92,54 @@
     :class:`FileDB` objects can be also stored on disk and read-in at later
     times.
 
     Examples
     --------
     >>> from pygama.flow import FileDB
     >>> db = FileDB("./filedb_config.json")
-    >>> db.get_tables_columns()  # read in also table columns names
+    >>> db.scan_tables_columns()  # read in also table columns names
     >>> print(db)
     << Columns >>
     [['baseline', 'card', 'ch_orca', 'channel', 'crate', 'daqenergy', 'deadtime', 'dr_maxticks', 'dr_start_pps', 'dr_start_ticks', 'dr_stop_pps', 'dr_stop_ticks', 'eventnumber', 'fcid', 'numtraces', 'packet_id', 'runtime', 'timestamp', 'to_abs_mu_usec', 'to_dt_mu_usec', 'to_master_sec', 'to_mu_sec', 'to_mu_usec', 'to_start_sec', 'to_start_usec', 'tracelist', 'ts_maxticks', 'ts_pps', 'ts_ticks', 'waveform'], ['bl_intercept', 'bl_mean', 'bl_slope', 'bl_std', 'tail_slope', 'tail_std', 'wf_blsub'], ['array_id', 'array_idx', 'cumulative_length']]
     << DataFrame >>
        exp period   run         timestamp type  ... hit_col_idx tcm_tables tcm_col_idx evt_tables evt_col_idx
     0  l60    p01  r014  20220716T105236Z  cal  ...        None         []         [2]       None        None
     1  l60    p01  r014  20220716T104550Z  cal  ...        None         []         [2]       None        None
     >>> db.to_disk("file_db.lh5")
     """
 
-    def __init__(self, config: str | dict, scan: bool = True) -> None:
+    def __init__(self, config: str | dict | list[str], scan: bool = True) -> None:
         """
         Parameters
         ----------
         config
             dictionary or path to JSON file specifying data directories, tiers,
-            and file name templates. Can also be path to existing LH5 file
-            containing :class:`FileDB` object serialized by :meth:`.to_disk()`.
+            and file name templates. Can also be path (or list of paths or
+            regular expression) to existing LH5 file containing :class:`FileDB`
+            object serialized by :meth:`.to_disk()`.
         scan
             whether the file database should scan the directory containing
             `raw` files to fill its rows with file keys.
         """
+        self.df = None
+
         config_path = None
         if isinstance(config, str):
-            if h5py.is_hdf5(config):
-                self.from_disk(config)
-                return
-            else:
-                config_path = config
+            config_path = config
+            try:
                 with open(config) as f:
                     config = json.load(f)
+            # can otherwise be (wildcard of) HDF5 file(s)
+            except (FileNotFoundError, json.JSONDecodeError, UnicodeDecodeError):
+                self.from_disk(config)
+                return
+
+        elif isinstance(config, list):
+            self.from_disk(config)
+            return
 
         if not isinstance(config, dict):
             raise ValueError("Bad FileDB configuration value")
 
         self.set_config(config, config_path)
 
         # Set up column names
@@ -164,20 +154,18 @@
 
         self.df = pd.DataFrame(columns=names)
 
         self.columns = None
 
         if scan:
             self.scan_files()
-            self.set_file_status()
-            self.set_file_sizes()
 
             # Use config columns and tables if provided
             if "columns" in self.config.keys() and "tables" in self.config.keys():
-                log.info("Setting columns/tables from config")
+                log.debug("setting columns/tables from config")
                 self.columns = list(self.config["columns"].values())
                 for tier in self.tiers:
                     self.df[f"{tier}_tables"] = [self.config["tables"][tier]] * len(
                         self.df
                     )
                     self.df[f"{tier}_col_idx"] = [
                         [self.columns.index(self.config["columns"][tier])]
@@ -185,193 +173,252 @@
                     ] * len(self.df)
 
     def set_config(self, config: dict, config_path: str = None) -> None:
         """Read in the configuration dictionary."""
         self.config = config
         self.tiers = list(self.config["tier_dirs"].keys())
         self.file_format = self.config["file_format"]
-        self.tier_dirs = self.config["tier_dirs"]
         self.table_format = self.config["table_format"]
+        self.sortby = self.config.get("sortby", "timestamp")
 
-        # Handle environment variables
-        data_dir = os.path.expandvars(self.config["data_dir"])
+        # expand/substitute variables in data_dir and tier_dirs
+        # $_ expands to the location of the config file
+        subst_vars = {}
+        if config_path is not None:
+            subst_vars["_"] = os.path.dirname(str(config_path))
 
-        # Relative paths are interpreted relative to the configuration file
-        if not data_dir.startswith("/"):
-            config_dir = os.path.dirname(config_path)
-            data_dir = os.path.join(config_dir, data_dir)
-            data_dir = os.path.abspath(data_dir)
+        data_dir = lgdo.lgdo_utils.expand_path(
+            self.config["data_dir"], substitute=subst_vars
+        )
         self.data_dir = data_dir
 
-    def scan_files(self) -> None:
-        """Scan the directory containing files from the lower tier and fill the
-        dataframe.
+        tier_dirs = self.config["tier_dirs"]
+        for k, val in tier_dirs.items():
+            tier_dirs[k] = lgdo.lgdo_utils.expand_vars(val, substitute=subst_vars)
+        self.tier_dirs = tier_dirs
+
+    def scan_files(self, dirs: list[str] = None) -> None:
+        """Scan the directory containing files from the lowest tier and fill the dataframe.
+
+        The lowest tier is defined as the first element of the `tiers` array.
+        Only fills columns that can be populated with just these files.
 
-        The lower tier is defined as the first element of the `tiers` array.
-        Only fills columns that can be populated with just the `raw` files.
+        Parameters
+        ----------
+        dirs
+            restrict search to this list of directories. Specified paths can be
+            absolute, relative to `self.data_dir` or relative to the root
+            directory of the lowest-tier files. If ``None``, the whole root
+            lowest-tier directory is scanned. Useful to build a partial
+            database.
         """
         file_keys = []
         n_files = 0
         low_tier = self.tiers[0]
         template = self.file_format[low_tier]
-        scan_dir = self.data_dir + self.tier_dirs[low_tier]
-
-        log.info(f"Scanning {scan_dir} with template {template}")
-
-        for path, _folders, files in os.walk(scan_dir):
-            log.debug(f"Scanning {path}")
-            n_files += len(files)
+        root_scan_dir = os.path.join(
+            self.data_dir, self.tier_dirs[low_tier].lstrip("/")
+        )
 
-            for f in files:
-                # in some cases, we need information from the path name
-                if "/" in template:
-                    f_tmp = path.replace(scan_dir, "") + "/" + f
+        scan_dirs = dirs
+        if dirs is None:
+            scan_dirs = [root_scan_dir]
+        elif not isinstance(dirs, list):
+            scan_dirs = [dirs]
+
+        log.info(f"scanning {scan_dirs} with template {template}")
+
+        for scan_dir in scan_dirs:
+            # some logic to guess where the scan directory is
+            if not os.path.isabs(scan_dir):
+                # first check if it's relative to lowest tier directory
+                if os.path.isdir(os.path.join(root_scan_dir, scan_dir)):
+                    scan_dir = os.path.join(root_scan_dir, scan_dir)
+                # or maybe relative to the data dir?
+                elif os.path.isdir(os.path.join(self.data_dir, scan_dir)):
+                    scan_dir = os.path.join(self.data_dir, scan_dir)
                 else:
-                    f_tmp = f
+                    scan_dir = os.path.join(os.getcwd(), scan_dir)
 
-                finfo = parse(template, f_tmp)
-                if finfo is not None:
-                    finfo = finfo.named
-                    for tier in self.tiers:
-                        finfo[f"{tier}_file"] = self.file_format[tier].format(**finfo)
+            log.debug(f"scanning {scan_dir}")
 
-                    file_keys.append(finfo)
+            for path, _, files in os.walk(scan_dir):
+                log.debug(f"scanning {path}")
+                n_files += len(files)
+
+                for f in files:
+                    # in some cases, we need information from the path name
+                    if "/" in template:
+                        f_tmp = path.replace(root_scan_dir, "") + "/" + f
+                    else:
+                        f_tmp = f
+
+                    finfo = parse(template, f_tmp)
+                    if finfo is not None:
+                        finfo = finfo.named
+                        for tier in self.tiers:
+                            finfo[f"{tier}_file"] = self.file_format[tier].format(
+                                **finfo
+                            )
+
+                        file_keys.append(finfo)
 
         if n_files == 0:
-            raise FileNotFoundError(f"No {low_tier} files found")
+            raise FileNotFoundError(f"no {low_tier} files found")
 
         if len(file_keys) == 0:
-            raise FileNotFoundError(f"No {low_tier} files matched pattern ", template)
+            raise FileNotFoundError(f"no {low_tier} files matched pattern " + template)
 
         temp_df = pd.DataFrame(file_keys)
 
         # fill the main DataFrame
         self.df = pd.concat([self.df, temp_df])
 
         # convert cols to numeric dtypes where possible
         for col in self.df.columns:
             self.df[col] = pd.to_numeric(self.df[col], errors="ignore")
 
         # sort rows according to timestamps
-        log.debug("Sorting database entries according to timestamp")
-        self.df["_datetime"] = self.df["timestamp"].apply(to_datetime)
-        self.df.sort_values("_datetime", ignore_index=True, inplace=True)
-        self.df.drop("_datetime", axis=1, inplace=True)
+        utils.inplace_sort(self.df, self.sortby)
+
+        # set file status and sizes
+        self.set_file_status()
+        self.set_file_sizes()
 
     def set_file_status(self) -> None:
-        """
-        Add a column to the dataframe with a bit corresponding to whether each
-        tier's file exists.
+        """Add a column with a bit corresponding to whether each tier's file exists.
 
         For example, if we have tiers `raw`, `dsp`, and `hit`, but only the
         `raw` file has been produced, ``file_status`` would be 4 (``0b100`` in
         binary representation).
         """
 
         def check_status(row):
             status = 0
             for i, tier in enumerate(self.tiers):
-                path_name = (
-                    self.data_dir + self.tier_dirs[tier] + "/" + row[f"{tier}_file"]
+                path_name = os.path.join(
+                    self.data_dir,
+                    self.tier_dirs[tier].lstrip("/"),
+                    row[f"{tier}_file"].lstrip("/"),
                 )
                 if os.path.exists(path_name):
                     status |= 1 << len(self.tiers) - i - 1
 
             return status
 
         self.df["file_status"] = self.df.apply(check_status, axis=1)
 
     def set_file_sizes(self) -> None:
-        """
-        Add columns (for each tier) to the database containing the
-        corresponding file size in bytes as reported by
-        :func:`os.path.getsize`.
+        """Add columns for each tier containing the corresponding file size in bytes.
+
+        As reported by :func:`os.path.getsize`.
         """
 
         def get_size(row, tier):
             size = 0
-            path_name = self.data_dir + self.tier_dirs[tier] + "/" + row[f"{tier}_file"]
+            path_name = os.path.join(
+                self.data_dir,
+                self.tier_dirs[tier].lstrip("/"),
+                row[f"{tier}_file"].lstrip("/"),
+            )
             if os.path.exists(path_name):
                 size = os.path.getsize(path_name)
             return size
 
         for tier in self.tiers:
             self.df[f"{tier}_size"] = self.df.apply(get_size, axis=1, tier=tier)
 
     def scan_tables_columns(
-        self, to_file: str = None, override: bool = False
+        self,
+        to_file: str = None,
+        override: bool = False,
+        dir_files_conform: bool = False,
     ) -> list[str]:
-        """Open files in the database to read (and store) available tables (and
-        columns therein) names.
+        """Open files to read (and store) available tables (and columns therein) names.
 
         Adds the available table names in each tier as a column in the
         dataframe by searching for group names that match the configured
         ``table_format`` and saving the associated keyword values.
 
         Returns a list with each unique list of columns found in each table
         and adds a column ``{tier}_col_idx`` to the dataframe that maps to the
         column table.
 
         Parameters
         ----------
-        to_file:
+        to_file
             Optionally write the column table to an LH5 file (as a
-            :class:`~.lgdo.vectorofvectors.VectorOfVectors`)
-
-        override:
-            If the FileDB already has a `columns` field, the scan will not run unless
-            this parameter is set to True
+            :class:`~.lgdo.vectorofvectors.VectorOfVectors`).
+        override
+            If the :class:`FileDB` already has a `columns` field, the scan will
+            not run unless this parameter is set to ``True``.
+        dir_files_conform
+            if ``True``, assume that all files in a directory contain tables
+            with the same columns (i.e. all file contents conform to the same
+            format) and scan only the first file. Significantly reduces
+            processing time.
         """
-        log.info("Getting table column names")
+        log.info("getting table column names")
 
         if self.columns is not None:
             if not override:
                 log.warning(
                     "LH5 tables/columns names already set, if you want to perform the scan anyway, set override=True"
                 )
                 return
             else:
-                log.warning("Overwriting existing LH5 tables/columns names")
+                log.warning("overwriting existing LH5 tables/columns names")
 
-        def update_tables_cols(row, tier: str) -> pd.Series:
-            fpath = self.data_dir + self.tier_dirs[tier] + "/" + row[f"{tier}_file"]
+        def update_tables_cols(row, tier: str, utc_cache: dict = None) -> pd.Series:
+            fpath = os.path.join(
+                self.data_dir,
+                self.tier_dirs[tier].lstrip("/"),
+                row[f"{tier}_file"].lstrip("/"),
+            )
+            this_dir = fpath[: fpath.rfind("/")]
+            if utc_cache is not None and this_dir in utc_cache:
+                return utc_cache[this_dir]
 
-            log.debug(f"Reading column names for tier '{tier}' from {fpath}")
+            log.debug(f"reading column names for tier '{tier}' from {fpath}")
 
             if os.path.exists(fpath):
                 f = h5py.File(fpath)
             else:
+                log.debug(f"{fpath} doesn't exist")
                 return pd.Series({f"{tier}_tables": None, f"{tier}_col_idx": None})
 
             # Get tables in each tier
             tier_tables = []
             template = self.table_format[tier]
             if template[-1] == "/":
                 template = template[:-1]
 
             braces = list(re.finditer("{|}", template))
 
             if len(braces) > 2:
-                raise ValueError("Tables can only have one identifier")
+                raise ValueError("tables can only have one identifier")
             if len(braces) % 2 != 0:
-                raise ValueError("Braces mismatch in table format")
+                raise ValueError("braces mismatch in table format")
             if len(braces) == 0:
-                tier_tables.append("")
+                tier_tables.append(0)
             else:
                 wildcard = (
                     template[: braces[0].span()[0]]
                     + "*"
                     + template[braces[1].span()[1] :]
                 )
 
                 # TODO this call here is really expensive!
-                groups = ls(f, wildcard)
-                tier_tables = [
-                    list(parse(template, g).named.values())[0] for g in groups
-                ]
+                groups = lh5.ls(f, wildcard)
+                if len(groups) > 0 and parse(template, groups[0]) is None:
+                    log.warning(f"groups in {fpath} don't match template")
+                else:
+                    tier_tables = [
+                        list(parse(template, g).named.values())[0] for g in groups
+                    ]
 
             # Get columns
             col_idx = []
             template = self.table_format[tier]
             fm = string.Formatter()
 
             for tb in tier_tables:
@@ -380,84 +427,169 @@
                 if len(names) > 0:
                     keyword = names[0]
                     args = {keyword: tb}
                     table_name = template.format(**args)
                 else:
                     table_name = template
 
-                col = ls(f[table_name])
+                try:
+                    col = lh5.ls(f[table_name])
+                except KeyError:
+                    log.warning(f"cannot find '{table_name}' in {fpath}")
+                    continue
                 if col not in columns:
                     columns.append(col)
                     col_idx.append(len(columns) - 1)
                 else:
                     col_idx.append(columns.index(col))
 
-            return pd.Series(
+            series = pd.Series(
                 {f"{tier}_tables": tier_tables, f"{tier}_col_idx": col_idx}
             )
+            if utc_cache is not None:
+                utc_cache[this_dir] = series
+            return series
 
         columns = []
+
+        # set up a cache to provide a fast option if all files in each directory
+        # are expected to all have the same cols
+        utc_cache = None
+        if dir_files_conform:
+            utc_cache = {}
+
         for tier in self.tiers:
             self.df[[f"{tier}_tables", f"{tier}_col_idx"]] = self.df.apply(
-                update_tables_cols, axis=1, tier=tier
+                update_tables_cols, axis=1, tier=tier, utc_cache=utc_cache
             )
 
         self.columns = columns
 
         if to_file is not None:
-            log.debug(f"Writing column names to '{to_file}'")
+            log.debug(f"writing column names to '{to_file}'")
             flattened = []
             length = []
             for i, col in enumerate(columns):
                 if i == 0:
                     length.append(len(col))
                 else:
                     length.append(length[i - 1] + len(col))
                 for c in col:
                     flattened.append(c)
             columns_vov = VectorOfVectors(
                 flattened_data=flattened, cumulative_length=length
             )
-            sto = LH5Store()
+            sto = lh5.LH5Store()
             sto.write_object(columns_vov, "unique_columns", to_file)
 
-        return columns
+        return self.columns
 
-    def from_disk(self, filename: str) -> None:
-        """
-        Fills the dataframe (and configuration dictionary) with the information
-        from a file created by :meth:`to_disk`.
+    def from_disk(self, path: str | list[str]) -> None:
+        """Read FileDBs from disk.
+
+        Overrides the dataframe, configuration dictionary and columns with the
+        information from a file created by :meth:`to_disk`.
+
+        Parameters
+        ----------
+        path
+            file or file pattern (or list of the latter).
         """
-        sto = LH5Store()
-        cfg, _ = sto.read_object("config", filename)
-        self.set_config(json.loads(cfg.value.decode()))
+        log.debug(f"reading FileDB from disk at {path}")
 
-        self.df = pd.read_hdf(filename, key="dataframe")
+        if not isinstance(path, list):
+            path = [path]
 
-        vov, _ = sto.read_object("columns", filename)
-        # Convert back from VoV of UTF-8 bytestrings to a list of lists of strings
-        vov = list(vov)
-        columns = []
-        for ov in vov:
-            columns.append([v.decode("utf-8") for v in ov])
-        self.columns = columns
+        # expand wildcards
+        paths = []
+        for p in path:
+            paths += lgdo.lgdo_utils.expand_path(p, list=True)
+
+        if not paths:
+            raise FileNotFoundError(path)
+
+        sto = lh5.LH5Store()
+        # objects that will be used to configure the FileDB at the end
+        _cfg = None
+        _df = None
+        _columns = None
+
+        for p in paths:
+            cfg, _ = sto.read_object("config", p)
+            cfg = json.loads(cfg.value.decode())
+
+            # make sure configurations are all the same
+            if _cfg is None:
+                _cfg = cfg
+            elif cfg != _cfg:
+                raise RuntimeError(
+                    "cannot merge FileDBs created with different configuration files"
+                )
+
+            # read in unique columns
+            vov, _ = sto.read_object("columns", p)
+            # Convert back from VoV of UTF-8 bytestrings to a list of lists of strings
+            columns = [[v.decode("utf-8") for v in ov] for ov in list(vov)]
+
+            # read in dataframe
+            df = pd.read_hdf(p, key="dataframe")
+
+            # first iteration
+            if _columns is None:
+                _columns = columns
+                _df = df
+                continue
+            elif _columns != columns:
+                log.debug("found inconsistent FileDB, trying to merge")
+                # if columns are not the same, need to merge the two dataframes
+                # in the right way
+                for idx, cols in enumerate(columns):
+                    if cols not in _columns:
+                        # add the new column at the end and save its index
+                        _columns += [cols]
+                        new_idx = len(_columns) - 1
+
+                        def _replace_idx(row, idx, new_idx, tier):
+                            col = row[f"{tier}_col_idx"]
+                            if col is None:
+                                return None
+                            else:
+                                return [new_idx if x == idx else x for x in col]
+
+                        # now go through the new dataframe and update the old index
+                        # everywhere in the {tier}_col_idx columns
+                        for tier in list(_cfg["tier_dirs"].keys()):
+                            df[f"{tier}_col_idx"] = df.apply(
+                                _replace_idx,
+                                args=(idx, new_idx, tier),
+                                axis=1,
+                            )
+
+            # now we can safely concat the dataframes
+            _df = pd.concat([_df, df], ignore_index=True, copy=False)
+
+        self.set_config(_cfg)
+        self.df = _df
+        self.columns = _columns
+
+        utils.inplace_sort(self.df, self.sortby)
 
     def to_disk(self, filename: str, wo_mode="write_safe") -> None:
         """Serializes database to disk.
 
         Parameters
         -----------
         filename
             output LH5 file name.
         wo_mode
             passed to :meth:`~.lgdo.lh5_store.write_object`.
         """
-        log.debug(f"Writing database to {filename}")
+        log.debug(f"writing database to {filename}")
 
-        sto = LH5Store()
+        sto = lh5.LH5Store()
         sto.write_object(
             Scalar(json.dumps(self.config)), "config", filename, wo_mode=wo_mode
         )
 
         if wo_mode in ["write_safe", "w", "overwrite_file", "of"]:
             wo_mode = "a"
 
@@ -493,15 +625,14 @@
         file_keys = []
         n_files = 0
 
         for path, _folders, files in os.walk(daq_dir):
             n_files += len(files)
 
             for f in files:
-
                 # in some cases, we need information from the path name
                 if "/" in daq_template:
                     f_tmp = path.replace(daq_dir, "") + "/" + f
                 else:
                     f_tmp = f
 
                 finfo = parse(daq_template, f_tmp)
@@ -522,14 +653,64 @@
         # fill the main DataFrame
         self.df = pd.concat([self.df, temp_df])
 
         # convert cols to numeric dtypes where possible
         for col in self.df.columns:
             self.df[col] = pd.to_numeric(self.df[col], errors="ignore")
 
+    def get_table_name(self, tier: str, tb: str) -> str:
+        """Get the table name for a tier given its table identifier.
+
+        Parameters
+        ----------
+        tier
+            specify the tier whose table format will be used.
+        tb
+            the table identifier that will be passed to the table format.
+
+        Returns
+        -------
+        table_name
+            the name of the table in `tier` with table identifier `tb`
+        """
+        template = self.table_format[tier]
+        fm = string.Formatter()
+        parse_arr = np.array(list(fm.parse(template)))
+        names = list(parse_arr[:, 1])
+        if len(names) > 0:
+            keyword = names[0]
+            args = {keyword: tb}
+            table_name = template.format(**args)
+        else:
+            table_name = template
+        return table_name
+
+    def get_table_columns(
+        self, table: str | int, tier: str, ifile: int = 0
+    ) -> list[str]:
+        """Return list of columns in table `table`, tier `tier`.
+
+        Assumes that the table contents do not change across data files. If
+        desired, `ifile` (default is 0) can be used to select a different file.
+        """
+        tables = self.df.iloc[ifile][f"{tier}_tables"]
+        if tables is None:
+            return []
+
+        table_idx = tables.index(table)
+        col_idx = self.df.iloc[ifile][f"{tier}_col_idx"][table_idx]
+        return self.columns[col_idx]
+
     def __repr__(self) -> str:
-        string = (
-            "<< Columns >>\n" + self.columns.__repr__() + "\n"
-            "\n"
-            "<< DataFrame >>\n" + self.df.__repr__()
-        )
-        return string
+        string = f"FileDB(data_dir={self.data_dir}, tiers={self.tier_dirs}, "
+
+        if self.df is not None:
+            string += "df=DataFrame(...), "
+        else:
+            string += "df=None, "
+
+        if self.columns is not None:
+            string += "columns=[...]"
+        else:
+            string += "columns=None"
+
+        return string + ")"
```

### Comparing `pygama-1.2.0/src/pygama/hit/build_hit.py` & `pygama-1.3.0/src/pygama/hit/build_hit.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     if lh5_tables_config is not None:
         tbl_cfg = lh5_tables_config
         # sanitize config
         if isinstance(tbl_cfg, str):
             with open(tbl_cfg) as f:
                 tbl_cfg = json.load(f)
 
-        for (k, v) in tbl_cfg.items():
+        for k, v in tbl_cfg.items():
             if isinstance(v, str):
                 with open(v) as f:
                     # order in hit configs is important (dependencies)
                     tbl_cfg[k] = json.load(f, object_pairs_hook=OrderedDict)
         lh5_tables_config = tbl_cfg
 
     else:
@@ -116,15 +116,15 @@
                     lh5_tables_config[f"{el}/dsp"] = hit_config
 
     if outfile is None:
         outfile = os.path.splitext(os.path.basename(infile))[0]
         outfile = outfile.removesuffix("_dsp") + "_hit.lh5"
 
     first_done = False
-    for (tbl, cfg) in lh5_tables_config.items():
+    for tbl, cfg in lh5_tables_config.items():
         lh5_it = LH5Iterator(infile, tbl, buffer_len=buffer_len)
         tot_n_rows = store.read_n_rows(tbl, infile)
         write_offset = 0
 
         log.info(f"Processing table '{tbl}' in file {infile}")
 
         for tbl_obj, start_row, n_rows in lh5_it:
```

### Comparing `pygama-1.2.0/src/pygama/lgdo/__init__.py` & `pygama-1.3.0/src/pygama/lgdo/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,60 +15,74 @@
   :attr:`nda` attribute.
 * :class:`.ArrayOfEqualSizedArrays`: multi-dimensional :class:`numpy.ndarray`.
   Access data via the :attr:`nda` attribute.
 * :class:`.VectorOfVectors`: a variable length array of variable length arrays.
   Implemented as a pair of :class:`.Array`: :attr:`flattened_data` holding the
   raw data, and :attr:`cumulative_length` whose ith element is the sum of the
   lengths of the vectors with ``index <= i``
+* :class:`.VectorOfEncodedVectors`: an array of variable length *encoded*
+  arrays. Implemented as a :class:`.VectorOfVectors` :attr:`encoded_data`
+  holding the encoded vectors and an :class:`.Array` :attr:`decoded_size`
+  specifying the size of each decoded vector. Mainly used to represent a list
+  of compressed waveforms.
+* :class:`.ArrayOfEncodedEqualSizedArrays`: an array of equal sized encoded
+  arrays. Similar to :class:`.VectorOfEncodedVectors` except for
+  :attr:`decoded_size`, which is now a scalar.
 * :class:`.Struct`: a dictionary containing LGDO objects. Derives from
   :class:`dict`
 * :class:`.Table`: a :class:`.Struct` whose elements ("columns") are all array
   types with the same length (number of rows)
 
 Currently the primary on-disk format for LGDO object is LEGEND HDF5 (LH5) files. IO
 is done via the class :class:`.lh5_store.LH5Store`. LH5 files can also be
 browsed easily in python like any `HDF5 <https://www.hdfgroup.org>`_ file using
 `h5py <https://www.h5py.org>`_.
 """
 
-from pygama.lgdo.array import Array
-from pygama.lgdo.arrayofequalsizedarrays import ArrayOfEqualSizedArrays
-from pygama.lgdo.fixedsizearray import FixedSizeArray
-from pygama.lgdo.lgdo import LGDO
-from pygama.lgdo.lh5_store import LH5Iterator, LH5Store, load_dfs, load_nda, ls, show
-from pygama.lgdo.scalar import Scalar
-from pygama.lgdo.struct import Struct
-from pygama.lgdo.table import Table
-from pygama.lgdo.vectorofvectors import (
+from pygama.lgdo.waveform_table import WaveformTable
+
+from .array import Array
+from .arrayofequalsizedarrays import ArrayOfEqualSizedArrays
+from .encoded import ArrayOfEncodedEqualSizedArrays, VectorOfEncodedVectors
+from .fixedsizearray import FixedSizeArray
+from .lgdo import LGDO
+from .lgdo_utils import copy
+from .lh5_store import LH5Iterator, LH5Store, load_dfs, load_nda, ls, show
+from .scalar import Scalar
+from .struct import Struct
+from .table import Table
+from .vectorofvectors import (
     VectorOfVectors,
     build_cl,
     explode,
     explode_arrays,
     explode_cl,
 )
-from pygama.lgdo.waveform_table import WaveformTable
 
 __all__ = [
     "Array",
     "ArrayOfEqualSizedArrays",
+    "ArrayOfEncodedEqualSizedArrays",
     "FixedSizeArray",
     "LGDO",
     "Scalar",
     "Struct",
     "Table",
     "VectorOfVectors",
+    "VectorOfEncodedVectors",
     "WaveformTable",
     "LH5Iterator",
     "LH5Store",
     "load_dfs",
     "load_nda",
     "ls",
     "show",
     "build_cl",
     "explode",
     "explode_arrays",
     "explode_cl",
+    "copy",
 ]
 
 import numpy as np
 
 np.set_printoptions(threshold=10)
```

### Comparing `pygama-1.2.0/src/pygama/lgdo/fixedsizearray.py` & `pygama-1.3.0/src/pygama/lgdo/fixedsizearray.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 from __future__ import annotations
 
 from typing import Any
 
 import numpy
 
-from pygama.lgdo.array import Array
+from .array import Array
 
 
 class FixedSizeArray(Array):
     """An array of fixed-size arrays.
 
     Arrays with guaranteed shape along axes > 0: for example, an array of
     vectors will always length 3 on axis 1, and it will never change from
```

### Comparing `pygama-1.2.0/src/pygama/lgdo/lgdo.py` & `pygama-1.3.0/src/pygama/lgdo/lgdo.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,12 +26,26 @@
         pass
 
     @abstractmethod
     def form_datatype(self) -> str:
         """Return this LGDO's datatype attribute string."""
         pass
 
+    def getattrs(self, datatype: bool = False) -> dict:
+        """Return a copy of the LGDO attributes dictionary.
+
+        Parameters
+        ----------
+        datatype
+            if ``False``, remove ``datatype`` attribute from the output
+            dictionary.
+        """
+        d = dict(self.attrs)
+        if not datatype:
+            d.pop("datatype", None)
+        return d
+
     def __str__(self) -> str:
         return repr(self)
 
     def __repr__(self) -> str:
         return self.__class__.__name__ + f"(attrs={repr(self.attrs)})"
```

### Comparing `pygama-1.2.0/src/pygama/lgdo/lh5_store.py` & `pygama-1.3.0/src/pygama/lgdo/lh5_store.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,37 +5,42 @@
 from __future__ import annotations
 
 import fnmatch
 import glob
 import logging
 import os
 import sys
-from bisect import bisect_left, bisect_right
+from bisect import bisect_left
 from collections import defaultdict
-from typing import Any, Union
+from typing import Any, Iterator, Union
 
 import h5py
 import numba as nb
 import numpy as np
 import pandas as pd
 
-from pygama.lgdo.array import Array
-from pygama.lgdo.arrayofequalsizedarrays import ArrayOfEqualSizedArrays
-from pygama.lgdo.fixedsizearray import FixedSizeArray
-from pygama.lgdo.lgdo_utils import expand_path, parse_datatype
-from pygama.lgdo.scalar import Scalar
-from pygama.lgdo.struct import Struct
-from pygama.lgdo.table import Table
-from pygama.lgdo.vectorofvectors import VectorOfVectors
-from pygama.lgdo.waveform_table import WaveformTable
+from . import compression as compress
+from .array import Array
+from .arrayofequalsizedarrays import ArrayOfEqualSizedArrays
+from .compression import WaveformCodec
+from .encoded import ArrayOfEncodedEqualSizedArrays, VectorOfEncodedVectors
+from .fixedsizearray import FixedSizeArray
+from .lgdo_utils import expand_path, parse_datatype
+from .scalar import Scalar
+from .struct import Struct
+from .table import Table
+from .vectorofvectors import VectorOfVectors
+from .waveform_table import WaveformTable
 
 LGDO = Union[Array, Scalar, Struct, VectorOfVectors]
 
 log = logging.getLogger(__name__)
 
+DEFAULT_HDF5_COMPRESSION = None
+
 
 class LH5Store:
     """
     Class to represent a store of LEGEND HDF5 files. The two main methods
     implemented by the class are :meth:`read_object` and :meth:`write_object`.
 
     Examples
@@ -70,15 +75,15 @@
             LH5 file name.
         mode
             mode in which to open file. See :class:`h5py.File` documentation.
         """
         if isinstance(lh5_file, h5py.File):
             return lh5_file
         if mode == "r":
-            lh5_file = expand_path(lh5_file)
+            lh5_file = expand_path(lh5_file, base_path=self.base_path)
         if lh5_file in self.files.keys():
             return self.files[lh5_file]
         if self.base_path != "":
             full_path = os.path.join(self.base_path, lh5_file)
         else:
             full_path = lh5_file
         if mode != "r":
@@ -93,15 +98,15 @@
         h5f = h5py.File(full_path, mode)
         if self.keep_open:
             self.files[lh5_file] = h5f
         return h5f
 
     def gimme_group(
         self,
-        group: str,
+        group: str | h5py.Group,
         base_group: h5py.Group,
         grp_attrs: dict[str, Any] = None,
         overwrite: bool = False,
     ) -> h5py.Group:
         """
         Returns an existing :class:`h5py` group from a base group or creates a
         new one. Can also set (or replace) group attributes.
@@ -111,15 +116,15 @@
         group
             name of the HDF5 group.
         base_group
             HDF5 group to be used as a base.
         grp_attrs
             HDF5 group attributes.
         overwrite
-            whether overwrite group attributes, ignored is `grp_attrs` is
+            whether overwrite group attributes, ignored if `grp_attrs` is
             ``None``.
         """
         if not isinstance(group, h5py.Group):
             if group in base_group:
                 group = base_group[group]
             else:
                 group = base_group.create_group(group)
@@ -160,14 +165,15 @@
         lh5_file: str | h5py.File | list[str | h5py.File],
         start_row: int = 0,
         n_rows: int = sys.maxsize,
         idx: np.ndarray | list | tuple | list[np.ndarray | list | tuple] = None,
         field_mask: dict[str, bool] | list[str] | tuple[str] = None,
         obj_buf: LGDO = None,
         obj_buf_start: int = 0,
+        decompress: bool = True,
     ) -> tuple[LGDO, int]:
         """Read LH5 object data from a file.
 
         Parameters
         ----------
         name
             Name of the LH5 object to be read (including its group path).
@@ -205,26 +211,30 @@
         obj_buf
             Read directly into memory provided in `obj_buf`. Note: the buffer
             will be expanded to accommodate the data requested. To maintain the
             buffer length, send in ``n_rows = len(obj_buf)``.
         obj_buf_start
             Start location in ``obj_buf`` for read. For concatenating data to
             array-like objects.
+        decompress
+            Decompress data encoded with pygama's compression routines right
+            after reading. The option has no effect on data encoded with HDF5
+            built-in filters, which is always decompressed upstream by HDF5.
 
         Returns
         -------
         (object, n_rows_read)
             `object` is the read-out object `n_rows_read` is the number of rows
             successfully read out. Essential for arrays when the amount of data
             is smaller than the object buffer.  For scalars and structs
             `n_rows_read` will be``1``. For tables it is redundant with
             ``table.loc``.
         """
         # Handle list-of-files recursively
-        if not isinstance(lh5_file, (str, h5py._hl.files.File)):
+        if not isinstance(lh5_file, (str, h5py.File)):
             lh5_file = list(lh5_file)
             n_rows_read = 0
             for i, h5f in enumerate(lh5_file):
                 if isinstance(idx, list) and len(idx) > 0 and not np.isscalar(idx[0]):
                     # a list of lists: must be one per file
                     idx_i = idx[i]
                 elif idx is not None:
@@ -247,32 +257,32 @@
                     lh5_file[i],
                     start_row=start_row,
                     n_rows=n_rows_i,
                     idx=idx_i,
                     field_mask=field_mask,
                     obj_buf=obj_buf,
                     obj_buf_start=obj_buf_start,
+                    decompress=decompress,
                 )
                 n_rows_read += n_rows_read_i
                 if n_rows_read >= n_rows or obj_buf is None:
                     return obj_buf, n_rows_read
                 start_row = 0
                 obj_buf_start += n_rows_read_i
             return obj_buf, n_rows_read
 
-        # start read from single file. fail if the object is not found
-        log.debug(
-            f"reading '{name}' from {lh5_file}"
-            + (f" with field mask {field_mask}" if field_mask else "")
-        )
-
         # get the file from the store
         h5f = self.gimme_file(lh5_file, "r")
         if not h5f or name not in h5f:
-            raise KeyError(f"'{name}' not in {lh5_file}")
+            raise KeyError(f"'{name}' not in {h5f.filename}")
+
+        log.debug(
+            f"reading {h5f.filename}:{name}[{start_row}:{n_rows}], decompress = {decompress}, "
+            + (f" with field mask {field_mask}" if field_mask else "")
+        )
 
         # make idx a proper tuple if it's not one already
         if not (isinstance(idx, tuple) and len(idx) == 1):
             if idx is not None:
                 idx = (idx,)
 
         # get the object's datatype
@@ -314,15 +324,14 @@
                 return obj_buf, 1
             else:
                 return Scalar(value=value, attrs=h5f[name].attrs), 1
 
         # Struct
         # recursively build a struct, return as a dictionary
         if datatype == "struct":
-
             # ignore obj_buf.
             # TODO: could append new fields or overwrite/concat to existing
             # fields. If implemented, get_buffer() above should probably also
             # (optionally?) prep buffers for each field
             if obj_buf is not None:
                 raise NotImplementedError("obj_buf not implemented for LGOD Structs")
 
@@ -332,15 +341,20 @@
                 if not field_mask[field]:
                     continue
                 # TODO: it's strange to pass start_row, n_rows, idx to struct
                 # fields. If they all had shared indexing, they should be in a
                 # table... Maybe should emit a warning? Or allow them to be
                 # dicts keyed by field name?
                 obj_dict[field], _ = self.read_object(
-                    name + "/" + field, h5f, start_row=start_row, n_rows=n_rows, idx=idx
+                    name + "/" + field,
+                    h5f,
+                    start_row=start_row,
+                    n_rows=n_rows,
+                    idx=idx,
+                    decompress=decompress,
                 )
             # modify datatype in attrs if a field_mask was used
             attrs = dict(h5f[name].attrs)
             if field_mask is not None:
                 selected_fields = []
                 for field in elements:
                     if field_mask[field]:
@@ -361,46 +375,51 @@
             col_dict = {}
 
             # read out each of the fields
             rows_read = []
             for field in elements:
                 if not field_mask[field]:
                     continue
+
                 fld_buf = None
                 if obj_buf is not None:
                     if not isinstance(obj_buf, Table) or field not in obj_buf:
                         raise ValueError(
                             f"obj_buf for LGDO Table '{name}' not formatted correctly"
                         )
 
                     else:
                         fld_buf = obj_buf[field]
+
                 col_dict[field], n_rows_read = self.read_object(
                     name + "/" + field,
                     h5f,
                     start_row=start_row,
                     n_rows=n_rows,
                     idx=idx,
                     obj_buf=fld_buf,
                     obj_buf_start=obj_buf_start,
+                    decompress=decompress,
                 )
                 if obj_buf is not None and obj_buf_start + n_rows_read > len(obj_buf):
                     obj_buf.resize(obj_buf_start + n_rows_read)
+
                 rows_read.append(n_rows_read)
+
             # warn if all columns don't read in the same number of rows
             if len(rows_read) > 0:
                 n_rows_read = rows_read[0]
             else:
                 n_rows_read = 0
                 log.warning(f"Table '{name}' has no subgroups accepted by field mask")
 
             for n in rows_read[1:]:
                 if n != n_rows_read:
                     log.warning(
-                        f"Table '{name}' got strange n_rows_read = {n}, {n_rows_read} was expected"
+                        f"Table '{name}' got strange n_rows_read = {n}, {n_rows_read} was expected ({rows_read})"
                     )
 
             # modify datatype in attrs if a field_mask was used
             attrs = dict(h5f[name].attrs)
             if field_mask is not None:
                 selected_fields = []
                 for field in elements:
@@ -419,14 +438,15 @@
                     and "values" in col_dict
                 ):
                     table = WaveformTable(
                         t0=col_dict["t0"], dt=col_dict["dt"], values=col_dict["values"]
                     )
                 else:
                     table = Table(col_dict=col_dict, attrs=attrs)
+
                 # set (write) loc to end of tree
                 table.loc = n_rows_read
                 return table, n_rows_read
             else:
                 # We have read all fields into the object buffer. Run
                 # checks: All columns should be the same size. So update
                 # table's size as necessary, warn if any mismatches are found
@@ -437,14 +457,99 @@
                 if set(obj_buf.attrs.keys()) != set(attrs.keys()):
                     raise RuntimeError(
                         f"attrs mismatch. obj_buf.attrs: "
                         f"{obj_buf.attrs}, h5f[{name}].attrs: {attrs}"
                     )
                 return obj_buf, n_rows_read
 
+        # ArrayOfEncodedEqualSizedArrays and VectorOfEncodedVectors
+        for cond, enc_lgdo in [
+            (
+                datatype == "array_of_encoded_equalsized_arrays",
+                ArrayOfEncodedEqualSizedArrays,
+            ),
+            (elements.startswith("encoded_array"), VectorOfEncodedVectors),
+        ]:
+            if cond:
+                if (
+                    not decompress
+                    and obj_buf is not None
+                    and not isinstance(obj_buf, enc_lgdo)
+                ):
+                    raise ValueError(f"obj_buf for '{name}' not a {enc_lgdo}")
+
+                # read out decoded_size, either a Scalar or an Array
+                decoded_size_buf = encoded_data_buf = None
+                if obj_buf is not None and not decompress:
+                    decoded_size_buf = obj_buf.decoded_size
+                    encoded_data_buf = obj_buf.encoded_data
+
+                decoded_size, _ = self.read_object(
+                    f"{name}/decoded_size",
+                    h5f,
+                    start_row=start_row,
+                    n_rows=n_rows,
+                    idx=idx,
+                    obj_buf=None if decompress else decoded_size_buf,
+                    obj_buf_start=0 if decompress else obj_buf_start,
+                )
+
+                # read out encoded_data, a VectorOfVectors
+                encoded_data, n_rows_read = self.read_object(
+                    f"{name}/encoded_data",
+                    h5f,
+                    start_row=start_row,
+                    n_rows=n_rows,
+                    idx=idx,
+                    obj_buf=None if decompress else encoded_data_buf,
+                    obj_buf_start=0 if decompress else obj_buf_start,
+                )
+
+                # return the still encoded data in the buffer object, if there
+                if obj_buf is not None and not decompress:
+                    return obj_buf, n_rows_read
+
+                # otherwise re-create the encoded LGDO
+                rawdata = enc_lgdo(
+                    encoded_data=encoded_data,
+                    decoded_size=decoded_size,
+                    attrs=h5f[name].attrs,
+                )
+
+                # already return if no decompression is requested
+                if not decompress:
+                    return rawdata, n_rows_read
+
+                # if no buffer, decode and return
+                elif obj_buf is None and decompress:
+                    return compress.decode(rawdata), n_rows_read
+
+                # use the (decoded object type) buffer otherwise
+                if enc_lgdo == VectorOfEncodedVectors and not isinstance(
+                    obj_buf, VectorOfVectors
+                ):
+                    raise ValueError(
+                        f"obj_buf for decoded '{name}' not a VectorOfVectors"
+                    )
+                elif enc_lgdo == ArrayOfEncodedEqualSizedArrays and not isinstance(
+                    obj_buf, ArrayOfEqualSizedArrays
+                ):
+                    raise ValueError(
+                        f"obj_buf for decoded '{name}' not an ArrayOfEqualSizedArrays"
+                    )
+
+                # FIXME: not a good idea. an in place decoding version
+                # of decode would be needed to avoid extra memory
+                # allocations
+                # FIXME: obj_buf_start??? Write a unit test
+                for i, wf in enumerate(compress.decode(rawdata)):
+                    obj_buf[i] = wf
+
+                return obj_buf, n_rows_read
+
         # VectorOfVectors
         # read out vector of vectors of different size
         if elements.startswith("array"):
             if obj_buf is not None and not isinstance(obj_buf, VectorOfVectors):
                 raise ValueError(f"obj_buf for '{name}' not a LGDO VectorOfVectors")
 
             # read out cumulative_length
@@ -612,17 +717,14 @@
 
             # Now read the array
             if obj_buf is not None and n_rows_to_read > 0:
                 buf_size = obj_buf_start + n_rows_to_read
                 if len(obj_buf) < buf_size:
                     obj_buf.resize(buf_size)
                 dest_sel = np.s_[obj_buf_start:buf_size]
-                # NOTE: if your script fails on this line, it may be because you
-                # have to apply this patch to h5py (or update h5py, if it's
-                # fixed): https://github.com/h5py/h5py/issues/1792
                 h5f[name].read_direct(obj_buf.nda, source_sel, dest_sel)
                 nda = obj_buf.nda
             else:
                 if n_rows == 0:
                     tmp_shape = (0,) + h5f[name].shape[1:]
                     nda = np.empty(tmp_shape, h5f[name].dtype)
                 else:
@@ -662,17 +764,44 @@
         name: str,
         lh5_file: str | h5py.File,
         group: str | h5py.Group = "/",
         start_row: int = 0,
         n_rows: int = None,
         wo_mode: str = "append",
         write_start: int = 0,
+        hdf5_compression: str | h5py.filters.FilterRefBase = DEFAULT_HDF5_COMPRESSION,
     ) -> None:
         """Write an LGDO into an LH5 file.
 
+        If the `obj` :class:`.LGDO` has a `compression` attribute, its value is
+        interpreted as the algorithm to be used to compress `obj` before
+        writing to disk. The type of `compression` can be:
+
+        string, kwargs dictionary, hdf5plugin filter
+          interpreted as the name of a built-in or custom `HDF5 compression
+          filter <https://docs.h5py.org/en/stable/high/dataset.html#filter-pipeline>`_
+          (``"gzip"``, ``"lzf"``, :mod:`hdf5plugin` filter object etc.) and
+          passed directly to :meth:`h5py.Group.create_dataset`.
+
+        :class:`.WaveformCodec` object
+          If `obj` is a :class:`.WaveformTable`, compress its `values` using
+          this algorithm. More documentation about the supported waveform
+          compression algorithms at :mod:`.lgdo.compression`.
+
+        Note
+        ----
+        The `compression` attribute takes precedence over the
+        `hdf5_compression` argument and is not written to disk.
+
+        Note
+        ----
+        HDF5 compression is skipped for the `encoded_data` dataset of
+        :class:`.VectorOfEncodedVectors` and
+        :class`.ArrayOfEncodedEqualSizedArrays`.
+
         Parameters
         ----------
         obj
             LH5 object. if object is array-like, writes `n_rows` starting from
             `start_row` in `obj`.
         name
             name of the object in the output HDF5 file.
@@ -692,55 +821,128 @@
               of array-like objects and array-like subfields of structs.
               :class:`~.lgdo.scalar.Scalar` objects get overwritten.
             - ``overwrite`` or ``o``: replace data in the file if present,
               starting from `write_start`. Note: overwriting with `write_start` =
               end of array is the same as ``append``.
             - ``overwrite_file`` or ``of``: delete file if present prior to
               writing to it. `write_start` should be 0 (its ignored).
+            - ``append_column`` or ``ac``: append columns from an :class:`~.lgdo.table.Table`
+              `obj` only if there is an existing :class:`~.lgdo.table.Table` in the `lh5_file` with
+              the same `name` and :class:`~.lgdo.table.Table.size`. If the sizes don't match,
+              or if there are matching fields, it errors out.
         write_start
             row in the output file (if already existing) to start overwriting
             from.
+        hdf5_compression
+            HDF5 compression filter to be applied before writing non-scalar
+            datasets. **Ignored if compression is specified as an `obj`
+            attribute.**
         """
+        log.debug(
+            f"writing {repr(obj)}[{start_row}:{n_rows}] as "
+            f"{lh5_file}:{group}/{name}[{write_start}:], "
+            f"mode = {wo_mode}, hdf5_compression = {hdf5_compression}"
+        )
+
         if wo_mode == "write_safe":
             wo_mode = "w"
         if wo_mode == "append":
             wo_mode = "a"
         if wo_mode == "overwrite":
             wo_mode = "o"
         if wo_mode == "overwrite_file":
             wo_mode = "of"
             write_start = 0
-        if wo_mode != "w" and wo_mode != "a" and wo_mode != "o" and wo_mode != "of":
+        if wo_mode == "append_column":
+            wo_mode = "ac"
+        if wo_mode not in ["w", "a", "o", "of", "ac"]:
             raise ValueError(f"unknown wo_mode '{wo_mode}'")
 
         # "mode" is for the h5df.File and wo_mode is for this function
         # In hdf5, 'a' is really "modify" -- in addition to appending, you can
         # change any object in the file. So we use file:append for
         # write_object:overwrite.
         mode = "w" if wo_mode == "of" else "a"
         lh5_file = self.gimme_file(lh5_file, mode=mode)
         group = self.gimme_group(group, lh5_file)
         if wo_mode == "w" and name in group:
             raise RuntimeError(f"can't overwrite '{name}' in wo_mode 'write_safe'")
 
         # struct or table or waveform table
         if isinstance(obj, Struct):
+            # In order to append a column, we need to update the `table{old_fields}` value in `group.attrs['datatype"]` to include the new fields.
+            # One way to do this is to override `obj.attrs["datatype"]` to include old and new fields. Then we can write the fields to the table as normal.
+            if wo_mode == "ac":
+                old_group = self.gimme_group(name, group)
+                datatype, shape, fields = parse_datatype(old_group.attrs["datatype"])
+                if datatype not in ["table", "struct"]:
+                    raise RuntimeError(
+                        f"Trying to append columns to an object of type {datatype}"
+                    )
+
+                # If the mode is `append_column`, make sure we aren't appending a table that has a column of the same name as in the existing table
+                # Also make sure that the field we are adding has the same size
+                if len(list(set(fields).intersection(set(obj.keys())))) != 0:
+                    raise ValueError(
+                        f"Can't append {list(set(fields).intersection(set(obj.keys())))} column(s) to a table with the same field(s)"
+                    )
+                # It doesn't matter what key we access, as all fields in the old table have the same size
+                if old_group[list(old_group.keys())[0]].size != obj.size:
+                    raise ValueError(
+                        f"Table sizes don't match. Trying to append column of size {obj.size} to a table of size {old_group[list(old_group.keys())[0]].size}."
+                    )
+
+                # Now we can append the obj.keys() to the old fields, and then update obj.attrs.
+                fields.extend(list(obj.keys()))
+                obj.attrs.pop("datatype")
+                obj.attrs["datatype"] = "table" + "{" + ",".join(fields) + "}"
+
             group = self.gimme_group(
-                name, group, grp_attrs=obj.attrs, overwrite=(wo_mode == "o")
+                name,
+                group,
+                grp_attrs=obj.attrs,
+                overwrite=(wo_mode in ["o", "ac"]),
             )
+            # If the mode is overwrite, then we need to peek into the file's table's existing fields
+            # If we are writing a new table to the group that does not contain an old field, we should delete that old field from the file
+            if wo_mode == "o":
+                # Find the old keys in the group that are not present in the new table's keys, then delete them
+                for key in list(set(group.keys()) - set(obj.keys())):
+                    log.debug(f"{key} is not present in new table, deleting field")
+                    del group[key]
+
             for field in obj.keys():
+                # eventually compress waveform table values with pygama's
+                # custom codecs before writing
+                # if waveformtable.values.attrs["compression"] is a string,
+                # interpret it as an HDF5 built-in filter
+                obj_fld = None
+                if (
+                    isinstance(obj, WaveformTable)
+                    and field == "values"
+                    and not isinstance(obj.values, VectorOfEncodedVectors)
+                    and not isinstance(obj.values, ArrayOfEncodedEqualSizedArrays)
+                    and "compression" in obj.values.attrs
+                    and isinstance(obj.values.attrs["compression"], WaveformCodec)
+                ):
+                    codec = obj.values.attrs["compression"]
+                    obj_fld = compress.encode(obj.values, codec=codec)
+                else:
+                    obj_fld = obj[field]
+
                 self.write_object(
-                    obj[field],
+                    obj_fld,
                     field,
                     lh5_file,
                     group=group,
                     start_row=start_row,
                     n_rows=n_rows,
                     wo_mode=wo_mode,
                     write_start=write_start,
+                    hdf5_compression=hdf5_compression,
                 )
             return
 
         # scalars
         elif isinstance(obj, Scalar):
             if name in group:
                 if wo_mode in ["o", "a"]:
@@ -750,14 +952,44 @@
                     raise RuntimeError(
                         f"tried to overwrite {name} in {group} for wo_mode {wo_mode}"
                     )
             ds = group.create_dataset(name, shape=(), data=obj.value)
             ds.attrs.update(obj.attrs)
             return
 
+        # vector of encoded vectors
+        elif isinstance(obj, (VectorOfEncodedVectors, ArrayOfEncodedEqualSizedArrays)):
+            group = self.gimme_group(
+                name, group, grp_attrs=obj.attrs, overwrite=(wo_mode == "o")
+            )
+
+            self.write_object(
+                obj.encoded_data,
+                "encoded_data",
+                lh5_file,
+                group=group,
+                start_row=start_row,
+                n_rows=n_rows,
+                wo_mode=wo_mode,
+                write_start=write_start,
+                hdf5_compression=None,  # data is already compressed!
+            )
+
+            self.write_object(
+                obj.decoded_size,
+                "decoded_size",
+                lh5_file,
+                group=group,
+                start_row=start_row,
+                n_rows=n_rows,
+                wo_mode=wo_mode,
+                write_start=write_start,
+                hdf5_compression=hdf5_compression,
+            )
+
         # vector of vectors
         elif isinstance(obj, VectorOfVectors):
             group = self.gimme_group(
                 name, group, grp_attrs=obj.attrs, overwrite=(wo_mode == "o")
             )
             if (
                 n_rows is None
@@ -783,61 +1015,91 @@
                 "flattened_data",
                 lh5_file,
                 group=group,
                 start_row=fd_start,
                 n_rows=fd_n_rows,
                 wo_mode=wo_mode,
                 write_start=offset,
+                hdf5_compression=hdf5_compression,
             )
 
             # now offset is used to give appropriate in-file values for
             # cumulative_length. Need to adjust it for start_row
             if start_row > 0:
                 offset -= obj.cumulative_length.nda[start_row - 1]
 
             # Add offset to obj.cumulative_length itself to avoid memory allocation.
             # Then subtract it off after writing! (otherwise it will be changed
             # upon return)
-            obj.cumulative_length.nda += offset
+            cl_dtype = obj.cumulative_length.nda.dtype.type
+            obj.cumulative_length.nda += cl_dtype(offset)
 
             self.write_object(
                 obj.cumulative_length,
                 "cumulative_length",
                 lh5_file,
                 group=group,
                 start_row=start_row,
                 n_rows=n_rows,
                 wo_mode=wo_mode,
                 write_start=write_start,
+                hdf5_compression=hdf5_compression,
             )
-            obj.cumulative_length.nda -= offset
+            obj.cumulative_length.nda -= cl_dtype(offset)
 
             return
 
         # if we get this far, must be one of the Array types
         elif isinstance(obj, Array):
             if n_rows is None or n_rows > obj.nda.shape[0] - start_row:
                 n_rows = obj.nda.shape[0] - start_row
+
             nda = obj.nda[start_row : start_row + n_rows]
+
             # hack to store bools as uint8 for c / Julia compliance
             if nda.dtype.name == "bool":
                 nda = nda.astype(np.uint8)
+
             # need to create dataset from ndarray the first time for speed
             # creating an empty dataset and appending to that is super slow!
             if (wo_mode != "a" and write_start == 0) or name not in group:
                 maxshape = (None,) + nda.shape[1:]
                 if wo_mode == "o" and name in group:
                     log.debug(f"overwriting {name} in {group}")
                     del group[name]
-                ds = group.create_dataset(name, data=nda, maxshape=maxshape)
-                ds.attrs.update(obj.attrs)
+
+                # create HDF5 dataset
+                # - compress using the 'compression' LGDO attribute, if
+                #   available
+                # - otherwise use "hdf5_compression"
+                # - attach HDF5 dataset attributes, but not "compression"!
+                comp_algo = obj.attrs.get("compression", hdf5_compression)
+                comp_kwargs = {}
+                if isinstance(comp_algo, str):
+                    comp_kwargs = {"compression": comp_algo}
+                elif comp_algo is not None:
+                    comp_kwargs = comp_algo
+
+                ds = group.create_dataset(
+                    name, data=nda, maxshape=maxshape, **comp_kwargs
+                )
+
+                _attrs = obj.getattrs(datatype=True)
+                _attrs.pop("compression", None)
+                ds.attrs.update(_attrs)
                 return
 
             # Now append or overwrite
             ds = group[name]
+            if not isinstance(ds, h5py.Dataset):
+                raise RuntimeError(
+                    f"existing HDF5 object '{name}' in group '{group}'"
+                    " is not a dataset! Cannot overwrite or append"
+                )
+
             old_len = ds.shape[0]
             if wo_mode == "a":
                 write_start = old_len
             add_len = write_start + nda.shape[0] - old_len
             ds.resize(old_len + add_len, axis=0)
             ds[write_start:] = nda
             return
@@ -880,23 +1142,30 @@
             rows_read = None
             for field in elements:
                 n_rows_read = self.read_n_rows(name + "/" + field, h5f)
                 if not rows_read:
                     rows_read = n_rows_read
                 elif rows_read != n_rows_read:
                     log.warning(
-                        f"table '{name}' got strange n_rows_read = {rows_read}, "
+                        f"'{field}' field in table '{name}' has {rows_read} rows, "
                         f"{n_rows_read} was expected"
                     )
             return rows_read
 
         # length of vector of vectors is the length of its cumulative_length
         if elements.startswith("array"):
             return self.read_n_rows(f"{name}/cumulative_length", h5f)
 
+        # length of vector of encoded vectors is the length of its decoded_size
+        if (
+            elements.startswith("encoded_array")
+            or datatype == "array_of_encoded_equalsized_arrays"
+        ):
+            return self.read_n_rows(f"{name}/encoded_data", h5f)
+
         # return array length (without reading the array!)
         if "array" in datatype:
             # compute the number of rows to read
             return h5f[name].shape[0]
 
         raise RuntimeError(f"don't know how to read datatype '{datatype}'")
 
@@ -941,25 +1210,28 @@
             ret.extend([f"{key}/{path}" for path in ls(lh5_file[key], splitpath[1])])
         return ret
 
 
 def show(
     lh5_file: str | h5py.Group,
     lh5_group: str = "/",
+    attrs: bool = False,
     indent: str = "",
     header: bool = True,
 ) -> None:
     """Print a tree of LH5 file contents with LGDO datatype.
 
     Parameters
     ----------
     lh5_file
         the LH5 file.
     lh5_group
         print only contents of this HDF5 group.
+    attrs
+        print the HDF5 attributes too.
     indent
         indent the diagram with this string.
     header
         print `lh5_group` at the top of the diagram.
 
     Examples
     --------
@@ -997,29 +1269,33 @@
         print(f"{indent}└──  empty")  # noqa: T201
         return
 
     # loop over keys
     while True:
         val = lh5_file[key]
         # we want to print the LGDO datatype
-        attr = val.attrs.get("datatype", default="no datatype")
-        if attr == "no datatype" and isinstance(val, h5py.Group):
-            attr = "HDF5 group"
+        dtype = val.attrs.get("datatype", default="no datatype")
+        if dtype == "no datatype" and isinstance(val, h5py.Group):
+            dtype = "HDF5 group"
+
+        attrs_d = dict(val.attrs)
+        attrs_d.pop("datatype", "")
+        attrs = "── " + str(attrs_d) if attrs_d else ""
 
         # is this the last key?
         killme = False
         try:
             k_new = next(it)  # get next key
         except StopIteration:
             char = "└──"
             killme = True  # we'll have to kill this loop later
         else:
             char = "├──"
 
-        print(f"{indent}{char} \033[1m{key}\033[0m · {attr}")  # noqa: T201
+        print(f"{indent}{char} \033[1m{key}\033[0m · {dtype} {attrs}")  # noqa: T201
 
         # if it's a group, call this function recursively
         if isinstance(val, h5py.Group):
             show(val, indent=indent + ("    " if killme else "│   "), header=False)
 
         # break or move to next key
         if killme:
@@ -1113,15 +1389,15 @@
         `f_list`.
     """
     return pd.DataFrame(
         load_nda(f_list, par_list, lh5_group=lh5_group, idx_list=idx_list)
     )
 
 
-class LH5Iterator:
+class LH5Iterator(Iterator):
     """
     A class for iterating through one or more LH5 files, one block of entries
     at a time. This also accepts an entry list/mask to enable event selection,
     and a field mask.
 
     This class can be used either for random access:
 
@@ -1142,165 +1418,276 @@
     reallocation of memory; this means that if you want to hold on to data
     between reads, you will have to copy it somewhere!
     """
 
     def __init__(
         self,
         lh5_files: str | list[str],
-        group: str,
+        groups: str | list[str],
         base_path: str = "",
         entry_list: list[int] | list[list[int]] = None,
         entry_mask: list[bool] | list[list[bool]] = None,
         field_mask: dict[str, bool] | list[str] | tuple[str] = None,
         buffer_len: int = 3200,
+        friend: LH5Iterator = None,
     ) -> None:
         """
         Parameters
         ----------
         lh5_files
             file or files to read from. May include wildcards and environment
             variables.
-        group
-            HDF5 group to read.
-        base_path
-            HDF5 path to prepend.
+        groups
+            HDF5 group(s) to read. If a list is provided for both lh5_files
+            and group, they must be the same size. If a file is wild-carded,
+            the same group will be assigned to each file found
         entry_list
             list of entry numbers to read. If a nested list is provided,
             expect one top-level list for each file, containing a list of
             local entries. If a list of ints is provided, use global entries.
         entry_mask
             mask of entries to read. If a list of arrays is provided, expect
             one for each file. Ignore if a selection list is provided.
         field_mask
             mask of which fields to read. See :meth:`LH5Store.read_object` for
             more details.
         buffer_len
             number of entries to read at a time while iterating through files.
+        friend
+            a ''friend'' LH5Iterator that will be read in parallel with this.
+            The friend should have the same length and entry list. A single
+            LH5 table containing columns from both iterators will be returned.
         """
         self.lh5_st = LH5Store(base_path=base_path, keep_open=True)
 
         # List of files, with wildcards and env vars expanded
         if isinstance(lh5_files, str):
-            lh5_files = expand_path(lh5_files, True)
+            lh5_files = [lh5_files]
+            if isinstance(groups, list):
+                lh5_files *= len(groups)
         elif not isinstance(lh5_files, list):
             raise ValueError("lh5_files must be a string or list of strings")
 
+        if isinstance(groups, str):
+            groups = [groups] * len(lh5_files)
+        elif not isinstance(groups, list):
+            raise ValueError("group must be a string or list of strings")
+
+        if not len(groups) == len(lh5_files):
+            raise ValueError("lh5_files and groups must have same length")
+
+        self.lh5_files = []
+        self.groups = []
+        for f, g in zip(lh5_files, groups):
+            f_exp = expand_path(f, list=True, base_path=base_path)
+            self.lh5_files += f_exp
+            self.groups += [g] * len(f_exp)
+
         if entry_list is not None and entry_mask is not None:
             raise ValueError(
                 "entry_list and entry_mask arguments are mutually exclusive"
             )
 
-        self.lh5_files = [f for f_wc in lh5_files for f in expand_path(f_wc, True)]
-
         # Map to last row in each file
-        self.file_map = np.array(
-            [self.lh5_st.read_n_rows(group, f) for f in self.lh5_files], "int64"
-        ).cumsum()
-        self.group = group
+        self.file_map = np.full(len(self.lh5_files), np.iinfo("i").max, "i")
+        # Map to last iterator entry for each file
+        self.entry_map = np.full(len(self.lh5_files), np.iinfo("i").max, "i")
         self.buffer_len = buffer_len
 
         if len(self.lh5_files) > 0:
+            f = self.lh5_files[0]
+            g = self.groups[0]
             self.lh5_buffer = self.lh5_st.get_buffer(
-                self.group,
-                self.lh5_files[0],
+                g,
+                f,
                 size=self.buffer_len,
                 field_mask=field_mask,
             )
+            self.file_map[0] = self.lh5_st.read_n_rows(g, f)
         else:
             raise RuntimeError(f"can't open any files from {lh5_files}")
 
         self.n_rows = 0
         self.current_entry = 0
+        self.next_entry = 0
 
         self.field_mask = field_mask
 
         # List of entry indices from each file
-        self.entry_list = None
+        self.local_entry_list = None
+        self.global_entry_list = None
         if entry_list is not None:
             entry_list = list(entry_list)
             if isinstance(entry_list[0], int):
-                entry_list.sort()
-                i_start = 0
-                self.entry_list = []
-                for f_end in self.file_map:
-                    i_stop = bisect_right(entry_list, f_end, lo=i_start)
-                    self.entry_list.append(entry_list[i_start:i_stop])
-                    i_start = i_stop
+                self.local_entry_list = [None] * len(self.file_map)
+                self.global_entry_list = np.array(entry_list, "i")
+                self.global_entry_list.sort()
 
             else:
-                self.entry_list = [[]] * len(self.file_map)
+                self.local_entry_list = [[]] * len(self.file_map)
                 for i_file, local_list in enumerate(entry_list):
-                    self.entry_list[i_file] = list(local_list)
+                    self.local_entry_list[i_file] = np.array(local_list, "i")
+                    self.local_entry_list[i_file].sort()
 
         elif entry_mask is not None:
             # Convert entry mask into an entry list
             if isinstance(entry_mask, pd.Series):
                 entry_mask = entry_mask.values
             if isinstance(entry_mask, np.ndarray):
-                self.entry_list = []
-                f_start = 0
-                for f_end in self.file_map:
-                    self.entry_list.append(
-                        list(np.nonzero(entry_mask[f_start:f_end])[0])
-                    )
-                    f_start = f_end
+                self.local_entry_list = [None] * len(self.file_map)
+                self.global_entry_list = np.nonzero(entry_mask)[0]
             else:
-                self.entry_list = [[]] * len(self.file_map)
+                self.local_entry_list = [[]] * len(self.file_map)
                 for i_file, local_mask in enumerate(entry_mask):
-                    self.entry_list[i_file] = list(np.nonzero(local_mask)[0])
+                    self.local_entry_list[i_file] = np.nonzero(local_mask)[0]
 
-        # Map to last entry of each file
-        self.entry_map = (
-            self.file_map
-            if self.entry_list is None
-            else np.array([len(elist) for elist in self.entry_list]).cumsum()
-        )
+        # Attach the friend
+        if friend is not None:
+            if not isinstance(friend, LH5Iterator):
+                raise ValueError("Friend must be an LH5Iterator")
+            self.lh5_buffer.join(friend.lh5_buffer)
+        self.friend = friend
+
+    def _get_file_cumlen(self, i_file: int) -> int:
+        """Helper to get cumulative file length of file"""
+        if i_file < 0:
+            return 0
+        fcl = self.file_map[i_file]
+        if fcl == np.iinfo("i").max:
+            fcl = self._get_file_cumlen(i_file - 1) + self.lh5_st.read_n_rows(
+                self.groups[i_file], self.lh5_files[i_file]
+            )
+            self.file_map[i_file] = fcl
+        return fcl
+
+    def _get_file_cumentries(self, i_file: int) -> int:
+        """Helper to get cumulative iterator entries in file"""
+        if i_file < 0:
+            return 0
+        n = self.entry_map[i_file]
+        if n == np.iinfo("i").max:
+            elist = self.get_file_entrylist(i_file)
+            fcl = self._get_file_cumlen(i_file)
+            if elist is None:
+                # no entry list provided
+                n = fcl
+            else:
+                file_entries = self.get_file_entrylist(i_file)
+                # check that file entries fall inside of file
+                if file_entries[-1] >= fcl:
+                    logging.warning(f"Found entries out of range for file {i_file}")
+                    n = np.searchsorted(file_entries, fcl, "right")
+                else:
+                    n = len(file_entries)
+                n += self._get_file_cumentries(i_file - 1)
+            self.entry_map[i_file] = n
+        return n
+
+    def get_file_entrylist(self, i_file: int) -> np.ndarray:
+        """Helper to get entry list for file"""
+        # If no entry list is provided
+        if self.local_entry_list is None:
+            return None
+
+        elist = self.local_entry_list[i_file]
+        if elist is None:
+            # Get local entrylist for this file from global entry list
+            f_start = self._get_file_cumlen(i_file - 1)
+            f_end = self._get_file_cumlen(i_file)
+            i_start = self._get_file_cumentries(i_file - 1)
+            i_stop = np.searchsorted(self.global_entry_list, f_end, "right")
+            elist = np.array(self.global_entry_list[i_start:i_stop], "i") - f_start
+            self.local_entry_list[i_file] = elist
+        return elist
+
+    def get_global_entrylist(self) -> np.ndarray:
+        """Get global entry list, constructing it if needed"""
+        if self.global_entry_list is None and self.local_entry_list is not None:
+            self.global_entry_list = np.zeros(len(self), "i")
+            for i_file in range(len(self.lh5_files)):
+                i_start = self.get_file_cumentries(i_file - 1)
+                i_stop = self.get_file_cumentries(i_file)
+                f_start = self.get_file_cumlen(i_file - 1)
+                self.global_entry_list[i_start:i_stop] = (
+                    self.get_file_entrylist(i_file) + f_start
+                )
+        return self.global_entry_list
 
     def read(self, entry: int) -> tuple[LGDO, int]:
-        """Read the next chunk of events, starting at entry. Return the
+        """Read the nextlocal chunk of events, starting at entry. Return the
         LH5 buffer and number of rows read."""
-        i_file = np.searchsorted(self.entry_map, entry, "right")
-        local_entry = entry
-        if i_file > 0:
-            local_entry -= self.entry_map[i_file - 1]
         self.n_rows = 0
+        i_file = np.searchsorted(self.entry_map, entry, "right")
+
+        # if file hasn't been opened yet, search through files
+        # sequentially until we find the right one
+        if i_file < len(self.lh5_files) and self.entry_map[i_file] == np.iinfo("i").max:
+            while i_file < len(self.lh5_files) and entry >= self._get_file_cumentries(
+                i_file
+            ):
+                i_file += 1
+
+        if i_file == len(self.lh5_files):
+            return (self.lh5_buffer, self.n_rows)
+        local_entry = entry - self._get_file_cumentries(i_file - 1)
 
         while self.n_rows < self.buffer_len and i_file < len(self.file_map):
             # Loop through files
-            local_idx = self.entry_list[i_file] if self.entry_list is not None else None
+            local_idx = self.get_file_entrylist(i_file)
             i_local = local_idx[local_entry] if local_idx is not None else local_entry
             self.lh5_buffer, n_rows = self.lh5_st.read_object(
-                self.group,
+                self.groups[i_file],
                 self.lh5_files[i_file],
                 start_row=i_local,
                 n_rows=self.buffer_len - self.n_rows,
                 idx=local_idx,
                 field_mask=self.field_mask,
                 obj_buf=self.lh5_buffer,
                 obj_buf_start=self.n_rows,
             )
 
             self.n_rows += n_rows
             i_file += 1
             local_entry = 0
 
         self.current_entry = entry
+
+        if self.friend is not None:
+            self.friend.read(entry)
+
         return (self.lh5_buffer, self.n_rows)
 
+    def reset_field_mask(self, mask):
+        """Replaces the field mask of this iterator and any friends with mask"""
+        self.field_mask = mask
+        if self.friend is not None:
+            self.friend.reset_field_mask(mask)
+
     def __len__(self) -> int:
         """Return the total number of entries."""
-        return self.entry_map[-1] if len(self.entry_map) > 0 else 0
+        return (
+            self._get_file_cumentries(len(self.lh5_files) - 1)
+            if len(self.entry_map) > 0
+            else 0
+        )
 
-    def __iter__(self) -> tuple[LGDO, int, int]:
+    def __iter__(self) -> Iterator:
         """Loop through entries in blocks of size buffer_len."""
-        entry = 0
-        while entry < len(self):
-            buf, n_rows = self.read(entry)
-            yield (buf, entry, n_rows)
-            entry += n_rows
+        self.current_entry = 0
+        self.next_entry = 0
+        return self
+
+    def __next__(self) -> tuple[LGDO, int, int]:
+        """Read next buffer_len entries and return lh5_table, iterator entry
+        and n_rows read."""
+        buf, n_rows = self.read(self.next_entry)
+        self.next_entry = self.current_entry + n_rows
+        if n_rows == 0:
+            raise StopIteration
+        return (buf, self.current_entry, n_rows)
 
 
 @nb.njit(parallel=False, fastmath=True)
 def _make_fd_idx(starts, stops, idx):
     k = 0
     if len(starts) < len(stops):
         for i in range(stops[0]):
```

### Comparing `pygama-1.2.0/src/pygama/lgdo/scalar.py` & `pygama-1.3.0/src/pygama/lgdo/scalar.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from __future__ import annotations
 
 import logging
 from typing import Any
 
 import numpy as np
 
-from pygama.lgdo import LGDO
-from pygama.lgdo.lgdo_utils import get_element_type
+from .lgdo import LGDO
+from .lgdo_utils import get_element_type
 
 log = logging.getLogger(__name__)
 
 
 class Scalar(LGDO):
     """Holds just a scalar value and some attributes (datatype, units, ...)."""
 
@@ -38,17 +38,22 @@
             return self.value.datatype_name
         else:
             return get_element_type(self.value)
 
     def form_datatype(self) -> str:
         return self.datatype_name()
 
+    def __eq__(self, other: Scalar) -> bool:
+        if isinstance(other, Scalar):
+            return self.value == other.value and self.attrs == self.attrs
+        else:
+            return False
+
     def __str__(self) -> str:
-        tmp_attrs = self.attrs.copy()
-        tmp_attrs.pop("datatype")
-        return f"{str(self.value)} with attrs={repr(tmp_attrs)}"
+        attrs = self.getattrs()
+        return f"{str(self.value)} with attrs={repr(attrs)}"
 
     def __repr__(self) -> str:
         return (
             self.__class__.__name__
             + f"(value={repr(self.value)}, attrs={repr(self.attrs)})"
         )
```

### Comparing `pygama-1.2.0/src/pygama/lgdo/struct.py` & `pygama-1.3.0/src/pygama/lgdo/struct.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 import logging
 from typing import Any
 
 import numpy as np
 
-from pygama.lgdo import LGDO
+from .lgdo import LGDO
 
 log = logging.getLogger(__name__)
 
 
 class Struct(LGDO, dict):
     """A dictionary of LGDO's with an optional set of attributes.
 
@@ -81,18 +81,17 @@
             if "\n" in str(v):
                 rv = str(v).replace("\n", "\n    ")
                 string += f" '{k}':\n    {rv},\n"
             else:
                 string += f" '{k}': {v},\n"
         string += "}"
 
-        tmp_attrs = self.attrs.copy()
-        tmp_attrs.pop("datatype")
-        if tmp_attrs:
-            string += f" with attrs={tmp_attrs}"
+        attrs = self.getattrs()
+        if attrs:
+            string += f" with attrs={attrs}"
 
         np.set_printoptions(threshold=thr_orig)
 
         return string
 
     def __repr__(self) -> str:
         npopt = np.get_printoptions()
```

### Comparing `pygama-1.2.0/src/pygama/lgdo/table.py` & `pygama-1.3.0/src/pygama/lgdo/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 from typing import Any
 
 import numexpr as ne
 import numpy as np
 import pandas as pd
 from pandas.io.formats import format as fmt
 
-from pygama.lgdo.array import Array
-from pygama.lgdo.arrayofequalsizedarrays import ArrayOfEqualSizedArrays
-from pygama.lgdo.lgdo import LGDO
-from pygama.lgdo.struct import Struct
-from pygama.lgdo.vectorofvectors import VectorOfVectors
+from .array import Array
+from .arrayofequalsizedarrays import ArrayOfEqualSizedArrays
+from .lgdo import LGDO
+from .struct import Struct
+from .vectorofvectors import VectorOfVectors
 
 log = logging.getLogger(__name__)
 
 
 class Table(Struct):
     """A special struct of arrays or subtable columns of equal length.
 
@@ -181,43 +181,55 @@
         if other_table.loc != self.loc and do_warn:
             log.warning(f"other_table.loc ({other_table.loc}) != self.loc({self.loc})")
         if cols is None:
             cols = other_table.keys()
         for name in cols:
             self.add_column(name, other_table[name], do_warn=do_warn)
 
-    def get_dataframe(self, cols: list[str] = None, copy: bool = False) -> pd.DataFrame:
+    def get_dataframe(
+        self, cols: list[str] = None, copy: bool = False, prefix: str = ""
+    ) -> pd.DataFrame:
         """Get a :class:`pandas.DataFrame` from the data in the table.
 
         Notes
         -----
         The requested data must be array-like, with the ``nda`` attribute.
 
         Parameters
         ----------
         cols
             a list of column names specifying the subset of the table's columns
             to be added to the dataframe.
         copy
             When ``True``, the dataframe allocates new memory and copies data
             into it. Otherwise, the raw ``nda``'s from the table are used directly.
+        prefix
+            The prefix to be added to the column names. Used when recursively getting the
+            dataframe of a Table inside this Table
         """
         df = pd.DataFrame(copy=copy)
         if cols is None:
             cols = self.keys()
         for col in cols:
-            if isinstance(self[col], VectorOfVectors):
-                column = self[col].to_aoesa()
+            if isinstance(self[col], Table):
+                sub_df = self[col].get_dataframe(prefix=f"{prefix}{col}_")
+                if df.empty:
+                    df = sub_df
+                else:
+                    df = df.join(sub_df)
             else:
-                column = self[col]
+                if isinstance(self[col], VectorOfVectors):
+                    column = self[col].to_aoesa()
+                else:
+                    column = self[col]
 
-            if not hasattr(column, "nda"):
-                raise ValueError(f"column {col} does not have an nda")
-            else:
-                df[col] = column.nda.tolist()
+                if not hasattr(column, "nda"):
+                    raise ValueError(f"column {col} does not have an nda")
+                else:
+                    df[prefix + col] = column.nda.tolist()
 
         return df
 
     def eval(self, expr_config: dict) -> Table:
         """Apply column operations to the table and return a new table holding
         the resulting columns.
 
@@ -321,18 +333,16 @@
         try:
             string = self.get_dataframe().to_string(**opts)
         except ValueError:
             string = "Cannot print Table with VectorOfVectors yet!"
 
         string += "\n"
         for k, v in self.items():
-            tmp_attrs = v.attrs.copy()
-            tmp_attrs.pop("datatype")
-            if tmp_attrs:
-                string += f"\nwith attrs['{k}']={tmp_attrs}"
-
-        tmp_attrs = self.attrs.copy()
-        tmp_attrs.pop("datatype")
-        if tmp_attrs:
-            string += f"\nwith attrs={tmp_attrs}"
+            attrs = v.getattrs()
+            if attrs:
+                string += f"\nwith attrs['{k}']={attrs}"
+
+        attrs = self.getattrs()
+        if attrs:
+            string += f"\nwith attrs={attrs}"
 
         return string
```

### Comparing `pygama-1.2.0/src/pygama/lgdo/vectorofvectors.py` & `pygama-1.3.0/src/pygama/lgdo/vectorofvectors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,169 +1,367 @@
 """
 Implements a LEGEND Data Object representing a variable-length array of
 variable-length arrays and corresponding utilities.
 """
 from __future__ import annotations
 
+import itertools
 import logging
+from collections.abc import Iterator
 from typing import Any
 
+import numba
 import numpy as np
-from numba import njit
+from numpy.typing import DTypeLike, NDArray
 
-from pygama.lgdo.array import Array
-from pygama.lgdo.arrayofequalsizedarrays import ArrayOfEqualSizedArrays
-from pygama.lgdo.lgdo import LGDO
-from pygama.lgdo.lgdo_utils import get_element_type
+from . import arrayofequalsizedarrays as aoesa
+from . import lgdo_utils as utils
+from .array import Array
+from .lgdo import LGDO
 
 log = logging.getLogger(__name__)
 
 
 class VectorOfVectors(LGDO):
     """A variable-length array of variable-length arrays.
 
     For now only a 1D vector of 1D vectors is supported. Internal representation
     is as two NumPy arrays, one to store the flattened data contiguosly and one
     to store the cumulative sum of lengths of each vector.
     """
 
     def __init__(
         self,
-        flattened_data: Array = None,
-        cumulative_length: Array = None,
+        listoflists: list[list[int | float]] = None,
+        flattened_data: Array | NDArray = None,
+        cumulative_length: Array | NDArray = None,
         shape_guess: tuple[int, int] = None,
-        dtype: np.dtype = None,
+        dtype: DTypeLike = None,
+        fill_val: int | float = None,
         attrs: dict[str, Any] = None,
     ) -> None:
         """
         Parameters
         ----------
+        listoflists
+            create a VectorOfVectors out of a Python list of lists. Takes
+            priority over `flattened_data` and `cumulative_length`.
         flattened_data
-            If not ``None``, used as the internal memory array for
-            `flattened_data`.  Otherwise, an internal `flattened_data` is
-            allocated based on `shape_guess` and `dtype`.
+            if not ``None``, used as the internal array for
+            `self.flattened_data`.  Otherwise, an internal `flattened_data` is
+            allocated based on `cumulative_length` (or `shape_guess`) and `dtype`.
         cumulative_length
-            If not ``None``, used as the internal memory array for
-            `cumulative_length`. Should be `dtype` :any:`numpy.uint32`. If
+            if not ``None``, used as the internal array for
+            `self.cumulative_length`. Should be `dtype` :any:`numpy.uint32`. If
             `cumulative_length` is ``None``, an internal `cumulative_length` is
             allocated based on the first element of `shape_guess`.
         shape_guess
-            A NumPy-format shape specification, required if either of
+            a NumPy-format shape specification, required if either of
             `flattened_data` or `cumulative_length` are not supplied.  The
             first element should not be a guess and sets the number of vectors
             to be stored. The second element is a guess or approximation of the
             typical length of a stored vector, used to set the initial length
             of `flattened_data` if it was not supplied.
         dtype
-            Sets the type of data stored in `flattened_data`. Required if
-            `flattened_data` is ``None``.
+            sets the type of data stored in `flattened_data`. Required if
+            `flattened_data` and `listoflists` are ``None``.
+        fill_val
+            fill all of `self.flattened_data` with this value.
         attrs
-            A set of user attributes to be carried along with this LGDO.
+            a set of user attributes to be carried along with this LGDO.
         """
-        if cumulative_length is None:
-            self.cumulative_length = Array(
-                shape=(shape_guess[0],), dtype="uint32", fill_val=0
+        if listoflists is not None:
+            cl_nda = np.cumsum([len(ll) for ll in listoflists])
+            if dtype is None:
+                if len(cl_nda) == 0 or cl_nda[-1] == 0:
+                    raise ValueError("listoflists can't be empty with dtype=None!")
+                else:
+                    # Set dtype from the first element in the list
+                    # Find it efficiently, allowing for zero-length lists as some of the entries
+                    first_element = next(itertools.chain.from_iterable(listoflists))
+                    dtype = type(first_element)
+
+            self.dtype = np.dtype(dtype)
+            self.cumulative_length = Array(cl_nda)
+            self.flattened_data = Array(
+                np.fromiter(
+                    itertools.chain.from_iterable(listoflists), dtype=self.dtype
+                )
             )
+
         else:
-            if isinstance(cumulative_length, Array):
-                self.cumulative_length = cumulative_length
+            if cumulative_length is None:
+                if shape_guess is None:
+                    # just make an empty vector
+                    self.cumulative_length = Array(np.empty((0,), dtype="uint32"))
+                else:
+                    # initialize based on shape_guess
+                    if shape_guess[1] <= 0:
+                        self.cumulative_length = Array(
+                            shape=(shape_guess[0],), dtype="uint32", fill_val=0
+                        )
+                    else:
+                        self.cumulative_length = Array(
+                            np.arange(
+                                shape_guess[1],
+                                np.prod(shape_guess) + 1,
+                                shape_guess[1],
+                                dtype="uint32",
+                            )
+                        )
             else:
                 self.cumulative_length = Array(cumulative_length)
-        if flattened_data is None:
-            length = np.prod(shape_guess)
-            if dtype is None:
-                raise ValueError("flattened_data and dtype cannot both be None!")
-            else:
-                self.flattened_data = Array(shape=(length,), dtype=dtype)
-                self.dtype = np.dtype(dtype)
-        else:
-            if isinstance(flattened_data, Array):
-                self.flattened_data = flattened_data
+
+            if flattened_data is None:
+                if dtype is None:
+                    raise ValueError("flattened_data and dtype cannot both be None!")
+
+                length = 0
+                if cumulative_length is None:
+                    if shape_guess is None:
+                        # just make an empty vector
+                        length = 0
+                    else:
+                        # use shape_guess
+                        length = np.prod(shape_guess)
+                else:
+                    # use cumulative_length
+                    length = cumulative_length[-1]
+
+                self.flattened_data = Array(
+                    shape=(length,), dtype=dtype, fill_val=fill_val
+                )
             else:
                 self.flattened_data = Array(flattened_data)
-            if dtype is None:
-                self.dtype = self.flattened_data.dtype
-            else:
-                self.dtype = np.dtype(dtype)
 
-        self.attrs = {} if attrs is None else dict(attrs)
+            # finally set dtype
+            self.dtype = self.flattened_data.dtype
 
-        super().__init__()
+        super().__init__(attrs)
 
     def datatype_name(self) -> str:
         return "array"
 
     def form_datatype(self) -> str:
-        et = get_element_type(self)
+        et = utils.get_element_type(self)
         return "array<1>{array<1>{" + et + "}}"
 
     def __len__(self) -> int:
-        """Provides ``__len__`` for this array-like class."""
+        """Return the number of stored vectors."""
         return len(self.cumulative_length)
 
+    def __eq__(self, other: VectorOfVectors) -> bool:
+        if isinstance(other, VectorOfVectors):
+            return (
+                self.flattened_data == other.flattened_data
+                and self.cumulative_length == other.cumulative_length
+                and self.dtype == other.dtype
+                and self.attrs == other.attrs
+            )
+
+        else:
+            return False
+
+    def __getitem__(self, i: int) -> list:
+        """Return vector at index `i`."""
+        stop = self.cumulative_length[i]
+        if i == 0 or i == -len(self):
+            return self.flattened_data[0:stop]
+        else:
+            return self.flattened_data[self.cumulative_length[i - 1] : stop]
+
+    def __setitem__(self, i: int, new: NDArray) -> None:
+        self.__getitem__(i)[:] = new
+
     def resize(self, new_size: int) -> None:
-        self.cumulative_length.resize(new_size)
+        """Resize vector along the first axis.
+
+        `self.flattened_data` is resized only if `new_size` is smaller than the
+        current vector length.
+
+        If `new_size` is larger than the current vector length,
+        `self.cumulative_length` is padded with its last element.  This
+        corresponds to appending empty vectors.
+
+        Examples
+        --------
+        >>> vov = VectorOfVectors([[1, 2, 3], [4, 5]])
+        >>> vov.resize(3)
+        >>> print(vov)
+        [[1 2 3],
+         [4 5],
+         [],
+        ]
+
+        >>> vov = VectorOfVectors([[1, 2], [3], [4, 5]])
+        >>> vov.resize(2)
+        >>> print(vov)
+        [[1 2],
+         [3],
+        ]
+        """
+
+        vidx = self.cumulative_length
+        old_s = len(self)
+        dlen = new_size - old_s
+        csum = vidx[-1] if len(self) > 0 else 0
 
-    def set_vector(self, i_vec: int, nda: np.ndarray) -> None:
-        """Insert vector `nda` at location `i_vec`.
+        # first resize the cumulative length
+        self.cumulative_length.resize(new_size)
 
-        Notes
-        -----
-        `flattened_data` is doubled in length until `nda` can be appended to
-        it.
+        # if new_size > size, new elements are filled with zeros, let's fix
+        # that
+        if dlen > 0:
+            self.cumulative_length[old_s:] = csum
+
+        # then resize the data array
+        # if dlen > 0 this has no effect
+        if len(self.cumulative_length) > 0:
+            self.flattened_data.resize(self.cumulative_length[-1])
+
+    def append(self, new: NDArray) -> None:
+        """Append a 1D vector `new` at the end.
+
+        Examples
+        --------
+        >>> vov = VectorOfVectors([[1, 2, 3], [4, 5]])
+        >>> vov.append([8, 9])
+        >>> print(vov)
+        [[1 2 3],
+         [4 5],
+         [8 9],
+        ]
         """
-        if i_vec < 0 or i_vec > len(self.cumulative_length.nda) - 1:
-            raise ValueError("bad i_vec", i_vec)
+        # first extend cumulative_length by +1
+        self.cumulative_length.resize(len(self) + 1)
+        # set it at the right value
+        newlen = self.cumulative_length[-2] + len(new) if len(self) > 1 else len(new)
+        self.cumulative_length[-1] = newlen
+        # then resize flattened_data to accommodate the new vector
+        self.flattened_data.resize(len(self.flattened_data) + len(new))
+        # finally set it
+        self[-1] = new
+
+    def insert(self, i: int, new: NDArray) -> None:
+        """Insert a vector at index `i`.
+
+        `self.flattened_data` (and therefore `self.cumulative_length`) is
+        resized in order to accommodate the new element.
+
+        Examples
+        --------
+        >>> vov = VectorOfVectors([[1, 2, 3], [4, 5]])
+        >>> vov.insert(1, [8, 9])
+        >>> print(vov)
+        [[1 2 3],
+         [8 9],
+         [4 5],
+        ]
+
+        Warning
+        -------
+        This method involves a significant amount of memory re-allocation and
+        is expected to perform poorly on large vectors.
+        """
+        if i >= len(self):
+            raise IndexError(
+                f"index {i} is out of bounds for vector owith size {len(self)}"
+            )
+
+        self.flattened_data = Array(
+            np.insert(self.flattened_data, self.cumulative_length[i - 1], new)
+        )
+        self.cumulative_length = Array(
+            np.insert(self.cumulative_length, i, self.cumulative_length[i - 1])
+        )
+        self.cumulative_length[i:] += np.uint32(len(new))
 
-        if len(nda.shape) != 1:
-            raise ValueError("nda had bad shape", nda.shape)
+    def replace(self, i: int, new: NDArray) -> None:
+        """Replace the vector at index `i` with `new`.
 
-        start = 0 if i_vec == 0 else self.cumulative_length.nda[i_vec - 1]
-        end = start + len(nda)
-        while end >= len(self.flattened_data.nda):
-            self.flattened_data.nda.resize(
-                2 * len(self.flattened_data.nda), refcheck=True
+        `self.flattened_data` (and therefore `self.cumulative_length`) is
+        resized, if the length of `new` is different from the vector currently
+        at index `i`.
+
+        Examples
+        --------
+        >>> vov = VectorOfVectors([[1, 2, 3], [4, 5]])
+        >>> vov.replace(0, [8, 9])
+        >>> print(vov)
+        [[8 9],
+         [4 5],
+        ]
+
+        Warning
+        -------
+        This method involves a significant amount of memory re-allocation and
+        is expected to perform poorly on large vectors.
+        """
+        if i >= len(self):
+            raise IndexError(
+                f"index {i} is out of bounds for vector with size {len(self)}"
             )
-        self.flattened_data.nda[start:end] = nda
-        self.cumulative_length.nda[i_vec] = end
 
-    def get_vector(self, i_vec: int) -> np.ndarray:
-        """Get vector at index `i_vec`."""
-        if i_vec >= len(self.cumulative_length) or i_vec < 0:
-            raise IndexError
-
-        if i_vec == 0:
-            start = 0
-            end = self.cumulative_length.nda[0]
+        vidx = self.cumulative_length
+        dlen = len(new) - len(self[i])
+
+        if dlen == 0:
+            # don't waste resources
+            self[i] = new
+        elif dlen < 0:
+            start = vidx[i - 1]
+            stop = start + len(new)
+            # set the already allocated indices
+            self.flattened_data[start:stop] = new
+            # then delete the extra indices
+            self.flattened_data = Array(
+                np.delete(self.flattened_data, np.s_[stop : vidx[i]])
+            )
         else:
-            start = self.cumulative_length.nda[i_vec - 1]
-            end = self.cumulative_length.nda[i_vec]
+            # set the already allocated indices
+            self.flattened_data[vidx[i - 1] : vidx[i]] = new[: len(self[i])]
+            # then insert the remaining
+            self.flattened_data = Array(
+                np.insert(self.flattened_data, vidx[i], new[len(self[i]) :])
+            )
 
-        return self.flattened_data.nda[start:end]
+        vidx[i:] = vidx[i:] + dlen
 
-    def __iter__(self) -> VectorOfVectors:
-        self.index = 0
-        return self
-
-    def __next__(self) -> np.ndarray:
-        try:
-            if self.index == 0:
-                start = 0
-                end = self.cumulative_length.nda[0]
-            else:
-                start = self.cumulative_length.nda[self.index - 1]
-                end = self.cumulative_length.nda[self.index]
-            result = self.flattened_data.nda[start:end]
-        except IndexError:
-            raise StopIteration
-        self.index += 1
-        return result
+    def _set_vector_unsafe(self, i: int, vec: NDArray) -> None:
+        r"""Insert vector `vec` at position `i`.
 
-    def __getitem__(self, index: int) -> list:
-        return list(self)[index]
+        Assumes that ``j = self.cumulative_length[i-1]`` is the index (in
+        `self.flattened_data`) of the end of the `(i-1)`\ th vector and copies
+        `vec` in ``self.flattened_data[j:len(vec)]``. Finally updates
+        ``self.cumulative_length[i]`` with the new flattened data array length.
+
+        Vectors stored after index `i` can be overridden, producing unintended
+        behavior. This method is typically used for fast sequential fill of a
+        pre-allocated vector of vectors.
+
+        Danger
+        ------
+        This method can lead to undefined behavior or vector invalidation if
+        used improperly. Use it only if you know what you are doing.
+
+        See Also
+        --------
+        append, replace, insert
+        """
+        start = 0 if i == 0 else self.cumulative_length[i - 1]
+        end = start + len(vec)
+        self.flattened_data[start:end] = vec
+        self.cumulative_length[i] = end
+
+    def __iter__(self) -> Iterator[NDArray]:
+        for j, stop in enumerate(self.cumulative_length):
+            if j == 0:
+                yield self.flattened_data[0:stop]
+            else:
+                yield self.flattened_data[self.cumulative_length[j - 1] : stop]
 
     def __str__(self) -> str:
         string = ""
         pos = 0
         for vec in self:
             if pos != 0:
                 string += " "
@@ -195,72 +393,85 @@
             + ", attrs="
             + repr(self.attrs)
             + ")"
         )
         np.set_printoptions(**npopt)
         return out
 
-    def to_aoesa(self) -> ArrayOfEqualSizedArrays:
-        """Convert to ArrayOfEqualSizedArrays, padding with NaNs"""
+    def to_aoesa(self, preserve_dtype: bool = False) -> aoesa.ArrayOfEqualSizedArrays:
+        """Convert to :class:`ArrayOfEqualSizedArrays`.
+
+        If `preserve_dtype` is False, the output array will have dtype
+        :class:`numpy.float64` and is padded with :class:`numpy.nan`.
+        Otherwise, the dtype of the original :class:`VectorOfVectors` is
+        preserved.
+        """
         ind_lengths = np.diff(self.cumulative_length.nda, prepend=0)
         arr_len = np.max(ind_lengths)
-        nda = np.empty((len(self.cumulative_length), arr_len))
-        nda.fill(np.nan)
+
+        if not preserve_dtype:
+            nda = np.empty((len(self.cumulative_length), arr_len))
+            nda.fill(np.nan)
+        else:
+            nda = np.empty((len(self.cumulative_length), arr_len), dtype=self.dtype)
+
         for i in range(len(self.cumulative_length)):
             nda[i, : ind_lengths[i]] = self[i]
-        return ArrayOfEqualSizedArrays(nda=nda)
+
+        return aoesa.ArrayOfEqualSizedArrays(nda=nda, attrs=self.getattrs())
 
 
 def build_cl(
-    sorted_array_in: Array, cumulative_length_out: np.ndarray = None
-) -> np.ndarray:
-    """build a cumulative_length array from an array of sorted data
-
-    So for example if sorted_array_in contains [ 3, 3, 3, 4 ], would return
-    [ 2, 3 ]
-
-    For a sorted_array_in of indices, this is the inverse of explode_cl() below,
-    in the sense that doing build_cl(explode_cl(cumulative_length)) would
-    recover the original cumulative_length.
+    sorted_array_in: NDArray, cumulative_length_out: NDArray = None
+) -> NDArray:
+    """Build a cumulative length array from an array of sorted data.
+
+    Examples
+    --------
+    >>> build_cl(np.array([3, 3, 3, 4])
+    array([3., 4.])
+
+    For a `sorted_array_in` of indices, this is the inverse of
+    :func:`.explode_cl`, in the sense that doing
+    ``build_cl(explode_cl(cumulative_length))`` would recover the original
+    `cumulative_length`.
 
     Parameters
     ----------
     sorted_array_in
-        Array of data already sorted; each N matching contiguous entries will be
-        converted into a new row of cumulative_length_out
+        array of data already sorted; each N matching contiguous entries will
+        be converted into a new row of `cumulative_length_out`.
     cumulative_length_out
-        This is an optional pre-allocated array for the output
-        cumulative_length. It will always have length <= sorted_array_in, so
-        giving them the same length is safe if there is not a better guess.
+        a pre-allocated array for the output `cumulative_length`. It will
+        always have length <= `sorted_array_in`, so giving them the same length
+        is safe if there is not a better guess.
 
     Returns
     -------
     cumulative_length_out
-        The output cumulative_length. If the user provides a
-        cumulative_length_out that is too long, this return value is sliced to
-        contain only the used portion of the allocated memory
+        the output cumulative length array. If the user provides a
+        `cumulative_length_out` that is too long, this return value is sliced
+        to contain only the used portion of the allocated memory.
     """
     if len(sorted_array_in) == 0:
         return None
     sorted_array_in = np.asarray(sorted_array_in)
     if cumulative_length_out is None:
         cumulative_length_out = np.zeros(len(sorted_array_in), dtype=np.uint64)
     else:
         cumulative_length_out.fill(0)
     if len(cumulative_length_out) == 0 and len(sorted_array_in) > 0:
         raise ValueError(
             "cumulative_length_out too short ({len(cumulative_length_out)})"
         )
-    return nb_build_cl(sorted_array_in, cumulative_length_out)
+    return _nb_build_cl(sorted_array_in, cumulative_length_out)
 
 
-@njit
-def nb_build_cl(
-    sorted_array_in: np.ndarray, cumulative_length_out: np.ndarray
-) -> np.ndarray:
+@numba.njit
+def _nb_build_cl(sorted_array_in: NDArray, cumulative_length_out: NDArray) -> NDArray:
     """numbified inner loop for build_cl"""
     ii = 0
     last_val = sorted_array_in[0]
     for val in sorted_array_in:
         if val != last_val:
             ii += 1
             cumulative_length_out[ii] = cumulative_length_out[ii - 1]
@@ -268,131 +479,149 @@
                 raise RuntimeError("cumulative_length_out too short")
             last_val = val
         cumulative_length_out[ii] += 1
     ii += 1
     return cumulative_length_out[:ii]
 
 
-def explode_cl(cumulative_length: Array, array_out: np.ndarray = None) -> np.ndarray:
-    """explode a cumulative_length array
+def explode_cl(cumulative_length: NDArray, array_out: NDArray = None) -> NDArray:
+    """Explode a `cumulative_length` array.
 
-    So for example if cumulative_length is [ 2, 3 ], would return [ 0, 0, 0, 1]
-
-    This is the inverse of build_cl() above, in the sense that doing
-    build_cl(explode_cl(cumulative_length)) would recover the original
-    cumulative_length.
+    Examples
+    --------
+    >>> explode_cl(np.array([2, 3]))
+    array([0., 0., 1.])
+
+    This is the inverse of :func:`.build_cl`, in the sense that doing
+    ``build_cl(explode_cl(cumulative_length))`` would recover the original
+    `cumulative_length`.
 
     Parameters
     ----------
     cumulative_length
-        the cumulative_length array to be exploded
+        the cumulative length array to be exploded.
     array_out
-        an optional pre-allocated array to hold the exploded cumulative_length.
-        The length should be equal to cumulative_length[-1]
+        a pre-allocated array to hold the exploded cumulative length array.
+        The length should be equal to ``cumulative_length[-1]``.
 
     Returns
     -------
     array_out
-        the exploded cumulative_length array
+        the exploded cumulative length array.
     """
     cumulative_length = np.asarray(cumulative_length)
     out_len = cumulative_length[-1] if len(cumulative_length) > 0 else 0
     if array_out is None:
         array_out = np.empty(int(out_len), dtype=np.uint64)
     if len(array_out) != out_len:
         raise ValueError(
             f"bad lengths: cl[-1] ({cumulative_length[-1]}) != out ({len(array_out)})"
         )
-    return nb_explode_cl(cumulative_length, array_out)
+    return _nb_explode_cl(cumulative_length, array_out)
 
 
-@njit
-def nb_explode_cl(cumulative_length: np.ndarray, array_out: np.ndarray) -> np.ndarray:
+@numba.njit
+def _nb_explode_cl(cumulative_length: NDArray, array_out: NDArray) -> NDArray:
     """numbified inner loop for explode_cl"""
     out_len = cumulative_length[-1] if len(cumulative_length) > 0 else 0
     if len(array_out) != out_len:
         raise ValueError("bad lengths")
     start = 0
     for ii in range(len(cumulative_length)):
         nn = int(cumulative_length[ii] - start)
         for jj in range(nn):
             array_out[int(start + jj)] = ii
         start = cumulative_length[ii]
     return array_out
 
 
 def explode(
-    cumulative_length: Array, array_in: Array, array_out: np.ndarray = None
-) -> np.ndarray:
-    """explode a data array using a cumulative_length array
-
-    This is identical to allocated_explode_cl, except array_in gets exploded
-    instead of cumulative_length. So for example, if array_in = [ 3, 4 ] and
-    cumulative_length = [ 2, 3 ], array_out would be [ 3, 3, 3, 4 ]
+    cumulative_length: NDArray, array_in: NDArray, array_out: NDArray = None
+) -> NDArray:
+    """Explode a data array using a `cumulative_length` array.
+
+    This is identical to :func:`.explode_cl`, except `array_in` gets exploded
+    instead of `cumulative_length`.
+
+    Examples
+    --------
+    >>> explode(np.array([2, 3]), np.array([3, 4]))
+    array([3., 3., 4.])
 
     Parameters
     ----------
     cumulative_length
-        the cumulative_length array to use for exploding
+        the cumulative length array to use for exploding.
     array_in
-        the data to be exploded. Must have same length as cumulative_length
+        the data to be exploded. Must have same length as `cumulative_length`.
     array_out
         a pre-allocated array to hold the exploded data. The length should be
-        equal to cumulative_length[-1]
+        equal to ``cumulative_length[-1]``.
+
+    Returns
+    -------
+    array_out
+        the exploded cumulative length array.
     """
     cumulative_length = np.asarray(cumulative_length)
     array_in = np.asarray(array_in)
     out_len = cumulative_length[-1] if len(cumulative_length) > 0 else 0
     if array_out is None:
         array_out = np.empty(out_len, dtype=array_in.dtype)
     if len(cumulative_length) != len(array_in) or len(array_out) != out_len:
         raise ValueError(
-            f"bad lengths: cl ({len(cumulative_length)}) != in ({len(array_in)}) and cl[-1] ({cumulative_length[-1]}) != out ({len(array_out)})"
+            f"bad lengths: cl ({len(cumulative_length)}) != in ({len(array_in)}) "
+            f"and cl[-1] ({cumulative_length[-1]}) != out ({len(array_out)})"
         )
     return nb_explode(cumulative_length, array_in, array_out)
 
 
-@njit
+@numba.njit
 def nb_explode(
-    cumulative_length: np.ndarray, array_in: np.ndarray, array_out: np.ndarray
-) -> np.ndarray:
-    """numbified inner loop for explode"""
+    cumulative_length: NDArray, array_in: NDArray, array_out: NDArray
+) -> NDArray:
+    """Numbified inner loop for :func:`.explode`."""
     out_len = cumulative_length[-1] if len(cumulative_length) > 0 else 0
     if len(cumulative_length) != len(array_in) or len(array_out) != out_len:
         raise ValueError("bad lengths")
     ii = 0
     for jj in range(len(array_out)):
         while ii < len(cumulative_length) and jj >= cumulative_length[ii]:
             ii += 1
         array_out[jj] = array_in[ii]
     return array_out
 
 
 def explode_arrays(
-    cumulative_length: Array, arrays: list, out_arrays: list = None
+    cumulative_length: Array, arrays: list[NDArray], arrays_out: list[NDArray] = None
 ) -> list:
-    """explode a set of arrays using a cumulative_length array
+    """Explode a set of arrays using a `cumulative_length` array.
 
     Parameters
     ----------
     cumulative_length
-        the cumulative_length array to use for exploding
+        the cumulative length array to use for exploding.
     arrays
         the data arrays to be exploded. Each array must have same length as
-        cumulative_length
-    out_arrays
-        an optional list of pre-allocated arrays to hold the exploded data. The
-        length of the list should be equal to the number of "arrays", and each
-        entry in array_out should have length cumulative_length[-1]. If not
+        `cumulative_length`.
+    arrays_out
+        a list of pre-allocated arrays to hold the exploded data. The length of
+        the list should be equal to the length of `arrays`, and each entry in
+        arrays_out should have length ``cumulative_length[-1]``. If not
         provided, output arrays are allocated for the user.
+
+    Returns
+    -------
+    arrays_out
+        the list of exploded cumulative length arrays.
     """
     cumulative_length = np.asarray(cumulative_length)
     for ii in range(len(arrays)):
         arrays[ii] = np.asarray(arrays[ii])
     out_len = cumulative_length[-1] if len(cumulative_length) > 0 else 0
-    if out_arrays is None:
-        out_arrays = []
+    if arrays_out is None:
+        arrays_out = []
         for array in arrays:
-            out_arrays.append(np.empty(out_len, dtype=array.dtype))
+            arrays_out.append(np.empty(out_len, dtype=array.dtype))
     for ii in range(len(arrays)):
-        explode(cumulative_length, arrays[ii], out_arrays[ii])
-    return out_arrays
+        explode(cumulative_length, arrays[ii], arrays_out[ii])
+    return arrays_out
```

### Comparing `pygama-1.2.0/src/pygama/lgdo/waveform_table.py` & `pygama-1.3.0/src/pygama/lgdo/waveform_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 from __future__ import annotations
 
 import logging
 from typing import Any
 
 import numpy as np
 
-from pygama.lgdo.array import Array
-from pygama.lgdo.arrayofequalsizedarrays import ArrayOfEqualSizedArrays
-from pygama.lgdo.table import Table
-from pygama.lgdo.vectorofvectors import VectorOfVectors
+from .array import Array
+from .arrayofequalsizedarrays import ArrayOfEqualSizedArrays
+from .encoded import ArrayOfEncodedEqualSizedArrays, VectorOfEncodedVectors
+from .table import Table
+from .vectorofvectors import VectorOfVectors
 
 log = logging.getLogger(__name__)
 
 
 class WaveformTable(Table):
     r"""An LGDO for storing blocks of (1D) time-series data.
 
@@ -27,17 +28,17 @@
     * ``t0[i]`` is a time offset (relative to a user-defined global reference)
       for the sample in ``values[i][0]``. Implemented as an LGDO
       :class:`.Array` with optional attribute ``units``.
     * ``dt[i]`` is the sampling period for the waveform at ``values[i]``.
       Implemented as an LGDO :class:`.Array` with optional attribute ``units``.
     * ``values[i]`` is the ``i``'th waveform in the table. Internally, the
       waveforms values may be either an LGDO :class:`.ArrayOfEqualSizedArrays`\
-      ``<1,1>`` or as an LGDO :class:`.VectorOfVectors` that supports
-      waveforms of unequal length. Can optionally be given a ``units``
-      attribute.
+      ``<1,1>``, an LGDO :class:`.VectorOfVectors` or
+      :class:`.VectorOfEncodedVectors` that supports waveforms of unequal
+      length. Can optionally be given a ``units`` attribute.
 
     Note
     ----
     On-disk and in-memory versions could be different e.g. if a compression
     routine is used.
     """
 
@@ -110,14 +111,15 @@
             t0_dtype = t0.dtype if hasattr(t0, "dtype") else np.float32
             nda = (
                 t0 if isinstance(t0, np.ndarray) else np.full(shape, t0, dtype=t0_dtype)
             )
             if nda.shape != shape:
                 nda.resize(shape, refcheck=True)
             t0 = Array(nda=nda)
+
         if t0_units is not None:
             t0.attrs["units"] = f"{t0_units}"
 
         if not isinstance(dt, Array):
             shape = (size,)
             dt_dtype = dt.dtype if hasattr(dt, "dtype") else np.float32
             nda = (
@@ -125,23 +127,29 @@
             )
             if nda.shape != shape:
                 nda.resize(shape, refcheck=True)
             dt = Array(nda=nda)
         if dt_units is not None:
             dt.attrs["units"] = f"{dt_units}"
 
-        if not isinstance(values, ArrayOfEqualSizedArrays) and not isinstance(
-            values, VectorOfVectors
+        if not isinstance(
+            values,
+            (
+                ArrayOfEqualSizedArrays,
+                VectorOfVectors,
+                VectorOfEncodedVectors,
+                ArrayOfEncodedEqualSizedArrays,
+            ),
         ):
             if isinstance(values, np.ndarray):
                 try:
                     wf_len = values.shape[1]
                 except Exception:
                     wf_len = None
-            if wf_len is None:  # VectorOfVectors
+            if wf_len is None:  # make a VectorOfVectors
                 shape_guess = (size, 100)
                 if dtype is None:
                     dtype = np.dtype(np.float64)
                 if values is None:
                     values = VectorOfVectors(shape_guess=shape_guess, dtype=dtype)
                 else:
                     flattened_data = np.concatenate(values)
@@ -151,15 +159,15 @@
                         length += len(values[i])
                         cumulative_length.append(length)
                     values = VectorOfVectors(
                         flattened_data=flattened_data,
                         cumulative_length=cumulative_length,
                         dtype=dtype,
                     )
-            else:  # ArrayOfEqualSizedArrays
+            else:  # make a ArrayOfEqualSizedArrays
                 shape = (size, wf_len)
                 if dtype is None:
                     dtype = (
                         values.dtype
                         if hasattr(values, "dtype")
                         else np.dtype(np.float64)
                     )
@@ -239,23 +247,18 @@
     def __str__(self):
         npopt = np.get_printoptions()
         np.set_printoptions(threshold=100)
 
         string = ""
 
         for i in range(self.size):
-            if isinstance(self.values, VectorOfVectors):
-                string += f"{self.values.get_vector(i)}"
-            else:
-                string += f"{self.values.nda[i]}"
-
-            string += f", dt={self.dt.nda[i]}"
+            string += f"{self.values[i]}, dt={self.dt[i]}"
             if self.dt_units:
                 string += f" {self.dt_units}"
-            string += f", t0={self.t0.nda[i]}"
+            string += f", t0={self.t0[i]}"
             if self.t0_units:
                 string += f" {self.t0_units}"
             if i < self.size - 1:
                 string += "\n"
 
         np.set_printoptions(**npopt)
         return string
```

### Comparing `pygama-1.2.0/src/pygama/math/histogram.py` & `pygama-1.3.0/src/pygama/math/histogram.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/math/peak_fitting.py` & `pygama-1.3.0/src/pygama/math/peak_fitting.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/math/utils.py` & `pygama-1.3.0/src/pygama/math/utils.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/pargen/AoE_cal.py` & `pygama-1.3.0/src/pygama/pargen/AoE_cal.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     files: list,
     lh5_path: str,
     cal_dict: dict,
     energy_param: str,
     cal_energy_param: str,
     cut_field: str = "Cal_cuts",
 ) -> tuple(np.array, np.array, np.array, np.array):
-
     """
     Loads in the A/E parameters needed and applies calibration constants to energy
     """
 
     sto = lh5.LH5Store()
 
     params = ["A_max", "tp_0_est", "tp_99", "dt_eff", energy_param, cal_energy_param]
@@ -94,15 +93,14 @@
     else:
         return lambda_s + lambda_b, sig, bkg
 
 
 def unbinned_aoe_fit(
     aoe: np.array, display: int = 0, verbose: bool = False
 ) -> tuple(np.array, np.array):
-
     """
     Fitting function for A/E, first fits just a gaussian before using the full pdf to fit
     if fails will return NaN values
     """
 
     hist, bins, var = pgh.get_hist(aoe, bins=500)
     bin_centers = (bins[:-1] + bins[1:]) / 2
@@ -189,15 +187,14 @@
     """Function definition for fitting A/E sigma against energy"""
     return np.sqrt(a + (b / x) ** 2)
 
 
 def AoEcorrection(
     energy: np.array, aoe: np.array, eres: list, plot_dict: dict = {}, display: int = 0
 ) -> tuple(np.array, np.array):
-
     """
     Calculates the corrections needed for the energy dependence of the A/E.
     Does this by fitting the compton continuum in slices and then applies fits to the centroid and variance.
     """
 
     comptBands_width = 20
     comptBands = np.array(
@@ -269,23 +266,31 @@
         fits_fig = plt.figure()
 
     # Fit each compton band
     for i, band in enumerate(comptBands):
         aoe_tmp = aoe[
             (energy > band) & (energy < band + comptBands_width) & (aoe > 0)
         ]  # [:20000]
-        pars, errs = unbinned_aoe_fit(aoe_tmp, display=display)
-        compt_aoe[i] = pars[2]
-        aoe_sigmas[i] = pars[3]
-        compt_aoe_err[i] = errs[2]
-        aoe_sigmas_err[i] = errs[3]
-        ratio[i] = pars[0] / pars[1]
-        ratio_err[i] = ratio[i] * np.sqrt(
-            (errs[0] / pars[0]) ** 2 + (errs[1] / pars[1]) ** 2
-        )
+        try:
+            pars, errs = unbinned_aoe_fit(aoe_tmp, display=display)
+            compt_aoe[i] = pars[2]
+            aoe_sigmas[i] = pars[3]
+            compt_aoe_err[i] = errs[2]
+            aoe_sigmas_err[i] = errs[3]
+            ratio[i] = pars[0] / pars[1]
+            ratio_err[i] = ratio[i] * np.sqrt(
+                (errs[0] / pars[0]) ** 2 + (errs[1] / pars[1]) ** 2
+            )
+        except:
+            compt_aoe[i] = np.nan
+            aoe_sigmas[i] = np.nan
+            compt_aoe_err[i] = np.nan
+            aoe_sigmas_err[i] = np.nan
+            ratio[i] = np.nan
+            ratio_err[i] = np.nan
 
         if display > 0:
             if np.isnan(errs[2]) | np.isnan(errs[3]) | (errs[2] == 0) | (errs[3] == 0):
                 pass
             else:
                 xs = np.arange(
                     pars[2] - 4 * pars[3], pars[2] + 3 * pars[3], pars[3] / 10
@@ -471,15 +476,14 @@
     else:
         return pars, sig_pars, results_dict
 
 
 def plot_compt_bands_overlayed(
     aoe: np.array, energy: np.array, eranges: list[tuple], aoe_range: list[float] = None
 ) -> None:
-
     """
     Function to plot various compton bands to check energy dependence and corrections
     """
 
     for erange in eranges:
         hist, bins, var = pgh.get_hist(
             aoe[(energy > erange - 10) & (energy < erange + 10) & (~np.isnan(aoe))],
@@ -497,15 +501,14 @@
         )
         plt.hist(aoe[idxs], bins=50, histtype="step", label=f"{erange-10}-{erange+10}")
 
 
 def plot_dt_dep(
     aoe: np.array, energy: np.array, dt: np.array, erange: list[tuple], title: str
 ) -> None:
-
     """
     Function to produce 2d histograms of A/E against drift time to check dependencies
     """
 
     hist, bins, var = pgh.get_hist(
         aoe[(energy > erange[0]) & (energy < erange[1]) & (~np.isnan(aoe))], bins=500
     )
@@ -587,23 +590,21 @@
     energy: np.array,
     peak: float,
     eres_pars: list = None,
     simplex=False,
     guess=None,
     verbose: bool = False,
 ) -> tuple(np.array, np.array):
-
     """
     Fitting function for energy peaks used to calculate survival fractions
     """
     hist, bins, var = pgh.get_hist(
         energy, dx=0.5, range=(np.nanmin(energy), np.nanmax(energy))
     )
     if guess is None:
-
         x0 = energy_guess(
             hist,
             bins,
             var,
             pgf.extended_gauss_step_pdf,
             peak,
             eres_pars,
@@ -753,15 +754,14 @@
     aoe: np.array,
     peak: float,
     ranges: tuple(int, int),
     dep_acc: float,
     eres_pars: list,
     display: int = 1,
 ) -> float:
-
     """
     Determines A/E cut by sweeping through values and for each one fitting the DEP to determine how many events survive.
     Then interpolates to get cut value at desired DEP survival fraction (typically 90%)
     """
 
     min_range, max_range = ranges
 
@@ -826,15 +826,14 @@
     aoe: np.array,
     peak: float,
     fit_width: tuple(int, int),
     aoe_cut_val: float,
     eres_pars: list,
     display: int = 0,
 ) -> tuple(np.array, np.array, np.array, float, float):
-
     """
     Calculates survival fraction for gamma lines using fitting method as in cut determination
     """
 
     # fwhm = np.sqrt(eres[0]+peak*eres[1])
     min_range = peak - fit_width[0]
     max_range = peak + fit_width[1]
@@ -851,15 +850,14 @@
     sf_errs = []
 
     cut_vals = np.arange(-5, 5, 0.2)
     # cut_vals = np.append(cut_vals, aoe_cut_val)
     final_cut_vals = []
     for cut_val in cut_vals:
         try:
-
             sf, err, cut_pars, surv_pars = get_survival_fraction(
                 peak_energy, peak_aoe, cut_val, peak, eres_pars
             )
             if np.isnan(cut_pars).all() == False and np.isnan(surv_pars).all() == False:
                 guess_pars_cut = cut_pars
                 guess_pars_surv = surv_pars
         except:
@@ -895,15 +893,14 @@
     energy: np.array,
     aoe: np.array,
     cut: float,
     peak: float,
     eres: list[float, float],
     display: int = 1,
 ) -> tuple(float, np.array, list):
-
     """
     Determines survival fraction for compton continuum by basic counting
     """
 
     fwhm = np.sqrt(eres[0] + peak * eres[1])
 
     emin = peak - 2 * fwhm
@@ -923,15 +920,14 @@
     peak: float,
     fit_width: tuple(int, int),
     eres_pars: list,
     aoe_low_cut_val: float,
     aoe_high_cut_val: float = None,
     display: int = 1,
 ) -> tuple(float, float):
-
     """
     Calculates survival fraction for gamma line without sweeping through values
     """
 
     min_range = peak - fit_width[0]
     max_range = peak + fit_width[1]
     if peak == "1592.5":
@@ -957,15 +953,14 @@
     aoe: np.array,
     peak: float,
     eres: list[float, float],
     aoe_low_cut_val: float,
     aoe_high_cut_val: float = None,
     display: int = 1,
 ) -> float:
-
     """
     Calculates survival fraction for compton contiuum without sweeping through values
     """
 
     fwhm = np.sqrt(eres[0] + peak * eres[1])
 
     emin = peak - 2 * fwhm
@@ -986,15 +981,14 @@
 
 def get_classifier(
     aoe: np.array,
     energy: np.array,
     mu_pars: list[float, float],
     sigma_pars: list[float, float],
 ) -> np.array:
-
     """
     Applies correction to A/E energy dependence
     """
 
     classifier = aoe / (mu_pars[0] * energy + mu_pars[1])
     classifier = (classifier - 1) / sigma_fit(energy, *sigma_pars)
     return classifier
@@ -1219,63 +1213,64 @@
     )
 
     if dt_corr == True:
         aoe, alpha = drift_time_correction(aoe_uncorr, energy, dt)
     else:
         aoe = aoe_uncorr
 
-    aoe_tmp = aoe[(energy > 1000) & (energy < 1300) & (aoe > 0)]  # [:20000]
-    bulk_pars, bulk_errs = unbinned_aoe_fit(aoe_tmp, display=0)
+    try:
+        aoe_tmp = aoe[(energy > 1000) & (energy < 1300) & (aoe > 0)]  # [:20000]
+        bulk_pars, bulk_errs = unbinned_aoe_fit(aoe_tmp, display=0)
+    except:
+        bulk_pars = np.full(8, np.nan)
+        log.error("1000-1300 keV mean determination failed")
 
-    log.info("Starting A/E correction")
-    mu_pars, sigma_pars, results_dict = AoEcorrection(energy, aoe, eres_pars)
-    log.info("Finished A/E correction")
+    try:
+        log.info("Starting A/E correction")
+        mu_pars, sigma_pars, results_dict = AoEcorrection(energy, aoe, eres_pars)
+        log.info("Finished A/E correction")
 
-    classifier = get_classifier(aoe, energy, mu_pars, sigma_pars)
+        classifier = get_classifier(aoe, energy, mu_pars, sigma_pars)
 
-    cut = get_aoe_cut_fit(energy, classifier, 1592, (40, 20), 0.9, eres_pars, display=0)
+    except:
+        log.error("A/E calibration failed")
+        mean_pars = np.full(2, np.nan)
+        sigma_pars = np.full(2, np.nan)
+
+    try:
+        cut = get_aoe_cut_fit(
+            energy, classifier, 1592, (40, 20), 0.9, eres_pars, display=0
+        )
+    except:
+        log.error("A/E cut determination failed")
+        cut = np.nan
 
     cal_dict.update(
         {
             "AoE_Corrected": {
                 "expression": f"(((A_max/{energy_param})/(a*{cal_energy_param} +b))-1)",
                 "parameters": {"a": mu_pars[0], "b": mu_pars[1]},
-            }
-        }
-    )
-
-    cal_dict.update(
-        {
+            },
             "AoE_Classifier": {
                 "expression": f"AoE_Corrected/(sqrt(c+(d/{cal_energy_param})**2)/(a*{cal_energy_param} +b))",
                 "parameters": {
                     "a": mu_pars[0],
                     "b": mu_pars[1],
                     "c": sigma_pars[0],
                     "d": sigma_pars[1],
                 },
-            }
-        }
-    )
-
-    cal_dict.update(
-        {
+            },
             "AoE_Low_Cut": {
                 "expression": "AoE_Classifier>a",
                 "parameters": {"a": cut},
-            }
-        }
-    )
-
-    cal_dict.update(
-        {
+            },
             "AoE_Double_Sided_Cut": {
                 "expression": "(b>AoE_Classifier)&(AoE_Classifier>a)",
                 "parameters": {"a": cut, "b": aoe_high_cut},
-            }
+            },
         }
     )
 
     try:
         log.info("  Compute low side survival fractions: ")
 
         peaks_of_interest = [1592.5, 1620.5, 2039, 2103.53, 2614.50]
@@ -1517,15 +1512,15 @@
                 plt.close()
 
             return cal_dict, out_dict, plot_dict
         else:
             return cal_dict, out_dict
 
     except:
-        log.error("survival fraction determination failed")
+        log.error("A/E Survival fraction determination failed")
         out_dict = {
             "correction_fit_results": results_dict,
             "A/E_Energy_param": "cuspEmax",
             "Cal_energy_param": "cuspEmax_ctc",
             "dt_param": "dt_eff",
             "rt_correction": False,
             "1000-1300keV_mean": bulk_pars[2],
```

### Comparing `pygama-1.2.0/src/pygama/pargen/cuts.py` & `pygama-1.3.0/src/pygama/pargen/cuts.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         for key in possible_keys:
             if key in param:
                 out_params.append(key)
     return np.unique(out_params).tolist()
 
 
 def generate_cuts(
-    data: dict[str, np.ndarray], parameters: dict[str, int], rounding: int = 2
+    data: dict[str, np.ndarray], parameters: dict[str, int], rounding: int = 4
 ) -> dict:
     """
     Finds double sided cut boundaries for a file for the parameters specified
 
     Parameters
     ----------
     data : lh5 table or dictionary of arrays
@@ -72,50 +72,30 @@
             all_par_array = data[par].to_numpy()
         except KeyError:
             all_par_array = data.eval(par).to_numpy()
         idxs = (all_par_array > np.nanpercentile(all_par_array, 1)) & (
             all_par_array < np.nanpercentile(all_par_array, 99)
         )
         par_array = all_par_array[idxs]
-        counts, start_bins, var = pgh.get_hist(par_array, 1000)
+        bin_width = (
+            np.nanpercentile(par_array, 70) - np.nanpercentile(par_array, 50)
+        ) / 5
+
+        counts, start_bins, var = pgh.get_hist(
+            par_array, range=(np.nanmin(par_array), np.nanmax(par_array)), dx=bin_width
+        )
         max_idx = np.argmax(counts)
         mu = start_bins[max_idx]
         try:
-            pars, cov = pgf.gauss_mode_width_max(
-                counts,
-                start_bins,
-                mode_guess=mu,
-                n_bins=50,
-                cost_func="Least Squares",
-                inflate_errors=False,
-                gof_method="var",
-            )
-
-            guess_mu, guess_sig, guess_amp = pars
-
-            lower_bound = guess_mu - 10 * guess_sig
+            fwhm = pgh.get_fwhm(counts, start_bins)[0]
+            guess_sig = fwhm / 2.355
 
-            upper_bound = guess_mu + 10 * guess_sig
+            lower_bound = mu - 10 * guess_sig
 
-            if lower_bound < np.nanmin(par_array) or upper_bound > np.nanmax(par_array):
-                pars, cov = pgf.gauss_mode_width_max(
-                    counts,
-                    start_bins,
-                    mode_guess=mu,
-                    n_bins=5,
-                    cost_func="Least Squares",
-                    inflate_errors=False,
-                    gof_method="var",
-                )
-
-            guess_mu, guess_sig, guess_amp = pars
-
-            lower_bound = guess_mu - 10 * guess_sig
-
-            upper_bound = guess_mu + 10 * guess_sig
+            upper_bound = mu + 10 * guess_sig
 
         except:
             bin_range = 1000
 
             if max_idx < bin_range:
                 lower_bound_idx = 0
             else:
@@ -125,17 +105,17 @@
             if max_idx > len(start_bins) - bin_range:
                 upper_bound_idx = -1
             else:
                 upper_bound_idx = max_idx + bin_range
 
             upper_bound = start_bins[upper_bound_idx]
 
-        if lower_bound < np.nanmin(par_array):
+        if (lower_bound < np.nanmin(par_array)) or (lower_bound > np.nanmax(par_array)):
             lower_bound = np.nanmin(par_array)
-        if upper_bound > np.nanmax(par_array):
+        if (upper_bound > np.nanmax(par_array)) or (upper_bound < np.nanmin(par_array)):
             upper_bound = np.nanmax(par_array)
 
         try:
             counts, bins, var = pgh.get_hist(
                 par_array, bins=200, range=(lower_bound, upper_bound)
             )
 
@@ -148,16 +128,19 @@
                 bins,
                 mode_guess=mean,
                 n_bins=20,
                 cost_func="Least Squares",
                 inflate_errors=False,
                 gof_method="var",
             )
-            mean - pars[0]
+            mean = pars[0]
             std = fwhm / 2.355
+
+            if mean < np.nanmin(bins) or mean > np.nanmax(bins):
+                raise IndexError
         except IndexError:
             bin_range = 5000
 
             if max_idx < bin_range:
                 lower_bound_idx = 0
             else:
                 lower_bound_idx = max_idx - bin_range
@@ -165,15 +148,15 @@
 
             if max_idx > len(start_bins) - bin_range:
                 upper_bound_idx = -1
             else:
                 upper_bound_idx = max_idx + bin_range
             upper_bound = start_bins[upper_bound_idx]
             counts, bins, var = pgh.get_hist(
-                par_array, bins=1000, range=(lower_bound, upper_bound)
+                par_array, bins=200, range=(lower_bound, upper_bound)
             )
 
             bin_centres = pgh.get_bin_centers(bins)
 
             fwhm = pgh.get_fwhm(counts, bins)[0]
             mean = float(bin_centres[np.argmax(counts)])
             std = fwhm / 2.355
@@ -181,16 +164,16 @@
         if isinstance(num_sigmas, (int, float)):
             num_sigmas_left = num_sigmas
             num_sigmas_right = num_sigmas
         elif isinstance(num_sigmas, dict):
             if "left" in num_sigmas:
                 num_sigmas_left = num_sigmas["left"]
             else:
-                num_sigmas["left"] = -np.inf
-                num_sigmas_left = -np.inf
+                num_sigmas["left"] = np.inf
+                num_sigmas_left = np.inf
             if "right" in num_sigmas:
                 num_sigmas_right = num_sigmas["right"]
             else:
                 num_sigmas["right"] = np.inf
                 num_sigmas_right = np.inf
         upper = float((num_sigmas_right * std) + mean)
         lower = float((-num_sigmas_left * std) + mean)
@@ -202,15 +185,14 @@
         }
     return output_dict
 
 
 def get_cut_indexes(
     all_data: dict[str, np.ndarray], cut_dict: dict, energy_param: str = "trapTmax"
 ) -> list[int]:
-
     """
     Returns a mask of the data, for a single file, that passes cuts based on dictionary of cuts
     in form of cut boundaries above
     Parameters
     ----------
     File : dict or lh5_table
            dictionary of parameters + array such as load_nda or lh5 table of params
@@ -255,15 +237,14 @@
 
 
 def cut_dict_to_hit_dict(cut_dict, final_cut_field="is_valid_cal"):
     out_dict = {}
     symbols = "/-+*"
     replacewith = "_"
     for i, param in enumerate(cut_dict):
-
         out_dict[
             f"{''.join(replacewith  if c in symbols else c for c in param).replace('(','').replace(')','')}_cut"
         ] = {
             "expression": f"(a<({param}))&(({param})<b)",
             "parameters": {
                 "a": cut_dict[param]["Lower Boundary"],
                 "b": cut_dict[param]["Upper Boundary"],
@@ -274,69 +255,109 @@
         quality_cut_exp += f"({''.join(replacewith  if c in symbols else c for c in par).replace('(','').replace(')','')}_cut)&"
     quality_cut_exp += f"({''.join(replacewith  if c in symbols else c for c in list(cut_dict)[-1]).replace('(','').replace(')','')}_cut)"
     out_dict[final_cut_field] = {"expression": quality_cut_exp, "parameters": {}}
     return out_dict
 
 
 def find_pulser_properties(df, energy="daqenergy"):
-
-    hist, bins, var = pgh.get_hist(df[energy], dx=1, range=(100, np.nanmax(df[energy])))
+    if np.nanmax(df[energy]) > 8000:
+        hist, bins, var = pgh.get_hist(
+            df[energy], dx=1, range=(1000, np.nanmax(df[energy]))
+        )
+        allowed_err = 200
+    else:
+        hist, bins, var = pgh.get_hist(
+            df[energy], dx=0.2, range=(500, np.nanmax(df[energy]))
+        )
+        allowed_err = 50
     if np.any(var == 0):
         var[np.where(var == 0)] = 1
-    imaxes = pgc.get_i_local_maxima(hist / np.sqrt(var), 5)
+    imaxes = pgc.get_i_local_maxima(hist / np.sqrt(var), 3)
     peak_energies = pgh.get_bin_centers(bins)[imaxes]
     pt_pars, pt_covs = pgc.hpge_fit_E_peak_tops(
-        hist, bins, var, peak_energies, n_to_fit=15
+        hist, bins, var, peak_energies, n_to_fit=10
     )
     peak_e_err = pt_pars[:, 1] * 4
 
-    out_pulsers = []
-    for i, e in enumerate(peak_energies):
-        if peak_e_err[i] > 200:
+    allowed_mask = np.ones(len(peak_energies), dtype=bool)
+    for i, e in enumerate(peak_energies[1:-1]):
+        i += 1
+        if peak_e_err[i] > allowed_err:
             continue
-        else:
-            try:
-                e_cut = (df[energy] > e - peak_e_err[i]) & (
-                    df[energy] < e + peak_e_err[i]
+        if i == 1:
+            if (
+                e - peak_e_err[i] < peak_energies[i - 1] + peak_e_err[i - 1]
+                and peak_e_err[i - 1] < allowed_err
+            ):
+                overlap = (
+                    peak_energies[i - 1]
+                    + peak_e_err[i - 1]
+                    - (peak_energies[i] - peak_e_err[i])
                 )
-                df_peak = df[e_cut]
-
-                time_since_last = (
-                    df_peak.timestamp.values[1:] - df_peak.timestamp.values[:-1]
+                peak_e_err[i] -= overlap * (
+                    peak_e_err[i] / (peak_e_err[i] + peak_e_err[i - 1])
+                )
+                peak_e_err[i - 1] -= overlap * (
+                    peak_e_err[i - 1] / (peak_e_err[i] + peak_e_err[i - 1])
                 )
 
-                tsl = time_since_last[
-                    (time_since_last >= 0)
-                    & (time_since_last < np.percentile(time_since_last, 99.9))
-                ]
-
-                bins = np.arange(0.1, 5, 0.0001)
-                bcs = pgh.get_bin_centers(bins)
-                hist, bins, var = pgh.get_hist(tsl, bins=bins)
+        if (
+            e + peak_e_err[i] > peak_energies[i + 1] - peak_e_err[i + 1]
+            and peak_e_err[i + 1] < allowed_err
+        ):
+            overlap = (e + peak_e_err[i]) - (peak_energies[i + 1] - peak_e_err[i + 1])
+            total = peak_e_err[i] + peak_e_err[i + 1]
+            peak_e_err[i] -= (overlap) * (peak_e_err[i] / total)
+            peak_e_err[i + 1] -= (overlap) * (peak_e_err[i + 1] / total)
 
-                maxs = pgc.get_i_local_maxima(hist, 40)
-                if len(maxs) < 2:
-                    continue
-                else:
+    out_pulsers = []
+    for i, e in enumerate(peak_energies[allowed_mask]):
+        if peak_e_err[i] > allowed_err:
+            continue
 
-                    max_locs = np.array([0.0])
-                    max_locs = np.append(max_locs, bcs[np.array(maxs)])
-                    if (
-                        len(np.where(np.abs(np.diff(np.diff(max_locs))) <= 0.001)[0])
-                        > 1
-                        or (np.abs(np.diff(np.diff(max_locs))) <= 0.001).all()
-                    ):
-                        pulser_e = e
-                        period = stats.mode(tsl).mode[0]
-                        out_pulsers.append((pulser_e, peak_e_err[i], period, energy))
-
-                    else:
-                        continue
-            except:
+        try:
+            e_cut = (df[energy] > e - peak_e_err[i]) & (df[energy] < e + peak_e_err[i])
+            df_peak = df[e_cut]
+
+            time_since_last = (
+                df_peak.timestamp.values[1:] - df_peak.timestamp.values[:-1]
+            )
+
+            tsl = time_since_last[
+                (time_since_last >= 0)
+                & (time_since_last < np.percentile(time_since_last, 99.9))
+            ]
+
+            bins = np.arange(0.1, 5, 0.001)
+            bcs = pgh.get_bin_centers(bins)
+            hist, bins, var = pgh.get_hist(tsl, bins=bins)
+
+            maxs = pgc.get_i_local_maxima(hist, 45)
+            maxs = maxs[maxs > 20]
+
+            super_max = pgc.get_i_local_maxima(hist, 500)
+            super_max = super_max[super_max > 20]
+            if len(maxs) < 2:
                 continue
+            else:
+                max_locs = np.array([0.0])
+                max_locs = np.append(max_locs, bcs[np.array(maxs)])
+                if (
+                    len(np.where(np.abs(np.diff(np.diff(max_locs))) <= 0.001)[0]) > 1
+                    or (np.abs(np.diff(np.diff(max_locs))) <= 0.001).all()
+                    or len(super_max) > 0
+                ):
+                    pulser_e = e
+                    period = stats.mode(tsl).mode[0]
+                    out_pulsers.append((pulser_e, peak_e_err[i], period, energy))
+
+                else:
+                    continue
+        except:
+            continue
     return out_pulsers
 
 
 def tag_pulsers(df, chan_info, window=0.01):
     df["isPulser"] = 0
 
     if isinstance(chan_info, tuple):
```

### Comparing `pygama-1.2.0/src/pygama/pargen/data_cleaning.py` & `pygama-1.3.0/src/pygama/pargen/data_cleaning.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/pargen/energy_cal.py` & `pygama-1.3.0/src/pygama/pargen/energy_cal.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,15 @@
         or func == pgf.gauss_step_pdf
         or func == pgf.extended_gauss_step_pdf
     ):
         # get mu and height from a gauss fit, also sigma as fallback
         pars, cov = pgf.gauss_mode_width_max(hist, bins, var)
         bin_centres = pgh.get_bin_centers(bins)
         if pars is None:
-            log.warning("get_hpge_E_peak_par_guess: gauss_mode_width_max failed")
+            log.info("get_hpge_E_peak_par_guess: gauss_mode_width_max failed")
             i_0 = np.argmax(hist)
             mu = bin_centres[i_0]
             height = hist[i_0]
             sigma_guess = None
         else:
             mu = pars[0]
             sigma_guess = pars[1]
@@ -298,15 +298,15 @@
                 bins,
                 var,
                 mx=height,
                 bl=bg - step / 2,
                 method="fit_slopes",
             )[0]
             if sigma == 0:
-                log.warning("get_hpge_E_peak_par_guess: sigma estimation failed")
+                log.info("get_hpge_E_peak_par_guess: sigma estimation failed")
                 if sigma_guess is not None:
                     sigma = sigma_guess
                 else:
                     return []
 
         # now compute amp and return
         n_sig = np.sum(
@@ -318,20 +318,19 @@
         return [n_sig, mu, sigma / 2, n_bkg, hstep, bins[0], bins[-1], 0]
 
     if (
         func == pgf.radford_cdf
         or func == pgf.radford_pdf
         or func == pgf.extended_radford_pdf
     ):
-
         # guess mu, height
         pars, cov = pgf.gauss_mode_width_max(hist, bins, var)
         bin_centres = pgh.get_bin_centers(bins)
         if pars is None:
-            log.warning("get_hpge_E_peak_par_guess: gauss_mode_width_max failed")
+            log.info("get_hpge_E_peak_par_guess: gauss_mode_width_max failed")
             sigma_guess = None
 
         else:
             sigma_guess = pars[1]
             # mu=pars[0]
             # height=pars[2]
         i_0 = np.argmax(hist)
@@ -576,15 +575,15 @@
                     Extended=True,
                     fixed=fixed,
                     simplex=simplex,
                     bounds=bounds,
                 )
 
             csqr = pgf.goodness_of_fit(
-                hist, bins, None, gof_func_i, pars_i, method="LR"
+                hist, bins, None, gof_func_i, pars_i, method="Pearson"
             )
             p_val = scipy.stats.chi2.sf(csqr[0], csqr[1])
 
             pars_i = np.array(pars_i)[mask]
             errs_i = np.array(errs_i)[mask]
             cov_i = np.array(cov_i)[mask, :][:, mask]
 
@@ -835,15 +834,15 @@
     # re-bin the histogram in ~0.2 keV bins with updated E scale par for peak-top fits
     Euc_min, Euc_max = (
         (np.poly1d(roughpars) - i).roots
         for i in (peaks_keV[0] * 0.9, peaks_keV[-1] * 1.1)
     )
     Euc_min = Euc_min[np.logical_and(Euc_min >= 0, Euc_min <= max(Euc_max))][0]
     Euc_max = Euc_max[
-        np.logical_and(Euc_max >= Euc_min, Euc_max <= np.nanmax(E_uncal))
+        np.logical_and(Euc_max >= Euc_min, Euc_max <= np.nanmax(E_uncal) * 1.1)
     ][0]
     dEuc = 0.2 / roughpars[-2]
 
     if uncal_is_int:
         Euc_min, Euc_max, dEuc = pgh.better_int_binning(
             x_lo=Euc_min, x_hi=Euc_max, dx=dEuc
         )
@@ -954,15 +953,15 @@
         varnames = func_i.__code__.co_varnames[1 : len(pk_pars[-1]) + 1]
         parsi = np.asarray(parsi, dtype=float)
         errorsi = np.asarray(errorsi, dtype=float)
         covsi = np.asarray(covsi, dtype=float)
         # parsigsi = np.sqrt(covsi.diagonal())
         log.info(f"\tEnergy: {str(Ei)}")
         log.info(f"\t\tParameter  |    Value +/- Sigma  ")
-        for (vari, pari, errorsi) in zip(varnames, parsi, errorsi):
+        for vari, pari, errorsi in zip(varnames, parsi, errorsi):
             log.info(
                 f'\t\t{str(vari).ljust(10)} | {("%4.2f" % pari).rjust(8)} +/- {("%4.2f" % errorsi).ljust(8)}'
             )
             # fwhm??
 
     # Do a second calibration to the results of the full peak fits
     mus = [
@@ -1120,15 +1119,14 @@
         while ii < len(ixtup) - 1:
             if ixtup[ii] < ixtup[ii + 1] - 1:
                 break
             ii += 1
 
         # quit if ii is the last index of ixtup and it's already maxed out
         if not (ii == len(ixtup) - 1 and ixtup[ii] == len(xx) - 1):
-
             # otherwise increment ii and reset indices < ii
             ixtup[ii] += 1
             ixtup[0:ii] = list(range(ii))
             continue
 
         # increment iytup
         # first find the index of iytup that needs to be incremented
@@ -1136,15 +1134,14 @@
         while ii < len(iytup) - 1:
             if iytup[ii] < iytup[ii + 1] - 1:
                 break
             ii += 1
 
         # quit if ii is the last index of iytup and it's already maxed out
         if not (ii == len(iytup) - 1 and iytup[ii] == len(yy) - 1):
-
             # otherwise increment ii and reset indices < ii
             iytup[ii] += 1
             iytup[0:ii] = list(range(ii))
             ixtup = np.array(list(range(len(iytup))))  # (reset ix)
             continue
 
         if n_close == len(iytup):  # found best
@@ -1200,15 +1197,14 @@
         log.error(f"get_i_local_extrema: delta ({delta}) must be positive")
         return np.array(imaxes), np.array(imins)
 
     # now loop over data
     imax, imin = 0, 0
     find_max = True
     for i in range(len(data)):
-
         if data[i] > data[imax]:
             imax = i
         if data[i] < data[imin]:
             imin = i
 
         if find_max:
             # if the sample is less than the current max by more than delta,
@@ -1288,19 +1284,17 @@
     n_pks = len(cal_pks) if len(cal_pks) < len(data_pks) else len(data_pks)
 
     cal_sets = combinations(range(len(cal_pks)), n_pks)
     data_sets = combinations(range(len(data_pks)), n_pks)
 
     best_err, best_m, best_b = np.inf, None, None
     for i, cal_set in enumerate(cal_sets):
-
         cal = cal_pks[list(cal_set)]  # lit energies for this set
 
         for data_set in data_sets:
-
             data = data_pks[list(data_set)]  # uncal energies for this set
 
             m, b, _, _, _ = linregress(data, y=cal)
             err = np.sum((cal - (m * data + b)) ** 2)
 
             if err < best_err:
                 best_err, best_m, best_b = err, m, b
@@ -1461,15 +1455,14 @@
         if plotFigure is not None:
             plot_map[energy] = (bin_centers, peak_hist)
 
     # Do a linear fit to find the calibration
     linear_cal = np.polyfit(centers, cal_peaks, deg=1)
 
     if plotFigure is not None:
-
         plt.figure(plotFigure.number)
         plt.clf()
 
         grid = gs.GridSpec(peak_num, 3)
         ax_line = plt.subplot(grid[:, 1])
         ax_spec = plt.subplot(grid[:, 2])
```

### Comparing `pygama-1.2.0/src/pygama/pargen/energy_optimisation.py` & `pygama-1.3.0/src/pygama/pargen/energy_optimisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,15 +237,14 @@
     gof_range,
     fit_range=(np.inf, np.inf),
     guess=None,
     tol=None,
     verbose=False,
     display=0,
 ):
-
     """
     Unbinned fit to energy. This is different to the default fitting as
     it will try different fitting methods and choose the best. This is necessary for the lower statistics.
     """
 
     bin_width = 1
     lower_bound = (np.nanmin(energy) // bin_width) * bin_width
@@ -355,16 +354,24 @@
         cs = cs[0] / cs[1]
         valid3 = (
             m.valid
             # & m.accurate
             & (~np.isnan(m.errors).any())
             & (~(np.array(m.errors[:-3]) == 0).all())
         )
-        if valid3 == False:
-            raise RuntimeError
+        if valid3 is False:
+            try:
+                m.minos()
+                valid3 = (
+                    m.valid
+                    & (~np.isnan(m.errors).any())
+                    & (~(np.array(m.errors[:-3]) == 0).all())
+                )
+            except:
+                raise RuntimeError
 
         pars = np.array(m.values)[:-1]
         errs = np.array(m.errors)[:-1]
         cov = np.array(m.covariance)[:-1, :-1]
         csqr = cs
 
     elif valid2 == False or cs * 1.05 < cs2:
@@ -405,15 +412,14 @@
     gof_func,
     peak,
     kev_width,
     guess=None,
     kev=False,
     display=0,
 ):
-
     """
     Applies the drift time correction and fits the peak returns the fwhm, fwhm/max and associated errors,
     along with the number of signal events and the reduced chi square of the fit. Can return result in ADC or keV.
     """
 
     correction = np.multiply(
         np.multiply(alpha, dt, dtype="float64"), Energies, dtype="float64"
@@ -670,15 +676,15 @@
             if fwhms[-1] < best_fwhm:
                 best_fwhm = fwhms[-1]
                 best_fit = fit_pars
         log.info(f"alpha: {alpha}, fwhm/max:{fwhm_o_max}+-{fwhm_o_max_err}")
 
     # Make sure fit isn't based on only a few points
     if len(fwhms) < 10:
-        log.error("less than 10 fits successful")
+        log.debug("less than 10 fits successful")
         return {
             "fwhm": np.nan,
             "fwhm_err": np.nan,
             "alpha": np.nan,
             "alpha_err": np.nan,
             "chisquare": np.nan,
             "n_sig": np.nan,
@@ -719,27 +725,27 @@
                 fit_vals + yerr_boot,
                 facecolor="C1",
                 alpha=0.5,
             )
             plt.show()
 
     except:
-        log.error("alpha fit failed")
+        log.debug("alpha fit failed")
         return {
             "fwhm": np.nan,
             "fwhm_err": np.nan,
             "alpha": np.nan,
             "alpha_err": np.nan,
             "chisquare": np.nan,
             "n_sig": np.nan,
             "n_sig_err": np.nan,
         }
 
     if np.isnan(fit_vals).all():
-        log.error("alpha fit all nan")
+        log.debug("alpha fit all nan")
         return {
             "fwhm": np.nan,
             "fwhm_err": np.nan,
             "alpha": np.nan,
             "alpha_err": np.nan,
             "chisquare": np.nan,
             "n_sig": np.nan,
@@ -787,15 +793,15 @@
                 gof_func,
                 peak,
                 kev_width,
                 kev=True,
                 display=display,
             )
         if np.isnan(final_fwhm) or np.isnan(final_err):
-            log.error(f"final fit failed, alpha was {alpha}")
+            log.debug(f"final fit failed, alpha was {alpha}")
         return {
             "fwhm": final_fwhm,
             "fwhm_err": final_err,
             "alpha": alpha,
             "alpha_err": alpha_err,
             "chisquare": csqr,
             "n_sig": n_sig,
@@ -920,35 +926,43 @@
         kev_widths = [kev_widths]
 
     sto = lh5.LH5Store()
     df = lh5.load_dfs(raw_files, ["daqenergy", "timestamp"], lh5_path)
 
     pulser_props = cts.find_pulser_properties(df, energy="daqenergy")
     if len(pulser_props) > 0:
-        out_df = cts.tag_pulsers(df, pulser_props, window=0.001)
-        ids = out_df.isPulser == 1
+        final_mask = None
+        for entry in pulser_props:
+            e_cut = (df.daqenergy.values < entry[0] + entry[1]) & (
+                df.daqenergy.values > entry[0] - entry[1]
+            )
+            if final_mask is None:
+                final_mask = e_cut
+            else:
+                final_mask = final_mask | e_cut
+        ids = final_mask
         log.debug(f"pulser found: {pulser_props}")
     else:
         log.debug("no_pulser")
         ids = np.zeros(len(df.daqenergy.values), dtype=bool)
     # Get events around peak using raw file values
     initial_mask = (df.daqenergy.values > threshold) & (~ids)
     rough_energy = df.daqenergy.values[initial_mask]
     initial_idxs = np.where(initial_mask)[0]
 
     guess_keV = 2620 / np.nanpercentile(rough_energy, 99)
     Euc_min = threshold / guess_keV * 0.6
     Euc_max = 2620 / guess_keV * 1.1
-    dEuc = 1 / guess_keV
+    dEuc = 1  # / guess_keV
     hist, bins, var = pgh.get_hist(rough_energy, range=(Euc_min, Euc_max), dx=dEuc)
     detected_peaks_locs, detected_peaks_keV, roughpars = pgc.hpge_find_E_peaks(
         hist,
         bins,
         var,
-        np.array([238.632, 583.191, 727.330, 860.564, 1620.5, 2614.553]),
+        np.array([238.632, 583.191, 727.330, 860.564, 1620.5, 2103.53, 2614.553]),
     )
     log.debug(f"detected {detected_peaks_keV} keV peaks at {detected_peaks_locs}")
 
     masks = []
     for peak_idx in peak_idxs:
         peak = peaks_keV[peak_idx]
         kev_width = kev_widths[peak_idx]
@@ -989,23 +1003,23 @@
 
     if isinstance(dsp_config, str):
         with open(dsp_config) as r:
             dsp_config = json.load(r)
 
     dsp_config["outputs"] = cts.get_keys(
         dsp_config["outputs"], list(cut_parameters)
-    ) + ["energy_parameter"]
+    ) + [energy_parameter]
 
     log.debug("Processing data")
     tb_data = opt.run_one_dsp(input_data, dsp_config, db_dict=db_dict)
 
     cut_dict = cts.generate_cuts(tb_data, cut_parameters)
     log.debug(f"Cuts are: {cut_dict}")
     log.debug("Loaded Cuts")
-    ct_mask = cts.get_cut_indexes(tb_data, cut_dict, "raw")
+    ct_mask = cts.get_cut_indexes(tb_data, cut_dict)
 
     final_events = []
     for peak_idx in peak_idxs:
         peak = peaks_keV[peak_idx]
         kev_width = kev_widths[peak_idx]
 
         peak_ids = np.array(idx_list[peak_idx])
@@ -1039,14 +1053,18 @@
         updated_adc_to_kev = peak / params[0][1]
         e_lower_lim = params[0][1] - (kev_width[0]) / updated_adc_to_kev
         e_upper_lim = params[0][1] + (kev_width[1]) / updated_adc_to_kev
         log.info(f"lower lim is :{e_lower_lim}, upper lim is {e_upper_lim}")
         final_mask = (energy > e_lower_lim) & (energy < e_upper_lim)
         final_events.append(peak_ids[final_mask][:n_events])
         log.info(f"{len(peak_ids[final_mask][:n_events])} passed selections for {peak}")
+        if len(peak_ids[final_mask]) < 0.5 * n_events:
+            log.warning("Less than half number of specified events found")
+        elif len(peak_ids[final_mask]) < 0.1 * n_events:
+            log.error("Less than 10% number of specified events found")
 
     sort_index = np.argsort(np.concatenate(final_events))
     idx_list = get_wf_indexes(sort_index, [len(mask) for mask in final_events])
     idxs = np.array(sorted(np.concatenate(final_events)))
 
     final_data = index_data(input_data, idxs)
     return final_data, idx_list
@@ -1056,22 +1074,19 @@
     """
     Fit the energy resolution curve
     """
     return np.sqrt(m0 + m1 * x + m2 * (x**2))
 
 
 def interpolate_energy(peak_energies, points, err_points, energy):
-
     nan_mask = np.isnan(points) | (points < 0)
     if len(points[~nan_mask]) < 3:
         return np.nan, np.nan, np.nan
-    elif nan_mask[-1] == True or nan_mask[-2] == True:
-        return np.nan, np.nan, np.nan
     else:
-        param_guess = [0.2, 0.001, 0.000001]  #
+        param_guess = [2, 0.001, 0.000001]  #
         # param_bounds = (0, [10., 1. ])#
         try:
             fit_pars, fit_covs = curve_fit(
                 fwhm_slope,
                 peak_energies[~nan_mask],
                 points[~nan_mask],
                 sigma=err_points[~nan_mask],
@@ -1087,16 +1102,18 @@
             # generate set of bootstrapped parameters
             par_b = rng.multivariate_normal(fit_pars, fit_covs, size=1000)
             qbb_vals = np.array([fwhm_slope(energy, *p) for p in par_b])
             qbb_err = np.nanstd(qbb_vals)
         except:
             return np.nan, np.nan, np.nan
 
-        if nan_mask[-2] == True:
-            qbb_vals += qbb_err
+        if nan_mask[-1] == True or nan_mask[-2] == True:
+            qbb_err = np.nan
+        if qbb_err / fit_qbb > 0.1:
+            qbb_err = np.nan
 
     return fit_qbb, qbb_err, fit_pars
 
 
 def fom_FWHM(tb_in, kwarg_dict, ctc_parameter, alpha, idxs=None, display=0):
     """
     FOM for sweeping over ctc values to find the best value, returns the best found fwhm
@@ -1113,17 +1130,17 @@
         dt = tb_in["dt_eff"].nda
     elif ctc_parameter == "dt":
         dt = np.subtract(tb_in["tp_99"].nda, tb_in["tp_0_est"].nda, dtype="float64")
     elif ctc_parameter == "rt":
         dt = np.subtract(tb_in["tp_99"].nda, tb_in["tp_01"].nda, dtype="float64")
     if np.isnan(Energies).any() or np.isnan(dt).any():
         if np.isnan(Energies).any():
-            log.warning(f"nan energy values for peak {peak}")
+            log.debug(f"nan energy values for peak {peak}")
         else:
-            log.warning(f"nan dt values for peak {peak}")
+            log.debug(f"nan dt values for peak {peak}")
         return {
             "fwhm": np.nan,
             "fwhm_err": np.nan,
             "alpha": np.nan,
             "chisquare": np.nan,
             "n_sig": np.nan,
             "n_sig_err": np.nan,
@@ -1177,19 +1194,19 @@
     ctc_param = kwarg_dict["ctc_param"]
     peak_dicts = kwarg_dict["peak_dicts"]
 
     out_dict = fom_FWHM_with_dt_corr_fit(
         data, peak_dicts[0], ctc_param, idxs=idx_list[0], display=0
     )
     out_dict["y_val"] = out_dict["fwhm"]
+    out_dict["y_err"] = out_dict["fwhm_err"]
     return out_dict
 
 
 def new_fom(data, kwarg_dict):
-
     peaks = kwarg_dict["peaks_keV"]
     idx_list = kwarg_dict["idx_list"]
     ctc_param = kwarg_dict["ctc_param"]
 
     peak_dicts = kwarg_dict["peak_dicts"]
 
     out_dict = fom_FWHM_with_dt_corr_fit(
@@ -1222,14 +1239,15 @@
         np.array(peaks), np.array(fwhms), np.array(fwhm_errs), 2039
     )
 
     log.info(f"Qbb fwhm is {qbb} keV +- {qbb_err}")
 
     return {
         "y_val": qbb,
+        "y_err": qbb_err,
         "qbb_fwhm": qbb,
         "qbb_fwhm_err": qbb_err,
         "alpha": alpha,
         "peaks": peaks.tolist(),
         "fwhms": fwhms,
         "fwhm_errs": fwhm_errs,
         "n_events": n_sig,
@@ -1242,27 +1260,25 @@
 )
 
 
 class BayesianOptimizer:
     np.random.seed(55)
     lambda_param = 0.01
     eta_param = 0
-    kernel = None
     # FIXME: the following throws a TypeError
     # kernel=ConstantKernel(1.0, constant_value_bounds="fixed") * RBF(1, length_scale_bounds="fixed") #+ WhiteKernel(noise_level=0.0111)
 
-    def __init__(self, acq_func, batch_size):
-
+    def __init__(self, acq_func, batch_size, kernel=None):
         self.dims = []
         self.current_iter = 0
 
         self.batch_size = batch_size
         self.iters = 0
 
-        self.gauss_pr = GaussianProcessRegressor(kernel=self.kernel)
+        self.gauss_pr = GaussianProcessRegressor(kernel=kernel)
         self.best_samples_ = pd.DataFrame(columns=["x", "y", "ei"])
         self.distances_ = []
 
         if acq_func == "ei":
             self.acq_function = self._get_expected_improvement
         elif acq_func == "ucb":
             self.acq_function = self._get_ucb
@@ -1273,84 +1289,62 @@
         self.dims.append(
             OptimiserDimension(name, parameter, min_val, max_val, rounding, unit)
         )
 
     def get_n_dimensions(self):
         return len(self.dims)
 
-    def add_initial_values(self, x_init, y_init):
+    def add_initial_values(self, x_init, y_init, yerr_init):
         self.x_init = x_init
         self.y_init = y_init
+        self.yerr_init = yerr_init
 
     def _get_expected_improvement(self, x_new):
-
-        # Using estimate from Gaussian surrogate instead of actual function for
-        # a new trial data point to avoid cost
-
         mean_y_new, sigma_y_new = self.gauss_pr.predict(
             np.array([x_new]), return_std=True
         )
-        sigma_y_new = sigma_y_new.reshape(-1, 1)[0]
-
-        # Using estimates from Gaussian surrogate instead of actual function for
-        # entire prior distribution to avoid cost
 
         mean_y = self.gauss_pr.predict(self.x_init)
         min_mean_y = np.min(mean_y)
-        z = (mean_y_new - min_mean_y - self.eta_param) / (sigma_y_new + 1e-9)  #
-        exp_imp = (mean_y_new - min_mean_y - self.eta_param) * norm.cdf(
-            z
-        ) + sigma_y_new * norm.pdf(z)
+        z = (mean_y_new[0] - min_mean_y - 1) / (sigma_y_new[0] + 1e-9)
+        exp_imp = (mean_y_new[0] - min_mean_y - 1) * norm.cdf(z) + sigma_y_new[
+            0
+        ] * norm.pdf(z)
         return exp_imp
 
     def _get_ucb(self, x_new):
-
-        # Using estimate from Gaussian surrogate instead of actual function for
-        # a new trial data point to avoid cost
-
         mean_y_new, sigma_y_new = self.gauss_pr.predict(
             np.array([x_new]), return_std=True
         )
-        sigma_y_new = sigma_y_new.reshape(-1, 1)[0]
-
-        return mean_y_new + self.lambda_param * sigma_y_new
+        return mean_y_new[0] + self.lambda_param * sigma_y_new[0]
 
     def _get_lcb(self, x_new):
-
-        # Using estimate from Gaussian surrogate instead of actual function for
-        # a new trial data point to avoid cost
-
         mean_y_new, sigma_y_new = self.gauss_pr.predict(
             np.array([x_new]), return_std=True
         )
-        sigma_y_new = sigma_y_new.reshape(-1, 1)[0]
-
-        return mean_y_new - self.lambda_param * sigma_y_new
-
-    def _acquisition_function(self, x):
-        return self.acq_function(x)
+        return mean_y_new[0] - self.lambda_param * sigma_y_new[0]
 
     def _get_next_probable_point(self):
         min_ei = float(sys.maxsize)
         x_optimal = None
         # Trial with an array of random data points
         rands = np.random.uniform(
             np.array([dim.min_val for dim in self.dims]),
             np.array([dim.max_val for dim in self.dims]),
             (self.batch_size, self.get_n_dimensions()),
         )
         for x_start in rands:
             response = minimize(
-                fun=self._acquisition_function,
+                fun=self.acq_function,
                 x0=x_start,
                 bounds=[(dim.min_val, dim.max_val) for dim in self.dims],
                 method="L-BFGS-B",
             )
-            if response.fun[0] < min_ei:
-                min_ei = response.fun[0]
+            if response.fun < min_ei:
+                min_ei = response.fun
                 x_optimal = [
                     y.round(dim.rounding) for y, dim in zip(response.x, self.dims)
                 ]
         if x_optimal in self.x_init and self.iters < 5:
             if self.iters < 5:
                 self.iters += 1
                 x_optimal, min_ei = self._get_next_probable_point()
@@ -1368,17 +1362,18 @@
                     if y > self.dims[i].max_val:
                         x_optimal[i] = self.dims[i].max_val
                     elif y < self.dims[i].min_val:
                         x_optimal[i] = self.dims[i].min_val
 
         return x_optimal, min_ei
 
-    def _extend_prior_with_posterior_data(self, x, y):
+    def _extend_prior_with_posterior_data(self, x, y, yerr):
         self.x_init = np.append(self.x_init, np.array([x]), axis=0)
         self.y_init = np.append(self.y_init, np.array(y), axis=0)
+        self.yerr_init = np.append(self.yerr_init, np.array(yerr), axis=0)
 
     def get_first_point(self):
         y_min_ind = np.nanargmin(self.y_init)
         self.y_min = self.y_init[y_min_ind]
         self.optimal_x = self.x_init[y_min_ind]
         self.optimal_ei = None
         return self.optimal_x, self.optimal_ei
@@ -1406,17 +1401,20 @@
             else:
                 db_dict[name][parameter] = value_str
         self.current_iter += 1
         return db_dict
 
     def update(self, results):
         y_val = results["y_val"]
-        self._extend_prior_with_posterior_data(self.current_x, np.array([y_val]))
+        y_err = results["y_err"]
+        self._extend_prior_with_posterior_data(
+            self.current_x, np.array([y_val]), np.array([y_err])
+        )
 
-        if np.isnan(y_val):
+        if np.isnan(y_val) | np.isnan(y_err):
             pass
         else:
             if y_val < self.y_min:
                 self.y_min = y_val
                 self.optimal_x = self.current_x
                 self.optimal_ei = self.current_ei
                 self.optimal_results = results
@@ -1425,16 +1423,22 @@
             self.prev_x = self.current_x
         else:
             self.distances_.append(
                 np.linalg.norm(np.array(self.prev_x) - np.array(self.current_x))
             )
             self.prev_x = self.current_x
 
-        self.best_samples_ = self.best_samples_.append(
-            {"y": self.y_min, "ei": self.optimal_ei}, ignore_index=True
+        self.best_samples_ = pd.concat(
+            [
+                self.best_samples_,
+                pd.DataFrame(
+                    {"x": self.optimal_x, "y": self.y_min, "ei": self.optimal_ei}
+                ),
+            ],
+            ignore_index=True,
         )
 
     def get_best_vals(self):
         out_dict = {}
         for i, val in enumerate(self.optimal_x):
             name, parameter, min_val, max_val, rounding, unit = self.dims[i]
             value_str = f"{val}*{unit}"
@@ -1442,49 +1446,56 @@
                 out_dict[name] = {parameter: value_str}
             else:
                 out_dict[name][parameter] = value_str
         return out_dict
 
     def plot(self, init_samples=None):
         nan_idxs = np.isnan(self.y_init)
+        fail_idxs = np.isnan(self.yerr_init)
         self.gauss_pr.fit(self.x_init[~nan_idxs], np.array(self.y_init)[~nan_idxs])
         if (len(self.dims) != 2) and (len(self.dims) != 1):
             raise Exception("Acquisition Function Plotting not implemented for dim!=2")
         elif len(self.dims) == 1:
             points = np.arange(self.dims[0].min_val, self.dims[0].max_val, 0.1)
             ys = np.zeros_like(points)
+            ys_err = np.zeros_like(points)
             for i, point in enumerate(points):
-                ys[i] = self.gauss_pr.predict(
-                    np.array([point]).reshape(1, -1), return_std=False
+                ys[i], ys_err[i] = self.gauss_pr.predict(
+                    np.array([point]).reshape(1, -1), return_std=True
                 )
             fig = plt.figure()
-            plt.plot(points, ys)
-            plt.scatter(np.array(self.x_init), np.array(self.y_init))
+
+            plt.scatter(np.array(self.x_init), np.array(self.y_init), label="Samples")
+            plt.scatter(
+                np.array(self.x_init)[fail_idxs],
+                np.array(self.y_init)[fail_idxs],
+                color="green",
+                label="Failed samples",
+            )
+            plt.fill_between(points, ys - ys_err, ys + ys_err, alpha=0.1)
             if init_samples is not None:
                 init_ys = np.array(
                     [
                         np.where(init_sample == self.x_init)[0][0]
                         for init_sample in init_samples
                     ]
                 )
                 plt.scatter(
                     np.array(init_samples)[:, 0],
                     np.array(self.y_init)[init_ys],
                     color="red",
+                    label="Init Samples",
                 )
-            plt.scatter(
-                self.optimal_x[0],
-                self.y_min,
-                color="orange",
-            )
+            plt.scatter(self.optimal_x[0], self.y_min, color="orange", label="Optimal")
 
             plt.xlabel(
                 f"{self.dims[0].name}-{self.dims[0].parameter}({self.dims[0].unit})"
             )
             plt.ylabel(f"Kernel Value")
+            plt.legend()
         elif len(self.dims) == 2:
             x, y = np.mgrid[
                 self.dims[0].min_val : self.dims[0].max_val : 0.1,
                 self.dims[1].min_val : self.dims[1].max_val : 0.1,
             ]
             points = np.vstack((x.flatten(), y.flatten())).T
             out_grid = np.zeros(
@@ -1548,40 +1559,38 @@
         self.gauss_pr.fit(self.x_init[~nan_idxs], np.array(self.y_init)[~nan_idxs])
         if (len(self.dims) != 2) and (len(self.dims) != 1):
             raise Exception("Acquisition Function Plotting not implemented for dim!=2")
         elif len(self.dims) == 1:
             points = np.arange(self.dims[0].min_val, self.dims[0].max_val, 0.1)
             ys = np.zeros_like(points)
             for i, point in enumerate(points):
-                ys[i] = self._acquisition_function(np.array([point]).reshape(1, -1)[0])
+                ys[i] = self.acq_function(np.array([point]).reshape(1, -1)[0])
             fig = plt.figure()
             plt.plot(points, ys)
-            plt.scatter(np.array(self.x_init), np.array(self.y_init))
+            plt.scatter(np.array(self.x_init), np.array(self.y_init), label="Samples")
             if init_samples is not None:
                 init_ys = np.array(
                     [
                         np.where(init_sample == self.x_init)[0][0]
                         for init_sample in init_samples
                     ]
                 )
                 plt.scatter(
                     np.array(init_samples)[:, 0],
                     np.array(self.y_init)[init_ys],
                     color="red",
+                    label="Init Samples",
                 )
-            plt.scatter(
-                self.optimal_x[0],
-                self.y_min,
-                color="orange",
-            )
+            plt.scatter(self.optimal_x[0], self.y_min, color="orange", label="Optimal")
 
             plt.xlabel(
                 f"{self.dims[0].name}-{self.dims[0].parameter}({self.dims[0].unit})"
             )
             plt.ylabel(f"Acquisition Function Value")
+            plt.legend()
 
         elif len(self.dims) == 2:
             x, y = np.mgrid[
                 self.dims[0].min_val : self.dims[0].max_val : 0.1,
                 self.dims[1].min_val : self.dims[1].max_val : 0.1,
             ]
             points = np.vstack((x.flatten(), y.flatten())).T
@@ -1590,15 +1599,15 @@
                     int((self.dims[0].max_val - self.dims[0].min_val) * 10),
                     int((self.dims[1].max_val - self.dims[1].min_val) * 10),
                 )
             )
 
             j = 0
             for i, _ in np.ndenumerate(out_grid):
-                out_grid[i] = self._acquisition_function(points[j])
+                out_grid[i] = self.acq_function(points[j])
                 j += 1
 
             fig = plt.figure()
             plt.imshow(
                 out_grid,
                 norm=LogNorm(),
                 origin="lower",
@@ -1693,14 +1702,16 @@
 
     out_param_dict = {}
     out_results_list = []
     for optimiser in optimisers:
         param_dict = optimiser.get_best_vals()
         out_param_dict.update(param_dict)
         results_dict = optimiser.optimal_results
+        if np.isnan(results_dict["y_val"]):
+            log.error(f"Energy optimisation failed for {optimiser.dims[0][0]}")
         out_results_list.append(results_dict)
 
     return out_param_dict, out_results_list
 
 
 def get_ctc_grid(grids, ctc_param):
     """
@@ -1893,15 +1904,14 @@
         opt_dict = opt_dict[e_param]
 
         detector = save_path.split("/")[-1]
         save_path = os.path.join(save_path, f"{e_param}-{param}.pdf")
         pathlib.Path(os.path.dirname(save_path)).mkdir(parents=True, exist_ok=True)
 
         with PdfPages(save_path) as pdf:
-
             keys = list(opt_dict.keys())
             print(keys)
             x_dict = opt_dict[keys[1]]
             xvals = np.arange(x_dict["start"], x_dict["end"], x_dict["spacing"])
             xs = (
                 np.arange(0, len(xvals), 1),
                 np.arange(x_dict["start"], x_dict["end"], x_dict["spacing"]),
```

### Comparing `pygama-1.2.0/src/pygama/pargen/extract_tau.py` & `pygama-1.3.0/src/pygama/pargen/extract_tau.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,16 +37,24 @@
     wf_field: str = "waveform",
 ) -> lgdo.Table:
     sto = lh5.LH5Store()
     df = lh5.load_dfs(raw_file, ["daqenergy", "timestamp"], lh5_path)
 
     pulser_props = cts.find_pulser_properties(df, energy="daqenergy")
     if len(pulser_props) > 0:
-        out_df = cts.tag_pulsers(df, pulser_props, window=0.001)
-        ids = ~(out_df.isPulser == 1)
+        final_mask = None
+        for entry in pulser_props:
+            e_cut = (df.daqenergy.values < entry[0] + entry[1]) & (
+                df.daqenergy.values > entry[0] - entry[1]
+            )
+            if final_mask is None:
+                final_mask = e_cut
+            else:
+                final_mask = final_mask | e_cut
+        ids = ~(final_mask)
         log.debug(f"pulser found: {pulser_props}")
     else:
         log.debug("no_pulser")
         ids = np.ones(len(df.daqenergy.values), dtype=bool)
 
     cuts = np.where((df.daqenergy.values > threshold) & (ids))[0]
 
@@ -59,15 +67,14 @@
     tb_data = lh5.Table(col_dict={f"{wf_field}": waveforms, "baseline": baseline})
     return tb_data
 
 
 def get_decay_constant(
     slopes: np.array, wfs: lgdo.WaveformTable, display: int = 0
 ) -> dict:
-
     """
     Finds the decay constant from the modal value of the tail slope after cuts
     and saves it to the specified json.
 
     Parameters
     ----------
     slopes : array
@@ -81,27 +88,28 @@
     -------
     tau_dict : dict
     """
     tau_dict = {}
 
     pz = tau_dict.get("pz")
 
-    counts, bins, var = pgh.get_hist(slopes, bins=500000, range=(-0.01, 0))
+    counts, bins, var = pgh.get_hist(slopes, bins=100000, range=(-0.01, 0))
     bin_centres = pgh.get_bin_centers(bins)
     high_bin = bin_centres[np.argmax(counts)]
     try:
         pars, cov = pgf.gauss_mode_width_max(
             counts,
             bins,
-            mode_guess=high_bin,
             n_bins=10,
             cost_func="Least Squares",
             inflate_errors=False,
             gof_method="var",
         )
+        if np.abs(np.abs(pars[0] - high_bin) / high_bin) > 0.05:
+            raise ValueError
         high_bin = pars[0]
     except:
         pass
     tau = round(-1 / (high_bin), 1)
 
     sampling_rate = wfs["dt"].nda[0]
     units = wfs["dt"].attrs["units"]
@@ -109,47 +117,47 @@
 
     tau_dict["pz"] = {"tau": tau}
     if display > 0:
         out_plot_dict = {}
         plt.rcParams["figure.figsize"] = (10, 6)
         plt.rcParams["font.size"] = 8
         fig, ax = plt.subplots()
-        bins = 10000  # change if needed
+        bins = np.linspace(-0.01, 0, 100000)  # change if needed
         counts, bins, bars = ax.hist(slopes, bins=bins, histtype="step")
         plot_max = np.argmax(counts)
-        in_min = plot_max - 10
+        in_min = plot_max - 20
         if in_min < 0:
             in_min = 0
-        in_max = plot_max + 11
+        in_max = plot_max + 21
         if in_max >= len(bins):
             in_min = len(bins) - 1
         plt.xlabel("Slope")
         plt.ylabel("Counts")
         plt.yscale("log")
         axins = ax.inset_axes([0.5, 0.45, 0.47, 0.47])
         axins.hist(
             slopes[(slopes > bins[in_min]) & (slopes < bins[in_max])],
             bins=200,
             histtype="step",
         )
+        axins.axvline(high_bin, color="red")
         axins.set_xlim(bins[in_min], bins[in_max])
         labels = ax.get_xticklabels()
         ax.set_xticklabels(labels=labels, rotation=45)
         out_plot_dict["slope"] = fig
         if display > 1:
             plt.show()
         else:
             plt.close()
         return tau_dict, out_plot_dict
     else:
         return tau_dict
 
 
 def fom_dpz(tb_data, verbosity=0, rand_arg=None):
-
     std = tb_data["pz_std"].nda
     counts, start_bins, var = pgh.get_hist(std, dx=0.1, range=(0, 400))
     max_idx = np.argmax(counts)
     mu = start_bins[max_idx]
     try:
         pars, cov = pgf.gauss_mode_width_max(
             counts,
```

### Comparing `pygama-1.2.0/src/pygama/pargen/mse_psd.py` & `pygama-1.3.0/src/pygama/pargen/mse_psd.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/raw/__init__.py` & `pygama-1.3.0/src/pygama/raw/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,16 +3,21 @@
 :func:`.build_raw`. This is a one-to many function: one input DAQ file can
 generate one or more output raw files. Control of which data ends up in which
 files, and in which HDF5 groups inside of each file, is controlled via
 :mod:`.raw_buffer` (see below). If no raw buffers specification is specified,
 all decoded data should be written to a single output file, with all fields
 from each hardware decoder in their own output table.
 
-Currently we support the following hardware:
+Currently we support the following DAQ data formats:
 
-* FlashCam ADC (requires `fcutils <https://github.com/legend-exp/pyfcutils>`_)
-* FlashCam ADC read out with `ORCA <https://github.com/unc-enap/Orca>`_
+* `FlashCam <https://www.mizzi-computer.de/home>`_
+* `CoMPASS <https://www.caen.it/products/compass>`_
+* `ORCA <https://github.com/unc-enap/Orca>`_, reading out:
+
+  - FlashCam
+  - `Struck SIS3302 <https://www.struck.de/sis3302.htm>`_
+  - `Struck SIS3316 <https://www.struck.de/sis3316.html>`_
 """
 
 from pygama.raw.build_raw import build_raw
 
 __all__ = ["build_raw"]
```

### Comparing `pygama-1.2.0/src/pygama/raw/buffer_processor/buffer_processor.py` & `pygama-1.3.0/src/pygama/raw/buffer_processor/buffer_processor.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,94 +6,117 @@
 
 import numpy as np
 
 import pygama.lgdo as lgdo
 from pygama.dsp.errors import ProcessingChainError
 from pygama.dsp.processing_chain import build_processing_chain as bpc
 from pygama.lgdo import Array, ArrayOfEqualSizedArrays, Table
+from pygama.lgdo.compression import WaveformCodec
+from pygama.lgdo.compression.utils import str2wfcodec
 
 if TYPE_CHECKING:
     from pygama.raw.raw_buffer import RawBuffer
 
 log = logging.getLogger(__name__)
 
 
 def buffer_processor(rb: RawBuffer) -> Table:
-    r"""
-    Takes in a :class:`.RawBuffer`, performs any processes specified in the :class:`.RawBuffer`'s ``proc_spec``
-    attribute, and returns a :class:`pygama.lgdo.Table` with the processed buffer. This `tmp_table` shares columns with the :class:`.RawBuffer`'s lgdo,
-    so no data is copied. Currently implemented attributes:
-
-    - "window" (list): [in_name, start_index, stop_index, out_name]
-      Windows objects with a name specified by the first argument passed in the ``proc_spec``, the window start and stop indices are the next two
-      arguments, and then updates the rb.lgdo with a name specified by the last argument. If the object is an :func:`pygama.lgdo.WaveformTable`, then
-      the ``t0`` attribute is updated accordingly. Although it is possible to use the DSP config to perform windowing, this hard-coded version
-      avoids a conversion to float32.
-    - "dsp_config" (dict): {dsp_config}
-      Performs DSP given by the "dsp_config" key in the ``proc_spec``. See :mod:`pygama.dsp.processing_chain.build_processing_chain` for more information on DSP config dictionaries.
-      All fields in the output of the DSP are written to the rb.lgdo
-    - "drop" (list): ["waveform", "packet_ids"]
-      Drops any requested fields from the rb.lgdo
-    - "dtype_conv" (dict): {"presummed_waveform/values": "uint32", "t_sat_lo": "uint16"}
-      Updates the data types of any field with its requested datatype in ``proc_spec``
+    r"""Process raw data buffers.
+
+    Takes in a :class:`.RawBuffer`, performs any processes specified in the
+    :class:`.RawBuffer`'s ``proc_spec`` attribute (a dictionary), and returns a
+    :class:`.Table` with the processed buffer. This `tmp_table` shares columns
+    with the :class:`.RawBuffer`'s LGDO (`rb.lgdo`), so no data is copied.
+
+    Currently implemented ``proc_spec`` processors:
+
+    ``"window": ["waveform", start_index, stop_index, "out_name"]`` `(list)`
+      Windows objects with a name specified by the first argument, the window
+      start and stop indices are the next two arguments, and then updates the
+      `rb.lgdo` with a name specified by the last argument. If the object is an
+      :class:`.WaveformTable`, then the ``t0`` attribute is updated
+      accordingly.  Although it is possible to use the DSP config to perform
+      windowing, this hard-coded version avoids a conversion to ``float32``.
+
+    ``"dsp_config": { <dsp_config> }`` `(dict)`
+      Performs DSP given by the ``<dsp_config>`` specification. See
+      :func:`~.dsp.processing_chain.build_processing_chain` for more information
+      on DSP configuration dictionaries.  All fields in the output of the DSP
+      are written to the `rb.lgdo`.
+
+    ``"drop": ["waveform" [, ...]]`` `(list)`
+      Drops any requested fields from the `rb.lgdo`.
+
+    ``"dtype_conv": {"lgdo": "dtype" [, ...]}`` `(dict)`
+      Casts `lgdo` to the requested data type.
+
+    ``"compression": { "lgdo": "codec_name" [, ...]}`` `(dict)`
+      Updates the `compression` attribute of `lgdo` to `codec_name`. The
+      attribute sets the compression algorithm applied by
+      :func:`~.lgdo.lh5_store.LH5Store.read_object` before writing `lgdo` to
+      disk.
 
     Parameters
     ----------
     rb
-        A :class:`.RawBuffer` to be processed, must contain a ``proc_spec`` attribute
+        A :class:`.RawBuffer` to be processed, must contain a `proc_spec` attribute.
 
     Notes
     -----
-    The original "waveforms" column in the table is not written to file if request! All updates are done on the
-    `tmp_table`, which shares the fields with `rb.lgdo` and are done in place. The `tmp_table` is necessary so that
-    the `rb.lgdo` keeps arrays needed by the table in the buffer.
-    An example ``proc_spec`` in an :mod:`pygama.raw.build_raw` ``out_spec`` is below
-
-    .. code-block:: json
+    The original ``waveforms`` column in the table is not written to file if
+    request! All updates are done on the `tmp_table`, which shares the fields
+    with `rb.lgdo` and are done in place. The `tmp_table` is necessary so that
+    the `rb.lgdo` keeps arrays needed by the table in the buffer.  An example
+    `proc_spec` in an :func:`~.raw.build_raw.build_raw` `out_spec` is below. ::
 
         {
-           "FCEventDecoder" : {
-           "g{key:0>3d}" : {
-              "key_list" : [ [24,64] ],
+          "FCEventDecoder" : {
+            "g{key:0>3d}" : {
+              "key_list" : [[24, 64]],
               "out_stream" : "$DATADIR/{file_key}_geds.lh5:/geds",
               "proc_spec": {
-                "window":
-                  ["waveform", 100, -100, "windowed_waveform"],
+                "window": ["waveform", 100, -100, "windowed_waveform"],
                 "dsp_config": {
-                  "outputs": [ "presummed_waveform", "t_sat_lo", "t_sat_hi" ],
-                    "processors": {
-                      "presummed_waveform": {
-                        "function": "presum",
-                        "module": "pygama.dsp.processors",
-                        "args": ["waveform", "presummed_waveform(shape=len(waveform)//16, period=waveform.period*16, offset=waveform.offset, 'f')"],
-                        "unit": "ADC"
-                        },
+                  "outputs": ["presummed_waveform", "t_sat_lo", "t_sat_hi"],
+                  "processors": {
+                    "presummed_waveform": {
+                      "function": "presum",
+                      "module": "pygama.dsp.processors",
+                      "args": [
+                        "waveform",
+                        "presummed_waveform(shape=len(waveform)//16, period=waveform.period*16, offset=waveform.offset, 'f')"
+                      ],
+                      "unit": "ADC"
+                    },
                     "t_sat_lo, t_sat_hi": {
-                        "function": "saturation",
-                        "module": "pygama.dsp.processors",
-                        "args": ["waveform", 16, "t_sat_lo", "t_sat_hi"],
-                        "unit": "ADC"
-                        }
+                      "function": "saturation",
+                      "module": "pygama.dsp.processors",
+                      "args": ["waveform", 16, "t_sat_lo", "t_sat_hi"],
+                      "unit": "ADC"
                     }
+                  }
                 },
-                "drop":
-                    ["waveform", "packet_ids"],
+                "drop": ["waveform", "packet_ids"],
                 "dtype_conv": {
-                    "presummed_waveform/values": "uint32",
-                    "t_sat_lo": "uint16",
-                    "t_sat_hi": "uint16",
+                  "presummed_waveform/values": "uint32",
+                  "t_sat_lo": "uint16",
+                  "t_sat_hi": "uint16",
+                ,}
+                "compression": {
+                  "windowed_waveform/values": RadwareSigcompress(codec_shift=-32768),
+                  "presummed_waveform/values": ULEB128ZigZagDiff(),
                 }
               }
-           },
-           "spms" : {
-             "key_list" : [ [6,23] ],
-             "out_stream" : "$DATADIR/{file_key}_spms.lh5:/spms"
-           }
+            },
+            "spms" : {
+              "key_list" : [ [6,23] ],
+              "out_stream" : "$DATADIR/{file_key}_spms.lh5:/spms"
+            }
+          }
         }
-
     """
     # Check that there is a valid object to process
     if isinstance(rb.lgdo, lgdo.Table) or isinstance(rb.lgdo, lgdo.Struct):
         # Create the temporary table that will be written to file
         rb_table_size = rb.lgdo.size
         tmp_table = Table(size=rb_table_size)
         tmp_table.join(other_table=rb.lgdo)
@@ -117,40 +140,54 @@
     if "dtype_conv" in rb.proc_spec.keys():
         process_dtype_conv(rb, tmp_table)
 
     # Drop any requested columns from the table
     if "drop" in rb.proc_spec.keys():
         process_drop(rb, tmp_table)
 
+    # at last, assign compression attributes
+    if "compression" in rb.proc_spec.keys():
+        for name, codec in rb.proc_spec["compression"].items():
+            ptr = tmp_table
+            for word in name.split("/"):
+                ptr = ptr[word]
+
+            ptr.attrs["compression"] = (
+                codec if isinstance(codec, WaveformCodec) else str2wfcodec(codec)
+            )
+
     return tmp_table
 
 
 def process_window(rb: RawBuffer, tmp_table: Table) -> None:
-    r"""
-    Windows arrays of equal sized arrays according to specifications
-    given in the rb.proc_spec "window" key.
-
-    First checks if the rb.lgdo is a table or not. If it's not a table,
-    then we only process it if its rb.out_name is the same as the window_in_name.
-
-    If rb.lgdo is a table, special processing is done if the window_in_name field
-    is an lgdo.WaveformTable in order to update the t0s. Otherwise, windowing of the field
-    is performed without updating any of the other attributes.
+    r"""Window :class:`.ArrayOfEqualSizedArrays`.
+
+    Windows arrays of equal sized arrays according to specifications given in
+    the `rb.proc_spec` ``window`` key.
+
+    First checks if the `rb.lgdo` is a :class:`.Table` or not. If it's not a
+    table, then we only process it if its `rb.out_name` is the same as the
+    window ``in_name``.
+
+    If `rb.lgdo` is a table, special processing is done if the window
+    ``in_name`` field is an :class:`.WaveformTable` in order to update the
+    ``t0``\ s.  Otherwise, windowing of the field is performed without updating
+    any of the other attributes.
 
     Parameters
     ----------
     rb
-        A :class:`.RawBuffer` to be processed
+        a :class:`.RawBuffer` to be processed.
     tmp_table
-        A :class:`pygama.lgdo.Table` that shares columns with the `rb.lgdo`
+        a :class:`.Table` that shares columns with the `rb.lgdo`.
 
     Notes
     -----
-    This windowing hard-coded; it is done without calling :mod:`pygama.dsp.build_dsp` to avoid
-    a conversion to float32.
+    This windowing hard-coded; it is done without calling :mod:`.dsp.build_dsp`
+    to avoid a conversion to ``float32``.
 
     """
     # Read the window parameters from the proc_spec
     window_in_name = rb.proc_spec["window"][0]
     window_start_idx = int(rb.proc_spec["window"][1])
     window_end_idx = int(rb.proc_spec["window"][2])
     window_out_name = rb.proc_spec["window"][3]
@@ -208,57 +245,62 @@
         log.info(f"{window_in_name} not a valid key for this RawBuffer")
         return None
 
 
 def window_array_of_arrays(
     array_of_arrays: ArrayOfEqualSizedArrays, window_start_idx: int, window_end_idx: int
 ) -> ArrayOfEqualSizedArrays:
-    r"""
-    Given an array of equal sized arrays, for each array it returns the view [window_start_idx:window_end_idx]
+    """Given an array of equal sized arrays, for each array it returns the view
+    ``[window_start_idx:window_end_idx]``.
     """
     if isinstance(array_of_arrays, lgdo.ArrayOfEqualSizedArrays):
         return array_of_arrays.nda[:, window_start_idx:window_end_idx]
     else:
         raise TypeError(
             f"Do not know how to window an LGDO of type {type(array_of_arrays)}"
         )
 
 
 def process_windowed_t0(t0s: Array, dts: Array, start_index: int) -> Array:
-    """
-    In order for the processed data to work well with :mod:`pygama.dsp.build_dsp`, we need
+    """In order for the processed data to work well with :mod:`.dsp.build_dsp`, we need
     to keep ``t0`` in its original units.
 
     So we transform ``start_index`` to the units of ``t0`` and add it to every
     ``t0`` value.
     """
     # don't want to modify the original lgdo_table t0s
+    # deepcopy also preserves attributes
     copy_t0s = copy.deepcopy(t0s)
 
     # perform t0+start_index*dt to rewrite the new t0 in terms of sample
     start_index *= dts.nda
     copy_t0s.nda += start_index
     return copy_t0s
 
 
 def process_dsp(rb: RawBuffer, tmp_table: Table) -> None:
-    r"""
-    Run a provided DSP config from rb.proc_spec using build_processing_chain, and add specified outputs to the
-    rb.lgdo.
+    r"""Run a DSP processing chain.
+
+    Run a provided DSP config from `rb.proc_spec` using
+    :func:`.dsp.build_processing_chain`, and add specified outputs to the
+    `rb.lgdo`.
 
     Parameters
     ----------
     rb
-        A :class:`.RawBuffer` that contains a `proc_spec` and an `lgdo` attribute
+        a :class:`.RawBuffer` that contains a `proc_spec` and an `lgdo`
+        attribute.
     tmp_table
-        A :class:`pygama.lgdo.Table` that is temporarily created to be written to the raw file
+        a :class:`pygama.lgdo.Table` that is temporarily created to be written
+        to the raw file.
 
     Notes
     -----
-    rb.lgdo is assumed to be an lgdo.Table so that multiple DSP processor outputs can be written to it
+    `rb.lgdo` is assumed to be an :class`.Table` so that multiple DSP processor
+    outputs can be written to it.
     """
     # Load the dsp_dict
     dsp_dict = rb.proc_spec["dsp_config"]
 
     # Try building the processing chain
     try:
         # execute the processing chain
@@ -267,31 +309,34 @@
     # Allow for exceptions, in the case of "*" key expansion in the build_raw out_spec
     except ProcessingChainError:
         log.info("DSP could not be performed")
         return None
 
     proc_chain.execute()
 
-    # For every processor in dsp_dict for this group, create a new entry in the lgdo table with that processor's name
-    # If the processor returns a waveform, create a new waveform table and add it to the original lgdo table
+    # For every processor in dsp_dict for this group, create a new entry in the
+    # lgdo table with that processor's name.  If the processor returns a
+    # waveform, create a new waveform table and add it to the original lgdo
+    # table
     for proc in dsp_out.keys():
         # # Check what DSP routine the processors output is from, and manipulate accordingly
         tmp_table.add_field(proc, dsp_out[proc], use_obj_size=True)
 
     return None
 
 
 def process_dtype_conv(rb: RawBuffer, tmp_table: Table) -> None:
-    """
-    Change the types of fields in an rb.lgdo according to the values specified in the ``proc_spec``'s ``dtype_conv`` list.
-    It operates in place on `tmp_table`.
+    """Change the types of fields in an `rb.lgdo` according to the values
+    specified in the ``proc_spec``'s ``dtype_conv`` list.  It operates in place
+    on `tmp_table`.
 
     Notes
     -----
-    This assumes that name provided points to an object in the rb.lgdo that has an `nda` attribute
+    This assumes that name provided points to an object in the `rb.lgdo` that has
+    an `nda` attribute.
     """
     type_list = rb.proc_spec["dtype_conv"]
     for return_name in type_list.keys():
         # Take care of nested tables with a for loop
         path = return_name.split("/")
         return_value = tmp_table
         for key in path:
@@ -308,13 +353,14 @@
         else:
             raise TypeError(f"Cannot recast an object of type {type(return_value)}")
 
     return None
 
 
 def process_drop(rb: RawBuffer, tmp_table: Table) -> None:
+    """Drops any requested fields from the `rb.lgdo`."""
     for drop_keys in rb.proc_spec["drop"]:
         try:
             tmp_table.remove_column(drop_keys, delete=False)
         except KeyError:
             log.info(f"Cannot remove field {drop_keys} from rb.lgdo")
             return None
```

### Comparing `pygama-1.2.0/src/pygama/raw/buffer_processor/lh5_buffer_processor.py` & `pygama-1.3.0/src/pygama/raw/buffer_processor/lh5_buffer_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,41 +13,48 @@
 
 log = logging.getLogger(__name__)
 
 
 def lh5_buffer_processor(
     lh5_raw_file_in: str,
     overwrite: bool = False,
-    out_spec: list[str | dict] = None,
+    out_spec: dict = None,
     proc_file_name: str = None,
 ) -> None:
-    """
-    This function performs data processing on an existing raw-level :func:`lh5` file according to the :func:`out_spec` passed in the arguments.
-    It iterates through any valid table in an :func:`lh5` file and checks that either the :func:`group_name` or the :func:`out_name` of this table
-    are found in the :func:`out_spec`. If there is a valid :func:`proc_spec` entry in the :func:`out_spec`, then the table is stored in a :func:`RawBuffer`
-    and the :func:`RawBuffer` is passed to the buffer processor. If no :func:`proc_spec` is found, the table is written to the file without any modifications.
+    r"""Process raw buffers from an LH5 file.
+
+    This function performs data processing on an existing raw-level LH5 file
+    according to `out_spec`.  It iterates through any valid table in the
+    `lh5_raw_file_in` file and checks that either the `group_name` or the
+    `out_name` of this table are found in the `out_spec`. If there is a valid
+    `proc_spec` entry in the `out_spec`, then the table is stored in a
+    :class:`RawBuffer` and the :func:`RawBuffer` is passed to the buffer
+    processor. If no `proc_spec` is found, the table is written to the file
+    without any modifications.
 
 
     Parameters
     ----------
     lh5_raw_file_in
-        The path of a file created from :meth:`pygama.raw.build_raw`
+        the path of a file created by :func:`~.raw.build_raw.build_raw`.
     overwrite
-        sets whether to overwrite the output file(s) if it (they) already exist.
+        sets whether to overwrite the output file(s) if it (they) already
+        exist.
     out_spec
-        An out_spec for :mod:`pygama.raw.build_raw` containing a `proc_spec` dict used for data processing.
-        See :mod:`pygama.raw.buffer_processor.buffer_processor` for an example of such an out_spec.
+        an `out_spec` for :func:`~.raw.build_raw.build_raw` also containing a
+        dictionary named `proc_spec` used for data processing.  See
+        :func:`.buffer_processor` for an example of such an `out_spec`.
     proc_file_name
-        The path to the processed output file created
-            - if None, uses ``{lh5_raw_file_in}_proc.lh5`` as the output filename.
+        The path to the processed output file created. If ``None``, uses
+        ``{lh5_raw_file_in}_proc.lh5`` as the output filename.
 
     Notes
     -----
-    This function assumes that all raw file data are stored in at most two :meth:`h5py.Group`s, as in the following
-    :func:`ch000/raw` or :func:`raw/geds`
+    This function assumes that all raw file data are stored in at most two
+    :class:`h5py.Group`\ s, as in e.g. ``ch000/raw`` or ``raw/geds``
     """
 
     # Initialize the input raw file
     raw_store = LH5Store()
     lh5_file = raw_store.gimme_file(lh5_raw_file_in, "r")
     if lh5_file is None:
         raise ValueError(f"input file not found: {lh5_raw_file_in}")
@@ -163,15 +170,14 @@
                 and (
                     out_name
                     == out_spec[decoder_name][list(out_spec[decoder_name].keys())[0]][
                         "out_name"
                     ]
                 )
             ):
-
                 # if out_name is a key, check that the out_name matches and use that
                 if (
                     "proc_spec"
                     in out_spec[decoder_name][
                         list(out_spec[decoder_name].keys())[0]
                     ].keys()
                 ):
```

### Comparing `pygama-1.2.0/src/pygama/raw/build_raw.py` & `pygama-1.3.0/src/pygama/raw/build_raw.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,34 +2,39 @@
 
 import glob
 import json
 import logging
 import os
 import time
 
+import hdf5plugin
 import numpy as np
 from tqdm import tqdm
 
 from pygama import lgdo
+from pygama.lgdo.lh5_store import DEFAULT_HDF5_COMPRESSION
 from pygama.math.utils import sizeof_fmt
 
+from .compass.compass_streamer import CompassStreamer
 from .fc.fc_streamer import FCStreamer
 from .orca.orca_streamer import OrcaStreamer
 from .raw_buffer import RawBufferLibrary, write_to_lh5_and_clear
 
 log = logging.getLogger(__name__)
 
 
 def build_raw(
     in_stream: int,
     in_stream_type: str = None,
     out_spec: str | dict | RawBufferLibrary = None,
     buffer_size: int = 8192,
     n_max: int = np.inf,
     overwrite: bool = False,
+    compass_config_file: str = None,
+    hdf5_compression: str | dict | hdf5plugin.filters.Filter = DEFAULT_HDF5_COMPRESSION,
     **kwargs,
 ) -> None:
     """Convert data into LEGEND HDF5 raw-tier format.
 
     Takes an input stream of a given type and writes to output file(s)
     according to the user's a specification.
 
@@ -61,45 +66,60 @@
 
     n_max
         maximum number of rows of data to process from the input file.
 
     overwrite
         sets whether to overwrite the output file(s) if it (they) already exist.
 
+    compass_config_file
+        specification of config file, used for decoding CoMPASS files
+
+        - if None, CompassDecoder will sacrifice the first packet to determine
+          waveform length
+        - if a str ending in ``.json``, interpreted as a filename containing
+          json-shorthand for the output specification (see
+          :mod:`.compass.compass_event_decoder`).
+
+    hdf5_compression
+        forwarded to :meth:`~.lgdo.lh5_store.LH5Store.write_object`.
+
     **kwargs
-        sent to :class:`.RawBufferLibrary` generation as `kw_dict`.
+        sent to :class:`.RawBufferLibrary` generation as `kw_dict` argument.
     """
-
     # convert any environment variables in in_stream so that we can check for readability
     in_stream = os.path.expandvars(in_stream)
     # later: fix if in_stream is not a file
     # (e.g. a socket, which exists if open and has size = np.inf)
     if not os.path.exists(in_stream):
         raise FileNotFoundError(f"file {in_stream} not found")
 
     in_stream_size = os.stat(in_stream).st_size
 
     # try to guess the input stream type if it's not provided
     if in_stream_type is None:
         i_ext = in_stream.split("/")[-1].rfind(".")
-        if i_ext == -1:
-            if OrcaStreamer.is_orca_stream(in_stream):
-                in_stream_type = "ORCA"
-            else:
-                raise RuntimeError("unknown file type. Specify in_stream_type")
-        else:
+        if compass_config_file is not None:  # skip right away if compass
+            in_stream_type = "Compass"
+        elif i_ext != -1:
             ext = in_stream.split("/")[-1][i_ext + 1 :]
             if ext == "fcio":
                 in_stream_type = "FlashCam"
-            elif OrcaStreamer.is_orca_stream(in_stream):
+            elif ext == "orca":
                 in_stream_type = "ORCA"
+            elif ext == "bin" or ext == "BIN":
+                in_stream_type = "Compass"
             else:
                 raise RuntimeError(
                     f"unknown file extension {ext}. Specify in_stream_type"
                 )
+        else:
+            if OrcaStreamer.is_orca_stream(in_stream):  # orca default is no ext
+                in_stream_type = "ORCA"
+            else:
+                raise RuntimeError("unknown file type. Specify in_stream_type")
 
     # process out_spec and setup rb_lib if specified
     rb_lib = None
     if isinstance(out_spec, str) and out_spec.endswith(".json"):
         with open(out_spec) as json_file:
             out_spec = json.load(json_file)
     if isinstance(out_spec, dict):
@@ -132,15 +152,15 @@
     else:
         log.info("output:")
         for out_file in out_files:
             log.info(f" -> {out_file}")
     log.info(f"buffer size: {buffer_size}")
     if n_max < np.inf:
         log.info(f"maximum number of events: {n_max}")
-    if log.getEffectiveLevel() >= logging.INFO:
+    if log.getEffectiveLevel() <= logging.INFO:
         if n_max < np.inf:
             progress_bar = tqdm(desc="Decoding", total=n_max, delay=2, unit=" rows")
         else:
             progress_bar = tqdm(
                 desc="Decoding",
                 total=in_stream_size,
                 delay=2,
@@ -153,37 +173,37 @@
 
     # select the appropriate streamer for in_stream
     streamer = None
     if in_stream_type == "ORCA":
         streamer = OrcaStreamer()
     elif in_stream_type == "FlashCam":
         streamer = FCStreamer()
+    elif in_stream_type == "Compass":
+        streamer = CompassStreamer(compass_config_file)
     elif in_stream_type == "LlamaDaq":
         raise NotImplementedError("LlamaDaq streaming not yet implemented")
-    elif in_stream_type == "Compass":
-        raise NotImplementedError("Compass streaming not yet implemented")
     elif in_stream_type == "MGDO":
         raise NotImplementedError("MGDO streaming not yet implemented")
     else:
         raise NotImplementedError("unknown input stream type {in_stream_type}")
 
     # initialize the stream and read header. Also initializes rb_lib
-    if log.getEffectiveLevel() >= logging.INFO:
+    if log.getEffectiveLevel() <= logging.INFO:
         progress_bar.update(0)
 
     out_stream = out_spec if isinstance(out_spec, str) else ""
     header_data = streamer.open_stream(
         in_stream,
         rb_lib=rb_lib,
         buffer_size=buffer_size,
         chunk_mode="full_only",
         out_stream=out_stream,
     )
     rb_lib = streamer.rb_lib
-    if log.getEffectiveLevel() >= logging.INFO and n_max == np.inf:
+    if log.getEffectiveLevel() <= logging.INFO and n_max == np.inf:
         progress_bar.update(streamer.n_bytes_read)
 
     # rb_lib should now be fully initialized. Check if files need to be
     # overwritten or if we need to stop to avoid overwriting
     out_files = rb_lib.get_list_of("out_stream")
     for out_file in out_files:
         colpos = out_file.find(":")
@@ -201,39 +221,48 @@
                 f"file {out_file_glob[0]} exists. Use option overwrite to proceed."
             )
 
         os.remove(out_file_glob[0])
 
     # Write header data
     lh5_store = lgdo.LH5Store(keep_open=True)
-    write_to_lh5_and_clear(header_data, lh5_store)
+    write_to_lh5_and_clear(header_data, lh5_store, hdf5_compression=hdf5_compression)
 
     # Now loop through the data
     n_bytes_last = streamer.n_bytes_read
     while True:
         chunk_list = streamer.read_chunk()
-        if log.getEffectiveLevel() >= logging.INFO and n_max == np.inf:
+
+        if log.getEffectiveLevel() <= logging.INFO and n_max == np.inf:
             progress_bar.update(streamer.n_bytes_read - n_bytes_last)
             n_bytes_last = streamer.n_bytes_read
+
         if len(chunk_list) == 0:
+            log.debug("Reached EOF, exiting...")
             break
+
         n_read = 0
         for rb in chunk_list:
             if rb.loc > n_max:
                 rb.loc = n_max
             n_max -= rb.loc
             n_read += rb.loc
-        if log.getEffectiveLevel() >= logging.INFO and n_max < np.inf:
+
+        if log.getEffectiveLevel() <= logging.INFO and n_max < np.inf:
             progress_bar.update(n_read)
-        write_to_lh5_and_clear(chunk_list, lh5_store)
+
+        write_to_lh5_and_clear(chunk_list, lh5_store, hdf5_compression=hdf5_compression)
+
         if n_max <= 0:
+            log.info(f"Wrote {n_max} rows, exiting...")
             break
 
     streamer.close_stream()
-    progress_bar.close()
+    if log.getEffectiveLevel() <= logging.INFO:
+        progress_bar.close()
 
     out_files = rb_lib.get_list_of("out_stream")
     if len(out_files) == 1:
         out_file = out_files[0].split(":", 1)[0]
         if os.path.exists(out_file):
             file_size = os.stat(out_file).st_size
             log.info(f"output file: {out_file} ({sizeof_fmt(file_size)})")
```

### Comparing `pygama-1.2.0/src/pygama/raw/data_decoder.py` & `pygama-1.3.0/src/pygama/raw/data_decoder.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,34 +14,66 @@
 LGDO = Union[lgdo.Scalar, lgdo.Struct, lgdo.Array, lgdo.VectorOfVectors]
 
 
 class DataDecoder:
     r"""Decodes packets from a data stream.
 
     Most decoders will repeatedly decode the same set of values from each
-    packet.  The values that get decoded need to be described by a dict called
-    `decoded_values` that helps determine how to set up the buffers and write
-    them to file. :class:`~.lgdo.table.Table`\ s are made whose columns
-    correspond to the elements of `decoded_values`, and packet data gets pushed
-    to the end of the table one row at a time. See
+    packet.  The values that get decoded need to be described by a dict stored
+    in `self.decoded_values` that helps determine how to set up the buffers and
+    write them to file as :class:`~.lgdo.LGDO`\ s. :class:`~.lgdo.table.Table`\ s
+    are made whose columns correspond to the elements of `decoded_values`, and
+    packet data gets pushed to the end of the table one row at a time.
+
+    Any key-value entry in a configuration dictionary attached to an element
+    of `decoded_values` is typically interpreted as an attribute to be attached
+    to the corresponding LGDO. This feature can be for example exploited to
+    specify the data compression algorithm used by
+    :meth:`~.lgdo.lh5_store.LH5Store.write_object` to write LGDOs to disk.
+
+    For example ::
+
+      from pygama.lgdo.compression import RadwareSigcompress
+
+      FCEventDecoder.decoded_values = {
+        "packet_id": {"dtype": "uint32", "compression": "gzip"},
+        # ...
+        "waveform": {
+          "dtype": "uint16",
+          "datatype": "waveform",
+          # ...
+          "compression": {"values": RadwareSigcompress(codec_shift=-32768)},
+        }
+      }
+
+    LGDOs corresponding to ``packet_id`` and ``waveform`` will have their
+    `compression` attribute set as ``"gzip"`` and
+    ``RadwareSigcompress(codec_shift=-32768)``, respectively. Before being
+    written to disk, they will compressed with the HDF5 built-in Gzip filter
+    and with the :class:`~.lgdo.compression.radware.RadwareSigcompress`
+    waveform compressor.
+
+    Examples
+    --------
+    See `decoded_values` attributes of
     :class:`~.fc.fc_event_decoder.FCEventDecoder` or
-    :class:`~.orca.orca_digitizers.ORCAStruck3302` for an example.
+    :class:`~.orca.orca_digitizers.ORSIS3316WaveformDecoder`.
 
     Some decoders (like for file headers) do not need to push to a table, so they
     do not need `decoded_values`. Such classes should still derive from
     :class:`DataDecoder` and define how data gets formatted into LGDO's.
 
     Subclasses should define a method for decoding data to a buffer like
-    ``decode_packet(packet, raw_buffer_list, packet_id)``.
-    This function should return the number of bytes read.
+    ``decode_packet(packet, raw_buffer_list, packet_id)``.  This function
+    should return the number of bytes read.
 
-    Garbage collection writes binary data as an array of :obj:`~numpy.uint32`\ s to a
-    variable-length array in the output file. If a problematic packet is found,
-    call :meth:`.put_in_garbage`. User should set up an enum or bitbank of garbage
-    codes to be stored along with the garbage packets.
+    Garbage collection writes binary data as an array of :obj:`~numpy.uint32`\ s
+    to a variable-length array in the output file. If a problematic packet is
+    found, call :meth:`.put_in_garbage`. User should set up an enum or bitbank
+    of garbage codes to be stored along with the garbage packets.
     """
 
     def __init__(
         self, garbage_length: int = 256, packet_size_guess: int = 1024
     ) -> None:
         self.garbage_table = lgdo.Table(garbage_length)
         shape_guess = (garbage_length, packet_size_guess)
@@ -106,28 +138,29 @@
         -------
         data_obj
             the newly allocated LGDO.
         """
 
         if not hasattr(self, "decoded_values"):
             raise AttributeError(
-                type(self).__name__, ":no decoded_values available for setting up table"
+                type(self).__name__
+                + ": no decoded_values available for setting up table"
             )
 
         data_obj = lgdo.Table(size=size)
         dec_vals = self.get_decoded_values(key)
         for field, fld_attrs in dec_vals.items():
             # make a copy of fld_attrs: pop off the ones we use, then keep any
             # remaining user-set attrs and store into the lgdo
             attrs = fld_attrs.copy()
 
             # get the dtype
             if "dtype" not in attrs:
                 raise AttributeError(
-                    type(self).__name__, ": must specify dtype for", field
+                    type(self).__name__ + ": must specify dtype for", field
                 )
 
             dtype = attrs.pop("dtype")
 
             # no datatype: just a "normal" array
             if "datatype" not in attrs:
                 # allow to override "kind" for the dtype for lgdo
@@ -143,24 +176,39 @@
 
             # waveforms: must have attributes t0_units, dt, dt_units, wf_len
             if datatype == "waveform":
                 t0_units = attrs.pop("t0_units")
                 dt = attrs.pop("dt")
                 dt_units = attrs.pop("dt_units")
                 wf_len = attrs.pop("wf_len")
+                compression = attrs.pop("compression", None)
+
                 wf_table = lgdo.WaveformTable(
                     size=size,
                     t0=0,
                     t0_units=t0_units,
                     dt=dt,
                     dt_units=dt_units,
                     wf_len=wf_len,
                     dtype=dtype,
                     attrs=attrs,
                 )
+                if compression is not None:
+                    if not isinstance(compression, dict):
+                        raise RuntimeError(
+                            "waveform/compression attribute must be a dictionary"
+                        )
+
+                    if "values" in compression:
+                        wf_table.values.attrs["compression"] = compression["values"]
+                    if "t0" in compression:
+                        wf_table.t0.attrs["compression"] = compression["t0"]
+                    if "dt" in compression:
+                        wf_table.dt.attrs["compression"] = compression["dt"]
+
                 data_obj.add_field(field, wf_table)
                 continue
 
             # Parse datatype for remaining lgdos
             datatype, shape, elements = lgdo.lgdo_utils.parse_datatype(datatype)
 
             # ArrayOfEqualSizedArrays
@@ -195,15 +243,15 @@
             )
 
         return data_obj
 
     def put_in_garbage(self, packet: int, packet_id: int, code: int) -> None:
         i_row = self.garbage_table.loc
         p8 = np.frombuffer(packet, dtype="uint8")
-        self.garbage_table["packets"].set_vector(i_row, p8)
+        self.garbage_table["packets"]._set_vector_unsafe(i_row, p8)
         self.garbage_table["packet_id"].nda[i_row] = packet_id
         self.garbage_table["garbage_codes"].nda[i_row] = code
         self.garbage_table.push_row()
 
     def write_out_garbage(
         self, filename: str, group: str = "/", lh5_store: LH5Store = None
     ) -> None:
```

### Comparing `pygama-1.2.0/src/pygama/raw/data_streamer.py` & `pygama-1.3.0/src/pygama/raw/data_streamer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Base classes for streaming data.
 """
 from __future__ import annotations
 
+import fnmatch
 import logging
 from abc import ABC, abstractmethod
 
 from .raw_buffer import RawBuffer, RawBufferLibrary, RawBufferList
 
 log = logging.getLogger(__name__)
 
@@ -124,31 +125,60 @@
                     rb_lib[dec_name].append(rb)
 
             # dec_name is in rb_lib: store the name, and initialize its buffer lgdos
             dec_names.append(dec_name)
 
             # set up wildcard key buffers
             for rb in rb_lib[dec_name]:
-                if len(rb.key_list) == 1 and rb.key_list[0] == "*":
-                    key_lists = decoder.get_key_lists()
-                    if len(key_lists) != 1:
+                if (
+                    len(rb.key_list) == 1
+                    and isinstance(rb.key_list[0], str)
+                    and "*" in rb.key_list[0]
+                ):
+                    matched_key_lists = []
+                    for key_list in decoder.get_key_lists():
+                        # special case: decoders without keys
+                        if rb.key_list[0] == "*" and key_list == [None]:
+                            matched_key_lists.append(key_list)
+                            continue
+                        key_type = type(key_list[0])
+                        for ik in range(len(key_list)):
+                            key_list[ik] = str(key_list[ik])
+                        matched_keys = fnmatch.filter(key_list, rb.key_list[0])
+                        if len(matched_keys) > 1:
+                            for ik in range(len(matched_keys)):
+                                matched_keys[ik] = key_type(key_list[ik])
+                            matched_key_lists.append(matched_keys)
+                    if len(matched_key_lists) == 0:
                         log.warning(
-                            f"{dec_name} has {len(key_lists)} lists of keys, need a rb for each. Only the first will be decoded."
+                            f"no matched keys for key_list {rb.key_list[0]} in {dec_name}.{rb.out_name}"
                         )
-                    rb.key_list = key_lists[0]
+                        continue
+                    rb.key_list = sum(matched_key_lists, [])
             keyed_name_rbs = []
             ii = 0
             while ii < len(rb_lib[dec_name]):
                 if "{key" in rb_lib[dec_name][ii].out_name:
                     keyed_name_rbs.append(rb_lib[dec_name].pop(ii))
                 else:
                     ii += 1
             for rb in keyed_name_rbs:
                 for key in rb.key_list:
-                    expanded_name = rb.out_name.format(key=key)
+                    # keys can be strs or ints; try as-is, but can get a
+                    # ValueError e.g. when using a wildcard with int keys. In
+                    # that case, switch to the other type and try again
+                    try:
+                        expanded_name = rb.out_name.format(key=key)
+                    except ValueError:
+                        if isinstance(key, str):
+                            key = int(key)
+                        else:
+                            key = str(key)
+                        expanded_name = rb.out_name.format(key=key)
+
                     new_rb = RawBuffer(
                         key_list=[key],
                         out_stream=rb.out_stream,
                         out_name=expanded_name,
                         proc_spec=rb.proc_spec,
                     )
                     rb_lib[dec_name].append(new_rb)
@@ -173,16 +203,15 @@
         .. note::
             Needs to be overloaded.
         """
         pass
 
     @abstractmethod
     def read_packet(self) -> bool:
-        """Reads a single packet's worth of data in to the
-        :class:`.RawBufferLibrary`.
+        """Reads a single packet's worth of data in to the :class:`.RawBufferLibrary`.
 
         Needs to be overloaded. Gets called by :meth:`.read_chunk` Needs to
         update :attr:`self.any_full` if any buffers would possibly over-fill on
         the next read. Needs to update :attr:`self.n_bytes_read` too.
 
         Returns
         -------
@@ -268,14 +297,16 @@
         for rb_list in self.rb_lib.values():
             for rb in rb_list:
                 if not only_full:  # any_full or read_one_packet
                     if rb.loc > 0:
                         list_of_rbs.append(rb)
                 elif rb.is_full():
                     list_of_rbs.append(rb)
+        if not still_has_data:
+            log.debug(f"decoding complete. flushing {len(list_of_rbs)} buffers")
         return list_of_rbs
 
     @abstractmethod
     def get_decoder_list(self) -> list:
         """Returns a list of decoder objects for this data stream.
 
         Notes
```

### Comparing `pygama-1.2.0/src/pygama/raw/fc/fc_config_decoder.py` & `pygama-1.3.0/src/pygama/raw/fc/fc_config_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/raw/fc/fc_event_decoder.py` & `pygama-1.3.0/src/pygama/raw/fc/fc_event_decoder.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,134 +10,90 @@
 from pygama.raw.data_decoder import DataDecoder
 
 log = logging.getLogger(__name__)
 
 # put decoded values here where they can be used also by the orca decoder
 fc_decoded_values = {
     # packet index in file
-    "packet_id": {
-        "dtype": "uint32",
-    },
+    "packet_id": {"dtype": "uint32"},
     # index of event
-    "eventnumber": {
-        "dtype": "int32",
-    },
+    "eventnumber": {"dtype": "int32"},
     # time since epoch
-    "timestamp": {
-        "dtype": "float64",
-        "units": "s",
-    },
+    "timestamp": {"dtype": "float64", "units": "s"},
     # time since beginning of file
-    "runtime": {
-        "dtype": "float64",
-        "units": "s",
-    },
+    "runtime": {"dtype": "float64", "units": "s"},
     # number of triggered adc channels
-    "numtraces": {
-        "dtype": "int32",
-    },
+    "numtraces": {"dtype": "int32"},
     # list of triggered adc channels
     "tracelist": {
         "dtype": "int16",
         "datatype": "array<1>{array<1>{real}}",  # vector of vectors
         "length_guess": 16,
     },
     # fpga baseline
-    "baseline": {
-        "dtype": "uint16",
-    },
+    "baseline": {"dtype": "uint16"},
     # fpga energy
-    "daqenergy": {
-        "dtype": "uint16",
-    },
+    "daqenergy": {"dtype": "uint16"},
     # right now, index of the trigger (trace)
-    "channel": {
-        "dtype": "uint32",
-    },
+    "channel": {"dtype": "uint32"},
     # PPS timestamp in sec
-    "ts_pps": {
-        "dtype": "int32",
-    },
+    "ts_pps": {"dtype": "int32"},
     # clock ticks
-    "ts_ticks": {
-        "dtype": "int32",
-    },
+    "ts_ticks": {"dtype": "int32"},
     # max clock ticks
-    "ts_maxticks": {
-        "dtype": "int32",
-    },
+    "ts_maxticks": {"dtype": "int32"},
     # the offset in sec between the master and unix
-    "to_mu_sec": {
-        "dtype": "int64",
-    },
+    "mu_offset_sec": {"dtype": "int32"},
     # the offset in usec between master and unix
-    "to_mu_usec": {
-        "dtype": "int32",
-    },
+    "mu_offset_usec": {"dtype": "int32"},
     # the calculated sec which must be added to the master
-    "to_master_sec": {
-        "dtype": "int64",
-    },
+    "to_master_sec": {"dtype": "int32"},
     # the delta time between master and unix in usec
-    "to_dt_mu_usec": {
-        "dtype": "int32",
-    },
+    "delta_mu_usec": {"dtype": "int32"},
     # the abs(time) between master and unix in usec
-    "to_abs_mu_usec": {
-        "dtype": "int32",
-    },
+    "abs_delta_mu_usec": {"dtype": "int32"},
     # startsec
-    "to_start_sec": {
-        "dtype": "int64",
-    },
+    "to_start_sec": {"dtype": "int32"},
     # startusec
-    "to_start_usec": {
-        "dtype": "int32",
-    },
+    "to_start_usec": {"dtype": "int32"},
     # start pps of the next dead window
-    "dr_start_pps": {
-        "dtype": "int32",
-    },
+    "dr_start_pps": {"dtype": "int32"},
     # start ticks of the next dead window
-    "dr_start_ticks": {
-        "dtype": "int32",
-    },
+    "dr_start_ticks": {"dtype": "int32"},
     # stop pps of the next dead window
-    "dr_stop_pps": {
-        "dtype": "int32",
-    },
+    "dr_stop_pps": {"dtype": "int32"},
     # stop ticks of the next dead window
-    "dr_stop_ticks": {
-        "dtype": "int32",
-    },
+    "dr_stop_ticks": {"dtype": "int32"},
     # maxticks of the dead window
-    "dr_maxticks": {
-        "dtype": "int32",
-    },
+    "dr_maxticks": {"dtype": "int32"},
     # current dead time calculated from deadregion (dr) fields.
     # Give the total dead time if summed up.
-    "deadtime": {
-        "dtype": "float64",
-    },
+    "deadtime": {"dtype": "float64"},
     # waveform data
     "waveform": {
         "dtype": "uint16",
         "datatype": "waveform",
         "wf_len": 65532,  # max value. override this before initializing buffers to save RAM
         "dt": 16,  # override if a different clock rate is used
         "dt_units": "ns",
         "t0_units": "ns",
     },
 }
+"""Default FlashCam Event decoded values.
+
+Re-used by :class:`~.raw.orca.orca_flashcam.ORFlashCamWaveformDecoder`.
+
+Warning
+-------
+This configuration can be dynamically modified by the decoder at runtime.
+"""
 
 
 class FCEventDecoder(DataDecoder):
-    """
-    Decode FlashCam digitizer event data.
-    """
+    """Decode FlashCam digitizer event data."""
 
     def __init__(self, *args, **kwargs) -> None:
         # these are read for every event (decode_event)
         self.decoded_values = copy.deepcopy(fc_decoded_values)
         super().__init__(*args, **kwargs)
         self.skipped_channels = {}
         self.fc_config = None
@@ -222,29 +178,31 @@
                 ii
             ] = fcio.eventnumber  # the eventnumber since the beginning of the file
             tbl["timestamp"].nda[ii] = fcio.eventtime  # the time since epoch in seconds
             tbl["runtime"].nda[
                 ii
             ] = fcio.runtime  # the time since the beginning of the file in seconds
             tbl["numtraces"].nda[ii] = fcio.numtraces  # number of triggered adcs
-            tbl["tracelist"].set_vector(ii, fcio.tracelist)  # list of triggered adcs
+            tbl["tracelist"]._set_vector_unsafe(
+                ii, fcio.tracelist
+            )  # list of triggered adcs
             tbl["baseline"].nda[ii] = fcio.baseline[
                 iwf
             ]  # the fpga baseline values for each channel in LSB
             tbl["daqenergy"].nda[ii] = fcio.daqenergy[
                 iwf
             ]  # the fpga energy values for each channel in LSB
             tbl["ts_pps"].nda[ii] = fcio.timestamp_pps
             tbl["ts_ticks"].nda[ii] = fcio.timestamp_ticks
             tbl["ts_maxticks"].nda[ii] = fcio.timestamp_maxticks
-            tbl["to_mu_sec"].nda[ii] = fcio.timeoffset_mu_sec
-            tbl["to_mu_usec"].nda[ii] = fcio.timeoffset_mu_usec
+            tbl["mu_offset_sec"].nda[ii] = fcio.timeoffset_mu_sec
+            tbl["mu_offset_usec"].nda[ii] = fcio.timeoffset_mu_usec
             tbl["to_master_sec"].nda[ii] = fcio.timeoffset_master_sec
-            tbl["to_dt_mu_usec"].nda[ii] = fcio.timeoffset_dt_mu_usec
-            tbl["to_abs_mu_usec"].nda[ii] = fcio.timeoffset_abs_mu_usec
+            tbl["delta_mu_usec"].nda[ii] = fcio.timeoffset_dt_mu_usec
+            tbl["abs_delta_mu_usec"].nda[ii] = fcio.timeoffset_abs_mu_usec
             tbl["to_start_sec"].nda[ii] = fcio.timeoffset_start_sec
             tbl["to_start_usec"].nda[ii] = fcio.timeoffset_start_usec
             tbl["dr_start_pps"].nda[ii] = fcio.deadregion_start_pps
             tbl["dr_start_ticks"].nda[ii] = fcio.deadregion_start_ticks
             tbl["dr_stop_pps"].nda[ii] = fcio.deadregion_stop_pps
             tbl["dr_stop_ticks"].nda[ii] = fcio.deadregion_stop_ticks
             tbl["dr_maxticks"].nda[ii] = fcio.deadregion_maxticks
```

### Comparing `pygama-1.2.0/src/pygama/raw/fc/fc_status_decoder.py` & `pygama-1.3.0/src/pygama/raw/fc/fc_status_decoder.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,71 +2,60 @@
 
 import fcutils
 
 from pygama.raw.data_decoder import DataDecoder, RawBuffer
 
 
 class FCStatusDecoder(DataDecoder):
-    """
-    Decode FlashCam digitizer status data.
-    """
+    """Decode FlashCam digitizer status data."""
 
     def __init__(self, *args, **kwargs) -> None:
         self.decoded_values = {
-            "status": {  # 0: Errors occurred, 1: no errors
-                "dtype": "int32",
-            },
-            "statustime": {  # fc250 seconds, microseconds, dummy, startsec startusec
-                "dtype": "float32",
-                "units": "s",
-            },
-            "cputime": {  # CPU seconds, microseconds, dummy, startsec startusec
-                "dtype": "float64",
-                "units": "s",
-            },
-            "startoffset": {  # fc250 seconds, microseconds, dummy, startsec startusec
-                "dtype": "float32",
-                "units": "s",
-            },
-            "cards": {  # Total number of cards (number of status data to follow)
-                "dtype": "int32",
-            },
-            "size": {  # Size of each status data
-                "dtype": "int32",
-            },
-            "environment": {  # FC card-wise environment status
+            # 0: Errors occurred, 1: no errors
+            "status": {"dtype": "int32"},
+            # fc250 seconds, microseconds, dummy, startsec startusec
+            "statustime": {"dtype": "float32", "units": "s"},
+            # CPU seconds, microseconds, dummy, startsec startusec
+            "cputime": {"dtype": "float64", "units": "s"},
+            # fc250 seconds, microseconds, dummy, startsec startusec
+            "startoffset": {"dtype": "float32", "units": "s"},
+            # Total number of cards (number of status data to follow)
+            "cards": {"dtype": "int32"},
+            # Size of each status data
+            "size": {"dtype": "int32"},
+            # FC card-wise environment status
+            "environment": {
                 # Array contents:
                 # [0-4] Temps in mDeg
                 # [5-10] Voltages in mV
                 # 11 main current in mA
                 # 12 humidity in o/oo
                 # [13-14] Temps from adc cards in mDeg
                 # FIXME: change to a table?
                 "dtype": "uint32",
                 "datatype": "array_of_equalsized_arrays<1,1>{real}",
                 "length": 16,
             },
-            "totalerrors": {  # FC card-wise list DAQ errors during data taking
-                "dtype": "uint32",
-            },
-            "enverrors": {
-                "dtype": "uint32",
-            },
-            "ctierrors": {
-                "dtype": "uint32",
-            },
-            "linkerrors": {
-                "dtype": "uint32",
-            },
+            # FC card-wise list DAQ errors during data taking
+            "totalerrors": {"dtype": "uint32"},
+            "enverrors": {"dtype": "uint32"},
+            "ctierrors": {"dtype": "uint32"},
+            "linkerrors": {"dtype": "uint32"},
             "othererrors": {
                 "dtype": "uint32",
                 "datatype": "array_of_equalsized_arrays<1,1>{real}",
                 "length": 5,
             },
         }
+        """Default FlashCam status decoded values.
+
+        Warning
+        -------
+        This configuration can be dynamically modified by the decoder at runtime.
+        """
         super().__init__(*args, **kwargs)
 
     def decode_packet(
         self, fcio: fcutils.fcio, status_rb: RawBuffer, packet_id: int
     ) -> bool:
         # aliases for brevity
         tbl = status_rb.lgdo
```

### Comparing `pygama-1.2.0/src/pygama/raw/fc/fc_streamer.py` & `pygama-1.3.0/src/pygama/raw/fc/fc_streamer.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/raw/orca/orca_base.py` & `pygama-1.3.0/src/pygama/raw/orca/orca_base.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/raw/orca/orca_digitizers.py` & `pygama-1.3.0/src/pygama/raw/orca/orca_digitizers.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 class ORSIS3302DecoderForEnergy(OrcaDecoder):
     """Decoder for `Struck SIS3302 <https://www.struck.de/sis3302.htm>`_ digitizer
     data written by ORCA.
     """
 
     def __init__(self, header: OrcaHeader = None, **kwargs) -> None:
-
         self.decoded_values_template = {
             "packet_id": {
                 "dtype": "uint32",
             },
             "energy": {
                 "dtype": "uint32",
                 "units": "adc",
@@ -49,14 +48,20 @@
                 "datatype": "waveform",
                 "wf_len": 65532,  # max value. override this before initializing buffers to save RAM
                 "dt": 10,  # override if a different clock rate is used
                 "dt_units": "ns",
                 "t0_units": "ns",
             },
         }
+        """Default Struck SIS3302 (read out by ORCA) waveform decoded values.
+
+        Warning
+        -------
+        This configuration can be dynamically modified by the decoder at runtime.
+        """
         self.decoded_values = {}
         super().__init__(header=header, **kwargs)
         self.skipped_channels = {}
 
     def set_header(self, header: OrcaHeader) -> None:
         self.header = header
 
@@ -89,19 +94,19 @@
                         int(channel / 2)
                     ]
                     if trace_length <= 0 or trace_length > 2**16:
                         raise RuntimeError(f"invalid trace_length {trace_length}")
                         sys.exit()
                     self.decoded_values[ccc]["waveform"]["wf_len"] = trace_length
 
-    def get_key_lists(self) -> list[str]:
+    def get_key_lists(self) -> list[list[str]]:
         key_lists = []
         for key in self.decoded_values.keys():
             key_lists.append([key])
-        return key_lists
+        return [key_lists]
 
     def get_decoded_values(self, key: int = None) -> dict[str, Any]:
         if key is None:
             dec_vals_list = self.decoded_values.values()
             if len(dec_vals_list) >= 0:
                 return list(dec_vals_list)[0]
             raise RuntimeError("decoded_values not built")
@@ -207,113 +212,55 @@
 
 
 class ORSIS3316WaveformDecoder(OrcaDecoder):
     """Decoder for `Struck SIS3316 <https://www.struck.de/sis3316.html>`_
     digitizer data written by ORCA."""
 
     def __init__(self, header: OrcaHeader = None, **kwargs) -> None:
-
         # store an entry for every event
         self.decoded_values_template = {
-            "packet_id": {
-                "dtype": "uint32",
-            },
-            "energy": {
-                "dtype": "uint32",
-                "units": "adc",
-            },
-            "peakHighValue": {
-                "dtype": "uint32",
-                "units": "adc",
-            },
-            "peakHighIndex": {
-                "dtype": "uint32",
-                "units": "adc",
-            },
-            "accSum1": {
-                "dtype": "uint32",
-                "units": "adc",
-            },
-            "information": {
-                "dtype": "uint32",
-            },
-            "accSum2": {
-                "dtype": "uint32",
-                "units": "adc",
-            },
-            "accSum3": {
-                "dtype": "uint32",
-                "units": "adc",
-            },
-            "accSum4": {
-                "dtype": "uint32",
-                "units": "adc",
-            },
-            "accSum5": {
-                "dtype": "uint32",
-                "units": "adc",
-            },
-            "accSum6": {
-                "dtype": "uint32",
-                "units": "adc",
-            },
-            "accSum7": {
-                "dtype": "uint32",
-                "units": "adc",
-            },
-            "accSum8": {
-                "dtype": "uint32",
-                "units": "adc",
-            },
-            "mawMax": {
-                "dtype": "uint32",
-                "units": "adc",
-            },
-            "mawBefore": {
-                "dtype": "uint32",
-                "units": "adc",
-            },
-            "mawAfter": {
-                "dtype": "uint32",
-                "units": "adc",
-            },
-            "startEnergy": {
-                "dtype": "uint32",
-                "units": "adc",
-            },
-            "maxEnergy": {
-                "dtype": "uint32",
-                "units": "adc",
-            },
-            "energy_first": {
-                "dtype": "uint32",
-            },
-            "timestamp": {
-                "dtype": "uint64",
-                "units": "clock_ticks",
-            },
-            "crate": {
-                "dtype": "uint8",
-            },
-            "card": {
-                "dtype": "uint8",
-            },
-            "channel": {
-                "dtype": "uint8",
-            },
+            "packet_id": {"dtype": "uint32"},
+            "energy": {"dtype": "uint32", "units": "adc"},
+            "peakHighValue": {"dtype": "uint32", "units": "adc"},
+            "peakHighIndex": {"dtype": "uint32", "units": "adc"},
+            "accSum1": {"dtype": "uint32", "units": "adc"},
+            "information": {"dtype": "uint32"},
+            "accSum2": {"dtype": "uint32", "units": "adc"},
+            "accSum3": {"dtype": "uint32", "units": "adc"},
+            "accSum4": {"dtype": "uint32", "units": "adc"},
+            "accSum5": {"dtype": "uint32", "units": "adc"},
+            "accSum6": {"dtype": "uint32", "units": "adc"},
+            "accSum7": {"dtype": "uint32", "units": "adc"},
+            "accSum8": {"dtype": "uint32", "units": "adc"},
+            "mawMax": {"dtype": "uint32", "units": "adc"},
+            "mawBefore": {"dtype": "uint32", "units": "adc"},
+            "mawAfter": {"dtype": "uint32", "units": "adc"},
+            "startEnergy": {"dtype": "uint32", "units": "adc"},
+            "maxEnergy": {"dtype": "uint32", "units": "adc"},
+            "energy_first": {"dtype": "uint32"},
+            "timestamp": {"dtype": "uint64", "units": "clock_ticks"},
+            "crate": {"dtype": "uint8"},
+            "card": {"dtype": "uint8"},
+            "channel": {"dtype": "uint8"},
             # waveform data
             "waveform": {
                 "dtype": "uint16",
                 "datatype": "waveform",
                 "wf_len": 65532,  # max value. override this before initializing buffers to save RAM
                 "dt": 8,  # override if a different clock rate is used
                 "dt_units": "ns",
                 "t0_units": "ns",
             },
         }
+        """Default Struck SIS3316 (read out by ORCA) waveform decoded values.
+
+        Warning
+        -------
+        This configuration can be dynamically modified by the decoder at runtime.
+        """
 
         self.decoded_values = {}
         self.skipped_channels = {}
         super().__init__(
             header=header, **kwargs
         )  # also initializes the garbage df (whatever that means...)
 
@@ -340,19 +287,19 @@
                                 trace_length,
                             )
 
                         self.decoded_values[ccc]["waveform"]["wf_len"] = trace_length
                     else:
                         continue
 
-    def get_key_lists(self) -> list[int]:
+    def get_key_lists(self) -> list[list[str]]:
         key_lists = []
         for key in self.decoded_values.keys():
             key_lists.append([key])
-        return key_lists
+        return [key_lists]
 
     def get_decoded_values(self, key: int = None) -> dict[str, Any]:
         if key is None:
             dec_vals_list = self.decoded_values.values()
             if len(dec_vals_list) == 0:
                 raise RuntimeError("decoded_values not built yet!")
```

### Comparing `pygama-1.2.0/src/pygama/raw/orca/orca_header.py` & `pygama-1.3.0/src/pygama/raw/orca/orca_header.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/raw/orca/orca_header_decoder.py` & `pygama-1.3.0/src/pygama/raw/orca/orca_header_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/raw/orca/orca_packet.py` & `pygama-1.3.0/src/pygama/raw/orca/orca_packet.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
     print_n_words: bool = False,
     max_words: int = np.inf,
     as_int: bool = False,
     as_short: bool = False,
     id_dict: dict = None,
     use_logging: bool = True,
 ) -> None:
-
     dump_cmd = print  # noqa: T202
     if use_logging:
         dump_cmd = log.debug
 
     data_id = get_data_id(packet, shift=shift_data_id)
     n_words = get_n_words(packet)
     if id_dict is not None:
```

### Comparing `pygama-1.2.0/src/pygama/raw/orca/orca_run_decoder.py` & `pygama-1.3.0/src/pygama/raw/orca/orca_run_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/raw/orca/orca_streamer.py` & `pygama-1.3.0/src/pygama/raw/orca/orca_streamer.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pygama.raw.data_streamer import DataStreamer
 from pygama.raw.orca import orca_packet
 from pygama.raw.orca.orca_base import OrcaDecoder
 from pygama.raw.orca.orca_digitizers import (  # noqa: F401
     ORSIS3302DecoderForEnergy,
     ORSIS3316WaveformDecoder,
 )
-from pygama.raw.orca.orca_flashcam import (  # noqa: F401
+from pygama.raw.orca.orca_flashcam import (  # noqa: F401; ORFlashCamListenerStatusDecoder,
     ORFlashCamADCWaveformDecoder,
     ORFlashCamListenerConfigDecoder,
     ORFlashCamWaveformDecoder,
 )
 from pygama.raw.orca.orca_header_decoder import OrcaHeaderDecoder
 from pygama.raw.orca.orca_run_decoder import ORRunDecoderForRun  # noqa: F401
 from pygama.raw.raw_buffer import RawBuffer, RawBufferLibrary
@@ -73,17 +73,18 @@
 
         # load into buffer, resizing as necessary
         if len(self.buffer) < n_words:
             self.buffer.resize(n_words, refcheck=False)
         n_bytes_read = self.in_stream.readinto(self.buffer[1:n_words])
         self.n_bytes_read += n_bytes_read
         if n_bytes_read != (n_words - 1) * 4:
-            raise RuntimeError(
-                f"only got {n_bytes_read} bytes for packet read when {(n_words-1)*4} were expected."
+            log.error(
+                f"only got {n_bytes_read} bytes for packet read when {(n_words-1)*4} were expected. Flushing all buffers and quitting..."
             )
+            return None
 
         # return just the packet
         return self.buffer[:n_words]
 
     def get_decoder_list(self) -> list[OrcaDecoder]:
         return list(self.decoder_id_dict.values())
 
@@ -109,28 +110,38 @@
         orca = OrcaStreamer()
         orca.set_in_stream(stream_name)
         first_bytes = orca.in_stream.read(12)
         orca.close_in_stream()
 
         # that read should have succeeded
         if len(first_bytes) != 12:
+            log.debug(f"first 12B read only returned {first_bytes}B: not orca")
             return False
 
         # first 14 bits should be zero
         uints = np.frombuffer(first_bytes, dtype="uint32")
         if (uints[0] & 0xFFFC0000) != 0:
+            log.debug(
+                f"first fourteen bits non-zero ({uints[0] & 0xFFFC0000}): not orca"
+            )
             return False
 
         # xml header length should fit within header packet length
         pad = uints[0] * 4 - 8 - uints[1]
         if pad < 0 or pad > 3:
+            log.debug(
+                f"header length = {uints[1]}B doesn't fit right within header packet length = {uints[0]*4-8}B: not orca"
+            )
             return False
 
         # last 4 chars should be '<?xm'
         if first_bytes[8:].decode() != "<?xm":
+            log.debug(
+                f"last 4 chars of first 12 bytes = {first_bytes[8:].decode()} != '<?xm': not orca"
+            )
             return False
 
         # it must be an orca stream
         return True
 
     def hex_dump(
         self,
```

### Comparing `pygama-1.2.0/src/pygama/raw/raw_buffer.py` & `pygama-1.3.0/src/pygama/raw/raw_buffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 :class:`.RawBuffer`: an LGDO (e.g. a table) along with buffer metadata, such as the
 current write location, the list of keys (e.g. channels) that write to it, the
 output stream it is associated with (if any), etc. Each
 :class:`~.raw.data_decoder.DataDecoder` is associated with a
 :class:`.RawBuffer` of a particular format.
 
 :class:`.RawBufferList`: a collection of :class:`RawBuffer` with LGDO's that
-all have the same structure (same type, same fields, etc). A
-:class:`~.raw.data_decoder.DataDecoder` will write its output to a
-:class:`.RawBufferList`.
+all have the same structure (same type, same fields, etc., but the fields can
+have different shape). A :class:`~.raw.data_decoder.DataDecoder` will write its
+output to a :class:`.RawBufferList`.
 
 :class:`.RawBufferLibrary`: a dictionary of :class:`RawBufferList`\ s, e.g. one
 for each :class:`~.raw.data_decoder.DataDecoder`. Keyed by the decoder name.
 
 :class:`.RawBuffer` supports a JSON short-hand notation, see
 :meth:`.RawBufferLibrary.set_from_json_dict` for full specification.
 
@@ -93,15 +93,15 @@
         a list of keys (e.g. channel numbers) identifying data to be written
         into this buffer. The key scheme is specific to the decoder with which
         the :class:`.RawBuffer` is associated. This is called `key_list`
         instead of `keys` to avoid confusion with the dict function
         :meth:`dict.keys`, i.e.  ``raw_buffer.lgdo.keys()``.
     out_stream
         the output stream to which the :class:`.RawBuffer`\ 's LGDO should be
-        sent or written. A colon (``,``) can be used to separate the stream
+        sent or written. A colon (``:``) can be used to separate the stream
         name/address from an in-stream path/port:
         - file example: ``/path/filename.lh5:/group``
         - socket example: ``198.0.0.100:8000``
     out_name
         the name or identifier of the object in the output stream.
     proc_spec
         a dictionary containing the following:
@@ -387,56 +387,67 @@
             if isinstance(key_range, list) and len(key_range) == 2:
                 info["key_list"][i : i + 1] = range(key_range[0], key_range[1] + 1)
                 i += key_range[1] - key_range[0]
             i += 1
 
         # Expand list_names if name contains a key-based formatter
         if "{key" in name:
-            if len(info["key_list"]) == 1 and info["key_list"][0] == "*":
+            if (
+                len(info["key_list"]) == 1
+                and isinstance(info["key_list"][0], str)
+                and "*" in info["key_list"][0]
+            ):
                 continue  # will be handled later, once the key_list is known
             for key in info["key_list"]:
                 expanded_name = name.format(key=key)
                 json_dict[expanded_name] = info.copy()
                 json_dict[expanded_name]["key_list"] = [key]
             json_dict.pop(name)
 
     # now re-iterate and expand out_paths
     for name, info in json_dict.items():
-        if len(info["key_list"]) == 1 and info["key_list"][0] != "*":
+        if len(info["key_list"]) == 1 and not (
+            isinstance(info["key_list"][0], str) and "*" in info["key_list"][0]
+        ):
             kw_dict["key"] = info["key_list"][0]
         if "out_stream" in info:
             if name != "*" and "{name" in info["out_stream"]:
                 kw_dict["name"] = name
             try:
                 info["out_stream"] = info["out_stream"].format(**kw_dict)
             except KeyError as msg:
                 raise KeyError(
                     f"variable {msg} dereferenced in 'out_stream' not defined in kw_dict"
                 )
             info["out_stream"] = os.path.expandvars(info["out_stream"])
 
 
 def write_to_lh5_and_clear(
-    raw_buffers: list[RawBuffer], lh5_store: LH5Store = None, wo_mode: str = "append"
+    raw_buffers: list[RawBuffer], lh5_store: LH5Store = None, **kwargs
 ) -> None:
-    r"""Write a list of :class:`.RawBuffer`\ s to LH5 files and then clears
-    them.
+    r"""Write a list of :class:`.RawBuffer`\ s to LH5 files and then clears them.
 
     Parameters
     ----------
-    raw_buffers : list(RawBuffer)
-        The list of RawBuffers to be written to file. Note this is not a
-        RawBufferList because the RawBuffers may not have the same structure.
-        If a raw_buffer has a `proc_spec` attribute, then :meth:`.buffer_processor.buffer_processor.buffer_processor`
-        is used to process that raw_buffer.
-    lh5_store : LH5Store or None
+    raw_buffers
+        The list of ``RawBuffer``\ s to be written to file. Note: this is not a
+        :class:`.RawBufferList` because the raw buffers may not have the
+        same structure.  If a raw buffer has a `proc_spec` attribute, then
+        :meth:`.buffer_processor.buffer_processor.buffer_processor` is used to
+        process that buffer.
+    lh5_store
         Allows user to send in a store holding a collection of already open
-        files (saves some time opening / closing files)
-    wo_mode : str
-        write mode, see also :meth:`.lgdo.lh5_store.LH5Store.write_object`
+        files (saves some time opening / closing files).
+    **kwargs
+        keyword-arguments forwarded to
+        :meth:`.lgdo.lh5_store.LH5Store.write_object`.
+
+    See Also
+    --------
+    .lgdo.lh5_store.LH5Store.write_object
     """
     if lh5_store is None:
         lh5_store = lgdo.LH5Store()
     for rb in raw_buffers:
         if rb.lgdo is None or rb.loc == 0:
             continue  # no data to write
         ii = rb.out_stream.find(":")
@@ -460,11 +471,11 @@
         if filename != "":
             lh5_store.write_object(
                 lgdo_to_write,
                 rb.out_name,
                 filename,
                 group=group,
                 n_rows=rb.loc,
-                wo_mode=wo_mode,
+                **kwargs,
             )
         # and clear
         rb.loc = 0
```

### Comparing `pygama-1.2.0/src/pygama/vis/mpl/clint.mpl` & `pygama-1.3.0/src/pygama/vis/mpl/clint.mpl`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/vis/mpl/root.mpl` & `pygama-1.3.0/src/pygama/vis/mpl/root.mpl`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/src/pygama/vis/waveform_browser.py` & `pygama-1.3.0/src/pygama/vis/waveform_browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     :func:`~.dsp.build_dsp.build_dsp` style JSON files, drawing horizontal and
     vertical lines at the values of calculated parameters, and filling a legend
     with calculated parameters.
     """
 
     def __init__(
         self,
-        files_in: str | list[str],
-        lh5_group: str,
+        files_in: str | list[str] | lgdo.LH5Iterator,  # noqa: F821
+        lh5_group: str | list[str] = "",
         base_path: str = "",
         entry_list: list[int] | list[list[int]] = None,
         entry_mask: list[int] | list[list[int]] = None,
         dsp_config: str = None,
         database: str | dict = None,
         aux_values: pandas.DataFrame = None,
         lines: str | list[str] = "waveform",
@@ -49,19 +49,21 @@
         buffer_len: int = 128,
         block_width: int = 8,
     ) -> None:
         """
         Parameters
         ----------
         files_in
-            name of file or list of names to browse. Can use wildcards.
+            name of file or list of files to browse. Can use wildcards. Can
+            also pass an LH5Iterator
 
         lh5_group
-            name of LH5 group in file to browse.
-
+            HDF5 group(s) to read. If a list is provided for both lh5_files
+            and group, they must be the same size. If a file is wild-carded,
+            the same group will be assigned to each file found
         base_path
             base path for file. See :class:`~.lgdo.lh5_store.LH5Store`.
 
         entry_list
             list of event indices to draw. If it is a nested list, use local
             indices for each file, otherwise use global indices.
 
@@ -145,37 +147,40 @@
 
         self.norm_par = norm
         self.align_par = align
         self.n_drawn = n_drawn
         self.next_entry = 0
 
         # data i/o initialization
-        # HACK: do not read VOV "tracelist", cannot be handled correctly by LH5Iterator
-        # remove this hack once VOV support is properly implemented
-        self.lh5_it = lh5.LH5Iterator(
-            files_in,
-            lh5_group,
-            base_path=base_path,
-            entry_list=entry_list,
-            entry_mask=entry_mask,
-            field_mask={"tracelist": False},
-            buffer_len=buffer_len,
-        )
+        if isinstance(files_in, lh5.LH5Iterator):
+            self.lh5_it = files_in
+        else:
+            # HACK: do not read VOV "tracelist", cannot be handled correctly by LH5Iterator
+            # remove this hack once VOV support is properly implemented
+            self.lh5_it = lh5.LH5Iterator(
+                files_in,
+                lh5_group,
+                base_path=base_path,
+                entry_list=entry_list,
+                entry_mask=entry_mask,
+                field_mask={"tracelist": False},
+                buffer_len=buffer_len,
+            )
 
         # Get the input buffer and read the first chunk
         self.lh5_in, _ = self.lh5_it.read(0)
 
         self.aux_vals = aux_values
         # Apply entry selection to aux_vals if needed
-        if self.aux_vals is not None and len(self.aux_vals) > len(self.lh5_it):
-            entries = []
-            for i, f_entries in enumerate(self.lh5_it.entry_list):
-                entry_offset = self.lh5_it.file_map[i - 1] if i > 0 else 0
-                entries += [entry_offset + entry for entry in f_entries]
-            self.aux_vals = self.aux_vals.iloc[entries].reset_index()
+        if self.aux_vals is not None and len(self.aux_vals) > len(
+            self.lh5_it.get_global_entrylist()
+        ):
+            self.aux_vals = self.aux_vals.iloc[
+                self.lh5_it.get_global_entrylist()
+            ].reset_index()
 
         # initialize objects to draw: dict from name to list of 2DLines
         if isinstance(lines, str):
             self.lines = {lines: []}
         elif lines is None:
             self.lines = {}
         else:
@@ -241,21 +246,22 @@
         if isinstance(self.align_par, str):
             outputs += [self.align_par]
 
         # Remove any values not found in aux_vals
         if self.aux_vals is not None:
             outputs = [o for o in outputs if o not in self.aux_vals]
 
-        self.proc_chain, self.lh5_it.field_mask, self.lh5_out = build_processing_chain(
+        self.proc_chain, field_mask, self.lh5_out = build_processing_chain(
             self.lh5_in,
             dsp_config,
             db_dict=database,
             outputs=outputs,
             block_width=block_width,
         )
+        self.lh5_it.reset_field_mask(field_mask)
         self.proc_chain.execute()
 
         # Check if all of our outputs can be found
         for name in outputs:
             if name not in self.lh5_out:
                 raise KeyError(
                     "Could not find "
@@ -264,14 +270,15 @@
                 )
 
         self.x_unit = ureg(x_unit) if x_unit else None
         self.x_lim = x_lim
         self.y_lim = y_lim
         self.auto_x_lim = [np.inf, -np.inf]
         self.auto_y_lim = [np.inf, -np.inf]
+        self.n_stored = 0
 
         # Set limit and convert to x-unit if needed; also set x_unit if needed
         if self.x_lim is not None:
             self.x_lim = list(self.x_lim)
             for i in range(2):
                 if isinstance(self.x_lim[i], str):
                     self.x_lim[i] = ureg.Quantity(x_lim[i])
@@ -351,24 +358,26 @@
         if not append:
             self.clear_data()
         if hasattr(entry, "__iter__"):
             for idx in entry:
                 self.find_entry(idx)
             return
 
-        if entry > len(self.lh5_it):
-            if not safe:
-                raise IndexError
-            else:
-                return
-
         # Get our current position in the I/O buffers; update if needed
         i_tb = entry - self.lh5_it.current_entry
         if not (self.lh5_it.n_rows > i_tb >= 0):
             self.lh5_it.read(entry)
+
+            # Check if entry is out of range
+            if self.lh5_it.n_rows == 0:
+                if safe:
+                    raise IndexError
+                else:
+                    return
+
             self.proc_chain.execute()
             i_tb = 0
 
         # get scaling factor/time shift if used
         if self.norm_par is None:
             norm = 1.0
         elif isinstance(self.norm_par, str):
@@ -489,15 +498,15 @@
         default_style = cycler(plt.rcParams["axes.prop_cycle"])
         for i, lines in enumerate(self.lines.values()):
             if isinstance(self.styles, list):
                 styles = self.styles[i]
             if styles is None:
                 styles = default_style
 
-            for line, sty in zip(lines, styles):
+            for line, sty in zip(lines, itertools.cycle(styles)):
                 if sty is not None:
                     line.update(sty)
                 if line.get_figure() is not None:
                     line.remove()
                 line.set_transform(self.ax.transData)
                 self.ax.add_line(line)
 
@@ -588,15 +597,15 @@
         return entries
 
     def draw_next(
         self, n_wfs: int = None, append: bool = False, clear: bool = True
     ) -> tuple[int, int]:
         """Draw the next `n_wfs` waveforms (default `self.n_drawn`). See
         :meth:`draw_next`."""
-        entries = self.find_next(append)
+        entries = self.find_next(n_wfs, append)
         self.draw_current(clear)
         return entries
 
     def reset(self) -> None:
         """Reset to the start of the file for :meth:`draw_next`."""
         self.clear_data()
         self.next_entry = 0
```

### Comparing `pygama-1.2.0/src/pygama.egg-info/PKG-INFO` & `pygama-1.3.0/src/pygama.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygama
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python package for decoding and processing digitizer data
 Home-page: https://github.com/legend-exp/pygama
 Author: The LEGEND collaboration
 Maintainer: The LEGEND collaboration
 License: GPL-3.0
 Project-URL: Documentation, https://pygama.readthedocs.io
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pygama-1.2.0/src/pygama.egg-info/SOURCES.txt` & `pygama-1.3.0/src/pygama.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -50,30 +50,37 @@
 src/pygama/dsp/processors/wiener_filter.py
 src/pygama/dsp/processors/windower.py
 src/pygama/evt/__init__.py
 src/pygama/evt/build_tcm.py
 src/pygama/evt/tcm.py
 src/pygama/flow/__init__.py
 src/pygama/flow/data_loader.py
-src/pygama/flow/datagroup.py
 src/pygama/flow/file_db.py
+src/pygama/flow/utils.py
 src/pygama/hit/__init__.py
 src/pygama/hit/build_hit.py
 src/pygama/lgdo/__init__.py
 src/pygama/lgdo/array.py
 src/pygama/lgdo/arrayofequalsizedarrays.py
+src/pygama/lgdo/encoded.py
 src/pygama/lgdo/fixedsizearray.py
 src/pygama/lgdo/lgdo.py
 src/pygama/lgdo/lgdo_utils.py
 src/pygama/lgdo/lh5_store.py
 src/pygama/lgdo/scalar.py
 src/pygama/lgdo/struct.py
 src/pygama/lgdo/table.py
 src/pygama/lgdo/vectorofvectors.py
 src/pygama/lgdo/waveform_table.py
+src/pygama/lgdo/compression/__init__.py
+src/pygama/lgdo/compression/base.py
+src/pygama/lgdo/compression/generic.py
+src/pygama/lgdo/compression/radware.py
+src/pygama/lgdo/compression/utils.py
+src/pygama/lgdo/compression/varlen.py
 src/pygama/math/__init__.py
 src/pygama/math/histogram.py
 src/pygama/math/peak_fitting.py
 src/pygama/math/units.py
 src/pygama/math/utils.py
 src/pygama/pargen/AoE_cal.py
 src/pygama/pargen/__init__.py
@@ -89,14 +96,19 @@
 src/pygama/raw/build_raw.py
 src/pygama/raw/data_decoder.py
 src/pygama/raw/data_streamer.py
 src/pygama/raw/raw_buffer.py
 src/pygama/raw/buffer_processor/__init__.py
 src/pygama/raw/buffer_processor/buffer_processor.py
 src/pygama/raw/buffer_processor/lh5_buffer_processor.py
+src/pygama/raw/compass/__init__.py
+src/pygama/raw/compass/compass_config_parser.py
+src/pygama/raw/compass/compass_event_decoder.py
+src/pygama/raw/compass/compass_header_decoder.py
+src/pygama/raw/compass/compass_streamer.py
 src/pygama/raw/fc/__init__.py
 src/pygama/raw/fc/fc_config_decoder.py
 src/pygama/raw/fc/fc_event_decoder.py
 src/pygama/raw/fc/fc_status_decoder.py
 src/pygama/raw/fc/fc_streamer.py
 src/pygama/raw/orca/__init__.py
 src/pygama/raw/orca/orca_base.py
@@ -127,48 +139,65 @@
 tests/dsp/processors/test_dwt.py
 tests/dsp/processors/test_fixed_time_pickoff.py
 tests/dsp/processors/test_get_multi_local_extrema.py
 tests/dsp/processors/test_histogram.py
 tests/flow/conftest.py
 tests/flow/test_data_loader.py
 tests/flow/test_filedb.py
+tests/flow/test_flow_utils.py
+tests/flow/configs/config.json
 tests/flow/configs/data-loader-config.json
 tests/flow/configs/filedb-config.json
+tests/flow/configs/nested/config.json
+tests/flow/configs/nested/data-loader-config-nested.json
 tests/functional/test_l200_dataproc.py
 tests/functional/test_teststand_dataproc.py
 tests/hit/test_build_hit.py
 tests/hit/configs/basic-hit-config.json
 tests/hit/configs/spms-hit-a-config.json
 tests/hit/configs/spms-hit-config.json
 tests/hit/configs/spms-hit-multi-config.json
 tests/integration/test_integration.py
 tests/lgdo/test_array.py
 tests/lgdo/test_arrayofequalsizedarrays.py
+tests/lgdo/test_encoded.py
 tests/lgdo/test_fixedsizearray.py
 tests/lgdo/test_lgdo_utils.py
 tests/lgdo/test_lh5_iterator.py
 tests/lgdo/test_lh5_store.py
 tests/lgdo/test_representations.py
 tests/lgdo/test_scalar.py
 tests/lgdo/test_struct.py
 tests/lgdo/test_table.py
 tests/lgdo/test_table_eval.py
 tests/lgdo/test_vectorofvectors.py
 tests/lgdo/test_waveform_table.py
+tests/lgdo/compression/conftest.py
+tests/lgdo/compression/test_compression.py
+tests/lgdo/compression/test_radware_sigcompress.py
+tests/lgdo/compression/test_str2wfcodec.py
+tests/lgdo/compression/test_uleb128_zigzag_diff.py
+tests/lgdo/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat
+tests/lgdo/compression/sigcompress/special-wf-clipped.dat
 tests/math/test_fwhm.py
 tests/pargen/test_ecal.py
 tests/pargen/test_energy_optimization.py
 tests/raw/test_build_raw.py
 tests/raw/test_cli.py
+tests/raw/test_daq_to_raw.py
 tests/raw/test_raw_buffer.py
 tests/raw/buffer_processor/test_buffer_processor.py
 tests/raw/buffer_processor/test_lh5_buffer_processor.py
 tests/raw/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json
 tests/raw/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json
 tests/raw/buffer_processor/test_buffer_processor_configs/raw_out_spec_no_proc.json
+tests/raw/compass/conftest.py
+tests/raw/compass/test_compass_event_decoder.py
+tests/raw/compass/test_compass_header_decoder.py
+tests/raw/compass/test_compass_streamer.py
 tests/raw/configs/fc-out-spec.json
 tests/raw/configs/orca-out-spec-cli.json
 tests/raw/configs/orca-out-spec.json
 tests/raw/fc/conftest.py
 tests/raw/fc/test_fc_config_decoder.py
 tests/raw/fc/test_fc_event_decoder.py
 tests/raw/fc/test_fc_status_decoder.py
```

### Comparing `pygama-1.2.0/tests/conftest.py` & `pygama-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/dsp/configs/icpc-dsp-config.json` & `pygama-1.3.0/tests/dsp/configs/icpc-dsp-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/dsp/configs/numpy-parsing.json` & `pygama-1.3.0/tests/dsp/configs/numpy-parsing.json`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/dsp/configs/sipm-dplms-config.json` & `pygama-1.3.0/tests/dsp/configs/sipm-dplms-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/dsp/configs/sipm-dsp-config.json` & `pygama-1.3.0/tests/dsp/configs/sipm-dsp-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/dsp/conftest.py` & `pygama-1.3.0/tests/dsp/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
         n_rows=10,
     )
     return obj
 
 
 @pytest.fixture(scope="session")
 def spms_raw_tbl(lgnd_test_data):
-
     out_file = "/tmp/L200-comm-20211130-phy-spms.lh5"
     out_spec = {
         "FCEventDecoder": {
             "raw": {"key_list": [[0, 6]], "out_stream": f"{out_file}:/spms"}
         }
     }
```

### Comparing `pygama-1.2.0/tests/dsp/processors/dplms_noise_mat.dat` & `pygama-1.3.0/tests/dsp/processors/dplms_noise_mat.dat`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/dsp/processors/test_dplms.py` & `pygama-1.3.0/tests/dsp/processors/test_dplms.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,44 +4,43 @@
 import pytest
 
 from pygama.dsp.errors import DSPFatal
 from pygama.dsp.processors import dplms
 
 
 def test_dplms(compare_numba_vs_python):
-
     with open(Path(__file__).parent / "dplms_noise_mat.dat") as f:
         nmat = [[float(num) for num in line.split(" ")] for line in f]
 
     length = 50
     len_wf = 100
     ref = np.zeros(len_wf)
     ref[int(len_wf / 2 - 1) : int(len_wf / 2)] = 1
 
     # ensure the DSPFatal is raised for a negative length
     with pytest.raises(DSPFatal):
-        dplms(nmat, ref, -1, 1, 1, 1, 1)
+        dplms(-1, nmat, ref, 1, 1, 1, 1, [])
 
     # ensure the DSPFatal is raised for length not equal to noise matrix shape
     with pytest.raises(DSPFatal):
-        dplms(nmat, ref, 10, 1, 1, 1, 1)
+        dplms(10, nmat, ref, 1, 1, 1, 1, [])
 
     # ensure the DSPFatal is raised for negative coefficients
     with pytest.raises(DSPFatal):
-        dplms(nmat, ref, length, -1, 1, 1, 1)
+        dplms(length, nmat, ref, -1, 1, 1, 1, [])
     with pytest.raises(DSPFatal):
-        dplms(nmat, ref, length, 1, -1, 1, 1)
+        dplms(length, nmat, ref, 1, -1, 1, 1, [])
     with pytest.raises(DSPFatal):
-        dplms(nmat, ref, length, 1, 1, -1, 1)
+        dplms(length, nmat, ref, 1, 1, -1, 1, [])
     with pytest.raises(DSPFatal):
-        dplms(nmat, ref, length, 1, 1, 1, -1)
+        dplms(length, nmat, ref, 1, 1, 1, -1, [])
     with pytest.raises(DSPFatal):
-        dplms(nmat, ref, length, 1, 1, 1, 2)
+        dplms(length, nmat, ref, 1, 1, 1, 2, [])
 
-    dplms_func = dplms(nmat, ref, length, 1, 1, 1, 1)
+    dplms_func = dplms(length, nmat, ref, 1, 1, 1, 1, [])
 
     # ensure to have a valid output
     w_in = np.ones(len_wf)
     w_out = np.empty(len_wf - length + 1)
 
     assert np.all(compare_numba_vs_python(dplms_func, w_in, w_out))
```

### Comparing `pygama-1.2.0/tests/dsp/processors/test_dwt.py` & `pygama-1.3.0/tests/dsp/processors/test_dwt.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/dsp/processors/test_fixed_time_pickoff.py` & `pygama-1.3.0/tests/dsp/processors/test_fixed_time_pickoff.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/dsp/processors/test_get_multi_local_extrema.py` & `pygama-1.3.0/tests/dsp/processors/test_get_multi_local_extrema.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 #           1         2         3
 wf = np.array([0, 0, 1, 2, 3, 4, 5, 4, 3, 4, 5, 6, 7, 8, 9, 10,
                9, 8, 7, 6, 5, 4, 3, 4, 5, 4, 3, 2, 1, 0, 0])  # fmt: skip
 
 
 # delta_min=delta_max tests (all searches should behave identical)
 
+
 # L->R
 def test_get_multi_local_extrema_ltor(compare_numba_vs_python):
     max_out = np.zeros(3)
     max_out[:] = np.nan
     min_out = np.zeros(3)
     min_out[:] = np.nan
     n_min_out = np.zeros(1)
@@ -137,14 +138,15 @@
     assert np.array_equal(max_out, np.array([15, np.nan, np.nan]), equal_nan=True)
     assert np.array_equal(min_out, np.array([np.nan, np.nan, np.nan]), equal_nan=True)
     assert n_max_out[0] == 1
 
 
 # delta_min != delta_max (result should be search direction dependent)
 
+
 # L->R
 def test_get_multi_local_extrema_ltor_asym(compare_numba_vs_python):
     max_out = np.zeros(3)
     max_out[:] = np.nan
     min_out = np.zeros(3)
     min_out[:] = np.nan
     n_min_out = np.zeros(1)
@@ -284,14 +286,15 @@
     assert np.array_equal(min_out, np.array([8, 22, np.nan]), equal_nan=True)
     assert n_max_out[0] == 1
     assert n_min_out[0] == 2
 
 
 # And now test if everything works well when vectorized
 
+
 # return nan tests
 def test_get_multi_local_extrema_return_on_nan(compare_numba_vs_python):
     wf = np.ones(20)
     max_out = np.zeros(3)
     max_out[:] = np.nan
     min_out = np.zeros(3)
     min_out[:] = np.nan
```

### Comparing `pygama-1.2.0/tests/dsp/processors/test_histogram.py` & `pygama-1.3.0/tests/dsp/processors/test_histogram.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/dsp/test_build_dsp.py` & `pygama-1.3.0/tests/dsp/test_build_dsp.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
             "/tmp/LDQTA_r117_20200110T105115Z_cal_geds_dsp.lh5",
             dsp_config=f"{config_dir}/icpc-dsp-config.json",
             write_mode="r",
         )
 
 
 def test_build_dsp_spms_channelwise(dsp_test_file_spm):
-
     assert ls(dsp_test_file_spm) == ["ch0", "ch1", "ch2", "dsp_info"]
     assert ls(dsp_test_file_spm, "ch0/") == ["ch0/dsp"]
     assert ls(dsp_test_file_spm, "ch0/dsp/") == [
         "ch0/dsp/energies",
         "ch0/dsp/trigger_pos",
     ]
```

### Comparing `pygama-1.2.0/tests/dsp/test_list_parsing.py` & `pygama-1.3.0/tests/dsp/test_list_parsing.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/dsp/test_numpy_constants_parsing.py` & `pygama-1.3.0/tests/dsp/test_numpy_constants_parsing.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/dsp/test_processing_chain.py` & `pygama-1.3.0/tests/dsp/test_processing_chain.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/flow/configs/filedb-config.json` & `pygama-1.3.0/tests/flow/configs/filedb-config.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'data_dir'": "'lh5/prod-ref-l200/generated/tier'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_dir": "generated/tier",
+    "data_dir": "lh5/prod-ref-l200/generated/tier",
     "file_format": {
         "dsp": "/{type}/{period}/{run}/{exp}-{period}-{run}-{type}-{timestamp}-tier_dsp.lh5",
         "evt": "/{type}/{period}/{run}/{exp}-{period}-{run}-{type}-{timestamp}-tier_evt.lh5",
         "hit": "/{type}/{period}/{run}/{exp}-{period}-{run}-{type}-{timestamp}-tier_hit.lh5",
         "raw": "/{type}/{period}/{run}/{exp}-{period}-{run}-{type}-{timestamp}-tier_raw.lh5",
         "tcm": "/{type}/{period}/{run}/{exp}-{period}-{run}-{type}-{timestamp}-tier_tcm.lh5"
     },
```

### Comparing `pygama-1.2.0/tests/flow/test_filedb.py` & `pygama-1.3.0/tests/flow/test_filedb.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,28 @@
-from datetime import datetime, timezone
+import json
+from pathlib import Path
 
 import pytest
 from pandas.testing import assert_frame_equal
 
 from pygama.flow import FileDB
-from pygama.flow.file_db import to_datetime, to_unixtime
+
+config_dir = Path(__file__).parent / "configs"
+
+
+def test_init_partial(lgnd_test_data, test_filedb_full):
+    with open(config_dir / "filedb-config.json") as f:
+        config = json.load(f)
+
+    config["data_dir"] = lgnd_test_data.get_path("lh5/prod-ref-l200/generated/tier")
+    fdb = FileDB(config, scan=False)
+    fdb.scan_files("cal/p01/r014")
+    fdb.scan_tables_columns()
+
+    assert fdb.df.equals(test_filedb_full.df)
 
 
 def test_filedb_basics(test_filedb):
     db = test_filedb
 
     assert list(db.df.keys()) == [
         "exp",
@@ -65,17 +79,16 @@
             15728,
             0,
             int("0b11110", 2),
         ],
     ]
 
 
-def test_scan_tables_columns(test_filedb):
-    db = test_filedb
-    db.scan_tables_columns()
+def test_scan_tables_columns(test_filedb_full):
+    db = test_filedb_full
 
     assert list(db.df.keys()) == [
         "exp",
         "period",
         "run",
         "timestamp",
         "type",
@@ -140,26 +153,26 @@
             "bl_std",
         ],
         ["hit_par1", "hit_par2"],
         ["array_id", "array_idx", "cumulative_length"],
     ]
 
 
-def test_serialization(test_filedb):
-    db = test_filedb
+def test_serialization(test_filedb_full):
+    db = test_filedb_full
     db.to_disk("/tmp/filedb.lh5", wo_mode="of")
 
     with pytest.raises(RuntimeError):
         db.to_disk("/tmp/filedb.lh5")
 
     db2 = FileDB("/tmp/filedb.lh5")
     assert_frame_equal(db.df, db2.df)
 
 
-def test_key_to_datetime():
-    assert to_datetime("20220716T105236Z") == datetime(
-        2022, 7, 16, 10, 52, 36, tzinfo=timezone.utc
-    )
-
-
-def test_key_to_unixtime():
-    assert to_unixtime("20220716T105236Z") == 1657968756
+def test_get_table_columns(test_filedb_full):
+    db = test_filedb_full
+    cols = db.get_table_columns(1, "dsp")
+    assert cols == ["bl_mean", "bl_std"]
+    with pytest.raises(KeyError):
+        db.get_table_columns(1, "blah")
+    with pytest.raises(ValueError):
+        db.get_table_columns(9999, "raw")
```

### Comparing `pygama-1.2.0/tests/hit/configs/spms-hit-a-config.json` & `pygama-1.3.0/tests/hit/configs/spms-hit-a-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/hit/test_build_hit.py` & `pygama-1.3.0/tests/hit/test_build_hit.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/lgdo/test_array.py` & `pygama-1.3.0/tests/lgdo/test_array.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 import numpy as np
 
-import pygama.lgdo as lgdo
+from pygama import lgdo
+from pygama.lgdo import Array
 
 
 def test_datatype_name():
-    array = lgdo.Array()
+    array = Array()
     assert array.datatype_name() == "array"
 
 
 def test_form_datatype():
-    array = lgdo.Array(shape=(12, 34))
+    array = Array(shape=(12, 34))
     assert array.form_datatype() == "array<2>{real}"
 
 
 def test_init():
     attrs = {"attr1": 1}
-    array = lgdo.Array(shape=(3,), dtype=np.float32, fill_val=42, attrs=attrs)
+    array = Array(shape=(3,), dtype=np.float32, fill_val=42, attrs=attrs)
     assert (array.nda == np.full((3,), 42, np.float32)).all()
     assert array.attrs == attrs | {"datatype": "array<1>{real}"}
 
 
 def test_resize():
-    array = lgdo.Array(nda=np.array([1, 2, 3, 4]))
+    array = Array(nda=np.array([1, 2, 3, 4]))
     array.resize(3)
     assert (array.nda == np.array([1, 2, 3])).all()
+
+
+def test_copy():
+    a1 = Array(np.array([1, 2, 3, 4]))
+    a2 = lgdo.copy(a1)
+    assert a1 == a2
+
+
+def test_insert():
+    a = Array(np.array([1, 2, 3, 4]))
+    a.insert(2, [-1, -1])
+    assert a == Array([1, 2, -1, -1, 3, 4])
```

### Comparing `pygama-1.2.0/tests/lgdo/test_arrayofequalsizedarrays.py` & `pygama-1.3.0/tests/lgdo/test_fixedsizearray.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 import numpy as np
 
 import pygama.lgdo as lgdo
 
 
 def test_datatype_name():
-    aoesa = lgdo.ArrayOfEqualSizedArrays()
-    assert aoesa.datatype_name() == "array_of_equalsized_arrays"
+    array = lgdo.FixedSizeArray()
+    assert array.datatype_name() == "fixedsize_array"
 
 
 def test_form_datatype():
-    aoesa = lgdo.ArrayOfEqualSizedArrays(dims=(2, 3))
-    assert aoesa.form_datatype() == "array_of_equalsized_arrays<2,3>{real}"
+    array = lgdo.FixedSizeArray()
+    assert array.form_datatype() == "fixedsize_array<0>{real}"
 
 
 def test_init():
     attrs = {"attr1": 1}
-    aoesa = lgdo.ArrayOfEqualSizedArrays(
-        dims=(2, 3), dtype=np.float32, fill_val=42, attrs=attrs
-    )
-    assert aoesa.dims == (2, 3)
-    assert (aoesa.nda == np.full((2, 3), 42, np.float32)).all()
-    assert aoesa.attrs == attrs | {"datatype": "array_of_equalsized_arrays<2,3>{real}"}
+    array = lgdo.FixedSizeArray(shape=(3,), dtype=np.float32, fill_val=42, attrs=attrs)
+    assert (array.nda == np.full((3,), 42, np.float32)).all()
+    assert array.attrs == attrs | {"datatype": "fixedsize_array<1>{real}"}
```

### Comparing `pygama-1.2.0/tests/lgdo/test_lgdo_utils.py` & `pygama-1.3.0/tests/lgdo/test_lgdo_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import numpy as np
 import pytest
 
 import pygama.lgdo.lgdo_utils as lgdo_utils
 
 
 def test_get_element_type():
-
     objs = [
         ("hi", "string"),
         (True, "bool"),
         (np.void(0), "blob"),
         (int(0), "real"),
         (np.uint8(0), "real"),
         (float(0), "real"),
@@ -22,15 +21,14 @@
 
     for obj, name in objs:
         get_name = lgdo_utils.get_element_type(obj)
         assert get_name == name
 
 
 def test_parse_datatype():
-
     datatypes = [
         ("real", ("scalar", None, "real")),
         ("array<1>{bool}", ("array", (1,), "bool")),
         ("fixedsizearray<2>{real}", ("fixedsizearray", (2,), "real")),
         (
             "arrayofequalsizedarrays<3,4>{complex}",
             ("arrayofequalsizedarrays", (3, 4), "complex"),
@@ -44,14 +42,29 @@
     ]
 
     for string, dt_tuple in datatypes:
         pd_dt_tuple = lgdo_utils.parse_datatype(string)
         assert pd_dt_tuple == dt_tuple
 
 
+def test_expand_vars():
+    # Check env variable expansion
+    os.environ["PYGAMATESTBASEDIR"] = "a_random_string"
+    assert lgdo_utils.expand_vars("$PYGAMATESTBASEDIR/blah") == "a_random_string/blah"
+
+    # Check user variable expansion
+    assert (
+        lgdo_utils.expand_vars(
+            "$PYGAMATESTBASEDIR2/blah",
+            substitute={"PYGAMATESTBASEDIR2": "a_random_string"},
+        )
+        == "a_random_string/blah"
+    )
+
+
 def test_expand_path(lgnd_test_data):
     files = [
         lgnd_test_data.get_path(
             "lh5/prod-ref-l200/generated/tier/dsp/cal/p01/r014/l60-p01-r014-cal-20220716T104550Z-tier_dsp.lh5"
         ),
         lgnd_test_data.get_path(
             "lh5/prod-ref-l200/generated/tier/dsp/cal/p01/r014/l60-p01-r014-cal-20220716T105236Z-tier_dsp.lh5"
@@ -66,8 +79,10 @@
         lgdo_utils.expand_path(f"{base_dir}/not_a_real_file.lh5")
 
     # Should fail if multiple files found
     with pytest.raises(FileNotFoundError):
         lgdo_utils.expand_path(f"{base_dir}/*.lh5")
 
     # Check if it finds a list of files correctly
-    assert sorted(lgdo_utils.expand_path(f"{base_dir}/*.lh5", True)) == sorted(files)
+    assert sorted(lgdo_utils.expand_path(f"{base_dir}/*.lh5", list=True)) == sorted(
+        files
+    )
```

### Comparing `pygama-1.2.0/tests/lgdo/test_lh5_iterator.py` & `pygama-1.3.0/tests/lgdo/test_lh5_iterator.py`

 * *Files 26% similar despite different names*

```diff
@@ -68,7 +68,51 @@
         ],
         buffer_len=5,
     )
 
     lh5_obj, n_rows = lh5_it.read(0)
     assert isinstance(lh5_obj, lgdo.WaveformTable)
     assert len(lh5_obj) == 5
+
+
+@pytest.fixture(scope="module")
+def more_lgnd_files(lgnd_test_data):
+    return [
+        [
+            lgnd_test_data.get_path(
+                "lh5/prod-ref-l200/generated/tier/raw/cal/p01/r014/l60-p01-r014-cal-20220716T104550Z-tier_raw.lh5"
+            ),
+            lgnd_test_data.get_path(
+                "lh5/prod-ref-l200/generated/tier/raw/cal/p01/r014/l60-p01-r014-cal-20220716T105236Z-tier_raw.lh5"
+            ),
+        ],
+        [
+            lgnd_test_data.get_path(
+                "lh5/prod-ref-l200/generated/tier/hit/cal/p01/r014/l60-p01-r014-cal-20220716T104550Z-tier_hit.lh5"
+            ),
+            lgnd_test_data.get_path(
+                "lh5/prod-ref-l200/generated/tier/hit/cal/p01/r014/l60-p01-r014-cal-20220716T105236Z-tier_hit.lh5"
+            ),
+        ],
+    ]
+
+
+def test_friend(more_lgnd_files):
+    lh5_raw_it = LH5Iterator(
+        more_lgnd_files[0],
+        "ch000/raw",
+        field_mask=["waveform", "baseline"],
+        buffer_len=5,
+    )
+    lh5_it = LH5Iterator(
+        more_lgnd_files[1],
+        "ch000/hit",
+        field_mask=["hit_par1"],
+        buffer_len=5,
+        friend=lh5_raw_it,
+    )
+
+    lh5_obj, n_rows = lh5_it.read(0)
+
+    assert n_rows == 2
+    assert isinstance(lh5_obj, lgdo.Table)
+    assert set(lh5_obj.keys()) == {"waveform", "baseline", "hit_par1"}
```

### Comparing `pygama-1.2.0/tests/lgdo/test_struct.py` & `pygama-1.3.0/tests/lgdo/test_struct.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/lgdo/test_table.py` & `pygama-1.3.0/tests/lgdo/test_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,27 +81,36 @@
     assert list(tbl1.keys()) == ["a", "b", "c", "d"]
 
     tbl2.join(tbl1, cols=("a"))
     assert list(tbl2.keys()) == ["c", "d", "a"]
 
 
 def test_get_dataframe():
-    tbl = Table(3)
+    tbl = Table(4)
     tbl.add_column("a", lgdo.Array(np.array([1, 2, 3])))
     tbl.add_column("b", lgdo.Array(np.array([[0, 1, 2], [3, 4, 5], [6, 7, 8]])))
     tbl.add_column(
         "c",
         lgdo.VectorOfVectors(
             flattened_data=lgdo.Array(np.array([0, 1, 2, 3, 4, 5, 6])),
             cumulative_length=lgdo.Array(np.array([3, 4, 7])),
         ),
     )
+    tbl.add_column(
+        "d",
+        lgdo.Table(
+            col_dict={
+                "a": lgdo.Array(np.array([2, 4, 6, 8])),
+                "b": lgdo.Array(np.array([[1, 1], [2, 4], [3, 9], [4, 16]])),
+            }
+        ),
+    )
     df = tbl.get_dataframe()
     assert isinstance(df, pd.DataFrame)
-    assert list(df.keys()) == ["a", "b", "c"]
+    assert list(df.keys()) == ["a", "b", "c", "d_a", "d_b"]
 
 
 def test_remove_column():
     col_dict = {
         "a": lgdo.Array(nda=np.array([1, 2, 3, 4])),
         "b": lgdo.Array(nda=np.array([5, 6, 7, 8])),
         "c": lgdo.Array(nda=np.array([9, 10, 11, 12])),
```

### Comparing `pygama-1.2.0/tests/lgdo/test_table_eval.py` & `pygama-1.3.0/tests/lgdo/test_table_eval.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/lgdo/test_waveform_table.py` & `pygama-1.3.0/tests/lgdo/test_waveform_table.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,21 +42,43 @@
     )
     assert (wft.t0.nda == np.zeros(10)).all()
     assert (wft.dt.nda == np.full(10, fill_value=1)).all()
     assert isinstance(wft.values, lgdo.VectorOfVectors)
     assert len(wft.values) == 10
 
     wft = WaveformTable(
+        values=lgdo.VectorOfEncodedVectors(
+            encoded_data=lgdo.VectorOfVectors(shape_guess=(10, 1000), dtype=np.ubyte),
+            decoded_size=lgdo.Array(shape=10, fill_val=6),
+        )
+    )
+    assert (wft.t0.nda == np.zeros(10)).all()
+    assert (wft.dt.nda == np.full(10, fill_value=1)).all()
+    assert isinstance(wft.values, lgdo.VectorOfEncodedVectors)
+    assert len(wft.values) == 10
+
+    wft = WaveformTable(
         t0=[1, 1, 1], dt=[2, 2, 2], values=lgdo.ArrayOfEqualSizedArrays(shape=(3, 1000))
     )
     assert (wft.t0.nda == np.full(3, fill_value=1)).all()
     assert (wft.dt.nda == np.full(3, fill_value=2)).all()
     assert isinstance(wft.values, lgdo.ArrayOfEqualSizedArrays)
     assert wft.values.nda.shape == (3, 1000)
 
+    wft = WaveformTable(
+        values=lgdo.ArrayOfEncodedEqualSizedArrays(
+            encoded_data=lgdo.VectorOfVectors(shape_guess=(10, 1000), dtype=np.ubyte),
+            decoded_size=10,
+        )
+    )
+    assert (wft.t0.nda == np.zeros(10)).all()
+    assert (wft.dt.nda == np.full(10, fill_value=1)).all()
+    assert isinstance(wft.values, lgdo.ArrayOfEncodedEqualSizedArrays)
+    assert len(wft.values) == 10
+
     wft = WaveformTable(t0=[1, 1, 1], dt=[2, 2, 2], wf_len=1000)
     assert (wft.t0.nda == np.full(3, fill_value=1)).all()
     assert (wft.dt.nda == np.full(3, fill_value=2)).all()
     assert isinstance(wft.values, lgdo.ArrayOfEqualSizedArrays)
     assert wft.values.nda.shape == (3, 1000)
 
     wft = WaveformTable(t0=[1, 1, 1], dt=[2, 2, 2], wf_len=1000, dtype=np.float32)
```

### Comparing `pygama-1.2.0/tests/math/test_fwhm.py` & `pygama-1.3.0/tests/math/test_fwhm.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/raw/buffer_processor/test_buffer_processor.py` & `pygama-1.3.0/tests/raw/buffer_processor/test_buffer_processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,22 +3,26 @@
 import sys
 from pathlib import Path
 
 import numpy as np
 
 import pygama.lgdo as lgdo
 from pygama.dsp import build_processing_chain as bpc
+from pygama.lgdo.compression import RadwareSigcompress, ULEB128ZigZagDiff
 from pygama.raw.build_raw import build_raw
+from pygama.raw.fc.fc_event_decoder import fc_decoded_values
+
+# skip compression in build_raw
+fc_decoded_values["waveform"].pop("compression", None)
 
 config_dir = Path(__file__).parent / "test_buffer_processor_configs"
 
 
 # check that packet indexes match in verification test
 def test_buffer_processor_packet_ids(lgnd_test_data):
-
     # Set up I/O files, including config
     daq_file = lgnd_test_data.get_path("orca/fc/L200-comm-20220519-phy-geds.orca")
     proc_out_spec = f"{config_dir}/buffer_processor_config.json"
     raw_out_spec = f"{config_dir}/raw_out_spec_no_proc.json"
 
     processed_file = "/tmp/L200-comm-20220519-phy-geds_proc.lh5"
 
@@ -42,15 +46,14 @@
     )
     raw_wfs, _ = sto.read_object(str(raw_group) + "/waveform/values", raw_file)
     assert processed_presummed_wfs.nda[0][0] == np.sum(raw_wfs.nda[0][:4])
 
 
 # check that packet indexes match in verification test
 def test_buffer_processor_waveform_lengths(lgnd_test_data):
-
     # Set up I/O files, including config
     daq_file = lgnd_test_data.get_path("fcio/L200-comm-20211130-phy-spms.fcio")
     processed_file = daq_file.replace(
         "L200-comm-20211130-phy-spms.fcio", "L200-comm-20211130-phy-spms_proc.lh5"
     )
     raw_file = daq_file.replace(
         "L200-comm-20211130-phy-spms.fcio", "L200-comm-20211130-phy-spms.lh5"
@@ -129,34 +132,36 @@
     # This needs to be overwritten with the correct windowing values set in buffer_processor.py
     window_start_index = window_config[1]
     window_end_index = window_config[2]
 
     sto = lgdo.LH5Store()
 
     for raw_group in lh5_tables:
-
         raw_packet_waveform_values = sto.read_object(
             str(raw_group) + "/waveform/values", raw_file
         )
         presummed_packet_waveform_values = sto.read_object(
             str(raw_group) + "/presummed_waveform/values", processed_file
         )
         windowed_packet_waveform_values = sto.read_object(
             str(raw_group) + "/windowed_waveform/values", processed_file
         )
 
         # Check that the lengths of the waveforms match what we expect
         assert len(raw_packet_waveform_values[0].nda[0]) == presum_rate * len(
             presummed_packet_waveform_values[0].nda[0]
         )
-        assert isinstance(presummed_packet_waveform_values[0].nda[0][0], np.uint32)
+        assert presummed_packet_waveform_values[0].nda.dtype == np.uint32
         assert len(raw_packet_waveform_values[0].nda[0]) == len(
             windowed_packet_waveform_values[0].nda[0]
         ) + np.abs(window_start_index) + np.abs(window_end_index)
-        assert isinstance(windowed_packet_waveform_values[0].nda[0][0], np.uint16)
+        assert (
+            windowed_packet_waveform_values[0].dtype
+            == raw_packet_waveform_values[0].dtype
+        )
 
         raw_packet_waveform_t0s, _ = sto.read_object(
             str(raw_group) + "/waveform/t0", raw_file
         )
         raw_packet_waveform_dts, _ = sto.read_object(
             str(raw_group) + "/waveform/dt", raw_file
         )
@@ -278,15 +283,14 @@
 
     # Make sure we are taking up less space than a file that has two copies of the waveform table in it
     assert os.path.getsize(processed_file) < os.path.getsize(raw_file) + wf_size
 
 
 # check that packet indexes match in verification test on file that has both spms and geds
 def test_buffer_processor_separate_name_tables(lgnd_test_data):
-
     # Set up I/O files, including config
     daq_file = lgnd_test_data.get_path("fcio/L200-comm-20211130-phy-spms.fcio")
     processed_file = daq_file.replace(
         "L200-comm-20211130-phy-spms.fcio", "L200-comm-fake-geds-and-spms_proc.lh5"
     )
     raw_file = daq_file.replace(
         "L200-comm-20211130-phy-spms.fcio", "L200-comm-fake-geds-and-spms.lh5"
@@ -391,15 +395,14 @@
             del lh5_tables[i]
 
     jsonfile = proc_spec
 
     sto = lgdo.LH5Store()
 
     for raw_group in lh5_tables:
-
         # First, check the packet ids
         raw_packet_ids, _ = sto.read_object(str(raw_group) + "/packet_id", raw_file)
         processed_packet_ids, _ = sto.read_object(
             str(raw_group) + "/packet_id", processed_file
         )
 
         assert np.array_equal(raw_packet_ids.nda, processed_packet_ids.nda)
@@ -427,19 +430,22 @@
             str(raw_group) + "/windowed_waveform/values", processed_file
         )
 
         # Check that the lengths of the waveforms match what we expect
         assert len(raw_packet_waveform_values[0].nda[0]) == presum_rate * len(
             presummed_packet_waveform_values[0].nda[0]
         )
-        assert isinstance(presummed_packet_waveform_values[0].nda[0][0], np.uint32)
+        assert presummed_packet_waveform_values[0].dtype == np.uint32
         assert len(raw_packet_waveform_values[0].nda[0]) == len(
             windowed_packet_waveform_values[0].nda[0]
         ) + np.abs(window_start_index) + np.abs(window_end_index)
-        assert isinstance(windowed_packet_waveform_values[0].nda[0][0], np.uint16)
+        assert (
+            windowed_packet_waveform_values[0].dtype
+            == raw_packet_waveform_values[0].dtype
+        )
 
         raw_packet_waveform_t0s, _ = sto.read_object(
             str(raw_group) + "/waveform/t0", raw_file
         )
         raw_packet_waveform_dts, _ = sto.read_object(
             str(raw_group) + "/waveform/dt", raw_file
         )
@@ -596,15 +602,14 @@
             del lh5_tables[i]
 
     jsonfile = proc_spec
 
     sto = lgdo.LH5Store()
 
     for raw_group in lh5_tables:
-
         # First, check the packet ids
         raw_packet_ids, _ = sto.read_object(str(raw_group) + "/packet_id", raw_file)
         processed_packet_ids, _ = sto.read_object(
             str(raw_group) + "/packet_id", processed_file
         )
 
         assert np.array_equal(raw_packet_ids.nda, processed_packet_ids.nda)
@@ -655,15 +660,18 @@
         # Check that the lengths of the waveforms match what we expect
         assert len(raw_packet_waveform_values[0].nda[0]) == presum_rate * len(
             presummed_packet_waveform_values[0].nda[0]
         )
         assert len(raw_packet_waveform_values[0].nda[0]) == len(
             windowed_packet_waveform_values[0].nda[0]
         ) + np.abs(window_start_index) + np.abs(window_end_index)
-        assert isinstance(windowed_packet_waveform_values[0].nda[0][0], np.uint16)
+        assert (
+            windowed_packet_waveform_values[0].dtype
+            == raw_packet_waveform_values[0].dtype
+        )
 
         raw_packet_waveform_t0s, _ = sto.read_object(
             str(raw_group) + "/waveform/t0", raw_file
         )
         raw_packet_waveform_dts, _ = sto.read_object(
             str(raw_group) + "/waveform/dt", raw_file
         )
@@ -696,20 +704,18 @@
         assert raw_packet_waveform_t0s.nda[0] == presummed_packet_waveform_t0s.nda[0]
         assert (
             presummed_packet_waveform_t0s.attrs["units"]
             == raw_packet_waveform_t0s.attrs["units"]
         )
 
         if pass_flag:
-
             presummed_packet_waveform_dts, _ = sto.read_object(
                 str(raw_group) + "/waveform/dt", processed_file
             )
         else:
-
             presummed_packet_waveform_dts, _ = sto.read_object(
                 str(raw_group) + "/presummed_waveform/dt", processed_file
             )
 
             # Check that the presum_rate is correctly identified
             presum_rate_from_file, _ = sto.read_object(
                 str(raw_group) + "/presum_rate", processed_file
@@ -735,34 +741,33 @@
 
             proc_sat_hi, _ = sto.read_object(
                 str(raw_group) + "/t_sat_hi", processed_file
             )
 
             assert np.array_equal(raw_sat_lo.nda, proc_sat_lo.nda)
             assert np.array_equal(raw_sat_hi.nda, proc_sat_hi.nda)
-            assert type(proc_sat_lo.nda[0]) == np.uint16
+            assert proc_sat_lo.dtype == np.uint16
 
 
 # check that packet indexes match in verification test
 def test_buffer_processor_multiple_keys(lgnd_test_data):
-
     # Set up I/O files, including config
     daq_file = lgnd_test_data.get_path("orca/fc/L200-comm-20220519-phy-geds.orca")
     processed_file = daq_file.replace(
         "L200-comm-20220519-phy-geds.orca",
         "L200-comm-20220519-phy-geds-key-test_proc.lh5",
     )
     raw_file = daq_file.replace(
         "L200-comm-20220519-phy-geds.orca", "L200-comm-20220519-phy-geds-key-test.lh5"
     )
 
     out_spec = {
         "ORFlashCamADCWaveformDecoder": {
             "ch{key}": {
-                "key_list": [0, 1],
+                "key_list": [1028800, 1028801],
                 "out_stream": processed_file + ":{name}",
                 "out_name": "raw",
                 "proc_spec": {
                     "window": ["waveform", 2000, -1000, "windowed_waveform"],
                     "dsp_config": {
                         "outputs": [
                             "presum_rate",
@@ -796,30 +801,30 @@
                         "t_sat_lo": "uint16",
                         "t_sat_hi": "uint16",
                         "presum_rate": "uint16",
                     },
                 },
             },
             "chan{key}": {
-                "key_list": [3, 4],
+                "key_list": [1028803, 1028804],
                 "out_stream": processed_file + ":{name}",
                 "out_name": "raw",
             },
         }
     }
 
     copy_out_spec = {
         "ORFlashCamADCWaveformDecoder": {
             "ch{key}": {
-                "key_list": [0, 1],
+                "key_list": [1028800, 1028801],
                 "out_stream": raw_file + ":{name}",
                 "out_name": "raw",
             },
             "chan{key}": {
-                "key_list": [3, 4],
+                "key_list": [1028803, 1028804],
                 "out_stream": raw_file + ":{name}",
                 "out_name": "raw",
             },
         }
     }
 
     raw_dsp_config = """
@@ -858,15 +863,14 @@
             del lh5_tables[i]
 
     jsonfile = proc_spec
 
     sto = lgdo.LH5Store()
 
     for raw_group in lh5_tables:
-
         # First, check the packet ids
         raw_packet_ids, _ = sto.read_object(str(raw_group) + "/packet_id", raw_file)
         processed_packet_ids, _ = sto.read_object(
             str(raw_group) + "/packet_id", processed_file
         )
 
         assert np.array_equal(raw_packet_ids.nda, processed_packet_ids.nda)
@@ -920,19 +924,22 @@
             len(raw_packet_waveform_values[0].nda[0])
             // len(presummed_packet_waveform_values[0].nda[0])
             == presum_rate
         )
         assert len(raw_packet_waveform_values[0].nda[0]) == len(
             windowed_packet_waveform_values[0].nda[0]
         ) + np.abs(window_start_index) + np.abs(window_end_index)
-        assert isinstance(windowed_packet_waveform_values[0].nda[0][0], np.uint16)
+        assert (
+            windowed_packet_waveform_values[0].dtype
+            == raw_packet_waveform_values[0].dtype
+        )
 
         # Check that the waveforms match
         # These are the channels that should be unprocessed
-        if group_name == "chan3" or group_name == "chan4":
+        if group_name == "chan1028803" or group_name == "chan1028804":
             raw_packet_waveform_values, _ = sto.read_object(
                 str(raw_group) + "/waveform/values", raw_file
             )
             windowed_packet_waveform_values, _ = sto.read_object(
                 str(raw_group) + "/waveform/values", processed_file
             )
             assert np.array_equal(
@@ -986,20 +993,18 @@
         assert raw_packet_waveform_t0s.nda[0] == presummed_packet_waveform_t0s.nda[0]
         assert (
             presummed_packet_waveform_t0s.attrs["units"]
             == raw_packet_waveform_t0s.attrs["units"]
         )
 
         if pass_flag:
-
             presummed_packet_waveform_dts, _ = sto.read_object(
                 str(raw_group) + "/waveform/dt", processed_file
             )
         else:
-
             presummed_packet_waveform_dts, _ = sto.read_object(
                 str(raw_group) + "/presummed_waveform/dt", processed_file
             )
 
             # Check that the presum_rate is correctly identified
             presum_rate_from_file, _ = sto.read_object(
                 str(raw_group) + "/presum_rate", processed_file
@@ -1025,15 +1030,15 @@
 
             proc_sat_hi, _ = sto.read_object(
                 str(raw_group) + "/t_sat_hi", processed_file
             )
 
             assert np.array_equal(raw_sat_lo.nda, proc_sat_lo.nda)
             assert np.array_equal(raw_sat_hi.nda, proc_sat_hi.nda)
-            assert type(proc_sat_lo.nda[0]) == np.uint16
+            assert proc_sat_lo.dtype == np.uint16
 
 
 def test_buffer_processor_all_pass(lgnd_test_data):
     # Set up I/O files, including config
     daq_file = lgnd_test_data.get_path("orca/fc/L200-comm-20220519-phy-geds.orca")
 
     raw_file = daq_file.replace(
@@ -1088,29 +1093,28 @@
                         proc_df = proc[obj].get_dataframe([str(sub_obj)])
 
             assert raw_df.equals(proc_df)
 
 
 # check that packet indexes match in verification test
 def test_buffer_processor_drop_waveform_small_buffer(lgnd_test_data):
-
     # Set up I/O files, including config
     daq_file = lgnd_test_data.get_path("orca/fc/L200-comm-20220519-phy-geds.orca")
     processed_file = daq_file.replace(
         "L200-comm-20220519-phy-geds.orca",
         "L200-comm-20220519-phy-geds-key-test_proc.lh5",
     )
     raw_file = daq_file.replace(
         "L200-comm-20220519-phy-geds.orca", "L200-comm-20220519-phy-geds-key-test.lh5"
     )
 
     out_spec = {
         "ORFlashCamADCWaveformDecoder": {
             "ch{key}": {
-                "key_list": [0, 1],
+                "key_list": [1028800, 1028801],
                 "out_stream": processed_file + ":{name}",
                 "out_name": "raw",
                 "proc_spec": {
                     "window": ["waveform", 2000, -1000, "windowed_waveform"],
                     "dsp_config": {
                         "outputs": [
                             "presum_rate",
@@ -1144,30 +1148,30 @@
                         "t_sat_lo": "uint16",
                         "t_sat_hi": "uint16",
                         "presum_rate": "uint16",
                     },
                 },
             },
             "chan{key}": {
-                "key_list": [3, 4],
+                "key_list": [1028803, 1028804],
                 "out_stream": processed_file + ":{name}",
                 "out_name": "raw",
             },
         }
     }
 
     copy_out_spec = {
         "ORFlashCamADCWaveformDecoder": {
             "ch{key}": {
-                "key_list": [0, 1],
+                "key_list": [1028800, 1028801],
                 "out_stream": raw_file + ":{name}",
                 "out_name": "raw",
             },
             "chan{key}": {
-                "key_list": [3, 4],
+                "key_list": [1028803, 1028804],
                 "out_stream": raw_file + ":{name}",
                 "out_name": "raw",
             },
         }
     }
 
     raw_dsp_config = """
@@ -1206,15 +1210,14 @@
             del lh5_tables[i]
 
     jsonfile = proc_spec
 
     sto = lgdo.LH5Store()
 
     for raw_group in lh5_tables:
-
         # First, check the packet ids
         raw_packet_ids, _ = sto.read_object(str(raw_group) + "/packet_id", raw_file)
         processed_packet_ids, _ = sto.read_object(
             str(raw_group) + "/packet_id", processed_file
         )
 
         assert np.array_equal(raw_packet_ids.nda, processed_packet_ids.nda)
@@ -1268,19 +1271,22 @@
             len(raw_packet_waveform_values[0].nda[0])
             // len(presummed_packet_waveform_values[0].nda[0])
             == presum_rate
         )
         assert len(raw_packet_waveform_values[0].nda[0]) == len(
             windowed_packet_waveform_values[0].nda[0]
         ) + np.abs(window_start_index) + np.abs(window_end_index)
-        assert isinstance(windowed_packet_waveform_values[0].nda[0][0], np.uint16)
+        assert (
+            windowed_packet_waveform_values[0].dtype
+            == raw_packet_waveform_values[0].dtype
+        )
 
         # Check that the waveforms match
         # These are the channels that should be unprocessed
-        if group_name == "chan3" or group_name == "chan4":
+        if group_name == "chan1028803" or group_name == "chan1028804":
             raw_packet_waveform_values, _ = sto.read_object(
                 str(raw_group) + "/waveform/values", raw_file
             )
             windowed_packet_waveform_values, _ = sto.read_object(
                 str(raw_group) + "/waveform/values", processed_file
             )
             assert np.array_equal(
@@ -1334,20 +1340,18 @@
         assert raw_packet_waveform_t0s.nda[0] == presummed_packet_waveform_t0s.nda[0]
         assert (
             presummed_packet_waveform_t0s.attrs["units"]
             == raw_packet_waveform_t0s.attrs["units"]
         )
 
         if pass_flag:
-
             presummed_packet_waveform_dts, _ = sto.read_object(
                 str(raw_group) + "/waveform/dt", processed_file
             )
         else:
-
             presummed_packet_waveform_dts, _ = sto.read_object(
                 str(raw_group) + "/presummed_waveform/dt", processed_file
             )
 
             # Check that the presum_rate is correctly identified
             presum_rate_from_file, _ = sto.read_object(
                 str(raw_group) + "/presum_rate", processed_file
@@ -1373,8 +1377,71 @@
 
             proc_sat_hi, _ = sto.read_object(
                 str(raw_group) + "/t_sat_hi", processed_file
             )
 
             assert np.array_equal(raw_sat_lo.nda, proc_sat_lo.nda)
             assert np.array_equal(raw_sat_hi.nda, proc_sat_hi.nda)
-            assert type(proc_sat_lo.nda[0]) == np.uint16
+            assert proc_sat_lo.dtype == np.uint16
+
+
+# check that packet indexes match in verification test
+def test_buffer_processor_compression_settings(lgnd_test_data):
+    # Set up I/O files, including config
+    daq_file = lgnd_test_data.get_path("fcio/L200-comm-20211130-phy-spms.fcio")
+    processed_file = "/tmp/L200-comm-20220519-phy-geds_proc_comp.lh5"
+
+    out_spec = {
+        "FCEventDecoder": {
+            "ch{key}": {
+                "key_list": [[0, 6]],
+                "out_stream": processed_file + ":{name}",
+                "out_name": "raw",
+                "proc_spec": {
+                    "window": ["waveform", 1000, -1000, "windowed_waveform"],
+                    "dsp_config": {
+                        "outputs": ["presum_rate", "presummed_waveform"],
+                        "processors": {
+                            "presum_rate, presummed_waveform": {
+                                "function": "presum",
+                                "module": "pygama.dsp.processors",
+                                "args": [
+                                    "waveform",
+                                    0,
+                                    "presum_rate",
+                                    "presummed_waveform(shape=len(waveform)/16, period=waveform.period*16, offset=waveform.offset)",
+                                ],
+                                "unit": "ADC",
+                            }
+                        },
+                    },
+                    "drop": ["waveform"],
+                    "dtype_conv": {
+                        "presummed_waveform/values": "uint32",
+                        "presum_rate": "uint16",
+                    },
+                    "compression": {
+                        "windowed_waveform/values": RadwareSigcompress(
+                            codec_shift=-32768
+                        ),
+                        "presummed_waveform/values": ULEB128ZigZagDiff(),
+                    },
+                },
+            }
+        }
+    }
+
+    build_raw(in_stream=daq_file, out_spec=out_spec, overwrite=True)
+
+    sto = lgdo.LH5Store()
+    presum_wf, _ = sto.read_object(
+        "/ch0/raw/presummed_waveform/values", processed_file, decompress=False
+    )
+    window_wf, _ = sto.read_object(
+        "/ch0/raw/windowed_waveform/values", processed_file, decompress=False
+    )
+
+    assert isinstance(presum_wf, lgdo.ArrayOfEncodedEqualSizedArrays)
+    assert isinstance(window_wf, lgdo.ArrayOfEncodedEqualSizedArrays)
+
+    assert presum_wf.attrs["codec"] == "uleb128_zigzag_diff"
+    assert window_wf.attrs["codec"] == "radware_sigcompress"
```

### Comparing `pygama-1.2.0/tests/raw/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json` & `pygama-1.3.0/tests/raw/buffer_processor/test_buffer_processor_configs/buffer_processor_config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/raw/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json` & `pygama-1.3.0/tests/raw/buffer_processor/test_buffer_processor_configs/lh5_buffer_processor_config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/raw/buffer_processor/test_lh5_buffer_processor.py` & `pygama-1.3.0/tests/raw/buffer_processor/test_lh5_buffer_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,24 @@
 
 import numpy as np
 
 import pygama.lgdo as lgdo
 from pygama.dsp import build_processing_chain as bpc
 from pygama.raw.buffer_processor.lh5_buffer_processor import lh5_buffer_processor
 from pygama.raw.build_raw import build_raw
+from pygama.raw.fc.fc_event_decoder import fc_decoded_values
+
+# skip compression in build_raw
+fc_decoded_values["waveform"].pop("compression", None)
 
 config_dir = Path(__file__).parent / "test_buffer_processor_configs"
 
 
 # check that packet indexes match in verification test
 def test_lh5_buffer_processor_packet_ids(lgnd_test_data):
-
     # Set up I/O files, including config
     daq_file = lgnd_test_data.get_path("orca/fc/L200-comm-20220519-phy-geds.orca")
     raw_file = "/tmp/L200-comm-20220519-phy-geds.lh5"
     proc_out_spec = f"{config_dir}/lh5_buffer_processor_config.json"
     raw_out_spec = f"{config_dir}/raw_out_spec_no_proc.json"
 
     processed_file = raw_file.replace(
@@ -46,15 +49,14 @@
     )
     raw_wfs, _ = sto.read_object(str(raw_group) + "/waveform/values", raw_file)
     assert processed_presummed_wfs.nda[0][0] == np.sum(raw_wfs.nda[0][:4])
 
 
 # check that packet indexes match in verification test
 def test_lh5_buffer_processor_waveform_lengths(lgnd_test_data):
-
     # Set up I/O files, including config
     daq_file = lgnd_test_data.get_path("fcio/L200-comm-20211130-phy-spms.fcio")
     raw_file = daq_file.replace(
         "L200-comm-20211130-phy-spms.fcio", "L200-comm-20211130-phy-spms.lh5"
     )
     processed_file = raw_file.replace(
         "L200-comm-20211130-phy-spms.lh5", "L200-comm-20211130-phy-spms_proc.lh5"
@@ -138,15 +140,14 @@
     # This needs to be overwritten with the correct windowing values set in buffer_processor.py
     window_start_index = jsonfile["ch0"]["window"][1]
     window_end_index = jsonfile["ch0"]["window"][2]
 
     sto = lgdo.LH5Store()
 
     for raw_group in lh5_tables:
-
         raw_packet_waveform_values = sto.read_object(
             str(raw_group) + "/waveform/values", raw_file
         )
         presummed_packet_waveform_values = sto.read_object(
             str(raw_group) + "/presummed_waveform/values", processed_file
         )
         windowed_packet_waveform_values = sto.read_object(
@@ -300,15 +301,14 @@
 
     # Make sure we are taking up less space than a file that has two copies of the waveform table in it
     assert os.path.getsize(processed_file) < os.path.getsize(raw_file) + wf_size
 
 
 # check that packet indexes match in verification test on file that has both spms and geds
 def test_lh5_buffer_processor_separate_name_tables(lgnd_test_data):
-
     # Set up I/O files, including config
     daq_file = lgnd_test_data.get_path("fcio/L200-comm-20211130-phy-spms.fcio")
     raw_file = daq_file.replace(
         "L200-comm-20211130-phy-spms.fcio", " L200-comm-fake-geds-and-spms.lh5"
     )
     processed_file = raw_file.replace(
         "L200-comm-fake-geds-and-spms.lh5", "L200-comm-fake-geds-and-spms_proc.lh5"
@@ -413,15 +413,14 @@
             proc_spec[key] = proc_out_spec["FCEventDecoder"][key].pop("proc_spec")
 
     jsonfile = proc_spec
 
     sto = lgdo.LH5Store()
 
     for raw_group in lh5_tables:
-
         # First, check the packet ids
         raw_packet_ids, _ = sto.read_object(str(raw_group) + "/packet_id", raw_file)
         processed_packet_ids, _ = sto.read_object(
             str(raw_group) + "/packet_id", processed_file
         )
 
         assert np.array_equal(raw_packet_ids.nda, processed_packet_ids.nda)
@@ -609,15 +608,14 @@
             proc_spec[key] = proc_out_spec["FCEventDecoder"][key].pop("proc_spec")
 
     jsonfile = proc_spec
 
     sto = lgdo.LH5Store()
 
     for raw_group in lh5_tables:
-
         # First, check the packet ids
         raw_packet_ids, _ = sto.read_object(str(raw_group) + "/packet_id", raw_file)
         processed_packet_ids, _ = sto.read_object(
             str(raw_group) + "/packet_id", processed_file
         )
 
         assert np.array_equal(raw_packet_ids.nda, processed_packet_ids.nda)
@@ -709,20 +707,18 @@
         assert raw_packet_waveform_t0s.nda[0] == presummed_packet_waveform_t0s.nda[0]
         assert (
             presummed_packet_waveform_t0s.attrs["units"]
             == raw_packet_waveform_t0s.attrs["units"]
         )
 
         if pass_flag:
-
             presummed_packet_waveform_dts, _ = sto.read_object(
                 str(raw_group) + "/waveform/dt", processed_file
             )
         else:
-
             presummed_packet_waveform_dts, _ = sto.read_object(
                 str(raw_group) + "/presummed_waveform/dt", processed_file
             )
         # Check that the dts match what we expect, with the correct units
         assert (
             raw_packet_waveform_dts.nda[0]
             == presummed_packet_waveform_dts.nda[0] / presum_rate
@@ -747,29 +743,28 @@
             assert np.array_equal(raw_sat_lo.nda, proc_sat_lo.nda)
             assert np.array_equal(raw_sat_hi.nda, proc_sat_hi.nda)
             assert type(proc_sat_lo.nda[0]) == np.uint16
 
 
 # check that packet indexes match in verification test
 def test_lh5_buffer_processor_multiple_keys(lgnd_test_data):
-
     # Set up I/O files, including config
     daq_file = lgnd_test_data.get_path("orca/fc/L200-comm-20220519-phy-geds.orca")
     processed_file = daq_file.replace(
         "L200-comm-20220519-phy-geds.orca",
         "L200-comm-20220519-phy-geds-key-test_proc.lh5",
     )
     raw_file = daq_file.replace(
         "L200-comm-20220519-phy-geds.orca", "L200-comm-20220519-phy-geds-key-test.lh5"
     )
 
     proc_out_spec = {
         "ORFlashCamADCWaveformDecoder": {
             "ch{key}": {
-                "key_list": [0, 1],
+                "key_list": [1028800, 1028801],
                 "out_stream": processed_file + ":{name}",
                 "out_name": "raw",
                 "proc_spec": {
                     "window": ["waveform", 2000, -1000, "windowed_waveform"],
                     "dsp_config": {
                         "outputs": [
                             "presum_rate",
@@ -802,30 +797,30 @@
                         "presummed_waveform/values": "uint32",
                         "t_sat_lo": "uint16",
                         "t_sat_hi": "uint16",
                     },
                 },
             },
             "chan{key}": {
-                "key_list": [3, 4],
+                "key_list": [1028803, 1028804],
                 "out_stream": processed_file + ":{name}",
                 "out_name": "raw",
             },
         }
     }
 
     raw_out_spec = {
         "ORFlashCamADCWaveformDecoder": {
             "ch{key}": {
-                "key_list": [0, 1],
+                "key_list": [1028800, 1028801],
                 "out_stream": raw_file + ":{name}",
                 "out_name": "raw",
             },
             "chan{key}": {
-                "key_list": [3, 4],
+                "key_list": [1028803, 1028804],
                 "out_stream": raw_file + ":{name}",
                 "out_name": "raw",
             },
         }
     }
 
     raw_dsp_config = """
@@ -866,15 +861,14 @@
             del lh5_tables[i]
 
     jsonfile = proc_spec
 
     sto = lgdo.LH5Store()
 
     for raw_group in lh5_tables:
-
         # First, check the packet ids
         raw_packet_ids, _ = sto.read_object(str(raw_group) + "/packet_id", raw_file)
         processed_packet_ids, _ = sto.read_object(
             str(raw_group) + "/packet_id", processed_file
         )
 
         assert np.array_equal(raw_packet_ids.nda, processed_packet_ids.nda)
@@ -932,15 +926,15 @@
         assert len(raw_packet_waveform_values[0].nda[0]) == len(
             windowed_packet_waveform_values[0].nda[0]
         ) + np.abs(window_start_index) + np.abs(window_end_index)
         assert isinstance(windowed_packet_waveform_values[0].nda[0][0], np.uint16)
 
         # Check that the waveforms match
         # These are the channels that should be unprocessed
-        if group_name == "chan3" or group_name == "chan4":
+        if group_name == "chan1028803" or group_name == "chan1028804":
             raw_packet_waveform_values, _ = sto.read_object(
                 str(raw_group) + "/waveform/values", raw_file
             )
             windowed_packet_waveform_values, _ = sto.read_object(
                 str(raw_group) + "/waveform/values", processed_file
             )
             assert np.array_equal(
@@ -994,20 +988,18 @@
         assert raw_packet_waveform_t0s.nda[0] == presummed_packet_waveform_t0s.nda[0]
         assert (
             presummed_packet_waveform_t0s.attrs["units"]
             == raw_packet_waveform_t0s.attrs["units"]
         )
 
         if pass_flag:
-
             presummed_packet_waveform_dts, _ = sto.read_object(
                 str(raw_group) + "/waveform/dt", processed_file
             )
         else:
-
             presummed_packet_waveform_dts, _ = sto.read_object(
                 str(raw_group) + "/presummed_waveform/dt", processed_file
             )
 
             # Check that the presum_rate is correctly identified
             presum_rate_from_file, _ = sto.read_object(
                 str(raw_group) + "/presum_rate", processed_file
```

### Comparing `pygama-1.2.0/tests/raw/fc/test_fc_config_decoder.py` & `pygama-1.3.0/tests/raw/fc/test_fc_config_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/raw/fc/test_fc_event_decoder.py` & `pygama-1.3.0/tests/raw/fc/test_fc_event_decoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,44 +17,47 @@
     # build raw buffer for each channel in the FC trace list
     rbkd = {}
     for i in fcio_obj.tracelist:
         rbkd[i] = RawBuffer(lgdo=decoder.make_lgdo(size=1))
 
     # decode packet into the lgdo's and check if the buffer is full
     assert decoder.decode_packet(fcio=fcio_obj, evt_rbkd=rbkd, packet_id=69) is True
+
+    # # check compression settings (here before any LH5Store.write_object() call
+    # assert "compression" in rbkd[0].lgdo["packet_id"].attrs
+    # assert "compression" in rbkd[0].lgdo["waveform"].values.attrs
+
     return rbkd
 
 
-def test_decoding(event_rbkd):
+def test_decoding_and_compression_attrs(event_rbkd):
     assert event_rbkd != {}
 
 
 def test_data_types(event_rbkd):
-
     for _, v in event_rbkd.items():
-        # assert v.out_name == 'FCEvent' FIXME: is this a bug?
         tbl = v.lgdo
         assert isinstance(tbl, lgdo.Struct)
         assert isinstance(tbl["packet_id"], lgdo.Array)
         assert isinstance(tbl["eventnumber"], lgdo.Array)
         assert isinstance(tbl["timestamp"], lgdo.Array)
         assert isinstance(tbl["runtime"], lgdo.Array)
         assert isinstance(tbl["numtraces"], lgdo.Array)
         assert isinstance(tbl["tracelist"], lgdo.VectorOfVectors)
         assert isinstance(tbl["baseline"], lgdo.Array)
         assert isinstance(tbl["daqenergy"], lgdo.Array)
         assert isinstance(tbl["channel"], lgdo.Array)
         assert isinstance(tbl["ts_pps"], lgdo.Array)
         assert isinstance(tbl["ts_ticks"], lgdo.Array)
         assert isinstance(tbl["ts_maxticks"], lgdo.Array)
-        assert isinstance(tbl["to_mu_sec"], lgdo.Array)
-        assert isinstance(tbl["to_mu_usec"], lgdo.Array)
+        assert isinstance(tbl["mu_offset_sec"], lgdo.Array)
+        assert isinstance(tbl["mu_offset_usec"], lgdo.Array)
         assert isinstance(tbl["to_master_sec"], lgdo.Array)
-        assert isinstance(tbl["to_dt_mu_usec"], lgdo.Array)
-        assert isinstance(tbl["to_abs_mu_usec"], lgdo.Array)
+        assert isinstance(tbl["delta_mu_usec"], lgdo.Array)
+        assert isinstance(tbl["abs_delta_mu_usec"], lgdo.Array)
         assert isinstance(tbl["to_start_sec"], lgdo.Array)
         assert isinstance(tbl["to_start_usec"], lgdo.Array)
         assert isinstance(tbl["dr_start_pps"], lgdo.Array)
         assert isinstance(tbl["dr_start_ticks"], lgdo.Array)
         assert isinstance(tbl["dr_stop_pps"], lgdo.Array)
         assert isinstance(tbl["dr_stop_ticks"], lgdo.Array)
         assert isinstance(tbl["dr_maxticks"], lgdo.Array)
@@ -62,15 +65,14 @@
         assert isinstance(tbl["waveform"], lgdo.Struct)
         assert isinstance(tbl["waveform"]["t0"], lgdo.Array)
         assert isinstance(tbl["waveform"]["dt"], lgdo.Array)
         assert isinstance(tbl["waveform"]["values"], lgdo.ArrayOfEqualSizedArrays)
 
 
 def test_values(event_rbkd, fcio_obj):
-
     fc = fcio_obj
     for ch in fc.tracelist:
         loc = event_rbkd[ch].loc - 1
         tbl = event_rbkd[ch].lgdo
 
         assert event_rbkd[ch].fill_safety == fc.numtraces
 
@@ -89,19 +91,19 @@
 
         assert np.array_equal(tbl["baseline"].nda[loc], fc.baseline[ch])
         assert np.array_equal(tbl["daqenergy"].nda[loc], fc.daqenergy[ch])
         assert tbl["channel"].nda[loc] == ch
         assert tbl["ts_pps"].nda[loc] == fc.timestamp_pps
         assert tbl["ts_ticks"].nda[loc] == fc.timestamp_ticks
         assert tbl["ts_maxticks"].nda[loc] == fc.timestamp_maxticks
-        assert tbl["to_mu_sec"].nda[loc] == fc.timeoffset_mu_sec
-        assert tbl["to_mu_usec"].nda[loc] == fc.timeoffset_mu_usec
+        assert tbl["mu_offset_sec"].nda[loc] == fc.timeoffset_mu_sec
+        assert tbl["mu_offset_usec"].nda[loc] == fc.timeoffset_mu_usec
         assert tbl["to_master_sec"].nda[loc] == fc.timeoffset_master_sec
-        assert tbl["to_dt_mu_usec"].nda[loc] == fc.timeoffset_dt_mu_usec
-        assert tbl["to_abs_mu_usec"].nda[loc] == fc.timeoffset_abs_mu_usec
+        assert tbl["delta_mu_usec"].nda[loc] == fc.timeoffset_dt_mu_usec
+        assert tbl["abs_delta_mu_usec"].nda[loc] == fc.timeoffset_abs_mu_usec
         assert tbl["to_start_sec"].nda[loc] == fc.timeoffset_start_sec
         assert tbl["to_start_usec"].nda[loc] == fc.timeoffset_start_usec
         assert tbl["dr_start_pps"].nda[loc] == fc.deadregion_start_pps
         assert tbl["dr_start_ticks"].nda[loc] == fc.deadregion_start_ticks
         assert tbl["dr_stop_pps"].nda[loc] == fc.deadregion_stop_pps
         assert tbl["dr_stop_ticks"].nda[loc] == fc.deadregion_stop_ticks
         assert tbl["dr_maxticks"].nda[loc] == fc.deadregion_maxticks
```

### Comparing `pygama-1.2.0/tests/raw/fc/test_fc_status_decoder.py` & `pygama-1.3.0/tests/raw/fc/test_fc_status_decoder.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/raw/fc/test_fc_streamer.py` & `pygama-1.3.0/tests/raw/fc/test_fc_streamer.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/raw/orca/test_or_run_decoder_for_run.py` & `pygama-1.3.0/tests/raw/orca/test_or_run_decoder_for_run.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 from pygama import lgdo
 from pygama.raw.orca.orca_run_decoder import ORRunDecoderForRun
 from pygama.raw.raw_buffer import RawBuffer
 
 
 @pytest.fixture(scope="module")
 def run_rbkd(orca_stream):
-
     decoder = ORRunDecoderForRun(header=orca_stream.header)
 
     rbkd = {}
     rbkd[0] = RawBuffer(lgdo=decoder.make_lgdo(size=1))
 
     this_packet = orca_stream.load_packet(skip_unknown_ids=False)
     orca_stream.close_stream()  # avoid leaving file open
 
     # assert correct type for ORRunDecoderForRun
-    assert (this_packet[0] >> 18) == 7
+    assert (this_packet[0] >> 18) == orca_stream.header["dataDescription"][
+        "ORRunModel"
+    ]["Run"]["dataId"] >> 18
 
     # assert that it worked and the buffer is full
     assert decoder.decode_packet(packet=this_packet, packet_id=1, rbl=rbkd)
 
     return rbkd, this_packet
 
 
 def test_decoding(run_rbkd):
     assert run_rbkd[0] != {}
 
 
 def test_data_types(run_rbkd):
-
     for _, v in run_rbkd[0].items():
         tbl = v.lgdo
         assert isinstance(tbl, lgdo.Struct)
         assert isinstance(tbl["subrun_number"], lgdo.Array)
         assert isinstance(tbl["runstartorstop"], lgdo.Array)
         assert isinstance(tbl["quickstartrun"], lgdo.Array)
         assert isinstance(tbl["remotecontrolrun"], lgdo.Array)
@@ -42,15 +42,14 @@
         assert isinstance(tbl["endsubrunrecord"], lgdo.Array)
         assert isinstance(tbl["startsubrunrecord"], lgdo.Array)
         assert isinstance(tbl["run_number"], lgdo.Array)
         assert isinstance(tbl["time"], lgdo.Array)
 
 
 def test_values(run_rbkd):
-
     this_packet = run_rbkd[1]
 
     decoded_values = ORRunDecoderForRun().decoded_values
 
     for _, v in run_rbkd[0].items():
         loc = v.loc - 1
         tbl = v.lgdo
```

### Comparing `pygama-1.2.0/tests/raw/test_cli.py` & `pygama-1.3.0/tests/raw/test_cli.py`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/raw/test_raw_buffer.py` & `pygama-1.3.0/tests/raw/test_raw_buffer.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         kw_dict={"file_key": "run0"},
     )
     assert rbl.get_list_of("out_name") == ["testspms"]
     assert rbl.get_list_of("key_list") == [[3, 4, 5, 6]]
 
 
 def test_raw_buffer_lib_json_load():
-
     rb_json = """
     {
       "FCEventDecoder" : {
         "g{key:0>3d}" : {
           "key_list" : [[24, 64]],
           "out_stream" : "$DATADIR/{file_key}_geds.lh5:/geds"
         },
```

### Comparing `pygama-1.2.0/tests/vis/configs/hpge-dsp-config.json` & `pygama-1.3.0/tests/vis/configs/hpge-dsp-config.json`

 * *Files identical despite different names*

### Comparing `pygama-1.2.0/tests/vis/test_waveform_browser.py` & `pygama-1.3.0/tests/vis/test_waveform_browser.py`

 * *Files identical despite different names*

